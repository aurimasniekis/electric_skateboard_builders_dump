# Y piece or canbus

### Replies: 281 Views: 11233

## \#1 Posted by: bigben Posted at: 2017-06-30T20:31:25.884Z Reads: 777

```
I'm putting my 2nd board together. What are people's preference for dual setup? 
I have a reciever y piece but could put a canbus cable together. Is there a real advantage to setting the vescs up as master slave with canbus cable?
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-06-30T20:42:02.000Z Reads: 713

```
i split and not use CAN.

two reasons.

one, redundancy.  if one vesc goes out you'll have the other still working.  if using CAN, if master goes down, slave does as well.

another, ease of configuration.  why mess with configuring BLDC tool to use CAN when you can just program each vesc as if it's single use?  i know CAN configuration isn't that complicated but why introduce that at all?

i know CAN is required if you're using any kind of monitoring tool, but i think that's beyond the scope of this discussion.

http://www.electric-skateboard.builders/t/how-should-i-go-about-programming-double-vesc/19731/7?u=thisguyhere
```

---
## \#3 Posted by: psychotiller Posted at: 2017-06-30T21:03:46.356Z Reads: 677

```
I also prefer the split. simple=better
```

---
## \#4 Posted by: Mikenopolis Posted at: 2017-06-30T21:32:06.664Z Reads: 667

```
hmmmm. So after reading that attached thread and this one I went ahead and bought a few servo splitters. So this would be as simple as setting setting up each vesc with one motor with the same values right? Connect both vescs to a single receiver with one of the 5V wires cut/disconnected...is this all correct?
```

---
## \#5 Posted by: Aggdaddy Posted at: 2017-06-30T21:33:47.492Z Reads: 655

```
yep, that's how my e-mtb is set up.
```

---
## \#6 Posted by: bigben Posted at: 2017-06-30T21:38:19.658Z Reads: 654

```
Thanks for the replies. Pressure is on now as I think I have all I need to complete the build....
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-30T21:48:49.482Z Reads: 643

```
I just took a regular servo, cut a small slit into the outer wrap on the PPM cable, and soldered another cable directly to it. The other VESC only needs 1 PPM cable going to it.
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-06-30T21:53:33.404Z Reads: 632

```
i would just do motor detection for each motor for its respective vesc, the values can vary just slightly across motors.

and yes, cut one of the 5v lines coming off the Y split.
```

---
## \#9 Posted by: Smorto Posted at: 2017-07-01T01:26:36.945Z Reads: 617

```
So just connect them up as normal and cut one of the red wires coming from one of the vesc servo cables?
```

---
## \#10 Posted by: Smorto Posted at: 2017-07-01T01:31:55.053Z Reads: 618

```
Where did you get your servo splitters from? A link would be much appreciated. I looked but could only find leads like this

http://www.ebay.com/itm/HobbyStar-Servo-Y-Harness-Connector-Adapter-100MM-US-SELLER-/182403115872?epid=2120886665&hash=item2a7812ab60:g:YjAAAOSw241YZHXd


Do you guys think I could just have one male to male connector on each vesc like normal. Then connect each of those those connectors to the 2 connectors on this Y harness? Then plug the remaining connector into the receiver? Then also cut one of the red wires?
```

---
## \#11 Posted by: thisguyhere Posted at: 2017-07-01T02:29:17.975Z Reads: 584

```
Yes, but don't know what color. The one in the middle.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-07-01T03:18:52.912Z Reads: 575

```
I have been using the split method since day one and it has been rock solid dependable.
Also torque when accelerating and braking feels very even across the back wheels.
```

---
## \#13 Posted by: Nowind Posted at: 2017-07-01T03:38:36.096Z Reads: 572

```
Have a look for this kind of split wire : 

<img src="/uploads/db1493/original/3X/9/4/94a302d11f75507849241933ef352092ab6bb6e9.jpg" width="382" height="289">

They are smaller and more compact, less wire mess (-:

ebay
https://www.ebay.de/i/310826874737?chn=ps&dispItem=1
```

---
## \#14 Posted by: thisguyhere Posted at: 2017-07-01T03:49:48.426Z Reads: 561

```
I use this exact same one, courtesy of @psychotiller
```

---
## \#15 Posted by: Nordle Posted at: 2017-07-01T07:11:49.299Z Reads: 551

```
I would solder them instead of these connectors, had them coming loose once...
```

---
## \#16 Posted by: FMS Posted at: 2017-07-01T07:14:47.565Z Reads: 546

```
Why do people use CAN bus? Is there an advantage to that over something like pwm? Also am I blind or is my account restricted? I can't find where to start a new thread. Im a new user. Also what kind of CAN is this, Ive only see that kind with 2 wires, can low and can high.
```

---
## \#17 Posted by: Jinra Posted at: 2017-07-01T07:22:58.995Z Reads: 541

```
You probably haven't spent enough time reading posts to post. You need 30 minutes.

Can has the added benefit of being able to retrieve data from both VESCs while using a bluetooth module and appropriate mobile software, though I suppose you can split servo while using the CAN connection purely for data.
```

---
## \#18 Posted by: Nowind Posted at: 2017-07-01T11:59:32.665Z Reads: 528

```
Yeah you are right they can come loose...
The linked one are better then some other from tight fitting factor... 
But I always take a piece of electrice tape or shrinktube to secure them.... better for sure!
```

---
## \#19 Posted by: Smorto Posted at: 2017-07-01T13:54:24.208Z Reads: 526

```
So I would simply solder the orange or white wire coming from one of the vescs to the orange or white wire from the other vesc?
```

---
## \#20 Posted by: Alanhunt123 Posted at: 2017-07-01T15:37:51.328Z Reads: 525

```
Glad this thread was made. I was debating on whether to use canbus or just split the servo lead. My friend told me to use canbus because then the motors would be "synced up", but he's never built a dual drive eSk8 before :joy:

Really, the only reason to use canbus that I can think of, is if you want to use the traction control setting, but traction control makes things a little too predictable for me!
```

---
## \#21 Posted by: i2oadsweepei2 Posted at: 2017-07-01T16:49:55.195Z Reads: 504

```
This thread came at the perfect time. I'm about to set up a couple vesc-x's. They came with the canbus cable. My gut was telling me to use the splitter as well. I've always used splitters so far with my esk8s and TB esc's and all my other rc stuff. My mind is made up now. Splitter it is. Thanks for a good discussion.
```

---
## \#22 Posted by: trampa Posted at: 2017-07-01T17:26:22.852Z Reads: 507

```
Don't use the Y-cables with VESC-based Hardware!!!! 
@Nowind killed two VESC, using this method. The VESC 4.xx are a bit less prone to burn the STM, when using a Y-bridge, but it can still happen. 
All new VESC hardware will fry pretty much immediately when using Y-bridges, especially when using the comm port.
Benjamin stated himself that Y-Cable use is something you should never ever do.
Always use the CAN-BUS!!!

Frank
```

---
## \#23 Posted by: bigben Posted at: 2017-07-01T17:29:52.736Z Reads: 496

```
Damn you @trampa. Just when I thought this was cut and dried.  ☹️
```

---
## \#24 Posted by: Jinra Posted at: 2017-07-01T17:38:38.651Z Reads: 484

```
What? How would split servo kill the vesc? I don't see how that makes any sense. Both my boards and tons of others on here split with no problems
```

---
## \#25 Posted by: i2oadsweepei2 Posted at: 2017-07-01T17:49:51.232Z Reads: 486

```
[quote="i2oadsweepei2, post:21, topic:26461"]
My mind is made up now. Splitter it is
[/quote]

Ok not so much now. Thanks Frank, for bringing any issues up. Learning mode on.
```

---
## \#26 Posted by: Alanhunt123 Posted at: 2017-07-01T18:29:07.239Z Reads: 478

```
Huh, I wouldn't expect that a y cable would fry it... I would figure that as long as you don't connect the 5v cable on both of them and only connect signal and ground that it would be fine.

I'd love to hear an explanation for why this is an issue if anyone has some insight!
```

---
## \#27 Posted by: Smorto Posted at: 2017-07-01T19:01:32.796Z Reads: 476

```
How? Why? Im confused now :joy:.
```

---
## \#28 Posted by: Nowind Posted at: 2017-07-01T22:12:14.769Z Reads: 475

```
This was not by connecting Vesc´s via parallel PPM...
Got a ADC input and put this in parallel

In the end too much splitted PPM Vesc 4 on the market as that could be a real issue with the Vesc4
```

---
## \#29 Posted by: Nordle Posted at: 2017-07-02T08:40:44.612Z Reads: 469

```
Please link this statement...
```

---
## \#30 Posted by: bigben Posted at: 2017-07-02T09:02:49.432Z Reads: 474

```
So are we saying Y piece is ok?

What does @longhairedboy use on his builds or is that a trade secret...?
```

---
## \#31 Posted by: Namasaki Posted at: 2017-07-02T15:24:28.017Z Reads: 468

```
@i2oadsweepei2   
I've been using a Y cable for dual Vescs on two builds for a long time and have not had any issues at all.
Both Vescs set up as masters running in parallel work very well
```

---
## \#32 Posted by: High-roller Posted at: 2017-07-02T15:31:59.889Z Reads: 460

```
Anyone know how FOCboxes would handle this?
```

---
## \#33 Posted by: Nordle Posted at: 2017-07-02T15:37:33.360Z Reads: 456

```
Actually they are just vesc's. Some ppl just like to confuse you because of their marketing. And any other esc would handle this also fine
```

---
## \#34 Posted by: Namasaki Posted at: 2017-07-02T15:37:37.810Z Reads: 449

```
Running Vesc 4.12 with a Y signal cable is fine. 
If you want to be extra safe, clip the 5v wire coming from one of the Vescs.
```

---
## \#35 Posted by: abenny Posted at: 2017-07-02T15:39:54.009Z Reads: 442

```
and both controllers set up as ppm on each vesc?
```

---
## \#36 Posted by: Namasaki Posted at: 2017-07-02T15:48:44.322Z Reads: 446

```
Yes, use ppm on both controllers and set each one up separately but with same settings.
I even run one of mine with ppm/uart and have a bluetooth module plugged in to monitor real time data.
I've have been running one of my builds this way for about 1 year and the other for about 9 months
This setup is simple and it works.
```

---
## \#37 Posted by: Nordle Posted at: 2017-07-02T15:48:55.890Z Reads: 439

```
What else, just use your brain-.-
```

---
## \#38 Posted by: abenny Posted at: 2017-07-02T16:43:27.610Z Reads: 444

```
alright thanks for clarification...you spoke to me about this on a previous post but now that my vesc is repaired and en-route to me, id really like to cover all my bases and not burn another vesc :D thanks
```

---
## \#39 Posted by: Namasaki Posted at: 2017-07-02T17:15:12.914Z Reads: 441

```
how did you burn it the first time?
```

---
## \#40 Posted by: abenny Posted at: 2017-07-02T18:55:03.971Z Reads: 447

```
first time trying a dual vesc set up, can bus connection and i messed up the settings on the master vesc, i had it set as master and to send can bus signal...drv chip when pop
```

