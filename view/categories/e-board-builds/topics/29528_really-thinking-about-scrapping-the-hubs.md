# Really thinking about scrapping the hubs

### Replies: 51 Views: 2154

## \#1 Posted by: Sapphirinia Posted at: 2017-08-03T02:39:11.360Z Reads: 319

```
They still work but I've been having so much trouble with my dual hub penny nickel. 2 out of 3 Vescs have now broken, one that I never actually got to work brand new. So now I have a total of 1 working VESC, not sure if it's worth the trouble of getting the other new one replaced for fixed. I think it might be time to try a single motor build with all the pulleys, belts, and stuff. What do yal think? I feel it may be easier to get working and to keep working... <img src="/uploads/db1493/original/3X/1/f/1f1846c334134192f49639a8e96aa469b5df0447.jpg" width="666" height="500">
```

---
## \#2 Posted by: willpark16 Posted at: 2017-08-03T02:59:58.289Z Reads: 305

```
Get different ones those aren't really that good
```

---
## \#3 Posted by: lrdesigns Posted at: 2017-08-03T06:44:17.178Z Reads: 288

```
I'm not sure 1 vesc 1 motor belt drive is electrically simpler but mechanically more complex than dual hubs x2 vesc. If you feel more mechanically inclined it may be better. 

A dual system runs cooler as the load is spread out among the components.
```

---
## \#4 Posted by: BigBoyToys Posted at: 2017-08-03T06:54:44.869Z Reads: 278

```
Dont give up! Blowing up vescs is just part of the deal. Consider it growing pains. As long as you can figure out what you did wrong the last time you are moving in the right direction.
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2017-08-03T06:58:04.462Z Reads: 273

```
yep I love throwing my old vesc on the concrete outside... I'm already at 3 destroyed =) actually 4 I'm sorry.
```

---
## \#6 Posted by: Vanarian Posted at: 2017-08-03T14:35:38.094Z Reads: 252

```
It does look like you didn't size your electronics up to your requirements, thus you overload the VESCs. If the hubs are running well it is not a motor problem. Low Kv is easier to manage than high Kv, no ERPM problems. 

You simply ask too much amps from your setup no? 

Are you running VESC 4.xx? 

You could improve the VESC settings by lowering max amps, play with ramp settings to improve "torque feeling " and of course put some cooling on your FETs. 
If that's not enough, yes you are right to look for drive setup but you need bigger motors and dual setup. Or try 4wd hubs?
```

---
## \#7 Posted by: anorak234 Posted at: 2017-08-03T15:44:40.845Z Reads: 223

```
Just get a better VESC... like a FOCBOX or VESC-6
```

---
## \#8 Posted by: NickTheDude Posted at: 2017-08-03T15:54:20.491Z Reads: 216

```
Before we give any advice it'd be nice to see your VESC settings. If VESCs getting blown is the issue then getting new motors probably won't fix it.

Also what kV/voltage are you using?
```

---
## \#9 Posted by: ATLesk8 Posted at: 2017-08-03T21:01:13.414Z Reads: 207

```
Just get one of the cheap ebay dual hub escs. I just got one shipped for $62 and it seems to work great with cheap hubs.
```

---
## \#10 Posted by: lowGuido Posted at: 2017-08-04T05:58:47.548Z Reads: 196

```
[quote="BigBoyToys, post:4, topic:29528"]
Dont give up! Blowing up vescs is just part of the deal. Consider it growing pains.
[/quote]

Thats an advertisement for VESC if I ever heard one!
I'd love to disagree and say its not true. But It kinda is. There are a lot of things you can do to prevent VESC cooking, but chances are if you are new to it then you are gonna burn some.
```

---
## \#11 Posted by: BigBoyToys Posted at: 2017-08-04T06:10:56.785Z Reads: 186

```
I wish I could say I stopped burning them but the deeper I get the more I demand from them.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-08-04T06:24:23.820Z Reads: 185

```
I have 4 vescs running on 2 boards.  Got my first set over 1 year ago and second set 10 months ago.
I have never had a single issue with them. And I don't baby them either. Motor max 80a / Batt max 50-60a.
This is because I started with quality vescs from @chaka with heatsinks.
They where not cheap upfront but in the long run they where worth the investment.

Hub motors  should do fine if your riding mostly flat ground or mild inclines.
And as long as the phase wires are not shorting intermittently. You can test that by unplugging the phase wires from the vesc, spread them so the connectors don't touch then spin the motor by hand while moving the wires around. If it feels like the brakes come on while moving the wires, then you have an intermittent short and that can blow the vesc.
```

