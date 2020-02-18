# VESC &#124; Smooth acceleration from a stand still

### Replies: 57 Views: 10322

## \#1 Posted by: longhairedboy Posted at: 2016-01-08T23:17:43.829Z Reads: 652

```
Since I'm new to configuring VESC and didn't see anything specific about this, i thought i'd start a thread for it for myself and anyone else. 

I want to start from a stand still without kicking, but it seems like my motors are just jittering as i slowly pull the trigger. When i kick and squeeze, its fine. But i want to not have to kick.  How do i do this? I'm not running sensored motors, so is it possible without them?

I've got twin R-SPEC 6355s on here  and I'm using FW 2.7 FOC.
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-01-09T00:45:49.784Z Reads: 646

```
That's interesting. I've never used a vesc, but I thought one of it's selling points was good startup torque using a special algorithm. Maybe the algorithm doesn't apply to foc.
```

---
## \#3 Posted by: treenutter Posted at: 2016-01-09T01:30:20.229Z Reads: 638

```
@longhairedboy I'm not the resident VESC expert, but I've been using one for a few months and with single motor I have always been able to take off from a standstill with only the tiniest bit of "jitter" when using the motor in "BDLC" mode. I'm assuming you've run the config for each motor already, correct?

Just last night I started using FOC mode and it's the smoothest startup I've ever experienced. If you haven't tried FOC already, start there!

You can bump up the "startup boost" value a tiny bit and that might get you moving from a standstill more easily.

Also, are you giving the throttle enough juice to get moving? I've found that w VESC the throttle curve is very progressive. Can you get moving if you "gun it" a little more?
```

---
## \#4 Posted by: cmatson Posted at: 2016-01-09T01:35:13.976Z Reads: 616

```
Huh, I can start from a standstill no problem with the VESC and a single enertion 6355.

I'll post a video this weekend (if I get to it)
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-01-09T01:47:35.679Z Reads: 610

```
ok Sorry for the false alarm! 

I was just too terrified to squeeze the trigger enough. I admit it. This build scares me. lol

Luckily i got a full face motorcycle helmet recently for free.
```

---
## \#6 Posted by: treenutter Posted at: 2016-01-09T01:59:27.154Z Reads: 605

```
@longhairedboy I've found the "Soft RPM Limit" in VESC (in the PPM tab) to be a huge help when I'm testing. By default it's set without an effective limit, so bringing it down (I use 25K-30K) means full throttle won't be a scary speed. Then you can crank it higher once you've got everything resolved.
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-01-09T02:21:48.628Z Reads: 603

```
soooooo sweeeeeeeetttttt

https://www.instagram.com/p/BATSHjkBBuV/?taken-by=longhairedboy

@treenutter i'll check that out. Thanks for the tips!
```

---
## \#8 Posted by: trbt555 Posted at: 2016-01-09T06:22:10.821Z Reads: 576

```
@treenutter which steps did you follow to set up FOC ?
It's only after your post yesterday that I realized FOC also works for sensorless motors !
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-01-09T16:00:44.082Z Reads: 566

```
i havn't yet. i tried simply enabling it but that was a terrible idea. thy just went in all different directions and stuttered.  I'm not sure yet what values go where for FOC on these, i'm still digging around. 

if anyone has known good FOC settings for Enertion's 6355 190kv, post them here. I would like to export a known good XML file with FOC enabled and anything else setting wise that can sweetly tune these motors to buttery goodness.
```

---
## \#10 Posted by: cmatson Posted at: 2016-01-09T16:05:23.174Z Reads: 554

```
[quote="longhairedboy, post:9, topic:947"]
if anyone has known good FOC settings for Enertion's 6355 190kv, post them here.
[/quote]

I think either OKP or WhitePony from ES have used FOC with dual R-Specs, so I might check their build threads too.
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-01-09T17:07:20.381Z Reads: 536

```
also i'd like to hear about or even see for myself what's possible with these in combination with VESC. 
product/electric-skateboard-motor-6355-230kv-2650w/

