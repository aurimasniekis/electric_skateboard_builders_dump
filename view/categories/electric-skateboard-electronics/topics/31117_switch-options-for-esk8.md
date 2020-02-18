# Switch Options for esk8

### Replies: 37 Views: 2238

## \#1 Posted by: RaceFlight Posted at: 2017-08-20T19:04:00.314Z Reads: 220

```
So I bought two switch from DIY Electric Skateboard, and both were stuck powered when I tried to use them.  They wouldn't turn off.  What are my options for switches?   Does anyone have any they recommend, its the only thing holding me back on my builds.
```

---
## \#2 Posted by: Deckoz Posted at: 2017-08-20T19:07:43.425Z Reads: 221

```
interesting name.... but my buddy and I ordered two as well and they both once powered on failed open(on) and couldn't be turned off.. I just went the route of xt90 anti spark loop key.
```

---
## \#3 Posted by: RaceFlight Posted at: 2017-08-20T19:15:41.963Z Reads: 220

```
Well at least I am not the only one.  Think I may go the old fashion switch route, till I can design something better.  I was hoping there was something else I could buy that would do the job.   May go the XT90 route too, doesn't look like a bad way to go either.
```

---
## \#4 Posted by: Deckoz Posted at: 2017-08-20T19:19:32.758Z Reads: 211

```
you could use a double switch system too... turn first switch on and it has an inline resistor to preload the system, then use a thicker guage on 2nd switch and turn that on for current to flow through. or  a relay system....there's other ways besides FETs..
```

---
## \#5 Posted by: Tuomalar Posted at: 2017-08-20T19:33:42.348Z Reads: 197

```
Xt90s is way to go. It takes less space, much more trustworth and less parts to broke.
```

---
## \#6 Posted by: Cobber Posted at: 2017-08-20T19:35:19.482Z Reads: 191

```
loop key all the way
```

---
## \#7 Posted by: Deckoz Posted at: 2017-08-20T19:41:51.167Z Reads: 194

```
yep and a 5 pack of xt90's is like 10 bucks...so you can just have extra keys with you or what not and your always able to control the board's power state :)
```

---
## \#8 Posted by: darkkevind Posted at: 2017-08-20T20:36:02.243Z Reads: 180

```
You could try something like my switch?

<img src="/uploads/db1493/original/3X/6/5/651d225926d9293091372aa2f833879a84830ea6.jpg" width="690" height="388">

It's a 120A momentary latching relay switch driven by 24v

Move rocker switch one way (momentary), it latches on, current can flow, move out the other way (momentary), it switches off, no spark. This type (rather than MOSFET type, doesn't consume power the whole time it's on.
```

---
## \#9 Posted by: willpark16 Posted at: 2017-08-20T20:42:39.767Z Reads: 172

```
Just get a vedder the diy electric skateboard ones suck and I do why people still buy them
```

---
## \#10 Posted by: Sourcecode Posted at: 2017-08-20T21:25:14.433Z Reads: 163

```
Agree the diy electric ones are shit. I also bought 2 from diy, both failed on first use. He basically told me it was my fault because I must have connected them wrong lol. On another note the one I made previous to the diy ones is still going strong so they look to be hit and miss 😑. I use a loop key now.
```

---
## \#11 Posted by: rich Posted at: 2017-08-20T21:54:41.587Z Reads: 158

```
I have 4 vedder antispark switches and couldn't live without them :grin:
I don't like loop keys or xt90 antisparks, what I need is on/off switch.
The only important thing is the switch must be connected and set OFF when connecting the battery and electronics, when it is ON it stays on because a diode get burnt.
```

---
## \#12 Posted by: darkkevind Posted at: 2017-08-20T21:56:15.126Z Reads: 154

```
The whole point of having a switch is so that the circuit is broken whilst connecting the batteries... You never want it on in that situation...
```

---
## \#13 Posted by: Jinra Posted at: 2017-08-20T22:03:04.580Z Reads: 148

```
the Vedder switches are known to fail too. However i haven't heard anyone review the direct fet version of Vedders switch
```

---
## \#14 Posted by: rich Posted at: 2017-08-20T22:04:01.083Z Reads: 144

```
That's true, just read about people who burned their antisparks (diode) because they didn't plug the switch to the pcb or let it on when they connect the battery the first time.
2 weeks ago I forgot to turn it off and changed one vesc. When I plugged the new vesc I had my first spark experience, it was scary! :joy:
```

---
## \#15 Posted by: evoheyax Posted at: 2017-08-20T22:04:39.819Z Reads: 141

