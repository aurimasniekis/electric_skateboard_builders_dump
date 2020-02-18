# Disappointing torque and speed

### Replies: 70 Views: 4244

## \#1 Posted by: sprocket12 Posted at: 2016-08-15T01:37:22.302Z Reads: 434

```
Hi guys. Just finishing up my build. Had a few test rides. I have:

Turning sk3-6354 motor 260kv
8s3p (hodgepodge of free 18650 batteries)
Entertion VESC fw 2.18
Sparkless 120a on/off switch
Torqueboards mini 2.4 Ghz remote controller
Enertion trucks and pulley
83mm wheels

The problem is I can't get the torque everyone talks about, nor the top end. I can get up to about 15 mph. This seems very low. One calculator said I should get up to 33 mph (no load). With load, I should be north of 25 mph. 

I'll post my VESC settings when I can, but anything I should zoom in on?  I'd like to enjoy it without investing more $$$ at this time. 

I know the batteries could be questionable. If I replace them, what should I consider for about 10-12 mile range in an 8s set up?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-08-15T01:41:19.153Z Reads: 402

```
What is your gearing?
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-08-15T01:42:30.674Z Reads: 397

```
Also http://calc.esk8.it
Calculate estimated speed
```

---
## \#4 Posted by: JLabs Posted at: 2016-08-15T01:42:51.100Z Reads: 395

```
You should all ready be around the 10 mile mark with the 8s3p. I'm sure the torque has to do with either the battery no supplying enough amps or some VESC settings are wrong.
```

---
## \#5 Posted by: chaka Posted at: 2016-08-15T01:48:32.037Z Reads: 387

```
Yeah 8s3p is not going to get you enough power. Figure you are going to get a max of 5 amps per cell,  at 8s3p that is less than 500 watts.
```

---
## \#6 Posted by: JLabs Posted at: 2016-08-15T01:51:46.269Z Reads: 381

```
I kinda semi disagree I'm running a 6s lipo and I got more than enough torque. Don't get me wrong it's not a smooth start but I can go up some long steep hills. 

But I'm sure you know a bit more about eboads then me.. just my opinion

Edit: unless lipo's are different then liion
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-08-15T01:52:02.041Z Reads: 356

```
Maybe switching to lipos would be the easy way to go or add to the current pack
```

---
## \#8 Posted by: chaka Posted at: 2016-08-15T01:53:47.838Z Reads: 354

```
Sounds like OP is using recycled li-ion 18650's, do you have any experience with these?
```

---
## \#9 Posted by: JLabs Posted at: 2016-08-15T01:54:42.338Z Reads: 342

```
I have only used lipo so far. I think the batteries 'life' has expired, not the 8s part
```

---
## \#10 Posted by: Blasto Posted at: 2016-08-15T01:56:42.973Z Reads: 338

```
[quote="sprocket12, post:1, topic:7648"]
8s3p (hodgepodge of free 18650 batteries)
[/quote]

Think the root cuase is right here
```

---
## \#11 Posted by: chaka Posted at: 2016-08-15T01:57:28.036Z Reads: 333

```
Well even fresh 5amp max cells will feel sluggish at 8s3p.....8s10p is a completely different story. :grin:
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-15T01:58:25.427Z Reads: 324

```
chaka is saying that the 18650's have way too low of a discharge rate because they're most likely laptop batteries. Low discharge rate leads to underwhelming wattage.
```

---
## \#13 Posted by: JLabs Posted at: 2016-08-15T01:59:13.937Z Reads: 321

```
Okay, I'll say your right. You have more experience, I was just providing another opinion. 

Edit: I didn't know there was any difference between lipo and liion, with the discharge! Learn something new everyday.
```

---
## \#14 Posted by: sprocket12 Posted at: 2016-08-15T02:01:18.123Z Reads: 318

```
I wanted to provide a complete picture with full disclosure. That's why I mentioned the mix of li-ion batteries. However, the same lot supplied batteries to a different custom 6s2p using an RC ESC. It is torquey and faaaast. 

When I can, I'll post BLDC tools screens. I'm hoping some adjustments can help.
```

