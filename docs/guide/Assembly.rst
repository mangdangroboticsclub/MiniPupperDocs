Assembly
========

.. contents::
  :depth: 2

1. Write the image into microSD
-------------------------------

Tools
^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly. キットに同梱されている工具の他に、組み立てには以下の物が必要です。

* USB keyboard USB キーボード 
* USB mouse USB マウス 
* PC
* microSD card interface microSDカードリーダ  
* HDMI Display HDMI ディスプレイ 
* HDMI micro HDMI convertor HDMI⇔microHDMI変換 
* microUSB cable microUSB ケーブル 
* USB charger


Step 1.1 Charging the battery
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* The battery is charged via USB, see picture for USB socket, and can be charged while still attached to the Mini Pupper body. 準備としてバッテリーをUSBで充電しておきます。USBの差込口は写真を参照。Mini Pupperに取り付けたままでも充電できます。

.. image:: ../_static/100.jpg
    :align: center 

Step 1.2 Download the image
^^^^^^^^^^^^^^^^^^^^^^^^^^^

* You can check other documents or latest image file via the below folder. 以下のフォルダから他のドキュメントや最新のイメージを確認できます.

	`MiniPupperRelease.from.MangDang <https://drive.google.com/drive/folders/12FDFbZzO61Euh8pJI9oCxN-eLVm5zjyi?usp=sharing>`_ 
	
	
* For the V1 Custom circuit board, the image file xxx_MiniPupper_PS4_Ubuntu_xxx.img.zip is shown as below. 
V1カスタム回路基板の場合、イメージファイルは xxx_MiniPupper_PS4_Ubuntu_xxx.img.zipになります。

.. image:: ../_static/146.jpg
    :align: center
    


* For the V2 Custom circuit board, the image file xxx_MiniPupper_V2_PS4_Ubuntu_xxx.img.zip is shown as below. 
V2カスタム回路基板の場合、イメージファイルは xxx_MiniPupper_V2_PS4_Ubuntu_xxx.img.zip になります。

.. image:: ../_static/147.jpg
    :align: center
    
	
"xxx.MiniPupper_V2_ROS&OpenCV_Ubuntu20.04.03.img.zip" is image file for the Ubuntu + ROS + OpenCV version for SLAM & Navigation & AI.   
「xxx.MiniPupper_V2_ROS&OpenCV_Ubuntu20.04.03.img.zip」はSLAM＆Navigation&AI のUbuntu + ROS + OpenCV バージョンのイメージファイルです。
	
* Download the image for Raspi 4 from MangDang on your PC.  PCでMangDangからラズパイ4用イメージをダウンロードします。
   
	
Step 1.3 Write the image into microSD
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Insert the microSD card into your PC's SD card reader and pwrite the image. We recommend the image creation tool balenaEtcher as it is easy and reliable. Please refer to the official manual and below link. It may take a while to complete. PCのSDカードリーダにmicroSDカードを入れて、イメージを書き込みます。イメージ作成ツール balenaEtcherが簡単かつ確実なのでおすすめです。オフィシャルマニュアルやリンク先を参考に書き込みましょう。完了までかなり時間がかかります。

Reference Link: `Download Etcher – Flash OS images to USB drives & SD cards <https://etcherpc.com/?usp=sharing>`_ 

参考：`簡単な 3 ステップで使えるブートUSB 作成ツール！「balenaEtcher」 <https://www.gigafree.net/system/os/Etcher.html?usp=sharing>`_ 

* Remove the SD card from the PC and insert it into the Raspberry pi. PCからSDカードを抜いて、ラズパイに挿す。

.. image:: ../_static/145.jpg
    :align: center 


2. Position of the screws
-------------------------

* The pictures show the position of the screws briefly. 写真はネジの位置を簡単に示しています。
    
.. image:: ../_static/136.jpg
    :align: center
    
.. image:: ../_static/137.jpg
    :align: center  
    
.. image:: ../_static/138.jpg
    :align: center
    
.. image:: ../_static/139.jpg
    :align: center
    