---
## \#41 Posted by: Stefan Posted at: 2017-07-02T20:36:25.128Z Reads: 440

```
I have a dual FOCBOX setup for about a good month now. No problems so far and i am using canbus. I have even mixed up the master and slave settings but it obviously did not harm the ESCs.
```

---
## \#42 Posted by: trampa Posted at: 2017-07-03T12:10:17.462Z Reads: 436

```
As I said, the VESC 4 is less prone to fry, when using Y-PPM. But it is still not recommended to do that.
The real problem is the following: The new designs we will see soon, will not like the Y-cable. If the users get used to the Y-solution, they will simply apply that same setup to the new hardware and will fry their two new expensive ESCs in a second.  @Nowind is a prime example.... Two new STMs will solve the matter in this case, but its still a bit sad that it happened.

So better stay away from the Y.

Frank
```

---
## \#43 Posted by: Jinra Posted at: 2017-07-03T13:29:23.570Z Reads: 430

```
He JUST said that wasn't because of parallel ppm. I don't see the logic at all in saying parallel ppm will fry your vesc, and you've said it twice now without providing an explanation
```

---
## \#44 Posted by: Smorto Posted at: 2017-07-03T15:33:23.933Z Reads: 426

```
[quote="trampa, post:42, topic:26461"]
@Nowind is a prime example
[/quote]



[quote="Nowind, post:28, topic:26461"]
This was not by connecting Vesc´s via parallel PPM...
[/quote]


Hmmmmm, now I'm even more confused :slight_smile:. I would like an explained as to how exactly it would fry the vescs.
```

---
## \#45 Posted by: longhairedboy Posted at: 2017-07-03T17:15:41.248Z Reads: 413

```
I use the can bus and enable traction control. 

I don't care what anyone says. Traction control works and does exactly what the name implies. I love it.
```

---
## \#46 Posted by: bigben Posted at: 2017-07-03T17:44:56.972Z Reads: 406

```
That's a good enough endorsement for me!
```

---
## \#47 Posted by: Smorto Posted at: 2017-07-03T17:49:30.851Z Reads: 408

```
Where I'm stuck is I like the settings I have now for my single vesc. I feel like the splitter is the simplest route to keeping my same settings. However, with the can bus you are able to have traction control which is nice, though it is more complicated to configure and if you do it wrong you could fry one or both of your vescs. I am still undecided at this point though leaning toward the splitter.
```

---
## \#48 Posted by: Jinra Posted at: 2017-07-03T17:56:13.165Z Reads: 410

```
I never really found traction control useful. For me it actually caused some issues with acceleration. Without traction control, a wheel can free spin when it lifts, but I never found it problematic. I tend to not lift my wheels when I ride anyway.

My can connection also severed 3 times. First time the connection was loose and made one of my VESCs spaz out. The second time I tried Ollins can bus connector and the wire broke. The third time I soldered the wire to the win and the wire literally broke off.
```

---
## \#49 Posted by: psychotiller Posted at: 2017-07-03T17:56:28.090Z Reads: 403

```
Sorry, but this is hysterical. splitting the signal from one receiver can't do the damage you're claiming. In fact, it's less complicated.
```

---
## \#50 Posted by: longhairedboy Posted at: 2017-07-03T18:00:44.632Z Reads: 403

```
you have to kill the 5v on one of the VESCs or you send too much juice to the receiver. @blasto just reminded me of this too.
```

---
## \#51 Posted by: longhairedboy Posted at: 2017-07-03T18:03:16.416Z Reads: 398

```
We'll have to settle this debate by paying two other people who have no stake in this at all to beat the crap out of each other. It's the only civilized thing to do.
```

---
## \#52 Posted by: psychotiller Posted at: 2017-07-03T18:03:48.052Z Reads: 401

```
True, but it still won't fry your vescs. They will just communicate in ways that are weird. 

Sounds like the problem isn't so much with the splitter, but with the new vesc.
```

---
## \#53 Posted by: Jinra Posted at: 2017-07-03T18:14:03.006Z Reads: 397

```
We'll play a game of chicken with 1 board on y-splitter, and the other on CAN. First one to back off is obviously wrong
```

---
## \#54 Posted by: thisguyhere Posted at: 2017-07-03T18:17:32.124Z Reads: 396

```
[quote="psychotiller, post:52, topic:26461"]
Sounds like the problem isn't so much with the splitter, but with the new vesc
[/quote]

<img src="https://www.mememaker.net/static/images/memes/2560762.jpg" />
```

---
## \#55 Posted by: psychotiller Posted at: 2017-07-03T18:18:40.236Z Reads: 387

```
Those are just fireworks brotha!
```

---
## \#56 Posted by: smurf Posted at: 2017-07-03T19:04:44.717Z Reads: 390

```
I don't know which way is more civilized but the American way of setting this is with a race 🏁
```

---
## \#57 Posted by: longhairedboy Posted at: 2017-07-03T19:12:07.632Z Reads: 383

```
Ok but only if we can light our battery boxes on fire before we floor our boards directly at each other. You know, because that will help solve the debate.
```

---
## \#58 Posted by: i2oadsweepei2 Posted at: 2017-07-03T19:36:08.320Z Reads: 375

```
Thanks @Namasaki for the reassurance. I've just sat down to delve into the world of vesc x. Gonna try the split ppm. Like rc stuff neither vesc should know the other is there. Since the vesc can function as a single drive I don't see any issues. Both will benefit from the help of the other without having to know why. This was my original thinking. I take full responsibility regardless.
```

---
## \#59 Posted by: thisguyhere Posted at: 2017-07-03T20:02:23.491Z Reads: 377

```
I have a good idea. Forget the CAN and y-split. 

One remote for each vesc, so you double fist remotes one in each hand.

Fixed.
```

---
## \#60 Posted by: psychotiller Posted at: 2017-07-03T20:08:55.746Z Reads: 377

```
Just make sure to cut the 5v on one side of the splitter. That way you only have a total of 5v going to your receiver.
```

---
## \#61 Posted by: Jinra Posted at: 2017-07-03T20:25:43.078Z Reads: 366

```
I mentioned this before but you'll have 5v going into it either way since it'll be in parallel. Just more available current if you don't snip.
```

---
## \#62 Posted by: psychotiller Posted at: 2017-07-03T20:28:48.995Z Reads: 367

```
True. I still cut my own builds though.
```

---
## \#63 Posted by: psychotiller Posted at: 2017-07-03T20:31:54.491Z Reads: 363

```
I just carry a couple of mattress springs in my pocket. same same :stuck_out_tongue_closed_eyes:
```

---
## \#64 Posted by: Blasto Posted at: 2017-07-03T20:48:58.301Z Reads: 365

```
Each DRV on each vesc is outputting the 5V, due to component tolerances, both vesc will not output exactly 5.000000V.

The voltage difference of each 5V rail is what will hurt one or the other DRV by creating a small short circuit and imbalance one or both buck coverters and that's where shit hits the fan. 

So it MAY work having both 5V in parallel, if it does, you got lucky.
```

---
## \#65 Posted by: psychotiller Posted at: 2017-07-03T21:02:40.904Z Reads: 355

```
uhhhh...Why? there is no feedback. It's just 5v power supply. Whether the second side of the splitter is cut or not, The vescs have no idea. The only issue is some receivers can trip out on inconsistent voltage. Thinking you have to use canbus is in line with thinking you have to use 2 vescs...lots of damaged single motor builds due to this confusion right?
```

---
## \#66 Posted by: Blasto Posted at: 2017-07-03T21:10:10.755Z Reads: 361

```
[quote="psychotiller, post:65, topic:26461"]
there is no feedback.
[/quote]

Actually yes there is, if you have one vesc at 5.00V and the other at 5.1V connected in //. You have a 0.1V that is creating a short circuit by dumping itself in the vesc that is at 5.00V

What this also does it pulls more current from the vesc w 5.1V and that might make it drop to a equilibrium...

But this applies to any voltage rail, not just the vesc, you do not put two different supplies in // if they don't have proper senses or ORring diodes
```

---
## \#67 Posted by: trampa Posted at: 2017-07-03T22:23:43.531Z Reads: 358

```
Thx @Blasto or your response. Especially the connectors going directly to the STM are very sensitive and have a very low tolerance to over voltage/current and this is why @Nowind fried the STM, although he disconnected the 5V from one cable. 

If you Y your STM/DRV will likely fry!

Frank
```

---
## \#68 Posted by: Jinra Posted at: 2017-07-03T22:36:42.925Z Reads: 357

```
So you admit to split PPM not being an issue. It's split 5v that's a problem.
```

---
## \#69 Posted by: i2oadsweepei2 Posted at: 2017-07-03T23:02:45.230Z Reads: 353

```
Yup for sure. Wouldn't have it any other way.
```

---
## \#70 Posted by: Namasaki Posted at: 2017-07-03T23:31:35.695Z Reads: 361

```
[quote="thisguyhere, post:59, topic:26461, full:true"]
I have a good idea. Forget the CAN and y-split. 

One remote for each vesc, so you double fist remotes one in each hand.

Fixed.
[/quote]

Here's an idea based on what you said:
One remote paired with 2 separate receivers connected to 2 seperate Vescs. 
Bet no one has tried that yet. 
Anyway, as I said before, I've been running dual Vescs with split ppm for over a year with no problem. 
NOTE: I did clip one of the 5v wires to be safe although what @Jinra said about parallel makes sense.
```

---
## \#71 Posted by: Jinra Posted at: 2017-07-03T23:33:27.295Z Reads: 351

```
I concede that I'm not familiar with electronics enough to understand what @Blasto said, but I'd trust him enough with it. 

For me anyway I just simply soldered another wire to the PPM on my servo to make a split PPM signal, no need for the other 5v or GND.
```

---
## \#72 Posted by: thisguyhere Posted at: 2017-07-04T00:21:48.575Z Reads: 348

```
I was just being stupid
```

---
## \#73 Posted by: Smorto Posted at: 2017-07-04T00:22:01.598Z Reads: 346

```
In my mind this would seemingly eliminate the problem that @trampa is saying which is over current/voltage with the Y splitter. Why doesn't 2 receivers work when one does if both the one recover and 2 recover have the same 5v cable going to a vesc?
```

---
## \#74 Posted by: psychotiller Posted at: 2017-07-04T00:26:02.550Z Reads: 337

```
So cut the single 5v.
```

---
## \#75 Posted by: abenny Posted at: 2017-07-04T00:59:47.231Z Reads: 344

```
i just feel like that the 'likely' term you used has been proven wrong by the amount of people that actually do use a y-split and not had any issues...
but please if anyone else has seen other cases of dead vesc from using a y-splitter post it here...im going to be setting up double vesc soon and already fried one doing a CAN connection...so in my mind im more 'likely' to fry it by can-bus..but thats just in my own experience..
```

---
## \#76 Posted by: Namasaki Posted at: 2017-07-04T03:04:47.004Z Reads: 334

```
And experience is the best teacher.
```

---
## \#77 Posted by: lock Posted at: 2017-07-04T03:40:21.925Z Reads: 342

