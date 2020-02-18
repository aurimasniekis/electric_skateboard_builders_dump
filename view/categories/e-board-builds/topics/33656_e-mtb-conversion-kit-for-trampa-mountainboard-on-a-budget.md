# E-MTB conversion kit for TRAMPA Mountainboard on a budget

### Replies: 30 Views: 4665

## \#1 Posted by: hahne Posted at: 2017-09-21T16:47:09.780Z Reads: 368

```
I bought a Trampa mountainboard with the objective of creating an E-MTB. I'm pleased to report that the journey from start to finish is almost complete, as I am only missing non-essential components (lights, etc). :slight_smile: 

<img src="/uploads/db1493/original/3X/2/c/2cd4524f6ed92625dbb70d908c484c86f15d4319.jpg" width="375" height="500">

I was inspired to do this project when I saw the amazing builds that @Nowind was creating. His direct-drive setup is the most beautiful mountainboard that I have ever seen (and I still REALLY want one!). Unfortunately for me (at least in this specific scenario), I live in Canada, and the currency conversion rate ensures that my bank account would be obliterated by international purchases. And so, I bought a 3d printer, and began my journey to DIY convert my new Trampa MTB into an E-MTB.

I went through a few iterations of just about every single 3d printed part, but I think I have nailed down the formula. I printed all the parts in PLA, which is very stiff, but can be brittle. Due to these properties, I tried to keep the load bearing parts relatively thick. So far, all the parts have held up extremely well, even after 100km and some minor offroading. I will start experimenting with other materials in the near future.

<img src="/uploads/db1493/original/3X/1/3/13a1c7934e8ecdda6e18bec48e3b9930b3cc0a4f.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/c/2/c2577f5ab1e42de76172415991de5570edc25f0d.jpg" width="666" height="500">
These are the front and back pictures of my wheels spacers. They hold the sprocket to the wheel. They are incredibly strong!

<img src="/uploads/db1493/original/3X/c/3/c309e2287fff2a700041adef2fdba8a3ba562190.jpg" width="666" height="500">
Failed print of 2nd part of the 1st generation motor mount. The infill network inside keeps the parts very light.

<img src="/uploads/db1493/original/3X/9/b/9bee443f437534681acf4bc42d5989d4ddb26958.jpg" width="666" height="500">
this is the completed 1st part of the 1st generation motor mount. it clamps on to the truck very easily.
I have updated and improved the entire motor mount assembly since these two pictures, and I will upload pics or videos of how they work as soon as they are printed. I am also going to adapt this system for 63mm motors.


**PARTS:**

ELECTRONICS:
Motor: [2x 5065 270kv](https://www.aliexpress.com/item/New-Arrival-Brushless-Outrunner-Motor-N5065-270KV-1665W-For-DIY-Electric-Skate-Board/32793724521.html?spm=a2g0s.9042311.0.0.tEWNAp) 
ESC: 2x Hobbywing MAX6
Battery: [2x Turnigy Multistar 6s 10,000mah batteries](https://hobbyking.com/en_us/multistar-high-capacity-6s-10000mah-multi-rotor-lipo-pack.html) (in parallel)
Transmitter/receiver: I used my phone as the transmitter, but I am working on a remote now. Receiver is an Arduino Nano with custom code, paired with an HC-05 bluetooth chip

CHAIN DRIVE: gearing 4.9:1
2x #25 59t Sprocket 
2x #25 12t Sprocket
2x #25 chain 
3D printed motor mounts/wheel-sprocket spacers for SuperStar Hubs. Chain tension is easily adjustable at any time.

**SPECS:**

Top speed: 54km/h 
Range: 24km (with a safe 20% remaining in the battery)
Motors: 2000w each (claimed by the company that I purchased them from)
Breaking: Regenerative
Weight: 29lbs or 12.9kg

Most of the high cost of an E-MTB is unavoidable. The electronics, chain-drive, and the board itself get to be quite expensive. I am, however, pleased that I could save several hundred dollars by 3D printing all the parts that I needed to connect the conversion to the board (wheel spacers/motor mounts/electronics case).
 
I am going to add lights, as well as braided wire sheaths and zip-ties to clean up the wiring. This is what the build looks like so far! 

<img src="/uploads/db1493/original/3X/7/1/71df9a902bfcaab7151ae4dd38e772375d19e758.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/3/4/34c08af72acd9a36c7a0faf47793599bc6f76a9f.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/d/5/d58a31c1dbaee42d27d3dba1f6a25593dae8879f.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/f/8/f823638c2ba4167f1b088035280ab9ee2910ff39.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/7/3/73cf82cecf3e488719cfeb769f291f08e020dc89.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/5/555dd104dfa0f70beec12b67a754429c79d8bce5.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/0/f047ec8a58dba4eeb1d12f545f8bb2820ed2ae47.jpg" width="666" height="500">

Looking forward to feedback! :slight_smile:
Ryan
```

