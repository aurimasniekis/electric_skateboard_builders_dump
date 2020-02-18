# Tuning vesc, shutdown but no fault code..SOLVED

### Replies: 110 Views: 5036

## \#1 Posted by: flywithgriff Posted at: 2017-02-13T06:44:44.225Z Reads: 314

```
**Motor:**
Tacon Bigfoot 160 - 245kv 

**Vesc:**
Ollin Boards VESC

**Mount:**
DIY's 63mm Motor Mount

**Driveline:**
DIY's ABEC 16/36 drive and 12mm belt

**Batteries:**
2x Turnigy 3s 8000 mah 30c Lipo

**Controller:**
TorqueBoards 2.4 ghz Nano

**Board:**
White Wave Shocker
Caliber II 10" Trucks
Hellion Bearings
Miami E Board's 83mm Flywheel clones

**Accessories:**
B6 AC Charger
JST 6S 20cm Extension
Miami E Board's Power Switch
Miami E Board's Charging Port


After about a month of research and advice I have finally ordered all of the parts for my first build. I think I have covered everything but feel free to let me know what I have missed or your opinions! I will update this thread as I build.
```

---
## \#2 Posted by: Tonto2k Posted at: 2017-02-13T10:41:14.346Z Reads: 286

```
How many 3s batteries are you using mate ? Post some pics of your items  🤙👍
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-02-13T11:09:36.348Z Reads: 281

```
Pls don´t use the nano remote, it´s not really reliable and does have cutouts.
Better take this one:
diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-02-13T11:12:53.351Z Reads: 269

```
Or if you really like to have a thumb control, buy the benchwheel remote from aliexpress :+1:
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-02-13T12:27:21.981Z Reads: 260

```
Im using 2x3s
```

---
## \#6 Posted by: Namasaki Posted at: 2017-02-14T00:20:32.161Z Reads: 249

```
The Torqueboards mini remote is excellent for control and dependability.
And a pair of  lithium AA batteries will last up to a year in this remote!
```

---
## \#7 Posted by: flywithgriff Posted at: 2017-02-14T20:09:41.769Z Reads: 238

```
Well guys the motor arrived last night. It kinda sucks having such a beautiful thing just sitting on the table awaiting its companions. If everything goes as planned, all parts will be in house a week from today. The only part I haven't received a shipping notice for is the VESC from @chaka. Hopefully soon!
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-02-16T00:03:25.949Z Reads: 227

```
Trucks, mount, and controller arrived today.
<img src="/uploads/db1493/original/3X/9/5/95f73b4804f36caa3f5d64169570735f991926ca.JPG" width="666" height="500">
```

---
## \#9 Posted by: flywithgriff Posted at: 2017-02-23T19:52:06.339Z Reads: 223

```
Parts are all in except the VESC! Take a look at the wiring here and let me know what you think. Yes, they are taped together for mock up.<img src="/uploads/db1493/original/3X/8/b/8b9c2f29127e725160aa6007c86f32399876339d.jpg" width="375" height="500">
```

---
## \#10 Posted by: UniqueSnowflakeN27 Posted at: 2017-02-23T20:06:55.170Z Reads: 210

```
Wiring looks good. But I'm assuming you'll cut it all to length when you're soldering on the right connections?

I had the exact same setup on V1 of my first board. After one test ride I ordered two more of those batteries. Really needed that extra range.
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-02-23T20:09:42.855Z Reads: 208

```
i will leave everything as is until its all tested and i will then cut everything to fit. Is there a problem with keeping the bullet connectors?
```

---
## \#12 Posted by: UniqueSnowflakeN27 Posted at: 2017-02-24T19:09:30.424Z Reads: 210

```
Oh, no not at all. I just thought they weren't the right ones since you hadn't connected them.
```

---
## \#13 Posted by: flywithgriff Posted at: 2017-03-13T02:40:00.659Z Reads: 199

```
Everything has finally arrived and the board is together. I made a few test runs today and was happy to finally be riding. However, I have a few concerns. 

6S (2x5000mAh 30-40c Lipo)
VESC
245 kv Tacon 160 63mm

Concerns:
1) Batteries at full charge and the range was about 3 Miles.
2) Acceleration was pleasant but with any hill the board would struggle greatly.
3) Braking above 12mph was nearly impossible and felt as if no brakes were present.


