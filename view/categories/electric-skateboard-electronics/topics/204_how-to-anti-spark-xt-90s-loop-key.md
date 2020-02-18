# How-To: Anti-Spark XT-90S Loop Key

### Replies: 177 Views: 30106

## \#1 Posted by: sl33py Posted at: 2015-09-14T05:00:00.821Z Reads: 2108

```
It's not a marvel of engineering.  It doesn't light-up blue.  It's not as nice as the [url=product/on-off-high-voltage-anti-spark-power-switch-2-14s/]push-button anti-spark[/url], or similar (out of stock) on [url=http://www.enertionboards.com/electric-skateboard-parts/high-amp-120A-electronic-ignition-on-off-switch/]Enertion[/url].
It's also not $45-60.

This might be a bit remedial for some of you (you know who you are), but i wanted to show how i built one in case someone else wants to make their own.  You can do it easier/simpler, but i had some time to fiddle in the garage and enjoyed making it for my next build.

Starting off with the [url=http://www.hobbyking.com/hobbyking/store/__61690__XT90_S_Anti_Spark_Connector_2pairs_bag_.html]anti-spark XT-90[/url]:
[img]/uploads/db1493/original/1X/375a1ec15848725109c784346730e69bb6f44239.jpg[/img]
[img]/uploads/db1493/original/1X/a5a2c96986fc0c6a7c5233555124f7121f732895.jpg[/img]
I took some 12/2 wire i had laying around and the copper ground wire works perfectly to bridge the contacts for the loop.

I like modular.  If it ever fails or i want to do something differently i can easily swap it out without cutting it out.
6mm connectors:
[img]/uploads/db1493/original/1X/2bb690df1c85fc2397ba878f376ea90d00eaae39.jpg[/img]
The slot is so i can squeeze it to better fit/solder.
[img]/uploads/db1493/original/1X/df029d1585ecfcd3d814cd8e7312fa019162977d.jpg[/img]

Mocked up:
[img]/uploads/db1493/original/1X/d7e8ea012913f3940cb4cf12fcdf9afb2da51a5a.jpg[/img]

Finished with some heatshrink and paracord so i can easily pull to disconnect.
[img]/uploads/db1493/original/1X/89337ab1bf4ca20ff1790812f986f3fabffee9c1.jpg[/img]
[img]/uploads/db1493/original/1X/57b8c5b1ad836ba59c94a71f9c700d3321117989.jpg[/img]

Finished:
[img]/uploads/db1493/original/1X/6cd781417fc60cc2018d6e55ad562fbcf88348f7.jpg[/img]

Only issue i can imagine is depth to fit.  I will likely turn it flat and secure the bottom down.  I might also attach a small cord/wire to the paracord loop to prevent it from getting lost.
[img]/uploads/db1493/original/1X/2e1abb337962ecfa1803787f0f07be9955529444.jpg[/img]

Nothing too special, but i think it turned out well.  I plan to install on my new e-Omen (ongoing slowly).

Hope it helps!
```

---
## \#2 Posted by: lox897 Posted at: 2015-09-14T05:23:07.677Z Reads: 1846

```
Nice job sl33py looks cool! Can you explain to me a bit more on how it works? Is it kind of like an arming switch? I think psychotiller did an arming switch...
```

---
## \#3 Posted by: lowGuido Posted at: 2015-09-14T05:29:10.061Z Reads: 1801

```
also if you don't have the XT-90 anti spark connectors you can do the same thing by soldering a resistor across the connector.
I have done this with a Deans type.
```

---
## \#4 Posted by: sl33py Posted at: 2015-09-14T05:43:39.307Z Reads: 1764

```
There are tons of ways to do this - slow the inrush (which arcs and sparks).  You can add a simple momentary button and resistor like so:
[img]/uploads/db1493/original/1X/bdf73cd2e16a8e46894588e52ba905032a2490ff.jpg[/img]
You would push the button to bypass the plug momentarily while plugging in the connector fully.

Or the pre-made XT-90 anti-spark is a great all-in-one and simple option.  

On the positive connector (right side w/ green) if you look down the inside where it connects you can see there is an early contact area (also insulated from the back connector on that side) before the negative connects as well:
[img]/uploads/db1493/original/1X/b8418cb618a8c4448754f285fba27243d3aff073.jpg[/img]
It has a resistor (labeled - something like 560Ω), so it slows the inrush and suppresses the spark.  There are two "wings" or tabs on the sides which stop the plug from fully seating to allow for that inrush.  When you seat it to that stop, then push in the tabs (i usually break one off to simplify), then finally seat it fully you are done.  I've been using these inline from my batteries for a while now and really like them.  For 8-12s they work great for me!
```

---
## \#5 Posted by: lox897 Posted at: 2015-09-14T23:27:29.057Z Reads: 1588

```
Thanks sl33py. I read the thread a few more times andI think I understand it more now.
```

---
## \#6 Posted by: Talk_Bull Posted at: 2016-02-20T13:29:22.911Z Reads: 1556

```
You mentioned above that it's possible to do this with a resistor between the contacts. What size resistor would work? Also, could I use an XT60 plug instead? What's the reason for the bigger plug?
```

---
## \#7 Posted by: lox897 Posted at: 2016-02-20T20:28:42.988Z Reads: 1524

```
I think XT90 just handles more amps. The XT90's are bigger as well. An XT60 should be able to handle the amount of amps an electric skateboard draws.
```

---
## \#8 Posted by: Mobutusan Posted at: 2016-02-20T21:22:10.707Z Reads: 1479

```
Pardon my ignorance, but is this necessary when you are using a regular car ESC with an on/off switch or just for VESC's?
```

---
## \#9 Posted by: psychotiller Posted at: 2016-02-20T21:37:25.288Z Reads: 1441

```
It's a good idea to use a loop key anyway. If that switch ever fails you will drain your batteries and could very well burn your house down.
```

---
## \#10 Posted by: Mobutusan Posted at: 2016-02-20T22:10:21.199Z Reads: 1419

```
Good to know. I definitely want to avoid burning my house down. That's where I keep my skateboards. Oh, and other stuff too.

And to follow up on the question a few posts back, what size resistor would make an XT60 work for this application?
```

---
## \#11 Posted by: lowGuido Posted at: 2016-02-20T22:21:54.280Z Reads: 1372

```
I cant remember exactly what value I used.. I grabbed one at random from my pile..  I think it may have been 100ohm? i think anything between 20ohm and 1kohm would probably work
```

---
## \#12 Posted by: Mobutusan Posted at: 2016-02-20T23:21:21.824Z Reads: 1350

```
Thanks. I think I remember reading where someone had used a 50 or 100 ohm resistor, but I wasn't sure if there was a "correct" size to use.
```

---
## \#13 Posted by: lowGuido Posted at: 2016-02-20T23:24:06.606Z Reads: 1331

```
there is no "correct" size, just something to limit the inrush current a little bit so it doesn't arc. there are many values that would work, and also depending on how many caps you have in your particular build..
```

---
## \#14 Posted by: Talk_Bull Posted at: 2016-02-22T11:02:09.525Z Reads: 1331

```
@lowGuido, do you maybe have an example, or a pic of where you used this? I get the whole intermediary circuit that contains the resistor, but not sure how you would wire it so that the current flows normally (without resistance) after it's plugged in.
```

---
## \#15 Posted by: lowGuido Posted at: 2016-02-22T16:51:25.647Z Reads: 1362

```
I'll take a photo tomorrow, but I'll try to explain now.
I take a male deans connector and solder the resistor across the terminals, 
then I short the two terminals of the female deans connector with a short loop.
hook up the batteries and then attach the loop.

here's a diagram.
<img src="/uploads/db1493/original/2X/8/80652660fba24fd7ae51fd65ab5d0b89bfe32f42.PNG" width="103" height="500">
```

---
## \#16 Posted by: trbt555 Posted at: 2016-02-22T17:34:13.838Z Reads: 1299

