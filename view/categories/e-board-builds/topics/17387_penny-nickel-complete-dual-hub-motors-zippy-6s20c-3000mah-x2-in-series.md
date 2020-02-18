# Penny &ldquo;Nickel&rdquo; complete dual hub motors zippy 6s20c 3000mah x2 in series

### Replies: 329 Views: 15729

## \#1 Posted by: Sapphirinia Posted at: 2017-02-08T16:13:54.965Z Reads: 944

```
Hi, I've been wanting to make a nice compact portable build for a couple months now. I've final started getting some parts and understanding things a little better. Basically, I'm on the lighter side,  completely used to commuting with a penny board, fruit boots 😁, and regular skateboards. I do my commuting in the city, Philadelphia to be exact. So crazy speed is not a concern, but philly is actually very bike friendly so skating in the bike lanes has always been a norm. You can get around faster in the city on a board or bike than in a car during rush hours. 
Soooo, I have embarked on this journey using a new nickel board. I got 2 zippy 6s20c 3000mah batteries which I will be setting up in series. Waiting on the connectors to come in the mail now. I have a balance charger and was told charging them in parallel will be faster so I got an adaptor for that as well on the way. I found a $23 reciever/transmitter on ebay that is on the way. I found a little tray at the thrift store for $0.99 that fits PERFECT for my enclosure. It even has vent holes. 
I've made a little holder for the batteries with some of the anti explosion box I was given for my Samsung note 7. Used some frozen duct tape to get that to work, and used more of the box for dividers just for safety from rattling and bouncing. 
I drilled 2 holes in the board and enclosure and used screws and nuts to connect them. So just 2 nuts to take it off and put it on. I will probably get the thumb nuts or whatever they're called to make it easier to put on and take off. 
I may drill more holes depending on what things look like when my hub motors finally come in. They should be 75kv. I will also have dual vesc which I'm also waiting on.
I would like to add an antispark switch but I'm still searching for one. If I can add a little screen that says the charge level that would be great too. 
 <img src="/uploads/db1493/original/3X/3/2/326901b952da47f07f67fb8538f24c7f4e8ba1d0.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/6/268b322232d7055c9718530241dd748876e0815f.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/5/5/553e82504ba431b49f0e46abb3b4a160e6391af5.jpg" width="507" height="500"><img src="/uploads/db1493/original/3X/3/6/362eda767720fc86775539b95dad2f2a390fc022.jpg" width="472" height="500">
```

---
## \#2 Posted by: Smorto Posted at: 2017-02-08T16:38:30.760Z Reads: 832

```
Looks great! Should be fun, only thing I see is that 20c with 3000mah is only 60A continuous **if** those batteries actually can do 20c which Zippys have a reputation of overstating what they can actually perform if that makes sense. You could always run 2 more in series than put those 2 12s packs in parallel to solve this issue. However, if you plan on going very low speeds and not up many hills maybe you could manage to not draw more than 60A. However I am not an expert in this by any means so if anyone has anything else to add that would be great.

PS-Just out of curiosity what KV will your motors be?
```

---
## \#3 Posted by: Sapphirinia Posted at: 2017-02-08T16:42:35.526Z Reads: 784

```
75kv motors
```

---
## \#4 Posted by: Sapphirinia Posted at: 2017-02-08T16:51:08.807Z Reads: 773

```
Thanks, I had to ask really quick on the kv lol. But anyways, what is an example of low speeds for you? I want to be able to keep up with the bikes and other people on skateboards. This is my first build. And I just updated my post a bit with that info.
```

---
## \#5 Posted by: Smorto Posted at: 2017-02-08T16:59:59.406Z Reads: 752

```
Low speed should be around 10ish MPH. However, I do not know how many amps you will draw at that speed or any speed for that matter. I do know that it depends on a number of factors though. This could be completely wrong but I believe you running 12s should help you draw less amps but again I am not sure. I would defiantly wait for someone else opinion.
```

---
## \#6 Posted by: radium Posted at: 2017-02-08T17:36:00.607Z Reads: 729

```
More voltage (so 12S = 44.4V 6S = 22.2V) will result in less current being drawn to generate a given amount of power. You will draw the most current when starting or going up hills, basically whenever motors have an increased load.

Power = Voltage * Current(Amps)

So a 44.4V nominal battery will draw half the current for a given power output when compared with a 22.2V nominal battery, all other things being equal.
```

---
## \#7 Posted by: Smorto Posted at: 2017-02-08T17:37:28.910Z Reads: 694

```
Aha! Thanks for the clarification and much better explanation on my point.
```

---
## \#8 Posted by: Sapphirinia Posted at: 2017-02-08T19:37:16.089Z Reads: 714

```
Getting my penny gripped
<img src="/uploads/db1493/original/3X/4/e/4e365e1a1116f335adc19ad6a22b3564dddaa3f2.jpg" width="690" height="427">
```

---
## \#9 Posted by: Sapphirinia Posted at: 2017-02-08T22:36:44.151Z Reads: 712

```
It's getting sexier by the day 😄<img src="/uploads/db1493/original/3X/3/2/322b76cd6f77a0da1f1a5618b760ad0a93377521.jpg" width="657" height="500">
```

---
## \#10 Posted by: Sapphirinia Posted at: 2017-02-08T23:36:45.209Z Reads: 710

```
<img src="/uploads/db1493/original/3X/b/e/be49d52657a6ff2055accc3d15f7dbf6fda0f423.jpg" width="247" height="500">
```

---
## \#11 Posted by: kane Posted at: 2017-02-09T09:10:14.139Z Reads: 688

```
I'm curious how your going to mount the motors. Or are you going to use hub motors, perhaps?
```

---
## \#12 Posted by: Pedrodemio Posted at: 2017-02-09T12:40:16.752Z Reads: 690

```
Nice board,  do you have idea about the final weight?

And about the discharge, in my opinion people tend to exaggerate what is really needed for a board, if can do 60A great, if not, just limit to 30A, 15A each vesc

For exemple, my board the limit is 20A due to the battery limitation, but that is plenty for a fun ride and to climb 12% hills with no problem

Sure, if you live in San Francisco you need massive amounts of current/power to be able to climb in a decent speed

The hubs could want more current, but if where you live is mostly flat with few hills you are good

What really need power is acceleration, when you are at cruising even at higher speeds the power consumption is "low"
```

---
## \#13 Posted by: Sapphirinia Posted at: 2017-02-09T13:37:44.127Z Reads: 636

```
Hub motors
```

---
## \#14 Posted by: Sapphirinia Posted at: 2017-02-09T14:17:44.870Z Reads: 627

```
Not sure on weight yet. Hoping under 10 lbs. And I hope you're right. I've gotten so much conflicting info on going series or parellel
```

---
## \#15 Posted by: osbor Posted at: 2017-02-09T14:19:17.052Z Reads: 621

```
your build is like, un-apologetically 90s as hell
like i expect someone on saved by the bell to be using it
```

---
## \#16 Posted by: Sapphirinia Posted at: 2017-02-09T14:26:03.267Z Reads: 620

```
It's beautiful lol. The 90s were the best anyway
```

---
## \#17 Posted by: Mikenopolis Posted at: 2017-02-09T15:48:37.820Z Reads: 660

```
I miss the late 90's. Compared to today, its seem much less pretentious. Zach Attack.

I totally forgot the Nickel had a kicktail, that make turning so much better. Are you sure that cardboard is anti explosion? Seems more fire prone.

Maybe you can look into CLEVIS PINS as a mounting option and use weatherproof seal around the enclosure to reduce rattling
```

---
## \#18 Posted by: Sapphirinia Posted at: 2017-02-09T17:44:21.748Z Reads: 659

```
It's got a fireproof coating. It's thick and white.
```

---
## \#19 Posted by: Sapphirinia Posted at: 2017-03-28T23:01:09.005Z Reads: 655

```
<img src="/uploads/db1493/original/3X/5/6/561f8e2aabea02dd4115bb66055a7e7b10ad9e99.jpg" width="690" height="388">
So, this picture got flagged in the no words posts but this was the aftermath of my second explosion during this build. Literally was showing off for one of my friends, brought the battery pack down the stairs, my button made contact and it blew part of my metal button apart. Bittersweet since the metal probably saved my skin, but the metal caused the problem in the first place... Be careful with lipo batteries guys
```

---
## \#20 Posted by: Jebe Posted at: 2017-03-28T23:23:58.284Z Reads: 646

```
Love the recycling of the Samsung air friendly box!
```

---
## \#21 Posted by: Smorto Posted at: 2017-03-29T00:49:01.458Z Reads: 631

```
Wow! Glad you are okay though.
```

---
## \#22 Posted by: Sapphirinia Posted at: 2017-03-30T05:39:11.326Z Reads: 634

```
<img src="/uploads/db1493/original/3X/3/7/37b84604631562f869c74dd6f6c62ad4a9fd2447.jpg" width="612" height="500">
I got lights! Gotta figure out the remote though, since it's not moving. Still slightly nervous as the lipos have shown me their power a few times now
```

---
## \#23 Posted by: saul Posted at: 2017-03-30T21:31:04.012Z Reads: 621

```
Careful with lipo! I usually tape over the connectors when I'm not using them.

Nice build, do you have a link to the hubs?
A mini remote would be good for this, funny to have such a huge remote on a mini build.
```

---
## \#24 Posted by: willpark16 Posted at: 2017-03-31T01:15:35.294Z Reads: 616

```
50 bucks each on eBay
```

---
## \#25 Posted by: Sapphirinia Posted at: 2017-03-31T02:38:21.489Z Reads: 628

```
I got the hubs from Alex Tech on here along with the vescs. I believe I connected everything right but I can't get the wattage reader to say the correct battery percentage and I can't the wheels to move. I believe I binder the remote. I bought the cheapest remote I could find, along with a 3d printer thinking I could make a small case for it later. 
 <img src="/uploads/db1493/original/3X/c/0/c07931427323f3ee92f654807302a6669723c6db.JPG" width="690" height="461">
```

---
## \#26 Posted by: Sapphirinia Posted at: 2017-03-31T02:45:19.976Z Reads: 602

```
Good idea with the tape. My friend stuck a balloon over the connector after it fried my pants lol. I had a party at my house that day
```

---
## \#27 Posted by: willpark16 Posted at: 2017-03-31T05:24:27.113Z Reads: 587

```
Let me know how those hubs are tho
```

---
## \#28 Posted by: Pr0dy Posted at: 2017-03-31T15:19:50.156Z Reads: 578

```
Those hubs got me (150lbs) up to 34km/h with 10s
```

---
## \#29 Posted by: faithfulpuppy Posted at: 2017-03-31T15:45:26.310Z Reads: 566

```
How's the torque on them?
```

---
## \#30 Posted by: willpark16 Posted at: 2017-03-31T15:57:59.223Z Reads: 563

```
Damn! More charachters
```

---
## \#31 Posted by: Wubbalubbadubdub Posted at: 2017-04-01T16:50:28.400Z Reads: 552

```
I bought his mach 1 elite. I have had two of his hubs and two of his VESCs burn out on me over the course of less than 1 mile total ride time.
```

---
## \#32 Posted by: Sapphirinia Posted at: 2017-04-01T18:41:12.080Z Reads: 562

```
Wow. That sucks. Hope I have better luck. Took long enough to get them...
```

---
## \#33 Posted by: jmasta Posted at: 2017-04-01T19:03:50.320Z Reads: 590

```
[quote="Sapphirinia, post:25, topic:17387, full:true"]
 <img src="/uploads/db1493/original/3X/c/0/c07931427323f3ee92f654807302a6669723c6db.JPG" width="690" height="461">
[/quote]

Hey I wanted to let you know that your truck is backwards...
```

---
## \#34 Posted by: Sapphirinia Posted at: 2017-04-03T04:51:49.759Z Reads: 551

```
Thanks for that. Good eye
```

---
## \#35 Posted by: paulus_germanus Posted at: 2017-04-06T21:18:23.313Z Reads: 571

```
[quote="Sapphirinia, post:19, topic:17387"]
robably saved my skin, but the metal caused the problem in the first place... Be careful with lipo batteries guys
[/quote]

wow! wasn't aware that those lipos can be so dangerous... thanks for sharing! i'll be like 10x more vigilant with them from now on. Glad you're fine!
```

---
## \#36 Posted by: Sapphirinia Posted at: 2017-04-09T19:45:57.689Z Reads: 569

```
Can anyone give me some tips on soldering? I'm so bad... <img src="/uploads/db1493/original/3X/0/c/0c14fa3460312fd2e1ec3ace61fb717a6821238a.jpg" width="281" height="500">
```

---
## \#37 Posted by: paulus_germanus Posted at: 2017-04-09T21:03:40.241Z Reads: 555

```
What I did was I dismantled some old radio and desoldered and resoldered back on evertyting inside I could lay my soldering iron on. But before that check youtube - there is like a million tutorials on soldering there. There is no way you're bad at it, you just haven't had enough practice, and I'm sure that if you put your heart to it and do practice according to the rules from the tutorials you'll be a master (maestra?;)) in no time! :smile_cat:
```

---
## \#38 Posted by: Smorto Posted at: 2017-04-09T21:05:46.135Z Reads: 560

```
I would recommend clamping the XT90 to keep it from moving and easier to work with. Then 'tin' the metal part which means to fill it with solder. I would do this by heating up the metal part with your iron from the bottom, then pushing your solder into the metal part so it melts and fills up. Then 'tin' your wire. Once you have that done, you need to melt the solder in the XT90 by putting your iron on the bottom once again. Then when it is liquid, push the wire into the melted solder and remove your iron and wait for it to harden. This step takes some practice and getting used to. This is how I do it and it works for me, though I am sure there are different ways.

I would also record a thinner solder as I find it easier to melt and work with.
```

---
## \#39 Posted by: Sapphirinia Posted at: 2017-04-09T22:13:58.291Z Reads: 558

