# How to Charge LiPo without taking it out of the case Using this method?

### Replies: 27 Views: 637

## \#1 Posted by: Toohat Posted at: 2018-07-31T05:14:50.938Z Reads: 135

```
![38191986_1679270275528966_2324322187609112576_n|281x500](upload://lVkOW6n7oyTXO1gOI8xxp80jty4.jpg)![38008789_1679270698862257_6717717794592391168_n|690x388](upload://4VYsydEf4SDaeJv7Gitw4HhuI49.jpg)![38071757_1679271565528837_7943576171826905088_n|281x500](upload://kQl9JfIZDQ987ejSmNacSnqUkZg.jpg)

So i tried making the lipo charge without taking it from the case but as you can see when i plugged the battery to the charger the charger blew and started smoking then it says reverse polarity. so can anyone tell me how to do this the correct way please.
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-07-31T06:14:48.059Z Reads: 114

```
Take out a multimeter and test whether the bullet connectors to the charger are correct according to their color, you could also test this by reversing the bullet connectors into the charger. As for the harness, the current is massively limited as there is a bottleneck with the 22awg balance leads. You wouldn’t want to push more than 1-2 amps through those wires.
```

---
## \#3 Posted by: Toohat Posted at: 2018-07-31T06:57:21.290Z Reads: 107

```
Yeah I managed to figure out what was wrong, turns out I confused between the bottom lipos and the top ones but after taking a long look I finally understood how it works and managed to connect them the proper way, but thank you for letting me know about the 1-2 amps through the balance leads I didn't know that. Thanks a lot Trdolan!
```

---
## \#4 Posted by: janpom Posted at: 2018-07-31T06:57:55.934Z Reads: 104

```
Make sure you don't have the 3S balance leads reversed. It's hard to see how the batteries are wired up.

This is how I do it:

