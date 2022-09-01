We are now going to dig in a little deeper into the structure of a sketch.

In the previous exercise you edited the input parameter of a function by changing the number in `delay()`. 

You might have noticed that the sketch was divided into two big sections, one starts with the line `void setup() {` and the second starts with the line `void loop() {`. There is a block of text at the very top that is grey, this is a comment block. The Arduino completely ignores comments, they are just notes to self or a note to a potential other coder. 

![Screenshot of the Blink example in the Arduino IDE with the setup and loop functions highlighted](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/ab62e9883c76e12613a1d2aaad86565aeb8b7b01/wiki-images/blink-setup-loop.png "Setup and Loop")

Each section of code starts with a `{` and ends with a `}`. The code just before the `{` is the name for that block, either `setup()` or `loop()` in this case. Each Arduino sketch has to have exactly one block of code named `setup()` and one block named `loop()`. It can't have more than one block with the same name.

The code inside the `setup()` block is run only once when the Arduino first turns on or reboots.

The code inside the `loop()` block runs immediately after the `setup()` finishes. Once the code inside `loop()` is finished, it is run again. And again. The code is repeated forever until the Arduino board is turned off.

In the below exercises you will explore how `setup()` and `loop()` by printing messages from the Arduino board to your computer.

## Tasks
1. In the Arduino IDE, open a new sketch by going to **File > New** You will see that the sketch already has the two core code blocks of `setup()` and `loop()` started for you.

![Screenshot of new sketch window in Arduino IDE](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/09c629da1c5092118af3365deb906279f2cfc9d6/wiki-images/new-sketch.png "New sketch")

2. Inside of `setup()` type in the below code. 
```
// start Serial communication at a rate of 9600 bps
Serial.begin(9600); 
// send a message
Serial.println("Hello from setup");
```

The lines starting with `//` are comments. You don't have to include them, but you may find them useful for taking notes. The line `Serial.begin(9600);` tells the Arduino board that it should get ready to send and listen to messages that will be travelling at a rate of 9600 bps. The 9600 isn't that important to understand right now. In general, if you don't have a reason to change it, start Serial communication at 9600 bps.

3. Make sure you've selected the board and port then upload the sketch.

4. Open the Serial Monitor. This is an area at the bottom of the Arduino IDE that will display any messages from the Arduino board.

![Screenshot of Arduino IDE with the Serial Monitor button highlighted](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/89b8839eec8bc5448cc8d8d832082a9213ebfe8c/wiki-images/serial-monitor.png "Serial Monitor")

5. You should see the message "Hello from setup" printed in the bottow portion of the IDE window.

6. Change the message to print different text of your choosing. Remember to upload the sketch after you make changes and then to reopen the Serial Monitor after the uploading has completed. You should see your new message printed now.

7. Now add the below line of code to inside of `loop()`. You shouldn't put `Serial.begin()` anywhere but inside of `setup()`, but once you have done that, you can print messages from inside `loop()`.

```
Serial.println("Hello from loop");
```

8. Upload the sketch and open the Serial Monitor. Note how messages are being continuously sent. This helps illustrate the difference between `setup()` which runs only once and `loop()` which is repeated forever.

9. Now make a final change to the code. Change the line of code inside of `loop()` to the below.
 
```
Serial.print("Hello from loop");
```

After uploading, you should now see in the Serial Monitor that the messages run into each other, they aren't on separate lines. This is the difference between `print()` and `println()`. The command with `ln` in the name will end the message with a new line, like the enter key has been used. The command without the `ln` doesn't include this. This can be useful when putting together more complex messages, as we will do in later exercises.

Your final sketch will look similar to the below, though your message text may vary if you customised it.

![Complete sketch that prints a message once in the setup and then continously without a line break in the loop](https://github.com/IDE-GID-Cyberphysical-Systems/CPS-Fundamentals/blob/63cc3dd68b74d90a0425b27fb1b1290d8c118583/wiki-images/printing.png "Serial Monitor printing")

## Skills Audit
Can you:
- [ ] Print a message only once, when the board first starts up.
- [ ] Print a message multiple times, each time `loop()` is called.
- [ ] Print a message without a new line/line break at the end.