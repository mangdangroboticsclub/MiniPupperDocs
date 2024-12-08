========
Assembly
========

.. contents::
  :depth: 2

Assemble Mini Pupper
######################

This is the video clip for the pre-assembled leg kit, please refer to the below sections for more detailed steps.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/R-KgMSxkVVw?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


Please also refer to Mini Pupper Fusion 360 CAD model: https://a360.co/3wFLSlT


.. raw:: html

    <iframe src="https://gmail1515401.autodesk360.com/g/shares/SH35dfcQT936092f0e43940e1e402362e6d4?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


0. Update change points after April 15 2022
---------------------------------------------

* Updated the body and hip parts from 3D printed to mold.
* Re-designed and unified the original four hip parts into one for mold, for the detailed info, please refer to the mechanical design section.
* If you get your Mini Pupper kit after April 15 2022, it will be easier to assemble.
* If you have 3D printer and still hope to use the previous 3D printed design, that's OK.


1. Write the pre-built image into microSD
-------------------------------------------

Tools
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly.

* USB keyboard
* USB mouse
* PC
* microSD card reader
* HDMI Display
* micro HDMI cable
* USB charger


Step 1.1 Charging the battery
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The battery is charged via USB, see picture for USB socket, and can also be charged while attached to the Mini Pupper body.

※ LED light: Green means there is enough power, and Red means you need to charge it.

※ We recommend 5V/1A adapter, if you use 5V/2A adapter, the battery IC will change it to 1A. It needs about 1 hour to charge 80% and the light will become green, and an additional 1 hour to 100%, anyway, you can use it when the light becomes green.

.. image:: ../_static/100.jpg
    :align: center

Step 1.2 Download the image
^^^^^^^^^^^^^^^^^^^^^^^^^^^

* You can download latest image file via the below folder.

	`Release.from.MangDang <https://drive.google.com/drive/folders/1c0ShF-R8yxiMnCgMnSOctBpkW707b1q6?usp=sharing>`_


* The below picture is the custom carry board.

.. image:: ../_static/147.jpg
    :align: center

※ “xxx_MiniPupper_Controller_Ubuntu_22.04.img” means the image is for Ubuntu 22.04 version.

※ "xxx.MiniPupper_ROS&OpenCV_Ubuntu20.04.03.img" is the image file for the Ubuntu + ROS + OpenCV version for SLAM & Navigation & AI.


Step 1.3 Write the image into microSD card
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Insert the microSD card into your PC's SD card reader and write the image. We recommend the image creation tool balenaEtcher or Win32DiskImager as it is easy and reliable. It takes a while to complete.



* Remove the SD card from the PC and insert it into the Raspberry pi.

.. image:: ../_static/145.jpg
    :align: center


2. Position of the screws
--------------------------

* The pictures show the position of the screws briefly.

.. image:: ../_static/136.jpg
    :align: center

.. image:: ../_static/137.jpg
    :align: center

.. image:: ../_static/138.jpg
    :align: center

.. image:: ../_static/139.jpg
    :align: center

(The up pictures are before April 15 2022 version, the below pictures are after April 15 2022 version)

.. image:: ../_static/139.png
    :align: center


.. image:: ../_static/140.jpg
    :align: center

.. image:: ../_static/144.jpg
    :align: center

(The up pictures are before April 15 2022 version, the below pictures are after April 15 2022 version)

.. image:: ../_static/144.png
    :align: center


.. image:: ../_static/141.jpg
    :align: center

.. image:: ../_static/142.jpg
    :align: center

3. Legs Assembly
----------------
Please refer to the below video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/Ut7UnS3CTZs?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


Tools
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly.

* Loctite

※ We don't recommand new users to use the Loctite at first, you can use it after you have much background.

※ Loctite prevents the nut from loosening, but it is not essential, as it can be tightened only when looseness is noticed.

Bolt to use
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
* M2x5mm	2x4=8	①+②, ⑤+⑥
* M2x8mm	3x4=12	②+③, ④+⑦, ③+④
* M2x12mm	1x4=4	⑤+⑦
* M2x14mm	1x4=4	③+⑤

Step 3.1 Single leg
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Assemble the four legs. The front and back of the right side are the same, and so are the front and back of the left side. Show you how to assemble the right side.

* Video Instructions, please refer to the link https://youtu.be/Ut7UnS3CTZs


* The parts are numbered as follows to explain.

.. image:: ../_static/1.jpg
    :align: center


Assemble ① and ②

* Use one M2x5mm screw.The screw is inserted from the bottom of ② upwards and tightened by inserting them into the screw holes in ①. Be careful about the sides of ②.

* The two ballbearings in ② should be inserted all the way in and the end should be slightly visible as shown in the picture below. Tap the ball bearing and press it in without gaps.

.. image:: ../_static/2.jpg
    :align: center

.. image:: ../_static/3.jpg
    :align: center

.. image:: ../_static/4.jpg
    :align: center

.. image:: ../_static/6.jpg
    :align: center


Assemble ② and ③

* Use an M2x8mm screw and an M2 locknut. Insert the screw from the bottom to the top of ③, pass through ② and tighten with the nut. It is important to pay attention to the orientation of ③. Look carefully at the position of the hole in the middle.

.. image:: ../_static/7.jpg
    :align: center

.. image:: ../_static/8.jpg
    :align: center

.. image:: ../_static/9.jpg
    :align: center


Adjustment of the length of ④

* The length of ④ must match the length of ⑤. When adjusting the length, it is easier to use two long screws to make sure that the lengths match. Once the lengths have been adjusted, take apart all.

.. image:: ../_static/10.jpg
    :align: center

.. image:: ../_static/11.jpg
    :align: center

* If it's hard to twist, you can use two screwdrivers to assist.

.. image:: ../_static/11_1.jpg
    :align: center


