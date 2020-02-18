# Motor stuttering when I try to accelerate - where&rsquo;s my problem?

### Replies: 96 Views: 4269

## \#1 Posted by: Nicolai Posted at: 2017-04-29T01:24:58.463Z Reads: 359

```
I've been riding my esk8 for the last 8 months without any issues at all, then all of a sudden it stopped working on me today. Whenever I try to accelerate now, the motor violently stutters (so badly that it's far from being rideable), though the brake still works. I took my board apart and hooked up my VESC to my BLDC tool and I can't seem to find the issue. I tried accelerating and no fault code came up at all. However when I try to do a motor detection, after some angry violent stuttering from my motor, it keeps saying bad detection result received and "detection failed". 

Board specs:
Battery: Space Cell Pro 4
VESC: Enertion
Motor: Enertion 190kv

Below are my VESC settings. In my realtime data, is it normal that the "current in" stays so low when I accelerate?

<img src="/uploads/db1493/original/3X/7/9/798124ccfe93e9e18c23fe68f1b1844c9373189c.png" width="690" height="437"><img src="/uploads/db1493/original/3X/a/5/a5a864f9fa9f5bda9c74449a3ae77e09be1da0aa.png" width="690" height="435"><img src="/uploads/db1493/original/3X/b/3/b3f42c005c50f1bf68649884be65c31043c63d4e.png" width="690" height="435">

Any help is hugely appreciated! I hope I didn't short my motor...
```

---
## \#2 Posted by: mmaner Posted at: 2017-04-29T01:28:41.599Z Reads: 323

```
Sounds like a phase wire short to me.  I'd check your bullet connectors at the motor and the VESC.  Also check where the wires enter the can of the motor.  You may have to remove heat shrink to check it well, just replace it when you are done and don't short them.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-04-29T07:22:47.780Z Reads: 309

```
It could also be a disconnection of one of your phase wires.
Example: if you unplug 1 phase wire on a working board and try to accelerate, the motor will just stutter.
you could have a bad solder joint, or a broken wire.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-04-29T07:24:52.364Z Reads: 297

```
[quote="Nicolai, post:1, topic:22005"]
Any help is hugely appreciated! I hope I didn't short my motor...
[/quote]

I don't think you shorted your motor because a motor short will usually kill the DRV chip on the vesc and you would have a  DRV fault show up in realtime data.
```

---
## \#5 Posted by: Nicolai Posted at: 2017-05-04T20:24:04.368Z Reads: 262

```
@Namasaki @mmaner Thanks for your input guys, but I can't find any short in the phase wires connecting to the VESC or to the motor itself... nowhere can I find uncovered wires touching each other. Could it be an issue within the wires themselves?
```

---
## \#6 Posted by: Nicolai Posted at: 2017-05-04T20:27:16.447Z Reads: 251

```
@Namasaki if one phase wire is disconnected from a working board, is that board still able to brake? The brake on my motor still works fine.
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-04T20:31:23.540Z Reads: 240

```
Turn on active sampling then try accelerating just a bit on the throttle. See if the bottom left Fault Code area gets populated with an error.

Also change your max input voltage back to default (57v)
```

---
## \#8 Posted by: treenutter Posted at: 2017-05-04T20:32:15.708Z Reads: 228

```
@Nicolai could you post some pics of your setup, highlighting the wires, connectors, and points where things are soldered? Sometimes a fresh pair of eyes looking at it can help!
```

---
## \#9 Posted by: Nicolai Posted at: 2017-05-04T20:44:53.914Z Reads: 225

```
Hey Jinra, yeah I've tried that already (see the last screenshot I put up) but no fault code appears when I accelerate. Is it weird that the "current in" stays so low when I accelerate though?
```

---
## \#10 Posted by: Nicolai Posted at: 2017-05-04T20:45:46.370Z Reads: 224

```
Yeah, let me try to upload one!
```

---
## \#11 Posted by: Jinra Posted at: 2017-05-04T20:47:24.991Z Reads: 221

```
No load current should be low. However, there should be a large spike when starting up in line with the other peaks of the red and green lines. Perhaps something on the VESC blew that prevents it from drawing the needed current. Hi-res pics of the VESC would be helpful.

