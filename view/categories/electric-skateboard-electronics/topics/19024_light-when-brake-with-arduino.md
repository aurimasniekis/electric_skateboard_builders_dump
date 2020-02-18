# Light when Brake with Arduino

### Replies: 14 Views: 1452

## \#1 Posted by: IsTalo Posted at: 2017-03-13T20:57:32.342Z Reads: 178

```
Hello Again Guys, now I want to know about Brake lights. I saw that Vedder video that is awesome and everybody said that he used Uart, but I really don't know. I imagined doing it with an arduino, like, the arduino read the position of the trigger (Gt2b or Mini Remote) and when the trigger is close to the brake it actives the light. I know it is possible, but I don't know the code to read the potentiometer inside the controller. I think we could use the Servo Data pin (yellow one in my vesc) to read it, so It would be connected on a Breadboard and them go to the Arduino and to the reciever. If someone know how to do it and want to help me I would like to help too.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-03-13T22:11:34.772Z Reads: 165

```
Are you referring to this video? 
https://youtu.be/G8f0xg7DNmM
```

---
## \#3 Posted by: LukeL Posted at: 2017-03-13T22:43:50.984Z Reads: 152

```
you can read the gt2b receiver from the servo data pin like you said, it out puts a pwm wave changing the duty cycle as you move the throttle.

You can use the arduino pulsein function to read the pulse widths in microseconds, you could read the pulsewidth 100 times a second or something and when the pulse width equals whatever it is when the throttle is pushed to the brake, turn on some leds with other arduino pins

only problem i could see is if connecting to both the vesc and arduino could draw too much current from the servo data pin. it shouldn't as i think they work on reading voltage so will have high impedance but i haven't tried it
```

---
## \#4 Posted by: IsTalo Posted at: 2017-03-13T23:01:20.728Z Reads: 139

```
Yep, this one
```

---
## \#5 Posted by: IsTalo Posted at: 2017-03-13T23:02:03.009Z Reads: 133

```
And I need that special machine to read the waves or can I read at The Serial Monitor? And what should be the code?
```

---
## \#6 Posted by: LukeL Posted at: 2017-03-13T23:25:43.169Z Reads: 134

```
yeah you can just use the serial monitor

use pulsein() its a built in function for arduino
Syntax: pulseIn(pin, value, timeout)

set the pin you're using to an input

put something like this in a loop
Throttle = pulseIn(2, HIGH, 25000);

you can then print out the variable to the serial monitor, or use if statement for brake lights

I also put a delay in the loop just to slow it down a bit as you might get some glitches or something if it's going as fast as it can

note the number constantly changes a little bit, i assume due to noise on the receiver's input 2.4GHz wave but shouldn't matter for brake lights. when i did it the receiver output 1500us at rest went upto 2500 and down to 500
```

---
## \#7 Posted by: IsTalo Posted at: 2017-03-13T23:27:57.728Z Reads: 129

```
Nice, I'll try tomorrow, Should I use a Analog Pin in the data pin of the reciever?
```

---
## \#8 Posted by: LukeL Posted at: 2017-03-13T23:34:41.915Z Reads: 127

```
no I used digital pin, it's a digital wave also it doesn't need to be one of the pwm ones they can output a pwm wave

I used pin 2 on a Uno
```

---
## \#9 Posted by: IsTalo Posted at: 2017-03-13T23:36:06.294Z Reads: 123

```
My Uno is broken (Science Project) and now I just have a nano, I think it works too. Do I have to power the Vesc to use it? Or could I just power the receiver?
```

---
## \#10 Posted by: LukeL Posted at: 2017-03-13T23:38:15.330Z Reads: 114

```

I did all this without it connected to vesc just as a test so i don't know if it will stop the vesc from reading it or cause problems for the vesc

if the nano has digital pins it should work fine, i used the uno to power the receiver from the 5V pin, i don't know if the nano has that but if not you could use some other 5V source
```

---
## \#11 Posted by: IsTalo Posted at: 2017-03-13T23:42:12.624Z Reads: 114

```
Yeah, It have, I did it last week. Tomorrow I will try with two red leds, if I have any question I ask you. Could you PM me with all the code?
```

---
## \#12 Posted by: LukeL Posted at: 2017-03-13T23:54:05.814Z Reads: 118

```
yeah sure, i think i got most of the code from here https://www.sparkfun.com/tutorials/348
```

---
## \#13 Posted by: saul Posted at: 2017-03-14T06:08:53.024Z Reads: 114

```
I have this working with an attiny85. used a nano for testing.

i'm still setting up a configuration bit so theres no need to reprogram.
check out the circuit here
http://www.electric-skateboard.builders/t/brake-lights-and-turn-signals-finally-for-any-esc/15888
```

---
## \#14 Posted by: IsTalo Posted at: 2017-03-14T08:57:19.273Z Reads: 111

```
Oh, Nice, I'll read
```

---