```
Relevant:
[Anti spark bullet connector][1]


  [1]: http://www.electric-skateboard.builders/t/diy-anti-spark-bullet-connectors/950/1
```

---
## \#17 Posted by: lowGuido Posted at: 2016-02-23T07:23:49.152Z Reads: 1330

```
Photo of my diy anti spark resistor.
<img src="/uploads/db1493/original/2X/2/2d4ba2b4af1b443af46820fe1ee476102890034a.jpg" width="513" height="500">
```

---
## \#18 Posted by: Talk_Bull Posted at: 2016-02-23T15:06:33.194Z Reads: 1332

```
Thanks for all the input. Here is a picture of my loop key I just finished. I used a 680 ohm resistor, as this was the closest I had to the one used in the actual XT90s plug (I think they use a 470, or 520 ohm one).
<img src="/uploads/db1493/original/2X/9/91560d7e09939b53eaf57bc35392ac984f8b0744.jpg" width="690" height="388">

I finished it off with bullet connectors to close the loop. So to turn everything off, I just unplug the XT60 plug and can leave my batteries connected without issues.
<img src="/uploads/db1493/original/2X/c/c355bbe20179eabc3d72c309bed9a6ad57e5e8a2.jpg" width="690" height="388">
I will provide more feedback on it once I've actually tested it.
```

---
## \#19 Posted by: trbt555 Posted at: 2016-02-23T15:09:21.316Z Reads: 1291

```
Where is the resistor / how does it work ?
```

---
## \#20 Posted by: Talk_Bull Posted at: 2016-02-23T15:15:03.676Z Reads: 1308

```
If you look closely on the first pic (it shows on the 2nd too), you'll see I've soldered the resistor between the two terminals. So essentially, when you first plug it in with the bullet connector unplugged, the current will flow through the resistor (albeit at a much lower volume than without it). Once you plug in the bullet connector, current flows normally through the circuit, bypassing the resistor, since current takes the path with least resistance.

The other plug (male XT60) will be connected to the positive wires between batteries and VESC (as per the first post in this thread)
```

---
## \#21 Posted by: trbt555 Posted at: 2016-02-23T15:22:57.809Z Reads: 1245

```
Right, now I see the resistor.
So it's a two-step process, first the bullet and then the loop key, right ?
```

---
## \#22 Posted by: lowGuido Posted at: 2016-02-23T15:28:11.067Z Reads: 1263

```
first the XT60, then the bullet.
```

---
## \#23 Posted by: rasmukri Posted at: 2016-12-26T20:08:35.375Z Reads: 1037

```
Love the idea bro, I plan on building something very similar.
I have a question though, in the place where you soldered the copper cable to connect the two sides of the xt90, could I solder in a fuse instead?
Basically right now I have a large fuse online on my negative power cable before the VESC. It's 50 amps and made for a car stereo. It's just so massive and annoyingly in the way. But if I was to put a nice small fuse, like one used on vedders anti spark board, 40 amp 50v I think.  Would that work, or am I missing something in the way power travels?
```

---
## \#24 Posted by: sl33py Posted at: 2016-12-28T18:56:42.021Z Reads: 1007

```
@Rasmukri - that *should* work!  The main concern i would have is resistance and heat.

I'll see if i can grab one of the fuses i have and see how it might fit on the back of the XT90.  Neat idea.

As always - having a spare to swap (anti-spark or not) is good peace of mind.
```

---
## \#25 Posted by: lowGuido Posted at: 2016-12-28T21:33:35.383Z Reads: 975

```
I'm not sure what you are proposing will work.
a fuse and an anti spark resistor both serve different purposes.

I think you would have to put the fuse inline further down not in parallel with the resistor.
```

---
## \#26 Posted by: rasmukri Posted at: 2016-12-28T21:52:54.419Z Reads: 960

```
I cant see why it would be a problem. I mean its just closing the circuit, so instead of closing the circuit with a solid wire why not close the circuit with a fuse? Seems like putting it farther down the line would be no different. Power goes the easiest way possible and that will be through the fuse not the resistor, (after it has completed its job). I mean I'm no Engineer but I've been working on car and home wiring for quite some time. Resistors yes they always give me a bit of research before i do anything but i see no logical reason why a fused link would in any way not work. Think about it regardless of where the fuse is on the circuit the Same amount of amps will be passing through it.
```

---
## \#27 Posted by: lowGuido Posted at: 2016-12-28T22:10:19.523Z Reads: 958

```
by putting a fuse in parallel with the resistor you are changing the circuit. the fuse would still be the path of least resistance so in an over current situation it would probably still blow. but the amount of current required to blow it would change, and once its blown it would not break the circuit like a fuse is supposed to, because the resistor still completes the circuit. 
the most likely following sonario would be that the resistor would get really hot and also blow.

[quote="rasmukri, post:26, topic:204"]
I mean I'm no Engineer [/quote]
True.

[quote="rasmukri, post:26, topic:204"]
Think about it regardless of where the fuse is on the circuit the Same amount of amps will be passing through it.
[/quote]

No, no, Nope no.
```

---
## \#28 Posted by: sl33py Posted at: 2016-12-28T23:39:43.873Z Reads: 923

```
[quote="lowGuido, post:27, topic:204"]
because the resistor still completes the circuit.
[/quote]

Hey LG - are you sure?

the way the anti-spark works it is only connected at that first few mm of plugging it in... afterwards it's out of the way and not connected - right?  or is it contacting and would then become the path (and quickly blow too)?

I'm no engineer...
```

---
## \#29 Posted by: lowGuido Posted at: 2016-12-28T23:50:06.709Z Reads: 923

```

if you are using an XT90-S that is the case. but not for the ones in the image above where the resistor is in parallel.

I apologise if that's what you meant originally, I was looking at the pictures directly above with the resistor in parallel.
```

---
## \#30 Posted by: rasmukri Posted at: 2016-12-30T15:53:17.130Z Reads: 969

```
So I just got my xt90 in the mail today.
I did a resistance test and it is 6.7 at partial insertion and 1.2 (for my voltmeter .65 is a direct contact between the two leads).
So this means the resistor is not in use once the connection is full. Meaning if I put my fuse on there it should work no problem.

<img src="/uploads/db1493/original/3X/d/6/d630908d1ff52d92be5d438aa4401cf93e39df1f.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/b/c/bcf8519364849d477eaf8015d4b2fd37e66f792d.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/7/e/7eef650f26c5967bc7255e040ea8073546d08b2b.jpg" width="690" height="388">
```

---
## \#31 Posted by: lowGuido Posted at: 2016-12-30T16:01:47.891Z Reads: 924

```
[quote="lowGuido, post:29, topic:204"]
I apologise if that's what you meant originally, I was looking at the pictures directly above with the resistor in parallel.
[/quote]

Yes that should work. clearly we were both talking about different things.
```

---
## \#32 Posted by: Talk_Bull Posted at: 2017-02-01T06:44:41.853Z Reads: 906

```
Ok, I've left this way too long, but, after testing my initial loop key (with the 680 ohm resistor), I was still getting spark when connecting the bullet connectors, unless I waited long enough for the VESC capacitors to charge up (think 6-10 seconds, counting in my head every time!).

So I modified it and replaced it with a 47 ohm resistor. This way, as soon as I plug the XT60 in, the VESC lights up, then I can close the bullet connectors. PLUS, there's no spark anywhere! I'm running 9S1P if that helps anyone.
```

---
## \#33 Posted by: paulus_germanus Posted at: 2017-06-15T10:03:10.329Z Reads: 862

