# Uneven Dual Rear Drive

### Replies: 94 Views: 11615

## \#1 Posted by: lowGuido Posted at: 2015-08-18T03:05:00.408Z Reads: 770

```
I was posting in another thread and It made me think of an Uneven drive board I built recently.
the build was a total accident, I was making a DR for a friend with parts he provided and he accidentally bought 2 motors of different size.
so I have by total accident probably pioneered the dual uneven drive board.
I figure no one else has probably been stupid enough to try this, but I was actually really interested to see how it turned out.
so I had one motor which was around 200kv and one with about 400kv 
would it work?
would it explode?

Or,
would it work like some sort of sequential twin turbo system where the torque from the 200kv would assist getting the board off the line and up to the top where the 400kv would take over and boost the top speed?

well turns out it was the twin turbo option. who knew? 
seriously, the low down is taken care of by the extra torque of the 200 and the 400 kicks in and boosts acceleration and top speed! 

each motor is powered from its own individual ESC so the loads on each motor are different but shared slightly, handled by different electronics so there is no real feedback or connection from one motor to the other.
So what happens when the 200kv motor exceeds its theoretical RPM limit? 

think of it this way: whats your theoretical top speed? 
mine is about 35km/h but we have bombed hills right? i have had my board up to ~38km/h-40km/h which is already exceeding the max RPM of my motor. 
So you could say its just the same as going down a hill, the load on the 200 will be reduced.

how long will it last? will things blow up?

Dunno. I'll keep you posted.
```

---
## \#2 Posted by: sl33py Posted at: 2015-08-18T03:44:00.609Z Reads: 695

```
Wow - sounds like a fun thing to test with full protective gear!

What voltage are you using for them?  My first dual motor (5065 200kv on 8s) did 30mph with a tailwind.  Would do 25mph easily the rest of the time.  I actually didn't realize how fast i was going (first run in the neighborhood the night i got it finished), and typically moderate the speed a little better now.  I try to gear mine so that it's top speed is around 22-25 max.  Keeps me out of trouble that way.

As for the motors i'm surprised it works well and wonder if the gearing works out to be limited by the fast or slow motor?  What gearing, wheel size and voltages?  I'll calculate both and see which one it seems to be limited to.

Cool and keep us posted!
```

---
## \#3 Posted by: lowGuido Posted at: 2015-08-18T03:56:49.664Z Reads: 668

```
I have done the maths, the theoretical top speed of the 200kv with 2.5:1 gear on 70mm wheels is 35km/h and the theoretical top of the 400kv with same ratio and wheels is 54km/h.
I say theoretical because I have never ridden it to the top speed, I run out of balls at upwards of 40km/h

oh im only using a 6S battery.
```

---
## \#4 Posted by: cmatson Posted at: 2015-08-18T13:52:15.312Z Reads: 643

```
thought it was doomed when I read the title, but as I look at what you are saying, it actually seems pretty sweet!

I think if done right, this will be super sweet, but consider some of the following:
you would need some way to switch to the second motor after picking up speed- you could possibly use the second channel on your rc remote (the steering wheel) to do the switching between motors- I don't know how you'd actually get it to switch though... the only thing I can think of is a servo on a switch which changes which esc goes to the throttle pins on the receiver. I just wouldn't connect both esc's to the throttle at the same time... it seems like a recipe for disaster. also, I think the 200kv motor will be fine exceeding its RPM limit so long as it's not powered when it exceeds it... if its just freely spinning because the other motor has taken over at that point, I don't see any reason for it to just blow up.

in all, I think it will work as long as you don't have both spinning at the same time, because they will want to go different speeds.
```

---
## \#5 Posted by: sl33py Posted at: 2015-08-18T16:21:03.408Z Reads: 627

```
@cmatson - he's running dual now w/ different kv.  Seems to work without toggling power to either.  Kind of amazing it works really!

lowGuido - cool!  I wanted to compare setups with the calculator i have, but it needs motor gear # teeth, and wheel # teeth.  

Looking at typical gearing around 2.5:1 - 16/40 = 25kph @ 200kv, 50kph @ 400kv (simple math at least).  I guess i'm close to your actual gearing.  

Honestly i never thought i was going all that fast, but in hindsight 30mph was pretty foolish.
If you ever want to use a good gps app for this, i really like strava for miles ridden, avg mph/kph, elevation gain, and top speed.
[img]/uploads/db1493/original/1X/30140cdaa46b317ecfb10bd76d3573bcbd8b7158.png[/img] Top speed run just after building dual rear setup (5065 200kv on 8s).  
[img]/uploads/db1493/original/1X/91975ab9ceb05402c35aefd2832a98f8ba243160.png[/img] Date night cruise on Alki w/ GF.  Wanted to see max distance on 8s 8Ah setup.

Show us pics of your setup?  Stay safe!
```

