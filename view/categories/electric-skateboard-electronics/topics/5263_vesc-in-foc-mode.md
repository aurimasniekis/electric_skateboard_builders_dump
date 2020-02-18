# VESC in FOC-Mode

### Replies: 31 Views: 6244

## \#1 Posted by: DeathCookies Posted at: 2016-06-28T13:09:55.540Z Reads: 604

```
Hey,
in the past time i read several times that eboarder have fried their VESC when using it with FOC.
I would like to know who has fried a VESC and from where you have bought the fried VESC.
```

---
## \#2 Posted by: hoochij4s Posted at: 2016-06-28T13:19:25.598Z Reads: 606

```
I'm having my doubts about using FOC. I bought Vedder's VESC and a CarvON v2 Single HUB, but I don't have my batteries yet. Maybe @RunPlayBack can give us some feedback about his experience.
```

---
## \#3 Posted by: RunPlayBack Posted at: 2016-06-28T13:48:50.391Z Reads: 596

```
There are so many posts about VESC FOC frying that it's turning into some kind of urban legend or something lol. I haven't had any problems with FOC. I've been running on Ollinboard VESC (no heatsink), Carvon V2 Single and @onloop Space Cell since January in every condition you can imagine. I may have just lucked out with this combo of parts but I would attribute it to the durability of @chaka VESC. Here's my settings:

Motor Max: 60.00 A
Motor Min: -60.00 A
Bat Max: 30.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A
Max ERPM: 60000.00
Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V
Startup Boost: 0.040
Soft RPM limit
ERPM limit start: 0.00
ERPM limit end: 60000.00
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-06-28T14:02:12.056Z Reads: 558

```
[quote="RunPlayBack, post:3, topic:5263"]
I would attribute it to the durability of @chaka VESC
[/quote]
I agree.
I just thought that the most fried VESCs are from enertion but i dont know exactly. So i made this topic to see how makes poor VESCs.
```

---
## \#5 Posted by: hoochij4s Posted at: 2016-06-28T14:05:12.752Z Reads: 539

```
Thanks bro! Always here to help :sunglasses:
```

---
## \#6 Posted by: treenutter Posted at: 2016-06-28T14:14:08.189Z Reads: 536

```
@DeathCookies I used FOC for a long time before I had an issue, and the issue was traceable to a short caused by some bad wiring on my part. Full story below.

http://www.electric-skateboard.builders/t/another-drv8302-fault-disconnected-motor-leads-cause-short/3908
```

---
## \#7 Posted by: RunPlayBack Posted at: 2016-06-28T14:14:19.365Z Reads: 523

```
The only problem I've ever had with FOC was from user error because one of my motor phase wires came loose. I would hit full throttle and when I hit throttle again it would automatically brake which was scary as hell but I was able to run it off. So one thing to keep in mind is that when you're running FOC always make sure your motor wires are super secure.
```

---
## \#8 Posted by: treenutter Posted at: 2016-06-28T14:19:51.475Z Reads: 521

```
@DeathCookies Sounds like for me and for @RunPlayBack the problems were not a result of using FOC; I think similar symptoms would arise using BLDC mode.

The two common issues attributable to FOC, it seems, are failed motor detections (resolved by reducing battery cable length) and strange braking behavior (resolved by using an updated HW version of VESC or adding a cap to C18).
```

---
## \#9 Posted by: elkick Posted at: 2016-06-28T16:14:26.872Z Reads: 504

```
VESC failures with FOC are not a manufacturing issue. 

It's a combination of motors (some fail, some don't under FOC), parameters in BLDC tool, cables (shorting them, length), bad solder joints due to vibrations, switching between FOC and BLDC with no reset to default values, using 12s sometimes causes that as well, and so on. Already wrote the in the FOC thread.
```

---
## \#10 Posted by: Godfrey Posted at: 2016-06-28T16:50:14.759Z Reads: 488

```
[quote="RunPlayBack, post:3, topic:5263"]
Bat Max: 30.00 A
[/quote]

Does that mean Battery pack discharge amps?
```

---
## \#11 Posted by: RunPlayBack Posted at: 2016-06-28T17:12:57.901Z Reads: 474

```
Max draw from the Space Cell battery. http://www.electric-skateboard.builders/t/vesc-faq-optimized-s-p-a-c-e-cell-settings/414
```

---
## \#12 Posted by: Godfrey Posted at: 2016-06-28T18:34:50.742Z Reads: 459

```
Im confused does this mean if i have a battery pack (12s2p) that discharges 20amps at MAX it can power dual motors?
```

---
## \#13 Posted by: Blacksheep Posted at: 2016-06-28T18:35:15.790Z Reads: 450

```
where does vadder sell his vesc?
```

---
## \#14 Posted by: hoochij4s Posted at: 2016-06-28T18:36:03.272Z Reads: 449

```
http://www.ollinboardcompany.com/product/vedder-s-speed-controller

Here you go my friend!
```

---
## \#15 Posted by: Hummie Posted at: 2016-06-28T18:39:01.597Z Reads: 442

```
U have a battery max amp and motor max amp on the vesc.  It converts higher voltage to amps for th motor so u can use less amps from the battery with higher voltage.  A big benefit of using higher voltage as it keeps the vescs temp down
```

---
## \#16 Posted by: Blacksheep Posted at: 2016-06-28T18:39:58.519Z Reads: 436

```
thanks! =)
```

---
## \#17 Posted by: treenutter Posted at: 2016-06-28T18:44:01.028Z Reads: 437

```
[quote="Blacksheep, post:13, topic:5263, full:true"]
where does vadder sell his vesc?
[/quote]


@hoochij4s @Blacksheep for clarity, OllinboardCompany is not where Vedder sells VESC. Vedder is the designer who releases the open-sourced VESC design, and OllinboardCompany is one of the groups that manufactures and sells them. 