---
## \#15 Posted by: sprocket12 Posted at: 2016-08-15T02:05:16.107Z Reads: 298

```
If I do replace the batteries, any suggestions on a lipo for the same 8s set up?  I've invested in a 33.6 charger and understand my motor can't go to 10s due to high kv?
```

---
## \#16 Posted by: JLabs Posted at: 2016-08-15T02:08:24.243Z Reads: 285

```
2x 4s lipo in series.
```

---
## \#17 Posted by: sprocket12 Posted at: 2016-08-15T02:19:18.381Z Reads: 296

```
Here are my current VESC settings

<img src="/uploads/db1493/original/2X/8/8ee2a8881d4cf55132dc9b2e574263fc323f649d.png" width="690" height="364">
<img src="/uploads/db1493/original/2X/6/6026c9c4b786bf0791402e88613fcf3e7b371d7d.png" width="690" height="364">
<img src="/uploads/db1493/original/2X/9/9a900940b15c63684281f7123a914a7d5b28397d.png" width="690" height="364">
```

---
## \#18 Posted by: sprocket12 Posted at: 2016-08-15T02:41:43.943Z Reads: 264

```
What about mAh?  5000, 8000, 10,000?  How about two of these?

ZIPPY Flightmax 8000mAh 4S1P 30C
http://www.hobbyking.com/hobbyking/store/__16226__ZIPPY_Flightmax_8000mAh_4S1P_30C.html
```

---
## \#19 Posted by: JLabs Posted at: 2016-08-15T02:54:55.321Z Reads: 267

```
The more the mAh the more the range, but also the more the price. They would work! I would have some VESC experts look at ur settings. Also if u go with the batteries don't forget a balance charger.
```

---
## \#20 Posted by: Blasto Posted at: 2016-08-15T04:01:28.063Z Reads: 255

```
Also crank up your maximum input voltage to 53V
```

---
## \#21 Posted by: sprocket12 Posted at: 2016-08-15T04:08:33.439Z Reads: 247

```
For my current VESC/batteries or the Zippy's if/when I go that route?
```

---
## \#22 Posted by: Blasto Posted at: 2016-08-15T04:10:34.167Z Reads: 240

```
for both. this just means your vesc will shutdown if more than 53V is applied (regen braking)
```

---
## \#23 Posted by: sprocket12 Posted at: 2016-08-15T04:14:15.240Z Reads: 237

```
Hey thanks. I'll do it. Any thoughts as to why I'm getting such a slow ride with the posted VESC settings?  Each pack is showing about 90% charged with 33+V.
```

---
## \#24 Posted by: Blasto Posted at: 2016-08-15T04:23:18.045Z Reads: 234

```
when your vesc is connected, on the app tab ppm config, do you see the display bar do it's full swing (hit the max and min of the bar)

could be a mechanical issue where your belt is to tight, or my last guess is your batteries are not able to output enough current
```

---
## \#25 Posted by: Hummie Posted at: 2016-08-15T04:28:12.567Z Reads: 231

```
Recycled li-ion.  Do you know which?  They likely have a one or two amp ability.  Do they get warm?  Bet that's what sucks.   They're probably toasted from what you've  done so far. Get some cheap lipo and youll be flying
```

---
## \#26 Posted by: sprocket12 Posted at: 2016-08-15T04:29:34.783Z Reads: 228

```
Ok. The ppm setting allows a full 0-100 on live remote. The belt has a little play. 

Last thing left .... Batteries 😩
```

---
## \#27 Posted by: Hummie Posted at: 2016-08-15T04:32:08.871Z Reads: 230

```
3p and recycled laptop cells.  Definatey.  Even if they were new.
It's good news.  You can get lipos cheaply
```

---
## \#28 Posted by: sprocket12 Posted at: 2016-08-15T04:55:15.973Z Reads: 225

```
Sooooo... @JLabs says 4s x 2 lipo. What is 'cheap'? And what mAh for a 10-12 mile range?
```

---
## \#29 Posted by: Hummie Posted at: 2016-08-15T04:58:33.676Z Reads: 230

