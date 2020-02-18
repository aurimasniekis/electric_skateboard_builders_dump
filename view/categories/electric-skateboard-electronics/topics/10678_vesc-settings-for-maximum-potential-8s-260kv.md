# Vesc Settings for maximum potential (8S, 260kV)

### Replies: 94 Views: 6853

## \#1 Posted by: ThomasRBK Posted at: 2016-10-05T13:18:25.408Z Reads: 508

```
Hey there fellow builders, I bought a second hand board bout I don't really understand what all the settings do in the BLDC tool. I want to know if I'm using my full boards potential. Below are the parts.
_Turnigy Aerodrive SK3 - 6354-260kv 2360W max 70A 8s-10s_
_4x MultiStar 4s 5,2A ( 2xseries)x2 in paralel giving: 8s4p10.4A at 10c_
I find the board kind of lacking in the initial torque departement so I thought maybe something isn't configurated the best way possible. Thanks in advance!
<img src="/uploads/db1493/original/3X/9/e/9e7ba360183584968cbaa5f32ee07fb874d70dfa.png" width="690" height="407">
```

---
## \#2 Posted by: treenutter Posted at: 2016-10-05T13:23:42.575Z Reads: 460

```
@ThomasRBK set Max ERPM to 60,000 or less to avoid exceeding VESC's RPM limit. You motor KV is  a little above the recommendation for 8S so this will help to avoid problems.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2016-10-05T13:25:41.341Z Reads: 458

```
If you want more power then set the motor max to 60 or 70 and the if that still isn't enough set the battery max to 40.
```

---
## \#4 Posted by: ThomasRBK Posted at: 2016-10-05T13:26:19.396Z Reads: 454

```
This won't hurt the motor? Don't wanna ruin my stuff because of this :stuck_out_tongue:
```

---
## \#5 Posted by: ThomasRBK Posted at: 2016-10-05T13:26:27.046Z Reads: 437

```
Thanks for the warning!
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-10-05T13:29:05.816Z Reads: 422

```
That doesn't hurt. Maybe the belt because there will be more power. And set motor min to - 60 and bat min to at least - 12.
```

---
## \#7 Posted by: ThomasRBK Posted at: 2016-10-05T13:30:19.179Z Reads: 408

```
Doesn't this store potential power and then kills the vesc?
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-10-05T13:37:48.409Z Reads: 396

```
No it doesn't.
```

---
## \#9 Posted by: ThomasRBK Posted at: 2016-10-05T13:38:17.494Z Reads: 390

```
But the motors produces current when rolling right? Where does that power go then?
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-10-05T13:43:14.474Z Reads: 390

```
Only when you break or give power otherwise it doesn't in current mode.
```

---
## \#11 Posted by: ThomasRBK Posted at: 2016-10-05T13:44:13.666Z Reads: 383

```
Ooh I didn't know that man, thanks. Can you let it produce power when not accelerating though?
```

---
## \#12 Posted by: Ackmaniac Posted at: 2016-10-05T13:51:37.668Z Reads: 377

```
Touch the break and it produces power while you break and charges the battery.
```

---
## \#13 Posted by: ThomasRBK Posted at: 2016-10-05T13:53:47.944Z Reads: 369

```
Changed eRPM to 60.000 now, motor max 50, motor min -60, batt min -12. This should be good right?
```

---
## \#14 Posted by: Ackmaniac Posted at: 2016-10-05T13:54:55.151Z Reads: 369

```
Test it and have fun
```

---
## \#15 Posted by: saul Posted at: 2016-10-05T14:07:49.472Z Reads: 368

```
motor min looks high, i think i have -40/ -45... it will have hard breaking. I would move in smaller increments.
```

---
## \#16 Posted by: ThomasRBK Posted at: 2016-10-05T20:35:31.076Z Reads: 360

```
Changed it :slight_smile:
```

---
## \#17 Posted by: JuniorPotato93 Posted at: 2016-10-06T02:45:18.965Z Reads: 360

```
Hey, how has the board responded to the changes? I have the same set up on a new board and will have to change the settings on mine because it experiences the same issues with acceleration and breaking and in fact is actually an 8S battery as well with the same settings apart from I had already set the max erpm set to 60000.

Question to others here, should the max input voltage be equal to that of the fully charges battery pack of 33.6 and not set to 50 or does that not matter?
```

