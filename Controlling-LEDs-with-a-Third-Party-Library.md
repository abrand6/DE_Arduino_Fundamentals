Whilst you can certainly build a wide variety of projects using the built-in resources provided by the Arduino platform, you will likely want to take advantage of the open source community's contributions. This most frequently is encountered by wanting to use a specific electronic component and its accompanying code library to make it easier to use.

As an example, here you will work with programmable RGB LEDs - lights whose colour can be controlled individually via a single data connection. The specific LED is the WS2812 also known as [NeoPixels](https://learn.adafruit.com/adafruit-neopixel-uberguide/the-magic-of-neopixels), which is the name given to them by the company AdaFruit. The specific LED can be found in products that are not only produced by Adafruit, such as the [Zip Stick by Kitronik](https://kitronik.co.uk/products/35129-zip-strip), but the set of NeoPixel Arduino Libraries written by Adafruit can often be used with non-Adafruit products.

In this lesson you will install the [Adafruit NeoPixel Libraries](https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library-installation) and use them to control a [Kitronik Zip Stick](https://kitronik.co.uk/products/35129-zip-strip) using an Arduino Nano Every board.

<img src="https://kitronik.co.uk/cdn/shop/products/35129_large-kitronik-zip-stick-leds-front_e7ca50db-bc14-4677-9e2d-e8460551b5a7_800x.jpg" width="300">



## Tasks
1. Read through the [basics of working with NeoPixels](https://learn.adafruit.com/adafruit-neopixel-uberguide/basic-connections) and [best practices](https://learn.adafruit.com/adafruit-neopixel-uberguide/best-practices) to understand how best to avoid burning them out.

2. [Follow this instructions to install the Adafruit NeoPixel Libraries](https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library-installation)

3. You are now ready to connect your LEDs to your Arduino:
   * Disconnect everything from power and turn the battery pack off.
   * Connect the DIN pin on the LED stick to Pin 6 on the Arduino Nano Every (see the pin diagram below).
   * Connect a GND pin on the LED stick to a GND pin on the Arduino (in both cases it doesn't matter which one).
   * Connect the black (-) wire from the battery pack to the GND pin on the LED stick.
   * Connect the red (+) wire from the battery pack to the 5VDC pin on the LED stick.

4. Open up the example `simple` from the Examples of the NeoPixel Library (look under the File menu in the Arduino IDE).

5. In the sketch, change line 14 to `#define NUMPIXELS 5`. This is to correspond the number of LEDs on the Zip Stick.

6. Upload the sketch to the Arduino board and turn on the battery pack. You should see the LEDs turn on sequentially in green.


## Skills Audit
Can you:
- [ ] Get the simple LED sketch to run.
- [ ] Change the LED colour to bright pink.
- [ ] Slow down how quickly the LEDs turn on.
- [ ] Have each LED turn on as a different colour.


## Pin Diagram
Once again the pin diagram is provided here for easy reference.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")