PS. If it turns out you need another VESC I have an extra and I'm right in your neighborhood :)
```

---
## \#12 Posted by: Nicolai Posted at: 2017-05-04T20:48:38.351Z Reads: 219

```
https://youtu.be/1w3lEfnN7wU
Here see if that video helps at all...

And @Jinra let me upload some right now. Thanks for all the help guys!
```

---
## \#13 Posted by: Nicolai Posted at: 2017-05-04T20:53:56.156Z Reads: 217

```
<img src="/uploads/db1493/original/3X/1/3/134d6292d397ab29d637b558adc453cd21966a2e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/d/3d16bcbed631266af37881b332b895490b90cabe.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/8/f/8f73428acac2a0cc667fac51914fb0aa22ea8ad6.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/0/105391847edfcb5a95058e4bd09d7fad6ab27446.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/f/9f17a7848b74bf142f010564658e766afb126594.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/7/2/7207b15fed4f0b258ada86cfa551d45b13311552.JPG" width="375" height="500">
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-04T21:26:27.587Z Reads: 193

```
Hm it might be a motor issue as well, but I don't see anything obvious from the vid/pics. One thing I did notice is that your motor is not on the mount securely. You can see it jumping around when you try to throttle, it must have loosened up, make sure you apply threadlocker.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-05-04T22:33:11.957Z Reads: 198

```
That stuttering looks like a poor connection on one of your phase wires.
I've seen it before on one of my builds. It turned out that one of the bullet connectors had a cold solder joint.

And when you say you "lost a bullet connector". How did that happen? Did it just fall off?
If so, then all your bullet connectors would be suspect for poor solder connections.

I would suggest that you remove the shrink wrap and have a close look at all your motor to Vesc bullet connections.
Twist the wire in the connector and see if you can break it loose.
Check continuity from the tip of the bullet connector to the wire before the solder joint.
Check for solder flux inside the female bullet connector or on the male bullet connector.
Also when you put then together, they should be very tight.
Last of all, open the motor and looks for loose or broken phase wire inside the motor.
That last guy that was having this problem found a loose phase wire inside his motor.
```

---
## \#16 Posted by: treenutter Posted at: 2017-05-04T23:05:35.779Z Reads: 181

```
I was just about to say what @Namasaki said! Look at the broken bullet connector, that is almost certainly a connection issue w a phase lead. How did you solder the lost bullet connector? 

If you soldered directly to the motor wire, did you remove the coating on the strands beforehand?

Btw great video I wish everyone w a question on the forum made a video like that, makes it so easy to help!
```

---
## \#17 Posted by: Nicolai Posted at: 2017-05-05T19:06:34.033Z Reads: 177

```
I really appreciate the help guys! I'm away from my build right now but when I get back I'll try everything you guys have suggested and I'll let you know if I still can't seem to figure it out. Thank you!!
```

---
## \#18 Posted by: Nicolai Posted at: 2017-05-09T20:25:22.069Z Reads: 175

```
Hey guys, so I'm still struggling to figure out my problem. Here are some modifications I've made to my setup. I'm pretty sure this method of connecting the phase wires together would mean a foolproof connection, but I could be totally wrong about this. Please let me know if I'm going about this the wrong way completely. 

https://www.youtube.com/watch?v=CZKNNfp3400

@Namasaki I've gotten rid of my bullet connectors on both the motor and the VESC sides, and just wrapped the phase wires together without any solder or flux to get in the way... This should prevent any "cold solder joints" right?
@Jinra thanks for your tips, I've reset my max input voltage to 57v, I'd love to hear what you have to say about my realtime data when you have the time. 
@treenutter I lost the bullet connector a while ago, I had been running my board without a female bullet connector joint with the loose phase wire (that would be holding the female end of the bullet connector) just soldered into the male connector, then wrapped all the ends in electrical tape to prevent shorting in the phase wires.

I seriously appreciate all the help you guys have been giving me. Do you have any further advice? Any idea what my problem might be? @EnertionSupport @onloop anything on your end?