```
My electrical engineering background is limited to some 2 semesters of study (I barely passed)  some 15 years ago... Please excuse my ignorance.

The PPM signal coming from the receiver is a series of 5v pulses. The receiver is powered by one of the VESCs, because you cut one to prevent the short (based on what I've read above). Based on what @Blasto said there could be some variance in the VESC voltage, so the receiver may be powered by 5.0v or 5.1v. Does this mean the PPM signal sent by the receiver will be either 5.0v or 5.1v depending on which VESC it is connected to? And does the VESC outputting 5.0v care if it receives a PPM signal at 5.1v? 

[quote="Namasaki, post:76, topic:26461, full:true"]
And experience is the best teacher.
[/quote]
Agree to some extent, however I still like to understand how/why something works.
```

---
## \#78 Posted by: Blasto Posted at: 2017-07-04T03:50:01.374Z Reads: 334

```
[quote="lock, post:77, topic:26461"]
And does the VESC outputting 5.0v care if it receives a PPM signal at 5.1v?
[/quote]

No the mcu does not care if the ppm signal is 5.0V or 5.1 (if i remember correctly the IO's of the stm32 is tolerent up to 5.3V)

What i am saying is by connecting two power rails in // it could unbalance one or the other buck converter (on the DRV) and that's where shit can hit the fan by bringing the voltage over 5V or damage the DRV's buck converter.

Side note, // = parallel because im a lazy fuck
```

---
## \#79 Posted by: Jinra Posted at: 2017-07-04T03:50:34.902Z Reads: 327

```
The ppm signal is not 5v. Only the 5v middle rail is 5v. I forget the exact voltage of the ppm wire but it's at least 2v lower than that. Which begs the question of why the minute difference in ppm voltages is fine for parallel ppm but not for the 5v rail @Blasto
```

---
## \#80 Posted by: lrdesigns Posted at: 2017-07-04T03:56:26.525Z Reads: 329

```
PPM Y cable with 1 red wire unpluged has been working good for me on vesc 4. I like the redundancy, I can still get home on one motor if need be.
```

---
## \#81 Posted by: lock Posted at: 2017-07-04T04:20:38.820Z Reads: 322

```
Thanks. Yeah, bit of Googling showed that the signal is regulated to some other voltage. Mostly 3.3v. Given the VESC must be tolerant to a range of PPM voltages I'm back to struggling to see how the Y cable could break stuff.
```

---
## \#82 Posted by: Namasaki Posted at: 2017-07-04T04:52:50.120Z Reads: 325

```
Back when I was considering using hobby Esc's with built in BEC, I heard somewhere that it was necessary to clip the red wire from on of the Esc's in a dual configuration.
When I started using Vescs, I just carried that principle over.
Better safe than sorry.
@Jinra Have you actually tried running dual vescs in a Y ppm setup without clipping one of the 5v wires?
```

---
## \#83 Posted by: Jinra Posted at: 2017-07-04T05:03:57.972Z Reads: 319

```
No since i use a standard 3 pin servo cable and attach a single other cable to the PPM wire via solder.
```

---
## \#84 Posted by: benwong Posted at: 2017-07-04T05:32:08.382Z Reads: 322

```
Correct, normal esc need to pull one possitive lead. So tat receiver oni send signal to esc. I make this mistake before. Fried my esc.
```

---
## \#85 Posted by: trampa Posted at: 2017-07-05T08:22:20.776Z Reads: 323

```
I talked to Benjamin last night and he said you should never ever do the Y. The VESC 4 can tolerate that better than the actual designs, but there is no guarantee that this solution will not fry the hardware. You could be lucky or not.100 working Y-twin setups do not necessarily mean, that Nr. 101 will not have an issue. This has nothing to do with cutting one 5V wire BTW! That is confirmed through BV.
The new hardware designs will not tolerate the Y-cable and will very likely fry. So promoting the Y-cable will only cause issues and it is not recommended. There will be a warning about that on the VESC Website.
Benjamin designed the thing and he will know it best. I trust him on that 100%. Who else should know it better?
If someone is of another opinion, and something goes wrong, you have to blame yourself.

Frank
```

---
## \#86 Posted by: TarzanHBK Posted at: 2017-07-05T08:40:24.763Z Reads: 311

```
But why? Whats the reason that its not tollerated by the Vesc 6? And why is the Vesc 4 more robust on this piece?
```

---
## \#87 Posted by: lrdesigns Posted at: 2017-07-05T08:40:55.484Z Reads: 321

```
Wow so we have been doing it wrong all these years, you would think this would be basic knowledge for setup of a dual. 

I get that vesc 6 is a different design and does not like the Y cable. 

I will keep running Y on vesc 4 though. :stuck_out_tongue_closed_eyes:
```

---
## \#88 Posted by: longhairedboy Posted at: 2017-07-05T11:26:22.097Z Reads: 324

```
Listen to @blasto on this guys. I just fried another 4.12 because of this nonsense. Guess its heading back to Canada at some point lol
```

---
## \#89 Posted by: i2oadsweepei2 Posted at: 2017-07-05T12:00:35.115Z Reads: 323

```
Just fried by splitting the PPM signal or splitting and not clipping one of the 5v sources? Thanks
```

---
## \#90 Posted by: longhairedboy Posted at: 2017-07-05T12:38:24.070Z Reads: 322

```
i didn't clip the +5 from the second vesc and connected the 5v from both vescs to the receiver.

The receiver is fine, one vesc fried. 

Its been so long since i've done a split PPM i just totally spaced on that.
```

---
## \#91 Posted by: WARMAN Posted at: 2017-07-05T13:26:07.628Z Reads: 309

```
Iv always used "can" i was advised when building not to by several people and go with the "y" connection but made my own mind up..why wouldn't you want traction control!
```

---
## \#92 Posted by: longhairedboy Posted at: 2017-07-05T13:47:59.732Z Reads: 306

```
on a dual drive CAN is the best option in my opinion. However, you can't run 4 4.12s together on a CAN bus without a mod or shit starts acting funny, so i split the ppm to two master vescs and then each one of those was jumped to a secondary via CAN.
```

---
## \#93 Posted by: Namasaki Posted at: 2017-07-05T14:00:54.058Z Reads: 307

```
Well that settles it. Gotta cut one of the 5v wires.
```

---
## \#94 Posted by: Namasaki Posted at: 2017-07-05T14:06:12.725Z Reads: 312

```
I've been running 4 Vesc 4.12's for 9-12 months with split ppm and one 5v wire clipped With no problem. 
Sorry but I don't buy the Luck argument.
Although, I must say that I am fortunate to have 4 high quality Vescs by @chaka
```

---
## \#95 Posted by: Namasaki Posted at: 2017-07-05T14:10:56.825Z Reads: 314

```
I went with split ppm in the beginning because it was more simple solution than canbus. 
People have fried their Vescs by just not getting the settings in bldc right. 
I haven't felt any need for traction control even when braking and accelerating in turns. Also I have heard of people having problems with traction control and the canbus setup.
```

---
## \#96 Posted by: sebaszz Posted at: 2017-07-05T14:30:07.064Z Reads: 316

```
Response Benjamin from VESC-Project forum:

> Dead MCU

> I got two VESCs where the STM32F4 had died. The reason was that the ADC inputs for an analog throttle have been connected in parallel. When VESCs are connected to the same battery there will be a voltage differential between them under load due do inductance and resistance in the cables. This voltage differential can reach quite high values and the MCU pins are very sensitive to that. Negative one volt is sure to kill the input and short the whole MCU. The PPM input is slightly less sensitive to this than the other pins as it has a low-pass filter, but it still is a bad idea (the VESC4 had a slower PPM filter and was slightly less sensitive). The CAN-bus can handle around +-60V difference, which is why it should be used on a multi-VESC setup. The CAN-bus also provides other advantages such as cruise control with several motors and traction control.

> Solution: Always use the CAN bus to connect VESCs in parallel and set up the apps accordingly. Never connect the other inputs in parallel in VESCs that are connected to the same battery.
```

---
## \#97 Posted by: WARMAN Posted at: 2017-07-05T14:43:05.392Z Reads: 294

```
Doesn't take long to learn how to set up properly and ran good with traction control for me since day one! 
Each to there own though just make sure you know what your doing.
If vedder recommends and uses it that's good enough for me.
```

---
## \#98 Posted by: Namasaki Posted at: 2017-07-05T14:50:10.467Z Reads: 298

```
[quote="WARMAN, post:97, topic:26461"]
Each to there own though just make sure you know what your doing.
[/quote]
 
I agree with you 100% on this. 
You gotta know what your doing when using a Vesc in either configuration.
```

---
## \#99 Posted by: WARMAN Posted at: 2017-07-05T14:53:21.660Z Reads: 295

```
How ever much time you put in to something the better it will be...life,family/friends,business or even learning to build a board!
```

---
## \#100 Posted by: Jinra Posted at: 2017-07-05T15:05:59.486Z Reads: 300

```
[quote="sebaszz, post:96, topic:26461"]
I got two VESCs where the STM32F4 had died. The reason was that the ADC inputs for an analog throttle have been connected in parallel.
[/quote]

straight from the horses mouth. No mention of fried vesc due to ppm @trampa

RIP @longhairedboy thanks for your sacrifice.. for science!

Honestly, id prefer can bus connection if i didn't have such bad experiences with it. A loose connection made one wheel go full throttle while the other one was unresponsive
```

---
## \#101 Posted by: TarzanHBK Posted at: 2017-07-05T16:37:03.622Z Reads: 286

```
I just fried both esk8.de vescs with a bad can connection. Apparently a solder joint went lose and both can chips fried. Had a fast repair by lp-electronics and will use thicker cables in the future, but still using can on all builds.
```

---
## \#102 Posted by: Namasaki Posted at: 2017-07-05T17:08:55.179Z Reads: 282

```
sounds like split ppm is the less risky option
```

---
## \#103 Posted by: Jinra Posted at: 2017-07-05T17:10:40.691Z Reads: 288

```
To be fair split PPM, has the same risk for improper soldering or a loose connection from vibration, but with PPM a connection coming loose usually just means no response on that VESC/motor vs my experience on CAN where my motor went full throttle
```

---
## \#104 Posted by: longhairedboy Posted at: 2017-07-05T17:16:19.745Z Reads: 294

```
https://www.pololu.com/product/1810

## +

one drop of flux on the pin after you slide it on

## +

One drop of solder that the flux wicks right into the connector

## =

never have to worry about it coming loose ever

Also with a touch of the iron tip the solder flows and the connector slides right off again, and when you want to put it on again, touch the tip of the iron, it flows, you slide it on again. 

/knowledgebomb
```

---
## \#105 Posted by: Jinra Posted at: 2017-07-05T17:18:01.937Z Reads: 280

```
Exactly what I did with my connection. The pin the VESC literally broke off after a while.
```

---
## \#106 Posted by: Namasaki Posted at: 2017-07-05T17:18:39.622Z Reads: 279

```
That's what I'm talking about. 
Split ppm comes loose, No big deal
Canbus comes loose, Outa control board or fried Vescs.
Although,I have never had a ppm wire come loose.
```