```
DIY ones are crap and I can't believe he still stands by them and sells them. @torqueboards way too many complaints, you need to pull this product, even if you don't have your replacement one yet. I had multiple fail within seconds of connecting. I know for a fact I did nothing wrong. Many others have the same issue. Either you've failed to explain or provided instructions on proper use, or your switches do not work for most people. I have yet to find ANYONE besides you who claims they have no issues with it...

So far, it's around 50-0 for the fail-success ratio I've seen on this forum. I can dig up the old thread if you'd like...

At this point, that switch is a scam...
```

---
## \#16 Posted by: Jinra Posted at: 2017-08-20T22:11:50.914Z Reads: 127

```
I'm using the diyes switch, almost a year now with no issues
```

---
## \#17 Posted by: rich Posted at: 2017-08-20T22:13:33.197Z Reads: 133

```
[quote="Jinra, post:13, topic:31117"]
the Vedder switches are known to fail too
[/quote]

Do you mean in the beginning or even after longer use?
Fortunately I have "good ones" up to now :laughing: but you make me think about adding a LED so I can see if it's really off (if the switch should fail).
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-20T22:17:07.403Z Reads: 130

```
I'm not sure, just heard a couple people talk about how theirs have failed. I think @Eboosted might be able to answer the question.
```

---
## \#19 Posted by: torqueboards Posted at: 2017-08-20T22:17:09.235Z Reads: 136

```
@evoheyax I use them with no issues time and time again. They do fail easily but we'll replace any switch if anyone has any issues.

We have a direct fet one hopefully have it tested soon and we'll replace it with the current and finally be done with the current version.

I have no idea how people damage it every time. I'd just recommend to plug in to the batteries (last) after everything else is connected and give the switch 2-3 secs before turning it on/off if you are turning it on and off often (when testing).
```

---
## \#20 Posted by: evoheyax Posted at: 2017-08-20T22:17:13.043Z Reads: 134

```
ok, 50-1 then, haha.

Do you have any theories as to why yours works, while the vast majority fail?
```

---
## \#21 Posted by: Jinra Posted at: 2017-08-20T22:18:27.182Z Reads: 124

```
No idea.. maybe voltage? I'm running 10s. It seems like they always fail at the fet, so perhaps the direct fet variant will fare better. @goldenHusky has a directfet Vedder switch available. Also @JdogAwesome has been collected dead switches for research, I wonder if he found anything yet.
```

---
## \#22 Posted by: evoheyax Posted at: 2017-08-20T22:21:44.837Z Reads: 127

```
[quote="torqueboards, post:19, topic:31117"]
They do fail easily but we'll replace any switch if anyone has any issues.
[/quote]

When I contacted you, you offered to replace it if i sent the old one in plus paid $40. I did, and the new one failed within minutes again. Never turned it on and off quickly. Only turned it on once, and never went off again. Didn't want to pay another $40, so I was out almost a $100 and no working switch. Feels like a scam. It's not rocket science to plug in bullets...

I'm about to try to hook up the @goldenHusky direct fet switch today :P