Finally: keep in mind the setup I'd been riding had been working flawlessly for about eight months, until it suddenly wasn't. No crashes, no serious stress on the motor. I was just riding along then all of a sudden when I tried to accelerate I almost got bucked off the board because the motor started stuttering on me and now I've had this issue ever since. Also, I can still brake totally fine. It's just accelerating that's the issue.
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2017-05-09T20:31:31.678Z Reads: 162

```
Have you redone any motor detection ? Also, please use some connector 😉
```

---
## \#21 Posted by: Nicolai Posted at: 2017-05-09T20:33:23.594Z Reads: 164

```
Just ran the motor detection, detection failed. You mean solder the wrapped phase wires together?
```

---
## \#22 Posted by: Namasaki Posted at: 2017-05-09T20:37:03.675Z Reads: 162

```
A disconnected phase wire will cause stuttering. 
A shorted phase wire will blow your Vesc. 
Your risking a lot will all those bare phase wires so close together. 
Wrapping phase wires together is not necessarily a good connection. 
Anyway, the last guy we helped with this problem found a loose phase wire inside his motor.
I'm suspecting the same problem here.
```

---
## \#23 Posted by: Nicolai Posted at: 2017-05-09T20:42:47.554Z Reads: 156

```
Ok, let me disconnect the VESC from the motor and make sure they never short. Thanks for the warning. Just to be clear, you're suggesting I remove the motor from the board, take it apart and see if I can find a disconnected phase wire anywhere inside? It sounds like my problem is very similar to the other guy with the same issue.
```

---
## \#24 Posted by: Namasaki Posted at: 2017-05-09T20:44:53.807Z Reads: 149

```
Wait, before you take the motor apart, do you have a multimeter
```

---
## \#25 Posted by: Nicolai Posted at: 2017-05-09T20:45:36.810Z Reads: 149

```
No I don't unfortunately!
```

---
## \#26 Posted by: Namasaki Posted at: 2017-05-09T20:47:51.578Z Reads: 145

```
If you had a multimeter you could easily test for disconnected phase wires.
You should get one, it is an essential tool for this hobby
```

---
## \#27 Posted by: Nicolai Posted at: 2017-05-09T20:50:13.515Z Reads: 145

```
Damn, that would make my life a lot easier hahaha
```

---
## \#28 Posted by: Namasaki Posted at: 2017-05-09T20:51:24.469Z Reads: 146

```
All you would have to do is test for continuity between the 3 phase wires while disconnected  from the Vesc
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2017-05-09T21:00:03.126Z Reads: 145

```
I don't know if it's the picture, but it look like something is shorting your transistor (between the first and second pin)

<img src="/uploads/db1493/original/3X/1/2/129c0eae5e9bfd5f08c5d3e8c83de959c0dbe38e.JPG" width="375" height="500">
```

---
## \#30 Posted by: Nicolai Posted at: 2017-05-09T21:06:57.067Z Reads: 140

```
<img src="/uploads/db1493/original/3X/d/6/d63d11091c2c7575a03b3083c5343a3a408c6e75.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/5/d/5dc5f51dfb90e2dee2e68113927ae9c768e5008e.JPG" width="375" height="500">

Do these photos help at all?
```

---
## \#31 Posted by: JohnnyMeduse Posted at: 2017-05-09T21:10:22.014Z Reads: 139

```
Yeah look like a short, maybe you could use a small knife, and try to remove the small metal beads between pad 1 and 2

