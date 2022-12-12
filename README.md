# RUMTemperature

ESP32’s equipped with Temperature sensors are to be placed in several rooms in
the Buildings across the University of Mayaguez Campus.

The devices send continuous measurements to Node Red via MQTT to a AWS LightSail server which
the user can access the data by via Apple's "Siri" or through our website.

The user has to download PlatformIO extension in visual studio code.
In Projects one must specify that the board is an Espressif ESP-Wrover Kit.
PlatformIO libraries to download:
  - Wrover Kit library
  - PubSub library
  
Afterwards build and download the project to the user's ESP32.

Users must install Shortcuts on their Apple device and use the following shortcut:
https://www.icloud.com/shortcuts/5386f90c8d2144149915f5a5ef6e1836

To use Siri the user must say: "Siri, college air conditioner status". Siri will 
ask the user for the specific room, in which case the user should say "Room XYZ" (XYZ=room number).

Additionally, if the server is running, the user may see the temperature value by connecting to this website:
http://rumtemperature.com:1880/ui
