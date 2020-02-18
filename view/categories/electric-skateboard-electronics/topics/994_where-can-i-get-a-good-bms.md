# Where can I get a good BMS?

### Replies: 44 Views: 8314

## \#1 Posted by: barajabali Posted at: 2016-01-13T18:42:27.573Z Reads: 527

```
Anyone know where to get a bms?
```

---
## \#2 Posted by: lox897 Posted at: 2016-01-13T20:07:49.989Z Reads: 523

```
Battery Supports or Bestech Power. What pack are you using? 10s3por 10s4p?
```

---
## \#3 Posted by: barajabali Posted at: 2016-01-13T20:15:00.447Z Reads: 522

```
well i use a few different one LIPO and Li ion. most are 6s
```

---
## \#4 Posted by: lox897 Posted at: 2016-01-13T20:18:30.654Z Reads: 514

```
How many in parallel? And how many amp hours?
```

---
## \#5 Posted by: barajabali Posted at: 2016-01-13T20:51:30.426Z Reads: 489

```
Oh I won't mix the chemistries they're for different boards. But on my main board it's 22.2 volt 18 amp hour. 6 cell
And that's the lipo
Custom made
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-01-13T20:55:54.633Z Reads: 466

```
who made your pack? I'm looking for a 6S pack to replace my dead 10Ah 6S i got last year. 

I'm toying with the idea of making my own 18650 packs though. not to sell at first, but just to learn how it all works and experiment with them.
```

---
## \#7 Posted by: barajabali Posted at: 2016-01-13T20:58:38.692Z Reads: 458

```
I made them 
I can make 18650 or flat lipo cells. 
If you need any help hit me up I'm happy to help. 
I'm trying to incorporate a bms into them so that way you don't need to have a balance charger to charge them.
```

---
## \#8 Posted by: barajabali Posted at: 2016-01-13T21:04:06.111Z Reads: 441

```
You ever consider repairing you battery cell? It's prob just one cell that's bad
```

---
## \#9 Posted by: lox897 Posted at: 2016-01-13T21:40:36.823Z Reads: 440

```
One more thing. Sorry. What's the c rating of your pack?

Do this calculation: Amount in parallel x max amp output per cell = max continuous current of lipo
Then you know what BMS you need because you look for the one that has those max continuous current protection.

Let's say it was 10c (3000mah per cell) So it would be able to push 30amps per cell:
4 x 30 = 120amps
So your pack can supply 120amps.

@chaka Please correct me if I'm wrong.

You could use a watt meter and see how many amps your battery is pushing out then get a bms related to that.

EDIT: Changed the calculations. They were wrong.
```

---
## \#10 Posted by: cmatson Posted at: 2016-01-13T21:44:06.756Z Reads: 418

```
[quote="lox897, post:9, topic:994"]
Let's say it was 10c:
[/quote]

I'm pretty sure 10c is really high for a discharge rating... I'm pretty sure most (reasonable) packs aren't anywhere near that rating. 

haha maybe you are right though :smile:
```

---
## \#11 Posted by: lox897 Posted at: 2016-01-13T21:47:34.047Z Reads: 395

```
For a lipo. I think that's right.
```

---
## \#12 Posted by: barajabali Posted at: 2016-01-13T21:57:10.074Z Reads: 394

```
Yea I'm actually at 30c lol @lox897 @cmatson
I used the cells out of 2 zippy 8amp hour 6 s cells
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-01-13T22:22:47.848Z Reads: 381

```
some of these high amp hour 6S multirotor packs have like a 2C rating. has anyone used one that low?
```

---
## \#14 Posted by: cmatson Posted at: 2016-01-13T22:33:01.613Z Reads: 380

```
[quote="barajabali, post:12, topic:994"]
ea I'm actually at 30c lol
[/quote]

haha nevermind then!
```

---
## \#15 Posted by: barajabali Posted at: 2016-01-13T22:33:42.745Z Reads: 373

```
Correct me if I'm wrong but I'm pretty sure multi rotors use really high C ratings because of the nature of the device. But I think 2c wouldn't really be much of an issue for our purposes.
```

---
## \#16 Posted by: barajabali Posted at: 2016-01-14T01:42:41.816Z Reads: 370

```
@lox897  so with my stats what bms so you recommend? maybe a link if you dont mind please :)
```

---
## \#17 Posted by: lox897 Posted at: 2016-01-14T06:01:27.027Z Reads: 366

