# FOC at 12S anyone?

### Replies: 60 Views: 2950

## \#1 Posted by: longhairedboy Posted at: 2017-07-13T15:59:45.708Z Reads: 329

```
Anyone doing FOC at 12S yet? 

What kinds of limitations are you seeing?

I haven't tried it out yet, since i've moved to sensored motors i've been obsessed with Hybrid mode. But i recently ordered some panel mount micro and mini USB cables for my boards so when i get them back on my own i'm going to give in to my urge to randomly try different settings on things at a whim for science since i won't have to drop my box and make a day of it anymore.
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2017-07-13T16:04:04.199Z Reads: 323

```
i just switched to hybrid last week, had some pretty bad issues with vesc cable..have you been using FOC at all? ive considered it after having so many vesc cutoutts.. anyways not to derail your topic, i really want to try FOC though.. i will have to read the faq on it first, i dont even know how to set it up yet =)
```

---
## \#3 Posted by: Jinra Posted at: 2017-07-13T16:08:06.021Z Reads: 318

```
Haha, I remember when Jason and others would scoff at people for wanting to run sensored saying "Is it that hard to just kick?" I've always run sensored and wouldn't do it any other way.

I believe @evoheyax runs 12s FOC on hubs and Ollin VESC4 (non-direct fets). I'm planning to run FOC as well (though on 10s, but still high eRPM) once I get my focboxes. Which VESCs are you planning to test with?
```

---
## \#4 Posted by: chaka Posted at: 2017-07-13T16:12:17.040Z Reads: 305

```
I have been running foc at 12s on my larger motors... no problems.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-07-13T16:13:15.025Z Reads: 307

```
[quote="Jinra, post:3, topic:27527"]
I believe @evoheyax runs 12s FOC on hubs and Ollin VESC4 (non-direct fets)
[/quote]

It is true, and up to 3 out of 4 motors sensored also!  Broke the tool opening up the 4th motor yesterday, haha.

There's no limitations. Everything just runs perfectly. These are upgraded VESCs though, so I wouldn't say this about any old VESC v4.
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-07-13T16:13:23.570Z Reads: 296

```
FocBoxes of course. Then I'll try it on generic 4.12s to see if i can release some of that glorious magic smoke. Then 'll probably try it on a set of AXLEs if the FocBoxes work out with it. 

@chaka Thanks! Any advice on settings?
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-07-13T16:14:21.281Z Reads: 294

```
[quote="evoheyax, post:5, topic:27527"]
These are upgraded VESCs though, so I wouldn't say this about any old VESC v4.
[/quote]

Upgraded? 'Splain. Stacking caps or what?
```

---
## \#8 Posted by: evoheyax Posted at: 2017-07-13T16:16:28.220Z Reads: 280

```
Well... We all know chaka has always been ahead with the upgrades on the VESC. I'm still running his custom quad VESCs with no issues.

I'm really curious to see his newest v4 design that he stated can likely do 70a continuous.
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-13T16:18:36.928Z Reads: 271

```
With axle (and pretty sure ollin and probably focbox) vesc at least, it has double stacked c37 caps, and I believe c26 is upgraded from the initial design as well.
```

---
## \#10 Posted by: chaka Posted at: 2017-07-13T16:19:20.241Z Reads: 264

```
You may want to use the new vesc-tool, it is better at motor calibration than the bldc-tool. I also recommend using a 4.7uf and 2.2uf capacitor at c18 and c26. I have found a variety of caps performs better since different values perform better at different frequencies. Just something I have recently began exploring in order to optimize for FOC function.
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-13T16:20:13.062Z Reads: 259

```
The new VESC tool supports h/w4.xx as well?
```

---
## \#12 Posted by: longhairedboy Posted at: 2017-07-13T16:25:41.870Z Reads: 256

