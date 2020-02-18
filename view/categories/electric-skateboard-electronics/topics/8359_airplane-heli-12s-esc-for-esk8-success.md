# Airplane/Heli 12S ESC for ESK8 - Success

### Replies: 49 Views: 5139

## \#1 Posted by: rmkao Posted at: 2016-08-26T06:06:18.844Z Reads: 443

```
*This is going to be a fairly short write up as this is still in testing phases.*

My first build has yet to come to life, as I'm waiting for parts to arrive. I luckily live about 30min from the US West distribution center for Hobby King. I was able to go pickup basically all of my electronics. I took a risk ordering some components I wasn't sure were going to work together properly for ESK8. In the mean time, I decided to get soldering and test a bit.

I've seen the idea kicked around about using boat ESCs in ESK8 setups. It seems as though a few guys on YouTube have had some success. They're a cheap solution for 6S capability, most have proper inputs for throttle, brake, and reverse, therefor ready to be used with a car TX/RX. Now, 6S is pretty meh, and for a few bucks more you can get a 6S car ESC such as the FVT, that's been proven to be a budget ESC solution for ESK8 usage.

Most of us want more than 6S. Only and handful of options are out there to safely and reliably power ESK8's with 8, 10, and 12S battery setups. VESC is known to be the "BEST" solution out there, but unfortunately has gained a somewhat bad reputation of frying due to user error. It's a fantastic system built from the ground up with ESK8 in mind, however in not necessarily a plug-in-play solution. Not only this, but it comes with a pretty hefty price tag as well. Other companies such as Torque Boards, Alien Power Systems, etc.. Have developed up to 12S capable car style ESCs. However, again come with a nice price tag.

I personally wanted to truly build a budget board, with at least 8S capability, and the safety and reliability of at least a car ESC. With a heavy background in competitive surface RC, short course, buggy, truck, you name it, I decided I could probably make a plane/heli ESC fit the bill. They're spec'd well. VERY well. A HV (5S-12S) air ESC will run you in the range of $80-120. 

I went with this, Turnigy K-Force 120a OPTO ESC:
http://www.hobbyking.com/hobbyking/store/__38782__TURNIGY_K_Force_120A_HV_OPTO_V2_5_12S_Brushless_ESC.html?strSearch=k-force
<img src="/uploads/db1493/original/2X/3/38007895be9d13bf382be96185b0e0fcd3b3324c.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/7/7f1edfbde7faeb588fa0005fb6ba5fb5c2b3d6e6.jpg" width="375" height="500">

Notice how similar this ESC looks to Torque Boards 12S ESC. The description in fact is almost identical. I suspect they share the same OEM, however TB has reflashed the ESC possibly? I digress.

I got the ESC all wired up, a BEC was needed as the ESC does not have one. First test, turn everything on, motor starts spinning up to what seems to be half throttle. This was the problem I was expecting. The ESCs end-points out of the box for planes and helis, are drastically far off from a surface TX. Not only this, but these ESC's also do not have input for braking from the transmitter. It does offer a programable "brake" which is basically a drag brake, ranging from soft, normal, to hard.

A surface radio's "bottom throttle point" is in the middle where the trigger rests, "top throttle point" is fully depressed toward the grip, and "brake/reverse point" is forward with the trigger. With no brake reverse endpoint to be set in the ESC, I had to crack into the radio housing to change the throw of the trigger assembly.

<img src="/uploads/db1493/original/2X/2/2650e48ec06b6e3271f02fffe86b1c66bca750cf.JPG" width="375" height="500">

I already repositioned the spring prior to this photo, it was originally connected vertically behind the trigger just in front of that phillips head screw. Above the keyed shaft the trigger slides onto is a retaining bumper. This piece allows the trigger to sit neutral in the middle, and have resistance when the trigger is moved backwards or forwards. Removing this bumper allowed the trigger free range of movement. A reposition of the spring, and we now have a linear throttle throw from top to bottom.

<img src="/uploads/db1493/original/2X/9/951942a15a1698564d60db93e30b10efb381f66f.JPG" width="375" height="500">

Power on the ESC and rescale the throttle top and bottom endpoints, and boom. We have a perfectly functioning high voltage ESC, aside from a proper trigger actuated brake. I will be doing testing to see how the drag break performs, or somehow find a way to potentially reflash the firmware and add a brake/reverse input. 

<img src="/uploads/db1493/original/2X/2/29ebc387249b2920a4bbfd86a65154c546d3f5cb.JPG" width="666" height="500">

Overall, success. 12S capability for $120, no complicated programming setup or risk for toasting the board like a VESC.  THIS IS NOT A VESC ALTERNATIVE. It still does not have the features VESC offers especially for ESK8, but hey its cheap and simple.
```

