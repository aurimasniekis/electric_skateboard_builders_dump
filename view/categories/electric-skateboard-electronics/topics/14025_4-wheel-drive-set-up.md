# 4 Wheel Drive Set up

### Replies: 35 Views: 4656

## \#1 Posted by: NewbieBoardBuilder Posted at: 2016-12-01T18:31:50.468Z Reads: 323

```
Does anyone have photos or a diagram of their 4 wheel drive electronics... It seems like the best type of setup, I don't get why everyone doesn't use it!
```

---
## \#2 Posted by: Stefan Posted at: 2016-12-01T18:34:10.365Z Reads: 323

```
Because it is freakin expensive?
```

---
## \#3 Posted by: NewbieBoardBuilder Posted at: 2016-12-01T18:35:40.633Z Reads: 317

```
I think I'll understand why once someone gives me a diagram or photo.
```

---
## \#4 Posted by: wolffoxx Posted at: 2016-12-01T18:42:11.840Z Reads: 314

```
[quote="Stefan, post:2, topic:14025, full:true"]
Because it is freakin expensive?
[/quote] Exactly. You need 4 motor controllers, and 4 motors (and 4 of a lot more things if you aren't doing hubs).  

@evoheyax was the first around here to get this done, as far as I know, and I've finished mine now.  I love it.  I'll do a build log soon, but I can send you a picture of my setup, in the meantime.  

I blew a DRV on a VESC so I'm technically a 3WD right now :sweat:.  The torque is great, the handling is nice, the redundancy of components has kept me from ever walking home.  When I can come up with some reliable Vesc$, I'll be a happy camper.
```

---
## \#5 Posted by: NewbieBoardBuilder Posted at: 2016-12-01T18:58:12.086Z Reads: 291

```
Do you have photos?
```

---
## \#6 Posted by: wolffoxx Posted at: 2016-12-01T19:08:38.821Z Reads: 289

```
I didn't mention this, before, but space is an issue :expressionless:<img src="/uploads/db1493/original/3X/6/e/6e4c69580325fbb6322beefa6537fea1efc29cb2.JPG" width="375" height="500">
```

---
## \#7 Posted by: NewbieBoardBuilder Posted at: 2016-12-01T19:43:34.102Z Reads: 275

```
Maybe a diagram would work better
```

---
## \#8 Posted by: NewbieBoardBuilder Posted at: 2016-12-01T19:44:43.114Z Reads: 272

```
WHO HAS A DIAGRAM?!?!?!?! I really need one before I buy my build...
```

---
## \#9 Posted by: jackw Posted at: 2016-12-01T19:47:54.100Z Reads: 267

```
Do a bit of reading on here and it shouldn't be too complicated to work it out! It's like dual duals :wink:
```

---
## \#10 Posted by: wolffoxx Posted at: 2016-12-01T20:44:03.702Z Reads: 267

```
[quote="jackw, post:9, topic:14025, full:true"]
Do a bit of reading on here and it shouldn't be too complicated to work it out! It's like dual duals
[/quote]

Yes, no diagrams; you've got some serious reading to do, but it's just battery to controller, to motor X 4.  You can link them up with CAN or Servo splitter.  Go searching for my old post where I almost sold all of my parts.  That will give you some idea of what you might be in for, in regards to parts.  There will be misc. cabling components and tools, and an enclosure to consider.

The real mysteries don't come until you get into VESC settings.  Word of advice: believe what you read in regards to quality of components.  Spend bigger, or spend again.
```

---
## \#11 Posted by: roonydagoony Posted at: 2016-12-01T20:46:40.639Z Reads: 256

```
introducing: The Qu4tro
https://www.indiegogo.com/projects/acton-blink-most-advanced-eboards-ever--2#/
```

---
## \#12 Posted by: NewbieBoardBuilder Posted at: 2016-12-02T00:56:17.411Z Reads: 245

