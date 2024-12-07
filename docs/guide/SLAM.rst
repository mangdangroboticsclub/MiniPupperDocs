=================
SLAM
=================

.. contents::
  :depth: 2

The SLAM (Simultaneous Localization and Mapping) is a technique to draw a map by estimating current location in an arbitrary space. Following the steps below, we can use Mini Pupper to draw a map of the surrounding area.

**NOTE: Please run the SLAM node on Remote PC.**
**Make sure to launch the Bringup from Mini Pupper before executing any operation.**

1. Run SLAM Node
------------------

1. If Bringup is not launched on Mini Pupper, launch Bringup first.

•	Open a terminal with Ctrl+Alt+T  to connect Mini Pupper.
•	Look at monitor of Mini Pupper to obtain the IP address of it.

•	Use one of the terminals and run the following command to connect to the Mini Pupper. The default password is mangdang.

::

	ssh ubuntu@{IP_ADDRESS_OF_MINI_PUPPER}

•	Bring up basic packages to start Mini Pupper applications.

::

	. ~/ros2_ws/install/setup.bash
	ros2 launch mini_pupper_bringup bringup.launch.py

2. Open a new terminal from Remote PC with Ctrl + Alt + T and launch the SLAM node.

::

	. ~/ros2_ws/install/setup.bash
	ros2 launch mini_pupper_slam slam.launch.py

2. Teleoperation
--------------------

Following the steps below, we can use teleoperation to explore unknown area of the map.

**NOTE: Once SLAM node is successfully up and running. Vigorous change of the linear and angular speed might lower the smoothness of map generated.**
**WARNING: Make sure to run the Bringup from the Mini Pupper before teleoperation. Be careful when testing the robot on the table as the robot might fall during teleoperation.**

2.1 Keyboard
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Open a terminal with Ctrl+Alt+T on remote PC.
2. Run teleoperation node using the following command.

::

	. ~/ros2_ws/install/setup.bash
	ros2 run teleop_twist_keyboard teleop_twist_keyboard

2.2 Joystick
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Open a terminal with Ctrl+Alt+T on remote PC.
2. Run teleoperation node using the following command.

::

	. ~/ros2_ws/install/setup.bash
	ros2 launch teleop_twist_joy teleop-launch.py joy_dev:=/dev/input/{NAME_OF_JOYSTICK}

After teleoperation, a map with unknown area revealed will be shown as followed:

.. image:: ../_static/Map_generation.jpg
    :align: center

|

3. Save the map
------------------------

Following the steps below, the files of the map will be saved.

1. Open a terminal with Ctrl+Alt+T on remote PC.
2. Use the following command to launch the map_saver_cli node in the nav2_map_server package to create map files.

The map file is saved in the directory where the map_saver_cli node is launched at.

::

	. ~/ros2_ws/install/setup.bash
	ros2 run nav2_map_server map_saver_cli -f ~/map

After running the above command, two files will be generated, namely map.pgm and map.yaml.

The following pictures shows the .pgm file to be saved.

.. image:: ../_static/map2.png
    :align: center

|
