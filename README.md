WeatherClient
=============

A simple sketch that displays the current weather conditions according to worldweatheronline.net
on an LCD.

## Configuration

You'll need to update five values in src/WeatherClient.ino so they make sense for your environment:

 * WLAN\_SSID     - Your network name
 * WLAN\_PASS     - Password to your network
 * WLAN\_SECURITY - One of: WLAN\_SEC\_WPA, WLAN\_SEC\_WPA2, WLAN\_SEC\_WEP, or WLAN\_SEC\_UNSEC
 * API\_KEY       - Your free API key from worldweatheronline.net
 * CITY           - Either your city and province, or your postal code. Must be URL encoded.

## Parts

 * 1 x [Arduino UNO](https://www.sparkfun.com/products/retired/9950)
 * 1 x [Adafruit CC3000 Shield](http://www.bc-robotics.com/shop/adafruit-cc3000-wifi-shield/)
 * 1 x [16x2 LCD](https://www.sparkfun.com/products/709)
 * 1 x 3.3 k&#8486; resistor
 * 2 x 47&#8486; resistors

## Wiring

The CC3000 shield uses the following connections:

 * SCK      -> Digital pin 13
 * MISO     -> Digital pin 12
 * MOSI     -> Digital pin 11
 * WCS      -> Digital pin 10
 * VBAT\_EN -> Digital pin 5
 * CCS      -> Digital pin 4
 * IRQ      -> Digital pin 3


The LCD is connected as follows:

 * LCD1  -> GND
 * LCD2  -> 5v
 * LCD3  -> 3.3 k&#8486; resistor -> GND
 * LCD4  -> Analog 0 (a.k.a digital pin 14)
 * LCD5  -> GND
 * LCD6  -> Digital pin 2
 * LCD11 -> Digital pin 6
 * LCD12 -> Digital pin 7
 * LCD13 -> Digital pin 8
 * LCD14 -> Digital pin 9
 * LCD15 -> 5v
 * LCD16 -> 47&#8486; resistor -> 47&#8486; resistor -> GRD

## Final Result

![Today's Weather](http://i.imgur.com/P8aqZpB.jpg)
