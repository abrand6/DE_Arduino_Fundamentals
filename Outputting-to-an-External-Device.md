You have added sensors to allow the Arduino Board to know the state of the physical world and you will now add an external device that can change the physical world. You have done a little of this by using the built-in LED on the Arduino board, but now you will add an LED on the breadboard.

Once again the pin diagram is provided here for easy reference.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")

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