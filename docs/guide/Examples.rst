==============================
Examples
==============================

.. contents::
   :local:
   :depth: 2


1. Custom shell parts
----------------------
Mini Pupper is an open source project, that means, you can custom what you want.
You can find all the `3D printed shell files <https://drive.google.com/drive/folders/12FDFbZzO61Euh8pJI9oCxN-eLVm5zjyi?usp=sharing>`_  and custom them.

How about connect it to LEGO parts? Or DIY it like @nisshan_

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="685" height="385" src="https://www.youtube.com/embed/PfGvPq9QuLQ?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


2. Custom Facial Animation
--------------------------

2.1 Prerequisites
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* HDMI Display
* micro HDMI cable
* Keyboard and mouse
* a new custom picture(size: 320x240 pix)

.. image:: ../_static/165.jpg
  :align: center

2.2 Run
^^^^^^^^

* Connect MiniPupper to a display, a keyboard and a mouse.

* Ubuntu login(The default password is mangdang)

.. image:: ../_static/172.jpg
  :align: center

* Replace the logo.png file using your custom picture

* Reboot Mini Pupper and then you will see your custom picture

.. image:: ../_static/172.2.jpg
  :align: center


3. Keyboard controller
-----------------------

3.1 Keyboard controller based on nonROS version
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The feature is based on `PupperKeyboardController project <https://github.com/stanfordroboticsclub/PupperKeyboardController>`_, it's Pygame-based keyboard controller for Stanford Pupper.

* Install PyGame

::

	pip install pygame


* Controls

::

	wasd: left joystick
	arrow keys: right joystick
	q: L1
	e: R1
	ijkl: d-pad
	x: X
	square: u
	triangle: t
	circle: c

3.2 Keyboard controller based on ROS version
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Please refer to the SLAM section.

4. Web controller
------------------

Please refer to `Mini Pupper Web controller project <https://github.com/mangdangroboticsclub/mini_pupper_web_controller>`_.

5. How to control a Mini Pupper PWM servo
--------------------------------------------

Mini Pupper servo is a PWM servo, You can connect one servo to Pi board as the following picture shows,
run the samle code,and then the servo will move.
You can find the code `here <https://drive.google.com/drive/folders/1QUYSe1RQOWlZGtCwDqMqtEGB5tKNtcVj?usp=sharing>`_.
You can run it on your Windows or Ubuntu with Python environment, just like the following picture shows.


6. Forward Kinematics
-----------------------

Lecture
^^^^^^^^^

Please study the basic knowledge of forward kinematics online first.

You can also refer to the following video clips come from `Stanford Robotics Independent Study <https://pupper-independent-study.readthedocs.io/en/latest/course-material/lab-3-spr22.html>`_.

Forward kinematics lecture

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="685" height="385" src="https://www.youtube.com/embed/nFqTsAEywpY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Follow-up lecture to clarify some things

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="685" height="385" src="https://www.youtube.com/embed/XAUXrRtINTQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


Sample code
^^^^^^^^^^^^^

We prepared a simple Forward kinematics sample code based on Mini Pupper, you can try it `here <https://drive.google.com/drive/folders/1QUYSe1RQOWlZGtCwDqMqtEGB5tKNtcVj?usp=sharing>`_.
You can run it on your Windows or Ubuntu with Python environment, just like the following picture shows.


.. image:: ../_static/ForwardKinematics_SimpleModeMove.png
  :align: center

|

7. Inverse Kinematics
-------------------------

Preparation
^^^^^^^^^^^^^^^^^^^^^^^^^^
0. Assemble the camera module

For convenient shipping, the camera module may be not assembled by default. After receiving it, please assemble it yourself.

* The connector typically has a hinged, flip-up latch that you need to open to insert the ribbon cable. This latch helps ensure the ribbon cable stays securely connected to the board during use.
* Take the ribbon cable that is compatible with your Camera Module and interface on the board.

.. image:: ../_static/kinematics_1.gif
   :align: center
   :width: 685px

1.1 Install ROS 2 Humble
^^^^^^^^^^^^^^^^^^^^^^^^^^

Open the terminal with Ctrl+Alt+T from Remote PC.

::

	cd ~
	sudo apt update
	git clone https://github.com/Tiryoh/ros2_setup_scripts_ubuntu.git
	~/ros2_setup_scripts_ubuntu/ros2-humble-ros-base-main.sh
	source /opt/ros/humble/setup.bash

After ROS 2 installation, download the Mini Pupper ROS package in the workspace.

1.2 Install Mini Pupper ROS Repository
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Open the terminal with Ctrl+Alt+T from Remote PC.

::

	mkdir -p ~/ros2_ws/src
	cd ~/ros2_ws/src
	git clone https://github.com/mangdangroboticsclub/mini_pupper_ros.git -b ros2-dev mini_pupper_ros
	vcs import < mini_pupper_ros/.minipupper.repos --recursive

.. image:: ../_static/kinematics_2.gif
   :align: center
   :width: 685px

Navigation
^^^^^^^^^^^^^^^^^

Navigation allows the robot to move from one location to the specified destination based on the infomation of a map given from the IMU and the lidar sensor created from SLAM.

The following video shows how we can use the navigation function to make the Mini Pupper move along the planned path.

.. image:: ../_static/kinematics_3.gif
   :align: center
   :width: 685px

2. Open a new terminal from Remote PC with Ctrl + Alt + T and launch the Navigation node.

::

    . ~/ros2_ws/install/setup.bash
    ros2 launch mini_pupper_navigation navigation.launch.py map:=$HOME/map.yaml

The map used in navigation is two-dimensional Occupancy Grid Map (OGM). The white area is collision free area while black area is occupied and inaccessible area, and gray area represents the unknown area.

.. image:: ../_static/kinematics_4.gif
   :align: center
   :width: 685px

Lecture
^^^^^^^^^^^^^

Please study the basic knowledge of inverse kinematics online first.

You can also refer to the following video clips come from `Stanford Robotics Independent Study <https://pupper-independent-study.readthedocs.io/en/latest/course-material/lab-4-spr22.html>`_.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="685" height="385" src="https://www.youtube.com/embed/FvQ6NbqDR1U" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

8. PID control
---------------

We prepared PID demo that utilize Minipupper2 IMU to create an auto-balance Mini Pupper, you can try it by

::

  cd StanfordQuadruped
  python IMU.Balancing.MP2.py

Try surfing with the pupper! See how it works in the following video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="685" height="385" src="https://youtube.com/embed/N8gnD9P8Ht0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>



The Demo architecture

.. image:: ../_static/IMU_PID_Chart.png
  :height: 300px
  :align: center



9. Docker
-------------

9.1 Docker for Pupper
^^^^^^^^^^^^^^^^^^^^^^
Dockerfile for Mini Pupper ROS package, comes from `docker-mini-pupper-ros project <https://github.com/Tiryoh/docker-mini-pupper-ros.git>`_.

9.2 Docker for Host
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Host computer setup for interfacing with a Mini Pupper over a network, comes from `mp_host_setup project <https://github.com/zmk5/mp_host_setup.git>`_.

10. Scratch program
--------------------

Will update soon!
