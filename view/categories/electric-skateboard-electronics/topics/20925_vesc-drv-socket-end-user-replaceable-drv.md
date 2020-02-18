# VESC DRV Socket (End-user Replaceable DRV)

### Replies: 46 Views: 1802

## \#1 Posted by: laurnts Posted at: 2017-04-13T12:08:19.228Z Reads: 280

```
I'm just wondering why we can't use smt chip socket to mount DRV motor control.
This would make it easier to replace DRV chip on the spot as an end user without ever sending / shipping the whole VESC around the globe.

I know that VESC 6 is reliable, but the price are very steep for some. Meanwhile this could be a nice fix for VESC supplier that doesn't want to deal with blown up DRV.

https://cdn-shop.adafruit.com/1200x900/1281-00.jpg
https://www.adafruit.com/product/1241
```

---
## \#2 Posted by: akira Posted at: 2017-04-13T12:23:33.376Z Reads: 267

```
This is pretty cool !
I did not know that there were ZIF sockets for SMD. HOw is the heat handled ?
The other problem is that it turns a SMD into a DIP. Yuou would have to design the VESC 4 PCB.
```

---
## \#3 Posted by: treenutter Posted at: 2017-04-13T13:33:23.642Z Reads: 252

```
@laurnts replacing a DRV chip this way looks like a lot more fun than removing it and replacing it with a reflow tool!
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-04-13T14:06:46.253Z Reads: 243

```
My concern are, there is no pad to connect the ground pad witch must be connect... And will probably reduce my customer base :smiling_imp:
```

---
## \#5 Posted by: laurnts Posted at: 2017-04-13T14:10:10.970Z Reads: 235

```
@akira I think redesigning the VESC is a must to accommodate the extra space for the socket, but I think someone with KiCad knowledge easily work it around.

Heat is least of my concern as DRV chip should not be heating alot. If it pop out anyway, just put new one in. Plug & Play!

@JohnnyMeduse Yea it have the potential to reduce your customer base sadly, but this could be a way also for you to make your VESC version with user replaceable DRV chip.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-04-13T14:14:53.521Z Reads: 227

```
And I've forgot to mention that vibration could be a real bad issue... [quote="laurnts, post:5, topic:20925"]
make your VESC version with user replaceable DRV chip
[/quote]

Sorry, but I prefer good old, lead soldering :sunglasses:
```

---
## \#7 Posted by: emepror Posted at: 2017-04-13T14:17:30.578Z Reads: 220

```
VESC 6 is a lot more expensive right now because its a beta run from one company. Wait till the design files are released/manufacturing is scaled up. Plus I think some features are optional on the VESC 6 that could reduce the price too.

There's no good way to make a socketed DRV8302 that is cheap and easy to work with. Especially considering the environment these boards live in. The test jig you linked, I did a very quick search and seems that they are minimum 50 bucks each (I'm sure cheaper in quantity). The way the DRV8302 is mounted now is the best possible way to do it, Sure the board could probably be redesigned a little bit to improve reliability but adding a socket isn't solving the problem.
```

---
## \#8 Posted by: jmasta Posted at: 2017-04-13T15:55:51.389Z Reads: 190

```
VESC 6 will not be open source, unless I am mistaken
```

---
## \#9 Posted by: lowGuido Posted at: 2017-04-13T16:23:07.274Z Reads: 191

```
[quote="JohnnyMeduse, post:4, topic:20925"]
My concern are, there is no pad to connect the ground pad witch must be connect... And will probably reduce my customer base :smiling_imp:
[/quote]

not to mention that socket is HUGE! like would it even fit on the board?
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-04-13T16:25:34.705Z Reads: 183

```
Yep, should be open source, but only the firmware, tool, and schematic.... but i'm not sure for the design... will see... :disappointed_relieved:
```

---
## \#11 Posted by: emepror Posted at: 2017-04-13T16:43:49.848Z Reads: 174

```
TIL I guess, interesting that the board layout is potentially propriety, that being said it shouldn't be too hard to create a board design anyways, most designs would probably bit literal copies of the official one.
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-04-13T16:48:42.361Z Reads: 168

