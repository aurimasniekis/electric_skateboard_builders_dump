# Tb 6374 sounding bad!

### Replies: 45 Views: 794

## \#1 Posted by: Bjork3n Posted at: 2018-12-19T19:41:07.115Z Reads: 209

```
So im about to complete my build when i noticed one off the motors had a bad sound at mid rpm. Its louder than it appears in the video
https://www.youtube.com/watch?v=AB5vbLUJsiM

I tried riding the board and i noticed this sound on both braking and acceleration, it was not constant but it appeared on about the same rpm every time.
Tonight i opend up the motor but i cant see any thing wrong?
Ive checked the magnets and none is loose. 
![20181219_202848|666x500](upload://u4JlFowRJB2ImjhdsVCnpyEsYau.jpeg) ![20181219_202856|666x500](upload://h2xKAlrxkpQNFe91R4mV86jr3lD.jpeg) ![20181219_202554|375x500](upload://fhFd6HIbJe89HdAAdkXkBDl0Wpi.jpeg) ![20181219_202851|666x500](upload://5WsloI5WprsVVIeFyvmQ1whNn1V.jpeg) ![20181219_202945|374x500](upload://cUrOHEG5sT0XQooNYblBizoMbdv.jpeg) ![20181219_202949|374x500](upload://9hkkvMQHYdpkI6g5xYENGwqYPbA.jpeg) 
What more can i check? 

Motor was bought last year but only been used 3 rides.


Thanks!
```

---
## \#2 Posted by: legend27 Posted at: 2018-12-19T19:57:40.039Z Reads: 183

```
https://www.electric-skateboard.builders/t/motor-sound-rpm-interval-where-it-seems-the-turbo-is-kicking-in/11109

Didn't find any solution but you might be able to.
```

---
## \#3 Posted by: b264 Posted at: 2018-12-19T20:02:03.539Z Reads: 177

```
Does it make the same noise running sensorless?

Wondering if this is the sensored/sensorless transition RPM
```

---
## \#4 Posted by: Bjork3n Posted at: 2018-12-19T20:04:59.499Z Reads: 178

```
Don't know but at the moment both motors are using sensors (hybrid) bldc. But only one motor makes the sound
```

---
## \#5 Posted by: B-b-q-tom Posted at: 2018-12-19T20:06:41.845Z Reads: 177

```
What I would do -

Repeat test with belt disconnected to confirm the motor is causing the vibration/noise

Swap the cans and repeat test 

This will tell you if it is the motor or the can

If it is the can I would suspect bent shaft

If it is the motor I would suspect bearings (I think you have 3 per motor)
```

---
## \#6 Posted by: Bjork3n Posted at: 2018-12-19T20:09:41.521Z Reads: 166

```
I can confirm it makes the same sound with no belt. 

I rather not tear down the working motor if possible :slight_smile:
```

---
## \#7 Posted by: b264 Posted at: 2018-12-19T20:20:48.675Z Reads: 164

```
Also swap which ESC is connected to that motor and see if it changes which one makes the noise
```

---
## \#8 Posted by: b264 Posted at: 2018-12-19T20:21:53.619Z Reads: 158

```
It could be something as simple as one wire in the windings that's vibrating and brushing on a coat of silicone conformal coating would fix it.  But first you need to isolate where it's coming from.  ESC, stator, or rotor
```

---
## \#9 Posted by: mikenyc Posted at: 2018-12-19T20:42:39.255Z Reads: 148

```
Did you reach out to their support?
```

---
## \#10 Posted by: DerelictRobot Posted at: 2018-12-19T20:47:03.119Z Reads: 148

```
This sounds like the same exact issue I have with my 6380s, down to it only being on one motor and only apparent between certain RPMs. 

Contact TB, they are aware of this. I'm waiting on the new batch of 6380s to receive replacements.
```

---
## \#11 Posted by: dareno Posted at: 2018-12-20T03:31:34.802Z Reads: 126

```
That sounds to me like a bearing about to go bad on you.  There also looks to be metal dust on the shaft.  
Check the bearings.  This happened to me on a sk8 motor to the rear bearing.  It disintegrated and caused a short which blew the vesc.  Can be an expensive failure
```

---
## \#12 Posted by: chaka Posted at: 2018-12-20T04:15:21.969Z Reads: 121

```
In one of the photos you can see two of the mags have evidence of touching the stator. I have repaired a motor with this issue in the past by removing and bedding the magnets back in place to create the clearance.
```

---
## \#13 Posted by: DerelictRobot Posted at: 2018-12-20T04:24:01.482Z Reads: 120

