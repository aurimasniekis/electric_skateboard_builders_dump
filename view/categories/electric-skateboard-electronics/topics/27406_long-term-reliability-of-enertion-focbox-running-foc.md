# Long term reliability of Enertion FOCBOX running FOC

### Replies: 49 Views: 4494

## \#1 Posted by: RiGo Posted at: 2017-07-11T22:54:15.347Z Reads: 534

```
I'm about to start a build using 2 FOCBOXs (bought when they were still VESC-X) and I intend to run FOC. I'll be using a 10s3p pack and dual 190kv 6355 motors and limit current at 40A (20A each). I've searched the forum and there's not much info on people running FOC with Enertion's FOCBOX. I'm hoping experiences will have been positive. I mean, FOC is in the name of the product!

So can you chime in with your experience running FOC on Enertion, both good and bad?
```

---
## \#2 Posted by: willpark16 Posted at: 2017-07-11T23:35:09.686Z Reads: 532

```
No bad only goodd the vesc x has been perfect in foc in 10s
```

---
## \#3 Posted by: Battosaii Posted at: 2017-07-12T00:06:01.455Z Reads: 521

```
ill let you know my focbox's should come sometime next week to replace my old enertion vesc's, i have a raptor dual which is identical to your build, i want to try FOC mode too.
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2017-07-12T00:21:13.064Z Reads: 509

```
Almost 9 months 12s FOC on Carvon hubs... zero issues
```

---
## \#5 Posted by: sl33py Posted at: 2017-07-12T00:31:37.897Z Reads: 492

```
I'll follow for sure.

Thing **you all need to note is KV of motor?**  Lower KV like hubs definitely is an advantage.

I just setup my first FOC setup on 149kv 8s (might eventually go 10 or 12s).

Love the silence!
```

---
## \#6 Posted by: RiGo Posted at: 2017-07-12T00:42:47.157Z Reads: 474

```
Updated original post - running 190kv 6355 motors with 40A total max current (20A each motor).
```

---
## \#7 Posted by: Eboosted Posted at: 2017-07-12T04:51:06.583Z Reads: 454

```
Who is runing FOC on Focbox on 12s with no issues and for how long have you been runing it?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-07-12T04:52:34.405Z Reads: 446

```
@Michaelinvegas....

[quote="Michaelinvegas, post:4, topic:27406, full:true"]
Almost 9 months 12s FOC on Carvon hubs... zero issues
[/quote]
```

---
## \#9 Posted by: Eboosted Posted at: 2017-07-12T05:03:19.693Z Reads: 436

```
I have a Trampa street carver with dual 6374 and I recently upgraded to Focbox, I wonder if runing FOC could be too risky
```

---
## \#10 Posted by: Jinra Posted at: 2017-07-12T05:04:22.095Z Reads: 434

```
I've heard from a couple people that it's "FOC-proof" and has a transistor that shuts off before anything can burn the DRV, but I'm not sure about that claim.
```

---
## \#11 Posted by: Eboosted Posted at: 2017-07-12T05:21:48.850Z Reads: 422

```
I had an issue yesterday, one Focbox could not make motor detection and threw an ABS overcurrent fault. So instead of burning the DRV or shunts some audible "clack" noise maybe some kind of thermoswitch activated and prevented the Focbox from frying. 

This happened while runing as well. At the end the issue was a faulty Focbox, but just to confirm there was indeed some kind of protection that saved the DRV
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-12T05:23:24.307Z Reads: 413

```
nice to know, though still sucks that it can potentially shut off mid ride, but I guess it's good for people to see if they can even run FOC on their setup.
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2017-07-12T05:31:06.675Z Reads: 409

```
I swear I think I've written that phrase like four of five times in the past month or so
```

---
## \#14 Posted by: Eboosted Posted at: 2017-07-12T05:38:52.710Z Reads: 403

```
Well, this protection is nice but yesterday I had a fucking scary nightmare, when I went to test the board, I gave it full throttle and the protection activated, this caused one motor to kept spinning for 3 seconds, it pushed me sideways, even though I left the throttle go, almost loose control buy fortunately was able to save it.

Nothing is more scary than being riding a board at full speed and not only loose your brakes but lock one motor at full throttle for the longest 3 seconds of your life
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-12T05:49:03.314Z Reads: 391

```
Wow that's crazy and seems like a huge design flaw. VESC should never lock at full duty cycle... I've seen some crappy remotes do that, but haven't heard of the VESC doing that. What remote were you using?
```

---
## \#16 Posted by: Eboosted Posted at: 2017-07-12T05:53:17.028Z Reads: 390

```
I was using a mini remote, but that was not the issue I can definitely confirm the bad FOCBOX  locked on full throttle, I also replicated that on the bench. 

After replacing the Focbox with a spare one the lock didn't happen anymore
```

---
## \#17 Posted by: treenutter Posted at: 2017-07-13T14:34:06.938Z Reads: 360

```
[quote="Jinra, post:15, topic:27406"]
Wow that's crazy and seems like a huge design flaw
[/quote]

