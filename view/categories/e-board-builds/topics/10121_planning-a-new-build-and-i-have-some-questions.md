# Planning a new build and I have some questions

### Replies: 37 Views: 2122

## \#1 Posted by: Smorto Posted at: 2016-09-25T13:26:01.440Z Reads: 169

```
Just to start, here is my parts list so far:
SK3 213kv motor (this is my ideal but might have to go 190kv if the 213kv isn't in stock when I buy it)

2 4s1p 5000mah batteries in series for 8s 5000mah battery

Enertions VESC

Enertions 12mm drive system

XT90 anti spark loop

90m flywheel clones

Reverse kingpin 180mm trucks

For the switch, I want to use just a regular light switch and hook it up to one of the battery wires running to the VESC

Custom deck

RC car receiver and transmitter from a friend

Extra XT90, XT60, 4mm bullet connectors, and 10 AWG wire

Now for my questions

Does the parts list look good, am I missing anything? 
Will all the parts work well together? 
Can y'all point me in the direction of some good VESC configuration tutorials? 
Does the VESC take XT60 or XT90 connectors for the power input? 
Will my standard light switch idea work or will the 8s battery fry it?
For connecting the batteries in series is it ok to just use the bullet connectors that come with them and just solder on an XT60 or XT90 to the remaining + and - or do I have to clip the bullet connectors of and make an XT60 or XT90 series wire harness?
Is the calc.esk8.it/ calculator very accurate even If I way around 115 pounds (52 kg)?
Will the Enertion wheel pulley fit my 90mm flywheel clones?
```

---
## \#2 Posted by: Mrmoonlight Posted at: 2016-09-25T18:12:20.771Z Reads: 132

```
For the trucks, go with Calibers or stuck with the Enertion trucks. Basically the same thing. Enertion's VESC uses an xt60 connector. DIYelectric uses an Xt90, and Ollin's doesn't come with one, but his cables are larger, so I'd recommend 90's.

Switches are cheap and easy to solder on. Better than trying to fit a light switch in your box. Plus it's easier to have your power switch external. 

Bullet connectors are fine, but I'd recommend soldering your connections to the VESC, motor, and reciever if you can. Connectors have a habit of coming undone.
```

---
## \#3 Posted by: Smorto Posted at: 2016-09-25T19:23:03.514Z Reads: 127

```
Thanks for the response. I think I will stick with the trucks I have simply because I am on a budget and I believe I can design my own motor mount. As for the light switch, I will definitely have enough room in my box for it and I chose it because A. I already have it and it requires no soldering or anything B. It is larger and tactile so I like the feel of it. Do you think that exertions wheel pulley will fit with my 90mm flywheels?
```

---
## \#4 Posted by: Mrmoonlight Posted at: 2016-09-25T19:58:55.125Z Reads: 122

```
I've seen a couple variations on 90mm Flywheel clones. I have a clone set on my Carvon hubs that is good quality, but the hole pattern is slightly different and my Flywheel pulley doesn't fit. Post a pic. 

As for additional goods, I recommend picking up some adhesive backed neoprene foam for padding, velcro to keep everything in place (but easy to rearrange), a charger and some shrink tubing. If I'm using a connector, I like to shrink tube over it to keep it from coming apart, but still have the ability to disconnect it. If you ride anywhere that might have interference, a ferrite bead on the wires that go from your receiver to your VESC helps. I pulled mine off an old computer cable.
```

---
## \#5 Posted by: Smorto Posted at: 2016-09-25T23:08:08.398Z Reads: 117

```
<img src="/uploads/db1493/original/3X/f/c/fc1b7cfa767993d347a04f2cb359715b5b657ba8.jpg" width="690" height="459"><img src="/uploads/db1493/original/3X/9/3/93ecdd507d74033e4b40485f3a70dab784f5a49e.jpg" width="690" height="459">

Here are some pics of the wheel
 I don't think interference will be an issue since I live in a rural area.
I have a charger picked out with a parallel charging board so I can charge both batteries at once. If I do that, I plug in both batteries with the power connector and the balance plug, so I would probably have to make the XT60 wire harness to put them in series then just un plug it to charge. I also have shrink tubing.
```

---
## \#6 Posted by: Mrmoonlight Posted at: 2016-09-26T05:25:30.745Z Reads: 97

```
I know the Enertion Pulley is compatible with genuine Flywheels, but your hole pattern has the larger spokes. I think Enertion's wheel uses the larger spokes, but you'd need to verify that with Enertion... or if anyone else who has more knowledge can chime in?
```

---
## \#7 Posted by: Sharkface Posted at: 2016-09-26T06:05:48.479Z Reads: 94

```
I will be trying to figure this out for myself, so ill be following along on this for this very reason lol
```

---
## \#8 Posted by: Smorto Posted at: 2016-09-26T10:22:32.409Z Reads: 94

