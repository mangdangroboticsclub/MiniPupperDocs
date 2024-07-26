=================
ROS2 Installation
=================

.. contents::
  :depth: 2

* Mini Pupper's ROS2 installation package is based on `ros2_setup_scripts <https://github.com/Tiryoh/ros2_setup_scripts_ubuntu>`_  which is written by one of our contributor @Tiryoh.
* Mini Pupper's ROS2 version is based on `Champ <https://github.com/chvmp/champ>`_  open source project, and we made some changes to SLAM and Navigation functions.
* Mini Pupper's software supporting lidar sensor is based on `ldlidar_stl_ros2 <https://github.com/ldrobotSensorTeam/ldlidar_stl_ros2>`_  open source project.

We recommend you explore Mini Pupper with ROS2 network, make sure your PC and Mini Pupper have connected to the same WiFi.

Through the following steps, you will be able to setup the ros2 for your remote PC and the Mini Pupper.

1. PC Setup
------------

PC Setup corresponds to PC (your desktop or laptop PC) for controlling Mini Pupper remotely. Do not apply these commands to your Mini Pupper.

**WARNING: The contents in this chapter corresponds to the Remote PC (your desktop or laptop PC) which will control Mini Pupper. Do not apply these commands to your Raspberry Pi on Mini Pupper or Compute Module 4 on Mini Pupper 2.**

**NOTE: This instruction was tested on Linux with Ubuntu 22.04 and ROS2 Humble.**

1.1 Install ROS 2 Humble
^^^^^^

Open the terminal with Ctrl+Alt+T from Remote PC. 

::

	cd ~
	sudo apt update
	git clone https://github.com/Tiryoh/ros2_setup_scripts_ubuntu.git
	~/ros2_setup_scripts_ubuntu/ros2-humble-ros-base-main.sh
	source /opt/ros/humble/setup.bash

After ROS 2 installation, download the Mini Pupper ROS package in the workspace.

1.2 Install Mini Pupper ROS Repository
^^^^^^

Open the terminal with Ctrl+Alt+T from Remote PC.

::

	mkdir -p ~/ros2_ws/src
	cd ~/ros2_ws/src
	git clone https://github.com/mangdangroboticsclub/mini_pupper_ros.git -b ros2-dev mini_pupper_ros
	vcs import < mini_pupper_ros/.minipupper.repos --recursive


1.3 Install Dependent ROS 2 Packages and Build Package
^^^^^^

Open the terminal with Ctrl+Alt+T from Remote PC.

::

	cd ~/ros2_ws
	rosdep install --from-paths src --ignore-src -r -y
	sudo apt install ros-humble-teleop-twist-keyboard
	sudo apt install ros-humble-teleop-twist-joy
	colcon build --symlink-install


1.4. Export Robot Model
^^^^^^

1. Open ~/.bashrc with text editor in the terminal.

::

	nano ~/.bashrc

2. Scroll to the end of the file.

.. image:: ../_static/bashrc.png
    :align: center  

| 

3. Add the following line to export the robot model with the computer. Please use the proper keyword among mini_pupper, mini_pupper_2 for the ROBOT_MODEL parameter according to your robot model.

::

 	export ROBOT_MODEL=mini_pupper_2

4. Save the file with Ctrl+S and exit with Ctrl+X.
5. Run the following command to apply the change.

::

	source ~/.bashrc


2. Mini Pupper Setup
------------

2.1 Image flashing
^^^^^^

The steps below are for you to setup ROS2 environment of Mini Pupper by yourself.
You can also download the `pre-built ROS image <https://drive.google.com/drive/folders/12FDFbZzO61Euh8pJI9oCxN-eLVm5zjyi>`_ for Mini Pupper side, named "YYYYMMDD_MD-Puppy2_ROS2Humble_Ubuntu22.04.img" or "YYYYMMDD_MD-Puppy1_ROS2Humble_Ubuntu22.04.img". Please select the appropriate image according to the date and the robot model.

1. The image can be flashed into the card using an adaptor. If your PC do not have a microSD slot, please use a microSD card reader to burn the image.
2. Download ubuntu-22.04.2-preinstalled-server-arm64+raspi.img.xz from the official website, and flash it into your SD card according to the following guide.
3. Download balenaEtcher from https://etcher.balena.io/.
4. Press the blue button to choose the destination where you download the image and select the image.

.. image:: ../_static/choose-image.png
    :align: center   

|

5. Press the blue button to choose the destination where you are flashing the image into (the address of the SD card).

.. image:: ../_static/target1.png
    :align: center   

|

.. image:: ../_static/target2.png
    :align: center   

|

6. Press the flash button and you will see the image below. Wait until the process to complete.

.. image:: ../_static/flashing.png
    :align: center   

|

.. image:: ../_static/validating.png
    :align: center   

|

2.2 Wifi-Setting
^^^^^^

1. Plug the card into the Mini Pupper card port and setup your own wifi.

.. image:: ../_static/Sd-card-reader.jpg
    :align: center   

|

2. Run the following command to edit the network setting of the pupper.

::

	sudo nano /etc/netplan/50-cloud-init.yaml

When the editor is opened, edit the content as below while replacing Mangdang and mangdang with your actual wifi SSID and password.

.. image:: ../_static/netplan-yaml.png
    :align: center   

|

3.	Save the file with Ctrl+S and exit with Ctrl+X.
4.	Run the following commands to reboot and connect to your actual wifi.

::

	sudo netplan apply
	sudo apt update
	sudo apt upgrade
	reboot

2.3 Robot model setting
^^^^^^

1. After reboot, open ~/.bashrc with text editor in the terminal.

::

	nano ~/.bashrc

2. Scroll to the end of the file.

.. image:: ../_static/bashrc.png
    :align: center 

|  

3. Add the following line to export the robot model with the computer. Please use the proper keyword among mini_pupper, mini_pupper_2 for the ROBOT_MODEL parameter according to your robot model.

::

	export ROBOT_MODEL=mini_pupper_2

4. Save the file with Ctrl+S and exit with Ctrl+X.
5. Run the following command to apply the change.

::

	source ~/.bashrc

3. Connecting Mini Pupper to PC
------------

1. Open two terminals with Ctrl+Alt+T twice, one for connecting to Mini Pupper and one for PC local.
2. Look at monitor of Mini Pupper to obtain the IP address of it.

.. image:: ../_static/IPaddress.jpg
    :align: center   

|

3. Use one of the terminals and run the following command to connect to the Mini Pupper. The default password is “mangdang”.

::

	ssh ubuntu@{IP_ADDRESS_OF_MINI_PUPPER}

4. Open ~/.bashrc with text editor in both terminals.

::

	nano ~/.bashrc

5. Scroll to the end of the file for both terminals.

.. image:: ../_static/bashrc.png
    :align: center  

| 

6. Add the following line in both terminals to setup the connection. The number inputted can be any number, but it should be the same for both terminals.

::

	 export ROS_DOMAIN_ID=42

7. Save the file with Ctrl+S and exit with Ctrl+X.
8. Run the following command to apply the change.

::

	source ~/.bashrc

9. Use the following command in both terminals to confirm that the PC and the Mini Pupper are connected:

::

	ros2 node list

10. Compare the output in both terminals:

.. image:: ../_static/node-list.png
    :align: center   

|

If the output in both terminals shows the same list of node which is similar to the picture, your PC and the Mini Pupper is connected

**NOTE: the node list depends on the nodes in progress, which may not be exactly the same from the image.**