```
[quote="wolffoxx, post:10, topic:14025"]
no diagrams
[/quote]

I just need a diagram, dude I have read a ton!
This is what I know: You need 4 VESCs for each motor, and there is a ton of necessary power… 
This would use the CANBUS basically just put them all in parallel with different address for each. You can power all 4 ESC from the same set of batteries.
```

---
## \#13 Posted by: johnny_261 Posted at: 2016-12-02T01:08:01.278Z Reads: 245

```
You might have a hard time getting a diagram... Anyone who has built a 4wd knows enough to not really need one.

So basically you need to learn enough to the point where you don't need one! Keep reading!
```

---
## \#14 Posted by: wiztecy Posted at: 2016-12-02T02:41:31.371Z Reads: 239

```
I like the idea of a 4wd hub system, however here are the disadvantages I see on the setup:

-increased drag
 You have 4 hub motors that now create drag so more rolling resistance which reduces efficiency.
-lower range
 due to increased drag and also the need to drive 3 more motors, your range will be dropped significantly.
-weight
 You now have 4 motors vs 2 or even one, so weight goes up.

@wolffoxx 4wd board looks great, saw the pre-build pics and it has fun fun fun written all over it.   Would love to see some finished pics as well as some specs, such as his battery capacity and range he's getting out of it.  Also curious about the acceleration and top speed.
```

---
## \#15 Posted by: NewbieBoardBuilder Posted at: 2016-12-02T03:52:07.511Z Reads: 234

```
<img src="/uploads/db1493/original/3X/d/f/df653b6ab81924fe9e280637ba5cc6854dfea8db.PNG" width="375" height="500">
Is this right...?
Where do you put the reciever...?
```

---
## \#16 Posted by: wolffoxx Posted at: 2016-12-02T04:08:37.785Z Reads: 226

```
@wiztecy Thanks, I'm going to make a log soon.  I'm still testing it.  I finished it right when it got cold, here, and then I blew a bargain VESC, so I'm on 3WD - maybe soon to be 2. :unamused: . I'm going to have to replace them with the Chaka vescs, I think.

As to the disadvantages that you listed, you're on point about the weight; that goes up whatever the weight of two hubs is, over what two 83mm skate wheels would have been.  The extra VESCS don't weigh enough to factor, and my battery is just the same 10s3P you might use on any mono or dual.  My particular board is a featherweight, from hi5ber.

Increased drag?  Sure, more drag than a basic longboard, but less drag than probably any satellite setup.  I kicked around on this thing while I waited for the parts, this summer.  No problems.  You forget it's electric until you try to kickstand it.

Range is an unknown.  I keep doing unscientific hill tests and joy rides and haven't looked at any telemetry so far.  I hope at 155lbs and for the casual commuting, i built it for, I can get close to 20 miles, but I could be disappointed, I guess.  I'll report back in my eventual build log
  
The torque is very very impressive, and of course having 4 braking motors is better than one or 2.  The board goes faster than I am comfortable with, and it goes there quickly.  That's in FOC with a 10s and conservative settings.  I built this as a commuter, and I'm not much of a scientist, so I may not ever yield much insight on the upper limits of 4WD hub sk8s.

Essentially, I'm a big proponent of the 4wd hub setup.  I think that's the way this is all going to go, as components hopefully get cheaper, lighter and more efficient.
```

---
## \#17 Posted by: wolffoxx Posted at: 2016-12-02T04:29:08.927Z Reads: 214

```
Ok, you met me half way with the art :sunglasses:  Mine is currently on a 4 way PPM split, from the receiver, so the picture I sent earlier isn't the exact same as this illustration. Also you may have trouble getting your 4 way battery to split that conveniently, unless you're building something custom. Basically you've got the layout, though!

<img src="/uploads/db1493/original/3X/3/7/37c2fe33520973934e027a1665584c9af56652ab.PNG" width="375" height="500">
```

---
## \#18 Posted by: NewbieBoardBuilder Posted at: 2016-12-02T04:39:20.316Z Reads: 200

