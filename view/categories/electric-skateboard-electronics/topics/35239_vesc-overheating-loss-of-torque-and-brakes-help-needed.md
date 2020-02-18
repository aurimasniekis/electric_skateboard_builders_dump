# VESC overheating loss of Torque and Brakes ***HELP NEEDED***

### Replies: 52 Views: 1642

## \#1 Posted by: Mattmccrary8 Posted at: 2017-10-10T13:25:54.469Z Reads: 177

```
Ok so I have a posted a couple times about this problem and really want to get to shredding. My board drops all Torque and brakes after about a mile to 2 miles. I can rip around @ 25-31mph and brake easily but then once I hit about a half mile it starts declining and then by a mile or 2 I can’t even get up to 20 mph. I previously ran 10s 5000mah lipos and series and would get 4+ miles @ 25 before losing power I figure the huge pack would give me more speed (which it has but only for a short time ) then a shit ton more distance.

TB 6374 190kv motor 
TB 12s4p
TB VESC 4.12 
16/36 with 12mm belt
Running 97mm wheels but also have 90 and 83mm 
Nano 2.4 ghz remote 

Is there anything wrong in my settings? 

All I want to do is coast around the flat streets around 25-30mph for 10+ miles which the motor, VESC and battery should all handle. I do know I’m pushing the erpm limit 

<img src="/uploads/db1493/original/3X/c/2/c23778bf040a81936873f2c1ced0015e7667f5b3.jpeg" width="667" height="500"><img src="/uploads/db1493/original/3X/3/4/347a3bc4b7d6673aaecb57370054e9d7cd0fc2b8.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/9/498b5a5f8bd0133857e2efa28134613a6542724c.jpeg" width="666" height="500">
```

---
## \#2 Posted by: Mattmccrary8 Posted at: 2017-10-10T14:22:35.652Z Reads: 148

```
Does anyone know what the problem could be or what I can do
```

---
## \#3 Posted by: cody00 Posted at: 2017-10-10T14:29:26.837Z Reads: 154

```
I'm not an expert by any means, but I have had similar issues recently.  Started off with heat issues and moved on to battery issues.

I cut windows out of the clear shrink on the VESC around the Mosfets
I drilled holes in my enclosure (yes no longer waterproof)
I ordered a heatsink package off of ebay for about $2
--I'm not sure which of these helped but I definitely do not have heat issues anymore.

After this, I ordered a $10 HM-10 LP Bluetooth module.  In my mind, this is the easiest solution to debugging these issues and was well worth the $10.  It let me see that by VESC was cutting out because of extreme voltage sag which I could not see otherwise.  It also gives you live temperature readings.  

Example Screenshot: 
<img src="/uploads/db1493/original/3X/a/5/a51ae31d08f4e2da5d0faa8d09fd4a92935074b5.jpeg" width="281" height="499">
```

---
## \#4 Posted by: Mattmccrary8 Posted at: 2017-10-10T14:50:12.972Z Reads: 137

```
Ya I’m thinking it has to be heat but when I touch my motor it isn’t burning hot. I mean it is very warm but not sizzilin. What setup were you running? Are my amps to high
```

---
## \#5 Posted by: cody00 Posted at: 2017-10-10T15:10:29.103Z Reads: 135

```


I had 10S3P Li-ion 18650.  with 36/16 100mm wheels.  In the process of going 40/16.  

I **dont** think your Batt/Motor Amps are too your high with single and 12s4p

The motor heat is different than the VESC heat as well. I have never experience motor heat with my twin 6355 (or even when I run single).  I imagine you would experience MOSFET temp limit before MOTOR temp limit  -  All from my very limited experience

One of my VESC completely burned at about the same time yours was shutting down.  It was after doing 25-30mph for a few miles - Trying to resolve my own similar problems :slight_smile:

Bluetooth module was well worth the money for charting statistics and debugging.
```

---
## \#6 Posted by: Mattmccrary8 Posted at: 2017-10-10T15:27:43.542Z Reads: 131

```
So all in all do you think there is a solution to my problem or do you think I just need a new vesc
```

---
## \#7 Posted by: cody00 Posted at: 2017-10-10T15:53:51.694Z Reads: 126

```
I wouldn't go out and buy a new VESC - You just need some hard facts to 100% know exactly what is going on.  
You need to first figure out if it is VESC Temp, Motor Temp, Low Voltage that is kicking your board into lower power mode. 
"once I hit about a half mile it starts declining and then by a mile or 2 I can’t even get up to 20 mph"

Whether you do this through your laptop, bluetooth, or some other means - get some hard data.
```

