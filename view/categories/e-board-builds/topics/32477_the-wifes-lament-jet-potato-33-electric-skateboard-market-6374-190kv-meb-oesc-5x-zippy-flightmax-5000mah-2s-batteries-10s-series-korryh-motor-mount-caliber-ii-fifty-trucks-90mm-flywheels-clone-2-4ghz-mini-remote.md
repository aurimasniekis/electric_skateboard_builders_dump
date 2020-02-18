# The Wife&rsquo;s Lament &#124; Jet Potato 33 &#124; electric-skateboard.market 6374 190kv &#124; MEB OESC &#124; 5x ZIPPY Flightmax 5000mah 2s batteries (10S series) &#124; KorryH Motor Mount &#124; Caliber II Fifty Trucks &#124; 90mm Flywheels Clone &#124; 2.4GHz Mini Remote

### Replies: 12 Views: 2508

## \#1 Posted by: topherbarnett Posted at: 2017-09-06T22:19:54.666Z Reads: 480

```
Here's a quick build page. I didn't take many photos during the actual construction, but can share what's in it, how it all went together, and a couple issues I had. But first the finished product:
<img src="/uploads/db1493/original/3X/0/1/0142145dab0eb5e89c0f9098dbcd47f390d28f11.jpg" width="589" height="500">

<img src="/uploads/db1493/original/3X/9/1/91ac452d5db0c3d85347b776e9988e542877f39d.jpg" width="396" height="500">

<img src="/uploads/db1493/original/3X/8/1/814877904dbe9d5cc5a537e9b1d5daf29e725880.jpg" width="690" height="342">

<img src="/uploads/db1493/original/3X/3/6/36234f099209138f1954cc019c104be0450538a1.jpg" width="679" height="500">

<img src="/uploads/db1493/original/3X/6/d/6dba950bbadacb30c38a579852b866311a62753a.jpg" width="400" height="500">


What's in it:
Deck: [Jet Potato 33](https://www.muirskate.com/longboard/completes/71821/jet-2016-potato-33-longboard-skateboard-custom-complete)
Trucks: Caliber II Fifty
Risers: [Luxe 1/2" TPR Riser Pad](http://www.skatewarehouse.com/LUXE_TPR_Flex_Formula_Riser_Pads_1_2/descpage-LX50RRP.html)
Wheels: 90mm Flywheel Clone
Wheel Pulley: [12mm 40T 3D Printed ABS @ 100% Infill](https://www.thingiverse.com/thing:2327563) by @mmaner 
Motor Pulley: [12mm 13T HTD5 Motor Pulley](diy-electric-skateboard-kits-parts/13t-htd5-motor-pulley-12mm/)
Motor: [Electric-Skateboard.Market 6374 190kv Outrunner](http://www.electric-skateboard.builders/t/6354-6374-stealth-motor-group-buy-part-2-rotating-light-rocket/8828/32)
Motor Key: [DIY 3x3x20mm Steel Keyway](diy-electric-skateboard-kits-parts/motor-keyway/)
VESC: [Miami Electric Boards OESC](https://miamielectricboards.com/shop-1/vesc) (running firmware version 2.54)
Motor Sensor Adapter: [Miami Electric Boards OESC Motor Adapter](https://miamielectricboards.com/shop-1/oesc-motor-adaptor)
Wireless Remote: [2.4GHz Mini Remote Transmitter/Receiver](http://www.ebay.com/itm/2-4GHz-Radio-Binding-Plug-Remote-Controller-Receiver-For-Electric-Skateboard-/192223853151?hash=item2cc16f3a5f:g:ddwAAOSwCmZZShOl)
Bluetooth Adapter: [HM10 BLE Bluetooth 4.0 Wireless Module](https://www.aliexpress.com/item/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module/32516357718.html?isOrigTitle=true11) (to run VESC app)
Loop Key: [XT90S](https://www.amazon.com/gp/product/B00WND5KFW/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)
Loop Key Mount: [XT90S Loop Panel Mount](https://www.thingiverse.com/thing:2323422) by @mmaner 
BMS: [eBay 60A Lithium-Ion 10S BMS](http://www.ebay.com/itm/60A-Lithium-Ion-7S10S13SBleeding-BMS-30A-60A-with-electronic-Switch-BMSOn-Off-/222373438930?var=&hash=item33c67d65d2)
Charge Port: [eBay 2.1mmx5mm Female DC Connector + Waterproof Cap](http://www.ebay.com/itm/282346888147)
Charger: 42v 2A from @JLabs group buy 
Battery: 5x [ZIPPY Flightmax 5000mAh 2S 30C Hardcase Packs](https://hobbyking.com/en_us/zippy-flightmax-5000mah-2s1p-30c-hardcase-pack-roar-approved-de-warehouse.html?___store=en_us) wired in 10S1P configuration
Battery Meter: [DROK DC8-63V](https://www.amazon.com/gp/product/B00VUUKIMY/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)

Here's a diagram of how things are hooked up:
<img src="/uploads/db1493/original/3X/3/d/3d1955da88b956c15dfb5d32f0f033eaa4742c34.jpg" width="690" height="266">

Putting it together:
1. The enclosure was used and had a couple holes in it. I ended up using painters tape on the outside, then applying several layers of ShoeGoo mixed with a couple drops of black modelers paint. This filled the holes nicely and should hold up to the abuse.
2. I cut new holes for the XT90S, charge port, and battery meter using a soldering iron with a flat tip. The fumes could be toxic, so I basically held my breath the whole time, had a window open, and a fan running. I cleaned up the edges with side snips and a box cutter. They're all mounted with ShoeGoo.
3. The battery, BMS, VESC and receiver are mounted with industrial strength velcro.
4. Most of the wiring is 10AWG, but I didn't want to unsolder the leads from the VESC, which I believe are 14AWG.
5. The BMS is wired for charging only, bypassing the discharge circuit, going directly to the VESC from the battery.
6. For the battery meter, I did a temporary version on [this mod](https://www.electric-skateboard.builders/t/what-is-the-best-voltage-meter/23857/9). I stripped a couple wires and used electrical tape to keep them in place, then powered the unit on holding down FDn, and touched the two wires together to get the function menu. Easy-peasy.

Issues:
1. One thing that really threw me for a while was when I couldn't get the 2.4GHz remote to make the VESC go. After much poking and prodding, it turns out that the sticker on my Rx was on upside down, so I was plugging in channel 3, rather than 2. Note: you have to look at the hard-to-see stamped numbers, rather than counting from what you may assume to be the top. :rolling_eyes:
2. With this motor mount, I really should have filed down some of the hanger to get it seated further in, but I didn't want to ruin anything, and I don't have a file or dremel at the moment. The 12mm wheel pulley sticks out far enough to hit the socket head screws, so I had to use 3 speed rings to get enough clearance. No big deal though.
3. With the 90mm wheels, I had to use 1/2" riser pads to get enough clearance to avoid wheel bite.
 
I really haven't had any other issues, and everything went together pretty well. I'd really like to run FOC to quiet the high-pitch noise when accelerating/decelerating, but I don't have the $ to replace the VESC if it dies, so I'll stick with BLDC for the time being. I also think running some non-clone wheels may give a smoother ride, but after the first ride, I'm a very satisfied customer. Thank you again electric-skateboard.builders!
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-09-06T23:54:28.272Z Reads: 339

```
More pics please!!
```

---
## \#3 Posted by: chinzw Posted at: 2017-09-07T00:37:32.024Z Reads: 336

```
What enclosure is that?
```

---
## \#4 Posted by: guyguy Posted at: 2017-09-07T03:24:43.564Z Reads: 327

```
love the name of this board
```

---
## \#5 Posted by: Clonkex Posted at: 2017-09-07T03:52:04.831Z Reads: 315

```
Wow, that's so freakin _clean!_ I love it! Even your wiring diagram is neat and clean. And obviously the name is fantastic :P

