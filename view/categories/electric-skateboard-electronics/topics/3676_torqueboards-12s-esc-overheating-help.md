# Torqueboards 12s esc overheating - Help!

### Replies: 96 Views: 5960

## \#1 Posted by: Mobutusan Posted at: 2016-05-23T06:10:44.043Z Reads: 313

```
So, I finally got my Torqueboards 12s esc setup running, and took a few test runs on 6s and 9s. In both cases, I took laser thermometer readings of the esc heatsink after a few miles, and they were showing 140-165°F, and definitely hot to the touch. On my last and only run on 9s, I must have hit an overheat cutoff twice within 4 miles of flat cruising at 15-20 mph where the board cut power and I could only go around 8-10 mph until I let the esc sit and cool for a while. At first, I thought the heat was caused by a combo of 6s, high amps, and a mostly, but not totally sealed enclosure. But it wasn't until I tried the 9s that the esc actually got so hot, it cut power to the system. Anybody have any thoughts on what may be causing this? My enclosure is definitely not airtight at all, but the esc also doesn't have any active airflow over the heatsinks, but I thought these ran cool enough under normal conditions that it wouldn't really be needed.  Maybe something is wrong with my wiring, but everything works great until the esc starts cooking. Here's some pics and specs of my setup. Please help. Thanks.

Specs/setup
6s battery: 4 x 5200mah 3s 10c Multistar in parallel & series
9s battery: 3 x 4500 mah 3s 35c Zippy Compact in series
Esc: Torqueboards 12s car esc
Esc settings: Timing= high, acceleration= very high, max forward= 100%
Motor: Turnigy sk3 245kv
Gearing & Wheels: 16T/36T & 83mm clones
Remote: Torqueboards mini remote
<img src="/uploads/db1493/original/2X/a/adb2f8e9dcc19356ea91f189540002f7b6130339.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/5/5fca13d3160ca888951afadbea83d13f4851dd74.jpg" width="690" height="388">
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-05-23T06:21:12.507Z Reads: 285

```
Maybe not enough gear reduction for a single setup? Do you own a watt meter to test the current draw?
```

---
## \#3 Posted by: chaka Posted at: 2016-05-23T06:25:41.998Z Reads: 290

```
That belt looks really tight. If it is that will draw a lot of wattage. Try backing the setting down a little, it may help reduce the current.
```

---
## \#4 Posted by: Mobutusan Posted at: 2016-05-23T06:51:21.400Z Reads: 282

```
I think this gearing is what Torqueboards runs, and it's what was recommended to me, at least for 6s.  When I had it running on my TB 6s esc, even with a 17T/36T and 20T/36T setup, it never got so hot that it would cut power, but that one had a fan on it, and I never checked the temp it got to.

I have a watt meter. I suppose I could rig it up somehow on my board so I could see the amp draw under load.
```

---
## \#5 Posted by: Mobutusan Posted at: 2016-05-23T06:56:50.680Z Reads: 269

```
Wow, you can tell just from those pics? It will try loosening it a little. I don't feel like it's too tight, but I'm still not sure what optimal tension feels like either. When I first set it up (too loose, I thought), the belt would skip teeth on hard braking, but it won't now.  Do you have a preferred method for finding proper belt tension?
```

---
## \#6 Posted by: torqueboards Posted at: 2016-05-23T07:22:10.174Z Reads: 258

```
What firmware version are you using?

I run very high, very high for motor timing, motor acceleration.

You shouldn't be overheating. Unless your climbing some steep hills - hill after hill on a single motor.

A tight belt will cause things to overheat as the motor will be overworked.
```

---
## \#7 Posted by: Mobutusan Posted at: 2016-05-23T07:30:44.762Z Reads: 247

```
I'm on v.150818. I had it on very high timing on 6s yesterday, and dropped it to high today, but didn't seem to fix anything. I'm hoping it's just the belt. Like you said, I figured it would take lots of hills to overheat things like this.
```

---
## \#8 Posted by: torqueboards Posted at: 2016-05-23T07:32:56.711Z Reads: 237

```
Try the belt. Let me know.
```

---
## \#9 Posted by: Mobutusan Posted at: 2016-05-23T07:53:54.632Z Reads: 235

```
@torqueboards Will do. Thanks for the help. 

And thanks @chaka and @claudiofiore88 for your help as well. I'm gonna try to hook up my volt meter and get an amp reading before and after I loosen the belt. For science.
```

---
## \#10 Posted by: Mobutusan Posted at: 2016-05-23T19:45:04.664Z Reads: 213

```
@torqueboards & @chaka I'm going to try loosening the belt, but before I do, does this look too tight? By hand, It doesn't feel like it's providing much of any extra resistance compared to just turning the motor alone by hand.
<img src="/uploads/db1493/original/2X/5/55bd60fbc27b8f515d2051955f17c5e06d45f57c.jpg" width="690" height="388">
```

---
## \#11 Posted by: barajabali Posted at: 2016-05-23T19:51:04.020Z Reads: 208

```
Man you're having trouble with that esc like no tomorrow. 