---
## \#6 Posted by: longhairedboy Posted at: 2015-08-18T18:13:50.781Z Reads: 558

```
This is a amazing. I never would have even thought about a hybrid kv system like this, but it makes total sense. 

I think you'll be just fine without actively switching between motors. In fact i kind of wonder what kind of performance I would have if i took one of my 270's and replaced it with one of my binned 245's. 

Have you noticed any sort of torque steering issues? 200 to 400 is a pretty big gap.
```

---
## \#7 Posted by: lowGuido Posted at: 2015-08-18T23:16:25.714Z Reads: 555

```
yeah, there is no active switching, as i said, once the RPM ceiling is exceeded the lower kv motor just has less load and acts in the same way it would as if you are going down hill. 
All the electronics are separate anyway.
I'm with most of you guys, I wouldn't have thought it would work either, but I guess that's why I tried it.
I'm also not saying this is a perfect system and that I have all the answers, cause I don't. i'm just relaying my findings with you guys to perhaps open new avenues.

and there is no torque steering issues. look at a single wheel drive board, they the the most differential possible, all and none, and yet they don't have any major torque steer problems.
in fact you are probably best to look at it as two separate 1 wheel drives on the same board.
```

---
## \#8 Posted by: torqueboards Posted at: 2015-08-19T05:43:42.785Z Reads: 539

```
Are you sure that would work? I highly doubt it.

Your slowest RPM is your maximum RPM in this scenario.

There's nothing that would make your RPM faster if it has resistance from the specific gearing of your slowest motor.

It would work if you removed the belt off the slowest RPM wheel but if you have the belt on the slowest option it will max out at the slowest RPM.

Your single motor would work even harder trying to pull a second pulley and the second motor is tapped out.
```

---
## \#9 Posted by: longhairedboy Posted at: 2015-08-19T13:36:28.479Z Reads: 516

```
This would work better if the rear pulleys were on ratchets (like the rear sprocket on a bike) and you had a nice brakeboard truck on the front. You would lose regen braking though.
```

---
## \#10 Posted by: lowGuido Posted at: 2015-08-30T06:35:56.974Z Reads: 515

```
well I tried a top speed run today on the UDR drive.
Results were pretty good.

so I took my board with a single motor down the road and peaked the speed at 30 as a control run.
then I took the UDR board down the same road and it was noticeably faster. however I only made it to 37 before I got a bit of a wobble up and slammed. not too hard fortunately, but I could feel that there was more in it.
I might have to try it again another day when I get the balls to give it another shot LOL.

one thing is for sure.. its fast enough.
```

---
## \#11 Posted by: longhairedboy Posted at: 2015-08-31T19:13:38.100Z Reads: 490

```
30 kph or 30 mph? Mine tops out at around 31mph and man that's scary. lol
```

---
## \#12 Posted by: lowGuido Posted at: 2015-09-01T00:54:52.960Z Reads: 484

```
30km/h.
don't get me wrong, I have had it up to 40km/h but on this particular road on this particular day I peaked at 30km/h
may have had a slight incline or my 40km/h run had a slight decline, or perhaps a bit of both.
but for the purpose of back to back testing, the peak of that board on that day was 30km/h.

also worth noting is that my single that I was testing against is a sturdy board with a kick tail that I'm very much used to riding. the UDR board is a flexy bamboo board with no kick tail and just slightly different physics that make it a little uncomfortable for me to ride hence why I slamed towards the top end.

bottom line is that the UDR really easily pulled an extra 7km/h with more in the tank before I slammed. that's quite a substantial difference when you break it down.
```

---
## \#13 Posted by: longhairedboy Posted at: 2015-09-01T12:26:13.032Z Reads: 474

```
I love this forum. There is some crazy stuff happening here.
```

---
## \#14 Posted by: onloop Posted at: 2015-09-03T00:23:12.263Z Reads: 485

```
we want pictures of this setup!
```

---
## \#15 Posted by: lowGuido Posted at: 2015-09-03T09:27:05.465Z Reads: 496