---
## \#18 Posted by: Jinra Posted at: 2016-10-06T02:49:41.252Z Reads: 351

```
Leave it at default 57v, no need to change it.
```

---
## \#19 Posted by: JuniorPotato93 Posted at: 2016-10-06T03:02:11.733Z Reads: 355

```
Well then, will change that back then. 

I do have a follow up question with regards to the motor max. The motors we have are rated for 70A max continuous and so if we set the motor max and min to be like 60A/-60A respectively, woukdnt that be 10 amps more than the continuous of the VESCs at 50A?
```

---
## \#20 Posted by: Jinra Posted at: 2016-10-06T03:05:55.602Z Reads: 350

```
there's more current running through the motor than what is supplied by the battery. The VESC can handle 50A continuous battery current, but you'll never run at that current for most users. You draw ~20 tops accelerating on flats, more if you floor it with high settings.
```

---
## \#21 Posted by: JuniorPotato93 Posted at: 2016-10-06T03:09:45.423Z Reads: 332

```
Well shit. I have a horrible grasp on the magnitudes of these things. I'm definitely more mechanically inclined so that is very useful to know. Thanks.
```

---
## \#22 Posted by: ThomasRBK Posted at: 2016-10-06T13:14:11.160Z Reads: 329

```
Could it be that it doesn't work when the battery gets low? It doesn't accelerate now...
```

---
## \#23 Posted by: ThomasRBK Posted at: 2016-10-06T16:42:50.784Z Reads: 329

```
Nevermind, found the problem: Bullet connector was a bit loose... :sweat_smile:
```

---
## \#24 Posted by: sandrewvdv Posted at: 2016-11-14T20:37:10.027Z Reads: 318

```
any update on this setup? I also have a 260 kV motor and would like to test it with 9s (with Erpm limit set at 60000). Does this change anything about the start torque?
```

---
## \#25 Posted by: ThomasRBK Posted at: 2016-11-14T22:14:04.542Z Reads: 307

```
Well I rode it for like 30-40k max, because the weather is getting too bad to ride in the Netherlands. I had no problems with the settings whatshowever, and I think you'd be able to push it ever farther if you wanted to. I'll upload a screen of what I use now just to make sure you use the same. With a 9S setup you need to change the voltage limits and I think 8S is the best with a 260kV motor, but that's another post on the forum.
<img src="/uploads/db1493/original/3X/3/8/3861679ab095d4d769a5ae03fbd2ded65e21bad9.png" width="690" height="409">I
```

---
## \#26 Posted by: benwong Posted at: 2016-11-15T06:16:31.006Z Reads: 283

```
wow, motor max can push till 50A, i should try try~~
```

---
## \#27 Posted by: ThomasRBK Posted at: 2016-11-15T06:34:05.722Z Reads: 273

```
Depends on how many S you run though, because otherwise you'll exceed the maximum wattage.
```

---
## \#28 Posted by: benwong Posted at: 2016-11-15T06:35:10.417Z Reads: 277

```
i am running 8s lipo 5000mah 20c.. 
so maximum potential i should rise to 50a?
```

---
## \#29 Posted by: ThomasRBK Posted at: 2016-11-15T06:36:09.585Z Reads: 275

```
Had no problems in terms of cutouts and heat, so you should be safe but I'd try 40 first and then check just to be sure.
```

---
## \#30 Posted by: benwong Posted at: 2016-11-15T06:37:29.515Z Reads: 277

```
okay..got it~~ 
what is your max speed can reach?

pulley ratio?
```

---
## \#31 Posted by: ThomasRBK Posted at: 2016-11-15T06:38:59.483Z Reads: 269

```
Top speed stays the same, only thing that changes is the acceleration thus how fast you get there ;) I have the 12mm kit from enertion.
```

---
## \#32 Posted by: ThomasRBK Posted at: 2016-11-15T06:40:06.944Z Reads: 265

```
http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-pulley-drive-hub-kit/
```

---
## \#33 Posted by: Ackmaniac Posted at: 2016-11-15T07:16:45.488Z Reads: 263

