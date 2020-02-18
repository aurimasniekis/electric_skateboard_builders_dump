# Arduino (Teensy 3.2) Power Issue

### Replies: 10 Views: 315

## \#1 Posted by: anorak234 Posted at: 2019-03-21T01:42:47.940Z Reads: 72

```
So I've been learning quite a few things recently, and have gotten into coding and the Arduino world. I am trying to put LED lights on my commuting board, and have gotten so far as to get everything working exactly how I want it when powered by my laptop. The LEDs turn on, do the pattern that they're supposed to, and then repeat indefinitely. However, the problem comes when I try to power it off of my battery. I purchased a 12V/24V to 5V 1A buck converter, and then chopped a micro usb to wire everything up. I made sure the wiring is correct, popped it in, turned it on, and nothing happened. Anybody have any idea what the issue could be?

![IMG_1265|375x500](upload://naQ7o6VM34EuzorKDvQVrZe6Qla.jpeg) ![IMG_1266|375x500](upload://8eS4zZ0Fs7ep9w1HJA4CvOCaqC0.jpeg) ![IMG_1268|666x500](upload://2AXdxutKMv3zukDVZvn9aSwNffv.jpeg) ![IMG_1272|666x500](upload://fcdgYMY6VLjmKjcNGVbYh9MniYc.jpeg) ![IMG_1273|666x500](upload://p1YWaRaF9Iref1zCLS5xFC3xVaY.jpeg)
```

---
## \#2 Posted by: threebysix Posted at: 2019-03-21T01:57:39.820Z Reads: 59

```
First, test for power. Take a volt meter to the buck converter's 5v output when the board is switched on and see if you have 5v coming out.
```

---
## \#3 Posted by: surferboy120 Posted at: 2019-03-21T04:29:20.211Z Reads: 55

```
Its either not getting power or the wrong amount of power.  I agree 5v check first
```

---
## \#4 Posted by: anorak234 Posted at: 2019-03-21T18:05:23.329Z Reads: 42

```
@threebysix @surferboy120  
Checked the converter, it's outputting 5.08V. According to the teensy website it can take 5V and I doubt that 0.08V is enough to make that kind of difference.
```

---
## \#5 Posted by: surferboy120 Posted at: 2019-03-21T18:26:24.222Z Reads: 39

```
@anorak234 look at using the VIN on the board its been awhile but I think thats for battery  you will need that.  When I get home I will try to look but you should look at the Teensy 3.2 pinout and see it on the opposite side of the board.   Please confirm  its use on the Teensy as I have not use that specific board but other Arduino boards.

UPDATE:I looked up the board and it looks like when running off battery you need to solder direct to the board.
```

---
## \#6 Posted by: olestra Posted at: 2019-03-21T19:34:38.125Z Reads: 31

```
some cheap converters will send a pulse of power, so to convert 12v to 5v it'll be something like 40% on 60% off. multimeter would show 5v coming out, but an O-scope would show the duty cycle. If that's the case, slapping a capacitor inline would fix the issue.
```

---
## \#7 Posted by: Pedrodemio Posted at: 2019-03-21T19:45:17.937Z Reads: 27

```
If it's anything like most Arduinos, when supplying 5V you should connect to the 5V port, not Vin

Vin usually need at least 7V since there is a voltage regulator
```

---
## \#8 Posted by: anorak234 Posted at: 2019-03-21T20:11:42.478Z Reads: 28

```
I figured it out! For whatever reason, the Teensy has a separate power circuit for external power sources vs USB, and somehow it could tell when I was using a hacked USB cable. Here is the correct wiring for external power at 5V:
 ![IMG_1291|666x500](upload://hsTFuvVmFHyVtsaKPf3VEdqcTkP.jpeg)
```

---
## \#9 Posted by: surferboy120 Posted at: 2019-03-21T21:29:37.080Z Reads: 24

```
Correct that is exactly where I was saying you needed to go for battery
```

---
## \#10 Posted by: Deodand Posted at: 2019-03-21T21:48:49.093Z Reads: 20

```
Often times USB will have a handshaking protocol before power delivery.... Though this is more common with newer USB. My guess is your USB cable didn't have continuity somewhere.
```

---
