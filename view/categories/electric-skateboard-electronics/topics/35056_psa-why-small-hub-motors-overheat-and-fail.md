# PSA: Why small hub motors overheat and fail

### Replies: 221 Views: 8961

## \#1 Posted by: evoheyax Posted at: 2017-10-07T21:52:35.940Z Reads: 491

```
Many people on this forum will buy the cheapest parts they can find. This may be on ebay, or even known vendors who are on this forum.

Hub motors, being relatively new technology, is in high demand right now. They are simpler (less maintenance, which is almost none), can be just as efficient as belt drive setups (raptor 2 for example), and are stealthier (No belt and pulley system, and supports FOC better, since they run at a lower erpm, which means almost no noise).

There are cons to hubs also, such as the lack of gearing (which means for speed freaks like me, more wasted battery and heat, since we need higher kv hubs to reach the speeds we want) and less urethane on hub wheels.

For most people though, hubs have become a more appealing choice, especially for new builders. Theres one problem though: **Almost all of the hub motors on the market today are simply too small.**

The reasons are simple:

- Small motors have small stators. The stator can become over saturated by the magnetic field, and they suffer from what I like to call the nuclear effect. More on this in a second...
- Small motors have little copper in them. What this means is they heat up quicker.
- Small motors use thinner copper strands, because of space issues. What this means is for the same fill, you have more insulation. The insulation on a 24, 22, and 20 awg wire are all the same, and despite a 20 awg only having 40% more copper than a 24 awg,  the 20 awg is rated at double the amps. The 18 awg is double the copper of a 24 awg wire, but is rated to 4 times the amps of the 24 awg. Why? Lower resistance and resistance is directly proportional to the amount of heat in the motor.
- Once over 130 F, your magnets strength drops quickly. Now you need more amps for the same power. More amps = more heat.
- Because of the combination of these three facts, the nuclear effect will drive the motor off the charts. This is why we see this difference in testings hummies hubs:

-old hubs: small stator, 15 turns of 24 awg, max temp of 260 F measured, will go higher if they didn't almost catch fire at this point
-new hubs: double stator length, 15 turns of 20 awg, max temp of 131 F.

Only 40% more copper and double the stator size, and we see all heat issues go away.

So what does this mean? Small motors are simply too small.

Now what do I mean by small hubs? I'm talking about jacobs hubs, maytechs hubs, koowheel hubs, and all of the direct from china hubs.

Now your asking yourself, why do so many people now make these inferior hubs? The answer is the same reason we have hover boards blowing up. Many manufacturers don't care about the quality of their product, and the ones that show they do, don't do adequate testing. For example, one manufacturer posted a video on youtube of their testing. Their test: 8 hours on a rack at full speed. The issue here, is that the current is very low without a load, fractions of an amp. With that low current, theres no way for the motors to get hot without a short in the motor. Compare that to the 20 amps you'll pull with them to go up a hill.

There's more to it than they don't care also. The terrain, riders weight, riding speed, and riding style play a huge role in how many amps you'll draw. On hummies small motors, I used to pull 4 amps on flat, and 10-15 on small hills. When you live in an area full of hills, you can see you'll generate 3-4 times the heat than when in a flat area. This means 20-25% of the range you'd expect to get also.

Some riders do ok with these small hubs, as they weigh 130 lb or less, and ride at speeds under 10 mph, on flats.

However, if you plan to ride on hills, are more than 130 lb, and like to go over 10 mph, you'll find these small hubs heat up quickly.

Some, like NVG, claim to have mastered the small motor, but why? Because they can do high heat, not because they have some magic way of cooling them. **This is no solution, because once they got hot (which is quickly because of the little copper), you need more amps to get the same power from the copper. The magnets strength weakens, and now you need more amps to get the same magnetic field. And finally, the stator gets over saturated very quickly, which now means heat goes off the charts.** Running a motor hot is not a solution to anything, because heat, creates more heat, which creates more heat. For programmers like me, this is the classic case of recursion with no base case. you end up with an exponential function of heat generation.

The solution? Simple... Bigger hubs. With hub motors, bigger, is simply better.

Now, why aren't there more big hubs on the market?

- Those in china producing and seller straight from the manufacturer are trying to be first to the market. Even if that means they poorly engineer them, and do no real tests on them to see how they perform, only that they work on a bench.
- Bigger hubs need a custom truck. Why? Because the wheel base will be wider, you need to push them towards the center on the hanger more or your going to have a ridiculously wide wheel base.
- Designing a new truck, in addition to the longer or wider hub, takes time, and they don't want to wait. They want to sell now. It also costs more, and looks less attractive to customers who don't know any better about hubs.

Now what does this mean?

As builders who want to use hubs as this time, unless your a slow, light rider who rides short short distances on flat, you have 3 options for hub motors:

- R-Spec hubs (not sold separately, must buy raptor 2 complete)
- Hummies NEW double wide hub motors
- Carvon v3 or v4

If you feel like wasting your time and money, go ahead and buy small motors from vendors, on ebay, or straight from china, but I'm tired of seeing threads on here and get messaged by people who buy these small motors from china and are surprised that they failed. Now you know why they fail, so either you head this advice, or you risk wasting your time and money. The choice is yours...
```

---
## \#2 Posted by: jrpwit Posted at: 2017-10-07T23:04:31.267Z Reads: 403

```
Bigger is always better! 

One question though. What are the benefits of having more poles on the stator? I have noticed that the rspec hubs have a lot more than carvon's.
```

---
## \#3 Posted by: Jreamer Posted at: 2017-10-07T23:08:48.625Z Reads: 398

```
Well put.

I have found the meepo hubs are pretty fkin good though. I am 260 and I have a 10s4p 8.8ah pack and I ran it from 100-0 mostly up and down 5-10 percent gradient till the battery died and the hubs where not that hot. These 90mm hubs are massive and the esc limit the speed to 22mph so they are not the best performer, but they are very good intro hubs.

I am buying 2 of the 3 hubs(Hummie/enertion) you mentioned cause I am heavy and do want to go fast, but I must say the 90mm meepo hub is pretty good for the money. It works for me at 260 where as the backfire 2 motor kinda doesn't. For heavy guys looking for a cheaper option, these hubs work well.
```

---
## \#4 Posted by: evoheyax Posted at: 2017-10-07T23:45:47.139Z Reads: 368

```
The stator hummie is using now is big enough. It's narrow though, and the space inside for copper grows exponentially when you increase diameter instead of length. But then your on thin thane... You can't win.

Your also limited in the stators not as large, so it can't produce the same level of magnetic field. At some point, more copper on the same sized stator causes the nuclear effect. There must be the right balance.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-10-07T23:49:00.519Z Reads: 349

```
[quote="jrpwit, post:2, topic:35056"]
What are the benefits of having more poles on the stator?
[/quote]

Not really sure yet... We know more poles means more iron losses due to the constant flipping. But we have had at least 5 serious engineers tell us that doing 24 instead of 12 does not mean more torque. Possibly, it will find it's position better when starting (less cogging), but with sensors, that's eliminated. We will work on that more and are open to any engineers who want to share there opinions...
```

---
## \#6 Posted by: Cobber Posted at: 2017-10-08T00:31:39.773Z Reads: 333

```
Love all the data in your post dude!

Does anyone actually know what size motors NGV used? The wind your own scorp. kits when wound at the factory weigh 658/660/664g a piece, with heli. guy on the forums saying custom winds fit a bit more copper again ~700g... 

How many poles and slots are you using now?
12n14p is the popular choice for aircraft and effeciency
whereas 12n10p  is used for a lot of the heli motors that focus on power/weight
and then the 1/5 car guys are running 4 poles and 12-24 slots...

no real consensus
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-10-08T01:08:15.466Z Reads: 318

```
[quote="evoheyax, post:1, topic:35056"]
There are cons to hubs also, such as the lack of gearing (which means for speed freaks like me, more wasted battery and heat, since we need higher kv hubs to reach the speeds we want)
[/quote]
How would belt drives/gear reductuon help acheive high speeds? Seems hubs will always be fastesr at given KV unless people start building 1:1 or overdriven belt drives. 

Why would a 50mph hub board be any less efficient than a 50mph belt drive? The belt drive would need double to triple the KV to achieve the same speed right? So wouldnt losses be similar?
```

---
## \#8 Posted by: NNGG Posted at: 2017-10-08T01:40:05.403Z Reads: 306

```
You are also forgetting something very important, 
There is very little heat dissipation in hub motors and little airflow. My aluminum motor mount is very hot always and no doubt my exposed SK3 motor can breath cool air and it carries all of my weight with a 3:1 reduction, You will want to over design any hub motors in order to overcome these flaws.
```

---
## \#9 Posted by: BigBoyToys Posted at: 2017-10-08T01:57:14.861Z Reads: 294

```
I agree with your statement about hubs trapping heat, what I was questioning was the idea that hubs lose more energy too heat than a belt drive geared for the same high speed.
```

---
## \#10 Posted by: evoheyax Posted at: 2017-10-08T02:03:54.922Z Reads: 293

```
You can do an efficient gearing to 40 mph as far as I've seen (look at chakras free ride for example, with those tiny motors.

Hubs have 2 issues, one being they need a higher kv to run more efficiently, and the other is they cool while spinning in te open air. Colin is hard in hubs, which creates a bigger issue.

As @NNGG said, hubs will always need to be over engineered. But over engineered doesn't mean more exspensive. Take gummies hubs. We recently found mjnor changes to the design that resulted in huge reduction of machining costs. This means we can afford to give better prices than we should be charging for motors this size. Not everyone has a motor working well enough to optimize. It's been years of refining, and t will take China years to do the same, as many are just starting. if they ever do catch on.
```

---
## \#11 Posted by: jmasta Posted at: 2017-10-08T02:56:54.448Z Reads: 271

```
This smells like a preamble for an upcoming product launch
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-10-08T02:57:56.496Z Reads: 275

```
[quote="evoheyax, post:10, topic:35056"]
Hubs have 2 issues, one being they need a higher kv to run more efficiently,
[/quote]

What do you mean higher KV? Higher than what? What KV does the ollin board use to acheive 40mph? I hit 40mph on 110-130kv hubs, are you saying his motors are lower KV than that? Or am I missing the point?
```

---
## \#13 Posted by: evoheyax Posted at: 2017-10-08T04:07:18.167Z Reads: 273

```
[quote="jmasta, post:11, topic:35056, full:true"]
This smells like a preamble for an upcoming product launch
[/quote]

You can call it what you want. I'm just trying to share my research and development with the community. Do don't have anyone else here sharing their secrets... Enertion won't even tell me the size of their stator, while carvon isn't sharing anything about their research and development. We have spent 10's of thousands of personal money developing this, and I'm giving china the answer to their problem. Because I'm honestly tired of all the junk that's on the market today. The vast majority of it, especially outside of this community. Out profits on these motors is not high, it's just enough to keep researching and developing. There's no classes about how to build or assemble motors. It takes time, money, and a dedication. I belief we have one of the solutions. I'm not bashing everyone though, and saying we are the only option. I'm opening admitting that the carvon and r-spect raptor 2 motors are good also. You don't and won't see others doing the same.
```

---
## \#14 Posted by: Cobber Posted at: 2017-10-08T04:26:19.648Z Reads: 263

```
[quote="jmasta, post:11, topic:35056, full:true"]
This smells like a preamble for an upcoming product launch
[/quote]

well loopy has lead the way...

[quote="evoheyax, post:13, topic:35056"]
You can call it what you want
[/quote]

First up I'll say I think Hummie works hard to make a better product, and he is doing a lot of things I like a lot!
and as before thanks for all the solid info but jmasta does kind of have a point.
From the tittle this does come across a bit like some sort of stunt Jason would pull. Maybe instead of bagging everyone else just let us all know why what you have discovered works... a bit more factual, less conjecture, think of it like a research article.

[quote="evoheyax, post:10, topic:35056"]
they need a higher kv to run more efficiently
[/quote]

lastly
and ill quote Hummie here:_"kv is kv"_
```

---
## \#15 Posted by: psychotiller Posted at: 2017-10-08T04:33:09.284Z Reads: 242

```
With all the hype around the ngv rig I think this post was completely relevant. "Urethane on hub" is still a huge weak link though.
```

---
## \#16 Posted by: Cobber Posted at: 2017-10-08T04:35:30.683Z Reads: 251

```
[quote="psychotiller, post:15, topic:35056"]
"Urethane on hub" is still a huge weak link though.
[/quote]

agreed

but as per above the hubs might weigh 700g sans thane.
is that small?
```

---
## \#17 Posted by: psychotiller Posted at: 2017-10-08T04:36:28.179Z Reads: 255

```
Certainly weighty.
```

---
## \#18 Posted by: evoheyax Posted at: 2017-10-08T04:41:31.085Z Reads: 258

```
[quote="psychotiller, post:15, topic:35056"]
"Urethane on hub" is still a huge weak link though.
[/quote]

yes and no. If your hub is small and long, you can still fit 23mm of urethane on every side of the hub and have an 83mm wheel. 28mm and we have a 90mm wheel. Much better than a wide hub. This is why every solution is different. I believe we all have working options, but they are all very different at the same time. There's no one size fits all solution, and everyone will need to find what works best for them.
```

---
## \#19 Posted by: Cobber Posted at: 2017-10-08T04:45:38.075Z Reads: 252

```
have you thought of using some kind of bridged core like a tang, flywheel... it would help with reducing the transfer of heat... increase air flow...
makes it bigger but if it solves a problem?
```

---
## \#20 Posted by: evoheyax Posted at: 2017-10-08T04:56:54.310Z Reads: 246

```
I think we would lose too much space. Wheel size would need to go up to around 100mm and even then, thane would be super thin. I'll do a better analysis though, thanks for the idea.

Really, the point of this was to share that bigger prevents heat in the first place. I think that it's better to prevent heat, than to deal with dissipating it. Once you move up to a motor around this size, heat doesn't build up the same way and active cooling is not needed. More thane ;P
```

---
## \#21 Posted by: Cobber Posted at: 2017-10-08T05:02:09.818Z Reads: 220

```
yeah Hummies current in progress hubs look better than any others I've seen, first I have been interested to learn more about... I'm still on the fence though :stuck_out_tongue_winking_eye:
```

---
## \#22 Posted by: evoheyax Posted at: 2017-10-08T05:08:50.406Z Reads: 229

```
[quote="BigBoyToys, post:12, topic:35056"]
What do you mean higher KV? Higher than what? What KV does the ollin board use to acheive 40mph? I hit 40mph on 110-130kv hubs, are you saying his motors are lower KV than that? Or am I missing the point?
[/quote]

First off, I'm not very experienced with belt and pulley systems. But my understandingBelt and pulleys generally run around 190 kv with a 2.5:1 gear reduction. If you want speed, you do a 2:1 gear reduction. You know from the hub motor world that a 190 kv motor is too high for a hub motor/direct drive motor. But reduce that by a 2:1, and you'd expect the same results as a 85 kv motor, right? Well, it's not really that simple. I don't understand it all myself when it comes to belt and pulley systems. But I have personally seen efficiency I can't comprehend with hubs so far. The stator of my original enertion motor is a fraction of the size of these small hub motors, yet far more efficient with a 2:1 I'm excited to do the first real measured range tests tomorrow with the new hubs. I believe I will see much better range due to far less heat loses. Might be able to get close to a belt drive efficiency. We'll see...
```

---
## \#23 Posted by: evoheyax Posted at: 2017-10-08T05:14:42.269Z Reads: 226

```
[quote="Cobber, post:21, topic:35056"]
I'm still on the fence though
[/quote]

The onces we are putting together right now are basically the old design, but longer and bigger outer bearing. The new ones are completely off the wall insane. But I think he's blended the best of the bike world mechanics into a hub motor. If all goes well, it will result in a motor that doesn't need loctite or anything to hold it together. This means easier to take apart, which is a huge plus for us, and end users who want to replace the big inner bearing. The design has also been optimized for machining. We worked with machinists to find changes that make it easier to machine. Those 14 grooves for the wheel, for example, are expensive cuts because they are round. Requires a higher axis cnc machine. We turned them to square, and the cost dropped significantly. This allows us to offer really good prices for what they are. We shall see in a few weeks when they send the first 2 samples. If all goes well, we will run with this design for sometime. I keep telling hummie, no more changes, and the next day, it's a whole new motor design, haha.
```

---
## \#24 Posted by: Cobber Posted at: 2017-10-08T05:22:31.217Z Reads: 212

```
[quote="evoheyax, post:23, topic:35056"]
I keep telling hummie, no more changes, and the next day, it's a whole new motor design, haha.
[/quote]

let him go bro...
such is the beast: _innovation_

look forward to seeing what you guys bring ;)
```

---
## \#25 Posted by: BigBoyToys Posted at: 2017-10-08T05:35:47.845Z Reads: 211

```
I would have agreed fully umtil recently. Now I belive other factors may have been contributing to the inefficiency we've seen from hubs thus far. The rolling resistance of hub thane has been terrible on every hub iteration Ive seen  to date when compared to the high quality  name brand skate wheels. So much so that its immediately noticable when kicking the boards. What convinced this was a huge factor was my range test with my Carvon V3's on 90mm flywheels. I got over 15 miles on 215whrs. That's better than a boosted board in eco mode and I weigh 285lbs.
```

---
## \#26 Posted by: Cobber Posted at: 2017-10-08T06:03:28.568Z Reads: 219

```
[quote="BigBoyToys, post:25, topic:35056"]
What convinced (me) this was a huge factor was my range test with my Carvon V3's on 90mm flywheels. I got over 15 miles on 215whrs. That's better than a boosted board in eco mode and I weigh 285lbs.
[/quote]

**_BOOM_** :anger_right:

https://youtu.be/LiQazjMVBMI

the big fella _brings the rain_

[quote="BigBoyToys, post:25, topic:35056"]
Now I belive other factors may have been contributing to the inefficiency we've seen from hubs thus far. The rolling resistance of hub thane has been terrible on every hub iteration Ive seen  to date when compared to the high quality  name brand skate wheels.
[/quote]

maybe someone could try taking a high quality skate wheel and build it around a hub, not just chop half of it out?

https://youtu.be/3R5gHF0vzew
```

---
## \#27 Posted by: b264 Posted at: 2017-10-08T06:19:20.180Z Reads: 214

```
14Wh per mile for 285lb of cargo is really good; were you driving "fun" or "eco" ?

Edit: said "range test" nevermind
```

---
## \#28 Posted by: BigBoyToys Posted at: 2017-10-08T06:29:11.034Z Reads: 212

```
Im not sure how much of the losses are coming from properties of the urathane itself vs the airgap that develops between the motor and the wheel vs increased resistance due to higher hub motor temp, but i think they are all big players in the losses we see in hubs. I think with good wheels and managable temps we should see hub efficiency surpass belt drives in some situations at least. Especially long rides with few stops at moderate to high speeds.
```

---
## \#29 Posted by: BigBoyToys Posted at: 2017-10-08T06:30:08.157Z Reads: 208

```
Yeah eco'ish. Average spees at the end of the test was about 13 if I recall correctly.
```

---
## \#30 Posted by: b264 Posted at: 2017-10-08T06:31:49.228Z Reads: 210

```
Oh ok.  I can pull off 15Wh/mi minimum (more like 18) riding like that but I'm 215 lbs, so yours is significantly better
```

---
## \#31 Posted by: Cobber Posted at: 2017-10-08T06:35:59.565Z Reads: 215

```
[quote="BigBoyToys, post:28, topic:35056"]
Im not sure how much of the losses are coming from properties of the urathane itself vs the airgap
[/quote]