```
Its not the greatest photo. But heres one that i have handy.
<img src="/uploads/db1493/original/1X/472095ee40751e95bfafcac550f9d474422a029e.png" width="503" height="500">
```

---
## \#16 Posted by: lowGuido Posted at: 2016-01-06T21:15:53.658Z Reads: 491

```
I just took this science experiment for another blast this morning.  God dam its fast. It definitely accelerates harder than even motors.
<img src="/uploads/db1493/original/2X/a/a2265fe4d754416d2cff90aa7fa23b00ade2533c.jpg" width="281" height="500">
Until such time  as I man up and do some damn science on this beast it will have to reside in the pile.
<img src="/uploads/db1493/original/2X/b/bae9cb349f4e16cd7fd2555a5793e08a72873b75.jpg" width="690" height="388">
```

---
## \#17 Posted by: sk8ace Posted at: 2016-01-06T21:47:29.717Z Reads: 475

```
Nice! I'll be running a dual diagonal setup(if I can fix my first vesc) with different motors. Rear will be Enertions big rspec and front will be a Tacon 160. It will be fun for sure!
```

---
## \#18 Posted by: treenutter Posted at: 2016-01-06T22:19:55.260Z Reads: 473

```
@lowGuido This is so cool! I'll mention something obvious, but not yet noted; this approach might allow dual-rear configs with more motor can options. Maybe you could use different motor can sizes, one large one (63mm) and one smaller one (50mm) without running out of room on your trucks!
```

---
## \#19 Posted by: lowGuido Posted at: 2016-01-07T10:41:21.233Z Reads: 477

```
Nice @sk8ace  a UDD setup as it would be.. interesting to hear how that goes for you.

@treenutter yes the can size is something that has crossed my mine once or twice before.
```

---
## \#20 Posted by: DougM Posted at: 2016-04-20T03:08:23.300Z Reads: 477

```
Ok, so here's my question - what if you put a brushed DC motor on one truck and a BLDC on the other?  Brushed motors have maximum torque at zero RPM, which would give you great take-off power and then as the power on the brushed motor diminishes with increased RPM the BLDC kicks in and pulls you the rest of the way.  

Also you wouldn't have any of the issues with over RPM drag since the brushed is not a "timed" motor.

I might have to try this.

DougM
```

---
## \#21 Posted by: lowGuido Posted at: 2016-04-20T04:25:50.462Z Reads: 449

```
don't BLDC also have max torque at 0 RPM?
```

---
## \#22 Posted by: trbt555 Posted at: 2016-04-20T09:06:56.375Z Reads: 460

```
Yes that is correct:
<img src="/uploads/db1493/original/2X/7/70783bd7d0762d17d2421b34c2364bf41dca2938.jpg" width="550" height="347">
```

---
## \#23 Posted by: DougM Posted at: 2016-04-20T18:49:37.324Z Reads: 447

```
Theoretically, but in reality I have to kick the board to get it going - otherwise it stutters a lot, whereas a brushed motor could give you clean smooth power off the line.

One problem with brushed motors is that the bigger they get the lower the rated RPM, so getting a powerful enough DC that matches RPM range of the BLDC would be tricky.

DougM
```

---
## \#24 Posted by: andrewhannay Posted at: 2016-05-11T13:05:44.391Z Reads: 432

```
Been reading this thread with intrigue, especially as I have a spare motor and ESC laying around. So it sounds like this setup worked quite well considering the weird configuration. I'm happy with the explanation given, but my only question is this:- Would the slower motor create a braking effect as it tries to turn slower?
```

---
## \#25 Posted by: laurnts Posted at: 2016-05-11T13:45:07.721Z Reads: 437

```
No it wont slow down. If you use VESC with current control, the motor always try to spin at maximum rpm all the time. If one motor has higher rpm than the other, the drag effect will occur (not braking).

Ideally uneven drive is similar case to car engine differential if I look at it. If there is less load on one side of the wheels, that wheels will spin faster taking all the current and power (normal differential and not slip differential). What it comes to eboard is that the motor and the batteries will self balance the power distribution.
```

---
## \#26 Posted by: longhairedboy Posted at: 2016-05-11T14:50:03.639Z Reads: 438

```
[quote="laurnts, post:25, topic:113"]
Ideally uneven drive is similar case to car engine differential if I look at it.
[/quote]

It works exactly the same on a regualr dual drive with the same motors. With two ESCs each driving thier own motor, each one will always try to do its best individually. 

I'm not 100% sure how the traction control option in VESC affects this when using dual with the CAN bus. I can't really tell the difference with it enabled or not enabled honestly.
```

