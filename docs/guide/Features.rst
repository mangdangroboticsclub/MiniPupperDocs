Features
==============================

.. contents::
  :depth: 2

.. image:: ../_static/Feature001.jpg
    :align: center 
	
Hardware Specifications
^^^^^^^^^^^^^^^^^^^^^^^^

* Dimensions: 210x110x165mm
* Weight: 509g
* Battery: 1000mAh / micro-usb charge
* Processor: Raspberry Pi 4B
* Screen: 240x320 ISP LCD
* Input charger: 5V 1A
* OS: Ubuntu/ROS

Dimension
^^^^^^^^^^
.. image:: ../_static/Dimension.png
    :align: center 

Open Source Hardware
^^^^^^^^^^^^^^^^^^^^^

* Lidar module

If you want to explore ROS SLAM, Navigation functions based on Lidar, you also need a Lidar module. We can ONLY ensure the Lidar module can work well based on our source code, and NOT ensure that you get from other channels. We already tested some Lidar modules, such as, PRLidar A1, YDLidar X2L, and LD06. For Mini Pupper, we refer to LD06 as it is smaller. 

* OpenCV Camera module

For potential security issues, the camera module is not included in our default package. If you want to explore camera AI functions, you can choose a normal USB camera module, of course, a 3D camera module is better for study. If try the 3D camera module, we recommend you OpenCV's latest 3D camera module, named OAK-D LITE, comes from OpenCV&Luxonis. We have good relationship with Luxonis, their RobotHub will release more interesting demos soon. 