---
## \#2 Posted by: Namasaki Posted at: 2016-08-26T06:30:09.674Z Reads: 386

```
Seems like a lot of trouble to save $25. 
And the Torqueboards esc has proper brakes
```

---
## \#3 Posted by: rmkao Posted at: 2016-08-26T06:50:43.685Z Reads: 382

```
In my case, the *$35* savings was worth it. ($10 shipping), also I got it faster than next day shipping (my benefit I realize). The moral of this story is however, there are options out there for 12s for well below what I paid. Only reason I went with this particular one was it was all the US West warehouse had in stock. Plenty for $100< that will function exactly like what I've found.
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-08-26T06:54:23.612Z Reads: 365

```
And don't forget.....for science 🤓
```

---
## \#5 Posted by: rmkao Posted at: 2016-08-26T06:58:11.944Z Reads: 345

```
MY GOD WE'VE DONE IT!!!!:tired_face:
```

---
## \#6 Posted by: Namasaki Posted at: 2016-08-26T07:00:26.262Z Reads: 334

```
I think it's fortunate for you that they were out of the cheaper ones because it's very doubtful that they would hold up under the high current demands of esk8.
I just sincerely hope that you don't find yourself  in a situation where you end up wishing you had spent the extra $35 for brakes.
```

---
## \#7 Posted by: rmkao Posted at: 2016-08-26T07:04:27.261Z Reads: 318

```
Who knows! I'm not horribly worried about the brakes, I'm almost positive the drag break system will work fine. Also this was more or less purposed to be a temp ESC while I wait for my damn Enertion VESC. Yes I know... Should've got one from Chaka. Oh well.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-08-26T07:13:57.550Z Reads: 315

```
Well, once you've tried the Vesc you are gonna be spoiled!
When it does arrive and before you power it up, open the shrink wrap and lift the red power wire and trim the pins sticking through the pcb from the socket on the top side. 
People have had there vescs blow from the wire shorting on those pins. Then power up with a 3s Lipo or 12v battery or power supply and update the firmware to fix a current ramp bug. Then use the low power to do initial settings and motor detection. And you should have no problems.
```

---
## \#9 Posted by: rmkao Posted at: 2016-08-26T07:18:31.941Z Reads: 294

```
I'm going to put down some solid miles with this ESC to get a feel for it, the switch to the VESC. See how much difference I can feel! It will then either become a spare, or I'll move it on to someone for cheap.
I appreciate the tips there, I'll make sure to do those. Luckily I have a few 3S packs lying around, perfect for testing.
```

---
## \#10 Posted by: torqueboards Posted at: 2016-08-26T07:19:53.930Z Reads: 279

```
Drag brake sucks.. That means you can't coast lol.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-08-26T07:23:02.967Z Reads: 269

```
Trust me, the difference between the Vesc and other Esc's is beyond huge.  Like night and day.
```

---
## \#12 Posted by: rmkao Posted at: 2016-08-26T07:23:10.824Z Reads: 272

```
Damn true. Well I'll have to see if I can crack the firmware and develop something to implement a break. Also quick note, my order of the mount kit is on hold with you guys? WAZ GOIN ON :sweat:
```

---
## \#13 Posted by: kaziupir Posted at: 2016-08-26T09:15:04.957Z Reads: 262

```
I have done the same after buying hifei160A-KII-12S esc, but eventually it sucks. The drag brake was frying the esc, so I had to turn it off. Without brakes it's too dangerous so I've ordered vesc this week.
```

---
## \#14 Posted by: rmkao Posted at: 2016-08-26T09:49:33.386Z Reads: 270

```
i'm in the process of flashing the firmware to basically make the ESC behave like a car ESC. Proper brakes and all. Hopefully within the next few days I can get it dialed. Need a USB adapter which I'm picking up tomorrow morning from the hobbyking warehouse.
```

---
## \#15 Posted by: thisrealhuman Posted at: 2016-08-26T15:54:34.667Z Reads: 257

```
I've got about 5k miles on K-force 120A's. I hope you get that firmware working, it's a really solid esc and deserves more options. The drag brake isn't bad at all, and doesn't actually kick in until the throttle is back to bottom, so you can let off the trigger almost all the way and coast down to 1% throttle. 
I can't find your kv, but I can tell you that the drag brake is useless if you are geared too low.