Current VESC settings:

Current Limits
Motor Max: 45A
Motor Min (regen): -40A
Batt Max: 40
Batt Min (regen): -12
Absolute Max: 130A

Voltage Limits
Min input Voltage: 8.0V
Max input Voltage: 40.0V
Batt cutoff start: 21.0V
Batt cutoff end: 19.8V

Any ideas or opinions on VESC settings?
```

---
## \#14 Posted by: thylen11 Posted at: 2017-03-13T09:43:36.103Z Reads: 184

```
I also run 6s and was asked for advice aswell. Here is the post: http://www.electric-skateboard.builders/t/vesc-first-time-vesc-configuring-some-questions/18912

If you read throught it you can deduce the sertings i used. Havent ridden with these settings though. Good luck!
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-03-13T15:50:15.678Z Reads: 178

```
@thylen11 thanks for the link. I read through your thread before posting but out motors are far different KV. Was hoping one of the veterans would have input.
```

---
## \#16 Posted by: thylen11 Posted at: 2017-03-13T16:57:22.899Z Reads: 179

```
Yea the motors are different indeed. Although I'm not quite sure if that matters. There will be a different torque and topspeed I suppose but dunno if the vesc parameters change when you change the motor. I believe only the motor detection part changes not the bldc tab.
```

---
## \#17 Posted by: flywithgriff Posted at: 2017-03-13T19:42:52.238Z Reads: 171

```
That makes sense. My main concern is I feel my range is far to short. I'm getting about 3 miles before the batteries are low enough the vesc shuts down.
```

---
## \#18 Posted by: longhairedboy Posted at: 2017-03-13T19:55:31.330Z Reads: 175

```
if you change out the old motor to a new motor of the same model and type, you'll only need to run motor detection. 

If you change it out to a completely different motor, you'll want to tweak your settings more than that based on how it feels when you street test. 

A 5Ah 6S is only going to give you about 5-7 miles max, its barely more watt hours than an airplane freindly boosted (99wh) and if you're going fun speed, expect less than that.
```

---
## \#19 Posted by: flywithgriff Posted at: 2017-03-13T19:59:35.271Z Reads: 163

```
I certainly don't want to change motors as this whole setup now has only about 7 miles on it. If the low range is all I can expect for this battery setup I am willing to add additional batteries. I would like to add to my current setup considering the money invested in what I currently have. What would you suggest?
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-03-14T11:06:44.526Z Reads: 153

```
You could double your range by going 6S 4P with two additional lipos if you can squeeze them onto your board. That would probably be the least expensive option. 10+ miles is a fun ride.
```

---
## \#21 Posted by: Jammeslu Posted at: 2017-03-14T12:44:54.972Z Reads: 147

```
just quick question, running 3s2p 5000mah each, range is enough but I want more speed so do I just increase mah rating and do i have to change bms and esc?
```

---
## \#22 Posted by: longhairedboy Posted at: 2017-03-14T13:06:38.308Z Reads: 149

```
you can do a few things to increase speed: 

- you could increase your voltage, which would require more lipos in series, a different BMS, possibly the same ESC depending on how far you go
- you could fiddle with your pulley ratios and find either bigger motor pulleys or smaller wheels pulleys or both, 
- get taller wheels
- get higher KV motors. At 6S you can run up to 270-300kv no problem. I ran NTM prop drive 270KVs for a long time. Great motors if you can find them. 
- some combination of all of the above
```

---
## \#23 Posted by: Jammeslu Posted at: 2017-03-14T18:23:39.264Z Reads: 148

```
What if i just go from 5000mah to 5800mah
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-03-14T18:33:24.740Z Reads: 151

```
that would increase range slightly but not speed.
```

---
## \#25 Posted by: flywithgriff Posted at: 2017-03-14T18:46:46.597Z Reads: 154

```
This is what I just rode with my setup, 2x3s 5000 mAh, and the vesc just hit the soft stop for voltage so I have maybe another 1/2 mile before I hit the hard stop.

<img src="/uploads/db1493/original/3X/0/4/043c6b23829c4150d6d652c9d9112e9256f83ab8.PNG" width="281" height="499"><img src="/uploads/db1493/original/3X/7/f/7f225b7e208143584626d660619bf7f3940e3024.PNG" width="281" height="499">
```