```
Finally got everything resoldered... Binder the remote but still no movement in the hubs... Can anyone Skype me though this? I'm so close<img src="/uploads/db1493/original/3X/1/6/1660b1dab66d30641fa1b7c1a7113f44c1331fc9.jpg" width="690" height="495">
```

---
## \#40 Posted by: Sapphirinia Posted at: 2017-04-11T19:08:13.311Z Reads: 548

```
I got 1 wheel spinning but can't get the other one spinning. It'll spin when I do the test/analyze thing in bldc
```

---
## \#41 Posted by: mmaner Posted at: 2017-04-11T20:52:37.283Z Reads: 506

```
I think I see your not using a CAN bus.  Do you have both VESCs set to PPM?  Go to General > App Configuration and make sure both are set to PPM or PPM with Uart if you are using bluetooth.
```

---
## \#42 Posted by: DaveMess Posted at: 2017-04-11T23:37:30.028Z Reads: 501

```
Your battery monitor is reading wrong because it probably hasn't been set up correctly. Are there any buttons on the back of it? If so try holding one of them on start up and it should go into a programming mode where you tell it what type/how many cells you have. I can't tell from the pic what kind of meter it is. 
Edit: for clarity
```

---
## \#43 Posted by: Sapphirinia Posted at: 2017-04-12T00:10:44.756Z Reads: 491

```
I know how to set it but not what to set it to.
```

---
## \#44 Posted by: Sapphirinia Posted at: 2017-04-12T00:16:24.963Z Reads: 489

```
I do have them both set to PPM. I've tried switching around a bunch of settings though. I was also trying to search to see what a can bus look like. So I still don't know
```

---
## \#45 Posted by: boards Posted at: 2017-04-12T00:40:20.416Z Reads: 495

```
Are your PPM wires going to the receiver going to the same channel (slot on the receiver)? It looks like they aren't.

You can try swapping them and the other wheel should spin if this is the case.

If that's the problem you want to make a y cable of sorts so that both ppm cables go to the same 3 pins on the receiver.
```

---
## \#46 Posted by: DaveMess Posted at: 2017-04-12T01:12:52.674Z Reads: 484

```
Oh ok sorry, I probably can't help you then. I had to search around and find a manual for mine online, the guy who sold it to me didn't include one.
```

---
## \#47 Posted by: mmaner Posted at: 2017-04-12T01:41:50.896Z Reads: 504

```
It's just a 2 wire lead that connects the VESCs so you have a master and slave.  You can get them from @torqueboards pretty cheap.
```

---
## \#48 Posted by: Sapphirinia Posted at: 2017-04-15T21:09:37.298Z Reads: 512

```
<img src="/uploads/db1493/original/3X/a/f/afe7f2ac502e7c3623b30a5f3cc0a64745c86001.jpg" width="690" height="388">

They're connected like this
```

---
## \#49 Posted by: mmaner Posted at: 2017-04-15T21:36:42.774Z Reads: 503

```
Splitting the RX channels is the other method of using dual VESCs.  Looks right but hard to tell from the pic.
```

---
## \#50 Posted by: Sapphirinia Posted at: 2017-04-15T23:38:38.930Z Reads: 490

```
They're both spinning now! Woot
```

---
## \#51 Posted by: mmaner Posted at: 2017-04-15T23:39:06.174Z Reads: 477

```
Yay 😀.  What was the problem?
```

---
## \#52 Posted by: Sapphirinia Posted at: 2017-04-16T00:40:35.663Z Reads: 480

```
Not a clue. But I did again resold er a bunch of stuff. Got it back together and they both worked. Going to take some getting used to. It's super powerful
```

---
## \#53 Posted by: Sapphirinia Posted at: 2017-04-16T00:50:32.808Z Reads: 504

```
UPDATE: I finally have a working board. Thanks for all the help. Had to ditch a few things, resolder stuff at least 4 times. Probably the longest thing I had to work on for the project. I still have an altoids headlight that I made that I'll eventually put on there. Will reevaluate my battery meter. It was hard fitting everything into the small space, plus I lost the power cable to my good drill so I didn't put anymore holes in to house the meter. I also bought a little camera on hobbyking.com that I want to find a nice spot for. Of course an easier way to charge the batteries would be great in the future, and actually incorporating an easier to use power switch. It's not too difficult to open the enclosure for access to the stuff inside. Just use the skate tool to unscrew one side and slide it over. <img src="/uploads/db1493/original/3X/1/b/1b2d99e76afef918d6ebca9421b243d9045a00c0.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/5/1/511520c87f69988f8a5e943d860380fa0bafa8ed.jpg" width="690" height="340">
Still not a fan of the big wheels and trucks
```

---
## \#54 Posted by: mmaner Posted at: 2017-04-16T00:55:45.843Z Reads: 486

```
I use a 3d printed panel mount for xt90-s connectors. Just drill a hole and hit glue it in.  Searxh for my mini-logo  build and you can see it in aactio.  PM me you address I'll mail you one.
```

---
## \#55 Posted by: Gabriel_Robinson Posted at: 2017-04-18T01:38:00.045Z Reads: 472

```
how does it ride i want to put my build on a penny
```

---
## \#56 Posted by: Sapphirinia Posted at: 2017-04-18T18:14:20.406Z Reads: 471

```
Will keep you updated. I left it in the car for a few days thinking I'd ride it and didn't get the chance and now it won't go. I think it overheated in my car... Womp Womp Womp....
```

---
## \#57 Posted by: Sapphirinia Posted at: 2017-04-18T19:04:02.426Z Reads: 463

```
So I got the chance to take it out, but it wouldn't go at first. I think maybe it was too hot in my car so I kept it inside for a while before I tried it again. It worked again, but after about a minute of riding it, it stopped again. Lights stayed on each time the motors weren't moving. Gave it a break again, and it worked again. Not sure if it's over heating, or somethings loose. But I'll take it apart tonight to see what I can figure out
```

---
## \#58 Posted by: Sapphirinia Posted at: 2017-04-18T19:08:05.898Z Reads: 454

```
Also, it seems as though it may be too powerful for me. Would it be a better idea to wire the batteries in parallel? I have to be extremely light on the throttle. While Im riding it tends to get jumpy and nearly throw me off.
```

---
## \#59 Posted by: mmaner Posted at: 2017-04-18T20:29:16.471Z Reads: 454

```
You could run it in 6s, no worries.  You might want to limit the VESC motor max setting first and see how that goes for you.  As far as running for a min and then not, It could be a million things.  SOunds like maybe a cold solder joint that expands when it gets hot and looses contact.  I would see if the VESC is still on when the cut-out occurs.
```

---
## \#60 Posted by: Sapphirinia Posted at: 2017-04-18T22:48:42.747Z Reads: 453

```
I charged the batteries and it seems to work now 😂 rookie mistake. I did resold er like 4 times already. Hopefully that was it. Won't get a chance to try it again til tomorrow when my kids aren't with me. Nervous to stuff everything back in the enclosure but I'll see. Thanks for the suggestions. This thing shoots from under me. I ordered a parallel connector that'll I'll try when it gets here.
```

---
## \#61 Posted by: mmaner Posted at: 2017-04-18T22:59:10.698Z Reads: 461

```
There's not a lot of real estate to a penny, so its never going to be incredibly stable.  You might look at getting a [Benchwheel](http://miamielectricboards.com/shop-1/handheld-electric-remote) or [Enertion Nano-X](http://Enertion Nano-X) remote so you can put the board in 'cruise' mode.  You can read more about them here...

https://www.electric-skateboard.builders/t/remotes-commercially-available-options/15162

Ill get that XT90 panel mount out to you this week, just been incredibly busy at work :frowning:
```

---
## \#62 Posted by: Sapphirinia Posted at: 2017-04-18T23:20:23.092Z Reads: 463

```
<img src="/uploads/db1493/original/3X/b/e/be92534a9f63076647d76f2010cc3889d6f6b2cd.jpg" width="281" height="500">
Im using this remote now. I wonder if these settings can change that
```

---
## \#63 Posted by: mmaner Posted at: 2017-04-18T23:39:36.119Z Reads: 448

```
I don't know.  I've never had a mini remote, I've got one ordered. I'll let you know when I get it.
```

---
## \#64 Posted by: Sapphirinia Posted at: 2017-04-23T02:24:36.465Z Reads: 440

```
So, my boards acting really odd. Like the trigger isn't working but the side turning thing makes the wheels spin. I rebinded the controller since it kept blinking. After I did that it seems to have some issues.some times it'll go without hitting the throttle, and stop when I hit it. When I move it in the opposite direction it speeds ups. Very wierd. I never changed the vesc settings since it started working. I posted a video. https://youtu.be/RBiLbaeCYPI
```

---
## \#65 Posted by: mmaner Posted at: 2017-04-23T02:42:09.628Z Reads: 427

```
Move the RX lead to channel 2.
```

---
## \#66 Posted by: hornet90 Posted at: 2017-04-23T07:41:59.857Z Reads: 422

```
move to ch2 i had same problem, and move the th trim till motor stops.
```

---
## \#67 Posted by: hornet90 Posted at: 2017-04-23T07:46:56.144Z Reads: 413

```
make sure u have a red light on the receiver and its not blinking,
```

---
## \#68 Posted by: Sapphirinia Posted at: 2017-04-24T18:43:39.584Z Reads: 407

```
That fixed it. Rode it for about 10mins off and on then it stopped working again... Motors stopped spinning when I use the remote
```

---
## \#69 Posted by: Michaelinvegas Posted at: 2017-04-24T19:33:23.911Z Reads: 402

```
Could be a bad reciver .... do you have a spare remote set?
```

---
## \#70 Posted by: Sapphirinia Posted at: 2017-05-20T21:01:43.859Z Reads: 400

```
So I've rechecked and tinkered since last time and attempted to run the batteries in parallel, but I couldn't actually get the motors to move like that. I messed around with the blcd tool and lowered it to 40amps from 60. It's still has a pretty jumpy start. Like I have to have sort of a rolling start but it still takes off from under me unless I'm super gentle on the throttle. Which settings should I mess with?
```

---
## \#71 Posted by: Sapphirinia Posted at: 2017-05-24T21:29:55.989Z Reads: 396

```
I can finally control the beast! Yay. Still super sensitive though. https://youtu.be/pL3quH_QRYs
```

---
## \#72 Posted by: boards Posted at: 2017-05-24T22:37:38.218Z Reads: 403

```
I think there is a "current ramp" setting that you could lower (ex half it) and it might help.
```

---
## \#73 Posted by: Sapphirinia Posted at: 2017-05-24T23:57:41.086Z Reads: 420

```
I'll look into that. Kind of just learning to work with it as if I was going from my Nissan to a Lamborghini lol. Getting some muscle memory. I changed the max watts(?) from 60 to 40. I'm also wondering if that means longer battery life. Now I have to make a little enclosure for this little camera and figure it out. <img src="/uploads/db1493/original/3X/f/1/f1fff8fda58e0f7be0aec1ac6d5131ce73ba4984.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/e/2/e20b866d194cc1a54404477c7b6ba1c5e4976420.jpg" width="374" height="500">
```

---
## \#74 Posted by: Sapphirinia Posted at: 2017-05-25T18:41:38.302Z Reads: 407

```
<img src="/uploads/db1493/original/3X/a/4/a45fc499bf728067bd7d6a012ce50f2e37c5ca36.png" width="243" height="500">I'm so excited. This is the best thing I've ever made.
```

---
## \#75 Posted by: Sapphirinia Posted at: 2017-05-28T19:23:38.648Z Reads: 397

```
Noo! I tried my connectors for like the 5th time trying to install the better meter. I finally got a dremel and made pretty spots for the anti spark and battery meter. Fit them in there but as I tried to connect the battery, again, I fried my connectors and now I have to replace them... I wanted to do my endurance test tomorrow but now I have a bunch more wiring to do. At least the Soldering iron I bought seems to work better.
```

---
## \#76 Posted by: Sapphirinia Posted at: 2017-05-29T22:07:56.946Z Reads: 405

```
<img src="/uploads/db1493/original/3X/a/0/a09501ebb988679ac9ebbe3ccfc6860f57426893.jpg" width="500" height="500">
I've discovered the dremel tool. Now I have voltmeter access. I'm not sure if it's programmed right but it's easy enough to change the settings. Just wasn't sure what info to put in for volts. Whether it be 22.2 or 44.4.i managed to get just one wheel to work again so hopefully it's an easy fix
```

---
## \#77 Posted by: Sapphirinia Posted at: 2017-05-30T02:41:42.159Z Reads: 391

```
Solder on the phase wires got messed up. It happened 3 more times before I got the board back together. All of them were probably ready to go. Really tight fit getting everything to fit in that enclosure
```

---
## \#78 Posted by: nimbuskate Posted at: 2017-05-30T03:29:05.988Z Reads: 393

```
Can i buy your nickel trucks? 😊
```

---
## \#79 Posted by: Sapphirinia Posted at: 2017-06-03T00:20:34.952Z Reads: 405

```
My vesc fried! 😢 I made it 3.53miles before it died on me. After I let it sit a few hours I could get it to turn back on but the light was blinking red on one vesc. I tried hooking it up to my computer to see if there were any error codes but when I hit test motor it caught on fire and fried it. Not sure what happened but that was my most expensive thing to break so far... 
<img src="/uploads/db1493/original/3X/f/7/f7e293333be47044f5c9f13876f1e367ae8dd7fc.jpg" width="449" height="500">
```

---
## \#80 Posted by: Sapphirinia Posted at: 2017-06-03T00:23:56.580Z Reads: 402

```
<img src="/uploads/db1493/original/3X/e/d/ed18e91bf04635edc4240148a4148480a2bb841b.jpg" width="374" height="500">
```

---
## \#81 Posted by: jet Posted at: 2017-06-03T01:35:36.931Z Reads: 377

```
Damn! Which vesc is that and where'd you get it from?

You can just downgrade to 1 motor for now right?
```

