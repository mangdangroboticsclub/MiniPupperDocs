=================
ROS2 Quick Start Guide
=================

.. contents::
  :depth: 2

1. Joystick Setup
------------

Through the following steps, you will be able to connect and set up the ROS2 software for the joystick.

1. Press the HOME button on the controller.

.. image:: ../_static/Bluetooth-connection-button.jpg
    :align: center   

|

2. Search for available bluetooth devices on your PC and connect to it.

.. image:: ../_static/controller-connection.png
    :align: center   

|

.. image:: ../_static/controller-address.png
    :align: center   

|

The video below shows the change of flashlight colour during connection.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/GzUFk6fD8s0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

|

3. Use the following command to check the name of the joystick.

Terminal output: In this case the name of the joystick is “js0”.

.. image:: ../_static/dev-input.png
    :align: center   

|

4. Use the following command to check if the joystick us connected.

::
    
	sudo apt install joystick
	jstest /dev/input/{NAME_OF_JOYSTICK}

There will be output as followed if joystick is connected.

.. image:: ../_static/jstest.png
    :align: center   

|

2. Bringup
------------

Through the following steps, you will be able launch the software to bringup the Mini Pupper hardware.

1. Open a terminal with Ctrl+Alt+T  to connect Mini Pupper.
2. Look at monitor of Mini Pupper to obtain the IP address of it.
3. Use one of the terminals and run the following command to connect to the Mini Pupper. The default password is mangdang.

::

	ssh ubuntu@{IP_ADDRESS_OF_MINI_PUPPER}

4. Bring up basic packages to start Mini Pupper applications. The command of sourcing the built package, ". ~/ros2_ws/install/setup.bash" can be replaced by ". ~/ros2_ws/install/setup.zsh", depending on the file type you use.

::

	. ~/ros2_ws/install/setup.bash
	ros2 launch mini_pupper_bringup bringup.launch.py

When the robot model is Mini Pupper 2, the terminal output will look like below.

.. image:: ../_static/Bringup1.png
    :align: center   

|

.. image:: ../_static/Bringup2.png
    :align: center   

|

5. Topics and services can be listed with commands below.

* Topic list

::

	ros2 topic list

.. image:: ../_static/topic-list.png
    :align: center   

|

* Service list

::

	ros2 service list

.. image:: ../_static/service-list.png
    :align: center   

|

3. Teleoporation
------------

Through the following steps, you will be able to teleoperate Mini Pupper either using the keyboard or joystick.

**WARNING: Make sure to run the Bringup from the Mini Pupper before teleoperation. Teleoperate the robot, and be careful when testing the robot on the table as the robot might fall.**

3.1 Keyboard
^^^^^^

1. Open a terminal with Ctrl+Alt+T on remote PC.
2. Run teleoperation node using the following command.

::

	. ~/ros2_ws/install/setup.bash
	ros2 run teleop_twist_keyboard teleop_twist_keyboard

Terminal output: 

.. image:: ../_static/keyboard-teleop.png
    :align: center   

|

You can drive the pupper using the keyboard following the guide below.

.. image:: ../_static/Keyboard-guide.jpg
    :align: center

|

The video shows the effect of each keyboard button on the movement of the robot.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/M9aV55VnKUw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div> 

| 

3.2 Joystick
^^^^^^

**NOTE: The design of button of joystick node on ROS2 is different from that mentioned in other sections which is used for non-ROS programs.**

**WARNING: Make sure to run the Bringup from the Mini Pupper before teleoperation. Teleoperate the robot, and be careful when testing the robot on the table as the robot might fall.**

1. Open a terminal with Ctrl+Alt+T on remote PC.
2. Run teleoperation node using the following command.

::

	. ~/ros2_ws/install/setup.bash
	ros2 launch teleop_twist_joy teleop-launch.py joy_dev:=/dev/input/{NAME_OF_JOYSTICK}

Terminal output:

.. image:: ../_static/joystick-teleop-node.png
    :align: center  

|

You can drive the pupper using the joystick following the guide below.

.. image:: ../_static/Controller-guide.jpg
    :align: center  

|

The video shows the effect of each button of the joystick on the movement of the robot.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/T8kwO7fDiqE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

|