Nice work with the gt2b, I think I'm going to try that.
```

---
## \#16 Posted by: treenutter Posted at: 2016-08-26T16:04:30.729Z Reads: 248

```
@rmkao I admire your ingenuity; but agree with @Namasaki that usable brakes are a very essential feature on an esk8. Please be really careful when you test out this build. Wear all the protective gear you've got and stay out of traffic. We want you intact so we can see your progress!
```

---
## \#17 Posted by: barajabali Posted at: 2016-08-26T16:42:37.739Z Reads: 240

```
You're late to the party
```

---
## \#18 Posted by: rmkao Posted at: 2016-08-26T20:20:30.639Z Reads: 237

```
This build is going to be utilizing a 245kv SK3, Geared 16/36, 8S. It's a fast setup, not a lot of torque, but I'm an extremely light rider and no big hills in my area. I'll do extensive testing prior to taking it to the streets to ensure safety.

I'll keep you all updated on the firmware, and do a write-up when I nail something down.
```

---
## \#19 Posted by: rmkao Posted at: 2016-08-26T20:21:33.981Z Reads: 238

```
Whatttttt :sweat: Dang I was just trying hang with the cool kids
```

---
## \#20 Posted by: barajabali Posted at: 2016-08-26T20:27:22.612Z Reads: 230

```
haha but im happy you found success!
```

---
## \#21 Posted by: lowGuido Posted at: 2016-08-26T20:55:46.431Z Reads: 223

```
brakes are overrated.
My first build had no brakes at all, no drag brake either.

have none of you guys ever ridden skateboards? they don't come with brakes but there are plenty of ways to stop them.

I admit that its pretty handy having a bit of brake here and there but I still rely on me more than my brakes.
```

---
## \#22 Posted by: Pantologist Posted at: 2016-08-26T21:05:25.920Z Reads: 212

```
Yeah I also don't get it. I guess if you are going 25mph+ all the time, you will need em. 

If I was going that fast all the time, I wouldn't trust the motor for braking.... maybe some 1/5 scale Baja HPI brakes would be better.
```

---
## \#23 Posted by: torqueboards Posted at: 2016-08-27T00:14:43.398Z Reads: 200

```
They do look similar to the ESCs we sell but different manufacturers end up copying other manufacturers as well.

I've had quite a few customers who have bought it and tried but they said no luck and/or didn't let me know afterwards.

If you can fix the firmware that would be awesome for everyone :slight_smile: 

@rmkao - PM me your order #. Most orders have been sent out. Let me know.
```

---
## \#24 Posted by: rmkao Posted at: 2016-08-27T01:31:01.234Z Reads: 195

```
I think I may have found the way to go about flashing the ESC. Utilizing a Arduino Uno board as a USB programming device, a slight modification to the ESC itself, I should be able to flash the ESC with a more customizable firmware developed by SimonK. I've found his firmware already has the ability for "throttle and reverse; RC car functionality" whether or not this will enable braking as well I'm still researching. 

Once I can fully develop this concept and get testing done I'll write up a tutorial along with compatible  high voltage plane/heli ESC's.

