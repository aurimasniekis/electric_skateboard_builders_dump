# The NTM Prop Drive 50-60 Rebuild Thread

### Replies: 68 Views: 6441

## \#1 Posted by: makepeace Posted at: 2016-04-10T12:05:35.207Z Reads: 184

```
Okay, so as per the edited title, this will be the thread of all threads for NTM Prop Drive 50-60 rebuilds. Watch the space. 

OP:

So after running my newly finished board (will post a build post soon!) for a few weeks, I've learned a lot. After the first run, I very absent mindedly left the batteries plugged in over night (didn't have a power switch by that point), and I ended up overdischarging my 8s LiPo pack to below 0.5 V per cell. I ended up recovering 7 of the 8 cells, but the other one would only build up to about 0.9 V, and then it would discharge straight back down to 0.0 V in about 2 minutes.

In any case, I'm running two NTM Prop Drive 50-60 270Kv motors, one on the front right and one on the rear left. I noticed from the start that the rear was running way hotter than the front one, but I didn't take much notice of it. Now running on only 7s, using an APS 120 A Twin ESC, I must have pulled too much current through the rear motor going up a hill, and I have very clearly burnt the windings in at least two places, verified with a multimeter. In any case, the motor still runs, albeit a bit less smoothly than the front motor and puts out about 20% less power and gets really hot.

The bearings on both motors are also absolutely stuffed.

With zero help from the well known Hobby supplier that I got these from, either in terms of replacement/money back for the one motor that was clearly a dud from the start, or in terms of any indication as to when they will be getting stock of the 50-60s again so that I can fork out for replacements, I'm forced to make another plan. Either I can get some more expensive work alikes, or get a set of bigger motors, which would necessitate a redesign of the mounts etc, or finally, rebuild the motors. 

I'm going to go for the option of rebuilding the motors. I plan on fitting some high quality bearings and rewinding the motors. DIY. #punk

I have a few questions, for anyone that has any experience with rewinding motors and eboard setupts.

1: Is it worth it to try and rewind these motors for a lower Kv and/or higher load capacity? Does anyone have any ideas as to what sort of winding spec I should go for to achieve this, off the top of the head? I could spend some time working it out, but I may just rewind the motors as is.

Which brings me to my second question: 

2: Does anybody know any details as regards the winding configuration on these motors? I'd like to know what I'm getting into before I pull the thing apart, just in case I mess something up and can't work it out myself.

I'll be looking for: termination style (wye/delta), winding pattern around the stator, number of turns, wire gauge, number of strands per wrap. That's probably about it.

Would be great if anyone has this info!

3: Would it be possible to use a thicker/thinner gauge of wire, with less/more strands per wrap? What are the pitfalls here? 

I would imagine to get the same performance out of the motor, I would need to keep the number of turns and the cross sectional area of copper of each turn the same. Is this correct? I would imagine that thicker wire would be harder to get a neat wind around the stator, due to the fact that there is more negative space around the wires for the same cross sectional area. Thicker wire would probably be more durable though. Does anyone have any advice here?

That's it so far! Need to get myself a heat gun so I can pull the stator.
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-04-10T17:31:26.599Z Reads: 149

```
Humm I've got a few "Paper Weights" at home...will follow this thread .... 

I was looking for some that could fix them for me...but no luck ...and I'm not abt to do it myself....

Hope you get your answers ‼️

All the best mate
```

---
## \#3 Posted by: Iceni Posted at: 2016-04-10T19:46:45.722Z Reads: 152

```
Seeing as i just finished a rewind of an R-spec motor, i'd say go for the rewind, it's really satisfying when it's done.

I'd suggest using a single thick wire for your sanity's sake, doing even two wires is a royal pain in the ass.

And i found a really neat way of removing the stator diving through countless rewinding threads.
Remove the bearings, put it in the freezer for and hour or so and then while holding the stator in your hand (use a glove) just whack the bearing tube with a hammer.
Make sure you find a spacer or similar item that is large enough to fit over the rim of the bearing tube, but not so big it'll hit the stator.
Will need to hit it pretty hard for it to loosen up.

No idea what number of turns or how thick the wires are in that motor.
So you might have to do what i did, count the number of turns as you unwind the old wires.
Then calculating the total cross sectional area with the number of strands and their respective thickness.

I used this calculator:
http://www.da-share.com/calculators/wire-cross-section-area/

And i used this for determining how to wind it:
http://www.bavaria-direct.co.za/scheme/calculator/

And this might be of use as well if you manage to figure out the original specs of the motors:
http://www.rcgroups.com/forums/showthread.php?t=2228201
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-04-10T23:03:53.947Z Reads: 132

