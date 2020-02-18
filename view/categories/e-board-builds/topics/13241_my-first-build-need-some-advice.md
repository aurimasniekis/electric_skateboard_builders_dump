# My first Build &#124; Need some advice!

### Replies: 10 Views: 1189

## \#1 Posted by: Naxos Posted at: 2016-11-17T21:31:11.754Z Reads: 98

```
Hey guys,

I'm new to the electric skateboard business and I need some advice for my first build. My goal is to build a simple skateboard which I can drive to campus and back. Speed should be around 25km/h, range about 10km, I'm very tall, but only about 65kg. Terrain is very flat here.
I already looked up the last couple of days for the right parts. Now I ask you guys if you can tell me if all the parts doing well together or if there are some better alternatives. Thanks alot!!

**Deck:**
MOB Gold Label Cruiser 32". I know this isn't a real Longboard, but i chose this because it's small enough to take it on the campus.
http://mob-shop.de/epages/b2b_mob-shop_de.sf/en_GB/?ObjectPath=/Shops/b2b_mob-shop_de/Products/15151

**Trucks:**
Paris - Paris Truck V2 50 180mm. Just found them in a german online store.
http://www.blackout-shop.de/products/Longboards/Paris-Paris-Truck-V2-50-180.html?

**Wheels:**
ABEC11 - ABEC11 Flywheels 83 mm - 78 A. I think those are standard.
http://www.blackout-shop.de/products/ABEC11-ABEC11-Flywheels-83-mm-81-A.html?

**Bearings:**
INDEPENDENT ABEC 5. It's true that I need 8 bearings and 4 spacers in between right?
http://www.tactics.com/independent/genuine-parts-abec-5-skateboard-bearings

**Motor:**
Turnigy Aerodrive SK3 - 6354-260kv Brushless Outrunner Motor. I want a single Motor Setup. Is the power of the Motor enough? And what about the 260kv?
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html

**Battery:**
2x in series: Turnigy 5000mAh 3S 20C Lipo Pack. This should get me a 6S 5000mAh. Should be enough I think? But I don't think if 2x 4S would be better together with a 190kv Motor? Help me please.
https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack.html

**Controller:**
HobbyKing® ™HK-GT2B 3CH 2.4GHz Transmitter and Receiver w/Rechargable Li-ion Battery. Also Standard I think so.
https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html

**Pulley+Belt:**
12mm wide drive pulley kit from enertion.
http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-pulley-drive-hub-kit/

**VESC:**
new: vesc-x motor controller from enertion. Do I need this VESC or is a simple ESC from Hobbyking enough? Whats the benefit of the VESC?
http://www.enertionboards.com/electric-skateboard-parts/vesc-x-motor-controller/

**Motor Mount:**
Going to do this by myself.

Did I forget something? Whats your opinion on these parts? If you need more information just ask me. Thanks for your advice!
Greetings from Germany, Nax
```

---
## \#2 Posted by: NickTheDude Posted at: 2016-11-17T21:36:00.768Z Reads: 83

```
You can use a car ESC, but you will only really be able to find one that will support up to 6S. The VESC is also much more customizable. If you're planning on using the VESC, I would reccomend going with a higher voltage, 10S is perfect. With 10S, you're going to want a lower kV. 

A common, well tested setup is 10S with a 6374 190kV motor for a single motor setup, and for dual 2x 6355 190kV motors.

You can use this to calculate your top speed: http://calc.esk8.it/
```

---
## \#3 Posted by: Naxos Posted at: 2016-11-17T21:50:22.413Z Reads: 79

```
Hey Nick,

thanks for you quick response! If I'm going with the VESC, do I need the 10S? I think the smaller Battery and Motor just are alright for me and my speed/range I want?
But if I'm going with the 10S, do I buy 2x5S or 1x10S? Maybe you got a link?

Thanks for the Calculator. It says around 30km/h weighted with the 6S which is more then enough for me.
```

---
## \#4 Posted by: NickTheDude Posted at: 2016-11-17T22:02:02.178Z Reads: 75

```
https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-20c.html

Those should be good, a single 10S battery would be a lot thicker so going with 2 5S packs would let you make your enclosure much lower profile. And no you don't need 10S for the VESC, but the amp limit on the VESC is pretty low and having higher voltage helps with that.

With a 6S setup and 260kV you're going to be losing out on a lot of torque, so if hill climbing is a priority that would be an issue.
```

---
## \#5 Posted by: Naxos Posted at: 2016-11-17T22:58:02.397Z Reads: 63

```
Okay now considering the VESC+10S LiPo.

As a Charger I thought of the IMAX B6 from HK (https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html). This can handle up to 6 Cells, how to charge the Packs when they are connected in series? Do I have to disconnect them every time I charge them and then charge separately? Are there any other options?
```

---
## \#6 Posted by: Smorto Posted at: 2016-11-17T23:20:45.064Z Reads: 54

```
Hi! Good luck with your build. The only thing I see quickly is that that motor has a 6mm shaft which won't fit the enertion pulley. You are going to want to find something with an 8mm shaft such as a 190kv motor like @NickTheDude mentioned.
```

---
## \#7 Posted by: Naxos Posted at: 2016-11-17T23:36:59.855Z Reads: 54

```
Hey Smorto thanks!

Thanks for the advice with the shaft, just saw i posted the wrong link of the 260kv motor. The 260kv got the 8mm shaft so it should be alright.
```

---
## \#8 Posted by: Smorto Posted at: 2016-11-17T23:50:21.289Z Reads: 50

```
Ok, Good Luck!
```

---
## \#9 Posted by: ACIN Posted at: 2016-11-18T02:06:29.311Z Reads: 51

```
Hey, also a 65kg tall noob from germany here.
I'll probably go 10S dual 190kv dual Vesc with a 15/32 Gearing on 83mm (/90?) wheels (My budget quite a bit higher I guess, I just want big performance and reliability).

One thing I do know: Your trucks cost 33€ **each**, you'll probably get them cheaper on ebay as a set of 2.
```

---
## \#10 Posted by: Hendrik.W Posted at: 2017-08-02T21:58:21.325Z Reads: 23

```
Hey, i am also from germany and looking for wheels. 90mm wheels would be perfectly.
Please help me :D
```

---
