# VESC current control problem

### Replies: 19 Views: 393

## \#1 Posted by: new Posted at: 2019-03-29T15:51:03.766Z Reads: 80

```
Hi folks! 
I try to control my VESC 6 using an arduino nano.

I use FOC with "Current" setting and the latest firmware.
The motor direction test spins the motor very nice and smoothly.
The RT app display in vesc tool shows the correct input values and the motor spins up **once**.

However the motor does not spin up again after ppm is set to neutral (1500). I have to **reverse** it (1400) or **turn it** in the opposite direction **manually**.

Could you please confirm that VESC 6 does work using the servo library and maybe provide some debug tips?
Thank you very much!

```
#include <Servo.h>
Servo servo;
int ppmOut = 11;
int ppmTestValue = 1500;

void setup() {
  Serial.begin(9600);
  servo.attach(ppmOut);
}

void loop() {
  if (Serial.available() > 0) {
    int ppmTestValue = Serial.parseInt();  
    if(ppmTestValue > 0){
      Serial.print("I received: ");
      Serial.println(ppmTestValue, DEC);
      servo.writeMicroseconds(ppmTestValue);
    }
  }
}
```

---
## \#2 Posted by: StefanMe Posted at: 2019-03-30T07:54:44.232Z Reads: 54

```
Doesn’t matter what VESC u use. 

Check the open source remotes for reference. FeatherRemote, firefly remote... all work with ppm and VESC 6
```

---
## \#3 Posted by: new Posted at: 2019-03-30T08:01:00.737Z Reads: 55

```
I see, so the servo library should work.
I reuploaded the firmware to clear the settings and reconfigured everything but the problem remains.

Do you think the arduino setup is fine if the vesc tool shows the correct ppm values?
```

---
## \#4 Posted by: StefanMe Posted at: 2019-03-30T10:18:59.094Z Reads: 47

```
Share your code... it should work normally.
```

---
## \#5 Posted by: new Posted at: 2019-03-30T10:29:16.924Z Reads: 42

```
See my first post for the code.

I chose "Current" mode and send 1600 which **worked**!

I discovered when I send 1500 which is neutral I am not able to drive the motor anymore afterwards except I send 1440 or less. Please note that i set safe start to false.

**This basically means that i have to reverse the direction (brake) or turn the motor backward manually to spin the motor up a second time.**
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-04-01T08:37:30.412Z Reads: 31

```
Sounds like you've set your ppm endpoints wrong in vesc tool.
```

---
## \#7 Posted by: new Posted at: 2019-04-01T08:41:18.700Z Reads: 30

```
Do you mean "Pulselength Start, End and Center" ? I went with the default settings.
Vesc tool always shows the correct values but the motor doesn't spin up again as described above.
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-04-01T08:41:57.079Z Reads: 31

```
Post a screenshot please.
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-04-01T08:49:28.814Z Reads: 28

```
Try turning on the pulselength mapping option at the bottom, then using the arduino to send both maximum and minimum commands.
```

---
## \#11 Posted by: new Posted at: 2019-04-01T08:53:28.225Z Reads: 29

```
![test|690x365](upload://7on8fZ3McvAEmuSEfqlvsfcKKIn.png) 
It's so strange. Could it be a hall sensor problem?
I think I got the mapping correct.
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-04-01T08:55:33.064Z Reads: 25

```
Did you apply the new pulselength settings?
```

---
## \#13 Posted by: new Posted at: 2019-04-01T08:55:48.971Z Reads: 27

```
yes i did.

1500, 1600, 1700 works like it should

1500, 1600, 1400, 1600 spins up twice as it's supposed to

1500, 1600, 1500, 1600 does spin up **only once**, second 1600 gets ignored

1500, 1600, 1500, manually turn the motor in the opposite direction, then 1600 works
```

---
## \#14 Posted by: MysticalDork Posted at: 2019-04-01T08:57:25.487Z Reads: 28

```
Hmm, weird. I'll mull it over some more, but I gotta hit the hay for tonight.
```

---
## \#15 Posted by: new Posted at: 2019-04-01T08:59:37.075Z Reads: 29

```
thank you for trying to help :slight_smile:
```

---
## \#18 Posted by: new Posted at: 2019-04-03T13:24:25.938Z Reads: 21

```
I noticed the arrow key motor control also works in PPM mode if the arduino isn't connected or if it does not run "servo.attach(ppmOut)" at all.

With the arduino connected arrow key control in vesc tool doesn't work, no matter what output pin i choose. Can anyone confirm this behaviour?
```

---
## \#19 Posted by: janpom Posted at: 2019-04-03T13:42:51.978Z Reads: 20

```
You don't need to ground any ADC. How do you connect the Arduino to the VESC? Isn't the problem that you connect the servo signal to the ADC pin on the COMM port rather than to the servo port?
```

---
## \#20 Posted by: new Posted at: 2019-04-03T13:46:52.152Z Reads: 17

```
No i checked the connections. After trying ADC (and the comm port) i switched back to PPM (with the servo pin).
I don't know why i have to turn the motor backwards before it spins up again.
```

---
## \#21 Posted by: new Posted at: 2019-04-03T16:39:51.074Z Reads: 16

```
This is related to current control types. In duty cyles control types i don't experience the problem.
```

---
## \#22 Posted by: new Posted at: 2019-04-03T17:19:17.574Z Reads: 15

```
Solved it by using "Current No Reverse With Brake"
```

---