I don't know either... but... if more thane is better why do some popular wheels have a core? it means less thane!
one possible answer: wheels are suspension to a large degree on a skateboard, does the core provide a different type of attenuation/dampening that is required???
alloy cores have been tried but don't seem superior or popular?

[quote="BigBoyToys, post:28, topic:35056"]
I think with good wheels and managable temps we should see hub efficiency surpass belt drives in some situations at least. Especially long rides with few stops at moderate to high speeds.
[/quote]

yeah, although I'm not sure a hub, even 4wd will be the fastest up Pikes

https://youtu.be/YIJiRh9hEGE
```

---
## \#32 Posted by: BigBoyToys Posted at: 2017-10-08T08:41:14.406Z Reads: 215

```
When I said proerties of the thane i didn't have thane thickness in mind as much as I did properties like rebound, but thane thickness also factors in per @ChrisChaput explanation.  Im just saying hub thane doesn't roll well and feels like lots of efficiency is being lost to friction from rolling resistance. 

Although Im confident that my 4wd hub boards have more than enough torque to climb pikes peak at 30mph, I wouldnt even try it. The pikes peak challenge is not a battle of efficiency or even power as I see it, its  purely a battle of heat management. Any of the hubs I have would heat up within the first few miles of the climb with me on them without a doubt, even with 4wd. If I race Pikes peak it will be on the 4wd trampa with 80mm motors Ive been working on for months 😉.

Ive never claimed that hubs have supieror heat management, they have obvious disadvantages in that area. However under low-med load cruising situations( at motor rpms within the efficincy range for its KV), where heat isnt much of a concern, the hubs should be more efficient since the motors do not have the frictional losses from the belts or from the higher motor rpm needed for a given wheel speed. I'll do some more logs with my V3's with whr comsumption overlaid on the video see if I can confirm this :).

Maybe @Hummie and @evoheyax longer motors will have what it takes though. Can we see expect to see those motors at the socal performance day next month at least if not Pikes peak?
```

---
## \#33 Posted by: guyguy Posted at: 2017-10-08T14:15:52.116Z Reads: 210

```
For some more stats on belt drive efficiency I get 12-13 wh/mile at high speed and can get as low as 8 wh/mile if I stay under 20 mph - this is all on flat terrain at 220-240lb (depends on what I'm carrying). This is on the freeride which uses a tensioner and the belts are run really loose. 

Just went on an R2 meet-up. Here's a shot so you can see motor size difference - even with my weight thermals have not become an issue. The low-end torque of the R2 was impressive, never felt that on a hub. 

<img src="/uploads/db1493/original/3X/5/3/5398546d808a1dbae9d1022d8fdf68d7241be4e7.jpg" width="690" height="460">
```

---
## \#34 Posted by: evoheyax Posted at: 2017-10-08T14:26:01.931Z Reads: 208

```
I think there are factors impacting the range of hubs that aren't existent in but what doesn't make sense to me is my first board. Enertion drive kit with a r-spec 2 motor. Top speed 20 mph, but riding at 20 mph most of the time, on a 201 Wh battery, I could get 7 miles of range on my route. With hummie hubs, I went down to 5 miles with a 403 Wh battery. I never really do range tests in the sense that I find the flattest ground, and ride slow for as long as possible. It means noting to me, cause I never ride slow, ever. I'm sure if I have, I'd see those numbers go way up. For example, I already found  pull 4x the amps going up the 10% grade hills. This should translate into 25% of the expected battery range is what you get, which, is about what I've always gotten. The question is though, how efficient can hubs get? I think very efficient. But it depends on the kv. 140 kv motor is more what I think we would like (carvon 2.5's for example). But you sacrifice low speed torque and efficiency.

I don't understand the gearing benefits fully, but I have seen a huge difference. Maybe these new hubs will change everything for me, we will see. Now that we have a core, we can make super nice wheels with great rebound. I road on a garbage road yesterday at around 25 mph, and hardly felt the vibrations. 

What I do know is the stator in the raptor 2 is half of the size of hummies original motors. But yet, I got way better range and they stayed so much cooler.

Maybe @chaka could chime in on the details of why belt drives are more efficient than hubs at higher speeds (40-50 mph). Belt drives are his specialty, while hubs are my specialty. I agree that we can bring efficiency up though to belt drives for lower speeds. I believe these new motors will do just that.
```

---
## \#35 Posted by: evoheyax Posted at: 2017-10-08T14:32:09.457Z Reads: 208

```
[quote="BigBoyToys, post:32, topic:35056"]
Maybe @Hummie and @evoheyax longer motors will have what it takes though. Can we see expect to see those motors at the socal performance day next month at least if not Pikes peak?
[/quote]

I will be bringing these motors everywhere I can. What I'm really excited about is the triple wide motors. We still want to bring those guys back. Hummie did simulations yesterday, and found the 12mm custom axle is 20 times stronger than a 8mm axle :P No motor motors snapping trucks like what happened before with the triple wide motors.

You'll see more video in the near future also. Planning on tamming mt. tamalpais as it is now. Or at least doing as much as the battery will allow me to do, lol. Want to give these motors a full range of tests. I chose a lower than desirable kv this time to get that extra bit of torque and efficiency.
```

---
## \#36 Posted by: chaka Posted at: 2017-10-08T15:24:55.417Z Reads: 205

```
Reduction will always produce more torque than a direct drive. Anyone with a slight understanding of mechanics can see this. If someone came on these forums with a 1:1 pulley drive everyone would be pointing out their error but none seem to care when a person comes to the plate with a hub drive. I'm guessing there is too much smoke in the air. 

One thing I know is nothing will beat out a rear mounted reduction drive. The size of the motors you can fit behind the trucks will dwarf anything you can fit inside a tube of polyurethane.

Those little cans we have been running on the FreeRide are nice little motors in a dual configuration but they are the absolute smallest I would ever go. We have since switched to a larger motor on the FreeRide choosing more power over weight savings.
```

---
## \#37 Posted by: evoheyax Posted at: 2017-10-08T15:52:27.964Z Reads: 198

```
Thanks for chiming in!

I honestly hope you get a chance to try the raptor 2 motors the carvon 3 motors and hummies new motors. You will notice a world of difference over the small hubs that everyone else sells today and that you've probably tried in the past. Lower heat, lower waste, and more thane, to the point that I think it's worth the tradeoffs for simplicity.
```

---
## \#38 Posted by: psychotiller Posted at: 2017-10-08T16:03:03.119Z Reads: 200

```
I'm glad to see the progression with hubs in regards to cored urethane and bigger motors. It was inevitable. My silence on the subject doesn't mean that I'm not watching, reading and taking note of everything that surfaces. But as archaic as y'all seem to think reduction systems are, they are superior. Yes they look like garden equipment, but they enable adjustable torque, acceleration and top speed without compromising consumption and heat production. Proof lies in the fact that we can run any size urethane and then swap out to pneumatics and run trails, grass and gravel without overheating our motors. (uphill)
```

---
## \#39 Posted by: chaka Posted at: 2017-10-08T16:53:41.875Z Reads: 195

```
> I think it's worth the tradeoffs for simplicity.

I think novelty is the word you are looking for. Novelty is good for business but not performance. If I seem abtuse it is only because there is a lot of misinformation going around regarding hub motors in reference to reduction drives. 

For me hubs do not solve any problems. The problems we faced early on in Eskate with belt slipping and poor fitting motor mounts has been solved with precision matched mounts and trucks... idlers. I don't want to derail this thread so this all I will say on the matter.

I will say, you have pretty much answered your own question through observation. You need to double the power potential of your hubs if you want to match a 2:1 reduction drive. Eventually you will run out of space and have to accept the compromise that hub motors cannot escape unless you engineer some gear reduction into your hub. Lowering KV is fine if you have a motor large enough to take the extra turns on the stator. lowering the kv too far on a small diameter motor creates inefficiency. This is the main problem hub motors face. You don't have the space to fit a motor large enough to be wound to a low enough KV to produce good torque without generating a lot of heat.
```

---
## \#40 Posted by: evoheyax Posted at: 2017-10-08T21:01:05.282Z Reads: 193

```
[quote="chaka, post:39, topic:35056"]
I think novelty is the word you are looking for.
[/quote]

Wow. I'm surprised to hear such harsh words from such an intelligent person, when you haven't even tried the best of hubs on the market today. These hubs have changed the game. Things are not the same anymore.

It hurts to have the person you respect and admire so much rip apart the research and development that I and many have done for the past two years. These small hub motors are novelty. But even pushing these new larger hubs hard now, I can not make then overheat the same way. There's always more to learn and more innovation to be done. If your try a pair of any of these three motors, you'll see that we have the space to fit a stable motor into the wheel, that won't overheat, even when pushed a bit.

I'm willing to concede and say things that aren't in best financial interest, such as conceding that belt drives have an advantage that hubs never will be able to fully utilize. But to go as far as to say they are "novelty" is insulting and it's clear your trying to protect your business. It's sad, because if you tried my board, as is now, with 4wd hubs, you'd be pretty happy with the torque and the max temps the motors get to.
```

---
## \#41 Posted by: chaka Posted at: 2017-10-08T22:02:17.209Z Reads: 179

```
I wouldn't get too butt hurt about it, I have been pretty open about my assessment of hub motors.  They are just too big a compromise for me on several levels.

Novelty is key to having a successful product so take it as an insult if you like but it does not change anything. If it were not for novelty none of the Chinese manufactures would be producing them.
```

---
## \#42 Posted by: psychotiller Posted at: 2017-10-08T22:17:30.853Z Reads: 185

```
[quote="chaka, post:41, topic:35056"]
compromise
[/quote]

@evoheyax  Until hubs are available, that ride plush, like abec 97s or 107s or can perform exactly the same as satellite set ups (trails/steeps or with pneumatics) they pretty much are a novelty. Popular yes! And if you poll it, or ask publicly the concensus for popularity is going favor hubs because of aesthetics. I suppose somebody needs to make a 70mph belted set-up to sway the masses?  

Care to trade a dual set of your best hubs for one of my Dual Drive systems with 97's? We could do a "Same Thread Forum Comparison"
```

---
## \#43 Posted by: GrecoMan Posted at: 2017-10-08T22:21:24.872Z Reads: 180

```
[quote="psychotiller, post:42, topic:35056"]
70mph belted set-up
[/quote]

15 to 20 gearing with 107mm wheels + 10s + 245kv = 75mph :wink:
```

---
## \#44 Posted by: psychotiller Posted at: 2017-10-08T22:24:46.862Z Reads: 183

```
It'll take more than that, but it is doable.
```

---
## \#45 Posted by: BigBoyToys Posted at: 2017-10-08T23:19:57.644Z Reads: 191

```
[quote="evoheyax, post:34, topic:35056"]
Maybe @chaka could chime in on the details of why belt drives are more efficient than hubs at higher speeds (40-50 mph).
[/quote]
I dont think this question was answered by Chaka, maybe because there is no good reason. How would a belt drive using 4.12 VESC even hit 40-50mph? With 12S voltage, a 190kv 14P motor, a 2:1 gear ratio at 85% efficiency and 90mm wheels it isnt even breaking 40mph and is already at the max recommended erpm limit of 60k. 

I made the following statement.
[quote="BigBoyToys, post:32, topic:35056"]
under low-med load cruising situations( at motor rpms within the efficincy range for its KV), where heat isnt much of a concern, the hubs should be more efficient
[/quote]

Here's a model that would test this idea.

Two eboards, both with 10S batteries, same vescs settings with 90mm flywheels maintaining a constant speed of 30mph. 
Board 1:  2:1 belt drive and a 220KV motor
Board 2: 110kv Carvon V3 direct drives(not quite hubs but close enough).

@chaka Can u argue that a belt drive is more efficient under the above circumstances?  Both motors are spinning at 80% of their max rpm, but belt drive has additiinal frictional losses from the belt and higher energy loss within the motor due to double the motor speed. Where is the hub motors disadvantage at cruising speed?

[quote="chaka, post:36, topic:35056"]
One thing I know is nothing will beat out a rear mounted reduction drive
[/quote]

This reminds me of when my grandfather told me automatic transmissions would never compare to the efficiency or reliability of a manual gearbox. Now 20 years later, less than 3% of cars in the US are stick shifts.

[quote="chaka, post:39, topic:35056"]
You need to double the power potential of your hubs if you want to match a 2:1 reduction drive.
[/quote]

As a general statement what you said is just plain false. U cant build build a 2000w belt drive that will match the performance of my 4000w hub board. Please do show up to performance day next month and try your luck if its worth it to you. If your 2000W board can beat my hub board in both a 50m and 100m sprint Ill pay your airfare home. Im guessing your board wont be sensored either since you said earlier this week that nobody needs them and their just another potential problem. 

 The only way I can see your statement above as even being close to true would be for a hub board and belt drive board with the same KV motors, but for two boards with the same topspeed your belt drive needs double the KV which cuts your torque advantage in half and increases your motors heat production as well.
```

---
## \#46 Posted by: psychotiller Posted at: 2017-10-08T23:47:12.184Z Reads: 168

```
Thing is, There is nothing that states we can't run less reduction. We can run it all the way down to 1:1 with belts. And we can change kv's. We can make a 1.5:1 4wd build @200kv @10s on 107's -64mph weighted/fully charged
```

---
## \#47 Posted by: NickTheDude Posted at: 2017-10-08T23:57:57.572Z Reads: 168

```
This is why I started this thread http://www.electric-skateboard.builders/t/are-hub-motors-worse/13330

I've always been curious where the inefficiencies in hub motors were coming from and at the time it seemed to be kV. Now all the hubs being produced are lower kV and many are still inefficient which lead me to believe heat was the culprit. I think Jason proved that they could be just as efficient with the Raptor 2 if they can dissipate all that heat.
```

---
## \#48 Posted by: chaka Posted at: 2017-10-09T00:17:26.750Z Reads: 170

```
Easy there big guy, no need to pound your chest. I was talking about apples to apples, identical motors on different drives. To argue that you get better low end torque using taller gearing doesn't make any sense. 

@NickTheDude From my understanding, the trouble starts by adding more turns to the stator windings to decrease the KV. Alternatively you can increase the number of stator teeth to lower the KV. By increasing the number of stator teeth you can effectively lower the kv without adding more turns. I assume this is why we see a higher number of stator teeth in hubmotors today. I could be wrong here, I still fall back on the engineers at the factory for these things.
```

---
## \#49 Posted by: evoheyax Posted at: 2017-10-09T00:42:57.550Z Reads: 169

```
[quote="psychotiller, post:42, topic:35056"]
Until hubs are available, that ride plush, like abec 97s or 107s or can perform exactly the same as satellite set ups (trails/steeps or with pneumatics) they pretty much are a novelty.
[/quote]

The word novelty implies that something has little to no practical value. The fact that these new round of hubs aren't having the overheating issues of the past, and are riding decently smooth (have you ridden a raptor 2?) shows practical use. Belts have their own uses, and unlike everyone else here, I'm not trying to say hubs are better or belt drives are better. They both have their uses.

I could argue the same about belt drive systems. To me, belt drives are a novelty and a nuisance. Aligning, tensioning (except for idler systems like chakas), and the space that could be used for more electronics if your bottom mounting (which most of the diyers are doing). They were so impractical compared to hubs for me, that belt drives are a novelty. Not practical for the masses or for most diyers. Too much of a pain and complication. Hubs are simple, but unless your invested in hubs, theirs no reason to admit this. And since theres no good hubs on places like alibaba, you don't have much of an entry into hubs, unless you start from the beginning and build your own. So the easiest thing to do is call them a novelty. Until these recent round, they were, but the game has changed.

[quote="BigBoyToys, post:45, topic:35056"]
This reminds me of when my grandfather told me automatic transmissions would never compare to the efficiency or reliability of a manual gearbox.
[/quote]

Totally agree here. They aren't perfect yet. But they are progressing so fast. As it is now, between enertions raptor 2 motors, hummies motors, and the carvon 3 and 4, you can get mostly everything you could every want. High top speed, low top speed, full abec wheels, off road wheels, you name, it can be done with one or multiple of these motors.

[quote="chaka, post:48, topic:35056"]
From my understanding, the trouble starts by adding more turns to the stator windings to decrease the KV.
[/quote]

To some degree, yes. More turns means more copper length, which means higher resistance. Higher resistance = higher heat. This can be solved though, by making the motor larger. We have cut resistance from 0.138 ohms down to 0.068 ohms by doubling the stator length, allowing for a thicker gauge wire and less turns (15 now instead of 30 for the same kv). So yes, we can engineer our way out of the problems hubs have faced. They can be sustainable. And this is still, far from a full copper filling on the motor too. Can do a 19 awg I believe, and reduce the resistance even further.
```

---
## \#50 Posted by: BigBoyToys Posted at: 2017-10-09T01:21:30.283Z Reads: 161

```
I agree that belts are more versatile in that wheels and gear ratios can be quickly changed. Theoretically you could even overdrive your  belt set up, but as u approach the 1:1 ratio you lose all the torque and efficiency belt drives claim to have over hubs. I dont think a 2:1 belt drive board with double the KV has any real torque advantage over a hub board with half the KV. I think both boards would accelerate similarly and have the same topspeed.

@chaka
I might have pulled your statements slightly out of context, I might also have been trying to incite some friendly rivalry to inspire you to join us next month 😉.

[quote="chaka, post:48, topic:35056"]
To argue that you get better low end torque using taller gearing doesn't make any sense.
[/quote]

When did I say taller gearing means more torque? 

[quote="chaka, post:48, topic:35056"]
I was talking about apples to apples, identical motors on different drives.
[/quote]

Well apples to apples the hub board is capable of twice the top speed of a 2:1 belt drive. So what u gained in torque you lost in top end.

Cheers,
From the 300lb guy  with the fastest Vesc powered board on the forum 😉.
```

---
## \#51 Posted by: psychotiller Posted at: 2017-10-09T01:26:26.714Z Reads: 146

```
Could we not double our motors from 2 to 4 just like you did to get the torque you wanted with your hubs? Doing that, we can raise our kv to get the desired top speed while maintaining our torque. That was what I was trying to convey.
```

---
## \#52 Posted by: BigBoyToys Posted at: 2017-10-09T01:31:29.315Z Reads: 144

```
Totally, but the erpm limit is a bit of an obstacle for gear reduction boards trying to break 40mph. Youd have to run very low gear ratios or switch to a different esc( rc or vesc 6).
```

---
## \#53 Posted by: psychotiller Posted at: 2017-10-09T01:36:07.990Z Reads: 141

```
A 3:1 ratio on my race day board netted 33mph with 2 motors @40a. So I'm pretty sure I could drop my ratio to well under 2, double my motors to account for the loss of low end torque, up my amps and allow you to go 60mph on my board.
```

---
## \#54 Posted by: BigBoyToys Posted at: 2017-10-09T01:49:43.623Z Reads: 151

```
Sounds feasible, but youd lose almost all your torque advantage and your motors would get much hotter too. So what real performance advantage does a high speed belt drive have over a high speed hub drive? Seems pretty comparable for boards that go faster than 35mph with the current erpm limit. If youre running the VESC 6  then I think gear/belt drives get the advantage back since 300+ kv motors are possible and you can keep you 3:1 and still hit high speeds.

