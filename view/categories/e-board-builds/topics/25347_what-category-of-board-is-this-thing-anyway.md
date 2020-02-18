# What category of board is this thing, anyway?

### Replies: 58 Views: 4564

## \#1 Posted by: MysticalDork Posted at: 2017-06-14T04:45:29.340Z Reads: 560

```
So, a year or so ago, I built my first esk8. It was a hackjob start to finish; oversized motors and battery, janky wiring, ugly DIY fiberglass enclosure, all on a cheap crappy Amazon longboard deck. The 6374 motors meant I had to go dual diagonal, and thus came all the issues with that. Despite all that, I greatly enjoyed the build (when I wasn't tearing my hair out over it :P ) and I had a lot of fun riding it. 

Then it was stolen. I never got it back.

Fast forward 8 months or so, and I just had to get back on the horse, which leads to this build log. I tried to address all the issues I had with the first build, and I think I did pretty well overall.

**Feature list:**

6" pneumatic wheels, because the roads around here are crap.
Caliber 50 degree 184mm trucks with custom axle extensions to fit the big wheels
Custom CNC'd and welded motor mounts
Dual sealed sensored 6355 motors from @JLabs 
10s4p INR18650-25R battery pack with 80A BMS
Custom LED headlight, soon to be taillight as well
A cheap drop-through bamboo/ply combo deck, nice and rigid, with good wheel clearance (Still had to remove some extra to get decent clearance)
Initially I had dual DIYES Vesc-alikes v4.12, but I ended up blowing the DRV8302s on the maiden ride. I then managed to shoehorn in dual VESC6s, which are gorgeous by the way.

Some photos showing parts as they arrived:

Motors, lens for the headlight, bullet connectors and a big sheet of Kydex:
<img src="/uploads/db1493/original/3X/f/3/f3598aa28099cad4ddb251fcf2db497e274492fd.jpg" width="689" height="388">

The LEDs. The long skinny ones are for the tail llight (and possible underglow, we shall see) and the hexagon ones are the high power white for the headlight:
<img src="/uploads/db1493/original/3X/3/c/3c75a34e3c70a434497037a4d7a1297a42e04575.jpg" width="689" height="388">

Voltmeter, LED drivers, A RC relay (remote light switch using GT2B 3rd channel), a button (installed but currently unused, planned to be used to enable/disable underglow), and lots of screws and nuts:
<img src="/uploads/db1493/original/3X/f/8/f85daefc85193c751c097c54bc333181b88df01c.jpg" width="689" height="388">

Deck!
<img src="/uploads/db1493/original/3X/1/3/1305078e54f64c1d2da65969d1b22e3c705b8604.jpg" width="281" height="500">

Thread inserts:
<img src="/uploads/db1493/original/3X/c/6/c681b59996c1f4e24a5b13ca5da277ce4adfc742.jpg" width="689" height="388">

The wheels took some machining to get something that wasn't monstrously too wide and unwieldy, as well as some custom adapters to allow the standard 8mm(5/16") truck axles fit the 1/2" bearings.

Two-piece hubs as they arrived, with spare batteries to for scale:
<img src="/uploads/db1493/original/3X/c/8/c8e6b7a8cb6eed5b064aa9c8fd469e2fba05eb82.jpg" width="689" height="388">

After machining:
<img src="/uploads/db1493/original/3X/9/3/93eb72e23d9fb13d64342b2ebda1b5a0297c08de.jpg" width="689" height="388">

Front hanger with wheels: 
<img src="/uploads/db1493/original/3X/b/2/b2902ed5e8352c3942b7e4f70fb981b029a60244.jpg" width="689" height="388">

Here you can see the axle extensions I came up with:
 <img src="/uploads/db1493/original/3X/e/f/efbb7ba7bdbd3fa50d323656dc69d6696da809bf.jpg" width="689" height="388">

Custom LED headlight: Single Cree XHP50 running at 12v and 700mA, with elliptical beam pattern lens. 
Pro tip: Blue Permatex threadlocker causes polycarbonate to crack:
<img src="/uploads/db1493/original/3X/1/2/12726c33162e6fd46d309a75fa6ba5c07f148c50.jpg" width="281" height="500">
Designed to mount under the front truck:
<img src="/uploads/db1493/original/3X/a/b/ab594d0d9fd1d599c005b61a2a814874b36133de.jpg" width="689" height="388">

I decided to mount the motors behind the trucks because I was a little tight on space underneath:
 <img src="/uploads/db1493/original/3X/4/7/47ea5251f5cbc0e0d75116d9f1ad4cc84c6726bb.jpg" width="689" height="388">

Many batteries, much danger:
<img src="/uploads/db1493/original/3X/9/f/9f37b86a246c0852e915441e80bf6e5605e08f7b.jpg" width="689" height="388">
<img src="/uploads/db1493/original/3X/9/d/9d203cbb597be92261d18df214a1e76813913953.jpg" width="689" height="388">
Add one BMS:
<img src="/uploads/db1493/original/3X/6/5/658045ed5a70ad4120f3c4e8334f8eddcfe371c9.jpg" width="689" height="388">

Much careful soldering later:
<img src="/uploads/db1493/original/3X/0/9/090c16c02682365c5caae4aa6fcb0ce963b7d825.jpg" width="689" height="388">

Quick mock-up to see what size cover I'd need: 
<img src="/uploads/db1493/original/3X/2/a/2afb2d0cd34771b744f899d7ebd3729fe3da00b4.jpg" width="689" height="388">

Thermoformed Kydex enclosure, very nearly too tight to fit everything: 
<img src="/uploads/db1493/original/3X/a/d/ad4a1ce460037b718cd0024dbc746ad8941a5264.jpg" width="689" height="388">

Grip tape:
<img src="/uploads/db1493/original/3X/a/6/a6d6dc49b29814b500e259ee285c8f18aae3180f.jpg" width="689" height="388">

Near-final assembly (I have since routed a channel for the LED wires and embedded them with hot glue):
<img src="/uploads/db1493/original/3X/6/0/60345d7913a0dc68ee13f3ec73d08461a8ffc90b.jpg" width="689" height="388">
<img src="/uploads/db1493/original/3X/4/6/469874466f6a3f29c19001c3af0ccfd198a4e21d.jpg" width="689" height="388">

It's not **_DONE_** done, but it's rideable. I still need to figure out some kind of handle, it's heavy to lug around at around 22 pounds (10 kilos), as well as finishing the tail lights and possible underglow.

Any questions, comments, suggestions or recommendations are welcome!
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-14T10:57:47.091Z Reads: 471

```
Awesome! How did you make that enclosure? Sick build dude!
```

---
## \#3 Posted by: Decdog Posted at: 2017-06-14T13:42:53.435Z Reads: 462

```
I think he used kydex. 