.. image:: ../_static/140.jpg
    :align: center  
    
.. image:: ../_static/144.jpg
    :align: center
    
.. image:: ../_static/141.jpg
    :align: center  
    
.. image:: ../_static/142.jpg
    :align: center  
    
3. Legs Assembly
----------------

Tools
^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly. キットに同梱されている工具の他に、組み立てには以下の物が必要です。

* Loctite
(!!! We don’t suggest you use Loctite at first before you have enough experience. !!!)
Loctite prevents the nut from loosening, but it is not essential, as it can be tightened only when looseness is noticed. However, some of them have to be dismantled in order to be tightened later, so fix them as much as possible. ロックタイトはナットの緩みを防止しますが、緩みに気づいたときに締めれば良いので必須ではありません。ただ、後から締めるためには一部解体しなければならないものもありますので、極力固定しましょう。

Bolt to use
^^^^^^^^^^^^^^^^^^^^^
* M2x5mm	2x4=8	①+②, ⑤+⑥
* M2x8mm	3x4=12	②+③, ④+⑦, ③+④
* M2x12mm	1x4=4	⑤+⑦
* M2x14mm	1x4=4	③+⑤

Step 3.1 Single leg
^^^^^^^^^^^^^^^^^^^^^

* Assemble the four legs. The front and back of the right side are the same, and so are the front and back of the left side. Show you how to assemble the right side.

* Video Instructions

.. |youtu.be-assembly-leg-1| raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/embed/H1ESo4Olz3s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

.. |youtu.be-assembly-leg-1-ja| raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/embed/WZFuACfvTAY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

|youtu.be-assembly-leg-1|

* The parts are numbered as follows to explain.

.. image:: ../_static/1.png
    :align: center


Assemble ① and ② / ①と②の組み立て:

* Use one M2x5mm screw.The screw is inserted from the bottom of ② upwards and tightened by inserting them into the screw holes in ①. Be careful about the sides of ②. M2x5mm のボルトを1つ使用します。ボルトは②の下から上に挿し、①の穴に挿し込んで締めます。②の表裏の向きに気をつけましょう。

* The two ballbearings in ② should be inserted all the way in and the end should be slightly visible as shown in the picture below. Tap the ball bearing and press it in without gaps. ②のボールベアリング2個は奥まで挿し込み、下記の写真のように先が少し見える状態になっている必要があります。叩くなどして隙間をなくせば大丈夫です。

.. image:: ../_static/2.png
    :align: center

.. image:: ../_static/3.jpg
    :align: center
    
.. image:: ../_static/4.jpg
    :align: center
    
.. image:: ../_static/5.png
    :align: center    
    
.. image:: ../_static/6.jpg
    :align: center    
    
    
Assemble ② and ③ / ②と③の組み立て:

* Use an M2x8mm screw and an M2 locknut. Insert the screw from the bottom to the top of ③, pass through ② and tighten with the nut. It is important to pay attention to the orientation of ③. Look carefully at the position of the hole in the middle. M2x8mm のボルトを1つと M2 Locknutを使用します。ボルトを③の下から上に挿し、②を通し、ナットで締めます。③の部品の向きには気をつける必要があります。真ん中の穴の位置を良く見ましょう。

.. image:: ../_static/7.png
    :align: center

.. image:: ../_static/8.png
    :align: center
    
.. image:: ../_static/9.jpg
    :align: center


Adjustment of the length of ④ / ④の長さの調整  

* The length of ④ must match the length of ⑤. When adjusting the length, it is easier to use two long screws, e.g. M2x15mm, to make sure that the lengths match. Once the lengths have been adjusted, take apart all. ④の長さが⑤と一致している必要があります。長さを調整するとき、M2x15mmなどの長いボルトを2本使うと、長さが一致しているか確認しやすいです。長さの調整が完了したら、これらはすべてバラしましょう。

.. image:: ../_static/10.png
    :align: center
    
.. image:: ../_static/11.jpg
    :align: center


Assemble ⑤ and ⑥ / ⑤と⑥の組み立て 