---
## \#2 Posted by: Okami Posted at: 2017-09-21T18:00:30.048Z Reads: 282

```
Nice fabric bag. I also got one, only in black.and not from same material. A while ago i spotted koreans also using such bags for their builds.. so interesting to see a few more.builds.incorporating this feature :)
```

---
## \#3 Posted by: hahne Posted at: 2017-09-21T18:16:40.671Z Reads: 281

```
Yeah I took inspiration from them too! I really like the look of it, as opposed to the hard plastic cases. I was scared that the plastic cases wouldn't conform to the curve of the board properly, or that it might rattle on the board. (I HATE rattles! :joy:)
```

---
## \#4 Posted by: Okami Posted at: 2017-09-21T18:33:20.466Z Reads: 271

```
Yeh, it sure elimates rattles but it might slide back and force, how did u secure the bag? Didnt see much details about how u might have done it.

Cool thing u also witnessed their builds.. i dont even remember anymore how i came up with the korean forum but it was mentioned somewhere or a picture lead to.the forum
```

---
## \#5 Posted by: hahne Posted at: 2017-09-21T18:40:38.817Z Reads: 242

```
I bought a bunch of adhesive velcro strips, put some on the top of the board and some on the bottom of the bag. The bag also has all these loop things that are found on tactical vests (I got the bag from an army surplus store), so I ran some stretchy velcro straps around the board and through the loops. It fit perfectly! and I can tip the board up vertically or upside down and the battery pack wont budge :slight_smile:

I saw it on this YouTube channel called Crazy RC. His board is pretty amazing too! and I think he somehow waterproofed it.
```

---
## \#6 Posted by: Okami Posted at: 2017-09-21T18:43:16.140Z Reads: 235

```
Clever / nice use of straps and velcro.
Yeh i remember crazy rc too. He had some crazy custom.made.mounts  / metal parts too, if i remember correctly

I had more trouble with my bag at first though, i tried to secure it just with some rope, so to speak. But the rope always got a bit loose or it was a bit too hard to properly tighten it, in end i just reinforced the bag sideways with some belts, the ones u might use for jeans lol but it worked better than just ropes and was easier to adjust. 

I assume straps, which can be adjusted and connected with the bag in some way would be the best.

As about the motors u use. Nice to see that your speed might be such high with 6s packs.. when i built mine i took 192kv motor as the rest on hobbyking was out of stock, even though i wanted to get the 245kv for higher top speed. Well at least i have more headroom now (also a bit more cooling / heating room comparing the two) but i still think now that i could have used smaller.motor amd basically 6374 might be a bit of over engineering. Especially for light off roading and city terrain

So yeh just my thoughts on why i think your motor choice was quite good.. :)
```

---
## \#7 Posted by: hahne Posted at: 2017-09-21T18:49:14.692Z Reads: 213

```
Thanks! 

Yeah he did. I will probably go metal one day too, but CNC stuff is so expensive, so i'll have to save up for a while
```

---
## \#8 Posted by: gogomrrobot Posted at: 2017-09-21T21:55:57.275Z Reads: 199

```
Very resourceful build. Your electronics enclosure for the Max6 case, can you post the STL files for that? It looks really cool.  At least include a few more close-ups if you don't wish to share the STL file.  Would be very appreciative.
```

---
## \#9 Posted by: hahne Posted at: 2017-09-22T00:10:23.179Z Reads: 202

```
I almost wish I went with an 8S pack though, as I have heard that voltage is better than capacity. The bottleneck that caused me to go for 6S was my balance charger. It can only do 6S, and i'm not very experienced with a BMS yet, so I didn't want to take a chance on one at this point. 

You definitely have a good point with the motors though. While mine do have a high top speed, and haven't given me any reason to believe that they are under-powered, the do get quite warm if I ride aggressively on a hot day. Cooler running 63mm motors would be of great benefit for me under these conditions. That said, as much as I am concerned that the warm motors might cause problems with the plastic mounts, its hasn't shown any evidence of this yet. We'll see in the future I suppose. Either way, its hard to complain when the motors were only $30 each. :slight_smile:
```

---
## \#10 Posted by: hahne Posted at: 2017-09-22T00:16:35.588Z Reads: 194

