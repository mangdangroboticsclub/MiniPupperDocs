=================
Robot operation 「ミニぷぱ」 操作
=================

Running the robot ミニぷぱ（以下、本体）を起動
-----------------
1. Power On Mini Pupper 電源オン
    
    * Push on the power button for at least 3 seconds on the battery to power on Mini Pupper. After power on, if you push on the power button for at least 3 seconds again, it will power off. 

.. image:: ../_static/127.gif
    :align: center
        
2. Connect the PS4 controller to the Pi by putting it pairing mode. コントローラーをペアリングモードにしてRaspberry Piに接続します。
    
    * To put it into pairing mode, hold the share button and circular Playstation button at the same time until it starts making quick double flashes. ペアリングモードにするには、「SHARE」ボタンと中央のPSボタンを同時に3秒以上長押しします。その後、ライトが2回点滅し始めます。
    * If it starts making slow single flashes, hold the Playstation button down until it stops blinking and try again. もし、ゆっくりと1回点滅し始めた場合、点滅が止まるまでPSボタンを押し続けて、もう一度やり直してください。
    
.. image:: ../_static/128.gif
    :align: center
        

3. Wait until the controller binds to the robot, at which point the controller should turn a dim green (or whatever color you chose in pupper/HardwareConfig.py for the deactivated color). コントローラーが本体に接続されるまで待ちます。
4. Press L1 on the controller to "activate" the robot. The controller should turn bright green (or again, whatever you chose in HardwareConfig). コントローラーのL1を押して、本体を「アクティブ化」します。 ここでコントローラーライトは明るい緑色に変わります。
5. You're good to go! Check out the controls section below for operating instructions. 上記で準備が完了です。操作手順については、以下の制御セクションを確認してください。

Robot controls 本体の制御
---------------

* L1: Press to toggle active mode and deactivate mode. L1を押し、アクティブモードと非アクティブモードに切り替えます。
    
    * Note: the PS4 controller's front light will change colors to indicate if the robot is deactivated or activated. コントローラーのライトは、本体がアクティブ化されているか、されていないかを示すために色が変わります。
    
* R1: Press to transition between Rest mode and Trot mode. R1を押して、レストモードとトロットモードに切り替えます。  

.. image:: ../_static/129.gif
    :align: center
    


* Left joystick　左スティック

    * Forward/back　前進/後退: moves the robot forward/backwards when in Trot mode. トロットモード時、本体を前進/後退させます
    * Left/right 左/右: moves the robot left/right when in Trot mode. トロットモード時、本体を左/右に動かします。
    
.. image:: ../_static/130.gif
    :align: center
        
    
* Right joystick 右スティック
    
    * Forward/back 前方/後方: pitches the robot forward and backward. 本体を前方および後方にピッチングします。
    * Left/right 左/右: turns the robot left and right. 本体を左右に回転させます。
    
.. image:: ../_static/131.gif
    :align: center    
    
* D-Pad 十字キー
    * Forward/back 前後: raises and lowers the body. 体を上げ下げします。
    * Left/rights 左/右: rolls the body left/right. 体を左/右に回転させます。
    
.. image:: ../_static/132.gif
    :align: center      
    
* "X" button 「X」ボタン: Press it three times to complete a full hop. 3回押すと、ジャンプします。

* Power off  電源オフ

.. image:: ../_static/133.gif
    :align: center

Important Notes 注意事項
---------------

* PS4 controller pairing instructions (repeat of instructions above) コントローラーのペアリング手順（上記の手順の繰り返し）
    
    * To put it into pairing mode, hold the share button and circular Playstation button at the same time until it starts making quick double flashes. ペアリングモードにするには、「SHARE」ボタンと中央のPSボタンを同時に押し続けます。その後、ライトが2回点滅し始めます。 
    * If it starts making slow single flashes, hold the Playstation button down until it stops blinking and try again. もし、ゆっくりと1回点滅し始めた場合、点滅が止まるまでPSボタンを押し続けて、もう一度やり直してください。

* Battery voltage バッテリー電圧
    
    * If you power the robot with anything higher than 8.4V (aka >2S) you'll almost certainly fry all your expensive servos! 8.4V（別名> 2S）を超えるものでロボットに電力を供給すると、すべての高価なサーボが壊れてしまう可能性が高くなります。
    * Please note that a lipo battery alarm is attached to the battery to indicate that the battery is exhausted when starting the robot. 本体を起動する際、バッテリーが消耗したことを提示するため、バッテリーにリポバッテリーアラームを取り付けているので、ご注意ください。
    * Also note that you should attach a lipo battery alarm to your battery when running the robot so that you are know when the battery is depleted. Discharging your battery too much runs the risk of starting a fire, especially if you try to charge it again after it's been completely discharged. A good rule-of-thumb for know when a lipo is discharged is checking whether the individual cell voltages are below 3.6V. 完全に放電した後、再度充電する際など、バッテリーの放電が多すぎると、火災が発生する危険性があります。バッテリーがいつ放電されるかを知るための経験則は、個々のセル電圧が3.6V未満であるかどうかをチェックすることです。
    * The robot will walk much more poorly when the battery is mostly discharged since a lower voltage is going to the motors. また、モーターへの電圧が低くなるため、バッテリーが大概放電していると、ロボットの歩行が鈍くなります。