<img src="/uploads/db1493/original/3X/b/e/bea8040f0c340dfd69b263214010858802d893dc.JPG" width="142" height="142">
```

---
## \#32 Posted by: Nicolai Posted at: 2017-05-09T21:18:42.683Z Reads: 139

```
@JohnnyMeduse Just removed the little solder ball but I still get the same result...
```

---
## \#33 Posted by: JohnnyMeduse Posted at: 2017-05-09T21:19:44.828Z Reads: 138

```
Probably it as damage one of the mosfet 😧
```

---
## \#34 Posted by: Jinra Posted at: 2017-05-09T21:21:24.690Z Reads: 135

```
You should be able to test for broken phase wires without a multimeter. Just touch any of the two leads together to see if the motor 'brakes', and repeat with the other lead. If all combinations 'brake' then it should be all connected.
```

---
## \#35 Posted by: Nicolai Posted at: 2017-05-09T21:23:13.270Z Reads: 135

```
Is that with the battery connected? What kind of configuration does that require?
```

---
## \#36 Posted by: Jinra Posted at: 2017-05-09T21:23:51.713Z Reads: 135

```
Everything disconnected, the motor will be harder to turn when any two phase leads are touching (without power)
```

---
## \#37 Posted by: Namasaki Posted at: 2017-05-09T21:24:54.356Z Reads: 132

```
[quote="Jinra, post:34, topic:22005, full:true"]
You should be able to test for broken phase wires without a multimeter. Just touch any of the two leads together to see if the motor 'brakes', and repeat with the other lead. If all combinations 'brake' then it should be all connected.
[/quote]


Good idea @Jinra
Why didn't I think of that?
```

---
## \#38 Posted by: Nicolai Posted at: 2017-05-09T21:28:08.017Z Reads: 138

```
You're totally right, the motor does brake when two wires are touching. The problem is, every single combination of two wires touching together makes the motor brake! So I guess the problem is, that's not the problem? Kind of a good problem to have I guess, at least we know the motor is working!
```

---
## \#39 Posted by: Jinra Posted at: 2017-05-09T21:33:17.883Z Reads: 139

```
Perhaps this has something to do with it?

<img src="/uploads/db1493/original/3X/8/8/88c97a255ec619c65b3ce30bff54c997c0764b5b.png" width="547" height="499">
```

---
## \#40 Posted by: Nicolai Posted at: 2017-05-09T21:49:08.192Z Reads: 135

```
Nope, I set tat thread straight and still the same issue. I also soldered all the naked wired to the VESC and e-taped them up to prevent a short and still the motor stutters... It's looking more and more like a VESC issue.
```

---
## \#41 Posted by: Jinra Posted at: 2017-05-09T21:50:18.545Z Reads: 138

```
I'm guessing you dont have any spare motors/vescs to narrow the issue down?
```

---
## \#42 Posted by: Nicolai Posted at: 2017-05-09T21:53:23.543Z Reads: 133

```
Haha I have a couple other VESCs but they both have DRV faults
```

---
## \#43 Posted by: Jinra Posted at: 2017-05-09T21:54:07.859Z Reads: 134

```
Ah I remember, from your stint with FOC right?
```

---
## \#44 Posted by: Nicolai Posted at: 2017-05-09T21:55:02.713Z Reads: 134

```
Exactly. I haven't had the best of luck when it comes to VESCs... If you're free anytime next week @Jinra I'd seriously consider buying that spare VESC off of you! hahaha
```

---
## \#45 Posted by: Jinra Posted at: 2017-05-09T21:57:05.016Z Reads: 134

```
Unfortunately I just sold it, sorry! It could still be your motor, I know another guy who had issues with the R-spec doing something similar.
```

---
## \#46 Posted by: Nicolai Posted at: 2017-05-09T21:59:31.053Z Reads: 135

```
Ah darn! Looks like the only way to figure out my problem might be to get a new VESC huh?
```

---
## \#47 Posted by: Jinra Posted at: 2017-05-09T22:01:19.437Z Reads: 133

```
I have spare motors you could try hooking up to it if you could make it out to either South city or my work in SF (near AT&T park). If my motors work it might just be your r-spec.
```

---
## \#48 Posted by: Nicolai Posted at: 2017-05-09T22:08:15.968Z Reads: 132

```
Yeah I might take you up on that offer, that's really kind of you. Thank you! I'm currently just finishing up my finals at Cal, so once I'm done a quick Bart trip from Berkeley to AT&T park would be pretty easy!
```

---
## \#49 Posted by: Jinra Posted at: 2017-05-09T22:14:57.970Z Reads: 135

```
No problem, just shoot me a PM whenever and I'll bring my motors with me.
```

---
## \#50 Posted by: Nicolai Posted at: 2017-09-25T18:15:13.392Z Reads: 124

```
Hey everybody, I've decided to revive my board and I bit the bullet and ordered a new FOCbox from Enertion while my other VESC is getting fixed. The problem is, this FOCbox didn't change anything. Maybe I'm doing something wrong in the setup, but here's another video showing my issues I'm still having with motor stuttering. @Jinra @JohnnyMeduse @Namasaki @treenutter your vast wealth of knowledge and wisdom would be very, very much appreciated if you have the time!

