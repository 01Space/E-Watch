E-Watch

Firmware fully compatible with  Watchy v1.0

Arduino Setup#
Watchy comes pre-loaded with firmware that demonstrates all the basic features. You can also try different watch faces and examples in Arduino.

1.Download and install the latest Arduino IDE

2.Start Arduino and open the Preferences window.

3.Under Additional Board Manager URLs add:

https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json

4.Open Boards Manager under Tools > Board menu and install the latest version of esp32 platform

5.Under Sketch > Include Library > Manage Libraries, search for Watchy and install the latest version

6.Make sure all the dependencies are updated to the latest version i.e. GxEPD2 , WiFiManager, rtc_pcf8563,etc.

Upload#

1.Plug in the USB on Watchy and select the serial port that shows up

2.If nothing shows up, or if you're having trouble uploading, make sure you have the USB-Serial drivers installed. Also make sure you're using a USB data cable, and not a charge-only cable. Try different USB ports as well.

3.Select Tools > Board > ESP32 Arduino > Watchy

4.Select Tools > Board Revision > Watchy v1.0

5.Select Tools > Partition Scheme > Huge App

6.Leave everything else as default

7.Choose an example and click upload

8.Try modifiying the examples or create your own app!

Wi-Fi Setup#

1.Click 'Setup Wifi' from the main menu on the watch

2.Connect to 'Watchy AP' Wi-Fi from another device such as a phone or computer / laptop

3.If you're on a computer, go to 192.168.4.1 in your browser. On a phone, the captive portal should automatically open when connecting to Wi-Fi

4.Click 'Configure WiFi'

5.Enter the SSID and password of your network you want to connect to. (Note: SSID can be prefilled by listed networks on the top of this screen)

6.Hit 'Save' button and wait for Watchy to connect

7.If the connection fails, Watchy will display 'Setup failed & timed out!'. Otherwise, it will display the local IP address and SSID of the connected network with confirmation

Troubleshoot Wi-Fi Setup:#

1.Click 'Info' from 192.168.4.1 page

2.Check your router settings to make sure the listed mac address is allowed

3.If the above doesn't fix it, then try clicking 'Erase Wifi Config' from the 'Info' page and wait for Watchy to restart itself. Once that happens, try the Wi-Fi setup again

PlatformIO Setup#

PlatformIO is a compatible alternative to arduino. It's more oriented for the command line user, but it is also more flexible and predictable in build configurations and dependency management (like libraries).

It has two parts: a "core" that has the command line tools that build and upload/flash, and an "ide" which is a bunch of plugins and extensions for editors you can find here.

Use whichever extensions you wish but this documentation is related to the core, so:

Install with instructions here.
    
    