Assemble ⑤ and ⑥

* Use one M2x5mm screw. Insert the screws into ⑤ first, insert them into the holes of ⑥, and tighten them. The large hole in ⑥ should be facing the surface.

.. image:: ../_static/12.jpg
    :align: center

.. image:: ../_static/13.jpg
    :align: center

.. image:: ../_static/14.jpg
    :align: center

Assemble ⑤ and ⑦

* Use an M2x12mm screw, an M2 locknut and two sets of ball bearings. Each ball bearing is made up of three parts, the top and bottom parts with the grooved side facing inwards. Insert a screw into a set of ball bearing. Then insert the screw into the hole ⑦. Taking care to look at the warped side of ⑦ to make sure it is facing the right way. Now screw in the another set of ball bearing. Finally, insert screw into ⑤ and tighten it with the nut.

.. image:: ../_static/15.jpg
    :align: center

.. image:: ../_static/18.jpg
    :align: center

.. image:: ../_static/19.jpg
    :align: center

.. image:: ../_static/21.jpg
    :align: center

.. image:: ../_static/20.jpg
    :align: center



Assemble ④ and ⑦

* Use an M2x8mm screw and an M2 nut. Insert the screw into ⑦ and put ④ through, then tighten it with the nut. The direction of the front and back of ④ can be either.

Left and right leg

.. image:: ../_static/22.jpg
    :align: center

.. image:: ../_static/23.jpg
    :align: center

.. image:: ../_static/24.jpg
    :align: center

Assemble ③ and ④

* Use an M2x8mm screw and an M2 nut. Insert the screw into ③ and put ④ through, then tighten it with the nut.

Left and right leg

.. image:: ../_static/25.jpg
    :align: center

.. image:: ../_static/26.jpg
    :align: center

Assemble ③ and ⑤

* Use M2x14mm screws and two sets of ball bearings. Thread the screws through the bearings, ③, bearings, ⑤, in that order. The screws are not fixed, but you will tighten them when you mount the servo in the next step.

.. image:: ../_static/27.jpg
    :align: center

.. image:: ../_static/29.jpg
    :align: center

.. image:: ../_static/30.jpg
    :align: center

Completion of a right leg


* Now we have one leg on the right side. Here are some pictures so you can see it from different angles. The left leg should be symmetrical with the right one.

.. image:: ../_static/31.jpg
    :align: center

.. image:: ../_static/32.jpg
    :align: center

.. image:: ../_static/33.jpg
    :align: center

opposite side

.. image:: ../_static/34.jpg
    :align: center

.. image:: ../_static/35.jpg
    :align: center

Step 3.2 Four legs
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/36.jpg
    :align: center

Step 3.3 Locktite
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* As the nut is on a moving joint, it will loosen quickly if tightened too tightly. They should be secured with Loctite. It is possible to dismantle the nut later, as it can be loosened by a strong force.

.. image:: ../_static/37.jpg
    :align: center

* Some screws are also secured with glue as the below picture shows.

.. image:: ../_static/37_2.jpg
    :align: center


4. Hips Assembly
----------------

Step 4.1 Hip
^^^^^^^^^^^^

Please refer to the below video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/n1rLuf3AmUc?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


There are two kinds of servo cables, No.1,4,7,10 cables length is 9cm, other cables length is 15cm.

* For the position of each servos, please refer to the below picture.

.. image:: ../_static/52.jpg
    :align: center

* Here shows how to assemble the rear right hip.

Confirm whether the servo shaft is at the right position.
The middle position marker is added on the output shaft, the output shaft is at its middle position by fault as the left picture shows. The shaft position may be changed during assembly as the middle picture shows, if you find it, you can use the servo horn to move the output shaft to the right position, and then finally make the servo horn at the place as the right picture shows.

.. image:: ../_static/39.jpg
    :align: center

Connect the servo and hip part.

.. image:: ../_static/40_1.jpg
    :align: center

.. image:: ../_static/40_2.jpg
    :align: center

Put two servos into hip parts

* Insert two servos into the box and fix them with M2x6mm screws.

.. image:: ../_static/42_1.jpg
    :align: center

Four hip parts, please refer to the servo positions.

.. image:: ../_static/42.jpg
    :align: center


Assemble leg and hip

※ If you have no technology background, it's easier to attach the leg to the hip during the calibration step.

※ If you are the first time to assemble quadruped robot, we don't recommand you use the Loctite.

* Attach the leg to the hip using the M2x12mm screws. Leg is tilted at approximately 45°, as shown in the manual.

.. image:: ../_static/43_1.jpg
    :align: center

* Tighten the screws with Loctite. Use a toothpick to apply Loctite to the servo's screw holes.

.. image:: ../_static/45.jpg
    :align: center


.. image:: ../_static/45_1.jpg
    :align: center


.. image:: ../_static/46_1.jpg
    :align: center


Step 4.2 Four Hips
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/47.jpg
    :align: center

※ Please pay attention to the positions of the servo gear output shaft

.. image:: ../_static/47_left.jpg
    :align: center

.. image:: ../_static/47_right.jpg
    :align: center


5. Body Frame Assembly
-----------------------

Step 5.1 Center parts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The position of each servos are shown as below.

.. image:: ../_static/52.jpg
    :align: center

※ There are two kinds of servo cables, No.1,4,7,10 cables length is 9cm, other cables length is 15cm.

* It is useful to put masking tape on the cables and write the number of servos during this process to make it easier later.


.. image:: ../_static/48_1.jpg
    :align: center

.. image:: ../_static/49_1.jpg
    :align: center



Step 5.2 Front parts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The front part is designed to hold the LCD screen. Make sure you don't mistake it for the rear part.

.. image:: ../_static/53_1.jpg
    :align: center

