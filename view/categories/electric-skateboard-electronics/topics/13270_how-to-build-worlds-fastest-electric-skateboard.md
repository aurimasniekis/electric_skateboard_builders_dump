# How to build world&rsquo;s fastest electric skateboard?

### Replies: 32 Views: 3954

## \#1 Posted by: flash Posted at: 2016-11-18T13:04:15.995Z Reads: 375

```
If your goal was to simply build a electric skateboard for world record speeds(60 mph+) how would you do it?
```

---
## \#2 Posted by: im-done Posted at: 2016-11-18T14:00:30.391Z Reads: 371

```
Castle creations mamba monster motor x4 with a 2:1 redution. I would also use nematic wheels for a more stable ride. Mamba monsters are 6s 200 amp 2,200kv motors. They claim they have 5hp each so x4 with that low of a reduction you should be fine and now you just need a battery that can handle a 800 constant amp draw. 

But at 60+ mph cracks in the pavment = death.
```

---
## \#3 Posted by: TarzanHBK Posted at: 2016-11-18T14:11:22.295Z Reads: 368

```
12s battery
12s escs
2x 300kv motors
16/32 geering
100mm wheels
62mph
```

---
## \#4 Posted by: evoheyax Posted at: 2016-11-18T15:26:12.850Z Reads: 346

```
I'm building one right now...

With 4x carvon v2's at 12s with a chaka quad vesc. My theoretical top speed will be 72 mph...
```

---
## \#5 Posted by: Jinra Posted at: 2016-11-18T15:37:22.566Z Reads: 329

```
It gets exponentially harder to overcome resistance after 30~mph. You'll probably be limited to a lot less than 72mph.
```

---
## \#6 Posted by: evoheyax Posted at: 2016-11-18T15:41:34.648Z Reads: 321

```
Yea, that's the problem with these insanely fast boards. But I think 55 ish will be possible, maybe 60 in the right wind conditions (i.e with a strong wind on my back, haha). I did 38 mph with a dual and the needle was flying up on my speedometer.. If I had more space, I could have hit 45 in less than a second more of acceleration, no doubts. 4wd should help with the wind.
```

---
## \#7 Posted by: ra.rend Posted at: 2016-11-18T16:17:30.636Z Reads: 307

```
Get rid of the rider
```

---
## \#8 Posted by: Namasaki Posted at: 2016-11-18T16:36:19.204Z Reads: 306

```
P[quote="evoheyax, post:4, topic:13270, full:true"]
I'm building one right now...

With 4x carvon v2's at 12s with a chaka quad vesc. My theoretical top speed will be 72 mph...
[/quote]

I ran dual V2's at 12s. 
The fasted I got was 33 mph.
Theoretically, adding motors does not increase top speed on flat
```

---
## \#9 Posted by: evoheyax Posted at: 2016-11-18T16:45:47.024Z Reads: 295

```
Like I said, I did 38 mph with plenty of room left (the torque at 30+ starts to get really good). With more motors, I hope to eliminate the VESC overheating I have experienced most importantly, but also, help fight the wind a bit better. The problem is, finding someone with enough balls to push it to it's speed limit... Cause I don't even want to do 50 mph, haha. Maybe with leathers (which I don't have), but even then...
```

---
## \#10 Posted by: Namasaki Posted at: 2016-11-18T17:27:12.927Z Reads: 279

```
I never ran my V2s with Vescs. 
I was using TB ESC's and mini remote. 
I found that when I switched from TBESC's
To Vescs with my belt drive system that I had a gain in top speed of at least 5 mph. 
I've also heard that the  GT2B controller gets substantially higher top speed than the mini remote.
```

---
## \#11 Posted by: evoheyax Posted at: 2016-11-18T17:41:11.829Z Reads: 263

```
I can see maybe the esc having some effect on top speed, but I can't see why a controller would get a higher top speed. If you configure it correctly under the ppm mode tab, you should be capable of the same ppm range, and thus, you shouldn't get any difference in remotes, other than the acceleration and braking curve. But those shouldn't affect top speed.
```

