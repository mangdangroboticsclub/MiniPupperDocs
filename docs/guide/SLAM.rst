SLAM & Navigation  SLAM＆ナビゲーション
========

.. contents 目次:: :depth: 2

Software setup for the SLAM & Navigation functions. SLAM & Navigation機能のソフトウェアセットアップ。

1. Things to prepare 準備するもの
-------------

Tools 工具
^^^^^^^^^^^^^^^^^^^^^
In addition to the tools included in the kit, the following items are required for assembly. キットに同梱されている工具の他に、組み立てには以下の物が必要です。

* PC（OS：Ubuntu20.04）
* microSD card interface microSDカードリーダ  
* HDMI Display HDMI ディスプレイ 
* HDMI micro HDMI convertor HDMI⇔microHDMI変換 
* microUSB cable microUSB ケーブル 
* New SD card 新しいSDカード
* Wi-Fi(PC and MiniPupper must be on the same network) Wi-Fiの環境（PCとMiniPupperを同じネットワークにする必要ある）

2. Setup on the PC side PC側の環境セットアップ
-------------
Step 2.1 Download the image  イメージのダウンロード
^^^^^^^^^^^^^^^^^^^^^

* "MiniPupper2004.zip" is zip file of the image for the Ubuntu + ROS version for SLAM & Navigation. Download and unzip the zip file.「MiniPupper2004.zip」はSLAM＆NavigationのUbuntu + ROSバージョンのイメージのzipファイルです。ファイルをダウンロードして、解凍します。

  `MiniPupper2004.zip <https://drive.google.com/file/d/11zeivhN-fyTMdf6iuhcVD-Ib6aKj7s_5/view?usp=sharing>`_ 
  
Step 2.2 Write the image into microSD microSDにイメージを書く
^^^^^^^^^^^^^^^^^^^^^

Here we introduce the method of writing the image into microSD through Raspberry Pi's Imager. ここでは、RaspberryPiのImagerを使用してイメージをmicroSDに書き込む方法を紹介します。

* Install the Imager tool of the Raspberry Pi. RaspberryPiのImagerツールをインストール

    snap install rpi-imager
    
* Write the image into the new SD card.  新しいSDカードにイメージを書き込みます。
.. image:: ../_static/148.gif
    :align: center

Step 2.3 Install ROS noetic ROS noeticをインストールする
^^^^^^^^^^^^^^^^^^^^^

* You can skip this step if you have already installed ROS noetic. Basically you can follow the instructions on http://wiki.ros.org/noetic/Installation/Ubuntu. ROS noeticをすでにインストールしている場合は、この手順をスキップできます。基本的に、http://wiki.ros.org/noetic/Installation/Ubuntu の指示に従うことができます。

Step 2.4 Cartographer_ros environment setup Cartographer_rosの環境セットアップ
^^^^^^^^^^^^^^^^^^^^^

		cd ~
    
		sudo apt-get update
    
		sudo apt-get install -y python3-wstool python3-rosdep ninja-build stow
    
		mkdir carto_ws
    
		cd carto_ws
    
		wstool init src
    
		wstool merge -t src https://raw.githubusercontent.com/cartographer-project/cartographer_ros/master/cartographer_ros.rosinstall
    
		wstool update -t src
    
		sudo rosdep init
    
		rosdep update
    
		rosdep install --from-paths src --ignore-src --rosdistro=${ROS_DISTRO} -y
    
		src/cartographer/scripts/install_abseil.sh
    
		sudo apt-get remove ros-${ROS_DISTRO}-abseil-cpp
    
		catkin_make_isolated --install --use-ninja
    
		source install_isolated/setup.bash
    
Step 2.5 Compile the package for Mini Pupper ROS Mini Pupper ROS用のパッケージをコンパイル
^^^^^^^^^^^^^^^^^^^^

* Download the required package `mnpp_ws.zip <https://drive.google.com/file/d/1gbuvy29hNnS3Ep2o_uR8qAYnFKkr7Dj4/view?usp=sharing>`_  and unzip it to home. 必要なパッケージ `mnpp_ws.zip <https://drive.google.com/file/d/1gbuvy29hNnS3Ep2o_uR8qAYnFKkr7Dj4/view?usp=sharing>`_ をダウンロードして、homeに解凍します。

.. image:: ../_static/149.gif
    :align: center
    
* Compile the package. パッケージをコンパイルします。

		cd ~/mnpp_ws/
		
		sudo apt-get install libudev-dev
		
		rosdep install --from-paths src --ignore-src -r -y
		
		catkin_make
		
		source ~/mnpp_ws /devel/setup.bash
		

.. image:: ../_static/150.gif
    :align: center
    
Step 2.6 Network setup ネットワークのセットアップ
^^^^^^^^^^^^^^^^^^^^^

* Connect your PC and MiniPupper to the same WiFi and find the IP address assigned by the command ifconfig. PCとMiniPupperを同じWiFiに接続して、コマンドifconfigで割り当てられたIPアドレスを見つけます。

		ifconfig
	
* Open the bashrc file. bashrcファイルを開きます。
		
		sudo gedit ~/.bashrc

* Update the ROS IP settings with the following command to add the master and hostname configuration in the bashrc file. 以下のコマンドでROSのIP設定を更新して、マスターとホスト名の構成をbashrcファイルに追加します。

		export ROS_MASTER_URI=http://192.168.1.7:11311
		
		export ROS_HOSTNAME=192.168.1.7
		
		source ~/carto_ws/install_isolated/setup.bash
		
		source ~/mnpp_ws/devel/setup.bash

* Source the .bashrc file. 

		source ~/.bashrc
		
.. image:: ../_static/151.gif
    :align: center
