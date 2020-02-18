# Vesc cutoff while accelerating

### Replies: 51 Views: 2970

## \#1 Posted by: Ishayc Posted at: 2017-09-10T19:57:27.212Z Reads: 230

```
Hi,

It's not my first vesc so I don't know what I'm doing wrong but while accelerating the vesc cutsoff.
Gear:
6s 5000mah lipo 25c, 245kv motor.
Vesc settings:
BLDC
Motor max: 85a
Motor min: -60a
Battery max: 30a
Maximum input voltage: 57v
Minimum input voltage: 8v
Cutoff voltage is very low just for the try.

I tried to change every possible settings I could think of but it acts the same, it even cutsoff while braking hard.

I looked for errors in the terminal but there are non.

Help please.

Ishay
```

---
## \#2 Posted by: Jammeslu Posted at: 2017-09-10T20:33:22.119Z Reads: 216

```
not an expert but motor max and min looks to high for sure
```

---
## \#3 Posted by: darkkevind Posted at: 2017-09-10T20:36:14.660Z Reads: 211

```
That depends on his motor ratings... Unusual to get a single motor rated above 60A though...
```

---
## \#4 Posted by: Jammeslu Posted at: 2017-09-10T20:39:22.818Z Reads: 208

```
yeah a 245 kv one sk3? maybe but anyway
```

---
## \#5 Posted by: ninja Posted at: 2017-09-10T20:39:59.482Z Reads: 206

```
If its sk3 245kv than 70a is max. rated for that motor.

60a mot min is ok. It can be even more like mot max.

 I have some modes were max is 70a, min is -70a

Also max 50a min -70a. But im using @Ackmaniac tool and firmware. So there is no problem to set min  even higher than max.
```

---
## \#6 Posted by: darkkevind Posted at: 2017-09-10T20:40:36.519Z Reads: 190

```
Actually HK SK3 6374 is rated at 80A so my mistake...
```

---
## \#7 Posted by: ninja Posted at: 2017-09-10T20:46:09.201Z Reads: 189

```
<img src="/uploads/db1493/original/3X/5/5/556f11bb4ef49c908795539bdd656d36db73a930.png" width="281" height="500">

But on their page says 70a.
```

---
## \#8 Posted by: darkkevind Posted at: 2017-09-10T20:47:10.240Z Reads: 184

```
My bad, I was looking at 192kv! 

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?gclid=Cj0KCQjwxdPNBRDmARIsAAw-TUl3n_4-GcW2NZ_5K1XS847x1N6UR2Dz095eAHJSLeaPcgji1w_yXc8aAmc_EALw_wcB&gclsrc=aw.ds&___store=en_us
```

---
## \#9 Posted by: ninja Posted at: 2017-09-10T20:47:41.061Z Reads: 182

```
That one is real beast😉
```

---
## \#10 Posted by: Ishayc Posted at: 2017-09-10T20:50:12.979Z Reads: 179

```
Well mine is the Bigfoot 160 and it is rated as 75a.
Any idea what I should change to make it work?
Maybe a faulty DRV or MOSFET?
```

---
## \#11 Posted by: Ishayc Posted at: 2017-09-10T20:50:49.706Z Reads: 171

```
I'm using Ackmaniac's tool as well
```

---
## \#12 Posted by: darkkevind Posted at: 2017-09-10T20:51:12.560Z Reads: 170

```
Well definitely not 85A as you have it. You're pushing more A to the motor than it can handle...
```

---
## \#13 Posted by: Ishayc Posted at: 2017-09-10T20:52:57.388Z Reads: 169

```
yup, changed it to 70a and same behavior
```

---
## \#14 Posted by: scepterr Posted at: 2017-09-10T21:04:58.112Z Reads: 166

```
What are your vesc temps like
```

---
## \#15 Posted by: Ishayc Posted at: 2017-09-10T21:13:29.047Z Reads: 168

```
@scepterr Seems hot when I touch the hit sink.
Another thing I've noticed is soon as I squeeze the throttle all the way the vesc stops and there's a weird sound from the motor.
If I don't push it all the way I can go up the hill.
Tried to recalibrate the rc, didn't work. Tried to replace the motor, didn't work.
It seems something with the remote or with the current peak. 
It does not matter what is the battery max it keeps on happening.
```

