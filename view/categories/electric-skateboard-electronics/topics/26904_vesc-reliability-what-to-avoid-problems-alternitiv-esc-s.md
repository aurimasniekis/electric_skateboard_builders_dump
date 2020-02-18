# VESC reliability - what to avoid problems? alternitiv ESC´s?

### Replies: 15 Views: 2083

## \#1 Posted by: dichter84 Posted at: 2017-07-06T11:16:22.938Z Reads: 242

```
Hi everyone,

i just startet motorising my Mountainboard to cruuuuze around the hills here around my home :XD Now i´m at the point to get an reliable ESC for that job.

I wanted do use an dual VESC, but as i read this forum i found out that many people had DRV-Errors  on that ESC.

My first question is now: is there a save way do avoid fried VESC´s or DRV´s?
I have read of two points that could cause an fried VESC:
-using FOC-Mode might be dangerous
-setting ERPM to high might be dangerous (and use the wrong motor-KV...)

So if i use only BLCD-Mode and set the ERPM to max. 60.000, can i be (nearly) sure to dont frie my VESC, or will it still be some kind of "luck"?

So my second question is:
What ESC would be more reliable than the VESC (if any exist...)?
-I heared of the FOCBOX, is this one maby an option and worth the more bucks?

For me it is importand to have an reliable ESC, i dont like walking home... ;)

Thanks for your help!
```

---
## \#2 Posted by: NAF Posted at: 2017-07-06T11:20:12.176Z Reads: 238

```
FOCBOX + AXLE + Ollinboard Vescs. All use upgraded components and are pretty safe to use in FOC. 
What's really dangerous is high KV motors and 12s battery running in FOC on VESC's without upgraded internals.
```

---
## \#3 Posted by: dichter84 Posted at: 2017-07-06T11:43:02.917Z Reads: 227

```
Ok, so i wanted to use 10s @ 170 KV-Motors... = 170KV * 37 V * 7 = 44.030 ERPM < 60.000, should be fine, right?

So will it also be safe to use FOC on these settings or should even i prefer BLDC?
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-06T18:39:25.334Z Reads: 195

```
Should be fine would stick to bldc no foc unless you know exactly what you're doing.  Newer hardware coming out is supposed to have better support but it was still experimental in the 4.x boards basically.  Small kick start and you won't get any jittering on start up anyhow.
```

---
## \#5 Posted by: rpn314 Posted at: 2017-07-06T19:21:06.404Z Reads: 182

```
If you're doing a mountain board, I'd say wait a bit for the VESC6. It'll be able to handle the current you'll most likely put through it better than any v4.12 VESC.
```

---
## \#6 Posted by: dichter84 Posted at: 2017-07-07T06:41:47.106Z Reads: 170

```
Hmmm the VESC 6 is very expensive yet, thats not in by budget :confused:

Kickstart is not that easy at a Mountainboard with bindings, thus i would use sensored motors, i heard that will also help to not frie the ESC...

Have anyone heared about the ALIEN-ESC´s? 
http://alienpowersystem.com/shop/esc/alien-150a-3-12s-esc-sensored-opto/
I could order them here from Germany so i would have 2 years of warianty and they could handle 120A each one. But dont know if they have progressive breaking..?
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-07T07:02:46.183Z Reads: 159

```
Could contact the company and ask.  After using the VESC configuration tool though unless another ESC has at least as much configuration and feedback I don't know that I'd want it, even if it could not explode (I did have one car ESC that didn't burn up).
```

---
## \#8 Posted by: sl33py Posted at: 2017-07-07T07:12:31.865Z Reads: 156

```
No mountainboard experience, but what i've seen is unreliability at the edge of the VESC capabilities.  And advantage to run lower kv motors like 192/190, 168, 149, etc.  Especially higher voltage setups also keeps speeds more reasonable.

Bad things happen:
12s and FOC for example
Right on the edge of 60k ERPM (then you coast downhill and brake...  dead DRV)

So if you can't wait for VESC Six (or group buy on VESC Six) - i'd suggest one of the upgraded v4.12 VESC's from Chaka (with direct fet and heatsinks), or FOCBox, or Axle v4.12 (he may have direct fet now, but had upgraded BOM w/ previous Fets too).  That would be my order of preference from v6 (via Trampa for $$$), Ollin board co direct fet w/ heatsink, Enertion FOCBox, Axle.

As for Alien ESC's - i'm not sure if they are still using flyer ESC's, but i'd ask before ordering (they were known to be problematic a few years back).  So to be fair - not sure, but look deeper before picking IMO.  

I am a bit VESC focused on my builds, so others should chime in...  VESC still seems the best solution for esk8 w/ configurability and ability to run 12s without super expensive (v6 being an exception).  Look at a Mamba XL2 for comparison and it only does 8s.

my .02.  GL!
```

