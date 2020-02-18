# Powell Peralta - Kevin Reimer Samurai Skateboard Deck (12s5p)

### Replies: 20 Views: 2497

## \#1 Posted by: Brad Posted at: 2017-06-12T14:22:19.412Z Reads: 424

```
Ok, finally getting the battery done, so may as well start up my build thread. This thread will be a bit slow as I wish to take it easy because this is my first DIY attempt.

Parts I will be using (enough to at least see if everything is in working order)

•	Alienware VTC3 trigger remote
•	2 Trampa VESC 6.0
•	Torqueboard 218mm trucks
•	Torqueboard V4 mounts and clamp
•	Powell Peralta - Kevin Reimer Samurai Skateboard Deck
•	60 Samsung 30Q’s in 12s5p configuration
•	Ollinboards antispark/switch/fuse
•	Servo Y split
•	83mm Evolve wheels
•	97mm Abec 11 75a wheels
•	Trampa 33t wheel pulleys
•	2 Maytech 6355 sensored motors
•	6s-14s Cycle satiator charger

Parts still to get

•	Battery/vesc enclosure
•	T-90 connecters
•	10 or 12 AWG silicone wires
•	Heat shrink wraps
•	18 AWG or thereabouts for balance lead
•	Maybe some more pure nickel strips

I was not sure which way to go for batteries, Li-po or Li-ion, but decided to go Li-ion first and see how it goes. If the sag is not reduced enough to an acceptable level, the enclosure screw spacing is large enough to go for Li-po if I wish to in the future. Also Li-ion is thinner.

After doing some online research about LI-po, I learned that 60c,75c,90c etc is bogus. There is no law to stop companies from slapping fake “c” ratings on the side of their products. 

For example, the 2s2p 7200mah 90c battery from [SMC](http://www.smc-racing.net/index.php?route=product/product&path=67_64&product_id=397&sort=p.price&order=DESC&limit=100) should produce an Amax of 324, which is not the case at all. It would only be able to achieve a “c” rating of just 36.6! That means it can only do continuous Amax discharge of 131 amps.  

To SMC's credit, they are one of the very few to be honest with their products. I cannot find their page explaining why they put 131Amps on their product page but it is there somewhere.

The true Amax at "c" is 131amps. The advertised 90 "c" is just in comparison with what other companies put on their products.

No wonder a lot of people complain about puffing because they thought the “c” was what the product was, which is not. 

Li-po still have better Amax discharge than Li-ion by a large margin, but no where near the advertised “c”.

Here is the calculations of my 12s5p 30Q battery pack. Max motor amps will be limited to 30amps for a combined Amax of 60. I worked out the "c" of a 30Q which is just a mere 5!

<img src="/uploads/db1493/original/3X/7/c/7c0283f0a2face18c2ddce9bf99cf49d5ae43730.png" width="690" height="414">

I had someone else make the battery pack for me and I will do all the rest myself. Below is the image of the pack that will power my board. I have not picked it up yet, but did request a photo taken so I have an idea of what work he did on it.

I’m somewhat concerned about the cuts and what appears to be mild burn marks on the batteries. I’m sure it is just superficial but if any of you think it is not, please say so. I will have to do the soldering of the tabs myself

<img src="/uploads/db1493/original/3X/5/3/530a7b47c8d4cdbff5df7dc0c5f6762d1db699f3.jpg" width="690" height="388">

That pack in the photo is actually four separate parts. A pair of 2p on both sides and a pair of 3p in the middle. I think I will be using nickel strips and solder them to the tabs at the end. Also solder 10AWG wires black and red on the other end. Would that be ok or do I also have to make sure that each series is also connected in parallel instead of just the two ends?

I will update this thread tomorrow afternoon with pics of all the other parts I will be using. Just really need to talk about the battery as I'm not fully confident that I know what I'm doing.
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-06-13T04:14:58.904Z Reads: 371

```
[quote="Brad, post:1, topic:25176"]
Here is the calculations of my 12s5p 30Q battery pack. Max motor amps will be limited to 30amps for a combined Amax of 60. I worked out the "c" of a 30Q which is just a mere 5!
[/quote]

I like what you have going on.  In Li-ion cell terms, the "C" rating does not apply. Only constant and max amperage specified by Samsung for the 30Q in your case. I can tell you for sure to not limit your motor max to 30 amps. It's not what you think. The current draw from your battery is different when output to the motors. Personally,  I'd worry about how I'm not going to break my knee with the voltage you will be running which is very good for bombing uphill fast. 

