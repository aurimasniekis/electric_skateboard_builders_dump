# New FOC ESC on the market?

### Replies: 29 Views: 3758

## \#1 Posted by: NAF Posted at: 2017-05-24T13:05:38.095Z Reads: 333

```
While I was browsing Alibaba today I've found this:   
Seems like WINBOARD is making their own ESC now. Looks pretty good.

<img src="/uploads/db1493/original/3X/2/d/2ddf0acaecc5fc534df0464fc59f1d4bfb4f886b.png" width="690" height="326">
<img src="/uploads/db1493/original/3X/8/c/8cfef88fce9d658a0b92d065f180c3d40e73f09b.png" width="474" height="416">


<img src="/uploads/db1493/original/3X/8/a/8a30579e23a99a40929c053fe10b593f82ba2800.png" width="605" height="362">
<img src="/uploads/db1493/original/3X/0/e/0e0229cbae835b9d827f1201da17ce565c6d6614.png" width="247" height="168">
<img src="/uploads/db1493/original/3X/8/e/8eb8d7fc7a57241879e930290c47aa65218e92e8.png" width="690" height="457">

This is what they claim on their Alibaba page:

What WINboard FOC skateboard features?
1) Generate full torque at zero speed, low energy with high performance, increase efficiency by 5%-8% than any other skateboards
2) Longer riding distance at single charge and extended battery life
3) Electric current is relatively low, less than 9A
4) Quiet motor without any noise makes your skateboard with higher efficiency
5) Easy to install and fits any skateboards, say goodbye to bulky wires if make your own skateboard.
6) We have more than 10 years in this field is the guarantee for your satisfaction.

What is the difference between VESC and FOC?
FOC genertate highest torque at the beginning speed with very low rmp, electric current is ver low, less than 9A, extending battery life and longer riding distance. What is more, quiet motor without any noise and heating problem. In this way, skateboard efficiency dramaticlly increased by 5%-8% than any other motor controller. However, VESC gets highest torque in a relatively higher speed, electric current much larger than FOC, which would do harm to skateboard battery and lower the performance and efficiency.<img src="/uploads/db1493/original/3X/9/e/9e4d70d5f75a40dad0db79f1fbaf7c7a3d5343b8.png" width="690" height="376">
```

---
## \#2 Posted by: NAF Posted at: 2017-05-24T13:06:52.011Z Reads: 318

```
Again ...wondering if anyone had it in hands ?
```

---
## \#3 Posted by: Okami Posted at: 2017-05-24T14:06:26.230Z Reads: 309

```
Check Lou (Loi?) skateboards.. some claim they have super tight ties with Winboards.

Looks good from case perspective and Foc ability. Otherwise I dont see any other data .. amps./volts, would be great, if you could share these if you can.
```

---
## \#4 Posted by: NAF Posted at: 2017-05-24T14:40:36.077Z Reads: 307

```
Yeah. I've read the LOU topic..for now it seems like the guys from LOU built there own deck and used Winboards components for the rest. 

At the end this FOC ESC is really interesting but at the end it all comes down to the software ..how would we configure anything ?
```

---
## \#5 Posted by: Michael319 Posted at: 2017-05-24T14:45:40.160Z Reads: 290

```
Did they give a Price?
```

---
## \#6 Posted by: NAF Posted at: 2017-05-24T14:46:26.925Z Reads: 285

```
No I havn't seen the price anywhere..we would probably have to approach them on their Aliababa page.
```

---
## \#7 Posted by: NAF Posted at: 2017-05-24T14:53:46.899Z Reads: 282

```
Guys I'll try to contact them tonight and we will see how it goes.
```

---
## \#8 Posted by: mmaner Posted at: 2017-05-24T15:52:15.882Z Reads: 268

```
You guys should look at this thread, it appears to be the same controller.

https://www.electric-skateboard.builders/t/can-someone-verify-this/20382
```

---
## \#9 Posted by: NAF Posted at: 2017-05-24T16:12:09.837Z Reads: 258

