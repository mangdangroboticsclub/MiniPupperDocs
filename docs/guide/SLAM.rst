=================
SLAM
=================

.. contents::
  :depth: 2

SLAM(Simultaneous Localization and Mapping)
-----------------

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/4gblGfd12IY?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Mini Pupper's ROS version is based on `Champ <https://github.com/chvmp/champ>`_  open source project, and we made some changes to SLAM and Navigation functions.


1.Installation
------------

We recommend you explore Mini Pupper with ROS network, make sure your PC and Mini Pupper have connected to the same WiFi.

1.1 PC Setup
^^^^^^
PC Setup corresponds to PC (your desktop or laptop PC) for controlling Mini Pupper remotely. Do not apply these commands to your Mini Pupper.

* 1.1.1 Cartographer ROS packages installation

Our SLAM and Navigation functions are based on `cartographer_ros <https://google-cartographer-ros.readthedocs.io/en/latest/compilation.html>`_ . 

::

	cd ~
	sudo apt-get update
	sudo apt-get install -y python3-wstool python3-rosdep ninja-build stow
	mkdir carto_ws
	cd carto_ws
	wstool init src
	wstool merge -t src https://raw.githubusercontent.com/cartographer-project/cartographer_ros/master/cartographer_ros.rosinstall
	wstool update -t src
	sudo rosdep init
	rosdep update
	rosdep install --from-paths src --ignore-src --rosdistro=${ROS_DISTRO} -y
	src/cartographer/scripts/install_abseil.sh
	sudo apt-get remove ros-${ROS_DISTRO}-abseil-cpp
	catkin_make_isolated --install --use-ninja
	source install_isolated/setup.bash

* 1.1.2 Mini Pupper ROS packages installation

::

	cd <your_ws>/src
	git clone --recursive https://github.com/mangdangroboticsclub/minipupper_ros
	cd ..
	rosdep install --from-paths src --ignore-src -r -y
	catkin_make
	source <your_ws>/devel/setup.bash


* 1.1.3 Network Setup

Connect your PC and Mini Pupper to the same WiFi and find the assigned IP address with the command below.

::

	ifconfig

Open the file and update ROS IP settings with commands below.

::

	sudo gedit ~/.bashrc

Then add your Master and hostname config, for an example

::

	export ROS_MASTER_URI=http://192.168.1.106:11311
	export ROS_HOSTNAME=192.168.1.106



1.2 Mini Pupper Setup
^^^^^^

You can also download the `pre-built ROS image <https://drive.google.com/drive/folders/12FDFbZzO61Euh8pJI9oCxN-eLVm5zjyi>`_ for Mini Pupper side, named "xxx.MiniPupper_ROS&OpenCV_Ubuntu20.04.03.img".

* 1.2.1 Hardware Dependencies

You should first install dependencies of servos, battery moniter and display screen. 
Please refer to `minipupper_ros_bsp <https://github.com/mangdangroboticsclub/minipupper_ros_bsp>`_ .

* 1.2.2 Controller Joystick interface installation

The Joystick interface in ROS is based on `ps4-ros <https://github.com/solbach/ps4-ros>`_  project. 

::

	pip install ds4drv
	sudo apt install ros-noetic-joy
	sudo wget https://raw.githubusercontent.com/chrippa/ds4drv/master/udev/50-ds4drv.rules -O /etc/udev/rules.d/50-ds4drv.rules
	sudo udevadm control --reload-rules
	sudo udevadm trigger
	sudo reboot

Then go into pairing mode with the controller: Home button + share button for ~3 sec.
Run $ds4drv from command line until the controller is connected.

::

	ds4drv

This will output something like "Created devices /dev/input/jsX".
Then give the permissions to the device

::

	sudo chmod a+rw /dev/input/jsX


* 1.2.3 Mini Pupper ROS packages installation

**Then you can install the ROS packages for Mini Pupper. This should be installed both on Mini Pupper and your PC.**

::

	cd <your_ws>/src
	git clone --recursive https://github.com/mangdangroboticsclub/minipupper_ros
	cd minipupper_ros/champ
	# it's not recommend to compile gazebo on raspberry pi
	sudo rm -rf champ_gazebo
	cd ../../..
	rosdep install --from-paths src --ignore-src -r -y
	catkin_make
	source <your_ws>/devel/setup.bash


* 1.2.4 Network Setup

Connect your PC and Mini Pupper to the same WiFi and find the assigned IP address with commands below.

::

	ifconfig

Open the file and update the ROS IP settings with the command below.

::

	sudo gedit ~/.bashrc

Then add your Master and hostname config,for an example

::

	export ROS_MASTER_URI=http://192.168.1.106:11311
	export ROS_HOSTNAME=192.168.1.107


2.Quick Start
------------

2.1 Calibration
^^^^^^

Through this script, you can calibrate the angle of every servo in one turn. Just input the angles.</br>
The hip and shank should be horizontal, and the ham should be vertical.

::

	roslaunch servo_interface calibrate.launch

Make sure Mini Pupper looks like this after calibrating.

.. image:: ../_static/109.jpg
    :align: center   

2.2 Walking
^^^^^^

* 2.2.1 Run the base driver

**You should run this command on Mini Pupper**

::

	roslaunch mini_pupper bringup.launch

If Mini Pupper didn't stand as what you expect, you can edit calibration.yaml in servo_interface/config/calibration to fix the angles.

* 2.2.2 Control Mini Pupper

There are two options to control Mini Pupper:

1.Use keyboard

**It's recommended to run this command on PC.**

::

	roslaunch champ_teleop teleop.launch


2.Use the controller

**It's recommended to run this command on Mini Pupper.**

**Don't run this command while using move_base because even if you are doing nothing with the joystick, it would still send cmd_vel with all the values as zero.**

::

	roslaunch ps4_interface ps4_interface.launch

For the controller usage, please refer to Quick Start Guide.

* 2.2.2 LCD Screen

::

	python3 ~/minipupper_ros_bsp/mangdang/LCD/demo.py

We also made a simple ROS interface of the LCD screen, which subscribes sensor_msgs/Image.

::

	rosrun display_interface display_interface.py


3. SLAM
------------

3.1 Run the base driver
^^^^^^

**You should run this command on Mini Pupper**

::

	roslaunch mini_pupper bringup.launch


3.2 Run Cartographer
^^^^^^

**You should run this command on PC**
**If you are using gazebo, set the param /use_sim_time to true in the launch file.**

::

	roslaunch mini_pupper slam.launch

Then you can use keyboard or joystick to control your Mini Pupper walking around and creating a map. To save the map, run these commands below.

::

	rosservice call /finish_trajectory 0
	rosservice call /write_state "{filename: '${HOME}/map.pbstream'}"
	rosrun cartographer_ros cartographer_pbstream_to_ros_map -map_filestem=${HOME}/map -pbstream_filename=${HOME}/map.pbstream -resolution=0.05

Remember to edit map.yaml</br>
The first line should be

::

	image: map.pgm

Then, copy map.pbstream, map.pgm and map.yaml files you just saved to 
<your_ws>/src/minipupper_ros/mini_pupper/maps