```
I don't know the math for ur 260kv motor and the max erpm but I think u might be able to go 12s and just limit the erpm.  That way u can keep the vesc cooler and the battery happier. I'd figure if that's possible first. 
  There are so many different batteries u could get.  Just assume everything is half its stated c rating.

I get 20 real miles on 8ah and 12s.  Not sure what nominal voltage is 12a but I like to call it 50v..so 400watthours.   That's like 200watthours to 10 miles

Cheap is hobbyking
```

---
## \#30 Posted by: Namasaki Posted at: 2016-08-15T08:09:46.517Z Reads: 215

```
[quote="JLabs, post:19, topic:7648"]
The more the mAh the more the range, but also the more the price.
[/quote]


The more the mah the more the range but also the current capability.
8000mah x 30c=240a discharge rate.
```

---
## \#31 Posted by: laurnts Posted at: 2016-08-15T08:17:43.369Z Reads: 216

```
Idk if you guys noticed, the first battery was li ion and not lipo cells. So that was an obvious no power when its only 8S3P as 3 parallels li ion could only discharge max around 30A constant which is very poor.

But its good that Chaka noticed it I suppose. Get high discharge / setup more parallels / more capacity and you're good to go.
```

---
## \#32 Posted by: Namasaki Posted at: 2016-08-15T08:42:49.377Z Reads: 215

```
according to that calculator, I'm only getting 70% efficiency on my new setup
10s 190kv 15/36 pulleys 90mm wheels
21mph top speed
my Lipo setup was only 60% efficient according to the calc.
12s 230kv 16/36 pulleys 90mm wheels
28mph top speed
Wondering if the vesc will improve this situation.
```

---
## \#33 Posted by: sprocket12 Posted at: 2016-08-15T16:17:38.434Z Reads: 203

```
Really?  This replacement Samsung in an 8s would be closer to what? 60A in 3p?

Specs per battery:

Chemistry:  INR
Max Continuous Discharging Current: 20A
Max Pulse current (less than one second pulse):  100A
Typical Capacity: 2500mAh
Style:  Flat top
Dimensions: 64.85 ± 0.15 mm (L) x 18.33 ± 0.07mm (D) 
Weight: 43-45g
Discharge cut-off voltage: 2.5V
Voltage: 3.6V
Full Charge Voltage: 4.2V ± 0.05V
Origin:  South Korea
```

---
## \#34 Posted by: laurnts Posted at: 2016-08-15T16:35:23.649Z Reads: 190

```
20A you think this constant as a constant? Not sure. You at least about 4p to get a nice torque start. Its easy to tell the difference between high amps setup compared to low amps setup. If your maths is right, eboard shouldnt pull more than 10-20A if you are gentle with throttle. Try to do 2p if that would make a difference, pretty sure it will dissapoint you.

The thing is that these motors on eboard could pull alot of amps although the amount of amps required are not so much. However the more "ready" amps you can deliver, it just burst all the way. General conception of electricity is that you can't never have too much amps. Your load decides.
```

---
## \#35 Posted by: Titoxd10001 Posted at: 2016-08-15T16:50:10.222Z Reads: 183

```
For what is worth I'm getting 27mph on full charge 9s lipo. Torqueboards 230kv (they are actually 190-200kv chaka said) 15/36 gearing with 90mm abecs. I also tried 12s but limited the erpm to 60,000 (can reach 67,000) and got 31mph, but should achieve around 36 on full charge.
```

---
## \#36 Posted by: Namasaki Posted at: 2016-08-15T16:55:15.925Z Reads: 180

```
Don't forget rider weight is a huge factor
```

---
## \#37 Posted by: chaka Posted at: 2016-08-15T16:55:46.509Z Reads: 181

```
I am about 195lbs and I can pull around 2000 watts on a powerful system accelerating from zero. 

2000/8s-28.8v=70amps

If you want this kind of power from common 18650's then you need at least 7 cells in parrallel, even at this size it will lack punch due to excessive voltage sag. In my experience common laptop grade cells will burst to 10 amps for short periods but high discharge 20amp cells will give you much more punch due to the lower resistance when only asked to output 10amps per cell.
```