---
## \#8 Posted by: i2oadsweepei2 Posted at: 2017-10-10T16:03:16.304Z Reads: 121

```
No expert here either. But 12s and 190kv are over the erpm limit of the vesc. 10s and 190kv is the sweet spot. I run 12s with 170kv motors. Maybe this is part or all of the problem.

There are ways to limit the erpm in bldc tool under the motor tab. I am not the right person to help with that. 

Search limit erpm. But becareful regarding the limiter and negative torque.

Best of luck.
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-10-10T16:03:58.605Z Reads: 116

```
If you can hold the motor for a 10 count then heat is not the issue. At least not motor heat...
```

---
## \#10 Posted by: Mattmccrary8 Posted at: 2017-10-10T16:08:02.285Z Reads: 118

```
I can hold it but it would be pretty hot for 10 seconds. Not burning but definitely not comfortable. 

Can I limit the erpm or duty cycle? I just want to get some intense range. I did 12s because I’ve seen so many builds with 190kv 12s but now I’m regretting it! I was being greedy
```

---
## \#11 Posted by: Mattmccrary8 Posted at: 2017-10-10T16:15:06.194Z Reads: 117

```
@Namasaki  @torqueboards you guys got any advice 🙌🏼🙏🏼
```

---
## \#12 Posted by: Crossfire Posted at: 2017-10-10T16:15:42.717Z Reads: 112

```
 You're probably overheating the VESC. What's the airflow in your enclosure?
Use the bluetooth module and analyze the data. Usually when the VESC overheats it's cutting the power. So you have worse performance later on.
If you can, go dual drive. I mean, it's easier on the motors, vesc's, and battery. And it pulls like mad. :)
```

---
## \#13 Posted by: Mattmccrary8 Posted at: 2017-10-10T16:18:11.882Z Reads: 110

```
No to much air flow in the enclosure but I cut holes in the bottom side for the charger port, on off and voltage meter so it should have air flow. @psychotiller do you think I should make holes in the front for more air flow?
```

---
## \#14 Posted by: Mattmccrary8 Posted at: 2017-10-10T16:18:36.156Z Reads: 114

```
Dual drive is the next step. I just wanted this working first
```

---
## \#15 Posted by: Crossfire Posted at: 2017-10-10T16:23:14.988Z Reads: 120

```
Yeah, I literally cooked one of my VESC 4.12 in the enclosure without the airflow. I wasn't monitoring it at all. When it was hot outside after like 5-7 min of bombing the roads it always started to cut top power. Enclosure was hot, so was the motor-but I could hold it without problems. It worked for like a month. Then on a very hot day after an hour of riding my first VESC went drv8032 :slight_smile:

Then with the new VESC I've started to monitor my temps, made some holes to let the heat out, even thought about the fan option. Well, after going dual with focboxes, my temps are at low 30-35C max with air temp around 20C. 
With VESC they were around 60+ with airflow on a single drive which was safe and it didn't cut any power at all. So under 80C it's safe but not in the long run anyway...heat is a b***h :D
```

---
## \#16 Posted by: Mattmccrary8 Posted at: 2017-10-10T16:29:10.566Z Reads: 116

```
The fan option seems like a pretty good idea if it’s cheap. So the only way to check my temp is with a Bluetooth modular? Otherwise a laptop would be off because it would be delayed due to me taking my enclosure off
```

---
## \#17 Posted by: Crossfire Posted at: 2017-10-10T16:38:23.381Z Reads: 111

```
Yeah but then you must get a step down converter because majority of fans operate at 12V. So that's more things to stuff into the enclosure.