```
I think you'd get best results if you used a watt meter and tracked how many amps you are pulling. There aren't many bms that are made for more than 100 amp continuous.
```

---
## \#18 Posted by: longhairedboy Posted at: 2016-01-14T12:10:11.399Z Reads: 368

```
i saw a 2C 6S 20Ah pack on hobby king the other day and now i can't find it, just the typical 20C. maybe it was a mis-print, but they sort of discussed extending the capacity by lowering the burst output or some such nonsense. Anywhooo.. that's way off topic. Sorry!
```

---
## \#19 Posted by: oriol360 Posted at: 2016-01-14T19:12:37.263Z Reads: 368

```
http://www.batterysupports.com/battery-pcbnbsp-bmsnbsp-pcm-c-32.html

Delivery took a while.
```

---
## \#20 Posted by: longhairedboy Posted at: 2016-01-14T20:24:20.048Z Reads: 369

```
how long did it take? I was looking at that same site just yesterday.

And does a PCB like that allow charging from a laptop style charger? or do you need a full BMS for that? I'm still new to the terminology with battery stuff and i'm not always sure what i'm looking at.
```

---
## \#21 Posted by: lox897 Posted at: 2016-01-14T21:04:44.802Z Reads: 339

```
Yes, you can use it with a laptop style charger. You just solder some leads to a charge port.
```

---
## \#22 Posted by: lox897 Posted at: 2016-01-14T21:06:27.735Z Reads: 325

```
@oriol360 The thing with that site is the 22.2v bms only goes up to 60amp continuous.He can supply much more than that and it would be a waste for the bms to think that's the max he can do.
```

---
## \#23 Posted by: lowGuido Posted at: 2016-01-15T00:20:45.077Z Reads: 313

```
lets say for a moment that you were able to discharge your 8000mah battery at 100A continuous your battery would be dead in 4 mins.

I don't think anyone requires 100A continuous
```

---
## \#24 Posted by: barajabali Posted at: 2016-01-15T00:38:36.570Z Reads: 297

```
yea i agree. i bought a watt meter and ill update this thread with my actual amp drainage.
```

---
## \#25 Posted by: lox897 Posted at: 2016-01-15T00:40:56.679Z Reads: 290

```
Good idea. You would never use 100 amps continuous but if you were climbing a hill or going 35mph you could get up to 80 amps according to @chaka

And you can supply that much so why not.
```

---
## \#26 Posted by: chaka Posted at: 2016-01-15T00:58:13.413Z Reads: 277

```
@barajabali I have a few 6s bms modules, If you need one let me know and I will get you the specs. They are all from bestech.
```

---
## \#27 Posted by: chaka Posted at: 2016-01-15T01:09:08.835Z Reads: 281

```
[quote="lox897, post:25, topic:994"]
Good idea. You would never use 100 amps continuous but if you were climbing a hill or going 35mph you could get up to 80 amps according to @chaka
[/quote]

This really depends on the motor you are using. larger motors will draw more current while accelerating and could pop the overcurrent while a smaller motor would not.
```

---
## \#28 Posted by: lowGuido Posted at: 2016-01-15T01:11:06.036Z Reads: 270

```
I think the main word here is continuous. Sure a short burst of high current every now and then but to continually draw 100A?

Correct me if im wrong but doesnt the space cell have a 30A fuse?
Im not arguing,  i just think most average consumers wont need that sort of current.
```

---
## \#29 Posted by: chaka Posted at: 2016-01-15T01:27:09.802Z Reads: 264

```
Not really worth arguing over that since you are not likely to find many bms modules rated for 100 amp continuous. But you want to have enough headroom so you don't lose power crossing an intersection.
```

---
## \#30 Posted by: oriol360 Posted at: 2016-01-15T01:46:10.045Z Reads: 263

```
@longhairedboy  After ordering it took about 4 weeks for delivery. I also ordered during holiday time so that might be why it took so long. It does allow charging through a laptop charger.

I use a 6S battery with a VESC. I've never hit 60amps. However, I live in Florida so there are no hills and i've only gone up to 30mph.
```

---
## \#31 Posted by: barajabali Posted at: 2016-01-15T02:02:13.346Z Reads: 251

```
For lipo or lifepo? Can I buy one off you
```

---
## \#32 Posted by: chaka Posted at: 2016-01-15T02:06:34.467Z Reads: 248

