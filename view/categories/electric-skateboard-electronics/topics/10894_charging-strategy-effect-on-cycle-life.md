# Charging strategy effect on cycle life

### Replies: 23 Views: 2377

## \#1 Posted by: Hillso Posted at: 2016-10-10T05:04:24.947Z Reads: 138

```
very interesting how a little difference in charging capacity prolongs the battery life.
http://blog.evandmore.com/lets-talk-about-the-panasonic-ncr18650b/
"**Now let’s look at the cycling chart. (Cycle Life characteristics)**
To estimate the number of cycles that the cell can undergo in its lifetime, we charge it at a maximal current of 0,5C and discharge at a current of 1C at 25 degrees Celsius and then we count the number of charge/discharge cycles until the cell degrades down to 70% of its initial capacity (2250mAh). In the case of these cells, the number is about 500 cycles.
500 cycles? But that’s (relatively) low! Yes. **But what is not shown on the spec sheet is that when you partially charge and discharge, degradation of the battery capacity is reduced. Thus, you can do over 40 000 charge/discharge cycles when going from 30% to 70% only. Or over 35 000 charge/discharge cycles from 20% to 80%; 28 000 cycles from 10% to 90%; 15 000 cycles from 8% to 92%, 7500 cylces from 6% to 94%, and the capacity reduction goes faster and faster, finally reaching 500 cycles when recharging from 0% to 100%.**
This explains the partial cycling strategies implemented by car manufacturers: GM limits the cycle from 17% to 80% of energy storage levels for the Volt. Nissan limits maximum charge level of the LEAF to 90% (4,15V). Tesla invites owners to limit the maximum load to 90%, and recommends avoiding deep depletion of the battery pack. All these strategies work well and significantly increase the number of battery cycles. When I manage the power levels of my own Tesla, I try to keep my maximum load below 90% and avoid depleting below 20%. Following this practice since the purchase of my Tesla, I have seen no capacity degradation. My wife’s 2012 Volt shows no degradation either. In fact, no Volt has yet shown degradation below 70% of the initial capacity which would have resulted in a warranty claim. In conclusion, we can trust the reliability of our Lithium batteries!"
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-10T05:09:59.012Z Reads: 127

```
This is also intersting

>Every 0.10V drop below 4.20V/cell doubles the cycle but holds less capacity. Raising the voltage above 4.20V/cell would shorten the life.

http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries
```

---
## \#3 Posted by: smurf Posted at: 2016-10-10T06:55:40.419Z Reads: 117

```
Would it really be that difficult to just build a 40V cccv charger?
```

---
## \#4 Posted by: Hillso Posted at: 2016-10-10T07:32:29.270Z Reads: 114

```
I don't think it's too hard, but than the bms might not reach it's balancing voltage.
```

---
## \#5 Posted by: smurf Posted at: 2016-10-10T08:08:26.357Z Reads: 111

```
Makes me wonder if balance is less of a problem with the under charging strategy because of the slower battery degradation
```

---
## \#6 Posted by: treenutter Posted at: 2016-10-10T19:01:13.084Z Reads: 94

```
[quote="smurf, post:3, topic:10894, full:true"]
Would it really be that difficult to just build a 40V cccv charger
[/quote]