```
Set the motor max to 70 and give it a try. You could reach those amps only till you go half speed. Afterwards the battery max reduces everything. So you would only hit the max amps for about 2 or 3 seconds.  
And depending on your battery you can also raise the battery max. Because at the moment it is quite low. If you have a single drive you only set your system up to around 1036 watts (3,7V * 8S * 35A = ). Set battery max to 50 A (1480Watts) or 60 A (1776 Watts). I drive my single with 1600 and my dual with even 2400 watts.
```

---
## \#34 Posted by: LukeL Posted at: 2016-11-15T14:20:18.359Z Reads: 257

```
What happens when you reach the MAX ERPM, will it just cruise at that speed? I have read other people calling it a cutoff/hard setting which i would assume shuts down the board?
```

---
## \#35 Posted by: ThomasRBK Posted at: 2016-11-15T14:35:30.624Z Reads: 250

```
The Vesc will generate a fault code and it will shut off. It will coast and you won't be able to brake.
```

---
## \#36 Posted by: LukeL Posted at: 2016-11-15T14:53:56.695Z Reads: 249

```
thanks for the reply, this seems like a bad idea right, i don't imagine the friction would slow you fast enough and i don't fancy trying to foot brake at 30mph

is this correct:
60000(ERPM)/7(PP) =  8571 RPM (motor side)
8571/2.4(gear ratio 15:36) = 3571 RPM (Wheel side)
3571*80*pi(wheel circumference) = 897597 mm per min = 33mph

do the soft ERPM  limits in the ppm tab stop this happening, could I set that end limit to 60,000 and leave the MAX ERPM 100,000
```

---
## \#37 Posted by: ThomasRBK Posted at: 2016-11-15T15:17:41.241Z Reads: 237

```
I'd change the max eRPM just to be sure, kind of a fool proof safe more than anything. Your 33mph is a nice theory but I think with human loads and friction you'll really 28-30mph, and honestly that is pretty scary :slight_smile:
```

---
## \#38 Posted by: treenutter Posted at: 2016-11-15T16:23:30.985Z Reads: 241

```
[quote="ThomasRBK, post:35, topic:10678"]
Vesc will generate a fault code and it will shut off. It will coast and you won't be able to brake.
[/quote]

I don't think this is right. When you reach max ERPM the VESC will stop supplying additional current so that you don't exceed the RPM you've programmed. It's smooth and just means that more throttle doesn't increase your riding speed any longer.

I use ERPM limits to cap my top speed and it works well. My VESC doesn't shut off or restart when I get to that RPM.
```

---
## \#39 Posted by: Jinra Posted at: 2016-11-15T16:24:57.255Z Reads: 234

```
I have a board on the bench, I should just test this when I get home. I've always heard conflicting stories. Nothing beats first hand experience! Maybe I'll make a video to settle it once and for all :smiley:
```

---
## \#40 Posted by: Ackmaniac Posted at: 2016-11-15T16:28:08.169Z Reads: 236

```
The VESC doesn't shut down when it reaches the max ERPM. It starts to brake until it is again below or equal to that ERPM. So if you would set this to 10km/h it feels a bit rouph because it would switch constantly between accelerating and braking. So it is better to set the soft ERPM Limit so that it starts to reduce the power before it reaches this ERPM. To shut down would be stupid.
When it reaches the soft ERPM limit it only drives the system with "Min Current" which is set in the advanced tab. So you have a soft behavior when you reach the max speed. And the difference between soft ERPM Limit start and end should have minimum a difference of 1000 ERPM because the VESC can't detect a constant ERPM, It fluctuates between +-400 ERPM.

And when you have a 8S system with 260 kv you won't reach that ERPM when you stand on the board. Only on the bench you could reach it. I simply set my system always to 60000 max ERPM, soft limit start 58000 and soft limit end 60000. And i can reach those speeds only on the bench with 12S 190kv. When i stand on the board i can't because the efficiency of the motor doesn't allow that.
```

---
## \#41 Posted by: Jinra Posted at: 2016-11-15T16:34:47.090Z Reads: 220

```
There are two places to specify an eRPM limit; one in the motor tab and one in app config, are you talking about both of them?
```

---
## \#42 Posted by: Ackmaniac Posted at: 2016-11-15T16:36:59.583Z Reads: 216

```
Yes.
Motor 60000
PPM start 58000
PPM end 60000
this way you are on the safe side. Only on a extremely steep hill where you could reach like 60 km/h without a motor you would get problems.
```

