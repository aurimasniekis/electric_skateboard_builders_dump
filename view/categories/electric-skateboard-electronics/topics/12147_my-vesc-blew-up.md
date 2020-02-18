# My VESC blew up!

### Replies: 40 Views: 3783

## \#1 Posted by: luckleineschaars Posted at: 2016-10-30T10:55:44.174Z Reads: 336

```
Hi,

One month ago I built my first electric skateboard. Decided to change my ESC for a VESC. After trying to run it in FOC mode the motor started jittering at startup. So I put it back in BLDC mode. Pulled the trigger. And BAM. Big spark from my DRV8302. See the pictures for the burned spots on my VESC. What went wrong? Is it my fault by setting some wrong parameters? Or is it just a faulty VESC? I assume this is not repairable, so what do I have to do so this does not happen again if I buy a new VESC?
It is a 12s setup with a 230kv. 
Greetings,
Luc

<img src="/uploads/db1493/original/3X/3/9/394a3d7c351d583d8a4d7dfb4df9e39089a9c4b0.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/6/26439b6709c076353e171d7db8b7911976be36af.png" width="690" height="382"><img src="/uploads/db1493/original/3X/1/f/1f2bb5f2700f068c31bdc75a004c841896818ca1.jpg" width="666" height="500">
```

---
## \#2 Posted by: Maxid Posted at: 2016-10-30T10:59:04.925Z Reads: 319

```
sounds like a typical fault due to the FOC-BLDC switching. Sorry to say but that is on you.
FOC is not recommended with the current VESC version.
```

---
## \#3 Posted by: luckleineschaars Posted at: 2016-10-30T11:02:11.271Z Reads: 314

```
Why is it not possible to put this VESC in FOC mode? And if I buy a new VESC and keep it in BLDC mode everything should be fine?
```

---
## \#4 Posted by: Schulerbible Posted at: 2016-10-30T11:07:40.829Z Reads: 310

```
Lots of blow ups seem to happen in FOC mode and 12s. No idea why people try it anyway and then wonder when things go wrong?
```

---
## \#5 Posted by: Dedbny Posted at: 2016-10-30T11:09:38.191Z Reads: 302

```
Are there warnings on that go wth the vecs about not to go into FOC. I thought some ppl did have vescs in foc or is it with certain battery set ups.
```

---
## \#6 Posted by: IDVert3X Posted at: 2016-10-30T11:11:39.359Z Reads: 289

```
When you switch between FOC and BLDC, you should reupload the firmware, otherwise bad things can happen.
```

---
## \#7 Posted by: luckleineschaars Posted at: 2016-10-30T11:11:50.611Z Reads: 281

```
Well a bit foolish of me. But if I knew I should not be running FOC mode with 12s I would not have done it.
```

---
## \#8 Posted by: Maxid Posted at: 2016-10-30T11:31:19.975Z Reads: 270

```
esk8.de says this on their website:
"WARNING: FOC is still in deveolpment, therefor we recommend using the VESC in BLDC mode only! Using FOC happens on your own responsibility and risk!"
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-10-30T11:49:00.972Z Reads: 264

```
1. 12s is sometimes critical for vesc. 10s is recommended 
2. Foc is not stable with our current version
3. Switching back to bdlc causes problems without a proper reset
4. 12s 230kv is a bad combo for vesc
```

---
## \#10 Posted by: luckleineschaars Posted at: 2016-10-30T11:51:39.299Z Reads: 256

```
Will it be less likely to go wrong with the new VESC-X?
```

---
## \#11 Posted by: Maxid Posted at: 2016-10-30T11:52:26.887Z Reads: 252

```
that is what they claim - not specifically though as they just say it is more robust in general.
```

---
## \#12 Posted by: TarzanHBK Posted at: 2016-10-30T11:53:52.830Z Reads: 242

```
Look at some reviews, perhaps someone tested it with 12s and foc. But your motor is still to high.
```

---
## \#13 Posted by: luckleineschaars Posted at: 2016-10-30T12:03:36.409Z Reads: 236

```
Well it is hard to find proper reviews of the VESC-X since it is not officially released yet. They claim it is 12s compatible, so it should be fine. But what is wrong with a 230kv motor?
```

---
## \#14 Posted by: Maxid Posted at: 2016-10-30T12:07:02.614Z Reads: 238

```
a little more research would have been good for you:
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#15 Posted by: luckleineschaars Posted at: 2016-10-30T12:20:06.383Z Reads: 218