---
## \#27 Posted by: Mobutusan Posted at: 2016-06-11T23:38:26.923Z Reads: 428

```
Here is my plan/theory. Use a Tacon 245kv and SK3 260kv motor with slightly different gearing; 17/36 & 16/36, respectively, since I have both of these motors and could fit them both on one truck. Theoretically, I'm expecting it to run similar to a normal dual drive, but I'm not sure if there would be any issues with running this setup. 

Has anyone else tried this type of even uneven setup or have any opinions or comments?

<img src="/uploads/db1493/original/2X/f/f10d7e54213c131c36fe0e6c3b6a34e6691f30b8.jpg" width="690" height="388">

<img src="/uploads/db1493/original/2X/6/6fc6685668cfe73a75b973b11f62ae1e0ba5afcd.png" width="281" height="500">

<img src="/uploads/db1493/original/2X/3/37e69fbce4b55b19bc804850673a5fd9d2f36471.png" width="281" height="500">
```

---
## \#28 Posted by: lowGuido Posted at: 2016-06-11T23:46:45.459Z Reads: 389

```
I don't see any reasons why this wont work.
what ESC's are you planning on using?

I would be interested in the results.. especially with different gearing. 

I encourage this kind of thinking. outside of the box, not just what everyone else tells them to do.
```

---
## \#29 Posted by: claudiofiore88 Posted at: 2016-06-11T23:52:48.898Z Reads: 395

```
I wonder if you could fit a Tacon 160 and Tacon 110 in a dual rear configuration, then you'd have an uneven drive and disguised as a regular old dr drive. Lol
```

---
## \#30 Posted by: lowGuido Posted at: 2016-06-11T23:57:44.027Z Reads: 396

```
well the 2 SK3's that I used in my original setup are so very similar in size that you hardly notice the difference. however you can feel it.
```

---
## \#31 Posted by: Mobutusan Posted at: 2016-06-12T00:32:57.640Z Reads: 402

```
I'm going with torqueboards 6s to start.
```

---
## \#32 Posted by: Arzamenable Posted at: 2016-06-12T00:59:54.978Z Reads: 400

```
This is awesome. Ya'll know what would be sweet mash up of unique ideas? Carvon skates dual drive from a single motor (pictured) x2 using the Stacked KV motor idea in this thread. Credit to carvon for the drive set up, I just like pictures. 
<img src="/uploads/db1493/original/2X/8/8a0c38300d9d1cefcb762c941282fc1aef0eec6a.jpeg" width="284" height="500">
```

---
## \#33 Posted by: Michaelinvegas Posted at: 2016-06-12T01:47:12.242Z Reads: 381

```
Lol who needs to stop?
```

---
## \#34 Posted by: whitepony Posted at: 2016-07-04T17:55:04.022Z Reads: 379

```
not 100% sure whats the point of this. :confused: if you run dual motors anyway, will you really ever need the extra torque of one low kv motor? or would you ever need some mixed topspeed of 2 different kv motors when you could just tailor kv to your max desired speed and go with that? I ran dual rear 63mm with max speed 50kph+ and more torque was the very last thing I needed on that setup. 

in my eyes, you just add an uneven load that will add extra wear on belts and wheels, will add extra load on motors leading to extra loud bldc noise and you probably loose efficiency too. ontop of that, while accelerating from stand still to max kph, the torque will smoothly swap sides on your truck, so youll constantly have to readjust your weight. probably no biggie, but might add some confusion and possible instability.
```

---
## \#35 Posted by: lowGuido Posted at: 2016-07-05T05:21:38.312Z Reads: 363

```
If everyone walked straight in a line no one would dance.
```

---
## \#36 Posted by: Michaelinvegas Posted at: 2016-07-05T05:49:47.064Z Reads: 374

```
[quote="whitepony, post:34, topic:113"]
swap sides on your truck, so youll constantly have to readjust your weight.
[/quote]

Not sure this would be the case...the motors are pushing and pulling the board....your weight will alway set you back a little regardless which has more torque ... I'm def gonna give it a go just need to figure out the right KV spread between the motors to get a flat-ish Torque curve....well maybe not flat-ish but wider range for torque through the throttle range

Edit: definitely not needed at the speeds you are going but def would be awesome to have that extra punch if needed
```

---
## \#37 Posted by: ugothakd Posted at: 2016-07-28T04:30:13.781Z Reads: 344