---
## \#12 Posted by: FredSaberhagen Posted at: 2016-11-18T18:07:10.415Z Reads: 250

```
When you look at the curve of a motors power and torque output it's dropping as you reach higher speeds.  You are linearly _losing_ torque as your torque requirement _increases_ with the square of velocity.  I'm not sure the easiest way to do this is with conventional BLDCs turning the wheel :-)  Since we have such small wheels.

I'm not being flippant or joking when I say I think the easiest way to build the fastest esk8 is by putting fucking jets on it.

Alternatively, some sort of variable gearing system would work if you could fit it in our form factor.  There was just a thread about CVTs on here a little while ago.  Keep your watts in the best spot of the power band throughout.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-11-18T18:41:31.163Z Reads: 233

```

Mobutusan
Regular
4d
@Namasaki Just out of curiosity, were you using the TB mini remote when you got those results? I ask because when I ran those same two 230kv motors on 12s with TB 12s esc's and 14/36 gearing on 83mm wheels with a GT2B, I hit 30mph on a full charge and still had a little extra throttle left (I got scared and backed off, but I'm guessing it could have gotten up to 32+mph, at least). When I swapped the GT2B out for the TB mini remote, making no other changes, on a freshly charged battery, I had the throttle pegged and only got up to 28mph. This is using the same two gps speed/tracking apps on the same stretch of flat bike path, and the only change/variable was the different remote. I fiddled with the trims, re-paired the mini remote many times and same result. And I'm around 75-80kg fully loaded when I ride.
```

---
## \#14 Posted by: Mobutusan Posted at: 2016-11-18T18:42:59.752Z Reads: 221

```
I can also confirm a drop in top speed after switching from the GT2B to the mini remote, at least on TB 12s esc's. I went from a top speed of around 33mph down to 28mph after the switch, making no other changes, and each time on a fully charged battery. Interestingly enough, my bench tests with a hand held tachometer revealed that swapping channels from the trigger to the steering wheel resulted in an increase of around 300rpm, unloaded. I haven't tried the steering wheel throttle in the street yet, but I'm suspecting that the mini remote trigger throw might be physically limited by the case or something. It's just a theory at this point though. I'll keep investigating this issue.
```

---
## \#15 Posted by: evoheyax Posted at: 2016-11-18T18:52:32.324Z Reads: 212

```
I am using the mini remote. I wonder now if I could get more speed with the gt2b... I might have to try it... It might just be the TB ESC though. I always use the vesc...
```

---
## \#16 Posted by: Jinra Posted at: 2016-11-18T18:55:57.432Z Reads: 216

```
Since it's current conrol (vs duty of TB's esc) it won't make  difference. Throttle commands only up the current being supplied, so unless you're not supplying enough current to drive max rpm, controller doesn't matter unless you set it up very wrong.
```

---
## \#17 Posted by: FredSaberhagen Posted at: 2016-11-18T20:33:27.457Z Reads: 203

```
It could be the trim for the throttle channel is set lower?  if you have a scope it would be cool to see the difference at the Rx in PWM duty cycle.
```

---
## \#18 Posted by: longhairedboy Posted at: 2016-11-18T20:44:07.898Z Reads: 200

```
60+ mph is completely insane. I can't imagine building a board like that. I can barely stand 35mph, but i'm also not a downhill guy. Those clowns routinely hit 70 and up.
```

---
## \#19 Posted by: ddoke25 Posted at: 2016-11-19T01:23:42.334Z Reads: 191

```
Did a lot of downhill back in high school/ some in college. 60mph is a little on the fast side, even with precision trucks and the correct setup, but cruising 45-50 mph is where all the fun is at.  My Raptor was pretty exciting for the first couple weeks but I am looking to speed it up. Any suggestions other than increasing wheel/ pulley size?
```

---
## \#20 Posted by: Pantologist Posted at: 2016-11-19T03:10:08.566Z Reads: 185

```
You guys are all crazy! I'm scared to go above 25 mph on a longboard. :stuck_out_tongue:
```

---
## \#21 Posted by: saul Posted at: 2016-11-19T03:48:45.569Z Reads: 177

```
I used to think the same thing and now after riding everyday 20mph feels slow and 25 is felling more normal :joy: (Tears from wind in my eyes...)

