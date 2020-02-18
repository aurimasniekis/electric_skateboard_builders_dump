# Flipsky VESC runing FOC

### Replies: 30 Views: 1947

## \#1 Posted by: Eboosted Posted at: 2018-08-12T05:33:50.658Z Reads: 406

```
Has anyone stressed enough this VESC in FOC a fair ammount of time to give a trustworthy opinion?
```

---
## \#2 Posted by: adrienfeve Posted at: 2018-08-12T06:49:26.481Z Reads: 396

```
I'm willing to get some feedback on that too. VESC 4.12 in my case.

Are talking about the 6.6?
```

---
## \#3 Posted by: Andy87 Posted at: 2018-08-12T07:09:09.278Z Reads: 389

```
I would be interested in Foc on 6.6
```

---
## \#4 Posted by: Eboosted Posted at: 2018-08-12T07:10:44.381Z Reads: 383

```
I was talking about the v4.12, sorry about the lack of information. I wonder if it has the same robustness as a Focbox
```

---
## \#5 Posted by: Eboosted Posted at: 2018-08-12T07:12:12.427Z Reads: 377

```
[quote="Andy87, post:3, topic:64618, full:true"]
I would be interested in Foc on 6.6
[/quote]

I don't have any doubt the V6.6 will perform great on FOC.
```

---
## \#6 Posted by: gigoy Posted at: 2018-08-12T08:55:06.113Z Reads: 361

```
I've been using it for a month on FOC. It doesn't have the aluminum case.

I don't know if this is enough stress test for it.

Single drive 6374 190kv
8-10km a day, 5 times a week for the last month or so.
Rider weight 100-105kg.
My usual route includes steep hills.

I haven't had any problems with it so far. I don't have any experience with FOCboxes so I really can't compare them both. But I can compare these:

ESCape > Flipsky 4.12 > HK Esk8 ESC

I'm not an expert but I feel like there's a big difference between the performance of the Flipsky and the HK esk8 ESC. I didn't think that was even possible given they follow the same design and maybe even components... or maybe it was just faulty to begin with because the drv burnt out after using it a few times.
```

---
## \#7 Posted by: visnu777 Posted at: 2018-08-12T09:16:08.467Z Reads: 342

```
I only used FOC with these running dual DIYeboard 90mm hubs and had no issues so far but I'll keep you updated :) I even made the mistake of not disconnecting Can while only powering one of them and they survived ;)
```

---
## \#8 Posted by: Newby Posted at: 2018-08-12T09:59:10.624Z Reads: 337

```
Sounds impressive. I think flipsky are earning a really good reputation now. They have a vedder eswitch for £13 without connectors or fuse nobody has tested. Is there a review of their motor yet?
```

---
## \#9 Posted by: Koolfarmer Posted at: 2018-09-04T23:01:04.822Z Reads: 281

```
My HK esk8 ESC is 4.10 and not 4.12 as they sell it now.
It was not possible to use it in FOC as I would loose the brake and I almost died twice haha.
I rapidly took of the FOC mode, however, I beleive the new HK would cope better in FOC since it is the 4.12 but I don-t own one so can-t be sure
```

---
## \#10 Posted by: kalebludlow Posted at: 2018-09-04T23:03:20.434Z Reads: 283

```
What battery do you have? 4.12 and FOC don't play very nicely when using a 12S battery
```

---
## \#11 Posted by: Koolfarmer Posted at: 2018-09-04T23:08:54.568Z Reads: 274

```
I'm on 10s with a 4.10. No Foc. Going pretty well, with the HK orange motor. I got used to the noise and i'm fine with it now. So much torque, And Barcelona has some serious hills. Still, I'm looking to make a dual drive soon
```

---
## \#12 Posted by: Eboosted Posted at: 2018-09-05T03:44:51.981Z Reads: 268

```
[quote="kalebludlow, post:10, topic:64618"]
FOC don’t play very nicely when using a 12S battery
[/quote]

My 4.12 focboxes run amazing on FOC and 12s on all my boards
```

---
## \#13 Posted by: kalebludlow Posted at: 2018-09-05T04:26:52.352Z Reads: 250

```
What brand of 4.12? I plan on running FOC on 12s with my Flipsky escs just haven't heard too many positive things
```

---
## \#14 Posted by: Eboosted Posted at: 2018-09-05T04:58:00.415Z Reads: 247

```
Please test it and keep us posted, it's a product I'm looking forward to hear good things but nobody was done a proper testing and review
```

---
## \#15 Posted by: kalebludlow Posted at: 2018-09-05T04:59:20.295Z Reads: 248

```
I dont have a remote yet, but am I able to do any testing with my PC? Waiting for the battery to arrive and havent had a chance to sit down with VESC-tool yet
```

---
## \#16 Posted by: Eboosted Posted at: 2018-09-05T05:12:57.415Z Reads: 247

```
No. You need to ride it in Foc and maximum throttle, see if it works consistently for at least a day and report back, that wouod be extremely helpful
```

---
## \#17 Posted by: kalebludlow Posted at: 2018-09-05T05:15:02.252Z Reads: 241

```
Well when I have all the stuff I'll do it, can't afford to finish the build right now as my normal mode of transport decided to shit itself last night
```

---
## \#18 Posted by: visnu777 Posted at: 2018-09-06T12:19:33.363Z Reads: 228

```
Still no problems so far, going steep passages and full speed on my daily ride, everything is still fine :) (2x FSVESC 412)
```