```
What if you used one motor, and had two gears to switch from? One for torque, and then one for top speed once you reach 15mph? The first gear would guarantee a quick startup then the second would lead you to top speed
```

---
## \#38 Posted by: maxchilton Posted at: 2016-07-28T04:49:27.832Z Reads: 355

```
[quote="lowGuido, post:10, topic:113"]
so I took my board with a single motor down the road and peaked the speed at 30 as a control run.then I took the UDR board down the same road and it was noticeably faster. however I only made it to 37 before I got a bit of a wobble up and slammed. not too hard fortunately, but I could feel that there was more in it.I might have to try it again another day when I get the balls to give it another shot LOL.

one thing is for sure.. its fast enough.
[/quote]

really? you're comparing a two motor set-up to a single motor set-up.   Of course the dual is going to be faster but not because of the "twin turbo" dual kv motors but because you have two motors!  lol! 


[quote="lowGuido, post:12, topic:113"]
bottom line is that the UDR really easily pulled an extra 7km/h with more in the tank before I slammed. that's quite a substantial difference when you break it down.
[/quote]

At low speed, your 400kv motor is adding drag and slowing you down, at high speed your 200kv motor is adding drag and slowing you down.   Two of the same motors working together at the same time is optimal.
```

---
## \#39 Posted by: lowGuido Posted at: 2016-07-28T05:38:52.689Z Reads: 328

```
Mate. A 200kv motor has the same RPM as two 200kv motors.
```

---
## \#40 Posted by: PB1 Posted at: 2016-07-28T12:27:06.235Z Reads: 341

```
Uneven Dual Drive is a very interesting concept. 

However I see one big danger for the controller of the lower Kv motor. Why? 

Once the lower Kv motor goes past it's unloaded top speed RPM it generates a voltage that is potentially far higher than that of the battery. That us such is not so bad. But if this voltage is far above of the voltage of the ESC it will damage the ESC. While there might not be a lot of current flowing, the motor will generate voltage spikes. 

Let's say you have a 200Kv and a 400Kv motor and a 6s battery and an ESC rated for 6s. If you have the same gearing for both motors and the gearing is geared at top speed for your 200Kv motor you will blow your ESC.

So your lower Kv motor needs to have an ESC that can handle the voltage the motor produces, in this case 12s. 

If you have different gearing for the motors, there is not much advantage.
```

---
## \#41 Posted by: lowGuido Posted at: 2016-07-28T22:06:55.791Z Reads: 311

```
Im going to point out the original post date.
The board in question has been rocking along for 12 months now with no failures.

There is a lot of talk about what people who havent done this think may happen.

I only comment on what I have actually done and real world results.

I should also point out again that I dont claim this is  a best thing to do. Its a fun experiment.
```

---
## \#42 Posted by: ugothakd Posted at: 2016-07-29T02:53:10.137Z Reads: 309

```
It's stated that two esc's are used, one for each motor. So technically they're running at different voltages. My question is what if we had a single motor, and then could gear for low speed like zero to 15mph, maxing out our motor to the highest voltage, then switch to a gear that allows for top speed, like 15mph to 30mph? Wouldn't that make it quicker?
```

---
## \#43 Posted by: PB1 Posted at: 2016-07-29T06:48:22.807Z Reads: 316

```
If it works ... it works, great!

Don't get me wrong, I really appreciate your work and your thinking outside of the box. 
And then getting it done!

Just tried to figure out in my head what is going on. Brain experiment before real life experiment. 

And one thought in my brain is: 
When your 200Kv motor with 70mm wheels and 2,5:1 gearing goes 37km/h it produces a voltage of around 37V and the ESC needs to be able to cope with that. Not many amps because there is not much load, but 37V. 
Obviously your ESC is able to cope with it. It works, great!
```

---
## \#44 Posted by: lowGuido Posted at: 2016-10-04T23:29:29.149Z Reads: 271

```
the UDR concept has come up again about 3 times this week so I thought I would update this thread.
the other day my friend and I were skating (he was on the UDR) and we had a bit of a drag race.

the UDR board KILLED it! like I was embarrassingly out accelerated.
I peaked at 36km/h and he just cruised away effortlessly.

I will try to get a video of it.
```

---
## \#45 Posted by: caustin Posted at: 2016-10-05T02:24:53.577Z Reads: 270

```
Thanks for pointing me back to this thread. Trying an uneven drive combo of 190kv enertion 6374 rear and 245kv Tacon Bigfoot front but on 12s. Think the uneven helps with the 245kv on 12s or still Erpm max issues with vesc?
```