@torqueboards basically has racing motors on his site on sale.
```

---
## \#12 Posted by: Blasto Posted at: 2016-01-09T17:46:21.423Z Reads: 527

```
@longhairedboy Slowly working on that, patiently waiting for onloops wood-cf deck and doing some layout mods to the vesc to directly use the motor sensor without changing the connector. All this bldc controller research i've been doing convince me that i need a eboard.

<img src="/uploads/db1493/original/2X/9/9d614db03bb7bc096011837b560a7a6a27715883.jpeg" width="281" height="500">


<img src="/uploads/db1493/original/2X/0/072f664769f392ade156be16b0dab6a782eb9d99.jpeg" width="329" height="500">
```

---
## \#13 Posted by: trbt555 Posted at: 2016-01-09T17:47:34.204Z Reads: 501

```
[Here] [1] is a post by okp on ES with the steps to setup the FOC parameters.
Tried it on the R-Spec @12S : failed. Back to BLDC mode.
I don't feel like mucking about in all these settings without knowing what I'm doing so either I start reading up on FOC or I wait till some friendly soul finally figures out how to do it and posts a decent step by step tutorial.
I don't even know if it's worth it. Less noise ? Don't care.
More efficient like in better range ? Do care.


  [1]: https://endless-sphere.com/forums/viewtopic.php?f=35&t=71511&p=1136665&hilit=Foc#p1136665
```

---
## \#14 Posted by: psychotiller Posted at: 2016-01-09T18:03:24.422Z Reads: 497

```
I just ran the tests then applied the settings that the program discovered.  Once that was done my board was amazingly quiet and will now barely stutter at all when starting from a standstill.  Breaking is quiet too.
```

---
## \#15 Posted by: trbt555 Posted at: 2016-01-09T18:42:28.807Z Reads: 500

```
@psychotiller in which order did you run the tests ?
When I try to measure R & L I get an error "R is zero, measure it first".
```

---
## \#16 Posted by: treenutter Posted at: 2016-01-09T18:58:20.463Z Reads: 494

```
@trbt555  Sure. I'll list the steps I took when I'm back at my "bench."
```

---
## \#17 Posted by: treenutter Posted at: 2016-01-09T18:58:58.417Z Reads: 490

```
I had pretty much the same experience. But I think I need some tweaking to get the brakes just right.
```

---
## \#18 Posted by: psychotiller Posted at: 2016-01-09T20:20:14.730Z Reads: 483

```
I did the steps in order of appearance. Top to apply button
```

---
## \#19 Posted by: elkick Posted at: 2016-01-09T20:36:13.953Z Reads: 483

```
How long are the battery cables between capPCB pads and your battery? They should not be longer than 20cm for FOC, I had the same error (and some more) when the cables where to long. BLDC is less sensitive though.
```

---
## \#20 Posted by: Jack Posted at: 2016-01-09T21:30:26.400Z Reads: 473

```
@elkick would the effect of long battery cables be reduced if using more capacitors in parallel?
```

---
## \#21 Posted by: elkick Posted at: 2016-01-09T21:34:45.064Z Reads: 445

```
I think it would reduce unwanted ripple current to increase the 2000µF caps to a higher value, but I'm not sure if the VESC would perform normally, I never tried it.
```

---
## \#22 Posted by: Jack Posted at: 2016-01-09T21:41:15.606Z Reads: 434

```
My board flexes a lot so I want to put the battery pack at the front of the board and run braided cable underneath the grip tape so I'm looking at a length of around 1m, I suppose I should test this before putting the board together!
```

---
## \#23 Posted by: cmatson Posted at: 2016-01-09T21:45:15.696Z Reads: 427

```
I ran a battery from the front of my board to the back, and didn't have any problems. 

