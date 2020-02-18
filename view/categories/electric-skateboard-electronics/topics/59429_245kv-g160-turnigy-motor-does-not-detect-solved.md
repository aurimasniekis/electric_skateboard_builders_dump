# 245kv g160 turnigy motor does not detect (SOLVED)

### Replies: 24 Views: 421

## \#1 Posted by: JamesNothing Posted at: 2018-06-19T23:36:28.925Z Reads: 65

```
so, new day new problem.
some time ago I bought a semi-functioning "complete" from  someone on this forum that lives (lived?) in Milano like me.
I have a 245kv turnigy motor, a esk8.de vesc and I can't do a motor detection :frowning:
The motor stutters and tries to spin, but bad detection results are the only thing that comes up. I tried with two different computers, with fw 2.18 in bldc tool (reflashed also), then I tried with 3.xx and vesc tool flashing a bootloader and the new fw.
The voltages for cutoff ecc. are ok for my 8s, motor A, bat A, regen.. all seems to be ok, but detection fails every time. I tried to play with the parameters in detect mode going from 1A all the way to 12A and with min. erpm and duty cycles changing them in increments, but nothing worked..    other things to try?

note that the motor was sorta spinning before, but if I gave him full throttle suddenly the vesc would reboot, so I had to do something to ensure it would work better than that... but now it does not work at all! :cry:
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-06-20T00:05:13.178Z Reads: 56

```
so during motor detection it is cogging? normally adding a bit of duty should resolve this. is the duty 0,05? Isn't there a tooltipp showing that?
```

---
## \#3 Posted by: Simnol Posted at: 2018-06-20T00:17:51.829Z Reads: 52

```
Single or dual motor?
```

---
## \#4 Posted by: JamesNothing Posted at: 2018-06-20T00:20:01.163Z Reads: 44

```
cycle is at 0.05 min erpm is 150, A is 5,0.
on top of that I have bemf at 600 and cycle integrator at 62.

single motor.
I tried to change cycle by 0.01 at a time from 0.01 to 0.06, but this didn't solve the problem
```

---
## \#5 Posted by: Simnol Posted at: 2018-06-20T00:33:21.187Z Reads: 40

```
Are you using the latest vesc tool?
https://vesc-project.com/node/17
```

---
## \#6 Posted by: JamesNothing Posted at: 2018-06-20T00:34:45.484Z Reads: 40

```
yup! the latest and greatest.
```

---
## \#7 Posted by: Simnol Posted at: 2018-06-20T00:36:49.658Z Reads: 37

```
Maybe some picture of each page and your setup.
Because I can't see what's wrong
```

---
## \#8 Posted by: JamesNothing Posted at: 2018-06-20T00:45:19.809Z Reads: 40

```
here they are:
I'm starting to think that I have a toasted motor, which is very possible having seen how the board was previously put together...

