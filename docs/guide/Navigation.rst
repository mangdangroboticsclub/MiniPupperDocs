==============================
Navigation
==============================

.. contents::
  :depth: 2

Summary
-----------------

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/jb2yxs2YUsI?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Mini Pupper's ROS version is based on `Champ <https://github.com/chvmp/champ>`_  open source project, and we made some changes to Navigation functions.

**NOTE: Please run the Navigation node on Remote PC.**
**WARNING: Make sure to run the Bringup from the Mini Pupper before navigation. Put the robot on the ground the prevent the robot from falling during movement.**

1.1 Run Navigation Node
^^^^^^

1.If Bringup is not launched on Mini Pupper, launch Bringup first.

•	Open a terminal with Ctrl+Alt+T  to connect Mini Pupper.
•	Look at monitor of Mini Pupper to obtain the IP address of it.

.. image:: ../_static/IPaddress.jpg
    :align: center  

•	Use one of the terminals and run the following command to connect to the Mini Pupper. The default password is mangdang.

::

	ssh ubuntu@{IP_ADDRESS_OF_MINI_PUPPER)

•	Bring up basic packages to start Mini Pupper applications. 

::
	
	. ~/ros2_ws/install/setup.bash
	ros2 launch mini_pupper_bringup bringup.launch.py

2. Open a new terminal from Remote PC with Ctrl + Alt + T and launch the Navigation node. 

::
    . ~/ros2_ws/install/setup.bash
    ros2 launch mini_pupper_navigation navigation.launch.py map:=$HOME/map.yaml

The map used in navigation is two-dimensional Occupancy Grid Map (OGM). The white area is collision free area while black area is occupied and inaccessible area, and gray area represents the unknown area.

1.2 Estimate Initial Pose
^^^^^^

1. Click the 2D Pose Estimate button in the RViz2 menu.
2. Click on the map on the place where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.
3. Repeat step 1 and 2 until the inaccessible area detected by the robot is overlapping completely with the black area on the map.

1.3 Set Navigation Goal
^^^^^^

1. Click the Nav2 Goal button in the RViz2 menu. Nav2 will plan the path and guide the robot towards reaching the goal.
2. Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing, while the root of the green arrow is the destination at which the robot will finally reach.
