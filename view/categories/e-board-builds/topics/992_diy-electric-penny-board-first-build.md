# DIY Electric Penny Board First Build

### Replies: 41 Views: 11036

## \#1 Posted by: jonathanngkh Posted at: 2016-01-13T19:44:22.074Z Reads: 449

```
Hi, I'm making my first build on a penny board. The idea is to have an e-board small enough to casually bring on trains and buses. Basically, I'm trying to achieve this http://www.instructables.com/id/DIY-Electric-Skateboard-3/?ALLSTEPS but with the new VESC, R-spec motor, nyko wireless controller and if possible a resized SPACE cell (i'll get to this later)

I'm using:
enertion motor kit,
enertion rspec motor,
enertion trucks and wheels
latest vesc,
nyko kama wireless controller,
22" penny board,
SPACE Cell v2

I bought a SPACE cell v2 without realizing it's too big to fit on a penny board, and I'm thinking of opening it up and removing some batteries to make it smaller by sacrificing some power. Any advice? I'll try to get some professional help at makerspaces/prototyping labs, but we all know the most professional help is on here :smile:

I'm a total noob with electronics and stuff, so I have some silly questions to ask.

1) How do I do a bench test without a controller? I haven't soldered the nyko wireless wiiceiver to the VESC yet, as I have no experience with that. 

2) I also don't know how to connect the motor to the VESC. Am I supposed to crimp the wires on the VESC and then somehow glue them to the gold female connectors that came with the motor??

3) If opening up, removing some cells from the SPACE cell and repackaging it to be smaller is not feasible, I'm considering simply using the zippy 5000mAh 2S1P 20C batteries. Will it be okay to use the fast charger that's originally for the SPACE cell for the zippy batteries?

4) Is it a good idea to open up the space cell, remove some cells and make it smaller? Or rather, is it a BAD idea? I've already spent so much on it that it'd be a waste to not use it, but of course it'll be an even bigger waste to ruin it. Could always use it for a longboard build.

Any help would be greatly appreciated! So excited to not have to kick or destroy my shoes to slow my boards down.
```

---
## \#2 Posted by: barajabali Posted at: 2016-01-13T19:50:56.443Z Reads: 407

```
I'm gonna love this thread when you have this up and running!

2) you need to solder brushless motor connectors simply crimping won't ( in my experience ) be a solid enough connection like brushed motors. Each wire so the the vesc and the motor both need a male and a female gold connected that is soldered on. 

3) the zippy batteries have balance leads and I'm pretty sure the space cell doesn't play the voltage is way off.
Just buy a balance charger I use the prophet sport duo. 

4) the space cell is already pretty much as small as it can get.


So add onto 2 I make my own lipo and 18650 packs so if you need help making you lipos thinner I can give you some tips on how to make them thinner with out changing any specs on them.
Or you can permenatly combine your two lipos together
```

---
## \#3 Posted by: barajabali Posted at: 2016-01-13T19:59:00.581Z Reads: 374

```
Also be careful with trucks that size your board is gonna bite easy
```

---
## \#4 Posted by: jonathanngkh Posted at: 2016-01-13T20:05:59.180Z Reads: 384

```
Wow thanks for replying so quickly!

So

1) Bench testing means using a controller to test and get the motor going

2) Solder the wires to the gold connectors, connect gold connectors

3) Space cell charger is only for space cell

4) I mean make it smaller by sacrificing some of the batteries, that should be possible, right? Or will the battery not be able to supply enough juice that way? Probably just need to remove 1000Ah worth of batteries or less to make it fit, although it is too wide as well as too long.. I might just give up on fitting the SPACE cell onto my penny board, such a pitty

The board seems to be so high above the wheels that it wont bite, and the trucks are actually so wide that the board fits in between the wheels. Maybe it won't when turning though haha
```

---
## \#5 Posted by: Iceni Posted at: 2016-01-13T20:10:39.365Z Reads: 352

