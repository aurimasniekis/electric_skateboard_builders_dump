# Went to grab board, had left on and battery is dead

### Replies: 14 Views: 308

## \#1 Posted by: moadymoad Posted at: 2019-05-25T14:40:50.444Z Reads: 136

```
I went to grab my board out after about 2 months of not riding (kids take up time apparently). Realised it had been left switched on when I last used it.

Charger isn’t charging the battery at all, checked with another board and it is charging. Nothing has changed since I last charged.

I assume the battery has over drained, is there anything I can do to get the pack charging again?
```

---
## \#2 Posted by: J_Dizzle Posted at: 2019-05-25T14:43:58.427Z Reads: 136

```
Try slow charging with a really low amp charger
```

---
## \#3 Posted by: DEEIF Posted at: 2019-05-25T14:44:11.722Z Reads: 131

```
Check the pack voltage, almost same thing happened to me...
```

---
## \#4 Posted by: moadymoad Posted at: 2019-05-25T21:29:29.191Z Reads: 103

```
I’ll borrow a multimeter, what happened with yours?

I’m pretty disappointed I’ve barely used it
```

---
## \#5 Posted by: DerelictRobot Posted at: 2019-05-25T21:46:24.892Z Reads: 98

```
[quote="J_Dizzle, post:2, topic:94930, full:true"]
Try slow charging with a really low amp charger
[/quote]

This is pretty bad advice until you have clarity on the voltage level of the battery. If the BMS isn't charging it, it might be below a safe voltage for recovery. 

Nothing should be done until you know the voltage level of that pack. If it's within a reasonable amount of drop (I won't try to recover anything below 2.9v per cell), sometimes batteries can be safely brought back up to a normal charge level but this should be done with extreme caution. Outside preferably and/or on cement with a fire extinguisher nearby.

Battery fires happen often from trying to force a charge on damaged cells.
```

---
## \#6 Posted by: kuphjr Posted at: 2019-05-25T22:01:45.242Z Reads: 90

```
Dude I've been there before.  Honestly, you are likely gonna have to replace the batteries. Its not the end of the world, but it sucks.  I've destroyed too many batteries to count...
```

---
## \#7 Posted by: moadymoad Posted at: 2019-05-25T22:08:47.681Z Reads: 86

```
Damn, pretty much a brand new pack and I don’t really ride enough to justify spending more money again.

Will probably just sell up if the pack is dead.

Will check voltage and go from there, might be able to send it back to the dude who built the pack to make it safe and replace damaged cells etc and work out a bit cheaper
```

---
## \#8 Posted by: JakeSkate Posted at: 2019-05-25T22:10:12.686Z Reads: 80

```
cells might still be fine, I'm guessing that your BMS probably has a low voltage cutoff and wouldn't let the cells discharge anymore hopefully. If the individual cells measure around 2.5v or more they might still be good depending on the manufacturer of them. HG2 cells for instance state that they should be used down to 2.0v so there is a very large range depending on the chemistry.

1.)measure individual parallel sections of the pack.

2.)use a bench power supply to charge the cells with a relatively low voltage 3.0v if they are 2.0-2.5v at around 1A or less of current(read the datasheet for the cells.)

3.)I would check the internal resistance if you have a meter otherwise plug it in outside and let it fully charge in a safe area, preferably concrete with a  metal container you can put over the top.

TLDR: Go for it dude. just take safety precautions.
edit: my spelling is awful lol
```

---
## \#9 Posted by: moadymoad Posted at: 2019-05-25T22:25:38.459Z Reads: 74

```
It’s bypassed BMS on discharge but there is a low voltage cutoff in the controllers (focbox)

Will get a multi and check cells today, then report back to work out the safest and best course of action
```

---
## \#10 Posted by: TinnieSinker Posted at: 2019-05-25T23:55:11.619Z Reads: 63

```
cells with quite often come back to life, but they will not have the same performance as they once did.

I've brought cells back from 0.5v, it was just two cells though. i set my charger to ni-mh and charged them just enough to get the volts within normal li-ion range then switched the charger mode to li-ion.

you made need to bypass the bms to bring the volts up to the normal range and use a lower volt charger at the start if you can else the battery could get too hot
```

---
## \#11 Posted by: moadymoad Posted at: 2019-05-26T00:45:40.589Z Reads: 55

```
Total pack is 4.2v didn’t measure individual P ranges as I don’t have another charger anyway.

I have a few local guys with more equipment to try and revive it
```

---
## \#12 Posted by: ryansinatra Posted at: 2019-05-26T00:51:31.402Z Reads: 49

```
If the total pack is at 4.2v.... that's not a good sign
```

---
## \#13 Posted by: moadymoad Posted at: 2019-05-26T00:53:03.138Z Reads: 49

```
Yeah...expecting it to be dead but hopefully can get it back to a little bit of life or I wasted $400 on the pack.

Probably only had 2 cycles through it
```

---
## \#14 Posted by: DEEIF Posted at: 2019-05-26T05:10:07.827Z Reads: 35

```
I left it turned off and the anti spark switch drained the battery. If you left it on it would have definitely drained. If you need help checking voltage contact me and I can link you to my thread.

Edit: Didn’t see that you already checked. It is un-revivable since a single fully charged cell should be at 4.2v...
```

---