---
## \#26 Posted by: flywithgriff Posted at: 2017-04-03T23:36:55.374Z Reads: 145

```
Rode the board to work and back today so the upgrade to 8000mAh batteries certainly helped! I am happy with the range but would like a little more torque. Losing some top speed is fine being I currently max out at 21mph but rarely hit 19mph as it is. Would a gearing change help accomplish this?

<img src="/uploads/db1493/original/3X/f/2/f28bb936806f136d2519347832ae19d3bddde684.PNG" width="281" height="499">
```

---
## \#27 Posted by: Aeroquiv Posted at: 2017-04-04T00:01:42.444Z Reads: 137

```
You can get smaller diameter wheels. Going from 90mm to 83mm will drop 2 mph. You can also change to a 14T Drive gear or a 40T slave pulley. This would give you ~18 mph.  All options will give you more torque. @SolidSurfer sells some 14T gears and probably the cheapest option.
```

---
## \#28 Posted by: flywithgriff Posted at: 2017-04-04T00:04:18.367Z Reads: 133

```
Im currently running 83m wheels and 16/36 gears
```

---
## \#29 Posted by: Aeroquiv Posted at: 2017-04-04T00:11:02.865Z Reads: 139

```
Can go 83mm to 76mm which will also drop 2 mph. 14T Drive gear and 40T slave pulley still stands. Oh forgot to mention you can do any combination of these for even more torque. Doing all three at once will drop your speed to ~15mph.
```

---
## \#30 Posted by: flywithgriff Posted at: 2017-04-04T00:12:58.166Z Reads: 141

```
Think Im gonna try ordering the 14t motor gear and see how that does. I can already take off without pushing but the board comes to a slow roll up a good size hill.
```

---
## \#31 Posted by: dakota4e Posted at: 2017-04-04T00:28:28.443Z Reads: 133

```
Where did you source the 8Ah batteries?
```

---
## \#32 Posted by: Hummie Posted at: 2017-04-04T00:30:48.615Z Reads: 132

```
Flightmax 30c hobbyKing 8ah 3s and 2s
```

---
## \#33 Posted by: flywithgriff Posted at: 2017-04-04T00:30:54.771Z Reads: 136

```
Hobby king

<img src="/uploads/db1493/original/3X/3/3/33c4327a916515e467eaa45d5ac42f5cdfff6825.PNG" width="281" height="499">
```

---
## \#34 Posted by: Hummie Posted at: 2017-04-04T00:32:04.410Z Reads: 131

```
Just beat u. After hours of hobbyKing window shopping they seem the best
```

---
## \#35 Posted by: flywithgriff Posted at: 2017-04-04T00:34:42.040Z Reads: 127

```
I'm happy with them! I'm dying to go dual motors and voltage increase but I need to be thankful for what I have! I'm 250lbs and I have a board pushing me over 7 miles of decent hills.
```

---
## \#36 Posted by: Hummie Posted at: 2017-04-04T00:55:05.724Z Reads: 129

```
go 10s.
you can up your motor amps much more too and it gives way more low speed torque and acceleration at slower speeds.  i dont think anyone will balk if you do...160!!!  so they say on the vesc maker's forum.  

I've got a tacon160 without bearings you can have for 20$.  never used just sits here.  took it apart and lost the bearings.  also have a motor mount that goes with it I'll give you for 20 that's permanently attached to the hanger.  I'll post pics
```

---
## \#37 Posted by: flywithgriff Posted at: 2017-04-04T00:55:53.359Z Reads: 124

```
I'm interested
```

---
## \#38 Posted by: Hummie Posted at: 2017-04-04T00:56:34.070Z Reads: 129

```
i'll post in 5  are you in san fran bay area possibly.  hate shipping
```

---
## \#39 Posted by: Hummie Posted at: 2017-04-04T01:16:29.594Z Reads: 135

```
<img src="/uploads/db1493/original/3X/e/8/e8bcb7af72d158cfef48fa5acbc2c6e7846b7f2c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/0/205f7f23ad2c2ac612b438b0d6546fd3c7207f99.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/f/2/f20aa23a823cc88d25e452d18febdcbe971f1a72.JPG" width="500" height="500"><img src="/uploads/db1493/original/3X/9/7/9778d92b45702b11e194d2aef1b377d769768436.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/3/1/31556d0d178e42bd543304b4536ec3430386eddc.JPG" width="500" height="500">[Uploading...]() 

the mount is the last one I have and maybe that 's a long shot that you'd want it but the motor is scratch-free and just has wax on it....designed the mount around the motor and cast it on.  mount still needs to be drilled and requires an exact belt and pulley combo.  Motor is as good as new just needs to be cleaned and the bearings and the tiny set screw for the shaft.  20 for either.  mount needs some sanding and smoothing too and it'd look nice
```

