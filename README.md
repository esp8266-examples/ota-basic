# ota-basic
OTA basic example for esp8266

This sketch makes esp8266 to be updateable via OTA over WIFI. Aditionally, it makes a led blink on pin 2 to check that the esp8266 is running.
The esp8266 can be reprogramed even without a flashing circuit.

#Contents
  * [Prerequisites](#prerequisites)
  * [Installing software with Boards Manager](#installing-software-with-boards-manager)
  * [Flashing the esp8266 for the first time](#flashing-the-esp8266-for-the-first-time)
  * Issues and support
  * Contributing
  * License and credits



#Prerequisites:
To use this sketch you need:
  - An esp8266 board
  - Arduino software 1.6.7 or later [Download here](https://www.arduino.cc/en/Main/Software)
  - An esp8266 programmer (only to flash the esp8266 the first time)

#Installing software with Boards Manager
 * Install the Arduino Software (1.6.7 version or later)
 * Update Board Manager with custom URL:Open up Arduino, then go to the Preferences (**File > Preferences**). Then, towards the bottom of the window, copy this URL into the “Additional Board Manager URLs” text box:

  http://arduino.esp8266.com/stable/package_esp8266com_index.json

 <p align="center"><img src ="./img/arduino-board-manager-link.png?raw=true"></p>

 Note: You can add multiple URLs, separating them with commas.
 
 * Open Boards Manager from **Tools > Board** menu and install esp8266 platform (and don't forget to select your ESP8266 board from **Tools > Board** menu after installation).
 
 <p align="center"><img src ="./img/arduino-board-install.png?raw=true"></p>
 <p align="center"><img src ="./img/arduino-board-select.png?raw=true"></p>

#Flashing the esp8266 for the first time
To make the esp8266 OTA ready we need to flash de initial firmware with a esp8266 flashing circuit. For example:

 <p align="center"><img src ="./img/arduino-board-flashing.png?raw=true"></p>

You'll need to edit the sketch to set your WIFI configuration. Change the 'ssid' and 'password' value to match your FIFI settings:
 <p align="center"><img src ="./img/arduino-sketch-edit.png?raw=true"></p>

And set the configutarion of your programming circuit:
 - Board: If you don't know which is yours then select 'Generic ESP8266 module'
 - Port: The COM port of your programmer
 - Speed: 115200
 <p align="center"><img src ="./img/arduino-upload-speed.png?raw=true"></p>