[quote="Eboosted, post:16, topic:27406"]
After replacing the Focbox with a spare one the lock didn't happen anymore
[/quote]

It seems that @Eboosted had a faulty FOCBOX; so hopefully it was a manufacturing glitch and not a design flaw inherent in the product. Is that your impression @Eboosted ?
```

---
## \#18 Posted by: Stef Posted at: 2017-07-13T15:36:06.492Z Reads: 352

```
I run 190KV TB6355 on 10S using sensored FOC for 4 weeks now. Im not babying the machine at all and its been 100% reliable so far.
```

---
## \#19 Posted by: E-Boarding Posted at: 2017-07-13T15:49:06.812Z Reads: 351

```
I've run my 10S dual-R-Spec in FOC through Snow, Forest, Rain, 20%-Hills and Shit and it's working fine
```

---
## \#20 Posted by: Jinra Posted at: 2017-07-13T15:51:49.231Z Reads: 351

```
I suspect that FOC reliability is heavily tied to eRPM, which would be why people running FOC on hubs don't have any issues. At 10s w/190kv motors you're running at about 45-50k eRPM after inefficiencies. 

I wonder if I'll counter problems when approaching 60k on my 230kv 10s board. I hit about 55-57k erpm on this setup.
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2017-07-13T15:57:23.512Z Reads: 341

```
Look at the problem, I think it might just be a bad connection over the PPM connector, It migt be that the pin are a little bit shorter, or it could be some oxydation, creating a bad connection inside the connector.

The only time I got these kind of behaviour was cause by a cheap cervo cable, the connector was to tall to reach the pins for a good connection.
```

---
## \#22 Posted by: Silverline Posted at: 2017-07-13T16:53:03.511Z Reads: 331

```
What is erpm vs. Rpm ? I run a 270kv motor on 6s. How many erpm's is that ? I have the default max erpm value 100.000 in bldc, should i change that ?
```

---
## \#23 Posted by: sl33py Posted at: 2017-07-13T16:57:01.963Z Reads: 330

```
You can estimate your ERPM w/ a calculator like esk8.it

Also see:
http://www.electric-skateboard.builders/search?q=ERPM

TONS of info on this - good to know before you fry a VESC.

And if you don't have a VESC/FOCBOX/ etc. - the 60k erpm limit should not apply.
```

---
## \#24 Posted by: Silverline Posted at: 2017-07-13T16:59:47.122Z Reads: 323

```
I have a vesc from esk8.de
Thanks 😃
```

---
## \#25 Posted by: Enrico Posted at: 2017-11-30T06:07:49.276Z Reads: 248

```
Planning to run foc on 12s belt drive with 190kv using FOCBOX 
safe? or better to just run bldc
```

---
## \#26 Posted by: FredrikHems Posted at: 2017-11-30T06:26:42.758Z Reads: 239

```
That is a little risky, but it can be done. You will be very close to 60k ermp after inefficiences, and maybe over too..
```

---
## \#27 Posted by: Enrico Posted at: 2017-11-30T07:05:21.942Z Reads: 235

```
ahh screw it, I'm staying with bldc.

I thought the focbox had a mechanical measure to protect the drv chip from frying?
```

---
## \#28 Posted by: Cobber Posted at: 2017-11-30T07:12:53.661Z Reads: 239

```
@Enrico this has been discussed a few times bro, try doing a search & a bit more research, thing is most of the time the motor you buy is not the kv you think, it will be under... so the reality of practice is that even going over erpm by a small amount will not cause any problem. So again I suggest you do a bit more research before you give up to make a informed decision.
```

---
## \#29 Posted by: longhairedboy Posted at: 2017-11-30T07:23:14.435Z Reads: 237

```
Been on the same VESC-Xs since before all the focbox nonsense. We haul ass all over. 12S, 190KV. 

Also We've been running 13S on them on 190kv motors on MBS 100mm wheels for about a month and a half using an old Tronik sled. That clunky shit is killing it at over 40mph. Not dead yet. 

They seem legit.  just sayin'
```

---
## \#30 Posted by: spannepacker Posted at: 2017-11-30T07:33:27.833Z Reads: 233

```
I think my FOXBOX croaked the other day while running 190kv at 12s in FOC. I had done well over 200 miles on it so I thought it was solid. I went on a medium hilly 7 mile ride with no problems but got all sorts of [**weird data**](https://metr.at/r/kAR74) from it with crazy high current readings. 

When I went to use it in the morning [**this is all it did**](https://drive.google.com/file/d/1XoI1hMME-ucAQzeabuEeZIuDd00gxP17/view?usp=sharing). When I pull the throttle the motor clicks and the VESC resets because of an over current fault (using metr). Its not showing up in BLDC_Tool but I can access and change settings with perimetr.
```

