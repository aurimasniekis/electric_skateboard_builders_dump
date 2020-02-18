# First onewheel build &#124; Need advice!

### Replies: 21 Views: 714

## \#1 Posted by: FireGhost Posted at: 2019-09-04T10:04:16.981Z Reads: 131

```
Hi guys,

I want to build my own Onewheel. So, it's been maybe a week that I'm reading a lot of stuff and, now, I've started to check the definitive components needed for the build.

Can you make a review of the chosen parts please ? If you know some cheaper parts, let me know too :)

## Wheel
https://www.aliexpress.com/item/32823573279.html

I was thinking about the 600w 48v version of this wheel.

But what are actually the differences between the 48v and 60v ? If I take the 60v and give it only 48v, would it be more reliable ?

## ESC
https://www.ebmakers.com/products/x-vesc4

This ESC is on sale right now and looks good !

## Battery (2 in serie)
https://hobbyking.com/en_us/turnigy-5000mah-6s-20c-lipo-pack-w-xt-90.html

Again, it's on sale and should be good too. I would take 2 of them in serie, so it would be a 12s1p.
And if it works well, I will buy another pair of this battery to use in parallel ? Is it a good idea ?

## Other
### Anti-spark switch
https://www.ebmakers.com/products/anti-spark-switch
### BMS
https://www.aliexpress.com/item/33008439523.html
The *13S 60A Separate Port* version. But I'm really not sure about this BMS... Some advice maybe ?
### Charger
https://hobbyking.com/en_us/turnigy-accucell-6-50w-6a-balancer-charger-lihv-capable.html

About the charger, if I'm plugin a BMS with my batteries, what kind of charger should I use ? I didn't find the information...

Last parts will be the Arduino and the gyroscope. But this will be another story (and easier to find !)

Thank you for reading to this! Let me know if something seems wrong or if I should change something, because it's my first build and it's pretty obscure for me for now...

Thanks ! :)
```

---
## \#2 Posted by: Grozniy Posted at: 2019-09-04T10:50:59.893Z Reads: 114

```
Ditch the anti spark, get AS150.
Lipo charger already balances the cells. If using BMS, you just need a brick charger.
Those lipos need to be at least 40C.
For BMS search bestech & supower.
```

---
## \#3 Posted by: Oeliboeb Posted at: 2019-09-04T12:21:19.241Z Reads: 111

```
Nice project! I've been looking into diy onewheels too as they look soooo cool. What's the gyro you will be using? 
Also I don't know too much about those hub motors, but I would imagine thoe things generate high voltage spikes. Maybe it would be better to use two 5s lipos in series and get the 48v version of the wheel to save the ESC a bit. 
Keep us posted!
```

---
## \#4 Posted by: FireGhost Posted at: 2019-09-04T12:22:06.524Z Reads: 103

```
Hey thanks for your reply :slight_smile:

I was thinking using the anti-park as the main on/off switch for the board. Does it make sense or can I add a button directly on the VESC's board ? (Couldn't find the information about an on/off button on the VESC)

For the BMS, I found this one from SuPower: https://www.aliexpress.com/item/32800557987.html
Looks like the one for my battery.

But then I would need a brick charger. What voltage/amp should I look for ? One that has more voltage than my battery ?

And about the C value, I chose a 5Ah 20C because the wheel would make 600W, so it would need, at maximum, (600w / 44.4v = ) 12.5amp and my battery would be able to produce 100amp. Plenty enough no ?

Thanks again for the time you spent for me !

I will keep posting here during the whole project :D
```

---
## \#5 Posted by: Toleg Posted at: 2019-09-04T12:31:18.352Z Reads: 93

```
Most of the work for a onewheel will be the software part ... good luck !
```

---
## \#6 Posted by: Grozniy Posted at: 2019-09-04T12:58:40.118Z Reads: 89

```
Anti spark switch will fail. AS150 will work as on/off button & anti spark.
With 4.12 hardware y should only use 10S.
With 6.6 hardware you can use 12S.
C rating is at least overrated twice. So that's why 40C minimum.
```

---
## \#7 Posted by: Grozniy Posted at: 2019-09-04T13:26:13.596Z Reads: 86

```
10s charger
https://www.ownboard.net/products/ownboard-electric-skateboard-charger-41-5v-3a
```

---
## \#8 Posted by: Surfer Posted at: 2019-09-04T18:31:37.415Z Reads: 71

```
the antispark he is willing to use has a precharge in positive, should be good.
```

---
## \#9 Posted by: FireGhost Posted at: 2019-09-04T22:04:29.283Z Reads: 70

```
Alright, thank you guys for your help!

I found a 5Ah 40C LiPo battery, so I'll take two of it and put them in serie :slight_smile:

I still have my first question tho. If I keep the same parts but take the 60v version of the wheel (instead of the 48v), would it be simply more reliable in time (more robust) ? Or would I be more slower and/or with less strength ?

And second question, why would the anti-spark button fail ? If it's the case, I would still need an on/off button... Do you have any recommendation (for an actual button, not electrical plugs :slight_smile:)  ?

Here a very quick and dirty sketch with the actual components:
![elec-schema-onewheel|492x499,75%](upload://1TYUCkz18hXgDvTBjL8aJmGwQpa.png)
```