```
[quote="emepror, post:11, topic:20925"]
it shouldn't be too hard to create a board design anyways
[/quote]

Not really, there is a lot of rules involve with certain part..... that why you haven't seen many of those direct Fets project... you really need to know what your doing in order to make a reliable product.
```

---
## \#13 Posted by: SkateYS Posted at: 2019-01-09T22:48:14.464Z Reads: 86

```
VESC 6 not that reliable! Just ran into DRV issue today. Honestly, I don't know what to do. In the couple of years I'm now at my 7th DRV fault. 7!!! Manufacturers never assist, they re more active at selling it. I used low current limits, default settings, read the whole internet, DRV is just gonna blow one day and it's $50 + no way out
```

---
## \#14 Posted by: Pedrodemio Posted at: 2019-01-11T01:16:39.239Z Reads: 75

```
Are you using the one from @trampa?
```

---
## \#15 Posted by: SkateYS Posted at: 2019-01-11T01:21:04.908Z Reads: 73

```
Yes I got it from Trampa
```

---
## \#16 Posted by: Pedrodemio Posted at: 2019-01-11T01:22:42.838Z Reads: 75

```
What are your configuration? As detailed as possible 

Make sure you have no short is any motor wire, no bad contact in sensors wire if using

I think you are the first I see reporting DRV problems
```

---
## \#17 Posted by: SkateYS Posted at: 2019-01-11T01:34:08.875Z Reads: 73

```
battery 102p (18650), single belt drive (16/36 gear ratio)
Motor max = 40 amps
motor min = -30 amps
Batt max = 30 amps
Batt min rgen = -10
I basically leave everything else by default and run motor detection etc and apply
```

---
## \#18 Posted by: Battosaii Posted at: 2019-01-11T01:35:38.553Z Reads: 74

```
Weird. I only had one Drv chip issue with my Focbox cause of the plastic film covering the heatsink manufacturer problem. And one DRV issue with an old VescX I got after 2 years of riding hard on 12s the other Vesc x never had a problem and they are running fine ever since the repair.
```

---
## \#19 Posted by: SkateYS Posted at: 2019-01-11T01:38:01.546Z Reads: 74

```
I spent over 300 on that thing and it lasted 3 month!
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2019-01-11T01:39:32.445Z Reads: 76

```
[quote="SkateYS, post:17, topic:20925"]
single belt drive (16/36 gear ratio)
[/quote]

What Motor are you using?
```

---
## \#21 Posted by: SkateYS Posted at: 2019-01-11T01:44:46.014Z Reads: 73

```
Torque board 6374mm 190KV, 80 amps max
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2019-01-11T01:59:36.990Z Reads: 71

```
hummm that weird, Are you sure it is a DRV faults and not something else? 

also, personally I would put the motor max at 70Amp.
```

---
## \#23 Posted by: Pedrodemio Posted at: 2019-01-11T02:13:59.505Z Reads: 71

```
Are you running sensored? Any malfunction on the sensors will throw a DRV fault 

A few weeks ago I thought I had also killed my VESC 6, turns out that if you do the sensor detection and change the order of the phase wires you have do the sensor detection again 

It’s kind obvious but I hadn’t realized at the time
```

---
## \#24 Posted by: SkateYS Posted at: 2019-01-11T02:19:48.019Z Reads: 69

```
I thought that high current limits are more likely to cause issues!!!?
```

---
## \#25 Posted by: SkateYS Posted at: 2019-01-11T02:20:43.594Z Reads: 70

```
Yeah, i m using sensors! Let me take a closer look one more time.
```

---
## \#26 Posted by: Pedrodemio Posted at: 2019-01-11T02:21:16.345Z Reads: 72

```
First thing to do is run unsensored them to confirm
```

---
## \#27 Posted by: JohnnyMeduse Posted at: 2019-01-11T03:02:03.153Z Reads: 68

```
Not really, It is problematic if you go too much over the limits.

But I think @Pedrodemio might be onto something here.
```

---
## \#28 Posted by: SkateYS Posted at: 2019-01-11T03:07:41.022Z Reads: 68