https://www.youtube.com/watch?v=VB34su167gs
```

---
## \#51 Posted by: Jinra Posted at: 2017-09-25T18:22:18.339Z Reads: 119

```
Does the motor have resistance when you roll it by hand?
```

---
## \#52 Posted by: Nicolai Posted at: 2017-09-25T18:23:28.106Z Reads: 116

```
No, it rolls just like it did when the board was working a few months ago.
```

---
## \#53 Posted by: Jinra Posted at: 2017-09-25T18:24:06.785Z Reads: 115

```
Try doing a BLDC detection and seeing if it does the same thing.
```

---
## \#54 Posted by: Nicolai Posted at: 2017-09-25T18:25:49.621Z Reads: 114

```
Just did, also says bad detection result received. Could it be the parameters I've set in the BLDC tool?
```

---
## \#55 Posted by: Jinra Posted at: 2017-09-25T18:26:36.491Z Reads: 116

```
try upping some of the detection paramters such as min erpm, low duty, and current.
```

---
## \#56 Posted by: Nicolai Posted at: 2017-09-25T18:27:15.490Z Reads: 112

```
What should I use as a benchmark for those?
```

---
## \#57 Posted by: Jinra Posted at: 2017-09-25T18:29:18.794Z Reads: 112

```
try .1 low duty, 1200 erpm, and 6-10 amps on BLDC detection.
```

---
## \#58 Posted by: Nicolai Posted at: 2017-09-25T18:31:07.718Z Reads: 112

```
Darn, still the same result, the motor just spins and stutters faster.
```

---
## \#59 Posted by: Jinra Posted at: 2017-09-25T18:32:01.474Z Reads: 114

```
yea.. you probably need a new motor.
```

---
## \#60 Posted by: Jinra Posted at: 2017-09-25T18:32:40.051Z Reads: 112

```
My guess is one of the phase wires isn't connected properly. Try tapping two leads together and see if the rotor can provides resistance with **all** combinations.
```

---
## \#61 Posted by: Nicolai Posted at: 2017-09-25T18:33:24.176Z Reads: 117

```
Damn. I thought as much. I really liked that motor, and Enertion doesn't make one anymore... Any recommendations on alternatives that have similar power, speed and torque?
```

---
## \#62 Posted by: Jinra Posted at: 2017-09-25T18:34:27.234Z Reads: 114

```
Torqueboards has a nice sensored one of the same kv and size. @JLabs (buildkitboards) has a 208kv version as well which I like since it's sealed. @Kaly has a 230kv version of Jlabs motor I'm using.