---
## \#40 Posted by: flywithgriff Posted at: 2017-04-04T01:44:57.344Z Reads: 129

```
Thats a pretty cool mount. Am I wrong or is there no way to order parts for these motors? I cannot find a link to buy the bearings to put the motor back together.
```

---
## \#41 Posted by: Hummie Posted at: 2017-04-04T01:49:57.975Z Reads: 121

```
its a standard bearing. with calipers you could measure the dimensions.  8mm shaft.  dont have calipers
```

---
## \#42 Posted by: PXSS Posted at: 2017-04-04T02:55:15.129Z Reads: 122

```
@flywithgriff. You don't need to change anything. 
Are your vesc settings still the same as above? If so all you need is to increase motor amps max from 45 to 75-80. That will give you more torque on the low end without sacrificing speed or spending $$
```

---
## \#43 Posted by: flywithgriff Posted at: 2017-04-04T02:56:44.211Z Reads: 122

```
All my settings are the same as above! I haven't touched anything as I really can't afford to blow a VESC!
```

---
## \#44 Posted by: PXSS Posted at: 2017-04-04T03:12:18.031Z Reads: 125

```
Changing the max motor amps won't burn anything. 
The limit is the maximum amount of RMS cyrrent that goes into your motor. 

Your maximum battery power is:
40A * 22.2V = 888W

You can get this at full speed since your motor limit is higher than your battery limit. But lets say at 50% max rpm, you get:

22.2V * 0.5 * 45A = 499.5W
Voltage * (rpm/max rpm) * max motor amps = motor power

If your speed is even lower your max power is lowered even more. So to get more torque on the low end you need to increase motor amps. 

You should still be safe though, as you're not exceeding any battery or esc limits. The only thing to be careful with is the stupid amounts of acceleration you can get playing with this setting. You should also have enough buffer between it and absolute current for any transients

E: @flywithgriff if you make any of the changes suggested by others, your board will still be sluggish up hills since it's limited in software not hardware...
```

---
## \#45 Posted by: flywithgriff Posted at: 2017-04-04T03:33:47.595Z Reads: 115

```
i bumped the motor max up to 75. Im gonna ride it tomorrow after work so ill check it out and see what happens,
```

---
## \#46 Posted by: PXSS Posted at: 2017-04-04T03:40:06.215Z Reads: 107

```
Cool. That should give you an increase in power of 66% from 0-53% max rpm. After that you'll be limited by the battery power output of 888W ish.
```

---
## \#47 Posted by: flywithgriff Posted at: 2017-04-04T03:42:08.976Z Reads: 103

```
Half throttle to top end is more than enough already so if this allows for a pickup in acceleration and take off i will be a very happy man!
```

---
## \#48 Posted by: PXSS Posted at: 2017-04-04T11:13:09.800Z Reads: 102

```
FYI. If top end gets scary stupid, you can adjust it by lowering battery max amps.
```

---
## \#49 Posted by: PXSS Posted at: 2017-04-05T11:48:32.827Z Reads: 95

```
@flywithgriff
Any updates
```

---
## \#50 Posted by: flywithgriff Posted at: 2017-04-06T00:37:51.806Z Reads: 92

```
I've actually torn the board down for reshape and a few asthetic changes. Should have everything back together next week.
```

---
## \#51 Posted by: riva_00 Posted at: 2017-04-06T13:10:56.157Z Reads: 93

```
What about a rocket motor?

http://hobby-hangar.co.uk/rocket-motors-accessories/13389-rocket-motors-b6-4-pk3-047776016064.html

Strap a couple to the back of your board and activate when you need something a bit extra :slight_smile: 
What could possibly go wrong.....
```

---
## \#52 Posted by: flywithgriff Posted at: 2017-04-12T19:30:58.520Z Reads: 89

