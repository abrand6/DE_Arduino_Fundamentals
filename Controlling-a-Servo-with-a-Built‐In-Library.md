So far you have been working with code that is automatically accessible in the Arduino IDE. Functions like `analogRead()` and `loop()` are already defined - you didn't have to tell the Arduino what they mean. You will now be working with code that is automatically included, but is defined in a library. This library isn't automatically loaded by the Arduino to help save memory. It is only loaded when you ask for it. It is referred to as a built-in library.

You will use the Arduino `Servo Library`, which is [fully documented online](https://www.arduino.cc/reference/en/libraries/servo/). While the single servo you will be using can be powered by the Arduino board, it is safer and best practice to power it with a second power supply. That will keep the servo working as expected and it will also keep you from accidentally damaging your Arduino board.

![Mini Servo available on RS](https://media.rs-online.com/image/upload/bo_1.5px_solid_white,b_auto,c_pad,dpr_2,f_auto,h_399,q_auto,w_710/c_pad,h_399,w_710/Y2153180-01?pgw=1)


## Tasks

1. Follow the steps in [this tutorial on using a servo](https://docs.arduino.cc/learn/electronics/servo-motors/) using the one supplied in your kit. Use the supplied battery AA pack to power the servo, paying close attention to the + and -. 



## Skills Audit
Can you:
- [ ] Build a circuit with a servo on a breadboard
- [ ] Program the servo to do some kind of automated movement or sweep after a button is pressed
- [ ] Program the servo to move slowly and smoothly while a button is being held down