```
I really liked your design so I went the same way, @sl33py! :) 

Here's my take on it:
<img src="/uploads/db1493/original/3X/1/4/143d5e8ec810010ac0fc085a9a1f7604716ef2bf.jpg" width="666" height="500">

Broken off the protruding crescent moon bits and the inner plastic ridges.
<img src="/uploads/db1493/original/3X/f/e/fe48b5421da2d395891960ea6cb02d4c1b044913.jpg" width="666" height="500">

Soldered a bridge between the connectors like @sl33py did. I did it with two 2mm bullet connectors.
<img src="/uploads/db1493/original/3X/2/7/276ce0030911817aeec285672a7b1cb17e2520f0.jpg" width="666" height="500">

Pulled a bit of paracord underneath.
<img src="/uploads/db1493/original/3X/6/e/6ed79072e1c7d9484e4ecbac056c4a23b9c9ca05.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/8/3/839783f15a3d2a06ed352def101ca93243112ab4.jpg" width="666" height="500">

Shaved off about 2mm off of top of the cup and squeezed it into the connector with the paracord sticking through the opening.
<img src="/uploads/db1493/original/3X/8/2/8214064b0dfc73ce944c4446873344e7ac428aa1.jpg" width="666" height="500">

Cut off a bit of leather off a belt...
<img src="/uploads/db1493/original/3X/9/4/941ed7b575f64474488268538e3cb321b39d2f8a.jpg" width="666" height="500">

...shaped it into a tiny bone-shaped piece...
<img src="/uploads/db1493/original/3X/d/5/d5cf1d4e6e6b16ba85f81c663f423e8595df2b97.jpg" width="666" height="500">

...and squeezed it between the paracord strands and into the opening of the connector cap.
<img src="/uploads/db1493/original/3X/8/e/8e9bc4e19ca9ae41fe9feacb097cd04bb42e220a.jpg" width="666" height="500">

Voila! :slight_smile:
```

---
## \#34 Posted by: mmaner Posted at: 2017-06-15T16:48:25.576Z Reads: 812

```
I have been doing mine this way for awhile, just never thought to post it.  

I use a piece of 10g solid copper wire, bend the ends to fit tight in the XT90-S poles and then fill with solder.  Then I cut the hald circles from the cap, super glue it in place and fill with hot glue.  After its cooled some, just a little tacky, I push it in and then smooth the edges.  It looks like this.

<img src="/uploads/db1493/original/3X/d/0/d01135f763ac549f3655493b17fac8440471fbcd.jpg" width="331" height="500">

After that I print the XT90-S Fob cover, insert a paracord loop, melt the edges of the paracord together, fill the fob with hot glue and then insert the loop key.  Let it cool and your good to go...ease to insert, easy to remote, the Fob protects the loop key.

<img src="/uploads/db1493/original/3X/a/7/a799fa69eafab9646e451479b7165a0ec79d5d14.jpg" width="690" height="469">

https://www.thingiverse.com/thing:2323416

_Edit:  link to Fob files_
```

---
## \#35 Posted by: Paulf Posted at: 2017-06-15T18:05:35.341Z Reads: 796

```
<img src="/uploads/db1493/original/3X/1/7/17958d9b93ae4a66f82f166c0f3bc0c7e719406a.jpg" width="374" height="500">
This is how I'm doing mine (the red Silicon wire is just to pull it out easily, the contact is actually made with copper wire inside)
```

---
## \#36 Posted by: gliz5714 Posted at: 2017-07-28T00:38:20.302Z Reads: 770

```
How does this solder joint look on my loop key?  First time soldering in a long time.  Also - can I just wrap a piece of Paracord around that for a pull tab or not?

<img src="/uploads/db1493/original/3X/4/0/4054dccaf8d52350b7f463ea0e4fc6be6018b8dd.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/0/e048a713866eae1b9b9b5d48bc14a3f15f780dd9.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/3/c/3c67a0623ef832ed52e13436738efe4446537c4d.jpg" width="666" height="500">


Bueller.... Bueller
```

---
## \#37 Posted by: Smorto Posted at: 2017-07-28T02:31:51.611Z Reads: 756

```
Looks good, maybe more solder next time but no biggie. Yes you can use some paracord but I recommend shrink-wrapping it first.
```

---
## \#38 Posted by: gliz5714 Posted at: 2017-07-28T09:06:05.845Z Reads: 749

```
Thanks!  So I assume I should almost fill the whole semi circle with solder?  I did forget to tin them which probably didn't help.
```

---
## \#39 Posted by: Smorto Posted at: 2017-07-28T13:34:04.121Z Reads: 750

```
What you have is fine but you can just add more next time. Im not sure if you can fill the whole semi circle but just try and add a little more.
```

---
## \#40 Posted by: mmaner Posted at: 2017-07-28T14:57:44.705Z Reads: 766

```
https://www.thingiverse.com/thing:2323416
```

---
## \#41 Posted by: sl33py Posted at: 2017-07-28T21:41:48.719Z Reads: 736

```
Agree it looks good.  I like the copper to reach all the way in if possible and fill the hole more fully w/ solder.
```

---
## \#42 Posted by: gliz5714 Posted at: 2017-07-28T22:13:03.357Z Reads: 729

```
Yea, that was the intent but then while soldering it got bumped up unfortunately.  As long as it can pass the current, I'm happy!
```

---
## \#43 Posted by: jkrider Posted at: 2017-07-29T00:06:19.449Z Reads: 713

```
Is there a performance or safety difference between using copper and a 12 awg wire?
```

---
## \#44 Posted by: sl33py Posted at: 2017-07-29T20:17:22.266Z Reads: 717

```
[quote="jkrider, post:43, topic:204, full:true"]
Is there a performance or safety difference between using copper and a 12 awg wire?
[/quote]


Not really - for such a short run it should be fine.  I would definitely go as thick as you can w/ whatever you use, and keep it as short as possible.  That was the main reason i went with the solid copper - because it was direct point to point vs a loop of wire, and strong enough to then tug on w/ the paracord.  

The only time i've heard of a problem is too thin of wire and a longer loop - more heat under load = bad.
```

---
## \#45 Posted by: jkrider Posted at: 2017-07-29T22:11:03.920Z Reads: 684

```
Good to know. My loop key haven't felt hot after riding so I think I should be good.
```

---
## \#46 Posted by: louwii Posted at: 2017-11-11T22:35:22.636Z Reads: 622

```
Sorry, newbie question. The anti-spark loop key is supposed to go on the + wire, between the battery and the VESC, right ?
And it allows you to leave your battery in the board and acts like a on-off switch ?
```

---
## \#47 Posted by: m4almbergs Posted at: 2017-11-11T22:57:10.304Z Reads: 601

```
Yes exactly! If you have a bms and charge port you should put it on the + wire in between the + of the charge port and the vesc. This way you can and should pull the key out when you are charging.
```

---
## \#48 Posted by: Eboostin Posted at: 2017-11-12T00:34:27.088Z Reads: 587

```
Maybe I missed it in here, but wouldn't it be more ideal to have the female side connected to the board and use the male portion as the "key"?
```

---
## \#49 Posted by: jjalibwa Posted at: 2017-11-14T18:52:49.451Z Reads: 588

```
Are the male ends Anti-Spark or will have to re-solder the female onto my battery and the male end onto my VESC ?
```

---
## \#50 Posted by: sl33py Posted at: 2017-11-22T19:23:14.330Z Reads: 613

```
That's a good way to do it as well.  

Easier to secure the Male portion to an enclosure flush, and if the anti-spark portion of the key does get damaged (not fully seated you will melt the resistor) - a simple regular XT90 (spark!) works in a pinch and you can still ride.
```

---
## \#51 Posted by: scepterr Posted at: 2017-11-22T21:51:52.954Z Reads: 621

```
Thanks for the panel mount models, came out great

<img src="/uploads/db1493/original/3X/0/9/0988febb36c4afabd1f68af7cbcc3f51284a1c80.jpg" width="567" height="500">
<img src="/uploads/db1493/original/3X/6/a/6ac52b1bd0b378c78f47bf8f0bb853d61e23b2f3.jpg" width="531" height="500">

One tip, after port inserted, heat up the mount for it shrink a bit to the connector, makes it impossible to push out the back even without a screw
<img src="/uploads/db1493/original/3X/4/c/4c3407f750573bed68fd7d192dd461d6b1408dce.jpg" width="690" height="490">
<img src="/uploads/db1493/original/3X/7/f/7f5032273b8ab5f039d1a37d10c0e22796d0da7f.jpg" width="592" height="500">
```