[quote="MysticalDork, post:1, topic:25347"]
Thermoformed Kydex enclosure, very nearly too tight to fit everything:
[/quote]
```

---
## \#4 Posted by: 1Q-Ford Posted at: 2017-06-14T13:50:35.370Z Reads: 440

```
Great looking build dude👍🏾
```

---
## \#5 Posted by: anorak234 Posted at: 2017-06-14T13:57:03.478Z Reads: 420

```
WOW!! This is one hellofa build! You should consider selling your machines wheels as I'm sure they would gain plenty of attention!
```

---
## \#6 Posted by: ACIN Posted at: 2017-06-14T14:02:40.758Z Reads: 408

```
Cleeaan!
Two questions:
Since you went for the big grippy rubberwheels - what is the torque like? Do you think you found the right balance between torque and speed within your motors, gearing and wheels?
```

---
## \#7 Posted by: jga Posted at: 2017-06-14T14:24:18.761Z Reads: 402

```
Amazing! I also have a couple of questions:
. what is the size of the Kydex sheet you used? And how did you manage to heat it up (it does not look it would fit in a conventional oven...)?
- I am interested by the axle extension on your trucks. Can you develop a bit how you did that?
Thanks
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-06-14T14:50:20.204Z Reads: 403

```
@Smorto I made a positive mold out of MDF in the shape of the electronics, and a negative mold out of Harbor Freight foam floor mat to push the Kydex into shape around the MDF. I made a frame to hold the Kydex, then stuck it in the oven for a few minutes until it was soft. I then sandwiched the Kydex between the molds and stood on it for about 20 minutes while it cooled. Once cool enough to hold its shape, I used a paint stick and a heat gun to fine-tune the shape and get better definition where I needed it.

@ACIN I've been riding it very gingerly, but so far I think it has torque to spare. The gearing results in a top speed around 25mph.

@jga The Kydex was 12"x24" and was just barely large enough. I decided to make a frame for it to keep it from contracting as I molded it, otherwise I think I would've run short. It was just big enough to fit in our oven with about 1/2" to spare.
The axle extensions are basically just tubes, with a 5/8" inside and a 1/2" outside, The inside has threads at one end to match the skateboard axle, and the outside has threads on the same end to take a 1/2" nut. The opposite end has a little flange to let the bearings sit up against them. Here's a rough cad model, the final design is a bit different. <img src="/uploads/db1493/original/3X/6/0/602f4e1d2594aa0428b836392ecaa792cf640988.png" width="690" height="388">
```

