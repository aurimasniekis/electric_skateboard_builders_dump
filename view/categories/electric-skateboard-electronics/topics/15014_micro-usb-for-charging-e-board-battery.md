# Micro USB for charging e-Board battery

### Replies: 32 Views: 2855

## \#1 Posted by: Eboosted Posted at: 2016-12-21T07:15:32.317Z Reads: 241

```
These newer cables have the ability to charge phones at 4A, could they handle charging an e-Board battery? 

I'd love to use these kind of magnetic adapter:


https://www.amazon.com/gp/aw/d/B01J4ZA26I/ref=mp_s_a_1_25?ie=UTF8&qid=1482304419&sr=8-25&pi=AC_SX236_SY340_QL65&keywords=Adapter+magnetic+micro
```

---
## \#2 Posted by: BoardSportsRN Posted at: 2016-12-21T07:26:01.716Z Reads: 241

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#3 Posted by: barajabali Posted at: 2016-12-21T07:28:48.316Z Reads: 239

```
14 if i remember right
```

---
## \#4 Posted by: BoardSportsRN Posted at: 2016-12-21T07:30:12.770Z Reads: 236

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#5 Posted by: Alextech Posted at: 2016-12-21T07:37:51.776Z Reads: 227

```
In most situations, No.  Charging cables are generally above 22awg and can't Handle the amperage or voltage.  It would be a firehazard also if you did try it,  you should stick with 18 and below to be safe if anything.  You can look up a chart for amperage to Awg wiring.
```

---
## \#7 Posted by: Eboosted Posted at: 2016-12-21T07:39:42.954Z Reads: 215

```
There must be a magnetic charger which supports 12awg currents
```

---
## \#8 Posted by: Maxid Posted at: 2016-12-21T07:45:58.049Z Reads: 213

```
total overkill. you only charge with 2-4A - almost every cable can handle that. 

@Eboosted Just look at my magsafe topic if you want a magnetic connector.
```

---
## \#9 Posted by: Mark Posted at: 2016-12-21T07:55:05.044Z Reads: 205

```
was about to ask the same, since im in a bus on my way to work atm and theres an usb charger in front of me.
```

---
## \#10 Posted by: Alextech Posted at: 2016-12-21T07:58:48.020Z Reads: 202

```
You'd have to use a voltage stepper from 5v to your max charge battery voltage lol
```

---
## \#11 Posted by: Maxid Posted at: 2016-12-21T08:06:34.433Z Reads: 195

```
we are not talking about USB chargers but magnetic usb cables.
```

---
## \#12 Posted by: rwxr Posted at: 2016-12-21T08:21:18.051Z Reads: 190

```
https://www.rosenberger.com/en/products/automotive/magcode.php

This supports currents 15A to 25A

http://www.lima-shop.de/en/product_info.php/info/p305_MagCode-Power-Port-Connector-16A-12V-24V-PowerSystem.html
```

---
## \#13 Posted by: Maxid Posted at: 2016-12-21T08:26:40.652Z Reads: 186

```
Rosenberger connectors are what mellow uses. They are huge however...
```

---
## \#14 Posted by: benwong Posted at: 2016-12-21T08:26:55.360Z Reads: 186

```
Wireless charge work? Like phone?
```

---
## \#15 Posted by: Maxid Posted at: 2016-12-21T08:27:56.854Z Reads: 178

```
No - there are no inductive chargers out there for the voltage we use.
```

---
## \#16 Posted by: Eboosted Posted at: 2016-12-21T15:00:18.248Z Reads: 164

```
Rosenberger look amazing, but I see they are only good for 24V, on a 10s4p the voltage would be 42V, would that be safe?
```

---
## \#17 Posted by: Maxid Posted at: 2016-12-21T15:04:20.398Z Reads: 160

```
typically the voltage rating is not as important as the current rating.
At 24 or 42V it usually does not matter.
```

---
## \#18 Posted by: treenutter Posted at: 2016-12-22T03:32:31.848Z Reads: 157

```
[quote="Maxid, post:17, topic:15014, full:true"]
typically the voltage rating is not as important as the current rating.At 24 or 42V it usually does not matter.
[/quote]

@Maxid could you explain more about how it doesn't matter? For battery systems that are above 24V (which is most of them for our use) wouldn't this port be unable to handle the voltage. For example, my 10S4P battery uses a charger that needs to reach 42V a full charge and for the BMS to balance the cells. 

I'm not disagreeing with you, I simply don't understand why we'd disregard the stated voltage rating.
```

---
## \#19 Posted by: Maxid Posted at: 2016-12-22T10:11:57.145Z Reads: 139