![Screenshot_1|690x431](upload://9T5Go52VUiY5ncB3TVzuNPerwvo.png)![Screenshot_3|690x431](upload://p3LRnjVfC5tiH76A94Fk72DRH2S.png)![Screenshot_4|690x431](upload://4bhdF0dQLAvgLEoGjI6OpWj1yqA.png)![Screenshot_5|690x431](upload://urxEna8B5cFwAbEXBxRvyWsK6Gw.png)![Screenshot_6|690x431](upload://xTTgeYXbCYoACqH2xVcBXTHB0a0.png)![Screenshot_2|690x431](upload://bDcS25Q7mq0DfDDKVromJ1cA84c.png)![Screenshot_7|690x431](upload://arvER7d1P04nX4ddY1z3pUXKvbN.png)![Screenshot_8|690x431](upload://4TCR2LnnwJemELxinqgAA3ksfzo.png)![Screenshot_9|690x431](upload://vA4vxXxPNvTuTnBUuVBfnRjFgsz.png)![Screenshot_12|690x431](upload://4lfFniMPtBzf6UxkY6s9MRu3dbh.png)![Screenshot_10|690x431](upload://5NuAgRDYD32LjOxvL0xh49xhNds.png)![Screenshot_13|690x431](upload://2afxUB00Uob78YieFMW54Oao4va.png)![Screenshot_11|690x431](upload://no4jfg0h4cSYYCLwOgGolww0kEi.png)![Screenshot_14|690x431](upload://70DVmfL75qqNM1DqtfVTajRegEc.png)![Screenshot_15|690x431](upload://ztPVupcWtu3ifFZunDuVkMczg3w.png)![Screenshot_16|690x431](upload://7bHpGG4WOu8LKvH6cHwA3lP8PwL.png)
```

---
## \#9 Posted by: Benjamin899 Posted at: 2018-06-20T00:49:51.644Z Reads: 31

```
try to increase Duty to 0.15 instead of 0.05 when you do detection. Btw Battery Regen is extremly low at -40. What Battery do you have? And lower max erpm to 60000 and -60000
```

---
## \#10 Posted by: JamesNothing Posted at: 2018-06-20T00:53:26.618Z Reads: 35

```
i run two 4s lipos in series with a bypassed bms for charge only. batt. regen is default now, what should I put there? I don't rely that much on batt. regen
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-06-20T00:56:01.117Z Reads: 33

```
well battery regen is important for breaking. depending on your battery capacity and max charge rate you will have to lower or increase that value, because if you feed to much back into the battery it can take damage and damaged batteries are dangerous
```

---
## \#12 Posted by: JamesNothing Posted at: 2018-06-20T01:00:26.606Z Reads: 34

```
I didn't dig that much into battery regen for the moment, as I can't get the motor to spin at all :smiley:
The battery is a 8s 5200mAh 35c, what could be a good parameter for batt regen in this case?
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-06-20T01:02:44.066Z Reads: 30

```
35c is the discharge, i am guessing it is 2C max charge current, so 10.4 amp charge and you can safely add a bit to that. so -13/-14 amps battery regen. But try increasing the duty on detection for the motor.
```

---
## \#14 Posted by: JamesNothing Posted at: 2018-06-20T01:17:02.526Z Reads: 28

```
already tried. went up by 0.01 from 0.05 to 0.19 with no results sadly.

will change the regen when I'll get the motor to move :slight_smile:
```

---
## \#15 Posted by: JamesNothing Posted at: 2018-06-20T10:30:14.855Z Reads: 28

```
so, after a good 4 hours of beauty sleep I'm here at work wondering why I didn't pull out a multimeter and checked the internale resistance of the motor phases.
I'll do as soon as I get back home, but my idea is that whoever did the soldering job to put silicon 10awg wire on the phases did a bad job and something is shorting out.
BUT I checked the motor before trying to detect it and it seemed to spin freely, so I'm not really sure whether or not this is the case.
in theory if I disconnect the motor and spin it it should spin freely, but shorting two phases together (or all three of them) should result in some resistance in the spin, right? I'll also check if there is continuity on every wire coming off the vesc to the motor to check if I fudged up somewhere and have a bad connection from vesc to motor.
I'm pretty sure the problem is at hardware level because of the "no fault" thing.
```

---
## \#16 Posted by: Benjamin899 Posted at: 2018-06-20T16:53:55.390Z Reads: 22

```
good idea to test with a multimeter
```

---
## \#17 Posted by: JamesNothing Posted at: 2018-06-20T17:16:39.540Z Reads: 22

```
It was indeed a good idea. One of the phase wires had a bad soldering job. 
In fact all three had one bad solder blob on them, but one was cracked and was my problem.
The job was done by a monkey with two left hands and the phase wires were cut very close to the can of the motor, so it was very hard to resolder, but I eventually did it.
The motor could finally run detection no problem (and I changed my regen to -13).

On the next topic: I jumped on the board to try it and brakes are very weak. I assume I have to change motor current max brake to enhance their performance? more amps=more brakes? I've put a conservative 50A max motor current and -50A on brake current (stock was 60A; -60A)... how does it work exactly?
```

---
## \#18 Posted by: Benjamin899 Posted at: 2018-06-20T18:09:04.634Z Reads: 22

```
as it was explained to me. Battery regen is mostly effective while braking at higher speeds, and motor brake current is for lower speeds. But yes ofc, since you lowered the amount of amps you can put back into the battery the force of your brakes is weaker. I think you could go even higher than that on regen since it is mostly only for a short time. Thas why most build dual drive with vesc or a bigger mAh Battery.
My old build had a APS ESC and that thing could brake like an anchor, but shit at smooth acceleration or controling my battery.
```

---
## \#19 Posted by: JamesNothing Posted at: 2018-06-20T18:38:24.945Z Reads: 21

```
I don't trust my battery enough to give her too many Amps more than she asks.
I'll try to go a little higher with max brake Amps and test. Tomorrow. Tonight I'll enjoy the feeling of a solved problem and cheer with a scotch whisky to your kindness and to all the good stuff  we can find on this freakin forum :smiley:
```

---
## \#20 Posted by: Benjamin899 Posted at: 2018-06-20T18:41:40.316Z Reads: 21

```
yeah i did phasewires myself on my sk3 and they also look horrible but resistance was ok, but the flex is realy superior to those hard wires that come with the motor.
```

---
## \#21 Posted by: JamesNothing Posted at: 2018-06-20T18:46:20.652Z Reads: 19

```
[quote="Benjamin899, post:20, topic:59429"]
the flex is realy superior
[/quote]
That's for sure. It's also true that the big stranded wires coming off the motor take solder like shit. They're really a nightmare to do joints with and you really need to know how to solder if you want to reliably connect them.
Anyway, I consider myself lucky and I hope my post could help someone not to throw away a motor or a Vesc :slight_smile:
```

---
## \#22 Posted by: Benjamin899 Posted at: 2018-06-20T18:54:26.441Z Reads: 18

```
i used my dremel to take of the coating and used some old copper wire strand  from my stereo and coiled it around the silicone wire and the phase wire. i will probably reopen it and make it smaller.
```

---
## \#23 Posted by: Simnol Posted at: 2018-06-20T23:27:41.965Z Reads: 15

```
I'm glad you found your issue :)
```

---
## \#24 Posted by: JamesNothing Posted at: 2018-06-21T09:35:00.217Z Reads: 13

```
[quote="Benjamin899, post:22, topic:59429"]
used some old copper wire strand from my stereo and coiled it around the silicone wire and the phase wire
[/quote]


This is an awesome trick! At adds a lot of mechanical strength to the solder joint and makes it last longer in stressful situations.
The resulting joint however is stiffer and I had too little of phase wire coming out the motor to do this, so I had to do the old "twist the wires together and hope for the best" thing to my motor.
We'll se whether it holds fine or not: if not then I'll have to get myself a new motor...

[quote="Simnol, post:23, topic:59429, full:true"]
I’m glad you found your issue
[/quote]

I'm glad too, and I'm also glad that the issue was in the motor and not in the vesc. This helps a lot as the money for the build were already very tight :smiley:
```

---