---
## \#31 Posted by: FredrikHems Posted at: 2017-11-30T08:35:44.594Z Reads: 228

```
Yes it protect the drv against some things, but not If you Go far over 60k on the erpm
```

---
## \#32 Posted by: Eboosted Posted at: 2017-11-30T22:07:17.470Z Reads: 225

```
[quote="Eboosted, post:7, topic:27406, full:true"]
Who is runing FOC on Focbox on 12s with no issues and for how long have you been runing it?
[/quote]

Now I've been runing FOCBoxes on 12S for 1 month with no issues.
```

---
## \#33 Posted by: WARMAN Posted at: 2017-11-30T23:20:00.175Z Reads: 219

```
What's the kv limit using focbox?
```

---
## \#34 Posted by: FredrikHems Posted at: 2017-12-01T21:08:31.509Z Reads: 214

```
That depends on voltage, but I think the Erpm limit is still 60k
```

---
## \#35 Posted by: ElskerShadow Posted at: 2017-12-04T09:31:04.117Z Reads: 205

```
What are thevalues of the battery in the BLDC tool. I will have soon a 12S battery and I don’t wan’t to do a stupid mistake.
```

---
## \#36 Posted by: Eboosted Posted at: 2017-12-04T17:10:21.542Z Reads: 197

```
What cells do you have? What cell count? What KV motors do you have? these are important questions to give you current limits
```

---
## \#37 Posted by: ElskerShadow Posted at: 2017-12-04T17:47:24.229Z Reads: 191

```
I have 12S5P 30Q pack carvon v3 so 114 i think
```

---
## \#38 Posted by: Eboosted Posted at: 2017-12-04T18:41:03.144Z Reads: 187

```
You could raise the battery max current up to 50A, 37.5A if you want to be inside manufacturer specs, but the 30Qs have proven to be a very good 20A cell.
```

---
## \#39 Posted by: longhairedboy Posted at: 2017-12-04T18:56:40.406Z Reads: 190

```
Full disclosure, I don't use FOC, i use BLDC in Ssnsored Hybrid mode. I may have accidentally something in this thread.
```

---
## \#40 Posted by: BigBoyToys Posted at: 2017-12-04T20:33:59.868Z Reads: 192

```
Ive run 70, 80, 110, 130, 149, and 170kv motors/hubs/direct drives at 12S and FOC on the FOC box(some were VESC-X) without any issues I believe were related to the voltage or FOC mode over the last year. 

Ive had 1 FOC failure at 12S on a TB VESC but to be fair I had very high motor Amp settings on that VESC (120A).
```

---
## \#41 Posted by: b264 Posted at: 2017-12-04T20:36:21.164Z Reads: 187

```
Has _anyone_ had a failure at 10S voltage on the enertion focbox in FOC mode?  Or just in 12S?
```

---
## \#42 Posted by: Mikenopolis Posted at: 2017-12-04T22:05:19.997Z Reads: 186

```
me, but probably a faulty vesc-x to begin with. it was repaired once but failed a second time. Replacement Vesc-x stilling works flawlessly with 10s battery under same settings, roughly 80 miles so far?
```

---
## \#43 Posted by: b264 Posted at: 2017-12-04T22:06:07.491Z Reads: 188

```
[quote="Mikenopolis, post:42, topic:27406"]
me, but probably a faulty vesc-x to begin with
[/quote]

Is that the same BOM & schematic as an enertion focbox?
```

---
## \#44 Posted by: Mikenopolis Posted at: 2017-12-04T22:08:35.548Z Reads: 188

```
same thing, just different name due to Trampa registered the word VESC.

My understanding is that early Vesc-x were not as well manufactured as newer ones. factories have changed in order to get better QC.
```

---
## \#45 Posted by: monkey32 Posted at: 2017-12-05T07:05:19.872Z Reads: 171

```
Ha yeah, I have the original enertion V1 that shit wouldn't even boot up. Jason has come a long way. Not reading many problems any more.
```

---
## \#46 Posted by: ElskerShadow Posted at: 2017-12-05T10:42:12.639Z Reads: 165

```
Should I change battery cut offf ? Now it’s 33 v start and 30 v end isn’t too low for 12 S ?
```

---
## \#47 Posted by: Eboosted Posted at: 2017-12-05T14:56:50.124Z Reads: 157

```
I'd set it up at 36 and 33.6v
```

---
## \#48 Posted by: ElskerShadow Posted at: 2017-12-05T16:47:29.753Z Reads: 150

```
Thank you very much !
```

---
## \#49 Posted by: BricE Posted at: 2018-08-24T15:08:28.501Z Reads: 73

```
I was runing focbox on foc 10s on my ebike. I did 250 km or so with it in the past month. The other day I got going (192 kv motor spinning 500-1000 rpm)  turn on the vesc  twist the throttle all it did was jerk and started to resist movement. On further inspection it appears I blew one of the direct fets. Probably my fault for freewheeling.
```

---