---
## \#52 Posted by: ryan_pogi Posted at: 2017-11-27T19:40:31.707Z Reads: 585

```
Question, would it be possible using a fuse holder, and a 80A fuse  as an alternative to anti-spark loop?
```

---
## \#53 Posted by: mmaner Posted at: 2017-11-27T19:44:10.138Z Reads: 590

```
You'd still get a big ass spark.  The only two viable options are an anti-spark switch, anti-spark loop key or BMS with E-Switch. 

This has been exhaustively covered many many time for a couple of years now.
```

---
## \#54 Posted by: mmaner Posted at: 2017-11-27T19:45:24.437Z Reads: 589

```
[quote="scepterr, post:51, topic:204"]
heat up the mount for it shrink a bit
[/quote]

Good tip, I usually just use super glue, never have used  screws. But that's even better as you might be able to heat it for removal as well.
```

---
## \#55 Posted by: lrdesigns Posted at: 2017-11-28T01:37:57.570Z Reads: 601

```
I embedded mine in the deck. I like to use the anti-spark male shape on the deck side as its cheaper to have multiple keys that way. Just in case I loose one. With this on the side of the deck I can access it from the top or bottom in an emergency. 

<img src="/uploads/db1493/original/3X/e/7/e7d1b5b95fefb6fb7c3d0a721cf337a7359207b8.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/c/bce73682050715309381714d8dd4c2805657289b.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/9/5/958909c90fba8b4a40a8a3e2221067442bd6d129.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/a/1/a1ee0712de05979c8efd3001ed4e6d756164a32e.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/b/6/b6a2622e226e1d4104a3d5da9134dfda9e210f60.jpg" width="666" height="500">
```

---
## \#56 Posted by: scepterr Posted at: 2017-11-28T01:44:04.271Z Reads: 582

```
What if you burn out the resistor?
```

---
## \#57 Posted by: lrdesigns Posted at: 2017-11-28T02:17:32.728Z Reads: 584

```
[quote="scepterr, post:56, topic:204, full:true"]
What if you burn out the resistor?
[/quote]

:confounded: :sob: Yeah since its epoxyed in it would suck to replace. How long do these things last? If it last 1000 insertions I would be happy.
```

---
## \#58 Posted by: scepterr Posted at: 2017-11-28T02:19:13.338Z Reads: 569

```
Honestly don't know, I've seen people burn them out quick, like weeks-months, though I've never burned one...
```

---
## \#59 Posted by: ARetardedPillow Posted at: 2017-11-28T02:22:58.850Z Reads: 572

```
Ive burned through like 4-5 lol
```

---
## \#60 Posted by: scepterr Posted at: 2017-11-28T02:24:50.897Z Reads: 574

```
You are very special 😥
```

---
## \#61 Posted by: ARetardedPillow Posted at: 2017-11-28T02:33:46.526Z Reads: 553

```
And very unlucky
```

---
## \#62 Posted by: sl33py Posted at: 2018-01-04T20:26:39.052Z Reads: 559

```
Just chiming in here.  With the non-resistor Female side fixed to deck - you can use any old XT-90 male w/ or w/o resistor/anti-spark in a pinch.  

I've killed a few resistors/XT-90s and do not want to cut out and re-mount into my enclosure or deck.  

Yes the "male" w/ resistor is cleaner and less able to short, but i like the more reliable and flexible way i setup the anti-spark loop key for these reasons.

my .02
```

---
## \#63 Posted by: Sebike Posted at: 2018-01-04T21:31:25.059Z Reads: 560

```
Making it this way should work though, right

<img src="/uploads/db1493/original/3X/a/7/a75aeae32954496da9ab4753111ac06f3bf520e4.jpeg" width="690" height="388">
```

---
## \#64 Posted by: lowGuido Posted at: 2018-01-04T21:37:46.832Z Reads: 551

```
yes that will work.
```

---
## \#65 Posted by: Sebike Posted at: 2018-01-04T21:38:18.242Z Reads: 544

```
That's a nice panel mount. Would anyone with a printer in EU care to print one for me and take my money?  :yum:
```

---
## \#66 Posted by: mmaner Posted at: 2018-01-04T21:38:46.680Z Reads: 538

```
[quote="Sebike, post:65, topic:204"]
That's a nice panel mount
[/quote]

thank you :slight_smile:
```

---
## \#67 Posted by: scepterr Posted at: 2018-01-04T21:38:59.435Z Reads: 521

```
I can ship you one too 😋
```

---
## \#68 Posted by: Sebike Posted at: 2018-01-04T21:40:59.668Z Reads: 512

```
That'd be really nice! Thank you! PM me your paypal and total $
```

---
## \#69 Posted by: lowGuido Posted at: 2018-01-04T21:44:44.767Z Reads: 509

```
so long as the plug is fully inserted it wont burn out.
```

---
## \#70 Posted by: Blitz Posted at: 2018-01-05T22:32:49.905Z Reads: 507

```
Stop me if i wrong, This is just a loop key that finishes the (Negitive/orPositive) line to say the Vesc, am i missing something?

I tend to over complicate things :)

I like what you did,
Can I just Solder the cable right on instead of using 6mm gold connectors?
And can i just use my leftover Xt90 Male and female connectors?
```

---
## \#71 Posted by: Blitz Posted at: 2018-01-05T22:48:43.036Z Reads: 477

```
IS it working good I want to do the same thing as you, Also Do you Loop the positive or negative?
```

---
## \#72 Posted by: Blitz Posted at: 2018-01-05T22:57:40.789Z Reads: 481

```
Did you just only use soldering TO make the loop? no copper?
```

---
## \#73 Posted by: scepterr Posted at: 2018-01-05T23:03:38.403Z Reads: 480

```
Do some reading, you'll get more answers
```

---
## \#74 Posted by: paulus_germanus Posted at: 2018-01-05T23:11:59.439Z Reads: 494

```
I've written: [quote="paulus_germanus, post:33, topic:204"]
Soldered a bridge between the connectors like @sl33py did. I did it with two 2mm bullet connectors.
[/quote]

By that I meant that I've soldered the bridge between the connectors with two 2mm bullet connectors :stuck_out_tongue_winking_eye:
```

---
## \#75 Posted by: Sebike Posted at: 2018-01-05T23:15:04.573Z Reads: 484

```
Reading is boring and takes time. So does scrolling and clicking on the search button.
```

---
## \#76 Posted by: paulus_germanus Posted at: 2018-01-05T23:16:30.990Z Reads: 485

```
I second that :innocent:
```

---
## \#77 Posted by: Paulf Posted at: 2018-01-06T08:08:53.962Z Reads: 476

```
Yeah it's still working very good after one year, I'm looping the positive
```

---
## \#78 Posted by: TheFluffiest Posted at: 2018-01-21T09:06:06.973Z Reads: 468

```
I am having trouble with a super slow board, and wanted to narrow some stuff down... I used 14 gauge wire to do this. Will this slow current enough to affect speed?
```

---
## \#79 Posted by: Blitz Posted at: 2018-01-22T09:56:18.271Z Reads: 483

```
IT depends on the following,

What is your battery setup like,

How much does your Vesc/esc pull or draw,

loop key should be ad-least the same AWG/size as the wire anything less will become the weakest part of the chain.
(your Cable)
```

---
## \#80 Posted by: b264 Posted at: 2018-01-22T10:07:28.506Z Reads: 500

```
[quote="TheFluffiest, post:78, topic:204"]
I used 14 gauge wire to do this. Will this slow current enough to affect speed?
[/quote]

Stop after going up an especially big hill or using the most power you'd typically use --  and see if it's hot

If it's hot you should increase the size.  That goes for everything too, not just a loop key
```

