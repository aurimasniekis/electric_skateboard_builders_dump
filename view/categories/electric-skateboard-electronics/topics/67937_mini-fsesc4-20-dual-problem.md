# Mini FSESC4.20 dual problem

### Replies: 37 Views: 741

## \#1 Posted by: gaetjen Posted at: 2018-09-13T18:39:48.271Z Reads: 210

```
So, I bought two mini FSESC4.20 and I connected them via CAN. I set up everything:
Master > ID-0, send over can: no, multiple escs over can: yes
PPM with UART, and can cable plugged in
Slave > ID-1, send over can: yes, multiple escs over can: no
no app

Now, only the master motor spins. I did everything again. Ackmaniac 3.102 firmware. Motor detection, etc. Again the same. Only one motor spins. I even soldered the can cable direkt to the pins. Still no.
Does anyone have any ideas? I used to run dual VESC 4.12 with no problem before that.
@BensonYong
```

---
## \#2 Posted by: Silverline Posted at: 2018-09-13T18:42:53.234Z Reads: 206

```
Try follow this guide : https://youtu.be/VPhExzFXeQo
```

---
## \#3 Posted by: L3chef Posted at: 2018-09-13T18:46:20.961Z Reads: 198

```
Did you plug in the canbus wire while power was on?
```

---
## \#4 Posted by: gaetjen Posted at: 2018-09-13T19:08:28.231Z Reads: 188

```
No, everything was connected beforehand
```

---
## \#5 Posted by: gaetjen Posted at: 2018-09-13T19:11:06.789Z Reads: 182

```
That´s exactly what I did. But still only one motor spinning
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-09-13T19:27:47.637Z Reads: 169

```
do they work individually?
```

---
## \#7 Posted by: gaetjen Posted at: 2018-09-13T19:29:13.602Z Reads: 166

```
Yes, they do
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-09-13T19:30:07.354Z Reads: 166

```
well, i run mine over split ppm, so no real expierence in can bus mode
```

---
## \#9 Posted by: L3chef Posted at: 2018-09-13T20:10:48.746Z Reads: 157

```
Try switching master to slave and vice versa
```

---
## \#10 Posted by: gaetjen Posted at: 2018-09-13T20:14:53.129Z Reads: 153

```
good idea. I´ll try that tomorrow!
```

---
## \#11 Posted by: Andy87 Posted at: 2018-09-13T20:27:00.757Z Reads: 149

```
Don’t you need to set „multiple vesc over can“ in master and slave to yes? 🤔
```

---
## \#12 Posted by: L3chef Posted at: 2018-09-13T20:30:49.394Z Reads: 146

```
Nope only master
```

---
## \#13 Posted by: Andy87 Posted at: 2018-09-13T20:32:38.354Z Reads: 147

```
I thought I have set it in both 🤔
Nu ok thx for clearing this up
```

---
## \#15 Posted by: gaetjen Posted at: 2018-09-14T09:04:33.386Z Reads: 133

```
tried the switching. Did not work either
```

---
## \#16 Posted by: L3chef Posted at: 2018-09-14T09:11:25.654Z Reads: 134

```
Probably a dull vesc. You can split ppm if you don't need canbus. But probably better to send ut back
```

---
## \#17 Posted by: BensonYong Posted at: 2018-09-18T01:22:43.489Z Reads: 116

```
Hi man.Sorry, I didn't reply to you in time. Has your problem been solved?
```

---
## \#18 Posted by: ervinelin Posted at: 2018-09-18T01:32:09.847Z Reads: 111

```
What I did was turn the switch to off first.. 

Then I ran the connection wizard for both escs, one for master, one for slave. The slave one has to be set to a different ID the. The master. Somehow the wizard worked better than when I tried doing this myself.

After this is done, turn switch back on (power down first). Then give it another go.

Incidentally I usually do all the motor detection separately too..
```

---
## \#19 Posted by: gaetjen Posted at: 2018-09-18T07:35:55.446Z Reads: 103

```
Not yet, seems like the CAN doesn´t work. Is there any way I can check, if the connection is working?
```

---
## \#20 Posted by: gaetjen Posted at: 2018-09-18T07:36:57.183Z Reads: 99