@whitepony [has a thread where we discussed chargers that have customizable settings](http://www.electric-skateboard.builders/t/cheap-chargers-with-customizeable-end-of-charge-voltage/6902), so you could set the charger to only reach 41V on a 10S pack. This has very little impact on capacity per charge, extends battery life, and also eliminates some the issues with VESC and regen braking with a full battery. 

The only downside, AFAIK, is that a BMS (at least, the ones we tend to use) would not reach its balancing state, so cells could drift over time.
```

---
## \#7 Posted by: Jinra Posted at: 2016-10-10T19:07:32.542Z Reads: 86

```
Some Bestech BMS's offer adjustable balance voltage as well.
```

---
## \#8 Posted by: treenutter Posted at: 2016-10-10T19:08:56.342Z Reads: 80

```
Thx @jinra! that's great news! I have to look for those, unless you already have a link in mind...

btw groetech.de is completely down so now we also need to find another supplier for customizable chargers.
```

---
## \#9 Posted by: lox897 Posted at: 2016-10-10T19:11:06.918Z Reads: 81

```
Just buy straight from modiary on ali
```

---
## \#10 Posted by: Jinra Posted at: 2016-10-10T19:13:05.310Z Reads: 79

```
Nothing that I can show you right now, but if you look at some of their BMS's they offer adjustable balance voltage. You can also email batterysupports.com because I know Lilian does some custom work for her BMS's as well such as adding an e-switch.
```

---
## \#11 Posted by: treenutter Posted at: 2016-10-10T19:20:59.010Z Reads: 75

```
 Thx @lox897 I found them but I don't see that the charger is customizable.

https://www.aliexpress.com/store/product/36V-CHARGER/110119_32691047739.html?spm=2114.8147860.0.0.DvZjTb
```

---
## \#12 Posted by: treenutter Posted at: 2016-10-10T19:26:31.759Z Reads: 69

```
@Jinra this looks promising: http://bestechpower.com/communicationbms/BMS-D298V1.html
```

---
## \#13 Posted by: Jinra Posted at: 2016-10-10T19:29:55.019Z Reads: 69

```
Yea, but it also looks HUGE. Not sure how big it actually is though..
```

---
## \#14 Posted by: Jinra Posted at: 2016-10-10T19:37:40.192Z Reads: 63

```
Kind of wish I got this one as it's small and provides an e-switch. 

https://www.aliexpress.com/item/Free-Shipping-36V-lithium-ion-battery-protection-circuit-10S-36V-37V-15A-BMS-ON-OFF-switch/32736786030.html?spm=2114.01010208.3.1.xuynry&ws_ab_test=searchweb0_0,searchweb201602_3_10056_10065_10055_10068_10067_10054_10069_10059_10073_10017_10070_10060_10061_10052_10062_10053_10050_10051,searchweb201603_6&btsid=a562c776-1019-4db7-a366-0b929438cfc6

My current one is the same size but no e-switch, and I plan to bypass discharge anyway. Hopefully improvements in li-ion battery tech in the next few years makes worrying about cycle life a thing of past.
```

---
## \#15 Posted by: lox897 Posted at: 2016-10-10T20:16:34.803Z Reads: 58

```
@treenutter it has a potentiometer inside it
```

---
## \#16 Posted by: Luke Posted at: 2016-10-10T20:43:18.930Z Reads: 59

```
[quote="Hillso, post:1, topic:10894"]
Thus, you can do over 40 000 charge/discharge cycles when going from 30% to 70% only. Or over 35 000 charge/discharge cycles from 20% to 80%
[/quote]

What is most important here, charging the battery less in one cycle, or the final voltage when you're done with charging. 
I ask this because I often charge from 40% to 95% but if it's more beneficial I'm open to charging from 20 to 75 or 80% 
Not sure if I'm explaining myself well enough here
```

---
## \#17 Posted by: Jinra Posted at: 2016-10-10T21:52:46.446Z Reads: 54

```
final charging voltage, check out my link for more details. But the TL;DR is

> Every 0.10V drop below 4.20V/cell doubles the cycle but holds less capacity. Raising the voltage above 4.20V/cell would shorten the life.
```

---
## \#18 Posted by: Spek Posted at: 2016-10-10T22:11:29.162Z Reads: 51

```
So for someone like me with a prebuilt liion pack and a 4a charger, what's the best practice for charging? Letting it get to 95%? Also my volt meter will read 100% well before the chargers led goes from red to green which I've assumed is the individual cells just topping off that little bit. Currently I wait tIL the charger says it's done before disconnecting
```

---
## \#19 Posted by: Jinra Posted at: 2016-10-10T22:12:56.012Z Reads: 49

```
Charging to 100% is fine, but if you really want to extend the cycle life of your pack charge to 95% and avoid discharging under 20% when possible. Every once in a while charge up to 100% to balance your pack.
```

---
## \#20 Posted by: Spek Posted at: 2016-10-10T22:25:29.356Z Reads: 49

```
Thanks! Thats very helpful. I definitely want my pack to last. Most common scenario for me is commuting which takes it down to about 60% each day going to work, lunchtime joyride and ride home.  I've only been able to get my battery down to 20% once so that shouldn't be a problem. 

One more question: Does a 4a charger kill a pack faster than a 2a charger?
```

---
## \#21 Posted by: Jinra Posted at: 2016-10-10T22:32:34.113Z Reads: 48

```
Depends on the 'P' of your pack. The lower the current you charge with the better. Generally you don't want to exceed 1C charging, but you should be able to handle 2C max. A 4A charging charging a 4P battery charges each cell at 1A which is about .5C for 18650 cells. 4A charging should be good for the life of the pack assuming you're running a 4p pack. You can do the math to find out charging rates for other setups.
```

---
## \#22 Posted by: Spek Posted at: 2016-10-10T22:51:09.385Z Reads: 47

```
Yep, 10s4p. Thanks for the info, very educational :slight_smile:
```

---
## \#23 Posted by: Randyc1 Posted at: 2016-10-11T00:20:10.918Z Reads: 43

```
Here is mine moded by Modiary to 41V just like i asked ..<img src="/uploads/db1493/original/3X/8/f/8f25aa5927186721745b430b705487af121a8873.jpg" width="690" height="388">
```

---