---
## \#82 Posted by: Sapphirinia Posted at: 2017-06-03T02:10:09.899Z Reads: 374

```
I got it from Alextech on here. I'm going to see if I can figure out how to just use one motor
```

---
## \#83 Posted by: Alextech Posted at: 2017-06-03T21:06:48.193Z Reads: 378

```
@Sapphirinia You should probably wait till you get another Vesc, I have had customers who used one and burned the enamel inside the Hub. It's odd to see it short like that, they look a little wet? Perhaps dust.  It's definitely blown on the DRV, check for shorts on the phase wires.
```

---
## \#84 Posted by: Sapphirinia Posted at: 2017-06-16T16:29:57.046Z Reads: 372

```
It's possible that there was a short in a phase wires as I had to resoldered like 4 of them. U should just resoldered all of them. Definitely was not wet. A little dusty though from riding I assume. Not sure where to go from here. No more money to dump into it at this moment
```

---
## \#85 Posted by: Sapphirinia Posted at: 2017-07-11T02:10:05.460Z Reads: 375

```
So I finally bought another vesc and all the connections are different. The rc connections aren't soldered on. The motor connections are bigger and the battery connections are xt90 instead of xt60. What would be my best way to reconnect everything? I like how much thicker the cables are on the new one but want to do it the best possible way. <img src="/uploads/db1493/original/3X/4/a/4a6c85a1679f7c1df437d94597f576cd697ed34e.jpg" width="374" height="500">
```

---
## \#86 Posted by: lrdesigns Posted at: 2017-07-12T02:56:52.769Z Reads: 349

```
Best way is to re-solder on the correct connectors, but your going to need a beefy iron to heat up these thick wires. Or you could make adapters but that would be messy and harder to fit in the enclosure.
```

---
## \#87 Posted by: Sapphirinia Posted at: 2017-07-12T23:19:36.096Z Reads: 356

```
Thanks. If I do that I SAS just going to cut off the old ones and stick them on the new ones. What about the receiver connection?
```

---
## \#88 Posted by: longjohn Posted at: 2017-07-15T07:11:33.762Z Reads: 358

```
how much money have you spent so far ?
```

---
## \#89 Posted by: Sapphirinia Posted at: 2017-07-16T19:03:59.156Z Reads: 360

```
Probably $600 or so
```

---
## \#90 Posted by: Sapphirinia Posted at: 2017-07-16T19:06:05.868Z Reads: 367

```
I resoldered everything, got all the lights on, been swapping around phase wires but still can't get the wheels to spin... <img src="/uploads/db1493/original/3X/9/0/90fea30e25d883a5bbd3b053aa0de67d6d553b3e.jpg" width="666" height="500">
```

---
## \#91 Posted by: wafflejock Posted at: 2017-07-16T19:07:12.935Z Reads: 356

```
What's going on in the bldc tool?  Did you do the calibration yet or mess with app/control settings?

Phase wire swapping will just reverse the motor direction it should move either way so long as they're connected even if one is loose the motor should jitter.  Would check battery cut off limits and do the calibration then check the app config assuming calibration works out.
```

---
## \#92 Posted by: Sapphirinia Posted at: 2017-07-16T19:08:43.065Z Reads: 345

```
Everything I try motor detection it fails. This is on either vesc. I did unplug all the phase wires when I resoldered them so I'm not exactly sure of the correct order. I've tried to set everything the same as it used to be when it used to work.
```

---
## \#93 Posted by: wafflejock Posted at: 2017-07-16T19:10:12.359Z Reads: 344

```
Make sure calibration is done with belts removed so the motor spins freely as well
```

---
## \#94 Posted by: Sapphirinia Posted at: 2017-07-16T19:13:18.627Z Reads: 332

```
They are hub motors
```

---
## \#95 Posted by: wafflejock Posted at: 2017-07-16T19:14:23.524Z Reads: 323

```
Ah okay yeah just no load on them while calibrating so make sure the board is just flipped in the case of hub motors I guess.
```

---
## \#96 Posted by: Sapphirinia Posted at: 2017-07-16T19:26:18.028Z Reads: 319

```
Ok, I'll try that. I had it raised
```

---
## \#97 Posted by: wafflejock Posted at: 2017-07-16T19:46:10.523Z Reads: 342

```
When it fails calibration is the motor moving at all or is it totally motionless the whole time?

If the former I'd assume your connections are good and you just need to adjust the settings it starts off with for the calibration maybe (I'm not too experienced with that issue though since mine seemed to calibrate basically first shot, after removing load).  If it jitters but doesn't fully turn could either be one loose phase line or lack of power through the mosfets feeding it, if it turns but the calibration just fails I'd lean more towards it just being something in the config that needs to be set before running the calibration (not sure what though exactly, perhaps different BEMF coupling and integrator values but not sure where a good starting point is for those I just trusted it gave me the right info)

If the latter (no motion) would guess wiring or power settings on the battery cut offs.
```

---
## \#98 Posted by: Sapphirinia Posted at: 2017-07-16T21:40:00.339Z Reads: 327

```
Not moving. It's vibrated before though
```

---
## \#99 Posted by: Sapphirinia Posted at: 2017-07-28T03:28:05.198Z Reads: 334

```
I killed one of my batteries so I ordered some more. Should get a bit more range out of them too when I get it working again. I'm curious if my servo connection is correct though. I left my board sitting for about a week with the batteries hooked up and the Watt meter was lit the whole time and now 2 of the cells are dead. Can I still try to get the vesc settings to work with one battery until my order gets here? I really need to get this thing working again.
```

---
## \#100 Posted by: mmaner Posted at: 2017-07-28T03:38:11.997Z Reads: 321

```
Is it a 3s or 4s lipo?  If so, yep.
```

---
## \#101 Posted by: Sapphirinia Posted at: 2017-07-28T04:29:46.784Z Reads: 302

```
The working battery I have is 6s
```

---
## \#102 Posted by: mmaner Posted at: 2017-07-28T11:56:14.427Z Reads: 299

```
Your fine, you can config and run a vesc on 6s.
```

---
## \#103 Posted by: Sapphirinia Posted at: 2017-07-28T16:35:42.612Z Reads: 313

```
Thanks for your help. I'm working on fixing it right now. What I've noticed, is that when I manually spin each hub, one vibrates like usual both ways, but the other only vibrates if I spin it in one direction. Is anyone available to sort of walk me through what I'm trying? especially with the BLDC. I'm trying to change so much. I still have lights on both VESCs, receiver light is solid, not sure what's wrong. I'll resolder everything again if I have to but it seems like everything is hooked up properly. Also, I read about split servo connections needing one center wire cut. Mine is not like that and it worked properly before so any suggestions on that?
```

---
## \#104 Posted by: Sapphirinia Posted at: 2017-07-28T17:40:25.584Z Reads: 341

```
Looks like the new VESC is the issue. Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : -0.1
Voltage          : 24.86
Duty             : 0.01
RPM              : 0.1
Tacho            : 3
Cycles running   : 4
TIM duty         : 410
TIM val samp     : 205
TIM current samp : 25682
TIM top          : 50955
Comm step        : 4
Temperature      : 29.44

Fault            : FAULT_CODE_DRV8302
Current          : -0.0
Current filtered : -0.2
Voltage          : 24.87
Duty             : 0.02
RPM              : 0.1
Tacho            : 4
Cycles running   : 3
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 5
Temperature      : 29.52

Fault            : FAULT_CODE_DRV8302
Current          : 0.1
Current filtered : 0.0
Voltage          : 24.87
Duty             : 0.01
RPM              : 1.0
Tacho            : 5
Cycles running   : 4
TIM duty         : 554
TIM val samp     : 277
TIM current samp : 24859
TIM top          : 49165
Comm step        : 6
Temperature      : 29.54
```

---
## \#105 Posted by: Sapphirinia Posted at: 2017-09-11T01:43:30.540Z Reads: 326

```
My temporary band-aid. Thanks to @akhlut. The amount of stuff that's gone wrong is insane! Lol
<img src="/uploads/db1493/original/3X/a/3/a362584431ca0e62a9168b9f5837ca99e14015d1.jpg" width="690" height="441">
```

---
## \#106 Posted by: hornet90 Posted at: 2017-09-11T05:24:45.193Z Reads: 317

```
Hi drv fault needs to be send off and replaced..
Where you running foc or u u think 2 wires might have touched......
```

---
## \#107 Posted by: Sapphirinia Posted at: 2017-09-11T18:58:41.761Z Reads: 306

```
One vesc was unfixable but @akhlut fixed 2 of them for me
```

---
## \#108 Posted by: hornet90 Posted at: 2017-09-11T19:00:53.649Z Reads: 307

```
Do you know how you blew them
```

---
## \#109 Posted by: Sapphirinia Posted at: 2017-09-11T19:58:45.209Z Reads: 301

```
I wish I knew. But they were from Alextech who notoriously sells junk on here. He's been banned at this point though.
```

---
## \#110 Posted by: hornet90 Posted at: 2017-09-12T04:19:44.782Z Reads: 294

```
What are you putting back in are they the same ones or have you to get new ones..........
```

---
## \#111 Posted by: Eboosted Posted at: 2017-09-12T05:36:39.646Z Reads: 299

```
Get a couple of Focboxes and forget all those issues, the Focbox has some kind of thermal switch that protects the DRV.

You need to show us everything on pictures from the vesc programing screenshots until the soldering  jobs, we might be able to keep you from. Blowing more things
```

---
## \#112 Posted by: Sapphirinia Posted at: 2017-09-12T13:41:22.674Z Reads: 305

```
They've been improved. <img src="/uploads/db1493/original/3X/8/9/896a268c67b27eded41074aa666da52ecee00bb9.jpg" width="374" height="500">
```

---
## \#113 Posted by: akhlut Posted at: 2017-09-12T13:48:07.533Z Reads: 299

```
I need to get some time with that deck and a pair of calipers to measure it for a new enclosure.  I really like the pan, but all the gaps between it and the deck throw my ocd into overdrive.
```

---
## \#114 Posted by: hornet90 Posted at: 2017-09-12T18:46:20.785Z Reads: 283

```
Baking tins are great so handy to pick up every store has them......you dont always get the size u want but for10 to 15 euros there great
```

---
## \#115 Posted by: Sapphirinia Posted at: 2017-09-15T00:42:48.658Z Reads: 283

```
I'm using a 99 cent one from the thrift store lol
```

---
## \#116 Posted by: Sapphirinia Posted at: 2017-09-18T11:24:02.049Z Reads: 291

```
So close
<img src="/uploads/db1493/original/3X/9/2/9208f2e1ecb7ec77d442f18227abf4933ee68991.jpg" width="326" height="500">
```

---
## \#117 Posted by: Clonkex Posted at: 2017-09-18T11:24:07.179Z Reads: 294

```
Dang you've just had the worst of luck! :( So far the worst that's happened to me is my controller got switched on by accident and the battery went below safe lipo discharge voltage because I had no protection circuit. Entirely on me of course, rather annoyed at myself :P

I really hope you find some more success after all you've gone through so far! That board looks pretty sick though, love the purple grip.
```

---
## \#118 Posted by: Sapphirinia Posted at: 2017-09-18T17:02:14.578Z Reads: 296

```
I kinda want to get the bumper guards for my board. Grip tape sucks on pennys. Any recommendations? My board is sexier now but I took it on the naked bike ride and got body painted and it got on the board.  <img src="/uploads/db1493/original/3X/7/b/7b63b58913656699ea2e5d6bef767461bb10453b.jpg" width="666" height="500">
```

---
## \#119 Posted by: anorak234 Posted at: 2017-09-18T19:24:40.829Z Reads: 291

```
That looks like a great travel board! I'd say go with the paint thing and make it look like a tie-die thing on the grip
```

---
## \#120 Posted by: Vieo Posted at: 2017-09-19T07:35:39.248Z Reads: 286

```
You could try a wooden Penny board clone, what wheels are they? they look nice
```

---
## \#121 Posted by: Sapphirinia Posted at: 2017-09-20T14:30:50.832Z Reads: 277

```
They are zombie hawgs wheels. They are awesome. I love the snazzy patterns on penny boards though
```

---
## \#122 Posted by: Sapphirinia Posted at: 2017-09-20T14:31:50.097Z Reads: 281

```
So... I finally got the mount to fit the new motor but it's not spinning. It's not doing anything when I hit the trigger. It worked before I got it on the motor mount... Somebody shoot me...
```

---
## \#123 Posted by: faithfulpuppy Posted at: 2017-09-20T14:46:20.894Z Reads: 283

```
Is the new mount significantly thinner than the old one? It could be that one of your screws is reaching the stator and shorting a coil. If that's the case the fix is to get shorter screws or cut/sand your short
```

---
## \#124 Posted by: Sapphirinia Posted at: 2017-09-20T17:07:26.238Z Reads: 265

```
No, I realized it's the controller settings. I started the wizard and it started spazzing. But the motor does work. Just can't get it to work with the controller. I had to go but I'll try more stuff with it later
```

---
## \#125 Posted by: Sapphirinia Posted at: 2017-09-26T03:41:01.287Z Reads: 269

```
Ok, so now my controller isn't working. It powers on but it won't bind to the transmitter. I've changed the batteries and tried on 2 different transmitters. So then I took out the old big one and it bonded but it's got so many settings on it that I'm not sure how to get it to work normal. It was spazzing out the motor and I redid the settings multiple times until I gave up. Why would the controller randomly stop working right? It worked when I was testing it in the street, I packed it up and tried it the next day and it wasn't connecting. I thought it might be the motor but motor detection was fine. Ugh...
```

---
## \#126 Posted by: scepterr Posted at: 2017-09-26T04:04:27.464Z Reads: 285

