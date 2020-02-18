# SuPower BMS max charging amps?

### Replies: 7 Views: 1198

## \#1 Posted by: chinzw Posted at: 2016-10-20T18:40:39.906Z Reads: 150

```
Hey guys, so i finally got my BMS and its all hooked up and working nicely. Only issue i found is the balance charging completely stops after a cell hits 4.25v.

Also, i couldn't find on their website the max charging current the bms can handle, im guessing if they state 60A it can take in as much as it puts out, but im not entirely sure about this. Anyone using one of their bms and has more info can chip in?
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-20T20:44:46.614Z Reads: 142

```
Went back home and i realized the BMS was still balancing even when unplugged and all the cells were back to 4.2 :slight_smile:

Still want to know the max charging current if anyone knows.
```

---
## \#3 Posted by: chinzw Posted at: 2016-10-21T05:06:59.598Z Reads: 136

```
So, another issue im having, not sure if this is a problem or not; But the charger that SuPower sold me outputs 25.3V instead of 25.2V so all my higher cells charge up to 4.25V and then the balancer lowers them to 4.2V

Should i buy a use a buck converter and lower that 0.1V or am i being too picky?
```

---
## \#4 Posted by: Namasaki Posted at: 2016-10-21T05:31:35.305Z Reads: 129

```
Because the Supower charges through the same port that it discharges through, it should be able to handle the same amperage for both. 
Problem is lithium charge ratings are always lower than discharge ratings. So your  batteries will determine your max charge and regen limits. 
The good news is that this. BMS  should protect your battery against over voltage during regen braking so you can feel confident braking down hill even with a full battery. 
You should test this theory to be sure though. 
I have tested this theory with Bestech BMS but not Supower.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-10-21T05:41:03.167Z Reads: 124

```
Regarding your concern abt the voltage. 
I don't think going .05v over is gonna hurt. 
If it was a problem, Supower would have set the voltage limit lower. 
My Bestech's over voltage protection kicks in at 4.28v 
My 10s charger only gets it up to 41.9 but I've seen it go up to 42.3 while braking down hill with a full battery. As soon as I stopped braking the voltage dropped back down to 41.9.
```

---
## \#6 Posted by: chinzw Posted at: 2016-10-21T06:24:15.350Z Reads: 122

```
Awesome, thanks for the info! I'm gonna splice the balance wires and leave a lipo monitor hooked up all the time with a switch, it will give me more piece of mind.

I do love the fact that the bms keeps dumping through the bleed resistors even while unplugged :slight_smile:
```

---
## \#7 Posted by: Namasaki Posted at: 2016-10-21T06:39:57.505Z Reads: 113

```
[quote="chinzw, post:6, topic:11558"]
I do love the fact that the bms keeps dumping through the bleed resistors even while unplugged
[/quote]

That is also a good feature especially with Lipos, you don't have to worry about them swelling while  sitting around fully charged.

This is like the best of both worlds. The power of Lipos with the convenience of Li-ions
```

---