---
## \#46 Posted by: michaeld33 Posted at: 2016-10-05T02:26:51.972Z Reads: 266

```
245kv on 12S? I think you'll hit the ERPM.
```

---
## \#47 Posted by: Jinra Posted at: 2016-10-05T02:27:10.184Z Reads: 272

```
definitely will hit the erpm limit and burn out your vesc
```

---
## \#48 Posted by: caustin Posted at: 2016-10-05T02:31:43.441Z Reads: 269

```
Sigh, really want to use these 2 Tacon Bigfoot on dual build but even 10s puts me slightly over 60k I believe but maybe in range of reasonableness?
```

---
## \#49 Posted by: Jinra Posted at: 2016-10-05T02:33:11.935Z Reads: 259

```
At 10s you're 12k over, you'll want to stick to 8s tops for the tacons
```

---
## \#50 Posted by: michaeld33 Posted at: 2016-10-05T02:39:34.857Z Reads: 257

```
Torqueboards or Maytech ESC? they should be able to handle the higher ERPM right?
```

---
## \#51 Posted by: caustin Posted at: 2016-10-05T02:46:38.810Z Reads: 252

```
That is a good point!  TB esc should be able to handle this at 10s, maybe 12s?  Was thinking too vest-centric. Anyone used TB esc for 245kv on 12s?  @torqueboards ?
```

---
## \#52 Posted by: michaeld33 Posted at: 2016-10-05T02:51:55.879Z Reads: 245

```
I never have, but I believe the ERPM is quite a bit higher than the VESC correct? It would be nice if @torqueboards chimed in.
```

---
## \#53 Posted by: torqueboards Posted at: 2016-10-05T02:57:58.611Z Reads: 243

```
No max ERPM for 12S TB ESC. It would work perfectly fine. VESC 6.0 shouldn't have a problem with this once it's available.
```

---
## \#54 Posted by: Jinra Posted at: 2016-10-05T02:58:10.054Z Reads: 248

```
I think the owner of Miami electric boards runs that high of erpm on his ESC, you could try that!

@oriol360
```

---
## \#55 Posted by: michaeld33 Posted at: 2016-10-05T02:59:37.990Z Reads: 241

```
I think we're all looking forward to 6.0
```

---
## \#56 Posted by: caustin Posted at: 2016-10-05T03:07:55.375Z Reads: 253

```
Good point, I actually got the 12s batteries from @oriol360 and was super satisfied there. Did not think to check his esc for 245kv on 12s. Maybe that or TB for sure, awesome!
```

---
## \#57 Posted by: lowGuido Posted at: 2016-10-05T06:13:56.570Z Reads: 260

```
well I went out today with every intention of filming the difference between a Dual diagonal 280kv twin and the 280/430kv uneven dual Rear drive.
unfortunately my friend left the nunchuck behind so we had 2 boards and 1 chuck.

so what did we do?

I grabbed a big stick and gave my mate the only chuck and used the stick to tow me along behind the UDR.

so I guess we tried a different type of experiment. the UDR can successfully haul ~170kg of human flesh up mild inclines.
```

---
## \#58 Posted by: saul Posted at: 2016-10-05T08:30:20.314Z Reads: 254

```
I wonder if the rc esc make this setup better or worse compared to vesc.

Can we start the formula esk8 racing already to see how much of a difference asymmetrical drives can make!
```

---
## \#59 Posted by: Mobutusan Posted at: 2016-10-05T09:38:02.002Z Reads: 253

```
I know dual TB 12s esc's work fine on 12s with TB 230kv motors up to 31mph. I rode two pretty spirited 13 mile and 15.5 mile tours on that setup the last two weekends, and it worked perfectly. When I finally finish my mountain board, I'm gonna run this same setup or go with a 245kv SK3 & 245kv Tacon pairing. I guess I'll find out if they both are really 245kv.
```

---
## \#60 Posted by: caustin Posted at: 2016-10-05T12:55:20.362Z Reads: 247

```
Nice, interested to hear how that build rides!  Yes, check vesc KV readout on those two motors and see how far apart they really are!
```

---
## \#61 Posted by: caustin Posted at: 2016-10-05T12:56:24.565Z Reads: 227

```
Oh no, I really wanted video evidence of you getting dusted!  Next weekend please!
```

---
## \#62 Posted by: lowGuido Posted at: 2016-12-10T04:24:52.539Z Reads: 220