```
I'll see if i can get my hands on the new vesc tool this weekend. 

One of the things i want to do with my boards is offer USB programming ports standard since the majority of my customers are enthusiasts and i either get them from forums like this or they end up here because i sent them here. 

Which of course means i need to up my tuning game because the questions will follow, so i need to start getting into it a lot more instead of primarily creating and loading known good configs for particular scenarios. And people are asking about FOC which is something i've been too busy to explore more than just read a bit about it.

Oh forgot the links to these. They're perfect for DIY builds. No more opening boards for programming. And they're cheap. 

FocBox, maytech, flier, and others with Micro B:  https://www.adafruit.com/product/3258

The more traditional 4.12 Mini B: https://www.adafruit.com/product/3318
```

---
## \#13 Posted by: chaka Posted at: 2017-07-13T16:26:29.684Z Reads: 240

```
Yes it does! It does not allow the freedom of configuration the bldc-tool allows but he did include a firmware version without limits if you wanna fry some hardware.
```

---
## \#14 Posted by: Jinra Posted at: 2017-07-13T16:27:25.905Z Reads: 241

```
Why not offer an HM-10 module instead so users can program single/dual VESCs from their phone!
```

---
## \#15 Posted by: NAF Posted at: 2017-07-13T16:28:57.714Z Reads: 243

```
@chaka an post link's with proper part's from mouser for the c18 and c26 ?
```

---
## \#16 Posted by: chaka Posted at: 2017-07-13T16:30:29.289Z Reads: 236

```
4.7uf @ 16v, 2.2uf 2 16v

Make sure you get the right package size, all there is to it!
```

---
## \#17 Posted by: longhairedboy Posted at: 2017-07-13T16:32:07.855Z Reads: 231

```
Eventually, yes. Haven't had a chance to test those as thoroughly as i'd like or work them into the model yet. But yes, that's where i'd like to be by next year.
```

---
## \#18 Posted by: longhairedboy Posted at: 2017-07-13T16:33:48.505Z Reads: 230

```
[quote="Jinra, post:3, topic:27527"]
Haha, I remember when Jason and others would scoff at people for wanting to run sensored saying "Is it that hard to just kick?"
[/quote]

Sounds like something someone selling uncensored motors would say. Oh wait...
```

---
## \#19 Posted by: Jinra Posted at: 2017-07-13T16:34:42.011Z Reads: 230

```
[quote="longhairedboy, post:18, topic:27527"]
uncensored motors
[/quote]

Motors gone wild?
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-07-13T16:39:54.279Z Reads: 227

```
Totally out of control motors! lol

un-sensored lol non-sensored? sans sensors... heh.. the last one is the only one without squiggly red spell check lines.
```

---
## \#21 Posted by: trancejunkiexxl Posted at: 2017-07-13T16:43:07.848Z Reads: 220

```
nub question, where can i get the "new" vesc application?
```

---
## \#22 Posted by: chaka Posted at: 2017-07-13T16:45:39.231Z Reads: 214

```
Vedder said he would be releasing for beta testing, he might have already? I think it will be released to the public in a week or two.
```

---
## \#23 Posted by: pennyboard Posted at: 2017-07-13T16:48:24.466Z Reads: 213

```
I've been running FOC at 12s on an Ollin vesc for the past few weeks. Unsensored 63mm sk3. Haven't had any problems so far. 

Let us know how running 12s FOC on generic goes, I'm planning to run it on a Torqueboards vesc after I get my set-up back up and running.
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-07-13T16:53:58.003Z Reads: 216

```
[quote="pennyboard, post:23, topic:27527"]
Let us know how running 12s FOC on generic goes, I'm planning to run it on a Torqueboards vesc after I get my set-up back up and running.
[/quote]

I've got a half dozen 4.12s freshly back from canada and ready to cook. Then i'll send them back to canada because one of my favorite things to do is send Jonny Repair the same burned up 4.12s over and over again so that eventually he'll claw his eyes out in a fit of deja vu madness. HAHAHAHAHAHAHAHAHA

I better go take my meds now.
```