```
I can probably put the STL (3files) on here, But first I will have to correct a mistake or two that I made with it. I was having trouble with one of the screw holes and managed to break a section of the cover, you might be able to see in the pictures that the top part of the case is slightly lifted from the bottom on one side. I also need to make a small adjustment to the bottom two pieces so that it will fit the bolt pattern of the board better.

They are pretty easy fixes, but I am a little busy this week. I should be able to find some time for this before the end of next week.
```

---
## \#11 Posted by: Multi Posted at: 2017-09-22T00:25:33.497Z Reads: 180

```
Nice, what filament did you use for it... did it last.... Enough
```

---
## \#12 Posted by: hahne Posted at: 2017-09-22T00:29:27.972Z Reads: 184

```
Everything is printed with PLA. I found ABS to be a little too problematic for my liking.

So far, its holding up great!
```

---
## \#13 Posted by: hahne Posted at: 2017-10-04T03:46:19.227Z Reads: 186

```
I just tried posting the .STL files, but it turns out you aren't allowed to post them. I suppose I can understand why this would be the case. 

So for anyone who wants a case, I may be able to sell one to you.
This is the voltage tester that fits with the case:
http://www.ebay.com/itm/Capacity-Tester-Battery-Indicator-12V-24v-48v-car-Lead-acid-batteries-lithium/311727524930?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649

-Ryan
```

---
## \#14 Posted by: gogomrrobot Posted at: 2017-10-04T04:29:07.059Z Reads: 178

```
You could always just post it on thingverse.com and link it to us.

In any case, if you don't wish to do that... how much would you sell one for?

EDIT: Here is a link to a Max6 esc 3d STL file for Trampa on thingverse.com - it's an OK shape, I think your design is better.

https://www.thingiverse.com/thing:2292066
```

---
## \#15 Posted by: hahne Posted at: 2017-10-04T17:31:25.357Z Reads: 172

```
Good point! I completely forgot about thingiverse. I will upload it there, but I have to wait 24hrs to upload because I just created my account. I am a little too lazy to figure out shipping and all that nonsense anyway.

However, if anyone does not have a 3d printer, I could still work something out for you.

-Ryan
```

---
## \#16 Posted by: hahne Posted at: 2017-10-05T17:40:35.614Z Reads: 170

```
For anyone interested in my electronics case, the .STL files are on thingiverse! 

https://www.thingiverse.com/thing:2568270

-Ryan
```

---
## \#17 Posted by: gogomrrobot Posted at: 2017-10-05T17:49:43.042Z Reads: 160

```
Ryan that is super-generous,

Thank you so much!
```

---
## \#18 Posted by: hahne Posted at: 2017-10-05T22:15:43.113Z Reads: 158

```
no problem! I haven't printed a new one since I made some small modifications, so please let me know if it needs any changes. also you'll probably need some pretty long m4 bolts (or something similar) to connect the top part of the case to the bottom.

The top part of the case also has some extra holes beside the speed controller that you can pass the voltage monitor wires through to connect to the esc main leads, and a small gap at the front and back of the top part of the case if you want to add lights or something to the setup.

Hope it works out for you,

-Ryan
```

---
## \#19 Posted by: Achmed20 Posted at: 2017-11-25T11:31:19.994Z Reads: 142

```
since its been a while now, how is your 3d printed mount holding up?

was thinking about  doing something like this as well but i have serious doubts that its going to hold since the smaller version i designed before allready, had troubles with a 3200W motor.
```

---
## \#20 Posted by: hahne Posted at: 2017-11-25T15:49:39.413Z Reads: 144

```
It actually worked out pretty well. I was able to do quite a bit of off-roading with them. Although on my last ride of the season, I hit a nasty speedbump too fast and one my the mounts broke at the clamp. Surprisingly I was still able to limp the board home with only one mount carrying the weight of two.

I redesigned the clamp recently with a stronger clamp section and this time I will print with nylon or ABS instead of PLA.

My motors were only 5055s, so not too heavy, but the job. If you go with larger motors, I would recommend keeping the distance from the motor and the truck as small as possible. That way, you'll put much less mechanical stress on the mount each time you go over a bump.

I will post my updated mount soon!
```

---
## \#21 Posted by: hahne Posted at: 2018-02-20T00:31:30.015Z Reads: 131

