# First build, 30+ mph, 2x 6374 190kv, help!

### Replies: 51 Views: 4019

## \#1 Posted by: Regas Posted at: 2017-11-01T14:46:57.945Z Reads: 368

```
So I’m planning on building an eboard and would like some friendly help, like telling me if the thing is going to fry/ or explode🙂.
Here are the parts:

1 of these:
products/torqueboards-218mm-trucks

2x these:
collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-w-drive-wheel-kit

1 of these: (I think these will fit and no need to drill holes, right?)
https://eskating.eu/product/all-terrain-longboard-wheels-black-100mm-set-of-4/

2x these:
products/electric-skateboard-motor-6374-190kv

2x these: (with both male to male servo and vesc sensor wire)
collections/featured-items/products/torque-esc-vesc-bldc-electronic-speed-controller

1 of these:
products/dual-vesc-xt90-parallel-connector

Do I need one of these?
products/vesc-can-bus-connector

1 of these: (with the battery glued in the enclosure)
https://eskating.eu/product/10s4p-eskating-electric-skateboard-battery-samsung-30q/

2 extra: (would these fit?)
collections/pulley-timing-belts/products/265mm-htd5-12mm-belt

10m4 bolts and 10 m4 threads: (for the enclosure)
https://eskating.eu/product/m4-bolts-for-enclosures-kit-of-6-pairs/

1 of these: (medium strength)
https://eskating.eu/product/thread-locker-for-pulleys-and-bolts-medium-strong/

1 of these: (don’t have any)
https://eskating.eu/product/sushi-ninja-longboard-skateboard-tool/

1 of these: (best one)
https://www.aliexpress.com/store/product/Electric-skateboard-refitting-parts-DIY-800MAH-remote-receiver-2-4G-bench-technology-benchwheel/1967440_32791243047.html

2x these: (I need these right?)
https://eskating.eu/product/2-x-seeger-for-8mm-shaft/

1 of these: (don’t have any)
https://www.aliexpress.com/item/120pcs-heat-shrink-tubing-with-glue-3-1-Shrink-the-shrinkable-tube-with-glue-Cable-Wire/32808904123.html?spm=2114.search0204.3.1.h3tbF3&s=p&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10344_10068_10345_10342_10343_10340_10341_10541_10084_10083_10305_10304_10307_10306_10177_5640015_10302_10060_10155_10154_10056_10055_10539_10538_5370015_10537_10312_10536_10059_10313_10184_10314_10534_10533_100031_10103_10073_10102_10142_10107,searchweb201603_1,ppcSwitch_4_ppcChannel&btsid=bfafd101-4baf-484e-a305-f47f988d08fb

And maybe only maybe one of these: (if everything fits)
https://eskating.eu/product/earthwing-belly-racer-37-50/

Couple questions:
1: would this setup be waterproof?
2: would the wheels fit the pulley with no drilling?
3: is it gonna explode?
4: could you tell me the range and the speed this setup would have?
5: could you tell me which vesc setup tutorial is closest to this setup.
6: I was looking maybe into another deck that would fit everything but that had a kick tail maybe like the super glider, you know any?
7: do you recommend to have master vesc and slave vesc connected via CAN bus or both connected to receiver or maybe both connected to receiver and via CAN bus?

If there are things I am missing feel free to tell me😃.
Thanks!
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2017-11-01T15:12:55.009Z Reads: 298

```
I have dual 6374 and 10s and first the all wheel terrain they work wonders but the motor pulley will not fit TB motor pulleys are to big and they don't include screws . I had issues when I upgraded my wheels to 97mm abec because wheels are bigger, so I recommend you  buy them from @chaka his website is  http://www.ollinboardcompany.com great customer service and quality everything else looks good , also water proof define water proof It rained  in Los Angeles yesterday and the road was still wet and well my board got soaked with puddles it all depends on the enclosure , I don't think any board is water proof just use weather sealing material
```

---
## \#3 Posted by: Regas Posted at: 2017-11-01T16:14:41.082Z Reads: 289

```
@Exiledd_Top By water proof I mean the motors because I think the enclosure is already water proof (no water infiltration).
I don’t get what you mean, do you mean the wheel pulley will not fit the MBS wheels because @torqueboards told me they did. Also,on their site you clearly see screws that come with the kit: 

collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-w-drive-wheel-kit