---
## \#25 Posted by: Jinra Posted at: 2017-07-13T17:07:13.982Z Reads: 206

```
I guess people like you are why he has bulk pricing for VESC repairs :laughing:
```

---
## \#26 Posted by: trancejunkiexxl Posted at: 2017-07-14T04:50:00.753Z Reads: 200

```
i ran foc today for the fist time on 12s w torqueboard 6355 motor.. I am blown away by how buttery smooth it is.. and its soo quiet.. the calibration was pretty painless also, best of all no cogging.. the main straightaway by my house seems like im getting slower passes but, it just feels so damn good..
```

---
## \#27 Posted by: Eboosted Posted at: 2017-07-14T05:38:23.621Z Reads: 189

```
Have you gone full throttle and full speed yet? 

You will feel less final speed against BLDC
```

---
## \#28 Posted by: trancejunkiexxl Posted at: 2017-07-14T05:51:11.396Z Reads: 192

```
ya, im hoping that there might be a way to fine tune this setup... it is really amazing though, completely different experience.. sure the top end is less, but i think im just going to stay put on FOC
```

---
## \#29 Posted by: Eboosted Posted at: 2017-07-14T05:56:03.018Z Reads: 191

```
Full throttle made me loose control on the board, vesc reseted and I lost brakes and throttle for 2 seconds, I had to switch back to BLDC for safety reasons
```

---
## \#30 Posted by: Jinra Posted at: 2017-07-14T05:57:52.511Z Reads: 188

```
wasn't that just because of a faulty focbox though? Or are you using BLDC with the faulty focbox for now
```

---
## \#31 Posted by: trancejunkiexxl Posted at: 2017-07-14T05:59:46.928Z Reads: 187

```
so how does one fine-tune FOC? are there values to tamper?
```

---
## \#32 Posted by: Eboosted Posted at: 2017-07-14T05:59:54.851Z Reads: 189

```
I was using tb vesc at the time, I haven't tested the Focbox on my new setup. I'll try next week and will report back
```

---
## \#33 Posted by: longhairedboy Posted at: 2017-07-14T12:21:07.998Z Reads: 178

```
[quote="Eboosted, post:27, topic:27527"]
You will feel less final speed against BLDC
[/quote]

this is something i heard about when FOC first started making an appearance backj when, which is why i never bothered with it until now. 

Apparently this is still an issue? What's behind the limitation? More math i won't understand?
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-07-14T12:26:17.961Z Reads: 179

```
[quote="Jinra, post:14, topic:27527, full:true"]
Why not offer an HM-10 module instead so users can program single/dual VESCs from their phone!
[/quote]

As of right this minute, who has the best app for the HM-10s? I actually do have a few of those modules already, the last time i tried a few apps on my iphone though none of them were saving changes.
```

---
## \#35 Posted by: chaka Posted at: 2017-07-14T13:20:49.727Z Reads: 173

```
I like the work @Ackmaniac has done on his app, works really well but it is an android app.
```

---
## \#36 Posted by: rpn314 Posted at: 2017-07-14T13:29:55.597Z Reads: 177

```
I agree with @Chaka on android. @Ackmaniac think has a pretty solid offering. On iOS, I haven't been convinced by any of them. The best one requires you to buy the Bluetooth module from him.

I'd love to do an iOS port of @Ackmaniac's if he'll send me the source :wink:
```

---
## \#37 Posted by: treenutter Posted at: 2017-07-14T13:40:04.864Z Reads: 175

```
[quote="longhairedboy, post:12, topic:27527"]
Oh forgot the links to these. They're perfect for DIY builds. No more opening boards for programming. And they're cheap.
[/quote]

@longhairedboy I bought a few of these last year to use with my 4.12 VESCs, but then I chickened out because I thought that the fragile USB port on VESC 4.12 would snap off if introduced to any additional stress or vibration from the cable. I never got around to finding a mounting solution for them, so if ya got one :) ...
```

---
## \#38 Posted by: treenutter Posted at: 2017-07-14T13:44:04.419Z Reads: 171

```
[quote="chaka, post:13, topic:27527"]
It does not allow the freedom of configuration the bldc-tool allows
[/quote]