Lastly I have an extra 5065 200kv if you need one locally.
```

---
## \#63 Posted by: Nicolai Posted at: 2017-09-25T18:34:45.709Z Reads: 115

```
Haha I literally just did that, and it does provide resistance for all combinations.
```

---
## \#64 Posted by: Jinra Posted at: 2017-09-25T18:35:42.314Z Reads: 109

```
Hm, weird, you could try taking it all apart and visually inspecting the wiring, stator, and magnets to see if anything's weird.
```

---
## \#65 Posted by: Nicolai Posted at: 2017-09-25T18:40:30.237Z Reads: 110

```
I might just have to do that at some point soon. And I may hit you up for that extra motor you have. Maybe I could come by SF someday this week and see if your motor works with my FOCbox/board setup? I'd like to try another motor on the board first before I get a new one just so I know that the motor I have doesn't work.
```

---
## \#66 Posted by: Jinra Posted at: 2017-09-25T18:42:00.065Z Reads: 110

```
Sure, I thought you lived by the Marina though
```

---
## \#67 Posted by: Nicolai Posted at: 2017-09-25T18:45:01.218Z Reads: 109

```
I'm a student at UC Berkeley :) I'm living in south berkeley right now.
```

---
## \#68 Posted by: Jinra Posted at: 2017-09-25T18:46:57.929Z Reads: 106

```
Cool, just PM me whenever you want to drop by.
```

---
## \#69 Posted by: Nicolai Posted at: 2017-09-25T18:47:50.015Z Reads: 109

```
Thank you so much for your help!!
```

---
## \#70 Posted by: JohnnyMeduse Posted at: 2017-09-25T18:49:16.452Z Reads: 111

```
Did you resolder new cable on the FocBox... if so make sure you didn't knock or short circuit any or the resistor near by.
```

---
## \#71 Posted by: Nicolai Posted at: 2017-09-27T22:44:17.107Z Reads: 105

```
How do I make sure that didn’t happen when I re-soldered the bullet connectors?
```

---
## \#72 Posted by: Namasaki Posted at: 2017-09-28T01:18:07.413Z Reads: 109

```
He meant if you soldered new phase wires to the vesc circuit board not new connectors to the wires.

If you soldered new connectors to the phase wires, then you might have got a cold solder joint. 
Especially if you used a low temp soldering pencil.

Example: I use either a 300 watt soldering gun or a butane torch. And put flux inside the connector and pre-tint the wire.
```

---
## \#73 Posted by: DanSkates Posted at: 2017-09-28T14:20:09.095Z Reads: 109

```
Hey @Nicolai - apologies if this has already been suggested as I've only had time to skim read the thread but I've watched your videos and the symptoms are identical to a problem I had with the R-SPEC motor too which I've now managed to correct - [see my thread for detailed info](https://www.electric-skateboard.builders/t/r-spec-given-up-the-ghost-fixed/28758)

The cause was a shorted phase wire where the shrink tubing had become exposed over time and 2 phase wires touched creating this jerky confused effect.  The solution was to remove the stator, solder the frayed wires (not sure if this was totally necessary as it was only a couple of loose threads) and shrink wrap up both exposed phase wires so they couldn't touch and hey presto - no more jerky only smooth goodness!

I would love it if this helps, but you may already have checked this?
```

---
## \#74 Posted by: Nicolai Posted at: 2017-09-28T16:28:46.195Z Reads: 103

```
!!! Dude this is huge, thanks so much!! I was gonna take apart my R-spec today to see what the matter was, your thread is hugely helpful. I'll let you guys know how it goes!
Thank you @DanSkates!
```

---
## \#75 Posted by: DanSkates Posted at: 2017-09-29T03:18:32.158Z Reads: 105

```
:grin: Hey my pleasure - I'm pretty sure that you'll find that to be the problem - I reckon the sleeving must just ride up over time eventually exposing the phase wires and if 2 touch that's when the motor gets confused.  

