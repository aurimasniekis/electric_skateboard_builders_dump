# GT2B Spare Potentiometer

### Replies: 50 Views: 3230

## \#1 Posted by: chinzw Posted at: 2016-09-01T00:37:08.249Z Reads: 225

```
Hey guys, i know a ton of people here use the GT2B, so im wandering if anyone has a spare trigger pot from a dead remote that you'd be willing to part with.
Let me know!

Thanks!
```

---
## \#2 Posted by: susplus Posted at: 2016-09-01T08:14:55.997Z Reads: 203

```
If you already have a GT2B that has a dead trigger....you can swap it for the second one which should be the turning wheel used in RC cars..it is the same kind of potentiometer :slight_smile:
```

---
## \#3 Posted by: chinzw Posted at: 2016-09-01T15:54:51.368Z Reads: 183

```
[quote="susplus, post:2, topic:8739, full:true"]
If you already have a GT2B that has a dead trigger....you can swap it for the second one which should be the turning wheel used in RC cars..it is the same kind of potentiometer :slight_smile:
[/quote]

The shafts are different lengths, doesn't work
```

---
## \#4 Posted by: Montiey Posted at: 2017-02-16T02:38:30.738Z Reads: 150

```
I've tried that… Either bending the leads or soldering too hot ruined the connection between the pins and the carbon tracks on the original… The potentiometer from the steering assembly has a 90° rotation instead of 50°, which gives it the wrong offset. As you may note, the brake travel is shorter than the throttle travel, and the microcontroller is tuned to compensate for this- with the 50° pot, that is.

I'm currently looking for a replacement, too. I have no clue how do fix this and use a normal potentiometer, however you can get pretty close if you add variable resistors to the supply lines and tweak them.. But it's superficial, and barely works half the time.
```

---
## \#5 Posted by: chinzw Posted at: 2017-02-16T03:45:13.458Z Reads: 140

```
Im working on a drop in 3d printed replacement with hall sensors, not sure when it will be done tough.
```

---
## \#6 Posted by: Montiey Posted at: 2017-02-16T22:30:22.156Z Reads: 126

```
Interesting!

By drop in, I assume you mean it will output the same analog range as the potentiometer, and fit the GT2B / Modded case housing the same?
```

---
## \#7 Posted by: michaelcpg Posted at: 2017-02-17T01:50:23.158Z Reads: 118

```
The second pot in the GT2B works fine. Depending on whether you're using a modded enclosure, you might just need to dremel off some of the longer pot so that it fits.
```

---
## \#8 Posted by: Montiey Posted at: 2017-02-17T02:01:52.056Z Reads: 108

```
It works alright, but it doesn't have the right offset. You don't get the full travel on braking
```

---
## \#9 Posted by: michaelcpg Posted at: 2017-02-17T02:16:04.906Z Reads: 109

```
You have to play around with it in BLDC tool a bit but it's doable, pretty sure I'm getting the full range on mine. Using the other pot is obviously a little bit easier if you can source one though.
```

---
## \#10 Posted by: chinzw Posted at: 2017-02-17T03:49:04.940Z Reads: 100

```
You end up clipping the signal on one of the ends to get 0 to 1 range, which is far from ideal.
```

---
## \#11 Posted by: Montiey Posted at: 2017-02-18T16:22:31.904Z Reads: 98

```
That's exactly what i'm experiencing. 1500 is still the physical center and I get 2000 microseconds on the high end, but I can only get 1300 microseconds on the braking side.. Even adding varistors to either side of the pot to supplement the offset doesn't help… If only BLDC tool could do some mapping to allow for an off-center midpoint...
```

---
## \#12 Posted by: chinzw Posted at: 2017-02-19T18:33:22.700Z Reads: 94

```
You can try the Extended BLDC tool, that allows you to set min, max and mid points.  It's a good way to make it work with non symmetrical signals.
```

---
## \#13 Posted by: Montiey Posted at: 2017-02-19T22:09:41.050Z Reads: 90

