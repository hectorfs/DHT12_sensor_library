This is an Arduino and esp8266 library for the DHT12 series of very low cost temperature/humidity sensors (less than 1$).

Tutorial: 

To download. click the DOWNLOADS button in the top right corner, rename the uncompressed folder DHT12. Check that the DHT folder contains DHT12.cpp and DHT12.h. Place the DHT library folder your <arduinosketchfolder>/libraries/ folder. You may need to create the libraries subfolder if its your first library. Restart the IDE.

# Reef complete DHT12 Humidity & Temperature

This libray try to emulate the behaivor of standard DHT library sensors (and copy a lot of code), and I add the code to manage
i2c olso in the same manner.

The method is the same of DHT library sensor, with some adding like dew point function.

To use with wire the constructor is:
DHT12 dht12;
and take the default value for SDA SCL pin. (It's possible to redefine with specified contructor for esp8266 but is not the
best way).
or
DHT12 dht12(uint8_t addressOrPin, false)
to change address.

To use one wire:
DHT12 dht12(uint8_t addressOrPin, true)
addressOrPin -> pin.

With examples, there are the connection diagram, it's important to use correct pullup resistor.

Thanks to Bobadas, dplasa and adafruit, to share the code in github (where I take some code and ideas).

DHT12 PIN
![DHT12 Pin](http://lmsotfy.com/so.png) 

DHT12 connection schema