BT module with a phone app or even apple watch app is very handy and you can easily monitor the ride and act accordingly.
```

---
## \#18 Posted by: Mattmccrary8 Posted at: 2017-10-10T16:40:28.390Z Reads: 111

```
Wait how easy is that to setup? Is it just plug in play or does is require soldering? I’d do that in a heartbeat if it could just plug in my vesc
```

---
## \#19 Posted by: Crossfire Posted at: 2017-10-10T16:44:12.852Z Reads: 109

```
You'll need the HM-10 bluetooth module with the 7-pin jst-xh 2.0mm connector to plug it in the VESC/focbox.
```

---
## \#20 Posted by: psychotiller Posted at: 2017-10-10T17:02:10.982Z Reads: 108

```
Look on ebay for an EZ run fan. They are easy to install in enclosures. Then you'll just need a servo splitter to get power to the fan. Plug and play. I think honestly 12s/190 kv is the culprit. I have lots of builds with little to no ventilation and no overheating issues  but I stayed within the vesc's limits.
```

---
## \#21 Posted by: Mattmccrary8 Posted at: 2017-10-10T17:05:22.099Z Reads: 102

```
Ok so your saying I shouldn’t be having any issues with this setup then? Would you make holes or just go with the fan
```

---
## \#22 Posted by: psychotiller Posted at: 2017-10-10T17:08:53.988Z Reads: 102

```
Nope, that's not what I said. You can make holes and get a fan, or both. But it won't change the fact that you are running 190kv @12s. You're going to end up over the erpm limit and you are going to burn out your drv's eventually.
```

---
## \#23 Posted by: thisguyhere Posted at: 2017-10-10T17:16:19.630Z Reads: 97

```
I'm running 190kv at 12s with limit set at 80k erpm, haven't had any issues yet but I'm rarely hitting top speed, if ever. 

also have giant holes in my enclosure for airflow and noticed vesc temps actually DROP at speed. 

get some venting going, pretty sure vesc throttles current when temps increase. also may consider cutting out vesc shrink wrap where the mosfets are. 

also how and where u have your vesc positioned in your enclosure may have an impact.
```

---
## \#24 Posted by: Mattmccrary8 Posted at: 2017-10-10T17:25:11.046Z Reads: 96

```
Are you running a dual motor setup. I have my 12s4p battery in the front and then I could fit another 2-3 vesc’s Where my one vesc is. I have everything velcored down to my board so there isn’t much stress on the enclosure. I did use weather proof strips so I know there isn’t much ventilation besides the wholes I cut for my battery charging port, on/off and voltage meter. 

So you think I should raise the erpm limit and cut some holes?
```

---
## \#25 Posted by: Namasaki Posted at: 2017-10-10T17:36:25.875Z Reads: 89

```
[quote="Mattmccrary8, post:11, topic:35239"]
Namasaki  @torqueboards you guys got any advice :raised_hands:🏼:pray:🏼
[/quote]

Heat sinks on the fets
```

---
## \#26 Posted by: Mattmccrary8 Posted at: 2017-10-10T17:48:17.516Z Reads: 87

```
So you thinks that’s all I need. Some heat sinks and a fan?
```

---
## \#27 Posted by: thisguyhere Posted at: 2017-10-10T17:52:27.964Z Reads: 88

```
my dual is 190kv 12s, another one is a mono but at 170kv 12s. 

cooling is not a panacea but it's worth trying since it's easy.

keep ur erpm where it is, my 80k may be too high
```

---
## \#28 Posted by: Mattmccrary8 Posted at: 2017-10-10T20:00:02.040Z Reads: 85

```
So no matter what I’m going to burn this thing out? What would you do if you were me. I really don’t want to spend more money at this point. I’ve thrown so much away
```

---
## \#29 Posted by: b264 Posted at: 2017-10-10T20:15:08.522Z Reads: 90

```
[quote="Mattmccrary8, post:1, topic:35239"]
once I hit about a half mile it starts declining and then by a mile or 2 I can’t even get up to 20 mph
[/quote]

If you stop after a mile and wait 15 whole minutes, then go again -- where the 15min delay is the only thing different -- does it still cut out?  If it resets your "mile or 2", then it might be heat problems because the 15 minutes could allow something to cool off.  But voltage sag could have similar symptoms.  
Try A) riding 2 miles B) riding 1 mile, 15 minute wait, riding 1 mile and C) riding 1 mile, charge battery while waiting 15 min, then ride one mile
Carefully scrutinise the differences
```

---
## \#30 Posted by: cody00 Posted at: 2017-10-10T20:42:30.871Z Reads: 87

```
The little heatsinks in this  pack worked for me.  They are the exact size of the mosfets.  (Blows my mind that someone can even sell and ship from China to US for $2 :slight_smile: )  

While you are waiting to receive these, definitely get the windows cut where the MOSFETS are - I did both top and bottom and tried to keep the window exact and not to expose the legs/terminals

http://www.ebay.com/itm/30PCS-Aluminum-Heatsink-Cooler-Adhesive-Kit-for-Cooling-Power-Raspberry-Board/141865269904?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649


I also picked this little fan up for $2.99.  I'm going to see if I all heat issues are resolved for myself before installing it.  
https://www.amazon.com/gp/product/B01K49K358/ref=oh_aui_detailpage_o08_s00?ie=UTF8&psc=1

