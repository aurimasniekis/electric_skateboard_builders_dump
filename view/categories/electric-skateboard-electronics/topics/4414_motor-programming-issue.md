# Motor Programming Issue

### Replies: 14 Views: 1975

## \#1 Posted by: michaeld33 Posted at: 2016-06-07T23:07:45.435Z Reads: 117

```
Alright, so unfortunately this is fairly complicated, but I am using a Turnigy Aerodrive SK3 6374 149kv motor, and a BlueSeries 70A ESC. So I have everything connected, and I'm powering the whole setup off of two 1300mah 3s lipos which have been put in series. I have connected my arduino with a joystick to the ESC (the code is below.) So I power it on, and I "calibrate" the joystick by bringing it to the top (2 beeps) then bring it to the bottom (2 beeps [ *wait* ] then the ESC counts the cells, and beeps once more.) I release the joystick and the motor starts moving (since the joystick is now in the middle) but when I push the joystick towards the top, the motor doesn't move any faster, but when I pull it back, it stops.
and then, RANDOMLY it will just go full speed (while the joystick is still in the middle), so I pull it back, it slows and then stops. When I release it, the motor spins again at normal speed, and nothing happens when I push it up. Sometimes it will spin at full speed again randomly. 

I know this is confusing, so I have attached a video and the code below.


[Video](https://youtu.be/xV1MglF7kvM)

CODE:

`#include <SoftwareServo.h>
int potentiometer=A0;
int potval;`

`SoftwareServo ESC;`

`void setup() {`
  
  `pinMode(potentiometer, INPUT);
  ESC.attach(9);   
  Serial.begin(9600);    
  ESC.setMinimumPulse(800);
  ESC.setMaximumPulse(2000);
}`

`void loop() {`

  `potval=analogRead(potentiometer);
  //potval=map(potval,0,1023,0,180);
  ESC.write(potval);
  SoftwareServo::refresh();
  Serial.println(potval);
 }
`
```

---
## \#2 Posted by: Jeefberky Posted at: 2016-06-08T09:02:00.644Z Reads: 70

```
Hey I'm new here.

Does an esc work within 1000 - 2000 microseconds instead of 800 - 2000?

Also, it looks like you are writing the potentiometer value to the esc as degrees instead of microseconds. I do not know if the arduino converts this to microseconds.

Edit: sorry went to quick through your code. I did not see the map(potval) part was excluded from your sketch. You are writing the potentiometer value directly to the esc. I think this should first be converted to microseconds like this potval=map(potval,0,1023,1000,2000). Right now the esc is getting values from 0 to 1023 (I think this is your problem but I do not know for sure).


Good luck!
```

---
## \#3 Posted by: michaeld33 Posted at: 2016-06-08T15:41:10.019Z Reads: 60

```
[quote="Jeefberky, post:2, topic:4414"]
potval=map(potval,0,1023,1000,2000)
[/quote]

I mapped it, like so: potval=map(potval,0,1023,0,180);
I tried maping it 1000-2000 but when I did so it just went through a series of weird beep sequences.
Still doing the same thing as before though...
```

---
## \#4 Posted by: Jeefberky Posted at: 2016-06-08T16:13:54.777Z Reads: 54

```
If you change the value 180 to 179 (potval=map(potval,0,1023,0,179)) ? If you use 0-180 you have 181 degrees instead of 180. Maybe this will solve the problem.
```

---
## \#5 Posted by: michaeld33 Posted at: 2016-06-08T16:17:58.698Z Reads: 47

```
Unfortunately the isssue is still there...
I am VERY confused as to why this isn't working...
```

---
## \#6 Posted by: Jeefberky Posted at: 2016-06-08T17:44:59.862Z Reads: 43

```
I found this page. The code they are using is almost the same you have. However they do not use the line ESC.setMinimumPulse and ESC.setMaximumPulse.

https://dronesandrovs.wordpress.com/2012/11/24/how-to-control-a-brushless-motor-esc-with-arduino/

I also control my motor with an Arduino. But my code is somewhat different because I send a wireless signal to the esc and instead of using ESC.write, I use something like ESC.writeMicroseconds.
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-06-08T19:15:38.671Z Reads: 36

```
Hmm, yeah it's interesting. I KNOW for a fact that this code works on other systems, so I am wondering if there is a compatibility issue, and if I need to get a new motor/esc.

EDIT: They also don't use SoftwareServo, they just use the regular Servo library. IDK if there is a big difference.
```

---
## \#8 Posted by: Jeefberky Posted at: 2016-06-08T20:57:36.279Z Reads: 35

```
I don't know either. It is really weird. You could try to send the esc a few codes to test it.
First the arming signal and then a certain speed for a couple of seconds.
```

---
## \#9 Posted by: fraannk Posted at: 2016-06-08T21:03:15.022Z Reads: 35

```
To control my ESC via Arduino I use the normal Servo.h library :)
```

---
## \#10 Posted by: Jeefberky Posted at: 2016-06-08T21:09:14.660Z Reads: 34

```
That could be it! I'm also using the servo.h library.
```

---
## \#11 Posted by: michaeld33 Posted at: 2016-06-08T21:46:39.824Z Reads: 33

```
Sorry guys, no luck. Only difference with Servo.h library is that it won't let me calibrate the potentiometer at the bottom, so it only starts moving when I push the thumbstick up.
```

---
## \#12 Posted by: michaeld33 Posted at: 2016-06-08T22:25:04.388Z Reads: 28

```
Is it possible that the issue is that I'm using the 149kv SK3 motor with a 6s setup? Should I buy the 236 SK3 motor instead? Different ESC? I can't shell out the cash/wait for the VESC to come back in stock, but if there are any recommendations.
```

---
## \#13 Posted by: Jeefberky Posted at: 2016-06-09T08:01:43.845Z Reads: 26

```
I don't think that would cause the problem. If I'm using a single 3s battery my motor still works and I can even ride my board with it. I'm using a 5055 sk3 280 kv motor, it is rated for 6s~10s.
The esc I'm using is a HK 90A boat esc. I do not recommend this esc because it may brake hard if you reaplly the throttle while the board is coasting.

Maybe you can use someone else his esc/motor to test what is wrong. Or even test your arduino code on some small drone motor/esc?
```

---
## \#14 Posted by: michaeld33 Posted at: 2016-06-09T14:30:56.220Z Reads: 26

```
I have a multirotor, so I may be able to test it on that. My next idea is to use the remote control from my quadcopter to control the esc, and see if something changes. I also want to try another ESC. Unfortunately, I CNC'd my mount for the board, and the bolt hole pattern is specific, if I can find another motor which has the same bolt hole pattern I could look into that. Bolt holes are 32mm apart. NTM Prop drive is 30mm apart... Damn.
```

---