---
## \#107 Posted by: longhairedboy Posted at: 2017-07-05T17:20:09.829Z Reads: 275

```
LOL For that i don't know man you got some serious vibration issues near that pin.
```

---
## \#108 Posted by: Jinra Posted at: 2017-07-05T17:22:02.849Z Reads: 277

```
Yea, unlucky me. Now I got a chaka VESC with a castrated CAN bus :'(

If I try again I'll probably just remove the header altogether and solder straight to PCB.
```

---
## \#109 Posted by: longhairedboy Posted at: 2017-07-05T17:27:31.029Z Reads: 275

```
that's how it was done in the Raptors. That's how i would do it if was doing my own 4.12s also. I wouldn't waste money on connectors.
```

---
## \#110 Posted by: Smorto Posted at: 2017-07-05T17:28:07.474Z Reads: 275

```
That is exactly what I am thinking, I like the traction control of the CAN but I am afraid if something happens (either it comes loose or I mess up the settings) that it will fry both expensive vescs. I also like the simplicity and redundancy of the Y splitter. I think that a Y adaptor with the 5v line cut and maybe the ground cut too for good measure even though it won't do anything, is the way to go for me.
```

---
## \#111 Posted by: longhairedboy Posted at: 2017-07-05T17:30:18.046Z Reads: 276

```
don't you need the ground line to complete the circuit for the signal?
```

---
## \#112 Posted by: Jinra Posted at: 2017-07-05T17:32:32.884Z Reads: 275

```
Nope, I use a single PPM line I soldered onto my servo cable on my other VESC.
```

---
## \#113 Posted by: longhairedboy Posted at: 2017-07-05T18:00:38.113Z Reads: 273

```
man this thread is full of useful info. I'm doing that from now on when i have to split  the ppm signal.
```

---
## \#114 Posted by: longhairedboy Posted at: 2017-07-05T18:07:56.429Z Reads: 276

```
i would just like to take an additional moment here to say that electrons are fucking weird.
```

---
## \#115 Posted by: psychotiller Posted at: 2017-07-05T18:16:32.000Z Reads: 277

```
That's a very quarky statement.
```

---
## \#116 Posted by: WARMAN Posted at: 2017-07-05T18:34:40.954Z Reads: 280

```
Iv not had the can cable come loose yet and I ride some real bad roads! 
Might tape it down though or put a drop of high strengh thread locker on it!
```

---
## \#117 Posted by: longhairedboy Posted at: 2017-07-05T18:57:30.281Z Reads: 276

```
i usually also fill the connector space with hot glue after soldering the crimped connectors on. Forgot to mention that.
```

---
## \#118 Posted by: bigben Posted at: 2017-07-05T22:18:41.826Z Reads: 275

```
Hey @trampa,
will the new software that will soon be available for everyone make it easier to program the dual vesc canbus configuration?
```

---
## \#119 Posted by: trampa Posted at: 2017-07-05T22:28:47.490Z Reads: 279

```
Wizard, 1 minute, job done.
```

---
## \#120 Posted by: JohnnyMeduse Posted at: 2017-07-05T22:32:48.500Z Reads: 280

```
[quote="trampa, post:119, topic:26461"]
Wizard
[/quote]

Someone summon me? How can I help you ?
```

---
## \#121 Posted by: Surfer Posted at: 2017-07-05T22:35:40.708Z Reads: 276

```
Hi Frank, just curious about foc, got improvements for 4.12 with the new vesc-tool? Aside of the bootloader trough usb.
Thanks
```

---
## \#122 Posted by: bigben Posted at: 2017-07-05T22:40:33.696Z Reads: 277

```
And is there a date for this release??
```

---
## \#123 Posted by: trampa Posted at: 2017-07-05T22:46:08.662Z Reads: 284

```
Beside FW 3.26 support, wizards, bootloader upload, different throttle curves, well improved FOC, VESC-Tool interface with tons of explanations and a comprehensive documentation, there is nothing new for HW 4.xx.

Betas can download it on Friday. After a short BETA phase Benjamin wants to release it.
Reference HW designs will follow as soon as finished and tested. 

Frank
```

---
## \#124 Posted by: Titoxd10001 Posted at: 2017-07-06T03:14:08.727Z Reads: 282

```
FML. I've been following this thread and I was on the fence with which is better. I do like having the ability to change settings through one USB with can bus, but also dread the day a belt breaks and have no power on either motor (right?). Do have dual 15mm so it's not to much of a concern. So today I was connecting my focboxes and connected my master through antispark xt90. My slave was disconnected from the power so I connected (not thinking) it how I usually have it in parallel. Guess what both my focers are fried. All because can bus I'm told. So that's $100 down the drain if they can be repaired and $250 if they can't. 😭

Just going to drive with a remote in each hand and turn like a tank from now on 😂 #TwoWheels
```

---
## \#125 Posted by: Jinra Posted at: 2017-07-06T03:18:05.753Z Reads: 268

```
By that logic, a single drive board should constantly be turning in one direction :P
```

---
## \#126 Posted by: psychotiller Posted at: 2017-07-06T03:21:43.767Z Reads: 261

```
Oh man...That sucks
```

---
## \#127 Posted by: Titoxd10001 Posted at: 2017-07-06T03:23:36.245Z Reads: 259

```
Scratch that last part. What if I made it 2wd tho? TwoWheels
```

---
## \#128 Posted by: Jinra Posted at: 2017-07-06T03:25:46.636Z Reads: 261

```
You mean dual remotes? A bit ridiculous, imo, but I guess the redundancy is extra safe!

RIP your Foc boxes :(
```

---
## \#129 Posted by: Namasaki Posted at: 2017-07-06T03:29:22.795Z Reads: 260

```
Very sorry to hear your VescX's are fried.
Sounds like there are more ways that canbus can fry a vesc than we realized.
That does it, I am never gonna get on the canbus

P.S.
You don't need 2 remotes. Just 2 receivers both paired to the same remote.
Now thats redundancy
```

---
## \#130 Posted by: Jinra Posted at: 2017-07-06T03:35:17.385Z Reads: 259

```
I did have my receiver shut off on me, leaving me brake-less. In that case dual remote would help, but still ridiculous.
```

---
## \#131 Posted by: Namasaki Posted at: 2017-07-06T03:35:54.532Z Reads: 257

```
why did your receiver go out
```

---
## \#132 Posted by: Jinra Posted at: 2017-07-06T03:36:38.947Z Reads: 257

```
No, the receiver acted like it wasn't bound. Restart of the board fixed it, but it happens sporadically so I changed it to the nano v2 remote.
```

---
## \#133 Posted by: Namasaki Posted at: 2017-07-06T03:37:12.242Z Reads: 256

```
So that happened with the Nano v1
```

---
## \#134 Posted by: Jinra Posted at: 2017-07-06T03:37:50.946Z Reads: 256

```
Nope benchwheel controller. It **only** happens on my Carbonated build though, never once happened on my Honey Driver build. No idea what causes it.
```

---
## \#135 Posted by: Namasaki Posted at: 2017-07-06T03:38:46.537Z Reads: 255

```
isn't the benchwheel remote a bluetooth system?
```

---
## \#136 Posted by: Jinra Posted at: 2017-07-06T03:39:03.743Z Reads: 262

```
Nope standard 2.4ghz radio
```

---
## \#137 Posted by: thisguyhere Posted at: 2017-07-06T03:49:19.669Z Reads: 268

```
[quote="Titoxd10001, post:124, topic:26461"]
both my focers are fried
[/quote]

<img src="https://media.giphy.com/media/A8mOE2k9WV0yc/giphy.gif" />

Foreal that fkn sux, I'm sorry. 

I got a spare vesc 4 if u wanna get up and going quckly. Barely used, friend prices.
```

---
## \#138 Posted by: wafflejock Posted at: 2017-07-06T04:14:41.769Z Reads: 264

```
In the VESC app config you can set the time for it to go idle if it doesn't get a signal from the receiver, can also give it a braking amperage I'm pretty sure though I don't set that value myself since I'd rather coast for a second in case the connection reestablishes instead of being ground to a halt and possibly tossed.  Don't have any dual motor setup so can' t speak to the CANbus issues with it spinning out when one disconnects or whatever the case may be but it does seem if the 5V regulators are too far off from each other or the voltage supplied to them is too far off for some reason then they could be interpreting the same signal differently and like he says the mcu components they a no like the reverse polarity.

I ought to replace the cable between the ESC and receiver just for the sake of making it look nice, but as is I haven't had a problem I just used a the regular JST connections and hot glued them into the 3D printed plastic parts wrapping the VESC and receiver box.  Hot glue isn't usually great but it does stick to the plastic really well and since it can ooze into the containers a bit that helps.
```

---
## \#139 Posted by: Titoxd10001 Posted at: 2017-07-06T04:18:19.262Z Reads: 262

```
That meme is totally me right now. Was even saving money to make a large purchase. Things are not going well, had to pay late car registration and now this. FML. And the only reason I had my slave disconnected from power was to test my vesc 4.12 I had for sale 😅 guess I'm going to pony up the $100 I and see if the "wizard" can make things happen. 

@namasaki two receivers now we're talking. Have a bunch of gt2b receivers laying around lol
```

---
## \#140 Posted by: Jinra Posted at: 2017-07-06T04:38:45.548Z Reads: 262

```
Are they both throwing the DRV8302 error? What happened exactly?
```

---
## \#141 Posted by: Titoxd10001 Posted at: 2017-07-06T04:45:50.649Z Reads: 254

```
@johnnymeduse might know more but I connected one focbox then I connected the other focbox. Usually connect them at the same time in one go through xt90 antispark. Now they don't power on, no LEDs, but still send power to receiver and Bluetooth module, cant connect to pc.
```

---
## \#142 Posted by: Jinra Posted at: 2017-07-06T04:51:55.894Z Reads: 252

```
So you connected one, it turned on fine, then you plugged in the other one and they both are off?
```

---
## \#143 Posted by: Titoxd10001 Posted at: 2017-07-06T04:59:55.088Z Reads: 253

```
Yes and now they're both foced
```

---
## \#144 Posted by: Namasaki Posted at: 2017-07-06T05:17:34.607Z Reads: 257

```
So, does this mean that if your running dual vescs with canbus. and one of them fails, it will take it's brother down with it?
```

---
## \#145 Posted by: psychotiller Posted at: 2017-07-06T05:21:27.533Z Reads: 249

```
Danh Danh Dah!!! Good question..
```

---
## \#146 Posted by: TarzanHBK Posted at: 2017-07-06T05:28:49.651Z Reads: 250

```
Thats what happened with mine. No LEDs and no connection through USB..both vescs fried at the same time. Can chip dead on both.
```

---
## \#147 Posted by: Titoxd10001 Posted at: 2017-07-06T06:17:23.749Z Reads: 245

```
It sure feels like if one goes down they'll both go down with can bus. @ackmaniac do you know?


@tarzanhbk did they fry while connecting things or while riding. Were you able to resurrect them from the dead
```

---
## \#148 Posted by: TarzanHBK Posted at: 2017-07-06T06:22:50.864Z Reads: 253