```
This is spot on with what I found in my to rebuild efforts on mine until I replaced them with Maytechs. 

Retainer ring loose, misaligned can magnets, clearance issues with the C clip. I tore mine down thrice before I gave up on your and just gritted my teeth to the noise. 

I was told to keep riding them until replacements arrived. Ha
```

---
## \#14 Posted by: Bjork3n Posted at: 2018-12-20T04:57:20.931Z Reads: 112

```
In order to remove the magnets I need to remove the retaining ring? Should you just try to pry it off and then remove the marked magnets and re glue them? Thanks!
```

---
## \#15 Posted by: chaka Posted at: 2018-12-20T05:16:01.936Z Reads: 110

```
It isn't an easy undertaking. It is extremely easy to shatter the magnets trying to remove them. The only reason I did it was to recover the motor from a return I did for a customer.
```

---
## \#16 Posted by: DerelictRobot Posted at: 2018-12-20T05:33:14.253Z Reads: 107

```
Chaka is correct here. I've got a bunch of pictures of the tear downs I did, but it's not something I'd recommend if you're not already confident in working on this kind of thing. 

Honestly at most all I was able to do was fix them for a few days before a new and exciting sound popped up, would fix that, then it started over again on my other motor and eventually got tired of breaking down my entire sealed gear drive to service the motors repeatedly.

Have you contacted support? They are generally pretty responsive to this kind of thing.
```

---
## \#17 Posted by: PatRocks Posted at: 2018-12-20T05:48:03.115Z Reads: 100

```
Yep, I am with @chaka and @DerelictRobot it's defo magnets wiggling, soon they will become even more. Contact TB before you glue, would be good advice, but if you're like me, you're probably gonna try to fix it yourself lol. if so it may not last long before the noise returns, as mentioned above. good luck!
```

---
## \#18 Posted by: never4getf150forums Posted at: 2018-12-20T06:11:34.411Z Reads: 101

```
i've heard this on about 3 kalys in nyc, they ride on it consistently, some say it's bearings, some say it's nothing.. and i guess it could be nothing considering they've been riding it with that high pitched whine for months with no issues.

i just call it the turbo whistle :rofl:
```

---
## \#19 Posted by: DerelictRobot Posted at: 2018-12-20T06:24:07.811Z Reads: 101

```
https://youtu.be/80aT3wSDOFI

If you ask me, TB needs to jump on patenting this sweet ass  "card-in-bike-spokes" drive sound effect feature they added before Frank and Jason crash the party. 

I'm kidding guys, gosh.
```

---
## \#20 Posted by: Sebike Posted at: 2018-12-20T06:32:44.186Z Reads: 100

```
At one point those motors will give up and self destruct. Let's just hope it won't turn ugly for those Kaly-turbo-drive riders.. 

Happened to me after running with these loose magnets for a while. Motor locked up as if phase wires were sorted or something, but it was just a magnet that due to vibrations (and already being loose) snapped onto the stator mid ride.
Luckily I was going att a very low speed and close enough to home to carry the board the last few hundred meters..

Manually rotating the can made the magnet snap back into place, but when opening it up, at that point I could move almost all of the magnets.
```

---
## \#21 Posted by: Sebike Posted at: 2018-12-20T06:36:52.900Z Reads: 92

```
Sure, it could be bearings, it could be magnets, or it could be dirt, but nothing...? :thinking::sweat_smile:
```

---
## \#22 Posted by: never4getf150forums Posted at: 2018-12-20T06:47:46.871Z Reads: 90

```
you're right it has to be something, but most people who have this issue rarely solve it, it seems.. so they keep riding and it seems to work fine.
```

---
## \#23 Posted by: dareno Posted at: 2018-12-20T06:54:49.664Z Reads: 92

```
[quote="chaka, post:12, topic:78464"]
In one of the photos you can see two of the mags have evidence of touching the stator.
[/quote]

That would account for the dust.  @DerelictRobot agrees then I would be going down that road.

two guys who know their stuff.
```

---
## \#24 Posted by: Bjork3n Posted at: 2018-12-20T09:13:57.876Z Reads: 91

```
Well then I guess I need to order a new motor...
It wont be tb motor I can tell you that.
I haven't had great luck with their products to be honest. 

Thanks for the help guys!
```

---
## \#25 Posted by: Jalapeno Posted at: 2018-12-20T10:08:29.311Z Reads: 91

```
It should be bearings or an unbalanced rotor resonating.
The latter is very plausible since the sound increases at certain speeds.
```

---
## \#26 Posted by: Bjork3n Posted at: 2018-12-22T20:35:59.788Z Reads: 75

```
The sound goes away on full throttle, It only makes this noise at 50-70% throttle. 
I checked all the magnets and they are secure. Retaning ring is also secured. 
Bearings maybe?
```

