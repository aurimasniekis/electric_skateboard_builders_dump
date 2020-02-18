# How do volts translate to battery capacity?

### Replies: 12 Views: 297

## \#1 Posted by: SlayBO Posted at: 2018-10-29T13:45:03.279Z Reads: 121

```
If I'm running a 12s4p setup of 30q cells 100% capacity = somewhere around 50 volts, right?  But 25 volts doesn't translate to 50% of my battery indicator showing because its not safe to take the battery all the way down to 0 volts.  But from there I'm lost.  How do volts translate to my batteries % indicator?
```

---
## \#2 Posted by: linsus Posted at: 2018-10-29T13:50:44.767Z Reads: 121

```
um. Lithium-ion cells(most chemestries) normally have an operating range of 2.9-4.2. (depends who you ask, its abit biblical)
Normally you dont want to charge them absolutely to the brim full. And maybe stop discharging at 3.2V in case one parallell group is drifting. The Voltage level is not really linear so its hard to really say exact percentage of the battery. But the cheap ones from ebay give some indication atleast. If you were to be precise you want to look at the current rather then the voltage level. keeping track of how many amp hours you've consumed f.e
```

---
## \#3 Posted by: linsus Posted at: 2018-10-29T13:52:21.624Z Reads: 114

```
To answer your question. your battery is full at 4.2x12=50.4V
And "empty" at 3.0x12=36V
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-29T13:53:27.459Z Reads: 110

```
[quote="linsus, post:2, topic:72704"]
an operating range of 2.9-4.2V
[/quote]
2.5-4.2V 😉
```

---
## \#5 Posted by: linsus Posted at: 2018-10-29T13:54:35.896Z Reads: 109

```
[quote="Andy87, post:4, topic:72704"]
2.5-4.2V :wink:
[/quote]

daredevil..
```

---
## \#6 Posted by: SlayBO Posted at: 2018-10-29T13:55:50.797Z Reads: 105

```
So, would mah translate in a similar manner?  The cells carry 3000 mah, so somewhere around 36k mah for the pack?  Once I'm down to 25k mah the battery is essentially done?
```

---
## \#7 Posted by: linsus Posted at: 2018-10-29T13:59:28.615Z Reads: 103

```
What. No. mAh is only multiple in parallell. So 3000x4=12 000 mAh top capacity. When you've drained 12 Ah from a full battery you've utilized 100% of the capacity. meaning empty
```

---
## \#8 Posted by: SlayBO Posted at: 2018-10-29T14:00:54.422Z Reads: 102

```
Got it.  Thank you.
```

---
## \#9 Posted by: linsus Posted at: 2018-10-29T14:01:12.846Z Reads: 102

```
I guess you could also count watthours. But energy over time usually confuses people..
```

---
## \#10 Posted by: wafflejock Posted at: 2018-10-29T15:07:21.346Z Reads: 90

```
You can find discharge to percentage charts for total capacity vs voltage.  In terms of meausring how much power you're carrying or consuming Wh which is voltage times amps times time, so say 50V drawing 10A for 1hr is 50 x 10 = 500W, 500W x 1hr = 500Wh.  Really amperage is a roller coaster so you have to make an average amperage guess or use a bluetooth module for relaying the data (metr or ackmaniac)

In general something like
4.2V = 100%
4.1V = 95%
4.0V = 90%
3.9V = 80%
3.8V = 70%
3.7V = 60%
3.6V = 45%
3.5V = 30%
3.4V = 15%
3.3V = 0%

Basically when you are topped off voltage is 4.2 but quickly drops to about 3.6-3.8V range and most of the charge it's in that range then little bit of extra below the 3.6 range, if you want to see more than rough numbers you'd need to find the discharge graph for the li-ion or lipo you're using and check the area under the graph to see what percentage you'd have left... it's a bit more art than science though since under high load the battery will bleed off more power as heat from internal resistance and won't get the full capacity out of the battery, other environmental conditions like temperature will effect the battery chemistry as well.

One other thing to keep in mind the voltages in the list above are 'resting voltage' or voltage when there is no load (no motor/current).  When under load the batteries will drop the higher the C rating (lower the internal resistance) the less the voltage will drop but there is always a dip while the batteries are under load, you don't want them to go over the voltage cliff (drop to 0 quickly after 3V for most cells) or the cells will never recover completely.
```

---
## \#11 Posted by: cryo Posted at: 2018-10-29T16:28:28.353Z Reads: 53

```
Adding on to what others have said,

4.2v is when your battery is full and 2.5v is when your battery is empty. This is generally true for all 18650 cells, if it isn't, the datasheet will tell you(always check the datasheet for this info btw, its like the users manual). 

You CAN go above or below these values, but that is going against manufacturer specs and can cause a fire if you overcharge too far past 4.2 and reduce lifetime if you overdischarge past 2.5v(samsung states to discard cells if they ever reach 1.0v and to bring cells that are below 2.5 back up using very low current <1c). Most users on here dont even take their packs below 3.0v. Why? To preserve the number of cycles you can use the battery for and the capacity it can hold.

![30q1|690x424](upload://fC5h7pWVFiZeg9Zy9xKFWsIpRrr.png)  

Samsung did 300 cycles of charging at 4amps to 4.2v and discharging at 15amps to 2.5v. At the end of these 300 cycles, the cells now only hold 2.2ah instead of the original 3ah. Capacity dropping over time is inevitable but you can mitigate it by using conservative cutoffs. Charging to <4.2v, discharging to >2.5(3.3v like wafflejock stated above), and not pulling more than the specified amps (15a in the 30q) can preserve more of your cells capacity over its lifetime.

![30q|594x369](upload://frgE7linaL3TVJC53VU3nEunXNQ.png) 

If you cutoff at a higher voltage like 3.3v, you will get less amp hours out of your cell, so instead of getting 2.9ah from draining it till 2.5v... you only get 1.5ah to 2.2ah(depending on how many amps youre pulling). So effectively, its a tradeoff between the short-term vs long-term.
```

---
## \#12 Posted by: SlayBO Posted at: 2018-10-29T19:14:50.388Z Reads: 41

```
Awesome info.  Thanks everyone.
```

---
