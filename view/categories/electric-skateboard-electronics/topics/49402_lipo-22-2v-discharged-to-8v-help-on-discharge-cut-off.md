# LiPo 22.2V discharged to 8V. Help on discharge cut off!

### Replies: 21 Views: 654

## \#1 Posted by: Armitage Posted at: 2018-03-18T12:24:38.793Z Reads: 99

```
Hey, so I unfortunately left my skateboard on for the night. I have 2x3s so 22.2v and i checked that they are now at 8.6v. I know that at this point it's better to just throw them away, since it is dangerous to charge them and 1 cell is actually fully dead. 

But now I need some help. Is there a way to have a device between the batteries, that cuts the power off, when the batteries come to the cut-off voltage. I have a 12v to 5v adapter also between the vesc and the batteries. Even if I switch the whole thing off, the batteries still discharge.
I did a quick schematic as well.

Thanks in advance.![Untitled|690x388](upload://q0Cw5vRWJmnZXsbtuU9E3aAn5y6.png)
```

---
## \#2 Posted by: Tuomalar Posted at: 2018-03-18T12:42:40.179Z Reads: 81

```
[quote="Armitage, post:1, topic:49402"]
. I have a 12v to 5v adapter
[/quote]

What for you need that 12V adapter? Did you set cut of voltage in vesc? What kind of switch? Batteries obiviously shouldn't drain themselves very fast if they aren't connected anything.
```

---
## \#3 Posted by: Armitage Posted at: 2018-03-18T13:13:44.889Z Reads: 72

```
I use the adapter for 5v led strip. As a switch is use a loop xt-90, so no power can go through there.
Yes, cut off voltage is set
```

---
## \#4 Posted by: FredrikHems Posted at: 2018-03-18T13:15:31.237Z Reads: 70

```
Do you mean that the batteries drained themselves after you had pulled out the XT-90? Cause according to your diagram, thats not possible..
```

---
## \#5 Posted by: Armitage Posted at: 2018-03-18T13:27:06.392Z Reads: 65

```
no, i had the xt90 attached, but i want to know that is there a way to have another autoswitch that cuts the power out when the cells are too low. Like the lipo alarm but as a switch.
```

---
## \#6 Posted by: Tuomalar Posted at: 2018-03-18T13:33:45.841Z Reads: 62

```
People use vesc and bms. I think that the fault is your batteries. You have over drained them multiple times or they are faulty in some other way. For example you shorted them in some point.
```

---
## \#7 Posted by: Armitage Posted at: 2018-03-18T13:44:41.606Z Reads: 54

```
I actually have shorted them before, but the batteries were basically new, charge count was maybe 4 or 5.

Forgot to mention that the charger is always connected, it's in the board. Maybe the charger is drawing power?
```

---
## \#8 Posted by: Tuomalar Posted at: 2018-03-18T13:54:23.233Z Reads: 49

```
One short was enough to ruin my lipos. Not saying that shorts always ruin your batteries, but it might.
What kind of charger?
```

---
## \#9 Posted by: FredrikHems Posted at: 2018-03-18T13:55:52.989Z Reads: 47

```
Its the vesc that have drawn current. If you let the XT90 stay in, the vesc will get power, and the LED`s will light.
```

---
## \#10 Posted by: Armitage Posted at: 2018-03-18T14:01:12.730Z Reads: 47

```
I use this charger rn, but I'm already replacing it with a proper bms:

 https://hobbyking.com/en_us/turnigy-b6-compact-50w-5a-automatic-balance-charger-2-6s-lipoly.html
```

---
## \#11 Posted by: Armitage Posted at: 2018-03-18T14:01:54.984Z Reads: 46

```
Yeah I know that, but the batteries still discharged even if the xt90 wasn't connected.
```

---
## \#12 Posted by: FredrikHems Posted at: 2018-03-18T14:24:05.879Z Reads: 42

```
Now I'm just confused, since first you said you had the XT90 switch connected.
[quote="Armitage, post:5, topic:49402"]
i had the xt90 attached
[/quote]

And then 1 hour later you say this...
[quote="Armitage, post:11, topic:49402"]
batteries still discharged even if the xt90 wasn’t connected.
[/quote]
 
Was the XT90 switch connected or not?
```

---
## \#13 Posted by: Armitage Posted at: 2018-03-18T14:29:32.138Z Reads: 39

```
lol

Basically, when the batteries went dead fast, the xt90 was connected. So i want something to cut off the power incase i forget the xt90 connected.

BUT another problem is that if the xt90 isn't connected, the batteries still discharge but a lot slower. So I want to know that what draws power then.

I have two problems!!
```

---
## \#14 Posted by: Acido Posted at: 2018-03-18T15:02:20.927Z Reads: 34

```
just get a charge only bms for 20$ dude, its worth it
```

---
## \#15 Posted by: Armitage Posted at: 2018-03-18T19:25:35.900Z Reads: 30

```
Any suggestions on what to choose?
```

---
## \#16 Posted by: Acido Posted at: 2018-03-18T19:32:27.481Z Reads: 31

```
Im not sure if you can fix these batteries somehow, but if you get new ones go with supower,bestech diebie but this one is a little expensive, bestech ones are great and small, and cost around 20
```

---
## \#17 Posted by: b264 Posted at: 2018-03-18T19:40:13.693Z Reads: 31

```
The device you are describing is called a BMS.
```

---
## \#18 Posted by: Armitage Posted at: 2018-03-18T19:59:59.724Z Reads: 30

```
Maybe I can every time just remember to take the xt90 out. But do you think that the charger draws the power?
```

---
## \#19 Posted by: Tuomalar Posted at: 2018-03-18T20:04:21.377Z Reads: 31

```
Can't say for sure but it is possible. I would say that buy new batteries, bms and some charger
```

---
## \#20 Posted by: Armitage Posted at: 2018-03-18T20:50:34.132Z Reads: 26

```
Is this one too sketchy to buy? 
https://www.aliexpress.com/store/product/6S-50A-bms-2017-new-Li-ion-50A-large-high-current-BMS-PCM-with-SAME-port/1821822_32826354127.html?spm=2114.12010612.0.0.29a63632cXR9Ve


Can anyone hit me up with a link to a good and cheap bms that includes discharging at 50-60A as well?
```

---
## \#21 Posted by: Armitage Posted at: 2018-03-18T20:55:15.746Z Reads: 24

```
I also found these but do I have to ask the price from the contacts?

http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D345.html
```

---
