# Board gets jumpy (stutter) at low and mid speeds

### Replies: 12 Views: 1287

## \#1 Posted by: Mackyfury Posted at: 2016-09-11T11:42:40.103Z Reads: 148

```
Wattup fellas! I just finished my first build thanks to everyone here and all the posts I vultured over the past few months. I was able to find all my info thanks to the search button but now I'm in a slight stump. 

I'll start with my setup and then my problem

-12s lipo 4x 3s zippy 5000 20c (100A?)  split and spliced into 2x 6s packs.
-Gt2b with mad munkey mod from FLATLINEcustoms on thingiverse
http://www.thingiverse.com/thing:1550237
*broke first potentiometer so modded steering wheel pot to fit.*

-14t enertian pulley
-38t 3D printed Kegel Hub from JuniourPotato93 on thingiverse http://www.thingiverse.com/JuniourPotato93/designs/page:1?sort=&filter=&search=Kegel
-265belt
-torqueBoards mount 
-Dual Ollin Motors
-Dual Vesc from Ollin

  **VESC SETTINGS**
 -BLDC Current w/ brake no reverse
 -motor max..........40 
 -motor min regen 20
 -batt max ............30
 -bat min regen ....10 
-startup boost .010 (set to .025 but didn't test yet due to rain)

BATT
-Min input........8v
-Max input......52v
-Cut off start...39.6v
-Cut off end....36v

So she has a weird characteristic. During bench testing the motors will keep spinning for a quick moment even after release the throttle at around 60+% in display tab. Same thing happens when I'm riding. The throttle will stick on release for a sec on initial take off which gets kinda scary haha. It will also do this when I'm rolling at a fast coast and throttle in to pick up speed.. Next thing I noticed is if I hold steady throttle at a good speed for a while It'll do a quick stall back with an audible "Jump" or "stutter" noise from the motor (not the belts slipping). When I did a bench test I grabbed one motor and was able to stop it easily by hand creating the same sound and the other wheel kept spinning. I don't have traction control enabled so I'm not sure if this is correct... Next part, last night I forgot to install a belt and went to a friends place. After a few beers :blush: : I was dying to ride so I removed the motor wires on the belt less wheel and went for a spin. I instantly noticed the problems were gone and it absolutely ripped! Hahah. After that, I started to think my dual drive issue needed more attention. Thank you guys so much, and sorry for the novel. :grin:
<img src="/uploads/db1493/original/3X/e/9/e95e68b25af7adfa240347a27d1e386c83c747f2.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/3X/a/2/a2f7f97fe33da23e505417ea04ec523d6f97b6c6.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/9/2947be15de399e4704ec3e99ed7aa38e6d6b9e54.jpeg" width="375" height="500">

Edit: forgot to add thingiverse links
```

---
## \#2 Posted by: Ackmaniac Posted at: 2016-09-11T12:07:56.742Z Reads: 134

```
this seems to me a problem with your receiver. It looses the connection. So it keeps on going with the last throttle position that it knows. And then after 1 second without a signal it stops powering. then it get's again a throttle signal so it powers again.

Long story short. Make a quick test by placing your receiver cable **not** between the wires. 
Give it some space (no touch with other wires). Maybe that helps.
```

---
## \#3 Posted by: Mackyfury Posted at: 2016-09-11T12:17:47.641Z Reads: 128

```
That makes a lot of sense. I'm really familiar with Building and racing FPV quads and that is a common thing to consider in a build. I'll move the rx and give it a try tomorrow. Thanks!
```

---
## \#4 Posted by: bigpianist Posted at: 2016-09-12T11:58:31.528Z Reads: 104

```

I think I know your problem cause I was just dealing with it today! I got worried cause I thought I cooked a GT2B aswell because it started cutting out after I did a mad munkey mod!    Issue I found is the antenna in the transmitter. If you break it off or twist it funny, it isnt as simple as just soldering it on to the one pad. Bit of a hack! Theres actually two pads on the blue antenna board where the antenna connects. If one of them breaks off the pad, you get patch AF reception especially when riding in the street!     So check the tiny little bit where the antenna attaches because chances are one of the two wires from the antenna has broken off.    If it is that then the fix is easy!
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-09-12T12:40:15.573Z Reads: 94

```
[quote="Mackyfury, post:1, topic:9387"]
-Max input......52v
[/quote]


Leave the Max Input at 57V
```

---
## \#7 Posted by: Mackyfury Posted at: 2016-09-13T00:50:09.887Z Reads: 75

```
She runs like a champ:heart_eyes:! After the fixes, we ramped up the amp limits and for the first time it actually scares me. This thing has so much torque I have a clip of my buddy spinning tire on dry road LOL. Will post soon


@bigpianist that totally helped with the sticky throttle situation! I opened controller back up and redid my solder, I actually broke off the unshielded area and replaced it before..Similar crappy range like u mentioned. Also  failsafe cause the steady throttle when out of "range" for a split second. Re-set failsafe with fixed antenna and no more stuck throttle!

 @JohnnyMeduse that was also the solution for the random cut outs!, Max V was too low and the voltage spikes caused the in and out stumbles.


Thanks so much guys!

In a nut shell

 1. Cut outs from the receiver, failsafe causing steady throttle after release at random times 

2. Maxx volt cut outs causing the board to skip under high load
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-09-13T01:15:28.568Z Reads: 70

```
Now just go outside and Enjoy.... And don't forget safety 3rd 😉
```

---
## \#9 Posted by: bigpianist Posted at: 2016-09-13T01:28:18.405Z Reads: 68

```
Yeah have fun mate! Stuck throttle on mine scared the hell out of me hahaha hated it
```

---
## \#10 Posted by: Mackyfury Posted at: 2016-09-13T10:58:59.230Z Reads: 63

```
haha thanks guys! @JohnnyMeduse @bigpianist. Speaking of safety 3rd and stuck throttles. Here's a little clip from the day we messed around on bldc... my buddy went down prety good haha. 
https://youtu.be/Z4ecFtBWB0o
```

---
## \#11 Posted by: bigpianist Posted at: 2016-09-13T11:04:11.587Z Reads: 59

```
Hahaha what a nasty stack! my mate went down speed testing my board when I was using some hobbyking boat escs :joy: hit full throttle and the esc couldnt handle the timing! locked up both motors and off he fell     

He's the reason I bought VESCs :grimacing:     hes okay though and starting his own build ahaha
```

---
## \#12 Posted by: Mackyfury Posted at: 2016-09-13T11:17:02.560Z Reads: 56

```
HAHAH! damnnn dude, I can only imagine how that one went LMAOO.. That is super  ironic because my friend had the same reaction :joy: , he caught the bug and totally wants to build one after feeling the ride. It's poison :imp:
```

---
## \#13 Posted by: bigpianist Posted at: 2016-09-13T12:07:24.834Z Reads: 56

```
Yeah ahah the rush is amazing!    Doesn't feel like anything else out there and building is heaps of fun! (When it works out)
```

---