---
## \#16 Posted by: Esk8HubsUS Posted at: 2017-09-10T21:39:38.292Z Reads: 159

```
If you don’t see the VESc throwing a fault in the logs then it could be your battery.  If your trying to pull more amps than the battery can supply (or BMS is configured to allow) than the BMS could be temporarily cutting out (by design).  What battery/bms do you have (what’s the max discharge ?)
```

---
## \#17 Posted by: jmasta Posted at: 2017-09-10T21:48:11.776Z Reads: 155

```
You can program a higher Motor Max than for what your motor is rated.  The 'true' amperage is defined by Battery Max


@Ishayc What are your battery cuttoff start/end values?
```

---
## \#18 Posted by: i2oadsweepei2 Posted at: 2017-09-10T21:52:11.826Z Reads: 156

```
[quote="Ishayc, post:15, topic:32813"]
Another thing I've noticed is soon as I squeeze the throttle all the way the vesc stops and there's a weird sound from the motor.
[/quote]


Does it sound like this?
https://youtu.be/eNSR-8s5K_Y
```

---
## \#19 Posted by: Ishayc Posted at: 2017-09-10T21:57:24.199Z Reads: 153

```
@Esk8HubsUS @jmasta I don't use bms and this battery is working fine on a different board with the same setup but the vesc. 
I put the start and end cutoff to 10v and 8v just to make sure it's not any battery sag issue.  

@i2oadsweepei2 nope, totally different. The motor is not braking and the noise is different.
```

---
## \#20 Posted by: Nix Posted at: 2017-09-10T23:33:18.298Z Reads: 146

```
So when you set the 40 amp battery max the vesc can only take 50a continuous, but then when you set the motor max it's based on the max amps of the motor not the max based on home many amps continuous the vesc can take? Right? (Sorry trying to learn)
```

---
## \#21 Posted by: Scoo_B_SK8 Posted at: 2017-09-11T03:36:59.186Z Reads: 139

```
would the "25C" rating on battery have anything to do with it when trying to grab 70A?
try and lower motor max & bat max all the way down to something like 30A and see if get same result.
```

---
## \#22 Posted by: Ishayc Posted at: 2017-09-11T05:40:11.819Z Reads: 135

```
@Nix You are correct.
@Scoo_B_SK8 the 25c along with the capacity gives you how many amps you can draw from it. In my case it will be 25*5 so 125a.
```

---
## \#23 Posted by: Cobber Posted at: 2017-09-11T05:49:05.325Z Reads: 134

```
[quote="Ishayc, post:22, topic:32813"]
In my case it will be 25*5 so 125a.
[/quote]

while technically that is 100% correct
manufacturers are a little generous with their _C_ ratings
having some headroom is always a good idea
```

---
## \#24 Posted by: Ishayc Posted at: 2017-09-11T06:01:42.780Z Reads: 127

```
Yup, I'm aware of that but I still have enough room so the battery is not the issue. Any other suggestions maybe?
```

---
## \#25 Posted by: jmasta Posted at: 2017-09-11T06:11:22.632Z Reads: 126

```
Are you using the Android app to log data while riding?  Your cutouts during acceleration may be a DRV8302 fault.  My VESC did something similar. It works fine otherwise, but sometimes cuts out on hard accelerations. Then resets a few seconds later and continues working...
```

---
## \#26 Posted by: Ishayc Posted at: 2017-09-11T06:17:02.998Z Reads: 121

```
No I don't have Bluetooth module. 
But it seems to acts as you say. 
Did you see any drv faults in the terminal?
```

---
## \#27 Posted by: jmasta Posted at: 2017-09-11T06:22:30.284Z Reads: 122

```
No I can't recreate it on the bench.  It seems that in many cases a DRV error is fatal.  However mine just resets and keeps going.  As some people in my thread commented, I believe the DRV chip is failing

http://www.electric-skateboard.builders/t/frequent-drv8302-faults-help-me-troubleshoot-with-telemetry/28332

Sounds like yours is doing the same thing. I recommend buying a BT module to be sure. Who manufactured your VESC?
```

---
## \#28 Posted by: darkkevind Posted at: 2017-09-11T08:50:56.159Z Reads: 122

