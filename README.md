# persona-rm
Persona styled rainmeter widget

## Preview
<img width="806" height="349" alt="image" src="https://github.com/user-attachments/assets/b5083450-1462-4557-8e54-0c835fbab369" />

## Description
A persona themed widget collection to display date, time of the day, day, and weather icons that update in real time.

This is technically multiple rainmeter skins bundled into one, and as such you will have to place each one of the widgets (skins) based on your screen coordinates manually. The color for each widget can be changed individually by clicking on the widgets (thanks to [RainRGB4](https://forum.rainmeter.net/viewtopic.php?t=6215)) or by editing the `@Resources\Variables.inc` (`@Resources\Config.inc` for weather skin)

## Installation

### Prerequisites
Make sure to have [Rainmeter](https://www.rainmeter.net/) installed on your system.

**OPTIONAL** - *ignore this if you do not need weather widget*

You will also need an account on [OpenWeatherMap](https://openweathermap.org) to setup weather display as per your location.


### Setup
1. Download the latest .rmskin package from the Releases tab on GitHub page and install via Rainmeter
     - You can uncheck 'Apply included layout' to arrange the widgets yourself
2. To setup Weather widget, you need to go to installation directory of the skin `default: C:\Users\<username>\Documents\Rainmeter\Skins`
3. Once inside go to the newly created Persona folder and into @Resources
4. Here create a new file with the name `Config.inc` with the following structure


   ```
   [Variables]
   ; Get your location from openweathermap.com
   Location=<your_location>

   ; As well as your API key by registering
   ApiKey=<your_api_key>

   ; You may choose your own r,g,b values here
   WeatherColor=79,163,253
   ```

   - You can generate your API key from open weather map by clicking on your username -> My API Keys
   - Search for your city in the search bar and from the results use the {city},{state},{country} **without any spaces between** as <your_location> in config
5. Refresh Rainmeter to reload the weather skin


## TODO
- Expose more customization options (size, font size, alignment, rotation)
- Better variable handling (for weather widget)
- ... and things i cannot remember