What Id really like to see is how torque compares on belt drive and direct drive compare that are set up for the same mph. Im not saying saying that the hubs would have more torque or vise versa, Im sayng that I dont think there would be much difference.
```

---
## \#55 Posted by: onloop Posted at: 2017-10-09T01:49:56.856Z Reads: 158

```
@evoheyax these belt drive dudes are never going to concede, even if video evidence & engineering literature is furnished proving many of their arguments to be invalid. 

> FACT: When applied to esk8 use case, belt drives also have engineering/[erformance constraints that cannot be overcome easily.

The only option left for anyone looking to push the envelope is an improvement in motor design! Understanding how to improve the efficiencies & performance from inside the motor itself is the holy grail. _@evoheyax this puts you ahead of the rest, anyone who doesn't talk about motor design from now on is not a real threat._

> REMINDER: Torque transfer of common 5mm pitch belts are a bottleneck that cannot be removed easily. You need wider belts. More teeth in mesh, Or no belts. 


----------

> ANOTHER INTERESTING FACT: If I put an R2 motor on a >=15mm wide belt, with appropriate teeth in mesh, maybe an idler (which reduces belt duty cycles) you could theoretically (assuming the transmission can handle the torque) have more torque at the wheels than the standard R2 HUB at 1:1, but it would be just ridiculous.... nobody actually needs that!! 


## More torque is no longer the objective here!

More efficiency is the new kid on the block in esk8 innovation. If you regard yourself as a legit esk8 builder & you aren't spending money doing R&D to improve efficiency (whilst preserving/improving torque) you have already lost the game.




## SUMMARY: LEARN HOW TO DESIGN BETTER MOTORS
```

---
## \#56 Posted by: psychotiller Posted at: 2017-10-09T01:53:51.803Z Reads: 154

```
[quote="onloop, post:55, topic:35056"]
More torque is no longer the objective here!
[/quote]

Right, really the objective now is just keeping the urethane on our wheels...Oh wait! Not us belt guys.

<img src="/uploads/db1493/original/3X/5/8/58bc67ef89a85ae7eee13f3c88e357777d35005f.jpg" width="300" height="168">
```

---
## \#57 Posted by: psychotiller Posted at: 2017-10-09T01:57:02.385Z Reads: 151

```
Derek! You can pilot my 4wd.
```

---
## \#58 Posted by: BigBoyToys Posted at: 2017-10-09T01:59:42.708Z Reads: 152

```
True story! Not a single full hub motor yet with good power has solved this completely. Its comimg though.  @evoheyax 🤞your urathane cores are up to the task but Im still skeptical.

@psychotiller  I'd love to 👌
```

---
## \#59 Posted by: evoheyax Posted at: 2017-10-09T02:01:28.120Z Reads: 156

```
[quote="psychotiller, post:56, topic:35056"]
Right, really the objective now is just keeping the urethane on our wheels...Oh wait! Not us belt guys.
[/quote]

hahaha, good one.

[quote="onloop, post:55, topic:35056"]
More efficiency is the new kid on the block in esk8 innovation. If you regard yourself as a legit esk8 builder & you aren't spending money doing R&D to improve efficiency (whilst preserving/improving torque) you have already lost the game.
[/quote]

Describes what we have been doing the past 2 years exactly. The new double wide hub motors increased torque significantly, while decreasing heat significantly. Just tested it on some 20% grade hills, did laps for 15 minutes up and down. Max temp was 151 F on one motor, and 130ish F on the other 3 (maybe a short, idk why one was so much higher, since they are all the same kv. We'll find out in time I guess). Pretty good, when the old motors would have hit 160 F in the first hill climb. I think I climbed it about 20 times, back to back. And it's a long block.

And we understand pretty much everything (except for the real cost benefit of 24 teeth instead of 12. Might have to get the 24 tooth stator of our current stator and see what happens) about how to increase efficiency, and in tern, lower heat :stuck_out_tongue:
```

---
## \#60 Posted by: evoheyax Posted at: 2017-10-09T02:05:34.747Z Reads: 149

```
[quote="BigBoyToys, post:58, topic:35056"]
your urathane cores are up to the task but Im still skeptical.
[/quote]

I know, its hard to believe, but its real. I've been pushing them hard the past few days, and they are holding up fantastic. These cores are a heat high material that won't deform and turn to dust like regular polyurethane will. This special polyurethane we're using right now bonds to the core so well, that we can't separate it, even with an exacto knife. Of the wheel fuck ups so far, we tried with everything to separate them, and we can't even get it to start separating. Wheels are not going anywheres anymore in my mind. And the rebound is nice. We'll get better at the right blend to get the right road feel. But even rough roads are light years better than before. Way smoother than many abec knockoffs in my mind. (but maybe not quite a real abec quality yet).

I was skeptical when hummie told me about this idea too, but it needed to be done. And I'm sold now. It's working great so far, were as before, I would of already started to see deformations in the ribbed structure, the wheels show no signs of wear, on the outside or in the core.
```

---
## \#61 Posted by: racidon Posted at: 2017-10-09T02:09:45.725Z Reads: 142

```
The borderline racist comments I see on this forum really disgusts me.
Heads up @evoheyax as far as I know majority of enertion products are made in china... China as a country has low income workforce and the infractstructure to support low cost manufacturing. Just because it says "Made in China" does not make it shit. Quite often the "chinese crap" you've spoken about is "crap" made by some westerner looking to make a quick buck. 

As for efficiency, no watter what you do using a gearing system will **_always_** make a motor more efficient. That's just how mechanics work. Perhaps if you find some magical law that changes how physics work you can let Car manufacturers know so that our vehicles can become cheaper, removing Diffs and Gear boxes for us!
```

---
## \#62 Posted by: psychotiller Posted at: 2017-10-09T02:16:05.676Z Reads: 144

```
[quote="racidon, post:61, topic:35056"]
As for efficiency, no watter what you do using a gearing system will always make a motor more efficient. That's just how mechanics work. Perhaps if you find some magical law that changes how physics work you can let Car manufacturers know so that our vehicles can become cheaper, removing Diffs and Gear boxes for us!
[/quote]

^This ^this ^this
```

---
## \#63 Posted by: evoheyax Posted at: 2017-10-09T02:22:07.436Z Reads: 156

```
[quote="racidon, post:61, topic:35056"]
Heads up @evoheyax as far as I know majority of enertion products are made in china... China as a country has low income workforce and the infractstructure to support low cost manufacturing. Just because it says "Made in China" does not make it shit. Quite often the "chinese crap" you've spoken about is "crap" made by some westerner looking to make a quick buck.
[/quote]

I'm not saying china can't produce good products. A lot of great products come from china. If you read any of my past comments about china producing stuff, you would know this.

My generalization here was about how these hubs are entering the market and being sold and tested as they stand today. The standards of every hub besides the 3 I have mentioned disgust me. If it's a western behind some of these, maybe. But it's not a racial thing. It's a situational thing, an opportunity that the people who make the decisions about what products they should produce and sell see, and jump on, with little regard about making something feasible. They lie to your face, and say theres no heat issues, they will work great, and the first ride, they over heat and burn up. Seriously, tired of trying hubs from straight from manufactures in china and having this happen. It has nothing to do with race though. My point was that I can explain to why all of these motors are too small to be practical. They are not unpractical because they came from china, or because Chinese people made them, that's just stupid. I live in liberal San Francisco for a reason man...

[quote="racidon, post:61, topic:35056"]
Perhaps if you find some magical law that changes how physics work you can let Car manufacturers know so that our vehicles can become cheaper, removing Diffs and Gear boxes for us!
[/quote]

Look back to before in this thread, and you'll see, cars and electric skateboards, while they have somethings in common, are nota good comparison.

Yes, gears are more efficient when you have many gears. But electric skateboards have **one** gear, not many. So they aren't utilizing their full potential. Do you see cars with 1 gear? no. 

Also, cars need a wider range of speed. The masses don't need faster than 25 mph, and even a lot of speed freaks like me are content with 40 mph.

So not a good comparison...
```

---
## \#64 Posted by: racidon Posted at: 2017-10-09T02:38:29.991Z Reads: 151

```
[quote="evoheyax, post:63, topic:35056, full:true"]
[quote="racidon, post:61, topic:35056"]
...(trimmed)...
[/quote]

I'm not saying china can't produce good products. A lot of great products come from china. If you read any of my past comments about china producing stuff, you would know this.

My generalization here was about how these hubs are entering the market and being sold and tested as they stand today. The standards of every hub besides the 3 I have mentioned disgust me. If it's a western behind some of these, maybe. But it's not a racial thing. It's a situational thing, an opportunity that the people who make the decisions about what products they should produce and sell see, and jump on, with little regard about making something feasible. They lie to your face, and say theres no heat issues, they will work great, and the first ride, they over heat and burn up. Seriously, tired of trying hubs from straight from manufactures in china and having this happen. It has nothing to do with race though. My point was that I can explain to why all of these motors are too small to be practical. They are not unpractical because they came from china, or because Chinese people made them, that's just stupid. I live in liberal San Francisco for a reason man...
[/quote]

I read the whole thread, no point replying otherwise. Whether it was a dig at china or not mate, you referenced "china" as the source of crap multiple times in just your first post alone. Could have left it at "small hub motors".
[quote="evoheyax, post:63, topic:35056, full:true"]
[quote="racidon, post:61, topic:35056"]
Perhaps if you find some magical law that changes how physics work you can let Car manufacturers know so that our vehicles can become cheaper, removing Diffs and Gear boxes for us!
[/quote]


Look back to before in this thread, and you'll see, cars and electric skateboards, while they have somethings in common, are nota good comparison.

Yes, gears are more efficient when you have many gears. But electric skateboards have **one** gear, not many. So they aren't utilizing their full potential. Do you see cars with 1 gear? no. So not a good comparison...
[/quote]

As above. I read the whole thing. Perhaps you could do some learning about cars. Cars although moving much larger amounts with much larger engines are essentially doing the exact same thing as an eboard is mate. Just so you know if you were to remove a differential from a car and place a 1:1 gear in that you'd completely screw the efficiency of the motor and the vehicle itself, regardless of the fact it still has a 6 speed gearbox in it.



What's efficiency to you?
How much power is wasted vs how much output you get?
Hub motors will ALWAYS have less either top speed or torque depending how you GEAR your belt/chain/sprocket driven motor. This is because you can either gear for top speed or torque. The only way around this is to gear within the hub itself, but then I guess it wouldn't be a hub motor anymore.

I think you need to realise noone here arguing your facts has any problem with hubs, just your misinformation. Hubs have a place as done chain/belt etc. All with benefits all with disadvantages.
```

---
## \#65 Posted by: Cobber Posted at: 2017-10-09T02:45:26.755Z Reads: 139

```
[quote="psychotiller, post:42, topic:35056"]
I suppose somebody needs to make a 70mph belted set-up to sway the masses?
[/quote]

We will see how fast they go at the 2nd SPD... I'm guessing we will see 50+ Mph

[quote="evoheyax, post:49, topic:35056"]
The word novelty implies that something has little to no practical value.
[/quote]

not true, the primary objective in a patent is to prove you have some thing _novel_. 
Novel = New
and a patent can have great value...
```

---
## \#66 Posted by: Titoxd10001 Posted at: 2017-10-09T02:50:33.219Z Reads: 137

```
[quote="evoheyax, post:63, topic:35056"]
Do you see cars with 1 gear? no
[/quote]

Tesla electric cars have single speed gearboxes
```

---
## \#67 Posted by: evoheyax Posted at: 2017-10-09T02:51:23.476Z Reads: 150

```
[quote="racidon, post:64, topic:35056"]
I read the whole thread, no point replying otherwise
[/quote]

Talking about the thread either earlier this year or last year about china and correlation of china = crap in most peoples minds. What I was trying to do is give people perspective into why these manufactures do what they do. Cause the first thing people are going to say, is why do they make and sell something as a good product when it's not?

[quote="racidon, post:64, topic:35056"]
I think you need to realise noone here arguing your facts has any problem with hubs, just your misinformation.
[/quote]

Can you point me to my mis information? I'll correct it right away

Again, cars aren't a good comparison. Gearing does help in some ways, especially below 10 mph, but as @onloop said, it also has it's bottle necks and weaknesses too. I also never said belts are bad. I agree they both have their place. But I think in time, hubs will win out, unless people start developing gear boxes for electric skateboards. Then, you can compare cars and electric skateboards. And then, hubs won't be able to compete without a built in gear box also.

I don't see this happening though, as now you need 2 gear boxes for a dual drive, synced together in such a way that they mechanical switch gears at exactly the same time. Also, how would you control this from your standard rc remote?

So until then, hubs are the future. Customers need to know though what they are getting, and most do not. You can blame the customer, but then, the customer assumes hubs are inherently bad, cause that's what so many people say and will tell them. The reality, is they cheaped out and didn't spend the money on a hub that actually works...
```

---
## \#68 Posted by: evoheyax Posted at: 2017-10-09T02:57:00.687Z Reads: 142

```
[quote="Titoxd10001, post:66, topic:35056"]
Tesla electric cars have single speed gearboxes
[/quote]

At the cost of some top speed and torque above 40 mph, yes. But not a single gas powered car has 1 gear only. And they are sacrificing efficiency by not having more gears. I think in the future, you'll see them develop more gears into electric cars to get better range and torqure through out the range. Remember, like electric skateboards, these cars are all very new. So it's easiest to start with 1 gear. In fact, tesla had 2 gears at first, but dropped one for simplicity, cause they couldn't get the 2 working fast enough.

This is why tesla's are beasts until about 40 mph, then all the super cars destroy it because they have gearing... Go watch the tesla racing channel on youtube and you'll see what Im saying happen over and over again.
```

---
## \#69 Posted by: psychotiller Posted at: 2017-10-09T03:13:48.364Z Reads: 142

```
[quote="evoheyax, post:67, topic:35056"]
Customers need to know though what they are getting, and most do not. You can blame the customer, but then, the customer assumes hubs are inherently bad, cause that's what so many people say and will tell them. The reality, is they cheaped out and didn't spend the money on a hub that actually works...
[/quote]

Actually I think it's the opposite. Generally, everyone on the forums and internet have been led to believe that belt drives are inefficient and melt when they get wet. Also, if that were true, "China" wouldn't have 200 different/same options available.

Reality -The boom in interest happened faster than good belt drives did. Most complaints about belt driven systems are true, but pertain to older versions that didn't adjust well and rattled loose. Furthermore people couldn't adjust anything properly on their own. So they gave up before they got it figured out.

Add in more misconceptions (problems that don't exist) such as Belts stretch, Belts break when they get wet, Belts create drag...Only the last one is true IF it's not set up correctly.

I'm not here bagging on Hubs. If you've fixed ride quality and ejection wheels you're at the top of your game right next to Carvon.

My offer still stands if you want to see why I get so worked up when people bag on belt drives.
```

---
## \#70 Posted by: evoheyax Posted at: 2017-10-09T03:23:35.784Z Reads: 144

```
[quote="psychotiller, post:69, topic:35056"]
My offer still stands if you want to see why I get so worked up when people bag on belt drives.
[/quote]

I might very well take you up on this offer. I wish as a community, we did more testing and less arguing.

This topic has turned in to a hubs vs belt drives again, when the topic was very clear. Why small hub motors have issues, and how they can be address to make better hub motors.

Did I add some flavor to it, yea, cause If I gave you a spread sheet with data, many would get lost or not fully see the picture I'm trying to paint in peoples heads. But I challange, anyone in this community, who thinks they have a small hub motor that won't overheat, come to SF, try it on my route with my weight and riding style, and I'll give you a pair new large hubs for free if they stay under 160 F the entire way. The real overall goal was to inform and share research and development with the community, so they can better understand why hubs up until now, couldn't do what the belt drive counter part could, and make better purchasing decision. $250-$800 for small hubs that are too small, or $400-$600 for larger hubs that don't have the same issues.
```

---
## \#71 Posted by: onloop Posted at: 2017-10-09T03:24:26.938Z Reads: 142

```
[quote="racidon, post:61, topic:35056"]
no watter what you do using a gearing system will always make a motor more efficient.
[/quote]

you need to clarify your claims in more detail..... are you talking about using identical motors? or just in general?

We compared R1 vs R2 and documented the results, surprisingly the R2 is more efficient.

https://www.youtube.com/watch?v=Pfu2BoXPB7Q
```

---
## \#72 Posted by: boramiNYC Posted at: 2017-10-09T03:24:28.905Z Reads: 139

```
OP, you seem to be very knowledgeable about hub motors and only recommends those three examples above. Another poster mentioned Meepo's 90mm hub motor and his good experience with it, which I happen to share. Any specific reason other than it's from China and inexpensive why you don't think it's worth mentioning about it? It doesn't seem to suffer from over-heating, it runs great at 22mph, climbs a 20% hill. It's been selling like hotcakes last couple months with many good experiences. If you are curious and want to take a look at it I have an extra slightly defective motor you are welcomed to take a look at. Where are you located? I'm near LA.
```

---
## \#73 Posted by: Titoxd10001 Posted at: 2017-10-09T03:33:25.362Z Reads: 134

```
The torque curve of a combustion engine and a electric motor are very different. Electric don't really need multiple gears. Think formula e does use transmissions though and some still choose single speed gearboxes. But my point is they are not using direct 1:1 drive.
```

---
## \#74 Posted by: racidon Posted at: 2017-10-09T03:39:44.037Z Reads: 137

```
[quote="onloop, post:71, topic:35056, full:true"]
[quote="racidon, post:61, topic:35056"]
no watter what you do using a gearing system will always make a motor more efficient.
[/quote]

you need to clarify your claims in more detail..... are you talking about using identical motors? or just in general?

We compared R1 vs R2 and documented the results, surprisingly the R2 is more efficient.

https://www.youtube.com/watch?v=Pfu2BoXPB7Q
[/quote]

Yes @onloop because otherwise there's no point comparing different implementations?
If you took you hub motor you had made and slapped a bit of gearing on it, it would become more efficient, obviously at the cost of theoretical top speed though are you likely to ever hit that?
```

---
## \#75 Posted by: onloop Posted at: 2017-10-09T03:46:42.838Z Reads: 131

```
[quote="racidon, post:74, topic:35056"]
it would become more efficient
[/quote]

just not in terms of distance traveled over time..... then it would be less efficient.... 

it would have fucking shite loads of torque potential though!..... however you might skip teeth on the belt, which is a loss of torque, which is also an inefficient use of torque.... so less efficient...



_Maybe edit your post & remove the word "ALWAYS" as its a bit misleading._
```

---
## \#76 Posted by: evoheyax Posted at: 2017-10-09T03:51:00.380Z Reads: 139

```
[quote="boramiNYC, post:72, topic:35056"]
Any specific reason other than it's from China and inexpensive why you don't think it's worth mentioning about it?
[/quote]

I haven't tried these in particular. The reason is simply down to stator size. I'm not entirely sure what the size of the stator is, but the stator size will tell you how much iron you have in the core and the amount of copper you can fit in the motor. There is a certain size of stator, that becomes large enough, to were the motors don't become saturated under any case. These small motors, simply can't fit the amount of copper or iron (stator size) to run efficiently. Once you hit 160 F, motor efficiency goes down the tube. And these small motors will always struggle to stay cool under harsh riding.

Everything comes down to how long you ride for, how many hills you hit, your weight as a rider, and how you ride.

I never said you can't have good results with these small hub motors, but that they have a lot of weakness, that will result in a shorter life of the motor specifically (possibly, very short, but best case, a fraction of what you should get from a motor). Unless you limit amp output to these little motors to control heat, but then, you won't get performance anywheres close to a belt drive system. The goal is be able to compete with belt drive systems, and it's physically impossible, in that little space, to fit enough stator (iron) and copper to make the motor be able to run the way we need it to compete with belt drives. Maybe meepo hub motors work, but they are very limited in the amps you can put into them, which limits torque. In addition, with the limited amount of copper and stator, they need even more amps to get the same torque as a larger motor. 

For example:
Before, I needed 4 amps to cruise at full speed on flat.
Now, I need less than 2 amps to cruise at full speed on flat. Which is going to result in better range?

Now, you can say the meepo gets great range, so don't they have great efficiency? That's due to is lower top speed. 15 mph is the best speed for efficiency of most of these motors. 10 mph or less, and your not running efficiently with a hub motor. I like to ride at least 25 mph at all times. Over 20 mph, the wind resistance is exponential, and kills range. So this is why it takes 4 amps for me to cruise at top speed. At 15 mph, it goes back down to around 2 amps again on the old motors. On the new motors, Its about 1 amp to cruise at 15 mph. But I never ride like that. So I get shitty range. It's not that my small motors are less efficient than meepos, just that I like to ride faster at all times than the meepo motors can even do, so my range takes a punch to the gut.

BTW: All of these numbers are per motor. System includes 4 motors.

At the end of the day, they can work, for certain people, but if your looking for reliability, durability, power, and better top speed, you simply can't get that from a small motor due to the limitations I've outlined in this thread.

Maybe for you and some others, they will work, but it's better to not be working your motors near their absolute potential. That will lead to issues.
```

---
## \#77 Posted by: chuttney1 Posted at: 2017-10-09T03:56:02.843Z Reads: 139

```
[quote="evoheyax, post:68, topic:35056"]
not a single gas powered car has 1 gear only.
[/quote]

How do you explain Koenigsegg decision to ditch the transmission in their Regera with the differential having a 2.73 final drive with a ratio?

http://1hosj01irnixn8onr1zmv5s1.wpengine.netdna-cdn.com/wp-content/uploads/2015/03/Illustration_Direct_Drive_20170525_07_lj-930x529.jpg

I understood how this propulsion system is possible.
```

---
## \#78 Posted by: racidon Posted at: 2017-10-09T03:59:52.884Z Reads: 139

```
[quote="onloop, post:75, topic:35056, full:true"]
[quote="racidon, post:74, topic:35056"]
it would become more efficient
[/quote]

just not in terms of distance traveled over time..... then it would be less efficient.... 

it would have fucking shite loads of torque potential though!..... however you might skip teeth on the belt, which is a loss of torque, which is also an inefficient use of torque.... so less efficient...



_Maybe edit your post & remove the word "ALWAYS" as its a bit misleading._
[/quote]

well unless you're trying to skew results it will always be more efficient, obviously with something as powerful as those on the R2 you'd barely be gearing, something like a 2:3 would still be insane. if you were to use the same gearing you used on the R1 that would obviously be insanely stupid
Distance traveled over time would be hard for anyone to prove without an apples to apples of **_actual_** riding
```

---
## \#79 Posted by: evoheyax Posted at: 2017-10-09T04:01:19.532Z Reads: 139

```
lol, you'll always find a fringe case. I guess I should be more specific and say none of the big dogs in the car industry are doing it. Ford, Crysler, Dogde, Audi, Subaru, BMW, Toyota, Honda, Acura, None of them use a single gear in their combustion cars.

Now, thats a bit unfair also, since its a hybrid, not a solo combustion car.

But as @Titoxd10001 said, it is a bit unfair to compared combustion cars to electric cars in their torque curves, so I'll leave it at that.
```

---
## \#80 Posted by: Titoxd10001 Posted at: 2017-10-09T04:17:51.175Z Reads: 139

```
Well the regera has a torque converter which is kind of like a transmission and and it has multiple electric motors. It's geared for like 250mph though lol
```

---
## \#81 Posted by: boramiNYC Posted at: 2017-10-09T04:24:03.716Z Reads: 136

```
Wow, thanks for the detailed reply. I agree those Meepo motors are much more efficient at 15mph than 20 and up from my experience.
```

---
## \#82 Posted by: evoheyax Posted at: 2017-10-09T04:37:19.390Z Reads: 134

```
That will be the case with any hub motor that size. Just because you can go up a 20% grade hill, doesn't mean your not stressing the hell out of your motors. Those motors should be used on mostly flat, with lighter riders, at 15 mph. Then, they might work ok (hummies small motors worked great for many too, but I was another story for them, lol). But don't expect to do crazy things with them. Or them to last as long as a motor should. I'm in SF BTW.
```

---
## \#83 Posted by: NickTheDude Posted at: 2017-10-09T06:18:44.386Z Reads: 132

```
So (other than heat dissipation) why is a 100kV hub worse than a 200kV 2:1 belt drive?
```

---
## \#84 Posted by: NNGG Posted at: 2017-10-09T06:30:31.280Z Reads: 134

```
There is less urethane and so more vibrations and shock is transferred to the motor. In addition to that, the motor needs to work harder to do the same amount of work. It is direct drive and so a 100kv motor will have more heat and more amps going through it.
```

---
## \#85 Posted by: NNGG Posted at: 2017-10-09T06:33:14.684Z Reads: 137

```
Hub motors are for special uses where certain trade offs are desired. I like my belt system because it is set and semi-permanent with little maintenance after you get rid of the teething problems. Hub motors will cost more due to design costs and less diy required. you basically get a pre made kit. Hub motors are almost pre built esk8 material unless you were re configuring a 149kv sk3 into a diy hub motor.
```

---
## \#86 Posted by: NickTheDude Posted at: 2017-10-09T06:46:38.250Z Reads: 139

```
[quote="NNGG, post:84, topic:35056"]
motor needs to work harder
[/quote]

Yeah that's what everyone says but no one ever explains why. Is the relation ship between kV and torque/speed not the same as gear ratio and torque/speed?

Since Carvons don't need to deal with vibration are they not subject to those inefficiencies?
```

---
## \#87 Posted by: appelton Posted at: 2017-10-09T07:44:03.145Z Reads: 146

```
[quote="psychotiller, post:56, topic:35056"]
Right, really the objective now is just keeping the urethane on our wheels...Oh wait! Not us belt guys.
[/quote]
<img src="/uploads/db1493/original/3X/d/2/d2c5519a6fb44b280ff95d4c00782e090a3fea17.jpg" width="375" height="499">
```

---
## \#88 Posted by: Agira Posted at: 2017-10-09T08:03:04.101Z Reads: 154

```
[quote="onloop, post:75, topic:35056"]
just not in terms of distance traveled over time..... then it would be less efficient....
[/quote]

Isn't distance traveled over time just speed?
Efficiency is energy put into the motor vs the mechanical energy obtain.
```

---
## \#89 Posted by: trampa Posted at: 2017-10-09T09:58:10.455Z Reads: 156

```
Hi @NickTheDude,  this is the reason:

**From** http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

_Let’s look at an example: Suppose an 8 turn motor has one ohm winding resistance. The winding resistance is proportional to the wire area times wire length. Making the same motor with 4 turns would allow twice as thick wire. Since that wire also is half as long, the resistance is four times lower: 0.25ohm. Further, since current times turns is proportional to torque, we need twice as high current with 4 turns to produce the same torque as with 8 turns. The copper losses are the voltage across the windings times the current: U*I. The voltage across them is R*I, so the losses are R*I*I. This square relation means that doubling the current will produce four times as much losses, however, since we got four times lower resistance the losses are the same for the 4t motor with double the current as for the 8t motor with half the current. Also note that the 4t motor will spin twice as fast as the 8t motor at the same voltage, so it will have double the kv. Putting this together, the 4t motor is equivalent to the 8t motor, but at half the voltage and double the current._

_So, regarding KV: different KV versions of the same motor are fully equivalent. KV only affects the battery and ESC choice. Therefore, while comparing motors, lets talk about torque instead of current because torque is proportional to current / KV and, as explained above, the KV value can be changed freely with the amount of turns and copper thickness._

_RPM/Losses/gear reduction_

_Now we know that copper losses are proportional to the square of the torque produced by the motor, and at low RPM and high load they are dominant. As RPM increases, other losses start to add up exponentially. In my experience, these losses start to get significant around 60k electrical RPM, which for a 14-pole motor is about 8570 mechanical rpm (most 50mm+ outrunners have 14 poles, some unusual ones have 18). Because of the square relation, it is desirable to run at as high speed and low torque as possible as long as we stay below 8.6k RPM. To express the square relation in some numbers, **having double the RPM and half the torque at a certain power output will cause four times less losses.** The lesson from this is that: make sure the top speed you design the skateboard for is at around 8.6k rpm on the motor if you are using an 50mm-60mm outrunner._

Conclusion: To do a fair comparison you have to do the following:

A: Take the same motor and wind it to a lower KV, higher torque output, suitable for a hub drive. Use it inside a wheel with no gearing
B: Take the same motor and wind it to a coordinated higher KV, lower torque, use it in a geared system (e.g. 1:2.5 reduction belt drive)

Now both systems result in a board/vehicle with roughly the same acceleration and top speed, but system A has high losses, while system B has low losses. The relation is non linear but a square one! 

If you want both systems to have the same efficiency, same losses, your hub motor would need to be a lot heavier than the geared one. This big and heavy motor doesn't fit inside the wheel any more. We are not talking about a slight increase in size. We are talking about roughly 3-5x the mass of the satellite motor! This motor will also be bigger in diameter and in consequence you will get wheel size gearing, working against you. The motor simply doesn't fit!

In consequence system A will end up splitting the torque in half, using two motors instead of one. So you will end up needing two motors instead of one and you will still be a lot less efficient than the 1:2.5 geared system with one motor.
And there is nothing you can do against it, since you can't cheat physics!

The only thing you can do is compare to different systems and state that A is better than B or vice versa. But that is BS and tells nothing about the matter itself.

**What you can do:**
You can optimize the motor and make it bigger **and use two of them**. 
This is what we currently see. 2.4 Kg of motor(s) vs. single 700gr satellite motor. 
But you have to be fair and apply the same optimizations and twin setup to the satellite system you compare it with. 
A race you can't win if you are aiming at making a system that compares to a geared one.
It only works if you compare two oranges to one apple. Apples to Apples doesn't work.

If you say that the belts are the weak link in a geared system, so in consequence the hub is better because it has no belt, you need to look deeper into the matter.

**Limits of Belts:**
How much a belt can transfer torquewise depends on the small pulley size, belt width and how many teeth interlock on the small pulley, + size of teeth. If a belt system is rates 3Nm and you gear down 1:2.5, that is 7.5Nm at the wheel. Usually you can transfer 1.5x as much, since there is a safety value in the calculations. _Some geared systems don't like belts to hop over (e.g. camshaft drives)._ But our systems won't die because a belt hops once a while, so you can assume a 3Nm rated system can transfer up to 1.5x more in real life without having to much of an issue.
If you improve the system a bit (longer belt, idler pulley), you can put 12-16Nm down to the tarmac without slipping the belt. The system is about 98% efficient and the 2% losses you have are nothing in comparison to the losses your 1:1 hub will have. 

The belt is not to much of a weak link and the acceleration you can achieve is massive. And if you feel like needing 20+Nm on a board, you can always go for a twin drive. But this is crazy anyway and only a very few users can handle that amount of acceleration. 95% of the users can't bring a good belt drive to the limits.
Service is minimal and also hubs will need some service and bearing change (tricky). 

**The production/build cost** 
The belt is probably the winner, since a single belt drive has the same or better performance as a twin hub. Two ESCs and two motors simply cost more than one ESC, one motor and one belt drive. So you have to compare price to performance wise.

**Top Speed**
Hub setups claim to have the best top speed performance. This is partly true. Since you gear to 1:1 reduction, you have the best efficiency at a ridiculous top speed where wind drag gets so dominant, that you can't make use of the  efficiency at that speed. The motor has a hard time to work against that drag. 
The best possible setup has gearing which provides the best efficiency at the speeds you usually ride at.
Some users face hills and in consequence they should pick a gearing suitable to climb these efficiently.
The top speed claim is a statement reading like this: usage of incorrect gearing.
Who wants to ride at 40 MPH? It's ridiculous to gear to this speed in 99% of the cases.
If you feel like this kind of gearing is appropriate, you can apply it to your geared system as well.
Try to paddle your bike in a high gear at low to medium speeds + climbing hills. This is how your hub motor feels like most of the time.  Exhausting, but the top speed is great!  You could go to the gym and train your legs to compensate for that inefficiency, buy a tandem bike - or simply use an appropriate gearing. Tour de France cyclists don't look like Arnold Schwarzenegger in his best ages, they paddle at high RPM and low torque output and use the correct gear for the situation. 

**Coasting** 
This argument is often used to state that hubs are superior. It is not true at all. If your hub board outputs the same torque as a geared one, the drag produced by the motor will be pretty much the same. Compare Apples to apples again! 
Hub often simply lack torque and the drag resistance is lower in consequence. You could achieve the same behaviour with a belt system, simply choosing a motor with an equivalent low torque, high KV or use low gearing or smaller motors. If your hub motor has high torque and in consequence good brakes, it is not the best performer when it comes down to coasting.
Apples to Apples again.

**Hubs VS. Belt:** 

If you look at the physics its obvious what you want and who is the winner. Still you could argue in both directions. Some boards want to look stealthy, some riders don't put lots of strain on the system (light, no steep hills, cool environment) etc, some boards compensate with a twin setup and heavy hub motors.
Some want the board to be light and don't want to carry 2.5Kg of motors all the time, some want to use different wheels + wheels from different vendors/manufacturers and experiment, others don't want that option or don't care for weight so much etc. Horses for courses! It comes down to personal preference and the average usage. 

But if you want to debate the matter objective: Understand the matter and Apples to Apples please!

The entire thread is full from one apple to twin/quad oranges comparison. This is not leading anywhere. 
Keep it simple: single to single drive for best comparison. 
Personal preference matters should be separated from technical objective matters. 
Then you can say: I know the disadvantages but I'm happy to accept them for other reasons - or not.
And you know why your hub is getting hot: Having double the RPM and half the torque at a certain power output will cause four times less losses. Losses = Heat. If your hub is getting hot it is simply operating with to much losses because the torque produced is to high. 

Frank
```

---
## \#90 Posted by: chaka Posted at: 2017-10-09T13:56:49.542Z Reads: 140

```
What you are not considering are physical size limitations and the role it plays in finding the best kv for a given size. Going too low effects efficiency. This why we don't see small motors with really low KV. It is better to have more poles and stator slots if you want torque at low RPM but this is hardly a good solution in motors this small.
```

---
## \#91 Posted by: trampa Posted at: 2017-10-09T13:57:56.729Z Reads: 138

```
Agreed!

Frank
```

---
## \#92 Posted by: longhairedboy Posted at: 2017-10-09T14:04:58.312Z Reads: 135

```
All of this is correct. 

All of this is why i'm still running belts on all my builds and try to get people not to jump on the hub wagon just yet. Some people just have to have them though.
```

---
## \#93 Posted by: chaka Posted at: 2017-10-09T14:06:51.707Z Reads: 135

```
This is the simplest explanation I have seen. 

> If you rise the number of turns you get a lower Kv (rpm/V)
> and a higher Kt (torque per amp)
> But you are obliged to decrease the amps .. (under a new limit)
> so you don't get more torque

> To keep the same power you are obliged to increase the voltage ..
> and returning to the same speed (and same torque but no more).
> If you keep the same voltage (lower rpm) you are limited to less power

https://www.rcgroups.com/forums/showthread.php?1741403-Winding-a-extremely-low-%28100%29-KV-motor/page2
```

---
## \#94 Posted by: trampa Posted at: 2017-10-09T14:32:29.086Z Reads: 132

```
Barney from the German forum was so kind to ad in a calculator into the VESC-Website.
We will try to ad more setups, batteries, motors etc.

http://www.vesc-project.com/calculators

Frank
```

---
## \#95 Posted by: longhairedboy Posted at: 2017-10-09T14:39:51.287Z Reads: 140

```
[quote="chaka, post:36, topic:35056"]
Reduction will always produce more torque than a direct drive. Anyone with a slight understanding of mechanics can see this. If someone came on these forums with a 1:1 pulley drive everyone would be pointing out their error but none seem to care when a person comes to the plate with a hub drive. I'm guessing there is too much smoke in the air.
[/quote]

lord .. its like you can hear me muttering under my breath all the way over there... 

hubs are almost like putting the pulleys in the wrong places. ITs not only not reduction, its almost accretion. Then they trap the heat on top of generating more of it.

Long stators, fat stators, more copper, less copper... if sinking the heat into the truck hangers isn't a priority none of it matters as much as we'd like it to. Hubs deal with a fuckton more startup load than belts and then they just cage all that heat. Until they can reliably sink it and sink it quickly they're going to keep degrading and won't be something i even consider using on a regular basis. 

Most aren't there yet and the people who are aren't sharing. I don't consider Carvons to be hubs. Those are direct drives and solve a lot of problems hubs have. So many in fact that its not the same class of drive system and shouldn't be called a hub drive. Enertion has hub drives but they've calling them direct drives and that's just confusing people. They're hubs.The stator is INSIDE the wheel.  Everything about the rspec hubs is a vast improvement over everything else i've sen but i still don't want them. Yet. 

i can get north of 35mph on 190kv at 16/32 on 80mm kegels. I can get north of forty on 97mm flywheels. I can do that regularly and my fat ass motors are still cool enough to keep your hand on. And that's on motors that we all know aren't actually 190KV because of how Jollin was holding her pencil that day and how the wire was coming off the spool. Yes I like to imagine Jollin sitting there in a rocking chair winding all of the motors herself, with the winding wire feeding off of spools nestled neatly in a knitting basket next to her chair, while catching up on Game of Thrones and smiling sweetly. 

the only thing attractive about hubs to me right now is how easy they would be to build with. Everything else about them is a non-starter for me. 

One good application for them besides niche speed boards is inexpensive and reliable beginner boards. They make the build cheap and make <$700 boards possible, which is accessible to people interested in the sport but have zero experience. That is literally the only reason i'm even looking at  koowheels right now. I gave one of my customers one at dealer pricing a couple months ago and he's already trashed it.
```

---
## \#96 Posted by: evoheyax Posted at: 2017-10-09T15:09:18.830Z Reads: 136

```
[quote="longhairedboy, post:95, topic:35056"]
That is literally the only reason i'm even looking at  koowheels right now. I gave one of my customers one at dealer pricing a couple months ago and he's already trashed it.
[/quote]

Because too small is too small. The stator we are using right now is around 4 times the size of the old r-spec 2 motors stator. So according to these formulas, I now have the same efficiency as that belt system with a hub motor.

[quote="longhairedboy, post:95, topic:35056"]
Most aren't there yet and the people who are aren't sharing.
[/quote]

We're there, and sharing it.

[quote="longhairedboy, post:95, topic:35056"]
I don't consider Carvons to be hubs. Those are direct drives and solve a lot of problems hubs have.
[/quote]

Besides getting more thane for a better ride quality, what else do they solve? Both the raptor 2 and hummies hubs have an interface that allows us to make different wheels that are easily swappable also.

They introduce new problems too, such as what happens when you hit a stone larger than the space between the motor can and the street?

[quote="trampa, post:89, topic:35056"]
This big and heavy motor doesn't fit inside the wheel any more.
[/quote]

You can fit a motor 4 times the size into a wheel. We have done it and Enertion did also. This is why heat is not an issue for either of us anymore.

Look, @trampa, you should be the least scared of any of the belt drive vendors out there. I think it will be hard to replace off road boards completely with hubs. But for street boards, with these new round of direct drive/hub motors, we do get the same efficiency as a belt drive now due to the large motor size, so the option is simple for new builders. 

Complexity (belt drive), or simplicity (hub motors)? Your getting the same efficiency either way now. It's just one weights a bit more than the other. And that's the only thing hubs can't make up on belt drives, weight. We can match the performance otherwise by simply going larger.

Now you can say well, let me put a motor that large on my belt and pulley system, but again, the belt becomes the bottle neck for transferring power. There's no bottle neck with hubs. It's direct power to the pavement.

I honestly think you guys have no idea what the real size of these hub motors are... I didn't realize how large the raptor 2 motors are until I saw them in person, pictures don't do justice.
```

---
## \#97 Posted by: trampa Posted at: 2017-10-09T15:43:52.245Z Reads: 131

```
Rode them already. First board shipped by Jason. A customer from Berlin met up with me...
So I know what we are talking about. Even dropped VESC-Tool on, which worked just fine. Reinstalled the Jason FW later again.
The motors are huge and there are two of them. I had a Carver with me, single drive 6364, 136 KV, 14/33 transmission.
The performance was pretty much the same. And doing the maths from the settings in VESC-Tool, both boards should output the same amount of power (Watt wise). 
I could not feel to much difference. I gave both boards a full acceleration on the flat and up the hill. So the belt was no bottle neck, since I only had one Belt drive without idler vs two hubs. 

_Now you can say well, let me put a motor that large on my belt and pulley system, but again, the belt becomes the bottle neck for transferring power. There's no bottle neck with hubs. It's direct power to the pavement._

Well, you would wind the motor to have less torque and the issue is sorted. Same torque at wheel but a lot more efficient, single drive instead of twin possible! 

Don't get me wrong, I'm not totally against hubs! I just want people to understand the physics and that comparison is done Apples to Apples only. There is no one horse for all tracks and personal preference varies a lot. It's the customers choice in the end. The more informed the customer is, the better he can decide what is good for him. And a lot of customers want hubs. Others want belts, so watt. Maybe we will make a hub drive one day, who knows....

Frank
```

---
## \#98 Posted by: evoheyax Posted at: 2017-10-09T15:47:29.530Z Reads: 131

```
Lets just compare hub motor prices vs belt drive prices for a dual drive setup:

If we go to torqueboards store, we can buy everything except for esc's, power switch, battery, and the deck for $480 for a dual drive belt system.

Now, everything in the hub version of those motors (hummies) right now is priced at $450 ($400 per pair if your doing 4wd or we're desperate for cash, lol).

So for $30 less, you get a simpler motor, that runs just as efficiently, but with only downside being extra weight with the hub motors.

Why would the masses want to deal with belt drives anymore?

You also forgot that for most people, and I mean the vast majority of people, don't need this kind of power to begin with. They are already more powerful then they need to be...

So even a single drive hub motor might be sufficient for lighter riders in flat areas who are going to go under 20 mph anyways. I watch these people riding all over sf on these cheap boards, and they ride very slow most of the time (under 15 mph), not just because it's more efficient or the board can't do faster, but because they don't feel safe riding any faster. Unless your a skilled rider, 20 mph feels really fast, lets not forget that. To the riders who have been at this for 10+ years, 35-40 mph doesn't feel unreachable at all, while the majority of riders out there will not want to go this fast.
```

---
## \#99 Posted by: evoheyax Posted at: 2017-10-09T15:57:25.363Z Reads: 132

```
[quote="trampa, post:97, topic:35056"]
The more informed the customer is, the better he can decide what is good for him.
[/quote]

I agree, but the problem right now is, there's a lot of mis information out there about hubs. Since you confirmed from vedder himself that you need a motor 4 times the size in a 1:1 to have the same efficiency for a given torque, and since we've shown it's possible to do so, I think any belt drive vendor should give their customers the understanding that hubs can do the same as a belt drive, just in a much larger package.

The small hubs today are at best, double the size of the motors most are using today in belt drives. So as a result, you get terrible efficiency. These new larger hubs are are closer, if not 4 times the size of the motors used on most belt drive systems. So you can do the same from a hub motor.

Now vyou can use a lrger single drive motor and compare it to a dual hub motor board. But you can't fit four of those large motors on a board, and I can fit 4 hub motors on any board. So neither is better in this case...

My whole goal on this forum has been t educate people. This is why I've written so many guides, and share a lot of what most would call trade secrets. I want to see this sport evolve faster, rather then slower.
```

---
## \#100 Posted by: longhairedboy Posted at: 2017-10-09T16:22:53.129Z Reads: 136

```
[quote="evoheyax, post:96, topic:35056"]
Besides getting more thane for a better ride quality, what else do they solve?
[/quote]

The BIGGEST problem. Cooling. Half of this conversation has been about caged heat. there's no cage here.  The second biggest problem: Wheels wear out and should be replaceable. Replaceable with the wheels you want not the wheels you're stuck with. 

About rocks. Ok so lets take a couple of 6355s and throw them out backboard to get them to a similar distance from the ground as the carvon drives are. Now they're low as shit and banging on the street. 
https://www.instagram.com/p/BWokznFgq44/?taken-by=theonlykindajake

yeah motor cans can probably handle some rocks. 

Of course different things have different problems. I ordered extra bacon on my steak club today and now i'm feeling a little greasy. IT was different, and now i have a different problem. The question is, are those better problems than you had before?
```

---
## \#101 Posted by: b264 Posted at: 2017-10-09T16:41:28.198Z Reads: 132

```
[quote="longhairedboy, post:100, topic:35056"]
The second biggest problem: Wheels wear out and should be replaceable. Replaceable with the wheels you want not the wheels you're stuck with.
[/quote]

Also, when they wear out, I don't want to be vendorlocked to any certain polyurethane supplier/manufacturer.  And I want to choose my wheels too.  And I want wheels that are designed to be the best wheels for a longboard, not wheels that have been shoehorned in with other engineering goals.  If your wheels suck, then your entire board sucks.  The wheels are what makes it work.
```

---
## \#102 Posted by: evoheyax Posted at: 2017-10-09T17:00:19.216Z Reads: 133

```
[quote="b264, post:101, topic:35056"]
And I want wheels that are designed to be the best wheels for a longboard, not wheels that have been shoehorned in with other engineering goals.  If your wheels suck, then your entire board sucks.  The wheels are what makes it work.
[/quote]

lol, people like Chris come here, and talk about wheels, but the reality is, they are not doing rocket science. There's no reason why others can't make wheels just as good. It's a process, but that's how they made them in the first place. They didn't wake up one day, and say, oh, I'm going to start making wheels with this magic formula and they will be great. Give hub motor manufactures time. There will be a wide array of options, and wheels will just get better.
```

---
## \#103 Posted by: longhairedboy Posted at: 2017-10-09T17:33:58.012Z Reads: 133

```
[quote="evoheyax, post:102, topic:35056"]
the reality is, they are not doing rocket science. There's no reason why others can't make wheels just as good. It's a process, but that's how they made them in the first place. They didn't wake up one day, and say, oh, I'm going to start making wheels with this magic formula and they will be great. Give hub motor manufactures time. There will be a wide array of options, and wheels will just get better.
[/quote]

That is correct. It is simply iterative formulaic science. Making good wheels is an iterative process that has had much, much longer to mature. Hubs have a ways to go thane wise. Materials science just isn't there yet. You can't absorb the same kinds of impacts with less thane as you can with more thane. Ride quality is directly affected. Chris didn't spend several years trying and failing urethane formulas because any fool can make wheels. IF any fool can make wheels now, its because companies benefitting from thane formula trial and error such as Chris's are popping them out. 

Can i call up Labeda and throw $10k at them and get wheels? yes! Can i call Chris up and throw $10k at him and get SuperFly's in pink  and with a bizarre durometer? Yes! 

Can i ever possibly get as much thane on a hub as I can on a direct drive or belt drive or gear drive? No!

Heat is still a problem, even though its a lot less of a problem than it was in two of the hub designer's motors out of a swath of garbage out there. Thane is still a problem, though the degree varies subtly between hubs.
```

---
## \#104 Posted by: b264 Posted at: 2017-10-09T17:42:44.962Z Reads: 126

```
[quote="evoheyax, post:102, topic:35056"]
There's no reason why others can't make wheels just as good.
[/quote]

Actually, there is one reason.  If you have to [try to fit a motor inside](https://www.youtube.com/watch?v=kHYiyv68q2o) it that's as big as possible.
```

---
## \#105 Posted by: NickTheDude Posted at: 2017-10-09T18:05:10.887Z Reads: 126

```
Sorry, I'm still not clear on why reductions are theoretically more efficient.

Is it because as torque in the motor increases, losses increase exponentially while when you use reduction the relationship is linear? And hub motors will always have to output more torque cause of no reduction?

Also if the only difference between the setups is ERPM then wouldn't changing the amount of poles fix that?

Sorry if my confused ramblings are derailing things, I've just always been curious about this.
```

---
## \#106 Posted by: Hummie Posted at: 2017-10-09T18:42:04.079Z Reads: 132

```
Me too.  Torque takes amps. Without a reduction u need more torque from the motor for same motor torque output.   U can trade speed for torque w a gear. If the motor is big enough though it's not a problem. More poles gives greater control but not really almost any more torque. U either end up w a bunch of smaller weak magnets or large powerful. Surprisingly despite a magnet's strength not being linear and they are stronger when closer..many experts have told me no free ride there. At best with more poles u can decrease the airgap diameter(not thickness) as the many magnets can be a hair less thick for same strength when in an array so now the aigap could be at maybe 47.5 instead of on the 47. It made sense thered be a lateral airgap and decreasing it would enable less current needed for same leverage.  Makes sense but at this point I've heard it from many experts saying it doesn't work that way.  Why I don't know.  
Bigboytoys has two hub motor sets, one w double the poles\magnets but I think otherwise the same. I think he might be able to do a comparison.
```

---
## \#107 Posted by: BigBoyToys Posted at: 2017-10-09T19:10:27.569Z Reads: 136

```
Unfortunately I just dissassembled them and the newer version of the TB hubs has a longer stator than the earlier version in addition to having 24poles so anapples to apples comparision for 14 vs 28 pole counts motors isnt possible with these. <img src="/uploads/db1493/original/3X/5/2/5220a709d05d808105fe3def709f664942624fdc.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/8/18e778a9c25281603c305b60ce6bf6bfd3ef440b.jpg" width="666" height="500">
```

---
## \#108 Posted by: trampa Posted at: 2017-10-09T20:11:31.136Z Reads: 138

```
[quote="evoheyax, post:99, topic:35056"]
Now vyou can use a lrger single drive motor and compare it to a dual hub motor board. But you can't fit four of those large motors on a board, and I can fit 4 hub motors on any board. So neither is better in this case...
[/quote]

You would need four motors while I would still only need one to outperform the four. Have you seen Jens Twin Leopard 80mm attached to one of our boards, twin VESC SIX at 120A per motor (5.3KW per motor). F...hell fire...
Even one of them would have outperformed a quad hub drive with ease, assuming realistic 1.2KW per hub. Motor size is approx the same.  

http://www.electric-skateboard.builders/t/e-toxx-directdrive-vs-trampa-vesc6-vs-leopard-8072-170kv-vs-nowind/30822/176

Apples to Apples again: single drive vs.single drive. 

At this stage we have roughly the same output power if we compare a rather small 650gr single belt drive motor to two big fat hubs (approx 1.2 Kg each), while the single belt drive is way more efficient, stays cooler and is light weight. And if you have an issue its only one issue, one motor, one ESC, one sensor cable to fix.

You can stick four hubs or belt drives to a board, but who wants that? Keep things simple!
The best part in a system is the part you don't need, agreed. You could argue that hubs stripped away the belt drive - at the price of two heavy motors, two ESCs and less efficiency. That is not really "getting rid of parts" in my eyes. It is shifting around things at the price of triple the weight and no choice of Urtehane/Wheels. To some this is appealing, others have a different view. From a vendors point of view this is appealing, since you can sell a lot of spare tires to your customers. Each hub sells four tires over time and there will be no standard. But you will sell zero tires to customers of your competition... 

**Other industries:**
Why cars have no hub motors although the would have the space to fit them: Weight is the answer. Heavy hub motors cause problems to the suspension system - more mass swinging up and down + batteries are heavy already and you want the car to be light. So they use a single or twin, small, geared motor instead. 

Modern E-Bikes use geared motors to keep the weight low and benefit from the efficiency gains. Less magnets, copper, centred weight, a lot more power etc. 

Wind turbines usually use geared systems. Some still use direct drives but neodymium price stands against this technology >> 10x the neodymium per MW. 

**Other industries have been through the hub design matter and ended using geared system.** Electric motors simply like higher RPM and low torque. Power density and efficiency is a lot higher when you gear down. 

The golden rule: If your application is running at high RPM low torque you can go for direct drive (e.g. spinning a small propeller).  If you need torque and low RPM you gear down.

And now I would like that heavy extra bacon thing @longhairedboy was talking about. Could you post an image please.  I imagine it to come with enough grease to kill a donkey. 

Frank

Ps.: I'm not sacred of hubs. What really scares me are those 80mm Leopards. They are lifting the boards front wheels when you pull the trigger. The only downside: The gears need extra grease...
```

---
## \#109 Posted by: Hummie Posted at: 2017-10-09T20:32:51.400Z Reads: 132

```
but there are hub motors on cars and bikes still and no sign of them disappearing.   lots of people use them and are happy with them.   Even if the hub is not 4x as big, and there were to be decrease in efficiency, there are many other benefits.  the biggest reason I got into hub motors is lack of noise of pulleys and I like the simplification and with it there's a lot less maintenance and possibility of parts to break.  and they do break.
   I know I was getting awesome efficiency with even the last hub motors and will get a test done...a real test...soooon.
```

---
## \#110 Posted by: calnick0 Posted at: 2017-10-09T20:49:49.212Z Reads: 134

```
[quote="racidon, post:61, topic:35056"]
As for efficiency, no watter what you do using a gearing system will always make a motor more efficient. That's just how mechanics work. Perhaps if you find some magical law that changes how physics work you can let Car manufacturers know so that our vehicles can become cheaper, removing Diffs and Gear boxes for us!
[/quote]

Teslas don't have multiple gears.
```

---
## \#111 Posted by: NickTheDude Posted at: 2017-10-09T20:50:11.750Z Reads: 129

```
This apples to apples thing is stupid. What kind of apples are you talking about? weight? If so then belts clearly win. If your apples are power output then apples to apples each has their advantages. I want hummies hubs cause they look cooler, their simpler to make a DIY with and I don't care about the extra weight or lower potential maximum power output as a dual drive will likely be enough for me.
```

---
## \#112 Posted by: calnick0 Posted at: 2017-10-09T20:51:36.343Z Reads: 124

```
[quote="evoheyax, post:63, topic:35056"]
Yes, gears are more efficient when you have many gears. But electric skateboards have one gear, not many. So they aren't utilizing their full potential. **Do you see cars with 1 gear?** no.
[/quote]

The Model S has always had just 1 gear. The Nissan Leaf has 1 gear. The BMW i3 has 1 gear.
```

---
## \#113 Posted by: Vanarian Posted at: 2017-10-09T21:11:59.715Z Reads: 122

```
The Koenigsegg Regera has only 1 gear too !

@evoheyax Thanks for the precious infos specially about awg wires differences IRL tests. When my motors fail on my due to heat I'll know what to upgrade first.
```

---
## \#114 Posted by: b264 Posted at: 2017-10-09T21:15:29.239Z Reads: 123

```
[quote="calnick0, post:110, topic:35056"]
Teslas don't have multiple gears.
[/quote]

Neither do locomotives.
```

---
## \#115 Posted by: Jreamer Posted at: 2017-10-09T21:24:33.291Z Reads: 122

```
I mean if you add a transmission to the board then hubs become second tier.  Seems like a very tough engineering challenge.
```

---
## \#116 Posted by: Jreamer Posted at: 2017-10-09T21:28:51.694Z Reads: 126

```
Doesn't it really come down to acceleration/top speed/efficiency? IDGAF about weight if I can get all the same metrics I care about in a hub.
```

---
## \#117 Posted by: Hummie Posted at: 2017-10-09T21:59:00.157Z Reads: 126

```
This debate is old and been going on in the bike world for a while with hubs vs mid-drive and results depends on the motor specifically and what type of riding.  General use will see a mid-drive do better, with the motors out there now, but a hub can be better efficiency in some cases such as sustained high speeds.  We will see.   There's also what happens to the energy when it's not converted to torque...is it stuck on a stator or is there a good thermal pathway to a good heatsink that can dissipate it into the air or something.  in that department a skate hub motor has an advantage over pulley motors or bike hub motors.  Even if the motor is bottled up inside urethane, which is very much a thermal insulator, air is not much better of a thermal pathway when there isn't much surface area to get it out there.   The new design I have coming with a hollow center has a huge amount of surface area as well as ability to transfer heat with great contact surface area going to a huge aluminum hanger.   I'm dying to do some testing and this week will.  maybe @Jinra you could do loops with me somewhere and we can compare watthours spent?
```

---
## \#118 Posted by: Okami Posted at: 2017-10-09T22:29:10.450Z Reads: 123

```
woah a lot of technical details in this thread ( will read them later)..

but @BigBoyToys does it mean that the motor with more teeth on the left has lower KV rating?

Im also still getting into this motor technology thing :)
```

---
## \#119 Posted by: racidon Posted at: 2017-10-09T23:16:15.191Z Reads: 135

```
[quote="NickTheDude, post:83, topic:35056, full:true"]
So (other than heat dissipation) why is a 100kV hub worse than a 200kV 2:1 belt drive?
[/quote]

I don't think either are worse or better than the other mate.

I think a lot of people here lost what the initial debate was once someone made a comment along the lines of the "belt drive guys" or whatever it was. A lot of the debate was not belt drive motors are better blah blah etc, it was that you can't make the claim hub motors are more efficient than a geared system, it's fundamentally wrong.

The key part of efficiency is the amount of input versus the amount of output. A 1:1 system will always generate more heat.

As for "apples to apples". I'm not sure why we started comparing weight.. as far as I'm concerned you can't compare anything other than the same kv or W based motors otherwise your comparison is pointless.

The reason you see this claim of "hub motors are more efficient" comes from the following analogy.

Geared systems have had a guy that's been able to lift 50kg/110pounds in a 1:1 ratio. He's been using a seasaw to do it though allowing him to lift 500kg/1100pounds with the same effort. Then came hub motors, to make it so that they can lift 500kg/1100pounds, they pumped the iron at the gym until the guy could lift 500kg/1100 pounds. The thing you have to note here is that both guys have to bust their asses to lift their 1:1 ratio. However you get that buffed guy a seasaw and all of a sudden 500kg/1100 pounds is something he can do with a single finger, thus requiring less effort, creating less heat, wasting less energy, creating a more efficient system. That is why you can't argue that gearing a motor will not make it more efficient. That is also why comparing a 100kv to 300kv @ 1:1 ratios efficiency is completely pointless.

Lastly, don't think I'm banging on hubs. They are my next focus on my next build. I love my dual leopard trampa and I'd challenge anyone to make a hub setup that can compare to the acceleration, speed and distance that thing can do. However it also attracts a lot of attention and I'd like a more stealthy setup ;) but I'm under no delusions that it would do much more than **_get me around town_**
```

---
## \#120 Posted by: Jinra Posted at: 2017-10-09T23:18:51.155Z Reads: 138

```
Sure maybe this weekend. We have a group ride on saturday, but maybe we can meet up sunday
```

---
## \#121 Posted by: BigBoyToys Posted at: 2017-10-09T23:21:13.070Z Reads: 139

```
Those stators are out of the newer and older version of Dexters TB hubs. Both are 130KV and have a 52mm diameter stator as part of a hub motor with a 90mm wheel. Hummie suggested we use them to compare the torque generated by a 24 Pole motor vs a 14pole motor but since the newer versions stator is also 10mm longer it's not a fair comparison. Some of the extra torque the 24pole motor creates comes from the extra length, so it would be hard to tell how much torque increase was from the increased pole count and how much is from the longer stator. Either way, these are the motors that convinced me that hubs can make torque. Hummies motors have comparable sized stators that are actually 7mm longer than then new version of the TB hubs pictured in my last poat.

My dual 170KV 6364 trampa with 15/66 gearing and 50A/100A current settings has very impressive acceleration but tops out at 24mph. Even geared down at over 4:1 ratio it pales in comparison to the start up acceleration and 40+mph top speed of my 4wd hub board. 

Also, my current 4wd hub board  with 12S6P weighs the same and has better range if not more than my 10S8P trapma with only 2 motors. 

A picture's worth a thousand words, so here's a video....or two.

https://youtu.be/ovGadNwhXOA

https://youtu.be/jSLgboSxy3o
```

---
## \#122 Posted by: BigBoyToys Posted at: 2017-10-09T23:52:33.923Z Reads: 136

```
[quote="Jreamer, post:116, topic:35056, full:true"]
Doesn't it really come down to acceleration/top speed/efficiency? IDGAF about weight if I can get all the same metrics I care about in a hub.
[/quote]

I feel similarly, my Trampa's a beast of board, super heavy and looses lots of efficiency to the off road pneumatic wheels but I still think its awesome and is one of my favorite boards to ride. The trampa Im building now will weigh over 40lbs and take over 50whr/mile!

Considering that any powerful board with a decent range is going to be heavy, 5 or 6lbs extra in motors for double the torque (compared to a 2wd hub board) and more topspeed is a compromise Im willing to make. That means I really dont even care if hubs are less efficient (i still think think they are very efficient at constant speed)as long as they break 30mph, accelerate well, dont overheat, wheels dont fly off, the ride quality is good and I can fit enough battery underneath to get 10-15 miles of range, none of which seem out of reach with the cureent and new hubs/direct drives entering the market.
```

---
## \#123 Posted by: psychotiller Posted at: 2017-10-10T01:20:37.980Z Reads: 132

```
[quote="BigBoyToys, post:122, topic:35056"]
That means I really dont even care if hubs are less efficient (i still think think they are very efficient at constant speed)as long as they break 30mph, accelerate well, dont overheat, wheels dont fly off, the ride quality is good and I can fit enough battery underneath to get 10-15 miles of range, none of which seem out of reach with the cureent and new hubs/direct drives entering the market.
[/quote]

Me neither! I'm pretty sure everyone is on the same page there. But the constant claims that belt drives are less efficient and problematic in comparison to hubs is fake news. I personally wouldn't chime in on any of these hub threads otherwise.
```

---
## \#124 Posted by: GrecoMan Posted at: 2017-10-10T01:21:35.445Z Reads: 131

```
[quote="psychotiller, post:123, topic:35056"]
fake news
[/quote]

uh oh...

Is that Little Rocket Man I hear?
```

---
## \#125 Posted by: psychotiller Posted at: 2017-10-10T01:22:42.064Z Reads: 131

```
Shouldn't you be making gears or something!?
```

---
## \#126 Posted by: GrecoMan Posted at: 2017-10-10T01:23:53.977Z Reads: 133

```
mounts actually :wink:

<img src="/uploads/db1493/original/3X/8/5/8595433ec2f1c5578c8bf16027f95f508ef47cc4.jpg" width="690" height="388">
```

---
## \#127 Posted by: psychotiller Posted at: 2017-10-10T01:25:23.071Z Reads: 133

```
Maybe put a wheel on the end and you wont have issues on those round truck hangers. :grinning:
```

---
## \#128 Posted by: GrecoMan Posted at: 2017-10-10T01:26:12.735Z Reads: 134

```
lol wat...
```

---
## \#129 Posted by: Hummie Posted at: 2017-10-10T01:46:39.687Z Reads: 133

```
that's not the mount for you bevel geared drive is it?  looks like it wouldn't take much lateral force.  looks like a regular mount
```

---
## \#130 Posted by: GrecoMan Posted at: 2017-10-10T01:47:53.656Z Reads: 133

```
nope that's for the jenso style direct drive

whipped it up in like 10 minutes for testing
```

---
## \#131 Posted by: evoheyax Posted at: 2017-10-10T02:09:34.638Z Reads: 134

```
Just got home from riding. And the verdict is in. I'[m up to about 10 miles of range, and even after that, I was only up to 150 F in one motor, and around 140 ish F in the rest. 

Torque is just insane, no doubt I'll crush most belt drives with this. From start (at standstill) to the end of a normal city intersection is less than 2 seconds. Way faster than most cars on the road in terms of acceleration.

And top speed is up to around 35 mph at only 80 kv (82 kv if you factor in the vesc can only do 95% duty cycle). I fly up 15% grade hills still maintaining above 30 mph. Since I have way more torque, I can get very close to that no load speed of 36 mph.

By definition, I'm getting twice the efficiency now, since I have twice the range and half the heat.

Now you say, only 10 miles for an 8 ah battery? Well when your doing hard starts and stops for 30 blocks, followed by miles above 32 mph (huge wind resistance), and then city riding again, followed by miles above 32 mph again, yea, 10 miles is really good.

Now if I rode at 15 mph with a light trigger finger, I bet 20 miles is easily doable. This is about the same range as a belt drive setup now, so what's to complain about hubs?

No wheels fell off, no deformation of the cores, no screws fell out, no rings fell out. Everything just worked like I couldn;t even imagine. Defiantly stronger than the raptor 2 right now (kinda expected since I'm running 4wd instead of 2wd).

Wheels still feel a bit jittery. Not the best at 30+ mph, but we gotta get a mold or two machined properly to get rid of the little imperfections that cause these jittery feeling at high speeds.

Really, not a concern at all for me, since I know it's easily fixable. That would be my biggest complaint right now. The rubber itself is good, but we gota make sure the lips of the wheel are more even, and that we don't get that line down the center. With the old polyurethane, that line wore off quickly, but after around 25 miles so far, They are still pronounced, and create vibrations that aren't ideal.

But it's all fixable with a better mold. This is what progress is about. Baby steps. The core works, so that's good. The motor stays cool now, which is good. The last thing to do is fix these imperfections with the wheel, and then, theres nothing to complain about.
```

---
## \#132 Posted by: evoheyax Posted at: 2017-10-10T02:21:53.152Z Reads: 133

```
[quote="b264, post:104, topic:35056"]
Actually, there is one reason.  If you have to try to fit a motor inside it that's as big as possible.
[/quote]

So did the math to compare to you guys what is the actuality.

We have a 58mm can, so  90-58 = 32/2 and you have 16mm of urathene for a 90mm wheel.
Now, ABEC Flywheels have a 45mm hub, so 90-45 = 45/2 = 22.5mm

16mm vs 22.5mm
90mm vs 90mm
hub motor vs ABEC Flywheel

Lets say we tale the wheel up to a 105mm.

Now, we have 105-58 = 47/2 = 23.5mm urathene depth, more than the 90mm ABEC.

So now, we have:

23.5mm vs 22.5mm
105mm vs 90mm
Hub motor vs ABEC Flywheel

So, if we go up to a 105mm, which these hubs can totally do, we have a thicker urethane patch than the ABEC 90mm Flywheels...

So yes, we can get great ride quality from hubs. If you want to set a mental barrier that it can't be done, then go for it. But it's simply not true, we are already not far behind a normal ABEC wheel as it is, and we can pass them with a bit thicker wheel...
```

---
## \#133 Posted by: b264 Posted at: 2017-10-10T02:43:41.183Z Reads: 128

```
If someone made a 105mm hub drive I'd be down for that.  Everytime I see "hub drive" I see "83mm" or "90mm" or "75mm" though.  Maybe this is but one way to fix this.  But that exacerbates the overheating problem.  But I'd try 105mm hubs for sure
```

---
## \#134 Posted by: evoheyax Posted at: 2017-10-10T03:00:21.989Z Reads: 130

```
My plan is simple. Just talked to hummie about it.

With this 20 awg wire, I can fit 2 or 3 more turns for a full copper fill. This will mean more copper, and lower kv (bit more torque, probably 70 kv), which will balance out the 105mm wheels. So I will be winding more in the near future and making 105mm wheels with these proper high heat cores.

Top speed will hopefully be about the same, but I'll calculate this before I wind.

Heat is not an issue anymore. I rode the shit out of them today. After the first mile with the small version of these motors (half the size), I got to 160 F. Today, 91 F. At the end on my normal commute, which is about 5 miles, The small motors would be at 260 F or even higher. Today with the new motors, 150 F was the highest and most were around 140 F.

So 1 mile old motors, 160 F.
And 5 miles new motors, 150 F. And that's with 8-10 mph more of wind resistance...

I'm a hard rider, heavy, ride through the avenues, so lots of full trotting from a full stop every block, get up to around 30 mph, and start braking again. This is around 25 blocks (1.5 miles), followed by smooth ride in golden gate park at around 35 mph another 3.5 miles straight. I don't sit around, I need to get to class, and I'm always running late, haha. So I push them hard. And they still won't overheat. Anything under 160 F is a win in my books, cause that's when efficiency starts to go down due to heat. Until then, the motors are just as efficient.

All problems in hubs until now and even today can be fixed. Give everything another year (probably way less), and the options of wheel size, hub motor size will change.

We're still planning on doing the 3x long motor, which will be even more efficient and powerful.

There will be some cases where belt drives will be a better option, but for most people, hubs will be a better option, and for many, already are.

I'm sure enertion will offer other wheel sizes in the near future, as we plan to also. And with both of our designs, in just a few minutes, you can switch from a 83mm wheel to a 105mm wheel. This is the easiest way also to finely tune top speed and torque and riding quality for each rider also.
```

---
## \#135 Posted by: FredSaberhagen Posted at: 2017-10-10T03:42:10.747Z Reads: 123

```
It puts the pics and video in the thread or it gets the hose again!
```

---
## \#136 Posted by: BigBoyToys Posted at: 2017-10-10T03:44:48.179Z Reads: 133

```
Well my origjnal statement wasnt that hubs were more efficient than belts as a general statement. I know hubs will always be less efficient at startup at least. It was a specific set of circustances I described under which I believe hub motors COULD be more efficient. I wanted someone to offer a valid reason why why it wouldnt. 

[quote="BigBoyToys, post:28, topic:35056"]
I think with good wheels and managable temps we should see hub efficiency surpass belt drives in SOME situations at least.
[/quote]

[quote="BigBoyToys, post:32, topic:35056"]
under low-med load cruising situations( at motor rpms within the efficincy range for its KV), where heat isnt much of a concern, the hubs should be more efficient since the motors do not have the frictional losses from the belts or from the higher motor rpm needed for a given wheel speed.
[/quote]

IMO, only one person was able to offer a valid reason why reduction drives would be more efficient than hubs UNDER THE SPECIFIC CONDITIONS I described at that was Frank @trampa  by sharing the following information.

[quote="trampa, post:89, topic:35056"]
Because of the square relation, it is desirable to run at as high speed and low torque as possible as long as we stay below 8.6k RPM. To express the square relation in some numbers, having double the RPM and half the torque at a certain power output will cause four times less losses.
[/quote]

Based on the above statement the belt drive motor would have less copper loses because it is operating at higher speed and lower torque than the hub motor.  That is a valid reason why hubs would be less efficient so thank you for explaining that. However, as also stated by Frank, copper loses are dominant in low speed high torque senarios and the the senario I described is the opposite since I said low load constant speed at 80% of max motor rpm (high speed/low torque for both motors). 

Frank also noted that above 8600 motor rpm other losses with in the motor start to be substantial. That statement leans efficiency towards hubs on high speed boards since 200KV at 12S on a belt drive motor to make up for the gear reduction would cost efficiency if your motor speed is aready exceeding 8600 rpm.

So what loses are dominant in the situation I described? I dont know exactly, but I do know that the faster you spin that belt with those belt cogs ziping through the air creating drag (also a square relation) combined with the energy it takes to bend that belt around your pulleys and the friction between the teeth, the more of the belt drives efficiency advantage is lost. Maybe thats neglible compared to the losses in the hub motor at high speeds idk, but Id like to. Where the losses come from at low speeds and hubs seems pretty well known and accepted.

Ive read through all the hub vs. Belts threads on the forum I could find but learned more on this thread so far than the rest. Thank you to all that have contributed thus far.
```

---
## \#137 Posted by: Hummie Posted at: 2017-10-10T04:03:36.890Z Reads: 128

```
iron losses, or switching losses, or core losses...as theyre known, are another square relationship based on speed and that's the other real loss in a motor. Eddy currents are one facet of iron losses and the other is magnetic hysteresis as the polarity of ferrous material is switching back and forth with a slight lag, in the stator and back iron.   ideally for the greatest efficiency of a motor it would balance these, so for example with little motors as we all use the primary loss is copper loss,  just I2r, current squared times resistance.   to be more efficient you'd want to make the motor bigger, and therefore it would have less R as the wire is thicker and would be more efficient as amps go through...and then at some point the motor is so big or the current so relatively small, or the speed so fast that those iron losses are the bigger loss and heat producer and that would be as efficient as you could get.
```

---
## \#138 Posted by: Cobber Posted at: 2017-10-10T04:21:05.323Z Reads: 124

```
@frank where does the 8.6k rpm ceiling come from?

where would I look for references of this...
```

---
## \#139 Posted by: Hummie Posted at: 2017-10-10T04:33:13.379Z Reads: 135

```
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

rpm losses section.  

iron losses become dominant at such a speed he feels.   60k erpm equals around 8.6k rpm with his goal top speed of about 25mph on a 84mm wheel with a 3.9:1 gear ratio.   the switching losses and eddy currents become considered too much. 
 60k erpm is also said to be a maximum speed for safe foc use on the 4.12.
```

---
## \#140 Posted by: Cobber Posted at: 2017-10-10T05:18:23.412Z Reads: 136

```
do you think it can be confusing for some when someone says one thing, but means something else taking several other things for granted?

essentially we are talking erpm then not rpm...
```

---
## \#141 Posted by: NAF Posted at: 2017-10-10T05:29:44.885Z Reads: 135

```
[quote="evoheyax, post:134, topic:35056"]
We're still planning on doing the 3x long motor, which will be even more efficient and powerful.
[/quote]

3xlong?? What contact patch width would it be? 
Please make the stator bigger in height as well to match raptor 2 size.
```

---
## \#142 Posted by: Hummie Posted at: 2017-10-10T05:37:21.117Z Reads: 130

```
He’s talking about both.  60k elec equaling 8.6k rpm w his setup
```

---
## \#143 Posted by: evoheyax Posted at: 2017-10-10T05:54:00.397Z Reads: 133

```
[quote="NAF, post:141, topic:35056"]
Please make the stator bigger in height as well to match raptor 2 size.
[/quote]

I've desired that for a while now, and it might happen in the future.

But the thinner motors allow for thicker urethane depth.

This is why I say, there's trade offs to every viable hub motor option at this point. a 90mm, the wheel of the raptor 2 is 11 in urethane depth. There appears to be some kind of core like material between the steel can and the wheel, which is about 2mm thick, so if you take those 26mm off, your looking at 64mm can size. That means to catch up to our 105mm wheel, the raptor 2 would need a 111mm wheel to get the same depth.

Now, maybe at that point in size, what is an extra 6mm? But maybe that extra little bit means a lot to some. Why do people buy 97mm abec flywheels instead of the 90mm?

They are more versatile, because regardless of the wheel size you want, they can do it. 70mm (not recommended, but possible), 83mm (more practical), 90mm (getting plusher), 97mm (plush), 105mm (ultra plush), even off rode tires at these lower temps could be possible. The ribbed structure is versatile, and really any wheel that fits that shape will work. So make wheels around it. The options are endless.

I do want a thicker motor in addition to this one though. The triple wide is 105mm contact patch I believe. Might be a few mm less. Quite large, but it's possible entirely to run as a single drive... Or for people who want to run dual drive that would otherwise need a quad drive, it should work well.
```

---
## \#144 Posted by: NAF Posted at: 2017-10-10T06:31:52.195Z Reads: 117

```
With 64mm can and your 3xtimes longer stator and 107mm thane we are looking at almost 22mm depth of urethane which is sufficent enough and provides good ride quality. That would be the best compromise there is..beast of a motor with awesome torque -- so no need for 4wd. 2wd would be suffucient for most people with full urethane wheels at front which adds additional comfort. Also 107mm will add to top speed.
```

---
## \#145 Posted by: evoheyax Posted at: 2017-10-10T07:04:07.992Z Reads: 117

```
Maybe well shoot for the moons with the next motors. I see a future were customers choose between a few models, that target difference audiences. The 4wd of those motors would be real houses.

Theres also the issue of the stator. Gota find one that they already have a mold for or were looking at almost 5k in mold costs.

This is why structure and organization is necessary, because coats to make small pieces of the puzzle add up in the first round.

I believe the new design is what we will likely sell indefinitely. Once the assembly process is streamlined, we'll start looking at even better options. Need get motors going to gain funding future developments though. Like better quality wheel molds. The future looks bright though. I know now after the tests I've been doing that theses are the first hubs besides the raptor 2'a not to give me heat issues. They are quite quiet, and pack a mean punch when you slam the throttle. Luckily a have nice pockets on my board for my feet and learn absurdly far forward lol.

Also remember that your setup makes a huge difference in performance. I recommend 12s with these hubs.

120 motor amps, 30 amps per motor using @Ackmaniacs firmware. Worked great for me so far. Great acceleration and braking. Enough so that I feel content with this size for the time being. Just want bigger wheels personally lol.
```

---
## \#146 Posted by: Vanarian Posted at: 2017-10-10T13:30:06.029Z Reads: 122

```
I'm not sure this has already been pointed out but 4WD hub setups generates 2 flaws / requirements : 

- you need 1x ESC per motor thus 4x ESC to run 4WD 
- above point allows better efficiency and overall less strain on both batteries, motors and ESC, but it requires more space and consequently more money
- you may aim for the lowest possible weight for a daily commuter for when you'll carry your board instead of using it ; so 4x motors averaging 700Gr minimum each (optimistic figure) + 4x ESC averaging 350gr each (optimistic figure again) alone is worth more than 3Kg to account for...to this you add all the rest : batteries, deck, trucks, wheels, enclosure
- setting 4x ESCs together, if not a plug-and-play solution, may prove to be challenging and a possible source of failure during ride (I'm thinking about fried VESCs due to bad CAN bus setup/communication).. If reliably done though, that's also an higher failsafe level (as long as at least 1x motor and 1x ESC work over the 4, you're able to get back to home and check later what failed).

IIRC a bit of conversation with @Hummie and LEVer/Pediglide, the efficiency of a small hub setup raises up drastically when you multiply them right?

For average numbers a single hub drive would get you only around 50% of mechanical power at best and remaining 50% of fed energy works hard to turn it into a barbecue. Dual hubs perform way better at around 75% efficiency on both motors, 4x hubs push the number toward upper 85-90% I think ?

Now an efficiency curve is only a curve and even with our current tiny hubs you **get** power and move. But how much should your upgrades improve these average numbers ? 

My 2 cents, most builders will stick to 1WD & 2WD letting 4WD / AWD to be the top choice for dragster users. 1WD hub drive for a skateboard is currently a very limited and low torque solution, do you think big hubs like yours, Onloop or Hummie's are enough to turn the low end into a decent solution or you'd still advice making belt drive if you do 1WD ?

BTW I'm gonna go Frankenstein on a stator and do dirty experiments because of your topic dude. Since energy and heat can be managed better, let's try and raise mechanical output.
```

---
## \#147 Posted by: evoheyax Posted at: 2017-10-10T14:11:22.578Z Reads: 119

```
It hunk with these small motors, efficient at 4wd is at best 60%. Dual drive is maybe 50% probably less.

With these new motors, I'm seeing efficiency at around 90 to 95%. Very high. Heat with 4 of these double sized motors is not an issue any more.

I think dual drive will be fine for 75% of users at least. Heavier guys (250 ish lb or more) or those around 200 lb with lots of hills like me, should do 4wd.

Yea, 4wd adds weight, but remember it also distributes weight more evenly, making it easier to carry, as long as the extra weight is not too much for you.

There are some risks, but if done correctly, those. An be mitigated. I be live when I have my first 4wd board for sale, I will have these little things ironed out and they will be non issues. I haven't had a canbus failure since I bought this quad bra from Chaka.

Motor failures, yea, and I was still able to ride home, always. That's the hidden beauty of 4wd.

These motors, in my tests, show they are more than 5 times better at staying cool. 1 mile, 160 f before. 5 miles, 150 f now. That's a huge difference.


I think 1wd will be possible with a slightly bigger version of this. If we went wider or longer or both, 1wd hub motors become totally doable.
```

---
## \#148 Posted by: chaka Posted at: 2017-10-10T14:34:06.207Z Reads: 118

```
I am having a little trouble following along without chiming in with a few facts. With each motor you add, power consumption will go up. The 5065 motors we sell consume about 45 watts unattached and free spinning. If I use 4 of them my free spinning consumption would be 180 watts! Thats with the wheel unattached.

Our 6085  motors consume about 70 watts, a quad with these will consume 300 watt! And this is just the power it take to keep the motor spinning at WOT.

These figures were taken while at 44.4v
```

---
## \#149 Posted by: Jreamer Posted at: 2017-10-10T14:43:25.078Z Reads: 111

```
Not quite how it works.
```

---
## \#150 Posted by: chaka Posted at: 2017-10-10T14:44:10.340Z Reads: 114

```
How so, do motors magically stop consuming power once you apply more load?
```

---
## \#151 Posted by: Jreamer Posted at: 2017-10-10T14:45:22.042Z Reads: 112

```
More like less load across the 4 motors.
```

---
## \#152 Posted by: chaka Posted at: 2017-10-10T14:47:08.939Z Reads: 112

```
Adding more motors just consumes more power, did you miss the part were I explained this is with motors spinning free, no load.
```

---
## \#153 Posted by: Jreamer Posted at: 2017-10-10T14:48:11.678Z Reads: 112

```
So 2 motors are going to work harder to get me up a hill compared to 4. They stay cooler. Cooler means they are more efficient.
```

---
## \#154 Posted by: chaka Posted at: 2017-10-10T14:50:07.403Z Reads: 110

```
This was a topic from years ago, we all came to the conclusion that a single drive is the most efficient. You get more miles per watthour
```

---
## \#155 Posted by: Jreamer Posted at: 2017-10-10T14:52:09.680Z Reads: 114

```
How where hub motors years ago?
```

---
## \#156 Posted by: longhairedboy Posted at: 2017-10-10T14:58:13.440Z Reads: 115

```
good god. 

i will build whatever anyone wants but there's no way anyone can tell me 4wd is more efficient than two and that the benefits of 4wd even remotely make it worth doubling the cost and weight of the drive system, not to mention 4 motors do not double the power of a two motor system on the street. The same amount of power just gets redistributed when used on the same battery pack, except now its being distributed across more copper and losing energy to inefficiencies across four motors instead of two. 

*yawn*
```

---
## \#157 Posted by: chaka Posted at: 2017-10-10T15:00:00.050Z Reads: 119

```
It makes no difference, adding more motors will always add more power consumption. It is inescapable, the key is providing adequate power with a minimal amount excess power usage. It is a Goldilocks scenario, if you want efficiency you need to provide just enough power capability for the design parameters. Too big or too many motors and you have excess consumption. Too little and you waste it with heat. Ideally we would use one big motor if we want a board built for range.
```

---
## \#158 Posted by: FredSaberhagen Posted at: 2017-10-10T15:11:40.518Z Reads: 119

```
Negative ghostrider - more motors to divide the current across resistances is actually more efficient - because resistors added in parallel actually decrease resistance ;-)
And since resitive losses are proportional to the square of current, if you divide current by two you improve (at least on resistance of windings) by a factor of 4.
Divide current by 4 and you improve by a factor of 16!!  :-0
Ofc what ends up happening is you have 4wd you start dumping hella more watts into the system because it's so fun lol.  But if you were building a long range system and could choose between 1 giant motor or 4 smaller ones your resistive losses would be much smaller in the system with 4wd
```

---
## \#159 Posted by: chaka Posted at: 2017-10-10T15:14:05.162Z Reads: 118

```
I thought the same thing, works on paper right? The reality is much different due to several factors. It wasn't until I started running real world test that I saw the difference and it is huge.

Where's @lowGuido when we need him?
```

---
## \#160 Posted by: Hummie Posted at: 2017-10-10T15:21:09.902Z Reads: 116

```
But MOTors are inductors. Maybe can be understood as resistors.  I'd think 4 motors with .06ohm resistance would produce the same heat as one big motor at .015ohms.  4 or 1 wouldnt make a difference in efficiency. I2r losses the same
 It would possibly help dissipate heat better w 4.  
Current spent at no load and core losses  I'd think would be the same or similar between the 4 or 1
```

---
## \#161 Posted by: Vanarian Posted at: 2017-10-10T15:30:48.172Z Reads: 112

```
Can rolling drag be a reason for this huge difference?

In riding condition drag is almost not noticed with hubs because there is lot of weight over a single rotation axe, no peripheral loads, magnets drag becomes negligible compared to the rider's weight. 

What about unloaded free spinning, magnets drag should become a more important data to account for thus require more amps (usually lost in the mass of wasted amps necessary to haul some weight around). 

Or that's my misunderstanding and it is all about copper resistance : more copper cable length to feed = more energy wasted?
```

---
## \#162 Posted by: evoheyax Posted at: 2017-10-10T15:32:33.926Z Reads: 117

```
Your talking about belts drives. Belt drives have resistance when spinning without a load. Add more belt drive motors, and you gain more resistance, so yes, it takes more energy.

Good hub motors have little to no resistance when spinning without power. Add more, and you split up current and you should reduce waste. I'm not 100% sure, since I haven't done real world tests. But @FredSaberhagen has a good point.

If you ride in variable terrain like me, then theres times I need to climb mountains, and theres times I need to ride flat for miles, in the same trip. Now you'll say a dual drive belt system can be geared to be efficient for both circumstances, I see that one coming.

Hub motors are a bit different. When climbing steep hills, due to the disadvantage I believe we all agree on now thanks to frank. 4wd gives good efficiency at all times. Why is it that I could get 20 miles with a 4wd hub motor and 8ah battery (if in the ideal conditions), and little heat, if it was not efficient?

Even if I was to get worse efficiency with 4, I get closer to the no load speed, more predictable acceleration, better handling (especially around corners), and your doing less work per motor, so you should expect a better life cycle.

Yes, it costs more up front, but if it last 5 years instead of 3, is it really that much more?

The only real downside is more weight. But for people like me, it's not an issue. I hope on and go to class. Put it down, charge it, and when I'm ready to go home, I unplug and go. I don't need to carry it around very much.

Even if it is less efficient, by how much? Clearly, not what your saying. I don't think anyone can get 40 miles on an 8ah 12s battery. If for some reason, it's not as efficient. At most, I would expect 25 miles from a good belt drive setup with this battery. That 5 mile difference is more likely a result of rider weight in this case, rather than efficiencies.
```

---
## \#163 Posted by: chaka Posted at: 2017-10-10T15:33:32.281Z Reads: 111

```
No, I am talking about a motor unattached and spinning free at WOT. I don't know how I could have made that more clear.
```

---
## \#164 Posted by: evoheyax Posted at: 2017-10-10T15:48:21.505Z Reads: 111

```
You said it sounds like 4 should better in theory, but not in the real world. Putting them on a board and riding is real world. Spinning them on the bench is not real world. The currents are low, and don't simulate what happens when they are ridden.
```

---
## \#165 Posted by: psychotiller Posted at: 2017-10-10T15:55:06.803Z Reads: 111

```
[quote="chaka, post:148, topic:35056"]
The 5065 motors we sell consume about 45 watts unattached and free spinning. If I use 4 of them my free spinning consumption would be 180 watts! Thats with the wheel unattached.

Our 6085  motors consume about 70 watts, a quad with these will consume 300 watt! And this is just the power it take to keep the motor spinning at WOT.

These figures were taken while at 44.4v
[/quote]

@evoheyax  What I get from this, is there is no way the motors will draw less when placed on the ground and weighted...And when Chaka say's unattached, he means no wheels or belts, which is as direct a comparison to hubs as we can get.
```

---
## \#166 Posted by: evoheyax Posted at: 2017-10-10T16:10:17.254Z Reads: 104

```
Well can you explain my real world range numbers?

Cause I'm not really behind belt drives in range anymore...

If it really used more power, how come I'm not seeing this in the real world?
```

---
## \#167 Posted by: Hummie Posted at: 2017-10-10T16:13:09.387Z Reads: 110

```
All the inefficiencies in a motor can be categorized.  Running MOTors wot the current draw reveals the iron losses.  A bigger motor has more and less copper losses.  A bigger motor will therefore generate heat more from high rpm than load. Only other losses are air friction and bearings. The thought that more small MOTors will have more iron losses than one big motor...I doubt it but still greater losses and higher no-load would likely happen from the increase in bearings and their friction.  Less thick grease in bearings would bring it down 
Actually the iron losses can go up when stators are magnetically saturated with a very large load and then they don't switch polarity as easily. But otherwise they stay the same and are just rpm dependent
```

---
## \#168 Posted by: chaka Posted at: 2017-10-10T16:32:23.575Z Reads: 110

```
Using your figures it looks like you are using about 17 watthours per mile. This is what I would call moderate to heavy usage and is what we see in a belt drive belt for moderate speeds around 30-40 mph. My board is geared to hit the low 40's and I use close to 20 watthours per mile but this is with "full throttle all the time" riding on highways. The high usage is due to the tall gearing in those drives. We see much better numbers from single drives with lots of reduction, geared to max out around 22-25 mph.
```

---
## \#169 Posted by: evoheyax Posted at: 2017-10-10T16:40:54.946Z Reads: 112

```
Well now we're comparing apples to oranges again...

If I wind a hub to 20 mph top speed, yea I'll be better off than having hubs with a max speed of 30 mph.

I will give you real world numbers when I ride home later today of what my actual WH per mile is. it used to be 7 wh per motor, so 28 wh total. Given, that's harsh riding in a hilly environment with a 200 lb guy. I expect the numbers will be around 4 wh per mile now per motor, or 16 ish total. If I were to be really kind, I bet I could get that a bit lower.
```

---
## \#170 Posted by: chaka Posted at: 2017-10-10T16:47:08.700Z Reads: 113

```
I used @Ackmaniac 's app and left my board on for several weeks to get my average usage. Best to get a large data set when we talk about these numbers. You should go ahead and wind a motor to max out at 22-25mph and see what happens, get back to us when you do. Not enough results from testing hubs can be found so keep it coming!
```

---
## \#171 Posted by: longhairedboy Posted at: 2017-10-10T17:27:01.654Z Reads: 111

```
@evoheyax so somehow adding more holes to the bucket gives us fewer leaks?  

I have built no less than 5 distinct all wheel drive boards and i have to say that by the time the tweaking is done to allow the use of four power plants on the same pack i had two on, not even the brakes improve that much. Acceleration does not improve. I'm still throwing the same watts on the street, but now throwing more current back into the pack while braking, making it an even more precarious balance of settings. 

In order to take advantage of the full power of four wheel drive over a two wheel drive you need twice the cells and twice the power bandwidth in the copper, and twice the BMS.
```

---
## \#172 Posted by: psychotiller Posted at: 2017-10-10T17:30:17.094Z Reads: 106

```
[quote="longhairedboy, post:171, topic:35056"]
so somehow adding more holes to the bucket gives us fewer leaks?
[/quote]

Yes, the leaks are all smaller right? Am I right?! Am I right?! In your Face!!!
```

---
## \#173 Posted by: longhairedboy Posted at: 2017-10-10T17:32:55.574Z Reads: 102

```
i'm going to go home tonight and dedicate myself to science by seeing if more beers results in less piss.
```

---
## \#174 Posted by: psychotiller Posted at: 2017-10-10T17:35:45.239Z Reads: 104

```
12 beers one person? Or 12 beers 4 people?
```

---
## \#175 Posted by: Hummie Posted at: 2017-10-10T17:50:58.493Z Reads: 106

```
Leaks= winding resistance.  Adding MOTors that are all .06ohms, they aren't in series or parallel but separate circuits. U still have .06ohm resistance regardless of how many motors.    More so the advantage w multiple motors I think would be how current creates heat w a square relationship ..and now all MOTors have a forth of that current.   That's what I think this hour .
```

---
## \#176 Posted by: longhairedboy Posted at: 2017-10-10T17:51:00.967Z Reads: 106

```
See, it doesn't even hold up here. I person can more efficiently pass more beer through one body resulting in more piss than four clones could due to losses from pirspiration and metabolic inefficiencies. 

To be clear, i'm saying if i drank 12 beers i would piss more than if four of me each drank 3.
```

---
## \#177 Posted by: longhairedboy Posted at: 2017-10-10T17:52:20.289Z Reads: 106

```
and then you have mechanical resistance. on belts its more, but on hubs you still have bearings, even though by comparison its almost none. That gets multiplied by four as well.
```

---
## \#178 Posted by: evoheyax Posted at: 2017-10-10T17:52:41.060Z Reads: 109

```
[quote="longhairedboy, post:171, topic:35056"]
I have built no less than 5 distinct all wheel drive boards
[/quote]

Were any of these boards hub motor boards first of all?

Second of all, what your saying makes no sense.

If I have 2x 4.12 vescs, I'm limited to 260 motor amps, due to the 4.12 vescs' 130 amp limit.

Now, if I have 4x 4.12 vescs, I'm limited to 520 motor amps, double to power potential.

Now, you might not be hitting that limit with 2wd and belts, so for you, this is a non issue.

But I'm telling you, If I turn 2 of my vesc's off right now, I will not get as good of an acceleration or braking. I simply can do more than what the limits of the controllers are.

Now with the focbox and vesc 6, you might hit this bottle neck and thus, not have as much of an issue. You probably can beat a 4wd with a single, huge belt drive motor. But man, good luck controlling that jerk of having one motor accelerate like that. With the motors most are using, the jerk is minimal, but if you want to match the power 4 of these hubs have, your going to need a huge motor for your belt drive. These also better control.

Maybe we just have to realize that at the end of the day, hubs and belts are just different systems. Maybe 4wd with belts are not going to give you much benefit (besides you'll get closer to the no load speed), but with hubs, more motors = more torque.
```

---
## \#179 Posted by: Cobber Posted at: 2017-10-10T18:03:57.004Z Reads: 104

```
[quote="psychotiller, post:174, topic:35056, full:true"]
12 beers one person? Or 12 beers 4 people?
[/quote]

12/4=3 beers, I won't even break the seal...
is that 100% efficiency?

If I drink three beers while riding my board will I go further?
all this beer talk is making me thirsty
```

---
## \#180 Posted by: Hummie Posted at: 2017-10-10T18:06:33.447Z Reads: 106

```
I don't think beers is a good analogy as the piss produced is equal to beers drank but if u drank ...something that expanded based on its total volume similarly to how the main copper losses in the motor occur, and that liquid were to expand w a square relationship...then the four clones drinking a beer each would piss two beers each but if u drank all four beers ud piss like 16 beers.
If they all drank 2 beers then they'd piss 16 beers worth of liquid and if u drank all 8 beers ud piss 56 beers worth
```

---
## \#181 Posted by: psychotiller Posted at: 2017-10-10T18:18:27.994Z Reads: 103

```
Hahaha @mccloed ?
```

---
## \#182 Posted by: longhairedboy Posted at: 2017-10-10T18:23:49.821Z Reads: 101

```
[quote="Cobber, post:179, topic:35056"]
If I drink three beers while riding my board will I go further?
[/quote]

The community demands answers. I shall give them these answers.
```

---
## \#183 Posted by: mccloed Posted at: 2017-10-10T18:26:03.904Z Reads: 100

```
I know about beer, not hub motors. :rolling_eyes:
```

---
## \#184 Posted by: JohnnyMeduse Posted at: 2017-10-10T18:26:21.132Z Reads: 105

```
[quote="psychotiller, post:174, topic:35056, full:true"]
12 beers one person? Or 12 beers 4 people?
[/quote]

What kind of question is that... We all know the answer you need 12 Beer per person to build a 4wdr... because if you give 12 to 4 people they will argue over none sens for the next decade 😜
```

---
## \#185 Posted by: Hummie Posted at: 2017-10-10T18:36:03.320Z Reads: 106

```
4 beers each for four clones is 16 beers worth of piss. The original drinking all 16 beers is ..256 beers of piss.  Who's gunna prove me wrong. ? This would apply to pulley or hub beers
```

---
## \#186 Posted by: L3chef Posted at: 2017-10-10T18:37:43.972Z Reads: 105

```
Hold on. I'm only on my second. I'll pm you when I'm done
```

---
## \#187 Posted by: BigBoyToys Posted at: 2017-10-10T18:37:52.019Z Reads: 107

```
Ive built 4wd board with 4 different types of hub motors and  three different 12S batteries from 3P to 6P. My experience with them is not inline with yours. On my 1st 2wd hub board was 12S3P with 130KV hubs, Low speed acceleration was rather poor but the board would still pull 38mph. I then added two more of the same hubs to make it 4wd and divided all battery max and regen settings in half but left the motor min and max the same per motor. Acceleration and braking (especially from low to moderate speeds) were drastically improved with the same 50A total battery Max and Min because the motor max and min total added up to double. 

I did see a loss of range from about 12 to 10 miles on a 7.5Ah pack but I attribute this to the increased rolling reaistance of the front hubs compared to the clones that were on the front in the 2wd configuration. 

I do agree that you need a larger battery to take FULL advantage of 4 motors but there are definite power advantages even with the same battery .The same would hold true for a belt drive.
```

---
## \#188 Posted by: Hummie Posted at: 2017-10-10T18:43:41.031Z Reads: 104

```
Motor amps are a true amount of amps circulating in the motor.  U get increased low speed power and the same losses based on whatever amps, motor or, and, battery, in the motor.
High motor amps since they occur at lowest speeds especially cause losses beyond the standard i2r
```

---
## \#189 Posted by: evoheyax Posted at: 2017-10-10T18:46:16.022Z Reads: 103

```
[quote="BigBoyToys, post:187, topic:35056"]
I do agree that you need a larger battery to take FULL advantage of 4 motors
[/quote]


Not if your using zippy lipos! I can put out almost 300 amps con from them, so more than enough juice :P
```

---
## \#190 Posted by: Cobber Posted at: 2017-10-10T18:48:16.820Z Reads: 104

```
[quote="evoheyax, post:189, topic:35056"]
Not if your using zippy lipos! I can put out almost 300 amps con from them
[/quote]

you can prob. half a zippy C rating...
just saying, it's not a tattu...
```

---
## \#191 Posted by: BigBoyToys Posted at: 2017-10-10T18:50:42.160Z Reads: 104

```
[quote="evoheyax, post:178, topic:35056"]
You probably can beat a 4wd with a single, huge belt drive motor.
[/quote]

The total amount of torque my 4wd board puts out would snap a single belt or bend pretty much any of the belt motor mounts Ive seen. I dont see this happening with a single FOC box, VESC 6 or other, but if anyone with a big single running a VESC wants to try there luck, performance day is only 1 month away 😉
```

---
## \#192 Posted by: BigBoyToys Posted at: 2017-10-10T18:52:50.665Z Reads: 108

```
@Cobber  But as far as braking goes, lipos should still be charged at 1C so with out double battery high speed braking cant be doubled.
```

---
## \#193 Posted by: Hummie Posted at: 2017-10-10T19:00:53.080Z Reads: 104

```
I've seen lipo and other chem that can be charged at a much higher rate.  Also seen evidence the charge rate doesn't effect cell cycles as much as max voltage charged
```

---
## \#194 Posted by: BigBoyToys Posted at: 2017-10-10T19:09:53.605Z Reads: 106

```
Agreed, but if whatever battery you were using with the 2wd was already maxed out for batt max and regen (1C or higher if you're comfortable with that) then youd need more battery to increase the limits and take full advantage of the extra hubs.

Extra total motor amps is a huge advantage for 4wd on vescs, but extra battery amps in addition to the motor amps would be taking full advantage imo.
```

---
## \#195 Posted by: longhairedboy Posted at: 2017-10-10T20:00:14.093Z Reads: 111

```
so... your two hubs were weak at launch and you added two more and finally got up to what your pack could actually put out. YEah that makes sense. And it cost four times as much as a 38mph RWD belt system that would have just torn off the mark to begin with. 

i get the math, and i get what happens on the street. 

No matter how i look at it, i can't justify 4wd in 99.9% of cases that don't involve overcoming wind resistance on the top end. 

Obviously my outlook is biased toward belt drives. I only just recently got to ride a raptor 2. I was pleasantly surprised that it almost kept up with my belt drives off the mark. I don't hate hubs or 4wd, they just don't deliver what i need yet. What i need is options and configurability. They have neither of those things, and the only pro is literally ease of build. The industry is driving hubs because they're cheaper to build boards with. I have never done things the easy way or the cheap way so benefits like that are easily dismissed by me. Up until about three months ago, i wasn't even THINKING about hubs. Direct drives, sure. Gear drives, yeah. Even planetary geared hubs would be a vast improvement provided the ratios could be adjusted easily. But thane on a can? 

i'm waiting for somebody to get it right (for me) still. So far, i see a lot of awesomeness but its still not right for me.
```

---
## \#196 Posted by: BigBoyToys Posted at: 2017-10-10T21:00:48.677Z Reads: 110

```
[quote="longhairedboy, post:195, topic:35056"]
your two hubs were weak at launch and you added two more and finally got up to what your pack could actually put out.
[/quote]

Yes by my 280lb standards startup was weak with two 90mm wheel (6355) 130kv hubs. It had way more than enough for my 130lb friend though. 

[quote="longhairedboy, post:195, topic:35056"]
And it cost four times as much as a 38mph RWD belt system that would have just torn off the mark to begin with.
[/quote]

It cost  me under 2k to build my 1st 4wd, which is comparable to the price you sell your builds for, but has double the motor amps a two vesc build can supply. You also said later in your post that hubs are cheaper to build with (obviously refering to 2wd hubs), which would imply that its not 4x the cost of a 2wd belt drive set up. The cost of wheels, bearings, trucks, pulleys and belts are also required for belt drive set ups but two pairs of hub motors have those parts included or are not required.

A dual belt drive with the same sized stators and a total of 50A battery and 260A motor is not going to tear off the line by my standards either unless its geared to much less than 38mph. The Raptor 2 I tested was impressive for a premade board but just moderate by my acceleration standards and was minor league compared to my 4wd hub boards acceleration from a dig all the way up, especially considering the raptor 2 tops out at 30 mph where as mine hits 40 mph.

Otherwise I agree with the rest of your post. I am also waiting for someone to get it right 🤞😉. And it doesnt make sense for most to go 4wd.
```

---
## \#197 Posted by: evoheyax Posted at: 2017-10-10T22:01:11.493Z Reads: 120

```
Where s the info on this performance day? I need to come out, where ever it is...
```

---
## \#198 Posted by: BigBoyToys Posted at: 2017-10-10T22:12:10.125Z Reads: 121

```
<img src="/uploads/db1493/original/3X/d/6/d62728e142af87af1e1bb29661171c523c4b8ba2.jpg" width="666" height="500">

YES! Maybe we should match settings on our 4wd boards to get some hub comparisons!
```

---
## \#199 Posted by: BigBoyToys Posted at: 2017-10-10T22:50:09.210Z Reads: 120

```
Breaking news, Enertion  might have something up their sleeve for performane day as well!

<img src="/uploads/db1493/original/3X/b/0/b0629a059ba73ce7bec3ffc630c4746a7be33697.jpg" width="641" height="500">
```

---
## \#200 Posted by: JohnnyMeduse Posted at: 2017-10-10T23:01:23.788Z Reads: 116

```
Nha Unless @onloop joint the party... I'm only one guy with is Raptor... If I can bring it, because of plane and restriction and the pain in the ass of sending a battery.
```

---
## \#201 Posted by: NummThumz Posted at: 2017-10-10T23:03:47.027Z Reads: 112

```
I'm still waiting on mine and I am local...but unless there is a miracle in the production timeline, I don't see it happening. If I do get it in time, happy to share so that you can ride a familiar board.
```

---
## \#202 Posted by: BigBoyToys Posted at: 2017-10-10T23:08:28.646Z Reads: 119

```
Im sure any of is local guys mynself included would host your board until your arrival if you wanted to ship it here via ground before the event.
```

---
## \#203 Posted by: lowGuido Posted at: 2017-10-10T23:10:36.189Z Reads: 118

```
OMG what the hell have I missed here?
```

---
## \#204 Posted by: JohnnyMeduse Posted at: 2017-10-10T23:12:31.261Z Reads: 123

```
Too Much.... My best advice will be to go back to sleep 😀
```

---
## \#205 Posted by: evoheyax Posted at: 2017-10-10T23:15:17.392Z Reads: 126

```
To find which hubs have more torque?

It's tough to compare boards when we all weigh different weights. But I really wana race whatever you've got up your sleeve. I could always crank my settings way high, haha. But they are nice as is right now.

I'll try to figure out if I can attend or not. Hope so, should be able to drive down. Says 7 hours, 403 miles... I've driven to LA before, and I love rode trips. Just depends were my school is at the time and if I can find a place to stay for Friday and Saturday night.
```

---
## \#206 Posted by: evoheyax Posted at: 2017-10-10T23:17:59.773Z Reads: 124

```
[quote="lowGuido, post:203, topic:35056, full:true"]
OMG what the hell have I missed here?
[/quote]

We started with why small hubs have issue, which turned into why belts are more efficient then hubs, which turned into a debate about whether 4wd is less efficient than 2wd, which turned into lets do more tests and show real world data, which is where we are now.
```

---
## \#207 Posted by: BigBoyToys Posted at: 2017-10-10T23:21:29.096Z Reads: 115

```
Excellent summary lol!
```

---
## \#208 Posted by: BigBoyToys Posted at: 2017-10-10T23:34:30.159Z Reads: 116

```
At 280lbs I have big sleeves, you sure you wanna see what I got hiding? Hahaha. 

If some other people are coming in from out of town too it might be worth pitching in for an AirBNB.
```

---
## \#209 Posted by: Cobber Posted at: 2017-10-11T01:05:34.662Z Reads: 130

```
[quote="BigBoyToys, post:192, topic:35056"]
But as far as braking goes, lipos should still be charged at 1C so with out double battery high speed braking cant be doubled.
[/quote]

_**CHURCH**_*

*depending, there is always a but... but the rule of thumb unless you have _tech_ is 1C
```

---
## \#210 Posted by: evoheyax Posted at: 2017-10-11T04:30:41.346Z Reads: 129

```
[quote="Cobber, post:209, topic:35056"]
but the rule of thumb unless you have tech is 1C
[/quote]

Oh I've got tech... Lots of tech. The best tech. No one has better tech than me. Who wants some tech? lol
```

---
## \#211 Posted by: lowGuido Posted at: 2017-10-11T06:16:12.512Z Reads: 135

```
Well the answer is most definitely that there are too many variables. 

I guarantee that with the same motors and the same rider 4 motors is less efficient than 2.
But with 4 efficient motors vs 2 inefficient motors.. who knows?
Belts vs hubs? 
Yeah again.. the only way to prove it is to get out and ride. From my experience I think the dragless costing ability of hubs would put them into the high efficiency zone.
I know that I have done a really long ride on a dual hub board and simmilar rides on belt drive and not made it as far.. but then wheel compound comes i to it too.  Softer rubber wont be as efficient as hard thane.
There are pros and cons of every setup..
```

---
## \#212 Posted by: Hummie Posted at: 2017-10-11T07:43:42.929Z Reads: 134

```
if you have a bigger motor you are more efficient.  more motors is the same as a bigger motor.  
motor inefficiencies worth mentioning are copper or iron losses

starting at the dragstrip with 50volts:
  if you have one giant motors with .02ohms resistance doing 100 amps the copper losses in the windings,decided by I2R are 200 watts.  100x100x.02 equals 200 so 200 watts wasted...and since the total elctrical input with 50v and 100a would be 5000watts, the major loss in the motor under heavy load, copper, is 200 watts and it's ...95percent efficiency.  
if you have 4 separate quarter sized motors then each will have probably .08ohm resistance, and the 100 amps will be devided between them, so 25 amps each.  current squared times resistance...  25x25x.08 is 50 watts loss to copper losses.  times that by 4 for the four motors and it's the same 200 watts and 95 percent efficiency.  


maybe the math is off but the idea I think is right. 
soon will see.
```

---
## \#213 Posted by: guyguy Posted at: 2017-10-11T14:28:49.575Z Reads: 131

```
[quote="evoheyax, post:22, topic:35056"]
But reduce that by a 2:1, and you'd expect the same results as a 85 kv motor, right? Well, it's not really that simple. I don't understand it all myself when it comes to belt and pulley systems.
[/quote]

I hate to wade into this conversation, since I'm just another non-engineer with an opinion but I'm gonna do it anyway-- lol. From what I've read KV doesn't change torque. Copper mass changes torque at the motor and gearing changes torque at the wheel. The more copper mass you have the more torque the _motor_ can produce. The more gearing you have the more torque the _at the wheel_ you can produce or you can look at this as the motor needing to produce less torque required for a scenario -- effectively you're exchanging RPM for torque. People here keep conflating torque output at the motor with torque at the wheel which makes it especially confusing to then talk about efficiency because only motor torque matters when we're talking about motor efficiency. If what Vedder is saying is true, that these electric motors are most efficient at low torque and high rpm (but not exceeding 60 k erpm) then lowering the torque needed _at the motor_ is the the most efficient way to run the motors because the motors simply need to produce less torque when ramping up to an efficient RPM, or in other words, gearing allows you to exchange RPM for torque because the wheel needs high torque lower RPM and the motor is more efficient at lower torque higher RPM. For a rider of the same weight and style looking to achieve a certain level of performance, the only way to lower the amount of torque needed _at the motor shaft_ is through mechanical advantage. Increasing the motor size don't reduce the amount of torque needed at the motor, it just produces more torque at the motor, which I guess is  becoming more efficient because you spend less time in high torque low rpm and they're better suited for higher torque scenarios than small motors.

I'm getting this from: http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#214 Posted by: evoheyax Posted at: 2017-10-11T15:30:26.823Z Reads: 132

```
There's 2 big factors that effect torque, which is the amount of copper and actually, the size of the stator. The iron in the stator places an important role in the whole thing. Just increasing the stator size while leaving copper amount the same will increase torque. A smaller factor is magnet size. Bigger magnets can create stronger magnetic fields, can being the key word. This does depend on copper and stator size too, and theirs a point where more magnet in a small motor will do nothing more for it.

kv just tells you how many amps you'll need to get the same amount of torque, higher kv, more amps needed to get the same torque (assuming no gearing). This means more heat, most importantly at the speed controller level. With smaller motors that are inefficient, this will make them worse. With larger motors, not necessarily. The carvon v2's/v2.5 are actually a similar stator size to our motors now (wider and shorter instead of thin and longer). Longer means bigger magnets, which should help with torque to some degree too. The v2's though, at 149 kv,, did not get really hot at all. But they would overheat 2x 4.12 vescs in under 2 miles, even with heatsinks... The range was also horrible for the same reason. As it is now with hummies new motors, my vescs seem not go above 120 F, way below their limit. So not an issue anymore, though I have my amp limits very high.
```

---
## \#215 Posted by: Vanarian Posted at: 2017-10-12T21:35:54.850Z Reads: 129

```
Can't say it better. Took me time to finally understand the "torque per amp" instead of "torque" thing...

BTW which seller can you recommend to get 20AWG insulated high heat copper wire ? I wanna upgrade my windings. Opened my motors and was like "Damn it is 29AWG or what ???" The real question is : how can I be sure that I'm keeping the same kv ? Should I count number of turns and make it the same ?

Once I'm done I'll do the redneck way : add more magnets like I'd add cubic inches inside a small block V8 !

EDIT : I got an APS 3300W motor to be delivered. I'll check the wire diameter since I'll hack through it.
```

---
## \#216 Posted by: evoheyax Posted at: 2017-10-16T17:17:56.268Z Reads: 126

```
I use Remington Industries 20 awg high heat wire. Great stuff, and works well.

To figure out how many turns you want, the best is if you can count it while unwinding.
```

---
## \#217 Posted by: Hummie Posted at: 2017-10-16T21:05:12.895Z Reads: 126

```
if you have an inductance meter, or that feature on a good multimeter, you can see what the inductance is per phase and that's a lot easier than trying to count the windings that are on there already especially because it's likely a multistrand winding and maybe 4 thin wires doing all the same amount of turns.  find what the inductance is and you can replicate it as you put the new on.  be prepared to spend many hours removing and winding.
```

---
## \#218 Posted by: Vanarian Posted at: 2017-10-17T12:36:11.636Z Reads: 125

```
Thank you for the tips.

Another question : can I bind strongly around the stator or I risk damaging the iron? BTW I have to look how the 3 wires go all around (beats my common sense)

I'm thinking of crafting a tool with the 3d printer to make the turns less difficult (make walls between phases) and pack it tight.
```

---
## \#219 Posted by: Hummie Posted at: 2017-10-17T14:53:33.707Z Reads: 123

```
A tool made on the printer I'd be interested to see.  So far the best tool I have beyond bamboo skewers is the hole cover on either end that holds the wires from blocking the shaft hole ehen putting it together after winding. Done that too many times. 
U won't damage the stator winding.  U could damage the insulation on the wire but if the stator is well insulated its unlikely you'll scratch the wire. The danger is a bare corner on the stator that scratches the insulation on the wire and then u short through the stator.

 lve been doing tons of the dlrk winding and terminated wye.  A classic u can find a guide for

The biggest reason I don't like putting these MOTors together and am hoping to slow peoples roll till the new show is theres 1.5mm less room for the end turns to fit. Everything must be perfect and adding the leads is surgery<img src="/uploads/db1493/original/3X/5/b/5b706e50746a03547a7026531e8eebebece30bb9.jpg" width="666" height="500">  hadn't anticipated getting as much copper on
had to put the "transits"( wires going between teeth you can see in the photo, on the other side of the motor) to make it fit.  but these just sit here and I'm not going to put them in the oven or waste magnets on these.  we're all going for the better big gamble with the new design. god forbid it has a problem I'll send the 15 of these I have to people I owe.   we will see.  I'm drinking beer waiting till this coming week.  I hear from @evoheyax that the tire's core are a bit subacceptable and  gunna get an aluminum done for sure.  thanks  and @ralphy for saying it and showing it I think you're right and don't want to mess with the pu core..  a relief really.  ill get those designed and ordered.  aluminum is of course the best, and the huge contact area for the urethane to adhere, that much shows true.  but I don't even ride with this and that and wait for the new and it's just @evoheyax and I translate to the custys
```

---
## \#220 Posted by: ralphy Posted at: 2017-11-11T15:15:17.962Z Reads: 102

```
Your welcome man. Keep at it and im happy to share what i have learned to make this sport safer and more reliable. Once you get everything worked out id like to get a pair myself.
```

---
## \#221 Posted by: Hummie Posted at: 2017-11-11T16:38:27.263Z Reads: 100

```
did an about face and long strand glass filled pu can be way stronger than aluminum and have been doing that.  the environment is a bit abrasive and the material needs to be tough for that but mostly the obstacle is getting a high enough tensile strength.
```

---