---
## \#81 Posted by: DevinG Posted at: 2018-04-07T16:22:33.165Z Reads: 453

```
![20180407_101534|666x500](upload://ldavN14w5PMwV2LfFOfZyYlUU5Z.jpg)
Can anyone help me make this work?
Id like to use my series adapter to make a loop key activated volt tester. I would like to know how I would solder my vt. I am thinking on trying it like pic 2.
![15231181072212128432164|666x500](upload://yQ7D4pvz5JYgPjbAWXLHJcDauZf.jpg)
 How am I wrong? what should I be aware of? I dont want to fry anything... thanks
```

---
## \#82 Posted by: wafflejock Posted at: 2018-04-07T16:30:39.637Z Reads: 433

```
No issue with anything frying there but wondering why you would want to do this?  Is the idea to be able to measure the voltage that's coming into the right side before it gets connected to whatever is on the left side?  Guess would be good to have some idea of what you're going for in the end.

With voltage testing you just want the meter in parallel with the spots you're measuring the voltage difference between and not in series but otherwise no major issues I'm aware of really.
```

---
## \#83 Posted by: DevinG Posted at: 2018-04-07T16:33:43.635Z Reads: 431

```
i guess what i imagined was plugging my key in to complete the circuit, getting a over all voltage for my 6s setup. Im looking into getting a foc-box since my last esc wasn't the right one. so that what would bee on the right side. 2 3s lipos would be on the left.
```

---
## \#84 Posted by: wafflejock Posted at: 2018-04-07T16:36:29.554Z Reads: 430

```
Okay gotcha yeah was just having trouble figuring out what goes where in my head there... so if you want it only on when the loop key is connected would have the red wire from the volt meter going to the right side of the loop key connection so it's disconnected until the loop key is in there, if you connect on the left side then would be on all the time.
```

---
## \#85 Posted by: DevinG Posted at: 2018-04-07T16:43:52.067Z Reads: 438

```
I stuck it in there for mock purposes but is this what you mean? I was gonna cut the red on the adapter then solder the female xt90 there.

So volt meter pos goes in to pos on xt90... where to put volt meter neg?

![1523119195732281930418|666x500](upload://290A25Cyx4VLj39lBRD5VZIPhHz.jpg)
```

---
## \#86 Posted by: wafflejock Posted at: 2018-04-07T16:47:35.436Z Reads: 427

```
Anywhere along the negative lead going between the battery and ESC will be at the same voltage so would put it on either plug there (black wire in bottom right of image).

Also yes that's what I meant with the red one.

Really you could just have the red and the black hooked up to the plug on the right going to the ESC since ultimately that's what you're going after but any of the options of along the main red and along the main black going into the ESC are the same electrically (some small drop in voltage along the line aside)
```

---
## \#87 Posted by: DevinG Posted at: 2018-04-07T16:54:25.765Z Reads: 435

```
Just for confirmation that I'm picking what your putting down...
![15231198001351894110608|666x500](upload://niNmbf9gVDqtPrVtmCd5VohKuh0.jpg)

Thank you you have been most helpful. I know it's kinda unorthodox comparitavely to the first part of the thread so thank a ton  big ^^s
```

---
## \#88 Posted by: wafflejock Posted at: 2018-04-07T16:54:52.961Z Reads: 415

```
No problem also looks good to me.

Actually just reminded me I need to put a voltmeter into my modified quadcopter transmitter to monitor the LiPo I slapped on there :)
```

---
## \#89 Posted by: DevinG Posted at: 2018-04-07T17:02:32.045Z Reads: 422

```
Thanks this whole thread has been really helpful. ill probably work on this today since the weather is shit in northern colorado :mountain_snow:
```

---
## \#90 Posted by: DevinG Posted at: 2018-04-16T21:49:55.466Z Reads: 421

```
![1523915419899-285342074|375x500](upload://sBj2JuTB1b7fehwM5HVosWBJpVC.jpg)

Can I get confirmation on this? Did I loop key?
```

---
## \#91 Posted by: FredrikHems Posted at: 2018-04-16T21:54:40.251Z Reads: 409

```
You’re good :wink:
```

---
## \#92 Posted by: sl33py Posted at: 2018-04-16T22:13:07.662Z Reads: 402

```
Looks good to me!
```

---
## \#93 Posted by: GrecoMan Posted at: 2018-04-16T22:15:02.052Z Reads: 396

```
you have successfully loop keyed.
```

---
## \#94 Posted by: mmaner Posted at: 2018-04-16T22:48:53.378Z Reads: 395

```
whats the xt60 on the right side of the pic for?  It will have to be bridged for you to get NEG.
```

---
## \#95 Posted by: DevinG Posted at: 2018-04-16T23:38:48.568Z Reads: 400

```
I'm running 2 3s lipos in series as of now other wise the other neg goes to vesc-x
```

---
## \#96 Posted by: DevinG Posted at: 2018-04-17T00:29:14.864Z Reads: 406

```
Tested it and my solder is good thanks for the support! I can taste the first ride now I so close just gotta make sure my foc setting are good.....no fires fingers crossed :upside_down_face:_
```

---
## \#97 Posted by: Hatman30 Posted at: 2018-05-12T15:54:48.013Z Reads: 409

```
I made one with an 80 amp strip fuse and also used a usb flash drive top as a removable cover. It works well!
I also used a Hip flask top for my XLR charging port cover.
![IMG_7584|500x500](upload://jActmSgVBGKfqGzJXu5lkqe9rrz.jpg)![IMG_7588|500x500](upload://yxOrDgkUZnk7VYJGw5v2bCorDV4.JPG)![IMG_7589|500x500](upload://6r4KYPFL9lOmGxJBgQmmGqriJob.JPG)
```

---
## \#98 Posted by: Sender Posted at: 2018-05-12T15:57:43.081Z Reads: 399

```
That is the most adorable thing I have ever seen! I love it!
```

---
## \#99 Posted by: cypa9904 Posted at: 2018-07-07T15:26:11.926Z Reads: 367

```
May I have not on/off switch but only this anti-spark loop key and f.ex setup my vesc, ride and so on? 

Thanks for answers!
```

---
## \#100 Posted by: abenny Posted at: 2018-07-07T15:27:35.152Z Reads: 369

```
yes you can use this loop key instead of a switch, i use it on 2 boards
```

---
## \#101 Posted by: lrdesigns Posted at: 2018-12-03T01:57:35.654Z Reads: 308

```
[quote="scepterr, post:56, topic:204, full:true"]
What if you burn out the resistor?
[/quote]

I killed it, but it was user error. Vaporized one of the bullet connectors. :exploding_head: I plugged it in while i was parallel charging. :flushed::face_with_symbols_over_mouth::sob:

![IMG_1419|690x398](upload://j9CwtJjtpEDsZbuLIVvm6EUhyBV.jpeg) 

It was not that hard to replace as the glue was sort of rubbery. It was tricky to glue in the new one though, trying to keep the glue from getting into the wrong spots. 

I think people who kill the resistor early are not pushing them 100% all the way in before riding. I always made sure of that.
```

---
## \#102 Posted by: High-roller Posted at: 2018-12-03T04:05:58.589Z Reads: 311

```
[quote="lrdesigns, post:101, topic:204"]
I think people who kill the resistor early are not pushing them 100% all the way in before riding.
[/quote]

I can confirm this, happened to me my first time out. The plug wasn't fully secured so it slid a bit as I was plugging in.
Make sure to brace or secure your plugs, a glue gun works great for this.
```

---
## \#103 Posted by: VECTOR.xyz Posted at: 2018-12-05T03:52:14.512Z Reads: 321

```
Just to clarify, is it ok to leave the BMS plugged in at all times, even if you don't have an on/off switch on the BMS? So the loop key would be in between the VESC and everything else, on the positive wire.
```