Optional: In case you find the adhesive backs not working well...
https://www.amazon.com/gp/product/B0009IQ1BU/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#31 Posted by: Mattmccrary8 Posted at: 2017-10-10T21:05:22.920Z Reads: 85

```
I’ve done that. It it’s completly fine. The problem is 100% over heating then. I am getting somewhere people! Just need to figure out how to keep it cool. I’m going home to cut a few holes in the enclosure, I’ll cut holes where the mosfets are... if that doesn’t work I’ll go to heat sinks and a fan?
```

---
## \#32 Posted by: cody00 Posted at: 2017-10-10T21:27:13.281Z Reads: 80

```
Good plan 
Here are some links for bluetooth items:

On the naked cable side, I would solder the 4 wires to the 4 points on the bluetooth chip.  

https://www.amazon.com/gp/product/B01IZBC0KI/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1
https://www.amazon.com/gp/product/B06WGZB2N4/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1
```

---
## \#33 Posted by: Deckoz Posted at: 2017-10-10T22:47:09.892Z Reads: 77

```
Your issue is a matter of leverage. 16/36 is fine for 83/90mm wheels. Switch to a 40T and watch your problems disappear.

The 36T with big wheels causes higher amp draw...which means more heat.
```

---
## \#34 Posted by: ShutterShock Posted at: 2017-10-11T00:20:10.305Z Reads: 75

```
I've got my dual 190kv 12s board running just fine limited to 60kerpm so I kind of feel like that isn't the issue.  I haven't had a single issue since I first configured my VESCS
```

---
## \#35 Posted by: Namasaki Posted at: 2017-10-11T01:12:30.600Z Reads: 72

```
heat sinks can be very helpful.
if your gearing is too tall and your climbing hills, then that's a problem.
If your just going fast on flat ground, you should not be overheating, unless your going against a strong wind.
if your doing a lot of stop and go and not pushing the board to get going then that could be a problem.
```

---
## \#36 Posted by: Namasaki Posted at: 2017-10-11T01:13:15.064Z Reads: 71

```
[quote="ShutterShock, post:34, topic:35239, full:true"]
I've got my dual 190kv 12s board running just fine limited to 60kerpm so I kind of feel like that isn't the issue.  I haven't had a single issue since I first configured my VESCS
[/quote]


what brand of vescs are your using>?
```

---
## \#37 Posted by: Deckoz Posted at: 2017-10-11T01:21:26.694Z Reads: 75

```
That's fine and all


But what wheel size and gearing? And how heavy are you? What works for one person won't always work for the next... 

My buddy runs 12s dual 6374 190kv with 60kerpm limit too..but it would be really vague if I left the info there.
 As he doesn't get over heating issues... But he's using 16/40 and 100mm wheels...and weighs about 180lbs.

As @Namasaki said, it all depends on factors. But factors you can control, are wheel size and gearing, as you cannot easily change your weight or the rest of the build without a "lot" of money. Pulleys, and wheels are a lot cheaper then different kv motors or batteries.
```

---
## \#38 Posted by: ShutterShock Posted at: 2017-10-11T05:01:58.045Z Reads: 67

```
I'm using the ones from DIYElectric.  Not the best in the game but they seem to be working fine so far and they were  more reasonable than buying FOCboxes
```

---
## \#39 Posted by: ShutterShock Posted at: 2017-10-11T05:05:32.506Z Reads: 75

```
Yeah, I do realize that, I was just trying to throw in some more data into the mix.  Probably should have included some more information.

I weigh about 145, and I am using 83mm wheels like some of you were suggesting for him to use.  Which I also agree would probably help his situation, as there is a higher torque amount transferred due to the smaller radius of the wheels.  And it does depend on factors.   I am also running 16/36 gearing on 12mm belt.  I have "knock you off the board" torque with that, and can climb hills no problem.  I haven't seen my temps go any higher than a peak of about 47-50 degrees in the Ackmaniac app.

Apologies for being a bit vague, that was less helpful than I originally intended lol
```

---
## \#40 Posted by: Ishayc Posted at: 2017-10-11T09:07:11.550Z Reads: 73

```
What @Deckoz said is completely right.

I had the same issue a few days ago.
Tried to punch holes in my enclosures - Didn't work, Tried to Switch between batteries - Didn't work, Switched motors - Didn't work, Heat sink on all 6 MOSFETs - Didn't work.
The ONLY thing that worked is changing my gear ratio.
I changed my wheel pulley from 36t to 44t getting the ratio of 15t/44t.

Running 10s with 245kv motor on 97mm wheels.
```

