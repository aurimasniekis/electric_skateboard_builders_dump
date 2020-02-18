# My battery pack turned into fireworks

### Replies: 159 Views: 5533

## \#1 Posted by: Quezacotl Posted at: 2017-12-19T15:12:25.627Z Reads: 567

```
Hello!

I got some Samsung 35E cells. 3,5Ah with 10A current.
I made an battery of 10S3P.
<img src="/uploads/db1493/original/3X/d/a/dab179155204befc1ecd0bf5c0a4027476ea3a3b.jpg" width="690" height="388">
I installed cardboard covers for the positive terminals to protect. And i spot welded the batteries:
<img src="/uploads/db1493/original/3X/6/3/630d46a22ad0d399f7619ed97378b1c913e18b41.jpg" width="690" height="388">
Here i'm going to fold those into what's in next picture. (Quit making assumptions that this is folded from middle! It is two-way fold, like a book)
<img src="/uploads/db1493/original/3X/6/9/697a43a615d6e24d476e135236461429062d7797.jpg" width="690" height="388">
Folded.
<img src="/uploads/db1493/original/3X/3/a/3a8209ac9ebefdefd3d59211e6503a508a400bb9.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/b/c/bc7f09c6ad46150ce0ff53840ffac3fff3ab76ee.jpg" width="690" height="388">
Installed the wires and connectors.
<img src="/uploads/db1493/original/3X/4/b/4b263815a0e3e6865601e01c198a635c1670e807.jpg" width="690" height="388">
Made an enclosure with some paddings and made sure that wires are loose and that nickel stripes won't cut the wires.
Then i wrapped it on duct tape so it's sealed.
<img src="/uploads/db1493/original/3X/c/4/c49254e71b121f2dc81fb177a1146d3661875fff.jpg" width="690" height="388">
I have charged it every now and then with 42V and 2A. It started sparkling like an rocket and i tossed it outside.
<img src="/uploads/db1493/original/3X/e/6/e6ee2ac067961b415ae1134c0ee3b87bb018f1c7.jpg" width="690" height="388">
Here's what i managed to salvage :D
<img src="/uploads/db1493/original/3X/e/b/eb16a9a91fd91315b86074d9a2c7002975ad7df0.jpg" width="690" height="388">

What do you think could have caused it? All the cells were oriented the right way, and connections were triple checked.
This was the very first time those cells were under a charge. series charging without balancing on 2A current. So it's 0,2C rate.
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-12-19T15:18:45.794Z Reads: 542

```
Fake cells?
```

---
## \#3 Posted by: vishal_tejwani Posted at: 2017-12-19T15:18:48.584Z Reads: 544

```
Dude, cover the cells with some tape from next time, cells might have touched and caused this, you are lucky that there is no major damage beside of burning up your cells.

After Soldiering all the wires make sure there is no contact point for anything to touch the +&- parts of the Battery
```

---
## \#4 Posted by: banjaxxed Posted at: 2017-12-19T15:22:01.431Z Reads: 541

```
Looks like poor insulation to me, and who knows maybe even a solder short

Ok looks like no solder used? Question why are the spot welds so discoloured? This should not be so....anode damage?
```

---
## \#5 Posted by: Idle Posted at: 2017-12-19T15:29:01.654Z Reads: 534

```
Post up what spot welder you used and the settings. 

Glad you and the rest of your board are ok.
```

---
## \#6 Posted by: Quezacotl Posted at: 2017-12-19T15:47:08.299Z Reads: 529

```
Not likely fake cells. They are from here:
https://eu.nkon.nl/rechargeable/18650-size/samsung-inr18650-35e.html

Hmm. I'm going to shrink-wrap the next cells from now on. But i don't think that was the case here of those rubbing to each other. But good point.
And i'm going to use double cardboards on positive terminals also.

Discolored? Hmm... Googling a little... yea they are discolored, meaning there is big currents going in spot-welder.

My spot welder is based on this:
http://www.avdweb.nl/arduino/hardware-interfacing/spot-welder-controller.html
(Appears that it has LCD screen nowadays. My circuit has only selectable main pulse.)

I have adjusted the settings, so that it welds that nickel stripe i have, not any thicker. Settings are 50ms pulse, 500ms wait, 400ms pulse. The current is that i remember, around 1000A-1300A

<img src="/uploads/db1493/original/3X/5/8/580483c99c3d41699106726f38923151caf656d6.jpg" width="690" height="388">
```

---
## \#7 Posted by: Blasto Posted at: 2017-12-19T16:00:44.797Z Reads: 507

```
was this the fold line?

<img src="/uploads/db1493/original/3X/a/9/a9b9d059676604f8ad59dc0d45f6436c81344095.png" width="690" height="437">

the cells dont look insulated in the middle,  i may be wrong...
```

---
## \#8 Posted by: Hummie Posted at: 2017-12-19T16:06:38.535Z Reads: 497

```
haha that's hilarious.  you folded the cells into each other.  of course they shorted.
```

---
## \#9 Posted by: SirDiff Posted at: 2017-12-19T16:09:46.031Z Reads: 499

```
Wait, did you not insulate them in the middle? I'm surprised it lasted till the first charge, the one time i made that mistake my whole pack instantly started to short and a nickel strip fused to save the day, and it happened because i had opened and uninsulated the whole thing for maintenance and my hand slipped while doing it!
```

---
## \#10 Posted by: florensvb Posted at: 2017-12-19T16:10:02.898Z Reads: 497

```
Yeah i was gonna say: How did you manage to just fold them onto each other without insulation?? :D
```

---
## \#11 Posted by: ducktaperules Posted at: 2017-12-19T16:12:25.322Z Reads: 495

```
my understanding was that he folded between row 1/2 and again between 3/4.
```

---
## \#12 Posted by: SilentException Posted at: 2017-12-19T16:12:38.885Z Reads: 493

```
I don't think that was the fold line. I think the fold was here and here :)

<img src="/uploads/db1493/original/3X/0/8/08afc5bd0599dd941953c1be5ec3ad44b59953aa.png" width="652" height="383">

Then the bottom (or top when folded) was done. Also, if you short the cells out, you don't really have to wait for a charge process to see a fire... :)
```

---
## \#13 Posted by: okp Posted at: 2017-12-19T16:14:11.144Z Reads: 488

```
OMG. You need a good isolation man.
```

---
## \#14 Posted by: psychotiller Posted at: 2017-12-19T16:25:18.930Z Reads: 483

```
If you folded them down the middle without putting insulation there I'm pretty sure you didn't even get to plug in your charger....
```

---
## \#15 Posted by: squishy654 Posted at: 2017-12-19T16:46:38.418Z Reads: 478

```
Oh this is awesome, thanks for the lesson dude, many people will learn from this...complacency will get you..
```

---
## \#16 Posted by: Blasto Posted at: 2017-12-19T16:49:51.065Z Reads: 478

```
Yes i think you are right.
```

---
## \#17 Posted by: deucesdown Posted at: 2017-12-19T16:52:09.255Z Reads: 475

```
So this fold looks okay, right?

I'm thinking balance wires shorted, but this was first charge on bench, not a lot of movement. Maybe cells torched by diy welder?

Scary.
```

---
## \#18 Posted by: scepterr Posted at: 2017-12-19T16:52:34.934Z Reads: 466

```
All those folds are not needed
That's the weirdest config I've seen 🤔
```

---
## \#19 Posted by: deucesdown Posted at: 2017-12-19T16:58:20.644Z Reads: 469

```
I clicked the photos, the discoloration is the sort that happens from lotta lotta heat. Like when cutting tools are burnt, and lose their temper and edgeholding ability. Very consistent amount of it on each weld.

I'm voting for damaged cells.

Only 2A charge current...

@Quezacotl if you have a spare cell, maybe weld nickel to the terminals (with same heat discoloration) and try to charge that single cell, see if flames shoot out? Make sure camera is running this time. ;)

