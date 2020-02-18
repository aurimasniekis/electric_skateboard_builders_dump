# High pitch whining noise FOC Helical Drive

### Replies: 71 Views: 787

## \#1 Posted by: Trdolan03 Posted at: 2018-11-07T00:36:56.695Z Reads: 214

```
Hello everyone,
I am having this annoying high pitch whine whenever I hit 20mph on my eMTB after I get to about 25mph it will stop and be smooth again but I ride a lot in this middle range. My setup is 12s with FOC boxes @CarlCollins . 190kv 6374 from @torqueboards and 1:5 helical drives from @Nowind. Can anyone shed some light on how to eliminate this? My switching frequency is 30khz but it wasn’t any better at 20

Edit: sometimes it is very smooth into and out of the whining but other times the sound hits a brick wall and just stops on a dime

Link to video: https://youtu.be/_qZ143e7yH4
```

---
## \#2 Posted by: michaelcpg Posted at: 2018-11-07T01:03:36.456Z Reads: 202

```
I've had something like this with one of my APS motors, the outer ring and a couple of the magnets had partly come loose and were creating a fairly ugly whine in a certain RPM range. Maybe try figure out if the noise is coming from a specific motor and if so, pull the motor apart so you can inspect the magnets inside the can
```

---
## \#3 Posted by: PatRocks Posted at: 2018-11-07T01:35:54.015Z Reads: 188

```
Yep, loose magnets are most likely. Check the windings as well

Edit: loktite 648 should take care of it
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-11-07T01:44:02.485Z Reads: 175

```
Damn. Ok. Luckily I got some green loctite sitting around so I will try to fix this tonight. Just put some loctite on the magnet and then place it in the can?