---
## \#104 Posted by: b264 Posted at: 2018-12-28T05:46:10.473Z Reads: 315

```
![20181107_022656_HDR|690x345](upload://5LE6LhVFvqQRdMuKi9V7tIrAor3.jpeg) 
&ZeroWidthSpace;
![20181107_022827|690x345](upload://bAi3k4N8OsmBKs1rmau35OQv5rq.jpeg) 

![20181107_023509|690x345](upload://wtUTjkYsRuofV0x88io58RZe5UN.jpeg) 

![20181107_023836|690x345](upload://Af6gFbYgRyfTfQq4K0NZ6S8EZ8o.jpeg) 

![20181107_034359_HDR|690x345](upload://7HFIgTxQMcU06larrqwfB1aj1Cr.jpeg) 

![20181107_035219|690x345](upload://okpFIHEiyhTinl47f0e37u2Wtg7.jpeg) 

![20181107_035230_HDR|690x345](upload://v74bm4BlHMK0kUNC9faiZID8lYq.jpeg) 

![20181107_035240|690x345](upload://nUY7LGWqcwJ1Xc6N3qESlS0zjgo.jpeg) 

![20181107_035248|690x345](upload://g0Q40I7TKGRzM6CMIflB9iS2OjZ.jpeg) 

![20181108_130921_HDR|690x345](upload://ztOF4RXC0IXSwPAyqxx2zC9ogaM.jpeg) 

![20181109_162010|690x345](upload://dCzBktHlf1BuMOwsz049LbzsH2A.jpeg) 

![20181107_040257|690x345](upload://88iWYKZ4UdsyxEIhFlyshP1mTJk.jpeg)
```

---
## \#105 Posted by: venom121212 Posted at: 2018-12-28T12:52:23.723Z Reads: 304

```
What size cable braid is that boss?
```

---
## \#106 Posted by: Andy87 Posted at: 2018-12-28T12:55:04.335Z Reads: 297

```
I´m not the boss, but i can say it´s three layers of 0.25" tinned copper braid ;)
```

---
## \#107 Posted by: venom121212 Posted at: 2018-12-28T12:57:40.996Z Reads: 296

```
Thanks boss #2! Is there a specific length you shoot for to achieve a specific fuse rating?
@b264, @Andy87, or anyone else knowledgeable on the topic?
```

---
## \#108 Posted by: Andy87 Posted at: 2018-12-30T21:11:16.765Z Reads: 282

```
Just choose diameter according to the fusing current you want.
https://www.powerstream.com/wire-fusing-currents.htm
```

---
## \#109 Posted by: venom121212 Posted at: 2018-12-30T21:14:07.863Z Reads: 277

```
Bookmarked
```

---
## \#110 Posted by: b264 Posted at: 2018-12-31T04:01:36.990Z Reads: 277

```
If I wanted it to fuse, I would solder an actual fuse to it.  I made that specific one rated for 135A+ continuous because I don't want it fusing.  Ever.

I've thought a lot about this, and everyone differs, but me personally, if the board starts severely malfunctioning while I'm at-speed in heavy traffic, I would prefer the battery stay connected as long as possible so I still might have brakes to stop while the board is burning-down.  If you'd prefer the loop key fuse-out to possibly save your expensive electronics instead, that's personal preference but I'd rather have the extra couple seconds of throttle response myself.  Once it fuses, you've got no brakes.

Basically it's 
ME > BOARD
or
BOARD > ME

I prefer to give the benefit of the doubt to myself over the safety of the board/battery itself.
```

---
## \#111 Posted by: venom121212 Posted at: 2018-12-31T04:06:52.932Z Reads: 267

```
Thank you for the confirmation
```

---
## \#112 Posted by: s5300 Posted at: 2018-12-31T09:15:21.854Z Reads: 252

```

Dumb question, but how did you urethane it so well?
```

---
## \#113 Posted by: b264 Posted at: 2018-12-31T09:44:05.692Z Reads: 253

```
About 30 coats heh heh heh.  No, I'm not exaggerating.
```

---
## \#114 Posted by: s5300 Posted at: 2018-12-31T10:50:20.834Z Reads: 257

```
I mean like, did you dip it, or brush it on. 

My initial thoughts would be to dip out of a larger can, your bottle just seemed like it didn't have a large enough opening to dip it in though.
```

---
## \#115 Posted by: deucesdown Posted at: 2018-12-31T16:08:46.452Z Reads: 251

```
[quote="b264, post:110, topic:204"]
Basically it’s
ME &gt; BOARD
or
BOARD &gt; ME
[/quote]

The other angle is, if something goes wrong in storage or charging, the fuse might save your house, family, and multi-unit domicile co-inhabitants. :slight_smile:
```

---
## \#116 Posted by: b264 Posted at: 2018-12-31T20:11:04.939Z Reads: 248

```
That's why I fuse the charging ;-)
```

---
## \#117 Posted by: b264 Posted at: 2018-12-31T20:11:36.908Z Reads: 263

```
[quote="s5300, post:114, topic:204"]
I mean like, did you dip it, or brush it on.
[/quote]

For wires and loopkeys and things needing physical abrasion resistance I use

MG Chemicals Urethane Conformal Coating in the 55ml brush-on bottle

But for PCB waterproofing I prefer

MG Chemicals Silicone Mofified Conformal Coating in the 55ml brush-on bottle

except on heatsinks, then

MG Chemicals Acrylic Conformal Coating in the 55ml brush-on bottle (because it's super-thin)
```

---
## \#118 Posted by: venom121212 Posted at: 2018-12-31T20:52:32.435Z Reads: 257

```
You just put a fuse of a rating slightly higher than your charge rating on your positive charge line?
```

---
## \#119 Posted by: deucesdown Posted at: 2018-12-31T21:16:45.798Z Reads: 268

```
In general, fuses should be rated to protect the wires behind it.

In this specific case, I'd fuse at the amps of the lowest component. Usually this is the 5.5mm dc jack. Next is the BMS charge max, then usually the charge wires (both positive and negative -- it's a circuit).

Fuses have some built-in room over their rating. If you oversize your fuse, it won't kick in in time to save your parts. (this may be true even if you perfectly size your fuse)

For example, for this specific mini blade fuse: https://www.littelfuse.com/products/fuses/automotive-passenger-car/blade-fuses/327.aspx

The Time-Current Charactistics table says:
- 110% of Rating: 100h Opening Time Min
- 135% of Rating: .75sec opening time min, 120sec opening time max
- 160% of Rating: .3s/50s
- 200%: .15s/5s
and so on.

So a 5 amp fuse will happily pass 5.5a most likely indefinitely, and will allow 6.75amps for up to 2 minutes.

(sorry I've been reading about fuses again)
```

---
## \#120 Posted by: venom121212 Posted at: 2018-12-31T21:27:51.323Z Reads: 252

```
No apologies. In my head I was thinking an 8 amp charger and maybe a 10 amp fuse as a reference point so good to know. You'd think chargers would just come with a fuse built in
```

---
## \#121 Posted by: deucesdown Posted at: 2018-12-31T21:28:29.277Z Reads: 239

```
chargers usually have a fuse, protecting the charger and the mains power. :)
```

---
## \#122 Posted by: venom121212 Posted at: 2018-12-31T21:30:09.588Z Reads: 242

```
Ok that makes much more sense to me. @b264 you're referring to just fusing the charging board/port side correct?
```

---
## \#123 Posted by: b264 Posted at: 2018-12-31T21:45:13.098Z Reads: 237

```
I usually put the fuse on the negative line, but yes.  Either one.

Yes, just the charge jack on the board.
```

---
## \#124 Posted by: venom121212 Posted at: 2018-12-31T21:56:51.205Z Reads: 237

```
Do some BMS have a built in fuse? This seems common sense for charge only ones given they already know what rate they're charging. I imagine all battery makers would want to include this to protect their packs.
```

