The word Arduino refers to many different parts of a technological ecosystem. It refers to a set of [physical products (boards)](https://www.arduino.cc/en/hardware), the [software (IDE)](https://www.arduino.cc/en/software) used to program those boards, and the [company](https://www.arduino.cc/en/about) that oversees the development of both the hardware and software along with developing educational resources.

We will work with the Arduino board called the [Nano Every](https://docs.arduino.cc/hardware/nano-every). It was chosen for being small and for being relatively low cost, while containing the necessary features for completing your final projects for the module.



## Tasks
### Install the software
1. Follow the Quickstart Guide on the [Nano Every site](https://docs.arduino.cc/hardware/nano-every). Select the **Arduino IDE 2.0 Option** and complete the **Downloading and Installing the Arduino IDE 2.0** instructions.

![Screenshot of the Arduino Quickstart Guide highlighting selecting the Arduino IDE 2.0](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/47d227f25c36bb443701a72716459e0337877ad7/wiki-images/quickstart-guide.png "Quickstart Guide for Arduino IDE 2.0")

2. Open the Arduino IDE on your laptop and connect your Arduino board to your computer using the USB lead.

3. Click on the Board Manager icon on the left side of the Arduino IDE window.

![Screenshot of Board Manager icon highlighted in Arduino IDE 2.0](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/47d227f25c36bb443701a72716459e0337877ad7/wiki-images/megaavr-install.png "Screenshot of Board Manager")

4. Search for the Arduino megaAVR Boards package. Click on the install button (you need to hover your mouse over the package description for the button to appear). It may take a few minutes to complete.

5. Quit and restart the Arduino IDE.


### Uploading your first sketch
Make sure your Arduino board is still connected. You now need to select the type of board you are working with along with which port it is connected to.

6. Open the example sketch `Blink` by going to **File > Examples... > 01.Basics > Blink**

7. Select the board you are using by going to **Tools > Board > Arduino megaAVR Boards** and selecting **Arduino Nano Every**

![Screenshot of menu paths to select the board](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/94b5c62aa9fe4f25c4d2aafeb7a6e96d6c7b910a/wiki-images/select-board.png "Select board")

8. Select the port the board is connected to - it is essential that the board is connected with the USB lead to your laptop. Go to **Tools > Port ** and select the option where the Nano Every is listed. The exact name of the port will vary between laptops.

![Screenshot of menu paths to select the port](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/94b5c62aa9fe4f25c4d2aafeb7a6e96d6c7b910a/wiki-images/select-port.png "Select port")

9. You should now see the current selected board and port at the bottom of your Arduino IDE window. Remember your port name will probably not be the same as in the below screenshot.

![Screenshot of bottom right of Arduino IDE showing current board and port selection](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/39adeaac86356f6820b4e9573c837a9e287fec0f/wiki-images/current-board-port.png "Current board and port")

10. Return to the Arduino Quickstart documentation and read through the **How to Upload a Sketch with Arduino 2.0** You will need to click next after the Arduino IDE installation steps.

11. Upload the Blink sketch to your board. You should see the LED blink and the Arduino IDE say that the sketch was uploaded successfully.

## Skills Audit
Can you:
- [ ] Launch the Arduino IDE on your laptop
- [ ] Select the correct board and port within the Arduino IDE
- [ ] Upload the Blink sketch to your board
- [ ] Confirm that the upload worked by observing the LED on your board