```
ok I know I promised this a while ago but I finally found myself in a situation where my mate and I were out skating on both the UDR and the DD twin and had a camera on us.
we organised a drag race and filmed it. I will do my absolute best to get the footage onto youtube tonight!
```

---
## \#63 Posted by: caustin Posted at: 2016-12-10T04:39:51.907Z Reads: 233

```
Haha, awesome!  And yes we did not forget and we're holding you to it lol
```

---
## \#64 Posted by: saul Posted at: 2016-12-10T06:04:20.008Z Reads: 242

```
yea I wanna see this too! :sunglasses:
```

---
## \#65 Posted by: lowGuido Posted at: 2016-12-10T11:52:08.234Z Reads: 242

```
apologies for bad audio
https://youtu.be/Arwcq_Cp9es

I even tried a sneaky head start on the 2nd run...
```

---
## \#66 Posted by: Michaelinvegas Posted at: 2016-12-11T02:21:15.493Z Reads: 232

```
Very nice .. def food for thought
```

---
## \#67 Posted by: lowGuido Posted at: 2016-12-11T03:52:07.995Z Reads: 231

```
Just as another closing thought.
The DD in not by any means slow. And my mate on the UDR is bigger than me and never reached top speed. He says there is more in it but doesnt have the balls to take it there.. not in those exact words..
```

---
## \#68 Posted by: johnny_261 Posted at: 2016-12-11T10:19:56.321Z Reads: 223

```
This is pretty awesome. Thanks for getting a video up.  Do you think similar results would be achieved with uneven gearing? I wonder what would be more efficient. Changing the motor KV or gearing.
```

---
## \#69 Posted by: lowGuido Posted at: 2016-12-11T10:39:59.492Z Reads: 223

```
I haven't tried different gearing but I assume it would work simmilarly.
```

---
## \#70 Posted by: wmj259 Posted at: 2016-12-12T05:37:02.458Z Reads: 216

```
Can someone explain how these two completely different motors can be used in the same board?
```

---
## \#71 Posted by: lowGuido Posted at: 2016-12-12T10:03:22.649Z Reads: 225

```
what part did you want explained @wmj259?

there is a 280kv motor and a 430kv motor. the 280 helps get the 430 off the line with more torque and the 430 boosts up the top end with higher RPM.
each motor runs a separate ESC and there is no communications between either ESC. 
its pretty much all explained towards the start of this thread. which I again point out is more than a year old and this board is ridden daily.
```

---
## \#72 Posted by: Hummie Posted at: 2016-12-12T16:18:08.280Z Reads: 221

```
Have you been able to find the amp draw from either motor in time probably using vesc and telemetry?  I've seen others doing different kv on one board and getting different temps, higher kv being hotter.  I wonder if they take amps equally at different speeds
```

---
## \#73 Posted by: lowGuido Posted at: 2016-12-12T16:21:35.306Z Reads: 214

```
they would almost certainly be different amps at different speeds and different temperatures too.
however I have not done any specific tests other than skating.
```

---
## \#74 Posted by: Michaelinvegas Posted at: 2016-12-13T00:40:32.659Z Reads: 206

```
Thinking about doing offset kv and offset gearing

Like 170kv on 14t and 200kv on 18t

Or is the spread between not enough?
```

---
## \#75 Posted by: Ackmaniac Posted at: 2016-12-13T00:54:20.521Z Reads: 211

```
Why not connecting them via CAN. The master needs to be the one with the higher kv rating. Then switch off the breaking when max erpm is reached. And of course switch off the traction control for that. You only need to set the same max motor amps. 
You even could use my watt mode in my modded firmware for that. When max erpm for the slower motor is reached then the vesc simply shuts this one off. But I think a even setup with proper motors like 6355 work better.
```

---
## \#76 Posted by: Magixpencer Posted at: 2017-09-07T20:16:52.721Z Reads: 169

```
I am planning on building a board for cruising long distance and am planning on using a 400kv motor as the drive. I am about 140lbs and don't need the acceleration torque, just looking for a decent top speed and long range. I plan on using 2 5ah 3s 50c batteries with a 150amp esc, gearing ratio is 17/44 This is my first build, any pointers are welcome and appreciated
```

---
## \#77 Posted by: Idle Posted at: 2017-09-07T22:04:24.404Z Reads: 172

```
I just read this same thing about your plan.
I'll see if I can find it for u


But I digress, this is a discussion about using two motors of different size and kw to have great startup torque and good top end speed.
```