---
## \#125 Posted by: b264 Posted at: 2018-12-31T22:03:29.124Z Reads: 255

```
No BMS I have ever seen is "charge-only"

They just have very low discharge rates like 10A or less, and we don't use that port.

"Charge-only" is more how you wire it up and not how the BMS is made.
```

---
## \#126 Posted by: Customesk8 Posted at: 2019-01-04T05:14:36.443Z Reads: 253

```
![image|274x500](upload://kPQPP6KKS8qE6GRfFsLNMkPEZRt.jpeg)     

As i don't want to cut my batteries leads, if i put bullet connectors where the blue arrows are is there any downside to this or reason not to? 

and is this correct loopkey? one side goes direct to battery and the other to the vesc.

Charger cable would be soldered onto the vesc wire and then in a bullet connector

Edit: I'm aware the wiring colours don't match up but i don't see that as a concern for this
```

---
## \#127 Posted by: deucesdown Posted at: 2019-01-05T01:23:28.887Z Reads: 237

```
[quote="Customesk8, post:126, topic:204"]
is there any downside
[/quote]

More places for shorts and disconnects and loss of power due to resistance. Use big bullets.
```

---
## \#128 Posted by: Customesk8 Posted at: 2019-01-05T01:25:38.141Z Reads: 233

```
Am I better off cutting the battery wire and just going with an XT-90?

It's 4 mm bullet already so if better to use big bullets i'd need to change that anyway
```

---
## \#129 Posted by: deucesdown Posted at: 2019-01-05T01:45:58.489Z Reads: 235

```
These are the types of questions we all ponder for days. :slight_smile:

4mm is not that big. 5.5mm or bigger will have better retention. If you can use shrouded bananas like XT150 even better, but XT150 are chunky.
```

---
## \#130 Posted by: b264 Posted at: 2019-01-05T03:12:46.957Z Reads: 230

```
The XT90S with the green stripe needs to be the loopkey.  Put the male (without the green stripe) on the board.  Also put [a fuse](https://www.mouser.com/ProductDetail/576-099707.5WXN) on your charge port negative line.
```

---
## \#131 Posted by: Customesk8 Posted at: 2019-01-05T03:15:02.214Z Reads: 228

```
keep seeing mixed opinions about this - does it really matter if it's the loop or on the board?
```

---
## \#132 Posted by: b264 Posted at: 2019-01-05T03:20:32.791Z Reads: 231

```
Yes, it matters.

There are many reasons, 3 of which are

* If you accidentally don't push it in all the way and ride, the broken part that you have to replace is the "key" and not the "board" (the burnt resistor will be in the easily-replaceable key)
* It's easier to mount because you can JB Weld right to it instead of trying to leave exactly a 0.75mm gap all around it
* Your stuff is compatible with everyone else's stuff if, for example, you misplaced your loop key or needed another one or someone was giving one away for free
```

---
## \#133 Posted by: deucesdown Posted at: 2019-01-05T04:36:42.706Z Reads: 218

```
Counters :wink:
- the elecrifeid parts are male and easy to short
- the more expensive/special part is the easily lost part
- uh need a third point... looks prettier mouned to your board
```

---
## \#134 Posted by: b264 Posted at: 2019-01-05T05:40:08.696Z Reads: 210

```
Ok, Devil's Advocate.  There are cons to doing it that way, but overall you want the male part on the board :smiley:  Just look at 10 builds and you'll see 9 are that way :stuck_out_tongue:
```

---
## \#135 Posted by: Customesk8 Posted at: 2019-01-05T05:44:10.418Z Reads: 214

```
gotcha, ill try one of each then ;)
```

---
## \#136 Posted by: skatardude10 Posted at: 2019-01-05T20:02:57.256Z Reads: 233

```
I've thought about it a lot for my build... Which side to mount to the board. 

https://www.electric-skateboard.builders/t/custom-loop-key-dual/79963/2?u=skatardude10

https://www.electric-skateboard.builders/t/custom-loop-key-dual/79963/9?u=skatardude10

Burning out the resistor probably would suck if you have it permanently mounted to the board and permanently wired in. Best to find a way to securely mount a female XT-90S that's easily removable.

I just went with bullet connectors and an M4 bolt that pinches a printed clamp. Very secure, and with a couple turns of the Allen wrenches I carry everywhere, I can disconnect the XT-90S from the board by unplugging the bullet connectors.

I feel much safer too potentially having exposed female side than two male pins in a wide opening 
incase my daughter just so happens to one day find the board and start poking around with her saliva fingers and I forget to cover it.
```

---
## \#137 Posted by: deucesdown Posted at: 2019-01-05T20:54:26.824Z Reads: 240

```
[quote="skatardude10, post:136, topic:204"]
start poking around with her saliva fingers
[/quote]


Your daughter's safe either way

https://www.youtube.com/watch?v=PH28BId6BuM

Also

https://www.electric-skateboard.builders/t/how-to-fused-xt90-s-anti-spark-loop-key/16912/8

https://www.electric-skateboard.builders/t/how-to-fused-xt90-s-anti-spark-loop-key/16912/12
```

---
## \#138 Posted by: Stas74 Posted at: 2019-01-11T06:37:45.221Z Reads: 222

```
What thiccnes is this copper rod?
```

---
## \#139 Posted by: b264 Posted at: 2019-01-11T11:45:55.708Z Reads: 225

```
10AWG&ZeroWidthSpace;
```

---
## \#140 Posted by: Stas74 Posted at: 2019-01-11T18:25:46.653Z Reads: 227

```
Hmmm... what in milimiters? 4mm? 3mm?
```

---
## \#141 Posted by: Indiangummy Posted at: 2019-01-11T18:29:18.610Z Reads: 229

```
![image|539x500](upload://oVgjBS2s4QIiAX2yTh2Z1xfbZ1X.png)
```

---
## \#142 Posted by: b264 Posted at: 2019-01-11T23:17:52.741Z Reads: 223

```
2.59mm minimum diameter (if solid copper)
```

---
## \#143 Posted by: Tato Posted at: 2019-01-24T14:03:59.210Z Reads: 220

```
It makes me sad there is no xt90 version of this that i can find. [https://www.amazon.com/Amass-XT60E-M-Mountable-Connector-Multicopter/dp/B07J5H5DPP](https://www.amazon.com/Amass-XT60E-M-Mountable-Connector-Multicopter/dp/B07J5H5DPP)
![](https://images-na.ssl-images-amazon.com/images/I/51Y5-LjUBlL._SL1000_.jpg)
```

---
## \#144 Posted by: Friskies Posted at: 2019-01-24T14:26:17.308Z Reads: 219

```
US $11.03  8％ Off | 1PC For Amass XT90 XT90-S Connector Plug Holder Battery Fixed Mount Base Deck CNC Support For RC Drone Spare Parts Accessories
https://s.click.aliexpress.com/e/cWTm6e7W
```

---
## \#145 Posted by: Tato Posted at: 2019-01-25T10:25:58.331Z Reads: 209

```
Thanks bae :wink:
```

---
## \#146 Posted by: Andy87 Posted at: 2019-01-25T10:35:40.166Z Reads: 216

```
Or this

https://s.click.aliexpress.com/e/ZKq4cp4
```

---
## \#147 Posted by: Superflim Posted at: 2019-01-26T11:55:44.877Z Reads: 212

```
Hobby king has one too but it’s like 2 euros
```

---
## \#148 Posted by: Riako Posted at: 2019-01-26T14:05:33.250Z Reads: 213

```
https://www.overion.fr/wp-content/uploads/2017/09/IMG_3747redim-Copier.jpg
:wink: on almost all my build I used this one :arrow_forward: https://www.overion.fr/produit/powerswitch-overion/
```

---
## \#149 Posted by: Superflim Posted at: 2019-01-26T16:22:32.679Z Reads: 208

```
How are you sure you won’t  pull the xt 90 anti spark out of the metal?
```

