# HALL sensor wire extension cable

### Replies: 22 Views: 2791

## \#1 Posted by: ikjahaa Posted at: 2017-12-18T21:30:24.442Z Reads: 392

```
I've been searching the interwebs for HAL-senor wire extention cable.
I found [this](https://hobbyking.com/en_us/200mm-sensor-lead-with-mesh-guard.html?___store=en_us) on hobbyking, but its mate to male...

Anyone else got some ideas ?
```

---
## \#2 Posted by: mmaner Posted at: 2017-12-18T21:39:36.525Z Reads: 392

```
https://psychotiller.com/product/sensor-wire-adaptor

products/vesc-sensor-wires

https://miamielectricboards.com/shop-1/oesc-motor-adaptor
```

---
## \#3 Posted by: pat.speed Posted at: 2017-12-18T21:42:49.029Z Reads: 352

```
you could just cut the connector off then solder some extra wide on the solder the connector back on
```

---
## \#4 Posted by: Mikenopolis Posted at: 2017-12-18T21:43:11.464Z Reads: 342

```
beat me to it with those links.

@ikjahaa are you looking for an adapter or extension? is the sensor wire from your motor the JST 2.0mm that the vesc takes?

Personally I just cut the wires and solder on wires to extend mine so I don't get that connector bulk outside my enclosure
```

---
## \#5 Posted by: ikjahaa Posted at: 2017-12-18T21:49:16.005Z Reads: 330

```
It's a maytech motor. The connector is mini, and by that I mean really effing tiny lol...

I need a female connector got this, so I can easily detach my m9tor from my deck. Yeah... I have 6 wires running through my deck directly in the enclosure. I could solder these sensor wires to these cables but that's pretty permanent.

Also, I like that the conne for is so tiny..
```

---
## \#6 Posted by: rich Posted at: 2017-12-18T22:09:30.047Z Reads: 312

```
If your connector is male you could solder this cables for an extension. On the left side the small one you need (JST-ZH 1.5mm pitch) and on the right side the one which goes into vesc (JST-PH 2mm pitch). If you want I have some spares for cheap (EU). 

<img src="/uploads/db1493/original/3X/e/b/ebf00df478aa15e714fde1976a5c519e6e5cf0e2.jpg" width="690" height="388">
```

---
## \#7 Posted by: ikjahaa Posted at: 2017-12-19T10:03:25.120Z Reads: 280

```
But this wouldn't fit the male hal sensor connector either ?
```

---
## \#8 Posted by: b264 Posted at: 2017-12-19T10:26:51.399Z Reads: 276

```
EU:

http://www.faradaymotion.com/cables-connectors/49-vesc-motor-hall-sensor-cable-20-cm.html
```

---
## \#9 Posted by: rich Posted at: 2017-12-19T10:49:26.872Z Reads: 275

```
If your sensor wire connector looks like this you can use the cable @b264 linked, nice find!
It's the same cable of the first link of @mmaner 

<img src="/uploads/db1493/original/3X/8/f/8f832a00e9597a7ca155e11650c9ef282c8989ed.PNG" width="690" height="478">
```

---
## \#11 Posted by: Rotko Posted at: 2018-02-20T14:09:15.794Z Reads: 234

```
Hi guys, I'm trying to hide my sensor wires in deck and I need to extend them (about 20 cm / 8 inches). I've purchased on line a set of them + JST connectors and noticed the 6 wires are monofilar (composed by just one thread) whereas the single wires coming out from my motors are composed by 5-6 threads each. The overall diameter of the motor wires is bigger than the one of the extention. Is it a problem if I solder these two different types of cable? will the hall sensors works? If not, could you please advise which type of wire (AWG, composition) should I get?
```

---
## \#12 Posted by: rich Posted at: 2018-02-20T16:22:13.896Z Reads: 220

```
I don't see a problem with soldering different wires together for hall sensor. I've soldered several hall sensor extensions made of different cable diameters and up to 85cm in length and never had troubles. For the longest extension I used 22AWG (maybe overkill), but usually hall sensor wires are 24-28AWG.

Do it! :sunglasses:
```

---
## \#13 Posted by: moon Posted at: 2018-05-17T21:11:39.998Z Reads: 197

```
[quote="rich, post:6, topic:41370"]
JST-ZH 1.5mm pitch
[/quote]

Is this what should be used for a focbox?
```

---
## \#14 Posted by: rich Posted at: 2018-05-17T21:16:37.459Z Reads: 186

```
I never had a focbox but I guess it's the same as on every other vesc: **JST-PH 2mm pitch**

Only some motors have the small JST-ZH 1.5mm pitch connector but not the vesc.
```

---
## \#15 Posted by: venom121212 Posted at: 2018-12-28T16:20:14.765Z Reads: 126

```
I'm housing my unity and batteries further in my box so I need a loooooong jst zh 1.5mm male to female adapter. I already have psychos adapter to connect the end to the vesc. Anyone know of a supplier for long cables? I keep finding real small ones. I'll pay to have 2 made if I have to.

Trying to avoid connecting a bunch of [these](https://www.amazon.com/dp/B07FC9GP72/ref=cm_sw_r_cp_apa_i_s3KjCbSKJ7J25)
```

---
## \#16 Posted by: Andy87 Posted at: 2018-12-28T16:28:12.744Z Reads: 124

```
Maybe just to cut the adapter cable and solder some extension inbetween?
```

---
## \#17 Posted by: venom121212 Posted at: 2018-12-28T16:36:17.927Z Reads: 118

```
Man another good idea. I didn't want to cut motor or extension and that solves it well. Beers on me if we ever meet up.
```

---
## \#18 Posted by: Andy87 Posted at: 2018-12-28T16:38:19.280Z Reads: 118

```
Bookmarked 😜
```

---
## \#19 Posted by: Psmrman90 Posted at: 2019-01-02T22:24:25.886Z Reads: 114

```
I have 2 different motors, both sensored.  I need to extend them both but am not sure how to do it because one motor only has 5 wires in the sensor while the other has six.  Is the one motor faulty or are only 5 wires needed? If so, which 5 wires, so I can prioritize properly
```

---
## \#20 Posted by: mmaner Posted at: 2019-01-02T22:26:59.934Z Reads: 112

```
the 6th wire is likely motor temp, you dont need it.
```

---
## \#21 Posted by: huntercasillas Posted at: 2019-05-03T00:21:16.923Z Reads: 67

```
Anywhere else I can buy an extension wire like these? It appears they aren't being sold anymore. I just need to extend the hall sensors from my motors so they can plug into the unity. (I'm in the US)
```

---
## \#22 Posted by: Andy87 Posted at: 2019-05-03T00:54:46.128Z Reads: 64

```
https://www.electric-skateboard.builders/t/wts-sensor-wire-extension-cables/82598?u=andy87

😉
```

---
## \#23 Posted by: huntercasillas Posted at: 2019-05-03T01:09:21.850Z Reads: 59

```
Yes thank you! Messaged you about buying them!
```

---
