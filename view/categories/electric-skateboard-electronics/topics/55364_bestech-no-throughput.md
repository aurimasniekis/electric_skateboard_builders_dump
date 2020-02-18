# Bestech - No throughput

### Replies: 24 Views: 962

## \#1 Posted by: trigger4point7 Posted at: 2018-05-14T01:56:14.869Z Reads: 151

```
So I'm hooking up my Bestech BMS and am having an issue getting any output at all I'm a little worried I may have shorted something. I have B1-10 (10S pack) connect properly as far as I can tell. I have the first P group (negative) soldered to B- and can't get a reading from P-. I probe the negitive lead and each B group sequentially and get the expected incremental voltage.

I've also connected the built in e-switch. 

When I first connected everything I had a reading from P- with the expected voltage WITHOUT connecting the e-switch. Which I thought was odd. Anything else I could try? 

I'm worried I shorted it because when checking the incremental voltage under the BMS I accidentally bridged two of the B group connections and here I tiny spark. Could that have been the fatal blow?![IMG_20180513_180610|374x500](upload://nMIvp3WM2z8Ttkn82alwpFXiTE4.jpg)
```

---
## \#2 Posted by: Namasaki Posted at: 2018-05-14T05:22:22.583Z Reads: 123

```
When you bridged 2 balance wires, you shorted one of the p-groups.
you likely have activated the short circuit protection.
You will have to turn off the e-switch and turn it back on to reset the bms.
```

---
## \#3 Posted by: b264 Posted at: 2018-05-14T05:50:31.046Z Reads: 118

```
![IMG_20180513_180610|690x419](upload://AjhOwyJ6mPmacZ90hIxWwkO8oMv.jpg)
![bomb|385x311](upload://9pfOnRFRvR41f1NLVvlxJE9eegk.gif)
```

---
## \#4 Posted by: Jinra Posted at: 2018-05-14T05:54:02.848Z Reads: 111

```
that should be connected tho
```

---
## \#5 Posted by: b264 Posted at: 2018-05-14T05:54:47.118Z Reads: 112

```
It should be connected, or not connected, not just laying there loosely touching the thing next to it
```

---
## \#6 Posted by: Jinra Posted at: 2018-05-14T05:55:26.378Z Reads: 112

```
yea for real. kapton anything exposed :/
```

---
## \#7 Posted by: trigger4point7 Posted at: 2018-05-14T07:10:18.240Z Reads: 108

```
Haha no worries that is my temporary series connection between 5 and 6 before I cement every thing down with silicon.
```

---
## \#8 Posted by: trigger4point7 Posted at: 2018-05-14T07:11:22.969Z Reads: 107

```
Is that as easy as separating the two e switch wires?
```

---
## \#9 Posted by: trigger4point7 Posted at: 2018-05-14T07:12:51.375Z Reads: 106

```
I'm planning on wrapping in PVC heat shrink (both 5s packs with a 1mm rubber silicon sheet in between and silicon on the bottom. Should do it I hope.
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-05-14T07:39:20.045Z Reads: 100

```
That series connection you have is VERY important.

If you had any load connected to the battery pack and that spot disconnected while delivering power, it fried the BMS.

I won't go into the full details, but the BMS only sees a differential between balance leads of 4.2 volts. When there is a load at the main leads and the battery internally disconnects like this, you end up with a voltage differential between balance leads that is your main battery voltage of like 45 volts or whatever. This translates to your BMS balancing circuitry and can seriously damage things.

You NEED to make sure this battery is complete and solid before you test using it, do NOT try and power anything, not even just plugging in a VESC and turning it on. Make that connection solid.
```

---
## \#11 Posted by: trigger4point7 Posted at: 2018-05-14T07:58:54.784Z Reads: 93

```
Ah I see. Thanks.for that explanation. Do you think just a multimeter would qualify as a load?
```

---
## \#12 Posted by: Namasaki Posted at: 2018-05-14T11:44:35.750Z Reads: 83

```
[quote="trigger4point7, post:8, topic:55364, full:true"]
Is that as easy as separating the two e switch wires?
[/quote]

Yes
10 characters
```

---
## \#13 Posted by: TowerCrisis Posted at: 2018-05-14T15:35:01.456Z Reads: 69

```
A multimeter should be okay because ideally they have infinite resistance between the two probes. But to be on the safe side I really would make that connection solid.
```

---
## \#14 Posted by: banjaxxed Posted at: 2018-05-14T23:11:21.000Z Reads: 62

```
I know it's weird but smell the bms, it may need a refill![IMG_8843|225x225](upload://b5KFxTfEaOaxqyUTg0d4d5qgHbm.JPG)
```

---
## \#15 Posted by: pixelsilva Posted at: 2018-05-15T08:56:27.212Z Reads: 54

```
This is why I either buy some Zippys or commission an expert to do my Li-ions. Stop pretending we are electronic know all freaks when we are in reality very capable of ruining our cell packs in a thousand different ways.
```

---
## \#16 Posted by: trigger4point7 Posted at: 2018-05-15T14:14:51.481Z Reads: 46

```
I didn't ask you dude.
```

---
## \#17 Posted by: pixelsilva Posted at: 2018-05-15T15:45:13.950Z Reads: 39

```
I wasn't replying to you. So don't worry.
```

---
## \#18 Posted by: trigger4point7 Posted at: 2018-05-17T03:02:05.915Z Reads: 31

```
So I soldered down that series connection, set the lead wires back up, in a temporary configuration and this happened... I get a reading with out one of the lead wires P 10) connected. That shouldn't happen right? I've read in a few places that the Bestech BMS won't turn one with out all the parallel packs connected.

![IMG_20180516_195701|666x500](upload://s5kgJuh35Hv0u80XIuJgEth5P3J.jpg)
```

---
## \#19 Posted by: trigger4point7 Posted at: 2018-05-17T05:48:12.603Z Reads: 27

```
Annnnnndddddd, it caught on fire. I think it might have been a bad unit. I could have done something wrong, certainly. My process was, I hooked up the main battery negative lead to B- and then the lead wires, I may have brushed against them moving around but I can't think of what I could have done to cause such a ruckus with the BMS. Any ideas? I'll try again on my spare one but I'll wait for suggestions first.
```

---
## \#20 Posted by: trigger4point7 Posted at: 2018-05-17T05:50:13.112Z Reads: 27

```
It was sitting ideal for about an hour before it blew up so maybe it was me. Ugh.
```

---
## \#21 Posted by: L3chef Posted at: 2018-05-17T06:02:09.395Z Reads: 25

```
[quote="trigger4point7, post:19, topic:55364"]
Annnnnndddddd, it caught on fire
[/quote]

The bms caught fire and not the battery pack right?
```

---
## \#22 Posted by: trigger4point7 Posted at: 2018-05-17T06:05:52.575Z Reads: 24

```
Correct. 10 char
```

---
## \#23 Posted by: trigger4point7 Posted at: 2018-05-17T06:08:16.441Z Reads: 24

```
No damage to the pack at all. Cells were perfectly cool. No Sparks. No burn marks on the leads from Sparks I couldn't see it hear, lead wires look like the came out of the box.
```

---
## \#24 Posted by: trigger4point7 Posted at: 2018-05-23T02:37:45.725Z Reads: 17

```
So I'm back with a new BMS, and soldered down cell leads. I'm seeing an issue where when I get 34.29V when the e-switch leads are connected and 33.67V when they're unconnected. I don't understand that. Ideas?
```

---