Here's my ride data with a VESC 4.7 using Samsung 25R 10S5P. You'll have to focus more toward the end of my ride. This is going up an 8% incline. Amperage draw from the battery was flatlined at 11 amps. Motor was 33 amps. There is a more technical and lengthy answer. I noticed motor amperage is not shown on the data, but it is in the app. You'll have to trust me on this.
https://metr.at/r/qJ67Y
```

---
## \#3 Posted by: Brad Posted at: 2017-06-13T12:23:27.497Z Reads: 349

```
I turned on motor current in the drop down list and can see it just fine. So does that mean motor amps is 3 times the battery draw amperage? 30 battery amps = 90 motor amps? (assuming about 3x due to 11 battery and 33 motor that I see in your metr app) I find that interesting. Funky maths!!!

I really wanted to set the limit for a combined 90 amps meaning 45max per motors but did not want to go over the 75amps battery continuous limit. Also knew not to go past 80% of max discharge for longer battery life, but if what you say is true, then that would make everything a lot easier!

<img src="/uploads/db1493/original/3X/e/e/eeb2a6eb1e281425bf563c2c90b13d732aa8c24b.png" width="690" height="461">

Here is the pic of all the hardware and electronics. Motors are Maytech 170kv. The bullets on the motors are way too big for the vesc 6.0

<img src="/uploads/db1493/original/3X/6/2/62b8929539173a19e45d3479210875e69685ce5f.JPG" width="405" height="500">

Also hall sensors are very small compared to vesc 6.0

<img src="/uploads/db1493/original/3X/e/f/ef2c4949ff6bf9bd77076a773c1a2896a19cd417.JPG" width="616" height="500">

<img src="/uploads/db1493/original/3X/8/2/822976582f988de202b470dfd07fb3cbe84d4986.JPG" width="586" height="500">

Very nice Abec11 pulleys from Trampa but way too thick. Will have to get someone to lathe off 4mm. Spokes a bit too wide but I suppose that is so it can fit on Abec11 clones.

<img src="/uploads/db1493/original/3X/b/6/b6af402e3e928017904ac7b98e505ec1427520bf.JPG" width="393" height="499">

A demonstration on how small the Alien Power VTC3 trigger remote is. Very comfortable and light! Based on the GTB 2 and has a range of 100 meters.

<img src="/uploads/db1493/original/3X/1/5/15ee20233db17d1d58bf226d700191fda2d538b4.JPG" width="581" height="500">

Torqueboard's 218mm trucks

<img src="/uploads/db1493/original/3X/0/0/004f0e2725161a13ec7d75f303cb88312ab83146.JPG" width="690" height="355">
```

---
## \#4 Posted by: mccloed Posted at: 2017-06-13T15:40:54.969Z Reads: 306

```
Looks like you've got a good amount of parts. :grin: You'll need an adapter for the sensor plug to work with the VESC6 diy-electric-skateboard-kits-parts/vesc-sensor-wires/
```

---
## \#5 Posted by: chuttney1 Posted at: 2017-06-13T17:20:57.590Z Reads: 310

```
[quote="Brad, post:3, topic:25176"]
I turned on motor current in the drop down list and can see it just fine. So does that mean motor amps is 3 times the battery draw amperage? 30 battery amps = 90 motor amps? (assuming about 3x due to 11 battery and 33 motor that I see in your metr app) I find that interesting. Funky maths!!!

I really wanted to set the limit for a combined 90 amps meaning 45max per motors but did not want to go over the 75amps battery continuous limit. Also knew not to go past 80% of max discharge for longer battery life, but if what you say is true, then that would make everything a lot easier!
[/quote]

My suggestion is based off reading users who post why they are not getting the performance they hoped for with the VESC. Most of it is in the programming of the settings. For me, I can't push my VESC 4.7 at 12S otherwise I get a DRV8302 error. You can with yours. VESC 6.0 does solve the DRV8302 issue. There should be a battery max amperage setting when you configure your VESC to prevent drawing more current than necessary.
```

---
## \#6 Posted by: Brad Posted at: 2017-06-14T03:53:48.301Z Reads: 264

```
@mccloed Thanks for the link. I wish to keep clutter to a minimum so will ordering JST-PH on it's own and do the attaching of the wires. Will also order a pair of each JST-PH slots available on the VESC 6.0.

Do not need even more parts than I already have! :stuck_out_tongue_winking_eye:

@chuttney1 Yes I'm aware about the limitations of the older 4.7. Will keep that in mind when I get around to configurating the VESC 6.0. I reckon the config part will be kept to a minimum, just amps for both motor and battery, brake adjustment, cutoff setup and speed limit at the start to test if everything is working as intended and that is all.
```

---
## \#7 Posted by: Lionpuncher Posted at: 2017-12-28T02:19:02.986Z Reads: 237

```
 So did this build ever get completed? Looks like it'd be such a nice build!!! Thinking about the Brian Essert deck for my next build....
