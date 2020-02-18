# \[Raptor Dual\] One motor starts breaking. (short in windings) Solution found

### Replies: 52 Views: 4996

## \#1 Posted by: Skitzor Posted at: 2016-06-19T11:06:50.477Z Reads: 276

```
Hi everyone, my first topic here. Too bad it's one with bad news for myself.
I've uploaded a video and some pictures to give you an idea of my problem. The motor just started breaking/reversing so I had to disconnect the vesc bridge to be able to drive home on one motor.
(sorry about the video angle but I guess the point is still made)

https://youtu.be/7dTEA5BNJEk 

The video shows the resistance of the motor now.The motor detection being run and causing the battery to shut down.
<img src="/uploads/db1493/original/2X/d/df2d60eb928691b05363f7fccb0b8666f04c11a3.JPG" width="666" height="500">
The raptor dual on it's side with motor unmounted
<img src="/uploads/db1493/original/2X/4/4ff69ec8a646d324c21bf0cd8621696029ace362.JPG" width="666" height="500">
Shot of the copper windings (which seem okay to me)
<img src="/uploads/db1493/original/2X/f/f55a3059af70bb5c0749adb201dff3f4fe05178b.JPG" width="666" height="500">
Shot of the magnets

I've ordered 2 new motors already from Enertion, but if anyone knows a good EU adress with fast shipping it would be appreciated !
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-06-19T11:26:23.482Z Reads: 254

```
if you want additional motors, i think @elkick has stock(esk8.de).
```

---
## \#3 Posted by: Skitzor Posted at: 2016-06-19T11:31:17.937Z Reads: 245

```
Can't seem to find the exact same motor there (6355 190kv). But thanks for the advice !
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-06-19T11:33:15.836Z Reads: 242

```
Ok, but they have 6354 with 200kv, this is so close you need not to change anything.
```

---
## \#5 Posted by: Dedbny Posted at: 2016-06-19T11:35:42.400Z Reads: 235

```
Enertion should be able to express you a new motor. Go to the enrtion support email address first ans mark Urgent
```

---
## \#6 Posted by: Skitzor Posted at: 2016-06-19T11:37:44.428Z Reads: 232

```
I've ordered 2 of them already asking for asap shipment. But I guess it will take 1-2 weeks still. So if there's a European option that could be quicker I'll take it and keep the other ones as spares.
```

---
## \#7 Posted by: Skitzor Posted at: 2016-06-19T16:20:55.238Z Reads: 225

```
But guys, for clarity, I didn't do anything totally wrong with the board. It just got a little hit by a curb. At the moment I was hoping it was only the wheel to jump up. Can't find any damage on the motor or impact mark. That's why I made this post...

I'm actually thinking of mounting the motors behind the trucks as it would still leave a little kicktail left but protect the motors for future bumps...
```

---
## \#8 Posted by: HH1 Posted at: 2016-06-19T21:46:25.146Z Reads: 214

```
maybe it is a short in the motor? through the shock even if it was not direct to the motor?
How did you get the pulley of the motor?
did you heat the screws which hold the motor in place to soften the loctight?
```

---
## \#9 Posted by: Skitzor Posted at: 2016-06-20T08:16:05.845Z Reads: 207

```
I don't rule a short-circuit out of the question, but it would be strange... Where should I look for it?
At the point where the wires enter the motor or at the VESC-connection? 
But then again since the VESC is totally glued shut I think it would be impossible for something to have moved in there. 
Even without power, there's sound and resistance on the motor. (video at start) 
I've disassembled it and checked the bearings. The motor- bell and rotor are still straight and nothing is deformed. 
I didn't have to heat anything, just apply the right amount of torque in the beginning for the loctite to break and loosen the screw.
```

---
## \#10 Posted by: flatsp0t Posted at: 2016-06-20T08:21:55.304Z Reads: 205

```
Maybe it is a short in the phase wires where they go into the motor(they sometimes are not heatshrinked enough).
Or a short in the windings themselves.

http://www.electric-skateboard.builders/t/new-ollinboard-vesc-drv-magic-smoke/1885/10?u=flatsp0t
```

---
## \#11 Posted by: Skitzor Posted at: 2016-06-20T16:12:06.015Z Reads: 202

```

<img src="/uploads/db1493/original/2X/c/c09868d07088603db5880e9f3bbd25a4978425bc.jpeg" width="666" height="500"> 

Take a look at the windings, all 3 in contact with each other and the aluminum of the motor. If I compare this to my good one it's exactly the same.I can still do motor detection trough the BDLC tool though... It just shuts down my battery (thank god for safety circuits)
```