```
I put in a message to the contact us page on enertions website, I'll give them a few days to answer
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-09-26T13:26:03.242Z Reads: 91

```
why are you going 8s? just to safe some moneys?
a sweat spot with a 190kv would be 10s - so 2 5s lipo perhaps.
or if you like to stay with 8s get yourself a 245kv.
more power - more fun :slight_smile:
```

---
## \#10 Posted by: EssEnn Posted at: 2016-09-26T14:00:48.040Z Reads: 92

```
For 10AWG wire I would recommend 5mm bullet connectors as I found the 4mm ones were way to small. For my build I replaced all the bullets with 5mm ones and XT90's in the batteries. 

I also bought an 80w soldering iron which made soldering easy but be caseful with the XT plugs as you can melt the plastic really easy. Make sure you have spares and after you have tinned the wire and connector, heat the wire first and then the connector.
```

---
## \#11 Posted by: Smorto Posted at: 2016-09-26T18:13:17.080Z Reads: 89

```
Yes, I am going with 8s because I found some 4s 5000mah batteries on HK for around $30 which is a good price. I originally wanted to go with 213kv because it seems like it has a good balance of speed and torque. If you think that 245kv will be enough torque for my weight (115 pounds 52 kg) to climb moderate hills than I would be more than happy to change to 245kv especially since they are currently in stock at HK.
```

---
## \#12 Posted by: Smorto Posted at: 2016-09-26T18:15:58.579Z Reads: 90

```
I will probably switch to 5mm bullet connectors but I don't know if it would be worth the extra $5 or whatever since I am only using them for the motor-VESC connection. Do you think it is worth buying them, or should I just solder the motor wire to the VESC directly and shrink wrap to avoid shorts?
```

---
## \#13 Posted by: Smorto Posted at: 2016-09-26T18:25:00.973Z Reads: 87

```
Ok so enertion answered but it wasn't very helpful. Their exact words were

Thank you for contacting Enertion Support. The Enertion 12mm pulley and 12mm drive hub both fit with Enertion power wheels and ABEC 11 flywheels.

I e-mailed them back saying thanks for the quick reply but asking if my specific wheels will fit the hub. We'll see what their answer is.
```

---
## \#14 Posted by: Jinra Posted at: 2016-09-26T18:29:20.819Z Reads: 87

```
Yea it wont fit those thicker spokes, they're made of spokes like these

http://www.sk8trip.com/mm5/graphics/00000001/ABEC11Flywheels_90mmLRG.jpg

You can file the spokes down to fit if you want. Though that might affect structural integrity.
```

---
## \#15 Posted by: EssEnn Posted at: 2016-09-26T18:38:40.648Z Reads: 80

```
If you are going to use bullets and 10awg wire you will need 5mm ones. The 4mm will be a right bugger to solder and I found the 5mm ones to be perfect. 

As for directly soldering to the VESC, I can't really help you there. Zero experience with those but just think about the mission to change your motor if it dies. Personally I would not like to be de-soldering / soldering frequently on the PCB but is just me. If you are working in a tight space then you probably won't have the room to put in bullets. 

I'm going to have to build me a street board with a VESC to see what all the fuss is about
```

---
## \#16 Posted by: Smorto Posted at: 2016-09-26T18:45:41.066Z Reads: 85

```
These are the trucks and wheels I am using, are yo sure they won't fit because the only difference I see is the three small cutouts in the middle of the abec wheels

https://www.amazon.com/Longboard-Trucks-Flywheels-Owlsome-Bearings/dp/B01IBJXW5Q/ref=sr_1_1?ie=UTF8&qid=1474915437&sr=8-1&keywords=90mm%2Bflywheels%2Band%2Btrucks&th=1
```

---
## \#17 Posted by: Jinra Posted at: 2016-09-26T18:51:58.548Z Reads: 83

```
That's exactly the difference that makes it not fit. You'll have to file the spokes (or the enertion pulley) down. It's much more work than it's worth IMO, but you can do it.

If you see the listing you linked, the spokes are thinner in the picture than in reality. You can probably return this to amazon for free under false advertisement.
```

---
## \#18 Posted by: Smorto Posted at: 2016-09-26T19:01:30.997Z Reads: 80

```
I am still confused because the enertion power wheels don't have that cut out

http://www.enertionboards.com/buy-build-your-own-electric-skateboard-parts/83mm-enertion-power-wheels/
```

---
## \#19 Posted by: Jinra Posted at: 2016-09-26T19:51:56.385Z Reads: 73

```
I think that was a picture from when they used a different mounting system. Their current wheels may be different.
```

---
## \#20 Posted by: Mrmoonlight Posted at: 2016-09-26T20:25:57.932Z Reads: 74

```
Check out . Their pulley is a bit different and would fit.
```

---
## \#21 Posted by: Smorto Posted at: 2016-09-26T22:34:05.035Z Reads: 66

```
Are you talking about this set?
diy-electric-skateboard-kits-parts/36t-abec-drive-pulley-belt-combo-kit/

Because I am not sure that the bolt would fit in between the spokes. Also would it be easy to find nuts to fit those bolts in the US?
Also, I would be using a turnigy sk3 motor which has an 8mm diameter shaft and the specs about this motor pulley aren't listed. It also doesn't come with a grub screw or key so I don't see how you attach the pulley to the motor.

