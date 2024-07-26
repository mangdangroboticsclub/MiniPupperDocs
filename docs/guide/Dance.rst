=================
Dance
=================

.. contents::
  :depth: 2

The video demonstrates the dancing function of Mini Pupper.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/RkcZOZatPDo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

|

**NOTE: The nodes for playing music and dance cand be executed on both Mini Pupper and Remote PC.**

1. Install Music Packages
------------

1. Open a terminal with Ctrl+Alt+T to connect Mini Pupper.
2. Look at monitor of Mini Pupper to obtain the IP address of it.

3. Use one of the terminals and run the following command to connect to the Mini Pupper. The default password is mangdang.

::

    ssh ubuntu@{IP_ADDRESS_OF_MINI_PUPPER}

.. image:: ../_static/IPaddress.jpg
    :align: center  

|

4. Use the following command to install required packages for the pupper to play music.

::

    sudo apt-get install ffmpeg portaudio19-dev -y
    pip install pydub pyaudio

2. Launch Bringup
------------

1.If Bringup is not launched on Mini Pupper, launch Bringup first.

•	Open a terminal with Ctrl+Alt+T  to connect Mini Pupper.
•	Look at monitor of Mini Pupper to obtain the IP address of it.


•	Use one of the terminals and run the following command to connect to the Mini Pupper. The default password is mangdang.

::

    ssh ubuntu@{IP_ADDRESS_OF_MINI_PUPPER}

•	Bring up basic packages to start Mini Pupper applications. 

::
    
    . ~/ros2_ws/install/setup.bash
    ros2 launch mini_pupper_bringup bringup.launch.py

3. Launch Music Node
------------

Open a new terminal with Ctrl + Alt + T and launch the Music node.

::

    . ~/ros2_ws/install/setup.bash 
    ros2 launch mini_pupper_music music.launch.py

4. Launch Dance Node
------------

Open a new terminal with Ctrl + Alt + T and launch the Dance node.

::

    source ~/ros2_ws/install/setup.bash
    ros2 launch mini_pupper_dance dance.launch.py
