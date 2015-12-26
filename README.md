# ota-basic
OTA basic example for esp8266

This sketch makes esp8266 to be updateable via OTA. Aditionally, it makes a led blink on pin 2 to check that the esp8266 is running.
The esp8266 can be reprogramed even without a flashing circuit.

#Contents
  * Prerequisites
  * Installing software with Boards Manager
  * Using git version
  * Using stable version with PlatformIO
  * Documentation
  * Issues and support
  * Contributing
  * License and credits

#Prerequisites:
To use this sketch you need:
  - An esp8266 board
  - Arduino software 1.6.7 or later [Download here](https://www.arduino.cc/en/Main/Software)

#Installing software with Boards Manager
After installing Arduino Software (1.6.7 version or later) we’ll need to update the board manager with a custom URL.
Open up Arduino, then go to the Preferences (**File > Preferences**). Then, towards the bottom of the window, copy this URL into the “Additional Board Manager URLs” text box:
  http://arduino.esp8266.com/stable/package_esp8266com_index.json

![Arduino Settings IMG](./img/arduino-board-manager-link.png?raw=true "Add Board Manager URL")




To begin, we’ll need to update the board manager with a custom URL. Open up Arduino, then go to the Preferences (File > Preferences). Then, towards the bottom of the window, copy this URL into the “Additional Board Manager URLs” text box:

COPY CODEhttp://arduino.esp8266.com/stable/package_esp8266com_index.json
If you already have a URL in there, and want to keep it, you can separate multiple URLs by placing a comma between them. (Arduino 1.6.5 added an expanded text box, separate links in here by line.)

Adding Board Manager URL to Arduino preferences



#Install Arduino software from the Arduino website.
Start Arduino and open Preferences window.
Enter http://arduino.esp8266.com/stable/package_esp8266com_index.json into Additional Board Manager URLs field. You can add multiple URLs, separating them with commas.
Open Boards Manager from Tools > Board menu and install esp8266 platform (and don't forget to select your ESP8266 board from Tools > Board menu after installation).
