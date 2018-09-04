# ESP8266 Weather Station Color

ESP8266 Weather Station Color using ILI9341 240x320 TFT display

## Hardware Requirements

The code in this project supports an ILI9341 480x320 TFT display with code running on an ESP8266. 

## Licensing, contributions and maintenance

The code in this repository is licensed under [MIT](https://en.wikipedia.org/wiki/MIT_License), a short and simple permissive license with conditions only requiring preservation of copyright and license notices. Thus, you're free to fork the project and use the code for your own projects as long as you keep the copyright notices in place.


## Wiring

The below wiring diagram is only needed when you do _not_ buy the self-contained kit from ThingPulse but rather assemble the components yourself.

![Wiring](resources/PlaneSpotterWiring.png)

| Wemos D1 Mini | ILI9341      |
| ------------- |:-------------:|
| D4            | T_IRQ         |
| D6            | T_DO          |
| D7            | T_DIN         |
| D3            | T_CS          |
| D5            | T_CLK         |
| D6            | SDO           |
| D8            | LED           |
| D5            | SCK           |
| D7            | SDI           |
| D2            | D/C           |
| RST           | RESET         |
| D1            | CS            |
| GND           | GND           |
| 3V3           | VCC           |


## Changes 

I removed the hard-coded WiFi code and replaced with the wonderful WiFi Manager to make it portable and relocatable: https://github.com/tzapu/WiFiManager

I changed the design from a hard-coded geo location to an automated geolocation based on your ISP IP address. This is a plug-and-play solution. Once you have connected to your home wifi, it will go out and find your geolocation and get weather info for your local area.
