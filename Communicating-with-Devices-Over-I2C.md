**The ultrasonic sensor we will be working with should not be connected to the Arduino board whilst the Arduino is powered on. It can damage the sensor. Make sure the Arduino board is not connected to your laptop when you are setting up your circuit.**

You have connected external devices such potentiometers and LEDs to your Arduino board. These devices are quite simple, either responding to a change in voltage and current provided by the Arduino board or the Arduino board can measure a change in voltage from the device.

More complicated devices need a more complex language to communicate either what the device is detecting or to instruct the device. One common language or protocol is I2C or I<sup>2</sup>C which stands for [Inter-Integrated Circuit](https://learn.sparkfun.com/tutorials/i2c/all). One great feature is that it only requires 4 connections, no matter what devices are being connected - power, ground, the data connection, and the clock connection which makes sures the devices speak with each other in a coordinated way. 

![Photo of a Grove Ultrasonic Ranger by Seeed Studio.](https://files.seeedstudio.com/wiki/Grove_Ultrasonic_Ranger/V2.jpg "Grove Ultrasonic Ranger")

You will connect an [ultrasonic distance sensor](https://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/) to your Arduino board, but this will be the same connection for any I2C device. However, it is important to note that the code will differ for different I2C devices. Most devices will have an Arduino library to make the code easier to read and write, so it is important to install the correct library for the device you are using. 

The pin diagram is provided again here for your convenience.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")

## Tasks
You will be following a slightly different set of steps to the [Grove Ultrasonic Ranger tutorial by Seeed Studio](https://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/). Feel free to refer to the original tutorial for additional information.

1. You first need to add the library for the Grove Ultrasonic Ranger to your Arduino IDE. [Download the library from GitHub](https://github.com/Seeed-Studio/Seeed_Arduino_UltrasonicRanger/archive/master.zip). 

2. To install the library within the Arduino IDE, go to **Sketch->Include Library->Add ZIP Library...

![Screenshot of the menu to add a zip file of a library.]()

3. You now need to connect your LED Bar to your Arduino board. This is easy to do on the LED Bar, you will use the white 4-pin Grove connector on the board. Use the Grove to 4 pin break-out cable included in your kit. It has the Grove socket connector on one side and 4 individual pins on the other side. Plug the Grove connector side into your LED Bar.

![Photo of the Grove to 4 pin cable](https://user-images.githubusercontent.com/394553/189597848-63a26386-ef9f-4c57-8bad-6dae1dc1b0a5.png "Grove to 4 pin cable")


4. On the other side you need to connect the 4 pins to your Arduino board as follows:
    * Red is connected to 5V on the Arduino board
    * Black is connected to ground on the Arduino board (either one, doesn't matter which)
    * White is connected to SCL (clock), which is pin A5 on the Arduino Nano Every
    * Yellow is connected to SDA (data), which is pin A4 on the Arduino Nano Every

5. If you now go to **File >> Examples...** in the Arduino IDE you should see the **Grove LED Bar** listed under the bottom section of the menu labelled **Examples from Custom Libraries**. Open the **Level** example from the library you just installed.

6. There is one line of code we need to change - the line of code that lists which pins are SCL and SDA. For the Arduino Nano Every these are pins A5 and A4. So the line just before `setup()` which sets up the the LED Bar should be changed to:

```
Grove_LED_Bar bar(A5, A4, 0); // Clock pin, Data pin, Orientation
```

7. Upload the sketch and you should see the lights move in an animation on the LED Bar. If it doesn't light up correctly, double check your connections. The most likely problem is that you didn't quite wire up the breadboard correctly.

8. Edit the code so that it starts at the maximum level and then decreases, the opposite of what it currently does.

9. As a final task, add a button to the breadboard and your Arduino board circuit. Have the lights of the LED Bar turn on only when the button is pressed.




## Skills Audit
Can you:
- [ ] Be able to install an Arduino library 
- [ ] Communicate with an external device using I2C
- [ ] Extend an example sketch by adding functionality