Checked my order again last night, 5 minutes after I mentioned it, it changed to shipped. Thanks @torqueboards :blush:
```

---
## \#25 Posted by: mattdig Posted at: 2016-08-27T02:36:28.973Z Reads: 194

```
I've had a 6S Heli ESC on my board for the last year. I made the exact same mod to my controller and it works fine. Not having an adjustable brake is annoying but I found a good setting (60% brake) that slows me quickly without throwing me off the board. Not being able to coast is the worst part.
```

---
## \#26 Posted by: thisrealhuman Posted at: 2016-08-27T03:17:05.219Z Reads: 197

```
[My build](http://www.electric-skateboard.builders/t/sector-9-look-at-me-lacey-single-245kv-10s-k-force-post-build-thread/2275/15) had 245kv and 12t/36t, and the soft brake worked well with 77mm wheels, but switching to 15t motor pulley made the brakes totally useless on hard. Your SK3 has a longer can and thus more potential torque, but I'm running 10s, and I can almost guarantee that a **16t on 245kv with 8s will not have enough brake force** even if you get the firmware flashed.
Currently, I'm using 190kv (rspec) with 15T and my brakes are slightly better than the original because i have a wider belt and more teeth to grip, and the torque on this motor is impressive to say the least. Your  top speed will be nice, but you will need plenty of room to slow down, so please be careful and consider a smaller gear!
```

---
## \#27 Posted by: mattdig Posted at: 2016-09-03T19:37:03.765Z Reads: 185

```
I'm at 17/36t on a 245 SK3 6364 and it has a LOT of braking force, so it depends on the motor and the rider's weight. I also have 90mm wheels.
```

---
## \#28 Posted by: OleksiiF Posted at: 2016-09-06T17:30:13.610Z Reads: 182

```
Hi! is there any news, did you succeeded in flashing your esc?
im interested because i bought this esc and i had no idea that it cant brake and dont have start mode "no move")
```

---
## \#29 Posted by: geohan Posted at: 2016-10-15T21:30:53.929Z Reads: 150

```
@rmkao Did you make any progress with this ECS?
```

---
## \#30 Posted by: Pantologist Posted at: 2016-10-15T22:14:46.197Z Reads: 153

```
There is no point in buying this ESC. Just get TB's 12S car ESC or a vesc... Trust me. Not worth the Hassel.
```

---
## \#31 Posted by: geohan Posted at: 2016-10-15T22:24:06.464Z Reads: 150

```
does tb ship to uk?
```

---
## \#32 Posted by: rtasca Posted at: 2016-10-16T19:11:38.266Z Reads: 148

```
You should give BLHeli firmware a try too. I have a homebuilt scooter with an 80A blueseries ESC ( in fact 2 stacked 40A )  and it gave me much better results, there is much more parameters you can adjust and even put in some regen ( damped light ), unfortunately the blueseries does not support this feature.   Using 6s and i am 100+ Kg. and it takes the punishment really well. With all that said, I DID buy a VESC to give it a try since it looks to be the norm around here and I NEED  brakes :slight_smile:
```

---
## \#33 Posted by: mclightning Posted at: 2016-12-25T14:26:33.911Z Reads: 132

```
How did you stack 2 x 40A blueseries ESC to get 80A?

I want to do that. But I cant find any instructions on it.
```

---
## \#34 Posted by: qtron Posted at: 2016-12-25T15:07:09.950Z Reads: 135

```
this is basically the same esc that fvt sell. try downloading the software from this link.
Car and E_SkateBoard PC setup software_150606 

http://www.szfvt.com/en/download-25-5-6-6.html

plug your esc in then if you get the software version pop into the window you should be able to progrm the brake.
```

---
## \#35 Posted by: torqueboards Posted at: 2016-12-28T03:28:36.223Z Reads: 124

```
@Geohan - Yes, we ship to UK.
```

---
## \#36 Posted by: rtasca Posted at: 2016-12-28T12:53:56.496Z Reads: 120

```
they have holes that you can put pin  headers between them in a stack. solder to both sides and you are good to go. In fact, many of the bigger escs are stacks of lesser current ones. 

<img src="/uploads/db1493/original/3X/4/b/4bfd8b66bc442fdfad6d79d64b5d09a8f63de047.jpg" width="690" height="401">
```

---
## \#37 Posted by: mclightning Posted at: 2016-12-28T13:06:40.848Z Reads: 117

```
Are there any instructions online somewhere about this?
I couldn't find anything. When I google stacking escs, only thing that come up is ; how to physically place them next to each other, not power combining.