```

---
## \#8 Posted by: Brad Posted at: 2017-12-29T20:35:14.496Z Reads: 238

```
No. I was going to use my 97mm FlyWheels on this board, but there has been a change of plans as soon as I found out that ABEC11 was selling those new [107mm SuperFly wheels](http://www.abec11.com/archives/2107). 

Those wheels are too big for the board, so I ordered a Caldera board from Red Ember Boards (Treenutter). 

Won't have to use any risers at all and it has a sweet 1" drop.

<img src="/uploads/db1493/original/3X/d/4/d40b0ad9461f7fb6930b1eb6da822e6c9f896ff1.jpg" width="500" height="500">

Still waiting to receive the board as Treenutter is still setting up international payments on his website. Another reason for the delay is the DieBie BMS of which I received just before Christmas.

Also an engineering business was all booked out till mid January next year for custom made bolts that is 55mm long for the caliber precison trucks to fit [MetroBoard's 36t pulleys](https://metro-board.com/shop/pulley-insert-for-abec-11-flywheels/). 

I will also get them to reverse engineer the Evolve GT enclosure into a .part file, so it can get edited later on to the correct dimensions and to round out the edges, etc. 

Never thought I would go to all this trouble just over a board in as little as two years ago...

I will make a new thread when I get around to it, as there will be no more changes in plan :slight_smile:
```

---
## \#9 Posted by: Lionpuncher Posted at: 2017-12-31T02:59:08.491Z Reads: 209

```
I dig your tenacity man! Looking forward to seeing the build!
So are you just ripping around on this thing without motors then?
```

---
## \#10 Posted by: Brad Posted at: 2018-01-03T19:14:52.856Z Reads: 197

```
Naw.

I do not push. Will sell it later on.
```

---
## \#11 Posted by: Powadangaboards Posted at: 2018-04-01T19:13:47.754Z Reads: 159

```
do you have the dimensions of this battery pack please?
```

---
## \#12 Posted by: Brad Posted at: 2018-04-01T20:17:21.292Z Reads: 153

```
40.25cm x 18.25cm

Length includes nickel strips.

Unfortunately the Caldera deck EFP is incorrectly stated and was also incorrectly confirmed as 25" when it is really 23". Was going to make do with it, but concluded that 23" is just too small as I was already aware that 25" was gonna be very tight.

I will be selling this Caldera and the Kevin Reimer board soon. (Only in Australia)

Got the perfect board from Subsonic that has a wheelbase of 28" and 35mm / 1.4" drop whilst allowing wheel size up to 5 1/2 inches with no wheel/rail bite via static testing. Could use 6 shooter pneumatic wheels if I want to.
```

---
## \#13 Posted by: Powadangaboards Posted at: 2018-04-01T20:34:32.796Z Reads: 140

```
was this flat back or stacked on top?
```

---
## \#14 Posted by: Brad Posted at: 2018-04-01T20:35:04.026Z Reads: 140

```
Flat back. I prefer the slim look. 

It is in the pic with the pink battery on the board at top of this thread.
```

---
## \#15 Posted by: Powadangaboards Posted at: 2018-04-01T21:07:01.067Z Reads: 133

```
thanks bro :) i am having a fully waterproof enclosure designed for up to 12s5p packs :slight_smile:
```

---
## \#16 Posted by: Brad Posted at: 2018-04-02T03:34:32.006Z Reads: 124

```
Looking forwards to seeing your finished product.
```

---
## \#17 Posted by: Gromok Posted at: 2018-04-02T08:30:54.085Z Reads: 108

```
Are you designing for personal use or planning to open shop?
```

---
## \#18 Posted by: Gromok Posted at: 2018-04-02T08:37:45.432Z Reads: 116

```
I can hardly think of a better board than the Brian Essert deck for smaller wheel electric skateboards.

It has a nice 27" wheelbase meaning you could also go for flat 11s5p and with a kick tail to boot.

If you do not mind, can you start a build thread if you get around to it.
```

---
## \#19 Posted by: stormboard1 Posted at: 2018-04-02T18:59:26.181Z Reads: 105

```
finally a waterproof enclosure i really hope this works for us peeps with crappy weather
```

---
## \#20 Posted by: Powadangaboards Posted at: 2018-04-03T05:19:26.617Z Reads: 94

```
It’s for personal use with he plan to offer for purchase, need to fully test before selling :)
```

---
