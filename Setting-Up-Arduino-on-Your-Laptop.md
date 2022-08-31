The word Arduino refers to many different parts of a technological ecosystem. It refers to a set of [physical products (boards)](https://www.arduino.cc/en/hardware), the [software (IDE)](https://www.arduino.cc/en/software) used to program those boards, and the [company](https://www.arduino.cc/en/about) that oversees the development of both the hardware and software along with developing educational resources.

We will work with the Arduino board called the [Nano Every](https://docs.arduino.cc/hardware/nano-every). It was chosen for being small and for being relatively low cost, while containing the necessary features for completing your final projects for the module.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")

A summary of the first tasks you need to complete are to:
1. Install the software
2. Install the supporting library for the Nano Every board
3. Upload the Blink sketch to verify everything is set up correctly



## Tasks
### Install the software
1. Follow the Quickstart Guide on the [Nano Every site](https://docs.arduino.cc/hardware/nano-every). Select the **Arduino IDE 2.0 Option** and complete the **Downloading and Installing the Arduino IDE 2.0** instructions.

2. Open the Arduino IDE on your laptop and connect your Arduino board to your computer using the USB lead.

3. You should see a pop-up message at the bottom left of the window that asks if you would like to install the supporting package for the Nano board. Click on the Install this package text.

4. The Boards Manager window will appear with the Arduino megaAVR Boards package. Click on the install button. It may take a few minutes to complete.

5. Quit and restart the Arduino IDE.


### Uploading your first sketch
Make sure your Arduino board is still connected. You now need to select the type of board you are working with along with which port it is connected to.

6. Open the example sketch `Blink` by going to **File > Examples... > 01 Basics > Blink**

7. Select the board you are using by going to **Tools > Board > Arduino megaAVR Boards** and selecting **Arduino Nano Every**

8. Select the port the board is connected to - it is essential that the board is connected with the USB lead to your laptop. Go to **Tools > Port ** and select the option where the Nano Every is listed. The exact name of the port will vary between laptops.

9. You should now see the current selected board and port at the bottom of your Arduino IDE window. Remember your port name will probably not be the same as in the below screenshot.

10. Return to the Arduino Quickstart documentation and read through the **How to Upload a Sketch with Arduino 2.0**

11. Upload the Blink sketch to your board.

## Skills Audit
Can you:
- [ ] Launch the Arduino IDE on your laptop
- [ ] Select the correct board and port within the Arduino IDE
- [ ] Upload the Blink sketch to your board
- [ ] Confirm that the upload worked by observing the LED on your board