anyways there was that unoffical video of someone doing 68mph...

but yea with some heavy duty 4x v2 carvons  on 107mm flywheels with 14s2p(140A cont.) LiFe a123 cells + lightish rider + mythically perfect roads == ++70mph
```

---
## \#22 Posted by: Pantologist Posted at: 2016-11-19T03:54:47.211Z Reads: 176

```
Most people die in car crashes at 60mph+ 

You'll definitely be dead at those speeds if you fall off and strike something at that velocity.

The expense and risk is not worth it even though it is probably equal in fun to downhilling.
```

---
## \#23 Posted by: saul Posted at: 2016-11-19T04:03:43.957Z Reads: 181

```
https://youtu.be/7cLF18RFCl0?t=6m


your probably right...lose the motors..find a hill  and you can hit 90mph ;)
```

---
## \#24 Posted by: evoheyax Posted at: 2016-11-19T04:38:41.357Z Reads: 179

```
[quote="Pantologist, post:22, topic:13270"]
You'll definitely be dead at those speeds if you fall off and strike something at that velocity.
[/quote]


True, but you can fall at those speeds and not die if your in the right environment, case in point, Mischo Erban falling while breaking the record...

I think anyone who does above 40 mph without leathers is crazy, but with leathers, you can fall at 60 mph and be fine, if you don't hit anything...
```

---
## \#25 Posted by: NNGG Posted at: 2016-11-19T06:52:56.389Z Reads: 174

```
Could you plank on the board? that would reduce wind and air resistance?
```

---
## \#26 Posted by: Dornacht Posted at: 2016-11-19T15:45:49.334Z Reads: 163

```
Then I would just convert a street luge to electric, if I wanted to hit thoes speeds.
```

---
## \#27 Posted by: GhettoFab.rictation Posted at: 2017-11-07T07:11:11.624Z Reads: 126

```
Why not build a transmission with just two gears and using longer board with wider trucks would help but I'd love to see a transmission setup
```

---
## \#28 Posted by: squishy654 Posted at: 2017-11-07T18:01:09.272Z Reads: 119

```
That's not a bad idea, just need a tall flag pole so the cars could see ya lol..
```

---
## \#29 Posted by: longhairedboy Posted at: 2017-11-07T18:04:21.080Z Reads: 124

```
last time i got in touch with NGV and then modified thier system to run on a custom deck shaped like a sword. 

Next time i'll probably get some hummies and run quad focboxes at 13S. Then I'll build the same board with carvon direct drives and do some comparisons. 

To be clear, i will be doing comparisons of some other damned fool's experience doing 65 because 40+ is fast enough for me. fuck 65.
```

---
## \#30 Posted by: hackware Posted at: 2017-12-17T18:24:29.830Z Reads: 100

```
could one of you guys share a quad-focbox setup...?

I'm working on a 4 x 10" hoverboard motor-wheel (700W each)  design for a farming assistance robot...

what i'd like is for my pi clone (asus tinkerboard (2gb)) to control the final drives...

as space constraints and weight limits are not a factor (extra weight is actually a plus), i plan on using 3 (or 6) marine deep discharge batteries for power...
(with super-capacitor battery banks if needed for power surge requirements)... 

as a robot, reverse under full power is also required...

a bonus would be to control 2 or more extra focboxs for implement drives on top of the 4wd...
(think mini-tractor)...

[ mississippi backwoods hacker/tinker ]

william...
```

---
## \#31 Posted by: faithfulpuppy Posted at: 2017-12-17T19:55:32.280Z Reads: 88

```
should be relatively simple, the FOCBOXES are highly programmable. I don't know the technical specifications of 2.4ghz radio receivers but all you'd need to do to control the FOCBOX is feed to it a PWM signal varying between 1 and 2 ms. (anybody who actually knows what they're talking about feel free to correct me)
```

---
## \#32 Posted by: Sunbum79 Posted at: 2018-05-20T01:34:23.075Z Reads: 59

```
Holy crap 70!!
```

---