```
Not sure if this will suit your needs but it's quite durable, at www.hi5ber.com  <img src="/uploads/db1493/original/3X/d/c/dc7d2ed98734cbbe4e42168817a3d443e8a9e05b.jpg" width="281" height="500">
It's metal lined
<img src="/uploads/db1493/original/3X/c/c/cce6cb279cc533307aad45708efb0f6c1abfb34d.jpg" width="375" height="499"><img src="/uploads/db1493/original/3X/6/1/617ed2b74f83c72cd5328d2a4a2fc676e61b661b.jpg" width="375" height="499">
```

---
## \#127 Posted by: Sapphirinia Posted at: 2017-09-26T04:10:08.154Z Reads: 268

```
Nice, just ordered it. Great price too
```

---
## \#128 Posted by: scepterr Posted at: 2017-09-26T04:14:56.293Z Reads: 261

```
Yep got 6 ft headed my way, my deck came with nose and tail preinstalled I'm gonna wrap the entire deck and integrate EL string
```

---
## \#129 Posted by: Sapphirinia Posted at: 2017-09-26T22:05:35.056Z Reads: 268

```
Still can't get either remote to move the board. I can use the arrow keys in the vesc tool to properly control the motor but not with the remote. Any specific settings I should check?
```

---
## \#130 Posted by: Sapphirinia Posted at: 2017-09-27T02:28:29.012Z Reads: 275

```
So here's "Pain" with everything working but the remote. So close. I really wanted to joyride for my birthday. Oh well. <img src="/uploads/db1493/original/3X/3/0/30b7054e838b07b9a5ca155cc0c8fdd81d71e559.jpg" width="672" height="500"><img src="/uploads/db1493/original/3X/a/5/a55b4c5182c41b1db26c341cfbbcdbc50dac9885.jpg" width="570" height="500">
```

---
## \#131 Posted by: BigBoyToys Posted at: 2017-09-27T02:48:41.907Z Reads: 263

```
[quote="Sapphirinia, post:118, topic:17387"]
I took it on the naked bike ride and got body painted and it got on the board.
[/quote]

Pics or It didnt happen 🤣😂😅....jk but not really.

Which remote are u using? Ive got an extra winning that Ill give you if you pay for shipping.
```

---
## \#132 Posted by: pat.speed Posted at: 2017-09-27T02:53:21.301Z Reads: 262

```
@JLabs might be a good place for a new remote. I've heard he has really fast shipping
```

---
## \#133 Posted by: Sapphirinia Posted at: 2017-09-27T03:09:14.925Z Reads: 271

```
<img src="/uploads/db1493/original/3X/2/9/290a0b9d64fdc6066caecda1467b515380b2947d.jpg" width="499" height="500">
```

---
## \#134 Posted by: Sapphirinia Posted at: 2017-09-27T03:11:05.268Z Reads: 263

```
I'd do that. Is it with the receiver too?
```

---
## \#135 Posted by: Sapphirinia Posted at: 2017-09-27T03:14:12.651Z Reads: 262

```
Free is better than not free so I think I'd like to take @BigBoyToys up on his offer. Thanks though. Everywhere I was looking had either too high price or too long to ship. I've dumped way too much money into this board
```

---
## \#136 Posted by: BigBoyToys Posted at: 2017-09-27T03:21:00.788Z Reads: 269

```
👌🙈

Yeah receiver included. Just PM me where youd like them sent. I admire your persistence, 🤞u catch a break after this and get a few hundred miles at least before something goes wrong.
```

---
## \#137 Posted by: Sapphirinia Posted at: 2017-09-29T17:37:10.301Z Reads: 263

```
FML! I went to charge my batteries and this happened. I don't even know what went wrong. Grr 😡<img src="/uploads/db1493/original/3X/6/7/67536e5e3fdfab528d528ea0c2121c3eb5272d81.jpg" width="666" height="500">
```

---
## \#138 Posted by: SORRENTINO Posted at: 2017-09-29T18:06:14.918Z Reads: 260

```
I tell you what went wrong. Your packs were extremely out of balance of each other and when you connected both packs the pack with higher voltage tried to balance out instantly with your lower voltage pack sending a ton of current through your balance wires. Thats probably what happened. Did you connect the xt60s first and let the packs balance between each other for a few minutes? Did you check voltage of each pack before hooking it up to a parallel board? :grinning:
You're lucky you didnt burn your place down. Parallel boards should not be used at all imo. It looks like you have a imax b6 charger and you dont gain anything by parallel charging your batteries with that low watt charger.
```

---
## \#139 Posted by: SORRENTINO Posted at: 2017-09-29T18:16:35.614Z Reads: 249

```
let me rephrase that. Parallel boards should only be used on good cell packs with similar IR in each pack.
```

---
## \#140 Posted by: Sapphirinia Posted at: 2017-09-29T18:31:23.796Z Reads: 253

```
I didn't even turn it on at the point. Soon as I plugged in the 2nd one they start smoking. I've charged them that way once before. I did plug the xt60s in before the balance connectors. Thanks for letting me know what went wrong. Batteries are probably done now right?
```

---
## \#141 Posted by: scepterr Posted at: 2017-09-29T18:34:30.254Z Reads: 247

```
I would check their internal resistance with a multimeter, they are probably fine just need new connectors.
If it was just a few seconds, I doubt there will be any noticeable damage to the cells themselves
```

---
## \#142 Posted by: SORRENTINO Posted at: 2017-09-29T18:38:00.670Z Reads: 250

```
Yeah, You should always check the pack voltage of each pack before plugging them into the parallel board. If they are way off you should charge the lower one up to the voltage of the higher one. If they are slightly off plugging in only the main connector and letting them sit like that for a few minutes should allow the packs to balance each other out and then you can connect the balance connectors. It was either that or you have a short somewhere in the parallel board.
```

---
## \#143 Posted by: pat.speed Posted at: 2017-09-29T23:08:38.584Z Reads: 248

```
The battery's should be fine since the small wires would have fried almost instantly, which would mean the batteries would only have been shorted for less than a second
```

---
## \#144 Posted by: AlexanderTheGrave Posted at: 2017-10-10T20:58:36.963Z Reads: 242

```
I'm starting to vaguely look into trying to build an electric nickel and I'm curious about how you mounted the motor to the nickel trucks after the hub motors gave out. Could you post more pictures showing the mount you used and how (or if) it fits around the triangular piece of the nickel truck (where the logo is).
```

---
## \#145 Posted by: Sapphirinia Posted at: 2017-10-14T17:20:04.322Z Reads: 269

```
Sorry for taking so long. I drew out the shape and cut it out of sheet steel manually. It took forever and I still had to make adjustments to get the right belt tension. I still want to just buy one of those cheap ebay motor mounts. There are sets with the belt, pulleys, and motor mounts for smaller wheels. I believe the set I got was for 70/73mm wheels. I got the one without the motor mount thinking it would be better to just make it custom. In retrospect, I believe it would've been easier to just cut out that notch on a premade mount. I basically used a hand saw, drill press, and dremel. It took me a few days to hack away into the right shape, then I epoxied it to the truck with the strongest kind. It won't budge now. I did a lot of the adjusting for the belt after I had already epoxied it and it never moved.<img src="/uploads/db1493/original/3X/a/b/ab39f6460f8e58840d12430c9b9fb011c75eea18.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/c/6/c677f1aa7199abe331856ddeff7c60b2bb5d0944.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/9/2/9208f2e1ecb7ec77d442f18227abf4933ee68991.jpg" width="326" height="500">
```

---
## \#146 Posted by: Sapphirinia Posted at: 2017-10-14T17:23:02.622Z Reads: 264

```
<img src="/uploads/db1493/original/3X/2/f/2fc367f37e39757bfe8d3d297d03dfa490a24b4a.jpg" width="666" height="500">
```

---
## \#147 Posted by: Sapphirinia Posted at: 2017-10-23T12:57:41.583Z Reads: 251

```
I have a little issue with the bumper coming off. Did you do anything to make it stay better?
```

---
## \#148 Posted by: Sapphirinia Posted at: 2017-10-23T16:42:30.438Z Reads: 257

```
UPDATED PARTS LIST:

Spike 27" penny board- $95
Diy Vesc (beefed up) -  $100
Turnigy 5000mAh 4S1P hard case x2- $50
Sk3 260kv motor- $60
Belt Pulley set- $13
Purple grip tape - $10
Zombie Hawgs 76mm wheels - $50
Sheet steel- $7
Baking tin enclosure- $0.99
Used penny bearings that came with board
Screws and bolts - $10
Button- $10
Locktight, epoxy and such- $15
Connectors: $10
Voltmeter $16

The amount of money I've wasted on parts that have broke? I don't even want to touch that. Please learn from my mistakes young grasshoppers.
```

---
## \#149 Posted by: scepterr Posted at: 2017-10-23T18:01:14.871Z Reads: 249

```
A dab of silicone inside the guard, tape or clamp it down, let it set and all good
```

---
## \#150 Posted by: Sapphirinia Posted at: 2017-10-24T16:53:01.702Z Reads: 259

```
Getting her hair did
<img src="/uploads/db1493/original/3X/d/d/dd9a74ee71f49a57d210b77b22381e6d2e30b681.jpg" width="666" height="500">
```

---
## \#151 Posted by: Sapphirinia Posted at: 2017-10-25T13:55:20.897Z Reads: 254

```
My face is important haha
<img src="/uploads/db1493/original/3X/f/0/f0d3a79cf31c90d1b333436e4f8158b431fb35f0.jpg" width="456" height="500">
```

---
## \#152 Posted by: Sapphirinia Posted at: 2017-10-26T12:55:40.739Z Reads: 250

```
Check out my Instagram if you want to see some of the other cool stuff I'm up to. I am a saxophonist, producer, and dj. My crazy kids make some appearances as well.

Kaylajazzmin
```

---
## \#153 Posted by: Sapphirinia Posted at: 2017-10-26T13:57:42.873Z Reads: 254

```
<img src="/uploads/db1493/original/3X/2/0/20e8ae522f90f768da9bdbd5dc5fa4d511a20b7d.png" width="243" height="500">

<img src="/uploads/db1493/original/3X/3/0/3057c89b76c9e6d0bcca181fbbadca56219ec3e7.png" width="643" height="500">

That's the fastest I could go without speed wobbles. Pretty satisfied at this point. But I'm using dangerous batteries still. Got me up all the hills that my hubs couldn't get me up no problem.
```

---
## \#154 Posted by: AlexanderTheGrave Posted at: 2017-10-26T14:45:16.736Z Reads: 235

```
Do you use risers with your board/ Do you ever have any problems with wheelbite using the zombie hawgs wheels? I know they're a fair bit bigger than the normal penny wheels.
```

---
## \#155 Posted by: Sapphirinia Posted at: 2017-10-26T16:28:55.876Z Reads: 232

```
Not at all. There is plenty of clearance. I could go bigger.
```

---
## \#156 Posted by: AlexanderTheGrave Posted at: 2017-10-26T16:38:06.324Z Reads: 237

```
Thank you! I really appreciate you documenting your build! So far it's been really helpful with the planning of mine!
```

---
## \#157 Posted by: Sapphirinia Posted at: 2017-10-26T17:01:50.659Z Reads: 240

```
Yea, I wish I would've done it the way it is now from the beginning lol. Glad I could help
```

---
## \#158 Posted by: Acido Posted at: 2017-10-26T18:45:25.126Z Reads: 243

```
I hate penny boards!!!
I seriously do not know what do you like about them
Anything under 36inch is not for me, i never liked skateboards but im a huge fan of flex longboards i had a custom made flexible board 44inch but it got stolen
```

---
## \#159 Posted by: Sapphirinia Posted at: 2017-10-27T00:47:00.449Z Reads: 247

```
I think they're awesome and much more convenient when you're using it as a last mile vehicle. I wouldn't want to lug a huge board when I get to my destination.

https://youtu.be/MMFC8vi9Ifk
```

---
## \#160 Posted by: thisguyhere Posted at: 2017-10-27T03:31:52.639Z Reads: 242

```
ur whole youtube channel is your esk8, nice
```

---
## \#161 Posted by: Sapphirinia Posted at: 2017-10-27T03:39:07.291Z Reads: 249

```
Yea, my main one is all my music stuff. That was the one Google forced me to get when they took over YouTube. But I wanted all my views and stuff so I kept both. Might as well make it eskate stuff. 

https://youtu.be/O_8PUDuX6DE
```

---
## \#162 Posted by: thisguyhere Posted at: 2017-10-27T03:42:09.183Z Reads: 243

```
damn ur a really good musician.

sennheiser 650hd?
```

---
## \#163 Posted by: Sapphirinia Posted at: 2017-10-27T03:48:46.633Z Reads: 232

```
HD 600. I like them for when I'm checking levels of tracks. I shouldn't use them while recording though. I really don't care too much for my youtube videos. Thanks for watching.
```

---
## \#164 Posted by: GJHS Posted at: 2017-10-27T04:06:50.057Z Reads: 234

```
Sounds great! Mindi Abair watch out
```

---
## \#165 Posted by: Lambjr088 Posted at: 2017-10-27T04:48:43.213Z Reads: 253

```
I've showed your progress to my wife @Sapphirinia she is inspired that you ride with a penny board she has a scooter and soon a longboard. She is afraid of the longboard but she finds it inspiring to see someone else trying lol
<img src="/uploads/db1493/original/3X/d/5/d5aed4d7166c6d24c817851ee39176446a3473d8.jpg" width="281" height="500">
```

---
## \#166 Posted by: Sapphirinia Posted at: 2017-11-13T01:08:33.887Z Reads: 245

