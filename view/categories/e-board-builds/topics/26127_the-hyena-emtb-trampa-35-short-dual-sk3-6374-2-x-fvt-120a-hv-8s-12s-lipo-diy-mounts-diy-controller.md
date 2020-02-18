# The Hyena EMTB &#124; Trampa 35 short &#124; Dual SK3 6374 &#124; 2 x FVT 120a HV &#124; 8S/12S lipo &#124; DIY mounts &#124; DIY controller

### Replies: 55 Views: 6617

## \#1 Posted by: vap Posted at: 2017-06-25T08:54:54.131Z Reads: 431

```
Hi, just finished my first build.
Trampa 35 short
SK3 6374 192 KV
Maytech VESC (!!BOTH MINE EXPLODED, DO NOT RECOMMEND!!)
8S/12S lipo, gonna start with 8S2P using 4x turnigy 4S 5000mah 25c, later add more to 12S2P with BMS and brick-charger
DIY aluminium mounts
3D printed pulleys
DIY controller using Arduino nano + NRF24l + OLED + power bank circuit + 750mah quadcopter lipo + central part from old quadcopter controller stick
HTD 5m 460x15mm belts, with idlers, 1:5 gear ratio, 15t motor, 75t wheel
http://i.imgur.com/dQkc83F.jpg

Image dump:
35 Short, cause i'm "small adult" and  also these things are expensive XD
http://i.imgur.com/ooHiGlj.jpg
The recommended 14 ply seems too stiff, but the heck do i know about mountainboarding. Probably gonna cut the board later to make it more holypro-ish
http://i.imgur.com/OjBYuX5.jpg
http://i.imgur.com/ztJXbYf.jpg
http://i.imgur.com/84FBk3x.jpg
Found a perfect box locally
http://i.imgur.com/83D9ZPc.jpg
Had to find a drill press to drill these clamps
http://i.imgur.com/x2FaeB5.jpg
Finding right people to 3d print took some time (still haven't found where i could print with thicker walls or even 100% fill, these are 25% infill)
http://i.imgur.com/26nW9SS.jpg
http://i.imgur.com/XGPecvZ.jpg
Testing vescs
http://i.imgur.com/YxLcT9u.jpg
Controller with telemetry
http://i.imgur.com/LcE8lnh.jpg
http://i.imgur.com/9HuSqb5.jpg
MDF prototype
http://i.imgur.com/ojafPKn.jpg
http://i.imgur.com/hi51Xxh.jpg
I don't have access to proper tools, but this chair-saw did the job amazingly well, i've cut second mout in  about 15 minutes (drilling and aligning took another hour though)
http://i.imgur.com/8gwl1SM.jpg
Complete mount
http://i.imgur.com/VVfqdT5.jpg
Idler
http://i.imgur.com/IsJGGZp.jpg

Just did a few runs before the rain started again, woah this thing has some crazy punch. Not sure if i want 12s.
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-25T10:36:06.591Z Reads: 330

```
Awesome looking setup, this is basically 2 of my board in one :) speaking of how much was the total hardware cost?  I think I ended up around $600 (not including things I fried along the way) but was really shooting for the low budget board since I didn't have a lot to spend on it.

These trampa boards seem pretty sweet but think the board and shocks and whatnot cost more than my whole setup.  Agree 12S is overkill, I did that for a while but scaled it back to 10S when I needed to redo my lipo box anyway cause going that fast on a skateboard is unnecessary I need to slow down at intersections anyhow so getting up to top speed usually wasn't practical (think you can also just scale back the settings in the VESC(s)).

Glad to see someone else is crazy enough to make their own remote too :) shared mine on github here ( https://github.com/shusain/eskatecontroller ) would be curious to see your code, I actually have one of those OLEDs laying around (made internet controlled frogger on it) and was thinking about putting it in my remote would like to see what you decided to use it to display.
```

---
## \#3 Posted by: vap Posted at: 2017-06-25T11:21:15.060Z Reads: 319

```
Yep, it was exactly twice your costs.
http://i.imgur.com/qVDJXMJ.png
I live in a small city in Russia, and the roads are pretty bad around here, i can ride my normal longboard only in the city center.
I've been wanting to make some kind of portable electric transport for a long time, and this year i've discovered mountainboards, that combine all the qualities i wanted.

Cool, gotta dig through vesc config, cause i've already ordered 12s BMS.

:+1: My code is almost the same :),  I'll post the code later, for now the OLED only displays voltage, amps and speed. I want to add menu pages with distance, amp hours, and so on, cause you can only read one value while riding anyway. I've also wired the 5 position joystick from camera osd http://surveilzone.com/OSD-Cable-For-HS1177-Camera-g-1816  i make quadcopters so i've got quite a few of these lying around.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-06-25T11:37:01.191Z Reads: 297