```
That's my next resort- But for now, adding 5k on one side of the pot (I forget which side) and tweaking the internal potentiometers gives me a range between 2000 and 2400 microseconds. But most importantly, it works out that the center is perfectly at 2200 microseconds.
```

---
## \#14 Posted by: rwxr Posted at: 2017-02-26T08:22:29.034Z Reads: 83

```
How many have broken trigger pots?
I'm currently talking to the manufacturer of the pots and he can hook us up with spare pots. They are manufactured and shipped from China so shipping will be $35-50 with DHL express so I guess we have to do this as a group buy if we're doing it.
```

---
## \#15 Posted by: Titoxd10001 Posted at: 2017-02-26T19:04:56.344Z Reads: 81

```
I've broken like two of those trigger pots. When you say spare pots are you talking about the whole assembly like the trigger, pot, and wires with connector?
```

---
## \#16 Posted by: okp Posted at: 2017-02-26T19:17:48.279Z Reads: 81

```
awesome! I may have broken... like 10 !
```

---
## \#17 Posted by: rwxr Posted at: 2017-02-26T19:20:33.459Z Reads: 81

```
Nope, just the pot. I'm just calling it the trigger pot since there are two pots in the gt2b and the pot for the steering wheel is different.
```

---
## \#18 Posted by: chinzw Posted at: 2017-02-27T16:54:33.034Z Reads: 78

```
I broke 1, but id like some spares.
```

---
## \#19 Posted by: Titoxd10001 Posted at: 2017-02-27T19:17:33.774Z Reads: 77

```
Removing the actual trigger from the pot seems difficult have you done it before? Does new pot have wires at least because soldering is how I messed up the ones I had
```

---
## \#20 Posted by: Montiey Posted at: 2017-02-28T01:03:15.398Z Reads: 78

```
To get the pot out of the gimbal assembly it's simple. just unhook the spring with needle nose pliers, then slide off the trigger. The exposes a small bolt. Then the pot just slides off the plastic bits.

As for integrity of the pot, I've noticed two things: When desoldering the original PCB from it (to fit it into enclosures, etc.), it's tempting to bend the leads, but I think this sometimes breaks the connection between the riveted pins and the silver traces on the pot's PCB. Second, is heat sensitivity. Capacitors, for example, are extremely heat sensitive (electrolytic, especially) and you should be quick. I don't know how quick is 'quick', exactly, but I wouldn't feel comfortable soldering to the bare pins of the pot when it's riveted to the board like that for more than say… 1.5 seconds? Any decent Iron with a chisel tip should work.

Also, mind your temperatures. For a sensitive job like this, I would keep it as low as humanly possible (310-330 for lead-free), while still making the joint within the 1.5 second margin. You can either solder hot and quick, or cold and slow, but it's usually safer to end up soldering too cold and raising your temps, than to solder too hot and realize that it's burnt up already.
```

---
## \#21 Posted by: rwxr Posted at: 2017-02-28T06:47:05.466Z Reads: 64

```
The new pots should have ears which you can connect a female connector on. I'm still trying to work out how to get new pots without spending a buttload of money. Will keep you updated.
```

---
## \#22 Posted by: rwxr Posted at: 2017-03-01T16:34:06.879Z Reads: 63

```
I can get 50 new pots for $55 including shipping to me.

Anyone want some?
```

---
## \#23 Posted by: Titoxd10001 Posted at: 2017-03-01T17:42:46.425Z Reads: 62

```
I would be interested but I'm in the US so shipping might be to high
```

---
## \#24 Posted by: rwxr Posted at: 2017-03-01T19:49:34.877Z Reads: 61

```
How many? I can look up shipping to .us tomorrow
```

---
## \#25 Posted by: chinzw Posted at: 2017-03-01T21:22:58.201Z Reads: 60

```
im up for a few, if you're willing to ship to CA
```

---
## \#26 Posted by: Titoxd10001 Posted at: 2017-03-01T21:48:32.613Z Reads: 60