```
After riding my build around where I live I have noticed the roads and sidewalks are pretty rough and have quite a bit of loose sand and debris. I am currently running 83mm flywheel clones with 16/36 gearing. I have already ordered a set of 14/36 gears but I am curious if this will be enough for the wheel change. I am running a single 63mm motor on 6s. The rest of my build info is in the top of this thread.
```

---
## \#53 Posted by: PXSS Posted at: 2017-04-12T22:04:58.817Z Reads: 86

```
Did the firmware edits not work?
```

---
## \#54 Posted by: flywithgriff Posted at: 2017-04-13T01:11:00.142Z Reads: 83

```
Board is still down for rebuild. I'm just curious about larger wheels while I'm putting it back together. Ive ordered a 15t and 14t motor gear. Curious if I can get away with larger wheels.
```

---
## \#55 Posted by: Hummie Posted at: 2017-04-13T01:22:29.905Z Reads: 82

```
if youre worried about getting the torque with larger gears...the way you have the vesc programmed you're not getting near the low speed power you could get.   get bigger wheels and up your motor amps
```

---
## \#56 Posted by: flywithgriff Posted at: 2017-04-13T01:45:00.624Z Reads: 79

```
I'll upload pics of my current settings in the next couple of days.
```

---
## \#57 Posted by: flywithgriff Posted at: 2017-04-28T04:07:41.512Z Reads: 74

```
Alright guys all my parts have arrived and I'll be putting the board back together this weekend. I want to thank you all in advance for the help I hope to receive fine tuning my VESC.
```

---
## \#58 Posted by: flywithgriff Posted at: 2017-04-28T04:18:00.778Z Reads: 83

```
These are my current untested settings. Feel free to give your opinion!<img src="/uploads/db1493/original/3X/d/c/dc6e49efd50440816e39d6d1d41c3554c3c55daf.JPG" width="666" height="500">
```

---
## \#59 Posted by: flywithgriff Posted at: 2017-04-30T03:00:13.823Z Reads: 74

```
I have tested these settings finally and my biggest concern is now brakes. They just don't slow down much. I am interested in upping batt settings to help with low end torque as well. @PXSS
```

---
## \#60 Posted by: PXSS Posted at: 2017-04-30T03:17:40.607Z Reads: 74

```
Low end torque is motor max not battery max. So you need to bump that higher.
I would increase it in steps of 5-10A and see what you like. Again, I would not go past 120A

As far as brakes go, same thing. At low speeds, you need to adjust motor min and at high speeds battery min.
Your battery can handle up to 5C charge according to the specs but I would limit it to 3C at most...
That translates to 24A, which is a lot imo. Same as above, start at 12 and slowly increase it to 15, 18, 21, 24 until you get to where you like.

Same thing with motor min, you can go as low as -120 but I like mine at -60, play with it and see what feels good for you
```

---
## \#61 Posted by: flywithgriff Posted at: 2017-04-30T03:59:59.396Z Reads: 72

```
Great information! Thank you!

I am loading these numbers now and headed out for a run.

<img src="/uploads/db1493/original/3X/0/4/04ae5a458ab3a3aea7e40d03e02cf1b3ce416e06.jpg" width="375" height="499">
```

---
## \#62 Posted by: PXSS Posted at: 2017-04-30T04:01:23.401Z Reads: 69

```
Sounds good.
Let us know how it feels.
```

---
## \#63 Posted by: flywithgriff Posted at: 2017-04-30T04:19:08.876Z Reads: 69

```
It felt much better, both take off and brakes! But about 300 yds into the ride and after braking down a short hill the brakes seemed to get less effective and when I throttled again it as well seemed much less. I again got on the brakes for about 3 seconds and it just quit all together. I let it sit for a minute and it started right back up but still subdued before stopping again. I left the board powered on and plugged it into BLDC but don't see any errors.
```

---
## \#64 Posted by: PXSS Posted at: 2017-04-30T04:20:47.797Z Reads: 68

```
The braking current might be causing an overvoltage on the ESC, but not having any errors is weird.
Motor wasnt hot or anything was it?
```

---
## \#65 Posted by: flywithgriff Posted at: 2017-04-30T04:21:21.909Z Reads: 68

```
Where would I find the error? Nothing popped up
```

---
## \#66 Posted by: flywithgriff Posted at: 2017-04-30T04:26:48.593Z Reads: 69

```
Motor was warm but certainly not hot
```