Throw a cpu fan on it
```

---
## \#12 Posted by: CSN Posted at: 2016-05-23T20:13:01.692Z Reads: 203

```
I have been using Metroboards belt tensioning technique that uses sound to determine belt tension with free guitar app.

Anybody have any opinions on it? The belt is relatively taut using this method

http://metro-board.com/maintain/
```

---
## \#13 Posted by: Mobutusan Posted at: 2016-05-23T21:24:32.037Z Reads: 202

```
@barajabali Actually, this wasn't the problem one until now. I might throw a fan on it or duct some cooling air to the heatsink, but I'd like to find out why it's overheating in the first place. I like that it's silent when it's on, so a fan is a last resort for me. 

@CSN I'll check that out. Did you ever take temp measurements when you were running these?
```

---
## \#14 Posted by: Michaelinvegas Posted at: 2016-05-23T21:29:51.628Z Reads: 196

```
@Mobutusan no more buffets for you my man
```

---
## \#15 Posted by: CSN Posted at: 2016-05-23T21:32:59.723Z Reads: 203

```
yeah and ran them in ambient temps up to 115 F. I was able to get the sensored to decrease power when I had it inside the Ollin Flux and there was no ventilation. Once I had some breather holes then it took some serious heat and hill climbing to get any power cut. I would have to ride it for an hour in 100+ and then hammer up a hill.

The non sensored one I only ran on flat ground but it did fine in hot temps. I had that ones heatsink exposed and never had any power cuts.

I would point the heat gun at the heatsink and got readings as high as 150 F. when the pavement was 175 F.  But usually it would be around 125 F.

BTW I am about 150#'s bodyweight.
```

---
## \#16 Posted by: Mobutusan Posted at: 2016-05-23T22:08:37.821Z Reads: 197

```
@Michaelinvegas If I lived in Vegas, that might be a very real problem for me. Lol. But fully loaded, I might be pushing 180 lbs., so I don't think weight is a problem.

@CSN Thanks for the feedback. That gives me a good range of normal temps to expect. There's got to be something wrong with my setup, but if it doesn't end up being the belt, I don't know what else it could be. 

@claudiofiore88 I checked my way meter and it's only rated to 10 amps. Any suggestions for a quick, easy way to measure the amp load or inexpensive watt meter that could handle the current we pull?
```

---
## \#17 Posted by: L3thaltank Posted at: 2016-05-23T22:21:21.716Z Reads: 206

```
Here's a good watt meter.
http://www.ebay.com/itm/New-130A-LCD-G-T-Power-RC-Watt-Meter-Tester-and-Power-Analyzer-High-Precision-/121325011305?hash=item1c3f88c169:g:j84AAOSwMzVTw4hy

this is the one I have. It's the same just different branding.
http://www.ebay.com/itm/G-T-POWER-RC-Watt-Meter-and-Power-Analyzer-High-Precision-130A-60V-GT-Power-/111724087614?hash=item1a0346493e:g:iRgAAOSw3ydVr2N7
```

---
## \#18 Posted by: barajabali Posted at: 2016-05-24T00:56:28.165Z Reads: 204

```
<img src="/uploads/db1493/original/2X/f/f97621096163f5b1088fb26fa073addcba21db32.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/4/4613d56b605fb0d2aa8fad40639bba8636da3148.jpg" width="375" height="500">

Worse comes to worst I have this processor fan and heat sink it'll keep the esc cool as ice
```

---
## \#19 Posted by: Mobutusan Posted at: 2016-05-24T01:44:05.359Z Reads: 195

```
Well, I loosened the belt to the point where I could only brake with about half force before the belt started skipping teeth. Then I did about 10 laps up and down the the street. I live on a culdesac that's about 0.1 miles long. So, I ride a total of about a mile with moderate acceleration and braking. I checked the temperature of the esc heatsink and it was 184 degrees at the hottest point, and around 160-170 degrees everywhere else. The motor windings inside were around 115 degrees, and the batteries were about 85 degrees. I'm gonna try my other 12s esc and see if it still happens, but I need to add a bec to it first.

Any other ideas besides the belt?
```

---
## \#20 Posted by: Namasaki Posted at: 2016-05-24T02:02:58.321Z Reads: 199

```
Set your motor timing to normal and acceleration to medium and the Esc will run cooler.
It will be more snappy power especially at lower speeds.
Mounting it outside the box helps as well allowing more air around it.
Just have to avoid water puddles.
<img src="/uploads/db1493/original/2X/1/10954a39da0182fb4fa5ef05ebdb7f0bc174ec05.jpeg" width="375" height="500">
```

---
## \#21 Posted by: Mobutusan Posted at: 2016-05-27T01:39:46.045Z Reads: 194

```
So, I tried changing my motor timing to normal and acceleration to medium. No luck. Then I drilled about 12 5mm holes on the front and rear of my enclosure to make sure there was some decent airflow, and still the same overheating issue. I can only go about 1-1.5 miles of flat riding before power gets cut due to overheating, and I have to limp along at 10mph. At least it's consistent though. Lol. Each time, the ESC heatsink is between ~160-180*F, the motor windings are ~100-115*F, and the batteries are ~80-85*F. Not sure what's going on here.

