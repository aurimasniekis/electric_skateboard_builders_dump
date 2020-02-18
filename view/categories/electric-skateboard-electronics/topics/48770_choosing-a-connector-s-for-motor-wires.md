# Choosing a connector(s) for motor wires

### Replies: 17 Views: 1151

## \#1 Posted by: Quezacotl Posted at: 2018-03-11T11:34:03.122Z Reads: 212

```
I'm building a deck with all things inside. Now i'm on struggle of choosing a connector for the motor wires. Two motors with sensors, that's total of 16 pins.
The hub-motors have about 0,5-0,8mm2 motor wires, so it doesn't need any thick wires, so i was thinking about how would D-25 or "ATX" connector perform?
That on the picture has too many pins, but i can get smaller.
I would prefer the "ATX" connector for now. Of course it needs to be waterproofed. Just enough silicone to cover it, because only time it needs to be disconnected is if the motor(s) need to be replaced.
So what are your thoughts about these, or what would be better? The connector needs to be low profile because the deck is 28mm thick.
![IMG_20180311_131633|690x388](upload://ot4b7Ty7KQjLLKcw4YPjRymp8F0.jpg)
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-11T18:23:44.981Z Reads: 183

```
JST connectors for the sensors. 3.5mm (4mm for less resistance) bullet connectors for motor phase wires.
As for the connectors in the pic the blue one on the left (VGA?) seems good.
```

---
## \#3 Posted by: Quezacotl Posted at: 2018-03-11T18:39:11.862Z Reads: 182

```
Those that you said were the same where i want out. And not very good to attach on wood. But well, i thought that the 20pin connector on the photo is afterall very good.
```

---
## \#4 Posted by: RedEagle Posted at: 2018-03-11T18:40:39.765Z Reads: 179

```
From what I've read here they will work. I however do not have personal experience with these.
```

---
## \#5 Posted by: deucesdown Posted at: 2018-03-11T18:45:35.219Z Reads: 169

```
Are you set on having everything for 2 motors on one connecor?
```

---
## \#6 Posted by: Quezacotl Posted at: 2018-03-11T18:46:16.714Z Reads: 166

```
Yea, like this. Two pins per phase.
Picture is work in progress. Next goes the sensor wires.
![IMG_20180311_204522|690x388](upload://zBp3tkEyClhuFGXLT4BXmLPXRwW.jpg)
```

---
## \#7 Posted by: Namasaki Posted at: 2018-03-12T00:43:13.400Z Reads: 146

```
Just so you understand the risk involved here, if you inadvertently short any of the phase wires to each other during operation, it will fry your Vesc.

Also wondering if that connector can handle the high voltage and high amps.

Unless I'm mistaken, they are designed for computer applications. Low voltage and Low amps.
```

---
## \#8 Posted by: Cobber Posted at: 2018-03-12T01:46:14.237Z Reads: 144

```
[quote="Namasaki, post:7, topic:48770"]
Also wondering if that connector can handle the high voltage and high amps.
[/quote]

:thinking:
```

---
## \#9 Posted by: AssaultedPotato Posted at: 2018-03-12T02:35:47.491Z Reads: 129

```
I'm using D-Shaped Connectors (like VGA looking) for my sensor wires [EDIT: whoops i misread and I'm actually using D connectors for my battery balance wires], and I'm planning on using MT60 Connectors for the phase wires.

I would say use the large plug for the sensor wires, but use a beefier plug for the phase wires.
```

---
## \#10 Posted by: Quezacotl Posted at: 2018-03-12T08:12:04.913Z Reads: 117

```
Yea, MT60 looks good. I remember actually seeing picture here someone burying that on board. I will definitely use that next time.
Just need to think the connector for the possible sensor wires.
```

---
## \#11 Posted by: Pedrodemio Posted at: 2018-03-12T14:12:22.023Z Reads: 98

```
Probably mine, I used them and I think is way better than bullets, I always had a problem with they getting loose over time, probably low quality ones

But with the MT60 they are rock solid since you have 3 holding points that prevent torque from wires moving it side to side
```

---
## \#12 Posted by: Acidfie Posted at: 2018-03-12T14:37:08.702Z Reads: 94

```
https://i.ebayimg.com/images/i/173099089203-0-1/s-l1000.jpg

damnit, too late!
```

---
## \#13 Posted by: Blitz Posted at: 2018-03-12T18:26:01.154Z Reads: 85

```
Can I use my 5.5mm bullets from my lipo batts or just direct solder?
```

---
## \#14 Posted by: lowGuido Posted at: 2018-03-12T18:31:50.785Z Reads: 86

```
I think those pins are gonna burn up man. I have seen 4mm bullets get hot enough to melt solder.
that plastic molex connector doesn't stand a chance.
```

---
## \#15 Posted by: Quezacotl Posted at: 2018-03-12T19:08:15.350Z Reads: 82

```
Good point. I didn't consider the heat sensitivity of the connector plastic. The pins are ok though. And phases use two pins each.
```

---
## \#16 Posted by: Jedi Posted at: 2018-03-12T19:29:15.264Z Reads: 84

```
Only problem with the MT60 connectors is that you can't swap phase wires. So make sure your motor is spinning the correct way before soldering. 

Have you looked at the panel mount bullet d-sub connector. I'm using one for motor wires only. 

http://www.electric-skateboard.builders/t/panel-mount-bullet-connector/3294
```

---
## \#17 Posted by: Pedrodemio Posted at: 2018-03-12T19:59:35.608Z Reads: 77

```
On firmware 3.xx you can swap the motor direction on the VESC tool
```

---