Give me a shout if you have any questions and I'll try to help.  Getting the stator off is fairly easy once you get the centre axle out but it does take a little bit of force :muscle:  One word of advice too once you lift the phase wires out - remember exactly how they lay before, it sounds stupid but I didn't do this and whilst they went back in fine and were perfectly secure 1 must have done an extra half lap as it was shorter than the rest!  Actually they were all slightly different lengths so I had to trim them all and refit the bullet connectors :smile:
```

---
## \#76 Posted by: whiteflight Posted at: 2017-09-29T18:44:10.803Z Reads: 105

```
Hi, I am having a similar issue of cogging, however it only cogs under mid to heavy throttle. It is still ride-able if I really baby it, yet it will cog if I try to accelerate at all. Braking is fine. do you think it could be the phase wires? I'd just like opinions on it before I take apart the motor.
```

---
## \#77 Posted by: Nicolai Posted at: 2017-10-02T20:50:31.218Z Reads: 105

```
I think I may have FINALLY found my problem!!!! There’s clearly a thin strip of phase wire that’s been broken through the motor use. @DanSkates there’s one final step that I need some guidance with, and that’s how to remove the last blue metal housing part of the motor so that I can re-solder and patch the broken wire. Can you walk me through how to do it? Thanks everyone so much for the help!<img src="/uploads/db1493/original/3X/c/a/cac4b3ee682099d5dd01445e1c859e52c1722b9a.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/b/ebe5185e4e98e05286a65707ecb882552ceb0329.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/2/a24ecc0982b882a4429be8854bf3b25720a1fd9e.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/6/46c5da219e7f19480ad482c3ac4e26f2e86533ab.jpeg" width="375" height="500">
```

---
## \#78 Posted by: Martinsp Posted at: 2017-10-02T20:55:02.529Z Reads: 103

```
It is glued so with enough force you should be able to take it off. Maybe try some gentle taps on the inside where the bearings are (not on the bearings themselves!) might get the motor apart. I have not done this before but I have seen people do it when rewinding motors. Be sure to protect the wires that are not broken right now so that you dont do more damage.
And do not use heat that would melt the enamel on the wire and short the motor completely.
```

---
## \#79 Posted by: Namasaki Posted at: 2017-10-02T21:57:30.283Z Reads: 97

```
Time for a new motor....
```

---
## \#80 Posted by: Martinsp Posted at: 2017-10-02T22:08:51.023Z Reads: 98

```
Well that might be an option :D If you are going to buy a new one I would try to fix this one if I were you, you can not make it worse
```

---
## \#81 Posted by: Namasaki Posted at: 2017-10-02T22:18:29.911Z Reads: 97

```
He could make it short out and break his Vesc though.
shorted phase wires are known to burn up DRV chips.
In my opinion, once the windings get broken it's time to get a new one.
```

---
## \#82 Posted by: Namasaki Posted at: 2017-10-02T22:23:04.554Z Reads: 98

```
Those wires are coated for insulation. I think soldering it back together would be very difficult. You would have to be able to clean the coating off of both ends of the broken wire and then over lap then to solder together. Then you would have to re-insulate the wire.
```

---
## \#83 Posted by: DanSkates Posted at: 2017-10-03T00:32:06.161Z Reads: 99

```
Hey man - glad you've diagnosed the fault.  

I’m afraid I couldn't get that bloody thing to come loose – it’s completely glued solid so I just worked around it.  My problem was the phase wires actually were touching which caused the issue – are yours touching too?  It looks like you’re shrink tube has ridden up exposing the wires to each other - that in itself I believe is enough to confuse motor detection.  If that’s the case what I did was pull the wires back through the opening so they’re accessible, re-shrink them (and resolder any loose strands, though if you have a lot this may be a bigger issue – they really don’t solder well) and then wrap them back as they were and pull back through the blue cover.  Make a mental note, or better take photos of how they went in as I put them back in differently and the wires came back through at different lengths! :smile: 

