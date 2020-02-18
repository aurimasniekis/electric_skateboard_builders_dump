# LiPo burst charge

### Replies: 15 Views: 161

## \#1 Posted by: Jarno Posted at: 2019-03-08T13:39:36.704Z Reads: 61

```
I'm setting up my VESC and am running in to the porblem that when I'm breaking I get a high current back from the motor when breaking. I have set my battery max current breaking to -8A since my battery is rated at 8000mAh. This however shuts down the VESC since my breaking bursts over 8A. 
Can a LiPo handle say 2C when it's only a burst?
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-03-08T13:43:14.249Z Reads: 59

```
Hmmm? Shouldn't shut down your vesc, I hit 65-70a peak when braking

I run -10a on a 10s3p lg hg2
```

---
## \#3 Posted by: Andy87 Posted at: 2019-03-08T13:52:09.849Z Reads: 56

```
[quote="AlanZhou, post:2, topic:86548"]
I hit 65-70a
[/quote]

Batt amps? 😱😱😱
Where you breaking? 😂
I never hit more than -10a per vesc
```

---
## \#4 Posted by: Jarno Posted at: 2019-03-08T13:56:07.329Z Reads: 53

```
It's not a shutdown it's an error,![image|324x500](upload://eAOK0hTdEWItm6b7edWUhVbbe6G.png) 

And it happens when breaking with an 8 amp max break
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-03-08T13:57:03.832Z Reads: 48

```
Nope motor amps per motor on the raptor hubs
```

---
## \#6 Posted by: Andy87 Posted at: 2019-03-08T14:09:48.040Z Reads: 46

```
Your lipo can handle more for a burst for sure.
8a shouldn’t be the reason why your vesc cut out.
The drv vault is no good sign. Do you have it permanent already? If yes you probably need a new drv chip.
Does the fault just occurring when hard breaking?
```

---
## \#7 Posted by: Jarno Posted at: 2019-03-08T14:10:47.756Z Reads: 42

```
Only when hard braking in FOC mode, it works fine in BLDC mode.
```

---
## \#8 Posted by: Andy87 Posted at: 2019-03-08T14:11:48.508Z Reads: 40

```
Ok that’s interesting.
Which vesc you using?
```

---
## \#9 Posted by: Jarno Posted at: 2019-03-08T14:12:48.726Z Reads: 38

```
I'm using a mtvesc50a
```

---
## \#10 Posted by: Jarno Posted at: 2019-03-08T14:15:06.468Z Reads: 38

```
It seems like it has happened to other people and adding some extra cappacity may help, http://vedder.se/forums/viewtopic.php?f=5&t=68%C2%A0
```

---
## \#11 Posted by: Andy87 Posted at: 2019-03-08T14:29:36.563Z Reads: 38

```
[quote="Jarno, post:9, topic:86548"]
mtvesc50a
[/quote]
Those aren’t really reliable in FOC.
It’s a cheap hw4.12 vesc and it’s not recommended to use FOC with this hardware.
```

---
## \#12 Posted by: Jarno Posted at: 2019-03-08T14:30:56.319Z Reads: 38

```
Thank, I'll switch to BLDC then since that option seemed to always work.
I am sad that I made a mispurchase then since I whould like FOC, maybe I can get a return.
```

---
## \#13 Posted by: rich Posted at: 2019-03-08T16:16:00.993Z Reads: 31

```
When I tried FOC with maytech 4.12 I got DRV fault every time when braking, furthermore braking was not possible, only cut offs. Maytech and FOC are no friends at all.
```

---
## \#14 Posted by: Jarno Posted at: 2019-03-08T16:30:20.068Z Reads: 27

```
It seems like Maytech an FOC do not play nice together, I'll try to retour the VESC tommorow. Do you guys have any recommendations for an VOSC 60A+?
```

---
## \#15 Posted by: Andy87 Posted at: 2019-03-08T16:36:05.149Z Reads: 26

```
Get a vesc 6 or vesc 6 derivat or focbox or focbox unity. All work reliable in FOC
```

---