Is there a quality motor that doesn’t have this issue? I have seen way too many cases of loose magnets recently
```

---
## \#5 Posted by: Trdolan03 Posted at: 2018-11-07T01:49:25.212Z Reads: 167

```
I will mark it as a solution once I get it solved😉
```

---
## \#6 Posted by: Trdolan03 Posted at: 2018-11-07T05:40:02.924Z Reads: 153

```
![image|375x500](upload://5hXxOCVtXuAcSTUUdYeixBpoxoR.jpeg) ![image|375x500](upload://ucEPdVBcqr2XXlmzt1LVxpYz9ni.jpeg) 
@torqueboards what is the problem/ solution here? I can’t see any obvious loose magnet but this wear is all the way around both the stator and can
```

---
## \#7 Posted by: torqueboards Posted at: 2018-11-07T05:45:39.075Z Reads: 149

```
@trdolan03 - You'll probably have to send that one in. Consistency on one of our latest batch hasn't been great on our 6380 Black. We have some new ones in production but won't be done until next month. Send us an email and let me know your @trdolan03 so I can remember this issue.

I still haven't isolated the actual high pitch noise specifically though.
```

---
## \#8 Posted by: Trdolan03 Posted at: 2018-11-07T05:49:50.803Z Reads: 145

```
@torqueboards  This is a 6374.
```

---
## \#9 Posted by: PatRocks Posted at: 2018-11-07T05:52:48.506Z Reads: 146

```
@torqueboards , exemplary customer service! @Trdolan03 , that's what you should do with the motor!
```

---
## \#10 Posted by: Trdolan03 Posted at: 2018-11-07T06:05:01.409Z Reads: 143

```
I added a video link to the original post. Watch only from 40 seconds to the end
```

---
## \#11 Posted by: Trdolan03 Posted at: 2018-11-07T06:12:08.977Z Reads: 135

```
@torqueboards email sent
```

---
## \#12 Posted by: Trdolan03 Posted at: 2018-11-08T00:00:49.521Z Reads: 130

```
So the motor in the pictures is not longer on my board and I am running single drive atm. Still getting the whine but now at 25-28mph. @Nowind Could this be a function of the helical drives?
```

---
## \#13 Posted by: CarlCollins Posted at: 2018-11-08T02:22:54.102Z Reads: 124

```
@Trdolan03
Please confirm is your setup is FOC or BLDC?
```

---
## \#14 Posted by: Trdolan03 Posted at: 2018-11-08T02:23:26.824Z Reads: 120

```
[quote="CarlCollins, post:13, topic:73761"]
Please confirm is your setup is FOC or BLDC
[/quote]

I’ve tried both and they both produce the same sound
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-11-08T02:24:09.882Z Reads: 121

```
@Trdolan03
If you are in FOC mode, try adjusting the frequency to 31K-35K using VESC tool
```

---
## \#16 Posted by: Trdolan03 Posted at: 2018-11-08T02:24:51.977Z Reads: 120

```
I tried 20k and 30k. I can try 35 tonight
```

---
## \#17 Posted by: Trdolan03 Posted at: 2018-11-08T02:55:34.108Z Reads: 116

```
No luck changing to 35k
```

---
## \#18 Posted by: CarlCollins Posted at: 2018-11-08T08:24:33.513Z Reads: 116

```
@Trdolan03

Have you asked @torqueboards about it?
```

---
## \#19 Posted by: rich Posted at: 2018-11-08T09:45:23.319Z Reads: 115

```
[quote="Trdolan03, post:12, topic:73761"]
Could this be a function of the helical drives?
[/quote]

100% not, they sound (I mean they don't sound :laughing:) equal no matter which speed.

This is for shure the motor. This whining sound reminds me on faulty APS 80mm motors which people posted. I know exactly how you feel now, chin up bro! I am also still searching for a reliable motor which holds longer than a few weeks, it's really frustrating.

These motors in general are made for hobby RC models and not for human transport I think this is the main problem regarding safety and reliability.
```

---
## \#20 Posted by: Andy87 Posted at: 2018-11-08T10:02:17.769Z Reads: 115

```
let me know in case you found one...
the problem is, when you think there is one long lasting motor they change something in production and the next who buy get shit again....
how about your sk8? still goes strong or already gave up?
```

---
## \#21 Posted by: rich Posted at: 2018-11-08T13:33:53.855Z Reads: 107

```
[quote="Andy87, post:20, topic:73761"]
how about your sk8? still goes strong or already gave up?
[/quote]

Well .......... Mounted them last month and had maybe 10-12 rides (180- 200km). One week ago I recognized the noise and it's getting worse  and worse. :tired_face:

https://youtu.be/g412YDp8u38
```

---
## \#22 Posted by: Andy87 Posted at: 2018-11-08T13:37:57.779Z Reads: 101

```
That I have seen, but you said you know that voice and you give that motor max 4-5rides before totally broke.
Was interested if that already happened or if it’s still ok.
Any feedback from hobbyking already?
```

---
## \#23 Posted by: rich Posted at: 2018-11-08T13:47:36.491Z Reads: 100

```
This is the third video of SK8 motor noise within 1 week and this is the worst :laughing: I didn't wrote HK yet, good reminder, I prefered riding.

[quote="Andy87, post:22, topic:73761"]
you give that motor max 4-5rides before totally broke
[/quote]

I had 3 rides so far, let's see.......
```

---
## \#24 Posted by: ethel Posted at: 2018-11-08T14:39:31.917Z Reads: 100

```
@rich 

Check this out. My motor sounded like @Trdolan03 and kept ridding until this new noise. 

 https://www.youtube.com/watch?v=8bGguXSdd68


![image|281x500](upload://xr89y1YmjGfCyD8RT61SL9TOE8o.jpeg) 

The motor stil does good enough for speed.
```

---
## \#25 Posted by: rich Posted at: 2018-11-08T14:42:08.587Z Reads: 95

```
Can't watch it, is it private?
Change it to "not listed"
```

---
## \#26 Posted by: ethel Posted at: 2018-11-08T14:47:23.682Z Reads: 88

```
Should be fixed now
```

---
## \#27 Posted by: rich Posted at: 2018-11-08T14:52:37.674Z Reads: 88

```
Damn :flushed:
```

---
## \#28 Posted by: torqueboards Posted at: 2018-11-08T14:59:17.615Z Reads: 87

```
@Trdolan03 Can you check to see if the cir-clip is obstructed? Does it freely spin when mounted to the motor mount on your gear drive.

@Ethel Yours could of been the same issue. I think you emailed us can you PM your email?
```

---
## \#29 Posted by: ethel Posted at: 2018-11-08T15:05:41.143Z Reads: 88

```
@torqueboards 🙌🙏

This 6374 motor cannot be service by you. I’ve ran it over 100s of miles, used the shit out of it. It’s not fair. I am going To test my new still in box  black 6380 motors unless you think I should swap them? 

Edit: oddly it did start to make noise when I updated Vesc settings to new FW and increased my motor max for MORE POWER. Could be coincidence
```

---
## \#30 Posted by: torqueboards Posted at: 2018-11-08T15:11:08.120Z Reads: 89

```
@Ethel You can still send it in and we can try if you want that is.

When did you get your 6380s? You should PM me as we seem to be having an issue with the 6380 Black for our last batch (retainer rings loose). We have some new ones that are in production with the issue fixed. We should definitely get yours fixed. It can be fixed by resealing the retainer ring with epoxy.
```

---
## \#31 Posted by: Trdolan03 Posted at: 2018-11-08T15:57:53.338Z Reads: 87

```
Yes the c clip is unobstructed. @torqueboards
I can send both motors in to your guys if you want to test them. I ordered a set of sk8 motors for the mean time.
```

---
## \#32 Posted by: Trdolan03 Posted at: 2018-11-08T16:23:15.679Z Reads: 83

```
@rich @torqueboards did you listen to the video?
```

---
## \#33 Posted by: Sender Posted at: 2018-11-08T16:27:29.520Z Reads: 83

```
So this is just on the blacks?  I have a pair of the silvers on the way.  No issues with those?  It will be a minute before I get a build up and running to test and don't want to wear out "warranty time"

Awesome that you are all over this!
```

---
## \#34 Posted by: Skunk Posted at: 2018-11-08T16:29:40.171Z Reads: 77

```
I have those motors in my cart right now. 
Curious myself.
```

---
## \#35 Posted by: rich Posted at: 2018-11-08T17:06:20.568Z Reads: 76

```
Yes if you mean yours in the OP

Once I had a Maytech motor which started with whining noises at higher speed and after some rides it sounded almost like the one from @ethel plus there was some resistance when spinning
```

---
## \#36 Posted by: ethel Posted at: 2018-11-08T17:40:55.652Z Reads: 75

```
Yep 👍🏼 

Mine does what yours does, except Mine is older motor. I hear the pitch noise at certain speed, under or over, noise is gone. However, I kept riding and the sound turned into what my video shows you. 😉
```

---
## \#37 Posted by: torqueboards Posted at: 2018-11-08T18:45:58.507Z Reads: 75

```
@Trdolan03 @Sender @Skunk @Ethel Yeah, obstructed C-clip is an issue typically more so for TB Mounts. This is mostly for 6380. The cir-clip is meant to be flushed but I believe, we needed an extra 1mm for 6380s so the cir-clip sticks up a bit. Could be for other setups but I'm not 100% sure, you'll have to check. You just want the cir-clip to spin with the shaft and not cause any added friction if it's stuck on a mount or what not. This goes for all motors too and can cause the "noise" you are experiencing @Trdolan03 (one of the reasons).

The fix for this would be to add M4 washers on the motor mount to gap about 1mm so the cir-clip spins with the motor shaft. See video below. I believe, this is what's mainly causing the retainer ring to be pushed out.

Although, this isn't the fix for ALL "high pitch whining noises". This is a possible solution for one.

https://www.youtube.com/watch?v=KjuMGeQHeLg	6374 6380 Motor CirClip

@Trdolan03 - I'd gap it 1mm and try it. You should be good by then. If not, let us know.

@Sender - Mostly, on blacks it seems but make sure that your cir-clip isn't obstructed. But yeah, we got you covered just let me know and I'll take care of you either way. If you want to double safe, you can add epoxy on the retainer ring but I believe the issue is caused by this cir-clip issue.

We tested like 20+ motors and for 6380s they all had this high pitched noise/resistance and the cir-clip was the culprit. Once we added the M4 washers to gap it 1mm. Everything was good.

@Skunk - So far everything seems to point to the cir-clip. You can purchase now or you can wait for the next batch which has fixed this issue. Either way now or later we got you covered.
```

---
## \#38 Posted by: Sender Posted at: 2018-11-08T19:13:14.524Z Reads: 71

```
Vendor action at its' damn finest!  Thank you!
```

---
## \#39 Posted by: Trdolan03 Posted at: 2018-11-08T19:26:51.843Z Reads: 71

```
[quote="torqueboards, post:37, topic:73761"]
Yeah, obstructed C-clip is an issue typically more so for TB
[/quote]

I am running @Nowind direct drive which has a hole in the motor mount wider than the c-clip.
```

---
## \#40 Posted by: torqueboards Posted at: 2018-11-08T19:27:36.563Z Reads: 70

```
@Trdolan03 Ok, got it. I think I read that wrong. I believe, you started an email so we'll discuss through there.
```

---
## \#41 Posted by: rich Posted at: 2018-11-09T00:17:07.415Z Reads: 68

```
[quote="Trdolan03, post:39, topic:73761"]
hole in the motor mount wider than the c-clip
[/quote]


Thanks, that made my day :rofl:
Perfect description for a massive hole which is bigger than the whole motor gear.
```

---
## \#42 Posted by: Trdolan03 Posted at: 2018-11-09T00:30:06.875Z Reads: 71

```
@rich  

@torqueboards I am still waiting on a response via email FYI
```

---
## \#43 Posted by: ElectricCoast Posted at: 2018-11-09T01:51:01.940Z Reads: 69

```
@torqueboards I'm having a high pitch issue as well on one of my two silver 6380s I just finished the build this morning running the motors on Kaly gear drives.  I have 3.5 miles on the motors.  First 2 miles were good.  Then high pitch noise at higher RPMs.  Lower seems fine.  There is a little bit of bell housing movement vertically compared to the other motor.  The high pitch begins when the RPMs cause the bell housing to move vertically.  Only moves maybe 2mm but just enough to so the sound is real bad.  It even sounds like the bearings are grinding.  Sent you a contact support request earlier today.
```

---
## \#44 Posted by: ElectricCoast Posted at: 2018-11-09T15:52:48.706Z Reads: 69

```
@torqueboards BTW I tried to install washers in between the motor and Kaly drive mount just in case and in my situation it didn't make a difference.  The sounds is sound bad that I am afraid to ride my board.  I sent an email response about the video link that Derek sent me explaining that the solution did not fix my problem.  This is a huge bummer since I only was able to ride the new build for 3.5 milles (2 miles were perfect).  It's killing me not to be able to ride my new build.  It's like Christmas morning but I'm being told i can't play with my new toy.  LOL
```

---
## \#45 Posted by: Rod12579 Posted at: 2018-11-09T16:16:29.184Z Reads: 68

```
Hey I have a set of 6380s from you guys (Black, 1st batch) I haven’t completed my build with them yet....I was thinking of pulling the motor apart and adding some 680 lock tight on the retainer ring...would that work just as well as epoxy or should I grab some epoxy? 🤷🏾‍♂️
```

---
## \#46 Posted by: torqueboards Posted at: 2018-11-09T16:18:25.142Z Reads: 66

```
@ElectricCoast - PM me your email. Did you already open a ticket?

@Rod12579 - I'd probably recommend a 2 part epoxy over the 6380. Don't have any exp trying 6380 with it so I'm not too sure.
```

---
## \#47 Posted by: ElectricCoast Posted at: 2018-11-09T16:47:46.260Z Reads: 63

```
@torqueboards PM'd you.  Found lower magnet ring loose on bell mouth.  It just fell off when pulling motor apart.  Should that be glued in place?  I'd like to put the motor back together but want to know if I should epoxy the ring in place.![20181109_101921|690x388](upload://w6zJBo3HZVrjH5Wyd3jGCYjWiiO.jpeg)
```

---
## \#48 Posted by: Kug3lis Posted at: 2018-11-09T16:55:36.603Z Reads: 62

```
@Trdolan03 that's a loose magnets had been listening to this noise for like a month so I know for sure. If you remove can it looks everything fine as magnets sticks to the enclosure so it doesn't move but at higher speeds magnetics get bigger and magnet starts lifting up from the enclosure and it causes small vibrations. 

You can take a flat screw driver and try to push under magnets some of them will definitely will lift up :)
```

---
## \#49 Posted by: Kug3lis Posted at: 2018-11-09T16:57:49.146Z Reads: 65

```
Use Loctite 648 :) or get magnet glueing Loctite or anything which is elastic and high temperature :)
```

---
## \#50 Posted by: torqueboards Posted at: 2018-11-09T17:08:28.320Z Reads: 63

```
@ElectricCoast The magnet should stick to the motor can. Is it no longer magnetic? I can also send you a new retainer ring. We just got some better ones in since yours is already off.

@Kug3lis - Nice find :smile:
```

---
## \#51 Posted by: Trdolan03 Posted at: 2018-11-09T17:11:54.292Z Reads: 65

```
@Kug3lis any idea about this wear pattern which is all the way around both the can and stator![image|375x500](upload://5hXxOCVtXuAcSTUUdYeixBpoxoR.jpeg) ![image|375x500](upload://ucEPdVBcqr2XXlmzt1LVxpYz9ni.jpeg)
```

---
## \#52 Posted by: telnoi Posted at: 2018-11-09T17:15:33.780Z Reads: 57

```
My SK3 sounded like that after 1000 km or so and now I am at 3000 total, same motor. Ride it till it disintegrates.
```

---
## \#53 Posted by: Trdolan03 Posted at: 2018-11-09T17:26:36.139Z Reads: 56

```
@Kug3lis @torqueboards  Does the ring need to be epoxyed in though?
```

---
## \#54 Posted by: torqueboards Posted at: 2018-11-09T17:57:30.572Z Reads: 57

```
@Trdolan03 Yeah, you want to epoxy the ring. I have some new ones if you want to wait a few days that I can send you the teeth on the retainer ring are longer. Let me know. As far as what Kug3lis said check the magnets esp the ones that are rubbing on the stator. See if they are loose or not flushed.
```

---
## \#55 Posted by: Trdolan03 Posted at: 2018-11-09T18:06:26.344Z Reads: 57

```
@torqueboards I was able to remove about 5 of the magnets which I reapplies with green loctite. If the new ring will make a different I am open to trying it. Did you still want me to send in the motor?
```

---
## \#56 Posted by: torqueboards Posted at: 2018-11-09T18:20:22.337Z Reads: 59

```
@Trdolan03 All the magnets you can actually remove. They aren't glued to the motor can. You can secure them to the motor can but make sure not to use too much that it adds to the thickness of the magnet otherwise it will rub against your stator.

Yeah, If you can wait. I'd suggest waiting for the new retainer ring. PM me your email so I can get those new retainer rings out to you. You can go ahead with the repair if you have issues afterwards just let me know and we'll take care of you.
```

---
## \#57 Posted by: Kug3lis Posted at: 2018-11-09T18:20:58.282Z Reads: 59

```
Not green but 648
```

---
## \#58 Posted by: ElectricCoast Posted at: 2018-11-09T20:58:26.411Z Reads: 56

```
The ring for the magnets appears to be aluminum and doesn't appear to be magnetic.
```

---
## \#59 Posted by: ethel Posted at: 2018-11-10T03:56:02.379Z Reads: 55

```
https://www.youtube.com/watch?v=R4jZfgO2oIs

I’m about to go for a test ride 😮 wish me luck 🤔😶
```

---
## \#60 Posted by: Trdolan03 Posted at: 2018-11-10T03:58:26.012Z Reads: 54

```
[quote="ethel, post:59, topic:73761"]
I’m about to go for a test ride :open_mouth: wish me luck :thinking::no_mouth:
[/quote]

It takes some big balls to ride that. I totally fucked up my can but the stator is in great condition. If it happens to be your stator causing the problems...
```

---
## \#61 Posted by: ethel Posted at: 2018-11-10T04:19:21.929Z Reads: 53

```
![image|281x500](upload://wrp1ghbYJERsDxAkKmPJYi4Ejbb.jpeg) 
👀
```

---
## \#62 Posted by: Trdolan03 Posted at: 2018-11-10T04:20:24.166Z Reads: 50

```
@ethel Holy fuck you're ballsy. 35.3mph with that motor.
```

---
## \#63 Posted by: ethel Posted at: 2018-11-10T04:20:52.089Z Reads: 49

```
I’m not sure what the foosticj  it is. But it still hit its gearing ratio speed
```

---
## \#64 Posted by: PatRocks Posted at: 2018-11-10T04:45:40.688Z Reads: 50

```
Dude, spinning that motor is damaging it every time you do it. It's only gonna get worse until it locks up.

Edit: it _is_ pretty funny though
```

---
## \#65 Posted by: ethel Posted at: 2018-11-10T05:20:37.139Z Reads: 52

```
Above a certain speed, noise ceases. It’s defiantly getting worse no doubt about it.

![image|281x500](upload://5X4TaS5QwQXKBrlMyU0251Mn6qp.jpeg)
```

---
## \#66 Posted by: torqueboards Posted at: 2018-11-10T14:37:42.673Z Reads: 50

```
[quote="ElectricCoast, post:58, topic:73761, full:true"]
The ring for the magnets appears to be aluminum and doesn’t appear to be magnetic.
[/quote]

Yeah, the ring isn't magnetic it is aluminum. I was referring to the magnets for Trdolan03's case.
```

---
## \#67 Posted by: Kug3lis Posted at: 2018-11-10T15:58:07.892Z Reads: 48

```
I was riding even worse situation :D

https://youtu.be/_jEw9UA6gx8

https://youtu.be/GnpjJCkaTmU

This is what I found after it finally locked up conveniently next to my home :D

![image|375x500](upload://e95NhGa7mpZMJCQiq8ScmIzm5Fv.jpeg)
```

---
## \#68 Posted by: Kug3lis Posted at: 2018-11-10T15:59:58.472Z Reads: 49

```
and this how motors sound with real brand bearings :P

https://youtu.be/ISuObS7DoY8
```

---
## \#69 Posted by: Linny Posted at: 2018-11-10T16:07:28.800Z Reads: 49

```
Hmm, i have two new black 6380s ordered from September. Have not opened it or anything yet. Should i be worried? @torqueboards
```

---
## \#70 Posted by: torqueboards Posted at: 2018-11-10T17:40:48.376Z Reads: 48

```
@Linny Up to you. You can inspect them or you can exchange them for when the new ones come in.
```

---
## \#71 Posted by: DerelictRobot Posted at: 2018-11-13T06:33:31.536Z Reads: 37

```
My exact situation/setup. I fixed the magnetic retainer ring and they were quiter for a bit, then as soon as I brought amps up to even 45, a twangy ringing noise around 16-20mph
```

---
