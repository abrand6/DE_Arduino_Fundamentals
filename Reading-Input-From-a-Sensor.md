You have so far controlled the LED on the Arduino board and sent messages to be displayed on your laptop. Next you will take input from the 
physical world and use it to output a message over Serial and to control the LED on your Arduino board.

You will use an object called a breadboard to connect your circuits to your Arduino board. A breadboard makes it easy to build a temporary circuit quickly, though it may take a little time to get used to how to make connections. It may not feel very intuitive at first.

The final note is that the Arduino Nano Every has an awkward design feature - the pin labels are all on the underside of the board. That means when you put it in a breadboard, you can't read the labels. We've provided a pin diagam here to help you out.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")



## Tasks

1. Read through [this guide to get an overview of how to use a breadboard](https://www.seeedstudio.com/blog/2020/01/06/how-to-use-a-breadboard-wiring-circuit-and-arduino-interfacing/).

2. Follow the steps in [this tutorial on reading the input from a potentiometer](https://docs.arduino.cc/built-in-examples/basics/AnalogReadSerial) using the one supplied in your kit. You are using a different Arduino board, so use the pin diagram above to find the correct pins for the circuit.

3. Modify the code and the circuit in the step above so that you are reading the potentiometer input from pin A7 instead of A0.

4. Remove the potentiometer from your breadboard to start again with an empty breadboard.

5. Follow the steps in [this tutorial on reading the input from a switch or button](https://docs.arduino.cc/built-in-examples/digital/InputPullupSerial). You will be controlling the LED on the Arduino board. Don't worry too much about the part of the code using `if` and `else`, we will look at that in more detail in a later lesson.

8. Modify the code and the circuit in the step above so that you are reading from the switch from pin 4 instead of pin 2.

## Skills Audit
Can you:
- [ ] Build a circuit on a breadboard
- [ ] Read in and display the value from a potentiometer
- [ ] Read in and display the value from a switch
- [ ] Change which input is used to read in a sensor