---
## \#9 Posted by: Smorto Posted at: 2017-06-14T16:06:07.010Z Reads: 358

```
Awesome, do you have pictures of those? Looks like a great way to make a kydex enclosure.
```

---
## \#10 Posted by: MysticalDork Posted at: 2017-06-14T16:20:34.678Z Reads: 357

```
I don't, sorry. I made a huge mess in the garage during the build and I already threw them away during the cleanup. The foam is only really good for one use anyway, the heat causes it to compress and not spring back. Later I can come up with a drawing or something to clarify, but I'm at work right now.
```

---
## \#11 Posted by: wmj259 Posted at: 2017-06-14T16:25:09.393Z Reads: 349

```
What did you machine off the wheel as it looks the same in the not assembled and assembled picture after that, unless that is the final product?
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-06-14T16:41:24.456Z Reads: 324

```
Admittedly not the best angle to see. Basically the hub was a lot wider where the bearings go, so I removed about half an inch of material on each half and then re-bored the bearing seats so they were closer together. I'll add a better photo and a sketch later.
```

---
## \#13 Posted by: MysticalDork Posted at: 2017-06-15T02:08:15.136Z Reads: 344

```
Here's a [PDF](http://files.andymark.com/LayoutPrints/am-2469+6in+pneumatic+wheel+hub+assembly.PDF) with drawings of the unmodified wheel hubs, as you can see the hub extends quite a ways out past each of the tire flanges. This results in a very stable and strong wheel because the bearings are widely spaced, which distributes forces and minimizes leverage, but means you'd need crazy-wide trucks or extensions. I took off about 1/4" on the inside (towards the truck) and 1/2" on the outside. This gives about 1.45" between the outside bearing face and the inside bearing face, and I made the axle extensions to fit.

@Smorto Here's where I got my idea: http://www.electric-skateboard.builders/t/thermoforming-a-kydex-battery-enclosure/8642
I did it a little differently, I cut out a hole in the foam that matched the shape of the wood mold, to allow it to take the shape better, and would reduce the force required to compress the foam, since I didn't build a press and instead simply relied  on my own weight.
```

---
## \#14 Posted by: MysticalDork Posted at: 2017-06-15T04:04:57.088Z Reads: 334

```
UPDATE: I took it out for an evening ride to see how the headlight works (It works pretty good!) and as I was coming up the hill to my house, I noticed that it felt distinctly sluggish compared to last time. When I got off, I did a general inspection and found this: <img src="/uploads/db1493/original/3X/5/e/5e487b466512b4db96e258ac941ac18f584bf0f6.jpg" width="689" height="388">