---
## \#13 Posted by: NAF Posted at: 2017-08-04T12:39:53.439Z Reads: 163

```
[quote="Namasaki, post:12, topic:29528"]
spread them so the connectors don't touch then spin the motor by hand while moving the wires around. If it feels like the brakes come on while moving the wires, then you have an intermittent short and that can blow the vesc.
[/quote]

Interesting tip ..I need to try this today on my Carvon Single Hub 2.5. I have experienced something weird ...3 or 4 times the motor started to spin on it's own ! It was never when the deck was on the ground it happened when I lifted the board to vertical position. It happened two weeks ago and it never happened again.  I am not sure what it was. Maybe it was Vesc and not the Motor.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-04T15:19:44.081Z Reads: 144

```
A short would not cause that. 
Could be interference cause wrong signal from the receiver or trim adjustment on the controller. 
Or you may need to calibrate your controller with Vesc in bldc tool.
```

---
## \#15 Posted by: Sapphirinia Posted at: 2017-08-07T00:47:16.797Z Reads: 131

```
75kv hubs
I was using 12s setup. 
Highest speed I hit was 17mph when the first vesc blew. Total of 3.5miles. I only rode on a primarily flat bike path around a park. Was still testing for range/speed. 
The second broken vesc NEVER actually got a hub to spin. Finally decided to check for faults and got the drv error
New setup is 8s, more concerned with distance than speed
```

---
## \#16 Posted by: Sapphirinia Posted at: 2017-08-07T18:16:20.520Z Reads: 126

```
I'm still trying to figure out what /who is at fault.
```

---
## \#17 Posted by: Sapphirinia Posted at: 2017-08-07T18:17:25.815Z Reads: 126

```
I also had the max at 40. It was too torquey at the default 60
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-08-07T19:40:26.307Z Reads: 118

```
Im leaning towards that motor having an internal short. Did u ever get it vert hot? Mine got hot within minutes even witj my 135lb friend riding it.
```

---
## \#19 Posted by: BigBoyToys Posted at: 2017-08-07T19:41:28.166Z Reads: 120

```
Send your vesc to @JohnnyMeduse. He can repair it for you.
```

---
## \#20 Posted by: akhlut Posted at: 2017-08-07T19:55:56.864Z Reads: 115

```
@Sapphirinia I'm down in the Atlantic City area and could swing up to Philly and check out your setup.  I hand-soldered my VESC and have the parts for 2 more, so we could try and troubleshoot/fix it.

Before I scrubbed it with alcohol. You can see a lot of flux there.
<img src="/uploads/db1493/original/3X/e/4/e4d821ba46ea16d982b5fc105627eed0f32b3923.jpg" width="281" height="500">

Let me know
```

---
## \#21 Posted by: BigBoyToys Posted at: 2017-08-07T20:42:42.616Z Reads: 107

```
Thats an awesome offer and what makes this community so great!
```

---
## \#22 Posted by: Sapphirinia Posted at: 2017-08-08T02:23:23.479Z Reads: 106

```
Please! I actually live in Camden. So you don't even have to cross the bridge!
```

---
## \#23 Posted by: Sapphirinia Posted at: 2017-08-09T02:21:14.932Z Reads: 101

```
So after an extensive diagnostic session, the vesc still doesn't work. Hopefully @akhlut can get it working when he gets more time. I'm not crazy, Yay!
```

---
## \#24 Posted by: akhlut Posted at: 2017-08-09T15:21:36.749Z Reads: 97