```
http://physics.stackexchange.com/questions/92502/why-do-high-current-conductors-heat-up-a-lot-more-than-high-voltage-conductors
```

---
## \#20 Posted by: PXSS Posted at: 2016-12-22T13:48:28.363Z Reads: 139

```
You wont be able to charge a 42V battery fully with a 24V charger without a step-up converter.
E: if we're talking about only the connectors then I agree, voltage doesn't matter.
E2: I lie. It probably has something to do with creepage or arcing, higher voltages need larger clearance to not arc
```

---
## \#21 Posted by: Maxid Posted at: 2016-12-22T13:59:14.139Z Reads: 136

```
At 24 or 42V the distance in air that would cause an arc is so small that you will not see a difference.
```

---
## \#22 Posted by: treenutter Posted at: 2016-12-22T15:24:18.079Z Reads: 127

```
Thx @PXSS for my part of it I was referring only to the connector, not the charger itself.
```

---
## \#23 Posted by: treenutter Posted at: 2016-12-22T15:36:47.419Z Reads: 122

```
Thx @Maxid I'm doing my best to understand the thread you shared and the related commentary. 

When I have to make choices about electronics, I think of it like this: would I bet my house on it? 

Would you bet your house on this idea that the voltage rating can be disregarded for charging ports as long as the amperage is not exceeding the port's threshold? I charge at 2A, so I think I'm good in this specific application.
```

---
## \#24 Posted by: Maxid Posted at: 2016-12-22T16:01:33.767Z Reads: 115

```
define betting my house on it. The question is what bad can happen - and the answer to that (for the low voltages we use) is: It will be just fine.
Just look at my Magsafe topic. Apple designed the plug for 20V - I use it with 41V now and it works just fine. 100kV will be a different story though.
```

---
## \#25 Posted by: jumbodrawn Posted at: 2016-12-23T08:05:11.225Z Reads: 111

```
Lots of people are commenting about the "size of the wires" being too small for the "large amount of current" being used in charging batteries. Also some about voltage. Let me clarify based on what I know:

**Yes, but it would be extremely slow**. Yes those small cables would melt with so much current, but you can charge a battery with any current. The only thing that must be at the rating of the battery is voltage. So yes, you can charge a battery with very low current but it would take a long time. The next problem is the low voltage. You would nee to step up 5v to x voltage based on what size lipo you have. The big problem with this is your current would be even lower. 

So to summarize:
You would need an on board circuit on the board that 
1) steps up voltage
2) controls the lipo chargeing

Hope that helps!
```

---
## \#26 Posted by: Maxid Posted at: 2016-12-23T08:12:09.777Z Reads: 108

```
Why do people keep talking about 5V - this thread was never about using the USB voltage to charge your board. It was meant to talk about the magnetic USB cable as charging cable - which should actually be fine at up to 4A and the voltage we use.
```

---
## \#27 Posted by: emstr Posted at: 2017-04-23T03:12:51.640Z Reads: 96

```
How about with usb-c? My macbook charger can deliver 60w through the port!
```

---
## \#28 Posted by: Shogu12 Posted at: 2017-04-23T07:44:43.597Z Reads: 92

```
Using these round magnet ports you can buy on alibaba
<img src="/uploads/db1493/original/3X/b/4/b4ff0c461a53964586398cf0d2b8696fe9fda259.jpg" width="690" height="451">
```

---
## \#29 Posted by: jackw Posted at: 2017-04-23T08:30:55.113Z Reads: 85

```
Anyone tried these? 
http://www.ebay.co.uk/itm/12-Volt-DC-Power-Connector-Magcode-Magnetic-Only-Live-When-Connected-/231148212430
```

---
## \#30 Posted by: Maxid Posted at: 2017-04-23T09:42:16.314Z Reads: 83

```
diameter 38mm? Seems massive
```

---
## \#31 Posted by: jackw Posted at: 2017-04-23T10:11:28.444Z Reads: 79

```
Yeah, I did think that.
```

---
## \#32 Posted by: Okami Posted at: 2017-04-23T12:43:28.148Z Reads: 78

```
But the current capability of this plug seems to be super good:

<img src="/uploads/db1493/original/3X/e/7/e71774b8a64629fef983f933619c6b812d5c6bed.jpg" width="289" height="500">

Though it does look a bit pricy even though it might be for high power applications.
```

---
## \#33 Posted by: hoeksame1 Posted at: 2018-07-01T08:49:14.657Z Reads: 36

```
Is it possible to put those magcode connector on 42v charger 2A??
```

---