@JLabs you want to weigh in on this? This motor has only seen maybe 10km and no crashes or similar trauma. Any idea where I can get a replacement shaft?

On a brighter note, it appears this board can climb my hill respectably even with one motor disengaged from the wheel, with 40A battery current and 60A motor current (each)
```

---
## \#15 Posted by: markyoe Posted at: 2017-06-15T06:35:47.270Z Reads: 315

```
Where did you find such a big sheet of Kydex?
```

---
## \#16 Posted by: JLabs Posted at: 2017-06-15T12:43:37.330Z Reads: 311

```
I have to say, I haven't seen that before.. I'll work on gettinf you another shaft and some more set screws. I have a shipment coming soon.
```

---
## \#17 Posted by: MysticalDork Posted at: 2017-06-15T16:13:46.495Z Reads: 295

```
I got it from a seller on Amazon. 

@JLabs thanks man! I really appreciate it!
```

---
## \#18 Posted by: JLabs Posted at: 2017-06-15T16:15:13.215Z Reads: 292

```
Yeah no problem, I'll take care if it or replace the motor. 

Please PM me so we can communicate further.
```

---
## \#19 Posted by: stealth71 Posted at: 2017-06-17T12:44:40.698Z Reads: 288

```
If you're in the US knifekits.com carries a bunch.

@MysticalDork Nice build.
```

---
## \#20 Posted by: MysticalDork Posted at: 2017-08-16T05:37:42.166Z Reads: 271

```
**Update** the wheels I'm using have started to show signs of stress cracking around the bearing seats. I'm planning to replace them with either Psychotiller's awesome 6x2 SixShooter wheels, or maybe the 7" Evolve wheels.
```

---
## \#21 Posted by: overint Posted at: 2017-08-16T06:46:14.669Z Reads: 267

```
Hey @MysticalDork, just wondering what thickness kydex you used?
Thanks!
```

---
## \#22 Posted by: Vanarian Posted at: 2017-08-16T09:50:07.659Z Reads: 261

```
That enclosure is like super clean, looks like a factory made one with your screen and stuff.
```

---
## \#23 Posted by: flywithgriff Posted at: 2017-08-16T11:51:59.177Z Reads: 259

```
What is the shafts size for the wheels you are using? They look considerably larger than the 8mm truck axles. If you remove them you will have wheel bite issues. Why not order a set of mbs rockstar II's and source the pulleys from @idea? This would have you on good quality wheels and pulleys for about $200.
```

---
## \#24 Posted by: MysticalDork Posted at: 2017-08-17T01:35:27.986Z Reads: 250

```
@overint I used 0.080" kydex.