```
I rode them without a problem, got back on my workspace, did a few things on the board - powered it up a few times and after that, i realised that the LED was off on both vescs, tried to connect them via USB but nothing. 

Like i said before, LP-electronics fixed them; replaced both can chips.
```

---
## \#149 Posted by: sebaszz Posted at: 2017-07-06T07:03:01.193Z Reads: 259

```
I had a loose ppm connector on the vesc 6 that also caused a full throttle runaway. 3 times before I discovered the issue.
So for safety I think there is no benefit  to use the splitter.
```

---
## \#150 Posted by: lock Posted at: 2017-07-06T07:37:52.405Z Reads: 264

```
Had a bit of a look at the [can bus stuff](http://www.ti.com/lit/ds/symlink/sn65hvd232.pdf) and it got me wondering why no one seemed to be using terminating resistors as per the docs.

<img src="/uploads/db1493/original/3X/b/a/ba8f4c5732517decb4f7b22e5a562465ed90f37c.png" width="649" height="268">

There's of course many advantages in open source, [being able to poke around](https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC_4.pdf) is one of them.
<img src="/uploads/db1493/original/3X/9/7/9778e3462286ec03a7b0f8976e545cd27981f3fb.png" width="461" height="333">
That R401 corresponds to a 100ohm resistor, which I guess is close enough to the 120ohm mentioned in the spec. So all VESCs have a terminating resistor built in. This is great if you're just connecting 2, but I reckon it might be a bit of an issue if you're stringing 4 together (ala @longhairedboy). This is a pretty uneducated hunch though, always happy to be told I'm wrong.
```

---
## \#151 Posted by: lock Posted at: 2017-07-06T08:05:07.250Z Reads: 259

```
[Relevant thread over on Endless Sphere](https://endless-sphere.com/forums/viewtopic.php?f=35&t=69381), can bus issues seem to go back a while...
```

---
## \#152 Posted by: longhairedboy Posted at: 2017-07-06T13:12:25.070Z Reads: 256

```
Maybe this will help.

<img src="/uploads/db1493/original/3X/7/f/7f992078da0d19ac52b87cc652672de93ae0da28.png" width="482" height="267">

Maybe I'll get some made at macrofab and pass them around for cheap. 

Only caveat is that for this to work properly we may need to remove R401, that's the same designator on both the standard 4.12 and the X. It can be done with a single iron, so you don't need anything special. Not 100% on that yet.
```

---
## \#153 Posted by: Nordle Posted at: 2017-07-06T14:27:48.625Z Reads: 260

```
Not so weird:) gnd is connected together already (battery input), else the pwm signal wouldn't have anything to compare with and therefore not work.
```

---
## \#154 Posted by: lock Posted at: 2017-07-07T02:43:00.464Z Reads: 254

```
Haha, love the name. And yeah, I'd be seeking expert opinion before pulling components off 4 VESCs. 

I'm not sure how much it matters as we're not looking at a 30m long can bus, but generally I think you'd aim to minimise the length of wire running from the bus wires to each of the nodes (VESCs). And bonus points if the bus wires are in a twisted pair config.
```

---
## \#155 Posted by: bigben Posted at: 2017-07-11T17:59:19.857Z Reads: 245

```
@chaka what is your current feeling on this? I was looking through old threads and I see you favoured a splitter. This was a couple of years back so as we know a lot had changed since then!
```

---
## \#156 Posted by: chaka Posted at: 2017-07-11T18:02:55.889Z Reads: 245

```
Yeah that was a long time ago, I use the canbus these days so I can get telemetry on the whole system.
```

---
## \#157 Posted by: psychotiller Posted at: 2017-07-11T18:43:33.873Z Reads: 245

```
So you're running master/slave or is their a way to run them teamed with canbus?
```

---
## \#158 Posted by: chaka Posted at: 2017-07-11T19:03:35.216Z Reads: 256

```
Yes, master>slave, sadist>masochist, Master>Blaster...;)

http://www.bluemaize.net/im/appliances/master-blaster-2.jpg
```

---
## \#159 Posted by: cwazy1 Posted at: 2017-09-02T18:11:40.666Z Reads: 234

```
is there any benefit to using signal + ground versus just signal on the parallel connection?
```

---
## \#160 Posted by: Namasaki Posted at: 2017-09-02T18:21:53.450Z Reads: 246

```
I don't know if it's necessary but I use signal and ground and it works
```

---
## \#161 Posted by: Pimousse Posted at: 2017-09-04T07:38:01.128Z Reads: 244

```
You mean for CAN connection ?

The rule is simple :
- VESCs powered by the same battery : NO ground connection, only CANH and CANL wires (middle of 4pin JST connector)
- VESCs powered by different batteries : ground connection REQUIRED.

This advice comes from Vedder himself ;)
```

---
## \#162 Posted by: Namasaki Posted at: 2017-09-04T12:01:10.537Z Reads: 240

```
You should read the post I was answering. 
We were talking about parallel ppm not canbus.
```

---
## \#163 Posted by: Pimousse Posted at: 2017-09-04T12:31:16.209Z Reads: 240

```
Sorry, but I don't see it.
Anyway, whether it's VESC 4.xx or VESC 6, Vedder strongly not recommends to use Y PPM cable.
On VESC 6 it may fry components (it happens to a beta guy, components are more sensitive than VESC 4 ones) if both VESCs are powered by the same battery pack.
CAN bus is the way to go. ;)
```

---
## \#164 Posted by: Nowind Posted at: 2017-09-04T13:05:11.807Z Reads: 236

```
[quote="Pimousse, post:163, topic:26461"]
On VESC 6 it may fry components (it happens to a beta guy
[/quote]

Yeah yeah i know this guy :wink:
```

---
## \#165 Posted by: Namasaki Posted at: 2017-09-04T13:48:52.219Z Reads: 236

```
I don't know about Vesc6. 
But as far as Vesc4 is concerned, it is perfectly safe to run parallel ppm. 
There are more than a few people doing it with no issues. 
I have been running parallel ppm for over a year with no issues. 
As long as you only supply 5v from one of the Vesc and not both to power the receiver. 
People have damaged their Vescs using canbus by powering one Vesc and not the other or by not powering them at the same time. Also by the canbus wire coming loose and by not getting the bldc tool settings just right. So canbus is not as safe as you think. 
There is a lengthy thread on this topic that is fairly recent.
```

---
## \#166 Posted by: Namasaki Posted at: 2017-09-04T13:51:21.912Z Reads: 237

```
[quote="Pimousse, post:163, topic:26461"]
Sorry, but I don't see it.
[/quote]

cwazy1
2d
is there any benefit to using signal + ground versus just signal on the parallel connection?

See he said parallel connection
```

---
## \#167 Posted by: Pimousse Posted at: 2017-09-04T14:55:44.705Z Reads: 234

```
Again, it's BV words who, I guess, is the best to have an idea about what is good or not with the VESC, ain't you agree ? ;)
See what Frank said few weeks ago :
http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461/85?u=pimousse
```

---
## \#168 Posted by: cwazy1 Posted at: 2017-09-04T16:40:58.699Z Reads: 232

```
The reason I'm planning to use split ppm is because my drv failed immediately after plugging in a canbus for dual motor configuration. 

See my thread here. 

http://www.electric-skateboard.builders/t/intermittent-drv8302-fault-code-from-initial-dual-motor-setup/32040/1

There was no obvious shorts, and I made no mistakes when connecting wires. I went through and programmed each vesc with the correct configurations as well as detection, then powered all down, and connected canbus.
```

---
## \#169 Posted by: BigBoyToys Posted at: 2017-09-04T17:23:40.435Z Reads: 223

```
Ive had problems with blowing CAN transceivers using both split ppm and CAN bus on 4wd setups. I just bought extra receivers and link them all to the same remote now. Add 4 bluetooth modules and they can all be tuned separately and wirelessly as well.
```

---
## \#170 Posted by: cwazy1 Posted at: 2017-09-04T20:13:49.041Z Reads: 228

```
When you blow a can transceiver, what fault does it show? Also how are you possibly blowing can transceiver with split ppm? You're not plugging anything into your can port? There was a thread recently about someone blowing their can transceiver and still be able to run split ppm afterwards.  

Mine was showing drv fault when I initially set it up through canbus

It looks like only the signal is required so I'll just run signal off one of the parallels
```

---
## \#171 Posted by: BigBoyToys Posted at: 2017-09-04T20:30:48.498Z Reads: 227

```
Depends,

Sometimes its lights out, sometimes the tranceiver just gets really hot. Never had codes though for a bad Transceiver though.
```

---
## \#172 Posted by: cwazy1 Posted at: 2017-09-04T20:36:11.526Z Reads: 224

```
Ah, I see.
```

---
## \#173 Posted by: Namasaki Posted at: 2017-09-05T00:28:29.864Z Reads: 225

```
[quote="Pimousse, post:167, topic:26461"]
Again, it's BV words who, I guess, is the best to have an idea about what is good or not with the VESC, ain't you agree ? :wink:
See what Frank said few weeks ago :
[/quote]

I do not agree simply because I personally have proven otherwise by running both of my Vesc 4.12 builds with split ppm for a long time with no problems.
And from what I've heard, there are more ways to damage the Vesc 4.12 with canbus than with split ppm.
I am not familiar with the Vesc6 so that is why I am referring only to the Vesc 4.12
```

---
## \#174 Posted by: psychotiller Posted at: 2017-09-05T02:54:38.138Z Reads: 216

```
Yeah, Split ppm works just fine. Not once have myself or anyone else I know locally burned out a vesc using split ppm. Same cannot be said for canbus.
```

---
## \#175 Posted by: Jinra Posted at: 2017-09-05T04:20:50.585Z Reads: 219

```
Frank can say anything he wants, but statistically, I've heard of more people frying something with CAN wayyyy more than split PPM. In fact I've never heard of anything frying with split PPM.

FYI, only the PPM wire is needed for split Y cable.
```

---
## \#176 Posted by: cwazy1 Posted at: 2017-09-05T04:35:17.123Z Reads: 213

```
ppm wire = signal wire = white wire ?
```

---
## \#177 Posted by: Jinra Posted at: 2017-09-05T04:57:07.151Z Reads: 217

```
yes, yes, and depends. Could be any color you're using.
```

---
## \#178 Posted by: thisguyhere Posted at: 2017-09-05T04:57:25.053Z Reads: 223

```
left and right most wires are PPM, middle one is 5v.

https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/9/59ce619a3e69ec59762b40bbc1930fae5a3e8390.jpg
```

---
## \#179 Posted by: Jinra Posted at: 2017-09-05T04:58:50.941Z Reads: 223

```
only 1 wire on a servo is for signal, middle is 5v as you said, and the other is ground.
```

---
## \#180 Posted by: Jinra Posted at: 2017-09-05T04:59:26.133Z Reads: 227

```
How I'm hooked up

<img src="/uploads/db1493/original/3X/0/2/02b2d6b456ce7274a667b4b3c5ebb961009d8dfe.png" width="382" height="481">
```

---
## \#181 Posted by: thisguyhere Posted at: 2017-09-05T04:59:55.006Z Reads: 223

```
oh damn, that works too?  sweet.
```

