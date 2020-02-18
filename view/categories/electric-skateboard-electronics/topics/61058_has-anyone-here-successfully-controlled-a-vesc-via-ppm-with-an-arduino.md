# Has anyone here successfully controlled a VESC via PPM with an Arduino?

### Replies: 16 Views: 1570

## \#1 Posted by: MaxMaker Posted at: 2018-07-06T13:32:28.403Z Reads: 177

```
I am trying to controll a VESC 6.4 with an Arduino Nano. The Nano is setup and can successfully control a little servo. What connections do I need to the VESC?


The Nano needs to be always powered on, so it is powered by an UBEC. Therefore I cannot have the VESC power the Arduino. 

Unfortunately one VESC already broke during my first attempt. Either it was my fault or it was already faulty. The VESC ended up powering the Nano over Signal and GND which is strange.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-07-06T13:36:27.822Z Reads: 174

```
Not sure how the nano could be powered by the signal wire so maybe check your wiring to the Vesc. Also please search for answers as there are multiple threads already about remotes using arduino chips
```

---
## \#3 Posted by: MaxMaker Posted at: 2018-07-06T13:44:35.728Z Reads: 166

```
I checked dozens of times. I guess at that point the VESC was sonewhat faulty.
```

---
## \#4 Posted by: faithfulpuppy Posted at: 2018-07-06T13:52:42.317Z Reads: 156

```
why does the arduino have to always be on? wouldn't that drain your battery over time? and the VESC has a 5v output already
```

---
## \#5 Posted by: MaxMaker Posted at: 2018-07-06T13:54:31.954Z Reads: 147

```
Because this is for an electric surfboard and the Arduino controls a lot of components other than the VESC. Among others a big 12V relay to cutoff the lipos.
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2018-07-06T13:56:19.042Z Reads: 143

```
ah, i see. But wouldn't you want the board to be either on or off anyway? What makes a esurf different from an eskate?
```

---
## \#7 Posted by: MaxMaker Posted at: 2018-07-06T13:59:33.203Z Reads: 135

```
It is similar, but a boat could go in circles for 30min if it goes out of control. So I need safety features. I also need a lot of power for relays and I don’t know how much the VESC can supply and I need 12V. The Arduino also performs the Anti Spark Routine. So it naturally needs to be powered on first.

Here are some details: https://youtu.be/fmtj-cBmLJQ
```

---
## \#8 Posted by: DougM Posted at: 2018-07-06T14:49:43.255Z Reads: 122

```
Are you married to PPM?  I controlled my 4.12's with a Teensy 3.2 using Serial and it worked well.  I've not tried it with VESC6, though.
```

---
## \#9 Posted by: MaxMaker Posted at: 2018-07-06T16:39:48.691Z Reads: 109

```
Yes. I can code and troubleshoot ppm, but not serial. The UART code I have seen is 5x as large as my current code too.
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-07-06T17:04:43.016Z Reads: 104

```
Yes, it is completely doable.

It's very very simple, you can use the same code that you use to control a servo. Just make sure it defaults to  a neutral PPM signal.

You will of course have to go through the normal vesc PPM setup by defining the bounds of the signal.
```

---
## \#11 Posted by: MaxMaker Posted at: 2018-07-06T17:50:09.978Z Reads: 99

```
And how? I am using the Arduino Servo library. The Servo already moves when I move the trigger.
```

---
## \#12 Posted by: TowerCrisis Posted at: 2018-07-06T20:29:13.196Z Reads: 90

```
It's exactly the same and uses the same wiring. Just don't connect the positive lead to the vesc, only use negative and signal.


In the code just make sure that the signal defaults to the middle position (ie if it has a position value range of 0-180, set it to 90)
```

---
## \#13 Posted by: junwoo091400 Posted at: 2018-07-07T15:46:10.930Z Reads: 70

```
Yeah, I guess your vesc will detect servo library's signal in range [1200, 2200]. Which is 200 ms off. But you can set that boundary inside bldc-tool -> App Configuration -> PPM window.

+) DON'T use Servo.write() function. Use Servo.writeMicroseconds() Instead. It is much more accurate. (https://www.arduino.cc/en/Reference/ServoWriteMicroseconds)
```

---
## \#14 Posted by: MaxMaker Posted at: 2018-07-08T11:36:54.947Z Reads: 51

```
Thanks for the tip, that is easy to change. Have you got any ideas how to establish some safety in the circuit? Like diodes or 10k ohm resistors? I don’t want to blow another Vesc. Again not sure if I blew it or if it was blown already.
```

---
## \#15 Posted by: junwoo091400 Posted at: 2018-07-08T12:37:14.045Z Reads: 44

```
Well I have not blown up any VESC so far.

 I think setting adequate (supplier recommended) **Maximum Current** for Battery & Motor should prevent any big damage.
 Also, software-wise, **set Maximum duty-cycle around 0.95**. If you set it to 1.0, program will be unstable, and (in theory) the mosfets that get stuck being ON can draw too much current and burn out. Causing battery short, which in your case will be prevented by the Fuse(that's massive).

Those are the 2 tips I remember being posted from people who had their VESCs blown.

***
About 'safety', hmm... I don't have a good idea. Since VESC already has setting to 'ignore' PPM value if wrong inputs are made for certain period of time. So if you have PPM signal disconnected, VESC would stop the motors(I just tested it and it does).
***
So I think if you set up critical VESC settings properly, any BIG(Fire, Explosion, Surf-board running away from you) Problems would not happen :) .

Nice Fiberglass job by the way! is your job related to FRP, or did you learn it to make stuff?
```

---
## \#16 Posted by: wafflejock Posted at: 2018-07-08T14:48:23.061Z Reads: 41

```
I've been using a custom receiver and remote for a couple of years now can take a look at my code here: https://GitHub.com/shusain/eskatecontroller/

I explain in the readme there a bit about how I set things up.  Using Arduino pro mini 3.3V makes it easier to use the 5V from the VESC but from skimming the thread here it appears you're powering it separately anyhow.   If you are doing wireless control let me know there are some extra details for safeties you can add there, otherwise ignore parts of my code about radio.
```

---