![IMG_1277|666x500](upload://bzbCUGFqGD7VMhaHkIGlkma4Z8u.jpg)

I use single wire connectors -- XT150 and AS150. Bullet connectors would also work. This makes wiring in series much easier. I have 12S (four 3S batteries). For charging, I disconnect the AS150 connectors from the ESC and disconnect one XT150 connector to split the 12S battery pack to two 6S packs, which I then charge with two chargers. The picture is showing one half of it.

In your case, this would be even slightly simpler since you only have 6S.
```

---
## \#5 Posted by: Toohat Posted at: 2018-07-31T07:02:45.732Z Reads: 89

```
I managed to fix it, I like your method but i don't want to keep removing the casing off the board just to charge it. And my batteries are 12s i have 4x3s
```

---
## \#6 Posted by: b264 Posted at: 2018-07-31T07:07:40.705Z Reads: 87

```
It's safer and better to use a BMS (battery management system) and a 5.5x2.1mm barrel plug with a regular laptop-style charger.  Then you also don't need to remove it from the case.
```

---
## \#7 Posted by: Toohat Posted at: 2018-07-31T07:10:06.083Z Reads: 83

```
I wish i knew this before but i dont even know what bms is and im too deep into this now and i dont really want to spend anymore money.
```

---
## \#8 Posted by: Toohat Posted at: 2018-07-31T07:16:16.365Z Reads: 87

```
one more thing since the lipo balance charger is blown is the power supply blown too? this thing
![38239130_1679391665516827_3951233126201556992_n|281x500](upload://p9tNM7vSZzE8a23bwXpRf28Mcgy.jpg)
```

---
## \#9 Posted by: b264 Posted at: 2018-07-31T07:19:21.707Z Reads: 79

```
You'd have to check with a multimeter to know
```

---
## \#10 Posted by: Toohat Posted at: 2018-07-31T07:19:42.840Z Reads: 76

```
I got one what do i check for?
```

---
## \#11 Posted by: b264 Posted at: 2018-07-31T07:20:14.777Z Reads: 75

```
The supply should be labeled, make sure the output voltage is as-described on the label
```

---
## \#12 Posted by: Toohat Posted at: 2018-07-31T07:23:14.939Z Reads: 77

```
its labeled 12v and the meter is reading about 12.1V so I guess its still good, thanks!
```

---
## \#13 Posted by: janpom Posted at: 2018-07-31T07:28:21.564Z Reads: 74

```
[quote="Toohat, post:5, topic:63380"]
I managed to fix it, I like your method but i don’t want to keep removing the casing off the board just to charge it.
[/quote]

Ah, I see. So the plan is to have two 6S balance leads going out of the casing and charge with two 6S chargers? I guess that should work as long as you keep the amps low as @Trdolan03 has mentioned. It will take a while to charge, though. About 5 hours with 1A.
```

---
## \#14 Posted by: Toohat Posted at: 2018-07-31T07:41:32.866Z Reads: 70

```
yeah thats the plan and I will probably charge at 2 amps which is good for the batteries anyways. Thanks a lot Janpom you've been very helpful
```

---
## \#15 Posted by: janpom Posted at: 2018-07-31T08:23:03.419Z Reads: 73

```
Makes sense. Good luck with that. Let us know how it works out.
```

---
## \#16 Posted by: lowGuido Posted at: 2018-07-31T09:42:38.423Z Reads: 72

```
looks like you got the polarity of the balance leads the wrong way around.
you would have burnt out the balance resistors inside the charger and maybe a FET aswell.
you have to really pay attention to make sure you have the balance leads correctly orientated to match the series wiring.
I have covered this many times in the past. please look at this diagram:
https://www.electric-skateboard.builders/t/charging-2-x-3s-lipos-in-series-please-look-over-my-schematic/734/11
```

---
## \#17 Posted by: mynamesmatt Posted at: 2018-07-31T10:30:01.496Z Reads: 60

```
cannot agree more, use a bms
```

---
## \#18 Posted by: janpom Posted at: 2018-07-31T11:12:33.054Z Reads: 62

```
@Toohat I'm actually not sure if the two chargers idea would work. If you only charge one 6S pack at the time with a single charger that should be fine. However, if you connect two chargers without taking the whole 12S pack apart to two 6S packs, then you would effectively wire the chargers in series. They would be connected to each other at the point where the two 6S packs connect. If that's OK is beyond my fairly limited understanding of electronics.

Can someone more experienced comment on this?

Here's a quick picture (no balance leads to keep it simple) to illustrate what I'm talking about:

![55|299x500](upload://iCHryZcCf2oFpXmJFib2Lr2o9Gx.png)
```

---
## \#19 Posted by: PXSS Posted at: 2018-07-31T11:42:36.326Z Reads: 55

```
Its okay as long as they are two independent chargers and not a single two channel charger. 

If it's a single two channel charger. It will blow up as the two channel are not meant to be placed in series ever. 

If they are two separate chargers with separate ac adapters. They should be technically isolated from each other and the reference ground should not matter. But if they are not properly isolated they could trip a breaker and or blow. I haven't had any issues with that though. I used to do that way back in the day with some other rc stuff.
```

---
## \#20 Posted by: deucesdown Posted at: 2018-07-31T11:47:18.743Z Reads: 56

```
Depends how power is supplied to the chargers. If psu has dc ground connected to ac ground (which is pretty common), charger2 would be shorted on the charge leads.

Must be super careful.
```

---
## \#21 Posted by: PXSS Posted at: 2018-07-31T11:50:27.066Z Reads: 50

```
Yes. This. I do remember now that I had to modify some of my power supplies to disconnect the ac ground from dc groung. 

There are also some power supplies that come without an ac ground. The ones without the third prong. These work good too.
```

---
## \#22 Posted by: janpom Posted at: 2018-07-31T12:20:08.498Z Reads: 46

```
That makes a lot of sense. An easy check should be to power up both chargers and measure voltages between the positive terminal of one and the negative terminal of the other. If there's voltage, it's a problem.
```

---
## \#23 Posted by: deucesdown Posted at: 2018-07-31T12:29:11.128Z Reads: 48

```
Or just beep out the grounds (zero ohm resistance)
```

---
## \#24 Posted by: janpom Posted at: 2018-07-31T12:30:45.401Z Reads: 46

```
Right. Thinking more about it, the common ground would also cause a short on one of the batteries. That could get really bad.
```

---
## \#25 Posted by: Toohat Posted at: 2018-07-31T17:17:21.957Z Reads: 38

```
Yeah I know it's fine to use two separate chargers, but I will be charging with one anyways. Maybe later on I will get another one just to make charging faster.
```

---
## \#26 Posted by: K5_guy Posted at: 2018-07-31T23:51:21.784Z Reads: 33

```
You released the magic smoke from somewhere.  Things don't produce smoke without a reason, you burned something and you need to figure out where first, doesn't matter if it still works, something could short out and start a fire when you're not around.  Was it from the batteries, charger, power supply, or one of the wires?
```

---
## \#27 Posted by: Toohat Posted at: 2018-08-01T02:16:49.653Z Reads: 29

```
I'm well aware from where it came from and have already fixed the problem. And the smoke came from the charger and I have already replaced it even though it still worked. And as for the batteries I checked the voltage and it's fine, everything else is fine.
```

---
