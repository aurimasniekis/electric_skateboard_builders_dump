# One R-Spec motor hotter than the other \[solved\]

### Replies: 31 Views: 3232

## \#1 Posted by: Iceni Posted at: 2016-03-12T15:42:12.610Z Reads: 123

```
After an extended test run today I noticed one of my motor was hotter than the other.
And after a bit of testing I also noticed that the same motor doesn't spin as long after releasing the throttle from full and is noticeably harder to turn by hand.

So hence my question, what could be the problem and what can I do to fix it?
Could the bearings be the problem?

Edit: Quick video:
https://youtu.be/IwTsb77DkSA
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-12T16:36:12.949Z Reads: 121

```
First, rule out the VESC by switching the phase wires between motors. If the problem persists on the same side, the problem is mechanical, then somehow the motor must be encountering friction.
Check if your pulley isn't rubbing against the mount.
Take them both out of the mount and nd try to turn the spindle, if one has more friction than the other one, there may be a problem sith a bearing. I've never taken a motor apart so I can't help with that. Perhaps someone who has, can commment on how to check the bearings.
```

---
## \#3 Posted by: Iceni Posted at: 2016-03-12T16:46:08.118Z Reads: 116

```
I'm pretty sure it's not vesc related, since it's harder to turn by hand when the power is off.
And the pulleys were clear of the mount as well, but removed them anyway.

So without anything attached to the axles it's still the same resault.
Not sure i wanna pull it apart without a go-ahead from @onloop @EnertionSupport
```

---
## \#4 Posted by: EnertionSupport Posted at: 2016-03-12T19:26:01.392Z Reads: 107

```
I would first follow what @trbt said and switch the motors to the other VESC. 

You said there was still friction when the motor wasn't attached to anything:
-does it feel like intensified magnetic resistance (like if two of the phase wires were just barely touching)
-or does it feel like a physical resistance such as a blew out bearing? 

We haven't ever had a bearing go on any of our motors, so our first assumption is that this is either a VESC related issue or possible two phase wires touching. Even if it isn't a VESC issue, the live data tab of the BLDC tool should be able to give you a slight indication that the motor isn't performing 100%

The phase wire touching could also have occurred where the motor wires go into the R-SPEC, as one strand of copper could be touching a different phase wire creating some resistance. Although we haven't seen this issue before, it (like anything else) is still a possibility.
```

---
## \#5 Posted by: Iceni Posted at: 2016-03-12T20:00:44.786Z Reads: 106

```
Hmm, might be magnetic, since there's no scraping sound or anything when turning the motor by hand.
I'll do a closer inspection of the connections and try with the other vesc, then report back.
```

---
## \#6 Posted by: Blasto Posted at: 2016-03-12T20:13:20.123Z Reads: 107

```
Too much tension on one of the pulleys?
```

---
## \#7 Posted by: Iceni Posted at: 2016-03-12T20:58:37.875Z Reads: 108

```
This is the realtime plot of the problematic motor:
<img src="/uploads/db1493/original/2X/2/29878401e9a38e380d8e7ea7d1a7b2661aec1cf4.png" width="690" height="459">


And this is the normal one.
<img src="/uploads/db1493/original/2X/f/f6c027b30cebb1150613e19887f71fc431547dae.png" width="690" height="459">

Also tried switching them around between the vescs, the same motor slows down considerably faster still.
And it gets warm to the touch with the small amount testing i did while the normal motor is still cold.
And even when the motor is disconnected from everything it still is sluggish.

Starting to suspect there's something inside the motor that's not quite right.
I could open it up and get you some pictures of the innards if you want. I might even be able to spot the problem myself.
```

---
## \#8 Posted by: barajabali Posted at: 2016-03-12T21:09:19.644Z Reads: 107

```
Just gonna post stuff that I would check right off the back even if you've already tried it lol 

Make sure nuts aren't tightened too much on the wheel
Belts have a little slack in them
Remove belts and see if the resistance is from the motor itself or the wheel
Check connecting phase wires

Disconnect vesc and see if resistance is still around
Make sure the motor doesn't have physical damage to it

Unfortunately this game is pay to play as we all know lol sometimes we just need replacements 
I have had this issue before with an E sc but it wasn't a VESc basically it was just fried. When I dissconectrd the esc motor turned fine
```

---
## \#9 Posted by: Iceni Posted at: 2016-03-12T21:27:10.636Z Reads: 106

```
Already went through that stuff, eliminated the escs and drivetrain as a problem source.
One motor is harder to turn than the other while disconnected from everything.
I'm just hoping it's an easy fix, otherwise i'd propably have to send it in for repair.
```

---
## \#10 Posted by: Hummie Posted at: 2016-03-12T21:37:56.438Z Reads: 106

```
If the motor's shorted it will have more resistance either with power or not.   Sounds like a partial short.  

The resistance difference between phases is probably almost the same and so low a multimeter isn't accurate enough to reveal a short. An LC meter will tell you using the inductance tool. More accurate but u likely don't have one.  30$ on eBay. 

Man up and rewind it!!
<img src="/uploads/db1493/original/2X/1/135b8642926f1bec8a8b562ebfb9f09a1faeceae.jpeg" width="375" height="500">

