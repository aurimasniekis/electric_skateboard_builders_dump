# VESC and Arduino giving the same speed of motor

### Replies: 15 Views: 1386

## \#1 Posted by: pengy Posted at: 2016-11-25T15:45:20.511Z Reads: 116

```
Hey everyone, got my setup:
4s battery
147KV Turnigy
Vesc

I'm trying temporarily to control the speed of my motor with an Arduino and a potentiometer. The code should work and I've tried also to manually input the speed, and always getting the same speed from the motor.

It is set to PPM which should work and I didn't change any unconventional settings in BLDC.
When I use the keyboard to control the motor it works fine.

<img src="/uploads/db1493/original/3X/5/f/5f03cdb46cec2c78700840f1ef126d35f9a46876.png" width="690" height="388">
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-25T18:36:30.229Z Reads: 102

```
Maybe post your arduino code? How are you generating the ppm pulse? Which pins are you using as output? How are you wiring everything together?
```

---
## \#3 Posted by: saul Posted at: 2016-11-25T19:54:42.106Z Reads: 94

```
You're on current control. It will go to the same speed when unloaded. Once you're on the board you will have more speed control based on torque.
```

---
## \#4 Posted by: pengy Posted at: 2016-11-25T20:07:54.739Z Reads: 87

```
This is the code, no matter how I change the value as long as it is 90 or more it runs at the same speed. Pin 9~

#include <Servo.h> 

Servo myservo;

void setup() 
{ 
  myservo.attach(9);
  myservo.write(40);  // set servo to mid-point 40
  delay(3000);
} 

void loop() {
  myservo.write(90); //90
  delay(2);
  }
```

---
## \#5 Posted by: pengy Posted at: 2016-11-25T20:09:00.840Z Reads: 79

```
That could be the thing Saul, to what do I need to change it? And I've understood UART might have better usage, maybe I should use that over PPM

Thanks.
```

---
## \#6 Posted by: saul Posted at: 2016-11-25T20:13:09.972Z Reads: 76

```
I always use write milliseconds for servos but it's the same.
If you want speed control switch to pid mode on the ppm tab. But not for riding.

The uart lib is pretty complicated I was trying to use it a couple days ago.
```

---
## \#7 Posted by: pengy Posted at: 2016-11-25T20:22:41.547Z Reads: 73

```
Still no luck, there's no movement at all now, attached some screen shots

<img src="/uploads/db1493/original/3X/9/5/95ae5b3a1461c951841a3ffd023866d28d0575f9.png" width="690" height="388"><img src="/uploads/db1493/original/3X/e/0/e0dc1a4233f87f332209f0d39aa6e2d920ea085c.png" width="690" height="388">
```

---
## \#8 Posted by: saul Posted at: 2016-11-25T20:26:09.100Z Reads: 64

```
That's weird. Well you can u check the multiple can bus box.
And check the display box. Will show the input signal live.
```

---
## \#9 Posted by: pengy Posted at: 2016-11-25T20:35:31.700Z Reads: 61

```
Not sure where these are located, but I think that the batteries ran out on this last attempt unfortunately.. I will charge them and try again tomorrow.

Thought about connecting a power supply I have, but it gives only 1.5 amp, so not sure of what good it will bring..
```

---
## \#10 Posted by: saul Posted at: 2016-11-25T20:38:58.911Z Reads: 63

```
Bottom of the second screen. Good luck.
```

---
## \#11 Posted by: anorak234 Posted at: 2016-11-26T17:05:03.863Z Reads: 51

```
Just because it can all be powered at 4s doesn't mean it's a good idea. Your top speed on 4s with that kv motor is going to be negligible. Get it up to at least 10s...
```

---
## \#12 Posted by: pengy Posted at: 2016-11-27T15:37:59.319Z Reads: 43

```
True, this is exactly what I'm using it for, just for setting it up. Since charging is a bit combersome at the moment.. Eventually will use a 12s to run it.
```

---
## \#13 Posted by: EssEnn Posted at: 2016-11-28T00:28:58.752Z Reads: 40

```
You should use myservo.writeMicroseconds and not myservo.write. 

When you attach a servo and do not define the range the PWM signal for 0 degrees is 544 microseconds and 180 degees is 2400 microseconds by default. RC controllers only have a range of around 1000 microseconds. 

Also with your code you are setting the mid point @ 40 but the range for the servo is 0 to 180 so 90 is actually your mid point, 180 is your max. You also don't need the delay in the void setup ()

Here is a bit of code I modified to move a servo back and forth at a fixed rate. (don't forget to add the include servo at the beginning). I'm trying to learn to code without the use of Delay as that function stops the Ardunio from doing anything while it is active but I don't have the time to change it right now. 

Servo myservo;  // create servo object to control a servo

double pos = 0;    // variable to store the servo position
int delayTime = 15; // this variable sets the delay time between each step

void setup() {
  myservo.attach(9, 1000, 2000);  // attaches the servo on pin 9 to the servo object
  myservo.writeMicroseconds(1500); // sets the servo to mid point
  Serial.begin(9600);
}

void loop() {
    for (pos = 1000; pos <= 2000; pos += 10) { // goes from 1000 microseconds to 2000 microseconds
    // in steps of 10
    myservo.writeMicroseconds(pos);              // tell servo to go to position in variable 'pos'
    delay(delayTime);                       // delays the time before moving to the next position
    Serial.println(pos);
  }
  for (pos = 2000; pos >= 1000; pos -= 10) { // goes from 180 degrees to 0 degrees
    myservo.writeMicroseconds(pos);              // tell servo to go to position in variable 'pos'
    delay(delayTime);                       // delays the time before moving to the next position
    Serial.println(pos);
  }
}
```

---
## \#14 Posted by: pengy Posted at: 2016-12-01T17:55:06.920Z Reads: 35

```
Thank you for the comprehensive answer, can't wait to try it. At the moment it is all on hold since I am waiting for a battery charger to arrive..Unless.. I assume a PC power supply could be able to provide enough amps for everything to work and maybe I could connect it to the 12 volts just for the settings. Is there a risk in doing that? Has anybody tried it successfully?
```

---
## \#15 Posted by: EssEnn Posted at: 2016-12-01T22:58:17.239Z Reads: 31

```
All I'm doing is letting you know what I have found out. The code works but I have not tried it with an ESC, only with a servo. Oh, you must make sure that the Arduino and VESC share a common ground BTW otherwise its not going to work at all.

I found this tutorial -  https://learn.adafruit.com/multi-tasking-the-arduino-part-1/ditch-the-delay
This is what I'm trying to get my head around lol
```

---