It’s not that I don’t like the Abec 11 97mm but they just aren’t AT.
Also, please answer the other questions 🙂!
```

---
## \#4 Posted by: Exiledd_Top Posted at: 2017-11-01T17:28:53.597Z Reads: 261

```
<img src="/uploads/db1493/original/3X/2/1/2143049b097ac9b11eb003b9888b7ff5745a0c00.png" width="281" height="500">
Talking about this , TB motor pulley is different and doesn't have the indentation it's big and the screws they provide are long so it will end up hitting the wheel if it's more than 90mm and changing the screws won't work
```

---
## \#5 Posted by: Regas Posted at: 2017-11-01T17:39:19.104Z Reads: 248

```
@Exiledd_Top So I should buy:
2x this:
collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-set-only-black
And 2x this:?
http://www.ollinboardcompany.com/product/16t-htd5-12mm-motor-pulley

Will this belt fit these components:?
collections/pulley-timing-belts/products/265mm-htd5-12mm-belt
```

---
## \#6 Posted by: Regas Posted at: 2017-11-01T17:39:56.051Z Reads: 226

```
Oh, and how about the wheel pulley?
```

---
## \#7 Posted by: WARMAN Posted at: 2017-11-01T17:41:06.258Z Reads: 231

```
Apparently most motors don't mind the rain and will fuction fine after being wet it's more debris you have to look out for!
As far as the canbus lead you can run it that way or just split the ppm and snip one of the wires.
No need to glue the battery in to the enclose you could add some foam to dampen the vibrations.
Your want a y piece xt90 connector or xt60 if your vesc's have that or you can make one.
I would only buy the all terrain wheels if you plan on going off road alot otherwise they wear down anyway "on road" and start to look like you standard road wheels.
```

---
## \#8 Posted by: Regas Posted at: 2017-11-01T18:14:38.624Z Reads: 222

```
@WARMAN So what’s the PPM? And which wire do I have to snip?
The y 2x vesc to battery is in the list up there.
That’s true, I won’t always be ridding this off road but I really want big wheels! Maybe the Abec 11 97mm that @Exiledd_Top posted before.
(Thanks for the feedback😋!)
```

---
## \#9 Posted by: WARMAN Posted at: 2017-11-01T18:19:16.151Z Reads: 225

```
http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461?u=warman
```

---
## \#10 Posted by: WARMAN Posted at: 2017-11-01T18:23:44.352Z Reads: 222

```
That should be all the info you need on it,I run the canbus at the minute,the traction control is nice especially in the wet but I will be switching to splitting the reciever signal soon simply because the connection from my canbus lead is now a little suspect and I have a splitter lying around!
```

---
## \#11 Posted by: Regas Posted at: 2017-11-01T19:40:20.491Z Reads: 219

```
Thank you! That thread was really interesting.
So would this one work? (All I have to do is cut one of the two middle red wires?)
https://www.hobbygo.com.au/receiver-transmitter/233-y-cable-0702105702215.html
```

---
## \#12 Posted by: longhairedboy Posted at: 2017-11-01T19:44:10.335Z Reads: 214

```
Add this to your gear list.

<img src="/uploads/db1493/original/3X/d/7/d716315e1832bb4edc03b1e29d19dd2c790f0a0c.png" width="500" height="500">
```

---
## \#13 Posted by: Exiledd_Top Posted at: 2017-11-01T20:00:40.684Z Reads: 201

```
The belt and tb mounts are find as long as there caliber 2 trucks your set
```

---
## \#14 Posted by: Regas Posted at: 2017-11-01T20:52:40.009Z Reads: 196

```
Could be a nice addition😉
```

---
## \#15 Posted by: Regas Posted at: 2017-11-01T21:04:17.415Z Reads: 203

```
Ok, lets start over:
I want a dual 6374 setup so I need 218mm trucks (from TB), I then need my motor mount which has to be compatible with the 218mm trucks: (I think these are?) 2x
collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-set-only-black
Will these fit these wheels?
http://www.ollinboardcompany.com/product/abec-11-flywheels-97mm-75a
Then need pulleys:
2x these: will these fit the wheels above?
products/36t-abec-pulley-combo-kit