```
OK, here are the VESC's!

Alextech VESC. Saddest VESC

Blown DRV, blown MOSFETS.

<img src="/uploads/db1493/original/3X/2/b/2b0009f06c4639a8d8dc962629e7433f0c58e3f8.jpg" width="690" height="433">

<img src="/uploads/db1493/original/3X/6/9/69758be112eed3da1f660c74081972ab42d1936f.jpg" width="690" height="425">

-----

Happier VESC

Alextech VESC, Gives DRV Error & need to replace inductor

<img src="/uploads/db1493/original/3X/4/4/44ede04b7e697961dbad25506c0929af361865ae.jpg" width="690" height="452">
<img src="/uploads/db1493/original/3X/3/b/3ba912b63712997d9f165610c67f81f82e6fe9ac.jpg" width="690" height="449">
---

Happiest VESC

Torqueboards VESC, Gives DRV Error

<img src="/uploads/db1493/original/3X/0/1/01579ed4cad85194088bd3d819bfa4e2927f14f3.jpg" width="690" height="457">

<img src="/uploads/db1493/original/3X/8/2/82e6889f38569c367102cabcbc210a3d41d99324.jpg" width="690" height="456">


So now for the fun!  Going to try and breathe life back into these guys and see what happens.
```

---
## \#25 Posted by: Blasto Posted at: 2017-08-09T15:27:32.972Z Reads: 86

```
[quote="akhlut, post:24, topic:29528"]
Alextech VESC, Gives DRV Error & need to replace inductor
[/quote]

Just to save you some work, you don't need to replace the inductor, that darn package chips easily, but doesn't affect it's performance (from what i know of)
```

---
## \#26 Posted by: akhlut Posted at: 2017-08-09T15:31:47.568Z Reads: 88

```
ok, will skip!
```

---
## \#27 Posted by: Sapphirinia Posted at: 2017-08-09T15:36:41.881Z Reads: 90

```
Currently transported to the intensive care unit. May the surgeons skilled hands reverse this death sentence. 😢😢🏥
```

---
## \#28 Posted by: akhlut Posted at: 2017-08-09T15:37:20.360Z Reads: 90

```
Also, took apart one of the alextech hub motors.  It looked just like the motor in this video:

[https://www.youtube.com/watch?v=9YO1IbQQ1w4](https://www.youtube.com/watch?v=9YO1IbQQ1w4)

So, that one at least is shot.  need to take apart the other to see what it looks like...
```

---
## \#29 Posted by: Blasto Posted at: 2017-08-09T15:38:18.195Z Reads: 86

```
This guy had a hard life, the top fet looks cracked also

<img src="/uploads/db1493/original/3X/e/5/e5ef69c77db61110c6eb327f7e355767b4ce24b5.png" width="512" height="499">
```

---
## \#30 Posted by: akhlut Posted at: 2017-08-09T15:40:42.544Z Reads: 82

```
Yep.  I noticed that.  think I'm gonna take all three off and just start fresh.
```

---
## \#31 Posted by: Sapphirinia Posted at: 2017-08-09T16:09:22.016Z Reads: 76

```
I'll take apart the other one and check it. Looks like I gotta replace even more stuff.
```

---
## \#32 Posted by: Sapphirinia Posted at: 2017-08-09T16:20:54.752Z Reads: 78

```
So... If my motors are shot, Im probably better off going to a single motor and ditching the hubs. I really only wanted smaller hubs and they were hard to find. Guess I should start looking for regular motors. At least they're cheaper than hubs.
```

---
## \#33 Posted by: akhlut Posted at: 2017-08-09T16:25:53.201Z Reads: 76

```
it's looking that way.  just be careful taking apart that hub motor!  

Post pics when you can.

Jlabs has a sale on motors now, $80.

https://buildkitboards.com/collections/motors/products/6354-208kv-motor
```

---
## \#34 Posted by: Sapphirinia Posted at: 2017-08-09T16:28:16.117Z Reads: 77

```
Any reason in particular you chose that over a hk one?
```

---
## \#35 Posted by: akhlut Posted at: 2017-08-09T16:36:41.783Z Reads: 78

```
yeah, I forgot you're running at 8s.  

Maybe this would be better:

diy-electric-skateboard-kits-parts/electric-skateboard-motor-5065-260kv/
```

---
## \#36 Posted by: akhlut Posted at: 2017-08-09T16:38:48.357Z Reads: 77

```
But before we get to that point, lets take a look at that other hub...
```

---
## \#37 Posted by: Sapphirinia Posted at: 2017-08-09T16:39:27.160Z Reads: 76

```
<img src="/uploads/db1493/original/3X/e/5/e50598853def7b39a020e4e742b612d250444d44.jpg" width="666" height="500">

Looks worse than the other one
```

