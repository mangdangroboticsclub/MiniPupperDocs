==============================
Machine Learning
==============================

.. contents::
  :depth: 2

Summary
-------

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/3Zi9soi4vEU?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


For potential security issues, the camera module is not included in our default package. If you want to explore camera AI functions, you can choose a normal USB camera module, of course, a 3D camera module is better for study. If try the 3D camera module, we recommend you OpenCV's latest 3D camera module, named OAK-D LITE, comes from OpenCV&Luxonis.

1. Single camera module
-------------------------
1.1 Collision Avoidance
^^^^^^^^^^^^^^^^^^^^^^^^^
Will update late.

1.2 Teleoperation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Will update late.

1.3 Road Following
^^^^^^^^^^^^^^^^^^^
Will update late.

1.4 Object Following
^^^^^^^^^^^^^^^^^^^^^^^
Will update late.

1.5 Face Detect
^^^^^^^^^^^^^^^^^
Will update late.

2. 3D(OAK-D-Lite) camera module
---------------------------------

2.1 Object Following
^^^^^^^^^^^^^^^^^^^^^^
You can download the `pre-built ROS image <https://drive.google.com/drive/folders/12FDFbZzO61Euh8pJI9oCxN-eLVm5zjyi>`_ , named "xxx.MiniPupper_ROS&OpenCV_Ubuntu20.04.03.img" to test the object following feature using OAK-D-LITE 3D camera module.

::

	# Terminal 1
	roslaunch mini_pupper bringup.launch

	# Terminal 2
	roslaunch depthai_examples mobile_publisher.launch

	# Terminal 3
	rosrun mini_pupper_detect oak_detect.py

2.2 Live streaming
^^^^^^^^^^^^^^^^^^^^
Will update late.