* Use two M2x5mm screws. Insert the screws into ⑤ first, insert them into the holes of ⑥, and tighten them. The large hole in ⑥ should be facing the surface. M2x5mmのボルトを1本使用します。⑤にボルトを挿し、⑥の穴に挿れて締めます。⑥は大きな穴がある方が表面側に来るように向けましょう。

.. image:: ../_static/12.png
    :align: center

.. image:: ../_static/13.jpg
    :align: center
    
.. image:: ../_static/14.jpg
    :align: center

Assemble ⑤ and ⑦ / ⑤と⑦の組み立て

* Use an M2x12mm screw, an M2 locknut and two sets of ball bearings. Each ball bearing is made up of three parts, the top and bottom parts with the grooved side facing inwards. Insert a screw into a set of ball bearing. Then insert the screw into the hole ⑦. Taking care to look at the warped side of ⑦ to make sure it is facing the right way. Now screw in the another set of ball bearing. Finally, insert screw into ⑤ and tighten it with the nut. M2x12mmのボルトとM2 locknutとボールベアリング2組を使用します。ボールベアリングは3つの部品から成り立っており、上下の部品は溝がある方を内側に向けて、真ん中の部品をはさみます。まずボールベアリングにボルトを通します。次に⑦の穴にボルトを挿します。このとき⑦の反っている方向を見て、向きを間違えないように気をつけます。次にもう一つのボールベアリングをボルトに通します。最後に⑤をボルトに通してナットで締めます。

.. image:: ../_static/15.png
    :align: center

.. image:: ../_static/16.jpg
    :align: center
    
.. image:: ../_static/17.jpg
    :align: center
    
.. image:: ../_static/18.jpg
    :align: center

.. image:: ../_static/19.jpg
    :align: center
    
.. image:: ../_static/20.jpg
    :align: center
    
.. image:: ../_static/21.jpg
    :align: center
    
Assemble ④ and ⑦ / ④と⑦の組み立て

* Use an M2x8mm screw and an M2 nut. Insert the screw into ⑦ and put ④ through, then tighten it with the nut. The direction of the front and back of ④ can be either. M2x8mmのボルトとM2ナットを使用します。⑦にボルトを挿し、④を通したら、ナットで締めます。④の表裏の向きはどちらでも大丈夫です。
    
.. image:: ../_static/22.png
    :align: center
    
.. image:: ../_static/23.jpg
    :align: center
    
.. image:: ../_static/24.jpg
    :align: center
    
Assemble ③ and ④ / ③と④の組み立て 

* Use an M2x8mm screw and an M2 nut. Insert the screw into ③ and put ④ through, then tighten it with the nut. M2x8mmのボルトとM2ナットを使用します。③にボルトを挿し、④を通したら、ナットで締めます。

.. image:: ../_static/25.png
    :align: center
    
.. image:: ../_static/26.jpg
    :align: center

Assemble ③ and ⑤ / ③と⑤の組み立て

* Use M2x14mm screws and two sets of ball bearings. Thread the screws through the bearings, ③, bearings, ⑤, in that order. The screws are not fixed, but you will tighten them when you mount the servo in the next step. M2x14mmのボルトとボールベアリング2組を使用します。ボルトをベアリング、③、ベアリング、⑤の順で通します。ボルトは固定されていませんが、次工程でサーボに取り付ける際にボルトを締めます。

.. image:: ../_static/27.png
    :align: center
    
.. image:: ../_static/28.jpg
    :align: center

.. image:: ../_static/29.jpg
    :align: center
    
.. image:: ../_static/30.jpg
    :align: center
    
Completion of a right leg / 脚部の仕上げ

Front side / 表

* Now we have one leg on the right side. Here are some pictures so you can see it from different angles. The left leg should be symmetrical with the right one. これで右側の脚が一本完成しました。色んな角度から見れるように写真を貼っておきます。左側は右側と線対称になるように組みます。
    
.. image:: ../_static/31.jpg
    :align: center

.. image:: ../_static/32.jpg
    :align: center
    
.. image:: ../_static/33.jpg
    :align: center