```
How can I run configure the ESC when the power is off? 
The problem is that both esc work on their own, but not in dual.
```

---
## \#21 Posted by: ervinelin Posted at: 2018-09-18T08:05:11.862Z Reads: 98

```
No I mean when u swap the USB cable turn off the power...

Setup using the wizard for both master and slave.

Incidentally, you are testing the motor movement with a remote?
```

---
## \#22 Posted by: DeathByBacon Posted at: 2018-09-18T08:12:46.578Z Reads: 91

```
Have you tried  multiple escs over can: YES on the master and slave?
```

---
## \#23 Posted by: BensonYong Posted at: 2018-09-18T08:37:36.477Z Reads: 87

```
We have received the feedback video from you and we will resolve your issue as soon as possible.
```

---
## \#24 Posted by: gaetjen Posted at: 2018-09-18T08:38:58.320Z Reads: 90

```
Yeah, did that.
@DeathByBacon: Tried that as well. Didn´t work
```

---
## \#25 Posted by: gaetjen Posted at: 2018-09-19T12:58:34.501Z Reads: 82

```
Does anyone know how I can check, if the CAN connection is working?
```

---
## \#26 Posted by: ervinelin Posted at: 2018-09-19T19:35:01.034Z Reads: 78

```
I wonder if u can test for connectivity using a multimeter on the CANBUS pins across the two escs... Just to make sure that they are indeed internally connected via the switch...

EDIT: I apologies, I re-read your post, you bought TWO mini VESCs... I thought you had the DUAL VESCs... apologies.. In this case make sure you connect the CANBUS wire in the correct order.
```

---
## \#27 Posted by: gaetjen Posted at: 2018-09-19T19:52:26.867Z Reads: 77

```
I just connected the two middle pins, but it doesn´t work
```

---
## \#28 Posted by: ervinelin Posted at: 2018-09-19T23:40:40.172Z Reads: 70

```
Did u connect the right pins to each other?
```

---
## \#29 Posted by: gaetjen Posted at: 2018-09-20T07:07:41.207Z Reads: 63

```
![19|281x500](upload://iu3P05BPdGT3qriBUrUotcgVwz.jpeg)
```

---
## \#30 Posted by: ervinelin Posted at: 2018-09-20T08:28:06.393Z Reads: 59

```
Running out of ideas... Are the two ESCs grounded to each other? (e.g. share the same battery).

Also, are you using your remote to check if they spin in unison or the VESCtool desktop app?
```

---
## \#31 Posted by: gaetjen Posted at: 2018-09-20T08:32:51.674Z Reads: 59

```
Tried everything. Running out of ideas as well. Gemma from flipsky now told me I should send them back
```

---
## \#32 Posted by: linsus Posted at: 2018-09-20T08:43:53.377Z Reads: 56

```
Make sure thats not a cold solder on the CAN connector..looks abit suspicous..
```

---
## \#33 Posted by: gaetjen Posted at: 2018-09-20T08:46:20.074Z Reads: 56

```
Had a normal can bus cable on it before which worked fine on another setting. Solder is solid
```

---
## \#34 Posted by: ervinelin Posted at: 2018-09-20T09:07:54.716Z Reads: 55

```
What do u mean the cable worked fine before on another setting?
```

---
## \#35 Posted by: gaetjen Posted at: 2018-09-20T09:12:11.632Z Reads: 56

```
I had two tb vescs for two years connected via can before that. Then, one vesc blew up and the other one didn't work properly, so I switch to flipsky vesc
```

---
## \#36 Posted by: gaetjen Posted at: 2018-09-21T22:38:05.442Z Reads: 41

```
So, I couldn´t get the two ESCs to work in dual mode, but they offerend me to send it back and refund my money for store credit and they pay for the shipping.  Will order the 6.6 dual next and hope that I will work :slight_smile:
```

---
## \#37 Posted by: Flashgod224 Posted at: 2018-09-21T23:22:38.629Z Reads: 36

```
I used to have that issue, I solved it by changing my cables be cause the CAN connector wires was a dud for some reason.
```

---
## \#38 Posted by: ervinelin Posted at: 2018-09-21T23:28:42.202Z Reads: 34

```
He soldered the pins directly and still couldn't get it to work...
```

---