.. image:: ../_static/54_1.jpg
    :align: center


Step 5.3 Rear side
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The same procedure as for the front part.

.. image:: ../_static/56_1.jpg
    :align: center

.. image:: ../_static/57_1.jpg
    :align: center

.. image:: ../_static/58_1.jpg
    :align: center

.. image:: ../_static/59_1.jpg
    :align: center



.. image:: ../_static/51_1.jpg
    :align: center


Step 5.4 Battery
^^^^^^^^^^^^^^^^^

* If you DIY the battery, please ensure our battery spec at first, especially the Voltage should be less than 7.4V, you can also refer to other backers work https://www.facebook.com/groups/716473723088464/posts/777616293640873/


* Install the battery pack.

.. image:: ../_static/83.jpg
    :align: center

* Be careful of the carbon fiber front and rear orientation.

.. image:: ../_static/84.jpg
    :align: center

* Slide the battery backwards and secure it. Pass the cable through the hole in the bottom plate and bring it up to the top.

.. image:: ../_static/85.jpg
    :align: center


Step 5.5 Bottom plate
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The orientation of the plate must be such that the hole is at the front.

.. image:: ../_static/61.jpg
    :align: center

* If the leg is stuck, turn the part ①

.. image:: ../_static/59_2.jpg
    :align: center

.. image:: ../_static/59_3.gif
    :align: center


Step 5.6 Display and Frame of face
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Remove the protective sheet for the display. Fold the thin flexible cable at the edge of the display. Attach the board and the display to the main unit. When attaching the display, you can use a stick to gently push the flexible cable, so that it goes as far back as possible.

.. image:: ../_static/74.jpg
    :align: center
.. image:: ../_static/75.jpg
    :align: center

.. image:: ../_static/76.jpg
    :align: center

.. image:: ../_static/77.jpg
    :align: center

.. image:: ../_static/78.jpg
    :align: center



* Be careful with the yellow parts as it has a front and back.

.. image:: ../_static/79.jpg
    :align: center

.. image:: ../_static/80.jpg
    :align: center

.. image:: ../_static/81.jpg
    :align: center


Step 5.7 Custom circuit board
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Plug the display cable into the custom circuit board.

.. image:: ../_static/88.jpg
    :align: center

.. image:: ../_static/89.jpg
    :align: center

* Insert the 12 servo cables. In the picture, you can see: J1,J2,J3.... . J12.

.. image:: ../_static/90.jpg
    :align: center

* Use four M2x5mm screws and four short supports.

.. image:: ../_static/63.jpg
    :align: center

.. image:: ../_static/64.jpg
    :align: center


* put on the carbon fiber board

.. image:: ../_static/91.jpg
    :align: center

* plug in the battery cable. This connector may interfere with the hips parts, so you have to slide it through a hole in the middle of the board.

.. image:: ../_static/92.jpg
    :align: center

* Use eight M2x5mm screws. The orientation of the plate must be such that the large opening is at the front.

.. image:: ../_static/66.jpg
    :align: center

* Pull the custom circuit board closer to the body. The board may float, but you can use four long posts to hold it in place.

.. image:: ../_static/93.jpg
    :align: center

.. image:: ../_static/94.jpg
    :align: center

.. image:: ../_static/95.jpg
    :align: center


※ Need to pay attention to the cable of the No. 1 servo to prevent it from being overwhelmed.

.. image:: ../_static/134.png
    :align: center



Step 5.8 Fan
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* To install the fan.

.. image:: ../_static/157.jpg
    :align: center

.. image:: ../_static/158.jpg
    :align: center


Step 5.9 Raspberry Pi 4
^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/96.jpg
    :align: center

.. image:: ../_static/97.jpg
    :align: center



6. Cover Assembly
-----------------
Please refer to the below video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/7s-ceq3U8jM?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>


Step 6.1 Side panels
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/111.jpg
    :align: center

.. image:: ../_static/112.jpg
    :align: center

Step 6.2 Shin guards
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Use four M2x10mm countersunk screws.

.. image:: ../_static/113.jpg
    :align: center

.. image:: ../_static/114.jpg
    :align: center

Step 6.3 Shoulders
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Insert only the screws first and then insert the shoulder parts into the gap. Insert the 2 mm hex driver into the hole in the shoulder part and tighten the screws.

.. image:: ../_static/115.jpg
    :align: center

.. image:: ../_static/116.jpg
    :align: center

.. image:: ../_static/117.jpg
    :align: center

.. image:: ../_static/118.jpg
    :align: center

Step 6.4 Top cover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Use four M2x10mm screws, if the holes are too small to fit the screws, as the part is made with a 3D printer, you can enlarge the holes by turning them with the supplied 2mm hexagonal screwdriver.

.. image:: ../_static/119.jpg
    :align: center

.. image:: ../_static/120.jpg
    :align: center

.. image:: ../_static/121.jpg
    :align: center

Step 6.5 Shoes
^^^^^^^^^^^^^^

* Put on 4 shoes.

.. image:: ../_static/122.jpg
    :align: center

.. image:: ../_static/123.jpg
    :align: center


Step 6.6 Completion!
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/124.jpg
    :align: center

.. image:: ../_static/125.jpg
    :align: center

7.Add-On Assembly
-----------------

Step 7.1 Lidar
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you order the Lidar, the Lidar holder will be shipped together.

.. image:: ../_static/126.jpg
    :align: center

.. image:: ../_static/127.jpg
    :align: center

.. image:: ../_static/130.jpg
    :align: center

Step 7.2 Camera
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you order the camera, the camera holder is not included in the kit.
But you can 3d-print it from the stl file down below.

https://drive.google.com/drive/folders/1lRADDbAt7mSBJE4j8HCji1WbWcpneUED

.. image:: ../_static/camera-1.jpg
    :align: center