```
Awesome!! also into quadcopter builds too though haven't gotten out to fly enough this summer.  This is my first electric build, but great that people like you and others shared experiences and build lists like this on the forum really helps out the noobs like myself find our way around.  Good deal on the motor mounts too, everything else looks around about what I'd expect, what I paid times 2, for 2 of them :) and trampa board isn't quite as much as I expected.  Curious what kind of range you'll get out of that beast, I can go 12 miles then my 5Ah 10S battery bank is pretty drained (80-90% or so)? **Edited I wrote 10Ah bad habit of adding everything up, they are in series**
```

---
## \#5 Posted by: vap Posted at: 2017-06-25T17:15:07.805Z Reads: 286

```
First test went awesome.
http://i.imgur.com/uk9cgNb.jpg
I'm covered in dirt, i love how this thing drifts on gravel, acceleration is crazy. Used half the battery, super fun.
I had some minor issues with motor connectors disconnecting at one point, and motor pulleys get clogged with dirt.
Also really need a wrist strap on the controller
Also cooling
```

---
## \#6 Posted by: itzsiebe Posted at: 2017-06-25T20:27:54.920Z Reads: 274

```
@vap
What is the range and the top speed?
```

---
## \#7 Posted by: vap Posted at: 2017-06-25T20:56:30.220Z Reads: 270

```
Don't know yet, i'm not gonna go far or fast until i test everything.
The theoretical top speed on fully charged 8s is 45 km/h.
```

---
## \#8 Posted by: vap Posted at: 2017-06-26T19:45:14.492Z Reads: 268

```
Secured all guts, still mess of wires
http://i.imgur.com/VvLHxxk.jpg
also cooling
http://i.imgur.com/EhU5KAk.jpg

Tuned the truck stiffness, i love how it feels now, this thing rolls over everything, and bindings give so much control.
Noticed after the ride one of the clamps started slipping, gotta add some aluminium strips connecting 2 clamps.
```

---
## \#9 Posted by: jess.t.moody Posted at: 2017-06-26T20:12:31.094Z Reads: 258

```
This is a great build! I really want a trampa, but can't justify the cost at the moment. I might just try slapping some all terrain tires on my current (normal) eboard until then. Yeah, I'm surprised those 3d printed gears/pulleys put up to that kind of stress at 25% infill! Even at 100% infill, some folks say metal's the only way to go. Your build proves otherwise I guess.
```

---
## \#10 Posted by: vap Posted at: 2017-06-27T09:50:35.572Z Reads: 252

```
I'm curious how long the pulleys would last, couple of spares are already in transit.
Probably i'm just going easy on the throttle for now, and i weigh 63kg at the moment. I'd imagine someone who's 90-100kg needs a lot more torque.
```

---
## \#11 Posted by: benwong Posted at: 2017-06-27T10:04:42.038Z Reads: 251

```
you fit battery and vesc in a same box? i feel that abit dangerous of it. 
anyway, your build is look awesome with DIY mounting and remote~~
```

---
## \#12 Posted by: vap Posted at: 2017-06-30T19:07:52.296Z Reads: 247

```
Hmm, haven't thought about that, can make some kind of fire retardant wall later.

Here's some video, still figuring out how to film this.
https://www.youtube.com/watch?v=UN0DYBLPfWI

Small mount fix to prevent clamp slipping:
http://i.imgur.com/BAWYFyW.jpg
In the last 3 long rides clamps haven't moved.
```

---
## \#13 Posted by: vap Posted at: 2017-07-03T16:18:42.605Z Reads: 240

```
I'm thinking of a name for my board. How about "the hyena"
Drifting on ground is tons of fun, gotta get padded shorts though.
I'm hitting ABS_OVER_CURRENT every time past certain speed, happens only on solid road.
So i accelerate, then sudden loss of thrust, and then after a short delay it shoots forward.

Here's the dump, only 2 of those are from startup on soft ground (justified), the rest happened at high speed.
https://pastebin.com/6Wb6SuQd

I'm not sure if "Battery max" and "Absolute max" apply for one VESC or for both.

Hmm, maybe i need better capacitors.

Spare pulleys arrived
http://i.imgur.com/aE8LkP2.jpg
```