---
## \#41 Posted by: Crossfire Posted at: 2017-10-11T09:23:57.153Z Reads: 68

```
I may sound like a fool but the real end solution to overheating the electronics and the motor is basically going dual drive.

You don't have to sacrifice the top speed gearing for it, you get amazing acceleration, fantastic brakes, a lot less heat and you really run your system the way it should be - cool and with less strain on the belts, pulleys and motor shafts; all that with lower, more conservative parameters in the BLDC/ VESC tools. 

I was on a single setup for like two months...only regret I got is that I didn't go dual earlier. :smiley:
```

---
## \#42 Posted by: Deckoz Posted at: 2017-10-11T13:28:24.516Z Reads: 68

```
Sure that's an answer... But i m pretty sure he already stated he didn't want to spend a lot more money to fix it.

A pulley and belt is about $25 bucks.

Another vesc, motor, motor mount, motor pulley, wheel pulley, belt, canbus wire, and sensor wire(if he has sensors) could be a varying cost of 250-500 depending on the components he chooses.

So is your solution really a solution? Sure for those that are willing to spend the money for the upgrade. But not for this guy.

Also sacrificing top speed?  16/36 on 83mm on 12s will net you about 33mph with a light rider. Move up to bigger wheels and your at 36-37mph. Increase your reduction with a 40T on the bigger wheels and you end up at basically the same top speed as the16/36T 83mm combo... So sacrifice? Not really.
```

---
## \#43 Posted by: Crossfire Posted at: 2017-10-11T14:36:46.843Z Reads: 66

```
The thing is...the money he'll throw in to find a solution for a single drive woes could be easily invested into dual drive. 
VESC is not designed to last, we all know that, especially in single drive setups. It's pushed to it's max and usually doesn't end well. 
12S and 190kV is drv8032 in just a matter of time. And we all want to enjoy the hobby as much as possible.

Going DIY is the most expensive path out of them all and in the end the most satisfying one. I could buy the evolve GT or raptor 2 and be done with it. It would cost me way less than going into single drive territories and now dual drive. God knows what else will itch me on the way :slight_smile:

It's just my perspective and the way I would do. You would buy bigger wheels, pulleys, belts and probably a new VESC and that's another 250-300$.

I would buy 2x focboxes, additional 190kV motor, belt and a pulley and that's like 400-450$. And much better ride experience. My 2 cents.
```

---
## \#44 Posted by: Namasaki Posted at: 2017-10-11T15:25:23.049Z Reads: 66

```
I'd start by changing the gear ratio as suggested by
@Ishayc
You might even get more speed once you stop overloading the motor.
```

---
## \#45 Posted by: Mattmccrary8 Posted at: 2017-10-12T16:07:33.635Z Reads: 55

```
Preach my friend! That fixed everything! I’m actually going dual 6374. Just ordered it all! Now that I got the board hauling ass! I don’t feel safe with mono breaks if I’m going to coast around 25-30mph all the time
```

---
## \#46 Posted by: Mattmccrary8 Posted at: 2017-10-12T16:08:17.185Z Reads: 54

```
Smaller wheels fixed it so in other words, gearing would of done I as well! Thanks everyone!
```

---
## \#47 Posted by: Namasaki Posted at: 2017-10-12T17:29:53.947Z Reads: 57

```
Yes, wheel size as well as pulley size all contribute to the gear ratio
```

---
## \#48 Posted by: Deckoz Posted at: 2017-10-12T17:35:08.205Z Reads: 54

```
Nice, glad stepping down in wheel size helped. 

Since your going dual 6374,  and you already have some nice big plush 97s, when you do end up with duals, swap out to a 16/40 and you should get all the road plush you want and the speed without any of the heat :)
```

---
## \#49 Posted by: Mattmccrary8 Posted at: 2017-10-12T17:49:33.006Z Reads: 51

```
So would there still be significant heat with dual 97’s 16/36 or you think I need to go to 40 no matter what?
```

---
## \#50 Posted by: Deckoz Posted at: 2017-10-12T17:58:32.922Z Reads: 51

```
How much do you weigh? If your sub 150lbs you'll be fine, above I'd switch to 40T
```

---
## \#51 Posted by: Mattmccrary8 Posted at: 2017-10-12T17:59:07.944Z Reads: 54

```
200lb so I am way above that lol
```

---
## \#52 Posted by: Deckoz Posted at: 2017-10-12T18:00:14.527Z Reads: 53

```
Yea I'd def switch to 40T then on 97s :)
```

---