Just make sure u don't damage the insulation on the stator on the unwind or you'll have an awful time with it. ...as I have. 
LRK wind is ideal for its ease to rewind on just every other tooth and better for longer torque motors as yours kind of is. 
Finally almost done both.  Doing it now
```

---
## \#11 Posted by: EnertionSupport Posted at: 2016-03-12T21:45:59.925Z Reads: 105

```
will you post some pics of the inside of the motor (without taking it apart)?

Just take it off the mount, and have one pic from the front, and one from the back. 

As @Hummie said it may be a partial short, where two parts of the phase wires are touching together when they aren't supposed to be. It could be as simple as pulling the two little strands away form each other, and then having it fixed!
```

---
## \#12 Posted by: Hummie Posted at: 2016-03-12T21:50:26.216Z Reads: 105

```
 it could also be shorting through the stator or the bearing tube.  If you have a multimeter see if you can get a circuit through each wire and the stator or the bearing tube. Radio shack has them for 20$. Harbor freight has them for free with a coupon!!

If it's a partial short it'll be in a winding on a tooth and more minor.   If it were shorting through the main phases I think you will get very hot quickly and the motor will really suck.  Yours sounds minor and a partial short.  I doubt visually it will show. 
See if u can isolate every wire from each other as best as possible and also from the bearing tube and try it then.   Maybe through vibration and rubbing insulation from wires has been removed.
```

---
## \#13 Posted by: Iceni Posted at: 2016-03-12T22:55:38.284Z Reads: 105

```
Can't really see much from the outside, except for one strand that's a bit off.
Tried to cover as many angles as possible.
Sorry about the dust.
<img src="/uploads/db1493/original/2X/5/57e833346dce29fbc95379091c2a43037dc7a38e.JPG" width="690" height="460">
<img src="/uploads/db1493/original/2X/7/72eec6661fb3dc79bfd7b3b29127961e55548cf8.JPG" width="690" height="460">
<img src="/uploads/db1493/original/2X/a/a73720195de7de3bd90ff06f2e46026e3532b4d5.JPG" width="690" height="459">
<img src="/uploads/db1493/original/2X/a/a8b326bb63d047318fba70b2563e913988c52e81.JPG" width="690" height="459">
<img src="/uploads/db1493/original/2X/6/6ef9109a1ff1f014da6c4bc6e13bc3b1064520c3.JPG" width="690" height="460">
[Uploading...]()
```

---
## \#14 Posted by: Iceni Posted at: 2016-03-12T23:10:27.785Z Reads: 101

```
upon closer inspection of that runaway strand, it seems to cross at least one other group of strands.
The right ring is where i originally found it, the left one is the same one, it continues in an odd way further in, but couldn't get a good pic of it.
<img src="/uploads/db1493/original/2X/9/93b0a8e2b009565ccf6bb8b5d1d7a699a1653448.JPG" width="690" height="459">
```

---
## \#15 Posted by: Iceni Posted at: 2016-03-13T07:47:54.304Z Reads: 101

```
Did some additional testing with a multimeter, seems that all three phase wires are connecting with the whatsitsname.
(The left one is the troublemaker btw)

https://youtu.be/-zYo_IacFPY
```

---
## \#16 Posted by: Iceni Posted at: 2016-03-14T16:40:08.324Z Reads: 96

```
Did some more poking around with the multimeter, some insulation has indeed come off some of the strands just after where the wires enter the motor.
Should i open it up and see if i can insulate them with something?
Because if that's all there is it shouldn't be too hard to fix, depending on how the wires are to work with.
```

---
## \#17 Posted by: EnertionSupport Posted at: 2016-03-14T18:52:52.954Z Reads: 95

```
Don't open the motor up just yet.

It is clear that there is a short, but the good news seems to be that it isn't terribly bad, and your VESC doesn't seem to have been damaged either. 

I'm starting to think it may be because of the extreme motor wire angles on your deck. Could at full turning it be pulling the wires at a less-than-ideal angle? Just turning back and forth with the bend occuring at the motor entry point could have wiggles a copper strand loose. 

Maybe change your R-SPEC's to face the other direction, and route the wires around next to your truck. This is what we do on our Raptors. You could also embed the wires into the deck or truck riser as @longhairedboy (embedded into the deck) or @cmatson (through the risers) have done.

All this said, I don't want you to open it up at this time, and risk damaging the motor further. You could send it back (just submit an RA on our website as the motor should not have died that quickly), but if you feel confident enough to fix the problem yourself we may be able to work something out.
```

---
## \#18 Posted by: Iceni Posted at: 2016-03-14T19:22:11.947Z Reads: 91

```
I thought the wires were fastened somehow in the can, but now that you mention it, when i turn the trucks i see an ever so slight wiggle in the wires inside. Guess that could be the cause of it.

I can rotate the motors and see how that works.

I'd rather not have to send it over to you, seeing as shipping and import duties will start to add up.

I've got fairly good skills with opening up and fixing stuff, and seeing the way it is assembled, it doesn't look all that advaced, and i'm pretty confident i can at least open it and close it without damage.
And once open i can judge if it's something i can fix or not.
Just popping the can shouldn't damage any of the windings if i'm careful.