---
## \#14 Posted by: vap Posted at: 2017-07-13T05:13:14.885Z Reads: 231

```
Sadly, i tried 12s and both my vescs exploded.
http://i.imgur.com/rnb58EQ.jpg
I only got about 10 rides :(
http://i.imgur.com/4fQMEHw.png

Anyway, that's $200 totally wasted.
Now i need new speed controllers, NOT vescs, and NOT from maytech.
```

---
## \#15 Posted by: benwong Posted at: 2017-07-13T06:45:44.811Z Reads: 221

```
damn, another proof to bang my head with NO-GO with Maytech VESC on MTB. 
@vap Sorry to hear that fried your VESC. 

Is this fried while riding normal terrain or off road with aggressive acceleration?
```

---
## \#16 Posted by: vap Posted at: 2017-07-13T08:32:56.075Z Reads: 217

```
Standing in place at home.
```

---
## \#17 Posted by: benwong Posted at: 2017-07-13T08:36:08.014Z Reads: 214

```
GOSH~~ something wrong with wiring ? short circuit? 
if not, too weird to be fried while "standing in place at home". 

:fearful:
```

---
## \#18 Posted by: vap Posted at: 2017-07-13T08:53:56.099Z Reads: 216

```
I did few test rides on 12s. First they were cutting off on 55amp max current (drv faults), so i lowered it to 40. It got better, no drv faults just overcurrents sometimes, but then 1 vesc just died, showing no LEDs at all.
Weirdly it still worked on 8s voltages and lower.
So i upped the voltage limit to 55v.
Plugged in 12s, it worked, motors spinned. I stood on the board, went couple of meters at home back and forth. Then, when i was standing for a couple of seconds in place, it all exploded.
I think only one vesc exploded, causing chain reaction.
```

---
## \#19 Posted by: benwong Posted at: 2017-07-13T08:57:40.455Z Reads: 216

```
that is so weird fried but still work in 8S. 
Chain reaction is most scary. cause two Vesc dead instant. 
There is lucky din hurt yourself. 

What is your next plan?
```

---
## \#20 Posted by: vap Posted at: 2017-07-13T10:07:46.874Z Reads: 215

```
[quote="benwong, post:19, topic:26127"]
What is your next plan?
[/quote]
1) Be really sad
2) Ask around about those 120a 12s FVT escs
3) If they are good, use them
```

---
## \#21 Posted by: benwong Posted at: 2017-07-13T10:10:56.389Z Reads: 203

```
Lolx, sad for a few hour and start research again. 
FVT can refer my reply from other thread. 
http://www.electric-skateboard.builders/t/help-choosing-electronics-trampa-e-mtb/27427/13?u=benwong

Cheer and Chill mate~~
```

---
## \#22 Posted by: vap Posted at: 2017-07-13T10:38:18.863Z Reads: 199

```
Thanks!
So Sleeping Lions work reliably on 12s.
How do you program them? Do they have usb port or need extra programmer?
Also where did you buy them?
```

---
## \#23 Posted by: Okami Posted at: 2017-07-13T11:49:13.835Z Reads: 201

```
Ask this in the other thread too maybe, there is a dedicated thread about.

http://www.electric-skateboard.builders/t/efx3-trampa-holypro-35-esc-fvt-120a-tunigy-sk3-6374-149kv-lipo-16ah-8s/14305/55
```

---
## \#24 Posted by: vap Posted at: 2017-07-15T13:47:31.504Z Reads: 210

```
Thanks.
I've contacted FVT, gonna order them lions.

I'm starting to have second thoughts about the batery i've soldered
http://i.imgur.com/9ghhUWa.jpg
http://i.imgur.com/TCEMEkQ.jpg
Cause i've used a bunch of 4s batteries it turned out a horrible mess of wires.
I've used acid flux to solder aluminium and nickel, and then neutralized it with soda, so it looks extra ugly.
It seems to be fine for now, and single port charging works, just worrying about some wires breaking off or cells going bad and killing whole thing in the future.
```