---
## \#38 Posted by: Titoxd10001 Posted at: 2016-08-15T17:00:12.472Z Reads: 182

```
I'm 210lbs and am only using one 6355 till i get my dual going. I'm scared to go faster because the "turbo" kicks in at 29+mph and it caught me off guard last time
```

---
## \#39 Posted by: Namasaki Posted at: 2016-08-15T17:17:35.775Z Reads: 172

```
I'm 190 and with 2 TB 6355 230kv and 12s Lipo I got only 28mph
Are you using Vesc?
```

---
## \#40 Posted by: Titoxd10001 Posted at: 2016-08-15T17:20:29.346Z Reads: 172

```
Yes im using a vesc
```

---
## \#41 Posted by: Namasaki Posted at: 2016-08-15T17:23:56.877Z Reads: 166

```
 That gives me hope Because I'm not but I will be soon
```

---
## \#42 Posted by: Titoxd10001 Posted at: 2016-08-15T17:36:15.524Z Reads: 165

```
Something to keep in mind is that the vesc feels like it has a mind of its own. Like I was max throttle going 30mph and I was about to stand up from a tuck motioning thats all you got because I wanted faster. Next thing you know the vesc kicks into to high gear ("turbo") and all my weight gets shifted to my back foot and I almost ate shit but thankfully I didn't. I put my hand on my chest the whole ride because I was so shaken up.
```

---
## \#43 Posted by: chaka Posted at: 2016-08-15T17:39:16.186Z Reads: 157

```
This might be due to mismatched motor and battery max. Could also be due to low voltage management, the vesc will throttle back if the voltage dips and it will come back once the voltage rises again after acceleration. Same goes for temp management.
```

---
## \#44 Posted by: Titoxd10001 Posted at: 2016-08-15T17:44:16.018Z Reads: 155

```
Wouldn't it be the RPM sweet spot where the motor accelerates a little on its own? But i do know I'm to heavy for a single because sometimes it doesn't want to go any faster than around 15mph or climb a slight hill I think I hit the temp start cutoff.
```

---
## \#45 Posted by: chaka Posted at: 2016-08-15T17:46:03.627Z Reads: 157

```
That shouldn't be so apparent as to knock you off the board. I really think it is a result of the various limiting functions within the vesc.
```

---
## \#46 Posted by: sl33py Posted at: 2016-08-15T17:47:05.400Z Reads: 165

```
Batteries for sure.  some of those laptop batteries probably only give 2-5A and starve your ESC of power.  

I have those Zippy 4s 8Ah batteries - run them regularly on GF's single motor Vanguard.  Work great and get good mileage.

Mileage - best way to estimate is to figure out Watt Hours (Wh).  Take your Voltage x Ah = Wh.

So your example Zippy cells - 4s (3.7v nominal = 14.8v) in series (x2) = 29.6v x 8Ah = 236.8Wh.  You should roughly expect 1km per 10Wh.  So approx 23.6km/14.6mi.  On the flats - not racing, and not being a big rider.  All those will decrease range, but it's still a good estimate on paper when planning battery size.
```

---
## \#47 Posted by: Titoxd10001 Posted at: 2016-08-15T17:48:47.084Z Reads: 161

```
The problem was on my end in part because I was going to stand up and at the same time the boost kicked in. I've learned to always stay in tuck when using vesc and going fast.
```

---
## \#48 Posted by: chaka Posted at: 2016-08-15T17:51:14.907Z Reads: 167

```
Another thing that could be happening is the voltage will come back from sagging after accelerating and increase the top speed due to the relationship between kv and voltage.

Edit: More I think about this the more sure i am that this is what is happening. I distinctly remember looking down at my voltage display in a tuck and seeing my voltage rise and feeling the slight boost in top end. 

I would be willing to guess that a pack with more voltage sag would result in a more apparent boost after leveling out at the top speed or cruising speed.
```

---
## \#49 Posted by: Titoxd10001 Posted at: 2016-08-15T18:08:03.525Z Reads: 171