```
I need like a Lego schematic or something because I'm so daft lol
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-04-11T18:08:20.611Z Reads: 123

```
I've never rewound a motor, but i have a couple that could benefit from it. I'm watching eagerly as well.
```

---
## \#6 Posted by: makepeace Posted at: 2016-04-11T18:09:06.203Z Reads: 127

```
Thanks for the encouragement and advice. I've never done this before, but I can get most things right so I'm sure it'll be okay.

I've just got some new bearings. A quality main bearing and a Chinese bell end bearing (it's pretty much exactly the same as the one that is stuffed). I've ordered some higher quality bearings that I'm getting on Thursday.

Thanks for the tip re. stator pulling @Iceni, and thanks for those other resources. 

Was wondering what the best way to do that was. I figured trying to shrink the bearing shaft was an idea, but there is a ton of terrible glue on the main bearing end that I was planning to heat up and loosen. Do you think that will be a problem with the freezing method or will it crack off nicely? I want to try and preserve the winding details so I can see what's going on in terms of termination etc.

I'm going to put another coating on the stator as well, just in case there are any bare metal areas.

Will also definitely go for one thick wire. Makes much more sense. I'd imagine the terminations are a mad las with multiple strands. I wonder why the Chinese don't do that?

Will definitely keep this thread updated, as I've found zero info regarding rewinding this motor and it'll be a valuable resource I bet.

As regards KV, does anyone have any ideas what effect the amount of copper has on this, directly? More copper = lower Kv? I'll Google anyway. Just wondering if anyone has any ideas off the top of their head.
```

---
## \#7 Posted by: Ulfberht Posted at: 2016-04-11T18:14:06.713Z Reads: 116

```
This thread is super cool. I've been thinking about rewinding motors too. Couldn't be much more difficult than rewinding guitar pickups. Just need to get some dead motors, now....
```

---
## \#8 Posted by: makepeace Posted at: 2016-04-11T18:18:37.318Z Reads: 117

```
@Ulfberht Exactly?! I've done that before. And wired my own inductors for a DIY studio ref power amp. What could be so hard?! 

These motors, apart from their super shart stock windings and bearings, are beasts for the price. 

Although, it must be said, extra work and supplies required would probably make them cost twice as much though. Meeep. Anyway, can't get them, can't afford the "big boys", can't afford to redesign. DIY. I'm punk like that.
```

---
## \#9 Posted by: Iceni Posted at: 2016-04-11T18:44:06.518Z Reads: 109

```
The stator on the r-spec I pulled apart was glued as well, but after a number of good hits on it it started to move.

The more copper you put in it the lower the resistance becomes, which leads to less wasted energy to heat.
It's the number of turns and termination you put in that determines the kv.
The reason why the commercially wound motors use thin wires is probably because they use machines to wind them and I doubt they'll handle the required thickness for single strand.
```

---
## \#10 Posted by: makepeace Posted at: 2016-04-11T19:20:34.861Z Reads: 101

```
That makes great sense.

So more turns is less or more Kv? For a constant termination style and winding pattern.

I'd actually dig to lower the KV a bit. Must needs torque, and I'd prefer to lower my top speed a bit. Geared for 50 km/h tops, which is too much, and I'd rather not modify my pulleys as what I have is a happy median for ground clearance.
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-04-11T19:23:18.151Z Reads: 105

```
Dang dudes...you make it seem easy...how the hell am I suppose to figure out how to put it back together...I need re-winding brushless motors for dummies book...better yet video ... Who is up to the task of taking it from A to Z for a slob like me
```

---
## \#12 Posted by: Iceni Posted at: 2016-04-12T19:17:16.394Z Reads: 97

```
More turns lower the Kv.
And if it's anything like the r-spec stock wind, it's terminated as delta, which from my reading seems to be standard for most commercially wound motors.
So you could use the same number of turns and terminate as star to lower the kv as well.
```

---
## \#13 Posted by: makepeace Posted at: 2016-04-13T05:46:50.206Z Reads: 92

```
Thanks for the info!

I've read that for the same wind, termination from delta to wye will divide my Kv by around 1.7. That's probably too low for me as it will end up at around 150Kv. Will probably opt for 1 or two more turns rather, if I can fit it them in. Only going to tear down the motors in a couple of weeks, as I'm under some time pressure at the moment.

Will keep this thread updated. Thanks for the help so far!
```

---
## \#14 Posted by: Hummie Posted at: 2016-04-18T08:19:45.817Z Reads: 94

```
Just do the LRK wind and terminate it delta. Easy. Just watch the starts and ends 

U can also raise the kv in other ways with the airgap or magnets.  One way to raise ur kv is cook ur magnets
```

---
## \#15 Posted by: Hummie Posted at: 2016-04-18T08:23:32.734Z Reads: 101

