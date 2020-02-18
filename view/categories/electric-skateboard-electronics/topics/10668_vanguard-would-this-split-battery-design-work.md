# Vanguard: Would this split battery design work?

### Replies: 27 Views: 2773

## \#1 Posted by: michaelcpg Posted at: 2016-10-05T08:06:50.781Z Reads: 276

```
Inspired by @whitepony's Vanguard build, I'm thinking about rebuilding my board with a split battery design on a 42" Flex 1 Loaded Vanguard with dual diagonal motors. The battery will be split into two parts but wired together to create a 10S4P pack. I'll be looking to get a small BMS just for charging and then something like @torqueboards softswitch. 

I've drawn up a basic circuit diagram but I'm hoping someone would be able to confirm if this design would actually work. The thing I'm unsure about is having a VESC at two different points in the battery circuit. Would this be an issue for any particular reason?

<img src="/uploads/db1493/original/3X/0/a/0ad83eece6c2587414f6d3144f4a44ed00218c8c.jpg" width="690" height="202">

I'm going to be looking at running grooves on the top side of the deck for wires to run down under the grip tape, similar to how @longhairedboy does with his boards. 

I've also thought about having both VESC's at one end which would probably save some space as it'd allow me to have them both connected to a single capacitor bank. The only issue with this is that I'd end up with a total of 5 wires running the length of the deck (3 phase wires and 2 battery wires) but I'd be concerned that this would probably be getting a bit much in regards to reducing the strength of the deck.

Looking forward to hearing people's thoughts :)
```

---
## \#2 Posted by: torqueboards Posted at: 2016-10-05T08:23:29.100Z Reads: 261

```
Typically, you'd wire both VESCs on one side and and just extend (one) motor with 10-15"+ motor wires to the opposite motor. Much easier that way and you want less "length" from the VESC to the Battery.

Otherwise, you'd have to also wire in the Canbus connector, power wires for the VESC.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-10-05T08:37:36.108Z Reads: 262

```
<img src="/uploads/db1493/original/3X/a/f/af7421670b13d97acc72bf7a341d7a261a285200.jpg" width="690" height="388">

That's essentially what I have now. This idea is really just to eliminate the need for any extra wires running down the deck for the other motor. I don't use canbus so that won't be an issue.
```

---
## \#4 Posted by: jujet Posted at: 2016-10-05T09:32:08.199Z Reads: 257

```
Hey OP, nice to see someone else building a vanguard :D I myself am ordering all the bits and pieces at the moment. 

What enclosures are you going to use?
```

---
## \#5 Posted by: Kaly Posted at: 2016-10-05T10:08:29.549Z Reads: 250

```
The idea will work. 
Another approach will be to split the enclosure one for the battery and the other for the VESC.

Like in this
<img src="/uploads/db1493/original/3X/8/5/851acb90980eb1b648be9b8030e469bbce568d35.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/1/d10331ba530450df1d325ff7e58a77171dd67890.JPG" width="690" height="388">

 And run flat wire like this one http://www.mcmaster.com/#69925k66/=14gnk59
under the grip tape.
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-10-05T10:52:58.818Z Reads: 237

```
I have thought about this a little bit, how does it handle the flexing though? One concern I have with a longer enclosure on one side is that it'll make it hard to make fairly watertight
```

---
## \#7 Posted by: whitepony Posted at: 2016-10-05T11:26:05.688Z Reads: 229

```
my 10S4P split vanguard build thread is here - the layout is very similar to yours and available on the first post: https://endless-sphere.com/forums/viewtopic.php?f=35&t=80808

the split vesc diagonal setup is something I dont really like - long wires everywhere (long wires = unecessary inductance = bad) and for me it simply doesnt look very pleasing to the eye compared to a dual rear 6355 setup. but thats just me ... and for flat norther germany, a single 15mm drive is best anyway. lighter and definitely more efficient. :smiley_cat:
```

---
## \#8 Posted by: michaelcpg Posted at: 2016-10-05T11:42:01.357Z Reads: 218

