==============================
Examples
==============================

.. contents::
  :depth: 2


.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/PfGvPq9QuLQ?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


1. Custom shell parts
-------------
Pupper is open source project, that means, you can custom what you want.
You can find all the `3D printed shell files <https://drive.google.com/drive/folders/12FDFbZzO61Euh8pJI9oCxN-eLVm5zjyi?usp=sharing>`_  and custom them.

2. Custom Facial Animation
-------------

2.1 Prerequisites
^^^^^^^^^^^^^^

* HDMI Display
* micro HDMI cable
* Keyboard and mouse
* a new picture

.. image:: ../_static/165.jpg
  :align: center

2.2 Run
^^^^^

* Connect MiniPupper to the display by mirco HDMI cable

.. image:: ../_static/168.jpg
  :align: center

* A: wireless adapter for the keyboard and mouse
* B: mirco HDMI cable

* Ubuntu login

.. image:: ../_static/172.jpg
  :align: center

The default password is mangdang

3. Keyboard controller
-------------

3.1 Keyboard controller based on nonROS version
^^^^^^
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
^^^^^^

Please refer to the SLAM section.

4. Web controller
-------------

Will update soon!

5. Mobile controller
-------------

Will update soon!

6. Docker
-------------

6.1 Docker for Pupper
^^^^^^
Dockerfile for Mini Pupper ROS package, comes from `docker-mini-pupper-ros project <https://github.com/Tiryoh/docker-mini-pupper-ros.git>`_.

6.2 Docker for Host
^^^^^^
Host computer setup for interfacing with a Mini Pupper over a network, comes from `mp_host_setup project <https://github.com/zmk5/mp_host_setup.git>`_.

7. Scratch program
-------------

Will update soon!