---
## \#67 Posted by: Hummie Posted at: 2017-04-30T04:27:08.039Z Reads: 67

```
if you could log what's happening maybe even you're overheating, but that would be strange considering it didnt happen before.   I can't think of anything else.  and all you did was up the motor amps?
```

---
## \#68 Posted by: flywithgriff Posted at: 2017-04-30T04:29:25.159Z Reads: 68

```
Upped motor max by 10 and upped batt min from -12 to -20
```

---
## \#69 Posted by: PXSS Posted at: 2017-04-30T04:33:54.246Z Reads: 66

```
you need to type faults in the command window for errors to come up
```

---
## \#70 Posted by: flywithgriff Posted at: 2017-04-30T04:44:59.783Z Reads: 70

```
<img src="/uploads/db1493/original/3X/0/b/0ba52b1c0bee8e010b6d9c02e2db969abe33a7e8.jpg" width="375" height="499">

dropped motor min and batt min. Only noticed decreased braking. However, same issue as last time. Decreased performance and then cut out.

Where is the command window for checking fault?
```

---
## \#71 Posted by: PXSS Posted at: 2017-04-30T14:06:17.557Z Reads: 67

```
Terminal tab almost all the way to the right. 

Lets try to determine what created the fault. Set your brake settings back to what they were and leave the torque stuff high. 

If no issues then increase your battery min. If no issues then increase you motor min. 

This way we can pinpoint to where the issue is
```

---
## \#72 Posted by: flywithgriff Posted at: 2017-04-30T14:20:27.890Z Reads: 64

```
I shut the board down when I went to bed but I'll make the changes and see what happens. I'll have results in about 20 minutes.
```

---
## \#73 Posted by: flywithgriff Posted at: 2017-04-30T14:53:35.191Z Reads: 59

```
Reduced some settings and it took longer to stop working but brakes back to the original barely braking. I hit the soft shutdown and it took a little longer but still shut down completely.  Maybe the 97's are just to much to sustain?
[Uploading...]()
```

---
## \#74 Posted by: flywithgriff Posted at: 2017-04-30T19:41:26.043Z Reads: 63

```
returned setting back to my original setup and simply boosted my battery max to 80 as @PXSS suggested. Headed out to see what happens.

<img src="/uploads/db1493/original/3X/8/2/827b03a59abb1eb32ef09262171aec92b6f8ae94.jpg" width="375" height="499">
```

---
## \#75 Posted by: flywithgriff Posted at: 2017-04-30T19:55:05.002Z Reads: 61

```
OK! Much better finally. Board still seemed to hit a soft shutoff. After cruising a few hundred feet and using the brakes it seemed as if each time i applied throttle it was much less significant than the beginning of the ride. Im fully aware of the sensation of torque in relation to current speed and i am positive this is not the case.
```

---
## \#76 Posted by: Titoxd10001 Posted at: 2017-04-30T20:20:05.967Z Reads: 64

```
When you go to larger wheels you're changing gear ratio. You want get the most reduction I would say for 97mm you want 15/40 minimum or 14/40. If you want to increase speed you should increase voltage.

What is your current setup? Wheels/pulleys/kv/voltage/top speed
```

---
## \#77 Posted by: flywithgriff Posted at: 2017-04-30T20:31:27.546Z Reads: 66

```
97mm, 15/36, 245kv, 6s2p, top speed unknown yet.

board seems to perform the same as it did with the 16/36 on 83mm which im ok with but have to solve the shut down issue.
```

---
## \#78 Posted by: Titoxd10001 Posted at: 2017-04-30T21:03:15.142Z Reads: 65

```
If you weren't having issues with 83mm 16/36, 15/40 on 97mm might help. If you had issues before it may be the voltage is to low and kv to high for a vesc.
```

---
## \#79 Posted by: flywithgriff Posted at: 2017-04-30T21:06:57.519Z Reads: 66

```
I had zero problems with the 83mm set up. Just needed more torque. I'm perfectly ok with a top speed of 18mph if it means low end torque and a bit better hill climbing. Would one of your 40T help?
```

---
## \#80 Posted by: Titoxd10001 Posted at: 2017-04-30T21:16:23.816Z Reads: 75

```
It will help with torque. Im not sure if it will solve your problems completely, but it should be very similar to how it was with 83mm wheels and 16l36
```

