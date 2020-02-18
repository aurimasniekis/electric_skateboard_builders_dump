# Should I throw out this battery&hellip;..?

### Replies: 10 Views: 344

## \#1 Posted by: Komamtb Posted at: 2019-02-08T08:59:32.912Z Reads: 169

```
I have an old Koowheel battery.
![IMG_20190208_104318|375x500](upload://k7hX25cKdWXWzpPAPeyZexTely.jpeg) 

CONDITION: Used for 8 months with koowheel during summer and winter.  
Stayed in the garage for ~1.5 years from -15 to +30.
 I found it at 25volts. Was charged to 46v.
Cells are 4.6-4-3.

PROBLEMS: It doesn't seem to stop charging at the right voltage. 
(Is it because of unbalanced cells?)

If I do motor detection, the motor just stutters, Vesc shows a pink light and shuts off. 
(Amp cutoff?)
After that the battery is at 25v.
(Goes right back up if I plug the charger, so some sort of bms safety feature?)

The bms is unknown for me, I seted a 30bat draw, it should be capable of that?
![IMG_20190208_104356|375x500](upload://mFSX3aW7ByYPCyB7FukRJJND5a4.jpeg) 

All in all I would use it in a quick and dirty second build, so I don't expect much, but also not sure if I should use this battery at all. What do you think guys?
```

---
## \#2 Posted by: linsus Posted at: 2019-02-08T09:01:02.059Z Reads: 156

```
[quote="Komamtb, post:1, topic:83571"]
Cells are 4.6-4-3.
[/quote]

and then down to 25V pack voltage after detection? Toss that shit
```

---
## \#3 Posted by: Komamtb Posted at: 2019-02-08T09:03:20.053Z Reads: 153

```
Yeah, but it goes back the second I plug the charger in, It kinda re opens the whole circuit? Atleast that is what I think, I had a like problems with a bestech bms. Or this is not possible?
```

---
## \#4 Posted by: TowerCrisis Posted at: 2019-02-08T09:08:24.085Z Reads: 149

```
If you wanna rule out the electronics being at fault, bypass the BMS by hooking up your vesc directly to the battery terminals instead of the xt90.

Alligator clips have always worked for me for bench tests, just limit your vesc battery current to ~5 amps or so. Motor detection and free-spin tests should work fine.

However, I suspect it's destiny is to be binned.
```

---
## \#5 Posted by: banjaxxed Posted at: 2019-02-08T09:12:19.727Z Reads: 137

```
Being a hoarder I could never bring myself to toss it. Just get rid of cells then you have a handly little carcass to put new cells into or give to someone who does? free area of parts market section?
```

---
## \#6 Posted by: Komamtb Posted at: 2019-02-08T09:16:31.614Z Reads: 125

```
well I would use the carcass, since it makes very easy to work with, on the other hand, If I would be buying new cells, going 10s3p would make a lot more sence, for not a whole much more buck, on a third hand, the build would not be quick and dirty. Well eventualy I think I would build it up to be a decent ride.
```

---
## \#7 Posted by: Narnash Posted at: 2019-02-08T13:09:07.966Z Reads: 95

```
either disassemble all cells and check them all individually (charging, IR, high/low discharge check + checking temps while doing that and at the end a capacity check) than you could use the left cells for various non critical applications but I wouldn't recommend esk8 with them.

Lights, DIY power banks, electronic projects may applications for probably damaged but still OK leftover cells.
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-02-08T16:12:37.130Z Reads: 75

```
[quote="Komamtb, post:6, topic:83571"]
on a third hand
[/quote]


Ive never heard a third option being described that way and it really threw me off for a second 
![bestsideye|299x283](upload://OECt5OZvmbrN7jIqP9zIrTDyBA.gif) 

dumpster the battery though. it seems lost, My space cell did the same thing awhile ago, just watch it if you dont charge it, it will probably ' leak ' charge
```

---
## \#9 Posted by: barajabali Posted at: 2019-02-08T16:31:07.883Z Reads: 68

```
Don't just TOSS it 

If you just toss it without discharging it first this can happen.

https://www.youtube.com/watch?v=oKFOqMZmuA8
Skip to 2:24

You don't want someone to be injured/die or set a waste plant on fire due to negligence
```

---
## \#10 Posted by: Fiori Posted at: 2019-02-08T18:01:51.103Z Reads: 42

```
I'd rip it apart and save the individual cells for smaller projects. 

46v is way overcharged for this pack. 

Check each cells individual voltage, charge them with a small 18650 charger and then recheck after charging. 

Aside from the cells, the rest is garbage. And even the cells will be mediocre at best.
```

---
