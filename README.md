Arduino STM32用 SH1106コントローラ使用 OLEDドライバライブラリ  

このライブラリは、下記の公開ライブラリを元にArduino STM32用対応しました.  
 - https://github.com/wonho-maker/Adafruit_SH1106  
 - https://github.com/rogerclarkmelbourne/Arduino_STM32/tree/master/STM32F1/libraries/Adafruit_SSD1306  

SPI、I2Cのインタフェースに対応しています.  

本ライブラリをArduino STM32安定版環境(R20170323)にて利用する場合は、  
Adafruit_SH1106_STM32.cpp 内の次の箇所の修正が必要です。

    #define OLD_ARDUINO_STM32 0  // Arduino STM32環境が R20170323:1、 それ以降 0

安定版にて利用する場合は、1を設定して下さい.  


以下、https://github.com/wonho-maker/Adafruit_SH1106  のREADMEの原文をそのまま掲載します.

---

Adafruit_SH1106
===============

Adafruit graphic library for SH1106 driver lcds.

some small oled lcd use SH1106 driver.

I change the adafruit SSD1306 to SH1106 

SH1106 driver similar to SSD1306. thus, just change the display() method. 
 
However, SH1106 driver don't provide several functions such as scroll commands.


 Adafruit-GFX-Library
 https://github.com/adafruit/Adafruit-GFX-Library




以下、https://github.com/rogerclarkmelbourne/Arduino_STM32/tree/master/STM32F1/libraries/Adafruit_SSD1306  
のREADMEの原文をそのまま掲載します.  

---

This is a library for our Monochrome OLEDs based on SSD1306 drivers  

  Pick one up today in the adafruit shop!  
  ------> http://www.adafruit.com/category/63_98  

These displays use SPI to communicate, 4 or 5 pins are required to  
interface  

Adafruit invests time and resources providing this open source code,   
please support Adafruit and open-source hardware by purchasing  
products from Adafruit!  

Written by Limor Fried/Ladyada  for Adafruit Industries.  
Scrolling code contributed by Michael Gregg  
BSD license, check license.txt for more information  
All text above must be included in any redistribution  

To download. click the DOWNLOADS button in the top right corner, rename the uncompressed folder Adafruit_SSD1306. Check that the Adafruit_SSD1306 folder contains Adafruit_SSD1306.cpp and Adafruit_SSD1306.h  

Place the Adafruit_SSD1306 library folder your <arduinosketchfolder>/libraries/ folder. You may need to create the libraries subfolder if its your first library. Restart the IDE.  

You will also have to download the Adafruit GFX Graphics core which does all the circles, text, rectangles, etc. You can get it from
https://github.com/adafruit/Adafruit-GFX-Library  
and download/install that library as well  