```
I think that sounds about right two of my lipo packs aren't in the greatest condition. I'm going to build a 18650 pack soon.

Is it possible that the vesc went over the set max erpm limit I set in bldc tool?
```

---
## \#50 Posted by: chaka Posted at: 2016-08-15T18:11:44.707Z Reads: 159

```
Multiply your kv by your nominal voltage and if you are under 8600rpm you should be fine. I like a little more buffer for the occasional dh session but it is only a real danger if you release the throttle and let the motor spin freely beyond the maximum voltage/rpm
```

---
## \#51 Posted by: devin Posted at: 2016-08-15T18:14:20.125Z Reads: 164

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#52 Posted by: sprocket12 Posted at: 2016-08-15T18:18:19.258Z Reads: 166

```
The Zippy's have a BMS already in each pack, right?  So what charger do you use?  What is your top speed?  

I'm at a little under 190lbs and my build goals were 10-12 miles (check) and around 25mph top cruising speed (I calculate 24.94mph weighted-- check?).
```

---
## \#53 Posted by: Titoxd10001 Posted at: 2016-08-15T18:46:52.012Z Reads: 168

```
I'm over the suggested limit. I have torqueboards motor that spins theoretically at 67k rpm at 12s which means 190-200kv? There is a bigger risk going downhill? I plan to get vesc v6 when it's available
```

---
## \#54 Posted by: chaka Posted at: 2016-08-15T18:49:07.274Z Reads: 165

```
It can be problematic if you are not careful.
```

---
## \#55 Posted by: sl33py Posted at: 2016-08-15T18:49:20.307Z Reads: 186

```
Nope - no BMS.  You need a regular Lipo charger.  On a budget and want simple - i recommend a iMax B6ACv2 - has AC-DC Power supply inside for one plug simplicity.  If you want ability to charge more than 5 Amps - and don't mind some complexity (or can use for other RC hobbies) - check out the iCharger chargers (206b/306b).  I have the 306b w/ dual dell server power supplies for 24v 1500w.  

To charge multiple batteries - a simple parallel board.  Helps to occasionally charge individually.

Speed is all in the gearing.  Not having her board in front of me, i'm not positive of motor gear, but likely:

83mm wheels - 200kv motor - 8s - 14/36 = 21mph.  She tops out at around 8mph realistically, but i do ride it every once in a while and it moves along fine w/ me on it (265lbs).

I usually gear for 25mph on my builds (single or dual motor).  8-10s usually and love running 97mm wheels for rough roads (or unattended small children).  I gear as low as i can w/ the larger wheels and higher voltage on 190-200kv setups.  Run some gear calculators and you should do fine.  Don't go below 13t on the motor on 9mm belts - it will skip.  I might not go below 14t on a single, or go at least 12mm or 15mm wide belts.

GL!
```

---
## \#56 Posted by: lrdesigns Posted at: 2017-01-13T09:52:36.499Z Reads: 127

```
So @sprocket12 did you get a new battery pack? I would concur and say this is your limitation. The peanut gallery is getting loud in here :stuck_out_tongue_closed_eyes:
```

---
## \#57 Posted by: sprocket12 Posted at: 2017-01-13T13:22:21.697Z Reads: 136

```
Oh yeah! I went with two Zippy 8000 mah 4s1p at 30c. I placed them together to make an 8s1p.  Plenty of torque. Top speed around 27 mph and i get just under 12 real world miles!

Rebuilding now. We are at around 14" snow and in single digit temperature  (F). So i needed something to do. :smile:
```

---
## \#58 Posted by: treenutter Posted at: 2017-01-13T15:33:50.063Z Reads: 140

```
@chaka @devin I keep my ERPM pretty low and my Real-world (and anecdotal) experience has been that if I approach or exceed that limit and apply throttle, I just continue to coast. I can hear VESC engaging but it never presents a "braking" effect if I'm beyond ERPM and apply more throttle. I forget which parameter it is in BLDC Tool, but I believe that this behavior is the default.
```

