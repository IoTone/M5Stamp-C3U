## This is an example project for M5Stamp C3U on PlatformIO

Project forked to explore how to use this board.   

- [x] Setup things with Arduino IDE 1.8.19, boards and lib. 
- [x] Understand how to communicate with I2C,  
Check [I2Cscan branch](https://github.com/nicolasdb/M5Stamp-C3U/tree/I2Cscan)
- [x] Play with a Oled .096 display and the ~~ENV unit~~ DHT11,  
Check [OledDHT11 branch](https://github.com/nicolasdb/M5Stamp-C3U/tree/OledDHT11)
- [x] Then go back to setup the board in platform.io,  
Here on Master branch.


----

### Notes:
Pay attention to the model you have.  
- C3 need a FTDI driver  
- C3U doesn't but need to be in program download mode.

For more stuff, check the [issue #1](https://github.com/nicolasdb/M5Stamp-C3U/issues/1)

#### - To use with Arduino IDE
[https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html#installing-using-arduino-ide](https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html#installing-using-arduino-ide)

#### - To use with Platform.io

Clone this repo, everything is adjusted in `platformio.ini`  
Just build and upload

#### - Test program
`main.cpp` : Internal led will change its color with each press on the button.

> For ARDUINO IDE: You can copy/paste the code from `main.cpp` Don't forget to install libraries. 

#### - To enter into "program download" mode operation:

- Long press the center button (G9) of STAMP C3U under power failure condition.
- Connect USB to the computer while holding the button, 

after that, the port is successfully identified, program burning.

> Windows 10, Arduino IDE
![image](https://user-images.githubusercontent.com/12049360/185742555-b4190a52-7720-4787-beb9-55e36e271cf4.png)

> Manjaro kernel 5.15 LTS, Arduino IDE
![image](https://user-images.githubusercontent.com/12049360/189372496-20315b99-53ec-4071-b5c7-1e33a9ff0d8e.png)
