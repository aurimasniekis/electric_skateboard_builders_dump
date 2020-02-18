# First Build! // Quest deck // Single 6374 190KV // 10S2P Basen 26650 // Nano-X // Kydex Enclosure

### Replies: 12 Views: 1477

## \#1 Posted by: landonkun Posted at: 2017-04-11T20:26:41.437Z Reads: 292

```
Hey guys! It's taken a while (damn shipping from China taking 3+ months for some things!), but I'm finally ready to start building my first board. :slight_smile: 

Parts list:

* Quest longboard deck (going to reshape and repaint it)
* Caliber II 50 degree trucks
* Single 6374 190kv motor (from the lovely @JLabs)
* 16/36 pulley kit
* 83mm Flywheel clones
* 10S2P Basen 26650 with BesTech BMS
* Maytech VESC
* Turnigy HV SBEC 5A Switch Regulator (8-42V input)
* 4.4kW High Power Switch for the VESC (from Current Control Systems)
* DROK battery capacity monitor
* Nano-X remote
* Kydex sheets for enclosure

I'm having the battery pack built by a friend. He does a lot of e-bike batteries :slight_smile:
I was recommended to buy the SBEC as a bonus add-on, but I have no idea what it does/where it connects to.

Here's where I'm asking for help! I want to make sure I have everything connected in the right order, because I will not be soldering this myself. I generally know where things go, but I'm a little fuzzy on what order the switch and LCD go in, etc.

**Would anyone be kind enough to draw up a diagram for me showing me what wires go where? I'll buy you a Jamba Juice. First Try!**

(battery pack not pictured)

<img src="/uploads/db1493/original/3X/a/1/a1d171fda8bbd8c1164565969cd6065575a909b6.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/5/7/5740b78c9ed72f227b31628bccb349361441c3c7.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/8/081bd78781370b7c809d5e3de5076f6e3ccc1b42.jpg" width="666" height="500">
```

---
## \#2 Posted by: JLabs Posted at: 2017-04-11T20:40:58.373Z Reads: 271

```
The 3 prong connector coming off the VESC plugs into channel two on the nano x receiver, black(brown) on the left. The 3 motor leads connect to the VESC. You solder the battery leads to the in of the switch (red to red, black to black) and then the VESC to the output of the switch. You can snip the connector off of the battery monitor and solder it right to the output of the switch. That should be about it, I'm not sure what the other thing you have there is used for.

I don't currently have the recourses to draw a diagram, but I would if I could.
```

---
## \#3 Posted by: landonkun Posted at: 2017-04-11T21:35:06.072Z Reads: 250

```
You are too kind. 
Where does the charge port go? I have a standard DC jack.
I'm also not sure where I should be using the anti spark xt90s, and where I can use the xt60s.
```

---
## \#4 Posted by: JLabs Posted at: 2017-04-11T21:48:21.923Z Reads: 236

```
Since you have an antispark switch you can use XT60's everywhere. It wouldn't hurt to upgrade to the XT90's tho for added protection (if you have enough of them).

What battery are you using? (Helps me help you)
```

---
## \#5 Posted by: landonkun Posted at: 2017-04-11T22:12:13.689Z Reads: 222

```
Only four xt90s. I was thinking of ordering more.
Basen 26650 in 10S2P config, so 80A continuous (realistically more like 60A, according to Namasaki).
```

---
## \#6 Posted by: JLabs Posted at: 2017-04-11T22:19:11.152Z Reads: 218

```
Ok, usually you solder  The negative end of the charge port to P- on the BMS. You then solder the positive end of the charge port to the positive end of the battery pack. 

I would verify that with your BMS schematic as I am not firmiliar with best tech
```

---
## \#7 Posted by: i2oadsweepei2 Posted at: 2017-04-12T10:52:13.729Z Reads: 188

```
Hey Landon, It's nice to see your build thread finally :) looking forward to battery building pics. Wink wink
```

---
## \#8 Posted by: landonkun Posted at: 2017-04-14T05:39:22.393Z Reads: 186

```
So, I'm going to connect a charge-only BMS (cause it only supports 15A) for now until my good BMS arrives next week, but the diagram I got for it is confusing the hell out of me.

<img src="/uploads/db1493/original/3X/5/3/53dde23d85db039278067d30486449e1c40204e4.jpg" width="655" height="500">

If I'm doing charge-only with this BMS, I'm assuming I just skip using the P-?

So...

_battery positive > charge port positive / anti-spark switch positive > ???_

_battery negative > B- > ???_

I am so lost between the battery, BMS, charge port, and anti-spark switch. Once I'm past this, I'm golden.
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-04-25T01:11:00.899Z Reads: 148

```
Did you get the temp bms all hooked up? What you asked makes sense to me. Skip the P- and use the B- inline to the esc for discharge. I've never had a bms before though so not sure if that's how it works. I have one on the way though.
```

---
## \#10 Posted by: misterchirinos Posted at: 2019-01-07T03:26:14.787Z Reads: 43

```
I'm looking into using the same deck, how does your board ride? How fast do you go, how do you feel at top speed (stability), what's your wheel base? Can't tell if that board is 44'' total length or shorter. The one I'm looking at has the same graphic in black.
```

---
## \#11 Posted by: landonkun Posted at: 2019-01-07T06:22:08.710Z Reads: 35

```
Honestly, I couldn't really tell you. I wound up chopping up that deck to make it shorter and a completely different shape, so it wouldn't have the same feeling as it was in its original form at 44". Sorry :sweat_smile:
```

---
## \#12 Posted by: misterchirinos Posted at: 2019-01-07T07:50:52.429Z Reads: 29

```
Haha well since it's shorter, I think if you feel comfortable at high speeds, I'll be fine. I'm aiming for a 30mph top speed. Where are you at? Also, can you post a pic of your board? I'm curious to see now
```

---