---
## \#59 Posted by: devin Posted at: 2017-01-13T16:07:19.185Z Reads: 154

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#60 Posted by: Ackmaniac Posted at: 2017-01-13T16:20:20.669Z Reads: 169

```
@treenutter Thats the parameter. When it is disabled then it simply shuts off the VESC. When it is enabled it brakes when it exceeds the MAX ERPM.

<img src="/uploads/db1493/original/3X/d/8/d8597e89281404d31ceccfc4b6f06bd8e7e768b1.png" width="690" height="417">
```

---
## \#61 Posted by: treenutter Posted at: 2017-01-13T16:32:06.060Z Reads: 162

```
@Ackmaniac Ahhh thanks for the reminder. This makes sense to me now... I use FOC mode so I think that this parameter does not engage in the current firmware when in FOC mode. Hence, I haven't experienced negative torque when exceeding the ERPM. I'm sure there are many other variables that apply, as @devin notes above.
```

---
## \#62 Posted by: Ackmaniac Posted at: 2017-01-13T16:58:41.655Z Reads: 164

```
Funny that you mentioned it. I checked the FOC code and i can't find a limitation of the max ERPM. So it seems that the only limitation is the soft ERPM limit from the application. That could be a bit risky if that value is not set and you run the board on the bench with a 200kv motor and a 12S battery. Because then you get above 60000 ERPM. 

So you should make sure that the soft ERPM limit is set in the application to prevent that.
It's also a bit strange that Vedder didn't implement that.
```

---
## \#63 Posted by: DeathCookies Posted at: 2017-01-14T19:55:44.960Z Reads: 156

```
But you could change the 
`App Configuration`  --> `PPM` --> `PID max ERPM` to limit the ERPM to 60k?!
```

---
## \#65 Posted by: Ackmaniac Posted at: 2017-01-15T02:24:06.127Z Reads: 148

```
That would be only for PID speed control. You need to set the App Configuration --> PPM --> Soft RPM Limit --> ERPM limit start and ERPM limit end. But if you run the VESC via the keyboard in BLDC-Tool you could reach higher speeds than 60000 ERPM. 
But it depends on the motors kv and the batterys voltage. With a 190kv motor and a 12S Battery you should be careful. But maybe it also doesn't really hurt the VESC when it is above 60000 ERPM. Who knows?
```

---
## \#66 Posted by: Marijulama Posted at: 2017-07-29T09:56:01.872Z Reads: 108

```
Hello Chaka,

I have made a 8s3p battery pack made from new VTC5 18650 cells. Voltage is 37V fully charged but max speed is 25kmh and it feels really weak.. Range is also not great. Can you think of what went wrong?
```

---
## \#67 Posted by: pat.speed Posted at: 2017-07-29T12:12:06.698Z Reads: 104

```
Well it would seem you have well over charged your batteries the max voltage per cell is 4.2v what you have said suggests you have charged the cells to 4.6v which is way to high
```

---
## \#68 Posted by: chaka Posted at: 2017-07-29T15:05:08.479Z Reads: 101

```
Pat is right, those cells are being over charged at 37v. 

Still, 8s3p is crazy small for an electric skateboard when using 18650 cells. If you want good torque you need a lot of cells. 60 cells seems to be the starting point if you want something that will be powerful throughout the discharge cycle.
```

---
## \#69 Posted by: psychotiller Posted at: 2017-07-29T16:20:44.147Z Reads: 100

```
I get good results with my 8s5p packs, but I use new cells.
```

---
## \#70 Posted by: chaka Posted at: 2017-07-29T16:36:55.568Z Reads: 96

```
Thats a big jump from 8s3p, you will still get a good deal of voltage sag during acceleration or hill climbing. And when our voltage sags we lose power, less watts. The absolute best setup I have tried is a 10s6p with sanyo 20700 cells. Like I have a freight train pushing me.  Hill climbing at speed is where the big packs shine since we are asking for more amps and running around 80 to 90% duty cycle.
```

---
## \#71 Posted by: psychotiller Posted at: 2017-07-29T16:40:21.871Z Reads: 93

```
True! I meant as a minimum for 8s should be 5p.
```

---