---
## \#27 Posted by: Lumaci Posted at: 2018-12-22T20:46:17.205Z Reads: 72

```
Had the exact same issue on my TBs 6374 i got for my first build.

The bearings died not long after it started to sound like this.
```

---
## \#28 Posted by: Bjork3n Posted at: 2018-12-22T21:40:34.720Z Reads: 73

```
Hard task to replace them?
```

---
## \#29 Posted by: DerelictRobot Posted at: 2018-12-22T22:01:12.566Z Reads: 73

```
[quote="Bjork3n, post:26, topic:78464"]
I checked all the magnets and they are secure. Retaning ring is also secured.
Bearings maybe?
[/quote]

This is my best guess. I kinda lost track as I had cascading issues in both motors before I benched them. There are a few issues I've seen on my own as well as a few local friends with the same batch. 

Originally I was told to check the C-clips and the clearance with the bushings below them, but that was never an issue for me. I have seen this issue on a buddies and he fixed it by adding washers to gap things out. 

I personally have encountered three distinct issues: 

I had the magnetic retainer ring come loose on my right motor before anything else happened, about 50 miles in. Broke the motor down to repair and tediously realigned all of the magnets on the can, and used JB weld to reattach the retainer ring. This held up for another 20 miles before it came loose again, repeated the process with more slightly more liberal application of jb weld, and that has held it since. The same thing later happened to my left motor and a single break down of the same treatment fixed it. 

I got about 50 miles of quiet, smooth riding after fixing the right motor's retainer ring, before it started exhibiting the 'twangy ringing' noise described and shown above in this thread. Despite multiple attempts to locate the source of this issue, I couldn't, and got tired of breaking them down to troubleshoot. 

Dexter shared that this was a batch issue and that a new batch was in the works, and I could "just keep riding them" until replacements were available. Eventually the noise showed up on my left motor, and then the right one started sounding like what I know to almost certainly be bearing failure. I stopped riding them simply due to the cringe inducing noise awhile back, still waiting for replacements.
```

---
## \#30 Posted by: Lumaci Posted at: 2018-12-22T22:19:35.036Z Reads: 68

```
You need a bearing press, but its not that hard.

It was harder finding the correct ones since TB didnt even know what was used.
```

---
## \#31 Posted by: ARetardedPillow Posted at: 2018-12-22T22:47:03.999Z Reads: 71

```
Its the magnets, so far I've had 7 motors with this issue, 4 are torqueboards, 2 are dark matter, and one is an old Kaly motor. I've yet to find a motor that magnets won't come loose after 500 miles. 

The torqueboards motor's retainer ring also comes loose after around 1000 miles or so.

Edit: It is not a bearing issue, I've replaced bearings multiple times and it doesn't do anything.
```

---
## \#32 Posted by: DerelictRobot Posted at: 2018-12-22T23:31:45.359Z Reads: 71

```
[quote="ARetardedPillow, post:31, topic:78464"]
Its the magnets
[/quote]

[quote="ARetardedPillow, post:31, topic:78464"]
Edit: It is not a bearing issue
[/quote]

Let's try not to be so quick to jump to absolutes. :slight_smile: Your own sample size (nor my own) isn't enough to determine that one issue you're seeing is the core cause for everyone. The magnets are definitely a factor, but I've seen multiple different issues at play here first hand. My own magnets are still firmly in place. 

If you could expand upon the issues you found with the magnets beyond the retainer ring coming loose, that would be much appreciated.

In the same respect I'll break down the worst offender of my pair tonight and do some further post-mortem. I definitely recall seeing a good amount of wear on the stators, which could misalignment or vibration caused by a bad bearing. The sound is pretty awful even slowly hand turning it. 

For what it's worth, I'm about 700 miles into a pair of sealed 6374 170kv maytechs that are purring along smoothly so far.
```

---
## \#33 Posted by: ARetardedPillow Posted at: 2018-12-23T01:07:37.764Z Reads: 67

```
I'm jumping into absolutes because I've had this problem before many many times and and that's the issue, if you ride the motor like that for long enough you can see rubbing spots on the magnet(s). The magnets become looser and looser if you keep riding it as it and soon enough it'll become so loose it'll have a clicking noise(magnets rubbing on the stator core).
```

---
## \#34 Posted by: PatRocks Posted at: 2018-12-23T01:19:20.291Z Reads: 69

