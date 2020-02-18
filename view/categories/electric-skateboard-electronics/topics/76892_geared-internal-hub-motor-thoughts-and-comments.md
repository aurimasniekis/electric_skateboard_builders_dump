# Geared internal hub motor ? Thoughts and comments

### Replies: 34 Views: 797

## \#1 Posted by: Simon-R Posted at: 2018-12-03T08:36:29.840Z Reads: 249

```
What are your thoughts on the geared hub motors like the new Zenboard will have ? ( not gear drive power)
I'm not enthusiastic about the 'no remote' set up but I'm curious about the geared hub motor it will use 
https://youtu.be/L5Sys_U94lc
```

---
## \#2 Posted by: AntiumOne Posted at: 2018-12-03T08:56:18.095Z Reads: 244

```
I'm a fan of the idea. It combines the advantages of a gear ratio with the stealth of hubs. If they can get a good amount of high quality urethane on the wheels, then they could have a winner.
```

---
## \#3 Posted by: linsus Posted at: 2018-12-03T09:14:28.463Z Reads: 239

```
stary had the same concept. The board was never released and ended up scaming tons of ppl. The few videos i saw, it was noisy asf. Idea is great, real application, not so easy to solve.
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-12-03T10:05:10.713Z Reads: 228

```
Hubs and gearing Sounds good. But all that Takes space. Dunno how it will perform. All that stuff in a wheel.....
```

---
## \#5 Posted by: linsus Posted at: 2018-12-03T11:57:47.455Z Reads: 219

```
performance wont differ from any other geared system. This case would be planetary gears and a motor ontop. Preferably helical geared. However, price on one unit would be ridiculous.
```

---
## \#6 Posted by: Vanarian Posted at: 2018-12-03T12:22:59.689Z Reads: 210

```
I call @Frank forth on thy matter!
```

---
## \#7 Posted by: Hummie Posted at: 2018-12-03T14:35:26.511Z Reads: 200

```
Small motors.  They made a fortune already though with practically no facts on their site.  I think the few facts I heard were 1500 charge cycles with Li-ion battery and 22 miles while super light!.  Bull
```

---
## \#8 Posted by: Friskies Posted at: 2018-12-03T15:36:25.953Z Reads: 184

```
![image|230x500](upload://5JUeDewGbMfZCvqABwHCCf4HPDx.jpeg) 
Awesome concept but they might be selling some free snake oil with those specs.
```

---
## \#9 Posted by: Hummie Posted at: 2018-12-03T16:02:22.988Z Reads: 173

```
Seems they said lithium iron so maybe possible to get that many cycles.  Australian accent!

But half the weight of the raptor, while using Li-iron cells especially, sounds like they’re missing something you might want.
```

---
## \#10 Posted by: Friskies Posted at: 2018-12-03T16:25:19.237Z Reads: 171

```
35km range out of a 225wh battery and 40km/h with those tiny motors...Not to mention you'd have to be Incredibly brave or maybe a bit stupid to ride any board at that kind of speed with no remote.
```

---
## \#11 Posted by: Sn4pz Posted at: 2018-12-03T17:29:45.844Z Reads: 165

```
with a rating of 6.4kw per km.... :rofl:

what the hell
```

---
## \#12 Posted by: evoheyax Posted at: 2018-12-03T18:59:45.935Z Reads: 158

```
It's an awesome idea on paper, but to fit the gears inside, you'll have a tiny stator that will over saturate and heat up like there's no tomorrow. If it was a centrax wheel width, you would still have a small stator, maybe around the size of hummies first hub motor. And they don't seem to be nearly as wide. So I would guess their stator is very small.

And 22 miles on 222wh? What are they smoking? Cause I want some of that! 10Wh per mile would be the lowest of any hub motor ever made.

It's the normal marketing bull you see with every campaign. Over promise and under deliver. Nothing new.
```

---
## \#13 Posted by: evoheyax Posted at: 2018-12-03T19:09:52.857Z Reads: 155

```
After looking into it some more, this total BS.

**Hill Climbing:** Zenboard's dual ArcDrive motors give you the power to coast up 30% grade hills with ease.
https://ksr-ugc.imgix.net/assets/023/314/874/4b1a37c2db71cca0533634843b21d5cd_original.gif?ixlib=rb-1.1.0&w=680&fit=max&v=1542631097&auto=format&gif-q=50&q=92&s=d1ed9480b65e2988f6ca2a4e08c45c90

Does that look like 30% grade to you?

That looks like at best 8% grade, and it struggled... I 15% is actually pretty steep. This is blatant false advertising. Range, you can argue about and it'll always be ambigous. But I'm smoking the wrong stuff if that's a 30% grade hill.

Here's a real 30% grade hill:
https://upload.wikimedia.org/wikipedia/commons/f/fc/House_at_Baldwin_Street.JPG
```

---
## \#14 Posted by: Jmding Posted at: 2018-12-03T19:23:47.885Z Reads: 150

```
Looking at this picture:
![image|680x453](upload://8i0vwLDDVdCqK0HP2BhhrAoKBgN.jpeg) 

and based on the known wheel diameter of 85mm, it appears they are using a 40mm diameter stator. Looking at this picture:
![image|680x481](upload://m89Q2F53AvYAw6V5hNxgTvlU4jC.jpeg) 

we can guess that it might be something like a 40x25 stator. That's basically what you'd find in a 5045 motor. 25 mph with 3:1 gearing, 12s LiFePO4 and 85mm wheels means roughly 200 Kv motors. For further context, Boosted runs what appears to be dual 5030, 200 Kv motors.

Agreed, 30% grade is almost certainly more than dual 5045 can handle, and its frustrating that they are exaggerating their performance characteristics so much.  But with 5045s, 3:1 gearing, and 12s LiFePO4 batteries, this thing will likely be a slight upgrade from a Boosted. Maybe not so interesting to DIY guys, but still quite competitive for the consumer market, which is much more in-line with the branding and design language anyway.



Another thought, from a heat perspective, 5045 200 Kv motors are good to about 35 amps, or 1500 Watts @12s. By comparison, hub motors built around 6374 motors at 75 Kv are good to about 30 amps or 1330 Watts @12s (unless they employ special strategies like heat pipes or higher temperature winding enamel). Overall the approach of using smaller motors with planetary gears is probably a smart way to go, if it is well implemented. And that's a big "if" of course, just look at the Stary fail.
```

---
## \#15 Posted by: evoheyax Posted at: 2018-12-03T19:36:36.481Z Reads: 142

```
The thing that is easy to forget though when comparing to boosted is the ventilation of that small motor. You can't cool hub motors the same way as belt driven motors (i.e. it's spinning in open air and constant airflow is cooling it). Hummie's small hub motors used a 47x25 stator, and those had serious over heating issues (especially if you are 200lb+), even in 4wd... I literally caught one on fire because it got so hot (in 4wd mind you), the enamel melted away and it shorted, catching fire (smoke was pouring out of it like crazy), haha.

Needless to say, I can imagine there will be many warranty requests due to motors overheating, and possible fires from them also.
```

---
## \#16 Posted by: dareno Posted at: 2018-12-03T20:13:02.508Z Reads: 137

```
Ok so we agree the math doesn't work.  How then did they achieve 37% funding in 2 days?  Who chucks money at a campaign with absolutely no real world testing?  Blows my mind tbh.
```

---
## \#17 Posted by: evoheyax Posted at: 2018-12-03T20:26:50.759Z Reads: 136

```
Because jayboston featured it (to his following of 17k subscribers) and didn't ask any of the hard questions.

Let's face it, this is targeted at people with no understanding of how electric skateboards work.

I have to say myself, it's a very clean design. But we are not there to make this happen in this form factor yet.
It's the problem we all face as builders: Aesthetics or Performance/Range? To really get 20 miles reliably with any sort of hills requires a second row of batteries (unless you've got a super wide press, like chaka), which instantly make the board super thick.

Not to mention, we've been there and done that with CF. I think it was pretty unanimous in the community, that CF only vibrates like a mofo compared to wood or a wood/CF composite.
```

---
## \#18 Posted by: Simon-R Posted at: 2018-12-03T21:29:07.889Z Reads: 125

```
Yep definitely  needs a remote.
```

---
## \#19 Posted by: vjsharpeyes Posted at: 2018-12-04T01:26:10.533Z Reads: 120

```
Its a really nice looking board. Will be interested to see how it pans out.

Personally the delay between the lean and actual results would have to be minuscule for me to be interested. 

Good luck to them.
```

---
## \#20 Posted by: chuttney1 Posted at: 2018-12-04T01:45:49.000Z Reads: 115

```
Starry Boards did use a planetary gear system, but there were issues with the design.
```

---
## \#21 Posted by: mccloed Posted at: 2018-12-04T01:51:54.056Z Reads: 104

```
Is that Filbert street in SF? I tried that hill and could not get enough traction on urethane.
```

---
## \#22 Posted by: mccloed Posted at: 2018-12-04T02:00:19.782Z Reads: 105

```
Another issue with the "no remote" boards is that they put the throttle in the front and the brake in the back. What do we do when we accelerate on our boards? We brace are back leg. What do we do when we hit the brakes? We brace our front leg. So, how is this going to be a comfortable transition?
```

---
## \#23 Posted by: alexnz Posted at: 2018-12-04T03:12:07.313Z Reads: 102

```
If the gearing provides 3 times the torque as a typical setup, how can you still achieve a similar top speed? 

Could it be that the Motor Design consultant presented on the KickStarter page is the chick from Maytech? 

Quite a few things seem to be overhyped, (weight, range, top speed?) which is unfortunate as this board looks pretty good and sleek in terms of design, and it's refreshing to see a team of Oz guys behind that. 
I'd be interested to find out how these pressure sensors react when you go over a bump, a curb, or simply when carving. The constant weighting and de-weighting would require a fair bit of smartness in the software.

Anyway, proof is in the pudding, and future will bring the truth out.
```

---
## \#24 Posted by: Simon-R Posted at: 2018-12-04T20:16:05.748Z Reads: 89

```
That's what I thought.
```

---
## \#25 Posted by: evoheyax Posted at: 2018-12-04T21:05:33.322Z Reads: 92

```
I think you a bit confused.

Motors in general have more torque when spinning at higher rpms and gear reduced that just at a lower kv.

The kv in the end will tell you the top speed. Higher = more top speed. Lower = more torque.

They uped the kv to something that would make a hub motor supper inefficient and weak, and by gear reduction, they increase the torque of the motor and turn it into an efficient motor again.

The idea is to get the torque of a geared system with the benefits of a hub motor. It's not a bad idea, but with a stator that small, you'll over heat quickly and it will become super inefficient. And heat in a motor is recursive exponentially. The current heat creates more heat, and that new heat can create even more new heat while the old heat still creates new heat, and it keeps compounding. 

If we merged a hummie hub with a system like this, we could have a killer efficient and powerful motor. But then there's two other issues.

First, gears are loud (look at @MoeStooge boards) unless in an enclosure with lube like @Kaly gear drives.
Second, gears, like belts, wear out, especially if they are not in an enclosure with lube. The idea of having to replace gears at best is annoying if designed well, and impossibly most likely in this case.

This is beyond the fact these motors are not sealed and have huge openings on the outside for debris to get into the motor and, most importantly, the gears, further accelerating wear.
```

---
## \#26 Posted by: epster Posted at: 2018-12-04T22:35:51.248Z Reads: 88

```
From a mechanical engineers perspective its a great idea! Planetary gears are perfect. They have really low friction and your gear ratio can be adjusted to whatever you like, and they can fit in small places because of the multiple planetary gears. However, The stators are way too small as mentioned earlier and should have been a lot wider. Judging by the design there is no to almost no airflow, so they will pop like popcorn probably. Unless they have some sort off safe switch.
Design is good and a super idea unless but personally I would have made the stators 1.5 to twice as big. Normally we calculate with a safety margin of 1.5-2 for such devices. Boosted has a margin of about 1.6 on the motors on their v2 dual + that makes it so reliable combined with the electronics. 
A good engineered device never outputs the full performance (unless you can engineer the rest so good that you can compensate for heat issues and such). Think about planes have a safety margin of 1.3-2.0. Because off their weight to fuel ratio, but they have these super in depth performance and in depth maintenance checks. Compared to a good reliable car which is only checked once every 2 or 3 years just to be sure sometimes there is even no need to do that.
So concluding. It's a great design it really is. But I think it just won't work with these design choices. Specs are weird and don't know why they trick people like that.
```

---
## \#27 Posted by: Jmding Posted at: 2018-12-04T23:09:51.517Z Reads: 80

```
Curious how you know about the Boosted safety margin? I ask because their motors look to me to be roughly 5025 externally (I'm guessing 4015 stators), and 200 Kv, and they're running them at up to 30A per motor. That seems if anything pretty aggressive to me, and (by my estimate) would be equivalent to running 5045 200 Kv motors at 45A, 6355 200 Kv motors at 70A, and 6374 200 Kv motors at 95A, generally a little higher than typical practice around here. It'd be awesome to up my motor currents by 10-20%.
```

---
## \#28 Posted by: epster Posted at: 2018-12-05T09:45:33.297Z Reads: 77

```
You are right. I wrote my post rather quick last night and i didn't really go in to that much depth and didn't describe everything in too much detail and got some things mixed up. The torque the motors produce is about 90% if their maximum. You can compare the BB stealth vs the v2 they have the exact same motors, but they still squished out about 6% more torque on the wheels. That's just turning the power a bit more open the result of changing some components but while compromising a bit reliability (still the chance that they break is really low). 
Still, they have rather a significant amount of margin left like they should. About 5-10% on the stealth motors (this is me guessing have had these motors too look at them but based on pictures performance and amount of issues they have with them and experience with other types of motors). Because when you design and calculate a motor you will over define it.
What i got mixed up was the motor safety margin (mostly about the electronics inside not the mechanical bits)  :smile:. Mechanical components simply just won't break in a good designed and made motor (think about parts like the axle). The electric components however cause the problems. They burn through and stuff. Or they get all fucked up and a mechanical component gets weakened by a side effect.
Concluding: on the mechanical components there is a safety Margin of minimal 1.5 to 2.0 Guessing and comparing it with other motors and such. However, the electronics just can`t handle more current or more current. So I was wrong in saying that it has a 1.5 over defined ratio because the mechanical components do however the electronics don't.
```

---
## \#29 Posted by: Jmding Posted at: 2018-12-05T16:17:36.187Z Reads: 60

```
That's an interesting perspective on it. I need to do more research to verify, but I can't think of the last time I heard of boosted motors having problems. That does seem to suggest that they, and we, are leaving some power on the table motor-current wise.
```

---
## \#30 Posted by: bevilacqua Posted at: 2018-12-05T16:54:05.378Z Reads: 60

```
Motors don't like becoming hot, not because of the winding epoxy threshold but because of the demagnetization effects happening in the PM + added resistance + iron-hysteresis. Its all added losses
```

---
## \#31 Posted by: Jmding Posted at: 2018-12-05T21:41:51.645Z Reads: 55

```
@bevilacqua, do you have a good way of estimating the amount of power being lost to iron-hysteresis? I've been trying to figure out this piece of the puzzle for a while but haven't found the right resource yet.
```

---
## \#32 Posted by: bevilacqua Posted at: 2018-12-05T21:55:28.108Z Reads: 54

```
No, I will look it up in my uni scripts tomorrom, maybe I find something on smaller PMSM motors. If not I might write an email to the professor/assistants
```

---
## \#33 Posted by: Michaelinvegas Posted at: 2018-12-05T22:20:38.137Z Reads: 46

```
[quote="mccloed, post:22, topic:76892"]
Another issue with the “no remote” boards is that they put the throttle in the front and the brake in the back.
[/quote]

Lol...I have a Board that we will review has this same control set up....It’s single hub and very difficult to ride comfortably
```

---
## \#34 Posted by: Anubis Posted at: 2018-12-05T23:30:36.704Z Reads: 40

```
- No remote
- Thin PU
- Not even better torque than chinese hubs
- really, REALLY LOUD
- super expensive hubs
- Comparable performance to a $800 board
```

---