```
Random post, but I didn't know where to put it lol. In my broken-boardness, I went on a philly group ride and someone leg me use their inboard and boosted board. I hated the braking on the inboard so he let me use the boosted for the rest of the time. I definitely preferred it. One of the guys had a diy board but unfortunately, it kept stopping so he had to leave the group ride. It really opened my eyes to the security in knowing you have a dependable board. Like the price point is basically justified after seeing how much went into how it was put together. I still am anti-longboard because sharp turns were pretty much impossible for me, unlike my penny with a kick tail. But it does at least make me more interested in the pre-built ones. I'm no where near being able to afford one but I can't bash those guys much anymore for spending so much on their boards. 

My perfect board would probably be a combination of the two. Color and size of my penny, but with rock solid parts. I didn't like the way you had to hold down 2 separate things on the remotes to go, and with my braking difficulty I actually had the board fly behind me since I forgot it had reverse. Of course there was also the carefully planned charge breaks that I wouldn't deal with my board though. But I'm a vet and it was veterans day so we had a good time going to IHOP and getting my freebies lol.

Glad I finally got to do my first group ride, even if it wasn't on my board. I think it gave me some more motivation to get my board up and running again. I was seriously depressed about my board lol. Didn't want to look at it.

I shouldve started this post with "dear diary" haha 😂
```

---
## \#167 Posted by: b264 Posted at: 2017-11-13T01:15:56.337Z Reads: 236

```
[quote="Sapphirinia, post:166, topic:17387"]
Color and size of my penny, but with rock solid parts
[/quote]

I actually love the metroboard [shortboard](https://imgur.com/a/F6iQQ) and it's built like a tank; I can't see it ever breaking.  Especially with 107mm wheels on it :heart_eyes:  Tacking it around with the kicktails is a beautiful thing.  I often find myself taking this board out instead of a longboard if I'm not going too far.
```

---
## \#168 Posted by: Sapphirinia Posted at: 2017-11-13T02:01:38.012Z Reads: 244

```
This one? It's pretty ugly. Specs are perfect for me though.  <img src="/uploads/db1493/original/3X/a/f/af227aff662e9a806e28f944e81a104a18c5c909.jpg" width="390" height="500">
```

---
## \#169 Posted by: ATLesk8 Posted at: 2017-11-13T02:28:50.704Z Reads: 240

```
Beauty is certainly in the eye of the beholder. I have swapped my deck on mine and I think it looks awesome, but really the only thing you should be worried about is it's reliability...didn't realize aesthetic is what you're after<img src="/uploads/db1493/original/3X/f/7/f7decdc656425c97c51eed66b16918c50662b863.jpg" width="580" height="500">
```

---
## \#170 Posted by: Sapphirinia Posted at: 2017-11-13T02:36:52.432Z Reads: 234

```
I just think the stuff underneath makes it look pretty bulky. Looks really high off the ground too. I'm sure it rides great though. I'm after aesthetics and reliability. Also at least 18mph max speed and 10 mile range. I think the next version up is more of my style. The mid size one.
```

---
## \#171 Posted by: PXSS Posted at: 2017-11-13T02:49:48.770Z Reads: 230

```
Are you still using hubs???

I love the look of your build btw!
Is it still getting fixed?
```

---
## \#172 Posted by: b264 Posted at: 2017-11-13T02:50:46.576Z Reads: 236

```
[quote="Sapphirinia, post:168, topic:17387"]
This one? It's pretty ugly. Specs are perfect for me though.
[/quote]

Yes, that one.  The photo from @ATLesk8 is the older version.  It is ugly as all get-out, but it's still my favourite board because everything else makes up for it.  It's light and has a handle and dual kicktails... and reliability...
```

---
## \#173 Posted by: ATLesk8 Posted at: 2017-11-13T02:52:59.732Z Reads: 240

```
<img src="/uploads/db1493/original/3X/a/d/adb0301977bb9ec311933f8b81a317ec61f94299.jpg" width="690" height="453">

Not so ugly when you can't see her naughty bits
```

---
## \#174 Posted by: scepterr Posted at: 2017-11-13T02:57:26.893Z Reads: 241

```
This might be an option
<img src="/uploads/db1493/original/3X/b/d/bdefc91410a35066d9053fcc590a885196d763ac.jpg" width="690" height="333">
<img src="/uploads/db1493/original/3X/a/7/a7cc90274a753abec4a1636b67cfe4d029c6d531.jpg" width="690" height="230">
<img src="/uploads/db1493/original/3X/5/7/57224c5566798b05cfe02f422ba983d34474cd48.jpg" width="375" height="499">
```

---
## \#175 Posted by: UniqueSnowflakeN27 Posted at: 2017-11-13T15:53:57.866Z Reads: 234

```
[quote="Sapphirinia, post:166, topic:17387"]
It really opened my eyes to the security in knowing you have a dependable board.
[/quote]

Haha this is the same argument I use AGAINST pre-built boards. That guy probably walked home knowing it was one of X numbers of things that was wrong with it and can fix it before the day is over. Personally I'd rather go through that process than having to ship my board back to the manufacturer and be without it for a week or more. If the warranty would still be in effect, that is.

Pre-built definitely has a (big) place in ESK8, but unless I get a good deal it's just not for me.
```

---
## \#176 Posted by: michichopf Posted at: 2017-11-13T16:43:28.916Z Reads: 224

```
Yeah, I also feel like that this is a subjective reasoning to come to this conclusion. Inn our group of 12 poeple +, there are 3 poeple who exlusively ride prebuilts, myself included. And so far none of us 3 had any issues. (some toock our boards to grouprides on their maidennn voyage, some belts where loos or a mount but overall diy have been super reliable in my experience.)

I ride mine daily, to commute to uni and back, twice per day. Total of 25-30km a day, around (20 days a month - 6 days cuz of weather) 385 km / month. ( not couting group rides, joy rides or late night meet ups) and the only issue I had once was a belt being to loose.
```

---
## \#177 Posted by: UniqueSnowflakeN27 Posted at: 2017-11-13T17:23:20.433Z Reads: 223

```
Yeah, agreed. But after following @Sapphirinia's build log I can totally understand her reasoning though. She's had an incredible amount of bad luck!
```

---
## \#178 Posted by: michichopf Posted at: 2017-11-13T17:25:52.686Z Reads: 216

```
yeah, its a bummer for sure :(
```

---
## \#179 Posted by: longhairedboy Posted at: 2017-11-13T17:32:29.686Z Reads: 224

```
10 out of 10 and also the clear winner in Best Use of Muffin Pan.
```

---
## \#180 Posted by: Sapphirinia Posted at: 2017-11-13T18:19:50.515Z Reads: 228

```
No longer using hubs but I do eventually want to fix them. And thanks, I'm definitely hooked on the way it looks. Still working on it. I have a lot of ideas but I need to make it dependable first. (lights, better fitting/looking enclosure, even if it's just modifying the current one, sleeker remote, 18650 battery pack).
```

---
## \#181 Posted by: Sapphirinia Posted at: 2017-11-16T13:42:49.444Z Reads: 231

```
<img src="/uploads/db1493/original/3X/9/f/9fe1cfc8a890839405641e6f3464027086550802.jpg" width="375" height="500">

I kind of messed it up, did it free hand and couldn't erase, but I still think it looks cool.
```

---
## \#182 Posted by: scepterr Posted at: 2017-11-17T02:14:10.965Z Reads: 236

```
This will be able to clean or erase anything off grip tape

https://www.amazon.com/Skateboard-Longboard-Sandpaper-Replace-Cleaning/dp/B07216SCB9/
```

---
## \#183 Posted by: GrecoMan Posted at: 2017-11-17T02:59:11.090Z Reads: 223

```
OH MY GOD! price is $6.66 skatan will consume your soul if you buy
```

---
## \#184 Posted by: b264 Posted at: 2017-11-17T04:31:01.564Z Reads: 229

```
[quote="GrecoMan, post:183, topic:17387, full:true"]
OH MY [diety]! price is $6.66 skatan will consume your soul if you buy
[/quote]

**skatan** ??  Ha ha ha ha

That must be the nemesis of Flying Spaghetti Monster LoLz rofl lmao
```

---
## \#185 Posted by: paulus_germanus Posted at: 2017-11-26T17:02:09.293Z Reads: 228

```
## **All hail Skatan!**
<img src="/uploads/db1493/original/3X/b/e/bed0f0d9e86e20e8af52f011e451cd60e7c5ba53.jpg" width="500" height="500">
```

---
## \#186 Posted by: Sapphirinia Posted at: 2017-12-18T04:27:57.536Z Reads: 227

```
I'm not sure if I can say who donated this to me but either way, I am forever grateful. 🙏🏾

<img src="/uploads/db1493/original/3X/c/3/c3e9e24d989b6c98e5123e5474d52477e1e5277e.JPG" width="690" height="461">

<img src="/uploads/db1493/original/3X/7/d/7d220c8d4f114f40bb42a6d2e03cd589f270cde2.JPG" width="690" height="461">
```

---
## \#187 Posted by: SeanHacker Posted at: 2017-12-18T04:35:47.227Z Reads: 220

```
That's awesome!
```

---
## \#188 Posted by: b264 Posted at: 2017-12-18T05:16:16.559Z Reads: 214

```
Love the cakepan enclosure :heart:
```

---
## \#189 Posted by: akhlut Posted at: 2017-12-18T12:40:16.231Z Reads: 210

```
Wow!  Awesome gift!
```

---
## \#190 Posted by: XvDarkVAngelvX Posted at: 2017-12-18T14:29:49.038Z Reads: 215

```
A lovely Happy ESK8 Merry Christmas Gift.😀
```

---
## \#191 Posted by: Grozniy Posted at: 2017-12-18T14:57:23.179Z Reads: 213

```
so somebody gifted you 600$+ ? wow that's awesome. this forum is full of great people and we don't even know each other ehehe
```

---
## \#192 Posted by: anorak234 Posted at: 2017-12-18T15:08:20.428Z Reads: 211

```
[quote="Grozniy, post:191, topic:17387"]
this forum is full of great people and we don't even know each other ehehe
[/quote]
Hence why we should have an esk8 convention. When I’m rich and famous that will be #1 priority :smile:
```

---
## \#193 Posted by: Sapphirinia Posted at: 2017-12-19T20:35:21.736Z Reads: 201

```
I rode my whole commute today on the way back instead of taking trains and it was awesome. I gotta do some video of it tomorrow. Went over the bridge too.
```

---
## \#194 Posted by: Rob69de Posted at: 2017-12-19T22:13:37.900Z Reads: 207

```
Awesome: 😎 people helping those in need..
```

---
## \#195 Posted by: Sapphirinia Posted at: 2017-12-27T04:54:20.308Z Reads: 212

```
Still a work in progress but I wound up frying my dremel in the process of chopping up the board.
I was trying to cut handles too. That's where it sparked and died. I managed to get the weight down some.  <img src="/uploads/db1493/original/3X/2/2/22a0ab3adec36f499400d4a1417e1ede0792aa83.jpg" width="374" height="500">
```

---
## \#196 Posted by: Mikenopolis Posted at: 2017-12-27T05:04:16.892Z Reads: 205

```
Nice to see you decided to use my belt idea!

You are planning to cut a handle into the deck?  Might I suggest you checking hardware stores for kitchen drawer handles?
```

---
## \#197 Posted by: Rob69de Posted at: 2017-12-27T14:15:10.916Z Reads: 199

```
You changed the deck? 
If so looks good shorter, still think a jet spud work work well for you.
```

---
## \#198 Posted by: Sapphirinia Posted at: 2017-12-27T17:45:08.974Z Reads: 199

```
Changed the deck. Didn't want to chop up the gifted one. Thanks
```

---
## \#199 Posted by: Sapphirinia Posted at: 2017-12-27T17:46:33.032Z Reads: 206

```
I want to make the deck lighter so I'd rather cut than add. Belt idea was awesome since I didn't have to buy anything. Besides cheap screws and bolts
```

---
## \#200 Posted by: Sapphirinia Posted at: 2017-12-27T17:57:20.600Z Reads: 210

```
Just looked at the jet spud. That would've been perfect as well. This one was a bit cheaper though. On sale at zumiez. Perhaps in the future. I was also looking at this one. It has a kick tail and it has the perfect wheelbase. <img src="/uploads/db1493/original/3X/9/f/9f0260d2a405d9f4afe17b8876be96b99b7da4d2.jpg" width="431" height="500">
```

---
## \#201 Posted by: Sapphirinia Posted at: 2017-12-29T02:03:09.637Z Reads: 203

```
So, hypothetically, if I was to swap out the strong motor on the new board with my old one, what would happen? Like the max I hit while riding the new one during city nav was 17mph. I've hit 18mph on my penny nickel. Would I wind up with a longer battery life and lighter board that way? I'm pretty nervous to change something that's already working but I do have back issues, and my shoulder surgery was a year ago and not yet 100%
```

---
## \#202 Posted by: pennyboard Posted at: 2017-12-29T02:13:54.598Z Reads: 193

```
Well it depends on the power that the smaller motor has, but generally any motor over, say 1000 watts should get you to 18 mph, perhaps just not quickly. 

More important than power, however, is the battery voltage, motor KV, and gearing. If those are different one your small board and big board, then the speed will likely be different. If you post how many cells the battery is on each board, as well as the gearing and motor KV for each board, it'd be possible to calculate your new top speed if you switched motors.
```

---
## \#203 Posted by: Sapphirinia Posted at: 2017-12-29T02:19:18.083Z Reads: 193

```
I was told the new board setup should get me 26mph. I'm sure it does but I don't really need to hit that speed. 20 is probably my max, and only if I was on a well known bike path or something where I didn't have to worry about cars, rocks, cracks, etc. I'll have to ask on the specifics on the battery because it looks to be custom made. It's really heavy lol. I was also looking into lighter wheels. I really like the way these feel but in the future, like maybe tax time 😂 getting something big and light possibly.
```

---
## \#204 Posted by: Sapphirinia Posted at: 2017-12-29T02:21:34.174Z Reads: 208

```
I went overboard with the spray paint 😂😂
I have my sites on a different lighter deck with a kick tail in the future as well. 

<img src="/uploads/db1493/original/3X/d/5/d5a8286ba3bd9b06d6855f0876914ca1288ad59f.jpg" width="690" height="480">
<img src="/uploads/db1493/original/3X/2/3/239a7d8ab80871a54df8024c9795bd6c40a80869.jpg" width="651" height="500">
```