```
Thank you all for answering my questions.
Well I first started out with a complete kit from  which included a 12s torqueboards ESC and a 230kv motor. But then I wanted something more programmable. And blindly assumed that a VESC would fit my needs. But lesson learned, I need to do better research next time.
```

---
## \#16 Posted by: Cjnutts Posted at: 2016-10-30T13:17:14.658Z Reads: 214

```
 I feel your pain brother.  I just learned this five days ago. I stumbled across this forum  because I couldn't get any response from Tb.  I didn't even ask them to pay for it I just wanted to know was it something I did  <img src="/uploads/db1493/original/3X/0/b/0b99579653649aabb462f5519c55ae03fde27a86.jpg" width="373" height="500">
```

---
## \#17 Posted by: TheImmortalJew Posted at: 2016-10-30T17:00:14.835Z Reads: 206

```
So, I don't know if I'm the only one that noticed...but your screenshot of settings shows your battery cutoff start and end at 36V and 33V respectively. Those are good settings, for a 10s setup. But if you're running 12s it should be 43.2V start cutoff and 42V end cutoff. 

I actually have been running the TB VESC and 230KV on my board for over a month. Over 200 problem free miles so far.
```

---
## \#18 Posted by: evoheyax Posted at: 2016-10-30T17:09:40.322Z Reads: 210

```
You can run 12s in FOC. I have 8 VESC 4.12s in FOC at 12s, hummie runs at 12s in FOC, and same with chaka with chaka vescs.

What you can't do is run 12s FOC with a standard enertion VESC and not expect problems...

I have also switched between FOC to BDLC and back to FOC before with no issues... It's where you choose to buy your vesc from that determines what you can do with it...

I hope the vesc-x fixes these issues. I will let you know when I beta test one if you can run 12s in FOC, since that's pretty much the only way I run...
```

---
## \#19 Posted by: E-Boarding Posted at: 2016-10-30T19:13:29.806Z Reads: 201

```
you can't even run 10S in FOC with Enerton-VESCs but they are cheap: 1 Enertion Vesc + 1 DRV-Repair is still cheaper than 1 Chaka or 1 esk8.de-Vesc which can blow up too

waiting for VESC-X
```

---
## \#20 Posted by: Jinra Posted at: 2016-10-30T19:31:16.477Z Reads: 196

```
yea but if a chaka vesc blows up you get it repaired under warranty
```

---
## \#21 Posted by: TarzanHBK Posted at: 2016-10-30T19:34:19.727Z Reads: 176

```
and so on esk8.de vesc
```

---
## \#22 Posted by: Luke Posted at: 2016-10-30T21:47:13.258Z Reads: 168

```
[quote="E-Boarding, post:19, topic:12147"]
you can't even run 10S in FOC with Enerton-VESCs
[/quote]

I've had no issues with enertion vescs on foc at 10s. I believe that a big factor of this is hitting the erpm limit that chaka talks about. 10s and 190kv motors seem to work fine for me but I wouldn't expect 10s and 230kv motors. I'm sure manufacturing quality helps prevent issues with soldering etc.
```

---
## \#23 Posted by: E-Boarding Posted at: 2016-10-31T07:03:39.431Z Reads: 156

```
I was using 190kv, you may get lucky or you may not, it's a gamble as nobody really understands what exatly happens and that's why you are never be save to use FOC.
```

---
## \#24 Posted by: jonfmalm Posted at: 2016-10-31T09:32:59.531Z Reads: 142

```
I'm using TB vesc, v4.12. Will I be fine running FOC at 12S?
```

---
## \#25 Posted by: TarzanHBK Posted at: 2016-10-31T09:35:09.700Z Reads: 143

```
FOC is always like russian roulette. It works or it fails. Some people are lucky, some are not.
```

---
## \#26 Posted by: jonfmalm Posted at: 2016-10-31T09:41:22.624Z Reads: 144

```
BLDC will be completely reliable though?

Does anyone have input on the % torque gain from FOC, and the %noise reduction from FOC?
```

---
## \#27 Posted by: webst Posted at: 2016-10-31T15:36:29.940Z Reads: 135

```
[quote="TarzanHBK, post:25, topic:12147, full:true"]
FOC is always like russian roulette. It works or it fails. Some people are lucky, some are not.
[/quote]
Can you please point me towards actual science behind your statement?
```