---
## \#182 Posted by: lrdesigns Posted at: 2017-09-05T05:20:52.857Z Reads: 222

```
I did mine like @Jinra 's diagram and been working good for me. Vesc 4
```

---
## \#183 Posted by: cwazy1 Posted at: 2017-09-05T05:49:23.771Z Reads: 229

```
OK, awesome, I should be good then. 

[url=https://ibb.co/mMShta][img]https://image.ibb.co/bSJYzF/image1.jpg[/img][/url]
```

---
## \#184 Posted by: skslingo21 Posted at: 2017-09-17T15:23:33.977Z Reads: 230

```
I will NOT run any of my VESC on split PPM.
Not saying it doesnt work, not saying it deep fries anything..

I first setup on split ppm(easiest)
-motor startups were off (not in sync)
-sometimes only one motor would spin...
-no traction control/rocks flying when tire lifts off the ground. 

Now the ppm signal goes to a switch. 
position 1 is PPM to master VESC
position 2 is PPM to slav VESC

Position 1 is dual drive, through can-bus.
The master handles the PPM from reciver and passes signal through can bus to slave. 

Position 2 is PPM to slave only. 
this allows only the slave to drive. 

If the slave motor/belt/VESC fails, I can remove the canbus connector and drive only the master without conflict. If master fails, i simply switch to slave only. 

I use the Traction Control function so if one motor is lost the other must be shut down to avoid rpm conflict. (rpm difference causes timeouts when on TC)
```

---
## \#185 Posted by: skslingo21 Posted at: 2017-09-17T15:35:05.297Z Reads: 226

```
If anyone has trouble setting up can-bus to dual VESC 4.xx please let me know and ill post a step by step.
```

---
## \#186 Posted by: Namasaki Posted at: 2017-09-17T15:55:02.295Z Reads: 233

```

"motor startups were off (not in sync)"
I've only noticed this while bench testing and barely nudging the throttle. 
If I pull more throttle, they start up together. 
Anyway, it is completely unnoticeable while riding. 

And if one of your wheels is lifting or loosing traction while turning, Then either your trucks are too tight or your bushings are too hard.
```

---
## \#187 Posted by: karma Posted at: 2017-09-17T20:02:24.855Z Reads: 237

```
Would love a step by step for setting it up. I am in the middle of deciding to go with a @Jinras' option or to go with CAN.
```

---
## \#188 Posted by: skslingo21 Posted at: 2017-09-17T21:43:14.111Z Reads: 241

```
Ive written out 14 simple steps for setting up dual VESC using CAN-bus with bldc tool. :persevere:
With VESC-tool, its one click of a button during the setup wizard :relieved:

Here are the steps I used to program two VESC to communicate through CAN bus.
Using the BLDC tool, and two 4.12 hardware VESC.

1.) Choose a master/slave ESC. label accordingly. 
2.) Open bldc tool and CONNECT to master ESC.
3.) open app configuration/general tab, and read config. 
4.) set controller ID to "0", save config. 
5.) Choose the appropriate tab for your control type(most will use ppm)
6.) Select the box that reads "multiple esc over can"
7.) save config. 
8.) Dissconnect Master, and CONNECT slave esc to bldc tool. 
9.) open app config/general tab and read config. 
10.) rename the controller ID "1" and select "send status over can" box. Dissconnect.
11.) Connect your canbus cable. I recommend the proper connector/jst-ph 2mm 4-pin
12.) Reconnect Master ESC to bldc tool and read config. 
13.) on the right side of bldc tool under the dissconnect button, select the slave controller ID (1) and select the CAN Fwd box. Write configuration, and dissconnect. 
14.) Reboot both VESCS and test controller, if only one motor spins, check to see that the "app config" settings for one VESC are the same as the other.
```

---
## \#189 Posted by: mmaner Posted at: 2017-09-19T17:42:23.551Z Reads: 234

```
[quote="skslingo21, post:188, topic:26461"]
12.) Select the box that reads "multiple esc over can"
[/quote]

Not on the slave, only the master
```

---
## \#190 Posted by: trampa Posted at: 2017-09-19T18:08:57.385Z Reads: 235

```
Long debate... 

When thinking about Y-PPM or CAN, you also should think of single battery or twin battery, each powering your ESC. Split battery is better for Y-PPM, since there is no common ground. This could even work on VESC Six.

@Pimousse mentioned it before and it's quite important to know, also for CAN setup.

There are pros and cons for both setups. 

Frank
```

---
## \#191 Posted by: skslingo21 Posted at: 2017-09-19T20:30:01.312Z Reads: 231

```
edited* ty 
Yes there are def benefits to both. 
Most wont need Traction Control which is the real benefit to setting up CAN-bus.
@Namasaki 
Its hard to keep the trucks loose for fine control when moving 40km/h top speed. When traveling over gravel/loose terrain is when the TC really shines. :grinning:
```

---
## \#192 Posted by: Namasaki Posted at: 2017-09-19T22:54:18.713Z Reads: 232

```
With the right after market bushings and pivot cups along with precision bushing washers, you can have decent maneuverability with stability.
Of course it also depends on your ability and endurance.
core balance, ankle and leg strength.
Ever notice how you seem to have less stability after riding a while.
Having your trucks too tight can get you in trouble when going fast on curvy roads.
```

---
## \#193 Posted by: Namasaki Posted at: 2017-09-20T03:03:05.596Z Reads: 231

```
[quote="trampa, post:190, topic:26461"]
Split battery is better for Y-PPM, since there is no common ground
[/quote]


How is running dual Vescs on a parallel power connection a problem when feeding them a parallel  ppm signal from the receiver?
How does having a common ground have anything to do with them both being fed with the same ppm signal?

I have never heard of anyone killing a Vesc4 with parallel ppm. As long as the receiver is powered by only one Vesc.

And running separate batteries. Think about that for a moment.
dual batteries
dual bms's
dual on/off switches
dual charge ports
dual voltage meters
and twice the wiring
Not very practical in my opinion.
```

---
## \#194 Posted by: longhairedboy Posted at: 2017-09-20T03:06:29.622Z Reads: 229

```
can bus yo. 

da fuck yall even talkin bout shiiiit

lblblblbllblblblblblblblblb just run that signal wire on over you don't have to worry about grounding
shut yo mouth. not a problem with can bus shit
```

---
## \#195 Posted by: longhairedboy Posted at: 2017-09-20T03:08:01.963Z Reads: 227

```
[quote="Namasaki, post:193, topic:26461"]
And running separate batteries. Think about that for a moment.
dual batteries
dual bms's
dual on/off switches
dual charge ports
dual voltage meters
and twice the wiring
Not very practical in my opinion.
[/quote]

dual fires lol
```

---
## \#196 Posted by: Namasaki Posted at: 2017-09-20T03:17:44.909Z Reads: 222

```
I didn't say there is a problem with canbus, I'm saying there is no problem with parallel ppm.
However, either one of them if not set up correctly can damage a Vesc.

BTW, glad to see that you survived your run in with Irma.
Hope you didn't suffer any loss.
```

---
## \#197 Posted by: longhairedboy Posted at: 2017-09-20T03:19:29.001Z Reads: 218

```
a shorted can bus will ruin your whole month for sure. 

i've been drinking. 

heavily.
```

---
## \#198 Posted by: cwazy1 Posted at: 2017-09-20T04:41:13.750Z Reads: 221

```
[quote="longhairedboy, post:197, topic:26461"]
i've been drinking. 

heavily.
[/quote]

yes we can tell.
```

---
## \#199 Posted by: Bloop Posted at: 2017-09-20T05:28:18.725Z Reads: 223

```
What about connecting one remote to 2 receivers?? I have 2 enertion nano x receivers laying around so could that work ?
```

---
## \#200 Posted by: cwazy1 Posted at: 2017-09-20T05:59:04.222Z Reads: 222

```
yes, just pair both receivers to your one controller.
```

---
## \#201 Posted by: Namasaki Posted at: 2017-09-20T06:11:15.945Z Reads: 221

```
I have done just that with the mini RC remote and it works. 
Don't know if it will work with nano remote
You'll just have to try it and see.
```

---
## \#202 Posted by: cwazy1 Posted at: 2017-09-26T19:05:12.712Z Reads: 221

```
Spent last night resoldering connections on my new focboxes and getting everything setup. 

I went with the split ppm route instead of can (previous dual TB vescs over can fried a drv instantly) 

I used only a signal wire into the second vesc. Both vescs were set up as master. Throttle min and max were the same on both vescs, but always verify it yourself through live reading. 

One of my motors was about 200 miles older than my other. So I had to set one motor at +60A max and another at +50A max to ensure both are spinning at the same rate.

Motor/battery settings were +50/-50/+15/-7 for each of the 6355's being powered on a 12s4p pack.

Working great so far. Torque is impressive and braking is sooo much better. Can actually come to a dead stop.
```

---
## \#203 Posted by: Colson003 Posted at: 2017-09-27T06:03:50.840Z Reads: 217

```
@cwazy1 I just ordered my second TB vesc and the can cable to connect them together. I don't want that to happen to me too. Was it just bad luck?
```

---
## \#204 Posted by: Jinra Posted at: 2017-09-27T06:09:37.590Z Reads: 218

```
make sure both VESCs have power if you're connecting CAN. If CAN is connected but only 1 VESC is powered, it'll blow up the can chip.
```

---
## \#205 Posted by: cwazy1 Posted at: 2017-09-27T07:20:04.799Z Reads: 220

```
If you want to be 100% sure you're not going to fuck up some can specific configuration, then go split ppm. It really comes down to luck. Unless you NEED traction control you're not exactly losing a lot and instead gain the confidence that you won't blow a chip. Also if one of your vesc fails while you're riding, you're not in master-slave configuration, you'll always have the other vesc to slow you down and get you home.
```

---
## \#206 Posted by: GrecoMan Posted at: 2017-09-27T11:39:01.742Z Reads: 216

```
You think it’d be possible to only use can for data like traction control but something else and then run split ppm for remote signal?  That way people that wanna use @Ackmaniac’s firmware could be happy but have less failures
```

---
## \#207 Posted by: Jebe Posted at: 2017-10-05T22:40:05.688Z Reads: 206

```
This may explain a few failures I've had. :confused:
```

---
## \#208 Posted by: gogomrrobot Posted at: 2017-10-15T13:13:59.640Z Reads: 199

```
what is the final world about this with Vesc6... i have canbus but debating y-splitter on second build.

Is @trampa stance no Y-cable with their product?
```

---
## \#209 Posted by: trampa Posted at: 2017-10-16T06:29:23.806Z Reads: 195

```
No Y. Y will always cause ground loops and should never be used in systems sharing a common ground. 
It is technically incorrect to connect PPM to two separate controllers. In consequence you should never do that. Better use two receivers  if you are desperate for twin PPM. 

Frank
```

---
## \#210 Posted by: cwazy1 Posted at: 2017-10-16T06:35:27.874Z Reads: 195

```
Seems like VESC6 has more sensitive parts and does not like split PPM, per frank's arguments if you read the thread.. Since there are not a lot of VESC6s out there, not many people have tested it out. 

On VESC with 4.x hardware, split ppm 100% so long as you clip a +5v
```