```
Yea I've looked through that thread several times, really awesome stuff :) 

Maybe it's not quite so obvious from my diagram but there wouldn't be any more longer wires than your build, the front motor would connect to the other end of the battery so that the only wires running between the two enclosures is two battery wires to connect the battery packs in the same way as yours. 
Ive never seen someone do a build where each vesc is connected to the opposite end of a battery but I can't see any reason why it wouldn't work?
```

---
## \#9 Posted by: whitepony Posted at: 2016-10-05T13:25:38.251Z Reads: 208

```
maybe my brain is damaged after a day of coding, but i dont see how you can get away with 2 instead of 4 wires? :confused:
```

---
## \#10 Posted by: PB1 Posted at: 2016-10-05T14:14:27.132Z Reads: 195

```
@michaelcpg,  you want to connect vescs at both ends of the battery? This  will not work. 

You could split the battery into two 10s2p packs,  each driving one motor.  
Then you only need thinner wires for can bus or ppm signal.  And possibly some wires to make sure the vescs are at the same voltage.  
This setup will need two power switches.
```

---
## \#11 Posted by: Kaly Posted at: 2016-10-05T14:25:16.155Z Reads: 198

```
It handles the flex pretty good. 
You can always split the long enclosure into 2 small ones  place side-by-side along the long axis for more flexibility. 

For waterproofing I use thin double side tape on the perimeter of the enclosure and clear pvc sheet  to cover everything. At the wires exit holes apply silicone. that seals all the electronics inside and allows for visual inspection.

The clear pvc sheet you can get at any flower shop. They use is to wrap the flower bouquet. You can get it for free if you ask nicely ;-)
```

---
## \#12 Posted by: TarzanHBK Posted at: 2016-10-05T14:40:47.968Z Reads: 195

```
<img src="/uploads/db1493/original/3X/c/1/c1b25915aefccc6cf793e444409d89e878b2f568.jpg" width="690" height="250">

i´d prefer the upper one. 4 wires
```

---
## \#13 Posted by: Titoxd10001 Posted at: 2016-10-05T16:06:44.205Z Reads: 184

```
And don't forget the extra long servo plug for the signal. Why do want dual diagonal vs dual rear?

Also with dual rear you have more space in the front because you can move batteries closer to the trucks.
```

---
## \#14 Posted by: michaelcpg Posted at: 2016-10-05T20:15:53.918Z Reads: 179

```
Looking at my diagram a bit more, a think the main issue with this design is that it'd be putting the VESCs in series instead of in parallel.

Not sure how I feel about the idea of two separate packs due to the added complexity/extra components required. Something to consider though.

@TarzanHBK  Would it be preferable to run longer wires between the battery and one of the VESCs or between a VESC and a motor? I thought you can have issues running long wires between a battery and VESC.

@Titoxd10001 Tbh I wouldn't mind dual rear. The main issue being though is that I already have dual Ollin motors which don't fit on the Enertion trucks/motor mounts that I have.

@whitepony Do you expect that if I ran wire along the top of the deck similar to how you did with your build, increasing the widths of the groves to add room for another 2 or 3 wires would reduce the strength of the deck too much on a Flex 1?

<img src="/uploads/db1493/original/3X/0/6/06a8b42b50760397761e0b834eb01f2fb97120b6.jpg" width="690" height="450">
```

---
## \#15 Posted by: maxz Posted at: 2016-10-05T21:38:20.006Z Reads: 166

```
Why not use flat wire and dont route your board?? Grip tape would hold it in place.
```

---
## \#16 Posted by: michaelcpg Posted at: 2016-10-05T21:41:06.704Z Reads: 165

```
This could end up being something I'll do tbh. Just trying to work out all options at this stage :)
```

---
## \#17 Posted by: maxz Posted at: 2016-10-05T21:43:44.725Z Reads: 162

```
Fair enough... Where did you get your batteries from?? I looked high and low for some here and the cheapest i could find were $8.5 each for samsung 25r
```

---
## \#18 Posted by: michaelcpg Posted at: 2016-10-05T21:46:23.070Z Reads: 159