```
Alright its been a while, but I finally stopped procrastinating and printed a new mount! I went through a few variations before I found one that seems to fit perfectly.

![new mount 4|666x500](upload://rRStaObCONlRnKKpciASh6YghHQ.jpg)

The first mount on the left was printed with PLA, which is the same material as my first generation mounts. Even though I have created extra reinforcements in the structure, I'm not too sure that I will use it because PLA is stiff and brittle. The Second mount was printed using nylon. This will likely be my choice material because nylon has super high strength. Unfortunately, it also has super strong warping and requires higher heat than my printer can manage for the time being. During printing, the part warped significantly, thereby causing it to become unusable. The third part was printed with ABS (I wish I had black, but I only had white laying around). It should be able to withstand more than the PLA, but likely a little less than the nylon. However, it is much easier to work with than nylon. I will test the new mount with ABS for now.

![new mount 1|375x500](upload://uhtCJqaXmCt4wE4OraxY1DTt2yL.jpg)

![new mount 2|375x500](upload://jhyy4w3Y6Mwvrfv4fFvPXyjN98X.jpg)

![new mount 3|375x500](upload://2Y8dn3YTxLhQ7Uo55UfkaGCWglp.jpg)

its still REALLY cold in Canada, so I'll probably have to wait a few weeks before I can do some field testing. Until then, I'll work on getting my printer to print nylon more effectively.

-Ryan
```

---
## \#22 Posted by: Der6FingerJo Posted at: 2018-02-20T06:46:28.590Z Reads: 121

```
I think ABS will be good for motor mounts, i don't use it only because of the smell and need for an enclosure, just can't be bothered to put so much effort in this kind of toxic stuff :smile:

I like the clamp design, i might even copy that and try it on one of my mounts. Looking forward to see how ABS will hold up!
```

---
## \#23 Posted by: hahne Posted at: 2018-02-20T23:47:42.709Z Reads: 115

```
It usually isn't so bad as long as you have a well ventilated area or an air filter, but yeah an enclosure is definitely a must. I took a day to build mine out of pine and Plexiglass. So far it works great!

 ![printer|375x500](upload://wWixlGofBfFCsf0taoprx9h0B7F.jpg)

Although it helps manage the ABS fumes, I'm looking forward to printing with less harmful nylon.

I'm going to add my second mount soon and then hopefully weather will cooperate long enough for me to test these out!
```

---
## \#24 Posted by: Der6FingerJo Posted at: 2018-02-21T06:06:49.160Z Reads: 106

```
That enclosure looks really nice, unfortunately my CR10 is huge so an enclosure would mean a lot more work :smile:

I think Nylon based stuff is the way to go!
```

---
## \#25 Posted by: krazor Posted at: 2019-02-07T12:02:01.416Z Reads: 71

```
im looking at building a trampa build and goign for a chain drive. i was wondering if you could point me in the direction of where you got the chain and sprockets from to fit the superstar hubs of the trampa?
```

---
## \#26 Posted by: Andy87 Posted at: 2019-02-07T13:30:46.014Z Reads: 70

```
Idk exactly about this one, but you can get them from here
https://www.e-toxx-shop.com/trampa/mtb/chain-drive/black-chaindrive-black-braces/#cc-m-product-9947927370

Or here

https://www.unikboards.com/en/

Or here

https://www.overion.fr/produit/kits-de-transmission-pour-motorisation-electrique/
```

---
## \#27 Posted by: hahne Posted at: 2019-02-07T16:18:28.132Z Reads: 71

```
I usually get most of that stuff from this website:
https://shop.sdp-si.com/catalog?brand=sdp 

it can be much cheaper to get it from a website like this, however, you will probably have to drill the holes precisely by yourself.
```

---
## \#28 Posted by: Nowind Posted at: 2019-02-08T12:20:46.752Z Reads: 65

```
[quote="krazor, post:25, topic:33656, full:true"]
im looking at building a trampa build and goign for a chain drive. i was wondering if you could point me in the direction of where you got the chain and sprockets from to fit the superstar hubs of the trampa?
[/quote]


He**y**
**Special Offer for this : 300€ shipped Worldwide**
https://www.e-toxx-shop.com/trampa/mtb/chain-drive/black-chaindrive-black-braces/#cc-m-product-9947927370
```

---
## \#30 Posted by: krazor Posted at: 2019-04-21T11:27:49.529Z Reads: 36

```
what bag are you using for the battery im thinking about a top mount but i dont want some thick big bulky plastic piece sitting on my deck
```

---
## \#31 Posted by: hahne Posted at: 2019-04-21T15:05:45.367Z Reads: 30

```
It's one that I got from a military surplus store. They usually have a bunch of different sizes that you can choose from
```

---
