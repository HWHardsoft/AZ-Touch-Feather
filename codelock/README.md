# Codelock Example

Simple Codelock / Keypad example for our [AZ-Touch Feather kit](https://www.hwhardsoft.de/english/projects/az-touch-feather/) 

![AZ-Touch Feather Codelock](https://user-images.githubusercontent.com/3049858/79955903-b58f4580-847f-11ea-8a44-0ffad80f72f7.jpg)


## compatible Feather boards

[Adafruit HUZZAH32](https://www.adafruit.com/product/3405)

[SparkFun Thing Plus - ESP32 WROOM boards](https://www.sparkfun.com/products/15663)

[SparkFun Thing Plus - ESP32 WROOM boards](https://www.sparkfun.com/products/15663)

[SparkFun Thing Plus - ESP32 WROOM boards](https://www.sparkfun.com/products/15663)



## Libraries

Install the following libraries through Arduino Library Manager

[Adafruit GFX Library](https://github.com/adafruit/Adafruit-GFX-Library/archive/master.zip)

[Adafruit ILI9341 Library](https://github.com/adafruit/Adafruit_ILI9341)

[Touchscreen by Paul Stoffregen](https://github.com/PaulStoffregen/XPT2046_Touchscreen/)


You can download the library also directly as ZIP file and uncompress the folder under yourarduinosketchfolder/libraries/   

After installing the libraries, restart the Arduino IDE. 


## Settings 

In the source code you can set the code number :: 

```bash
#define codenum 42
```

42 is the answer for everything, but you can change this to any number between 0 and 999999.


## License

This library is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
Lesser General Public License for more details.