I actually think that could be a good thing! There are a lot of features in BLDC Tool that a typical user doesn't use. I've seen hundreds of forum posts here where the questions is "what do I do for ___ setting" and the answer from other forum members is "don't touch it!"
```

---
## \#39 Posted by: longhairedboy Posted at: 2017-07-14T13:45:43.394Z Reads: 178

```
That would be ideal, yeah. So basically on ios the state of things really hasn't changed at all this past year. I have an ASUS and an LG tablet so i'll probably just test with those guys for now. I would be more conveninet to iuse my iphone but whatever. 

I have a few HM-10s in a drawer now that i think about it. 

@Ackmaniac 's  stuff is something i've been trying to get around to fully evaluating but i haven't had the chance. Does his software require a firmware update on the ESCs? I thought I read somewhere that it does. 

An app for IOS that actually fucking works needs to happen. It doesn't seem to be a limitation with the HM-10s since that's basically just a BT to serial converter. It seems to be a limitation of determination and mission.
```

---
## \#40 Posted by: chaka Posted at: 2017-07-14T13:46:02.843Z Reads: 187

```
You can still adjust everything but you need to stay within the pre-configured maximums. 100 amp motor max, 150 absolute max.... etc
```

---
## \#41 Posted by: rpn314 Posted at: 2017-07-14T13:47:10.426Z Reads: 185

```
[quote="longhairedboy, post:33, topic:27527, full:true"]
[quote="Eboosted, post:27, topic:27527"]
You will feel less final speed against BLDC
[/quote]

this is something i heard about when FOC first started making an appearance backj when, which is why i never bothered with it until now. 

Apparently this is still an issue? What's behind the limitation? More math i won't understand?
[/quote]

By my understanding It is a limitation because of how well FOC sends power to the motors. 
In BLDC mode, there's a lot of spikes (and they're not always sent at the best time compared to the position of the rotor) and motors respond to that with torque. 
In FOC, it's much closer to a perfect sine wave (i.e. fewer spikes) that is sent at the perfect time, and so it's much smoother, but you also loose the torque bump (which means speed on the high end) caused by that spike. That's also the reason for the difference in sound.

Or ignore me and just read this :slight_smile: 
http://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/3002
```

---
## \#42 Posted by: longhairedboy Posted at: 2017-07-14T13:49:22.783Z Reads: 174

```
Thank you for explaining that in terms i can actually understand and use to explain to other people when they ask. 

IT makes total sense now that you say that. This may explain why i'm enjoying hybrid mode so much. the spikes still happen, but the timing of them is likely much better.
```

---
## \#43 Posted by: chaka Posted at: 2017-07-14T13:59:29.728Z Reads: 175

```
You can use his app with 2.18 firmware but you will not be able to make changes wireless. You need to upload his firmware if you want to use all the features. 

@Ackmaniac any chance you can make the app log and store mileage like an odometer to see mileage over the lifetime of a board? It would need to be a transferable file so nothing is lost when switching to a new phone.
```

---
## \#44 Posted by: longhairedboy Posted at: 2017-07-14T14:28:45.841Z Reads: 171

```
That odometer functionality is a must. And holy crap what if you could also store that data in the board and reset the odometer PER COMPONENT? My motors have about 300 miles on them, the ESC is fresh and only has five.. but the pack has 210 charge cycles according to that smart BMS somebody is inventing that talks to the UART, so its time to....

Yeah. That needs to happen. Modular onboard log storage as well as in your phone with the onboard data being the master in the sync process since its constantly receiving write requests.
```

---
## \#45 Posted by: Jinra Posted at: 2017-07-14T14:38:43.477Z Reads: 170

```
[quote="longhairedboy, post:39, topic:27527"]
Does his software require a firmware update on the ESCs? I thought I read somewhere that it does.
[/quote]