---
## \#205 Posted by: ATLesk8 Posted at: 2017-12-29T02:26:03.104Z Reads: 201

```
It's ermm...beautiful? Eye of the beholder right? I had to say something because you called my metro fat and ugly (which she might be) haha
```

---
## \#206 Posted by: Sapphirinia Posted at: 2017-12-29T02:30:00.495Z Reads: 199

```
It is UGLY! No doubt about it. I sprayed it real fast because it was like 19° outside. Then I tried to fix it with the glitter spray lol. I shouldve just left it how it was. But I have my eyes on a different deck.
```

---
## \#207 Posted by: E1Allen Posted at: 2017-12-29T02:41:06.620Z Reads: 196

```
If you keep the same components and only swap out the deck I can't see you losing that much weight.  I can't imagine much of a performance increase from it.
```

---
## \#208 Posted by: pennyboard Posted at: 2017-12-29T03:01:27.973Z Reads: 197

```
Getting light weight is difficult. At around 11 pounds it starts to get difficult to get any lighter without sacrificing either range, performance, or reliability.
```

---
## \#209 Posted by: paulus_germanus Posted at: 2017-12-29T12:18:42.736Z Reads: 196

```
Ugly? I love it!:heart_eyes_cat:
```

---
## \#210 Posted by: Sapphirinia Posted at: 2017-12-29T23:23:22.789Z Reads: 203

```
Fiberglass/carbon fiber, lightweight. Merry Christmas to me.

 <img src="/uploads/db1493/original/3X/b/2/b2b454d62860a13dd7aeb89a69813552daf9487a.jpg" width="315" height="500">
```

---
## \#211 Posted by: XvDarkVAngelvX Posted at: 2017-12-29T23:33:14.275Z Reads: 196

```
Congratulations and Merry wishes to the new deck. Can't wait to see what you do with it. 😎
```

---
## \#212 Posted by: Hummie Posted at: 2017-12-29T23:46:45.679Z Reads: 199

```
[quote="Sapphirinia, post:201, topic:17387, full:true"]
So, hypothetically, if I was to swap out the strong motor on the new board with my old one, what would happen? Like the max I hit while riding the new one during city nav was 17mph. I've hit 18mph on my penny nickel. Would I wind up with a longer battery life and lighter board that way? I'm pretty nervous to change something that's already working but I do have back issues, and my shoulder surgery was a year ago and not yet 100%
[/quote]

if you put a higher kv motor on it will go faster.  the rated power of the motor barely will effect speed.  power is decided by the battery first (if they can put out the amps and not get hot) and then what the esc is programmed to send to the motor next.  
kv decides torque and speed and the size of the motor will decide if it can sustain it.   

that is a nice looking deck
```

---
## \#213 Posted by: Sapphirinia Posted at: 2017-12-29T23:50:23.463Z Reads: 187

```
Great explanation. Thanks. I love this deck
```

---
## \#214 Posted by: Hummie Posted at: 2017-12-29T23:55:12.268Z Reads: 195

```
but if you had a really small motor then lets say on your full 10s or 12s battery going full speed on the bench lets say you hit 1000rpm, and on the road lets say youre only hitting 700, that would be because the motor is so small and if you increase the motor size but with same kv you could bump it up to getting closer to the 1000 rpm and that could be a big increase in speed.  typically you want a motor that will do about 85% of the no-load speed when in use, and that's an efficient place to be.    so motor size can effect speed even with the same kv.  ..but kv is the real decider.
and you'll get better range with the bigger motor.  more efficient in that it has less internal electrical resistance and also riding closer to that sweet spot of about 85% of whatever voltage is applied.
```

---
## \#215 Posted by: Sapphirinia Posted at: 2017-12-30T00:44:40.840Z Reads: 195

```
Efficiency is guud
```

---
## \#216 Posted by: Sapphirinia Posted at: 2017-12-30T00:46:14.933Z Reads: 201

```
<img src="/uploads/db1493/original/3X/8/9/8944aa5082d01a050d11fed2d49c5f127b908ec1.jpg" width="374" height="500">
```

---
## \#217 Posted by: Sapphirinia Posted at: 2017-12-30T05:11:05.388Z Reads: 201

```
The commute I was trying to post sooner. I have an extremely cheap camera and it took forever to get it to convert to a proper video format. 6 miles stuffed into 20 minutes. Enjoy? :) or not lol. I cross the bridge towards the end. It shows an example of the commute I was talking about. All music is by me.

https://youtu.be/MyYzIy66-Cs
```

---
## \#218 Posted by: Hummie Posted at: 2017-12-30T08:07:57.224Z Reads: 204

```
theres no music.  that's my old neighborhood and I lived all around west philly.  upenn you start and I've been over the bridge to Jersey on the side there, by bike.  thought you were going to go over south street bridge but you go a lot farther.  with no music and no nice camera with a gimbal its hard to watch but if you did those things, and choose the shots better I think, like looking more forward, because I keep twisting my neck to try to see where youre going, then could get through 20minutes happily.
that's pretty funny with the polish on the screws.  very girl I think!
```

---
## \#219 Posted by: Sapphirinia Posted at: 2017-12-30T18:39:21.150Z Reads: 198

```
Thanks for letting me know. I definitely put music on it so I'll have to investigate now. Good to see a fellow philly native. I'm debating on using my phone to record. It has great video/stabilization but I really don't want to accidentally bail and break it.
```

---
## \#220 Posted by: Sapphirinia Posted at: 2017-12-30T21:27:33.085Z Reads: 200

```
https://youtu.be/MyYzIy66-Cs
```

---
## \#221 Posted by: wafflejock Posted at: 2017-12-30T21:46:55.801Z Reads: 196

```
Not sure if you tried any digital image stabilization but YouTube can do it after a video is uploaded (granted stabilization of the raw video in an editor before it gets cut together probably works better adding it through YouTube video edits is pretty hands off, just need to wait forever for it to process)
```

---
## \#222 Posted by: Sapphirinia Posted at: 2017-12-30T22:20:12.889Z Reads: 195

```
I'll try that. I was using Sony movie studio platinum and every time I tried the built-in stabilization it took forever for each 30sec or so clip and then it came out really blurry/fuzzy looking so I put it back to normal. I'll try the YouTube stabilization. I didn't see it. Thanks
```

---
## \#223 Posted by: Sapphirinia Posted at: 2017-12-31T22:45:48.323Z Reads: 197

```
Let me introduce you to the ultimate troll. 
<img src="/uploads/db1493/original/3X/f/4/f411d8b15a76b02426d9dedf5e20fbcbbacca1f4.jpg" width="690" height="476"><img src="/uploads/db1493/original/3X/a/a/aa332e917fa7cf60218272f2f6943491eaa138c0.jpg" width="690" height="467">
```

---
## \#224 Posted by: ATLesk8 Posted at: 2017-12-31T22:59:40.977Z Reads: 191

```
My parents always warned me about flashbacks...bull i thought....they were right
```

---
## \#225 Posted by: Hummie Posted at: 2018-01-01T06:21:46.720Z Reads: 188

```
wow how did you get that print on there?  I assume its a print. I would even take it as is with my little pony or whatever it is!  wow that's something else.
```

---
## \#226 Posted by: Mobutusan Posted at: 2018-01-01T06:36:07.518Z Reads: 189

```
Sweet upgrade. Nice use of rainbows and ponies. Lol. Are you planning to install your foot belt on this deck, or is it too pretty now? If you are, I could probably help a sister out with a slight foot strap upgrade. (Not that I don't like the DIY S&M belt vibe.) 😉
```

---
## \#227 Posted by: Sapphirinia Posted at: 2018-01-01T17:27:21.528Z Reads: 182

```
It's griptape. I couldn't not get it after I saw it in the store lol.
```

---
## \#228 Posted by: Sapphirinia Posted at: 2018-01-01T17:29:22.112Z Reads: 184

```
Thanks. I think it's too pretty for a belt now. It has a kick tail so that's covered. I can turn yay
```

---
## \#229 Posted by: E1Allen Posted at: 2018-01-01T17:50:22.972Z Reads: 180

```
I'd ride that board.  It works!
```

---
## \#230 Posted by: Sapphirinia Posted at: 2018-01-01T17:56:29.533Z Reads: 179

```
Ooh, can I see a picture of yours?
```

---
## \#231 Posted by: E1Allen Posted at: 2018-01-01T18:06:49.672Z Reads: 185

```
<img src="/uploads/db1493/original/3X/3/f/3fd6710bb9ee336c1c2f9b376fc0aaaea2575c21.jpg" width="690" height="388">

Still a work in progress. Waiting on 18650 pack
```

---
## \#232 Posted by: Sapphirinia Posted at: 2018-01-02T02:00:59.594Z Reads: 188

```
I rode a little today in 24°F weather and froze my fingers off. More specifically, my trigger finger. I couldn't bare waiting any longer. I might have to get some of those hot hands things for next time

<img src="/uploads/db1493/original/3X/1/4/141b4620596cccbbf37b9a1fef4ff354c6285a21.jpg" width="494" height="499">
```

---
## \#233 Posted by: Holyman92 Posted at: 2018-01-02T02:04:20.672Z Reads: 187

```
[quote="Sapphirinia, post:1, topic:17387"]
IMG_20170208_100102.jpg1815x1920 1.51 MB
[/quote]

-plays lute-  Reindeer are better than people...
```

---
## \#234 Posted by: Sapphirinia Posted at: 2018-01-02T02:08:36.176Z Reads: 186

```
Actually it was 21° lol
https://youtu.be/_CAm0bppRBY
```

---
## \#235 Posted by: Holyman92 Posted at: 2018-01-02T02:20:22.579Z Reads: 178

```
okay, so i just read from the camera post to here, trying to see if you would mention it again... what is that little thing
```

---
## \#236 Posted by: Sapphirinia Posted at: 2018-01-03T14:17:51.101Z Reads: 178

```
The board?
```

---
## \#237 Posted by: Holyman92 Posted at: 2018-01-03T16:55:02.646Z Reads: 175

```
The camera
```

---
## \#238 Posted by: Sapphirinia Posted at: 2018-01-03T21:51:58.240Z Reads: 181

```
This piece of junk. Took me forever to convert it to a format that Sony Movie Studio could use but I think it was like $15 on black Friday at K-Mart so I guess it was worth it. I had it clipped onto my backpack strap.
https://www.bhphotovideo.com/bnh/controller/home?A=details&O=&Q=&ap=y&c3api=1876%2C%7Bcreative%7D%2C%7Bkeyword%7D&gclid=CjwKCAiAm7LSBRBBEiwAvL1-L0hWyPAO3JV5iAXKHNwmmwRqgl0i9ZHrm5g-f8-_zPawqVs_i_DedBoCQSUQAvD_BwE&is=REG&m=Y&sku=1345152
```

---
## \#239 Posted by: Holyman92 Posted at: 2018-01-03T21:54:08.036Z Reads: 184

```
what format was it in?

not that cam, the naked cam module u had... this 1
<img src="/uploads/db1493/original/3X/a/1/a11e761188816c4d3d41ee902c6863ca79b1533f.png" width="374" height="500">
```

---
## \#240 Posted by: Sapphirinia Posted at: 2018-01-03T23:36:25.711Z Reads: 177

```
https://hobbyking.com/en_us/hd-wing-camera-1280x720p-30fps-5mp-cmos.html

Unfortunately I threw it in my backpack and broke the lens off.
```

---
## \#241 Posted by: Sapphirinia Posted at: 2018-01-03T23:36:57.288Z Reads: 174

```
I break everything :(
```

---
## \#242 Posted by: b264 Posted at: 2018-01-03T23:53:49.252Z Reads: 182

```
[quote="Sapphirinia, post:232, topic:17387"]
I rode a little today in 24°F weather and froze my fingers off. More specifically, my trigger finger.
[/quote]

It was -7°F (-22°C) the other day, it's 22°F (-6°C) right now and freezing trigger finger is a very, very, VERY real thing.  I have found that you have to wear a glove, of course, with the fingertip cut off, but then you put the whole gloved hand with remote in a pocket.  I hope your outer coat has big pockets.  I figured that out after, upon arrival, my finger was numb and blue one night for a lot longer than I was comfortable with...  If my pocket wasn't big enough, I would recommend putting a paper bag over your entire hand and tying it there
```

---
## \#243 Posted by: Sapphirinia Posted at: 2018-01-04T00:15:32.662Z Reads: 176

```
That's friggin cold. Wow. I was looking at heated gloves too. I could probably make something to fit around my hand with the controller though. I had a sewing phase and lots of cloth leftover.
```

---
## \#244 Posted by: Holyman92 Posted at: 2018-01-04T00:17:07.823Z Reads: 179

```
im kinda digging this lil guy https://hobbyking.com/en_us/runcam-split-fpv-camera.html
```

---
## \#245 Posted by: Sapphirinia Posted at: 2018-01-04T07:39:58.687Z Reads: 179

```
So, I couldn't sleep and decided to whip out my sewing machine and make a grip tape cover for my board. It's super awkward to hold still so I wanted to try doing that then using a strap, or holding it regular without scratching up my jacket.

<img src="/uploads/db1493/original/3X/4/9/4970504327b5328fb553ace02f5e020eda7270b8.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/1/414a29f4ad38ddbc579fa73fb6ca5d4055a48058.jpg" width="666" height="500">
```

---
## \#246 Posted by: E1Allen Posted at: 2018-01-04T07:41:58.373Z Reads: 169

```
To big for carrying on a backpack?
```

---
## \#247 Posted by: Sapphirinia Posted at: 2018-01-04T07:53:12.680Z Reads: 169

```
Yea. I keep my backpack pretty much empty for weight reasons and it would be way too slouchy with a board strapped on. It's 34in and kind of heavy
```

---
## \#248 Posted by: E1Allen Posted at: 2018-01-04T08:00:18.974Z Reads: 170

```
Wonder if you could do a strap up front or in back and pull it like a suitcase
```

