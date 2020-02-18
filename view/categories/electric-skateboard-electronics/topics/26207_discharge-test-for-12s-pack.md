# Discharge test for 12s pack

### Replies: 6 Views: 428

## \#1 Posted by: thisguyhere Posted at: 2017-06-26T17:09:58.812Z Reads: 105

```
aside from using an expensive 12s balance charger, how can i discharge a 12s pack?

putting a new pack together right now and want to perform charge / discharge cycles before putting it into use.  charging is handled with a bms.

previous pack was a 10s and testing it wasn't a problem since i have a 10s balance charger.

thought about just getting some lightbulbs, or any device that would put a load on the circuit, but would probably be dreadfully slow to drain the pack.
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-26T17:48:25.160Z Reads: 92

```
Think high watt resistors are the cheap way to go for making an artificial load otherwise there are variable load battery testers, but I can't seem to find one rated for that kind of voltage so would need to drain them in sets at which point the resistors or lights sound like a better idea really.  I guess any sort of heater element is a good high wattage resistor too so if you've got any sort of heating elements laying around that could work (just you know don't set your place on fire).

https://www.amazon.com/Keenstone-Precision-Consumption-Performance-Measurement/dp/B06Y5DDK6N/ref=sr_1_12?ie=UTF8&qid=1498498568&sr=8-12&keywords=Battery+Load+Tester+high+voltage

^^ could hook something like that up in between the load and batteries to monitor the discharge too if you want to get some more detail about the discharge

Might want to just run the motor till it dies too although that might get annoying depending on how long that takes when there's no real load on the motor.

For the resistor something like the listing below could work.  If you hook all 5 in series you have 5Ohms so with 50V fully charged should be about 10A discharge rate and 100W per resistor to dissipate I think (don't quote me on this).

https://www.amazon.com/Accuni-Chassis-Aluminum-Wirewound-Resistor/dp/B01NAMG2L9/ref=sr_1_1?ie=UTF8&qid=1498498899&sr=8-1&keywords=high+watt+resistor
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-06-27T02:56:40.798Z Reads: 70

```
You could take 4 12v light bulbs and put them in series. That would surely draw some current if they were high enough wattage. Or, if you have 24v bulbs, use 2 in series. I've been thinking about putting something like this together to test my batteries.
```

---
## \#4 Posted by: krloz Posted at: 2017-06-27T08:57:47.801Z Reads: 58

```
I got a 2 ohm and a 10 ohm 100w resistor like the ones shown by wafflejock. Much cheaper from china
```

---
## \#5 Posted by: jmasta Posted at: 2017-06-27T14:16:34.042Z Reads: 45

```
I made a 200W 12s discharge rig from two power resistors, similar to those above. I used 2X 25 Ohm 100W resistors in parallel, so 12.5 Ohm overall, which gives about 4A discharge.  I can also hook them up in series for ~1A discharge.  It has the same DC port as my charger
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-06-27T16:45:12.869Z Reads: 36

```
gonna get these and put them in parallel:

<img src="/uploads/db1493/original/3X/5/8/58f4c30d0b295bc4d899832da4edb675910524b3.png" width="690" height="476">

http://www.ebay.com/itm/2-pcs-25-ohm-25-100W-Watt-Aluminum-Housed-Metal-Case-Wirewound-Resistors-/371887178559
```

---