```
Just tried! no luck. I think drv is gone! Blinking red, fault code = drv
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2019-01-11T03:09:22.031Z Reads: 67

```
Is the light blinking all the time or just when your try to run the motor?
```

---
## \#30 Posted by: SkateYS Posted at: 2019-01-11T03:10:51.273Z Reads: 67

```
Only when i try to run motor
```

---
## \#31 Posted by: JohnnyMeduse Posted at: 2019-01-11T03:11:24.333Z Reads: 66

```
hummm... yeah sound like a DRV or a blown Mosfet.
```

---
## \#32 Posted by: SkateYS Posted at: 2019-01-11T03:13:00.094Z Reads: 65

```
Thanks! Well, If this keeps up, i'm gonna end up giving up. It's been too much money spent so far
```

---
## \#33 Posted by: Pedrodemio Posted at: 2019-01-11T03:21:27.783Z Reads: 65

```
Paging @trampa

I think the warranty is more than 3 months

And I think Vedder would definitely would like to take a look to see what happened for a fail with no apparent reason, even more since you were running really conservative values

Does the error say anything more? Type faults at the terminal and post a screenshot here
```

---
## \#34 Posted by: SkateYS Posted at: 2019-01-11T03:53:50.726Z Reads: 62

```
![Capture|690x388](upload://tHO8kSdazL9PyidJIU1BBIMgOIA.png)
```

---
## \#35 Posted by: SkateYS Posted at: 2019-01-11T03:55:00.514Z Reads: 62

```
I also just noticed that it's not completely dead, the motor just worked a couple of times!
```

---
## \#36 Posted by: Pedrodemio Posted at: 2019-01-11T04:01:01.958Z Reads: 62

```
Ground under volt on the DRV, don’t know what could cause that, can you post a picture of the internal of your board?
```

---
## \#37 Posted by: SkateYS Posted at: 2019-01-11T04:10:58.783Z Reads: 63

```
I just put everything back together probably later on! Thanks for all 👌
```

---
## \#38 Posted by: Gamer43 Posted at: 2019-01-11T04:33:22.602Z Reads: 66

```
Maybe gate drive undervoltage fault?


If so, a few things can cause this, either the gate drive bypass caps have become a short, something (debris) is shorting the gate drive rail, or the charge pump on the DRV8301 is busted.
```

---
## \#39 Posted by: trampa Posted at: 2019-01-11T08:09:22.215Z Reads: 64

```
Hi @SkateYS , you need to get back to us via mail. david.garlinge at trampaboards dot com 
Would be the first ever VESC SIX with a DRV issue. 
What else did you attach to the VESC? Bluetooth module? 
Please also check your motor and connections.
```

---
## \#40 Posted by: Andy87 Posted at: 2019-01-11T08:38:25.001Z Reads: 58

```
Check your screws on the motor mounts.
If they too long they could have shorted the phase wires, what could fry the drv.
If that’s the issue it will happen again and again till you fixed the phase wire isolation.
```

---
## \#41 Posted by: Parafodas Posted at: 2019-01-11T13:09:20.272Z Reads: 54

```
Yeei johnny how can i test if the mosfet is good or bad . ??
```

---
## \#42 Posted by: JohnnyMeduse Posted at: 2019-01-11T13:14:03.943Z Reads: 55

```
https://youtu.be/bkvv9QZi4Pg?t=189

It is the same technique I us for every vesc out there.
```

---
## \#43 Posted by: Parafodas Posted at: 2019-01-11T13:17:12.996Z Reads: 54

```
I cant thank you enouqhf men .rly some day i il some money for all the help . 😉😉
```

---
## \#44 Posted by: SkateYS Posted at: 2019-01-11T23:00:04.530Z Reads: 43

```
Thanks I will! I'm not using any bluetooth module on it and i'm using pretty decent current settings.
```

---
## \#45 Posted by: trampa Posted at: 2019-01-12T10:48:08.941Z Reads: 36

```
If the device is damaged, it's covered. We will do some simple tests, if there is an issue, you send it to us and we will check it and send out a new device.
```

---
## \#46 Posted by: ducktaperules Posted at: 2019-01-12T11:05:26.340Z Reads: 37

```
what a useful video :slight_smile: thanks
```

---