opposite side / 裏

.. image:: ../_static/34.jpg
    :align: center
    
.. image:: ../_static/35.jpg
    :align: center
    
Step 3.2 Four legs
^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/36.jpg
    :align: center

Step 3.3 Locktite
^^^^^^^^^^^^^^^^^^^^^

* As the nut is on a moving joint, it will loosen quickly if tightened too tightly. They should be secured with Loctite. It is possible to dismantle the nut later, as it can be loosened by a strong force. ナットは動く関節にあるので、ナットを強く締めても直ぐに緩んでしまいます。ロックタイトで固定しましょう。なお、ロックタイトで固定されたナットは強い力ならば緩められるので、あとから解体も可能です。

.. image:: ../_static/37.jpg
    :align: center


4. Hips Assembly
----------------

Tools
^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly. キットに同梱されている工具の他に、組み立てには以下の物が必要です。

* Elongated screwdriver/ 細長いプラスドライバー 
* Elongated hex wrench (2mm) / 細長い2mm経の六角レンチ
* Loctite / ロックタイト
* Thin things like a toothpick / 爪楊枝のような細いもの

Bolt to use
^^^^^^^^^^^^^^^^^^^^^

* M2x6mm(Self tapping)	1x4=4	
* M2x6mm	1x4+4x4=20  

Step 4.1 Hip
^^^^^^^^^^^^^^^^^^^^^

※ For the latest kit, there are two kinds of servo cables, No.1,4,7,10 cables length is 9cm, other cables length is 15cm. 

最新のキットには、サーボケーブルが2種類あります。No.1、4、7、10のケーブル長は9cm、その他のケーブル長は15cmです。

* The position of each servomotors are shown as below. 各サーボモータの位置は以下のとおりです。

.. image:: ../_static/52.png
    :align: center 


* There are four hips to assemble, all with different shapes. Here shows how to assemble the rear right hip. 臀部(でんぶ)は4個組み立てますが、全て部品の向きが異なります。右後ろの臀部の組立方法を紹介します。

Servo horn サーボホーン

* Insert a servo horn to a servo. サーボホーンを挿す。

.. image:: ../_static/38.jpg
    :align: center

Assemble servo horn and hip parts サーボホーンと臀部部品の組み立て

* Use an M2x6mm Tapping screw and an M2x6mm screw. You will need a long cross-head screwdriver and a 2 mm hexagonal wrench. M2x6mm(タッピング)とM2x6mmを使用します。長い十字ドライバーと2mmの六角レンチが必要です。

.. image:: ../_static/39.jpg
    :align: center

.. image:: ../_static/40.jpg
    :align: center

.. image:: ../_static/41.jpg
    :align: center  
    
Put two servos into hip parts サーボ2つを臀部部品に入れる。

※ You may need to clean the residue around the holes in the 3D printed part at first. Make sure the servo mounting surface is flat. 最初に、3Dプリントされたパーツの穴の周りの残留物をきれいにする必要があるかもしれません。サーボ取付面が平らであることを確認してください。


* Insert two servo into the box and fix them with M2x6mm screws. 2つのサーボを箱にはめて、M2x6mmのボルト4本で固定します。

.. image:: ../_static/42.jpg
    :align: center  
    
Assemble leg and hip 脚部を臀部に取り付ける

* Attach the leg to the hip using the M2x12mm screws. Leg is tilted at approximately 45°, as shown in the manual. M2x12mmのボルトを使って、脚を臀部に取り付けます。マニュアルの通り、脚がだいたい45度傾くように取り付けます。

.. image:: ../_static/43.jpg
    :align: center  
    
.. image:: ../_static/44.jpg
    :align: center  
      
* Tighten the screws with Loctite. Use a toothpick to apply Loctite to the servo's screw holes. ロックタイトでボルトをしっかりと固定しましょう。爪楊枝を使ってサーボの穴にロックタイトを塗っておきます。

.. image:: ../_static/45.jpg
    :align: center  
   
.. image:: ../_static/46.jpg
    :align: center 
    

