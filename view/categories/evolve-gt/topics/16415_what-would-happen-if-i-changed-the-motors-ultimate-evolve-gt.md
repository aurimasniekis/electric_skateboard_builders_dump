# What would happen if I changed the motors? {Ultimate Evolve GT}

### Replies: 26 Views: 3637

## \#1 Posted by: VikasG Posted at: 2017-01-21T00:34:16.085Z Reads: 297

```
I've started a few topics and discussed with a few people over at the Evolve forums but I need to know what would happen if I replaced the current 140Kv Evolve motors with [200Kv](http://www.banggood.com/Racerstar-5065-BRH5065-200KV-6-12S-Brushless-Motor-With-Gear-For-Balancing-Scooter-p-1117658.html?rmmds=search) ones using the same body and connectors. Would it work fine, break the ESC/motors, or have the motors run at a lower RPM? 

I've done some research along with gaining information after starting a few topics etc. and here is the final build that I wanted to do with the board:

[200Kv Motors: $100](http://www.banggood.com/Racerstar-5065-BRH5065-200KV-6-12S-Brushless-Motor-With-Gear-For-Balancing-Scooter-p-1117658.html?rmmds=search)
[Si3N4 Bearings for Motors: $50](http://www.ebay.com/itm/Full-Ceramic-608-Bearing-8-x-22-x-7-mm-Metric-full-Si3N4-Silicon-Nitride-/262724870130?hash=item3d2b9f5ff2:g:254AAOSwRgJXhQBw)
[38T Gears: $100](https://evolveskateboardsusa.com/collections/wheels/products/38t-gt-drive-gear-upgrade-kit?variant=20932040388)
[Abec 11 97mm Wheels: $100](https://evolveskateboardsusa.com/collections/wheels/products/abec-11-flywheels-97mm-75a?variant=32784427524)
[10s4p VTC6 Battery: $350](https://liionwholesale.com/collections/batteries/products/sony-vtc6-3000mah-15a-30a-battery-genuine-tested-flat-top-wholesale-discount?variant=28023263057)

Assuming everything works according to plan, the remote would still show speed correctly as it measures it based on RPM. There would be no noticeable voltage sag and the it will have nice speed boost to 32 mph (51 km/h). Basically a perfect electric skateboard.
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2017-01-21T00:42:15.670Z Reads: 285

```
Should work fine... your top speed will be less but you can compensate with gearing
```

---
## \#3 Posted by: VikasG Posted at: 2017-01-21T00:52:49.863Z Reads: 282

```
Wait, wouldn't top speed be more considering I'm going from 140Kv to 200Kv?
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2017-01-21T00:53:17.365Z Reads: 273

```
Lol yea sorry read that wrong mate u are correct

You would need to drop the gearing a little to keep the torque
```

---
## \#5 Posted by: VikasG Posted at: 2017-01-21T00:55:00.164Z Reads: 263

```
I was wondering how it would affect torque though. Would I lose torque and braking power because of it?
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2017-01-21T00:55:55.649Z Reads: 253

```
You will loose torque and that could be bad for the motors if your going off road
```

---
## \#7 Posted by: psychotiller Posted at: 2017-01-21T00:56:26.527Z Reads: 247

```
Getting to top speed or starting from a stop I think you will notice voltage sag because you are going to pull more amps in the beginning and everytime you accelerate in the powerband. More kv=Less torque, but more top end.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2017-01-21T00:56:43.338Z Reads: 241

```
There is a method to their madness I suppose
```

---
## \#9 Posted by: VikasG Posted at: 2017-01-21T01:00:58.994Z Reads: 233

```
I'm trying to mitigate that by using VTC6 cells - those offer a really high discharge rate. The biggest thing I was worried about was breaking - how would it affect it?
```

---
## \#10 Posted by: psychotiller Posted at: 2017-01-21T01:12:23.517Z Reads: 232

```
Honestly I don't think it will hurt your brakes that much.
```

---
## \#11 Posted by: saul Posted at: 2017-01-21T04:20:05.171Z Reads: 217

```
seems like a lot of mods for commercial board. it really comes down to how smart/dumb the esc is.
if its simple like a rc esc it should keep going fine with the changes. but if its configured for the stock motors or has top speed limiting you might just lose torque and efficiency for nothing....

since you're going with abecs I don't see why you wouldn't go full custom?
```

---
## \#12 Posted by: VikasG Posted at: 2017-01-21T04:54:33.153Z Reads: 203

