# 40% climbs offroad - doable?

### Replies: 40 Views: 2255

## \#1 Posted by: telnoi Posted at: 2017-10-17T08:50:22.193Z Reads: 267

```
I recently completed my build (mountain board, dual Turnigy Sk3 149KV, dual VESC ESK8 Controller 1.1) and will mainly be using it to travel to work. About 80% offroad with hills ranging in between 16-40% incline, where 40 is the exception. Total distance, 9.6 km.

I am contemplating if it makes sense to upgrade from a li-ion pack to lipo (10s2p 5000mah 60C or 12s2p 5000mah 60c). Currently, I have a 10S5P LG rated at a max. discharge of 50A and whilst the board manages to slowly climb 30 degree hills, anything above is too much..especially offroad. In addition, braking is limited at 12A max combined. Not enough to completely stop me with hills steeper than 35 degree.

What can realistically be expected when upgrading to the above mentioned Lipos? I haven't seen any vids of mountain boards going up hill on 40 degree slopes. 
Is 12S safe, or would it be better/safer to stick to 10S? I'm uncertain if additional caps have to be installed for 12S, nor if stressing the components to the max voltage rating would be wise when taxing the controllers with such hills.

Any info welcome.
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-17T08:59:26.233Z Reads: 267

```
Is battery current your limiting factor climbing hills? 
Are you currently hitting 50A?