Step 4.2 Four Hips
^^^^^^^^^^^^^^^^^^^^^

.. image:: ../_static/47.jpg
    :align: center 
    
    
5. Body Frame Assembly 
-----------------------

Tools
^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly. キットに同梱されている工具の他に、組み立てには以下の物が必要です。

* Screwdriver / プラスドライバー
* Superglue / 瞬間接着剤※
* Masking tape / マスキングテープ※

※ These are not essential. Use in case of trouble or when more strength is required. 必須ではありません。トラブル時やより強度を求める場合に使用します。

Bolt to use
^^^^^^^^^^^^^^^^^^^^^
* M2x8mm	4+4=8	 
* M3x8mm	2+2=4	
* M2x5mm	8+8+4=20

Step 5.1 Center parts
^^^^^^^^^^^^^^^^^^^^^

* The position of each servomotors are shown as below. 各サーボモータの位置は以下のとおりです。

.. image:: ../_static/52.png
    :align: center 

※ For the latest kit, there are two kinds of servo cables, No.1,4,7,10 cables length is 9cm, other cables length is 15cm. 最新のキットには、サーボケーブルが2種類あります。No.1、4、7、10のケーブル長は9cm、その他のケーブル長は15cmです。

* Use four M2x8mm screws. It is useful to put masking tape on the cables and write the number of servomotors during this process to make it easier later. M2x8mmのボルト4本を使って取り付けます。この工程でケーブルにマスキングテープを貼り番号を書くと、後で楽です。

.. image:: ../_static/48.jpg
    :align: center 
    
.. image:: ../_static/49.jpg
    :align: center 

.. image:: ../_static/50.jpg
    :align: center 
    
.. image:: ../_static/51.jpg
    :align: center 

Step 5.2 Front parts
^^^^^^^^^^^^^^^^^^^^^

* Tighten the two M3x8mm screws with a screwdriver. The front part is designed to hold the LCD screen. Make sure you don't mistake it for the rear part. M3x8mmの皿ネジ2本をプラスドライバーで締めます。前面パーツは液晶画面が入る形になっています。後部パーツと間違えないようにしましょう。

.. image:: ../_static/53.jpg
    :align: center 
    
.. image:: ../_static/54.jpg
    :align: center 


Step 5.3 Rear side
^^^^^^^^^^^^^^^^^^^^^

* The same procedure as for the front part. 前部と同じ要領です。

.. image:: ../_static/55.jpg
    :align: center 
    
.. image:: ../_static/56.jpg
    :align: center 

.. image:: ../_static/57.jpg
    :align: center 
    
.. image:: ../_static/58.jpg
    :align: center 
    
.. image:: ../_static/59.jpg
    :align: center 
    
.. image:: ../_static/60.jpg
    :align: center 


Step 5.4 Bottom plate
^^^^^^^^^^^^^^^^^^^^^

* Use eight M2x5mm screws. The orientation of the plate must be such that the hole is at the front. M2x5mmのボルトを8本使用します。プレートの向きは、写真のように、前の方に穴が来る必要があります。

.. image:: ../_static/61.png
    :align: center 
    
.. image:: ../_static/62.jpg
    :align: center 
    
Step 5.5 Top plate and supports
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Use four M2x5mm screws and four short supports. M2x5mmのボルト4本と短い支柱4本を使用します。
    
.. image:: ../_static/63.jpg
    :align: center 
    
.. image:: ../_static/64.jpg
    :align: center 

    
Step 5.6 Top plate
^^^^^^^^^^^^^^^^^^^^^

* Use eight M2x5mm screws. The orientation of the plate must be such that the large opening is at the front. M2x5mmのボルトを8本使用します。プレートの向きは、写真のように、前の方に大きな開口部が来る必要があります。

.. image:: ../_static/65.jpg
    :align: center 
    
.. image:: ../_static/66.jpg
    :align: center 
    
.. image:: ../_static/67.jpg
    :align: center 

6. Assemble the function component
----------------------------------

Tools
^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly. キットに同梱されている工具の他に、組み立てには以下の物が必要です。