```
I got the Evolve GT as a gift - sort of. I spent a lot of my money but my parents helped - fairly close in age to the youngest eSk8 builder on the forum.

My biggest reason is aesthetics. I really like how the integrated enclosure keeps the board slim and sleek looking. Also, going full custom means I have to start over and since anything else I spend my money on I have to earn 100% of, it really would just be too expensive. I'm not 100% sure how the ESC works - I'll have to contact the Evolve team.
```

---
## \#13 Posted by: NickTheDude Posted at: 2017-01-21T06:09:22.003Z Reads: 194

```
Yeah I would presume it all comes down to the ESC. If you were willing to pay extra I suppose you could get a couple VESCs though.
```

---
## \#14 Posted by: VikasG Posted at: 2017-01-21T06:51:47.990Z Reads: 191

```
Wouldn't that mean I can no longer use the existing Evolve remote? I really like the remote and the statistics it gives me (voltage, motor rpm, speed). I've gotten used to the sensitivity as well.
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2017-01-21T07:28:47.186Z Reads: 188

```
[quote="VikasG, post:14, topic:16415"]
Wouldn't that mean I can no longer use the existing Evolve remote?
[/quote]

In a nut shell


Yep
```

---
## \#16 Posted by: saul Posted at: 2017-01-28T03:15:23.825Z Reads: 173

```
even if it does work, the power meter may be off and i've heard it wasn't very reliable to begin with....

with the cost of those "upgrades" you are very close to the cost of a custom single drive that would smoke any evolve anyways! 

$100 for drive gears alone..they're just flywheels rights?
```

---
## \#17 Posted by: mwkeefer Posted at: 2017-09-18T00:41:07.525Z Reads: 123

```
I can give you an Arduino module that will fake out evolve's ESC UART and Sw connectors, that would let you keep the evolve controller and use with any pack - it would be stupid and reply that your battery was always at 90% SOC no matter its voltage or SOC (I could add smart interface but not freely)...

If your interested still let me know and I will open source the code I've got working now (I'm using to run a tiny lipo 10S pack with the evolve controller, less sag and range but also less weight by far).

Regards,
Mike
```

---
## \#18 Posted by: ThermalChild Posted at: 2018-06-11T20:38:47.115Z Reads: 74

```
Wait... you have something that can circumvent the evolve proprietary BMS? How has nobody heard of this?
```

---
## \#19 Posted by: ThermalChild Posted at: 2018-06-11T20:39:46.041Z Reads: 75

```
By all means send me that code dude. I'd love to be able to make a custom battery and have the crap one as a spare.
```

---
## \#20 Posted by: never4getf150forums Posted at: 2018-06-11T20:44:05.848Z Reads: 75

```
IDK, but i need this NOW!

please Mike :smiley:
```

---
## \#21 Posted by: Arzamenable Posted at: 2018-06-11T20:48:52.204Z Reads: 75

```
Just put in VESCs. You already have a solid, $2k mechanical foundation. What’s another $240 for some focboxs from enertion if still on sale?

![image|374x500](upload://m9rkttnoRk6ONVuqRigjql5OcL9.jpeg)![image|666x500](upload://4CFCBuWm6z00f70l5O0ETOF8zuH.jpeg)![image|374x500](upload://Ig72Ghw7hzFas2A24uPtXcfqBf.jpeg)
```

---
## \#22 Posted by: ThermalChild Posted at: 2018-06-11T20:57:07.511Z Reads: 72

```
But his method would allow you to keep the evolve remote.
```

---
## \#23 Posted by: Dazeto Posted at: 2018-06-12T22:53:47.618Z Reads: 67

```
hello, in case i dont get my refund on my gtx. im _very_ interested in doing this.
Did u have to replace the bms as well, and can it be done using the stock battery pack? thanks
```

---
## \#24 Posted by: Arzamenable Posted at: 2018-06-13T12:56:57.650Z Reads: 58

```
Only the motors and carbon fiber are stock. You could save the battery, but They will quickly become the bottle neck in a build as they age. 

The bms was taken out because we had several floating around and there was something goofy about the stock one. 

A 10s4p 30q battery fit easily.
```

---
## \#25 Posted by: Itsmedant Posted at: 2018-06-13T14:14:48.934Z Reads: 54

```
not sure if he is still doing them, but @longhairedboy was doing evolve battery upgrades!


https://longhairedboy.com/collections/all/products/evolve-bamboo-series-gt-battery-mod
```

---
## \#26 Posted by: G_FPV Posted at: 2020-02-06T21:36:30.213Z Reads: 7

```
Hi Mike

I would really appreciate this code and a little about the wire/pin mapping if that’s still good with you please.  This has been driving me crazy 😜 

Thanks
G
```

---