---
## \#250 Posted by: Sapphirinia Posted at: 2018-01-05T01:09:16.024Z Reads: 175

```
Solution

Just needs a little more padding. 
<img src="/uploads/db1493/original/3X/4/e/4ec8dc4563487a4a93e9eca27faf01d72c2fdd3b.jpg" width="374" height="500">
```

---
## \#251 Posted by: Sapphirinia Posted at: 2018-01-05T04:50:01.915Z Reads: 173

```
Part of my next crazy idea
😉 
<img src="/uploads/db1493/original/3X/9/f/9f76f83369c9198fc348e87171d44b9f3da71278.jpg" width="374" height="500">
```

---
## \#252 Posted by: Hummie Posted at: 2018-01-05T07:39:02.764Z Reads: 170

```
think youre going to get your nice white sweater dirty still..  and all the weight on one shoulder.  id rather have it contained in a backpack with it supported and sticking up high out of it
```

---
## \#253 Posted by: pat.speed Posted at: 2018-01-05T11:55:28.628Z Reads: 167

```
What about straps that clip onto each side of the trucks and you wear it as a back pack?
```

---
## \#254 Posted by: Sapphirinia Posted at: 2018-01-05T15:53:23.796Z Reads: 163

```
There's a griptape cover I made protecting me from the grip.
```

---
## \#255 Posted by: Sapphirinia Posted at: 2018-01-05T15:54:44.290Z Reads: 162

```
I could do that, but I think it would be uncomfortable for my head if it goes straight up and down. I'd rather have it go diagonally across my back.
```

---
## \#256 Posted by: Hummie Posted at: 2018-01-05T15:59:18.145Z Reads: 163

```
but the wheels
```

---
## \#257 Posted by: Sapphirinia Posted at: 2018-01-05T16:00:35.840Z Reads: 168

```
Oh, they face out. I didn't really notice them touching my sweater lol.
```

---
## \#258 Posted by: Sapphirinia Posted at: 2018-01-05T21:11:23.370Z Reads: 171

```
One more part to print. 
<img src="/uploads/db1493/original/3X/b/2/b2c31fe1c2ed581ab1ceea38cab0fe462fde5121.jpg" width="445" height="500">
```

---
## \#259 Posted by: Sapphirinia Posted at: 2018-01-06T18:12:13.439Z Reads: 176

```
<img src="/uploads/db1493/original/3X/8/7/87e367034bca5b1608af9576575ed03f8c5a6f47.jpg" width="568" height="499">
I'm attempting to use inline skate wheels. I've read they're super smooth. Well I used to aggressive  inline anyway. And they're thinner=lighter
```

---
## \#260 Posted by: Sapphirinia Posted at: 2018-01-20T22:23:39.168Z Reads: 173

```
I had my first esk8 crash today. I was doing a philly group ride and some lady cut me off with her car. 😡
https://youtu.be/GIZ2bk04Yqo
![20180120_152151|374x500](upload://wFFRNG9LdK533ZZ32mPSRIl7SLO.jpg)
```

---
## \#261 Posted by: Mobutusan Posted at: 2018-01-20T22:37:03.589Z Reads: 165

```
Aww, Wtf?! Did she stop and give you money? If not, fuck that. Doesn't she know you don't need help breaking stuff? :wink: I kid, I kid. Seriously, it seems like you finally got it all dialed in, then this? Weak. How far down the deck does the damage go? Looks like you might be able to cut the busted nose off and epoxy any loose layers back together. Was there any other damage besides the deck?
```

---
## \#262 Posted by: Caleb1 Posted at: 2018-01-20T22:37:08.010Z Reads: 158

```
You could glue the board layers together and put a bash guard over it
```

---
## \#263 Posted by: Sapphirinia Posted at: 2018-01-20T22:41:20.513Z Reads: 157

```
Luckily the deck went under her moving car through the wheels so it didn't get run over. That's all the damage. Its a fiberglass layer that got peeled back and I can't squeeze it together. I definitely don't need any help breaking stuff lol. Just annoying because I spent $150 on the deck that I shouldn't have spent in the first place. Only rode it probably 4 times so far. I'll probably try to make a 3d printed bumper of some sort. Original Skateboards sells a special bumper for the deck but it doesn't fit after it's already been busted.
```

---
## \#264 Posted by: BigBrit Posted at: 2018-01-20T23:39:16.416Z Reads: 149

```
That looks pretty easy to fix up from the picture.  Get some wood glue and once its glued clamp it up and let it dry
```

---
## \#265 Posted by: koralle Posted at: 2018-01-20T23:41:57.399Z Reads: 152

```
mix the glue  with a little water so it's easier to insert deep into the crack with a knife or similar object. Use multiple Clamps!
```

---
## \#266 Posted by: Sapphirinia Posted at: 2018-01-21T01:10:52.841Z Reads: 150

```
My body hurts 😣
```

---
## \#267 Posted by: akhlut Posted at: 2018-01-21T01:30:51.995Z Reads: 146

```
No brakes?
```

---
## \#268 Posted by: Sapphirinia Posted at: 2018-01-21T01:50:10.182Z Reads: 157

```
She cut me off so fast I couldn't brake fast enough. People don't pay attention. She said she didn't see me. She says she's going to compensate me for the deck so I hope she really does. That deck was basically brand new. I'll get the bumpers for it next time. Unfortunately I'll have to get it regripped. And the price went up on the deck since I caught the Christmas sale.
```

---
## \#269 Posted by: akhlut Posted at: 2018-01-21T02:03:45.280Z Reads: 158

```
Try to adjust the braking curve in the vesc firmware to make them stronger.
```

---
## \#270 Posted by: Sapphirinia Posted at: 2018-01-21T02:15:57.636Z Reads: 163

```
Ok. I haven't adjusted anything since I got the board. If it would've braked hard, I would've still flown off the board.
```

---
## \#271 Posted by: Sapphirinia Posted at: 2018-01-21T04:07:59.681Z Reads: 166

```
Despite it all, today was a good day

![20180120_154805|673x500](upload://mTw2uFxV3FSxEtE7hPy4PyoJPZR.jpg)
![Screenshot_20180120-155549|620x499](upload://4Edjj7FVHfXs84bdm2Wzow6699i.jpg)

We hit higher speeds and went probably 10 miles with a break before the accident,  but I forgot to start up my tracker on my phone until the last few miles.
```

---
## \#272 Posted by: akhlut Posted at: 2018-01-21T04:09:43.044Z Reads: 158

```
2.5 miles?  Where did you go?
```

---
## \#273 Posted by: Sapphirinia Posted at: 2018-01-21T05:08:40.844Z Reads: 158

```
We probably went 10miles.all around center city and south Philly. We saw the woman's March and quickly got out of there lol. Too many people. It was really fun. Accident didn't happen until the end.
```

---
## \#274 Posted by: akhlut Posted at: 2018-01-21T05:19:36.163Z Reads: 151

```
That's better!  Hey, how did those other boards perform compared to yours?  The look like retail stuff.
```

---
## \#275 Posted by: topcloud Posted at: 2018-01-21T05:22:13.256Z Reads: 150

```
[quote="akhlut, post:274, topic:17387"]
how did those other boards perform compared to yours?  The look like retail stuff.
[/quote]

you noticed too ha
```

---
## \#276 Posted by: Sapphirinia Posted at: 2018-01-21T05:23:22.678Z Reads: 148

```
Well the most obvious part is battery life. They had boosted board, inboard, and wowgo. I could've done the whole thing on 1 charge but they needed to charge a few times. I could keep up with them fine but I'm more gentle on the throttle so they would pick up speed faster and when I got comfortable I'd go their speed. At one point t I had to tighten my truck since I started getting speed wobbles. I haven't taken the board past 18mph before that so I'm pretty sure we were hitting 25mph or so before I started tracking. We had some nice long stretches before that.
```

---
## \#277 Posted by: akhlut Posted at: 2018-01-21T05:27:49.732Z Reads: 142

```
Good.  Gotta represent DIY.  Those boosted guys are always on the lookout for an outlet like a meth head looking for a fix.

Also, don't try keeping up with people - ride at your own pace, whatever you're comfortable with.  It's just not worth it - ride within your ability.
```

---
## \#278 Posted by: Sapphirinia Posted at: 2018-01-21T05:40:51.718Z Reads: 147

```
😂😂😂. Well as you know, I use my board mainly to commute. So I rarely need to hit any top speeds. I. Typically brake going downhill. I wasn't even going that fast when that car hit me though lol. Good thing I wasn't.
```

---
## \#279 Posted by: b264 Posted at: 2018-01-21T08:06:35.109Z Reads: 154

```
Almost every time I've crashed it was because I was trying to keep up with [whatever] or trying to rush because [reason].  I stopped doing that.  I recommend riding at your own pace NO MATTER WHAT.  If you're late, you're late, so what.  Better than tripping off the board.  Plus you always have to be vigilant of the cars {aka: death machines} because most people driving can't see people on {skateboard, bicycle, motorcycle, pedestrian}

Car driving becomes instinctual after a while and you stop consciously focusing on it.  People's bodies take over in autopilot mode and their brains are trained to pay attention to where the other cars are at.  Unless they are actively looking for pedestrians or skateboarders or people on bicycles or motorcycles (which they aren't because there is an urgent incoming text message) then you are effectively invisible to them unless you wear a car-sized helmet so their subconscious auto-detection system picks you up

So you have to treat every car like the driver cannot physically see you.  Because often they can't.  Even if you are lit up and in their line-of-sight.



*TL;DR: don't rush -- and treat every car like it's trying to kill you*
```

---
## \#280 Posted by: meesie Posted at: 2018-01-22T12:00:25.916Z Reads: 148

```
DON'T MIX GLUE WITH WATER!

i'm studying woodworking and carpentry and this is one of the most terrible mistakes i've ever made. you're basically watterlogging your longboard whilst also sealing it with glue, which is too thin to really glue anyhting by now. the water will get trapped inside and delaminate your whole deck if you do this.

to get the effect @korralle describes you can use high viscosity resin.
```

---
## \#281 Posted by: koralle Posted at: 2018-01-22T12:14:41.438Z Reads: 143

```
If it is normal good old fashioned white wood glue, it's water based. It doesn't make any difference to the gluing capability if you dilute it with a litte water. I didnt say water it down until theres no glue left. So youre not waterlogging anything. How do you think the water thats normally in the glue gets out? It can dissipate through wood and the glue itself. You studying woodworking makes me a little sceptical tbh :smiley:
```

---
## \#282 Posted by: meesie Posted at: 2018-01-22T22:00:40.856Z Reads: 138

```
A month or two ago a self pressed pintail started delaminating in the rear. A clasmate suggested to dilute the glue with water for the same reason/result (5 parts glue 1 part water.) 
 In the end it did help a little to get it into the cracks, but because the glue on the outside (more exposed to air) dried quicker than the glue on the inside it trapped the moisture inside of the board. 

End result: The tip of the tail held strong, but the the bit behind the tail showed signs of delamination.

Also, my teacher told me that he prefers epoxy resin over regular wood glue for glueing pieces that already have lacquer on it because of the moisture.
```

---
## \#283 Posted by: Sapphirinia Posted at: 2018-01-24T16:37:38.950Z Reads: 139

```
So, the insurance company is writing me a check to replace the board. I'm not sure whether I should get the same one or the slightly drop deck version. I'm using 150mm wheels this time around. Help me decide. Oh, and I will be getting the bumpers in purple. I have to do a new enclosure anyway so I was thinking split fiberglass one. Originally I had the 34" because well smaller equals lighter. But I really loved the 37" because it looked cooler. I wound up not getting it because it was so much more expensive. Now I'm not sure if the slight size difference would matter, plus I don't think the split enclosure would fit right on the 34". Then again, I could still make it a single enclosure lol. 

https://originalskateboards.com/product/apex-37-diamond-drop-deck/

Or

https://originalskateboards.com/product/apex-34-rocker-concave-deck/
```

---
## \#284 Posted by: mmaner Posted at: 2018-01-24T16:43:46.766Z Reads: 130

```
I personally like the drops on the 37 better.  Instead of being a gradual curve these give a place to 'lock in'.
```

---
## \#285 Posted by: Rob69de Posted at: 2018-01-24T16:45:27.393Z Reads: 126

```
Looks like the old board can easily be fixed
Like many have said some Elmer’s wood glue and a clamp
Or something really heavy pressing the split down like a few heavy cinder blocks.
```

---
## \#286 Posted by: Sapphirinia Posted at: 2018-01-24T17:21:57.363Z Reads: 140

```
I'm just going to replace it. I'd rather set it up better this time. I want the bumpers so it doesn't happen again. They're a really tight fit. Also, its not just wood that's separated. It's also the fiberglass. You can see it if you zoom in. I just don't think it'll keep the same quality over time with it split like that. I've gotten less than a month out of it and was hoping to ride it for a long time. Especially since they're supposed to be basically indestructible. They've been run over by trucks on youtube. I don't want to have to worry about it later
```

---
## \#287 Posted by: Sapphirinia Posted at: 2018-01-24T17:57:02.974Z Reads: 138

```
A chunk of the wood got pushed inside so it doesn't look like it would lay flat anyway. 

![20180124_125511|666x500](upload://csDFCSvS0KgS4Csi9YFfpfE4Y7H.jpg)
```

---
## \#288 Posted by: Sapphirinia Posted at: 2018-01-24T18:02:41.964Z Reads: 136

```
I suppose I can donate the busted deck to whoever feels they can fix it and would use it. Just pay shipping. I have to get my new one first though.
```

---
## \#289 Posted by: Mobutusan Posted at: 2018-01-24T18:39:34.571Z Reads: 135

```
I'll take it and fix it up, when you get your new board. That's awesome that insurance is covering it. Thumbs up to the lady that hit you for doing the right thing.
```

---
## \#290 Posted by: Sapphirinia Posted at: 2018-01-24T18:47:25.428Z Reads: 133