* Screwdriver プラスドライバー

Bolt to use
^^^^^^^^^^^^^^^^^^^^^

* M2x5mm	2
* M2x8mm	2
* M1.4x3mm(皿)  4

Step 6.1 Display 画面
^^^^^^^^^^^^^^^^^^^^^

* Use two M2x5mm screws. Remove the protective sheet for the display. Fold the thin flexible cable at the edge of the display. Attach the board and the display to the main unit. When attaching the display, you can use a stick to gently push the flexible cable, so that it goes as far back as possible. M2x5mmのボルト2本を使用します。ディスプレイの保護シールはここで取りましょう。ディスプレイと専用基板の間に通る薄いフレキシブルケーブル(通称フレキ)をディスプレイの端で折ります。基板、ディスプレイの順に本体に取り付けます。ディスプレイを取り付ける際に、フレキがなるべく奥にいくように棒状の物で軽く押すと良いです。


.. image:: ../_static/72.jpg
    :align: center 
    
.. image:: ../_static/73.jpg
    :align: center 
    
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
    
Step 6.2 Frame of face 
^^^^^^^^^^^^^^^^^^^^^^^

* Use four M1.4x3mm countersunk screws. Be careful with the yellow parts as it has a front and back. M1.4x3mmの皿ネジを4本使用します。黄色いパーツには表裏の区別があるので気をつけましょう。

.. image:: ../_static/79.jpg
    :align: center 
    
.. image:: ../_static/80.jpg
    :align: center 
    
.. image:: ../_static/81.jpg
    :align: center 

Step 6.3 Battery 
^^^^^^^^^^^^^^^^^^^^^

* If you DIY the battery, please ensure our battery spec at first, especially the Voltage should be less than 7.4V, you can also refer to other backers work https://www.facebook.com/groups/716473723088464/posts/777616293640873/ 


* Install the battery pack. Be careful of the front and rear orientation. Fit the battery from the bottom to the top, then slide it backwards and secure it. Pass the cable through the hole in the bottom plate and bring it up to the top. バッテリーパックを取り付けます。前後の向きに気をつけましょう。底からバッテリーを上にはめて、後ろにぐっとずらし固定します。ケーブルを底のプレートの穴に通し、上まで持ってきます。

.. image:: ../_static/82.jpg
    :align: center 
    
.. image:: ../_static/83.jpg
    :align: center 
    
.. image:: ../_static/84.jpg
    :align: center 
    
.. image:: ../_static/85.jpg
    :align: center 
    
.. image:: ../_static/86.jpg
    :align: center 
    
.. image:: ../_static/87.jpg
    :align: center 
    
Step 6.4 Custom circuit board 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Use four long supports. First, plug the display cable into the custom circuit board. Then, plug in the battery cable. This connector may interfere with the hips parts, so you have to slide it through a hole in the middle of the board as temporary solution. Next, you need to insert the 12 servo cables. In the picture, you can see: J1,J2,J3.... . J12. After inserting the 12 cables, pull the custom circuit board closer to the body. The board may float, but you can use four long posts to hold it in place. 長い支柱4本を使用します。最初にディスプレイのケーブルをカスタム回路基板に挿します。次にバッテリーのケーブルを挿します。このコネクタが臀部パーツに干渉する恐れがあるので、（暫定対策として）このコネクタを基板の真ん中の穴に通して逃しておきます。次にサーボのケーブルを12本挿します。写真で説明すると、J1,J2,J3...J12順番の通りに挿していきます。茶色がGNDなので全て手前になるように挿しましょう。12本のケーブルを挿したらカスタム回路基板をぐっと力を入れてボティに近づけます。ケーブルの反発で基板が浮いてきますが、長い支柱を4本挿して固定しましょう。
    
.. image:: ../_static/88.jpg
    :align: center 
    
.. image:: ../_static/89.jpg
    :align: center 
    
.. image:: ../_static/90.jpg
    :align: center 
    
.. image:: ../_static/91.jpg
    :align: center 
    
.. image:: ../_static/92.jpg
    :align: center 
    