```
What makes you think it's the same  controller ? There is not even a single word about FOC in that link. It seems like a different one to me.
```

---
## \#10 Posted by: mmaner Posted at: 2017-05-24T16:13:59.141Z Reads: 249

```
Sorry wrong thread.  Long day, lack of sleep and 4 kids...all I got :slight_smile:
```

---
## \#11 Posted by: NAF Posted at: 2017-05-24T16:22:24.337Z Reads: 239

```
Little VIDEO about that FOC Esc. 
Anyone knows this guy ??? :slight_smile: 
https://www.youtube.com/watch?v=GTexIZ_k8aE
```

---
## \#12 Posted by: Sean555 Posted at: 2017-05-24T17:06:10.947Z Reads: 234

```
I recently purchased their gt-m2 containing the same FOC controller.   It is dead quiet!  I have converted any of my soft boards to FOC so I don't really know how'd it compare.  Acceleration and braking are very linear, smooth.   I've only taken it out on a 2 mile flat run so it's hard to give any real review yet.

My guess is that this will be the same motor controller on the LOU boards. And the same hub motors on their 2.0 and 3.0
```

---
## \#13 Posted by: NAF Posted at: 2017-05-24T17:10:19.026Z Reads: 224

```
Great to hear that ! Seems like we might have something interesting here.
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2017-05-24T17:14:08.084Z Reads: 222

```
Hummm.... Isn't FOC (field oriented control) also a option on the VESC... I'm not sure but I think they try to refer to BLDC and not VESC... Can there ESC work in sesorsless, because what make the VESC "The VESC" is the algorithm behind sesorsless BLDC and FOC... I not sure they really know what can be done with a VESC.
```

---
## \#15 Posted by: Blasto Posted at: 2017-05-24T17:16:19.387Z Reads: 223

```
Marketing wanks got it wrong

<img src="/uploads/db1493/original/3X/3/b/3bf5bb4f9ff26eb9491caf0114ab5121ec625ae4.png" width="591" height="336">
```

---
## \#16 Posted by: evoheyax Posted at: 2017-05-24T17:22:19.813Z Reads: 222

```
[quote="NAF, post:1, topic:23802"]
3) Electric current is relatively low, less than 9A
[/quote]

What does this mean? You can only put 9 battery amps through this? If that's the case, then we have a fraction of the amp limit of the current 4th gen vescs.

Interesting and I know theres others working on their own FOC esc's, so we'll have to see where things go in the near future.

[quote="Blasto, post:15, topic:23802, full:true"]
Marketing wanks got it wrong
[/quote]

