# Slave motor starts turning then stops

### Replies: 36 Views: 681

## \#1 Posted by: Freddiecook Posted at: 2018-03-11T15:45:08.578Z Reads: 90

```
So my master vesc is running fine, by when I accelerate my slave vesc will accelerate for a second then stop all together until I give it 0 throttle and start again. I've tried changing the polls over and ran motor detection on it, when its doing the detection the motor spins exactly as it should. Any ideads?
Thanks in advance
```

---
## \#2 Posted by: bimmer Posted at: 2018-03-11T15:45:52.264Z Reads: 90

```
are they connected over can?
```

---
## \#3 Posted by: Freddiecook Posted at: 2018-03-11T15:46:07.170Z Reads: 88

```
Yes
10 char
```

---
## \#4 Posted by: bimmer Posted at: 2018-03-11T15:47:50.074Z Reads: 81

```
Does the cable wiggle? Does the motor spin after you set up slave/master and use the computer to spin the master?
```

---
## \#5 Posted by: Freddiecook Posted at: 2018-03-11T15:49:09.582Z Reads: 69

```
Cable is in fully and doesn't move. it was working fine but I left my board alone for a week or 2 and this happened.
Yes, when I run motor detection the motor spins as it should
```

---
## \#6 Posted by: bimmer Posted at: 2018-03-11T15:50:41.819Z Reads: 64

```
no arrow controls not detection
```

---
## \#7 Posted by: Freddiecook Posted at: 2018-03-11T15:50:42.615Z Reads: 64

```
When I give it some throttle the esc lights up as to say its receiving the signal okay
```

---
## \#8 Posted by: Freddiecook Posted at: 2018-03-11T15:51:26.324Z Reads: 66

```
I'll try that now
```

---
## \#9 Posted by: Freddiecook Posted at: 2018-03-11T15:55:47.403Z Reads: 64

```
When I use the arrow keys on BOTH of them they just judder back and forth. Forgot to mention im running it in FOC if that matters
```

---
## \#10 Posted by: bimmer Posted at: 2018-03-11T15:56:08.233Z Reads: 60

```
That is weird
```

---
## \#11 Posted by: bimmer Posted at: 2018-03-11T15:56:46.277Z Reads: 53

```
do you use vesc-tool or bldc tool?
```

---
## \#12 Posted by: Freddiecook Posted at: 2018-03-11T15:57:08.897Z Reads: 53

```
VESC tool
10 char
```

---
## \#13 Posted by: bimmer Posted at: 2018-03-11T15:57:31.186Z Reads: 54

```
Reflash them and re configure.
```

---
## \#14 Posted by: Freddiecook Posted at: 2018-03-11T15:58:09.193Z Reads: 53

```
When you say that do you mean use the wizard again?
I've tried that and nothing
```

---
## \#15 Posted by: bimmer Posted at: 2018-03-11T15:58:25.864Z Reads: 52

```
Firmware update
```

---
## \#16 Posted by: GrecoMan Posted at: 2018-03-11T16:05:08.539Z Reads: 50

```
hes on the latest FW already.

try downgrading to 2.18 and use BLDC tool
```

---
## \#17 Posted by: Freddiecook Posted at: 2018-03-11T16:06:10.382Z Reads: 52

```
Yeah I just tried reflashing anyway, I'll give this a go now
```

---
## \#18 Posted by: Freddiecook Posted at: 2018-03-11T16:12:42.031Z Reads: 51

```
BLDC tool makes you realise how easy the VESC tool is lol
I'm just confused as this was working a week or 2 ago
```

---
## \#19 Posted by: GrecoMan Posted at: 2018-03-11T16:13:14.243Z Reads: 51

```
LOL

are you using sensors?
```

---
## \#20 Posted by: Freddiecook Posted at: 2018-03-11T16:13:42.302Z Reads: 51

```
Yes
10 char
```

---
## \#21 Posted by: RedEagle Posted at: 2018-03-11T16:14:27.799Z Reads: 51

```
Have a look at your receiver and remote. I left mine alone to for a week and the battery holder on my remote was loose. Changed the batteries and fortified the battery holder. Now it works fine. Try swapping vescs and see if it helps.
```

---
## \#22 Posted by: RedEagle Posted at: 2018-03-11T16:15:14.272Z Reads: 48

```
For me bldc tool is easier than vesc tool, but maybe that's just me.
```

---
## \#23 Posted by: Freddiecook Posted at: 2018-03-11T16:22:07.662Z Reads: 46

```
I haven't been eboarding long, the controller seems fine
Unfortunately I don't have a spare vesc around 
Don't know if this is significant or not but I made the master now the slave and the slave now the master and still the same motor only spins briefly, they're both from esk8.de but one of them was second hand if that helps
```

---
## \#24 Posted by: RedEagle Posted at: 2018-03-11T16:23:35.478Z Reads: 42

```
Maybe try split ppm cable?
```

---
## \#25 Posted by: Freddiecook Posted at: 2018-03-11T16:24:42.794Z Reads: 42

```
Don't know if that would solve the issue or not as the newly made master motor is the one slightly spinning
```

---
## \#26 Posted by: Namasaki Posted at: 2018-03-11T16:28:03.751Z Reads: 42

```
Which Vesc is loosing output, the new or used one?
```

---
## \#27 Posted by: Freddiecook Posted at: 2018-03-11T16:28:46.042Z Reads: 40

```
used which doesn't look good
```

---
## \#28 Posted by: Namasaki Posted at: 2018-03-11T16:29:32.926Z Reads: 42

```
Did you try swapping motors to see if the motor has an issue?
```

---
## \#29 Posted by: Namasaki Posted at: 2018-03-11T16:30:42.685Z Reads: 40

```
Sounds like the used Vesc made be defective.
Try running it alone as a single drive and see if it still drops out
```

---
## \#30 Posted by: Freddiecook Posted at: 2018-03-11T16:35:13.144Z Reads: 38

```
Well this has confused me even more as when I run it solo it works fine
```

---
## \#31 Posted by: Freddiecook Posted at: 2018-03-11T16:43:13.543Z Reads: 35

```
Strange, I've noticed my loop key has got quite warm though, could this be the issue?
```

---
## \#32 Posted by: RedEagle Posted at: 2018-03-11T18:15:53.037Z Reads: 30

```
Warm loopkey usually means lots of current going through. Generally the less warm it is the better.
```

---
## \#33 Posted by: Namasaki Posted at: 2018-03-11T18:16:22.859Z Reads: 33

```
[quote="Freddiecook, post:30, topic:48781, full:true"]
Well this has confused me even more as when I run it solo it works fine
[/quote]
Try using split ppm but clip red wire from one Vesc.
```

---
## \#34 Posted by: Namasaki Posted at: 2018-03-11T18:18:57.752Z Reads: 36

```
[quote="Freddiecook, post:31, topic:48781, full:true"]
Strange, I’ve noticed my loop key has got quite warm though, could this be the issue?
[/quote]

Any connector heating up usually means a poor connection creating excessive resistance and possible arcing between contacts.
```

---
## \#35 Posted by: Freddiecook Posted at: 2018-03-11T23:25:38.314Z Reads: 26

```
I'll give this a go when I next have time and will update the progress, thanks
```

---
## \#36 Posted by: Freddiecook Posted at: 2018-03-12T22:10:02.730Z Reads: 19

```
No idea why or how but I tested it this evening again before making any changes and all if hunky dory again. Thanks everyone
```

---