```
More wire means more resistance.  Ultimately u can have the same torque out of any kv motor, either a many turn low kv motor with lots of resistance and few amps, or a few turn motor with thinner wires with less resistance but u need to put in more amps to get the same torque.  Ultimately it balances out and u get the same heat to torque.  So u could run on 5 volts and a 500kv motor or 50 volts and a 50kv motor and get the same performance...except I think with the higher voltage u can get more power as u can push more amps, but maybe not necessarily true as it would be a very low resistance motor
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2016-04-18T08:40:40.411Z Reads: 103

```
Man .... it looks like a pain to do .... It's like knitting 

https://youtu.be/AimKJTIOqkU
```

---
## \#17 Posted by: Hummie Posted at: 2016-04-18T08:47:59.967Z Reads: 98

```
Stare at the diagram I posted for a bit and when it clicks you'll realize it's simple.  Just wrap a wire clockwise around a tooth, skip to the compete other side of the stator with the same wire and do it counter clockwise.  Repeat three times.  Just remember to watch the "starts" and "ends"
```

---
## \#18 Posted by: makepeace Posted at: 2016-05-11T20:04:10.360Z Reads: 101

```
Finally got a chance to pull my first motor apart.

This is what a deconstructed NTM Prop Deive 50-60 270 Kv looks like.
 
<img src="/uploads/db1493/original/2X/e/eb052225dc74079b845b42af89a12bba12b3da3a.jpeg" width="690" height="388">

I used @Iceni's tip to pull the stator from the base. Stuck it in the freezer overnight and then took a 1/4" 9mm socket and extension to the spindle bearing side with a hammer. Worked like a charm! Thanks for the advice @Iceni. 

I'm going to do a photo documented rebuild of the first motor, and then I'll make a 'for dummies' video of the second motor rebuild when I've learned what I need to in order to do the second motor fairly quickly.

More updates soon!
```

---
## \#19 Posted by: Ulfberht Posted at: 2016-05-11T20:17:17.757Z Reads: 98

```
Man!! I can't wait so see this build!! I'm seriously on the edge of my seat!! Are you going to build a winder or just wind it all by hand?
```

---
## \#20 Posted by: makepeace Posted at: 2016-05-11T20:30:48.227Z Reads: 101

```
@Ulfberht, I appreciate your excitement. I'm pretty amped too! I'm going to wind these ones by hand I think, as I'm going to opt for a single wire wrap, which should be fairly easy by hand. Also, rewinding two motors doesn't justify me building a winder for the moment.

Tearing into the phase wire connection, we can clearly see that this motor is delta terminated, and, fucked.

<img src="/uploads/db1493/original/2X/6/64d1ca83894727ae1811a2f0647cee6d1f5baba1.jpg" width="690" height="388">

If you look at the image above, you'll notice that the ends of the coils are connected, similar to the diagram below. You can also see how stuffed this motor's coils are. Chinese poo wire. :wink: 

<img src="/uploads/db1493/original/2X/3/3c382f5614824318bf28e828c379d9e75cff4704.gif" width="633" height="490">
I'm going to keep these motors delta terminated, as wye terminating will drop their Kv a bit too low, reducing it by a factor of 0.58 or so to about 160Kv, which is verging on too low to be suitable for an eboard. I will rather add another turn or two (when I figure out how many there are stock) to drop the Kv a bit. I'll aim for a Kv of 230 or lower.

For those interested, a wye termination looks like this:

<img src="/uploads/db1493/original/2X/3/36eaec692232bd83cffd92f3c997e0a4e0c0c190.gif" width="633" height="490">

More soon.
```

---
## \#21 Posted by: Hummie Posted at: 2016-05-12T04:52:06.581Z Reads: 98

```
Save yourself a lot of pain and maybe do the LRK wind with delta.  Winding every other tooth you can't end up too jammed.

That motor looks like a real bitch to get the wire off.  I've had a tacon160 I gave up trying to remove the wires and it's a paperweight forever.  If u can figure out how many strands are wound in parallel and you take off all of those parallel strands together it can be a difference between night and day
```

---
## \#22 Posted by: Iceni Posted at: 2016-05-12T05:01:56.531Z Reads: 98

```
Be careful if you're only winding every other tooth.
The windings barely cleared the bell when winding every tooth on the r-spec, wouldn't have managed it doing every other tooth.
```

---
## \#23 Posted by: makepeace Posted at: 2016-05-12T14:30:36.814Z Reads: 96

```
Busy pulling the windings off the stator. It's easier to bake the stator in an oven set to 200 degC, to soften the glue, which makes pulling the windings easier.

<img src="/uploads/db1493/original/2X/7/7c960eccad392360d0c893f602ccf39ef0ff1670.jpg" width="690" height="388">

That said, these windings are very brittle due to the heat damage, and I've struggled to keep track of the orientation of the windings of each coil due to breakages, and due to the tight wind, these motors are very hard to unwrap. It seems like the winding pattern is AabBCcaABbcC though, which is simple enough.

<img src="/uploads/db1493/original/2X/5/5b80e6c0534a4464df8ed57938d550677d78c961.jpg" width="690" height="388">