```
I'd be in for 3 pots. Do you have any pictures? I'm also in California
```

---
## \#27 Posted by: LukeL Posted at: 2017-03-01T21:54:58.647Z Reads: 59

```
I'd be up for 2 if you could ship to UK
```

---
## \#28 Posted by: michaelcpg Posted at: 2017-03-01T22:01:11.844Z Reads: 56

```
Any idea how much it'd be to ship 2 or 3 to NZ?
```

---
## \#29 Posted by: rwxr Posted at: 2017-03-02T07:33:04.949Z Reads: 56

```
As untracked letter up to 50g shipping is $4 to all EU and non-EU.
Tracked letter is $12.

Untracked letter should be just fine. I've ordered tons of stuff from china as untracked and I've lost just one package with some heat shrink.
```

---
## \#30 Posted by: rwxr Posted at: 2017-03-02T07:34:12.319Z Reads: 57

```
@Titoxd10001: I don't know if I can get pictures, but I've sent a picture with measurements to the distributor and he says it's the same pot.
```

---
## \#31 Posted by: Titoxd10001 Posted at: 2017-03-02T20:43:24.038Z Reads: 57

```
Okay just wanted to see how we are going to connect these because I don't want to solder on sensitive pcb pot
```

---
## \#32 Posted by: rwxr Posted at: 2017-03-03T05:17:53.967Z Reads: 56

```
Maybe we can use this instead of soldering?

<img src="/uploads/db1493/original/3X/2/b/2b9a1d0e379ac9dee86b73c01f17e4d73314df3b.jpg" width="500" height="500">
```

---
## \#33 Posted by: Titoxd10001 Posted at: 2017-03-04T01:15:37.699Z Reads: 53

```
It would be better if the pot PCB had wires so we can solder to that, but those connectors should work
```

---
## \#34 Posted by: rwxr Posted at: 2017-03-04T07:29:18.420Z Reads: 52

```
Agreed. So, should I order the pots? @Titoxd10001 @chinzw @unik  @michaelcpg @LukeL

You don't need to send me any money beforehand. He said around $55 for 50 pots including shipping, but I don't know if I need to pay customs fees aswell.
The total per pot should end up being something like $1.5-2+shipping from me to you.

If there's any interest, I'll see if I can find some connectors as well to include.
```

---
## \#35 Posted by: Titoxd10001 Posted at: 2017-03-04T07:59:24.502Z Reads: 47

```
I'm down to give it a try
```

---
## \#36 Posted by: michaelcpg Posted at: 2017-03-04T08:05:44.635Z Reads: 42

```
I'll take 2 or 3 at that price. Not that I'd need them but happy to take a few more if needed to fill the order :)
```

---
## \#37 Posted by: chinzw Posted at: 2017-03-04T08:44:16.158Z Reads: 40

```
ill take 5 for sure
```

---
## \#38 Posted by: LukeL Posted at: 2017-03-04T12:09:36.067Z Reads: 41

```
yeah i'd take 3 for that price
```

---
## \#39 Posted by: LukeL Posted at: 2017-03-04T12:29:15.685Z Reads: 46

```
I think if the pcbs have ears on it should be fine without the connectors, my first pot only broke when i cut off the ears, second one was fine at same temp solder just with ears left on. Did any of yours brake with ears on?

Also the connectors might be hard to fit inside the case, I found the fit pretty tight on my mad munkey mod.
```

---
## \#40 Posted by: rwxr Posted at: 2017-03-04T15:48:38.530Z Reads: 47

```
I'll investigate the room with connectors once i receive them.

Will order the pots tomorrow. Should take about 7 days with DHL from China to me.
Cheers!
```

---
## \#41 Posted by: rwxr Posted at: 2017-03-06T10:11:46.806Z Reads: 41

```
I've ordered them but haven't gotten any confirmation yet.
```

---
## \#42 Posted by: rwxr Posted at: 2017-03-09T07:42:13.098Z Reads: 44