.. image:: ../_static/camera-2.jpg
    :align: center

.. image:: ../_static/camera-3.jpg
    :align: center

Step 7.3 Completion!
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/OAK-Lidar.FrontView.jpg
    :align: center

.. image:: ../_static/OAK-Lidar.SideView.jpg
    :align: center

.. image:: ../_static/OAK-Lidar.TopView.jpg
    :align: center

.. raw:: html

   <div style="page-break-before: always;"></div>

Assemble Mini Pupper 2
######################

This is the video clip for the complete kit, please refer to the below sections for detailed steps.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/ZfJUBo4a09A?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Please also refer to Mini Pupper 2 Fusion 360 CAD model: https://a360.co/485n8mP


.. raw:: html

    <iframe src="https://a360.co/485n8mP?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


1. Write the pre-built image into microSD
------------------------------------------

Tools
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly.

* USB keyboard
* USB mouse
* PC
* microSD card reader
* HDMI Display
* micro HDMI cable
* USB charger


Step 1.1 Charging the battery
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The battery is charged via USB, see picture for USB socket, and can also be charged while attached to the Mini Pupper body.

※ LED light: Green means there is enough power, and Red means you need to charge it.

※ We recommend 5V/1A adapter, if you use 5V/2A adapter, the battery IC will change it to 1A. It needs about 1 hour to charge 80% and the light will become green, and an additional 1 hour to 100%, anyway, you can use it when the light becomes green.

.. image:: ../_static/100.jpg
    :align: center

Step 1.2 Download the image
^^^^^^^^^^^^^^^^^^^^^^^^^^^

* You can download the pre-built image files from  `Mini Pupper pre-built images <https://drive.google.com/drive/folders/1c0ShF-R8yxiMnCgMnSOctBpkW707b1q6?usp=sharing>`_

※ “xxx_stanford**.img” means the image is for Ubuntu 22.04 version.

* The picture below is the custom carry board.

.. image:: ../_static/147.v2.jpg
    :align: center

Step 1.3 Write the image into a microSD card
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Insert the microSD card into your PC's SD card reader and write the image. We recommend the image creation tool balenaEtcher or Win32DiskImager as it is easy and reliable. It may take a while to complete.


2. Position of the screws
-------------------------

* The pictures show the position of the screws briefly.

.. image:: ../_static/MPv2.screws1.jpg
    :align: center

.. image:: ../_static/MPv2.screws2.jpg
    :align: center

.. image:: ../_static/MPv2.screws3.jpg
    :align: center


3. Legs Assembly
----------------
Please refer to the below video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/Ut7UnS3CTZs?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Bolt to use
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
* M2x5mm	2x4=8	①+②, ⑤+⑥
* M2x8mm	3x4=12	②+③, ④+⑦, ③+④
* M2x12mm	1x4=4	⑤+⑦
* M2x14mm	1x4=4	③+⑤

Step 3.1 Single leg
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Assemble the four legs. The front and back of the right side are the same, and so are the front and back of the left side. Show you how to assemble the right side.

* Video Instructions, please refer to the link https://youtu.be/Ut7UnS3CTZs


* The parts are numbered as follows to explain.

.. image:: ../_static/1.jpg
    :align: center


Assemble ① and ②

.. image:: ../_static/2.v2.jpg
    :align: center

.. image:: ../_static/6.v2.1.jpg
    :align: center

* The two sides of bearings inside ② are different.

.. image:: ../_static/3.jpg
    :align: center

.. image:: ../_static/6.v2.jpg
    :align: center

Assemble ② and ③

* Use an M2x8mm screw and an M2 locknut. Insert the screw from the bottom to the top of ③, pass through ② and tighten with the nut. It is important to pay attention to the orientation of ③. Look carefully at the position of the hole in the middle.

.. image:: ../_static/7.v2.jpg
    :align: center

.. image:: ../_static/8.v2.jpg
    :align: center


Adjustment of the length of ④

* The length of ④ must match the length of ⑤. When adjusting the length, it is easier to use two long screws to make sure that the lengths match. Once the lengths have been adjusted, take apart all.

.. image:: ../_static/10.jpg
    :align: center

.. image:: ../_static/11.jpg
    :align: center

* If it's hard to twist, you can use two screwdrivers to assist.

.. image:: ../_static/11_1.jpg
    :align: center


Assemble ⑤ and ⑥

* Use one M2x5mm screw. Insert the screws into ⑤ first, insert them into the holes of ⑥, and tighten them. The large hole in ⑥ should be facing the surface.

.. image:: ../_static/12.jpg
    :align: center

.. image:: ../_static/13.jpg
    :align: center

.. image:: ../_static/14.jpg
    :align: center

Assemble ⑤ and ⑦

* Use an M2x12mm screw, an M2 locknut and two sets of ball bearings. Each ball bearing is made up of three parts, the top and bottom parts with the grooved side facing inwards. Insert a screw into a set of ball bearing. Then insert the screw into the hole ⑦. Taking care to look at the warped side of ⑦ to make sure it is facing the right way. Now screw in the another set of ball bearing. Finally, insert screw into ⑤ and tighten it with the nut.

.. image:: ../_static/15.jpg
    :align: center

.. image:: ../_static/18.jpg
    :align: center

.. image:: ../_static/19.jpg
    :align: center

.. image:: ../_static/21.jpg
    :align: center

.. image:: ../_static/20.jpg
    :align: center



Assemble ④ and ⑦

* Use an M2x8mm screw and an M2 nut. Insert the screw into ⑦ and put ④ through, then tighten it with the nut. The direction of the front and back of ④ can be either.

Left and right leg

.. image:: ../_static/22.jpg
    :align: center

.. image:: ../_static/23.jpg
    :align: center

.. image:: ../_static/24.jpg
    :align: center