---
## \#43 Posted by: Jinra Posted at: 2016-11-15T16:38:26.335Z Reads: 205

```
Hm good to know, I'll play around with it when I get home as well. Honestly, I'm not ever comfortable going my top speed downhill anyway. Sounds suicidal.
```

---
## \#44 Posted by: ThomasRBK Posted at: 2016-11-15T18:21:02.071Z Reads: 204

```
Looking forward to the results man!
```

---
## \#45 Posted by: Ackmaniac Posted at: 2016-11-16T12:52:26.023Z Reads: 214

```
And you can also switch off the breaking in the general motor tab. Because it can be very disturbing at lower speeds. For example when you set the board for a maximum of 20 km/h to give it to the kids. This way the board stops powering instead of braking which can bring them out of balance.

<img src="/uploads/db1493/original/3X/8/9/89495bccbbd41983698094ce7b69615569e04c7e.png" width="690" height="407">
```

---
## \#46 Posted by: lrdesigns Posted at: 2016-12-09T05:11:25.369Z Reads: 203

```
Hi Guys really liking this thread. So the consensus is for safe ERPM

 - Motor tab 60k max. With negative torque turned off. 
But what does min ERPM do? Should we also set to -60k ? Or is this only relevant when reverse is used?

- App / PPM Tab. Soft limit start 58k / Soft limit end 60k. 

If you exceed the ERPM going down a hill what will happen, will it damage the VESC? If you are on throttle or coasting does it make a difference?

Thanks.
```

---
## \#47 Posted by: ThomasRBK Posted at: 2016-12-09T09:46:24.579Z Reads: 198

```
If you exceed your max eRPM the Vesc will shutdown, but if I recall correctly it won't be damaged. I don't know what min ERPM does but my guess is that it's the minimal RPM the motor goes for when you press the throttle.
```

---
## \#48 Posted by: Ackmaniac Posted at: 2016-12-09T12:33:40.361Z Reads: 200

```
Min ERPM is for max speed in reverse. So the same like max ERPM but only backwards.
```

---
## \#49 Posted by: Hatman30 Posted at: 2017-11-20T21:11:38.360Z Reads: 128

```
In the respect of max and min erpm being both limited to 60k, how come the gen 1 Raptor has them both set to 100k? Thx
<img src="/uploads/db1493/original/3X/d/0/d018e2de4c93cfdb783f8be5c9d0c4ca3e346d1c.jpeg" width="666" height="500">
```

---
## \#50 Posted by: Ackmaniac Posted at: 2017-11-20T23:28:07.085Z Reads: 119

```
Because 190kv motors at 10S with 14 magnets don't reach that speed.

So even at a full charge the max erpm at no load (free spinning wheels) are 190kv * 10S * 4.2V * (14 magnets / 2) = 55860 ERPM.

When you stay on the board (with load) they might reach 50000 ERPM max.
```

---
## \#51 Posted by: ltlderek Posted at: 2018-02-08T16:00:15.883Z Reads: 108

```
I have a 260kv motor with two 5000Mah 4c (14.7v) batteries in series, would anyone know if these settings would apply? Or am I just severely underpowering my VESC?
```

---
## \#52 Posted by: cliofreak Posted at: 2018-02-22T23:49:42.663Z Reads: 111

```
Hey,

I have serious voltage sag when going up medium hill and pretty much just stops on steeper inclines.
Im running 10s4p 30Qs with Vesc and 6374 200KV motor.

I think it might be because Ive got conservative settings in my Vesc but I could be wrong. Here is a bit of a screen grab from the Metr app. Any ideas whats going on!?

What should my settings be to get max performance (without blowing up Vesc)? 
![59|690x86](upload://jYAwql3bKLHKcOayzHh2IJpQnD6.png)
```

---
## \#53 Posted by: cliofreak Posted at: 2018-02-22T23:58:11.726Z Reads: 112

```
![IMG_0187|230x500](upload://kAdy6Q9lC77pzJPaFscZm1WlSTL.jpg)![IMG_0184|230x500](upload://kBX1k8ul8WMZv3ARNyQ9HHFGcmv.jpg)![IMG_0186|230x500](upload://Jpv5GPUcZyBaQlMesknfyXgM5t.jpg)![IMG_0185|230x500](upload://rsZZ5qdyHHzd9seoWWNnK7WGM3W.jpg)
```