I tried 2 of the @JdogAwesome switches. Nice guy, but neither worked for very long either.
```

---
## \#23 Posted by: torqueboards Posted at: 2017-08-20T22:23:15.605Z Reads: 122

```
@evoheyax - Guess you'll need to test the new switch then.. :) I'll post in the forum once they're available and do a beta run. Make sure it's bulletproof for everyone (that's the goal).
```

---
## \#24 Posted by: Eboosted Posted at: 2017-08-20T22:38:20.701Z Reads: 121

```
Can't wait for those direct fet switches Dexter!

Keep up the good work!
```

---
## \#25 Posted by: evoheyax Posted at: 2017-08-20T22:45:45.266Z Reads: 118

```
I know you mean the best for everyone. I just hate watching a product be sold that fails over and over. Even if the fail rate is only 10%, that's too high.

Hope you finish that new switch soon. We need reliable switches.
```

---
## \#26 Posted by: torqueboards Posted at: 2017-08-20T22:46:52.249Z Reads: 118

```
@evoheyax - I know.. it sucks. I'll send you one when it's available since you had issues with your old one.
```

---
## \#27 Posted by: JdogAwesome Posted at: 2017-08-20T22:50:25.433Z Reads: 118

```
@Jinra Thanks for tagging me in this, good discussion going on. From what I can tell I believe that most of the Mosfet switches out there fail from improper gate drive voltage though I'd still love to get my hands on a Diy Esk8 switch to dissect. Another thing could also be most FET's voltage rating of 60V which we often times get relatively close to at 10 or 12S. @longhairedboy recommend to me the IRFS7730 which is a 75V MOSFET that's practically identical to the 7530 though it has a ever so slightly higher RDSon. He said he hasn't had any switches fail on him since using these and it's what I'm going to use from now on. 

@evoheyax  thanks for the kind words lol. The switches that I originally sold you were my very first version and they were complete crap I'm so sorry that I thought they were viable. My new designs are far better and incorporate dual zener gate drive as well as Osh Park PCB's. I'm going to have an extra switch or two from this next batch I'm making and I'd love to send you one free of charge to makeup for my crap ones I sold you before. DM me if your interested!

P.S. like @Jinra said I still would really like to see some broken EBoard switches so if anybody has any dead ones DM me as well.
```

---
## \#28 Posted by: JdogAwesome Posted at: 2017-08-20T23:04:00.221Z Reads: 109

```
Also I have received one broken switch from @mmaner which he sent to me for free, super nice of him. It was one of @VladPomogaev V1 designs on the red PCB with the four FET's. Ended up being it was only a solder bridge causing it not work though it was going to fail anyways because the FETs are once again driven improperly only using a voltage divider, no zener diode clamping. Anyways thought I'd give the little bit of info I have from the one switch I have taken a look at.
```

---
## \#29 Posted by: evoheyax Posted at: 2017-08-20T23:08:21.160Z Reads: 112

```
Thanks for sharing. I wish this community as a whole was more open about everything. I'll pm you, cause I want everyone to get their switch game on! It saddens me that so m\any (including myself) have turned physically breaking the circuit instead of using logic. Imagine a car that you use some xt9000 plug to turn on, haha.
```

---
## \#30 Posted by: mmaner Posted at: 2017-08-20T23:14:44.878Z Reads: 112

```
I've got x2 @goldenHusky direct fet switches I'll be putting in next weekend. I'll let you guys know how it goes.
```

---
## \#31 Posted by: RaceFlight Posted at: 2017-08-21T00:33:30.018Z Reads: 109

```
So who made the switch that he is selling?
```

---
## \#32 Posted by: Rob69de Posted at: 2017-08-21T00:49:35.895Z Reads: 108

```
Hi all, I too had a @torqueboards fail on the second day..
Currently I have two @VladPomogaev v2 switches in to builds   Going strong for 6 months booth builds are ridden every day and one I even lent with obtain to buy. to a neighbor whom knows nothing of the mechanics of esk8 , he just rides. And no problems
```

---
## \#33 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-21T06:46:43.818Z Reads: 103

```
I used my Torqueboards switch for over a year on my 6S build without a problem. I'll be using it in my 10S build from now on. 

We'll see how that works out, but I'm hopeful! :slight_smile:
```

---
## \#34 Posted by: Cobber Posted at: 2017-08-21T08:18:37.913Z Reads: 101

```
[quote="evoheyax, post:22, topic:31117"]
It's not rocket science to plug in bullets...
[/quote]
Quote of the day...
```

---
## \#35 Posted by: JdogAwesome Posted at: 2017-08-21T21:46:06.987Z Reads: 88

```
Hey guys thought id drop this bye cause I just found another amazing super cheap MOSFET, the [TPH2R608NH](https://toshiba.semicon-storage.com/ap-en/product/mosfet/detail.TPH2R608NH.html). I was looking at [THIS](http://www.electric-skateboard.builders/t/diebieesc-hiamp-based-on-vesc6-hw/30829) thread and @hexakopter suggested the [TPW1R306PL](https://toshiba.semicon-storage.com/ap-en/product/mosfet/detail.TPH1R306PL.html) which got me interested in the Toshiba line of FET's which lead me to the 608. Its only a $1.57 or cheaper on Arrow and has a RDSon of 2.1mOhm.
```

---
## \#36 Posted by: Eboosted Posted at: 2017-08-22T05:35:58.750Z Reads: 80

```
I'd really like to build my own switch, if anyone has a good schematics that would like to share, I'd really appreciate it
```

---
## \#37 Posted by: JdogAwesome Posted at: 2017-08-22T06:15:03.613Z Reads: 78

```
Hey @Eboosted on my EbSC Switch thread [HERE](https://www.electric-skateboard.builders/t/boom-jda-ebsc-switch-boom-35-compact-mosfet-switch/26946), I have a link to my schematics if you want to build your own. You could also just build a Vedder one or design your own board.
```

---