Some numbers describing the wind on these motors:

No. of strands: 22
Gauge of single strand: 0.23 mm
No. of turns per core: 9
Winding pattern: AabBCcaABbcC

I've been giving things some thought, and I have decided I'm going to opt for a Wye termination, because it just seems like a far better idea both in terms of space restrictions and current capacity. What I plan on doing is reducing the number of turns by about a third (for a higher Kv) and increasing the copper cross sectional area and then terminating in Wye. I should get a Kv close to 225.
```

---
## \#24 Posted by: longhairedboy Posted at: 2016-05-12T16:52:00.037Z Reads: 93

```
this thread is awesome.
```

---
## \#25 Posted by: makepeace Posted at: 2016-05-12T19:42:38.576Z Reads: 94

```
The stator is free from windings.
<img src="/uploads/db1493/original/2X/4/4c3921e5b28fd6e8d32bf09a4bcbef0733518c10.jpg" width="690" height="474">

To all those interested, it is a quite a serious mission with all of the glue involved, especially with the brittle burned coils.

Now to work out the wire gauge and length of wire I'll need for the new wind. I'm going to be going with the Wye wind, 6 turns per core to get the Kv I want.
```

---
## \#26 Posted by: longhairedboy Posted at: 2016-05-12T19:53:42.829Z Reads: 90

```
will it make any difference that the epoxy coating on the stator is all flaked off and cracking and peeling now?
```

---
## \#27 Posted by: Hummie Posted at: 2016-05-12T20:01:17.191Z Reads: 93

```
i had the green epoxy coating come off when I "unwound" as well.  I picked at it and took off a whole lamination.  Don't do that. I spend many many fruitless hours trying to recoat the stators edges.  I made a pie with three types of glue on top of each other: crazy glue, liquid electrical tape, Task9 polyurethane.  Don't do that. It's definately worth the time to get some high heat epoxy.  I read harbor freight has some.  Rcgroups has a a thread on doing it worth reading.  I also tried using super thin fiberglass which I read about there.  Don't do that either!  Otherwise, if u don't recoat all the edges well it will be a nightmare of shorts through the stator.  I hate my stator now and now hate rewinding.  I must have rewound it four times and shorted everytime.  Coat the edges with good lighting so u can really see and get them all.  My stator was harder as its already pressed on an aluminum shaft and hard to access as well but none-the-less coat all the edges well
```

---
## \#28 Posted by: psychotiller Posted at: 2016-05-12T20:09:24.253Z Reads: 91

```
@longhairedboy @Hummie  Did you try taping the outside all the way around and then the inside? Then you could just dip it into a cup of whatever you choose to coat it with. Then peel off the tape.
```

---
## \#29 Posted by: Karmannghiagirl Posted at: 2016-05-12T20:11:33.983Z Reads: 89

```
I was thinking just coat it in a high heat enamel like this: http://www.homedepot.com/p/Rust-Oleum-Automotive-12-oz-High-Heat-Enamel-Flat-Black-Spray-Paint-Case-of-6-248903/202628557
```

---
## \#30 Posted by: Ulfberht Posted at: 2016-05-12T20:19:18.046Z Reads: 90

```
Here's what I found on ES. 
https://endless-sphere.com/forums/viewtopic.php?f=30&t=38873
Sprayon red insulating varnish
https://www.zoro.com/sprayon-red-insulating-varnish-20-oz-s00601000/i/G1811056/?gclid=Cj0KEQjw09C5BRDy972s6q2y4egBEiQA5_guv82NXM4j5vRbPeZQYr4iaDhQqdt5NhSF6-SJBf8Hb4IaAqwc8P8HAQ&gclsrc=aw.ds
```

---
## \#31 Posted by: makepeace Posted at: 2016-05-12T20:37:13.481Z Reads: 86

```
@longhairedboy Yes! Forgot to mention that re-insulating the stator is actually the next step, which I'll do while I'm trying to source wire. 

I also forgot to mention that while I was unwrapping the coils, under the two offensive poles with the burned wires, there was bare metal, which is obviously where this whole thing started. I think that some of the NTM motors suffer from poor stator core insulation, and I think that's what caused this motor to fail.

I've found a couple of tips online, and I think I'm going to go with a high heat epoxy, and mask off the outside of the core as well as the inside.

I'm going to spend some time sanding off the epoxy on the top and the bottom of the core, but I won't worry too much about in between the teeth.
```

---
## \#32 Posted by: Michaelinvegas Posted at: 2016-05-12T22:15:35.374Z Reads: 85

```
Lol I bet not lol