---
## \#25 Posted by: Smorto Posted at: 2017-07-15T16:04:38.760Z Reads: 197

```
That looks scary to me... If it works maybe secure everything with hot glue then shrink wrap it.
```

---
## \#26 Posted by: Okami Posted at: 2017-07-15T16:23:30.445Z Reads: 200

```
I agree.. i would isolate these connections.. if one wire breaks loose.. it might touch things it usually shouldnt touch lol
```

---
## \#27 Posted by: vap Posted at: 2017-07-16T14:17:59.693Z Reads: 208

```
Of course it was hot glued and taped all over, i opened it to add extra balance plugs for voltage checking.
I'll probably take it apart into 4x6s batteries, with their own connectors. If i place escs outside the box, there's enough space for wire harness.
Anyway soldering a lipo is so much stress, never want to do that again :|

I'm a little spooked after one of my quadcopter batteries almost burned during charging recently. The voltage on 2 cells out of 4 froze at 4.0 and it got hot, good thing i've noticed it.
```

---
## \#28 Posted by: vap Posted at: 2017-08-10T11:00:23.239Z Reads: 206

```
Some updates.
http://i.imgur.com/Tti3jnb.jpg

Took the battery apart into 6 x 4S. This way i can alternate between 8s/12s using different wire harness. For now running 8S 15Ah
http://i.imgur.com/y2nV2Ho.jpg

Been using FVT 120a for a couple of weeks now.
They arrived in different colors, and one of the capacitors was dented.
http://i.imgur.com/Xfq21uW.jpg
I opened the esc to check if the cap was shorted, cap was fine, but some other components were pre-burned inside, and it's before i even powered it:
http://i.imgur.com/dnF7576.jpg
Surprisingly ESC still works, though it frequently loses sync if i spin it without load.

Second ESC works alright, though BEC failed soon after installation, gives 0 volts on red wire. Powering everyhting from first ESC.

I have mixed feelings about these ESCs. They are very powerful, can handle lots of amps, and with a small fan they stay completely cool no matter the load. They can go full power from standstill, and do a sick wheelie (later about that).  Can startup uphill in sensorless mode, can startup rolling backwards. I like duty cycle control a lot more than vescs current control. Works a lot better offroad, on vescs speed offroad drops significantly, while these escs don't care about the type of the road. And also i'm using expo (x^1.5) on the throttle, feels great.

Brakes are a little tricky, the curve is very steep, i had to trim the PWM output to the spot before they completely block the wheels. I can still access full brakes if i press the button on the controller. Already got used to them.

What i don't like about them: sometimes after braking they go crazy and apply full throttle from standstill. You never know when the board is gonna do a wheelie. Happens 1-2 times a ride, usually goes away on it's own or i have to reboot. Also rarely they go into some protection mode(?) and limit speed to 10-20% for a few seconds. Happens after sudden wheelies or hard bumps (less than once a ride). Also on 12s it happens a lot more frequently, and sometimes they loose sync under load on 12s, so for now still running 8s.

http://i.imgur.com/X7Oww1F.jpg
Added some extra caps, startups feel better now, though glitches persist
http://i.imgur.com/ptd8fwi.jpg
Esc box is water-resistant, got into a rain once, the box was dry inside. The escs are hot-glued to the lid.
http://i.imgur.com/SuWhEFZ.jpg

Switched to MT60 connectors, they're pretty good
http://i.imgur.com/WbHwXG2.jpg
Also changed all the crappy zinc plated screws to fancy hardened-steel hex screws.

Ready for the night ride
http://i.imgur.com/uVCx3dq.jpg

I need stronger pulleys now
http://i.imgur.com/3JN5db3.jpg
```

---
## \#29 Posted by: vap Posted at: 2017-08-10T11:08:23.893Z Reads: 194

```
Oh and some video. Rode my board to the motocross spot, but because of constant rains the track is all overgrown, oh well
https://www.youtube.com/watch?v=4HTSJQ2cBS8
```

---
## \#30 Posted by: vap Posted at: 2017-08-20T08:56:27.399Z Reads: 188

```
Oh btw, pulleys can be easily fixed with styrofoam+acetone mix
http://i.imgur.com/hUUxZiX.jpg
holds up pretty well
http://i.imgur.com/u4tvqvJ.jpg
Also initially i wiped them with acetone.
They break when i land on the pulley itself, like rolling over rocky terrain or a broken curb.
```