What, you haven't heard of rmp? It's the new rpm!!!! lol
```

---
## \#17 Posted by: longhairedboy Posted at: 2017-05-24T17:29:07.657Z Reads: 213

```
That's revolu mer pinute, which from Ancient Aramaic translates to Holy Fuck Units. As you can see from this chart, the VESC clearly has more Holy Fucks than the FOC at 1000 MAX N.M which is also Ancient Aramaic for Shit Pants, a unit of acceleration. At 1000 Shit Pants you're experiencing far more Holy Fucks on the VESC.
```

---
## \#18 Posted by: NAF Posted at: 2017-05-24T17:32:44.405Z Reads: 211

```
Come on Guys ..they did their best to sound like "scientific mambo jambo":)
```

---
## \#19 Posted by: Tomer Posted at: 2017-05-24T18:22:04.654Z Reads: 202

```
Maytech released as well a new ESC with FOC functionality featuring an ON/OFF anti-spark switch. 
[Link to Aliexpress](https://www.aliexpress.com/item/Maytech-skateboard-esc-FOC-Controller-electro-skateboard-sensor-dual-ESC-60A-10s/32810049612.html?ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10068_10136_10137_10157_10060_10138_10155_10062_10156_437_10154_10056_10055_10054_10059_303_100031_10099_9915_10103_10102_10096_10147_10052_10053_10107_10050_10142_10051_10172_10084_10083_10080_10082_10081_10110_519_10111_10112_10113_10114_10037_10183_10182_10185_10032_10078_10079_10077_10073_10123_142-9915,searchweb201603_4,ppcSwitch_2&btsid=206e261f-bcd6-4e45-89e0-66a5dbfdc211&algo_expid=956b6298-10c5-41ea-b2e6-3e5ed2e98cb0-1&algo_pvid=956b6298-10c5-41ea-b2e6-3e5ed2e98cb0).
```

---
## \#20 Posted by: Davey Posted at: 2017-05-24T18:59:58.629Z Reads: 197

```
This is a whack price! 100 bucks for DUAL ESC, with  On/Off switch and foc compability?
```

---
## \#21 Posted by: evoheyax Posted at: 2017-05-24T19:05:07.062Z Reads: 190

```
Anyone have experience with it?

That looks really promising if it can do what it claims... slightly more amps than the VESC 4.12, a smaller footprint, and half of the price, with an on/off switch...
```

---
## \#22 Posted by: Tomer Posted at: 2017-05-24T19:21:54.000Z Reads: 190

```
Yeah, I know! Must be a dream.
```

---
## \#23 Posted by: longhairedboy Posted at: 2017-05-24T19:33:07.438Z Reads: 187

```
hmmm... budget board possibilities... i might have to request a sample.
```

---
## \#24 Posted by: voy2k Posted at: 2017-05-24T20:55:13.966Z Reads: 175

```
Sean555! I've been looking everywhere for real-world information about this board (I spend a lot of time over on the Electric Skateboarding sub-Reddit and lurk a lot on this builders forum. Side note: You folks are much more civil and kind than those on the esk8 sub-Reddit).

I got a quote for about $450 shipped to Southern California for the GT-M2 and have come very close to pulling the trigger. I've hesitated because there's seems to be zero information about the M2 in 'the wild'.

PLEASE let us know how it's working for you when you get a chance to use it a bit more. Thanks very much.
```

---
## \#25 Posted by: saul Posted at: 2017-05-24T21:17:08.947Z Reads: 168

```
yea I saw this one a few weeks ago too. but it didn't look like anything special for the price and the numbers seemed a bit too magical.
```

---
## \#26 Posted by: Sean555 Posted at: 2017-05-24T21:35:56.072Z Reads: 167

```
I will post a video and some pics tomorrow.   It is honestly a decent board for the price. They told it was a 10s3p battery but I'll open it up tomorrow to confirm.

Here are some observations so far besides what I stated:

1) they told me the battery could be swapped out but it looks like you'd need to remove some deck screws to gain access.  I'll post pictures  tomorrow
2) Bluetooth app: will not work because they said they the 2.4 GHz receiver causes interference.  I call B.S. on this, might be because of LOU
3.) Board they sent me had "Radley" hub covers instead of winboard covers. 
4.) Remote: it has 2 modes fast and slow.   It is a thumb throttle but if you push it all the way up or down it will sort of lock in place.  I guess it's like a cruise control, but will only let you cruise at Max.   To reverse, simple press down on thumb throttle once and it's in reverse mode.
4)Top speed: they said 35 kmh.  According to Strava it reached that once in my 2 mile trip, only for a second and this is in flat pavement.   They later told me being 180lbs to only expect 30kmh.
```

---
## \#27 Posted by: voy2k Posted at: 2017-05-24T21:41:54.242Z Reads: 165

```
Very much appreciate this Sean. I'm a casual, recreational rider (on mostly flat ground), so unless you find some serious red flags, I'll probably take a flyer on this board. Look forward to further feedback and thanks again for your willingness to share.
```

---
## \#28 Posted by: lox897 Posted at: 2017-05-24T21:43:50.258Z Reads: 164

```
I was on public transport and I still laughed so hard at this. Never stop your jokes Damon!
```

---
## \#29 Posted by: voy2k Posted at: 2017-05-30T01:03:21.918Z Reads: 136

```
Hey Sean555- Have you had a chance to ride your Winboard GT-M2 any more? I'd love to get your further thoughts on this board when you have a chance. If it's behaving for you, I'll probably pick one up.
```

---