---
## \#81 Posted by: PXSS Posted at: 2017-04-30T21:21:39.005Z Reads: 71

```
Was your board charged? Were you able to get it to shut off again?
I'm thinking you might be hitting your low voltage cutoff as you hit throttle again and again

Can you post a screenshot of the realtime tab
```

---
## \#82 Posted by: flywithgriff Posted at: 2017-04-30T21:41:51.902Z Reads: 69

```
The problem started while the board was fully charged.  I have gotten it to shut down each test ride, but cannot get a fault to come up on BLDC. Forgive my ignorance of the realtime tab but what exactly are you asking for?
```

---
## \#83 Posted by: PXSS Posted at: 2017-04-30T21:45:47.984Z Reads: 70

```
Let me see if I can pull up screenshots or a video of what you need to do to pull up the fault codes.
```

---
## \#84 Posted by: flywithgriff Posted at: 2017-04-30T21:49:41.654Z Reads: 71

```
That would be great, I have been going to the terminal tab and typing in Faults which makes it display NO_FAULT...
```

---
## \#85 Posted by: Blasto Posted at: 2017-04-30T22:42:40.094Z Reads: 65

```
Set your maximum input voltage to 57V
```

---
## \#86 Posted by: flywithgriff Posted at: 2017-04-30T22:59:50.096Z Reads: 64

```
I have max at 57 and min at 8.
```

---
## \#87 Posted by: flywithgriff Posted at: 2017-05-01T23:56:29.550Z Reads: 67

```
Just had a thought!

COULD MY VESC BE SHUTTING DOWN BECAUSE MY BATTERY WIRES ARE TOO LONG??

My build has separate enclosures and the 10 AWG cables are about 20" long. Could this be a problem with overheating?
```

---
## \#88 Posted by: JohnnyMeduse Posted at: 2017-05-01T23:59:35.844Z Reads: 70

```
Is everything shutting down or the vesc just had a red light flashing... if the vesc and everything shut down. You problem probably something else than the vesc... actually I belive it most likely to be tour E-switch.
```

---
## \#89 Posted by: flywithgriff Posted at: 2017-05-02T00:01:46.190Z Reads: 71

```
It's never a sudden shutdown. It always starts strong and then performance decreases like I'm hitting a soft shutdown and if I keep riding I get a shutdown. When that happens if I just stop for about 5 seconds the board come right back to life and cycles again.
```

---
## \#90 Posted by: JohnnyMeduse Posted at: 2017-05-02T00:32:14.023Z Reads: 70

```
Does the red led flash or the power go down... also can you post some picture of your setup.
```

---
## \#91 Posted by: flywithgriff Posted at: 2017-05-02T00:35:27.036Z Reads: 72

```
I have a permenant enclosure mounted so unfortunately I cannot see the vesc without destroying my griptape and unmounting the enclosure.
```

---
## \#92 Posted by: JohnnyMeduse Posted at: 2017-05-02T00:59:44.303Z Reads: 72

```
Sorry but It's going to be really hard to figure what is your problem if you can't access any of the electronics 😧...
```

---
## \#93 Posted by: flywithgriff Posted at: 2017-05-02T01:05:49.699Z Reads: 71

```
I'm trying to figure why I would be getting a shutdown but not having a fault code on the vesc. The only thing that I have changed as far as my setup that was working fine is as follows.

83mm wheels up to 97mm wheels
Motor gear from 16 down to 15
Battery wires extended to 20"
Replaced motor wires with 10 AWG
```

---
## \#94 Posted by: JohnnyMeduse Posted at: 2017-05-02T01:31:59.436Z Reads: 73

```
There 3 reason you will have no faults on a vesc, first when the vesc shutdown for low voltage, second when the maximum input voltage is way over the, third when there is no faults... so if you don't have any fault problem is somewhere else...
```

---
## \#95 Posted by: flywithgriff Posted at: 2017-05-02T01:41:51.771Z Reads: 69

```
That certainly makes sense!  

If the batteries are being drained at a rate that is to high would that not explain the decreased power that eventually shuts the vesc off? Would it make sense that the batteries become unstrained when the vesc shuts down which allows them to basically reset for another run?
```

---
## \#96 Posted by: Hummie Posted at: 2017-05-02T03:41:48.070Z Reads: 69