```
Nice project, I've been thinking of electrifying my Penny as well, but just finished my longboard and waiting for spring so i can ride it properly for the first time, so it'll be interesting to see what a Penny can look like!

You can use the arrow keys to control the motor in bldc tool.
Might have to tick the box marked Kb Ctrl if it is not checked already.

I'd say save the space cell for a board that fit it and use other smaller batteries for the penny.
```

---
## \#6 Posted by: barajabali Posted at: 2016-01-13T20:44:06.765Z Reads: 335

```
To take out any cells from the space cell you'll have to have some battery know how. You'll have to take one cell from each parallel connection. So all the series connections are even 

I'm not sure you can bench test without a receiver and controller in my experience 

And yes in an old build I had a basically exact setup and it bite so much lol
```

---
## \#7 Posted by: jonathanngkh Posted at: 2016-01-13T21:18:10.558Z Reads: 317

```
I guess the solution to that are raisers and maybe shaving some of the board off lol
```

---
## \#8 Posted by: barajabali Posted at: 2016-01-13T21:31:09.462Z Reads: 325

```
Yea maybe raisers and there are those weird wheel cover things. They're called wheel shields or something I'm not sure. They'll work BUT not sure if the skateboarding community will approve 😄
```

---
## \#9 Posted by: EnertionSupport Posted at: 2016-01-13T21:38:55.073Z Reads: 354

```
[quote="jonathanngkh, post:1, topic:992"]
I'm thinking of opening it up and removing some batteries to make it smaller by sacrificing some power. Any advice?
[/quote]


Without all the cells, the space cell won't be able to sustain it's original amp rating. This probably isn't a good idea because all the cells are spot welded together, and taking it apart would be a very easy thing to screw up. Nothing against you , but we don't feel it is a wise decisions for someone who is not very experienced with board electronics yet. 

[quote="jonathanngkh, post:1, topic:992"]
Will it be okay to use the fast charger that's originally for the SPACE cell for the zippy batteries?
[/quote]

you will have to buy a lipo balance charger to charge those zippy batteries. The charger for the space cell works only with the space cell because it has a built in BMS (battery management system). The BMS on the space cell regulates the cell voltages so the charger doesn't have to.

With the zippy's, there isn't anything to regulate the cells, so you'd need a charger that can do that. Your other option is to add a BMS, but that is significantly more work and a balance charger is the easiest solution. 

[quote="jonathanngkh, post:1, topic:992"]
but of course it'll be an even bigger waste to ruin it. Could always use it for a longboard build.
[/quote]

You could still make a compact commuter, it'd just be a little longer and wider than a penny board.

minimum deck length would probably be around 30" for the space cell to fit. Maybe more, maybe less depending on truck mounting locations.
```

---
## \#10 Posted by: claudiofiore88 Posted at: 2016-01-13T21:44:02.322Z Reads: 304

```
You should be able to return the spacecell to @onloop. Doesn't enertion have like a 300 or 600 day return policy? Or you could sell it for a loss.
```

---
## \#11 Posted by: cmatson Posted at: 2016-01-13T21:46:02.312Z Reads: 309

```
[quote="claudiofiore88, post:10, topic:992"]
You should be able to return the spacecell to @onloop
[/quote]

true, but because of the really strict battery regulations he would be required to ship it overseas by boat, and it'd be really expensive.. 

plus it'd take many months to get back to Australia (assuming you are not in Australia @jonathanngkh)
```

---
## \#12 Posted by: jonathanngkh Posted at: 2016-01-13T23:03:06.602Z Reads: 288

```
Wow emotional rollercoaster right here. 'Oh yeah I could send it back' 'Oh yeah I paid $100 in import taxes to get it in'

I'll just save it for a future r-spec build then. And order that balancing charger. Such great info you guys
```

---
## \#13 Posted by: lowGuido Posted at: 2016-01-13T23:22:37.586Z Reads: 278

