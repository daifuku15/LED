# Pi でデバイスドライバを使用したGPIO操作によるLEDの点滅
#LED点滅
echo 0 > /dev/myled0 → LEDを消灯
echo 1 > /dev/myled0 → LEDを点灯
デモ　→　https://youtu.be/
#Dependency
C
#Setup
ハードウェア：Rasberry Pi 3 Model B V1.2
ソフトウェア：Raspbian　3.2.1
#Usage
Rasberry Piの2２番ピンと３９番ピンにLEDを接続
myled.c を　makefile でコンパイルする
sudo insmod myled.ko
sudo chmod 666 /dev/myled0
echo 0 > /dev/myled0 → LEDを消灯
echo 1 > /dev/myled0 → LEDを点灯
<終了時のみ>
sudo rm /dev/myled0
sudo rmmod myled
#License
This software is released under the MIT License, see LICENSE.
#References
https://github.com/ryuichiueda/robosys2019.git
