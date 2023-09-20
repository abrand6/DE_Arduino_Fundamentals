**The ultrasonic sensor we will be working with should not be connected to the Arduino board whilst the Arduino is powered on. It can damage the sensor. Make sure the Arduino board is not connected to your laptop when you are setting up your circuit.**

You have connected external devices such potentiometers and LEDs to your Arduino board. These devices are quite simple, either responding to a change in voltage and current provided by the Arduino board or the Arduino board can measure a change in voltage from the device.

More complicated devices need a more complex language to communicate either what the device is detecting or to instruct the device. One common language or protocol is I2C or I<sup>2</sup>C which stands for [Inter-Integrated Circuit](https://learn.sparkfun.com/tutorials/i2c/all). One great feature is that it only requires 4 connections, no matter what devices are being connected - power, ground, the data connection, and the clock connection which makes sures the devices speak with each other in a coordinated way. This particular sensor is so simple it doesn't need to use I2C, but it does use the same physical cable to make the electrical connections. As part of Cyber Physical Systems you will be using a different Grove board to control three motors. This sensor is a gentle introduction to working with Grove hardware.

![Photo of a Grove Ultrasonic Ranger by Seeed Studio.](https://files.seeedstudio.com/wiki/Grove_Ultrasonic_Ranger/V2.jpg "Grove Ultrasonic Ranger")

You will connect an [ultrasonic distance sensor](https://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/) to your Arduino board, but this will be the same connection for any I2C device. However, it is important to note that the code will differ for different I2C devices. Most devices will have an Arduino library to make the code easier to read and write, so it is important to install the correct library for the device you are using. 

The pin diagram is provided again here for your convenience.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")

## Tasks
You will be following a slightly different set of steps to the [Grove Ultrasonic Ranger tutorial by Seeed Studio](https://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/). Feel free to refer to the original tutorial for additional information.

1. You first need to add the library for the Grove Ultrasonic Ranger to your Arduino IDE. [Download the library from GitHub](https://github.com/Seeed-Studio/Seeed_Arduino_UltrasonicRanger/archive/master.zip). 

2. To install the library within the Arduino IDE, go to **Sketch->Include Library->Add ZIP Library...**. When asked select the zip file you just downloaded. There should be a temporary message at the bottom of the Arduino that appears after the library has successfully installed.

![Screenshot of the menu to add a zip file of a library.](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/9dcc92cc03fe6c40c9323fba77e3fc80ee9a5ac1/wiki-images/add-zip-library.png)

3. You now need to connect your ultrasonic sensor to your Arduino board using the white 4-pin Grove connector on the board. **Be sure that your Arduino is not connected to power, do not connect your ultrasonic sensor to a powered Arduino board or you might damage it!** Use the Grove to 4 pin break-out cable included in your kit. It has the Grove socket connector on one side and 4 individual pins on the other side. Plug the Grove connector side into your sensor.

![Photo of the Grove to 4 pin cable](https://user-images.githubusercontent.com/394553/189597848-63a26386-ef9f-4c57-8bad-6dae1dc1b0a5.png "Grove to 4 pin cable")


4. On the other side you need to connect the 4 pins to your Arduino board as follows:
    * Red is connected to 5V on the Arduino board
    * Black is connected to ground on the Arduino board (either one, doesn't matter which)
    * White is not connected 
    * Yellow is connected to D7 on the Arduino Nano Every

5. If you now go to **File >> Examples...** in the Arduino IDE you should see the **Grove Ultrasonic Ranger** listed under the bottom section of the menu labelled **Examples from Custom Libraries**. Open the **UltrasonicDisplayonTerm** example from the library you just installed.

6. Plug in the Arduino to your laptop and upload the sketch. Open the serial monitor and you should see the distance between the sensor and any object in front of it printed out. If it doesn't do that, double check your connections. The most likely problem is that you didn't quite wire up the breadboard correctly.

8. Add a button to the breadboard and your Arduino board circuit. Have the values of the sensor print only when the button is pressed.

9. As a final task, add your three LEDs and have them each light up as an object gets closer to the sensor.




## Skills Audit
Can you:
- [ ] Be able to install an Arduino library 
- [ ] Communicate with an external device using a Grove cable
- [ ] Extend an example sketch by adding functionality