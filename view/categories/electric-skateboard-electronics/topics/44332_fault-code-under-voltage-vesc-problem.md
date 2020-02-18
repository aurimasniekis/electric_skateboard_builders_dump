# FAULT_CODE_UNDER_VOLTAGE (VESC problem)

### Replies: 30 Views: 1418

## \#1 Posted by: MaxMalouf Posted at: 2018-01-22T07:02:25.344Z Reads: 134

```
Hi all,

I was test riding my DIY electric skateboard the other day and after a while of testing, it started to cut in and out, I hopped off the board immediately. I thought it was just running low on battery but the issue was much larger than that.

The electronics on the board:

-10s 5Ah lipo battery
-45a 10s BMS
- 2x Maytech Vecs 
- 2x Maytech hub motors.

I am using the classic "key" design (A xt60 plug that shorts the positive wire to complete the circuit - if that makes sense) to turn off and on the board. After recharging the board, I went to plug in the "key". It sparks every time I plug it in, however this time, it didn't spark. This concerned me.

I span the motors to see if it still worked. They both span up fine for one second then the power cut then VESCs blink red about 5 times. This happens every time I try to use the motors and has nothing to do with a broken remote as the motors only span for a second using the BLDC tool. 

I typed "faults" into the terminal on the BLDC tool and this came up:

Fault            : FAULT_CODE_UNDER_VOLTAGE
Current          : -0.2
Current filtered : 0.4
Voltage          : 7.88
Duty             : 0.49
RPM              : 4718.0
Tacho            : 165
Cycles running   : 4345
TIM duty         : 3895
TIM val samp     : 1960
TIM current samp : 5937
TIM top          : 7955
Comm step        : 6
Temperature      : 31.08 

I've checked all of my solder joints on my board they all seem fine. 
These are two brand new VECS's which makes me really annoyed with Maytech, as I have not had good experience with them.

can anyone help out?

Max.
```

---
## \#2 Posted by: scepterr Posted at: 2018-01-22T07:08:56.358Z Reads: 125

```
Firstly the "classic" loopkey uses an XT90S
![3-Pairs-Amass-XT90S-Anti-spark-connector-male-female-with-two-soldering-protection|690x485](upload://uel0A30ler2lCxfQITf3KndyiRX.jpg)

And the vesc is seeing less than 8V that's why it's giving an error, can you check voltage coming from battery?
[quote="MaxMalouf, post:1, topic:44332"]
Voltage          : 7.88
[/quote]
```

---
## \#3 Posted by: MaxMalouf Posted at: 2018-01-22T07:16:59.510Z Reads: 120

```
I do have an antispark xt90 plug coming in the mail,

I checked my battery voltage with a multimeter and it is 34.1V![voltage|657x500](upload://2v4xyYNwcIREv13nx7RsW0YeBtd.PNG)
```

---
## \#4 Posted by: scepterr Posted at: 2018-01-22T07:20:25.807Z Reads: 118

```
Do you have a bms? For 10S that's empty and would trigger low battery shutoff which would trigger low voltage shutoff on vesc
```

---
## \#5 Posted by: MaxMalouf Posted at: 2018-01-22T07:22:22.275Z Reads: 118

```
I have it set on 33V battery cutoff. I'll give it a charge and see if it changes anything
```

---
## \#6 Posted by: scepterr Posted at: 2018-01-22T07:23:25.448Z Reads: 114

```
Your battery is at 34V that's pretty much empty...it needs to be 41-42

You don't have a problem other than needing to charge your battery...
```

---
## \#7 Posted by: MaxMalouf Posted at: 2018-01-22T07:26:06.819Z Reads: 116

```
Update: the battery doesn't charge. :tired_face:
```

---
## \#8 Posted by: scepterr Posted at: 2018-01-22T07:26:45.365Z Reads: 112

```
There we go 😉
Likely need to replace BMS

Can you take some pics of that?
```

---
## \#9 Posted by: MaxMalouf Posted at: 2018-01-22T07:27:26.303Z Reads: 111

```
Actually want to die
```

---
## \#10 Posted by: scepterr Posted at: 2018-01-22T07:28:10.886Z Reads: 108

```
Out of all the problems you could have thats one of the simplest and cheapest to fix...don't be too down
```

---
## \#11 Posted by: MaxMalouf Posted at: 2018-01-22T07:28:54.521Z Reads: 110

```
It's like the 5th time replacing the BMS
```