What's your gearing and wheel size
```

---
## \#3 Posted by: b264 Posted at: 2017-10-17T09:07:18.944Z Reads: 260

```
40° incline?!?  Something like [this](http://geekologie.com/assets_c/2015/01/mini-ripsaw-thumb-640x418-29587.jpg) might work
:wink:
```

---
## \#4 Posted by: Cobber Posted at: 2017-10-17T09:21:18.313Z Reads: 255

```
40% is serious... gear down bro like scepy is eluding to...
```

---
## \#5 Posted by: telnoi Posted at: 2017-10-17T09:22:29.188Z Reads: 253

```
Have to research how to check the vesc log, but since others have mentioned that they already notice slow downs with 100A packs as opposed to 300A packs, I have no doubt that I am hitting the 50A limit (it's just 25 per motor).

Gear ratio is 4.8:1
(15 for motor pulley, 72 for wheels, 8'' tires).
```

---
## \#6 Posted by: telnoi Posted at: 2017-10-17T09:26:30.067Z Reads: 239

```
haha, almost sounds like maybe I am expecting too much? Luckily, that's just one 15 meter slope and one near my house (250 meters that I currently walk).
```

---
## \#7 Posted by: jmasta Posted at: 2017-10-17T09:40:33.970Z Reads: 232

```
Do you mean 40% grade or 40° incline?

40% grade = 22° incline (which is steep)
40° incline = 84% grade (which is insane)
```

---
## \#8 Posted by: SilentException Posted at: 2017-10-17T09:43:29.638Z Reads: 223

```
I believe many don't even know the difference. Even the vendors in the specs often have no idea whether it is grade or incline. "Reviewers" mix it up even more. For 40 incline you need mountain climbing gear and not esk8 :)
```

---
## \#9 Posted by: scepterr Posted at: 2017-10-17T09:51:33.994Z Reads: 217

```
Deck mounted grappling hook gun with motor doubling as winch...🤣
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-10-17T09:58:18.371Z Reads: 216

```
Please post your Motor and Battery Settings via Screenshot or tell me at least your motor max value. Because that defines how much torque will be available.

But all in all you have the wrong battery if it only can provide 50A. Which cells do you use exactly?
```

---
## \#11 Posted by: telnoi Posted at: 2017-10-17T10:13:51.498Z Reads: 208

```
That's grade, sorry.
```

---
## \#12 Posted by: telnoi Posted at: 2017-10-17T10:14:54.095Z Reads: 207

```
motor max is currently set at -70/70 and battery max to 25 for each VESC with braking at -6.´
The pack was prebuilt/using LG MJ1.
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-10-17T10:22:28.573Z Reads: 205

```
80 should be fine. Even 90 should be doable as long as you get no Overcurrent errors. And if you still can touch the motors with your hand for at least a couple of seconds the motor temp is also no problem. Weakest link is definitely the battery.
```

---
## \#14 Posted by: telnoi Posted at: 2017-10-17T10:29:10.166Z Reads: 203

```
The max loading as indicated by HK is 70A. The motors are currently luke warm though after my ride.
Safe to go up to 80/90 despite of the specs?
```

---
## \#15 Posted by: Ackmaniac Posted at: 2017-10-17T10:35:56.544Z Reads: 191

```
Well i could be wrong but i think the 70A is meant that this is the maximum you can use continuous because RC-Airplanes mostly run at full power all time.
So if the temperature don't get too hot it should be fine. But maybe you can rip the magnets out with too high amps. I just run my 6355 all the time with 80A and have no problems.
Long story short i can only speak about my experiences and i would raise the amps to 100A if i would need it.
On the other side @Nowind ripped out the magnets of the bell. So maybe a bad made motor or he reached the limit.
```

---
## \#16 Posted by: telnoi Posted at: 2017-10-17T10:47:34.930Z Reads: 184

```
slipping magnets typically happen when low temp glue is used (allot cheaper) and no engraved ring is in place on the bell (experience from multi-rotors). Not something I want at those speeds :stuck_out_tongue:

Anyway, based on all the experience posted here and elsewhere, the battery is the main issue.

The only remaining question is..10S or 12S?
The VESCs I am using have upgraded components. 

* Upgrade by C1,C8,C9,C39,C40,C42,C43,C44,C45,C49 from 10yF 50V to 4,7yF 100V
* Extra upgrade by C46,C47 2 resistors extra 4,7yF 100V and to the C37, C51 we build
for more reserve on C48 2x 4,7yF 100V resistor.
* R53,R54 WSLP2726 Shunts

Going to 12S would give me a theoretical top speed that is 10km/h higher. Not sure if that would help with hill climbing...Not sure if my controllers would happily accept 12S without additional cap banks.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2017-10-17T10:51:06.433Z Reads: 164

```
Just get a bluetooth module and a android smartphone and use my app to make a video with the realtime data. Would be interesting to see in detail what happens.
```

---
## \#18 Posted by: telnoi Posted at: 2017-10-17T10:53:11.720Z Reads: 170

```
Stupid question probably, but does your app work with the vesc-tool firmware?
```

---
## \#19 Posted by: rich Posted at: 2017-10-17T10:54:36.298Z Reads: 175

```
Max.discharge 50A sounds weak. Do you have a mounted voltmeter? The voltage sag could be huge. But on the other side I guess the 63mm motors could be a bottleneck, too. I use(d) 10s 10Ah Lipo with max. cont. discharge of 150A, 6364 136kv motors and esk8 4.12 controller (14T/66T gear ratio 4.71:1 on 8" wheels). My vesc settings for motor and batt max is 100A together. When catching some speed I can climb crazy hills but it's impossible to climb too steep hills especially offroad. Once I tested the limits of hill climbing, I had to take several brakes because the motors got sizzling hot and had no more power, it was too steep. I am switching to Vesc 6 soon and looking forward to see if there is a difference in hill climbing.according to V4.12, then I know if the motor or the V4.12 was the bottleneck. Unfortunately I killed my lipo and can't test it now. Since 2 weeks I can't decide if I should go with Lipo or Li-ion. I'm afraid of weak brakes with Li-ion. 

[quote="telnoi, post:1, topic:35759"]
Is 12S safe, or would it be better/safer to stick to 10S?
[/quote]


For safety I would stay with 10s on esk8 1.1 controller as long as you don't need more top speed. Personally I wouldn't risk it but it could work.

Which FW do you use and which mode? BLDC or FOC? 

From my experience I get much more torque and power with FOC compared to BLDC at slower speed. In BLDC mode I slow down on a hill and with FOC I can even accelerate a bit on the same hill. I've made a stupid video comparing the modes (sorry it is way too long in the middle, have to skip)

https://www.youtube.com/watch?v=ptlHqK7kqCA
   .
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-10-17T10:54:40.999Z Reads: 160

```
Yes it does.
```

---
## \#21 Posted by: telnoi Posted at: 2017-10-17T11:04:23.790Z Reads: 148

```
Thanks for the valuable feedback (and others)..6374 motors a limitation. That would suck.
I do have a mounted volt meter, but it's mounted on the back and not visible during day light. Will get a BT module as suggested before and will record the ride.

Yah, weak brakes is the primary reason for not even considering Li-ion as an upgrade path, along with the the low A rating and price (even when switching to 30A cells).

I run BLDC.
```

---
## \#22 Posted by: Ackmaniac Posted at: 2017-10-17T11:09:39.269Z Reads: 148

```
Don't know exactly about the trampa motors but most 6364 motors are in reality a 6355 motor. And a sk3 for example also isn't a 63 diameter, it is only 59mm but a bit longer.
http://www.electric-skateboard.builders/t/whats-the-difference-in-performance-between-dual-a-6374-and-dual-6355/25902/46?u=ackmaniac
So a 6374 should make a noticeable difference when it comes to heat and torque at high amps.

For street setups that can be ignored if you weigh less than 100 kilos but for offroad builds that might makes the difference.
```

---
## \#23 Posted by: rich Posted at: 2017-10-17T11:34:15.590Z Reads: 145

```
Yes, that could be the reason due to stator size, also the trampa motors are rated for 2400W. Would love to feel the difference compared to 6374 but I'm broke :laughing: But I haven't seen any video where someone climb really steep hills with an e-mtb, please post if someone knows one.

@telnoi just as a reference, my voltage sag with my 10s 10Ah 150A Lipo pack was about 0.5V on flats and max 1V with full throttle on steep hills.
```

---
## \#24 Posted by: telnoi Posted at: 2017-10-17T11:37:25.537Z Reads: 144

```
those lying bast... 
Ah well, I'll ride these motors until they fall apart. 

Until then, perhaps a lower KV version of this will become available.
https://www.banggood.com/Racerstar-6368-BRD6368-280KV-6-12S-Brushless-Motor-For-Balancing-Scooter-p-1117657.html?rmmds=search

Perhaps not that big of an improvement though.

In conclusion. First implement a BT module, record a ride, probably upgrade to 10s2p lipo based on recorded results...in the end, new motors.

Due to the walking I currently have to do I'll probably loose some weight = automatic performance gains.
```

---
## \#25 Posted by: Cobber Posted at: 2017-10-17T11:43:32.400Z Reads: 137

```
seems you have avoided answering key questions bro...
```

---
## \#26 Posted by: Ackmaniac Posted at: 2017-10-17T11:44:41.332Z Reads: 136

```
I would recommend to raise the motor max settings. Problem is that at very low speed (like starting at a hill) the motors are very inefficient. And inefficiency means that the power is transferred into heat.  So i think it is better to start quickly with a short high amp pulse (80A for example) instead of stressing the motors at like 50A for a long time because you gain no speed. Then you also wouldn't have the power issues uphill.

And it would be awesome if you could get a bluetooth module and make some videos with realtime data logging on that track.
```

---
## \#27 Posted by: telnoi Posted at: 2017-10-17T11:45:21.505Z Reads: 131

```
I think I missed one question out of all here...though feel free to reiterate the ones I have missed/I double checked.
I run the latest vesc-tool firmware (one that I saw I missed).
```

---
## \#28 Posted by: telnoi Posted at: 2017-10-17T11:53:10.469Z Reads: 131

```
Ordering a BT Module. Will report back as soon as things are up & running.
Will be interesting/also to see what influence motor max has. Thanks again for all the help & suggestions.
```

---
## \#29 Posted by: telnoi Posted at: 2017-10-18T08:14:00.688Z Reads: 121

```
Was able to monitor the voltage today.
Whilst moving at 2/3rd speed, voltage dropped from about 40 to 37. When the board grinds to a halt due to a hill, it drops further to 35.3V.

That said, I greatly improved my average speed today and cut down traveling time from 50 minutes to 35. The additional speed helped the board to slowly crawl up to one hill where I had to walk before. Slowly getting used to it :grin: Best transportation yet.
```

---
## \#30 Posted by: telnoi Posted at: 2017-10-27T15:57:11.966Z Reads: 108

```
I just increased my motor min and max to -80 & 80 from 60 respectively. Braking sucks now, even though I did not change any other settings. Normal? Why does that happen?

Vesc tool .28.
```

---
## \#31 Posted by: esk8 Posted at: 2017-10-27T17:17:20.154Z Reads: 106

```
The esk8 1.1 controller can give out continuous 60A,
I ride my Flame Board with 60A/-60A/60A/-20A and its working perfect with FW 2.18.
I have 10S/6P Li-Io 18650.
I don´t like the SK3 Motors, and i think that´s the motors working fine with
12S in a Airplane when the motor was in the wind, but behind one MTB 
and only by 30Km/h became the motors not enough cooling and can overheat.
The most important is that your battery have enough discharge.
Sorry but not for uncomfortable but the bluetooth modul working good with FOCBox 
and Ackmaniacks FW but i don´t know how working with the esk8 1.1 controller.
In last time have some people problems with the Vesc Tool and the bluetooth module.
```

---
## \#32 Posted by: esk8 Posted at: 2017-10-27T17:20:50.375Z Reads: 103

```
https://youtu.be/RgVthPpuI6E
```

---
## \#33 Posted by: telnoi Posted at: 2017-10-27T18:24:24.898Z Reads: 101

```
Thanks for the warning about the temperature of SK3 @12s.
Yes, the Li-Ion pack I have is not sufficient for E-MTB purposes. 
Today during a 400 meter climb (height difference), the voltage sagged from 39 to 33V, very close to the cut-off value.

At 80A motor max, the voltage sag appeared to be more severe and braking as mentioned before was pretty much useless except for slowing down a bit. I have to get a different pack for safety reasons.
```

---
## \#34 Posted by: esk8 Posted at: 2017-10-27T19:35:41.562Z Reads: 100

```
I think the problem can be
also at the BMS
The esk8 controller became not enough power from the BMS
and they  must splitting the A between the two controller.
So your motors became not enough power.
But i think it better when you go with 10S 
so you don't going to the limit.
```

---
## \#35 Posted by: telnoi Posted at: 2017-10-27T19:37:45.043Z Reads: 98

```
Agreed.

<img src="/uploads/db1493/original/3X/b/f/bf3264a39f1ea4a24dba1fb06e78601248061da1.png" width="690" height="175">

Should solve it.
```

---
## \#36 Posted by: telnoi Posted at: 2017-11-04T15:31:40.885Z Reads: 83

```
Same route today that normally gave me difficulties, though with just two packs instead of 4 (waiting for new charger). Holy cow, what a difference...and I'm only using 35A battery max at the moment. 

No voltage sag with the lipos and the power delivery is allot more constant/not nearly as much variation in speed previously caused by constantly changing ground conditions. Smoother ride, more stability. Also climbs those hills allot better.

Range with just 8000 is reduced, now stuck on a parking lot waiting for my wife :P
```

---
## \#37 Posted by: telnoi Posted at: 2017-11-13T09:07:46.675Z Reads: 62

```
Increased from 35 to 50A battery max after removing the anti-spark switch (replaced with XT-90 anti-spark). 

Very little performance increase, though it has a bit more torque now and is a little bit faster on steep hills. I may have hit the limit of my SK3 149 KV.
```

---
## \#38 Posted by: WARMAN Posted at: 2017-11-13T09:31:07.597Z Reads: 62

```
[quote="telnoi, post:1, topic:35759"]
will mainly be using it to travel to work. About 80% offroad
[/quote]

Not one comment about your route to work,I'm very jelous...80% off road!...living the dream!
```

---
## \#39 Posted by: telnoi Posted at: 2017-11-13T09:38:45.661Z Reads: 63

```
Yeah, it's awesome :slight_smile:
There are allot of cool spots around here, including an old American military field with a few KM of concrete roads in the middle of nowhere. I often ride though the entire forest you see there in the upper left corner. 16 AH is just about enough to cover part of it.

 <img src="/uploads/db1493/original/3X/2/5/250b6fa7c0cba3c96076fc5f7742cf82bf0c4839.jpg" width="282" height="500">
```

---
## \#40 Posted by: WARMAN Posted at: 2017-11-13T09:44:22.006Z Reads: 62

```
Nice! There's a few good places to ride where I live but being able to commute to work 80% offroad is by far the best commute iv ever heard of..enjoy!
```

---