@flywithgriff The wheels have bearings for a 12mm (Or 1/2", I don't remember) shaft. I made my own axle extensions/sleeves to fit.  I'm trying to avoid going much larger in diameter for two reasons, wheel bite and ride height, I'm trying to keep the board as low as possible. The wheels I have are slightly side-set, so I may indeed have issues with the evolve wheels. I'm strongly considering @psychotiller's sixshooter wheels which are also side-set, which should make up for the extra width. 

If I do run into pulley/mount issues, it'll just give me another excuse to redo my motor mounts to raise them up off the ground a little more, which I need to do at some point anyway.


Thanks @Vanarian!
```

---
## \#25 Posted by: MysticalDork Posted at: 2017-09-01T06:05:51.033Z Reads: 252

```
now that I've got some swanky slightly-used sixshooter wheels, and since (of course) my current motor mounts don't fit with the new wheels, I'm designing new motor mounts, this time clamp-type instead of welded, to avoid this kind of thing in the future. At work I have access to a bunch of "scrap" (cutoffs from a larger project) 3/8" aluminum plate, so I'm going to try to make as much of the mount out of that as possible. Since 3/8" isn't enough width to give good clamping stability, I'm planning to bolt two pieces together where the mount meets the truck, to give me a 3/4" wide clamping area. Here are some screenshots of the cad drawings as they stand currently: <img src="/uploads/db1493/original/3X/6/f/6f7cf4d3f66e2331ec187ab64722a811e28a22a7.png" width="690" height="388"><img src="/uploads/db1493/original/3X/b/f/bf61650deb3c553252e1255fff9dc1f907155191.png" width="690" height="388">
```

---
## \#26 Posted by: MysticalDork Posted at: 2017-10-12T16:35:08.197Z Reads: 233

```
Some updates on the mounts: the main arms are done, I've finished one core, and I'm contemplating just ignoring the secondary clamp. We'll see how rigid it is without it. <img src="/uploads/db1493/original/3X/5/a/5af510f1c7f270da1b655e8eb04385ee54e7da84.jpg" width="689" height="388">
<img src="/uploads/db1493/original/3X/8/e/8e1c484b382298ab22703910eca681bbbabb9963.jpg" width="689" height="388">

Yo @GrecoMan check this out.
```

---
## \#27 Posted by: Clonkex Posted at: 2017-10-13T03:01:46.985Z Reads: 218

```
Where did you buy your Vesc6? I think if I were to invest in a Vesc I'd want the 6 to avoid the (apparently very common) DRV failures of the 4.
```

---
## \#28 Posted by: MysticalDork Posted at: 2017-10-13T03:04:12.969Z Reads: 219

```
Straight from Trampa. I was one of the beta testers, so mine were a little discounted. Still a good chunk of change though. 

Absolutely worth every penny.
```

---
## \#29 Posted by: MysticalDork Posted at: 2017-10-28T23:38:28.991Z Reads: 217

```
Finished board with new mounts, finished tail light and some dirt on the grip tape. <img src="/uploads/db1493/original/3X/9/4/9426e8ed95ad8574b3abc23aaaef7237ec38d8e7.jpg" width="689" height="388"><img src="/uploads/db1493/original/3X/6/f/6f9914a4f41b78032ce60f7febfaed909f40ab7d.jpg" width="689" height="388">
```

---
## \#30 Posted by: GrecoMan Posted at: 2017-10-28T23:40:23.198Z Reads: 209

```
ooohhh post pics of the new mounts
```

---
## \#31 Posted by: MysticalDork Posted at: 2017-10-28T23:44:47.668Z Reads: 211

```
<img src="/uploads/db1493/original/3X/b/f/bf4e5484d391ae4bee47dc0dd430b89aae199ac8.jpg" width="689" height="388"> there's the arms, I don't think I have pix of the whole thing.
```

---
## \#32 Posted by: GrecoMan Posted at: 2017-10-28T23:45:32.083Z Reads: 204

```
damn.
next time you take them off... 😉
```

---
## \#33 Posted by: MysticalDork Posted at: 2017-10-29T08:08:42.303Z Reads: 199

```
I'll get pictures tomorrow of them on the trucks.
```

---
## \#34 Posted by: Acido Posted at: 2017-10-29T09:15:11.147Z Reads: 197

```
How much did you pat the pneumatics,i found ones for 40$ but they are just too thick
```

---
## \#35 Posted by: MysticalDork Posted at: 2017-10-29T17:37:34.765Z Reads: 195

```
They're @psychotiller's Sixshooters, [available here.](https://psychotiller.com/product/6-billet-wheel-hubs) They're a little steep, but rock solid.
```

---
## \#36 Posted by: psychotiller Posted at: 2017-10-29T21:09:44.315Z Reads: 178

```
Your build turned out great!!! Good job man
```

---
## \#37 Posted by: mmaner Posted at: 2017-10-29T21:51:32.671Z Reads: 175

```
Love the grip tape design. I've managed octogons  and racing stripes, nothing that elaborate though. I even tried to build a 2d laser cutter, about burnt my house down 😀.  Did you use a knife and ruler or some other method?
```

---
## \#38 Posted by: GrecoMan Posted at: 2017-10-29T22:21:16.726Z Reads: 179

```
I could use the schools laser cutter and ship some grip tape with your mounts lol 😉

but seriously, if you want me to, i’m down
```

---
## \#39 Posted by: mmaner Posted at: 2017-10-29T22:35:49.152Z Reads: 183

```
I appreciate it, but I'm still trying to figure out a system.
```

---
## \#40 Posted by: GrecoMan Posted at: 2017-10-29T22:36:51.810Z Reads: 183

```
good luck!

i bet your local maker space has a vinyl cutter you could use.  not sure if that would cut griptape but it’s worth a try!
```

---
## \#41 Posted by: pixelsilva Posted at: 2017-10-29T22:44:34.790Z Reads: 182

```
One of the most original grip tape designs in this forum, right there :astonished: :point_down:

<img src="/uploads/db1493/original/3X/1/b/1b130e6c1c575a0f7facd499f6d0220b0d2d3e7e.png" width="689" height="388">
```

---
## \#42 Posted by: pixelsilva Posted at: 2017-10-29T22:47:05.200Z Reads: 174

```
Question # 1
 Them 6355 motor specs? Impressions?  :point_down:

<img src="/uploads/db1493/original/3X/3/f/3f848d7fb3932f27fd998f5f85daa2d54fc5b094.jpg" width="689" height="388">
```

---
## \#43 Posted by: mmaner Posted at: 2017-10-29T22:47:40.425Z Reads: 174

```
The most local one to me is 3 hours away. I've read that vinyl cutters don't work, it dulls the blade too quick and the grip residue is harmful to the tiny roller motors.
```

---
## \#44 Posted by: GrecoMan Posted at: 2017-10-29T22:48:11.825Z Reads: 167

```
dang you must live in the boonies!
```

---
## \#45 Posted by: mmaner Posted at: 2017-10-29T22:48:30.659Z Reads: 171

```
Podunk Alabama, right here 😀
```

---
## \#46 Posted by: pixelsilva Posted at: 2017-10-29T22:51:17.966Z Reads: 175

```
Question # 2
What's the reason for the six holes on this rims? wheel pulleys? :point_down:

<img src="/uploads/db1493/original/3X/1/4/14766c8598eb70980495e8fc71d982424f4a3ed9.jpg" width="689" height="388">
```

---
## \#47 Posted by: mmaner Posted at: 2017-10-29T22:55:18.061Z Reads: 172

```
Most 60t or 72t pulleys have 6 mounting slots.
```

---
## \#48 Posted by: MysticalDork Posted at: 2017-10-30T02:02:43.986Z Reads: 183

```
Damn guys, I go and do something else for ONE day, and my thread blows up! 

@mmaner I used a ruler and pencil to draw it out on paper first, then used some spray adhesive to stick my paper template to the grip tape, and used a utility knife to cut it out. I cut it out before sticking it to the board.

Thanks @pixelsilva, I appreciate it! I had a lot of trouble coming up with a design that was "me" you know? I ended up with this one, which I like because it looks like the waveform a BLDC motor runs on, as well as a kinda Celtic knotwork type thing.  

The motors came from @JLabs, and as far as I know, they're pretty much the same as what he's selling on buildkitboards.com, minus the logo on the side. I'm very happy with them. I had one of my belts **WAY** too tight at first and broke one of the motor shafts off, but that was my error, not the fault of the motor.

The wheels I used at first were designed for robotics (FIRST, or battlebots, etc) and those were the standard mounting holes that their pulleys etc use. I just copied the pattern when I was machining my pulleys.

Speaking of pulleys, when I swapped from those wheels to psycho's sixshooters, they came with 60t pulleys instead of 72, so that brought my gearing down a little more, and increased my top speed from ~24 to ~28mph. Still has plenty of torque for hills though :smiley: 

Here's a shot of the mounts @GrecoMan: <img src="/uploads/db1493/original/3X/c/f/cfcf526727ad01e37d522fce25060d0491c26ead.jpg" width="689" height="388"><img src="/uploads/db1493/original/3X/a/4/a42c3e7ed602a8b1eeddf26701ee517f3899225f.jpg" width="689" height="388">
```

---
## \#49 Posted by: GrecoMan Posted at: 2017-10-30T02:11:16.872Z Reads: 169

```
DAYUM those are sexy mounts!

5 stars on yelp!
```

---
## \#50 Posted by: pixelsilva Posted at: 2017-10-30T02:34:46.154Z Reads: 174

```
**GrecoMan** so flattered and humble...

https://m.popkey.co/024033/K03l0.gif
```

---
## \#52 Posted by: pixelsilva Posted at: 2017-10-30T02:50:54.064Z Reads: 175

```
Mystical, I'm intrigued by your motors. By the numbers they seem a bit in between 50xx and 6374s, but how big they really are? Like that they are short length, that saves a lot of headaches with short truck widths. Could be an options for my build if my chinese motors end up being to large to fit between my future mount installation.

By the way, the grip tape design really look celtish or nordic.
```

---
## \#53 Posted by: MysticalDork Posted at: 2017-10-30T05:45:48.684Z Reads: 174

```
Yeah, they're the same diameter as a '74 but they're only ~55mm long (excluding the shaft ofc) That makes them a perfect fit for 10" trucks.
```

---
## \#54 Posted by: ATLesk8 Posted at: 2017-11-01T00:44:13.992Z Reads: 174

```
I have the same motors...theyre 6355s<img src="/uploads/db1493/original/3X/7/2/72d2a5c40fa76162443724c199306256ef920555.jpg" width="690" height="388">
```

---
## \#55 Posted by: MysticalDork Posted at: 2017-11-12T01:33:18.485Z Reads: 159

```
Due to some interest from the Esk8 Lights thread, here's some more info on my lighting setup: I'm using LDU48 (or LDU56) led drivers, one for the headlight and one for the tail light. They're good for up to 60v input, and can provide up to 48(or 56) volts output to the LEDs at constant current. They're available in various current options, and I'm using a 150mA for the tail, and a 700mA for the front. They can drive as few as one LED, or as many as can be put in series and still have their combined forward voltage be below the battery voltage.

They allow PWM dimming, which I'm taking advantage of using an Adafruit Trinket microcontroller to allow me to have high beams/low beams, and tail lights/brake lights, using input from the receiver. @Clonkex helped me out immensely with the code side of things.

The headlight LED is a Cree XHP35 (12v forward voltage) running at 700mA,  with some nice TIR optics.
The tail light is a red COB module with 16 leds in parallel (2.7v forward voltage) running at 150mA.
```

---
## \#56 Posted by: Okami Posted at: 2017-11-25T21:25:28.844Z Reads: 131

```
Hi!  Very nice board you've made! I got interested in the original wheels you used. Did you order the tires from aliexpress? As about the hubs of the first version - did you printed them somewhere or there is a shop where to order them?

Otherwise very resourceful build log! .. a lot of things to learn from you :) grip tape design sure is nice and Im also impressed with axle mod :)
```

---
## \#57 Posted by: MysticalDork Posted at: 2017-11-25T21:47:23.934Z Reads: 137

```
Thanks for the question! The hubs are from [Andymark](https://www.andymark.com/product-p/am-2469.htm) and the tubes and tires came from monsterscooterparts, [here](http://www.monsterscooterparts.com/6x114-angle-stem-scooter-tube.html) and [here.](http://www.monsterscooterparts.com/6x125-pneumatic-tire.html)

You can get the same tubes and tires for cheaper on aliexpress etc, but I was impatient, so I paid a little more to have them sooner.
```

---
## \#58 Posted by: DEEIF Posted at: 2017-11-26T00:07:25.082Z Reads: 128

```
Hey nice build mystical I was wondering if u took the extension off when u got the sixshooters
I’m in love with the grip design
```

---
## \#59 Posted by: MysticalDork Posted at: 2017-11-26T00:08:24.347Z Reads: 129

```
Yeah, the sixshooters have 8mm bearings. No need for the extensions.
```

---