Yep it's actually pretty simple, just go to his thread and follow the Dropbox link to download the files. You'll get a modified BLDC tool and f/w. Use the special BLDC tool and flash the 2.54 f/w to the vesc in the normal manner.

(FYI there's a bug with the osx client where it'll crash when the vesc reboots, this will happen when you flash. For me the vesc flashed successfully but it did give me a scare)
```

---
## \#46 Posted by: longhairedboy Posted at: 2017-07-14T14:41:04.914Z Reads: 169

```
OSX and windows? or linux too? Sorry, i know i should RTFM but i'm rapidly switching between this and actual life stuff right now and need to know all the things.
```

---
## \#47 Posted by: rpn314 Posted at: 2017-07-14T14:50:27.307Z Reads: 167

```
Yep. Available across the board. I've personally used it on all 3 systems (Mac principally, and virtual machines of ubuntu and Windows 10)
```

---
## \#48 Posted by: pshaw Posted at: 2017-07-31T01:06:20.780Z Reads: 160

```
So what's the consensus? Has anyone had success with 12S and FOC?
```

---
## \#49 Posted by: Eboosted Posted at: 2017-08-01T06:16:56.097Z Reads: 157

```
I have 12S on my Trampa, but I'm not confident to try even with my Focboxes.
```

---
## \#50 Posted by: pshaw Posted at: 2017-08-03T01:37:51.324Z Reads: 152

```
[quote="Eboosted, post:49, topic:27527, full:true"]
I have 12S on my Trampa, but I'm not confident to try even with my Focboxes.
[/quote]

Why not? I don't see what the issue would be? Isn't this tried and tested already?
```

---
## \#51 Posted by: Hummie Posted at: 2017-08-03T01:58:24.177Z Reads: 151

```
I use 12s and foc always.  been good to me.   I run at very low erpm with hub motors though and that's probably why  vesc 4.12...and other 4s
```

---
## \#52 Posted by: Yecrtz Posted at: 2017-08-18T21:24:43.387Z Reads: 139

```
Does anyone has news on FOC @12s? With all these posts of focboxes blowing up I'm getting kinda worried.
```

---
## \#53 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-19T09:32:10.463Z Reads: 133

```
How low erpm is very low? Like 40000 or less?
```

---
## \#54 Posted by: Hummie Posted at: 2017-08-19T16:19:48.966Z Reads: 129

```
I forget exactly what I am at with hub motors but had done the math before.   less than 40000.   voltage x kv x 7 I think gives you the erpm for a 14 magnet motor.   50 x 100 x 7....35000 I think.
```

---
## \#55 Posted by: trancejunkiexxl Posted at: 2017-08-19T16:33:32.615Z Reads: 130

```
FOC @ 12s began to cutout on me when trying to accelerate from speeds around 3mph, switched back to bldc no problems
```

---
## \#56 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-19T17:13:03.006Z Reads: 131

```
Never heard of that formula before, I'll research it a little. Thanks! :)
```

---
## \#57 Posted by: Yecrtz Posted at: 2017-08-19T17:21:58.896Z Reads: 132

```
On what kind of setup?
```

---
## \#58 Posted by: trancejunkiexxl Posted at: 2017-08-19T18:49:49.031Z Reads: 132

```
12s2p single 6355 190kv focbox

mind you this was experienced when trying to power through intersections from full stop
```

---
## \#59 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-21T21:35:44.079Z Reads: 114

```
[quote="Hummie, post:54, topic:27527"]
voltage x kv x 7 I think gives you the erpm for a 14 magnet motor.   50 x 100 x 7
[/quote]

If you had a motor with 28 magnet, would it be 14 instead of 7 in that formula?
```

---
## \#60 Posted by: BigBoyToys Posted at: 2017-08-21T22:22:32.116Z Reads: 111

```
Yes, 28 pole motors have 14 pole pairs.
```

---