---
## \#12 Posted by: scepterr Posted at: 2018-01-22T07:29:18.885Z Reads: 110

```
Using the same charger between all the BMS?

Also as a general rule, sparks aren't good for electronics
```

---
## \#13 Posted by: MaxMalouf Posted at: 2018-01-22T07:32:46.870Z Reads: 108

```
Yeah it's an evolve charger, works fine.![20180122_172939|243x500](upload://g58ztd9INWt82BGRBa7ldYFxbvT.jpg)![20180122_172958|690x335](upload://pmlFm6oZUw9QwYwc3lfmTC61OUf.jpg)![20180122_173005|690x335](upload://ylmPxlow8AOxPuxIFVRgHxCcx4W.jpg)
```

---
## \#14 Posted by: scepterr Posted at: 2018-01-22T07:35:38.432Z Reads: 98

```
Gonna need to see the PCB of the BMS to spot any damage 
I don't know if i would feel comfortable with lipos that look like that under my feet 🤔
```

---
## \#15 Posted by: MaxMalouf Posted at: 2018-01-22T07:40:39.082Z Reads: 97

```
Thinnest diy board man! Haha the lipos are inside the deck!
```

---
## \#16 Posted by: scepterr Posted at: 2018-01-22T07:43:23.987Z Reads: 94

```
I get that but how did they get all the almost puncture marks on almost every cell?
```

---
## \#17 Posted by: MaxMalouf Posted at: 2018-01-22T07:45:12.765Z Reads: 95

```
Magic hahaha
```

---
## \#18 Posted by: MaxMalouf Posted at: 2018-01-22T07:45:46.079Z Reads: 95

```
I cant get into the BMS. It's soldered shut
```

---
## \#19 Posted by: scepterr Posted at: 2018-01-22T07:46:52.166Z Reads: 96

```
Have you been getting the same BMS model each time or diff ones?
```

---
## \#20 Posted by: TarzanHBK Posted at: 2018-01-22T07:55:24.540Z Reads: 93

```
Pls isolate your cells dude!
Sooner or later you´re gonna have magic smoke comming out that deck!
Lipos like it best in a soft environment, not wiggeling around like that.

Also your wiring confuses me a bit with that bms. In your picture, you´ve connected the top two contacts together?
```

---
## \#21 Posted by: scepterr Posted at: 2018-01-22T07:56:53.302Z Reads: 88

```
It's a "smartbms"(at least looks like one) they're weird af lol
```

---
## \#22 Posted by: TarzanHBK Posted at: 2018-01-22T08:15:10.211Z Reads: 86

```
Some of them go in a protection mode, where you´re not able to do something.
They activate it to keep you from starting a fire.
Wire it off, check your cells, charge them a bit and try to connect them again and see how things go.
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2018-01-22T13:50:43.601Z Reads: 81

```
Have you try to bypass something on the BMS ?

![image|690x335](upload://vh6izudOtmm18gdwdiwOyc9dvVs.jpg)

And is the BMS made for LIPO?
```

---
## \#24 Posted by: MaxMalouf Posted at: 2018-01-23T12:26:56.422Z Reads: 71

```
How do I charge?
```

---
## \#25 Posted by: MaxMalouf Posted at: 2018-01-23T12:27:42.871Z Reads: 73

```
What high amp BMS should I get?
```

---
## \#26 Posted by: MaxMalouf Posted at: 2018-01-23T12:29:31.020Z Reads: 72

```
I have Velcro under them. They aren't moving anywhere. I'll be sure to protect them better in the future. Also, who doesn't love a bit of magic smoke every now and again
```

---
## \#27 Posted by: TarzanHBK Posted at: 2018-01-23T13:37:06.703Z Reads: 71

```
with some other lipo charger, like an imax b6 or something.

lipos like to be coated, don´t just glue them in place naked, that´s kinky :no_good_woman:
```

---
## \#28 Posted by: MaxMalouf Posted at: 2018-01-31T02:45:29.034Z Reads: 57

```
coated with what?
```

---
## \#29 Posted by: scepterr Posted at: 2018-01-31T03:00:59.731Z Reads: 53

```
I believe he meant wrapped 
This is how I repacked a lipo
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/3511
```

---
## \#30 Posted by: TarzanHBK Posted at: 2018-01-31T07:17:06.626Z Reads: 48

```
heatshrink and then something cushy, like a neopren sheet to avoid vibrations
```

---
