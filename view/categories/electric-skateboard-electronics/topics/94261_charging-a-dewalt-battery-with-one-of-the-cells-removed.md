# Charging a Dewalt battery with one of the cells removed

### Replies: 22 Views: 372

## \#1 Posted by: hamac2003 Posted at: 2019-05-18T19:08:34.256Z Reads: 77

```
I want to use 20 volt Dewalt battery packs as a power source for an electric longboard build, but I can't seem to find any ESCs that run off of 20 volts. And rather than buy a custom buck/boost converter to get the voltage into a more standard range (24 volts or 36 volts), I want to alter the Dewalt battery instead. From what I can tell, the batteries I have are 5s 2p, and each of the cells output 4.1-4.2 volts. So if I remove one of the cells from the series, then the battery becomes 4s 2p, and it would output 16 volts. I could then take an unaltered 20 volt battery pack, wire it in series with the modified 16 volt battery pack, to get a total of 36 volts.

My question is whether I would be able to charge the modified 16 volt battery pack on a standard Dewalt charger. From what I can tell, as long as I close the circuit after removing a cell from the pack, the battery should charge normally. The smarts of the charger should just think that the missing cell has a charge of 0 volts.
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-05-18T19:22:11.685Z Reads: 70

```
[quote="hamac2003, post:1, topic:94261"]
seem to find any ESCs that run off of 20 volts
[/quote]

20v is too low of a voltage to get much speed or torque

Although you can probably use vesc on 20v
```

---
## \#3 Posted by: hamac2003 Posted at: 2019-05-18T19:50:08.788Z Reads: 61

```
That doesn't really answer my question, but thanks for the heads up.
```

---
## \#4 Posted by: J0ker3366 Posted at: 2019-05-18T20:12:10.745Z Reads: 54

```
@skatardude10, you have some experience with power tool batteries. Wanna hold his hand through it lol?
```

---
## \#5 Posted by: skatardude10 Posted at: 2019-05-18T20:16:25.764Z Reads: 51

```
Sure! 

OP, why don't you just put two unmodified batteries in serial? Why modify one?

Modifying power tool batteries is a pain, and it probably won't charge, or worse, if you try to charge a modified (to 4s) battery. The little balance board will probably detect no cell and cause it to not work, blinking red light or something. 

Feel free to try it, but not modifying anything and just slotting them in in series will work and is painless.
```

---
## \#6 Posted by: hamac2003 Posted at: 2019-05-18T20:24:32.797Z Reads: 47

```
> OP, why don’t you just put two unmodified batteries in serial? Why modify one?

Mainly because I was hoping to use [this ESC](https://usa.banggood.com/2436V-Single-Motor-Electric-System-Driver-Noninductive-Longboard-Skateboard-Controller-p-1381110.html?gmcCountry=US&currency=USD&createTmp=1&utm_source=googleshopping&utm_medium=cpc_bgcs&utm_content=garman&utm_campaign=pla-usg-all-pc&gclid=CjwKCAjw8e7mBRBsEiwAPVxxiOKQrJbTe_mzeM1Jb5Lw1TDoJjJkpB60CRVjfnXM-9Dq00WvslOcExoCWuIQAvD_BwE&ID=516800&cur_warehouse=CN) which appears to only operate on 24v or 36v. I may just end up having to purchase a more expensive ESC that tolerates a wider range of input voltages, but I don't really want to have to pay $100+ just for the controller :roll_eyes:
```

---
## \#7 Posted by: J0ker3366 Posted at: 2019-05-18T20:28:25.618Z Reads: 48

```
Invest into a VESC! There are affordable options for a budget board. Plus when you realize the voltage youre running isnt enough fun, the vesc can already handle up to 60v (iirc).

Dont skimp out on your battery or vesc. Those are the blood and brains of your board. Spend the extra money for a vesc. Youre welcome lol
```

---
## \#8 Posted by: skatardude10 Posted at: 2019-05-18T20:30:14.912Z Reads: 45

```
Are you sure it's not 36v nominal on the ESC? 10S, or 2x 5S (if you know for sure that's whats in the batteries) is 36v nominal.
```

---
## \#9 Posted by: hamac2003 Posted at: 2019-05-18T20:37:15.062Z Reads: 46

```
To be honest, I'm not entirely sure. The documentation on that ESC is severely lacking. But I'm not surprised as the price is so cheap. "Rated Voltage: 24V / 36V (optional)" This is literally the only mention of a rated voltage for that ESC.

