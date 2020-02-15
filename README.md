# Sith GPS Tracker
Sith GPS and wearable device tracker

## Hardware
- [Adafruit Ultimate GPS FeatherWing](https://www.adafruit.com/product/3133)
- [Adafruit Feather M4](https://www.adafruit.com/product/3857)
- [SMA to uFL/u.FL/IPX/IPEX RF Adapter Cable](https://www.adafruit.com/product/851)
- [GPS Antenna - External Active Antenna - 3-5V 28dB 5 Meter SMA](https://www.adafruit.com/product/960)
- Arduino Uno

![](https://github.com/AmieDD/Sith-GPS-Tracker/blob/master/Images/2020-02-15_Disney.png)

## GPS
Global Positioning System (GPS) is a way to naivated based on satelites.  The U.S. Department of Defense (USDOD) orginally put up satellites in orbit for military use and then made public for normal civilian use in the 1980's. There are 24 satlieetes that work in any anywhere in the world 24/7 and has no fees or charges. 

## NMEA Data from GPS 
National Marine Electronics Association (NMEA) is the format that defines how GPS data is transmitted between devices. Most of my research uses the GPS receiver output data in the NMEA format.

$GPGGA
Global Positioning System Fix Data



NMEA Header | Value | Description
------------ | ------------- | ------
StartCharacter | $ | ASCII 36
SentenceName | GPGGA | NMEA Sentence ID
Separator | , | ASCII 44
Data_1 to Data_N | 083445.00, 1256.60109, N | Data fields longitude and latitude
CheckCharacter | * | ASCI 42
CheckSum | 7E | Hexadecimal 8bit or all characters between $ and *
EndCharacter | CR LF | Carriage return line
