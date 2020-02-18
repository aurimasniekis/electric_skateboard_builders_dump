# HELP &#124; ESC/ MOTOR issue

### Replies: 26 Views: 2479

## \#1 Posted by: shaohad Posted at: 2016-04-01T10:37:07.519Z Reads: 118

```
hello, this is my setup

10S battery pack
turnigy 6364 213 kv motor
diyelectricskateboards trucks and hardware
wiiciver
5V battery pack (power the wiiciver)
turnigy k-force 120A 8S-12S ESC
remote: nyko nuncheck 
problem:

when i connect everything , motor keep beeps but wont turn.

what i have check ot tired to do:
- i tries to run with 6S battery pack and 6S ESC and working well.
- with servo tester the system fires up and motor is spining.

any idea?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-04-01T18:18:03.896Z Reads: 104

```
Don't think it's recognizing the wiiceiver ... Did you try using a different hand controller? Or plugged incorrectly
```

---
## \#3 Posted by: thisrealhuman Posted at: 2016-04-01T18:29:16.308Z Reads: 101

```
I'm also using the K-force 120A, if the beeps are once every 1.5 seconds, you have no signal from the Tx/Rx. If the beeps are 4 beeps per second, its' asking for your throttle range. It should be as simple as pulling the throttle to max and then brake to max. I've always used the GT2B so nunchucks are outside my experience.
```

---
## \#4 Posted by: shaohad Posted at: 2016-04-01T18:40:04.997Z Reads: 94

```
thanks for replaying.
i also tried with 12S freind ESC and it worked.
i have 2 nuncheks , and as mentioned i have tried with 6S esc and also with 12S freind ESC both worked.
whitch means wiicive battery pack, remte and motor are good and well functioning.
i think it beeps every 1.5 seconds.

any more ideas?
```

---
## \#5 Posted by: shaohad Posted at: 2016-04-01T18:41:41.795Z Reads: 85

```
sorry my bad i didnt tried 12S esc , but i did tired to swap the wiiciver with 2.4ghz reciver and transmitter and it worked.
i am pritty sure its the ESC cusing the issue but i have no idea how to solve
any ideas?
```

---
## \#6 Posted by: Ulfberht Posted at: 2016-04-01T20:15:31.437Z Reads: 81

```
I'd go over the whole ESC very carefully and look for wires with shorts or anything that might be a problem. With electronics it could be something as simple as a shorted wire. Also look for signs of burning or heat damage. Give it a good sniff to see if it smells like it's been too hot for too long.
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-04-01T20:44:13.254Z Reads: 77

```
Ahhh....nothing better than the smell of burnt wiring in the morning 🌅
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-04-01T20:45:53.062Z Reads: 73

```
So you're saying swapping out the reciver made it work?
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-04-01T20:49:10.699Z Reads: 73

```
For some reason sometimes the wiiceiver has a hard time working with different ESCs and doesn't recognize it...dunno why..never bothered to find out
```

---
## \#10 Posted by: laurnts Posted at: 2016-04-01T22:15:33.533Z Reads: 72

```
I am using similar esc with yours. It seems that your esc doesnt detect any RX / TX module and or connections, 90% this is the cause of the 1.5s motor / esc beeps.
```

---
## \#11 Posted by: shaohad Posted at: 2016-04-02T06:22:07.942Z Reads: 68

```
yea well it dosent reconize the wiiciver and it didnt reconize my freind 2.4ghz reciver + transmitter.

i dont think there are shorts, and as mention with simple servo tester and same ESC its working, so im super fusrated.
any more ideas?
```

---
## \#13 Posted by: shaohad Posted at: 2016-04-03T16:08:22.372Z Reads: 59

```
any one? any more ideas?
```

---
## \#14 Posted by: laurnts Posted at: 2016-04-03T16:28:50.299Z Reads: 63

```
First you have to test your nunchuck if it works (easy if you have wii) or find friends who have. If it doesnt work then you know your nunchuck doesnt work and might return it for warranty. If it works fine, than the wiiceiver is the one that doesnt work. As it appears that you get this from diyelectricskateboard (I hope I am right), you can contact @torqueboards for help.
```

---
## \#15 Posted by: shaohad Posted at: 2016-04-03T17:36:48.622Z Reads: 57

```
i have tested both with freind 6S system and both work
```

---
## \#16 Posted by: lox897 Posted at: 2016-04-03T21:13:18.798Z Reads: 57

```
Are you able to post a picture of your wiring and your UBEC (The thing that powers the receiver)?
```

---
## \#17 Posted by: torqueboards Posted at: 2016-04-04T07:00:55.872Z Reads: 55

```
@shaohad - As I mentioned to you. I can refund you for the Wiiceiver and you can keep it. We test these prior to shipping them out. Not sure, why yours would not work. Contact me. Hopefully, you get it working however.
```

---
## \#18 Posted by: shaohad Posted at: 2016-04-04T09:54:03.674Z Reads: 54

```
i do not use ubec.
i use 5V battery pack to power up the wiiciver.
what does it means if it keep beeping every sec? not slow beeping but very fast beeping
<img src="/uploads/db1493/original/2X/d/d98d7d40a53eba53d4f26a6b7e843488eb17b75c.jpg" width="666" height="500">

attched picture
```

---
## \#19 Posted by: lox897 Posted at: 2016-04-04T11:03:29.114Z Reads: 52

```
Are you able to try a different 5v power source? I had the same problem of beeping and it was because my UBEC was broken. It may also be the connection between the esc and receiver.
```

---
## \#20 Posted by: shaohad Posted at: 2016-04-04T11:31:33.671Z Reads: 51

```
dont have other 5v power source , but wiciver turn on and i measuered it with multi meter and the voltage is 5.2v
its not the problem

What do you mean by say— conection between the esc and reciver , what could be wrong?
```

---
## \#21 Posted by: lox897 Posted at: 2016-04-04T21:06:01.266Z Reads: 48

```
Is the data cable in the servo connector properly? Some one had that problem.
```

---
## \#22 Posted by: shaohad Posted at: 2016-04-05T05:23:28.580Z Reads: 43

```
i have followed the insturctions on diyelectric skateboard site
still same problem.
how should i connect it?
```

---
## \#23 Posted by: torqueboards Posted at: 2016-04-05T05:33:24.088Z Reads: 45

```
Usually beeping noise is the ESC can't find the remote.
```

---
## \#24 Posted by: shaohad Posted at: 2016-04-05T05:48:53.152Z Reads: 46

```
i know for sure all those are ok becuase test on my freind setup

battery pack, remote and dongle, motor, 5V battery pack (replace ubec).

any ideas? im really start to loose hope
can anyone explain how should connect esc to wiiciver when using 5V p.s and not ubec?
```

---
## \#25 Posted by: lox897 Posted at: 2016-04-05T20:24:21.140Z Reads: 42

```
Have you tried switching the two cables of the 5v battery pack and the esc? Are you sure they are in the correct order?
```

---
## \#26 Posted by: lox897 Posted at: 2016-04-05T20:25:13.380Z Reads: 41

```
Does the wiiceiver light up when your board is turned on?
```

---
## \#27 Posted by: shaohad Posted at: 2016-04-05T20:42:38.637Z Reads: 41

```
Yes it is .................
```

---
