# 10S BMS on 8S battery?

### Replies: 13 Views: 747

## \#1 Posted by: StefanMe Posted at: 2018-09-11T18:16:35.215Z Reads: 107

```
Hi guys! 

I got a little accident a few days ago (thanks I am fine!) my battery enclosure broke and the battery fall off the board and blocked my back wheels. I had to remove two of the cells from my li-ion pack and have now an 8s battery left.

First crap is: I cannot charge this with my 42V charger... to find an 8S Battery charger is not that easy... :) but I found one and bought it (15euro from AliExpress.). Now I want to bring the battery back in nice condition and bought some huge shrink stuff and will connect my old BMS to it. BUT can I connect my 10s BMS to the 8s Battery? I guess yes, just leave the last two wires open... correct? 

![IMG_5820|375x500](upload://w80vgXpDeLITwRZDxRLFwwFXeDS.JPG)

Thanks for you help guys! Have a safe ride!!
```

---
## \#2 Posted by: Acido Posted at: 2018-09-11T19:14:05.502Z Reads: 95

```
Bestech D140 is a small compact bms, if you get a 10s version just leave the 2 wires disconnected and it will work normally, same would be for 12s version. should work in your case too
```

---
## \#3 Posted by: GunnarK Posted at: 2018-09-11T19:54:44.885Z Reads: 86

```
I myself have a 10s BMS with 8s batterypack lipos.
I use my 10s charger. Works fine

Make sure you leave BMS balance wires 9 and 10 disconnected
```

---
## \#4 Posted by: b264 Posted at: 2018-09-11T20:02:43.339Z Reads: 85

```
[quote="StefanMe, post:1, topic:67733"]
can I connect my 10s BMS to the 8s Battery?
[/quote]

Yes, if you do it properly

Start from negative, and connect up to the more positive cells and leave the last two empty
```

---
## \#5 Posted by: StefanMe Posted at: 2018-09-11T20:26:54.303Z Reads: 77

```
And u can also use an 10s(42v) charger?! So tue BMS Tales also care about the right voltage if the batter is connected properly?
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-09-11T20:34:19.219Z Reads: 79

```
As long as it is a constant current / constant voltage charger. It will charge the pack when empty at the appropriate voltage, and once the voltage exceeds the BMS over voltage protection for cell level voltage (4.2 or 4.25 sometimes) it will disconnect from the charger.

If the charger has an indication light on it it should also turn green as it stops drawing current.

Please verify that the BMS has over voltage protection and is able to disconnect. Keep in mind that you MUST charge through the BMS.
```

---
## \#7 Posted by: TowerCrisis Posted at: 2018-09-11T20:38:11.993Z Reads: 74

```
On a slightly different note, separate from my explanation above.

Who here is experienced in lithium battery chemistry? I ask because normally when a battery charges it is constant current until the charger reaches 4.2V per cell, and then remains at constant voltage.

This leads to the charger current gradually platouing until it reaches 0.

What happens when you charge at the full 2 amps until full? Is it detrimental to the battery?

Theoretically this should lead to a faster charge time. If I'm using a BMS anyways wouldn't it be better to use a 12S battery for 10S so I can get a boost charge at the high end of capacity? This is assuming the BMS doesn't fail of course.
```

---
## \#8 Posted by: StefanMe Posted at: 2018-09-12T00:54:30.189Z Reads: 61

```
Awesome! Worked as expected! Green light
Showed up, my is saying battery is full. Thanks a lot!

![image|375x500](upload://ezlVtdl3TvLFRzWy80oFeJtIfxJ.jpg)
```

---
## \#9 Posted by: b264 Posted at: 2018-09-12T03:41:54.520Z Reads: 54

```
[quote="TowerCrisis, post:7, topic:67733, full:true"]
On a slightly different note, separate from my explanation above.

Who here is experienced in lithium battery chemistry? I ask because normally when a battery charges it is constant current until the charger reaches 4.2V per cell, and then remains at constant voltage.

This leads to the charger current gradually platouing until it reaches 0.

What happens when you charge at the full 2 amps until full? Is it detrimental to the battery?

Theoretically this should lead to a faster charge time. If I’m using a BMS anyways wouldn’t it be better to use a 12S battery for 10S so I can get a boost charge at the high end of capacity? This is assuming the BMS doesn’t fail of course.
[/quote]

This sounds extremely dangerous, but I've wondered the same thing before.  I would not want such a thing charging in my home, though.
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-09-12T04:30:59.529Z Reads: 50

```
It definitely is more risky without additional protection circuitry other than a BMS.

But the method is proven. Phone batteries will turbo charge at 9V when the cell itself is only 4.2V.

I'm by no means advocating that you hook up extra voltage to your charge only BMS.
```

---
## \#11 Posted by: b264 Posted at: 2018-09-12T05:11:16.792Z Reads: 47

```
I live in a high-rise so it's imperative I'm a little more safe than others who only live in single-family dwellings.  LoL
```

---
## \#12 Posted by: TowerCrisis Posted at: 2018-09-12T05:13:04.655Z Reads: 45

```
Yes I can imagine a "spontaneous and catastrophic kitchen oil fire" would be a lot more dangerous in a high-rise. ;)
```

---
## \#13 Posted by: sk8l8r Posted at: 2018-09-12T08:34:48.464Z Reads: 37

```
[quote="b264, post:11, topic:67733"]
I live in a high-rise
[/quote]

when I charging something even slightly risky, I always have a quick disposal plan 'it can go thru this door/window if it really has too' not really any way of quick dispose at height, would really worry me!
```

---
