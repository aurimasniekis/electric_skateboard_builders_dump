# Best BUDGET way to test battery capacity on 10S2P Setup

### Replies: 13 Views: 252

## \#1 Posted by: myles.drake Posted at: 2019-02-12T04:49:31.823Z Reads: 89

```
Hey guys!

Been learning a lot from this forum. Want to first start by saying thank you to this community as it's been tremendously valuable to me.

So I have a battery pack out of a hoverboard. Its advertised at 36V 4400mah. What would be the cheapest way to accurately measure that it ACTUALLY has 4400mah? There is only an XT60 connector popping out of it and I'd rather not rip it apart and test each cell .... 

Currently I'm charging it up with a cheap 42V charger with an XT60 connector on the end of it and its working great, but it obviously can't tell me the capacity.

Could I theoretically .... discharge it to a known voltage (like 30 Volts) and then assume that my charger is charging at 42V 2A consistently, and track how long it takes to charge to 42volts? And calculate from there?

I'm hoping not to drop $135 on an iCharger 1010B+ .... 

Would love to hear your thoughts, thank you very much!
Myles
```

---
## \#2 Posted by: Andy87 Posted at: 2019-02-12T05:00:58.089Z Reads: 79

```
[](http://)
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-02-12T05:06:50.850Z Reads: 73

```
my thoughts exactly
```

---
## \#4 Posted by: pat.speed Posted at: 2019-02-12T05:10:25.023Z Reads: 74

```
That will give you a rough estimate but not very accurate as he charger starts to charger slower as it reaches full charge.

Your best bet is to find a known load between 500ma and 2a and connect that to then battery when fully charged and see how long it takes to discharge as this load will be constant
```

---
## \#5 Posted by: J_Dizzle Posted at: 2019-02-12T05:18:01.075Z Reads: 70

```
Or you could buy a battery meter... :thinking:
```

---
## \#6 Posted by: pat.speed Posted at: 2019-02-12T05:28:55.197Z Reads: 66

```
That doesn’t tell you Ah tho. A watt meter connected to a load will also tell you how many Wh and Ah have been drawn
```

---
## \#7 Posted by: myles.drake Posted at: 2019-02-12T05:57:08.876Z Reads: 66

```
Thanks man,

Any suggestion for a constant load?

Actually would something like this work?

https://www.ebay.com/itm/100A-60V-DC-RC-Helicopter-Airplane-Battery-Power-Analyzer-Watt-Meter-Balancer-QU/292855818390?hash=item442f912896:g:fKYAAOSw4CFYwqYO:rk:9:pf:0
```

---
## \#8 Posted by: myles.drake Posted at: 2019-02-12T06:07:31.825Z Reads: 57

```
The reviews on Ebay for a few of them say that they're cheap / chinese and inaccurate. So it would be a gamble, but I guess they're not too expensive to try out right?
```

---
## \#9 Posted by: pat.speed Posted at: 2019-02-12T06:26:08.946Z Reads: 50

```
I’ve got one, it seems accurate enough. I use it to monitor charging through my boost converter. You just need to add a load onto it, an esc powering a motor on the bench should be enough to drain it after a few hours. Another option is some high current lights connected in series to handle the voltage. 

A load resistor is the best bet but can be expensive
```

---
## \#10 Posted by: myles.drake Posted at: 2019-02-12T07:32:47.490Z Reads: 40

```
Could you hook it up in reverse so its going from the charger to the battery? And then monitor how much energy the charger is putting into the battery?
```

---
## \#11 Posted by: b264 Posted at: 2019-02-12T07:33:26.752Z Reads: 40

```
https://www.aliexpress.com/item/7-in-1-OLED-Electrical-Parameter-Meter-Power-Meter-Voltage-Current-Time-Power-Energy-Capacity-Temp/1000001907208.html
```

---
## \#12 Posted by: dareno Posted at: 2019-02-12T07:36:26.776Z Reads: 42

```
What a well thought out reply.
```

---
## \#13 Posted by: pat.speed Posted at: 2019-02-12T09:48:23.479Z Reads: 38

```
Yep, that will work too. I didn’t think of that even though that’s exactly what I do lol
```

---