---
## \#12 Posted by: Skitzor Posted at: 2016-06-20T20:05:01.104Z Reads: 195

```
I'm not sure what I've done. Which makes this still a problem...

I played with the heatshrink and put the wires as nice as possible without disconnecting anything. I put the remote on my second vesc and tested again. It's working again !!!
Next thing I did is soldered the two vesc's together again ( master/ slave connection) alligned everything as it should. Both motors up and running again. Just did a small test-drive of a kilometer. Like nothing ever happened...

So what's the cause of this short exactly (as a hit on my wheels, obviously not motor, could trigger it...
```

---
## \#13 Posted by: Mr_Mahal Posted at: 2016-06-20T21:32:57.259Z Reads: 182

```
Seems like a VESC related problem..or at least I'm hoping it has nothing to do with the motor..
```

---
## \#14 Posted by: Dedbny Posted at: 2016-06-20T21:52:09.318Z Reads: 188

```
Could it be the connection of the reciever to that other vesc. You woukd think its the vesc. I know the connection between motor and vesc is an issue. The soldering may look right, but not. The da, biard just gets a pounding on ridges. i for ine dont ride on cross timber decking. I know you shouldnnt have to worry about it, but its hard to ride over anyway with the vibration. Glad yourve fixed it yourself. Well you cab make another board with the motors your getting. Did Enertion support help you at all?
```

---
## \#15 Posted by: Skitzor Posted at: 2016-06-21T07:47:06.124Z Reads: 192

```
I've only been concentrating on the motor, since the VESC part is so tightly glued.
Will try a definite solution and then I will do some serious testing, I will go to that same bump again and see if I can reproduce it. But as for now. Everything is pointing in the direction of the wires entering the motor, where some smaller stranded wires came loose, it's either that or the shaking rubbed the enamel off the copper.
```

---
## \#16 Posted by: Skitzor Posted at: 2016-06-27T09:39:55.765Z Reads: 194

```
So I found the problem, described in my post above. It's a combination of the motor wires being able to move freely at the motor entrance and the large amount of copper inside the motor underneath the coils. Some of the stranded wires were broken from the vibrations and rubbing against each other.

So the solution. (Has been tested thoroughly by myself, hence why this post comes in so late)

Rubber isolation spray I've used: 
<img src="/uploads/db1493/original/2X/c/c771aaf5d52283e7c97e5ca00d91d9263f203f39.JPG" width="375" height="500">

Without disconnecting anything (since the raptor is nicely glued tight), pushed back the wires inside the motor and coated them in rubber.
<img src="/uploads/db1493/original/2X/a/a09bbccf544086bd2fb221a253ec3ce9e7ae1463.JPG" width="375" height="500">

After the coating, pushed back the wires in original place:
<img src="/uploads/db1493/original/2X/d/d11493108e21f5f64f446f6349db4b54241fdfcd.JPG" width="375" height="500">

Pulled the triple heat-shrink back, and glued it tight in position with a hot glue gun.
<img src="/uploads/db1493/original/2X/3/3a4427c35836cb429fc1139057eaff553ef819f4.JPG" width="375" height="500">

Put the motor back together and on the raptor. Adding cable management to the wires so they are more stiff and can't move anymore. And replaced the Enertion paperclips with cable ties secured under the raisers.
<img src="/uploads/db1493/original/2X/0/07720e5b268607a2b8ca9d828a6b34679edf8878.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/f/fe8e9ff8a56e168dcc35af032153026edeeb6759.JPG" width="375" height="500">
```

---
## \#17 Posted by: Skitzor Posted at: 2016-07-08T17:20:28.501Z Reads: 170

```
So I swapped out the motor today. Got everything as smooth as possible again (motorwires as in the pictures above) So I decided to go for a test-run.

Seriously minding everything that makes the board vibrate (cobblestones, sidewalk pavements) and after an hour, the heat-shrink was loosely again outside the motor and the wheel was shorting again. I took pictures of the surface. I seriously can't be the only one with this problem

<img src="/uploads/db1493/original/2X/1/1e3a01690615380ae1b3c2542a9b751e4fb24973.jpeg" width="374" height="500">

<img src="/uploads/db1493/original/2X/9/9348b8ad2012f440e2e7a3cbaf7b93f54455adf4.jpeg" width="374" height="500">

I'll have to contact @EnertionSupport again...
```

