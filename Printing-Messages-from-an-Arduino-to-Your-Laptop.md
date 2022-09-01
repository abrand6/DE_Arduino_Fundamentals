We are now going to dig in a little deeper into the structure of a sketch.

In the previous exercise you edited the input parameter of a function by changing the number in `delay()`. 

You might have noticed that the sketch was divided into two big sections, one starts with the line `void setup() {` and the second starts with the line `void loop() {`. There is a block of text at the very top that is grey, this is a comment block. The Arduino completely ignores comments, they are just notes to self or a note to a potential other coder. 

Each section of code starts with a `{` and ends with a `}`. The code just before the `{` is the name for that block, either `setup()` or `loop()` in this case. Each Arduino sketch has to have exactly one block of code named `setup()` and one block named `loop()`. It can't have more than one block with the same name.

The code inside the `setup()` block is run only once when the Arduino first turns on or reboots.

The code inside the `loop()` block runs immediately after the `setup()` finishes. Once the code inside `loop()` is finished, it is run again. And again. The code is repeated forever until the Arduino board is turned off.

In the below exercises you will explore how `setup()` and `loop()` by printing messages from the Arduino board to your computer.

## Tasks
1. In the Arduino IDE, open a new sketch by going to **File > New**



## Skills Audit
Can you:
- [ ] Print a message only once, when the board first starts up.
- [ ] Print a message multiple times, each time `loop()` is called.
- [ ] Print a message without a new line/line break at the end.
- [ ] Combine multiple strings and variables together to ouput a custom message.