```
But battery's don't have 2 output areas
I also couldn't find what a 4WD CANBUS harness is
```

---
## \#19 Posted by: wolffoxx Posted at: 2016-12-02T04:50:10.681Z Reads: 202

```
[quote="NewbieBoardBuilder, post:18, topic:14025, full:true"]
But battery's don't have 2 output areasI also couldn't find what a 4WD CANBUS harness is
[/quote]

I know they don't, typically, but that's what you drew, I thought. You need to buy or splice up a y cable and then hook it to two more y cables (or xt90 adapters, check diyboards).

Same with the canbus harness.  Either splice one yourself or request a custom from Ollin. I had one, but I mutilated it...
```

---
## \#20 Posted by: NewbieBoardBuilder Posted at: 2016-12-02T04:50:34.912Z Reads: 186

```
Can you send a photo of your wiring where it splits into the 4 parts... or a photo of your electronics spread out...
```

---
## \#21 Posted by: NewbieBoardBuilder Posted at: 2016-12-02T05:08:06.593Z Reads: 183

```
I was told: "so you can do a 4 Y Servo to 1 output which goes into your receiver.I wouldn't use canbus since all 3 slaves to 1 master might be too much data."
DIY BOARDS
```

---
## \#22 Posted by: NewbieBoardBuilder Posted at: 2016-12-02T05:13:45.733Z Reads: 199

```
<img src="/uploads/db1493/original/3X/e/4/e45648564d8b9713abd6e8fb7e3c0532165d6786.PNG" width="375" height="500"> is this correct?
```

---
## \#23 Posted by: Ackmaniac Posted at: 2016-12-02T11:09:43.264Z Reads: 184

```
The original source code of the VESC is even setup for supporting up to 10 slaves. So it will be absolutely fine. Connect the receiver to one VESC and the others via can.
```

---
## \#24 Posted by: DeathCookies Posted at: 2016-12-02T11:12:56.646Z Reads: 192

```
How do you connect them? Make a Y-Can ?
```

---
## \#25 Posted by: wolffoxx Posted at: 2016-12-02T21:40:02.895Z Reads: 182

```
[quote="DeathCookies, post:24, topic:14025, full:true"]
How do you connect them? Make a Y-Can ?
[/quote]

Double Y-Can.  Or servo split

<img src="/uploads/db1493/original/3X/7/3/73ffd335dda41715154f869f730daaea185ae2d5.jpg" width="240" height="176">
```

---
## \#26 Posted by: wolffoxx Posted at: 2016-12-02T21:45:00.154Z Reads: 178

```
[quote="NewbieBoardBuilder, post:21, topic:14025"]
I was told: "so you can do a 4 Y Servo to 1 output which goes into your receiver.I wouldn't use canbus since all 3 slaves to 1 master might be too much data."
[/quote]

Evoheyax is using 4wd on can, I'm using 4 way Servo split.  See picture, above.  

You go from your reciever to that splitter, then from that splitter to all 4 vescs.  You lose traction control, and one stop VESC setting adjustments, but IMO you gain some reliability since your splitter is probably less likely to fail than your master VESC, which would drop signal to all of your motors in the event of a fail.

However, I may eventually move to Canbus, because I'm interested in the emerging bluetooth telemetry apps, that require all of my VESCS to talk.
```

---
## \#27 Posted by: Hummie Posted at: 2016-12-02T22:24:10.428Z Reads: 162

```
How exactly is it more inefficient to do 4 hub motors?  Assuming the tire rubber is good as anything else out there the rolling resistance will be the same, the differences in bearings there's really none. 
If you're doing 2000 watts out of a battery and it's splitting it to 500 for each of four motors I don't see how that would be any less efficient than one motor the same size as the added four doing 2000.  I know evohyaks range sucks but he's heavy with hills and we haven't gotten around to comparing exactly. 
The rolling resistance meaning literally the rubber on the road could be a factor as your tires aren't the best yet. 80mm wheels. 
If anything it makes sense being more efficient than having less motors if the load gets big if only because you'd stay cooler from having more motor. But I know evohyaks is still really hot.  How do you do on heat and it'd be nice to hear how many watts it takes you to stay at 15mph
```