For my next trick, I'm going to swap my SK3 245kv motor with my Tacon 160 245kv, and see if that changes anything, but I'm guessing it won't. Then, I'm going to swap my BEC over to my other 12s ESC and see if that one overheats too. I'm running this on 9s, and it's sooo much fun, while it lasts.

Any other suggestions or theories are welcome. :cry:
```

---
## \#22 Posted by: torqueboards Posted at: 2016-05-27T01:49:47.269Z Reads: 191

```
@Mobutusan - Try running at "very high" for motor timing. Let me know how that works.

You can send it back and I can send you a replacement. Let me know.
```

---
## \#23 Posted by: oriol360 Posted at: 2016-05-27T02:07:43.574Z Reads: 193

```
@Mobutusan My ESC's have a heat sink also and I noticed they run much better when the heat sink is exposed to the air. Keeping it inside the case heats them up quite a bit. See if cutting a hole in your case and having the heat sink stick out a bit keeps it cool. you can also hot glue or clear caulk the edges of the cut out to keep water out. 

<img src="/uploads/db1493/original/2X/a/a6778d29f045052d3340d4c1716049a964e9173a.jpg" width="373" height="500">
```

---
## \#24 Posted by: Mobutusan Posted at: 2016-05-27T02:29:49.982Z Reads: 184

```
Thanks for the offer and advice. I'll try that too. And you do know I bought this use from another member, right? Do you accept returns from second owners? (would be awesome if you did, but understand if you don't)
```

---
## \#25 Posted by: torqueboards Posted at: 2016-05-27T02:41:23.279Z Reads: 184

```
I don't normally but we can work something out. Send me an email.
```

---
## \#26 Posted by: thisrealhuman Posted at: 2016-05-27T03:26:16.918Z Reads: 186

```
Your sk3 has a longer can than my 245kv eflite motor, so you probably have more torque than me. My [ESC](http://www.hobbyking.com/hobbyking/store/__62679__TURNIGY_K_Force_120A_HV_OPTO_V2_5_12S_Brushless_ESC_US_Warehouse_.html) is very similar to TB's 12s esc, and my gearing and wheels are almost identical now. I'm using 83mm clones, 15t/36t, 10s. I recently changed my motor pulley from a 12t (25mph) to 15t (31mph) and I've noticed my motor and esc getting hotter along with my breaking torque almost totally gone. I think your heat issue is the same as mine, and the solution is to go higher volts and smaller motor pulley. You'll get higher rpms and have mechanical torque at all speeds, whereas a lower kv motor will move the same load at a lower rpm using electrical torque.

The problem with the 12t pulley is the number of useful teeth, so even though I just said your solution is a smaller pulley, I'm switching to a lower kv to test my understanding.
```

---
## \#27 Posted by: Michaelinvegas Posted at: 2016-05-27T03:48:52.224Z Reads: 181

```
I'm gonna be testing out a new esc at 12s with 149kv....I was considering moving up to 18t from 14t .... Maybe I shouldn't?
```

---
## \#28 Posted by: Mobutusan Posted at: 2016-05-27T04:01:49.592Z Reads: 177

```
Dude, you rock! That is above and beyond. I REALLY appreciate that, but I am going to try everything I can so I don't have to take you up on that. :grin:
```

---
## \#29 Posted by: thisrealhuman Posted at: 2016-05-27T08:02:37.433Z Reads: 173

```
Id stick to 14t till you can feel the limits of your motor. Increasing gearing by 35% is like adding 35% weight, the esc cant tell the difference.
```

---
## \#30 Posted by: Mobutusan Posted at: 2016-05-27T08:11:53.678Z Reads: 168

```
I have a 14T pulley that I can try too, but what's weird is when I was running 6s through it, the esc got pretty warm, but not hot enough to cut power. It was only after jumping up to 9s that I started having problems cutting out. I thought the higher voltage would reduce current and heat, but not the case for some reason. Once I figure out the best way to wire my four 3s multistars with xt60's in series, or find aluminum solder paste to fix my fourth shorted zippy, I'll try out 12s.
```

---
## \#31 Posted by: Mobutusan Posted at: 2016-05-27T08:18:52.123Z Reads: 170

```
On a side note, with my other 6s TB esc running 20/36 gearing with 97mm wheels, I was able to ride at least 3-4 miles or more and never had that esc cut power though it did get pretty warm. I did get pretty hefty voltage sag under load, but top speed was sure fun for 6s.
```

---
## \#32 Posted by: Michaelinvegas Posted at: 2016-05-27T11:52:20.869Z Reads: 163

```
Man I keep looking at the pictures....it's gotta be there's no air circulation and that plastic you have it in stays warm like a blanket...id ride with the lid off for science
```

---
## \#33 Posted by: RogerD Posted at: 2016-05-27T12:34:47.268Z Reads: 161

```
I'm really surprised you get anywhere with an ESC in a sealed box. I'm 90 Kg, and on 6s, with an EZ run pro 150A esc, I can ride fanless (with the esc not in a box or any sort) in the autumn and winter, but get cut outs in the spring/summer. With a fan it runs all year round.

I know higher volts = less amps and heat, but still, an ESC still has to dissipate heat somehow .
```

---
## \#34 Posted by: Mobutusan Posted at: 2016-05-27T18:49:32.421Z Reads: 166

```
Well, before my last attempt yesterday, I had drilled a bunch of holes in my box and still only made it a mile. I'm trying to figure out a good way to mount the esc outside my box to test that way, but with all those holes in the box and going 15-20 mph, I would think it has at least enough air movement to not overheat after a mile of flat riding. Plus, the box is not gasketed, so it's not even close to airtight by any means. Gonna do some more testing this weekend.

<img src="/uploads/db1493/original/2X/8/832b9a463f51880a26189a6b74a977b58f0b3673.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/f/fa40c06a6f31cefd5b87babf0343efdddf82fd41.jpg" width="690" height="388">
```

---
## \#35 Posted by: Michaelinvegas Posted at: 2016-05-27T18:56:04.245Z Reads: 155

```
i don't think those little holes aren't gonna give you the air flow you are looking for..maybe if you cut a door like opening just before the esc on your lid to act like a little air scoop when your riding ...
```

---
## \#36 Posted by: FLATLINEcustoms Posted at: 2016-05-27T19:02:32.605Z Reads: 154

```
Cut a hole big enough for the ESC fins to stick out of the enclosure. Seal the box to the aluminum fins. Fins would then be outside the box and breathing.

Could you ride around with the lid off to see if that is the issue?
```

---
## \#37 Posted by: Mobutusan Posted at: 2016-05-27T19:31:58.103Z Reads: 152

```
I can't remove the lid without ripping it off, and I was trying not to completely hack up my box, but I guess I may have to. 

Does everyone running these esc's have the heatsinks fully exposed to the outside air? Does nobody run these inside enclosures?
```

---
## \#38 Posted by: Michaelinvegas Posted at: 2016-05-27T19:39:56.683Z Reads: 148

```
Like the box cost a lot of money lol
```

---
## \#39 Posted by: Michaelinvegas Posted at: 2016-05-27T19:41:37.281Z Reads: 147

```
I've only seen ESCs with fans enclosed ... I've always seen ESCs with fins or no fan exposed ... Me be its just me
```

---
## \#40 Posted by: Mobutusan Posted at: 2016-05-27T20:06:26.429Z Reads: 149

```
It's not about the money, it's about the time. The box cost me $5, but carefully cutting/melting out all of the dividers with a soldering iron/hot knife without destroying the box was really tedious. Plus, I was all ready to start playing with EL wire to illuminate the box, so destroying it would be a huge waste of time right now. I'll figure something out.
```

---
## \#41 Posted by: Michaelinvegas Posted at: 2016-05-27T20:11:35.215Z Reads: 141

```
Lol I feel you man.... I have to re-configure myself ... And I'm LAZY to do it.....

I say cut a door and let it hang down a little like an air scoop ... I think that's your least invasive and most effective way to push air over the esc without having to take the top off or installing a fan....

Box cutter ... Three cuts (leaving one side attached ) and bend the plastic down and go for a ride a see if it helps...

Edit: it could be a matter of a few degrees separating you from your endless ride
```

---
## \#42 Posted by: Mobutusan Posted at: 2016-05-27T20:48:14.125Z Reads: 141

```
Ok, I'm going to try cutting a scoop hole over the esc to send as much air as I can over the heatsinks. I'll post back if it works. These things might just run a lot hotter than I had expected.
```

---
## \#43 Posted by: Namasaki Posted at: 2016-05-27T22:18:55.937Z Reads: 142

```
oh wait, I just remembered something. check the screws that hold the heat sink on. sometimes they get loose.
```

---
## \#44 Posted by: Namasaki Posted at: 2016-05-27T22:32:38.290Z Reads: 151

```
here's a solution for low cost enclosures that allow quick easy access for swapping or charging Lipos.
There made of abs and are tough. I have had a few crashes with it and no damage.
http://www.serpac.com/s-series.aspx
http://www.mouser.com/_/?Keyword=serpac+enclosures&FS=True
http://www.amazon.com/s/ref=nb_sb_ss_i_5_7?url=search-alias%3Daps&field-keywords=serpac+enclosure&sprefix=serpac+%2Caps%2C189
```

---
## \#45 Posted by: torqueboards Posted at: 2016-05-27T23:33:40.469Z Reads: 152

```
You shouldn't need to keep it open. I keep mine enclosed and it works fine.
```

---
## \#46 Posted by: Michaelinvegas Posted at: 2016-05-27T23:34:47.168Z Reads: 151

```
I think it's buffets and he's not tell us lol
```

---
## \#47 Posted by: lox897 Posted at: 2016-05-27T23:36:02.848Z Reads: 148

```
Same as @torqueboards I run mine in an enclosure. My enclosure has a big hole in the end of the motor side (motor wires come out of that hole) and some air gets in there.
```

---
## \#48 Posted by: Namasaki Posted at: 2016-05-27T23:51:25.689Z Reads: 142

```
I run mine outside and they still get warm with dual belt drive 230kv 16/36 gears when climbing long hills.
With hub motors, they would get down right hot and I even burned one up on those long hills.
Although, it may have shorted out because 2 of the caps had come undone.(wires broke off the the pcb) 
and there was never a temp cut out. The wires from the caps where very light gauge and may have just failed because of vibration. Plus I was running dual and only one esc failed. I disconnected it and rode back up the hill with just one esc/motor.
```

---
## \#49 Posted by: Mobutusan Posted at: 2016-05-28T00:01:51.859Z Reads: 140

```
Thanks for the feedback and link to those enclosures. I'll take a look at those.

And since these were used, I took the screws out, and went over the esc with alcohol and a q-tip to make sure there was no debris interfering with anything. So, I know the heatsink is still stuck well to the circuit board, and the screws are snug. I'll have to do a test run and see if that changes anything.
```

---
## \#50 Posted by: Mobutusan Posted at: 2016-05-28T00:08:08.415Z Reads: 142

```
@torqueboards & @lox897 
Thanks for posting this. I thought I could get away with enclosing the esc without issue, especially if I'm just cruising on flat ground. With or without airflow though, getting the esc heatsink up to 170-180*F after only a mile of riding while the motor and batteries are barely warm doesn't seem right to me.
```

---
## \#51 Posted by: Mobutusan Posted at: 2016-05-28T00:27:28.884Z Reads: 131

```
On a side note, and this might be a dumb question, but what do I need to connect two of your 12s esc's or two of your 6s esc's together to run a dual setup?
```

---
## \#52 Posted by: Namasaki Posted at: 2016-05-28T03:31:08.143Z Reads: 137

```
All you need is a Y-connector for the signal wires to the receiver and another Y-connector for the power wires.
```

---
## \#53 Posted by: Mobutusan Posted at: 2016-05-28T03:59:57.921Z Reads: 139

```
I assume you can find those on hobby king or something? I'm looking now, but they're not jumping out at me.
```

---
## \#54 Posted by: torqueboards Posted at: 2016-05-28T04:14:34.148Z Reads: 142

```
https://www.motionrc.com/products/100mm-4-servo-y-extension-cable?gclid=CJqLxeDz-8wCFUVsfgodj3YEJA

It's just a Y Servo Connector.

If you use dual 6S, you want to remove one red wire from one of the ESCs. You can then just heatshrink it to the side of the wire folded.

<img src="/uploads/db1493/original/2X/6/65ddf729be8c9096708099e6024902d120b269b3.png" width="690" height="460">
```

---
## \#55 Posted by: Mobutusan Posted at: 2016-05-28T06:20:33.472Z Reads: 139

```
@torqueboards Thanks for the link. I'll have to get a couple of these. I can't even find these connectors on Hobby King, and I thought they had everything. 

Do you have to cut the red wire when running dual 6s only? Is that cause each esc supplies is own power to the receiver?
```

---
## \#56 Posted by: RogerD Posted at: 2016-05-30T18:41:09.200Z Reads: 134

```
That's a misleading statement. How hot the ESC gets depends on rider weight, ambient temperature, speed ridden, hills. Saying it doesn't need air is too generic. His might.

The last two boards I've built (one a 10s VESC board) both had problems until actively cooled.
```

---
## \#57 Posted by: torqueboards Posted at: 2016-05-30T18:57:12.626Z Reads: 135

```
@Mobutusan You would only need to cut it on one of the 6S ESCs and not both. If you cut it on both there won't be any power going to the receiver.

Did you ever get that heating issue resolved?

@RogerD This was meant for the TorqueBoards 12S ESC and I haven't needed to keep it out in the open although it's always better too.
```

---
## \#58 Posted by: Mobutusan Posted at: 2016-05-30T21:14:05.515Z Reads: 136

```
Thanks Dexter. I got a couple y connectors coming, so I'll make sure to do this.

On the overheating front, I'm perplexed as to why these are running so hot. I tried swapping out my sk3 245kv with my Tacon 245kv, and still had it overheat, although I did manage to get almost 2 miles this time before it cut power. Then I tried the other sensored one, and that one overheated too in about 1.3 miles. Also, on the non-sensored that I've been running this whole time, I can easily get up to 25mph without topping out, but when I swapped the sensored one in, it topped out at 19-20mph. I'm gonna check the settings, but I thought they were both set up identically on the same firmware. I'm not sure what the issue is or if I'm doing something wrong, but this is frustrating. I think the only other thing left for me to try is to add a fan or cut open a scoop to directly cool the esc. For 170lbs. on 9s, with a moderately loose belt, on flat ground, I'd like to think I could go more than 1-2 miles without the esc hitting 170-180°F and cutting out, enclosed or not.
```

---
## \#59 Posted by: Michaelinvegas Posted at: 2016-05-30T22:12:21.071Z Reads: 135

```
Somethings janky with that esc ..... Gremlins
```

---
## \#60 Posted by: Namasaki Posted at: 2016-05-31T06:03:45.663Z Reads: 135

```
http://www.electric-skateboard.builders/t/how-you-burn-up-ur-esc-or-motor-going-slowly-and-despite-seeing-few-amps-from-the-battery/4008
```

---
## \#61 Posted by: torqueboards Posted at: 2016-05-31T19:39:55.164Z Reads: 124

```
@Mobutusan - Just FYI. The person who sold you those mentioned he had no heat issues. So it could be an issue with your setup.
```

---
## \#62 Posted by: Mobutusan Posted at: 2016-05-31T21:52:53.213Z Reads: 127

```
@torqueboards After testing the second, sensored esc, and still having the overheating issue, I'd have to agree. I just can't figure out what else could be left to check that's causing the problem. I've changed programming, loosened the belt, swapped motors, swapped esc's, checked all connections, checked tightness of wheels/bearings, drilled holes in my enclosure for airflow. The only thing that's stayed the same are the board, 9s batteries, mini remote, and BEC. 

Out of curiosity, what are your normal operating temp for these esc's measured at the heatsink, (in an enclosure, I assume)?

Could the batteries (9s, 4500mah, 35c) or the BEC possibly be the problem? Seems unlikely to me, but I'm running out of things to try besides mounting the esc's completely outside of the box.
```

---
## \#63 Posted by: Mobutusan Posted at: 2016-05-31T22:07:39.119Z Reads: 126

```
Hey, I didn't get a chance to read your replies in that thread before I responded here, but great job with testing! That gives me some hope for fixing my issues, and figuring out my setup for these esc's.
```

---
## \#64 Posted by: Namasaki Posted at: 2016-05-31T22:54:31.282Z Reads: 122

```
It may be possible that the internal resistance of that motor is high. Did you try a different motor yet?
```

---
## \#65 Posted by: Mobutusan Posted at: 2016-05-31T23:26:59.986Z Reads: 124

```
I did try a 245kv sk3 and 245kv Tacon, with similar results. Maybe the kv rating is part of the problem?
```

---
## \#66 Posted by: torqueboards Posted at: 2016-06-03T05:01:11.091Z Reads: 121

```
Are you running high timing?

If your up for it send it to me and when I get time I'll swap it and run it for 10 minutes or so.
```

---
## \#67 Posted by: Mobutusan Posted at: 2016-06-03T05:14:01.852Z Reads: 119

```
@torqueboards I've run the timing high, very high and normal with the same results. I appreciate the offer to take a look, but I think there is something wrong with my setup since I got similar overheating with both the sensored and unsensored versions. After reading @Namasaki's test results from that other thread, I'm thinking that maybe the combo of 9s voltage, 16/36 gearing, and single 6364 motor is pulling too much amps.
```

---
## \#68 Posted by: Michaelinvegas Posted at: 2016-06-03T05:30:38.702Z Reads: 116

```
Did you switch up gearing?

Edit: meaning where you using different gearing in the past? Like a 12T?
```

---
## \#69 Posted by: Mobutusan Posted at: 2016-06-03T05:51:40.118Z Reads: 110

```
So far, I've only tried 16/36 on 6s and 9s with the 12s ESC. Originally, I didn't think there would be a problem with that setup, but I am gonna try 14/36 on 9s this weekend and try to run as close to full throttle for as long as I can, ~22-24mph, and see what happens.
```

---
## \#70 Posted by: Namasaki Posted at: 2016-06-03T05:59:16.888Z Reads: 108

```
Bro, I don't think the problem is your voltage or gearing. 
I did part of my road test with dual 6355 230kv. 6s, 16/36 gears and 90mm wheels and went full throttle up some hills and nothing got hot. I'm begining to suspect that this particular brand of esc does not like sk3 motors. My hub motors where similar to sk3 motors and the TB esc's did not like them at all. They got hot all the time and I even burned one up climbing long hills. it could have something to do with the gauge wire they use for windings.
or something about them, I don't know. 
I'm using TB 6355 motors now and running them hard with no overheating problems at all either at 6s or 12s
```

---
## \#71 Posted by: Michaelinvegas Posted at: 2016-06-03T06:06:16.500Z Reads: 108

```
Could he be getting some type of feed back into the esc some how??? 

I'm not even sure if possible or if something like that could happen...
```

---
## \#72 Posted by: Mobutusan Posted at: 2016-06-03T06:35:51.081Z Reads: 111

```
Did you try single drive? The guy I got these esc's from was about my size running the following setups and only had overheating occur on the sensored unit on hills in hot temps.

5060 TB motor 200 kv (non sensored)
R-Spec 6350 190kv (sensored)
8s ~29 volts 20c (non sensored)
80 18650's 8 x 10s with BMS (sensored)
97mm
16/44
```

---
## \#73 Posted by: torqueboards Posted at: 2016-06-03T07:06:48.231Z Reads: 113

```
It's not an SK3 issue. My first motors were Sk3's. They ran cool Sk3 50s and Sk3 63s.

The sensored if not connected properly will cause heat and may possibly fail.

Sk3s I got nearly 3k+ miles easy. Those motors are still working I just don't use that setup anymore.
```

---
## \#74 Posted by: Namasaki Posted at: 2016-06-03T07:09:19.190Z Reads: 114

```
What do you think his problem is?
```

---
## \#75 Posted by: Mobutusan Posted at: 2016-06-11T16:54:07.577Z Reads: 119

```
I just picked up one of those watt meters, but I'm curious as to how you have yours set up. Since these units don't log data, I'd like to be able to view the unit while I ride. I know it will show max and min values, but I'm curious to see what the instantaneous current draw, voltage sag, and power consumption are while I'm accelerating, cruising, etc. 

My thought was to mount the unit on top of the deck at the front truck, and run 10 gauge wire to the battery and ESC from the unit which would be ~ 12-18" of wire for the source and load side of unit. I know we are supposed to keep the battery leads as short as possible, and the unit comes with about 3" of 12 gauge wire on either side, but for testing purposes, would running a 2-3' loop of cable from the battery through the watt meter, and back to the ESC cause significant issues with performance, resistance, or accuracy of readings?

https://www.amazon.com/Tenergy-Precision-Meter-Analyzer-Backlight/dp/B017YCTRKK?ie=UTF8&*Version*=1&*entries*=0
```

---
## \#76 Posted by: psychotiller Posted at: 2016-06-11T17:08:12.206Z Reads: 117

```
I think his board is just pissed he's using that lunchbox instead of one of these:
<img src="/uploads/db1493/original/2X/c/c2fea17916f0be44097dedca2ca3db365cd9ab4d.jpg" width="690" height="389">
```

---
## \#77 Posted by: psychotiller Posted at: 2016-06-11T17:12:03.396Z Reads: 114

```
Seriously though, you should take Torque up on his offer. You probably just have an issue in that ESC.
```

---
## \#78 Posted by: Mobutusan Posted at: 2016-06-11T17:12:41.799Z Reads: 113

```
Don't "gloss" over my problem, bro. A pretty box can solve a lot of problems in life, but not all of them. :laughing:

Btw, it's on my list, along with a lot of other things...
```

---
## \#79 Posted by: Mobutusan Posted at: 2016-06-11T17:16:36.363Z Reads: 113

```
Well, I might still, but I also have a second, sensored unit that I have only tested once, but got the same results. If I see a difference between those units after more testing, I'll probably go for it. I definitely don't want to abuse TB's privelage/offer without exhausting all other possibilites on my end first. Just wish I had more free time in life to do all this testing. I'm lucky to find time to get out once or twice a weekend and run through a single battery before life calls me back. Oy.
```

---
## \#80 Posted by: Mobutusan Posted at: 2016-06-11T17:21:38.601Z Reads: 117

```
Oh yeah, and small update. Last weekend, after my normal 1-1.5 mile ride ending in a power cut/overheat situation, I changed from a 16/36 to 14/36 gearing, and was able to go almost 3 miles before I got a rock stuck in my motor pulley, and ran out of time, so that's promising. The ESC was still up around 150*F at its hottest point, but got me much farther without overheating/cutting power. 

Also, running at 80% forward limit with the programming card seemed to do nothing for my overheat situation. Pretty much same results.
```

---
## \#81 Posted by: psychotiller Posted at: 2016-06-11T17:30:50.369Z Reads: 117

```
More aerodynamic, less drag, less heat. Just saying lol
```

---
## \#82 Posted by: c4Lvin Posted at: 2016-06-17T17:47:18.891Z Reads: 106

```
how long (mm) is your belt? Also I always wondered why people run their motor wires right below the motor area? If you are doing a tight turn with some normal or semi-loose trucks, it will rub on those wires. I shifted mine because original owner had done the same thing and I see rub marks on the wires. If you don't remove them (assuming you run tight trucks) they will short out soon I believe.
```

---
## \#83 Posted by: monkey32 Posted at: 2016-09-11T16:07:14.798Z Reads: 90

```
My torqueboard 12s just started doing the overheat thing too......gets stupidly hot and the motor does too. Just switched all my components over to a new board, went outside to try and got the death beep after less than a km......did a bench test with a towl burn for resistance and both the motor temp and esc temp skyrocketed. really weird. it's pretty warm here in Madrid Spain but i didn't think it was that warn mid 80's.

Im a heavier dude, 95 kg, running 90mm wheels, 6355 enertion motor, 7s battery and 15mm 36t x 15t belt and pully

Any thoughts gentlemen?

 Might try to change my ESC to a VESC this weekend see if that will fix it.
```

---
## \#84 Posted by: torqueboards Posted at: 2016-09-12T03:14:24.183Z Reads: 87

```
@monkey32 Do you have a 12S SBEC model?
```

---
## \#85 Posted by: Pantologist Posted at: 2016-09-12T03:54:50.318Z Reads: 89

```
I've got overheating issues as well. I run at a higher voltage (38.4) Around 10S. I'm using 83mm wheels, an SK3 190kv 6364 motor and 15T 36T gearing. My belt is not overly tight either. It just just tighter than letting the belt slip during heavy braking. 

I was thinking about changing the heatsink. I have the OPTO version.
```

---
## \#86 Posted by: monkey32 Posted at: 2016-09-12T21:24:33.432Z Reads: 82

```
Yes, the older 12s with sbec. Any thoughts? Worked like a charm last year and a half.
```

---
## \#87 Posted by: Pantologist Posted at: 2016-09-12T21:44:07.995Z Reads: 84

```
Might be the thermal paste between the heatsink and PCB in your case? I've heard that stuff wears out after being hot a lot.

But mine is new still.

EDIT: I tried riding today when it was 60 degrees out and it still overheated....
```

---
## \#88 Posted by: relaxnfly Posted at: 2016-09-13T02:59:27.183Z Reads: 85

```
I'm also having an overheating problem on two different set ups using the TB 12s w/ SBEC.  I just think it is the 90+ degree temps Im riding in.  I can ride hard for about 4 miles before The esc cuts the power due to overheating.  I will also add that I am using two different Pychotiller enclosures.  They look great but there is little/ no air flow or space for air in the box.  I am planning on creating some ventilation holes in the enclosure above where the esc is mounted.  I think this will solve the problem and I'll post my finding as soon as I can.
```

---
## \#89 Posted by: relaxnfly Posted at: 2016-09-13T03:04:19.481Z Reads: 85

```
The enclosures look so good, I hate having to cut into them for ventilation.  
<img src="/uploads/db1493/original/3X/6/9/6997f8e39a715a3cbc0ee3cc03bbb575a1d9a920.jpeg" width="666" height="500">g
```

---
## \#90 Posted by: Pantologist Posted at: 2016-09-13T03:38:06.083Z Reads: 83

```
Yeah, wouldn't look as beautiful anymore ;(

Barajabali said changing timing to normal should fix overheating issues. I'll post my findings soon.
```

---
## \#91 Posted by: Pantologist Posted at: 2016-09-14T02:38:26.670Z Reads: 83

```
After setting motor timing to "Normal" and acceleration to Medium, my ESC overheated only after 4 miles. Before it was every mile. 

I am 180lb and using a single Sk3 190kv 6364 with 15t/36t gearing. It was only around 65 degrees F outside and I was not going full speed most of the time.
```

---
## \#92 Posted by: relaxnfly Posted at: 2016-09-17T01:49:30.554Z Reads: 77

```
Added some air vents and test rode my board tonight.  It definitely helped cool things down.   I rode hard for 6.6 miles and the last .6 was a long steep hill.  It overheated at the top so I had to take a break and then rode it 2 more miles home.  I added 2 larger air entry holes on the side of the enclosure and several air exit holes right above my the ESC.  The temp was about 85degrees F. I'm running a sks6364 230kv motor with. 16/36 gearing on 83m wheels.  My current ESC setting are soft acceleration, high motor timing so I still have some room to play around with those.<img src="/uploads/db1493/original/3X/5/a/5a2c804479935d7c1ec959e5fb3e5a5366411b82.jpeg" width="557" height="500">
```

---
## \#93 Posted by: torqueboards Posted at: 2016-09-17T02:14:03.959Z Reads: 76

```
Hey guys,

The 12S TB ESC's that are SBEC are having heating issues. We've switched back to the 12S TB OPTO's with the external UBEC's like before.

If you still have an SBEC we might be able to exchange them for you. Just send us an email.

Thanks!
```

---
## \#94 Posted by: relaxnfly Posted at: 2016-09-17T03:14:07.953Z Reads: 77

```
How can I tell if I have an SBEC or UBEC?
```

---
## \#95 Posted by: torqueboards Posted at: 2016-09-17T16:22:03.381Z Reads: 70

```
SBEC will have one wire. OPTO will have 2x 2pin wires.
```

---
## \#96 Posted by: bmiklozek Posted at: 2016-09-19T01:28:49.549Z Reads: 64

```
Off subject and new to the site no don't know how to pm but I can not go to your website. I am hit with popups every time I try. I bought stuff from you earlier this year but now I can't get back to your website to buy more. Thanks.
```

---