---
## \#54 Posted by: PXSS Posted at: 2018-02-23T00:01:18.400Z Reads: 101

```
Your battery current max is low for a 30Q 10S4P. You can upp that to 60A if you want to.

Batt current max regen is too low. That should not be below -16A. I'd say a min of -20A
```

---
## \#55 Posted by: cliofreak Posted at: 2018-02-23T00:04:31.694Z Reads: 100

```
Awesome, just the kind of answer I was hoping for!!!
```

---
## \#56 Posted by: PXSS Posted at: 2018-02-23T00:05:36.765Z Reads: 112

```
Motor current can also be upped, to 80A maybe. Some people do up to 120A but I say 80 is more than plenty.

Battery voltage cutoff is too high for a 10S in my opinion. There is nothing wrong with where you have it but decreasing it to 31/28 will give you 15ish% more range.
```

---
## \#57 Posted by: cliofreak Posted at: 2018-02-23T00:06:15.575Z Reads: 113

```
Yes!! I knew I was under selling this setup!
```

---
## \#58 Posted by: PXSS Posted at: 2018-02-23T00:09:44.314Z Reads: 114

```
15kW is wayyyy too high for your max wattage. Like extremely dangerous high! 2500W should be more than plenty. Same thing with your braking wattage, way too high. You could burn a motor like that. -1000W is plenty there. 

Your max erpm reverse is also wrong. Set it to the negative of the maximum erpm
```

---
## \#59 Posted by: cliofreak Posted at: 2018-02-23T00:12:55.782Z Reads: 109

```
I think the motor is rated at 3000W. I didnt even really look at those settings! I just followed a really simple Vesc setup tutorial that skipped all of that. Thanks man! Anything else before I loose your knowledge!?
```

---
## \#60 Posted by: PXSS Posted at: 2018-02-23T00:17:01.481Z Reads: 106

```
Thats basically it as far as what I see wrong. You may want to start there and fine tune based on your needs. Make sure you reread all of my comments as I tend to edit a lot so you may have missed something if I edited after you read it.
```

---
## \#61 Posted by: cliofreak Posted at: 2018-02-23T00:27:30.221Z Reads: 108

```
![IMG_0192|230x500](upload://amv0p7nW5OC46ax9JB3F7EPID0R.jpg)![IMG_0189|230x500](upload://dEAjzVKtV8G4ixanj1v1cZqwDKK.jpg)![IMG_0188|230x500](upload://lMzKJ5zmMTtz5Y83umx9lObHJCw.jpg)![IMG_0190|230x500](upload://ehxh6ppwM1QencaYFxXApPBR4Qy.jpg)![IMG_0191|230x500](upload://9qUcoThfKaYLO5nuT4VpzDDDZ0g.jpg)
```

---
## \#62 Posted by: cliofreak Posted at: 2018-02-23T00:28:34.375Z Reads: 96

```
Just followed your instructions... all look cool!?
```

---
## \#63 Posted by: PXSS Posted at: 2018-02-23T00:38:44.667Z Reads: 96

```
Yep. Looks good. That's just a starting point though. You should definitely read up on things and try to get a better understanding of all the settings and fine tune them for what you need. 

You also need to look up how to set up your failsafe in your remote/receiver and ESC if you have not.
```

---
## \#64 Posted by: cliofreak Posted at: 2018-02-23T00:41:22.806Z Reads: 95

```
Thanks man, I didnt even know there was a 'failsafe'. Ive built a bunch of multicopers and they had failsafe for return to home etc. Not sure what a failsafe on a skateboard could be for.
```

---
## \#65 Posted by: PXSS Posted at: 2018-02-23T00:42:02.245Z Reads: 94

```
Losing signal while on full throttle. Try braking then. ;)
```

---
## \#66 Posted by: cliofreak Posted at: 2018-02-23T00:44:52.178Z Reads: 95

```
Ahhh. Im on 2.4 rather that a bluetooth connection so probs less likly to drop out but I guess its possible. As long as it doesnt throw on the brakes randomly!? Thatd be worse than no brakes.
```

---
## \#67 Posted by: PXSS Posted at: 2018-02-23T00:46:38.881Z Reads: 95

```
It depends on the remote. Some may apply full brakes when you lose signal, that's why you need to set up your failsafe. Make it do what you want.
```