And you said 2x these: (just wont use TB motor pulley because it doesn’t fit?)
http://www.ollinboardcompany.com/product/16t-htd5-12mm-motor-pulley
```

---
## \#16 Posted by: Exiledd_Top Posted at: 2017-11-01T21:06:38.908Z Reads: 191

```
Is not that it won't fit the motor it just won't fit  anything past 90 mm wheels so that is why you go for ollin motor pulley
```

---
## \#17 Posted by: pennyboard Posted at: 2017-11-01T21:21:41.435Z Reads: 188

```
I have to call BS on this. I have that exact mount and pulley kit and it fits 97mm wheels. The only reason I can see why the pulley wouldn't fit is if you're running really short belts like 240mm in length or something.
```

---
## \#18 Posted by: Regas Posted at: 2017-11-01T21:24:25.511Z Reads: 186

```
@pennyboard So you mean all the parts I said before just without the ollins pulley will work and fit perfectly?
```

---
## \#19 Posted by: Regas Posted at: 2017-11-01T21:28:16.916Z Reads: 189

```
@pennyboard Even this belt will work with the setup above?
collections/pulley-timing-belts/products/265mm-htd5-12mm-belt
```

---
## \#20 Posted by: pennyboard Posted at: 2017-11-01T21:29:28.154Z Reads: 182

```
Let me check what size my belts are when I get home and then I'll be able to let you know for sure.
```

---
## \#21 Posted by: Regas Posted at: 2017-11-01T21:31:08.269Z Reads: 167

```
Yeah because you know, I’m the one asking so got no clue.
```

---
## \#22 Posted by: Michael319 Posted at: 2017-11-01T21:32:03.857Z Reads: 164

```
Good luck getting those 97mm 75a. Those are pretty much the least common wheels you can find. Sold out most places.
```

---
## \#23 Posted by: Regas Posted at: 2017-11-01T21:33:24.660Z Reads: 167

```
We’ll see about that!
```

---
## \#24 Posted by: Michael319 Posted at: 2017-11-01T21:34:19.145Z Reads: 169

```
If you can't get those, I hear clones aren't too bad. And a lot cheaper
```

---
## \#25 Posted by: Regas Posted at: 2017-11-01T21:39:08.638Z Reads: 174

```
Will these bearing fit the Abec 11 wheels above? Or do I have to get Abec 11 bearings?
https://eskating.eu/product/waterproof-abec-9-bearings-enuff-set-of-8/
```

---
## \#26 Posted by: themegak Posted at: 2017-11-01T21:42:41.561Z Reads: 177

```
@JLabs sells those belts for a better price and last i checked, you could still get 97mm 75a flywheels from evolve (although they might be sold out).  I highly recommend those wheels though.  They are magnificent.  Here is a link to the belts.  

https://buildkitboards.com/collections/belts/products/265m-belt
```

---
## \#27 Posted by: WARMAN Posted at: 2017-11-01T21:46:55.771Z Reads: 177

```
Yep that's the one you need and just snip the red wire..or was it the blue.. tick tock⏰🔥...jokes it's the red! Seen too many movies! 
@longhairedboy hahaha what an idea,we could start a new trend,jousting on esk8's,we both pick up speed and scream at the top of our lungs and see who comes out on top! Winner gets those skittles or fruit pastilles!  
<img src="/uploads/db1493/original/3X/7/2/724fcbf9baf9f03d13265433b7dd80e1a3df54d1.jpg" width="601" height="500">
```

---
## \#28 Posted by: Regas Posted at: 2017-11-01T21:47:44.449Z Reads: 158

```
How about the bearings?
```

---
## \#29 Posted by: Michael319 Posted at: 2017-11-01T21:52:16.623Z Reads: 156

```
Skateboard bearings are universal. Although nicer bearings will give you better efficiency
```

---
## \#30 Posted by: Regas Posted at: 2017-11-01T21:55:17.827Z Reads: 163

```
OK is everyone sure for sure that this “kit”
products/36t-abec-pulley-combo-kit
Will fit the Abec 11 97 mm flywheels and the motor pulley will fit TB 6374 motor?
No issues???
```

---
## \#31 Posted by: E1Allen Posted at: 2017-11-01T23:46:34.974Z Reads: 154

```
Motors can handle water fairly well. I crashed a large foam flying wing in a river once. It landed upside down and I could still run the big 11 inch prop in the water. The only thing that didn't work after that was one servo. Everything else was fine.
```

---
## \#32 Posted by: longhairedboy Posted at: 2017-11-02T03:02:50.770Z Reads: 148

```
YESSSSSSSSS this NEEDS TO BE DONE
```

---
## \#33 Posted by: WARMAN Posted at: 2017-11-02T03:43:40.536Z Reads: 152

```
Haha sippin on aberlour 60% whiskey=some crazy idea's!! But I feel like the esk8 idea in general was probably thought of by some bloke kickin back getting wasted on high % whiskey!! 
<img src="/uploads/db1493/original/3X/1/4/140082681f328d741fee34a9a8c2c9c0e0bd1965.jpg" width="409" height="500">
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-11-02T03:44:46.384Z Reads: 140

```
i got a few yuenglings keeping me company.
```

---
## \#35 Posted by: WARMAN Posted at: 2017-11-02T03:48:44.987Z Reads: 140

```
A shot of that and they'd be asleep in no time!
```