---
## \#78 Posted by: Idle Posted at: 2017-09-07T22:09:57.330Z Reads: 177

```
This thread I think is for you to read.
 *too high KV motor

http://www.electric-skateboard.builders/t/build-review-aiming-high-torque-with-final-speed-of-45km-h/13023/18
```

---
## \#79 Posted by: Magixpencer Posted at: 2017-09-07T22:11:04.742Z Reads: 176

```
Thank you for looking at it, I do intend on going dual motor eventually, and was intuiged by the mismatched kv value, mybe could use in leu of a transmission to achieve a greater band of acceleration
```

---
## \#80 Posted by: Namasaki Posted at: 2017-09-07T22:13:40.016Z Reads: 181

```
[quote="Magixpencer, post:76, topic:113, full:true"]
I am planning on building a board for cruising long distance and am planning on using a 400kv motor as the drive. I am about 140lbs and don't need the acceleration torque, just looking for a decent top speed and long range. I plan on using 2 5ah 3s 50c batteries with a 150amp esc, gearing ratio is 17/44 This is my first build, any pointers are welcome and appreciated
[/quote]


That doesn't sound like a recipe for long range, but then I guess it depends on what you consider long range.
And I would agree with @Magixpencer that 400kv is too high
```

---
## \#81 Posted by: lowGuido Posted at: 2017-09-08T07:46:50.680Z Reads: 162

```
I have been in a situation where the belt snapped on the 280kv side of the UDR and needed to ride it home on the 430kv only. It worked but it wasnt happy.
```

---
## \#82 Posted by: scepterr Posted at: 2017-09-08T08:06:03.870Z Reads: 163

```
Belt snap :hushed: clearly I'm not doing something right....hehe
How did that happen?
```

---
## \#83 Posted by: lowGuido Posted at: 2017-09-08T09:21:38.008Z Reads: 159

```
they wear out eventually. nothing exciting.
```

---
## \#84 Posted by: scepterr Posted at: 2017-09-08T09:24:32.342Z Reads: 160

```
How many miles do you think you got on that belt?
```

---
## \#85 Posted by: lowGuido Posted at: 2017-09-08T09:32:28.051Z Reads: 158

```
no idea. it was ridden daily for about a year or so. it was a lot.
```

---
## \#86 Posted by: Cobber Posted at: 2017-09-08T09:37:42.711Z Reads: 171

```
[quote="Namasaki, post:80, topic:113"]
that 400kv is too high
[/quote]

It is not normal for sure, but depending on system voltage combined with wheel roll out/ gearing it might not be funky.
Hub guys are running <70kv but the Stooge is running >1350kv so...
@Magixpencer prob more questions in another thread would be a better idea ;) as it sounds a bit different
```

---
## \#87 Posted by: Namasaki Posted at: 2017-09-08T13:37:42.206Z Reads: 167

```
Maybe it would be more appropriate to say that 400kv is simply not practical for Esk8
```

---
## \#88 Posted by: Magixpencer Posted at: 2017-09-08T22:18:28.472Z Reads: 163

```
Thank you, I will make changes and post again.
```

---
## \#89 Posted by: TheFluffiest Posted at: 2018-02-28T09:38:32.921Z Reads: 129

```
How did you do dual independent vescs? I'm very interested in this, but don't know if I would be able to do it. Are they ran on separate channels or something?

Sorry for revamping the really old thread, I'm just super intrigued by this!
```

---
## \#90 Posted by: pat.speed Posted at: 2018-02-28T09:40:49.025Z Reads: 132

```
You have to split the ppm cable or use dual receivers. I'm not sure if canbus would work with uneven dual drive
```

---
## \#91 Posted by: lowGuido Posted at: 2018-03-01T22:13:38.368Z Reads: 120

```
Split ppm cable with 5v cut on one end.
```

---
## \#92 Posted by: TheFluffiest Posted at: 2018-03-05T23:59:15.230Z Reads: 115

```
In that case, could you use seperate brands of vesc? Or maybe even different types of esc altogether? I don't plan on doing that, I'm just curious to see if it would work
```

---
## \#93 Posted by: pat.speed Posted at: 2018-03-06T01:02:54.197Z Reads: 107

```
There's no reason is wouldn't work
```

---
## \#94 Posted by: lowGuido Posted at: 2018-03-06T03:31:45.303Z Reads: 98

```
Yeah there is literally no communication between ESCs so you can use different ones if you want to.. it would make no difference.
```

---
