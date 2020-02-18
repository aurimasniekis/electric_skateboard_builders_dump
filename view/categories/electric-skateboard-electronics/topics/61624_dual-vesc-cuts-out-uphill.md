# Dual VESC cuts out uphill

### Replies: 18 Views: 496

## \#1 Posted by: PDXroses Posted at: 2018-07-12T07:04:04.876Z Reads: 127

```
I’m running dual VESCs in BLDC over canbus. On uphill climbs, the skateboard stops when it reaches 70.2C.  This happens consistently.  I used real-time data monitoring and observed this. My FET cutout start is at 85C and ends 100C. Also, I’ve observed no correlation between my motor temp cutout nor voltage dropping below the min (30V) with the skateboard cutting out. 

Has anyone had this type of experience?  Why’s the VESCS cutting out at 70.2C when I set it to cut out at 85C?  Thank you.
```

---
## \#2 Posted by: Ishayc Posted at: 2018-07-12T07:31:20.693Z Reads: 114

```
Did you try checking for faults in the terminal after it happens?
```

---
## \#3 Posted by: PDXroses Posted at: 2018-07-13T01:43:00.280Z Reads: 83

```
No faults. It seems like the VESC thinks the fets are at 85C and shuts down the board even when real time data shows they’re only at 70C. Either the fet cutout reading is not working right or the temp monitor on real time data isn’t accurate.
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-07-13T01:52:46.275Z Reads: 80

```
mmh just to be safe, can you post your settings?
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-07-13T02:17:10.656Z Reads: 73

```
the 85c isn’t a hard temp cutoff, it’ll just throttle your performance back, 100c it will be a hard cutoff
```

---
## \#6 Posted by: PDXroses Posted at: 2018-07-13T02:28:53.996Z Reads: 68

```
Here are my general settings and temp settings.  I meant 80C for the FET cutout start, not 85C. The board slows down to a crawl uphill rather than abruptly cut out.  That was yesterday.  Then today (92F), on a flat, rectangular, 0.5 mile course, my 210lb buddy rode it hard.  It crawled to a stop after four laps.  I couldn't measure the real time data, but the behavior was very similar to the one where I was climbing hills.  I think the VESC thinks its at 80C when it's really at 70C, but I can't confirm or correct that.  Thanks all.

![Screenshot%20(1)|690x460](upload://pZgDxvYMxUrwU1OIrJSDFww9Ur6.png)![Screenshot%20(4)|690x460](upload://M0WxqjzD1UgggNbeDrnzY9l1su.png)
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-07-13T02:49:49.544Z Reads: 59

```
how is it even possible for a dual drive on a flat to go into thermal throttling? what motor and gear ratio are you running? that sounds crazy to me.
```

---
## \#8 Posted by: PDXroses Posted at: 2018-07-13T02:52:06.395Z Reads: 60

```
38:15 gear ratio
Is it because the VESCs are closed off inside a plastic case without a heat sink?

My buddy was accelerating up to 28mph every 0.1 mile and he weighs 201lbs. It was 92F’ish at the time.
```

---
## \#9 Posted by: Sender Posted at: 2018-07-13T02:52:12.680Z Reads: 62

```
Nah, mine goes out after riding hard in the Alabama heat....
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-07-13T03:01:35.945Z Reads: 63

```
well ok, i live in mild german climate. but i never even got close even with my single 6s drive. guess my weight does give me a hughe advantage.
@PDXroses are you running vesc4.12 or focboxes? havnt even thought about that angle.
```

---
## \#11 Posted by: PDXroses Posted at: 2018-07-13T03:02:40.239Z Reads: 62

```
I’m running Vesc 4.12. Must be nice not to be heavy.
```

---
## \#12 Posted by: Benjamin899 Posted at: 2018-07-13T03:06:20.421Z Reads: 63

```
alright, yes those things have no direct fet cooling, making them run hot faster. there are some How to heatsink vesc in this forum or just buy one from flipsky over banggood or ebay. I have one and it saves alot of time, but if you like going DIY there are some ways to tune those things^^
```

---
## \#13 Posted by: PDXroses Posted at: 2018-07-13T03:08:31.701Z Reads: 65

```
You’re awesome. Thank you. Will the heat sinks help if there is no way for the air to ventilate and is trapped inside the plastic?  Won’t it just delay the cutout by a few minutes?  

And my broader question is why the board is cutting out at 70C when I set the FET temp cutout start at 80C. This right here is a mystery.
```

---
## \#14 Posted by: Benjamin899 Posted at: 2018-07-13T03:13:23.269Z Reads: 62

```
maybe it isnt even your fets but your battery. what do you have?
btw here is the link. and yes it just delays the heating. you could take a aluminium/copper plate/pipe and lead it out of the enclosure and have at the outside some cooling fins. 
https://www.electric-skateboard.builders/t/how-to-heatsink-your-vesc/26129
or if you are lazy^^
https://www.banggood.com/de/HGLRC-Flipsky-Black-CNC-Aluminium-ESC-Protective-Case-For-VESC-V4_12-BLDC-Controller-Rc-Car-Parts-p-1296902.html?rmmds=search
```

---
## \#15 Posted by: Holyman92 Posted at: 2018-07-13T03:15:03.340Z Reads: 55

```
If you're in Germany I recommend hitting up @Kug3lis he makes dual cases for vesc  

![15314516139161532122481|374x500](upload://gTdTPdCZQ0yjBRVWXsJJhpguZMy.jpg)

They're solid aluminum and the whole case is a heatsink
```

---
## \#16 Posted by: Benjamin899 Posted at: 2018-07-13T03:18:03.942Z Reads: 49

```
isnt he from london? i asked for his case, he is currently sold out for the 4.12. But that info is 2weeks old.
```

---
## \#17 Posted by: Holyman92 Posted at: 2018-07-13T03:22:02.001Z Reads: 46

```
My point was he's across the pond for us over in the US... and he might be right now, but I just installed the case and will be testing tomorrow after work... it's supposed to be 34° tomorrow so let's see how well the board handles the heat now haha
```

---
## \#18 Posted by: PDXroses Posted at: 2018-07-19T22:00:14.102Z Reads: 31

```
Thanks Benjamin.  Maybe it is the batteries.  Will test it.
```

---