---
## \#211 Posted by: Jinra Posted at: 2017-10-16T06:36:22.693Z Reads: 195

```
My guess is that split Y would work fine on the 6 as well.
```

---
## \#212 Posted by: trampa Posted at: 2017-10-16T06:39:52.154Z Reads: 198

```
Y-PPM always causes ground loops. You don't want to set up you HW like that. 

Frank
```

---
## \#213 Posted by: bigben Posted at: 2017-10-16T06:45:04.644Z Reads: 203

```
I guess a poll would throw up some results as to who has blown up which vesc with which setup?
```

---
## \#214 Posted by: Crossfire Posted at: 2017-10-16T06:52:43.835Z Reads: 203

```
Loving canbus so far. Reliable and works like a charm.
```

---
## \#215 Posted by: Jinra Posted at: 2017-10-16T06:55:04.891Z Reads: 205

```
You say that, but ground doesn't even need to be hooked up on the second VESC, only the PPM wire needs to be.
```

---
## \#216 Posted by: Nordle Posted at: 2017-10-16T07:02:39.695Z Reads: 202

```
Can is better in any way, why are you so obsessed on splitting ppm?...
```

---
## \#217 Posted by: Jinra Posted at: 2017-10-16T07:07:48.007Z Reads: 209

```
how am i obsessed? this thread is literally asking ppm or split y. I never said one is better than the other and i don't believe either is.

I used can but it's very fickle on the connection and having a weak/severed connection causes can to behave erratically and unexpectedly. In my case it caused a wheel to go full throttle with no input. Another time it caused one wheel to stutter. And these incidences were with two different cables. Also breaking a belt on CAN may give you problems as well as @Titoxd10001 has experienced
```

---
## \#218 Posted by: Pimousse Posted at: 2017-10-16T09:47:13.463Z Reads: 203

```
Hi Frank,

I'm still wondering if my custom accessory board won't create the GNC loop as you say.
I posted on VESC project forum but I'm struggling having any answer : http://vesc-project.com/node/162
Somehow, it's the same as creating a GNC like Y cable, no?
So, may I get a confirmation stating I can go this way, and if not, what component should I add to avoid fry anything ?

Many thanks Sir !
```

---
## \#219 Posted by: Namasaki Posted at: 2017-10-16T11:33:04.503Z Reads: 203

```
[quote="Nordle, post:216, topic:26461, full:true"]
Can is better in any way, why are you so obsessed on splitting ppm?...
[/quote]

Split ppm is simple, safe and reliable. 
Canbus is complicated, dangerous and unreliable
More people have encountered issues with canbus than with split ppm

This is in reference to Vesc4,  not Vesc6
```

---
## \#220 Posted by: gogomrrobot Posted at: 2017-10-16T11:49:37.395Z Reads: 202

```
I used to use split PPM with Max6 ESC as that was the only option.

Now that I am on the VESC6, I find canbus super convenient... I only need to use the USB cable on one VESC to configure both VESC's settings.

I do understand your point on redundancy, fail-over.  But I haven't heard of canbus issues on specifically the VESC6 hardware.  I don't know about other versions of the hardware.  Also, as these things cost a good chunk of money, I just want to take it under advisement to use the method the vendor recommends -- to protect the warranty/investment. The vendor says no Y-PPM due to ground loop circuit then that is probably what advice I will follow.

If there are some canbus VESC6 issues, Trampa would surely resolve them, etc
```

---
## \#221 Posted by: Nordle Posted at: 2017-10-16T13:18:54.518Z Reads: 205

```
[quote="Namasaki, post:219, topic:26461"]
Split ppm is simple, safe and reliable. 
Canbus is complicated, dangerous and unreliable
[/quote]
Chosing one out of 3 wires is simple, and connecting 2 wires is complicated.. smart...
For me, no issues with both, only difference is that i have more funcionality with can.
```

---
## \#222 Posted by: Namasaki Posted at: 2017-10-16T14:09:58.200Z Reads: 202

```
When I spoke of simplicity, I was referring more to the software settings, not the wiring.
```

---
## \#223 Posted by: Namasaki Posted at: 2017-10-16T14:11:44.769Z Reads: 202

```
You are smart to follow Trampa's instructions for the sake of your warranty on Vesc6
```

---
## \#224 Posted by: longhairedboy Posted at: 2017-10-16T15:00:10.222Z Reads: 205

```
jake and i talk about this all the time. He likes split ppm and i like can busses. I prefer traction control and can fwding and minimal/organized wiring and he like breaking traction on one side to throw dirt  to irritate cyclists when they talk shit. Can't do that with traction control. 

honestly as far as wiring goes they're both dead simple easy to get right. Also easy to get wrong. But if you're at the point where you're wiring ESCs in your board then you are already aware of how wrong things can get on even the simplest tasks when you're not paying attention.
```

---
## \#225 Posted by: trampa Posted at: 2017-10-16T18:33:58.919Z Reads: 200

```
I'll point Benjamin at your schematics.

Frank
```

---
## \#226 Posted by: racidon Posted at: 2017-11-09T01:56:11.932Z Reads: 198

```
[quote="Jinra, post:211, topic:26461, full:true"]
My guess is that split Y would work fine on the 6 as well.
[/quote]

Spot the cash to replace my two and I'll test it for you :p

[quote="Jinra, post:217, topic:26461, full:true"]
how am i obsessed? this thread is literally asking ppm or split y. I never said one is better than the other and i don't believe either is.

I used can but it's very fickle on the connection and having a weak/severed connection causes can to behave erratically and unexpectedly. In my case it caused a wheel to go full throttle with no input. Another time it caused one wheel to stutter. And these incidences were with two different cables. Also breaking a belt on CAN may give you problems as well as @Titoxd10001 has experienced
[/quote]
To be fair wiring your motors to your ESCs incorrectly can also cause serious problems...
```

---
## \#227 Posted by: Jinra Posted at: 2017-11-09T03:58:18.227Z Reads: 186

```
You can wire wrong on both setups, not sure what you mean
```

---
## \#228 Posted by: racidon Posted at: 2017-11-09T04:00:16.628Z Reads: 196

```
[quote="Jinra, post:227, topic:26461, full:true"]
You can wire wrong on both setups, not sure what you mean
[/quote]

You're fear of can you said was due to how bad it can be when wired incorrectly or even when shit breaks between the bus, what I'm saying is that the same can be said about motor to ESC too, it's just how it all works :(
```

---
## \#229 Posted by: Jinra Posted at: 2017-11-09T06:36:14.271Z Reads: 196

```
I never talked about wiring it wrong. I've had my CAN connection be "semi-connected" because the wire frayed or the connection was loose. This caused very odd behavior where 1 wheel would spin by itself and the other wouldn't, or it'd have other weird behavior. If a split Y frays, you just dont get response to that wheel.
```

---
## \#230 Posted by: racidon Posted at: 2017-11-09T21:17:42.577Z Reads: 195

```
[quote="Jinra, post:229, topic:26461, full:true"]
I never talked about wiring it wrong. I've had my CAN connection be "semi-connected" because the wire frayed or the connection was loose. This caused very odd behavior where 1 wheel would spin by itself and the other wouldn't, or it'd have other weird behavior. If a split Y frays, you just dont get response to that wheel.
[/quote]

As I said below, not saying Y isn't a good choice. But  I get what you mean :slight_smile: 

[quote="racidon, post:228, topic:26461, full:true"]
[quote="Jinra, post:227, topic:26461, full:true"]
You can wire wrong on both setups, not sure what you mean
[/quote]

... or even when shit breaks between the bus...
[/quote]
```

---
## \#231 Posted by: thisguyhere Posted at: 2018-03-17T17:42:17.820Z Reads: 175

```
[quote="Namasaki, post:70, topic:26461"]
Here’s an idea based on what you said:

One remote paired with 2 separate receivers connected to 2 seperate Vescs.
[/quote]

hey @Namasaki i finally tried this because i noticed a small delay with the split ppm and getting poor signal at very low speed while walking / running two small dogs.

anyway, scavenged a receiver from an extra remote and it's WAY better responding than the split PPM.

but now i have a small problem with remotes without receivers so wanted to get extra receivers.

only receivers on their own i could find on banggood is $17 just for the receiver so looking elsewhere for a cheaper option.

found these 2.4ghz receivers on aliexpress, but just wondering if they'd be compatible with the 2.4ghz mini (product description says they're for gtb2 and its variants).

https://www.aliexpress.com/item/5PCS-LOT-Flysky-FS-GR3C-GR3C-FS-GR3E-GR3E-3CH-2-4Ghz-Receiver-For-FS-GT3B/32231952259.html
```

---
## \#232 Posted by: Namasaki Posted at: 2018-03-17T18:23:52.844Z Reads: 176

```
Those receivers from Aliexpress are $26.86 and I don't know if they are compatible.
You can buy the Mini remote with receiver from eBay for $17.59 with free shipping
Anyway, it's a good idea to have extra transmitters in case the one your using gets lost or damaged during a fall.
https://www.ebay.com/itm/2-4GHz-Radio-Remote-Controller-w-Receiver-Binding-Plug-for-Electric-Skateboard/263054079597?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D20131003132420%26meid%3D47bb037213004404b160c94c7baa9171%26pid%3D100005%26rk%3D1%26rkt%3D6%26sd%3D232284516689%26itm%3D263054079597&_trksid=p2047675.c100005.m1851
```

---
## \#233 Posted by: thisguyhere Posted at: 2018-03-17T18:44:46.585Z Reads: 168

```
yea it's $27 for 5 receivers though. 

ok I won't risk it then, just have some extras lying around, no worries.
```

---
## \#234 Posted by: bigben Posted at: 2018-03-17T18:47:31.937Z Reads: 172

```
They're gt3b receivers? Someone must have them and see if they can pair them with the mini remote. Pretty sure we managed to do this when we were testing @Russell23 vesc and battery a while back?
```

---
## \#235 Posted by: Namasaki Posted at: 2018-03-17T18:57:35.487Z Reads: 178

```
Ok, I misread the site.
```

---
## \#236 Posted by: Sebike Posted at: 2018-03-17T23:09:53.966Z Reads: 180

```
https://www.electric-skateboard.builders/t/support-your-bro/47957/48?u=sebike

Edit; Oh... you were after mini receivers..
```

---
## \#237 Posted by: ATLesk8 Posted at: 2018-03-17T23:22:03.159Z Reads: 181

```
Using a split PPM cable; is it ok to have both 5V wires going to the receiver? I think I remember someone saying that iy should only have one power wire.
```

---
## \#238 Posted by: thisguyhere Posted at: 2018-03-17T23:54:49.402Z Reads: 192

```
[quote="Sebike, post:236, topic:26461"]
Oh… you were after mini receivers
[/quote]

right, but the question is do these receivers work for both...?

[quote="ATLesk8, post:237, topic:26461"]
I think I remember someone saying that iy should only have one power wire.
[/quote]

yup, cut one of the 5v:

http://www.electric-skateboard.builders/t/how-should-i-go-about-programming-double-vesc/19731/20
```