```
It seems like I'm having the exact same issue. Hard acceleration or reasonable acceleration on a slight incline and it cuts out but just resets and comes back a couple of seconds later. Sometimes on braking too.

Where would one get one of these bluetooth modules please?

I have a usb extension socket on the side of my enclosure, it is possible to plug in my phone via usb while riding to record the data?
```

---
## \#29 Posted by: Ishayc Posted at: 2017-09-11T09:05:15.576Z Reads: 119

```
Don't turn off your vesc after the ride, connect it to pc and search for the faults/errors in the terminal
Tab. 
I had no faults so it makes it even harder to identify the problem.
```

---
## \#30 Posted by: jujet Posted at: 2017-09-11T10:30:09.321Z Reads: 117

```
This happens to me as well. 

If I accelerate really fast, I get a weird noise from my motor and the control loses connections for a few seconds, just to reconnect again. 

It doesn't happen if I don't accelerate suddenly. 

10s Li Ion, BMS and 190 KV motor
```

---
## \#31 Posted by: darkkevind Posted at: 2017-09-11T11:00:01.125Z Reads: 113

```
That's no good because it's actually re-booting, so all errors get cleared.
```

---
## \#32 Posted by: darkkevind Posted at: 2017-09-11T11:00:35.389Z Reads: 110

```
I don't get any noise at all, just literally the VESC cuts out and re-boots.
```

---
## \#33 Posted by: Ishayc Posted at: 2017-09-11T11:46:44.686Z Reads: 106

```
Exactly what I'm having.
Faulty drv then?
```

---
## \#34 Posted by: darkkevind Posted at: 2017-09-11T12:30:56.137Z Reads: 104

```
What causes a faulty DRV then?
```

---
## \#35 Posted by: Ishayc Posted at: 2017-09-11T12:53:04.806Z Reads: 103

```
A bunch of stuff can cause drv to fry.
Not sure what went wrong in my case.
```

---
## \#36 Posted by: jmasta Posted at: 2017-09-11T17:50:45.566Z Reads: 99

```
I think mine may have been a result of buggy firmware provided by the manufacturer.  Had the current ramp step bug, and I was unknowingly running a value maxed out at 50, instead of the default 0.04
```

---
## \#37 Posted by: trampa Posted at: 2017-09-11T19:00:44.129Z Reads: 92

```
Have you tried the new VESC-Tool with 3.28FW? www.vesc-project.com


Frank
```

---
## \#38 Posted by: Ishayc Posted at: 2017-09-11T22:08:27.488Z Reads: 92

```
@jmasta I was aware of this bug so I kept it at 0.04.  
@trampa didn't know there's a new software but I'll give it a try, Thanks!
```

---
## \#39 Posted by: trampa Posted at: 2017-09-11T22:13:18.065Z Reads: 92

```
Do so! and if you like it invite Benjamin on a blonde cool beer. Frank
```

---
## \#40 Posted by: darkkevind Posted at: 2017-09-11T22:16:00.761Z Reads: 98

```
Can we update 4.12 hardware with 3.28FW?

What's the changelog? Any new decent features or only for VESC 6?
```

---
## \#41 Posted by: MontPierre Posted at: 2017-09-11T23:33:10.419Z Reads: 95

```
[quote="darkkevind, post:28, topic:32813"]
Where would one get one of these bluetooth modules please?
[/quote]

Im using this one - and it has iPhone app but you have to pay for module - approx £27/$34 delivered to UK - that's him much I paid. Plug and play :) 

http://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483/447 

If you have android @Ackmaniac has a free app- and you can get one of clone Bluetooth modules to go with it. 


Btw - what step down converter are you using to have USB out?
```

---
## \#42 Posted by: MontPierre Posted at: 2017-09-11T23:36:08.358Z Reads: 96

```
[quote="darkkevind, post:40, topic:32813, full:true"]
Can we update 4.12 hardware with 3.28FW?

What's the changelog? Any new decent features or only for VESC 6?
[/quote]

It's all over here - lengthy discussion on new firmware and vesc tool ;) 


http://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268?u=montpierre
```

---
## \#43 Posted by: darkkevind Posted at: 2017-09-12T08:01:42.960Z Reads: 87