If you look at some of the DIY boosted boards on ES, they run their cables from front to back and I know I've seen a couple using VESC's.
```

---
## \#24 Posted by: elkick Posted at: 2016-01-09T21:52:56.429Z Reads: 416

```
Are they using FOC? It's no problem with BLDC, but I tested it with different VESCs and long cables (40cm) with FOC, no luck at all.
```

---
## \#25 Posted by: Jack Posted at: 2016-01-09T21:56:35.076Z Reads: 408

```
Yeah I want all this FOC goodness!
```

---
## \#26 Posted by: longhairedboy Posted at: 2016-01-09T23:25:36.836Z Reads: 406

```
my battery cables are definitely less than 20cm. However, WTF do the battery cables have to do with it? I would understand if maybe we were talking about phase wires, but source power cable lengths make a difference?
```

---
## \#27 Posted by: trbt555 Posted at: 2016-01-10T08:18:49.920Z Reads: 406

```
@elkick my cables are certainly longer than 20cm so that may be the problem. 

Please excuse my scepticism but I would like to hear some objective opinions from real life experience why FOC would be better than BLDC on an e-skate.
At the moment it all seems like much ado about nothing, really.
```

---
## \#28 Posted by: elkick Posted at: 2016-01-10T10:07:57.244Z Reads: 400

```
Quoting Benjamin:
"Don't expect any magic from FOC. You will hear a big difference in sound, but you are not likely to gain any noticeable difference in efficiency. The FETs will most likely get warmer and the motor efficiency might increase a bit a low speed, which can be good for hub motors and ebikes. Also, the top speed (or motor kv) will get lower with FOC with a factor of sqrt(3) / 2 or 0.866 since the modulation is a bit limited when full sine waves are modulated. With a three shunt version of the VESC the modulation could be increased to 100%, but that means that the commutation at full speed will be trapezoidal, the same as bldc. Another way to increase the top speed is using field weakening, but I don't know how well that works and how efficient that is on our motors. The difference in sound is really worth FOC for me though :-)"
```

---
## \#29 Posted by: trbt555 Posted at: 2016-01-10T10:59:40.546Z Reads: 392

```
So basically the only real difference is less sound and hotter FET's.
I'm sticking with BLDC.
```

---
## \#30 Posted by: longhairedboy Posted at: 2016-01-10T14:20:26.014Z Reads: 381

```
better sound isn't much of an improvement. They already sing my favorite song. 

So we now have three bullet points that are great on paper and mean ~nothing on the street:

 - regenerative braking
 - traction control
 - FOC

However, whatever they are doing is hella better than any other ESC i've ever used.
```

---
## \#31 Posted by: donblub Posted at: 2016-01-10T14:39:30.751Z Reads: 367

```
Does anyone know which of the two options is set the Raptor?
```

---
## \#32 Posted by: longhairedboy Posted at: 2016-01-10T14:55:09.574Z Reads: 376

```
probably BLDC since there is a lack of documentation on properly setting up FOC with Enertion R-SPECS. @onloop is great about sharing his findings, so i suspect there are no findings yet from his camp, or they are still being gathered. 

And after test riding this build for the past two days i suspect there's no rush. Its already sooo good in BLDC mode.
```

---
## \#33 Posted by: treenutter Posted at: 2016-01-10T22:08:46.870Z Reads: 376

```
@longhairedboy @trbt555 I think that FOC might be a matter of preference in terms of what it means on-the-street. In early testing I'm experience much better low-speed control and smoother startups. Silent operation (if it doesn't come with a major performance hit) is a big benefit in my usage. I ride amongst other people and I definitely prefer the quiet operation. All just preference, but I think it's fair to call FOC legit a benefit of VESC, especially over other ESCs that can be neighborhood-waking loud at times. Now to see if I can actually perfect it in implementation :)
```

---
## \#34 Posted by: onloop Posted at: 2016-01-10T22:35:26.691Z Reads: 370

```
Am still deciding... I've got a few more days until the new remotes arrive and i have to ship the Raptors. So I will be testing to see if there's any benefits having the FOC for raptor...