Assemble ③ and ④

* Use an M2x8mm screw and an M2 nut. Insert the screw into ③ and put ④ through, then tighten it with the nut.

Left and right leg

.. image:: ../_static/25.v2.jpg
    :align: center

.. image:: ../_static/26.jpg
    :align: center

Assemble ③ and ⑤

* Use M2x14mm screws and two sets of ball bearings. Thread the screws through the bearings, ③, bearings, ⑤, in that order. The screws are not fixed, but you will tighten them when you mount the servo in the next step.

.. image:: ../_static/27.v2.jpg
    :align: center

.. image:: ../_static/29.jpg
    :align: center

.. image:: ../_static/30.jpg
    :align: center

Completion of a right leg


* Now we have one leg on the right side. Here are some pictures so you can see it from different angles. The left leg should be symmetrical with the right one.

.. image:: ../_static/31.v2.jpg
    :align: center

.. image:: ../_static/32.jpg
    :align: center

opposite side

.. image:: ../_static/34.v2.jpg
    :align: center

Step 3.2 Four legs
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/36.v2.jpg
    :align: center

Step 3.3 Locktite
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

After Mini Pupper run sometime, some screws or nuts will loose, you have to check and tighten them if needed. It's helpful to understand how it works.

※ We don't recommend new users to use the Loctite at first, you can use it after you have much background.

※ Loctite prevents the nut from loosening, but it is not essential, as it can be tightened only when looseness is noticed.

.. image:: ../_static/37.jpg
    :align: center

.. image:: ../_static/45.jpg
    :align: center

* Some screws are also secured with glue as the below picture shows.

.. image:: ../_static/37_2.jpg
    :align: center

4. Display and Frame of face
-----------------------------

Remove the protective sheet for the display. Fold the thin flexible cable at the edge of the display. Attach the board and the display to the main unit.

.. image:: ../_static/74.jpg
    :align: center

.. image:: ../_static/79.v2.1.jpg
    :align: center

.. image:: ../_static/79.v2.2.jpg
    :align: center

.. image:: ../_static/79.v2.3.jpg
    :align: center

* When attaching the display, you can use a stick to gently push the flexible FPC cable, so that it goes as far back as possible. Don't bend this FPC cable at 180 degrees.

.. image:: ../_static/79.v2.4.jpg
    :align: center

.. image:: ../_static/79.v2.5.jpg
    :align: center


5. Body Frame and Hips Assembly
---------------------------------

* Refer to the top video for how to set servo ID.
* For the position of each servo, please refer to the below picture.

.. image:: ../_static/52.v2.jpg
    :align: center

Step 5.1 Body center parts
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Connect the No.1, 4, 7, 10 servos to the body center parts.

* It is useful to put masking tape on the cables and write the number of servos during this process to make it easier later.


.. image:: ../_static/49.v2.1.jpg
    :align: center

* Pay attention to the center part direction.

.. image:: ../_static/49.v2.2.jpg
    :align: center

.. image:: ../_static/49.v2.3.jpg
    :align: center

Connect the center parts to the bottom carbon fiber

* Be careful of the carbon fiber front and rear orientation.

.. image:: ../_static/49.v2.4.jpg
    :align: center

.. image:: ../_static/49.v2.5.jpg
    :align: center

Step 5.2 Hip parts
^^^^^^^^^^^^^^^^^^^^
Assemble four hip parts, please refer to the servo positions.

.. image:: ../_static/49.v2.6.jpg
    :align: center

.. image:: ../_static/49.v2.7.jpg
    :align: center

Ensure the No.1, 4, 7, 10 servos at the right position.

.. image:: ../_static/49.v2.8.jpg
    :align: center

Use the custom cable to connect the battery to the top PCB board, and click the battery button for more than 3 seconds to boot up it.

.. image:: ../_static/49.v2.9.jpg
    :align: center

Connect the servos to the top PCB board, please pay attention to the servo connector directions.

.. image:: ../_static/49.v2.10.jpg
    :align: center

.. image:: ../_static/49.v2.11.jpg
    :align: center

Connect the four hip parts to the body, please pay attention.

* Don't power off the battery now.
* Ensure all the servo positions are right.

.. image:: ../_static/49.v2.12.jpg
    :align: center

Step 5.3 Front and back body parts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Power off the battery, and connect the front and back body parts.

.. image:: ../_static/49.v2.13.jpg
    :align: center

.. image:: ../_static/49.v2.14.jpg
    :align: center

Pay attention to the directions.

.. image:: ../_static/49.v2.16.jpg
    :align: center

Power on the battery to check the hip parts all at their right positions, connect all the rest servos to the PCB board, and then power off the battery and go ahead.

.. image:: ../_static/49.v2.19.jpg
    :align: center

Connect the LCD cable to the PCB board, make the servo cables clear.

.. image:: ../_static/49.v2.20.jpg
    :align: center

.. image:: ../_static/49.v2.21.jpg
    :align: center

Fix the top and bottom boards.

.. image:: ../_static/49.v2.22.jpg
    :align: center

.. image:: ../_static/49.v2.23.jpg
    :align: center

.. image:: ../_static/49.v2.24.jpg
    :align: center


Step 5.4 Assemble four legs to the body
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/49.v2.25.jpg
    :align: center

Pay attention to the theoretically best angles, it's better to meet the theoretically best angles as much as possible.
But don't worry, we'll use the software to calibrate the angles later.

.. image:: ../_static/49.v2.26.jpg
    :align: center

.. image:: ../_static/49.v2.27.jpg
    :align: center


Step 5.5 Assemble the battery to the body
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/49.v2.28.jpg
    :align: center

Slide the battery backward and secure it.

.. image:: ../_static/49.v2.29.jpg
    :align: center

.. image:: ../_static/85.jpg
    :align: center