---
## \#150 Posted by: louwii Posted at: 2019-01-26T20:37:23.081Z Reads: 209

```
I'm using this on my board: https://www.thingiverse.com/thing:2323422

If you use strong glue to glue the socket on your enclosure, and same for the XT90 connector in the socket, it works pretty well. I haven't had any issue. And it looks quite clean. Gave it 2 coats of mat black spray paint to match the enclosure.
```

---
## \#151 Posted by: Skunk Posted at: 2019-01-26T21:44:03.904Z Reads: 205

```
Fixed title to xt90s. i keep seeing people think xt90 and xt90s are the same thing.
```

---
## \#152 Posted by: b264 Posted at: 2019-01-28T08:16:07.111Z Reads: 198

```
[quote="louwii, post:150, topic:204"]
glue
[/quote]

Always use epoxy and never glue
```

---
## \#153 Posted by: Alex753 Posted at: 2019-01-29T20:12:42.957Z Reads: 190

```
![image|666x500](upload://drCL31YHWfQtKGWQ8STY865AkYr.jpeg)
```

---
## \#154 Posted by: xsynatic Posted at: 2019-02-10T17:36:10.679Z Reads: 178

```
Is this correct? Can Minus cause a problem because its longer compared to plus?![photo_2019-02-10_17-57-08|665x499](upload://ijffTbMPauM46R4NMyJFdMLFgWa.jpeg)
```

---
## \#155 Posted by: Mich21050 Posted at: 2019-02-10T17:38:39.127Z Reads: 176

```
Typically you interrupt the positive line using the xt90s loop key but it should be alright like that... :slight_smile:
```

---
## \#156 Posted by: xsynatic Posted at: 2019-02-10T17:41:03.093Z Reads: 178

```
Is there a difference if Minus is the loop instead of Positive?
```

---
## \#157 Posted by: Mich21050 Posted at: 2019-02-10T17:42:23.770Z Reads: 176

```
No, not really. It will work either way. It's just a personal preference.
```

---
## \#158 Posted by: xsynatic Posted at: 2019-02-10T17:43:28.002Z Reads: 179

```
alright. The fact that Minus is a tad longer compared to plus is okay?
```

---
## \#159 Posted by: Mich21050 Posted at: 2019-02-10T17:44:19.054Z Reads: 174

```
You mean the wire length? It doesn't matter...
```

---
## \#160 Posted by: xsynatic Posted at: 2019-02-10T17:48:27.336Z Reads: 175

```
Perfect.

Now comes the moment i'm afraid of. Connecting the Battery to the VESC for the first time. I hope nothing blows up.
```

---
## \#161 Posted by: venom121212 Posted at: 2019-02-10T19:06:22.629Z Reads: 169

```
Unplug the loopkey while hooking everything up!
```

---
## \#162 Posted by: Michal Posted at: 2019-04-15T21:51:53.453Z Reads: 150

```
Maybe this is a noob question, but do i need a special antispark XT-90 or will any XT-90 connector work? I found one on ebay and it's like $7 for a single pair of connectors plus $4 for shipping, $11 seems kind of expencive for a connector.
```

---
## \#163 Posted by: mmaner Posted at: 2019-04-15T21:52:47.914Z Reads: 149

```
You need an XT90-S, a standard XT90 will not lessen the spark at all.
```

---
## \#164 Posted by: SkatesontheBay Posted at: 2019-04-15T22:00:52.624Z Reads: 148

```
Your better off buying 5+ pairs. Much better price and it’s not a bad idea to have extra connectors.
```

---
## \#165 Posted by: b264 Posted at: 2019-04-15T22:05:08.935Z Reads: 150

```
Yes, you want to solder them while they are plugged together to make sure the pins stay straight while they are hot.  For this you will also need some spares.
```

---
## \#166 Posted by: SkatesontheBay Posted at: 2019-04-15T22:22:11.329Z Reads: 145

```
The exact reason^^^ I murdered a couple in my pursuit of soldering self education
```

---
## \#167 Posted by: b264 Posted at: 2019-04-15T22:23:53.276Z Reads: 139

```
I think we've all done that :smirk:
```

---
## \#168 Posted by: Michaelppainter Posted at: 2019-05-11T15:56:36.972Z Reads: 124

```
Hi anyone know a reason why I couldn't/shouldn't put my loopkey on possitive line between the two batteries in series? Will it still work to break circuit properly?
I want to be able to isolate them from eachother so I can charge independently without removing from the board...
My brain tells me it should be ok, but if anyone with more experience knows otherwise please shout out!?
```

---
## \#169 Posted by: venom121212 Posted at: 2019-05-11T16:59:40.655Z Reads: 122

```
If the loopkey is between the 2 series batteries, one of your batteries will be left "hot" to your system and will become imbalanced over time.
```

---
## \#170 Posted by: Michaelppainter Posted at: 2019-05-12T09:27:27.147Z Reads: 121

```
So power can be drawn from a battery when it's negative lead is disconnected? Is that because the system is connected to the negative of the other battery?![battery|340x499](upload://2o4wapC4XYpAh53ygwavhMKc59D.png)
```

---
## \#171 Posted by: visnu777 Posted at: 2019-05-12T09:33:56.198Z Reads: 117

```
It will work out and is quite an elegant solution for using a dual 5/6s charger on both halves of the battery pack. Never thought about it... Edit: after some thought the synchronous charging might not work so you won't gain any benefit compared to the common way. You'd need to separate the halves on both poles to make it work.
When I want to charge my two halves at the same time I'll get a polarity error when I connect the second part. It works with two separate chargers though...
```

---
## \#172 Posted by: venom121212 Posted at: 2019-05-12T11:28:17.918Z Reads: 115

```
Oops nope I was picturing your setup differently. Not sure what I was thinking at the time. Disregard my comment.
```

---
## \#173 Posted by: Michaelppainter Posted at: 2019-05-12T12:04:35.589Z Reads: 121

```
Cool that's what I was thinking- put a charge port and balance port on each half of the pack, pull out the loop key, n charge with two chargers
```

---
## \#174 Posted by: Michaelppainter Posted at: 2019-05-12T12:53:02.347Z Reads: 114

```
No worries I made it more complicated than I needed to ! Thanks for your help
```

---
## \#175 Posted by: deucesdown Posted at: 2019-05-13T17:54:13.753Z Reads: 105

```
One thing that happened to me, with a BMS in the system, when breaking the series connection via loopkey between packs, the BMS completed the circuit via the balance leads. VESC still had power. Still scratching my head a bit... I quickly moved the loop key to the end of the pack.
```

---
## \#176 Posted by: Michaelppainter Posted at: 2019-05-14T06:05:58.483Z Reads: 101

```
Ah good point I'll avoid that then! To be honest part of the reason for doing it this way was so I didn't need a BMS to charge a 10s pack - I could just separate them with loop key and charge each 5s group ndividually with my IMAX B6. So in this case balance leads won't be connected to anything except when charging, and even then they won't connect the two packs together.
Thanks for the heads up though!
Mike
```

---
## \#177 Posted by: b264 Posted at: 2019-05-14T06:17:00.727Z Reads: 99

```
[quote="Michaelppainter, post:168, topic:204"]
Hi anyone know a reason why I couldn’t/shouldn’t put my loopkey on possitive line between the two batteries in series?
[/quote]

Yes, because you won't be able to charge your board.

[quote="Michaelppainter, post:168, topic:204"]
Will it still work to break circuit properly?
[/quote]
 Yes

[quote="Michaelppainter, post:168, topic:204"]
I want to be able to isolate them from eachother so I can charge independently without removing from the board
[/quote]

You should probably just add a tiny BMS and a charge port.

[quote="Michaelppainter, post:168, topic:204"]
My brain tells me it should be ok, but if anyone with more experience knows otherwise please shout out!?
[/quote]

It'd be okay if you're using a hobby charger on one battery at a time, but I can never recommend hobby chargers for esk8.
```

---