---
## \#18 Posted by: flatsp0t Posted at: 2016-07-08T21:32:32.362Z Reads: 163

```
I had this Problem too, pushed it back in and used a cable tie.

It works for now, lets see how long^^
```

---
## \#19 Posted by: Skitzor Posted at: 2016-07-08T23:13:15.032Z Reads: 166

```
I get that, but what's so perfect about my right motor then? 
Could it be the vesc and coincidence? 
Geting kinda mad at the problem right now
```

---
## \#20 Posted by: fredx Posted at: 2016-07-08T23:43:46.494Z Reads: 172

```
I had the same problem with one motor in my Raptor Dual.  Enertion sent me a replacement motor quickly, at no charge.  But I'm impatient, so in the meantime I used JB Weld to separate and insulate the shorting phase wires.  Seemed to work; I haven't installed the replacement motor yet.  I haven't been skating a lot recently, though; not big mileage since my repair.

Anyway, yeah, you're not the only one to have this trouble...
```

---
## \#21 Posted by: flatsp0t Posted at: 2016-07-09T05:45:22.520Z Reads: 165

```
I think it is luck that you got one good.
Seems like there is a Monday batch out there.
```

---
## \#22 Posted by: Skitzor Posted at: 2016-07-10T11:54:25.231Z Reads: 163

```
Well, it got even better. The vesc from that motor doen't give any output anymore. I've heatshrinked the motor like it should. it's working on the other vesc. I can connect to it with the BLDC-tool, but motor detection fails and nothing is happening when I throttle. What should I check on the vesc ? Or what is probably broken on it ?
```

---
## \#23 Posted by: flatsp0t Posted at: 2016-07-10T13:06:26.124Z Reads: 161

```
Any burn marks on the DRV?
```

---
## \#24 Posted by: Skitzor Posted at: 2016-07-10T13:52:23.266Z Reads: 174

```
At first didn't see anything, now i doublechecked there is a small burn on the drv... Is that an expensive component and is it replacable without programming? 

Dammit !

<img src="/uploads/db1493/original/2X/2/2e85b3860f239052180cd136375aff14f33155ab.jpeg" width="666" height="500">
```

---
## \#25 Posted by: flatsp0t Posted at: 2016-07-10T14:37:22.716Z Reads: 189

```
If your soldering skills (hot air) allow it.
The chip is something around 8€

Just replace it and with a bit of luck it will work flawlessly again(if nothing else is fried).
```

---
## \#26 Posted by: massy Posted at: 2016-07-12T17:31:14.177Z Reads: 186

```
I have this problem too(board breaks randomly when riding) . All the wires are touching each other on the inside and moves freely when wiggling them around (doing so causes the motor to sometimes go bananas). One of the wires has gone slightly black (burned). Contacted enertion  support 1.5 weeks ago and no response yet. Ping @EnertionSupport.   <img src="/uploads/db1493/original/2X/c/c01f79752185c766a8ad00d12cc18d078462b899.JPG" width="281" height="500">

If it's not the remote it's the motor or some other shit. When this gets fixed the batteries will probably catch on fire and burn the whole thing to ashes.
```

---
## \#27 Posted by: Skitzor Posted at: 2016-07-12T19:07:12.027Z Reads: 179

```
I feel you, mine has spent more time on the bench tweaking and repairing then actually cruzin'. 
Still, it's one of the best on the market. These are first batches, you have to expect some child deseases, giving them a chance to learn from those mistakes. I've been helped everytime, sometimes it takes a couple days. I can't imagine what a chaos his garage must be at this point when he has to get all those shipments out. 

As for trying to help you (on the short run):
Do you have a little bit of electricity skills? (please don't be offended, I just don't know your background)
So you have the motor removed. Good, You have all the cir-clips removed as well, so now push it open, removing the bell and rotor from the stator. If your bullet connectors are still connected, give them a little twink and they should just pop out of the back of the VESCs that have been glued in. 
Get yourself the right size of heatshrink and push it as far as you can over the exposed copper wires inside so they are nicely isolated. This way they can't short anymore and this part of your problem is fixed. If you have a dual, do it for the other motor as well, since this will go the same road as this one.

Contact enertion support again, replying on the previous support mail with a kind reminder. They will get back to you as soon as they can, I promise. But given his wife just gave birth and all the backorders coming in from the VESC's that just arrived, give em some time to catch up... I'm in the same boat with my vesc DRV thats fried, but I'm sure I will get response before the end of the week.
```

