
# ESP8266 Weather Station

based on the work by [Daniel Eichhorn - Thingpulse](https://github.com/ThingPulse/esp8266-weather-station)

This fork is changed for our [AZ-Touch Feather kit](https://www.hwhardsoft.de/english/projects/az-touch-feather/) equipped with [Adafruit HUZZAH ESP8266](https://www.adafruit.com/product/2821) 

![My image](https://user-images.githubusercontent.com/3049858/93122689-3ff27300-f6c7-11ea-8985-9fe069cd710f.jpg)


## Libraries

Install the following libraries through Arduino Library Manager

[Mini Grafx by Daniel Eichhorn](https://github.com/ThingPulse/minigrafx)

[Json Streaming Parser by Daniel Eichhorn](https://github.com/squix78/json-streaming-parser/blob/master/library.properties)

[simpleDSTadjust by neptune2](https://github.com/neptune2/simpleDSTadjust)

[ESP8266 WeatherStation by Daniel Eichhorn](https://github.com/ThingPulse/esp8266-weather-station)

You can download the library also directly as ZIP file and uncompress the folder under yourarduinosketchfolder/libraries/   

After installing the libraries, restart the Arduino IDE. 


## Settings WiFi

Open the file settings.h in the Arduino IDE and enter your WiFi SSID & password in the fields in the WiFi section: 

```bash
#define WIFI_SSID "your ssid"
#define WIFI_PASS "your password"
```


## Settings OpenWeatherMap

Account for OpenWeatherMap: To receive later data by the platform OpenWeatherMap you will need an own account. Sign up here to get an API key: https://docs.thingpulse.com/how-tos/openweathermap-key/

Enter your API key in line 38 of settings.h

```bash
String OPEN_WEATHER_MAP_APP_ID = "your_api_key";
```

Your location: Go to https://openweathermap.org/find?q= and search for a location. Go through theresult set and select the entry closest to the actual location you want to display data for. It'll be a URL like https://openweathermap.org/city/2657896. The number at the end is what you assign to the constant below. Enter the number and name of your location in line 45 and 46 of settings.h

```bash
String OPEN_WEATHER_MAP_LOCATION_ID = "2804279";
String DISPLAYED_CITY_NAME = "Ziesar";
```


## Settings Time

Please choose your timezone in line 65 of settings.h

```bash
#define UTC_OFFSET +1
```


## License

This library is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
Lesser General Public License for more details.