```
Thanks for the info mate. I'm on android so where would I get a clone module for ack's software please? (I could search but I'm just being lazy! :/ )

I don't have usb power out, I just have a short extension lead from my VESC to the edge of the enclosure, so I can plug in the VESC without taking the enclosure off.

I am thinking about adding USB charging capabilities. If I did I'd use this module...

http://www.ebay.co.uk/itm/352155418648
```

---
## \#44 Posted by: MontPierre Posted at: 2017-09-12T08:32:12.276Z Reads: 80

```
There you go you lazy ass! :stuck_out_tongue_winking_eye:


http://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888?u=montpierre

He has linked the module in his post, from AliExpress. Order it now to have it before xmass haha ;)

I wouldn't get any other module as compatibility is a big issue, a lot of guys have problems getting them to work - unless you'll find exactly same model on eBay uk .... might be hard, pictures are usually stolen from listing to listing and module itself might not look like pictured one.

Thanks for the link with step down module!

I found even cheaper one on AliExpress 

Look what I found on AliExpress
http://s.aliexpress.com/nIB3YFJR

Or this one - quicker shipping from eBay 

https://www.ebay.co.uk/itm/222244391709 

I'll just have to get micro USB to female USB 2 extension or solder female USB onto it ;) Winter project :D 

Edit :slight_smile:

Found one with female USB already soldered on from Ireland ;) double the price at £4 but easier. Not sure how well USB 2 will hold to the enclosure...

https://www.ebay.co.uk/itm/322543582068 


Wait... I don't have any space left in enclosure :disappointed:
```

---
## \#45 Posted by: darkkevind Posted at: 2017-09-12T09:12:06.614Z Reads: 77

```
[quote="MontPierre, post:44, topic:32813"]
He has linked the module in his post, from AliExpress. Order it now to have it before xmass haha :wink:
[/quote]

lol thanks! Although that particular one is no longer available. I found what looks to be the exact same module on Amazon though and I ordered with Prime, so it'll be here tomorrow ;)

https://www.amazon.co.uk/LANMU-Bluetooth-Wireless-Adapter-Arduino/dp/B01H2ZHXF0/ref=sr_1_2

I'm sure you could get those modules cheaper, I wasn't sure how many cells you had in series so I looked for one that would cover all scenarios. I'll be getting one for 8s which you can find a bit cheaper :thumbsup:

 Haha! No space! :( That's going to be my problem soon too!!
```

---
## \#46 Posted by: jujet Posted at: 2017-09-12T09:13:24.460Z Reads: 74

```
Dunno, I switched to FOC recently and it's so much better. 

Not sure if it's a faulty DRV, as the VESC is working......
```

---
## \#47 Posted by: MontPierre Posted at: 2017-09-12T09:15:27.351Z Reads: 75

```
Just search @Ackmaniac thread I linked above for new link to the module - I think someone else also said it was no longer available and he linked new one - I might be wrong. You don't want to have this problem:

 http://www.electric-skateboard.builders/t/bluetooth-module-with-ackmaniacs-app/32220?u=montpierre
```

---
## \#48 Posted by: wafflejock Posted at: 2017-09-12T18:50:56.212Z Reads: 74

```
Not sure if it's relevant to the problem everyone here is having but I've had drop offs that happen because of power coming from the VESC for the receiver would dip when the voltage is getting relatively low on my battery (when it gets down from 42V fully charged to around 38V).  With mine I have a custom receiver and adding a capacitor to the ground/vin on the custom recevier and on its radio (since they are separate pcbs in my case) gets rid of the drop outs entirely.  I would take advice of others here to reproduce the problem then check for faults but assuming nothing comes through there would look at either adding capacitors to the power input on the receiver so it can deal with small dips in power from the VESC voltage regulator or try repositioning the receiver to see if it has any effect (further from the VESC).  Might be red herrings but some things to try if you're out of ideas.
```

---
## \#49 Posted by: Ishayc Posted at: 2017-09-13T11:51:55.415Z Reads: 70

```
Hi!

Tried the new FW but it does not work.
I can't get the remote to connect and I tried 2 remotes.. any idea why? 

Ishay
```

---
## \#50 Posted by: Z4MSupreme Posted at: 2019-04-12T16:00:25.489Z Reads: 24

```
so did all your issues go away using FOC?
```

---
## \#51 Posted by: jujet Posted at: 2019-04-15T07:12:28.002Z Reads: 24

```
Pretty much, yes
```

---