20 stupid words
```

---
## \#33 Posted by: Hummie Posted at: 2016-05-13T17:12:50.774Z Reads: 87

```
I didn't do it that way thinking it'd be filling valuable space where there could be wire.  It's not much space but I try to over optimize 
:expressionless:
```

---
## \#34 Posted by: psychotiller Posted at: 2016-05-13T18:19:10.436Z Reads: 89

```
I suppose it depends on how viscous the insulator is...But I think if the excess could drip off it would work well that way. My guess is, people aren't in factories brushing that stuff on.
```

---
## \#35 Posted by: makepeace Posted at: 2016-05-13T18:22:50.224Z Reads: 89

```
Did some shopping for some vital rewinding supplies. Grade 3 enamelled magnet wire (more about this later), some Rustoleum high heat spray enamel, silicone lead wire, heat shrink and beer.

<img src="/uploads/db1493/original/2X/0/061bc48cd85fe4549343dd71df719129fb773ca8.jpg" width="690" height="388">

Black Label is a local South African favourite, and a quart is fondly referred to as 'Zamalek', named after the Egyptian Zamalek FC's walloping win over local favourite, the Kaizer Chiefs. The beer is said to be as strong as the Egyptian team that night. If you haven't tried it, you owe it to yourself to make a plan.

<img src="/uploads/db1493/original/2X/4/4c29d285e9f8488fa9dbcb0edd4579cf8c93c3ee.jpg" width="690" height="388">

The stator is masked up and ready for a hit of enamel, after a little sanding. I went for the spray on over dipping, as most of the coating is intact. If I was doing a fully stripped motor, I would go for a high heat epoxy dip.
```

---
## \#36 Posted by: Hummie Posted at: 2016-05-13T18:55:21.797Z Reads: 87

```
Looks like you'll be doing a better job than me. 

Strong beer I like. Here in San Francisco there's the Speakeasy brand. Everything they make is strong.  They have no story though. 

Are u going to waterproof it!? I want to and figure all that needs to be done is insulate the three connections from magnet wire to whatever it is you're connecting them to.  And maybe a spraying of some of that spray on enamel for the windings just to make sure and also keep them from moving.
```

---
## \#37 Posted by: makepeace Posted at: 2016-05-13T19:42:23.390Z Reads: 88

```
@Hummie  Yeah, I plan on waterproofing as much as I can. What I'm planning to do is once everything is wound and the phase wires soldered up is spraying the whole thing with 2 light coats of this this enamel paint and then dipping the whole thing in laminating resin, with the inside and outside masked up as above. Should hold up to much abuse.
```

---
## \#38 Posted by: makepeace Posted at: 2016-05-13T19:53:23.604Z Reads: 89

```
I've put on two thick coats of the enamel paint. It stacks up quite nicely, and I reckon I've got about 1.5mm of it on the ends and about 0.5mm on the insides of the teeth.

<img src="/uploads/db1493/original/2X/2/2628eb2749473c0a6f9b2775026f29528f4ffaef.jpg" width="690" height="388">

While that's drying, on to discussing the winding wire.

I opted for 1.12 mm conductor diameter grade 3 magnet wire. The outer diameter is approx 1.18 mm. I based this on a calculation of the cross sectional area of the stock wind, multiplied by a factor of 1.2 or so based on what I could comfortably fit on the teeth.

 The height of the conductor bearing part of the teeth was about 8 mm, and the smallest radial gap is about 2.8 mm.  This leaves me with a bit of wiggle room. 

I'm going for a single strand wrap. Grade 3 based on the fact that I want to never have to do this again. It's not all that fun, as @Hummie has mentioned.
```

---
## \#39 Posted by: Hummie Posted at: 2016-05-13T19:59:29.126Z Reads: 87

```
Doing three coatings of enamel or resin of some sort you say. did it ever get hot before because that sounds pretty insulating. What's wrong with 2 or 1?
```

---
## \#40 Posted by: Michaelinvegas Posted at: 2016-05-13T20:49:30.749Z Reads: 87

```
Omg this is a pain in the stator 

I'm never gonna try this lol
```

---
## \#41 Posted by: makepeace Posted at: 2016-05-13T20:53:31.527Z Reads: 76

```
Haha. It's not all that bad. $5 in wire and as much for the paint and a couple of hours work. Worth it considering I already have the motors which you can't seem to buy, and I enjoy fixing things. Would have preferred it if they didn't break in the first place though, if I'm honest.
```

---
## \#42 Posted by: Hummie Posted at: 2016-05-13T22:15:46.124Z Reads: 82

```
It's not fixing but upgrading and will keep cooler and all the phases can be made to have a more balanced inductance. If u do the windings really well, lining them up and keeping it even you'll get better inductance and can go for a fatter wire:  I've got a bunch of 90kvs in name, they all are 30 turns of the same thickness wire, but the variation in inductance on my LC meter is large.. do a great turn and you can get more inductance, need fewer turns, and can therfore use a fatter wire. 
To anyone who doesn't know.  And that's how u get a great motor.
```

---
## \#43 Posted by: makepeace Posted at: 2016-05-14T14:36:47.567Z Reads: 82

```
Okay so the Rustoleum was a failasaur. This morning when I checked it out (supposed to be fully cured in 24 hrs), it was still 'wet', ie, it just peeled off and was soft and doughy. Don't ever use that stuff for this application.