.. image:: ../_static/84.jpg
    :align: center

Step 5.6 Assemble the speaker
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/MP2.Speak.1.jpg
    :align: center

.. image:: ../_static/MP2.Speak.2.jpg
    :align: center


6. Cover Assembly
-----------------
Please refer to the below video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/Nw8dl4CGt9A?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Step 6.1 Side panels
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/111.v2.jpg
    :align: center

.. image:: ../_static/112.v2.jpg
    :align: center

Step 6.2 Shin guards
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Use four M2x10mm countersunk screws.

.. image:: ../_static/113.v2.jpg
    :align: center

.. image:: ../_static/114.v2.jpg
    :align: center

Step 6.3 Shoulders
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Insert only the screws first and then insert the shoulder parts into the gap. Insert the 2 mm hex driver into the hole in the shoulder part and tighten the screws.

.. image:: ../_static/114.v2.2.jpg
    :align: center

.. image:: ../_static/117.v2.jpg
    :align: center

.. image:: ../_static/117.v2.2.jpg
    :align: center

.. image:: ../_static/122.v2.jpg
    :align: center

Step 6.4 Shoes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Put on 4 shoes.

.. image:: ../_static/122.v2.jpg
    :align: center

.. image:: ../_static/123.v2.jpg
    :align: center


Complete!
^^^^^^^^^^



7. Add-On Assembly
-------------------

Step 7.1 Lidar
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you order the Lidar, the 3D-printed Lidar holder and custom cable will be shipped together. You can also print the holder by yourself using the  `Mini Pupper 2 STL files <https://drive.google.com/drive/folders/1G8TsAhhomSA2-VkI1Wiqmuhu92EsJNb2>`_

.. image:: ../_static/MP2.Lidar.1.jpg
    :align: center

Connect the 3 holders to the 3D-printed part.

.. image:: ../_static/MP2.Lidar.2.jpg
    :align: center

Connect the custom cable to the Lidar connector on the PCB board.

.. image:: ../_static/MP2.Lidar.3.jpg
    :align: center

Fix the 3D-printed part on the PCB board.

.. image:: ../_static/MP2.Lidar.4.jpg
    :align: center

Connect the custom cable to the Lidar module and fix it using the self-tapping screws.

.. image:: ../_static/MP2.Lidar.5.jpg
    :align: center

Step 7.2 Camera
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Mini Pupper 2 also supports the single Pi camera or OpenCV OAK-D-Lite camera module. You can also print the holder by yourself using the `Mini Pupper 2 STL files <https://drive.google.com/drive/folders/1G8TsAhhomSA2-VkI1Wiqmuhu92EsJNb2>`_


.. image:: ../_static/MP2.LidarCamera.1.jpg
    :align: center

.. image:: ../_static/MP2.LidarCamera.2.jpg
    :align: center

.. image:: ../_static/MP2.LidarCamera.3.jpg
    :align: center

.. raw:: html

   <div style="page-break-before: always;"></div>

Assemble Mini Pupper 2 Pro
###########################


※ General DIY process:

* Assemble --> Calibration --> Run

※ Attention:

* The MCU(ESP32 and AT32) software are both pre-installed, you don't need to flash any MCU image.
* You don't need to set each servo number as Mini Pupper 2 because the servo number is fixed by the hardware design, please follow the guide to put the servo to the right positions.


Please refer to Mini Pupper 2 Fusion 360 CAD model for your reference: https://a360.co/485n8mP


.. raw:: html

    <iframe src="https://a360.co/485n8mP?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


1. Write the pre-built image into microSD
-----------------------------------------

Tools
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly.

* USB keyboard
* USB mouse
* PC
* microSD card reader
* HDMI Display
* micro HDMI cable
* USB charger


Step 1.1 Charging the battery
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The battery is charged via USB, see picture for USB socket, and can also be charged while attached to the Mini Pupper body.

※ LED light: Green means there is enough power, and Red means you need to charge it.

※ We recommend 5V/1A adapter, if you use 5V/2A adapter, the battery IC will change it to 1A. It needs about 1 hour to charge 80% and the light will become green, and an additional 1 hour to 100%, anyway, you can use it when the light becomes green.

.. image:: ../_static/100.jpg
    :align: center

Step 1.2 Download the image
^^^^^^^^^^^^^^^^^^^^^^^^^^^

* You can download the pre-built image files from  `Mini Pupper pre-built images <https://drive.google.com/drive/folders/1c0ShF-R8yxiMnCgMnSOctBpkW707b1q6?usp=sharing>`_

※ “v2Pro_stanford**.img” means the image is for Ubuntu 22.04 version.

* The picture below is the custom carry board.

.. image:: ../_static/147.v2.jpg
    :align: center

Step 1.3 Write the image into a microSD card
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Insert the microSD card into your PC's SD card reader and write the image. We recommend the image creation tool balenaEtcher or Win32DiskImager as it is easy and reliable. It may take a while to complete.


2. Position of the screws
-------------------------

* The pictures show the position of the screws briefly.

.. image:: ../_static/MPv2.screws1.jpg
    :align: center

.. image:: ../_static/MPv2.screws2.jpg
    :align: center

.. image:: ../_static/MPv2.screws3.jpg
    :align: center


3. Legs Assembly
----------------
Please refer to the below video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/Ut7UnS3CTZs?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Bolt to use
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
* M2x5mm	2x4=8	①+②, ⑤+⑥
* M2x8mm	3x4=12	②+③, ④+⑦, ③+④
* M2x12mm	1x4=4	⑤+⑦
* M2x14mm	1x4=4	③+⑤

Step 3.1 Single leg
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Assemble the four legs. The front and back of the right side are the same, and so are the front and back of the left side. Show you how to assemble the right side.

* Video Instructions, please refer to the link https://youtu.be/Ut7UnS3CTZs