But i leave the final say to you, if you want me to send it back, i'll do it, no problem.
I can do monodrive for a while if need be.
```

---
## \#19 Posted by: EnertionSupport Posted at: 2016-03-14T23:52:17.745Z Reads: 89

```
If you are happy to proceed with opening the motor please go for it, the motor is fairly simple and should be easy to open with the correct tools and a logical approach.

I have discussed this matter with the motor factory and they suggest simply gluing the wires back onto the bundle should resolve the issues.

epoxy or some other durable heat resistant glue would work.

if you get stuck please post photos on this forum showing how you did it. Actually, if you don't get stuck maybe posting the photos of your work might help others in the future.
```

---
## \#20 Posted by: Iceni Posted at: 2016-03-15T06:27:23.056Z Reads: 86

```
I'll get cracking later today, got some high heat silicone I could coat the wires with.
Will just have to see if I can get enough of the cables out to work with them.

If not I'll let you know.
```

---
## \#21 Posted by: Iceni Posted at: 2016-03-15T17:18:27.049Z Reads: 83

```
So after opening it up and seperating all the bundles as much as i could it still shorted between all three phases, so it seems the fault is deeper than i expected.
Found two spots where there had been some burn damage, propably where the insulation had scraped off.
Those i could pull out of the casing and seperate from any other metal parts.
A few strands had burned off completely, but managed to get them into the open air as well.
One phase wire is too short to do anything with, but couldn't see any damage to it, which is odd since that shorts to the other two as well.

So, yea, i kinda ran into a wall on this one.
Put it all back, since i don't want to do anything irreversible, though i'm fearing it's gonna need a major overhaul anyway.

So, what're my options now?
```

---
## \#22 Posted by: onloop Posted at: 2016-03-16T01:12:47.575Z Reads: 77

```
What ESC where you using? What was the MAX amps these were getting?
```

---
## \#23 Posted by: Iceni Posted at: 2016-03-16T05:24:23.096Z Reads: 77

```
Using the vesc.
Motor max is set at 60, batt max 15.
Motor min is -15 if I remember correctly.

But if what you said about the angles of the cables being the propable cause, then that's really on me.
```

---
## \#24 Posted by: onloop Posted at: 2016-03-16T06:08:53.273Z Reads: 76

```
Are there burn marks Or is it broken from stress?
```

---
## \#25 Posted by: Iceni Posted at: 2016-03-16T07:05:53.282Z Reads: 78

```
Burn marks.
There are some signs of abrasion against the body where the cables are wrapped around.
My guess is the insulation has been rubbed off some of the stands causing a short circuit, thus burning off the stands.
There were four or five loose stands inside, so possibly one or two have contacted with another phase wire.
One had been fused to the body.
```

---
## \#26 Posted by: Iceni Posted at: 2016-03-17T16:40:20.822Z Reads: 80

```
Well, after inspecting the other motor a bit more carefully it shows the same kind of wear, it just hasn't gone critical yet.
So it's pretty certain the way i mounted them was less than ideal.
Now I know and you guys know, don't mount the motors the way i did, they will break unless you fasten the wires inside the can somehow.

I'm thinking of ponying up for a new set and rewinding these for science, i'm not gonna trust them to perform as they are right now.

@onloop @EnertionSupport
```

---
## \#27 Posted by: onloop Posted at: 2016-03-17T21:40:43.294Z Reads: 76

```
[quote="Iceni, post:26, topic:1780"]
Now I know and you guys know, don't mount the motors the way i did,
[/quote]

For the record i have always warned people not to mount that way. I am sorry you had to find out the hard way.
```

---
## \#28 Posted by: Iceni Posted at: 2016-03-17T21:46:16.767Z Reads: 77

```
Must have missed it, oh well.
Thanks for helping out with the troubleshooting nonetheless, much appreciated.

Currently researching how to wind motors, will propably get a thread up about that soon-ish ;)
```

---
## \#29 Posted by: NIK Posted at: 2016-03-18T07:56:10.437Z Reads: 76

```
[quote="Iceni, post:26, topic:1780"]
Now I know and you guys know, don't mount the motors the way i did, they will break unless you fasten the wires inside the can somehow.
[/quote]

Just want to make sure I understand this right, by saying that means the phase wire must go backwards and to the VESC right? and not directly straight lines towards VESC.
```

---
## \#30 Posted by: onloop Posted at: 2016-03-18T08:19:31.610Z Reads: 76

```
this is how I do it. it means the that the wires are only bending a very small amount, also is prevents bending directly where they exit the motors.

<img src='/uploads/db1493/original/2X/2/2997e423f89bd5eba672bc6511416b33447aad7f.jpg'>
```

---
## \#31 Posted by: NIK Posted at: 2016-03-18T08:24:47.976Z Reads: 76

```
Yep, that's exactly what I did with mine. I noticed that when I do it the other way around which is the 'not good' way, it tends to push the wires directly into the can. Maybe I push to hard. haha. But yeah, the small bent will give good clearance for any movement. Cheers
```

---