```
Man, the amount of time I've spent fixing my motors... it's silly. Here's what has worked for me with the twangy sound:

1. pull motor apart and clean as much as freaking possible. On the can, place the shaft in a drill. Place a dab of locktite 480 or 648 (648 is higher temp, but thicker and has a less-instant cure time. 480 is basically a rubberized super glue) in between each magnet and spin it with the drill immediately. It's best to do this in a bucket to catch the spray. Then wipe the excess with a paper towel. Do this process 1-3 magnets at a time. I also apply this to the ring, and use a punch to lightly hammer it snugly against each magnet. 

2. Inspect the stator for _**ANY**_ possible loose windings and hit them with either epoxy or a lacquer (I used urethane conformal coating recently, but made sure it wouldn't melt the wire lacquer). 

3. The stock bearings in most motors are metal-shielded. While I have everything apart, I replace them with rubber **sealed** bearings. These are bulletproof:
http://www.ebay.com/itm/130565237238

4. Have a beer then go ride!
```

---
## \#35 Posted by: DerelictRobot Posted at: 2018-12-23T01:28:49.419Z Reads: 62

```
And this totally makes sense to me, thanks for the input on this. I've emotionally already abandoned my 6380s awhile ago, but I'm curious enough that I'll break both down tonight and post some pictures. I put 600-700 miles on them before the right one unlocked it's third and final form.

Mind posting any pictures you have of tear downs as well?
```

---
## \#36 Posted by: ARetardedPillow Posted at: 2018-12-23T01:32:30.709Z Reads: 62

```
Yeah sure, I'll post photos later tonight. I have a whole box of just bad motors
```

---
## \#37 Posted by: DerelictRobot Posted at: 2018-12-23T01:33:20.398Z Reads: 64

```
[quote="PatRocks, post:34, topic:78464"]
pull motor apart and clean as much as freaking possible. On the can, place the shaft in a drill. Place a dab of locktite 480 or 648 (648 is higher temp, but thicker and has a less-instant cure time. 480 is basically a rubberized super glue) in between each magnet and spin it with the drill immediately. It’s best to do this in a bucket to catch the spray. Then wipe the excess with a paper towel. Do this process 1-3 magnets at a time. I also apply this to the ring, and use a punch to lightly hammer it snugly against each magnet.
[/quote]

Dude. This is an incredibly helpful explanation. Thanks for the insight. I have the feeling I'm going to end up trying to revive these 6380s for the 4th time now, haha.
```

---
## \#38 Posted by: PatRocks Posted at: 2018-12-23T01:40:14.462Z Reads: 62

```
The hardest part is cleaning between the magnets, and is CRITICAL. Otherwise the glue will be absorbed by the dirt and won't flow under the magnets. Though, if it's a relatively new motor, should be easy money
```

---
## \#39 Posted by: dareno Posted at: 2018-12-23T07:45:27.047Z Reads: 59

```
Lets ask the man himself.  @torqueboards  
Dexter can you shed some light here on this issue?
```

---
## \#40 Posted by: 701Superjet Posted at: 2018-12-23T23:53:00.656Z Reads: 54

```
My motors are also brand new and do the same thing. My retainer rings also fell out before I even rode my board. They are sending me new rings with longer teeth to hopefully stay in better. I was hoping that noise work go away with the new ring. I was hoping maybe the magnets we're not properly spaced causing the noise. Looks like I may be on the hunt for new motors and I haven't even rode these. Pretty disappointed in them.
```

---
## \#41 Posted by: torqueboards Posted at: 2018-12-24T06:29:10.507Z Reads: 51

```
Send us an email if you have this issue. We'll replace it.
```

---
## \#42 Posted by: 701Superjet Posted at: 2018-12-27T00:22:34.739Z Reads: 46

```
@torqueboards  Done! I look forward to resolving these issues.
```

---
## \#43 Posted by: Bjork3n Posted at: 2018-12-27T10:42:05.745Z Reads: 44

```
![20181227_114013|374x500](upload://3n5ZmJOvqQah80v1OnUuVxnoTjw.jpeg) 
Found the issue.. Was a broken magnet that was hard to spot.. 
Anyone have a some spares or even a replacement can? 😇
```

---
## \#44 Posted by: PatRocks Posted at: 2018-12-31T03:14:03.609Z Reads: 36

```
@DerelictRobot were you able to fix your motors?? I see them spinning on the insta!
```

---
## \#45 Posted by: DerelictRobot Posted at: 2018-12-31T03:26:41.759Z Reads: 35

```
Those are different motors on @Spiritrunner47's board, it's in the shop for a rebuild so I'm guinea pigging on it. 

I've not yet fixed my own. I've been promised replacements and already dropped in maytech 6374s in their place once the right one hit stage 4 terminal. I did actually open one up with the intention of posting pictures, but with the holidays I've been too scatter brained to make a proper post-mortem. I did see that my retaining ring has completely shattered on my right motor, though it's still holding on for dear life thanks to jbweld. There's further wear on the stator too, I'll post pictures here in a minute.
```

---