```
sell the space cell and buy a small lipo.
```

---
## \#14 Posted by: MonsterCoatings Posted at: 2016-01-15T15:37:52.333Z Reads: 282

```
@jonathanngkh  I would keep it for your next project, just read all the posts here it really is an excellent product & design. PM me if you need to sell the space cell. I was looking to buy a space cell for my next MTB project.
```

---
## \#15 Posted by: jonathanngkh Posted at: 2016-01-18T21:37:18.769Z Reads: 301

```
Hi, I have a question regarding batteries, not sure if I should start a new thread, just let me know.

I understand that if I have a 5000mAh battery with 20Cs, that's 100A. And That's already "too much" considering onloop recommends that 60A is enough, right?

But if I have 2 5000mAh batteries in series, both at 20Cs, 7.4V each, what's the A rating then? The same?

Also, where does battery life come in to this? It seems like having more mAh would provide a longer battery life, is that correct?

I just busted my zippies by connecting them together, rookie mistake I know, just lucky to be alive and no explosion (no battery swelling too, just the plugs got fried)

So should the new batteries that I'm going to get be like 3000mAh at 20Cs to achieve the power efficient rating of peak 60A? I'm a light guy, only 58kgs, and would like as efficient a build as possible with long battery life.
```

---
## \#16 Posted by: cmatson Posted at: 2016-01-18T21:46:33.394Z Reads: 310

```
[quote="jonathanngkh, post:15, topic:992"]
And That's already "too much" considering onloop recommends that 60A is enough, right?
[/quote]

it's not too much, it's just saying that is what it *can* peak.

Being able to deliver more amps than your system needs won't hurt anything- if anything it's just some safe breathing room.

If you were to knock down from 5,000mah to 3,000mah, you'd be hurting your range more than you probably want.
```

---
## \#17 Posted by: lox897 Posted at: 2016-01-18T22:00:10.700Z Reads: 286

```
@cmatson Explained it perfectly.
```

---
## \#18 Posted by: jonathanngkh Posted at: 2016-01-18T22:01:38.599Z Reads: 288

```
Thank you so much, as always for the great info and quick replies too.

Guess I'll stick with 5000s!
```

---
## \#19 Posted by: jonathanngkh Posted at: 2016-01-18T22:04:34.019Z Reads: 305

```
I have a VESC, how does regenerative braking work with batteries that don't have a BMS (like the zippy flightmax 5000s)?

Sorry for all the silly questions and thanks for your patience and guidance always
```

---
## \#20 Posted by: cmatson Posted at: 2016-01-18T22:15:38.592Z Reads: 306

```
haha everyone has to start somewhere, so no question is a stupid question! 

the regen braking is so minimal it won't hurt your batteries. They will get more unbalanced from just being discharged than they will from regen braking, so I wouldn't even worry about it. 

I'd just set your lipo cutoff above the minimum 3.2v per cell to ensure the batteries don't get damaged over a long period of time.
```

---
## \#21 Posted by: delta_19 Posted at: 2016-01-18T22:23:45.727Z Reads: 265

```
what would you suggest is a good voltage to stop at? so far i quit at 3.7v giving me .5v of room to boot on from a full charge.
```

---
## \#22 Posted by: cmatson Posted at: 2016-01-18T22:45:54.157Z Reads: 277

```
you could go lower than that if you wanted to squeeze a little more range out of it, but 3.7 is a fine stopping point. 

I have my cutoff set at 3.4
```

---
## \#23 Posted by: jonathanngkh Posted at: 2016-01-18T22:56:33.738Z Reads: 285

```
Just read onloop's regen braking thread http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353

Still confused. 2x 5000mAh 2S 20C batteries in series at 7.4V each would give me 14.8V total, so I should set the Minimum Input Voltage at 14.8/4 = 3.7V ?

I guess what I really want to know is what to fill in in all the blank spaces in the BLDC app given my configuration. Perhaps just the defaults will be fine
```