If this doesn’t work for you then try and take that cover off but I literally hammered it in a vice after freezing it for several hours and couldn’t get it to budge :grimacing:
```

---
## \#84 Posted by: Nicolai Posted at: 2017-10-03T04:06:06.183Z Reads: 97

```
OH MY GOD I GOT IT TO WORK! I realized I couldn't get a soldering iron through the cracks of the blue capsule housing so I decided to use a paper clip to insert a very tiny amount of glue onto the frayed copper wire and hold it in place so it wouldn't touch any other wires. Then I hooked everything back up, turned on my VESC and connected it to my computer and hey presto, FOC mode works!! 
My last few questions to you guys are with regards to my FOC settings (I've never used FOC before). Are there any irregularities you would fix, given that I'm riding a 10S4P battery, a 190kv 6374 R-spec, with an 83mm wheel setup? I weigh around 150 lbs and ride in a hilly place.
<img src="/uploads/db1493/original/3X/2/2/22629314956f654a716a75b2b4450a13782af4e0.png" width="690" height="353"><img src="/uploads/db1493/original/3X/b/4/b41dae5a6459b338d2691a8fd9124adfc24c3f60.png" width="690" height="361">
```

---
## \#85 Posted by: MrHappy Posted at: 2017-10-03T04:34:18.204Z Reads: 87

```
Dude, be careful. Depending on what type of glue you just used, you're looking at 1 - 50+ miles before your motor chunks and locks up again. Possibly destroying your vesc with it. I'm a college student as well, and I know spending money sucks ass, but don't kill yourself over $100, or have to spend $250 on a new motor and vesc in a month or so.
```

---
## \#86 Posted by: Namasaki Posted at: 2017-10-03T04:56:50.294Z Reads: 83

```
Listen to @MrHappy
You are risking too much to save a few bucks. 
Not only risking your Vesc but risking your life as well.
```

---
## \#87 Posted by: Nicolai Posted at: 2017-10-03T04:58:49.222Z Reads: 86

```
Agh, that's a scary concept... Hopefully the "gorilla" brand super glue holds up? I'm just so hesitant to get another motor when this one now works (though I still haven't ridden it) and a new motor this size is upwards of $80 to $100...
```

---
## \#88 Posted by: Namasaki Posted at: 2017-10-03T05:03:43.958Z Reads: 85

```
Super glue is a joke and no, it won't hold up. It will fail when you least expect it and then the wire will short and lock up the motor and send you flying on your face into the asphalt. 
You have been warned.
```

---
## \#89 Posted by: Nicolai Posted at: 2017-10-03T05:06:02.071Z Reads: 87

```
Yikes. Sounds like the best bet would be to either find a way to solder it down or to buy a new motor?
```

---
## \#90 Posted by: Namasaki Posted at: 2017-10-03T05:08:03.092Z Reads: 85

```
Your only real and safe option is a new motor
```

---
## \#91 Posted by: Nicolai Posted at: 2017-10-03T05:11:03.918Z Reads: 88

```
Rough... Thanks for the reality check. 

ok. So new motor time. Any suggestions? I'm looking at either the Ollin motor (http://www.ollinboardcompany.com/product/om-6085-200kv) or the Torqueboards one (collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv-3150w) or maybe something else?
```

---
## \#92 Posted by: Jinra Posted at: 2017-10-03T05:13:47.146Z Reads: 88

```
you have advantage of being able to pick one up locally (or i can ship) if you want the 200kv Ollin
```

---
## \#93 Posted by: Nicolai Posted at: 2017-10-03T05:15:22.220Z Reads: 91

```
I'll hop on that! I'll PM you about it. Thanks!!
```

---
## \#94 Posted by: Nicolai Posted at: 2017-10-03T14:18:34.784Z Reads: 91

```
Aside from that though, how do my FOC settings look? Any tips would be supremely appreciated.
```

---
## \#95 Posted by: Jebe Posted at: 2017-10-08T22:53:10.566Z Reads: 82

```
Have you opened the motor up at all ? I had similar problems and found a dry joint where the silicon wire attaches to the phase wires. It's a very small crimp. Also the phase wiring wasn't insulated adequately close to the windings and was shorting against the housing. Haven't had problems with those motors since.
Be careful pulling the motor apart - those magnets are strong and will pinch hard should you get your hands caught.
```

---
## \#96 Posted by: Jebe Posted at: 2017-10-08T23:16:48.865Z Reads: 82

```
And have you tried this ? Changing the erpm start and end settings in the PPM settings seems to have fixed my issue :)
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/1162?u=jebe
```

---
## \#97 Posted by: SlimSh8y Posted at: 2019-06-24T16:17:13.626Z Reads: 27

```
From watching your uploaded video I recognize this issue as one I too have faced at one point, but this is NOT a motor stuttering problem. This is a motor "jerking" problem due to the motor being loose on the motor mount. I thought I had completely fried one of my motors but it was simply jerking back and forth with torque because the motor mount screws are either stripped or just loose. Just with naked eye and no zoom you can still easily and clearly see the whole motor jerking back and forth, with a stutter you would only see the motor pulley appear to hesitate repeatedly when given enough power but the whole motor will NOT jerk back and forth. The ONLY way that can happen is if the motor is loose on the mount. You can also clearly see that at least your top motor mount screw is not tightened all the way down onto the mount. Make sure your motor is mounted solidly to the motor mounts and the issue will go away.
```

---