1 cell is probably not going to be conclusive, but it should give you more information on whether you need to rethink your welder.
```

---
## \#20 Posted by: ducktaperules Posted at: 2017-12-19T17:15:03.945Z Reads: 452

```
may i ask how you charged it without a balance charger?
```

---
## \#21 Posted by: banjaxxed Posted at: 2017-12-19T17:47:37.774Z Reads: 429

```
I'm pretty sure Isis released the layout spec
```

---
## \#22 Posted by: bimmer Posted at: 2017-12-19T18:31:09.236Z Reads: 434

```
How did you charge those cells?
What is  the  material you used to spot-weld the batteries? 
The series connections look way to small and the discoloration indicated that it was cheap nickel plated steel from aliexpress.
So either you didn't insulate correctly on the fold ie. use poly-amid tape and while charging something got warm  and expanded  causing a short or your charge leads shorted one of those weak series connections your undersized connection got redhot and bent down melting through the batteries insulation, shorting  the battery to itself causing a fatal termal runaway in your battery, Once one battery goes they all go.

Next time use 100% pure  nickel. 8mmx0.15mm Nickel can handle 6A plated steel can handle 2A.
Also Kapton or poly-amid tape is important.
Double check your balance leads!
```

---
## \#23 Posted by: thisguyhere Posted at: 2017-12-19T18:35:23.803Z Reads: 427

```
no, look at the original pictures, it's folded down the middle of the two-cell stacks. 

this should be stickied for what not to do.
```

---
## \#24 Posted by: SilentException Posted at: 2017-12-19T18:36:56.458Z Reads: 426

```
No man. You should take another look at the finished pack.
```

---
## \#25 Posted by: darkkevind Posted at: 2017-12-19T18:49:58.250Z Reads: 431

```
I think your problem was here where I've marked when you folded the pack...

Of course, you bridged the polarities so of course, they shorted :confused:

<img src="/uploads/db1493/original/3X/4/1/4171a6e77a58feb1bfab188003054c70f1207780.png" width="690" height="386">
```

---
## \#26 Posted by: scepterr Posted at: 2017-12-19T19:20:06.730Z Reads: 423

```
Each half should be like this if thats the shape you want
<img src="/uploads/db1493/original/3X/f/5/f57f4fc2104d31d5bb6568a6cf4fd30343806719.jpg" width="666" height="499">

