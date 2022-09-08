Now that you have tackled how to get information in and out of the Arduino using circuits or Serial communication, you are going to look at how you can use code to route that information and make decisions.

We will group decision making into two broad categories: responding to a yes/no question and repeating the same action multiple times. You will use the `if` and `else` commands to ask a question and then respond to the answer and you will use `for` loops to repeat the same lines of code.

The pin diagram is provided again here for your convenience.

![Pin diagram of the Nano Every. Image created by Arduino.](https://docs.arduino.cc/static/90c04d4cfb88446cafa299787bf06056/ABX00028-pinout.png "Nano Every Pin Diagram")



## Tasks
1. Go through the [If Statement example in the Arduino documentation](https://docs.arduino.cc/built-in-examples/control-structures/ifStatementConditional).

2. Set up an external LED on pin 2 and change the code so that you control that LED instead of the built-in LED.

3. Add a second LED on pin 3. Change and add code to the sketch so that only one LED is turned on when the potentiometer is above the threshold and then only the other LED is turned on when below the threshold.

4. Add a third LED on pin 4. Change the code once more, this time setting a second threshold at a different value. Have only one LED turn on at a time depending on if the potentiometer is (1) below both thresholds, (2) between the two thresholds, or (3) above both thresholds. You might find [the documentation on using `&&`](https://www.arduino.cc/reference/en/language/structure/boolean-operators/logicaland/) useful.

5. Moving away from `if` statements and onto `for` loops, go through the steps in the [Arduino looping tutorial](https://docs.arduino.cc/built-in-examples/control-structures/ForLoopIteration). You will need to make a few changes though as you have only 3 LEDs. You can remove the potentiometer from your circuit, but keep the LEDS on pins 2, 3, and 4. You then need to change the values in the `for` loops to reflect that you are using 3 LEDS, not 6. In lines 33 and 44 of the sketch you need to change the value where the looping stops to `thisPin < 5`. and in line 60 have the looping start at 4.

```
# in lines 33 and 44 make the following change
for (int thisPin = 2; thisPin < 5; thisPin++) {

# in line 60 make the following change
for (int thisPin = 4; thisPin >= 2; thisPin--) {
```

## Skills Audit
Can you:
- [ ] Use an `if` statement to test if something is true or false
- [ ] Use a collection of `if` statements to make selection