.. image:: ../_static/93.jpg
    :align: center 
    
.. image:: ../_static/94.jpg
    :align: center 
    
.. image:: ../_static/95.jpg
    :align: center 


※ Need to pay attention to the cable of the No. 1 servo to prevent it from being overwhelmed. 
※ No.1サーボのケーブルに圧倒されないように注意する必要があります。

.. image:: ../_static/134.png
    :align: center


Step 6.5 Fan 
^^^^^^^^^^^^^^^^^^^^^

* Use two M2x8mm screws. To install the fan. M2x8mmのボルト2本を使用します。ファンを取り付けます。

.. image:: ../_static/157.jpg
    :align: center 
    
.. image:: ../_static/159.jpg
    :align: center 
    
.. image:: ../_static/158.jpg
    :align: center 

Step 6.6 Raspberry Pi 4
^^^^^^^^^^^^^^^^^^^^^^^^
    
.. image:: ../_static/96.jpg
    :align: center 
    
.. image:: ../_static/97.jpg
    :align: center 
    
.. image:: ../_static/98.jpg
    :align: center 
    
.. image:: ../_static/99.jpg
    :align: center 

   
7. Cover Assembly
-----------------

Tools 工具
^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly. キットに同梱されている工具の他に、組み立てには以下の物が必要です。

* Screwdriver / プラスドライバー

Bolt to use 使用するボルト
^^^^^^^^^^^^^^^^^^^^^
* M1.4x3mm	4x2=8	 
* M2x4mm	2x4=8	
* M2x10mm	4+4=8

Step 7.1 Side panels
^^^^^^^^^^^^^^^^^^^^^

* Use eight M1.4x3mm countersunk screws. M1.4x3mmの皿ネジを8本使用します。
    
.. image:: ../_static/111.jpg
    :align: center   
    
.. image:: ../_static/112.jpg
    :align: center   

Step 7.2 Shin guards
^^^^^^^^^^^^^^^^^^^^^

* Use four M2x10mm countersunk screws. M2x10mmのボルトを4本使用します。

.. image:: ../_static/113.jpg
    :align: center   
    
.. image:: ../_static/114.jpg
    :align: center 

Step 7.3 Shoulders 肩
^^^^^^^^^^^^^^^^^^^^^ 

* Use 8 x M2x4mm screws. Insert only the screws first and then insert the shoulder parts into the gap. Insert the 2 mm hex driver into the hole in the shoulder part and tighten the screws. M2x4mmボルトを8本使用します。先にボルトだけ挿し、その隙間に肩パーツを差し込みます。肩パーツの穴に2mm六角レンチを入れてボルトを締めます。

.. image:: ../_static/115.jpg
    :align: center   
    
.. image:: ../_static/116.jpg
    :align: center   
    
.. image:: ../_static/117.jpg
    :align: center   
    
.. image:: ../_static/118.jpg
    :align: center   
    
Step 7.4 Top cover
^^^^^^^^^^^^^^^^^^^^^   

* Use four M2x10mm screws; if the holes are too small to fit the screws, as the part is made with a 3D printer, you can enlarge the holes by turning them with the supplied 2mm hexagonal screwdriver. M2x10mmボルトを4本使用します。3Dプリンタで作られたパーツなので、穴が小さくボルトが入らない場合は、付属の2mm六角ドライバでグリグリと回して穴を大きくしましょう。

.. image:: ../_static/119.jpg
    :align: center   
    
.. image:: ../_static/120.jpg
    :align: center   
    
.. image:: ../_static/121.jpg
    :align: center   
    
Step 7.5 Shoes
^^^^^^^^^^^^^^^^^^^^^  

* Put on 4 shoes. 靴を4つ履く

.. image:: ../_static/122.jpg
    :align: center   
    
.. image:: ../_static/123.jpg
    :align: center   
    
    
Step 7.6 Completion!   
^^^^^^^^^^^^^^^^^^^^^  

.. image:: ../_static/124.jpg
    :align: center   

.. image:: ../_static/125.jpg
    :align: center   
    