---
## \#24 Posted by: NNGG Posted at: 2016-01-18T23:02:57.627Z Reads: 272

```
I have mad hills where I live and I am wondering if I should just connect all three motor leads together to act as a generator as I go down the hill and that energy will be released as heat.
```

---
## \#25 Posted by: lowGuido Posted at: 2016-01-19T23:02:28.866Z Reads: 263

```
I would not suggest that anyone ever connect all 3 leads together.

just use the brakes on the VESC to control your decent.
if you are worried about over charging then don't fully charge the battery before you descend the hills.
leave yourself a little bit of headway.

if you do the math, you can bomb the hill and work out how many amp hours you gain and leave that amount out of your full charge.
```

---
## \#26 Posted by: trbt555 Posted at: 2016-01-20T06:09:42.142Z Reads: 259

```
[quote="delta_19, post:21, topic:992, full:true"]
what would you suggest is a good voltage to stop at? so far i quit at 3.7v giving me .5v of room to boot on from a full charge.
[/quote]

I  was wondering about the same thing some weeks ago and decided to do a [few tests][1] to see what a good cutoff point would be. 3.6V seemed to be ideal.

  [1]: http://www.electric-skateboard.builders/t/loaded-dervish-dual-r-spec-6355-dual-vesc-nunchuck-paris-195-90mm-flywheels/524/62
```

---
## \#27 Posted by: NNGG Posted at: 2016-01-20T07:05:41.441Z Reads: 253

```
Connecting all three leads in not bad or dangerous, Its just that the energy the motor get is transferred into heat. VESC brakes are better just because they already do that and more.
```

---
## \#28 Posted by: NNGG Posted at: 2016-01-20T07:07:20.630Z Reads: 260

```
I have had lipos at 2.99V-3.7 and I would say 3.4 is the lowest you wanna go, and that gives you some extra wiggle room. I will set mine at 3.4-3.7V.
```

---
## \#29 Posted by: lowGuido Posted at: 2016-01-20T07:10:08.857Z Reads: 274

```
you're not wrong it would generate heat.
but
a.) you don't know how much heat. maybe enough to melt insulation and burn out the motor?
and that's if
b,) you can even get it to roll at all with a shorted motor.

i'm all for science though. give it a try and report back.
```

---
## \#30 Posted by: NNGG Posted at: 2016-01-20T07:17:09.920Z Reads: 269

```
All ready have and its just scary not having any control and going down a 30 degree hill at 5mph. You are correct about using esc brakes, they are fine on my 1/10 scale 3S esc and cant wait for the vesc
```

---
## \#31 Posted by: jonathanngkh Posted at: 2016-01-21T17:12:43.184Z Reads: 275

```
Hi guys, I made some progress today. Soldered the nyko kama nunchuk receiver to the jst connectors and they connect just fine. Soldered the vesc to the motor connectors too, and soldered leads for my zippy batteries.

But I think I fudged up my vesc, really hope not. I was having a lot of trouble with the BLDC, but eventually i got it connected. Motor detection wasn't working, but then I realised that was because i had my receiver plugged in. So I unplugged it, rebooted and reconnected and ran motor detection.

VEEEEEEE the motor starts going, slows down just like in Vedder's video, then VSH it starts up and chokes. Next thing I know, the VESC is no longer connected, and the LEDs on the VESC no longer light up, so I can't connect it.

I had my space cell connected to the VESC, VESC connected to motor. Did it short? Is it fudged? Should I get a new one? If so, how do I prevent the same thing from happening?

So close, yet so far
```

---
## \#32 Posted by: chaka Posted at: 2016-01-21T22:23:26.228Z Reads: 254

```
Sounds like you have a short somewhere. Check with your distributor and make sure you wont void the warranty before pealing the shrink wrap off and inspecting the board for loose solder and bridged processor/driver legs.
```