Can you explain why 2x 5s batteries have a 36v nominal voltage? Is it simply because the battery packs are almost never at full capacity?
```

---
## \#10 Posted by: J0ker3366 Posted at: 2019-05-18T20:42:28.849Z Reads: 42

```
I do believe that esc is the one you have to bridge balance pins to change from 6s to 10s. 

Bruv. Seriously. Invest into a VESC. Torque Boards makes a great 4.12. Flipsky as well. 

You could probably search "vesc for sale" in the forum search and mostly likely find one around your budget. Hell, go here
 https://www.electric-skateboard.builders/t/wanted-cheap-or-free-in-progress-requests-only/60454
and say youre looking for a single 4.12 vesc. See what bites you get. 

Also, update your profile info. Youll get more bites that way.
```

---
## \#11 Posted by: Dirt_Bag Posted at: 2019-05-18T21:12:07.898Z Reads: 31

```
is there anyway to run tool batteries in series if you bypass the internal bms?
```

---
## \#12 Posted by: hamac2003 Posted at: 2019-05-18T21:15:49.041Z Reads: 31

```
Why can't you just link the B+ B- pins in series? Where does the internal bms come into play?
```

---
## \#13 Posted by: Dirt_Bag Posted at: 2019-05-18T21:16:25.054Z Reads: 30

```
all  power flows through it, they shut off the batteries before damage is done
```

---
## \#14 Posted by: hamac2003 Posted at: 2019-05-18T21:18:29.743Z Reads: 31

```
So that means if I were to link the B+ B- pins in series, the internal bms would shut off the batteries?
```

---
## \#15 Posted by: Dirt_Bag Posted at: 2019-05-18T21:19:59.130Z Reads: 29

```
it would probably fry the bms. you need to get inside and discharge straight from the cells from a new set of wires. i think it could be done like that easily, but figuring out wiring for the bms to still hook up to a charge might be hard
```

---
## \#16 Posted by: hamac2003 Posted at: 2019-05-18T21:25:38.727Z Reads: 28

```
[This guy](https://www.youtube.com/watch?v=ISR8pKoIa5k) made an E-Bike using Dewalt batteries in series to power it. And based on his description I wouldn't say he made any significant modifications to the batteries. So either he came up with some sort of fix for the problem you are proposing without mentioning it in his video, or it is a non issue. @skatardude10 Any comment?
```

---
## \#17 Posted by: b264 Posted at: 2019-05-18T21:43:43.130Z Reads: 26

```
The VESC 4.x can work down to 8 or 9V, if I recall.  I'd recommend using one.  The top end is arguable, but around 40V to 55V.  I wouldn't run them over 44V.
```

---
## \#18 Posted by: b264 Posted at: 2019-05-18T21:44:46.785Z Reads: 26

```
[quote="hamac2003, post:1, topic:94261"]
I want to alter the Dewalt battery instead. From what I can tell, the batteries I have are 5s 2p, and each of the cells output 4.1-4.2 volts. So if I remove one of the cells from the series, then the battery becomes 4s 2p, and it would output 16 volts. I could then take an unaltered 20 volt battery pack, wire it in series with the modified 16 volt battery pack, to get a total of 36 volts.
[/quote]

You'd be much better off not removing the cell, and just using all ten in series.

So the answer to your question is N/A - not applicable.

10S li-ion will range from 42.0V fully charged to 30V fully dead and is commonly labeled "36V"

Be liberal with your cutoffs using cells like that, make sure the cutoff start is very high, like 36.5V cutoff begin and 30.0V cutoff end
```

---
## \#19 Posted by: hamac2003 Posted at: 2019-05-18T22:17:22.204Z Reads: 23

```
Do you have any idea about the possible issue Dirt_Bag mentioned?
```

---
## \#20 Posted by: b264 Posted at: 2019-05-18T23:35:52.502Z Reads: 21

```
You probably will have to bypass the internal BMS for discharge.
```

---
## \#21 Posted by: hamac2003 Posted at: 2019-05-18T23:42:34.938Z Reads: 21

```
Is there a specific reason for this? Does the BMS not allow the batteries to be wired in series due to power flowing in and out of the batteries? It probably wouldn't be too difficult to add some sort of separate cable for discharge. What would the BMS do if I tried to wire two batteries in series? Would they just quit and not provide any voltage?
```

---
## \#22 Posted by: b264 Posted at: 2019-05-18T23:57:48.048Z Reads: 20

```
[quote="hamac2003, post:21, topic:94261"]
Is there a specific reason for this?
[/quote]

BMS will limit current at a number much too low.

[quote="hamac2003, post:21, topic:94261"]
Does the BMS not allow the batteries to be wired in series due to power flowing in and out of the batteries?
[/quote]

No, it has no control over that.
```

---