* The parts are numbered as follows to explain.

.. image:: ../_static/1.jpg
    :align: center


Assemble ① and ②

.. image:: ../_static/2.v2.jpg
    :align: center

.. image:: ../_static/6.v2.1.jpg
    :align: center

* The two sides of bearings inside ② are different.

.. image:: ../_static/3.jpg
    :align: center

.. image:: ../_static/6.v2.jpg
    :align: center

Assemble ② and ③

* Use an M2x8mm screw and an M2 locknut. Insert the screw from the bottom to the top of ③, pass through ② and tighten with the nut. It is important to pay attention to the orientation of ③. Look carefully at the position of the hole in the middle.

.. image:: ../_static/7.v2.jpg
    :align: center

.. image:: ../_static/8.v2.jpg
    :align: center


Adjustment of the length of ④

* The length of ④ must match the length of ⑤. When adjusting the length, it is easier to use two long screws to make sure that the lengths match. Once the lengths have been adjusted, take apart all.

.. image:: ../_static/10.jpg
    :align: center

.. image:: ../_static/11.jpg
    :align: center

* If it's hard to twist, you can use two screwdrivers to assist.

.. image:: ../_static/11_1.jpg
    :align: center


Assemble ⑤ and ⑥

* Use one M2x5mm screw. Insert the screws into ⑤ first, insert them into the holes of ⑥, and tighten them. The large hole in ⑥ should be facing the surface.

.. image:: ../_static/12.jpg
    :align: center

.. image:: ../_static/13.jpg
    :align: center

.. image:: ../_static/14.jpg
    :align: center

Assemble ⑤ and ⑦

* Use an M2x12mm screw, an M2 locknut and two sets of ball bearings. Each ball bearing is made up of three parts, the top and bottom parts with the grooved side facing inwards. Insert a screw into a set of ball bearing. Then insert the screw into the hole ⑦. Taking care to look at the warped side of ⑦ to make sure it is facing the right way. Now screw in the another set of ball bearing. Finally, insert screw into ⑤ and tighten it with the nut.

.. image:: ../_static/15.jpg
    :align: center

.. image:: ../_static/18.jpg
    :align: center

.. image:: ../_static/19.jpg
    :align: center

.. image:: ../_static/21.jpg
    :align: center

.. image:: ../_static/20.jpg
    :align: center



Assemble ④ and ⑦

* Use an M2x8mm screw and an M2 nut. Insert the screw into ⑦ and put ④ through, then tighten it with the nut. The direction of the front and back of ④ can be either.

Left and right leg

.. image:: ../_static/22.jpg
    :align: center

.. image:: ../_static/23.jpg
    :align: center

.. image:: ../_static/24.jpg
    :align: center

Assemble ③ and ④

* Use an M2x8mm screw and an M2 nut. Insert the screw into ③ and put ④ through, then tighten it with the nut.

Left and right leg

.. image:: ../_static/25.v2.jpg
    :align: center

.. image:: ../_static/26.jpg
    :align: center

Assemble ③ and ⑤

* Use M2x14mm screws and two sets of ball bearings. Thread the screws through the bearings, ③, bearings, ⑤, in that order. The screws are not fixed, but you will tighten them when you mount the servo in the next step.

.. image:: ../_static/27.v2.jpg
    :align: center

.. image:: ../_static/29.jpg
    :align: center

.. image:: ../_static/30.jpg
    :align: center

Completion of a right leg


* Now we have one leg on the right side. Here are some pictures so you can see it from different angles. The left leg should be symmetrical with the right one.

.. image:: ../_static/31.v2.jpg
    :align: center

.. image:: ../_static/32.jpg
    :align: center

opposite side

.. image:: ../_static/34.v2.jpg
    :align: center

Step 3.2 Four legs
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/36.v2.jpg
    :align: center

Step 3.3 Locktite
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

After Mini Pupper run sometime, some screws or nuts will loose, you have to check and tighten them if needed. It's helpful to understand how it works.

※ We don't recommend new users to use the Loctite at first, you can use it after you have much background.

※ Loctite prevents the nut from loosening, but it is not essential, as it can be tightened only when looseness is noticed.

.. image:: ../_static/37.jpg
    :align: center

.. image:: ../_static/45.jpg
    :align: center

* Some screws are also secured with glue as the below picture shows.

.. image:: ../_static/37_2.jpg
    :align: center

4. Display and Frame of face
-------------------------------

Remove the protective sheet for the display. Fold the thin flexible cable at the edge of the display. Attach the board and the display to the main unit.

.. image:: ../_static/74.2pro.jpg
    :align: center

.. image:: ../_static/79.v2.1.jpg
    :align: center

.. image:: ../_static/79.v2.2.jpg
    :align: center

.. image:: ../_static/79.v2.3.jpg
    :align: center

* When attaching the display, you can use a stick to gently push the flexible FPC cable, so that it goes as far back as possible. Don't bend this FPC cable at 180 degrees.

.. image:: ../_static/79.v2.4.jpg
    :align: center

.. image:: ../_static/79.v2.5.jpg
    :align: center


5. Body Frame and Hips Assembly
-------------------------------

* Before you connect the CM4 module to the carry board, please make sure to remove the protective film on the Thermal Pad.

.. image:: ../_static/53.v2Pro.jpg
    :align: center


* Don't need to set servo ID for v2 pro version, the servo ID is fixed by hardware design.
* For the position of each servo, please refer to the below picture.

.. image:: ../_static/52.v2Pro.jpg
    :align: center

Step 5.1 Body center parts
^^^^^^^^^^^^^^^^^^^^^^^^^^

Connect the No.1, 4, 7, 10 servos to the body center parts.

* It is useful to put masking tape on the cables and write the number of servos during this process to make it easier later.