```
I initially bought a 3p space cell from Enertion then ended up buying another 10 cells from here:
https://thevapingkiwi.co.nz/

Not cheap at $10 a cell but getting them overnight as opposed to having to wait multiple weeks to get them shipped from overseas was enough of an incentive for me to buy locally :p
```

---
## \#19 Posted by: maxz Posted at: 2016-10-05T21:50:31.406Z Reads: 156

```
Yeah fair enough, these guys https://vapourium.nz/products/samsung2500mah18650 would drop the price to $8.5 if i brought 30 and put one of his stickers on my board haha. Im getting a battery from torque boards but highly contemplated to make my own but i didnt want to purchase a spot welder and wasnt comfortable to solder $255 worth of batteries together haha
```

---
## \#20 Posted by: michaelcpg Posted at: 2016-10-05T21:53:47.969Z Reads: 162

```
Yea I wasn't too sure about it initially either but I'm glad I did build my own in the end, learnt a lot and now I can fairly easily rebuild my battery/add more cells as needed. 
I use fuse wire on all my cells for an extra level of safety which also makes it much easier to solder directly to the cells seeing as the fuse wire is really thin.
```

---
## \#21 Posted by: maxz Posted at: 2016-10-05T21:57:14.898Z Reads: 160

```
What bms did you go with?? a cheap one from ebay or something?? the guy making my board can also make an enclosure for it so it is very tempting haha. Just dont want to stuff it up but it is a lot safer then trying to get one in the country.
```

---
## \#22 Posted by: michaelcpg Posted at: 2016-10-06T02:47:46.683Z Reads: 155

```
Is anyone able to comment on whether this stuff should be suitable to use between the battery packs and VESCs instead of standard 10AWG wire in one of the configurations that @TarzanHBK has provided in his diagram?

There's also an 11mm wide option but I'm not sure if this would be thick enough?

http://www.ebay.com/itm/1m-3-3ft-15mm-Flat-Copper-Braid-cable-Bare-copper-braid-wire-ground-lead-/151895915285?_trksid=p2141725.m3641.l6368

@maxz I'm still using the BMS that came with my space cell, I'll be looking to order a new one just for charging to replace it though as my current one is too big.
```

---
## \#23 Posted by: zmoney Posted at: 2016-10-06T03:12:30.017Z Reads: 145

```
This might help you: http://www.coonerwire.com/flat-braided-wire/
```

---
## \#24 Posted by: TarzanHBK Posted at: 2016-10-06T07:49:51.708Z Reads: 141

```
it should not be a problem running these longer wires to the vesc, as long as you don´t build up much resistance with too small ones. So 10Awg should be fine. Just keep in mind that some people getting problems with long wires in combination with FOC, so you should stay in bdlc mode, just to be safe.
Also i wouldn´t risk weakening your deck with 4 wires running through your deck. Better take flat wires, that are comparable with 10awg wires and go the BoostedBoard way ;)
```

---
## \#25 Posted by: whitepony Posted at: 2016-10-06T08:55:07.018Z Reads: 135

```
inductance of long wires is the problem, less the resistive losses. it can be somewhat counteracted by larger capacitors at the vesc.

https://www.eeweb.com/toolbox/wire-inductance
```

---
## \#26 Posted by: whitepony Posted at: 2016-10-06T18:10:51.035Z Reads: 128

```
[quote="michaelcpg, post:14, topic:10668"]
Do you expect that if I ran wire along the top of the deck similar to how you did with your build, increasing the widths of the groves to add room for another 2 or 3 wires would reduce the strength of the deck too much on a Flex 1?
[/quote]


probably because you have a flex 1, it would probably not be a problem. but yea, flat wide wires should work too - in the end the wires will have the same "volume" either way if you want to have the same resistance - so you could router very shallow and wide or more in a rectangular shape for the flat wires. running them ontop is something I wouldnt do, because it would show through the grip tape. :stuck_out_tongue:
```

---
## \#27 Posted by: barkeep89 Posted at: 2020-02-06T10:06:42.931Z Reads: 11

```
I looked on vapeproducts.co.nz and bought 10 cells for my board. It's enough of an incentive for me to buy in New Zealand :grinning:
```

---