```
If you are located in the US I can get you one. If you are abroad it might be better for you to buy direct from bestech.
```

---
## \#33 Posted by: barajabali Posted at: 2016-01-15T02:15:17.854Z Reads: 248

```
I'm in the US. Chicagoland area. 

Are they lipo bms? Or lithium iron phosphate
```

---
## \#34 Posted by: chaka Posted at: 2016-01-15T02:39:01.676Z Reads: 252

```
They are li-ion, 4.2V to 3V
```

---
## \#35 Posted by: massy Posted at: 2016-01-15T16:12:23.158Z Reads: 258

```
I'm also looking for a BMS for 2x 5s LiPo batteries making one 10s battery in series. Using a 10s BMS is it simple to get the balancing wires and so on sorted since I guess you need to merge these somehow?

Also when you say buying directly from Bestech, I have checked their site out but they don't seem to have a web shop and the highest rated BMS I can find seems to be 25A continuous.

It would be amazing if you could help clear these things up.

Edit: This one: http://www.batterysupports.com/36v-37v-42v-10s-45a-10x-36v-lithium-ion-lipolymer-battery-bms-p-266.html

would cost 44 USD with shipping to Sweden, it should do what I want fine, right?
```

---
## \#36 Posted by: chaka Posted at: 2016-01-15T16:48:07.050Z Reads: 255

```
25 amps continuous is about 900 watts, good to about 30 mph. The peak amperage on these things is much higher.  There is a lot of information out there on how the balance connectors should be connected. If you run an image search you will get some good diagrams. I would research this until you fully understand how it all works before you begin.

And to clear up any confusion, I do not recommend using a bms on Li-po packs. You really want to have many layers of protection against overdischarge and li-po cells don't have any internal fusing. You could add cell level fusing if you have the skill/time to do it but it can be a painful process if you are not geared up for it.
```

---
## \#37 Posted by: massy Posted at: 2016-01-15T17:11:33.504Z Reads: 253

```
Wouldn't adding a BMS between batteries and VESC just give me another layer of protection against discharging the batteries too much since the VESC has a cut off too or does the BMS remove the VESC's ability to sense what's going on?
```

---
## \#38 Posted by: chaka Posted at: 2016-01-15T17:45:11.824Z Reads: 259

```
Individually you would be wiring the cells in parallel and then series. Without cell level fusing a faulty cell can take a whole string of cells with or without a bms. If this is going on inside an enclosure you will be unaware and it could end up catching fire. This is one of the reasons 18650 cells are internally fused.
```

---
## \#39 Posted by: Sirshaunsta Posted at: 2017-11-30T12:11:50.321Z Reads: 86

```
Hey guys I have ordered 8 zippy 5s 5000mah batteries I plan to run them in 2 series with 4 of the sets in parallel meaning 4 10s 5000 mah batteries adding to 20 000 mah. Do I NEED a bms or can I get away without one if using xt90 connectors to hook them up and unplug for singular charging. I will be running them with 2 focbox and 2 190kv sk3s
```

---
## \#40 Posted by: Sirshaunsta Posted at: 2017-11-30T13:07:33.506Z Reads: 89

```
Another question I've decided to run with 4 motors and 4 vesc to add torque to my build in low end without sacrificing top end speeds, any ideas how to wire the 4 vescs to on reciever?
```

---
## \#41 Posted by: Acido Posted at: 2017-11-30T14:53:59.113Z Reads: 84

```
check out the build threads of awd skates
```

---
## \#42 Posted by: louwii Posted at: 2017-12-01T03:34:49.083Z Reads: 84

```
You can always use a standard balance charger and charge one battery at a time. People use BMS so they don't have to unplug the batteries each time they need to charge them. A BMS also offers a protection for battery over-discharge (but a VESC does the same thing).

I was planning on setting up a BMS on my first build, but I went for a balance charger for now, it's easier when you're not sure of what you're doing.
```

---
## \#43 Posted by: Sirshaunsta Posted at: 2017-12-01T07:37:21.301Z Reads: 77

```
Ok cause I have 2 b6s and 2 boards so I can charge 12 at a time with their own plugs. Thank you
```

---
## \#44 Posted by: Luca1 Posted at: 2018-04-27T10:02:59.446Z Reads: 44

```
You can have 90c packs but it is mostly for race drones or rc vehicules
```

---