---
## \#9 Posted by: dichter84 Posted at: 2017-07-07T10:29:31.641Z Reads: 138

```
@sl33py: What do you mean with "using flyer ESC" at the Alien-Power-Systems?

@wafflejock: do you mean you hand only one car ESC that did not burn up or did you have several ESC´s and only one did NOT burn up?
```

---
## \#10 Posted by: sl33py Posted at: 2017-07-07T15:45:36.767Z Reads: 118

```
Flyer is a brand/manufacturer of inexpensive ESC's.  A few years back lots of people had issues w/ Alien ESC's (re-branded from Flyer), and it was generally recommended to avoid them.  
I know DIYes also had some, and stopped carrying them.  I know DIYes has a "torqueboards" 6 and 12s ESC now, but believe it's a maytech or similar and has been pretty reliable.  Price-wise on the high voltage ESCs - once you go past 6s on RC Car ESCs they typically get very expensive, so another reason why i've stuck with VESCs.  

Bruno is a good guy and stands behind his warranty - but i personally have had several weeks working with him on an issue before it was addressed.  He'll take care of you, but if the hardware is poor quality and fails frequently - the warranty wouldn't be my concern.  

So do some more research and see if others have this ESC without issue today.  Personally i'd avoid and go VESC.  

my .02 and hope it helps.
```

---
## \#11 Posted by: wafflejock Posted at: 2017-07-07T15:50:45.556Z Reads: 115

```
Yeah I had several that I burnt up or didn't work out.. one of them had the hard brake automatically activated when letting go of the throttle.... I somehow figured out how to ride that without it constantly throwing me but it wasn't safe at all so never went any substantial distance with it, think it eventually fried, then I think I tried a boat ESC that was pretty cheap and rated with high A and enough V but it also quickly cooked (afterthought they probably expected some sort of water cooling or maybe not a dude on a skateboard on top of it).  The last car ESC I got actually survived but I had just gotten it as a stop gap till the VESCs weren't back ordered anymore.  Was rated 120A, can check specifics if you want but has a fan and heatsink, it worked pretty well really but required extra proprietary bits of hardware for adjusting the programming and still not as configurable as the VESC (ah also pretty sure it had a 6S limit but can verify).
```

---
## \#12 Posted by: dichter84 Posted at: 2017-07-07T17:11:18.192Z Reads: 111

```
@sl33py:
you mean this one from Torqueboards? 
diy-electric-skateboard-kits-parts/torqueboards-12s-120a-car-esc-opto-hv/
Only they say it´s a non sensored ESC...

When i search the Internet for Alien-ESC´s i find some broken ESC´s and people were not happy with them, but all i find is about 2013 or 2014... No newer reviews...

Hmm still dont know... VESC has no warianty, and i dont want to have to learn soldering DRV´s ;)

Has anyone killed a VESC when riding at safe Parameters like only BLDC, stay unter 60.000 ERPM, but needet much AMP´s?
```

---
## \#13 Posted by: sl33py Posted at: 2017-07-07T18:37:01.800Z Reads: 106

```
[quote="dichter84, post:12, topic:26904"]
you mean this one from Torqueboards?
[/quote]

Yes - that's one several run and have had good feedback from what i've heard.  It's another brand (maytech or similar), and you can try to search/find it elsewhere for less $.  Or spend a few $ more and get it from DIYes/@Torqueboards and get help if you get stuck.  Worth it in my opinion.  Help with getting firmware sorted if needed, vs good luck finding it elsewhere...

Perhaps @Torqueboards can comment on his 12s ESC use for MTB.  I'm sure others will comment, but i've never run mountainboards so i'll let them chime in.
```

---
## \#14 Posted by: benwong Posted at: 2017-07-10T07:31:31.197Z Reads: 92

```
I using FVT 12S sleeping lion ESC on my MTB. There have two firmware suitable use in MTB. ESC was running well sensorless mode. I not sure torque oard ESC same with FVT or not.
```

---
## \#15 Posted by: dichter84 Posted at: 2017-07-10T16:46:07.240Z Reads: 79

```
How long are you using the Sleeping Lion ESC now? Is it reliable? Have you had any issues or problems with it?

I Think the TB esc is the same than the other ESC from FVT, i mean the one for planes. It looks very the same, but i heared they are maby using an other Firmware. Does any one know where to get that firmware?

I have read many good things about the FVT ESC´s the last days... Has any one had problems wiht these?
```

---