And that nickel should only be used for parallel, never series
```

---
## \#27 Posted by: deucesdown Posted at: 2017-12-19T19:27:07.370Z Reads: 407

```
He's right. 8 cell stack on bottom, 7 cell stack on top.
```

---
## \#28 Posted by: pixelsilva Posted at: 2017-12-19T19:42:49.349Z Reads: 411

```
(first, I know so few about batteries that's why I will rely on an expert to build mine).



@eboosted was right. This thing is a bomb. 'am sorry to say this but the FAA, airlines and transportation authorities have all the right to be concern. Batteries are capable to bring down  commercial aircraft easily and produce a major catastrophe. Specially a hand-made custom battery pack. A few years ago one of the most modern airplanes, if no the most, a Boeign 777, was destroyed by a short from a faulty battery inside the avionics compartment below the cabin. A hundred million dollar aircraft destroyed by a simple faulty battery. :open_mouth:
```

---
## \#29 Posted by: saul Posted at: 2017-12-19T19:47:45.217Z Reads: 408

```
[quote="Quezacotl, post:1, topic:41458"]
This was the very first time those cells were under a charge. 

[/quote]

where they all at the same voltage to start? Did you check?


[quote="Quezacotl, post:1, topic:41458"]
series charging without balancing
[/quote]

if not then this is what did it. one got over charged. then a chain reaction. :boom:

folding could have also shorted like other people suggest. not sure why you would fold them sine they are 2 wide and 2 high either way....
```

---
## \#30 Posted by: Hummie Posted at: 2017-12-19T19:56:10.749Z Reads: 399

```
I think for sure it was the folding that shorted the cells and then the charging later while shorted that set it on fire.  very unlikely a faulty cell as they are very very rare and if series charging especially with a new pack its very unlikely to be out of balance already and even if it were out of balance and were to send a cell way high I don't think that would do it.  According to manufacturers' testing I think maybe all the 18650s in whatever chemistry pass a standardized shorting test and overcharge tests and don't go into thermal runaway and it's only when many of them are put beside each other that they will build up a temp that's capable of sending one into runaway.  so I read.
```

---
## \#31 Posted by: Quezacotl Posted at: 2017-12-19T20:15:35.228Z Reads: 400

```
Haha. (Almost) All of you are convinced that i folded those like on the edited picture Blasto posted.
Like you see, the bottom two rows have 7 cells and top two has 8. 7 folds to 7, and 8 folds to 8. The center-fold would be very foolish :smiley:
And that fold is the easiest way to get the pack in the form it was. Minimum cutting and bending of the nickel stripes.
Actually if you folded the pack like Blasto pointed, it would maybe be slightly possible to avoid the sparks for a long time, if you are in luck :stuck_out_tongue_closed_eyes:

@bimmer: I have tested that those are pure nickel. Sand it to expose potential steel and keep in salt water for overnight. So the discoloration must be related to welder settings.
I happened to be today at my local hackerspace, and we also discussed about this topic. Friend told also that the most plausible thing that happened, was what you said; one of the cells were faulty, expanded, heated and caused an chain reaction.
Also the friend told that while it would discolor, it is still not that much heat that it would damage the cell internals. Soldering the cells is way more destructive/dangerous and yet still people get successful packs.

@ducktaperules: Charging the whole pack from one end to other, while monitoring the individual cell voltage.

@scepterr:  Shape you pointed was my first idea also. I came up with the different configuration, because it was easier to accomplish, especially with the folding-part. Of course i could have folded every cell-pair individually, but that again, would have been harder.
Yea, single nickel stripe is not enough in series if you are going to run serious currents. What i use is around max 10A

@saul: Yes i measured they all were the same voltage. And like i said on this post earlier, they were individually monitored.

@Hummie: It is not the folding. Read the top lines of this post.
But a friend said that he has had a few faulty cells also that were wrapping-melting hot. Luckily he did not have the series cells hugging each other. Only the one parallel got bad.

So the most plausible conclusion; A faulty cell.
What i learned; Use kapton tape or similar to wrap the cells, and cycle the cell capacity one time before assembling into a pack.

But what you suggest for the spot-welder settings?

About my background; I have hundreds of salvaged laptop-battery cells. I have made many batteries for my e-bike and different things, though i have always used these brackets which protect the cells touching each other:
(picture is for quick illustration purpose only)
<img src="/uploads/db1493/original/3X/b/e/bebd2d293679fa5cff6cf5a053a45f660a64454a.jpg" width="690" height="388">

This time i were over-convinced that the cells are surely good, that only the voltage measurement would do. The old laptop cells have to be measured with capacity on nominal current and also internal resistance.
```

---
## \#32 Posted by: scepterr Posted at: 2017-12-19T20:20:38.058Z Reads: 382

```
There would be only 1 fold in the configuration I posted

Those shaped "nickel" rolls, are not pure nickel,
It sparks when you weld right?
```

---
## \#33 Posted by: Deckoz Posted at: 2017-12-19T20:21:14.124Z Reads: 391

```
Proper insulation. Yes masking tape is proper abrasive resistance when applied over kapton like fishpaper...if ya don't believe me disassemble any production LiPo battery. 

<img src="/uploads/db1493/original/3X/b/e/be105f4207a60faa7960030e8477cb9511a1af91.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/6/6/662fbb0de06ed3890b036f4a8eb423fdcf6eaf09.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/1/c/1cc264ef147b61c7389ffdbf01a53a82068f589c.jpg" width="374" height="499">

Edit: general reply..not directed towards who I replied to
```

---
## \#34 Posted by: GrecoMan Posted at: 2017-12-19T20:26:47.477Z Reads: 376

```
improper insulation. kapton insulates heat, the thing that you dont want in you pack. you have the entire pack wrapped in it so no airflow or heat movement is possible
```

---
## \#35 Posted by: Deckoz Posted at: 2017-12-19T20:31:23.338Z Reads: 375

```
Greco... Been building Li-ions for a long time, the ends are insulated, and the packs are never operating at 100% of thier rated capacity. Yea kapton traps heat, but cells don't get hot when you pull less then half of thier current capabilities 90% of your riding.

My packs run cooler then my ESC's. Say improper insulation... Or safe insulation and not stressing cells... I'll choose safe insulation and treating my cells like babies.
```

---
## \#36 Posted by: pixelsilva Posted at: 2017-12-19T20:35:03.100Z Reads: 362

```
Why they never leave a few cut openings on the plastic wrap? That should fix the heat trapped inside, no?
```

---
## \#37 Posted by: Quezacotl Posted at: 2017-12-19T20:37:26.185Z Reads: 369

```
@scepterr: To accomplish the shape you see on original post 5th picture how do you do it with one fold?
It doesn't spark while i weld. Although while welding to nickel-plated steel, you can get spark-free weld if you give enough and even pressure. But i will test the stripe again to make sure. Could be that i haven't sanded it enough :slight_smile:

 @Deckoz: Yea i have the same paper than on production packs. Material is plastic and surrenders under soldering iron. I have used that on every LiPo-packs i have made.

@pixelsilva: Humidity gets in...
```

---
## \#38 Posted by: GrecoMan Posted at: 2017-12-19T20:38:42.799Z Reads: 359

```
it will help but not eliminate the problem. try to cover as little surface area as possible when using kapton in packs <6p and heatshrink the whole thing.
```

---
## \#39 Posted by: scepterr Posted at: 2017-12-19T20:39:17.064Z Reads: 356

```
Just 1 fold between 5th and 6th series at the end
```

---
## \#40 Posted by: deucesdown Posted at: 2017-12-19T21:03:32.423Z Reads: 360

```
[quote="Quezacotl, post:31, topic:41458"]
monitoring the individual cell voltage.
[/quote]

What was going on with voltages? Nothing crazy, everything coming up nice and evenly?

Did it start sparking immediately?

I'm really hoping we develop some kind of theory, for safety's sake.

Melting insulation shouldn't even have been an issue, whatever went wrong was already far gone at that point
```

---
## \#41 Posted by: Acido Posted at: 2017-12-19T21:04:51.720Z Reads: 327

```
Because of too much heat
```

---
## \#42 Posted by: Acido Posted at: 2017-12-19T21:08:39.190Z Reads: 332

```
Yea that happened to me 2 days ago while i was measuring how much nickel strip i needed like the thing just melted and fell down and stick to the first layer

Damn I got scared an instant burst of 120+A is no joke!
```

---
## \#43 Posted by: Acido Posted at: 2017-12-19T21:10:07.611Z Reads: 321

```
If its shrink wrapped isnt it the same thing?
```

---
## \#44 Posted by: scepterr Posted at: 2017-12-19T21:10:54.561Z Reads: 319

```
Shrink would melt away wayyyy before kapton tape
It gets holes while shrinking if you get too close...
```

---
## \#45 Posted by: deucesdown Posted at: 2017-12-19T21:15:48.287Z Reads: 340

```
How do you even reasonably monitor cell voltages while charging... lipo cell monitors wired in? those are typically 6s/8s not 10s. And not terribly accurate.

Cycle testing every cell is a big pain in the balls. Need to build a fixture to hold cells and wire up to balance charger, which usually only do 8s at a time. Don't want parallel here as you're trying to determine individual cell capacity/health.

And it's quite rare to get bad cells from brands like Samsung.

And, I don't think soldering temperatures will discolor nickel that way. I'll test though...
```

---
## \#46 Posted by: Sebike Posted at: 2017-12-19T21:16:26.462Z Reads: 340

```
Ladies and Gentlemen, the Fold;

<img src="/uploads/db1493/original/3X/f/8/f8ed505932675b5f249f80acdebb5c79c06a0355.jpeg" width="690" height="388">

😁
```

---
## \#47 Posted by: Acido Posted at: 2017-12-19T21:17:13.982Z Reads: 337

```
Im was thinking about no airflow with the kapton
Its the same with and without if you shrink it
```

---
## \#48 Posted by: scepterr Posted at: 2017-12-19T21:22:49.965Z Reads: 335

```
Not really, it's not sticking to anything underneath
```

---
## \#49 Posted by: Quezacotl Posted at: 2017-12-19T21:48:40.920Z Reads: 340

```
@deucesdown: I don't know how rapidly the voltages changed. I wish i had my meter attached, but it was under repair. So i just measured through the balance-connector with multimeter, one by one, and repeat after a while.
This meter is what i'm talking about:
(Don't analyze it further. Just for illustration)
<img src="/uploads/db1493/original/3X/5/8/583c8ea77d1071f791b1e6382e73faff7ae9df38.jpg" width="281" height="500"> 

The pack started sparkling like... zzrrt.... huh? ...zzrrtt...smoke... and i ran with it outside... and it zizzled and sparkled for a while, until it was like an fireworks. :boom:
There was no way i could unwrap and open the box in time to stop the reaction :frowning:

By the way, i have a nickel stripe on salt water now again, and surely well sanded. We'll see the result tomorrow.
```

---
## \#50 Posted by: deucesdown Posted at: 2017-12-19T22:42:46.693Z Reads: 328

```
[quote="Quezacotl, post:49, topic:41458"]
The pack started sparkling like... zzrrt.... huh?
[/quote]


Did this happen immediately? Or did it charge for a while, then zzrrt. Sounds like you did some multimeter readings, so it took some time, and voltages looked okay?

btw awesome contraption. I ordered some small voltmeters, but the accuracy seemed horrid, and it's kind of hard to hook them up? The 2 wire versions, can't turn on/off as a set, need to unplug, and the 3 wire versions, need a voltage divider or something.
```

---
## \#51 Posted by: Cobber Posted at: 2017-12-19T23:42:57.451Z Reads: 329

```
[quote="deucesdown, post:45, topic:41458"]
How do you even reasonably monitor cell voltages while charging... lipo cell monitors wired in? those are typically 6s/8s not 10s. And not terribly accurate.
[/quote]

with my icharger
http://www.icharger.co.nz/icharger-308-duo
http://www.icharger.co.nz/assets/full/308DUO.jpg
has a 31hour data log file :slight_smile: 
accurate? i'll put it up against anything
```

---
## \#52 Posted by: Funktapus Posted at: 2017-12-19T23:46:08.400Z Reads: 313

```
If it was fine when not charging, then you can rule out bad welding, nickel strips etc. If the problem occurred when charging then it might have something to do with the balance leads. Are you confident that they were wired correctly?
```

---
## \#53 Posted by: PXSS Posted at: 2017-12-20T00:04:18.324Z Reads: 326

```
[quote="Hummie, post:8, topic:41458, full:true"]
haha that's hilarious.  you folded the cells into each other.  of course they shorted.
[/quote]

Wrong

[quote="SilentException, post:12, topic:41458"]
I think the fold was here and here :slight_smile:
[/quote]

Correct

[quote="thisguyhere, post:23, topic:41458, full:true"]
no, look at the original pictures, it's folded down the middle of the two-cell stacks. 

this should be stickied for what not to do
[/quote]

Wrong

[quote="darkkevind, post:25, topic:41458"]
Of course, you bridged the polarities so of course, they shorted :confused:
[/quote]

Wrong

[quote="Hummie, post:30, topic:41458"]
I think for sure it was the folding that shorted the cells
[/quote]

Wrong

[quote="GrecoMan, post:34, topic:41458"]
kapton insulates heat
[/quote]

Wrong

[quote="Deckoz, post:35, topic:41458"]
kapton traps heat,
[/quote]

Wrong
```

---
## \#54 Posted by: Deckoz Posted at: 2017-12-20T00:06:59.346Z Reads: 297

```
[quote="PXSS, post:53, topic:41458"]
Wrong
[/quote]

Let me reword. Kapton reflects heat. However it is negligible when talking about heat soaking. The benefits outweighs the bad. As your talking about less then 1-2c difference in soaking with kapton
```

---
## \#55 Posted by: stormboard1 Posted at: 2017-12-20T00:07:10.184Z Reads: 303

```
kapton does tap heat tho???
```

---
## \#56 Posted by: deucesdown Posted at: 2017-12-20T00:47:07.306Z Reads: 309

```
[quote="PXSS"]
Wrong

Correct

Wrong

Wrong

Wrong

Wrong

Wrong
[/quote]

Oh my actually laughed out loud. Great post!
```

---
## \#57 Posted by: deucesdown Posted at: 2017-12-20T00:48:37.835Z Reads: 298

```
But... This is not reasonable :slight_smile: And you have to split the 10s, right? Accurate I'll give you
```

---
## \#58 Posted by: Cobber Posted at: 2017-12-20T01:02:34.394Z Reads: 312

```
http://www.icharger.co.nz/icharger-4010-duo
10s duo...
just costs a bit more coin :money_mouth:
http://www.icharger.co.nz/assets/full/4010DUO.jpg
I don't own this one though I have the 308
```

---
## \#59 Posted by: psychotiller Posted at: 2017-12-20T01:11:36.868Z Reads: 312

```
<img src="/uploads/db1493/original/3X/9/d/9dab1beee749d581027065b8a6411e3a98e67255.png" width="652" height="383">

How does the parallel configuration work with this circled group?
```

---
## \#60 Posted by: Funktapus Posted at: 2017-12-20T04:23:56.680Z Reads: 305

```
@psychotiller You might be onto something there. How would you wire this up with a balance lead? Was the charger trying to charge one cell on its own thinking it was a group of three?
```

---
## \#61 Posted by: Hummie Posted at: 2017-12-20T04:59:50.656Z Reads: 299

```
the pic guide with them leading to the fire was classic really I couldn't help but laugh and the folding seemed the obvious answer.  but what guess will you throw in.
```

---
## \#62 Posted by: lrdesigns Posted at: 2017-12-20T06:42:18.734Z Reads: 301

```
This is just some theories based on the pics. Note the fireworks happened during charging. 

1. Red arrow, positive looks very close to negative here. 
2. Black arrow, the heat from spot welding carbonized the paper insulation. Carbonized paper can be conductive. 

<img src="/uploads/db1493/original/3X/8/0/8048ba5c2e6e1e25584f48cab6e269b4628bede1.jpg" width="690" height="278">

<img src="/uploads/db1493/original/3X/e/b/ebb354a338105fad3bc3bd970020a173cd156ffc.jpg" width="690" height="413">
```

---
## \#63 Posted by: scepterr Posted at: 2017-12-20T07:04:03.239Z Reads: 293

```
[quote="psychotiller, post:59, topic:41458, full:true"]
How does the parallel configuration work with this circled group?
[/quote]

@Quezacotl can you explain those 6 cells at the end
```

---
## \#64 Posted by: Jones_Blake Posted at: 2017-12-20T08:08:00.665Z Reads: 287

```
The line problem? It may because the electricity comes from power supply and charger overpass the highest electricity that the line can bear.
```

---
## \#65 Posted by: Maxid Posted at: 2017-12-20T08:08:54.900Z Reads: 283

```
I think he connected them in parallel on the top once folded - it's actually quite an elegant method if you think about it.
```

---
## \#66 Posted by: Sebike Posted at: 2017-12-20T08:26:08.867Z Reads: 279

```
Unless the pack is secured not to allow any movement (but also if firmly secured), I believe parallel packs not connected in series should have insulation between them (fish paper or equivalent).
```

---
## \#67 Posted by: pat.speed Posted at: 2017-12-20T11:46:47.382Z Reads: 283

```
Imagine flipping the two side up into the shape it is meant to be when complete. It forms a triangle of those three cells with the red insulator. They are then connected in series to the group of three cells on the bottom. It's a bit hard to picture in your mind but it is connected correctly
```

---
## \#68 Posted by: Quezacotl Posted at: 2017-12-20T11:48:53.300Z Reads: 291

```
@deucesdown: I remember that i charged it, took out of charging, then when another time charging, it was like few minutes and suddenly started.
And now i remember another thing! I charged it, then took out of charging so i could install the top cover and duct tape, and after that i when i charged, the catastrophe started.
But when i installed the top cover, there is a small possibility that when i secured the top cover with rivets(stapler-looking, not airplane-style), maybe some of the rivets shorted some wires accidentally :open_mouth: Most likely then the balance leads.

Those meters i have are 2-wire. Ranges from 3V to 17V, and they are accurate despite they are cheap chinese.
https://www.ebay.com/itm/DC-3-0V-17V-LED-Panel-Meter-Mini-Lithium-Battery-Accuracy-Digital-Voltmeter-BE-/121834333285?hash=item1c5de46465

@Cobber: Maybe even this would do: http://www.icharger.co.nz/icharger-1010b
I have been thinking of getting that. Just enough features for me, except would be nice to see all voltages at the same time, but i'm not paying 200 extra just for that :smiley:

@lrdesigns: Heh, your name looks like irdesigns. I hate those indifferences (Il|) :smiley: 
But you have a good point there. That's why i'm going to do double-cardboard-layer, and weld those in an angle if possible that no extra heat gets on the cardboard.

@scepterr: That circled group is just 3 in parallel.

I'll try to explain this apparently unusual configuration in picture
<img src="/uploads/db1493/original/3X/3/b/3bfaeb5588931bd5c23c924a4b19911e10e7f1d8.jpg" width="690" height="403">
10S3P configuration. Red lines indicate the connections, and green numbers are where the balance leads go. "Minus" and "Plus" are the endpoints.

Oh, and i got one stripe overnight at salt water. (focused on point where i sanded it). No rust!
<img src="/uploads/db1493/original/3X/b/c/bc4726036c9c78be508a01d2814e24590c3f2770.jpg" width="690" height="388">
```

---
## \#69 Posted by: PXSS Posted at: 2017-12-20T13:10:21.162Z Reads: 275

```
Your folds were good. You would have known immediately if they were bad. There is no such thing as shorting a cell now and it catching on fire later. 

If you had shorted a cell while folding then you would have seen sparks immediately as the hundreds of amps flow through the nickel strip. 

—-

Did you check your voltages before charging?
If I had to guess, you over charged a cell and since there was no balancing, the fire started once a cell hit thermal runaway and it made adjacent cells go into thermal runaway, starting the chain reaction.
```

---
## \#70 Posted by: PXSS Posted at: 2017-12-20T13:15:20.861Z Reads: 268

```
There isn’t much heat transfer due to radiation thus the reflection is negligible. Space ships and satellite use kapton as insulation as all the heat transfer is through radiation, and reflection is the best insulation. 

Kapton tape is actually quite thermally conductive when it comes to tapes.

Therefore in our application, Kapton tape is NOT an insulator
```

---
## \#71 Posted by: Quezacotl Posted at: 2017-12-20T13:27:41.952Z Reads: 269

```
http://www.electric-skateboard.builders/t/my-battery-pack-turned-into-fireworks/41458/31?u=quezacotl
```

---
## \#72 Posted by: Vanarian Posted at: 2017-12-20T13:33:22.766Z Reads: 263

```
Well now that's some extreme fold (didn't know it was done this way on battery packs),but in a way it makes sense to be able to fold strips like origami.

Where do you buy your cardboards insulator rings btw?
```

---
## \#73 Posted by: Quezacotl Posted at: 2017-12-20T13:35:10.013Z Reads: 265

```
https://www.ebay.com/itm/200pcs-1x18650-Cardboard-Battery-Insulators-Electrical-Insulating-Adhesive-Paper/302508198861?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649
```

---
## \#74 Posted by: longhairedboy Posted at: 2017-12-20T13:47:10.783Z Reads: 268

```
[quote="PXSS, post:69, topic:41458"]
There is no such thing as shorting a cell now and it catching on fire later. 

If you had shorted a cell while folding then you would have seen sparks immediately as the hundreds of amps flow through the nickel strip.
[/quote]

Thank you. I was sitting here having a wtf moment at all the "oh there's your short!" comment. Best case you get a loud pop and momentary short resulting in holes in your nickel, some melted heat shrink on the cells, and maybe a lost charge cycle but still usable cells with a little work. 

More likely though  that short would have wicked up into flame and broken the connection almost immediately, hopefully not taking a cell or two into ignition with it. 

In all cases it would have been immediate, loud, and startling.
```

---
## \#75 Posted by: Quezacotl Posted at: 2017-12-20T14:02:34.155Z Reads: 266

```
I came with a new assumption. Staples that i used to seal the top cover, could have penetrated the negative lead and one of the balance leads. And since it didn't trigger the effect right away, it must have been very weak short in beginning, and escalating into bigger short.
Although i always staple with good enough clearance, it is an option though.
<img src="/uploads/db1493/original/3X/4/e/4ef6a9dbd5cc0ddba06ed79665de62b3b86750bf.jpg" width="690" height="388">
```

---
## \#76 Posted by: PXSS Posted at: 2017-12-20T15:05:55.824Z Reads: 266

```
[quote="Quezacotl, post:75, topic:41458"]
it must have been very weak short in beginning, and escalating into bigger short.
[/quote]

A short is a short, there is no such thing as a little short working itself into a bigger short. 

—-
If you really want to see a short in action, you can do it safely. 
Grab an old cell and solder wires to each end and while wearing safety glasses touch the ends of the wires, you’ll see the sparks fly immediately, disintegrating either wire. 

—-

It is possible that you nicked a wire’s insulation and then while charging, you bumped into it which caused it to short. While shorted, the insulation of balance wires melts in about 10 seconds. At which point the exposed wire could have melted through adjacent wires or cells and shorted them too. 

—-

***A short is very violent***. If it was a short that triggered the fire, it was because a wire got nicked or heat shrink was damaged and while you moved the pack around, the short happened. It did not happen before the fire happened. 

***More likely*** is the situation where you over charged a single cell if you did not verify the individual voltages before charging them. In this scenario the cell’s internal resistance rises over time to the point where the cell enters thermal runaway and then it shorts internally. Starting the chain reaction
```

---
## \#77 Posted by: Quezacotl Posted at: 2017-12-20T15:15:01.698Z Reads: 254

```
Try to read what is offered to you. The voltages were monitored.
And i maybe chose wrong words. Weak short, as wiggling back and forth, and ultimately "welding-short". Just like your 3rd chapter points.
```

---
## \#78 Posted by: psychotiller Posted at: 2017-12-20T15:22:08.576Z Reads: 251

```
Yeah...I imagined that. And also all of the other packs touching together when the whole pack was folded together. Big No No.
```

---
## \#79 Posted by: longhairedboy Posted at: 2017-12-20T15:23:48.992Z Reads: 252

```
[quote="psychotiller, post:78, topic:41458"]
And also all of the other packs touching together
[/quote]

your mom's packs are touching together.
```

---
## \#80 Posted by: psychotiller Posted at: 2017-12-20T15:28:47.660Z Reads: 253

```
Your moms face is on fire!!!
```

---
## \#81 Posted by: longhairedboy Posted at: 2017-12-20T15:30:55.703Z Reads: 238

```
this is all going into my book. The fire, your face, and your mom.
```

---
## \#82 Posted by: florensvb Posted at: 2017-12-20T16:04:55.934Z Reads: 243

```
I have just built my first battery pack where i used 10 awg silicon wire. Then i covered all the connections in Kapton tape before insulating them with tape and shrink wrap. Was that a bad move or not? Do i need to be worried?
```

---
## \#83 Posted by: PXSS Posted at: 2017-12-20T16:17:25.762Z Reads: 247

```
No need to worry
```

---
## \#84 Posted by: psychotiller Posted at: 2017-12-20T16:40:21.350Z Reads: 255

```
I'll have her send more pics! <img src="/uploads/db1493/original/3X/b/8/b8724da83f56216bccd9bcbadf7327d766e97a2a.jpg" width="690" height="388">
```

---
## \#85 Posted by: scepterr Posted at: 2017-12-20T16:45:57.175Z Reads: 249

```
That's not the configuration in the picture @psychotiller highlighted though

That makes sense....the other pic doesnt

Where are those 2 triangles at the end on this?

https://www.electric-skateboard.builders/uploads/db1493/original/3X/9/d/9dab1beee749d581027065b8a6411e3a98e67255.png

Oh I think I finally got that lone cell gets added to the other 2 in parallel after it's folded?
```

---
## \#86 Posted by: Quezacotl Posted at: 2017-12-20T20:07:27.511Z Reads: 236

```
Yep. That lone foldable cell unites with those two cells on other side, making the same triangle pattern.
```

---
## \#87 Posted by: psychotiller Posted at: 2017-12-20T20:16:32.509Z Reads: 235

```
Not anymore it doesn't. :joy:
```

---
## \#88 Posted by: scepterr Posted at: 2017-12-20T20:22:24.513Z Reads: 228

```
Regardless of what/how it happened, can we all agree this is not a design that should ever be repeated again.
```

---
## \#89 Posted by: Hummie Posted at: 2017-12-20T20:25:25.790Z Reads: 225

```
 You cant  rule-out the possibility of shorting earlier.  I had a non-exciting short once when soldering a pack as two cells shorted through poor shrink wrap on their cans and the only indication was the noise of a pressure release valve opening that clued me in.   If I hadnt heard it I maybe wouldve never known and then on the charger I bet things couldve gone up.

my guess is when folding or some other physical manipulation the sharp corner of a nickel strip went beyond the small circle of the positive terminal and got to the can.
```

---
## \#90 Posted by: Quezacotl Posted at: 2017-12-20T20:30:30.617Z Reads: 222

```
What is wrong with this design? Can you point out?
```

---
## \#91 Posted by: psychotiller Posted at: 2017-12-20T20:34:07.756Z Reads: 217

```
Answer: It caught fire. That's what's wrong with it. 

Nothing left to point to.
```

---
## \#92 Posted by: Hummie Posted at: 2017-12-20T20:37:15.398Z Reads: 224

```
no one has a good answer for what went wrong and probably no answer will be found just possibilities. 

 seems you did everything right except insulate between the p groups with something...but my bets on a corner of a nickel tab getting beyond the terminal to the can.  the donuts look beat up after the spot welding and theres some sharp corners that could be bent in there.
```

---
## \#93 Posted by: Quezacotl Posted at: 2017-12-20T20:38:50.392Z Reads: 226

```
So... if i burn down world's safest car, it should never be manufactured again? :joy:
```

---
## \#95 Posted by: psychotiller Posted at: 2017-12-20T20:53:24.809Z Reads: 232

```
Meh...or keep at it. Whatever
```

---
## \#96 Posted by: Quezacotl Posted at: 2017-12-20T20:53:33.710Z Reads: 239

```
@mmaner: You are being an a$$%&le by saying that. It's the worst thing to say.

But speaking of building again, here's revision 2 in early phases. Precharging and wrapping in polyimide tape. Next phase is discharging, and the next is building the pack this time with that plastic sheet going like snake between series cells.
And then routing of cables way better.
<img src="/uploads/db1493/original/3X/b/d/bd2acb9e4c51ffb15ab41064b780b4d535bc16ba.jpg" width="690" height="388">
```

---
## \#97 Posted by: Funktapus Posted at: 2017-12-20T20:59:38.874Z Reads: 237

```
His battery design was fine. 
The fold was fine. 
The configuration was clever to the point that most of us here couldn't figure it out.
The welds were questionable.
But the fold defenitley didn't cause the short.

It seems it was either:
a bad cell,
mixed balance wires or a,
short that was made when making the enclosure.

All of which we could be guilty of at some stage.

We should give him more credit than's due.
```

---
## \#98 Posted by: mmaner Posted at: 2017-12-20T21:00:46.743Z Reads: 231

```
[quote="Quezacotl, post:96, topic:41458"]
You are being an a$$%&le by saying that. It's the worst thing to say.
[/quote]

Well, I was trying to be kind and truthful, some people don't like the truth.  Im just saying if you want the battery now, another option is to get someone who has done it a few hundred times to build you one.  Maybe if you have delicate feelings you shouldn't be talking to a bunch of skaters.
```

---
## \#99 Posted by: scepterr Posted at: 2017-12-20T21:07:34.886Z Reads: 228

```
Uhm clever it is not, there is a right way and wrong way, clever is not right in this case.

All the battery builders going "wtf" is not a good thing
```

---
## \#100 Posted by: Quezacotl Posted at: 2017-12-20T21:11:51.123Z Reads: 226

```
It is very civilized discussion here compared to many other forums. Many times people tell someone just to quit at something and then they get depressed. Well yea that is good thing to say if you are literally about to cut your hand with a chainsaw or something, but too often people just slam it to your face, "there's no point, just quit!".
I don't mind whatever people say. But just don't make it a common thing to say.
```

---
## \#101 Posted by: scepterr Posted at: 2017-12-20T21:14:24.522Z Reads: 216

```
I'll put together a pack later today using the configuration I suggested, unless you can tell me why it's not better, please use it.
```

---
## \#102 Posted by: mmaner Posted at: 2017-12-20T21:15:06.614Z Reads: 207

```
I said what I said in a kind and courteous manner, I then explained what I said in a kind and courteous manner.  Not sure what the problem is here, but whatever.  Good luck and have a nice day.
```

---
## \#103 Posted by: GrecoMan Posted at: 2017-12-20T21:15:46.888Z Reads: 208

```
he said that to try to keep you and your belongings (and family) safe...

not sure why your mad 🤔
```

---
## \#104 Posted by: Maxid Posted at: 2017-12-20T21:19:59.871Z Reads: 206

```
Guys you are being ridiculous - the configuration he used seems perfectly fine and there is no reason to blame him. I am pretty sure that what happened here could have happened to everyone of us and it is a good thing to have people tell these stories.

@Quezacotl please don't get discouraged - it seems some of us have taken this thread the wrong way.
```

---
## \#105 Posted by: GrecoMan Posted at: 2017-12-20T21:22:28.120Z Reads: 198

```
I never said the strategy was bad, just think he made a tiny mistake and led to a fire. if you decide to keep going, please make sure to insulate everything twice
```

---
## \#106 Posted by: scepterr Posted at: 2017-12-20T21:30:02.421Z Reads: 205

```
Well then I encourage you to make a pack like that lol

Come on dude, clever has its place, this isn't it

I'm not saying the OP should give up and never touch a cell again, just that there are best practices and they should be followed. 

Find 1 battery sold that looks like that or even another made by anybody that looks like that
```

---
## \#107 Posted by: Quezacotl Posted at: 2017-12-20T21:34:28.051Z Reads: 208

```
Then tell a better configuration for two layer, about square pack consisting of 30 cells as 10S3P? I couldn't think but couple of different, other as what i made and other same but all parallels as triangles.
Of course one layer is easier, or two layer long pack.
```

---
## \#108 Posted by: scepterr Posted at: 2017-12-20T21:35:45.091Z Reads: 207

```
I'll build a pack with this configuration later today, 1 fold, leads come out the same end, exterior side of the pack

<img src="/uploads/db1493/original/3X/f/5/f57f4fc2104d31d5bb6568a6cf4fd30343806719.jpg" width="666" height="499">
```

---
## \#109 Posted by: mmaner Posted at: 2017-12-20T21:36:26.999Z Reads: 203

```
<img src="/uploads/db1493/original/3X/b/1/b1cf8bfde5b41f81b198cb4303c4b2d615671e04.png" width="666" height="500">
```

---
## \#110 Posted by: Quezacotl Posted at: 2017-12-20T21:48:46.629Z Reads: 201

```
That's the same as mine. But what's with replicating it?
```

---
## \#111 Posted by: koralle Posted at: 2017-12-20T21:59:15.929Z Reads: 203

```
[quote="scepterr, post:106, topic:41458"]
there are best practices
[/quote]

is there a nice summary somewhere? There are a bunch of topics that would be cool to have in a esk8 wiki. For noobs such as me it is incredibly hard to gather some basic info sometimes as these threads tend to get really cluttered and often have like 1000 replies lol
```

---
## \#112 Posted by: scepterr Posted at: 2017-12-20T22:01:37.920Z Reads: 202

```
You can start with ebikeschool, batteryuniversity
```

---
## \#113 Posted by: Sebike Posted at: 2017-12-20T22:04:32.324Z Reads: 209

```
How I built mine. In love with fish paper. Kapton really won't protect from almost any mechanical wear though, so if a nickel strip moves, it will tear a whole in several layers of Kapton in an instant. 
<img src="/uploads/db1493/original/3X/6/e/6e61a71eae7ac44e6e200ab3e6779a3eeff28152.jpeg" width="690" height="388">
```

---
## \#114 Posted by: Funktapus Posted at: 2017-12-20T22:20:19.657Z Reads: 204

```
Too many people thought the battery shorted when he folded it. That itself says a lot about the battery builders here.
```

---
## \#115 Posted by: scepterr Posted at: 2017-12-20T22:22:23.847Z Reads: 203

```
Nobody has had to fold over a single cell to complete a P group so it was an interesting mess to  decipher
```

---
## \#116 Posted by: Mikenopolis Posted at: 2017-12-20T22:24:18.705Z Reads: 200

```
[quote="Quezacotl, post:96, topic:41458"]
You are being an a$$%&le by saying that. It's the worst thing to say.
[/quote]

Don't be dramatic. That's not the WORST thing to say. Just take it as @mmaner wanting to make sure you don't burn down your place, family, neighbors.
```

---
## \#117 Posted by: Hummie Posted at: 2017-12-20T22:30:30.010Z Reads: 196

```
it still might have shorted when he folded it or because of the fold and theres no assurance of anything that happened.  those corners of the nickel couldve come under or through some insulation because of the fold.  I think that's still the most likely reason.
```

---
## \#118 Posted by: Funktapus Posted at: 2017-12-20T22:53:04.771Z Reads: 195

```
If the fold caused the short, it would've happened imediantly. I'm not sure how you could argue against that.
It caught fire while charging. It was a fresh battery pack. 
Since it hadn't even been used yet, there's no evidence to suggest that mechanical wear caused a short either. 

The main clue is that it happend while charging.
```

---
## \#119 Posted by: Quezacotl Posted at: 2017-12-20T22:57:30.741Z Reads: 192

```
There is no folding with parallel groups, only series. But anyways, it doesn't hurt to add an additional insulation also there :slight_smile:
```

---
## \#120 Posted by: Funktapus Posted at: 2017-12-20T23:04:56.461Z Reads: 198

```
That's true. 
But just because his battery pack caught fire, doesn't mean we should automatically assume he's a simpleton. Some of the language here has been patronising.  I don't remember this type of talk when  @eboosted board caught fire. 

@Quezacotl was nice enough to share his misfortune despite any possible embarrassment so that we might learn from his mistake (assuming we can find out what caused it).

We should be helping each other and we do most of the time.
```

---
## \#121 Posted by: scepterr Posted at: 2017-12-20T23:08:21.108Z Reads: 203

```
"what" caused it is impossible to tell at this point without a video of it being built to when it caught fire. While it is a "working" configuration, meaning yes you have a 10S battery it is inherently danger and risk prone where it should not be, and it's simpler for it not to be
```

---
## \#122 Posted by: Cobber Posted at: 2017-12-20T23:13:05.664Z Reads: 202

```

https://youtu.be/u4ZgVRJ-H8U
```

---
## \#123 Posted by: Hummie Posted at: 2017-12-20T23:28:47.732Z Reads: 193

```
as I wrote abobve I've shorted a battery while building it and there wasn't anything to notice other than the sound of a pressure valve blowing and hissed in a cell.    a short can happen without you even knowing possibly...and then later could put it on a charger.
```

---
## \#124 Posted by: deucesdown Posted at: 2017-12-20T23:29:53.193Z Reads: 198

```
I'm wary of saying stuff like "don't do this, do it this way". A lot of it is in the execution and knowledge built up by making mistakes (experience). For those who are still developing the knowledge/experience, thoughtfulness and being aware of what the dangers are (failure modes) is going to really help. IMO shutting down the discussion doesn't help this.

And we're all here because we like to do things our way, right? Tweak this, tweak that, I think this could be better, etc. And we've all blown various things up.

I know I'm still relatively noob, and a ton of this stuff has been discussed endlessly in the past on endless-sphere.com, etc., so I understand some of the impatience of the old timers. And I question if I'm being naive...

I don't see anything inherently wrong/bad with OP's design. Bunch of people looked it over and agree, although they feel nervous about the unfamiliarity.

Execution, this is where we're all learning from OP's experience, I think. @Quezacotl I hope you keep at it and figure out what went wrong, and how to improve safety, or how to check things between steps to affirm things are going well.
```

---
## \#125 Posted by: scepterr Posted at: 2017-12-20T23:43:28.910Z Reads: 197

```
10s3p dual stack dual row configuration example
**Cells are not connected,not insulated, only layout example**
<img src="/uploads/db1493/original/3X/1/d/1ddd308b5a17ea0f1cb1dbd3c96caea417b573a4.jpg" width="666" height="499">
<img src="/uploads/db1493/original/3X/9/d/9d8e24640a9ed4309a916a28b87a8dcaecb66c64.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/6/66b77c719245c1cecff808d1d8061724c45b0853.jpg" width="666" height="499">
```

---
## \#126 Posted by: psychotiller Posted at: 2017-12-21T00:04:49.947Z Reads: 191

```
Nice touch with the insulation between the packs too!
```

---
## \#127 Posted by: scepterr Posted at: 2017-12-21T00:15:14.097Z Reads: 187

```
Lol I can't resist even when absolutely nothing is connected 😋
```

---
## \#128 Posted by: PXSS Posted at: 2017-12-21T00:37:58.782Z Reads: 189

```
Send me the cells and I’ll make it. There is NOTHING wrong with the design
```

---
## \#129 Posted by: scepterr Posted at: 2017-12-21T00:45:21.356Z Reads: 189

```
Lol I never said it can't be made, I can make it too, but why, when a more reliable method exists?
```

---
## \#130 Posted by: PXSS Posted at: 2017-12-21T00:45:48.242Z Reads: 185

```
Why is your method more reliable?
```

---
## \#131 Posted by: scepterr Posted at: 2017-12-21T00:46:13.081Z Reads: 185

```
Dual series links, more even current distribution, single fold
```

---
## \#132 Posted by: PXSS Posted at: 2017-12-21T01:05:48.155Z Reads: 191

```
[quote="scepterr, post:131, topic:41458"]
Dual series links
[/quote]

His pack has 3 series links. 

[quote="scepterr, post:131, topic:41458"]
more even current distribution
[/quote]
His pack current distribution is good with the exception of connections 3/5 which are on the outside where the current goes through one tab. Still not that bad...

[quote="scepterr, post:131, topic:41458"]
single fold
[/quote]

Your single fold is on the edge of the battery, with enough vibrations those tabs can break easy. 

Vs 

His fold is supported throughout by the several nickel tabs creating less strain overall. 

---

His design does not require insulation between folds. 
Vs
Yours does

---

You can find pros and cons on both designs. One is not necessarily better than the other. Just because it seems complicated, it doesn’t make it bad. 

I wouldn’t do it either way, but I am not claiming that the way I would do it is the end all be all of battery design.
```

---
## \#133 Posted by: scepterr Posted at: 2017-12-21T01:17:10.879Z Reads: 182

```
I'm no battery god lol uhm there are plenty of series connections that are single in there...only 4 are triple linked, so current draw can be quite diff between the series from one end of the pack to the other

@PXSS come on, have you ever built a pack with a hanging cell that you have to connect to it's p group after it's assembled?

I've said all I have to say on this topic, I'll just patiently wait for the next it's on fire thread
```

---
## \#134 Posted by: PXSS Posted at: 2017-12-21T01:44:16.169Z Reads: 190

```
[quote="scepterr, post:133, topic:41458"]
@PXSS come on, have you ever built a pack with a hanging cell that you have to connect to it's p group after it's assembled?
[/quote]

Yes! Plenty of times actually! I’ve also built packs with parallel groups have cells across different levels (each fold would be a new level) where I have to run a wire across two cells to connect some of the cells to the rest of the group!

You forget that I do this as a living (and somewhat hate it, which is why I dont offer to build packs for others), I have designed battery packs that are crazy but are the (what I consider) optimal configuration for the specific task. 

There is a battery pack I make that has 40 folds in a 2 level pack. I hate building it because it takes so much time but it has to be that way in order to fit the space available. 

[quote="scepterr, post:133, topic:41458"]
only 4 are triple linked, so current draw can be quite diff between the series from one end of the pack to the other
[/quote]

Looking at pictures on the first post and the one with the connections numbered on post 68:

1 - negative - 3 tabs triangle
2 - 3 series tabs (2 to the bottom cells and 1 to the top cell)
3 - 1 series tab on outside
4 - 3 series tabs
5 - 1 series tab on outside
6 - 3 series tabs
7 - 3 series tabs
8 - 3 series tabs
9 - 1 series tab on outside
10 - 3 series tabs
11 - positive with one tab

---

Again, there are spots where he does have one series tab on the outside of the pack, but they are not detrimental, especially if he doubles or triples the tabs on top of each other.
```

---
## \#135 Posted by: scepterr Posted at: 2017-12-21T01:46:29.139Z Reads: 177

```
All good, do you think this is the optimal layout for the OP, considering **his** experience level?
```

---
## \#136 Posted by: PXSS Posted at: 2017-12-21T01:55:42.278Z Reads: 192

```
No, but again, I don’t think yours is either...

In all honesty, I would do his before yours. Mainly because I would not trust the 2 tabs to survive after many vibration cycles... :smile:

***WHAT I WOULD DO*** is the same triangle pattern that you have but instead of going all the way to one side on one layer and then back on the other, I would go back and forth between the layers so that the fold is supported throughout.
```

---
## \#137 Posted by: scepterr Posted at: 2017-12-21T01:56:12.263Z Reads: 199

```
I use 1/2" copper braid for the fold, 2,3,4 pieces depending on P count
```

---
## \#138 Posted by: Hummie Posted at: 2017-12-21T02:01:45.791Z Reads: 199

```
<img src="/uploads/db1493/original/3X/9/7/97bcfe99e9bb8c2a772fc7b7fcff105b3331b348.JPG" width="666" height="500">

Dont want detach from the OP's story but how bout some criticism over here.  Ive got a pile of battery handlers here and want to see what you think.   You think this is safer or more dangerous?  the tape surely cant keep compression as long as extreme (4) rubber bands I have coming but it looks nice with the clear stretchable tape.    it's .5mm copper strip 17mm wide.  not going to cut into the insulation of a cell with no sharp edges.  With a shorter strip of copper can stack them on top of each other too and keep the exposed copper recessed.  too me its awesome and cant wait to put it on a new board with new motors.

how much copper strip you think I should put in, I read the thinner the better stacked and it contours to the cell but I'd like to see the math for current and conductivity of copper at this volume and forget it.

looking at it again here with more critical eyes the bands need to be able to get to the part they're pulling better.  that lip on the bottom really reduces what the band can do.
```

---
## \#139 Posted by: Cobber Posted at: 2017-12-21T02:17:37.421Z Reads: 190

```
Rubber bands perish with heat after a while. Maybe nitrile rubber might be better?
```

---
## \#140 Posted by: Hummie Posted at: 2017-12-21T02:20:23.058Z Reads: 198

```
https://www.aerorubber.com/all-weather-rubber-bands/
my best lead but surely there's a band out there that can do it.  even if I have to change them once a year i'll be happy.
```

---
## \#141 Posted by: Clonkex Posted at: 2017-12-21T02:39:59.875Z Reads: 196

```
[quote="mmaner, post:94, topic:41458, full:true"]
I swear I'm not being an a$$%&le when I say this, but maybe YOU shouldn't build it again.
[/quote]

Wtf. No no no no no. That's _terrible_ advice. What you're saying is, "you made a mistake therefore you should never try again". That's so incredibly dumb I can't even express it. How would anyone do anything if they're not allowed to learn from their mistakes? Are you telling me if you accidentally missed a traffic light a nearly hit another car, you'd stop driving? No, you'd learn from your mistake and be more careful in future. Geez...
```

---
## \#142 Posted by: PXSS Posted at: 2017-12-21T02:43:57.427Z Reads: 190

```
[quote="Clonkex, post:141, topic:41458"]
Are you telling me if you accidentally missed a traffic light a nearly hit another car,
[/quote]

More like t-boned the car and got lucky that nobody got hurt.
```

---
## \#143 Posted by: Clonkex Posted at: 2017-12-21T02:45:58.009Z Reads: 185

```
Either way works for my argument.
```

---
## \#144 Posted by: deucesdown Posted at: 2017-12-21T03:13:45.883Z Reads: 186

```
I think for some people @mmaner advice could be appropriate and excellent. DIY is just no good for some people. OP seems okay though.
```

---
## \#145 Posted by: Quezacotl Posted at: 2017-12-21T07:43:34.082Z Reads: 200

```
Okay now i see it how it goes with one fold. That looks actually easier and you are able to get stronger bonds between series cells, except the one fold which can of course be strenghtened.

My design has better current draw? Those designs have equal amout of squares in series(except the folded single series).

Does the vibration really matter if the whole pack is wrapped tight as hell? I've experienced that it doesn't matter as long as you make a sturdy enclosure and wrap the pack tight. Of course the stripes need to be in relaxed position, not like first weld and then pull into tight tension.

@Hummie: Is that rubber bracket only meant for protected cells? Judging from the small tab -looking hole. Or do they just need very, very good tightness? But anyways for tightening, why not use glassfiber-strenghtened tape?(forgot the exact name)
```

---
## \#146 Posted by: davidbonde Posted at: 2017-12-21T09:21:34.003Z Reads: 207

```
[quote="scepterr, post:85, topic:41458"]
Oh I think I finally got that lone cell gets added to the other 2 in parallel after it's folded?
[/quote]


I just need to understand this completely. Could anyone help me out? 

Folding it up like that makes it possible to connect the lone cell directly in parallel at the -pole. What about the +pole? I see these are connected through the next groups parallel connections through the series connection. Does that work?  To illustrated it further (maybe my explanation is not that good) it would be like doing a config shown in blue/green (green showning where there would not be a connection). Would that still make it two 3p-groups i series? 
<img src="/uploads/db1493/original/3X/e/d/ed77f654cd895dfe39696cd4e398ee1160a1ffea.png" width="652" height="383">
```

---
## \#147 Posted by: PXSS Posted at: 2017-12-21T11:05:30.439Z Reads: 199

```
Yes. It would.
```

---
## \#148 Posted by: pixelsilva Posted at: 2017-12-23T07:30:37.365Z Reads: 200

```
> @Cobber

> <img src="/uploads/db1493/original/3X/e/3/e3d4923abd35b9b56d6193b9bb4235a7f6c72f00.png" width="660" height="464"> 

Deciving electronic piece, designed like a plastic toy. Looks like a taiwanese game console from the 70's.
```

---
## \#149 Posted by: Quezacotl Posted at: 2017-12-24T18:04:03.889Z Reads: 196

```
Bah, my spot-welder is busted. It is already second time the triac blew. And with or without coincidence, a cell i was welding, started hissing because the spot-welding heated a hole in a cell...

Because of that, and because it is very bulky and cumbersome to use and not very accurate, it is time for me to get a new welder. Any suggestions? I've seen a welder that takes it's power from a car battery. I was thinking something like that.
Maybe this, unless you have something else to recommend:
https://malectrics.eu/product/diy-arduino-battery-spot-welder-prebuilt-kit-v3/
```

---
## \#150 Posted by: scepterr Posted at: 2017-12-24T19:18:12.928Z Reads: 194

```
I'm using the v3.1 Arduino spot welder, love it
<img src="/uploads/db1493/original/3X/f/9/f9635392ad11b08d25f3688bea5fa863250524ee.jpg" width="666" height="499">
```

---
## \#151 Posted by: Eboosted Posted at: 2017-12-24T19:23:34.598Z Reads: 193

```
I've used the arduino spot welder for almost 10 battery packs already, it has worked flawlessly so far, get the additional parts to avoid the avalanche current to back into the welder and bust it.
```

---
## \#152 Posted by: Eboosted Posted at: 2017-12-24T19:24:24.191Z Reads: 195

```
Did you print that enclosure for the welder or it came as it?
```

---
## \#153 Posted by: scepterr Posted at: 2017-12-24T19:33:34.098Z Reads: 192

```
Printed, file is available on malectrics, you can also buy the case from him
```

---
## \#154 Posted by: Quezacotl Posted at: 2017-12-24T23:45:54.529Z Reads: 194

```
Okay then. I'll go buy that :slight_smile:
```

---
## \#155 Posted by: banjaxxed Posted at: 2017-12-25T20:53:24.412Z Reads: 202

```
http://www.electric-skateboard.builders/t/boss-level-custom-spot-welder/25980
```

---
## \#156 Posted by: Quezacotl Posted at: 2017-12-26T00:18:57.305Z Reads: 192

```
I saw that too. Not much different from the arduino spot welder. It has better looking tip though.
```

---
## \#157 Posted by: lrdesigns Posted at: 2018-03-12T08:29:18.050Z Reads: 160

```
Any updates on the new pack, photos?
```

---
## \#158 Posted by: Quezacotl Posted at: 2018-03-12T08:59:13.933Z Reads: 160

```
Yea, i got the Arduino spot welder and built the battery.
The battery is working good. Although it feels little more lazy especially on hills than LiPo. But well, the next pack has 5 in parallel instead of 3.
![IMG_20180212_195316|690x388](upload://zxVSFad9P4gKUkvr8S0t2LjNCHc.jpg)
![IMG_20180213_144255|690x388](upload://tT6YauAZquV0zIrZqRR3uiOqpWQ.jpg)
![IMG_20180213_171837|690x388](upload://n18HL5rrwL5wAI09kCorL0xlfAT.jpg)
![IMG_20180222_154301|690x388](upload://tOnMkQIvPvzEZqfT2sKhY77Avpt.jpg)
![IMG_20180222_161929|690x388](upload://cAWyv0tBxen2k8GqROFZ4XQJoeo.jpg)
![IMG_20180222_155026|690x388](upload://JeBS7aWalehewxkcj1fuTDL5Jx.jpg)
![IMG_20180222_164938|690x388](upload://ilVGSYQyGjjaZER86SScnL6ioVx.jpg)
```

---
## \#159 Posted by: Acidfie Posted at: 2018-03-12T09:49:20.901Z Reads: 155

```
The real question here is;

Who the fuck uses cells with 10a discharge ad puts them 3 in parallel? 

That’d be 30a cont discharge.

What do you power with that? A torch?
```

---
## \#160 Posted by: bimmer Posted at: 2018-03-13T12:56:03.402Z Reads: 126

```
Jesus this battery is sketchy again.
```

---