---
## \#38 Posted by: Blasto Posted at: 2017-08-09T16:41:13.467Z Reads: 76

```
[quote="Sapphirinia, post:37, topic:29528"]
Looks worse than the other one
[/quote]

what the hell happened there, those don't even looked cooked... just broken...

could ask @evoheyax to rewind them, I hear he's getting the hang of it ;)
```

---
## \#39 Posted by: Sapphirinia Posted at: 2017-08-09T16:41:39.406Z Reads: 77

```
<img src="/uploads/db1493/original/3X/8/2/826a570bf818e4b7d8a65437466ed640f7de5740.jpg" width="375" height="500">
```

---
## \#40 Posted by: Sapphirinia Posted at: 2017-08-09T16:43:47.096Z Reads: 77

```
I wonder if there's a way I could just redo all the windings on both and make them work. Since all the other parts seem fine on them. And redo the phase wires.
```

---
## \#41 Posted by: akhlut Posted at: 2017-08-09T16:47:00.224Z Reads: 75

```
oh no...that's bad.
```

---
## \#42 Posted by: akhlut Posted at: 2017-08-09T16:48:43.989Z Reads: 74

```
can you take a pic of the long axis?
```

---
## \#43 Posted by: Sapphirinia Posted at: 2017-08-09T16:51:11.652Z Reads: 75

```
On the same part? <img src="/uploads/db1493/original/3X/a/d/adedb3b6a75eb6004155ff70761a6aa81ea02cc7.jpg" width="374" height="500"> 
Looks nice and neat from the top
```

---
## \#44 Posted by: Sapphirinia Posted at: 2017-08-09T16:51:59.790Z Reads: 75

```
<img src="/uploads/db1493/original/3X/5/3/53b84ae17b63d0c63a84f61bb44ee3005799a41e.jpg" width="375" height="500">
```

---
## \#45 Posted by: Sapphirinia Posted at: 2017-08-09T17:45:33.110Z Reads: 70

```
I found a link, and got some advice from evohayax so Im going to try to bring them back to life.
```

---
## \#46 Posted by: Sapphirinia Posted at: 2017-08-09T17:45:46.864Z Reads: 72

```
Plus I have more time then I have money...
```

---
## \#47 Posted by: Sapphirinia Posted at: 2017-08-09T18:02:01.827Z Reads: 74

```
Literally wasn't even connected to anything


<img src="/uploads/db1493/original/3X/f/a/faf90ee095164b6b7e011c4608d9e06127d1b210.jpg" width="374" height="500">
```

---
## \#48 Posted by: akhlut Posted at: 2017-08-09T19:40:29.620Z Reads: 70

```
Well OK then!  I guess it's time to unwind...
```

---
## \#49 Posted by: akhlut Posted at: 2017-08-09T22:56:15.401Z Reads: 67

```
Sad VESC looking happier!

<img src="/uploads/db1493/original/3X/b/f/bf4cc3ace13cbe2887aed626d6802ef70d8d5c4e.jpg" width="347" height="500">

But!  Pad 29 lifted when the DRV came off. 

<img src="/uploads/db1493/original/3X/1/d/1dd0c82c54b879e090b07cbb35363a3d946b1782.jpg" width="690" height="470">

But a 30GA wire from Pin 29 to C39 should do the trick!

<img src="/uploads/db1493/original/3X/1/d/1d6ca249cfc236fcdfa1c6e42f4c3ae4fb0afc24.png" width="690" height="388">

Making progress, but I have to get to the pool to put some laps in!
```

---
## \#50 Posted by: akhlut Posted at: 2017-08-10T23:31:14.164Z Reads: 61

```
Moar progress!

Removed all the bad chips and reflowed the DRV's on the two known good boards.  Waiting for some connectors to arrive tomorrow to test.  

Covered the connectors with kapton, but they got a little crispy.

Need to hit them with some isopropyl and a scrub brush.

<img src="/uploads/db1493/original/3X/9/5/956050e6548608960a860906b565d732f0c33196.jpg" width="690" height="388">
```

---
## \#51 Posted by: akhlut Posted at: 2017-08-12T00:30:16.229Z Reads: 52

```
Ready to test.

<img src="/uploads/db1493/original/3X/a/0/a0e15d017185430e11956ebb4abf90712756a330.jpg" width="690" height="388">
```

---