---
## \#10 Posted by: Grozniy Posted at: 2019-09-04T23:13:49.250Z Reads: 60

```
High discharge bestech BMS usually have electronic switch built in, check on search, I don't remember which one exactly
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-09-05T04:41:18.520Z Reads: 61

```
He's using 12s not 10s
```

---
## \#12 Posted by: Fosterqc Posted at: 2019-09-06T09:19:16.554Z Reads: 59

```
Surprised nobody has taken to time to let you know the 48v and 60v versions are identical it's the phub188 either way. That is from the Onewheel build guide thread.
https://www.electric-skateboard.builders/t/onewheel-build-guide/80129/76

What shipping do you get quoted? Mine is $47 and others is under $30. I contacted Pei Pei scooter, they said only that rate is available but could deliver two for $290. (Two Onewheels>Onewheel)
```

---
## \#13 Posted by: Byngham Posted at: 2019-09-06T20:38:21.438Z Reads: 51

```
The thing I'm seeing in your plan is that you don't have anything included that will have a gyro in it, and I'm not sure where you'll be running the software to manage acceleration/deceleration.

There have been a number of folks that are taking the approach of running the software on an Arduino, which would have a gyro connected to it.  The Arduino would read the gyro, make appropriate calculations of how much you're leaning forward (accelerate) or leaning back (decelerate), and send the appropriate signal to the VESC.  This would work with the VESC 4.12 you have.

The other way I'm seeing folks going is to use a VESC 6+, which has the gyro/accelerometer built in, and building the software to run on the VESC 6+ itself (which it sounds like there's a few folks already working on.)  I need to decide which path makes most sense, but I'm leaning towards the VESC 6+.

There is some really good reading about how folks are approaching this on this thread:  https://www.electric-skateboard.builders/t/onewheel-build-guide/80129/195
```

---
## \#14 Posted by: Surfer Posted at: 2019-09-06T20:57:42.912Z Reads: 49

```
Thanks for your input, I'm connecting it directly without any Arduino in the middle, as I read other forums/post is more convenient to have the gyro as close to the vesc as possible, even better if it's built-in, noise related.
Anyway the wiring was correct, now is working good, the problem was I didn't flash the right firmware to the vesc.
```

---
## \#15 Posted by: Khurtana Posted at: 2019-09-08T00:21:52.092Z Reads: 49

```
So you just added an IMU to a VESC?  Which VESC did you use?
```

---
## \#16 Posted by: Khurtana Posted at: 2019-09-08T00:33:46.403Z Reads: 47

```
I’m torn between the 36v and 48v/60v Variants.  At 12S, I’m pretty sure 48v/60v is the best choice, right?  As far as I understand it, if you feed 60v instead of 48v you get a faster wheel.  In terms of what to select, I think I’m superstitious enough to go for 48v, 600w.  Am I on the right track?
```

---
## \#17 Posted by: Fosterqc Posted at: 2019-09-08T04:59:23.514Z Reads: 49

```
@Khurtana 

[quote="Fosterqc, post:12, topic:101339"]
Surprised nobody has taken to time to let you know the 48v and 60v versions are identical
[/quote]
Fairly certain the 36v is the same deal, just advertising voltages you might want to use with it.
same price too, dead giveaway.
 
I'm gonna be ordering two Phub188's and some VESC 6 plus and some 21700s 
should be cool might take me a couple months to finish though.
```

---
## \#18 Posted by: Khurtana Posted at: 2019-09-08T08:49:37.631Z Reads: 41

```
I’m actually pretty sure they are ALL the same motor.
```

---
## \#19 Posted by: Byngham Posted at: 2019-09-09T19:59:36.595Z Reads: 33

```
[quote="Fosterqc, post:17, topic:101339"]
Phub188
[/quote]

I've gotten my Phub 188 motor in, and have a question.  The power lines are straight forward enough, but the wires that I'm assuming are for sensors are in a connector that doesn't match anything I'm seeing on any controllers, and I can't find a wiring schematic for the motor itself to tell me what those wires are for.  

Does anyone know how to use those wires correctly?

Thanks.
```

---
## \#20 Posted by: Surfer Posted at: 2019-09-09T21:39:24.179Z Reads: 31

```
Vesc autodetect the position for hall sensors, doesn't matter how you connected them, just 2 power lines 3 sensors and 1 if you have thermistor.
The connector is JST, sorry I don't remember the pich.
```

---
## \#21 Posted by: Byngham Posted at: 2019-09-13T12:48:48.814Z Reads: 28

```
Looking at the Trampaboards.com website for the documentation on the Vesc 6plus and the connectors they sell on their site, it looks like the sensor connection are a JST PH 6-pin.
```

---