---
## \#36 Posted by: Regas Posted at: 2017-11-02T05:35:28.839Z Reads: 135

```
@WARMAN Do you know if post number 30 will work?
```

---
## \#37 Posted by: Regas Posted at: 2017-11-02T05:51:29.162Z Reads: 136

```
OH and are the 218mm tb trucks compatible with these washers? (Correct me if I’m wrong but those are to make sure the bearing doesn’t touch the trucks and the bolt thingy at the end)
```

---
## \#38 Posted by: Regas Posted at: 2017-11-02T05:51:46.618Z Reads: 141

```
https://eskating.eu/product/longboard-washers-10x/
```

---
## \#39 Posted by: scepterr Posted at: 2017-11-02T06:22:26.839Z Reads: 136

```
From first hand experience I can say MBS wheels are not good above 20-25mph, they are very unbalanced and it really starts to show at speed
```

---
## \#40 Posted by: torqueboards Posted at: 2017-11-02T06:50:55.866Z Reads: 140

```
@WARMAN We've since changed out the motor pulleys. We have our old pulleys back again.
```

---
## \#41 Posted by: Regas Posted at: 2017-11-02T07:21:16.289Z Reads: 141

```
Right now only thing left is:
1: circlips:
https://eskating.eu/product/2-x-seeger-for-8mm-shaft/
In the Enertion single motor mount installation hey does put two of these do I need to?
https://www.youtube.com/watch?v=J40FfVTBxVc

Then I need you guys to answer these following questions:
1: is it gonna explode?
2: could you tell me the range and the speed this setup would have?
3: I was looking maybe into another deck that would fit everything but that had a kick tail maybe like the super glider, you know any?
```

---
## \#42 Posted by: torqueboards Posted at: 2017-11-02T07:24:15.100Z Reads: 130

```
You don't need cir-clips. It's an option but you don't need them. That's why there's a hub on the motor pulley to stop any  horizontal movement. We've since removed them from our motors since they limit your options as your setup is otherwise fixed to a specific area/position.
```

---
## \#43 Posted by: Exiledd_Top Posted at: 2017-11-02T08:28:32.686Z Reads: 128

```
the motor mount that he is using TB motor mount is really short,so before you start being rude,i am throwing my experience and troubles.
```

---
## \#44 Posted by: torqueboards Posted at: 2017-11-02T13:38:33.127Z Reads: 128

```
@Exiledd_Top He's most likely using the 16T Motor Pulley with the shorter hub vs the one you have. If your still having issues with it. Send me a PM. You can pay for shipping and I'll send you the newer 16T Motor Pulleys.
```

---
## \#45 Posted by: pennyboard Posted at: 2017-11-02T16:03:03.705Z Reads: 123

```
I'm not trying to be rude. You seem intent that there is no way the torque boards pulley will work and he has to buy the ollin boards one. In my experience, that is not true, as I've had no problems with it. So I'm just trying to make sure that since it's his first build and he doesn't have a lot of experience, that he's not getting thrown false information, or directed to spend more money than he has to.
```

---
## \#46 Posted by: Regas Posted at: 2017-11-02T16:56:24.881Z Reads: 120

```
ALRight calm them horses I’ve already contacted @torqueboards and he has cleared everything up, @Exiledd_Top you have the old motor pulley and @pennyboard has the new, as torqueboards said before you can prob just get a new one if you want. 😃
```

---
## \#47 Posted by: Exiledd_Top Posted at: 2017-11-02T17:03:51.139Z Reads: 118

```
I was unaware I had the "old ones " I check there site never seen a "new one " , I ordered ollin motor pulleys and I haven't had issues am not bashing on TB or anything I have bought everything from them.
```

---
## \#48 Posted by: Regas Posted at: 2017-11-02T18:06:00.727Z Reads: 120

```
Do you guys know any other decks that good fit the battery enclosure and the motor mounts? Does the super glider by earthwing work with this setup?
```

---
## \#49 Posted by: Regas Posted at: 2017-11-02T20:10:13.195Z Reads: 127

```
Dammmm son! Where’d you find this? Looks great but pricey as hell! I wonder if this beauty’ll have the space to put everything down there?😍
https://boardsbay.com.au/products/arbor-backlash-37-longboard-complete
```

---
## \#50 Posted by: Regas Posted at: 2017-11-03T09:40:09.461Z Reads: 121

```
Do you guys know any waterproof epoxy or silicone type glue for motor wires, enclosures... etc?
```

---
## \#51 Posted by: moadymoad Posted at: 2018-02-04T11:34:53.488Z Reads: 96

```
How’d your build end up? Looking at putting something similar together
```

---
