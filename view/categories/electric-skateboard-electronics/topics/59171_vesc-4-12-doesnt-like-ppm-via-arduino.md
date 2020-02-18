# VESC 4.12 doesn&rsquo;t like PPM via Arduino

### Replies: 21 Views: 620

## \#1 Posted by: AchimWurm Posted at: 2018-06-17T11:33:06.742Z Reads: 102

```
Hey,
I have a selfmade VESC 4.12 (currently) using Ackmaniacs modded FW 3.102. Somehow, I am not able to make the VESC eat my PPM signal.
I am using an Arduino Nano v3 and generate the signal using the Servo library. This is for testing purposes and thus very (very) basic.

    #include <Servo.h>

    #define serial Serial

    Servo ppm;
    int poti = A0;
    int poti_wert = 0;
    int ppm_wert = 0;
    int pwm = 6;

    void setup() {

    pinMode(6, OUTPUT);  
    serial.begin(115200);
    ppm.attach(5, 1000, 2000);


    }

    void loop() {

    poti_wert = analogRead(poti);
    delay(1);
    analogWrite(pwm, poti_wert / 4);
    poti_wert = map(poti_wert, 0, 1023, 1000, 2000);
    ppm.writeMicroseconds(poti_wert);
    serial.println(poti_wert);
    delay(1);
    }


Here is what the ESC-Tool reading looks like:
![nano_ppm|690x426](upload://8QZaTWR1AKdQbh77dLkhKH4ofW3.gif)

A simple PWM output via analogWrite doesn't work at all...

I would really appreciate advise on how to get a clean reading.

Thanks and greetings :slight_smile:
```

---
## \#2 Posted by: ervinelin Posted at: 2018-06-17T11:39:11.224Z Reads: 83

```
You are doing it wrong... You should be writing servo commands not analogue write.

Check for @solidgeeks remote or mine both run arduinos.
```

---
## \#3 Posted by: AchimWurm Posted at: 2018-06-17T12:04:56.667Z Reads: 81

```
Thanks for the reply.
I bet I'm doing something wrong :wink:. Just don't exactly know what. Isn't the ppm.writeMicroseconds function what I need? I had a look at solidgeeks remote and as well compared my code with yours. I still don't get the important difference.

Btw.: Scoping the signal doesn't show any noise :face_with_raised_eyebrow:
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-06-17T12:05:53.728Z Reads: 77

```
Make sure you’re looking Solid’s developer branch not master
```

---
## \#5 Posted by: ervinelin Posted at: 2018-06-17T12:10:12.398Z Reads: 78

```
Why do you have both an analogwrite and a millisecond write?
```

---
## \#6 Posted by: AchimWurm Posted at: 2018-06-17T12:17:39.573Z Reads: 72

```
Testing purposes. Thought it doesn't hurt to have a look at what happens by passing over a simple PWM - turned out it doesn't work at all :roll_eyes:
Right now I'm digging through solidgeeks dev branch as @Jc06505n recommended. But as far as I can tell, he uses this here

    esc.attach(throttlePin);
    esc.writeMicroseconds( map(throttle, 0, 1023, 1000, 2000) );

what should be pretty much be the same I'm doing (or trying to do?).
```

---
## \#7 Posted by: pat.speed Posted at: 2018-06-17T12:28:32.115Z Reads: 63

```
Why don’t you start off with the simple sweep or knob example and that way you can make sure it works first, then try modifying it
```

---
## \#8 Posted by: AchimWurm Posted at: 2018-06-17T12:38:44.065Z Reads: 64

```
Thanks @pat.speed, but thats what I did. Maybe I should be more precise about what the problem is. I am able to scale the ppm signal in the defined range. I can see it in the ESC-Tool reading (shown above, the reading moves from left to right and back as I am turning the potentiometer) and I can verify it using a scope.
This nervous jittering around +/-5% of the signal is what I am worried about :neutral_face:
```

---
## \#9 Posted by: pat.speed Posted at: 2018-06-17T12:40:34.089Z Reads: 64

```
Ahhhb nah that’s pretty normal, even happens a bit on my remote. Make sure you set the neutral deadband around 15% and you’ll be fine. Have you tested it with motors connected?
```

---
## \#10 Posted by: AchimWurm Posted at: 2018-06-17T12:45:13.739Z Reads: 59

```
No, too afraid of scary things that might happen :roll_eyes:
Ok, give me a minute...