On to new things. I scraped off whatever I could of that, and got some Hammerite metal paint. I read the data sheet and it can do up to 150 degC peak and 80 degC continuous. I figured that's good enough, and it would be super easy to work with.

Out of the can it was a bit thick, so I thinned it down with about 1:25 of acetone, which according to the Internet works as a thinner.

Dipped the whole stator in the tin and left it in there for a few seconds. Pulled it out and set it to drip dry, rotating it every 10 mins or so. 

<img src="/uploads/db1493/original/2X/a/a2689ea5f94b3f1efb679b68055ecbbc811272c4.jpg" width="690" height="388">

I might give it another coat. Will see how I feel about it.

I like this stuff. I think what I'm going to do when the windings are on and the motor leads are connected is just dip that end again and be done with it. Should be waterproof enough. I also kind of like the look of enamelled copper through the open end of the cage.
```

---
## \#44 Posted by: makepeace Posted at: 2016-05-14T15:21:03.067Z Reads: 82

```
Twisted motor wires.

<img src="/uploads/db1493/original/2X/0/0cd7f3cf357b5b111cb447c954f80f960cca808d.jpg" width="690" height="388">

Because my shop only had 1.55 mm silicon, and also why the eff not. And I'm bored waiting for this paint to dry. 

They look kind of cool though. And will be a bit more flexy.
```

---
## \#45 Posted by: makepeace Posted at: 2016-05-14T15:51:04.464Z Reads: 81

```
So my winding scheme is going to look something like this:

<img src="/uploads/db1493/original/2X/0/096a9763807fc9325e3c2cc962e42f9ad5c96805.png" width="500" height="500">