```
Maybe over-temp.  Are u big going up hills?  With the low voltage you're doing you must rely on hot amps
```

---
## \#97 Posted by: flywithgriff Posted at: 2017-05-02T03:44:19.622Z Reads: 68

```
im 250lbs and there is a slight hill in my complex but its maybe a 3 foot rise over a 300ft distance so thats barely a hill at all. I think im gonna bite the bullet and build a 10s pack.
```

---
## \#98 Posted by: JohnnyMeduse Posted at: 2017-05-02T03:45:34.194Z Reads: 67

```
[quote="flywithgriff, post:95, topic:17634"]
If the batteries are being drained at a rate that is to high would that not explain the decreased power that eventually shuts the vesc off
[/quote]

or you just trigger some safety on your bms or switch.
```

---
## \#99 Posted by: Hummie Posted at: 2017-05-02T03:45:57.065Z Reads: 67

```
If u get one of those things that sends ur vesc info to ur phone u can see the temp.  Maybe move ur temp sensor max a bit lower and see if the shut off is sooner
```

---
## \#100 Posted by: flywithgriff Posted at: 2017-05-02T03:47:08.867Z Reads: 67

```
No bms and im running a switch from DIY
```

---
## \#101 Posted by: flywithgriff Posted at: 2017-05-02T03:48:01.495Z Reads: 67

```
I don't have an android device unfortunately. Im unaware of anything available for apple devices.
```

---
## \#102 Posted by: flywithgriff Posted at: 2017-05-03T00:01:57.101Z Reads: 64

```
UPDATE:

I have just plugged up my board for charging and the cells are at 3.7v. I have put less than a mile and a half range on the packs since full charge. With the power problems and such a short range on an entire battery cycle would it be safe to say amp draw could be my problem?
```

---
## \#103 Posted by: anorak234 Posted at: 2017-05-03T01:46:53.378Z Reads: 66

```
Amp draw could definitely be a problem - but it may also be the efficiency of your system. How tight is your belt? How well aligned is your system? I redid an old mountainboard recently and had to switch to street wheels for testing bc the large rubber wheels with a slight wobble in the gear got me 2 miles of range out of battery packs that normally push 8 or 9 on the drivetrain
```

---
## \#104 Posted by: flywithgriff Posted at: 2017-05-03T01:56:47.867Z Reads: 67

```
Everything is lines up pretty well. The belt might be a tad bit on the tight side as well but nothing crazy. Im really thinking its the 97mm wheels that are killing me. Im charging the board right now and will be testing the setup with the 83mm to see what happens.
```

---
## \#105 Posted by: anorak234 Posted at: 2017-05-03T01:59:08.067Z Reads: 69

```
Honestly if I were you I'd just get a battery that can handle it. I know from experience that small lipos like yours are good for starters but all they do is leave you craving something with more punch
```

---
## \#106 Posted by: flywithgriff Posted at: 2017-05-03T02:00:31.505Z Reads: 68

```
I'm in the process of ordering the parts for a 10s battery pack! I'm a big guy at 250 lbs and 6s with big wheels just don't cut it i'm afraid.
```

---
## \#107 Posted by: flywithgriff Posted at: 2017-05-04T02:33:45.811Z Reads: 69

```
Good News! 

I switched back to the 83mm wheels and 14/36 gearing. Plenty of torque and no heating issues!
```

---
## \#108 Posted by: flywithgriff Posted at: 2017-05-05T15:51:18.001Z Reads: 62

```
I made further adjustments last night and ran the 83mm wheels with a 16/40 gearing. Best performance yet!
```

---
## \#109 Posted by: Titoxd10001 Posted at: 2017-05-08T19:04:56.082Z Reads: 60

```
Have you tried 14/40 and 97mm wheels
```

---
## \#110 Posted by: flywithgriff Posted at: 2017-05-08T19:37:03.794Z Reads: 53

```
I did, still had shut down problems. I have changed it to a 15/36 with 83mm wheels and it is performing much better. This is the exact setup I was running before I extended the battery wires and had zero problems. I'm not sure if I'm now experiencing a voltage sag/ low power problem or what the downfall is but I do know it's caused by the lengthened wires from the battery to the VESC. I rode several miles this weekend and only had an issue while running full throttle for an extended period of time. As long as I ride around half power and don't brake too aggressively I have no issues.
```

---