---
## \#28 Posted by: c4Lvin Posted at: 2016-07-12T19:08:52.070Z Reads: 167

```
do you have another motor to try on for the braking issues? Mine was like that and it was my VESC. Kept riding *slowly*, braking randomly by itself (more like stuttering), and it completely has no response but there were still lights and NO RED error flashes either. Friend replaced some parts and fixed my VESC.
```

---
## \#29 Posted by: massy Posted at: 2016-07-12T19:15:13.624Z Reads: 163

```
Well the jiggling the wires around causes the same thing in the bench and the wire is burnt inside the motor. Also smells kinda funny when doing so. Pretty sure that's the problem. No other VESC available at this time unfortunately.
```

---
## \#30 Posted by: massy Posted at: 2016-07-12T19:17:10.892Z Reads: 162

```
Yeah, actually I was on my way to try and fix it today but lacked the tool required to get the small screws out of the motor. Probably should be possible but it's not like I wanna risk fixing it crappy myself vs. getting a good working one.
```

---
## \#31 Posted by: Adam0311 Posted at: 2016-07-12T19:52:47.874Z Reads: 156

```
It seems several of us are having the same or similar problems. I went 4 months without any issues, so I guess I've been lucky, but the brakes slamming on expectedly is not something I ever want a repeat of. 

I have not yet taken my motor apart, but it appears the issue was my slave VESC. I disconnected the slave VESC side motor and powered the board up and the slave VESC sparked and caught fire. I removed slave VESC and powered the board up and the master VESC and motor are working fine. 

Has anyone experienced this issue on the master VESC...or is it always the slave vesc/motor...and if so, why?
```

---
## \#32 Posted by: Skitzor Posted at: 2016-07-12T20:11:54.265Z Reads: 150

```
Btw be carefull when you try to undo those, with the small allen key and the threadlocker on there they get twisted over easily. Do it by hand if you can. I had to drill one over at each motor because of this, but I had spare bolts at home for those...
```

---
## \#33 Posted by: Skitzor Posted at: 2016-07-12T20:13:33.649Z Reads: 147

```
There have been lots of issues regarding the VESC and 63** motors, They are actually at the limit. If you want to read more, head over to the VESC 6.0 thread :

 http://www.electric-skateboard.builders/t/vedders-vesc-6-0/
```

---
## \#34 Posted by: massy Posted at: 2016-07-12T21:09:28.902Z Reads: 150

```
I'm running my personally built board (not raptor, 1 VESC only, [more info here](http://www.electric-skateboard.builders/t/untitled-slipstream-the-twin-caliber-trucks-single-enertion-r-spec-enertion-mount-10s-8000-mah-vesc/1095/4)) so no slave VESC here and as mentioned, short in motor is confirmed (although not 100% the braking was caused by this). As you can see in my previous picture the wires are slightly black where they touch the most, might as well just have one motor connector instead of 3 LOL.
```

---
## \#35 Posted by: Nate Posted at: 2016-07-13T02:57:57.591Z Reads: 147

```
Is this a recurring issue with the Raptor Dual? Getting my Raptor soon so I want to be pre-cautious.
```

---
## \#36 Posted by: Skitzor Posted at: 2016-07-13T07:23:41.651Z Reads: 144

```
The new motors I've got only leave like a cm of copper exposed when they go in. So they aknowledged that production issue. I would however advice you to stiffen the cables anyway so they can barely move.
Burning DRV chips on the VESC is also a common problem with those big motors.

Another hint for you guys, if you lost confidence in the board. Stop keeping the throttle always on, if you're not accellerating. Just let it coast, give some extra when your about to slow down. It will keep the motor from shorting and braking and a bit of extra range if you use it wisely
```

---
## \#37 Posted by: Nate Posted at: 2016-07-13T14:30:38.088Z Reads: 143

```
Hmm, sounds like I'll have to put some Velcro on the wires so that it'll stick to the board. I wonder if this is a known issue for Raptors.
```

---
## \#38 Posted by: Hummie Posted at: 2016-07-13T14:44:54.497Z Reads: 146

```
You could pot or do a conformal coating on the windings with high heat epoxy.  Most motors come with enough on there that wires aren't moving around and rubbing and shorting.  J and b weld is filled with metal and conductive and not a good choice.  Omega 100 high heat epoxy for 10$.
```

---
## \#39 Posted by: onloop Posted at: 2016-07-13T15:02:37.025Z Reads: 147