.. image:: ../_static/49.v2.1.jpg
    :align: center

* Pay attention to the center part direction.

.. image:: ../_static/49.v2.2.jpg
    :align: center

.. image:: ../_static/49.v2.3.jpg
    :align: center

Step 5.2 Hip parts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Assemble four hip parts, please refer to the servo positions.

.. image:: ../_static/49.v2.6.jpg
    :align: center

.. image:: ../_static/49.v2.7.jpg
    :align: center

* Connect the No.1, 4, 7, 10 servos to the servo MCU PCB baord.

.. image:: ../_static/v2pro.1.jpg
    :align: center

* Connect the rest servos to the servo MCU PCB baord.

.. image:: ../_static/v2pro.2.jpg
    :align: center

Pay attention to the servo cable connectors' directions.

.. image:: ../_static/v2pro.2.1.jpg
    :align: center

* Use the DIY cable to connect the top PCB board to the servo MCU PCB baord.

.. image:: ../_static/v2pro.3.jpg
    :align: center

* Power on the battery and connect to the top PCB board.

.. image:: ../_static/v2pro.4.jpg
    :align: center

* Connect the four black hip parts to the relative servos(No. 1,4,7,10).

.. image:: ../_static/v2pro.5.jpg
    :align: center

Connect the four hip parts to the body, please pay attention.

* Don't power off the battery now.
* Ensure all the servo positions are right.

Step 5.3 Front and back body parts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Power off the battery, adjust the red cable position and connect the front and back body parts.

.. image:: ../_static/v2pro.6.jpg
    :align: center

Use the screws to fix the top PCB board.

.. image:: ../_static/v2pro.7.jpg
    :align: center

You can tighten the servo MCU PCB board with tape.

.. image:: ../_static/v2pro.7.1.jpg
    :align: center


Power the battery and connect to the top PCB board to ensure the four black hip part positions are right.

.. image:: ../_static/v2pro.8.jpg
    :align: center


Connect the center parts to the bottom carbon fiber.

.. image:: ../_static/v2pro.9.jpg
    :align: center

* Be careful of the carbon fiber front and rear orientation.


Step 5.4 Assemble four legs to the body
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Prepare the four pre-assembled legs

.. image:: ../_static/v2pro.10.jpg
    :align: center

Pay attention to the theoretically best angles, it's better to meet the theoretically best angles as much as possible.

But don't worry, we'll use the software to calibrate the angles later.

.. image:: ../_static/v2pro.11.jpg
    :align: center

.. image:: ../_static/v2pro.12.jpg
    :align: center


Step 5.5 Assemble the battery to the body
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/49.v2.28.jpg
    :align: center

Slide the battery backward and secure it.

.. image:: ../_static/49.v2.29.jpg
    :align: center

.. image:: ../_static/85.jpg
    :align: center

.. image:: ../_static/84.jpg
    :align: center

Step 5.6 Assemble the speaker
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/MP2.Speak.1.jpg
    :align: center

.. image:: ../_static/MP2.Speak.2.jpg
    :align: center


6. Cover Assembly
-----------------
Please refer to the below video clip.

.. raw:: html

    <div style="position: relative; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/Nw8dl4CGt9A?mute=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

Step 6.1 Side panels
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/111.v2.jpg
    :align: center

.. image:: ../_static/112.v2.jpg
    :align: center

Step 6.2 Shin guards
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Use four M2x10mm countersunk screws.

.. image:: ../_static/113.v2.jpg
    :align: center

.. image:: ../_static/114.v2.jpg
    :align: center

Step 6.3 Shoulders
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Insert only the screws first and then insert the shoulder parts into the gap. Insert the 2 mm hex driver into the hole in the shoulder part and tighten the screws.

.. image:: ../_static/114.v2.2.jpg
    :align: center

.. image:: ../_static/117.v2.jpg
    :align: center

.. image:: ../_static/117.v2.2.jpg
    :align: center

.. image:: ../_static/122.v2.jpg
    :align: center

Step 6.4 Shoes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Put on 4 shoes.

.. image:: ../_static/122.v2.jpg
    :align: center

.. image:: ../_static/123.v2.jpg
    :align: center


Complete!
^^^^^^^^^^



7. Add-On Assembly
-------------------

Step 7.1 Lidar
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you order the Lidar, the 3D-printed Lidar holder and custom cable will be shipped together. You can also print the holder by yourself using the  `Mini Pupper 2 STL files <https://drive.google.com/drive/folders/1G8TsAhhomSA2-VkI1Wiqmuhu92EsJNb2>`_

.. image:: ../_static/MP2.Lidar.1.jpg
    :align: center

Connect the 3 holders to the 3D-printed part.

.. image:: ../_static/MP2.Lidar.2.jpg
    :align: center

Connect the custom cable to the Lidar connector on the PCB board.

.. image:: ../_static/MP2.Lidar.3.jpg
    :align: center

Fix the 3D-printed part on the PCB board.

.. image:: ../_static/MP2.Lidar.4.jpg
    :align: center

Connect the custom cable to the Lidar module and fix it using the self-tapping screws.

.. image:: ../_static/MP2.Lidar.5.jpg
    :align: center

Step 7.2 Camera
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Mini Pupper 2 also supports the single Pi camera or OpenCV OAK-D-Lite camera module. You can also print the holder by yourself using the `Mini Pupper 2 STL files <https://drive.google.com/drive/folders/1G8TsAhhomSA2-VkI1Wiqmuhu92EsJNb2>`_


.. image:: ../_static/MP2.LidarCamera.1.jpg
    :align: center

.. image:: ../_static/MP2.LidarCamera.2.jpg
    :align: center

.. image:: ../_static/MP2.LidarCamera.3.jpg
    :align: center


.. raw:: html

   <div style="page-break-before: always;"></div>