I wanna see more of this build.
```

---
## \#6 Posted by: WawiKirsinger Posted at: 2017-09-07T17:50:04.784Z Reads: 270

```
hey whats your tops speed and range?
```

---
## \#7 Posted by: sl33py Posted at: 2017-09-07T18:18:40.012Z Reads: 257

```
Great looking build and really well thought out diagram!  Would be super helpful for all the "how do i bypass BMS?" questions we get non-stop...

Well done sir!

One minor critique - i would replace the socket head bolts on the motor mount w/ lower profile bolts, and flip your motor gear so there is less leverage and you run it closer to the motor plate.
```

---
## \#8 Posted by: topherbarnett Posted at: 2017-09-07T20:59:32.329Z Reads: 251

```
[quote="chinzw, post:3, topic:32477, full:true"]
What enclosure is that?
[/quote]
It's a @psychotiller 25" Monolith Low Pro

[quote="WawiKirsinger, post:6, topic:32477, full:true"]
hey whats your tops speed and range?
[/quote]
I have no idea yet. This is not just my first esk8, but my first skateboard in general, so I'm taking my time getting comfortable. The gearing is probably a bit low for a high top speed, but it handles hills nicely. I may swap to a 16T motor pulley later, if I feel the need for more speed. Once I brave the full trigger pull, I'll update here.

[quote="sl33py, post:7, topic:32477"]
One minor critique - i would replace the socket head bolts on the motor mount w/ lower profile bolts, and flip your motor gear so there is less leverage and you run it closer to the motor plate.
[/quote]
Thanks for the suggestion, that makes sense!
<br><br>

There are a few more things I need to finish up on here. First is the motor sensor wire, then the bluetooth module so I can try out the phone app. Lastly, I want to find a good, but cheap lighting solution. I may just end up going [this route](https://www.electric-skateboard.builders/t/eskate-lights-thread/199).
```

---
## \#9 Posted by: Blitz Posted at: 2018-01-10T14:25:47.459Z Reads: 162

```
How do you Charge all them batteries?

Did you Direct solder groups together?
```

---
## \#10 Posted by: cosmicc89 Posted at: 2018-01-10T15:40:26.748Z Reads: 160

```
Your build is so clean! It looks fantastic. 

Is your enclosure waterproof? I see there is some kind of weather stripping along the edge?
```

---
## \#11 Posted by: topherbarnett Posted at: 2018-05-24T19:23:26.522Z Reads: 108

```
They're soldered together is series and charged with a 10s BMS and a 42V power supply. Charge times are high, but the ease of use makes it worth it.
```

---
## \#12 Posted by: topherbarnett Posted at: 2018-05-24T19:26:11.982Z Reads: 105

```
Thanksn there's some weatherstripping around the edge, but it's not totally waterproof because the enclosure is two overlapping halves and theres a hole where the wires go to the motor. I just don't ride in the rain.
```

---