---
## \#31 Posted by: vap Posted at: 2017-09-17T23:08:55.080Z Reads: 177

```
Had 2 pretty bad falls in one day, next day got a cold, didn't ride for 2 weeks. I'm back.

Swag from @trampa
https://i.imgur.com/IS6SUgA.jpg
No more rattling for now
https://i.imgur.com/kag44YP.jpg

And new pulleys from @idea:
https://i.imgur.com/mIgCNz0.jpg
3mm walls, just tested them, work fine :+1:

Here's the model if anyone needs it, original was made by a friend of mine, this one is modified by me:
https://dl.dropbox.com/s/tiymrytcc12uycg/Pulley_HTD-5mm_75_tooth_width_15mm_V3_2.stl
```

---
## \#32 Posted by: pat.speed Posted at: 2017-09-18T10:44:59.536Z Reads: 164

```
Have you looked at the new firmware for the escs it is meant to fix lots of the issues your having with them
```

---
## \#33 Posted by: vap Posted at: 2017-09-19T11:53:58.654Z Reads: 159

```
I'm using **Mountain skateboard_120A (5-12S) _ singleDrive _170818**  from here http://www.szfvt.com/en/download-6.html
I think it has less problems, though can still go crazy sometimes.
```

---
## \#34 Posted by: pat.speed Posted at: 2017-09-19T12:08:59.111Z Reads: 157

```
Ah ok. Maybe I was thinking of the firmware fix for the sleeping lion Esc
```

---
## \#35 Posted by: vap Posted at: 2017-09-19T13:09:44.261Z Reads: 150

```
It is sleeping lion, they are very inconsistent with naming :D
```

---
## \#36 Posted by: pat.speed Posted at: 2017-09-19T21:01:11.385Z Reads: 144

```
Oh wow now I'm confused😂 There was a thread on the problem and someone found firmware that fixed the issue
```

---
## \#37 Posted by: pat.speed Posted at: 2017-09-19T21:06:30.926Z Reads: 149

```
Found it scroll down to post 59 or 60 and the new firmware that someone found is there although you may already have this

https://www.electric-skateboard.builders/t/efx3-trampa-holypro-35-esc-fvt-120a-tunigy-sk3-6374-149kv-lipo-16ah-8s/14305/69
```

---
## \#38 Posted by: vap Posted at: 2017-09-26T11:12:33.279Z Reads: 141

```
Yea, i already have the latest firmware. Same problems, probably would work better with sensors.
I'm kinda used to riding without triggering sudden wheelies - just don't let it freewheel and limit the brake.
```

---
## \#39 Posted by: vap Posted at: 2017-09-26T11:31:24.478Z Reads: 148

```
Brakes are very dangerous on this thing at speed, can suddenly block and cause you to loose control. I still have bruises from a month ago.

**The obvious lesson for me is - don't ride at speeds beyond your skills.**

So staying on 8s, also thinking of freeboard bindings. Couldn't find them for a reasonable price though, official site asks $75 for the shipping.

Finally getting charging system working.
[36v 180w power supply](https://www.banggood.com/36V-180W-AC-DC-Switching-Power-Supply-Board-High-Power-Industrial-Power-Supply-Module-p-1111658.html)
[36v CCCV DC-DC module](https://www.banggood.com/DC-DC-8A-300W-Buck-Adjustable-Solar-Charging-LED-Driver-Vehicle-Power-Supply-Module-p-1166654.html)
(hah, just noticed, it's listed as 32v, when i was buying it was 36v)
First try - blown crappy caps
https://i.imgur.com/6UWEhHi.jpg

Replaced all the caps, real ones are quite bigger, charging at 5 amps:
https://i.imgur.com/PBl4Oqb.jpg
Quite pleased with the balancing.
```

---
## \#40 Posted by: linsus Posted at: 2017-09-26T11:43:23.846Z Reads: 142

```
Hi, Just stumbled upon your post. The VESC is not recommended to run on 12S, there are many known issues about this before you. Simply does not hold for that voltage. Bummer you had to find out by plugging them in.

I recommend searching benjamins forums in the future, board looks great tho!

//Linus
```

---
## \#41 Posted by: GCB Posted at: 2018-01-04T23:48:12.452Z Reads: 126

```
Kinda looks like a time bomb :grin:
```