---
## \#68 Posted by: cliofreak Posted at: 2018-02-23T00:49:05.959Z Reads: 98

```
Im pretty sure some dont have a fail safe option if its anything like the rc quadcopter world. I remember havin to get a more expensive receiver that had a fail safe mode. Im using a GT2B in a 3d printed case.
```

---
## \#69 Posted by: mmaner Posted at: 2018-02-23T03:59:20.380Z Reads: 97

```
The GT2B has a failsafe...

http://www.electric-skateboard.builders/t/board-got-stuck-on-full-throttle-with-no-brakes-what-could-cause-this-related-story-slid-my-e-skate-for-the-first-time/26314/12?u=mmaner
```

---
## \#70 Posted by: cliofreak Posted at: 2018-02-23T10:38:28.937Z Reads: 97

```
Hey, 

I did all the fixes and its definitly more eager to go but its still 'sagging' on the hill and even on a very slight slope right after the hill... kinda like it hasnt recovered yet. Here is the data: https://metr.at/r/W5XFi


I think this is an overheating issue based on what ive read on here??  Im running MBS 100mm wheels on 15/36T. You think this is causing it!?

I think I need 40T Pulley. But, where the hell do I get one without a $40 shipping from US to UK!?
```

---
## \#71 Posted by: pat.speed Posted at: 2018-02-23T11:37:41.627Z Reads: 91

```
I don't think that could be causing it to overheat, I am running 14:27 on 97mm wheels and my stuff doesn't overheat or sag. Although I do run dual 6355 but that isn't much different in terms of torque
```

---
## \#72 Posted by: cliofreak Posted at: 2018-02-23T11:42:13.475Z Reads: 88

```
Thanks,
are you running up hills ok?
```

---
## \#73 Posted by: GrecoMan Posted at: 2018-02-23T11:55:14.986Z Reads: 86

```
it’s definitely possible. my vesc started thermal throttling within 5 minutes of riding on single 10s/190kv. 16/36 gearing and 97mm wheels

doesn’t do it anymore since I changed to dual and made a massive heatsink 😜
my vescs don’t get above 40c anymore.
```

---
## \#74 Posted by: cliofreak Posted at: 2018-02-23T13:28:01.112Z Reads: 83

```
I just changed back to my 90mm wheels to see if it made a difference...
YES, indeed it did. It lost a bit of power near the top of the hill but it was way way way better than the 100mm MBS. I wonder will a 40T pully have the same effect an allow me to run the 100mm?

The Metr stats are interesting too. I accidentally left the app running for about 20min after i shut down the board. Dunno if that made a difference. It shouldnt have. What you think? Lower temp ave etc![36|690x256](upload://zLMXXjngaanUXWz4IdG1M259aOV.jpg)
```

---
## \#75 Posted by: cliofreak Posted at: 2018-03-17T14:30:45.235Z Reads: 78

```
Hey, I want to make a torque monster while fixing previous issues...

So Ive done a few changes:

Ive now got 83mm Wheels (had 100 and 90s before)
Ive now got a Focbox (had a Maytech Vesc)
Ive now gone from 15/32 to 15/42T
Im still running 10s4p with a single 6374 200Kv

Initial very brief testing is very impressive. Wheel spin says it all really!

I just want to double check on some of my numbers if someone could have a look? @PXSS ?

![IMG_0448|230x500](upload://kiDIzGoariO5XRFJDJn84IRkVQr.jpg)![IMG_0453|230x500](upload://hYprF85AiteVEquWywm6KC1EVFK.jpg)![IMG_0452|230x500](upload://bNqDp3b41z0mmZvHpiKQNBAcyhm.jpg)![IMG_0449|230x500](upload://8kCCLD3FaQ35XkOV4Kvr7rEP5tY.jpg)![IMG_0451|230x500](upload://xGqwoRDczzE1xa8kMqKKn40SvXC.jpg)![IMG_0450|230x500](upload://8nUCtvldLvXbFkqUgKq0T8QrOVi.jpg)![IMG_0446|230x500](upload://oGKeqCzCFQ1goKE6RR2MPQm5j7j.jpg)![IMG_0447|230x500](upload://941uQO1k8pv0dFFqcmUnmDC5LUK.jpg)![IMG_0445|230x500](upload://frgRmzD93sSUZexGfAyXjbdSWjK.jpg)![IMG_0443|230x500](upload://8LQMrlFbkyF77xOO6CSz8lBlLTj.jpg)![IMG_0444|230x500](upload://1Q1rUtqtqsbWJjy1XiJxBkWTPeT.jpg)![IMG_0442|230x500](upload://a87L5j2ppeQudi7XYISfUI5Ps2H.jpg)
```