if the start-up performance is better it is worth it... but the startup is already very good....
```

---
## \#35 Posted by: longhairedboy Posted at: 2016-01-10T22:58:42.415Z Reads: 361

```
Agreed. ITs already quieter than the road noise on most pavement, and the startup is already good. 

I'm just not sure i want any more heat in my boxes. no fans, no sinks, and no ventilation means they need to operate cooler, but i definitely want to try it out.
```

---
## \#36 Posted by: cmatson Posted at: 2016-01-10T23:10:28.089Z Reads: 374

```
[quote="longhairedboy, post:35, topic:947"]
I'm just not sure i want any more heat in my boxes. no fans, no sinks, and no ventilation means they need to operate cooler
[/quote]

agreed, I'm in the same boat.

And as you mentioned before the whining up sound of the R-Spec's is actually pretty sweet, so I don't mind it very much :smile:
```

---
## \#37 Posted by: trbt555 Posted at: 2016-01-11T11:54:14.972Z Reads: 378

```
I also like the whine. People hear me coming, no surprises, added safety.
```

---
## \#38 Posted by: Jonsme Posted at: 2016-10-10T16:01:54.910Z Reads: 301

```
Any tips on installing a VESC on one of these: Magneto [Electric Longboard ](https://magnetoelectricskateboard.com/) 
Thanks in advance.
```

---
## \#39 Posted by: Eboosted Posted at: 2017-01-29T05:21:07.038Z Reads: 272

```
I read a lot of threads trying to smooth out the acceleration from stand stills but they all end up talking about something else.

Are there any settings or tricks on the VESC we could set in order to accomplish butter smooth acceleration from a dead stop?

Maybe I'll give sensors a try but for now couid anyone suggest to try something?
```

---
## \#40 Posted by: longhairedboy Posted at: 2017-01-30T20:51:44.924Z Reads: 265

```
sensors definitely help. Here my son is starting from a standstill at the bottom of a ditch filled with gravel and sand and leaves:

https://www.instagram.com/p/BPsYgt6gIoL/?taken-by=longhairedboy

super smooth, even in those shitty conditions. And there's nothing special going on in the VESC settings, just ran motor detection on my new sensored motors. 

https://www.instagram.com/p/BOnF4h9gYEk/?taken-by=longhairedboy
```

---
## \#41 Posted by: Bender Posted at: 2017-01-30T21:10:17.032Z Reads: 251

```
Nothing beats a sensored motor for a smooth start from standstill. Period.
```

---
## \#42 Posted by: IDVert3X Posted at: 2017-01-30T21:49:01.499Z Reads: 249

```
Another rebranded motor?

Thats getting funny, many people selling the same product under their brand 😂
```

---
## \#43 Posted by: Hummie Posted at: 2017-01-30T21:52:15.507Z Reads: 241

```
putting your vesc motor amp limits at 200 does starting from stop with no cogging for me.
```

---
## \#46 Posted by: longhairedboy Posted at: 2017-01-31T15:11:53.888Z Reads: 232

```
 

i definitely had a good laugh when i realized how silly i was NOT getting my own branded motors when I can get them at half retail AND with my logo etched on them and with keyways and snap ring grooves and sensors and exactly the phase lead length I want. I bought about 30 R-SPECs last year. So yeah, i'm giggling too.
```

---
## \#48 Posted by: Randyc1 Posted at: 2017-01-31T18:16:53.234Z Reads: 223

```
Are those Maytech Motors ?

What KV are they ?
```

---
## \#49 Posted by: longhairedboy Posted at: 2017-01-31T19:15:55.844Z Reads: 217

```
Maytech made them for me, yes. 190kv, under the name TOTALLY BITCHIN' 190KVS

and so far, they have in fact been totally bitchin'.
```

---
## \#50 Posted by: JohnnyMeduse Posted at: 2017-01-31T19:25:00.886Z Reads: 212

```
Does the RED give you more speed per torque? 😉
```

---
## \#51 Posted by: longhairedboy Posted at: 2017-01-31T19:27:43.249Z Reads: 211

```
Yes, absolutely. 20% performance bump over the exact same motor in any other color. 

It's also important to know that LASERS were involved in making these. 

FRICKIN' LASERS.
```

---
## \#52 Posted by: Randyc1 Posted at: 2017-01-31T23:10:54.293Z Reads: 204

```
Nice Motors !
```

---
## \#53 Posted by: Eboosted Posted at: 2017-02-01T08:06:39.349Z Reads: 202

```
I installed the sensors today, OMG I have completely brand new board again!
```

---
## \#54 Posted by: Randyc1 Posted at: 2017-02-01T10:18:27.035Z Reads: 195

```
Do you recall a Member here had a thread about an Identical Maytech  Baseplate (mounting plate) as your motors, that were allways Breaking , do you know if the problem was resolved ?

Are you willing to share a link of your Maytech source?

Thanks.
```

---
## \#55 Posted by: longhairedboy Posted at: 2017-02-01T13:18:03.723Z Reads: 198

```
Im aware of that thread, in fact i just saw it again yesterday while derping around on here. 

My motor housings are basically identical  to R-SPECs and i've had no less than 50 of those motors come through my shop in one form or another, either doing raptor repairs on highly abused boards or using them in my own builds. I have a bin of about a dozen of them with various things wrong with them such as wire shorts, gashes in the motor can, wrecked bearings, or other mechanical failures resulting from heavy abuse or impact with objects. 

Not a single one has ever broken like that. I've never seen with my own eyes in person a motor break like that. Whatever happened with that motor was probably due to a factory defect affecting a short run of motors and/or seriously extreme circumstances that other people just aren't seeing. 

My personal suspicion on that one is that three of the screws broke loose just enough to cause undue stress on the single spoke containing the bolt hole in question in which the bolt was still tight enough to allow the spoke to stay put while the rest of the motor flexed, causing the cast aluminum to break off in a chunk on impact with some sort of immovable object. Religiously using thread locker on the motor mounting bolts would keep that from happening.
```

---
## \#56 Posted by: Randyc1 Posted at: 2017-02-01T18:06:13.003Z Reads: 184

```
I've seem Tacon 160's which I think are  Maytech also in a 6364 size,  selling for $63.00.

Could we get your source for 6355 Maytech's ??
```

---
## \#57 Posted by: longhairedboy Posted at: 2017-02-01T18:37:23.464Z Reads: 187

```
My source is Maytech. I emailed them directly and we had a conversation over email. I didn't go through a third party. 

If i ordered 1000 motors with zero modifications save the anodize color and laser etching, i could probably sell mine for $63 too. But i didn't, i only got 20 of them. And since they retail individually from maytech for $160 without keyways, superworm phase leads, VESC sensor adaptors, keys, or 5.5mm bullets, $130 is kind of a deal.
```

---
## \#58 Posted by: Randyc1 Posted at: 2017-02-01T18:40:22.483Z Reads: 182

```
Ok thanks bud , I appreciate info !
```

---
## \#59 Posted by: Smorto Posted at: 2017-02-01T19:15:24.473Z Reads: 189

```
Hello,
      Not to bring this thread off topic but I have a question regarding your sensored motors @longhairedboy. I have the sensored 190kv motor from the electric-skateboard.market and I couldn't find a place to plug in the sensor wire that fit on my VESC, is there something I am missing here? 

P.S. The sensor wires/plug look exactly the same as yours except white.
```

---
## \#60 Posted by: longhairedboy Posted at: 2017-02-01T19:21:01.859Z Reads: 181

```
replied in the other thread
```

---