Update: Well, you are right. Works. Seems like my problem was located somewhere else.
What happened in this thread stays in this thread :shushing_face:

Thanks again guys!
```

---
## \#11 Posted by: pat.speed Posted at: 2018-06-17T12:59:07.278Z Reads: 53

```
It does look a little bit jumpy-er than usual, maybe there is a way to kinda smooth out the pulses from the arduino? I’m not very good with arduino but maybe a filter of some sort to slow the pulses
```

---
## \#12 Posted by: AchimWurm Posted at: 2018-06-17T13:36:55.409Z Reads: 46

```
Indeed. Now I got some soldering to do and maybe give it a test ride tomorrow. I get back here after that :slight_smile:
```

---
## \#13 Posted by: MaxMaker Posted at: 2018-06-20T20:56:19.606Z Reads: 35

```
I am trying the same with a VESC 6.4. My code reliabily makes a small servo move, but when I connect gnd and Signal of the VESC, nothing happens. The BLDC tool shows no values. Not even random ones.
```

---
## \#14 Posted by: AchimWurm Posted at: 2018-06-21T08:03:01.393Z Reads: 31

```
I'm back. Everything went pretty well. Had to increase the deadband to 17% though. Approx 10km ride with no issues at all.

@MaxMaker
I don't know your wiring but I power my arduino based receiver via a BEC due to the vesc's power supply beeing very noisy. I only connected the ppm wire to the vesc.
In your case you mos defnhave to connect 5V in addition to GND and signal ;D.
I'm planing on soldering a vesc 6 but for now I can't say much about the 6's power supply.
```

---
## \#15 Posted by: MaxMaker Posted at: 2018-06-21T21:00:18.094Z Reads: 21

```
So my VESC is connected to the Arduino only via Gnd and Signal. I know I cannot connect the +5V since then two power supplies are fighting each others. 

I just cannot get any readings in the throttle mapping part of the VESC tool. Very frustrating. I am out of ideas...
```

---
## \#16 Posted by: wafflejock Posted at: 2018-06-21T21:19:29.677Z Reads: 24

```
@AchimWurm would suggest taking out the serial communication once you're done debugging through the serial port and see if it helps smooth out the signals getting sent to the VESC, the Serial communication seems to add a surprising amount of overhead.  @MaxMaker would suggest sharing your arduino code so others can give it a go or let you know if something is weird in the code that might cause issues.  Make sure in the VESC tool you have real time app data active as well if you aren't seeing any motion whatsoever.  Last thing I'd suggest is getting your hand on an oscilloscope either borrow one or get one of the ultracheap ones on amazon or elsewhere (jbtek brand ones are very cheap, I built a kit one for fun and it works great for these types of simple things)
```

---
## \#17 Posted by: MaxMaker Posted at: 2018-06-21T21:33:19.112Z Reads: 22

```
Here is a video of the Setup with proof that PPM is working at least on a servo. 

https://youtu.be/xz4k2G3NhTQ
```

---
## \#18 Posted by: AchimWurm Posted at: 2018-06-21T21:35:48.794Z Reads: 22

```
Of course. No bloat code active :relieved:
Stuff for further investigation... But for now I'm trying to figure why the vesc doesn't like 10s. But thats a whole nother story. Other stuff for another thread :wink:
```

---
## \#19 Posted by: AchimWurm Posted at: 2018-06-21T21:43:27.696Z Reads: 20

```
As @wafflejock mensioned - can you provide your arduino code and some sort of wiring diagram? Like a table of what goes to what.
```

---
## \#20 Posted by: wafflejock Posted at: 2018-06-21T22:22:08.200Z Reads: 20

```
Okay so at this point my only guess is something in the vesc tool isn't turned on... I think you only need "RT/App" turned on... I need to hook up my old vesc here though and upgrade the firmware to see what exactly happens with that wizard.
```

---
## \#21 Posted by: wafflejock Posted at: 2018-06-21T22:45:50.573Z Reads: 20

```
Just went through the setup here and using the input wizard I didn't have to start anything in advance to see the input start showing up.  The RTApp selection is only needed if you go into the App Settings -> PPM -> Mapping section, it seems.

---

https://youtu.be/fiioWswwRts

---

Also my code is on github
https://github.com/shusain/eskatecontroller
```

---
