# Code collection for AZ-Touch-Feather
A collection of different demo sources for Zihatec [AZ-Touch Feather wall mount touchscreen kit](https://www.hwhardsoft.de/english/projects/az-touch-feather/)

![My image](https://user-images.githubusercontent.com/3049858/116822654-38ada600-ab80-11eb-9d09-22b8a9e6d055.png)


## Used pins

![My image](https://user-images.githubusercontent.com/3049858/116822653-36e3e280-ab80-11eb-96f6-3615512153ef.png)

Please note: For HuzzahESP8266 the Beeper is on xx and the TFT_LED pin is not in use.


## Migration of AZ-Touch ESP projects

Existing projects for AZ-Touch ESP or MOD for ESP32 or ESP8266 can be migrated to AZ-Touch Feather and ESP32 or ESP8266 based Feather boards very simple.

For ESP32 please use the following pin definitions:

bash'''
#define TFT_CS   33
#define TFT_DC   15
#define TFT_LED  13
#define TOUCH_CS 32
#define TOUCH_IRQ 14 
#define BEEPER 27
'''



For ESP8266 please use the following pin definitions:

bash'''
#define TFT_CS   15
#define TFT_DC   0
#define TOUCH_CS 16
#define TOUCH_IRQ 2 
#define BEEPER 5
'''

Remove the TFT_LED control from your project for ESP8266. (The TFT backlight will be always on). 