---
## \#42 Posted by: vap Posted at: 2018-01-10T18:07:12.121Z Reads: 130

```
Winter insulation:
https://i.imgur.com/5qyGQKA.jpg
https://i.imgur.com/It16rcG.jpg
https://i.imgur.com/ARcEtVT.jpg

Seems to be working.
```

---
## \#43 Posted by: vap Posted at: 2018-01-10T19:42:53.749Z Reads: 128

```
And in case anyone is wondering, riding on snow on stock wheels is quite possible and is a lot of fun. (i'm using fresh trampa treads)
Pushing on rear truck and a wheelie can help starting up. With a bit of momentum i can ride through pretty deep snow.
Grips get icy and slippery :expressionless:
Tried zip ties on the tyres, they work well, noticeable improvement in traction, though they all popped after 15 minutes.

https://i.imgur.com/qxgRBw8.jpg

@trampa Any plans for winter tyres?
```

---
## \#44 Posted by: trampa Posted at: 2018-01-10T20:58:08.146Z Reads: 126

```
Snoe chains.. @barajabali made some last winter. I think someone has used wood screws as spikes, some years back.

Frank
```

---
## \#45 Posted by: telnoi Posted at: 2018-01-10T21:28:38.951Z Reads: 120

```
Great thread and awesome to see that so much can be done with regular tools.

Are those bushings in the second picture? Of what exactly? Judging by the count (5), I am hoping these are not the original truck bushings.
```

---
## \#46 Posted by: Yecrtz Posted at: 2018-01-10T21:59:00.232Z Reads: 114

```
Noticed the same with the zipties. They eventually fly off. Would love to hear more from trampa about potential winter wheels. Riding through a moderate layer of a snow was fine.. but 13+ cm was impossible.
```

---
## \#47 Posted by: vap Posted at: 2018-01-10T22:05:43.995Z Reads: 116

```
I thought about @barajabali chains, but there's not enough clearance on my build for them. Though i can extend pulleys and make new cross bars, maybe next year.
```

---
## \#48 Posted by: vap Posted at: 2018-01-10T22:09:26.985Z Reads: 118

```
[quote="telnoi, post:45, topic:26127"]
Are those bushings in the second picture? Of what exactly? Judging by the count (5), I am hoping these are not the original truck bushings.
[/quote]

Yep, these are truck bushings, i got about 30 spares. They don't last long.
```

---
## \#49 Posted by: barajabali Posted at: 2018-01-10T22:27:52.239Z Reads: 118

```
I’m going to redesign my chains to be cheaper and lighter.
```

---
## \#50 Posted by: vap Posted at: 2018-01-13T14:14:49.419Z Reads: 115

```
Just had an idea, 40-60mm clamp:
https://i.imgur.com/j56c3kE.jpg
Enough clearance:
https://i.imgur.com/YN6stEN.jpg
(3pcs for a dollar :D)
```

---
## \#51 Posted by: vap Posted at: 2018-01-18T23:22:59.136Z Reads: 112

```
https://i.imgur.com/68yp6lV.jpg?1
https://i.imgur.com/iMu774P.jpg?1
Nope, they lasted a bit longer than zipties, but not much. Every single one popped.
The belts and pulleys are okay, but would not attempt again.
https://i.imgur.com/1azIOUE.jpg?1
```

---
## \#52 Posted by: Okami Posted at: 2018-01-19T13:35:04.766Z Reads: 104

```
Did it have any extra grip at all? It is hard to judge whenever they add more grip or not
```

---
## \#53 Posted by: vap Posted at: 2018-01-19T15:00:29.239Z Reads: 107

```
Oh yes, forgot to mention. Difference in forward traction is very noticeable especially on startup. Without them i have to put all weight on rear truck to start. They dont add any sideways traction.

I think they break because of constant flexing, when tyre compresses. I'll try to see what i can do with steel cable, nylon belts or rope :) fun stuff
```

---
## \#54 Posted by: vap Posted at: 2018-01-24T20:16:07.560Z Reads: 99

```
https://youtu.be/Wc475O_rTuE
```

---
## \#55 Posted by: Chrisjarram Posted at: 2019-01-13T08:11:32.049Z Reads: 37

```
I couldn't help but hear the A-Team theme tune in my head the whole time I was reading this thread - all while still reeling from the possible consequences of sitting on the wrong chair in your house...
```

---