The owner of OllinBoardCompany, @chaka, is a member here and I personally own one of the VESCs he sells, and it is very high quality, but it isn't Vedder who builds them to sell.
```

---
## \#18 Posted by: Godfrey Posted at: 2016-06-28T18:46:53.040Z Reads: 427

```
thanks a lot very helpful
```

---
## \#19 Posted by: hoochij4s Posted at: 2016-06-28T19:38:03.924Z Reads: 425

```
My bad @treenutter , thanks for the correction!
```

---
## \#20 Posted by: DeathCookies Posted at: 2016-06-29T05:52:03.933Z Reads: 426

```
[quote="elkick, post:9, topic:5263"]
using 12s sometimes causes that as well
[/quote]

I use my repaired VESC since 2 Weeks in FOC on 12S and dont have problems at all.
```

---
## \#21 Posted by: Bender Posted at: 2016-07-13T02:46:46.487Z Reads: 391

```
What motor/kv are you running?

I'm getting "abs over current" errors after breaking hard then light accelerate or accelerating hard and breaking
Doesn't seem to happen in BLDC. :thinking:
```

---
## \#22 Posted by: DeathCookies Posted at: 2016-07-13T05:50:57.269Z Reads: 395

```
Turnigy SK3 149kv
but sadly my VESC has now problems too... I do not see any faults in BLDC but it still does not want to drive... :(
```

---
## \#23 Posted by: philipp Posted at: 2016-07-30T20:34:19.167Z Reads: 415

```
RPB, you really got me hooked with your awesome esk8 clips and your very informative blog! :)

So I've built my board based on your blog post and could finally assemble it fully yesterday.

I did a few 10-20 minute rides with the settings you posted.

I have a few questions:
**Question 1:**
[quote="RunPlayBack, post:3, topic:5263"]
Startup Boost: 0.040
[/quote] In my BLDC-Tool it says (Startup boost (BLDC only), does it still have an effect in FOC?

**Question 2:(Solved)**
[quote="RunPlayBack, post:3, topic:5263"]
Bat Max: 30.00 A
[/quote]
I think the new SpaceCell BMS has a 40Amp limit and a 40 Amp fuse, so I think it should be okay to set it 40.
Will this maybe have and effect on the torque?
**EDIT:(Solved)** I upped the Bat Max to 40A, still working fine and feels more torquey.

**Question 3:(Solved)**
[quote="RunPlayBack, post:3, topic:5263"]
ERPM limit end: 60000.00
[/quote]
On your blog you have this setting at the default value of AFAIK 10k.
Does this setting have an effect on the speed limit?
**EDIT:(Solved)** I set this back to 100k, since in my BLDC tool it says BLDC Mode only. Soft ERPM Settings do take effect, but I disabled it.

**Question 4:(Solved)**
If I do benchtesting (I use the mini 2.4ghz "Winning" Remote) it's almost impossible to let the wheel turn slow and then slowly accelerate, it goes from 0 to max RPM very quickly. While riding it seems to work pretty good. Is this normal, or is there a setting to smoothen out the acceleration?
**EDIT:(Solved)** Got this solved with setting the correct minimum and maximum pulsewith in the PPM settings-tab.
This video explained it nicely: https://www.youtube.com/watch?v=OtuofrQr3F8

**Question 5:**
After about 10 minutes of riding it somehow feels that the torque lowers (I have a SPACE Cell 3 with Battery cut off start at 35.20 V). On one ride it started to feel like almost 30% of the torque towards the end of the ride. Is this maybe an overheating issue? I have the temperature limits set like this:
<img src="/uploads/db1493/original/2X/5/58ed95cf076e9795868a1f64fa25c1ee6d080aff.png" width="690" height="92">
**EDIT:(Unsolved)** This problem seems to still exist, torque is decreasing over a 10minute ride.



Thanks!
```

---
## \#24 Posted by: gaetjen Posted at: 2016-11-04T17:21:56.460Z Reads: 315

```
I just switched to FOC mode. Before that I was riding in BLDC. I didn't flash the firmware. Just reseted it to the default settings and set up the new ones. Now, the board accerlates much smoother and is much quieter. I'm using an esk8.de VESC and an SK3 6364 245kv motor with an 8s lipo battery. First ride was awesome. Hope it will last.
```

---
## \#25 Posted by: noob Posted at: 2016-12-03T20:57:39.775Z Reads: 310

```
do you know what video you watched to set it up?
```

---
## \#26 Posted by: gaetjen Posted at: 2016-12-04T15:24:28.104Z Reads: 300

```
https://www.youtube.com/watch?v=xSCEFK7Zljw
```

---
## \#27 Posted by: pkasanda Posted at: 2017-02-17T06:38:20.999Z Reads: 272

```
Great video.
```

---
## \#28 Posted by: Martinsp Posted at: 2017-02-18T00:29:16.171Z Reads: 262

```
Hey guys, 
has anyone tried to run maytech vesc in foc mode?
```

---
## \#29 Posted by: Eboosted Posted at: 2017-02-18T06:10:43.530Z Reads: 253

```
This video makes me feel FOC is so damn simple to set.

I wonder why have people blown so many VESCs in the past because of incorrect parameters, if the ones on this video are so straight forward and easy to follow?
```

---
## \#30 Posted by: Tuomalar Posted at: 2017-02-18T19:06:40.437Z Reads: 245

```
I'm wondering it too. I would like to give try, but apparently there is so many little thing to go wrong..
```

---
## \#31 Posted by: Donson Posted at: 2017-11-19T18:28:26.130Z Reads: 120

```
yes me.... and it blow up..... the red led blinking now
```

---