Except it will have 6 winds per tooth instead of 5. It was generated by [this](http://www.bavaria-direct.co.za/scheme/calculator/) handy calculator. [bavaria-direct](http://bavaria-direct.co.za) is a great resource for rewinding BLDC motors.

I've debated going with 7 winds instead of 6, depending on whether I could fit them in, which I probably won't be able to. But that will drop my Kv to around 192 with the Wye wind, which is probably going to be a bit low for this motor, considering I'm probably going to be running it at 8s as is my current setup.
```

---
## \#46 Posted by: Ulfberht Posted at: 2016-05-14T19:58:45.474Z Reads: 79

```
[quote="makepeace, post:43, topic:2263"]
Okay so the Rustoleum was a failasaur. This morning when I checked it out (supposed to be fully cured in 24 hrs), it was still 'wet', ie, it just peeled off and was soft and doughy. Don't ever use that stuff for this application.
[/quote]
Try this stuff....
https://www.zoro.com/sprayon-red-insulating-varnish-20-oz-s00601000/i/G1811056/?gclid=Cj0KEQjw09C5BRDy972s6q2y4egBEiQA5_guv82NXM4j5vRbPeZQYr4iaDhQqdt5NhSF6-SJBf8Hb4IaAqwc8P8HAQ&gclsrc=aw.ds
```

---
## \#47 Posted by: makepeace Posted at: 2016-05-14T20:04:42.803Z Reads: 78

```
Looks good. Will try it next time. The Hammerite seems to be doing well. It's also quite fuss free to dip, and it seems to work quite well for this sort of thing.
```

---
## \#48 Posted by: makepeace Posted at: 2016-05-15T13:45:58.707Z Reads: 80

```
Stator is now coated.

<img src="/uploads/db1493/original/2X/5/5c34defa5e14c4a760f240e394138c6aee8c0bf4.jpg" width="690" height="446">

It's not ideal, but it will work. Learned some things for the next one.

<img src="/uploads/db1493/original/2X/2/2db4f252afd7e0989e318084ee31ee1082104d7a.jpg" width="690" height="472">

Wire trimmed to more or less the right length for one phase and ready to go. On to winding!
```

---
## \#49 Posted by: barajabali Posted at: 2016-05-15T13:49:56.705Z Reads: 77

```
Can you take pictures of each winding you do? So we can get a step by step 

Thanks buddy
```

---
## \#50 Posted by: makepeace Posted at: 2016-05-15T14:55:07.980Z Reads: 79

```
I'll take photos of each winding on the first tooth, and then of each tooth's winding from there on.
```

---
## \#51 Posted by: barajabali Posted at: 2016-05-15T14:56:51.704Z Reads: 78

```
Thanks! I'm a ghost follower of this thread lol as I'm sure a lot of others are too
```

---
## \#52 Posted by: makepeace Posted at: 2016-05-15T17:33:44.440Z Reads: 78

```
Wound 2 teeth and found a short to the stator. Back to the drawing board re. stator insulation. The Hammerite also cured too soft and rubbery. I think I'm going to dip in laminating epoxy thickened with a bit of enamel paint. That should do it.

This is one long hard mission. Hopefully I've learned enough to make the 2nd motor easy.

I'm going to get some slightly smaller wire too. 6 winds hardly fit and it's a struggle with this thick wire. My hands are destroyed already with blisters.
```

---
## \#53 Posted by: Iceni Posted at: 2016-05-15T18:46:06.636Z Reads: 79

```
I feel your pain man, I used 1.4mm (1.45mm with insulation) in my rewiring.
Tip is to use small pliers with some tape on the ends to get the wire to bend nicely along the teeth without having to pull too hard.
```

---
## \#54 Posted by: Hummie Posted at: 2016-05-15T21:29:42.457Z Reads: 79

```
Square wire maybe!?  They say it's better..get more copper in fill all the little voids.  

I've heard that there are eddy currents in the windings and I've heard not.  

Regardless, if I were to be able to have my dream winding..  It would be flat and thin like a sheet of metal. A heatsink already.   

Will  an inner winding create more inductance than an outer winding?
```

---
## \#55 Posted by: makepeace Posted at: 2016-05-16T06:44:48.449Z Reads: 72

```
Good plan @Iceni. I've been thinking that it's going to be easier with some tools.
```

---
## \#56 Posted by: Iceni Posted at: 2016-05-16T08:34:10.090Z Reads: 74

```
I used pliers, a small flat-head screwdriver and two small sheets of plastic 1.5mm and 2mm thick.
Just be careful with hard edges on the pliers and screwdriver, change the tape on them regularly, otherwise you risk nicking the insulation.
Doing it once or twice on the outside bends isn't a big deal as long as they don't connect with each other.
```

---
## \#57 Posted by: Karmannghiagirl Posted at: 2016-05-16T13:11:50.238Z Reads: 71

```
Maybe flat speaker wire would work?
```

---
## \#58 Posted by: Hummie Posted at: 2016-05-16T22:38:09.807Z Reads: 73

```
I looked it up but just see that it's wire to get to the speakers and not really wire in the speaker right?  It's really way on the fringe of performance and you'd want the stator gaps between the teeth to match up the wire exactly.  U can get more copper in that way but it's really going overboard. I'm interested in the flat wire more so because I think, maybe, maybe, if the center of each winding is where it's flux is concentrated, then u could have a winding that would go way beyond upwards and downwards...a flat widing that would transfer heat away.  But immpretty sure that the wire's end turns are useless for creating inductance. If somehow the windings can be cooled a little motor could do everything
```

---
## \#59 Posted by: makepeace Posted at: 2016-05-19T09:14:56.497Z Reads: 74

```
Unfortunately there isn't much in the way of flat or square wire in South Africa. I decided I'm going to go with the current wire and diameter that I've got, as I definitely should be able to fit it on if I'm careful. It's just a matter of working out a technique.

I coated the top and bottom of the stator with nail enamel sponsored  by the girlfriend. I figured I've already put too much gunk on this thing and dipping it laminating epoxy is going to add too much material and make winding an issue.

The tools I'm using:

<img src="/uploads/db1493/original/2X/1/1317914732de6387775a8c7fbea0712a39424e3c.jpg" width="690" height="388">

I put a pen lid in the top of the stator to use to wrap the wire around when I'm moving between poles.

<img src="/uploads/db1493/original/2X/1/1738884f8a57654d4531b16e1d907ccc535c2184.jpg" width="690" height="388">

First turn:

<img src="/uploads/db1493/original/2X/c/cc8a32f4b458083c20cc5915bfdb88acfad85281.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/3/35c776667818d469576a77df806b4c3fe191af04.jpg" width="281" height="500">

 Second turn:

<img src="/uploads/db1493/original/2X/1/16d490bb30e5270a6ec4988d482b8997ec63c255.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/1/1847b08f46c1f7c38e5b62156640d30efcd21e9d.jpg" width="281" height="500">

Third:

<img src="/uploads/db1493/original/2X/5/5048ac59fbb709b49bb285c318dd4704181cebe0.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/f/f7841446ce3d5442b32fc2c54e7fc895720086c7.jpg" width="281" height="500">

Fourth:

<img src="/uploads/db1493/original/2X/2/2ad15b98690740dc19e6f3f9b86f465ae656d599.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/c/c06ca7390e37554ebee0e37d9df6ffb439367a45.jpg" width="281" height="500">

5th:

<img src="/uploads/db1493/original/2X/5/5a3d1ad83a641caf7aa929120b63cfa5b4c8e954.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/5/52be9307ccc4859cff0a1ac9ab9c693f37d05388.jpg" width="281" height="500">

6th:

<img src="/uploads/db1493/original/2X/7/716b9300d3a4c7dac59b150095ae218a9bf56fe6.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/b/b37423223e365cf7dc8e3ab1450525ededbbddae.jpg" width="281" height="500">

I've heated up the wire and stator slightly in the oven to about 50degC to soften the wire a bit. The method I'm using to wind is to take the wire and wrap it round half a tooth, pulling it tight with the taped up pliers. Then I use the taped up knife and slot it between the opposite tooth and the wire to lever it against the wire all along it's length to make sure it's bent flush against the tooth it's being wound around. I then wrap it around the other end half of the tooth and repeat. When it gets to the 5th and 6th turns, I use a taped up screw driver to press radially on the coil on the end of the tooth (ie towards the centre hole of the stator) to compress the windings and bunch them up nicely so I can fit the last windings in.

Unfortunately like the clutch plate I am, I wound the 2nd tooth in the same direction as the first, so I have to start again, as reusing this bent wire isn't going to work. 

More soon.
```

---
## \#60 Posted by: Iceni Posted at: 2016-05-19T09:22:38.056Z Reads: 73

```
Looking good so far!

At least you didn't mess up on the last tooth like I did, had to rewind the other three, that was fun :p
```

---
## \#61 Posted by: makepeace Posted at: 2016-05-19T18:49:47.178Z Reads: 70

```
Haha, yeah that sounds like a las. Btw for anyone watching, this is really not easy. I never want to have to do this again. Quality motors from here on, and if they break and you can afford new ones, chuck them.

2nd winding:

<img src="/uploads/db1493/original/2X/7/7c6935c203461d6dcc9168ef597652d765fe5f27.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/f/fc117bdf5f6300f140ab8b605391cbe4bff25193.jpg" width="281" height="500">

I used some thread here to hold the end of the first winding in place, as the last turn kept on wanting to come off the tooth due to the lack of tension.

3rd wind:

<img src="/uploads/db1493/original/2X/a/ad2aa3c7e5db280d7c79f07e14b743687e7be213.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/4/406746ac655cc49c6ff924ecdbc6a61f11d67bc0.jpg" width="281" height="500">

4th wind:

<img src="/uploads/db1493/original/2X/9/97e014fcbe543aba3e9c42c148db210bacb1f87c.jpg" width="281" height="500">
<img src="/uploads/db1493/original/2X/a/a981f837b2f6626fc6bbc9a04b49a447bc4d2123.jpg" width="281" height="500">

Measured for continuity between the stator and the coil and there are no shorts! Also, the resistance of the coil is about 0.3 ohms, which the same as that of the length of wire I used, which means I have no shorted turns. Thank g.

First phase is done! Now it's time for beer.

I'm definitely going to dip this whole stator in laminating resin, as it's very hard to get things tight enough with this thick wire, especially where the turns are reversed in such a way that there is no tension on the previous coil.

Btw, the board in the background is my current board and is there for inspiration mostly, as it only has 1 working Prop Drive on it at the moment which isn't particularly useful. I'm going to rewind that one too at some point, and I'll make a video of that to summarise the process.
```

---
## \#62 Posted by: Ulfberht Posted at: 2016-05-19T21:35:19.129Z Reads: 65

```
Really awesome to watch you do this build! Looks like a pain in the ass to do! LOL
```

---
## \#63 Posted by: WeeChumlee Posted at: 2016-05-20T10:47:50.565Z Reads: 64

```
Great thread.
Really interested to hear what the end result is and if you feel an appreciable difference in performance.
```

---
## \#64 Posted by: Karmannghiagirl Posted at: 2016-06-07T03:19:06.139Z Reads: 60

```
Hows your rewind going? i just finished soldering on the leads for my first one. Hopefully going to be able to test it tomorrow after the epoxy dries.
```

---
## \#65 Posted by: makepeace Posted at: 2016-06-07T12:12:43.479Z Reads: 61

```
Been put on hold for a while. Going to get going again this weekend. Will hopefully be able to finish the first one and do the video of the second.

Exciting! Let us know how it goes. What did you rewind and how?
```

---
## \#66 Posted by: Karmannghiagirl Posted at: 2016-06-07T13:40:16.223Z Reads: 59

```
rewound the same motor that your doing :D

i did it slightly differently though (a little more hacky)

I'll post up a build log, but unfortunately i was fairly frustrated at some points so i don't have many pictures `:/`

But, i will say that it works!!!!!!
```

---
## \#67 Posted by: Stuntmanmike Posted at: 2016-06-21T00:02:56.006Z Reads: 52

```
Nice job man!
Can you tell me the bearing sizes that you used with this motor? I have 3 right now sitting on my desk in desperate need of bearings.
```

---
## \#68 Posted by: Ulfberht Posted at: 2016-06-27T20:04:14.894Z Reads: 45

```
@makepeace Any progress updates? I'm curious about how this all worked out. :v:
```

---