---
## \#28 Posted by: Jaraya92881 Posted at: 2016-12-02T22:54:52.396Z Reads: 150

```
Where are those VESC from? :)  Maytech?
```

---
## \#29 Posted by: NewbieBoardBuilder Posted at: 2016-12-03T15:11:11.905Z Reads: 152

```
[quote="wolffoxx, post:26, topic:14025"]
See picture, above.
[/quote]
Your electronics are way to mashed together under your board to understand it.
```

---
## \#30 Posted by: evoheyax Posted at: 2016-12-03T17:07:20.087Z Reads: 150

```
Check out my 4wd build ;) just search for 4wd rocket board, you can't miss it :slight_smile:

Lots of pictures, and you can see clearly how everything is connected.
```

---
## \#31 Posted by: wolffoxx Posted at: 2016-12-03T20:12:32.145Z Reads: 151

```
[quote="Hummie, post:27, topic:14025"]
How exactly is it more inefficient to do 4 hub motors?  Assuming the tire rubber is good as anything else out there the rolling resistance will be the same, the differences in bearings there's really none.
[/quote]


Yeah, I'm with you.  There is no efficiency loss, and there are probably actual gains.  Today, I rode the board front wheel drive, only.  This was the first time I noticed any heat off of the motors.  The truck was warm as I carried the board back to the house.  I never noticed anything like that in 4WD.

Front wheel drive was pretty fun, actually.  The board wasn't as keen to put me on my ass, and it might have felt more carvey, as a result.  However, I missed that big torque up hill and the 4WD brakes on the downs.

I'm going to put an order in to @chaka to get the rears back in commission.  And kudos @hummie for these sweet motors.  I hope you keep making them.
```

---
## \#32 Posted by: wolffoxx Posted at: 2016-12-03T20:34:40.118Z Reads: 151

```
[quote="NewbieBoardBuilder, post:29, topic:14025"]
Your electronics are way to mashed together under your board to understand it.
[/quote]

<img src="/uploads/db1493/original/3X/b/2/b29ec973c1fbc9b01156c45f7e2a657c0743d2dd.png" width="375" height="500">
```

---
## \#33 Posted by: kchxaz Posted at: 2019-01-22T06:25:46.006Z Reads: 54

```
Qu4tro. An absolutely stunning board, hands down. fast, solid, torque like you can't believe. The owners of Acton however do not give two shits about their customers. I have had three critical parts break on me and the last one was the ESC itself - caught out in a rainstorm. Asked, no begged them to sell me the part to fix it and they refuse. Flat out ignore me. Even offered them a whopping 50% more for the part. Seems they are comfortable remaining a small business as they certainly have no interest in supporting their product after sale unless there is big money in it for them. Would never buy anything from Acton ever again. Would never recommend Acton to anyone, ever again. Try Haloboard, they actually help their customers after the fact. I'll never know if my recommendation ever stopped a sale from them but even one sale lost would be a victory. So short sighted to not sell a $160 part but to require three times that to repair it themselves for a customer that will never pay that and certainly bitch about their service OR they could sell the part and have that customer talk them up over and over again. Not very smart business Acton practices
```

---
## \#34 Posted by: Winfly Posted at: 2019-01-22T07:11:51.458Z Reads: 50

```
Doesnt Action uses generic Chinese ESC? you can find them everywhere.
```

---
## \#35 Posted by: kchxaz Posted at: 2019-01-25T03:03:44.047Z Reads: 35

```
They do. And you can.

Problem is there are two smaller PCB board that are attached by jumper pins and they are so close together it is impossible to resolder them onto the new ESC without bridging them :frowning:
```

---