---
## \#19 Posted by: Eboosted Posted at: 2018-09-06T14:09:01.235Z Reads: 221

```
12s? How many maximum battery amps?
```

---
## \#20 Posted by: visnu777 Posted at: 2018-09-06T14:17:19.895Z Reads: 222

```
10s3p (vtc6), max battery amps set to 22.5A each (45A total), diyeboard 90mm hubs (replaceable pu)

https://metr.at/r/THPMS
```

---
## \#21 Posted by: mike_o Posted at: 2018-12-18T00:22:56.366Z Reads: 158

```
Tried SK8 VESC first with conventional (non FOC) drive, then went FOC and re-tuned for the motor parameters. The noise went down, but the motor seemed to get a very little bit warmer, and efficiency also seemed to go down. ESC cool all along, though.
```

---
## \#22 Posted by: slick Posted at: 2019-04-30T17:52:09.936Z Reads: 117

```
Jumping in late to this thread but I just recently bought a Flipsky 4.12 VESC with aluminium case.

I run it with 8S1P lipos and a SK3 5065/ 275KV motor FOC and here is what I've experienced. 

After setup with the newest version of the VESCTOOL I've experienced some cogging after attempting to accelerate after a hard deceleration. So cogging occurred after braking hard. I could get rid of cogging after disconnecting the VESC from the battery. I'm not quite sure what exactly caused the cogging.

Anyway, when setting up the VESC with the newest version of VESCTOOL, the motor wizard  will let you specify your motor's weight. My specific motor is between ~200 and ~750 (my memory could be wrong on this) but anyway, I told VESCTOOL that my motor's weight was ~750ish. I'm suspecting that this could be the reason why my motor was cogging.

Now, I've ran on BLDC for a day and tried to do some serious hill climbing tests and it was ok but not too impressive. I felt that the starting torque was weaker on BLDC vs. FOC - I digress, the point is that I didn't experience cogging on that day.

A few days ago I decided to go back to VOC but this time I told VESCTOOL motor wizard that my motor's weight was~200ish. And what do you know...it has been raining since then and I couldn't try out the new VESC setting.sheesh.

I'm waiting for good weather to see how this VESC with these settings will work on the long run. I'll report back when I've ran it everyday for a week or so.

I had a HK VESC 4.12 prior to this one.on FOC last year since day one with exactly the same motor and lipos running perfectly. Only difference is VESCTOOL version and maybe VESC FW (sorry, can't remember VESC FW verion on my HK VESC)
```

---
## \#23 Posted by: slick Posted at: 2019-05-07T20:06:30.967Z Reads: 90

```
Reporting back...

So, I got some km with my Flipsky running on FOC.
I still have it on the same setup - sk3 aerodrive 5065/275KV , 8S1P Lipo, 1:3 / 83mm wheels. I was having **no problems** since my last VESC-Tool setup. 

**BUT** 

I realised today that I overlooked my motor was only pulling 30 amps max. My motor can take a max. load of 65 amps (i think) according to the datasheet. So essentially, I was only running at roughly 50% motor power output :rofl:

And I thought to myself  "man, this VESC feels lame ! gotta step up a notch...maybe LiPos are dying on me?" :rofl::rofl:

So, here I am waiting for another day to come - I´m sure It´s gonna be fine though...be back after a fey more km to confirm this VESC´s reliability on FOC.

see ya,:
```

---
## \#24 Posted by: murdomeek Posted at: 2019-09-10T21:03:16.091Z Reads: 52

```
did anyone confirm if flipsky 4.12 VESC can run on FOC 10s reliably?  My motor will be low Kv so hitting the Erpm limit wont be an issue

I'm talking about these ones or equivalent: https://flipsky.net/products/torque-esc-vesc-%C2%AE-bldc-electronic-speed-controller
```

---
## \#25 Posted by: visnu777 Posted at: 2019-09-10T21:25:45.859Z Reads: 51

```
Yes, I do.
```

---
## \#26 Posted by: murdomeek Posted at: 2019-09-11T00:06:46.849Z Reads: 50

```
thanks! 
10char
```

---
## \#27 Posted by: semiStationary Posted at: 2019-09-11T03:00:25.328Z Reads: 52

```
I've been running a Flipsky dual 4.20 for 5 or so weeks, over 100 miles easy. I also live in the mountains of PA, so I'm usually riding steep hills. I have an large offroad board with 8" tires. I've been nothing but impressed with it. It's almost more performance than I can utilize.
```

---
## \#28 Posted by: Movation Posted at: 2019-09-11T05:04:19.430Z Reads: 51

```
Have a 6.6 Plus 3 months now, 12S & 13S packs.
Duel 6354 FS motors, Abec 107
so far flawless. 
Issues with older FS 6 Vesc was 2 of mine singles have dead anti-spark switches, easy to bypass.
Building a eloft DD with 4.12 dual Plus atm.
Wont see the 13S pack, maybe 12S and 10S x 26650
rule of thumb with FS dont early adopt, they do sort their **** out eventually.
See VX2 fiasco, early 6.6 singles popcorn A/S
```

---
## \#29 Posted by: Tinp123 Posted at: 2019-09-11T05:41:40.034Z Reads: 51

```
using cheapest flipsky 4.12 in dual, 30A battery each and 60A motor each in FOC, never had any problem/overheating. and they do have power (I have 12s setup too so I can compare)
```

---
## \#30 Posted by: murdomeek Posted at: 2019-09-11T17:48:37.148Z Reads: 41

```
thanks everyone for your answers :)
```

---