---
## \#76 Posted by: cliofreak Posted at: 2018-03-17T17:44:33.360Z Reads: 67

```
For what its worth, some big changes now that I've changed all these elements listed above. 

This is 15/42 with Focbox and 83mm Wheels...
Obvious differnce is Max temp, down from 78 deg to a very safe 62 deg with no 'sag' what so ever. Result. I suppose I should try the 100mm on this new 42T pulley/focbox setup to just to see if it makes much difference to the Vesc temp. I miss the smoothness of them.

Also, the 83mm single drive is wheel spinning, even goin up hill.


![46|690x85](upload://mbH1gLfLn4deCCSFM1dTvGwNHDM.png)
```

---
## \#77 Posted by: cliofreak Posted at: 2018-03-17T20:04:09.242Z Reads: 71

```
Ah sweet! 
So happy that the 100mm MBS wheels have not hampered the performance too much. This is the same run as the previous ones. Max temp only went up 1 deg C. This run includes a 200mtr very steep incline near the end of the 4km (possibly 25-30%). No issue at all.

The 83mm wheels had crazy torque but the 100s are totally acceptable with the ability to roll over anything being the biggest selling point. In the dark I went over a inch thick plank at 15mph with no issue, thankfully. 

SO, I dunno whats done the most good... Focbox rather than Maytech Vesc OR the 42mm Pulley instead of the 32.

![22|690x82](upload://pGCHjbX2zts1rQV6BB95nZi87uM.png)
```

---
## \#78 Posted by: PXSS Posted at: 2018-03-17T21:09:04.479Z Reads: 65

```
Try out the 32mm pulley with fb. This is really good data
```

---
## \#79 Posted by: cliofreak Posted at: 2018-03-17T22:11:30.335Z Reads: 61

```
Im pretty sure that'll be very similar but with less torque. The Focbox really keeps the temp down vs the Vesc.
```

---
## \#80 Posted by: cliofreak Posted at: 2018-05-05T09:58:30.515Z Reads: 56

```
So I’ve been riding with the 90mm wheels, Focbox, 15T 42 10s4p 30Qs 200kv 6374.

Can I push the battery max from 60 to 80? 

I’m getting awesome torque now but topping out around 20mph. I’m wondering if I up the max battery amp will I:
1. Fry my battery
2. Live a beautiful life filled with torque and top end.
```

---
## \#81 Posted by: professor_shartsis Posted at: 2018-05-05T12:12:18.780Z Reads: 54

```
[quote="cliofreak, post:80, topic:10678, full:true"]
So I’ve been riding with the 90mm wheels, Focbox, 15T 42 10s4p 30Qs 200kv 6374.

Can I push the battery max from 60 to 80?

I’m getting awesome torque now but topping out around 20mph. I’m wondering if I up the max battery amp will I:

Fry my battery
Live a beautiful life filled with torque and top end.
[/quote]

@cliofreak according to my calculations your top speed jumps from ~24mph to nearly ~49mph by simply switching the motor pulley from 15t to 39t (red line, bottom left chart - vehicle thrust minus wind drag force)...

34v pack, 0.1ohm winding, 200kv, 2 motors, 90mm tire, 42t wheel, 15t vs 39t motor, 80a motor amp limit & 60a battery limit, bldc mode
https://image.ibb.co/fpRkjS/15t_vs_39t.gif
```

---
## \#82 Posted by: cliofreak Posted at: 2018-05-05T13:39:50.111Z Reads: 51

```
Interesting, however... a 39T motor pully!? 

It’d take too much torque to turn that surly.
```

---
## \#83 Posted by: professor_shartsis Posted at: 2018-05-05T13:41:25.677Z Reads: 48

```
@cliofreak predicted peak vehicle thrust would drop from 106lbs (15t) to 41lbs (39t)... take a look at the yellow line, bottom left chart (vehicle thrust pounds - 2 motors)
```