So this syncs ESCs to work together?
```

---
## \#38 Posted by: mclightning Posted at: 2016-12-28T13:18:31.780Z Reads: 116

```
Can you share a link to any big ESC that is combination of smaller ones like that?
```

---
## \#39 Posted by: mclightning Posted at: 2016-12-28T13:33:07.249Z Reads: 115

```
For example, the post here suggests it will end up killing one of the ESCs due to target voltage difference.
https://www.rcgroups.com/forums/showthread.php?2233888-SBEC-s-connected-in-parallel
```

---
## \#40 Posted by: rtasca Posted at: 2016-12-28T14:32:04.080Z Reads: 115

```
I will take mine apart and send you some pictures.
```

---
## \#41 Posted by: rtasca Posted at: 2016-12-29T13:59:03.533Z Reads: 116

```
OK, there is a catch, you have to remove the drivers from all but one board: 


My esc:
<img src="/uploads/db1493/original/3X/0/d/0d3ffa6caa1775dc670a8241d9cdb3c8f814be26.jpeg" width="375" height="500">

Red Brick.

<img src="/uploads/db1493/original/3X/8/e/8efbefa5b2d1f7af127ba68bdeb244c324909481.jpg" width="375" height="500">
```

---
## \#42 Posted by: Kaly Posted at: 2016-12-29T14:53:18.588Z Reads: 110

```
I hope that does not cause any problems. 
The space in between is so narrow that I think the FETS in the middle can't get proper heat dissipation. 
Keep us posted on this please. 

In regards to the ESC I have had great success with the FVT 12S for close to 2 years now. They just need to run in 10S -12S, to keep the Amps in the 50-60 range and install 50 x 50 mm high speed fans 8-12 V to help with the heat dissipation and you should be riding with no problems at all.
```

---
## \#43 Posted by: telnoi Posted at: 2017-08-20T10:18:37.644Z Reads: 93

```
So, has this worked out for anyone? Contemplating buying these due to EU stock.
```

---
## \#44 Posted by: vap Posted at: 2017-08-21T12:58:54.709Z Reads: 90

```
Here's an interesting ESC
http://rctimer.com/product-1757.html
```

---
## \#45 Posted by: OleksiiF Posted at: 2017-08-21T21:19:39.649Z Reads: 85

```
not a good idea at all. 
i have one, and a had to buy a VESC, because its Super dangerous to use airplane esc. trust me
```

---
## \#46 Posted by: telnoi Posted at: 2017-08-22T04:28:33.559Z Reads: 84

```
Bought some VESCs yesterday. They were cheaper than these, so no more reason to consider them for my first build.
```

---
## \#47 Posted by: Cobber Posted at: 2017-08-22T07:34:09.132Z Reads: 79

```
I have a couple of airplane/heli esc's for [my current build](https://www.electric-skateboard.builders/t/the-bat-mobile-trampa-hs11-e-toxx-driven-duel-scorpion-sii-5535-160kv-90a-135a-scorpion-commander-14s-59v-opto-escs-duel-yge-typ-9-cap-banks-graphene-12s2p-65c-130c-gt2b-mad-munkey/28482), no brakes but I don't need them and I spoke to the manufacturer and they are happy to warranty me both the motors and esc's so happy days :grin: the esc is rated to 14s but I'm only going to run 12s. The guy I spoke to said they will be bullet proof with the motors I purchased.
```

---
## \#48 Posted by: slick Posted at: 2018-05-23T16:34:19.147Z Reads: 57

```
I just smoked one of these. Thankfully it happened while I was going really slow (walking speed). Dunno what caused it to fall but I have a suspicionson.
```

---
## \#49 Posted by: BrokeAF Posted at: 2018-07-17T14:01:06.300Z Reads: 34

```
I know this is an old post, but you can pick up an 80A plane ESC from hobbyking for around 35$. Runs 6s (which is what im going with) and is relatiely low profile. I have yet to make my first eSk8 but I'm ordering the parts soon (I'll be using a 70A ESC I picked up earlier for 20$-ish).
```

---