---
## \#28 Posted by: Cjnutts Posted at: 2016-10-31T15:47:13.753Z Reads: 134

```
 I definitely would not try it with TBs vest.( again )
 They will not contact you back .
 But my Enetion vest on 9s 149kv  has ran flawlessly for a couple months but I probably won't change out of it. 🐥🐥🐥🐥
```

---
## \#29 Posted by: Maxid Posted at: 2016-10-31T16:29:54.980Z Reads: 130

```
when nobody knows why it fails - why should there be actual evidence written down somewhere?
```

---
## \#30 Posted by: Jinra Posted at: 2016-10-31T17:27:05.273Z Reads: 130

```
More statistics than science at this point.
```

---
## \#31 Posted by: e-Octo Posted at: 2016-10-31T17:34:12.970Z Reads: 142

```
[quote="TarzanHBK, post:9, topic:12147"]
Switching back to bdlc causes problems without a proper reset
[/quote]

Could you clarify what the "proper reset" procedure is for this?  I want to try FOC (on 8-10s), and if it's not awesome i'll switch back to BLDC.  Curious on the specific steps to do this safely to avoid killing the VESC or DRV chip.

[quote="webst, post:27, topic:12147"]
Can you please point me towards actual science behind your statement?
[/quote]

Vedder.se forum - post and ask.  Those guys are the experts, with Ben also looking and possibly answering.
```

---
## \#32 Posted by: Jinra Posted at: 2016-10-31T17:35:35.832Z Reads: 138

```
Re-flash the firmware.
```

---
## \#33 Posted by: MannyM0E Posted at: 2018-02-12T06:59:45.524Z Reads: 79

```
12s with mono 190kv on vesc4.12 from diyelectricskateboard should be fine ? Or am I risking my vesc ?
```

---
## \#34 Posted by: b264 Posted at: 2018-02-12T07:48:46.935Z Reads: 75

```
Don't use FOC on diyelectricskateboard vescs and I don't ever recommend 12S on VESC but lots of folks do it
```

---
## \#35 Posted by: SimosMCmuffin Posted at: 2018-02-12T07:53:43.658Z Reads: 76

```
Is there any consensus on using FOC on the VESC 6.4 or are they better designed to handle it.
```

---
## \#36 Posted by: ShutterShock Posted at: 2018-02-12T07:59:37.705Z Reads: 76

```
I'm running 12S foc on my board on 2 focboxes, and I haven't had any issues yet.  Full no-load spin up only brings me to about 54k erpm. This is with 190kv tb motors, sensored.
```

---
## \#37 Posted by: b264 Posted at: 2018-02-12T08:01:23.389Z Reads: 74

```
No amount of "I did it and I'm fine" will get me to risk my body.  All those parts have manufacturing tolerances of like 10% for every single piece.  Running it a the razor-edge of what's possible, maybe, is not on my agenda for something that can throw me on the roadway at speed if it fails.  You can do it all you want.  But please don't act like it's not dangerous.
```

---
## \#38 Posted by: Eboosted Posted at: 2018-02-13T02:34:49.587Z Reads: 57

```
Almost all my boards are 12s, all working perfect. More voltage less current flowing through all the components, everything works cooler, the acceleration is impressive every time o push it to the limit. 
Focboxes working like a clock, VESC6 also working reliably. 
I think the respect/fear for 12s is overrated
```

---
## \#39 Posted by: ZackoryCramer Posted at: 2018-02-13T03:09:28.639Z Reads: 55

```
I had one of those TB Vesc's blown up on me too. I was trying to do UART communication with Arduino and after using BLDC to manually set current it turned into a firework. :fireworks: :disappointed_relieved: I then talked to DIY and they sent me a full replacement for $80 free shipping and I didn't even have warrenty on the one I blew up. :grinning:
```

---
## \#40 Posted by: ThermalM16 Posted at: 2018-02-13T04:12:55.409Z Reads: 48

```
@luckleineschaars It sounds like you may have incorrectly configured a setting during FOC setup. I was testing a 4.12 the other day and figured I'd see what would happen if I tried to spin a big motor at 15000 RPM and blew it up pretty similar to this. However, this is repairable and I can repair it for you. I run a repair service for VESCs out of Florida. Let me know if you're interested

JK this was over a year ago :joy:
```

---