```
Hi guys.

Just a reminder.

Your raptors are all under warranty. Email support@enertionboards.com with photos and video of your problems.

There was a batch of about 80 motors made with excess copper inside. This problem has been resolved now.

If you have a motor with excess copper and you have not got over heating problems or any obvious issues yet I recommend securing the wires internally with epoxy.

Spare parts will be sent for free. We also will have ample stock of vesc to send for replacing failed vesc.

Replacing parts on raptor is fairly straight forward. If you get stuck we can help with instructions or find a repair agent nearby to assist..
```

---
## \#40 Posted by: massy Posted at: 2016-07-13T21:57:01.612Z Reads: 141

```
Not having a complete Raptor (got many parts though) but seem to have motor with the same issue. Opened a ticket July 4th on the website, no answer yet, should I still email?
```

---
## \#41 Posted by: Skitzor Posted at: 2016-07-14T06:52:35.413Z Reads: 130

```
Mail them a kind reminder, they have always replied me... He even came to the topic this time ;-)
```

---
## \#42 Posted by: guyguy Posted at: 2016-08-08T17:22:25.362Z Reads: 101

```
Do you know who got the motors that have this problem? Just want to check before taking any remedial steps.
```

---
## \#43 Posted by: Skitzor Posted at: 2016-08-08T17:24:32.807Z Reads: 102

```
I would say batch 1 and 2 from the raptors. You could check your stator for excessive copper wire exposed
```

---
## \#44 Posted by: guyguy Posted at: 2016-08-08T17:25:52.329Z Reads: 105

```
Thanks Skitzor. How do I tell if it's excessive or not?
```

---
## \#45 Posted by: Skitzor Posted at: 2016-08-08T17:27:24.351Z Reads: 104

```
<img src="/uploads/db1493/original/2X/c/c09868d07088603db5880e9f3bbd25a4978425bc.jpeg" width="666" height="500">

That's excessive
```

---
## \#46 Posted by: guyguy Posted at: 2016-08-08T17:28:56.729Z Reads: 101

```
and not excessive would mean there's no winding at the top?
```

---
## \#47 Posted by: c4Lvin Posted at: 2016-08-08T18:04:11.334Z Reads: 100

```
Till this day I don't know how a motor works. And how it "shorts" to tell you the truth. I've made longer shrink tubing on 2 of the 3 leads and seems to have fixed it because on the bench I can wiggle where the 3 wires meet by the aluminum can and it doesn't short anymore so I'm assuming it has fixed it. The funny thing is that if you touch any of the phase wires on its end, the motor will be hard to turn. But seeing those phase wires within the motor are already touching each other and don't seem to have that effect. Strange indeed.
```

---
## \#48 Posted by: Skitzor Posted at: 2016-08-08T18:15:39.986Z Reads: 102

```
@guyguy, exactly, they should be insulated all the way to where they enter the copper coils. (in other words, as far as you could push the shrink tubing till the end)

@c4Lvin The copper inside is treated with some enamel (which insulates the bare copper) but due to the vibrations they have to withstand, this rubs off and makes the copper short. Exactly the same way as you would short the bullet connectors a the end. If this happens at full speed when you hit a bump, bad things could (read: will) happen. Hope this explains it a little for you.
```

---
## \#49 Posted by: chaka Posted at: 2016-08-08T18:17:57.002Z Reads: 97

```
They are coated in enamel and it insulates, but you really don't want the separate phases resting on each other or rubbing on the housing. Ideally they would be fixed in place with epoxy at the factory, at least that is what you would want to see in a quality motor.
```

---
## \#50 Posted by: Skitzor Posted at: 2016-08-08T18:21:03.318Z Reads: 102

```
If you would ship to europe without import duties I'll gladly check ur motors out. I've already paid a total of 500 euros in import duties, just to get my raptor up to spec. Still having the issue with the batteries. So don't tell me I'm cheap for asking it :smiley:
```

---
## \#51 Posted by: c4Lvin Posted at: 2016-08-08T18:30:08.024Z Reads: 103

```
Thanks guys. I didn't do the 3rd one because it was the one that was the longest to wrap around.
```

---
## \#52 Posted by: guyguy Posted at: 2016-08-09T23:27:05.871Z Reads: 95

```
Anyone know what size circlips go on the motor shaft or have a link where I can buy more? I broke one taking it off the board when I was trying to take a peek @ the windings. 

Thanks!!
```

---