If @Jinra you think it wouldn't be a huge mod to the wheel or the pulley, then I will stick with the exertion set but if you think otherwise, let me know
```

---
## \#22 Posted by: Jinra Posted at: 2016-09-26T22:41:29.870Z Reads: 57

```
The old pulley required you to driller through the wheels so the bolts would fit. I suppose you can do the same for the new enertion pulley, but I'm not sure how well it'll work. I don't have flywheel clones with those types of spokes so it's anybody's guess!
```

---
## \#23 Posted by: Smorto Posted at: 2016-09-26T22:43:02.692Z Reads: 58

```
Actually, taking a closer look at the wheels from enertion through Jason's videos, there doesn't appear to be any cut outs like in the abec 11 ones. Wouldn't that cut out be covered up by the bearing anyway?
```

---
## \#24 Posted by: Sean555 Posted at: 2016-09-26T22:46:16.485Z Reads: 60

```
These are the clone 90s that I purchased off eBay, they fit Enertion mounts 
http://www.ebay.com/itm/131875341711
```

---
## \#25 Posted by: Smorto Posted at: 2016-09-26T22:47:36.241Z Reads: 58

```
Those look exactly like mine so that gives me confidence that they will work! Thanks a ton!
```

---
## \#26 Posted by: Jinra Posted at: 2016-09-26T22:55:18.183Z Reads: 57

```
Report back with your findings! Someone on the Evolve thread said the evolve pulley didn't fit their 97mm clones due to the fatter spokes. However, Enertion's pulley is thinner so maybe it'll fit all flywheel clones.
```

---
## \#27 Posted by: Smorto Posted at: 2016-09-26T23:53:57.560Z Reads: 55

```
@Sean555 just to be clear you meant they will work with the enertion wheel pulley, not mounts right?
```

---
## \#28 Posted by: Sean555 Posted at: 2016-09-27T00:18:45.133Z Reads: 56

```
Yes, they work with the pulley. 100%
```

---
## \#29 Posted by: Smorto Posted at: 2016-09-27T00:42:16.894Z Reads: 55

```
Sounds good, thanks!
```

---
## \#30 Posted by: TarzanHBK Posted at: 2016-09-27T06:31:55.510Z Reads: 57

```
you won´t have any problems going up any hill trust me :smiley:
```

---
## \#31 Posted by: Smorto Posted at: 2016-09-28T00:14:49.080Z Reads: 50

```
Sorry to keep bothering you @Sean555 but you did mean to say the 90mm wheels right, not the 83mm ones? Cause just got another e-mail from enertion support saying the pulley is made for 83mm wheels. But if you are sure they were 90mm then I will take your word for it
```

---
## \#32 Posted by: Jinra Posted at: 2016-09-28T00:31:47.273Z Reads: 52

```
same pulleys for 83-97mm abec styles. legit 107mm flywheels wont fit the axle, but they all have the same hub profile.
```

---
## \#33 Posted by: Smorto Posted at: 2016-09-28T01:14:53.715Z Reads: 53

```
ok, thanks!
```

---
## \#34 Posted by: Sean555 Posted at: 2016-09-28T01:17:00.103Z Reads: 53

```
I used my enertion pulleys on the clone 90s I linked to.<img src="/uploads/db1493/original/3X/a/8/a8f1f3a9bbdcf035a7b8770653318efafb14da56.jpg" width="668" height="500">
```

---
## \#35 Posted by: Smorto Posted at: 2016-10-09T01:59:21.618Z Reads: 46

```
Okay @Jinra @Sean555 @TarzanHBK @Mrmoonlight just wanted to notify you so you see it. I got my enertion set and the pulley did end up fitting after I just clamped it a little bit. 
 src="/uploads/db1493/original/3X/c/a/cac58b623545196aed862c86f28822843e80994b.jpg" width="690" height="459">




<img src="/uploads/db1493/original/3X/f/9/f93ca5c509b4a4764cfcd8ac9c5c5d2c15e05f4f.jpg" width="690" height="459">



Lengthened one of the truck axels<img 


<img src="/uploads/db1493/original/3X/a/3/a38e943a448a1dade05c2f9f08adf149d447bb80.jpg" width="690" height="459">    




<img src="/uploads/db1493/original/3X/a/9/a93be0a726869517a5bddbf321e4c24ba71400fe.jpg" width="690" height="459">


And done!

 I will post the rest of the mechanical build and the electronics will be posted after Christmas as I will be asking for most of the parts for Christmas
```

---
## \#36 Posted by: Mrmoonlight Posted at: 2016-10-09T03:01:26.457Z Reads: 44

```
The pulley should be a tight fit. You don't want it jiggling around at all since your inside bearing is resting on it.

Looks good!
```

---
## \#37 Posted by: Sean555 Posted at: 2016-10-09T06:15:35.025Z Reads: 41

```
Tight is always good.   Free life lesson😀
```

---
