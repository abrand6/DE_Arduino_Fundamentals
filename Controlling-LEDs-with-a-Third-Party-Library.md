Whilst you can certainly build a wide variety of projects using the built-in resources provided by the Arduino platform, you will likely want to take advantage of the open source community's contributions. This most frequently is encountered by wanting to use a specific electronic component and its accompanying code library to make it easier to use.

As an example, here you will work with programmable RGB LEDs - lights whose colour can be controlled individually via a single data connection. The specific LED is the WS2812 also known as NeoPixels, which is the name given to them by the company AdaFruit. The specific LED can be found in products that are not only produced by Adafruit, such as the [Zip Stick by Kitronik](https://kitronik.co.uk/products/35129-zip-strip), but the set of NeoPixel Arduino Libraries written by Adafruit can often be used with non-Adafruit products.

In this lesson you will install the Adafruit NeoPixel Libraries and use them to control a [Kitronik Zip Stick](https://kitronik.co.uk/products/35129-zip-strip) using an Arduino Nano Every board.

![Kitronik Zip Stick with 5 LEDs](https://kitronik.co.uk/cdn/shop/products/35129_large-kitronik-zip-stick-leds-front_e7ca50db-bc14-4677-9e2d-e8460551b5a7_800x.jpg?v=1582131382)

Once again the pin diagram is provided here for easy reference.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")


https://learn.adafruit.com/adafruit-neopixel-uberguide/the-magic-of-neopixels

[Follow this instructions to install the Adafruit NeoPixel Libraries](https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library-installation)


## Tasks
1. Return to the [blink sketch](https://docs.arduino.cc/built-in-examples/basics/Blink), but this time follow the below steps for adding an LED via the breadboard.

2. Change the pin number in the code and in the circuit so that you control the LED on pin 10.

3. Go the [Fade tutorial](https://docs.arduino.cc/built-in-examples/basics/Fade) and follow the steps to not just turn your LED on and off, but to control the brightness. We will go through some of the more advanced aspects of the code in a future lesson. For now, just be sure to understand the function `analogWrite()`. You can read more about [Pulse Width Modulation in the Arduino documentation](https://docs.arduino.cc/learn/microcontrollers/analog-output).

4. Return to the [sketch that had a button control the LED](https://docs.arduino.cc/built-in-examples/digital/InputPullupSerial). Modify your circuit so that you are controlling an external LED instead of the built-in LED.

5. Add a second LED to the breadboard and connect it to pin 6. Modify the code so that when the button pressed one LED is on and the second is off, and when the button is released the LED that was off turns on and the LED that was on turns off.


## Skills Audit
Can you:
- [ ] Build a circuit with an LED on a breadboard
- [ ] Control the LED with code
- [ ] Change the pin controlling the LED
- [ ] Build multiple LED circuits that can be controlled independently of each other