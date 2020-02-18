# VESC from Enertion: DRV8302 spectacularly blown, what went wrong?

### Replies: 21 Views: 2295

## \#1 Posted by: EvanAndDadProd Posted at: 2016-08-16T12:30:17.112Z Reads: 223

```
It looks like the DRV8302 of my VESC has suffered a massive failure. It was purchased from Enertion earlier this year and wasn't ridden particularly hard. I started braking, the board came to a halt and never restarted. My friend told me that some smoke had come out and here's what I found:

<img src="/uploads/db1493/original/2X/9/9dd109d2b857c0bd632792fa7ab64c049ef103ec.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/e/e4e8442626964c34a6b03ecbc67e05c8f781fc01.jpg" width="666" height="500">

I saw a few comments about bad capacitors triggering that issue. My questions are:

* Is there a most likely cause to this issue?
* How can I ensure it doesn't happen again with a new VESC?

HW config details:

**Motor: 3.2kW 63mm motor:**
> KV: 170
> MAX POWER: 3200W
> WIRE WINDS: 10
> MAX AMP: 80A
> MAX VOLT: 10S
> RESISTANCE: .56
> NO LOAD CURRENT: 1,4

**Battery pack:**
> 2x 5s in series
> 8000 mAh
> 30C discharge
> 5C max charge rate
```

---
## \#2 Posted by: Skitzor Posted at: 2016-08-16T13:05:40.631Z Reads: 212

```
Wooow, that's one for on the wall ! Also curious on how to extra-protect the DRV chip since I also blewn one already (BLDC)
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-08-16T13:07:59.151Z Reads: 213

```
What is your enclosure made of? Because carbon enclosure can shred, leaving bit of highly conductive carbon shorting the board.

EDIT: also you need to give your drv some love... or it can cry tear of fire.. :slight_smile:
```

---
## \#4 Posted by: Lizardking0069 Posted at: 2016-08-16T13:14:17.825Z Reads: 207

```
My guess is a small metal debris getting between the pads of the controller chip.
```

---
## \#5 Posted by: Blasto Posted at: 2016-08-16T13:22:08.212Z Reads: 199

```
That almost looks like a massive overvoltage failure, does your soft switch allow to regen the battery?
```

---
## \#6 Posted by: EvanAndDadProd Posted at: 2016-08-16T16:41:23.980Z Reads: 181

```
Hey @JohnnyMeduse, the enclosure is made of ABS.
```

---
## \#7 Posted by: EvanAndDadProd Posted at: 2016-08-16T16:42:53.137Z Reads: 174

```
@Blasto, yes the soft switch does allow to regen the battery, it's been working fine that way for the last few months.
```

---
## \#8 Posted by: Blasto Posted at: 2016-08-16T16:47:58.575Z Reads: 173

```
I just looked at the high rez, man that is some massive roastage, not sure the pcb is salvageable. C39 just blew up, no where to be found.
```

---
## \#9 Posted by: sl33py Posted at: 2016-08-16T17:01:25.152Z Reads: 174

```
WOW.  That's pretty epic.  Sucks, but impressive failure.  This obviously isn't the usual DRV failure, so i'm not sure anyone here can tell you how to avoid.  Did you do anything differently?  Were you braking down a steep hill with the battery already full charged?  That voltage has to go somewhere... but i'm just guessing.

It might be worth posting on vedder.se forum and seeing what they say - but be as specific as you can on details.  Might also send back to Vedder to do VESC autopsy!

GL!
```

---
## \#10 Posted by: Dornacht Posted at: 2016-08-16T17:08:33.834Z Reads: 166

```
My vesc also went but on the first trial run, in bldc, still waiting to hear from warranty

 <img src="/uploads/db1493/original/2X/1/1d00f4bcbf9aceff303825c4740bebb91541a3db.jpeg" width="375" height="500">
```

---
## \#11 Posted by: chaka Posted at: 2016-08-16T17:58:29.627Z Reads: 162

```
> Might also send back to Vedder to do VESC autopsy!

I sure Benjamin would love that! Just the other day he was telling me how much free time he has. :sweat_smile:
```

---
## \#12 Posted by: sl33py Posted at: 2016-08-16T18:47:25.929Z Reads: 158

```
LOL - yeah, i know.  However i know he's done this in the past.  Not quickly, but still may be worth looking at.  When he can get to it...
```

---
## \#13 Posted by: treenutter Posted at: 2016-08-16T19:20:39.023Z Reads: 150

```
@EvanAndDadProd wow that's probably the worst one I've ever seen!
```

---
## \#14 Posted by: EvanAndDadProd Posted at: 2016-08-17T19:27:32.708Z Reads: 127

```
I've posted the question on vedder.se as suggested. We'll see what comes out. The thread is [here](http://vedder.se/forums/viewtopic.php?f=7&t=334).
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-08-17T19:36:28.148Z Reads: 122

```
this deserves some kind of award. Its as if Lord Skatan reached in and shot fire into the heart of this poor bastard himself.
```

---
## \#16 Posted by: Mobutusan Posted at: 2016-08-18T03:09:36.388Z Reads: 111

```
Did those heat sinks come with the  Enertion VESC? I thought Chaka was the only one that had those.
```

---
## \#17 Posted by: EvanAndDadProd Posted at: 2016-08-18T05:16:54.630Z Reads: 101

```
They were ordered off eBay separately.
```

---
## \#18 Posted by: kyo Posted at: 2016-08-18T06:51:45.605Z Reads: 95

```
@EvanAndDadProd 
Hi, can i ask how did you stick the haet sink on the vesc?
```

---
## \#19 Posted by: EvanAndDadProd Posted at: 2016-08-18T07:55:55.157Z Reads: 95

```
@kyo: Sure, I used a thermal glue I found on eBay: http://www.ebay.co.uk/itm/Halnziye-HY910-10g-Tube-White-Silicone-Thermal-Plaster-Glue-Adhesive-Paste-/121174513266?hash=item1c36905672
It takes a few hours to settle and then it's relatively robust.

While I'm at it, here are the heatsinks that I used : http://www.ebay.co.uk/itm/New-High-Quality-Aluminum-Heat-Sink-For-Memory-Chip-IC-3-Sizes-UK-Seller-/281757356192?var=&hash=item419a0c10a0
```

---
## \#20 Posted by: kyo Posted at: 2016-08-18T09:17:49.134Z Reads: 95

```
Thanks man, appriciate it :smile_cat:
```

---
## \#21 Posted by: EvanAndDadProd Posted at: 2016-09-05T13:21:15.928Z Reads: 78

```
Quick update: The post on vedder.se forum didn't turn up anything material in relations to the failure. I found out in passing that the heatsinks I've added only have cosmetic value but are not playing a significant role in keeping the VESC cool.

Anyway, I'm now suspecting the soft switch: 
Does anyone know what would happen if the soft switch opened the circuit after I started braking, for instance because it's overheating? would the current generated by the braking continue to power up the VESC until it blows up because this current has nowhere to go? Would that be consistent with the failure that I experienced?

Equally, what if the power switch kept the circuit closed but temporarily prevented battery regen for some reason, would the result be consistent with what I got? 

Specs of the soft switch here in case it helps. 
http://wiki-en.rc-electronic.com/index.php/SPS_SafetyPowerSwitch
My model is the discontinued SafetyPowerSwitch 60V 60/120A.

Any further help to understand what's wrong with our design would be greatly appreciated.
```

---