```
Where are you located? I just posted in the freebies lol
```

---
## \#291 Posted by: Sapphirinia Posted at: 2018-01-24T18:48:24.405Z Reads: 133

```
The majority of the money is from pain and suffering but they did cover the deck cost and a bit of the labor for me to rebuild it.
```

---
## \#292 Posted by: Mobutusan Posted at: 2018-01-24T19:04:18.210Z Reads: 136

```
I'm in California.
```

---
## \#293 Posted by: Sapphirinia Posted at: 2018-01-27T19:37:36.800Z Reads: 142

```
I'm definitely going to do a drop through setup when I get the replacement deck. This is so high lol. Wheels have clearance. Still lots to do but I think I have the Pulley out of the way for now. I'll have even more space with the 37" deck. It's so rolley lol. I rolled a little on my floor. ![20180127_143204|666x500](upload://80ogaGPh5M1OjA1tWW1HQsJjsAZ.jpg)![20180127_143525|374x500](upload://9RrD3FYlpzrpCJ3JFujjDKOGMK9.jpg)
```

---
## \#294 Posted by: ATLesk8 Posted at: 2018-01-27T23:49:20.198Z Reads: 138

```
I finished a little cruiser spud today. It's a single Carvon with an old vesc I had laying around with a 10s3p pack from @willpark16  . Sorry if it posts upside down I don't know why on mobile ![20180127_155344_HDR|690x388](upload://i4iDSJzGK1JGuGQAs0WHUb68Z5O.jpg)
```

---
## \#295 Posted by: Sapphirinia Posted at: 2018-01-28T00:03:18.576Z Reads: 136

```
Awesome you got a carvon. Good stuff.
```

---
## \#296 Posted by: Sapphirinia Posted at: 2018-01-29T13:16:52.725Z Reads: 129

```
![Screenshot_20180129-080910|251x500](upload://tUQYWHz96Gdpv2ziOUOgUgb28D9.jpg)
```

---
## \#297 Posted by: Sapphirinia Posted at: 2018-01-29T23:42:18.690Z Reads: 126

```
Easiest, safest way to get these batteries out? I'm am stripping my board now and starting tge new hopefully split enclosure for the new deck. ![20180129_183916|485x500](upload://xWnrR8jb0G2DcmwKtHlqFeHUOgf.jpg)
```

---
## \#298 Posted by: meesie Posted at: 2018-01-30T14:29:53.424Z Reads: 122

```
Holy crap! Those are things for racing skates right? How do they compare to “normal” longboard wheels? 

I’m sceptical about those kind of wheels because of their thin profile
```

---
## \#299 Posted by: Sapphirinia Posted at: 2018-01-30T14:32:29.677Z Reads: 121

```
They're 30mm wide which is wider than normal skate wheels. They're for off road skates. They are very grippy. My new deck is going to to be here by the end of the day so I'll see very soon lol. I had to alter the trucks due to the width of them.
```

---
## \#300 Posted by: Sapphirinia Posted at: 2018-01-30T14:33:01.197Z Reads: 120

```
![Screenshot_20180130-092955|571x499](upload://l6loXRviwQ5KmNMV3YEg7HpXgc5.jpg)
😀
```

---
## \#301 Posted by: meesie Posted at: 2018-01-30T14:46:11.575Z Reads: 116

```
Cool! How do they fare against normal longboard wheels regarding roll resistance?
```

---
## \#302 Posted by: Sapphirinia Posted at: 2018-01-30T14:49:06.695Z Reads: 118

```
I haven't attached the motor yet because I'm still waiting on a belt that fits. But by themselves it rolls so smooth in my room. I could lean one way way and it would roll. Like without kicking, I could lean forward and it roll forward, lean back and it would roll backwards. I can't wait to actually test it outside.
```

---
## \#303 Posted by: Sapphirinia Posted at: 2018-01-31T12:11:39.486Z Reads: 118

```
I'm making my fiberglass enclosure. So far so good. I'm sticking with the smaller wheels. I got wheelbite with the 150mm ones. Weirdly enough, I didn't with the shorter deck. Can't wait to file it down and paint it. And get the goodies back inside the enclosure. I'm going to try t-nuts this time for securing it. 

![20180131_070701|374x500](upload://as0nbUfBAWWeOK5TaB44SX3GkA5.jpg)
```

---
## \#304 Posted by: Sapphirinia Posted at: 2018-02-03T23:30:01.953Z Reads: 114

```
I love how this one rides. It's so comfy. Just gotta slap some more stickers on it. I also did a bad job lining up the voltmeter lol. I got to ride it up and down my block real quick and can't wait to ride again. Unfortunately it's about 20° here. I got some neon lights but I think I should put them on my helmet instead. ![20180203_161246|406x500](upload://wwBpklxkQg2mSIuDYGmwFgWWXaq.jpg)
```

---
## \#305 Posted by: akhlut Posted at: 2018-02-04T00:09:42.537Z Reads: 108

```
Word.  Too cold to skate.  Brutal out there!
```

---
## \#306 Posted by: GrecoMan Posted at: 2018-02-04T00:17:07.791Z Reads: 107

```
pshhhh

i rode today and it’s 4 here and snowing 🤣
```

---
## \#307 Posted by: michichopf Posted at: 2018-02-04T01:17:51.834Z Reads: 106

```
bruh, try minus 8 degree celcius. Still 6-8 hour skate sessions. No bad weather ma man only bad clothing :)

FML, you guys use Farenheit I forgot.... so actually the same :)
```

---
## \#308 Posted by: akhlut Posted at: 2018-02-04T01:24:10.041Z Reads: 107

```
It's not a nice, crisp dry cold.  It's a raw, damp cold with wind.  It's just ugly here in [coastal Jersey](https://weather.com/weather/today/l/08234:4:US).
```

---
## \#309 Posted by: Sapphirinia Posted at: 2018-02-13T01:31:24.379Z Reads: 102

```
Sooo, because I'm accident prone, I managed to get this board to stop working too. I'm hoping I can fix it. The voltmeter seems to still be accurate so I don't think it's the batteries, the vesc is lighting up and powering the rx so I think that's fine, the tx/rx seem to be fine since it's a solid light. Only thing that's left is the motor and I'm not sure how to test it. Please help.

I rode it while it was wet outside but I was told the motors are naturally water proof... 
 ![20180212_202728|441x500](upload://q2q3UdXCCrymFKhNsS7KPJj18TP.jpg)
```

---
## \#310 Posted by: Mobutusan Posted at: 2018-02-13T01:50:43.269Z Reads: 97

```
Check your motor phase wire connections and make sure they haven't come undone. If those look good, unplug the motor phase wires and touch two of them together. You should feel cogging and resistance when you do that. If that's all good, it should eliminate the motor as the source of the problem. Next would be to plug in the VESC to the computer and check for fault codes. And make sure your battery voltage isn't so low that it dropped past the battery cutoff voltage level.

Oh yeah, and make sure all your electronics are  bone dry first. Hair dryer works well.
```

---
## \#311 Posted by: b264 Posted at: 2018-02-13T01:57:33.949Z Reads: 98

```
Hall sensors maybe, try it with those unplugged.  I had a motor's hall sensors go bad from brine corrosion while the motor itself still worked fine
```

---
## \#312 Posted by: Sapphirinia Posted at: 2018-02-13T02:10:09.819Z Reads: 102

```
Batteries at 90%. I didn't get very far lol. I geuss I'll cut the shielding off to see what it looks like inside. ![20180212_210853|374x500](upload://grVkGpWyFJr5S1tjPiEE6bMv9Jq.jpg)
```

---
## \#313 Posted by: Sapphirinia Posted at: 2018-02-13T02:10:51.046Z Reads: 98

```
I don't think this motor has hall sensors
```

---
## \#314 Posted by: b264 Posted at: 2018-02-13T02:15:26.523Z Reads: 104

```
Try what @Mobutusan suggested then

Make sure touching motor leads 1&2 together makes the motor hard to turn and choppy
Make sure touching motor leads 2&3 together makes the motor hard to turn and choppy
Make sure touching motor leads 1&3 together makes the motor hard to turn and choppy
Make sure touching motor leads 1&2&3 together makes the motor **really** hard to turn and **smooth**
Make sure touching no motor leads together makes the motor easy to turn, just barely magnet indents you can feel a little
```

---
## \#315 Posted by: Sapphirinia Posted at: 2018-02-13T02:21:58.752Z Reads: 105

```
Yay, I wasn't connected all the way inside the shielding. There's a pretty cool 3 prong connector in there. It's fixed
```

---
## \#316 Posted by: Sapphirinia Posted at: 2018-02-13T02:26:25.281Z Reads: 105

```
Are there any tricks to keeping this together? Especially now that I had to cut the shielding off? ![20180212_212238|374x500](upload://6S8iJdEVTXFgvgnL6biLoQ1DEM2.jpg)
```

---
## \#317 Posted by: MysticalDork Posted at: 2018-02-13T02:30:23.782Z Reads: 97

```
I put tape or heatshrink over my bullets to keep them form coming apart.
```

---
## \#318 Posted by: Sapphirinia Posted at: 2018-02-13T02:32:52.980Z Reads: 99

```
I'll try that. Hopefully I have some that's big enough.
```

---
## \#319 Posted by: MysticalDork Posted at: 2018-02-13T02:40:13.118Z Reads: 103

```
If not, you could use some thin nylon string and tie the connections together.
```

---
## \#320 Posted by: Mobutusan Posted at: 2018-02-13T03:12:49.126Z Reads: 103

```
Glad it was something simple. If you have shrink tubing that's almost big enough you can widen it by putting some needle nose pliers through it and pulling the handles apart to stretch it out.
```

---
## \#321 Posted by: Sapphirinia Posted at: 2018-02-13T03:20:24.305Z Reads: 105

```
Me too. Hardest part was getting the enclosure off lol
```

---
## \#322 Posted by: Sapphirinia Posted at: 2018-02-13T23:47:18.400Z Reads: 104

```
So I think my inboard friend is in denial. We were riding together when I thought my board had water damage (which it didn't) he kept saying his board was fine in the water. So... Now he's saying he can't get the battery in and it's sparking when he tries to put it back in the board. But he insists that it's not from the rain and puddles... Also said inboard told him it was water damage but he says it can't possibly be. Hmm...
```

---
## \#323 Posted by: ATLesk8 Posted at: 2018-02-14T22:14:41.686Z Reads: 100

```
Well this person spent well over $1K on an inboard...reasonable?
```

---
## \#324 Posted by: Sapphirinia Posted at: 2018-02-14T22:21:11.562Z Reads: 104

```
He has an inboard m1 and boosted board. Both out of commission atm
```

---
## \#325 Posted by: Sapphirinia Posted at: 2018-02-19T23:17:59.288Z Reads: 100

```
So what type of clear coat should I use on my enclosure to go over my stickers and seal them on? Speaker is almost done :slight_smile:
```

---
## \#326 Posted by: Sapphirinia Posted at: 2018-03-13T14:35:42.460Z Reads: 91

```
I told @Deckoz I was stealing his speaker idea, and through lots of stuff working then breaking, here's my version. I was a bit heavy handed with the hot glue. I'll clean it up later. I used a slide on slide off design and the bottom is secured to the board. ![20180313_102023|690x431](upload://gYbBxxS8OTvg3QyKa6VqsFR9OMA.jpg)
```

---
## \#327 Posted by: Deckoz Posted at: 2018-03-13T14:50:31.151Z Reads: 91

```
[quote="Sapphirinia, post:326, topic:17387"]
@Deckoz I was stealing his speaker idea
[/quote]

Stealing? Nah, you made it your own :) how's it sound!!?
```

---
## \#328 Posted by: Sapphirinia Posted at: 2018-03-13T17:34:51.263Z Reads: 85

```
I like it. I have some more tweaks I've thought of while having it sit in my car next to me lol. I'll probably reprint it so it looks more professional.
```

---
## \#329 Posted by: Sapphirinia Posted at: 2018-03-13T20:37:16.982Z Reads: 85

```
https://youtu.be/8NGh9PT9pic
Testing out with some BTS. I think it sounds good. I definitely want to reprint it though to make it neater. I had to take it apart a few times. I'm thinking about coating the black in rubber paint too.
```

---
## \#330 Posted by: Sapphirinia Posted at: 2019-02-03T20:01:33.027Z Reads: 40

```
![20190113_004908|374x500](upload://x8YB2blfelfjaVAjXoC4mbne34P.jpeg)
Hey guys, some updates. The board has had its ups and downs. I gave up on it for a while. The vesc wound up frying on this one as well. But I did recently get a focbox and installed it. I was getting sparks whenever I plugged in the charger so I recently got a replacement input that soon I'll be installing. Lastly, after I had everything working in bldc, the motors moving properly when I controlled it with the arrows in my laptop, magically the remote no longer wanted to control the motors 🤦🏽‍♀️. I tried switching the receiver plug slots as many ways as I could think of and still a no go so I finally ordered another gtb2 to take apart and put into the case.

 I've also been working on making some gummie knock off wheels using nylon filament on my 3d printer. That's been a bit of trial and error. The design is solid but printing accurately is tricky. I bought a polyurethane mix but it wound up being too hard.

My speakers are becoming pretty dependable and I'm fairly sure the final design is done. Just gotta work on securing the innards better... Cuz vibration. I really like how they came out though. 

In other news, I wound up moving to Ohio in an attempt at saving money as I was evicted from my home in New Jersey. Things are going a lot better now that I'm out here. More time for creating and less time for stressing. 

I'm really hoping to get some skating in soon but the Temps have been brutally cold. Like 4° F. I remember my board not responding too great back in philly due to frigid Temps.

Anyways, thanks for reading. I miss the community and riding. Still have a bunch of back pain but I don't like taking the fun out of my life due to injuries. 
![20190105_194717|666x500](upload://gVEae9CitMoQYCRxEKwiN3LnROK.jpeg)
```

---