---
## \#33 Posted by: jonathanngkh Posted at: 2016-01-21T22:55:56.604Z Reads: 251

```
Does the one from @EnertionSupport come with warranty? If so, does it qualify?

So the solution is to check for broken pieces? Sorry, I don't know much. What do I look out for visually?
```

---
## \#34 Posted by: jonathanngkh Posted at: 2016-01-21T23:19:51.157Z Reads: 255

```
I'll upload pictures soon
```

---
## \#35 Posted by: jonathanngkh Posted at: 2016-03-03T19:20:15.243Z Reads: 276

```
Hey everyone, I got a new VESC and it works wonders. I've almost got everything in place now, can't wait to ride it!

I'll put up pictures for everything else.

What balancing charger specifically would you guys recommend? I have 2 x ZIPPY 5000mAh 2S1P 20C batteries in series.

Also, can someone tell me what settings I should have my VESC on specific to that battery set up?

Thanks
```

---
## \#36 Posted by: mohammedex Posted at: 2016-04-18T23:47:37.693Z Reads: 274

```
Any updates?
20 characters max be damned
```

---
## \#37 Posted by: jonathanngkh Posted at: 2016-04-21T10:15:57.200Z Reads: 278

```
<img src="/uploads/db1493/original/2X/b/b5604bc54e8a9341d413ecd39e9447df2bb995ef.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/3/36e19c5c858a049a8800996d62609ed79526d96d.jpg" width="666" height="500">

Sorry it took me so long to update this! So this is my electric enertion penny hybrid board and it's looking so so sexy with that white on white. Final build:

Deck: Penny Deck
Batteries: 2x Zippy 5000mAh 2S 7.4v 20C Li-Po batteries in series
ESC: VESC
Remote Controller: Nyko Kama Nunchuk
Wheels/Decks/Motors: Enertion Single Motor Kit

It goes at about 20km/h~ max as I'm only running a 14.8v setup. I have space in my enclosure to fit in 3S or even 4S batteries, so that should provide a big speed boost to 30-40km/h. It rides like a dream, and is tiny and weighs about 4.5kg currently.

For the 'enclosure' i sawed off the top of a piece of tupperware and screwed it to the base of my penny board, then put velcro on all 4 sides, and made the cover out of duct tape strips that I folded in half and weaved together. It turned out looking pretty unique I think.

I wouldn't have done it without all you guys' help!

Let me know what you guys think!
Also should I update the first post on here with this?
```

---
## \#38 Posted by: itsmikeholland Posted at: 2016-06-10T20:57:13.548Z Reads: 252

```
I don't know much about the underside of the pennyboards, but it looks like you have quite a significant amount of room to move the trucks to the edges of the board and make more room for extra batteries. Have you considered this?
```

---
## \#39 Posted by: jonathanngkh Posted at: 2016-06-12T14:50:26.976Z Reads: 254

```
That's a good point. Unfortunately, it starts to curve a lot more beyond where I've put in the screws for the trucks
```

---
## \#40 Posted by: Sapphirinia Posted at: 2017-01-21T19:28:27.779Z Reads: 166

```
Do you have any tips for someone trying to do the same with a nickel board?
```

---
## \#41 Posted by: jonathanngkh Posted at: 2017-01-29T15:00:58.316Z Reads: 153

```
Make sure everything fits. Working on Pennys/Nickels, we have less space to work with so just be mindful of that when you're buying batteries and thinking of how to configure them.

You might want to get grip tape for your Nickel board too, going at those speeds, a little more friction goes a long way.

You definitely don't need a dual drive configuration.

Get your truck alignment right. You'll likely have to drill new holes into the Nickel board if you're using the enertion giant trucks and wheels. You only get one chance to do this! I messed mine up, so turning right is a lot harder than turning left. Don't make the mistake I did.
```

---
