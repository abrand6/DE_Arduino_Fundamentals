You have connected external devices such potentiometers and LEDs to your Arduino board. These devices are quite simple, either responding to a change in voltage and current provided by the Arduino board or the Arduino board can measure a change in voltage from the device.

More complicated devices need a more complex language to communicate either what the device is detecting or to instruct the device. One common language or protocol is I2C or I<sup>2</sup>C which stands for [Inter-Integrated Circuit](https://learn.sparkfun.com/tutorials/i2c/all). One great feature is that it only requires 4 connections, no matter what devices are being connected - power, ground, the data connection, and the clock connection which makes sures the devices speak with each other in a coordinated way. 

You will connect an [LED Bar](https://wiki.seeedstudio.com/Grove-LED_Bar/) to your Arduino board, but this will be the same connection for any I2C device. However, it is important to note that the code will differ for different I2C devices. Most devices will have an Arduino library to make the code easier to read and write, so it is important to install the correct library for the device you are using. 

The pin diagram is provided again here for your convenience.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")

## Tasks

https://wiki.seeedstudio.com/Grove-LED_Bar/

## Skills Audit
Can you:
- [ ] Install an Arduino library to support communicating over I2C
- [ ] Communicate with an external device using I2C