---
## \#239 Posted by: ATLesk8 Posted at: 2018-03-18T01:29:17.153Z Reads: 185

```
What happens if you don't?
```

---
## \#240 Posted by: thisguyhere Posted at: 2018-03-18T01:46:52.725Z Reads: 190

```
http://www.electric-skateboard.builders/t/how-should-i-go-about-programming-double-vesc/19731/17?u=thisguyhere
```

---
## \#241 Posted by: Zacky Posted at: 2018-06-06T13:28:19.853Z Reads: 168

```
![20180606_210504|281x500](upload://Ag8R8QU6Ctqt2kTPovrActwomma.jpg)
```

---
## \#242 Posted by: banjaxxed Posted at: 2018-06-06T15:50:58.806Z Reads: 165

```
I'm not done with canbus slave control but due to a short of the sensors on my master the slave actually exploded inside its case, really exploded charred remains

It's all I could put it down to...master is fine..sizzle like a fuse burning followed by a huge bang almost worth the experience!
```

---
## \#243 Posted by: onepunchboard Posted at: 2018-06-06T17:22:22.432Z Reads: 160

```
Sounds... fun?! 
 When I got my first android phone I droped from second floor to polished granite tile of first floor landed on display side. with huge sound it exploded inside. funny enoungh glass of screen was not cracked.
eventually it started smoke and cought on fire. it was painful but worth it.
```

---
## \#244 Posted by: banjaxxed Posted at: 2018-06-06T18:55:10.839Z Reads: 158

```
I have always liked a good explosion and although it has set me back a little, I learned something and can build it into the total cost of ownership.

I have not found an example of the same thing via searchand it has me wondering a little since a shorted sensor wire *should* be fairly common
```

---
## \#245 Posted by: lrdesigns Posted at: 2018-06-07T00:53:56.709Z Reads: 158

```
[quote="banjaxxed, post:242, topic:26461"]
really exploded charred remains
[/quote]

Got pics?  .
```

---
## \#246 Posted by: Deckoz Posted at: 2018-06-07T01:04:16.302Z Reads: 159

```
[quote="banjaxxed, post:244, topic:26461"]
shorted sensor wire *should* be fairly common
[/quote]

It had to have shorted on the ground, as Halls, temp and voltage will all just make each other fluctuate with erroneous readings?
```

---
## \#247 Posted by: banjaxxed Posted at: 2018-06-07T10:44:21.414Z Reads: 157

```
sure do!
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5342?u=banjaxxed
```

---
## \#248 Posted by: banjaxxed Posted at: 2018-06-07T10:46:58.401Z Reads: 157

```
I would suspect you are very right, unfortunatly I did not inspect the sensor cable before dismantling it.

I don't have the knowledge how that damage could cause the master to be able to explode the slave via a canbus signal
```

---
## \#249 Posted by: SORRENTINO Posted at: 2018-06-07T17:15:00.759Z Reads: 153

```
Ah you have the old vesc on FOC? Probably more so that the old vesc is shitty unreliable garbage lol. Just my opinion from seeing a few go for no reason at all within my group of friends that ride lol. @Deckoz knows what im talking about.
```

---
## \#250 Posted by: banjaxxed Posted at: 2018-06-07T17:23:19.177Z Reads: 152

```
I bought another one that has a small problem, will give it one more try when(if) I fix it

Failing that 3dservisas send me two single focbox cases as backup
```

---
## \#251 Posted by: Skunk Posted at: 2018-07-20T15:07:34.855Z Reads: 130

```
Started reading this to figure out if I wanted to go can bus or Y split. I'm less sure then when I started lol
```

---
## \#252 Posted by: sayekim Posted at: 2018-07-20T15:32:02.218Z Reads: 131

```
It’s simple if you ask yourself do you want to have a bluetooth module for readings on your phone (if you wish to monitor both esc with metr pro). 
If the answer is yes go canbus. Otherwise it doesn’t matter unless you want traction control, then you still need to go canbus.
```

---
## \#253 Posted by: Skunk Posted at: 2018-07-20T15:48:14.028Z Reads: 126

```
I would assume having it connect your phone would allow you to monitor your systems?
I just don't wanna hurt my focbox
```

---
## \#254 Posted by: PatRocks Posted at: 2018-07-20T15:52:44.777Z Reads: 126

```
Then split! Error rates for CAN/split are as one-sided as fire rates for Liion/Lipo (in esk8 anyway) HA
Edit: shutup self, that's not funny
```

---
## \#255 Posted by: Skunk Posted at: 2018-07-20T15:56:27.058Z Reads: 127

```
Okay. I'lll have to make sure I read up on exactly how to do a split. 

*everything is funny,  everything
```

---
## \#256 Posted by: craigthemachine Posted at: 2018-07-20T16:01:43.382Z Reads: 125

```
Just buy a split PPM cable. Connect to both Focbox. Double check and make sure one doesn’t ground out the other.
```

---
## \#257 Posted by: PatRocks Posted at: 2018-07-20T16:01:44.192Z Reads: 122

```
Universal truth. Another: anything's a dildo if you're brave enough (my favorite thing to say). 

Back on track, y piece is easy. Disconnect one of the +5v in a safe and insulated way so that you can connect it again if needed.
```

---
## \#258 Posted by: craigthemachine Posted at: 2018-07-20T16:06:22.301Z Reads: 122

```
Exactly ! , If you really really really don’t want issues with DIY Eskate.. buy a bicycle. Other than that, enjoy the adventure and bring your wallet !
```

---
## \#259 Posted by: Skunk Posted at: 2018-07-20T16:08:16.955Z Reads: 127

```
I don't even know what +5v is lol. I've still got alot of reading to do. 
Very mechanically inclined and I've worked on cars for a long time but typically 60s and 70s stuff, I've  avoided electrical stuff like the plague. 
Everything except for the fact that these are skateboards is outside of my comfort zone.
```

---
## \#260 Posted by: PatRocks Posted at: 2018-07-20T16:11:41.700Z Reads: 123

```
The pwm consists of 3 wires: black white and red. Ground, signal and 5v positive respectively. Two focbox equals 6 wires. Subtract one red and you're all set
```

---
## \#261 Posted by: craigthemachine Posted at: 2018-07-20T16:11:58.717Z Reads: 129

```
![image|375x500](upload://qMuNTYyQYVwgmbchEtFTeipVaLZ.jpeg)https://www.electric-skateboard.builders/uploads/db1493/original/3X/4/9/49e97d871a6c8eaae5e00cd59cd5320d7774ab0c.jpeg 

The red wire. Notice one is missing. You only need power from one Focbox to the receiver.
```

---
## \#262 Posted by: Skunk Posted at: 2018-07-20T16:17:40.322Z Reads: 128

```
All makes sense now.  Thanks guys
```

---
## \#263 Posted by: PatRocks Posted at: 2018-07-21T00:23:07.299Z Reads: 125

```
By the way, if you're still in the market for a remote, I have the benchwheel and it's awesome. It has two channels set up so that you can run both pwm cables for two different escs without any modifications
```

---
## \#264 Posted by: Skunk Posted at: 2018-07-21T00:32:38.368Z Reads: 127

```
I do still need a remote, I was shooting for the benchwheel actually @PatRocks
```

---
## \#265 Posted by: PatRocks Posted at: 2018-07-21T00:35:18.142Z Reads: 125

```
People have had trouble ordering them and not specifically ordering BOTH the transmitter and receiver, be careful to check that. It can be a pain to pair them, but once configured that's a good remote
```

---
## \#266 Posted by: Skunk Posted at: 2018-07-21T00:46:32.792Z Reads: 123

```
Yeah I've been having a hard time finding any in stock. Would I be running one or two receivers?
```

---
## \#267 Posted by: PatRocks Posted at: 2018-07-21T01:03:13.361Z Reads: 126

```
I don't know if you _can_ pair two receivers. @mmaner ?
```

---
## \#268 Posted by: mmaner Posted at: 2018-07-21T01:12:33.347Z Reads: 124

```
I don't think you can use 2 receivers but the RX has 2 PPM connections.
```

---
## \#269 Posted by: Skunk Posted at: 2018-07-21T02:00:55.292Z Reads: 124

```
Is the RX a type of receiver?
```

---
## \#270 Posted by: PatRocks Posted at: 2018-07-21T02:12:15.675Z Reads: 128

```
It's an abbreviation for receiver. Tx is transmitter. you can plug both pwm connectors into the single Rx, without disconnecting any red 5v wires. Then, you can power one esc off and still power the Rx without plugging/unplugging pwm's (like for programming)
```

---
## \#271 Posted by: TarzanHBK Posted at: 2018-07-25T08:09:37.370Z Reads: 124

```
[quote="PatRocks, post:257, topic:26461"]
anything’s a dildo if you’re brave enough
[/quote]

that just hit my best-quotes-of-the-week hitlist :smiley:
```

---
## \#272 Posted by: PatRocks Posted at: 2018-07-25T09:31:09.872Z Reads: 122

```
Thank you, I can't believe this is the first feedback I've gotten for that statement.
```

---
## \#273 Posted by: lrdesigns Posted at: 2018-07-26T05:06:19.016Z Reads: 114

```
[quote="PatRocks, post:260, topic:26461, full:true"]
The pwm consists of 3 wires: black white and red. Ground, signal and 5v positive respectively. Two focbox equals 6 wires. Subtract one red and you’re all set
[/quote]

Actually you only need the signal (white) on the second esc.
```

---
## \#274 Posted by: PatRocks Posted at: 2018-07-26T06:24:45.235Z Reads: 112

```
What did I say differently? I suck at words sometimes
```

---
## \#275 Posted by: ElectricCoast Posted at: 2018-09-28T12:01:38.342Z Reads: 93

```
What type of cable is the canbus cable guys?
```

---
## \#276 Posted by: chrischo1996 Posted at: 2018-09-28T12:36:11.096Z Reads: 90

```
Looks like [this](https://flipsky.net/collections/accessories)
Just two wires that connect the middle two pins of the "can" port
```

---
## \#277 Posted by: Andy87 Posted at: 2018-09-28T13:47:12.822Z Reads: 88

```
Same like your sensor wires just 4pin 2mm jst (from which you need only the middle two)
```

---
## \#278 Posted by: ChicagoSkater Posted at: 2018-09-28T13:54:01.234Z Reads: 88

```
You can pair two receivers; I have 2 mini remotes, but both receivers are paired to 1 remote. Essentially functions as two, single drive VESCs.
```

---
## \#279 Posted by: DAddYE Posted at: 2018-09-28T15:06:56.638Z Reads: 85

```
I’m still not sure about Y cables. Is still a problem with FSVesc 6.6? If you cut the red cable and the vesc with the power dies the rx will not have power no? What’s the point then?
```

---
## \#280 Posted by: PatRocks Posted at: 2018-09-28T19:36:46.521Z Reads: 82

```
In the quoted text, I was referring specifically to the benchwheel remote! I don't think you can do it with the BW
```

---
## \#281 Posted by: ChicagoSkater Posted at: 2018-09-29T00:25:02.376Z Reads: 74

```
Ah I missed that, my bad!
```

---