```
Hi guys,
There is a hiccup in this. The distributor sent me a specification of the pot and it doesn't look like the GT2B pot.
I've asked for clarification a few days ago but still no answer.

<img src="/uploads/db1493/original/3X/4/1/411c1328dc915e4234498f75c7b40190c24a7a2f.png" width="667" height="500">
```

---
## \#43 Posted by: michaelcpg Posted at: 2017-03-09T07:57:58.783Z Reads: 44

```
Yea that's definitely different to the one in the GT2B. Bugger
```

---
## \#44 Posted by: rwxr Posted at: 2017-03-09T08:19:16.081Z Reads: 40

```
Yeah. Hopefully it's just a general description of a pot.
I won't order anything until I've heard from Joe again.
```

---
## \#45 Posted by: Montiey Posted at: 2017-06-28T22:22:48.743Z Reads: 37

```
@rwxr, any news on this? I kinda forgot about the thread. That is, until yesterday when some CA glue screwed up my potentiometer (Damn! I had it working so good, too…). I had to grind off bits of the steering pot to get it to work, so I'd assume you'd be able to grind off the shafts of these and make them work, too. I assume you haven't gone ahead and ordered these. In the meantime, I will attempt to use [THESE [amazon.com]](https://www.amazon.com/Gikfun-Knurled-Linear-Potentiometer-Arduino/dp/B0146DJWFU/ref=sr_1_4?ie=UTF8&qid=1498688380&sr=8-4&keywords=potentiometer) potentiometers. Again, by grinding down the shafts.

It would be great if we had a sustainable source for components. Group buys are fantastic, but if these work it'll be even better for the community, I think. Wish me luck!
```

---
## \#46 Posted by: chinzw Posted at: 2017-06-28T22:48:21.482Z Reads: 34

```
Good luck! But i wouldn't count on them being "soft" pots, most pots are quite stiff to turn and wont work for this application.
You need the soft preload ones, which are not that common and pretty hard to find.
```

---
## \#47 Posted by: Montiey Posted at: 2017-06-29T00:33:04.854Z Reads: 32

```
That's an interesting point. I'll have to see just how usable they really are. I'll keep you posted!
```

---
## \#48 Posted by: oldguy Posted at: 2017-06-29T01:51:35.528Z Reads: 30

```
 The trigger potentiometer in mine was DOA. I tried to swap them and failed as well. Tiny little wires and awkward spaces made clean disassembly an unsurmountable challenge.
```

---
## \#49 Posted by: rwxr Posted at: 2017-06-29T05:21:50.301Z Reads: 30

```
@Montiey: Sorry, the pot's Joe tried to sell didn't look exactly the same so I never ordered.
```

---
## \#50 Posted by: Montiey Posted at: 2017-06-30T22:37:16.462Z Reads: 31

```
I got the pots in today, and they were all gummy like you'd warned. 
…But they work! That being said, a stock spring might reveal the sluggishness, but I swapped mine for a stronger one.

I took a file to the pot and ground out a notch, measuring identically to the stock one.
<img src="/uploads/db1493/original/3X/6/d/6da136e75faa102967d473ba2ce8b75e29b178d3.JPG" width="333" height="250">

Here's where I think this experiment can be of use:
[These](https://www.amazon.com/Gikfun-Knurled-Linear-Potentiometer-Arduino/dp/B0146DJWFU/ref=sr_1_4?ie=UTF8&qid=1498688380&sr=8-4&keywords=potentiometer) potentiometers work as decent replacements to the stock GT2B potentiometers. With the only modification being filing the shaft, that is.

A simple metal file should do the trick- if you clamp the pot down, don't clamp the casing, PCB, or threaded shaft- only the knob itself. This helps reduce strain on the internal components. If you use a rotary tool, be cautious not to get the metal sizzling hot, as you may melt the plastic piece on the inside.

When soldering wires to the new pots (or when working on old ones), it's critical to only apply heat to the thin lead protruding from the board, and nothing else- even for a quick second. I think many people find that if you heat the rivet or any metal close to it, it ruins the connection. I know I do!
```

---