---
## \#84 Posted by: cliofreak Posted at: 2018-05-05T15:01:52.450Z Reads: 49

```
Yeah that’s a crazy loss. I’d get 32mph+ just by going 15T 32T with 100mm wheels I’d imagine, while still keeping mediocre torque.
```

---
## \#85 Posted by: professor_shartsis Posted at: 2018-05-05T16:24:37.564Z Reads: 48

```
@cliofreak with 15t motor 32t wheel, 100mm wheel about 34mph top speed and 73lbs peak thrust is predicted (versus 24mph & 106lbs w/ 15t 42t 90mm).

https://image.ibb.co/cWU017/100mm.gif
```

---
## \#86 Posted by: cliofreak Posted at: 2018-05-05T16:26:25.952Z Reads: 44

```
So, any thoughts as to why my 10s4P wont charge past 61%?

Im using BMS only for charging.
```

---
## \#87 Posted by: Colson003 Posted at: 2018-05-07T17:20:02.813Z Reads: 43

```
Sounds like one P group has died or just disconnected
```

---
## \#88 Posted by: cliofreak Posted at: 2018-05-07T19:40:18.886Z Reads: 43

```
Yeah, one or maybe one has taken out 4? 60% sounds like it’s become 6s4p rather than 10s4p? Would it still function like that!?
```

---
## \#89 Posted by: Colson003 Posted at: 2018-05-07T20:19:24.873Z Reads: 43

```
No it’s likely just one p group. 10S full charge - 42v so take away 4.2v from that, given that it’s one p group, is  37.8v. That would be about 61% like you said. So it’s just 9s right now. You should open it up.
```

---
## \#90 Posted by: cliofreak Posted at: 2018-05-07T21:18:59.536Z Reads: 38

```
I know that must make sense but I can’t see how 4 Cells (4 18650s ) could account for 40%?
```

---
## \#91 Posted by: TehAtheist Posted at: 2018-05-07T21:27:51.632Z Reads: 36

```
0% is not 0V.

0% = 37V I believe?
100% = 42V
So 60% = 40V

If 1S isn't connected or died or whatever, there is a series voltage of 3.7-4.2 volt missing.

Hence, your 42V becomes suddenly much less, even when only 1S is gone. It looks as if your battery is depleted, but actually 9S is fully charged and 1S is not, I suppose. Or, you know, something along those lines.

Although your battery meter indicates only 60% is charged, the actual battery WH isn't 40% less than what it used to be.

Atleast, that is my understanding. But I do suppose that a bad group could be bad for the rest, so taking them out is a must?
```

---
## \#92 Posted by: cliofreak Posted at: 2018-05-07T21:52:42.518Z Reads: 37

```
Ahh, that makes sense I think. 
The group shouldn't be bad. I mean, they've only had about 15 full charges and Ive never depleted past about 40%. Theyre good 30Q cells so I'm gonna presume its a break in the  wiring. I'll have to open it up and get the multi-meter out! 

I do feel like I've lost a bit of power. Its maxing out at about 20mph and I think it used to be more.

Ive got a 15T 42 with 90mm wheels so I know Im sacrificing top end but 20mph seems too low for 10s4p.
```

---
## \#93 Posted by: TehAtheist Posted at: 2018-05-07T22:12:49.911Z Reads: 38

```
Max speed is not related to power but to voltage 🙂.
```

---
## \#94 Posted by: cliofreak Posted at: 2018-05-08T14:34:30.942Z Reads: 36

```
So, 

My 10s4p is giving only 37.8 V on full charge and is only showing as 61% charged. There’s a bad pack or a bad connection. I’ve used multimeter on whole pack and the issue starts at B6. So, am I looking for a bad connection between B5 and B6, or a bad connection between B6 and the BMS?

I've found that a pack in the middle isn't showing any voltage. The packs either side are OK.
What would cause this!!?![31964074_10160357957130223_3987592227680419840_n|666x500](upload://vl7RocJTR5ht7brsHkF8wvkIAJY.jpg)![32191275_10160357997865223_4477597637662474240_n|666x500](upload://whSqFZL0iUZj09I5Qpa8fRri8Vb.jpg)![31961034_10160357957285223_947015377957683200_n|666x500](upload://nh3rQq4kY2OWcSkb0UxA6wNJLEJ.jpg)
```

---
