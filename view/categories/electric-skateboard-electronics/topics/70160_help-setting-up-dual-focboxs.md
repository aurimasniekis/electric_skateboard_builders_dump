# Help setting up dual focboxs

### Replies: 20 Views: 230

## \#1 Posted by: kylem21 Posted at: 2018-10-04T18:23:33.045Z Reads: 94

```
Hi I have been stuck working on bldc tool for about 2 days now and I still can't figure out what the problem is. I am setting up 2 focbox's on foc and I seem so have figured out every step except for measuring the pulse width.
![53%20PM|690x382](upload://q1M0uPgcMOycnsrYVYbv4XIVIdD.png) ![14%20PM|690x389](upload://ki0TMWlLil0VuOFCV06lTP4vqhH.png) ![29%20PM|690x378](upload://noFNbhJWBinQ2HCRdlq6EV8jmdv.png) ![10%20PM|690x391](upload://6NFfZyZiMtQHbyDx85qmclH2RJ1.png) ![24%20PM|690x375](upload://eAchazt7i2d5KWnNmBYFbnNeWrC.png) ![43%20PM|690x380](upload://xqYuiBUGOKLaqgoqh5oSEanWrVa.png) 
these are my settings for the master and slave 
I can get both motors to spin one at a time with my keyboard but I cannot get the remote to spin the motors. maybe it is an issue with my gt2b binding? I followed the instructions to bind it and the receiver stays solid red when both are on but my remote is slowly blinking green. Any help would be greatly appreciated :grin:
```

---
## \#2 Posted by: barajabali Posted at: 2018-10-04T19:01:13.980Z Reads: 72

```
In your app config tab, your control mode is disabled. Change it to current no reverse with brake.

You will need to bind your gt2b. Can can tell if it’s binding by looking at the display bar while connected
```

---
## \#3 Posted by: kylem21 Posted at: 2018-10-04T19:37:44.993Z Reads: 66

```
Do I set the control mode to that in the master and slave? 
I don’t think I’ve been able to bind the remote because the display bar hasn’t moved
```

---
## \#4 Posted by: barajabali Posted at: 2018-10-04T19:41:10.045Z Reads: 61

```
Both always do everything on both. 

There is a guide on YouTube for how to bind that remote
```

---
## \#5 Posted by: Andy87 Posted at: 2018-10-04T20:01:37.808Z Reads: 56

```
Sounds like you in the wrong channel on your receiver.
If I remember right it should be ch2
```

---
## \#6 Posted by: kylem21 Posted at: 2018-10-04T20:17:22.637Z Reads: 52

```
I start with the bind plug in channel 3 and the ppm cord to channel 2. Then I hold the bind button and turn on the remote. The receiver turns solid red and the remotes green light starts blinking. I then turn receiver off, controller off, unplug bind key, controller on, receiver on. 
The remote stays blinking green and receiver is solid red
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-04T20:21:47.238Z Reads: 51

```
If the receiver is solid red it means you definitely bind both.
But usually it’s green solid light.
Maybe it’s the battery indicator for low battery.
Did you charge it up?
Double check also if the wires on the receiver in the right order.
If that’s all not the case than try ch1 😅 maybe I was remembering it wrong 😬
```

---
## \#8 Posted by: barajabali Posted at: 2018-10-04T20:32:39.416Z Reads: 46

```
Show me a picture of the receiver while plugged
```

---
## \#9 Posted by: kylem21 Posted at: 2018-10-04T20:38:49.339Z Reads: 46

```
![image|375x500](upload://7sXW62PVR91FwmqSMWBTMbVp50Y.jpeg)
This is after I remove bins plug
```

---
## \#10 Posted by: barajabali Posted at: 2018-10-04T20:40:40.226Z Reads: 45

```
I asked you to do this so I could see the wire orientation. Is the wire in the 2nd channel and in the correct orientation? Negative on the left according to picture
```

---
## \#11 Posted by: kylem21 Posted at: 2018-10-04T20:56:22.562Z Reads: 39

```
:sweat_smile: it appears my ppm cable flipped inside the little sheath I made so that’s why I couldn’t calibrate the remote, haha thank you. 
But now when I pull the throttle, only one motor spins and only In reverse
```

---
## \#12 Posted by: barajabali Posted at: 2018-10-04T20:57:07.662Z Reads: 41

```
Glad I could help, were getting somewhere now. 

Okay so are you running split ppm or canbus?

The motor is spinning backwards- You need to flip two of the 3 phase wires and then run your detection's again
```

---
## \#13 Posted by: kylem21 Posted at: 2018-10-04T21:24:35.047Z Reads: 36

```
For some reason the motor accelerates only when I move the remote to the reverse position. When I squeeze down to move forward the display shows it going to brakes. Also the motors stuttering when it does move sometimes
```

---
## \#14 Posted by: barajabali Posted at: 2018-10-04T21:29:32.008Z Reads: 36

```
Did you make the control mode on them both current no reverse with brake
```

---
## \#15 Posted by: kylem21 Posted at: 2018-10-04T21:46:07.847Z Reads: 32

```
Yeah I did, both of them now spin in the forward direction when I put the throttle in reverse and don’t move when pull the throttle to accelerate
```

---
## \#16 Posted by: barajabali Posted at: 2018-10-04T21:50:43.212Z Reads: 31

```
That means that your remote throttle is flipped. Flip one of those switches on your remote until you find which one it is
```

---
## \#17 Posted by: kylem21 Posted at: 2018-10-04T22:33:32.740Z Reads: 29

```
Okay just got it to go in the right direction but when I put reverse the motors spun fast in reverse without me touching the throttle until I turned off the battery
```

---
## \#18 Posted by: barajabali Posted at: 2018-10-04T22:45:22.531Z Reads: 29

```
You need to calibrate your remote in the app configuration
```

---
## \#19 Posted by: kylem21 Posted at: 2018-10-04T23:12:24.695Z Reads: 29

```
I coppied the max and min pulse width into the master but the motors are only going when I tap the reverse then they spin really fast in reverse
```

---
## \#20 Posted by: barajabali Posted at: 2018-10-04T23:13:55.422Z Reads: 29

```
You need some help I think. I can get on a teamveiwer with you if you want. I have a few minutes.
```

---
