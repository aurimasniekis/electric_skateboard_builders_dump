# &ldquo;Raptor 2.1 GTX&rdquo; &#124; R-SPEC DRIVE &#124; FOCBOX Unity &#124; 12S3P VTC5 &#124; 3D printed custom enclosure

### Replies: 44 Views: 2580

## \#1 Posted by: occino Posted at: 2019-01-29T10:28:42.765Z Reads: 474

```
![Complete1](https://raw.githubusercontent.com/occino/enertion/master/complete/DSC_0062.JPG)

**Hi guys,**

I'm Nico from Berlin, Germany and I'm building electric longboards since two years now. I would like to share with you my latest and easiest build which is technically a Raptor 2.1 with at GTX deck. I'm also motivated to write this post because of the **Enertion R-SPEC DRIVE KIT | Best Build Competition** [[link](https://www.electric-skateboard.builders/t/enertion-r-spec-drive-kit-best-build-competition-win-cash-back/ "Enertion")].

## Specs & features:

* R-SPEC DRIVE KIT w/ 90mm wheels [[link](https://www.enertionboards.com/electric-skateboard-direct-drive-hub-motor-kit-r-spec/ "R-SPEC DRIVE KIT")]
* FOCBOX UNITY ESC [[link](https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc/ "FOCBOX UNITY ESC")]
* Evolve GTX deck [[link](https://evolveskateboardsusa.com/products/deck-bamboo-gtx "Evolve")]
* Custom 12S3P battery pack w/ VTC5 + BMS [[link](https://eu.nkon.nl/sony-us18650vtc5-flat-top.html "eu.nkon.nl"), [link](https://www.aliexpress.com/item/BMS-6S-7S-8S-9S-10S-11S-12S-13S-4-2V-25A-Adjustable-BMS-Lithium-Li/32931097519.html "BMS")]
* 3D printed custom enclosure + PVC bottom plate [[link](https://www.thingiverse.com/thing:3382660 "Thingiverse")]
* Enertion Nano-X 2.4Ghz Controller [[link](https://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/ "Remote")]
* Voltage display [[link](https://de.aliexpress.com/item/0-36-DC0-100V-LED-Mini-Digital-Voltmeter-Blue-red-green-LED-Display-Volt-Meter/32817252098.html "link")]
* USB charging port module [[link](https://de.aliexpress.com/item/LM2596HV-5V-DC-DC-Step-Down-Buck-Converter-Module-9V-12V-24V-36V-48V-to-5V/32831931798.html "link")]
* Loop key

## GTX deck
![GTX1](https://raw.githubusercontent.com/occino/enertion/master/deck/DSC_0008.JPG)
The GTX deck by evolve is perfectly suited in my opinion because it comes already with a notch for the battery pack. Furthermore it's flexible and looks nice.

In order to use a 10S4P battery, the notch had to be enlarged by about 1 cm. I used the original screw holes to mount the enclosure.

## Enclosure
![Enclosure1](https://raw.githubusercontent.com/occino/enertion/master/enclosure/enclosure.png)
The enclosure is a modular 3D printed frame with a PVC plate underneath. Due to the dimension limits of 3D printing, I decided to design a modular system which can be printed in multiple parts. To ensure water resistence, I used a *tongue and groove* technique which makes the enclosure flexible as well. I also used sponge rubber between deck and enclosure as well as between PVC plate and enclosure.
You can find all parts on [thingiverse](https://www.thingiverse.com/thing:3382660 "Thingiverse").

![Enclosure2](https://raw.githubusercontent.com/occino/enertion/master/enclosure/IMG_20190126_122641.jpg)

### Mounting
In order to mount the PVC plate underneath, I glued M4 threaded sleeves (5mm x 18mm) ([link](http://www.lignoshop.de/gewindehuelse-stahl-m4-5mm-37811022000.html "link")) into the parts as you can see in the picture below. This way I could use proper thread screws. The threaded sleeves pass through the entire material. This allowed the deck to be screwed on from both sides. This makes the construction pretty strong. 

![Enclosure3](https://raw.githubusercontent.com/occino/enertion/master/focbox/DSC_0018.JPG)

### FOCBOX UNITY case
![FOCBOX1](https://raw.githubusercontent.com/occino/enertion/master/focbox/focbox_case.JPG)
The rear part of the enclosure contains the FOCBOX UNITY as well as a battery voltage display  and the power switch provided by enertion. The voltage display is powered by the CAN bus port (5V, GND) and the measuring wire is connected to the BATT+ pin of the AUX port. The FOCBOX sits tightly into the compartment, so there is no need to mount it with screws.

### Connector box
![ConnectorBox1](https://raw.githubusercontent.com/occino/enertion/master/connectorBox/connectorBox.jpg)
The connector box is the middle part of the enclosure and contains receiver, 3A USB charging module (LM2596HV), XT60 charging port, XT60 key loop and all wiring. The charging port is connected to the BMS via XT30 in order to change the battery easily. The receiver of the Enertion Nano-X 2.4Ghz Controller fits perfectly in a small compartment and doesn't need to be srewed down.

### Battery pack (12S3P, Sony Konion VTC5)
![Battery1](https://raw.githubusercontent.com/occino/enertion/master/battery/battery.jpg)
12S3P or 10S4P? I chose both variants. 12S for more fun and 10S for more range. For the 12S3P pack I used 36 **Sony Konion US18650VTC5 cells 2600mAh** with a total capacity of 336Wh. I paid 128€ for 36 VTC5 cells on [eu.nkon.nl](https://eu.nkon.nl/ "eu.nkon.nl"). 36 VTC6 cells with 3000mAh would have cost 207€ for additonal 53Wh. Range is not that important to me, so I took the cheaper option.

![Battery1](https://raw.githubusercontent.com/occino/enertion/master/battery/spotwelder.JPG)

For spotwelding, I used the amazing kWeld by [keenlab](https://www.keenlab.de/ "keenlab") powered by a high discharge lipo. The nickel strips are pure nickel  (8mm x 0.3mm). I made some tests and figured out that they can easily handle 25A. In order to archive the full rated 90A of the cells, I used 4 layers of nickel (pyramid technique) at the S-transitions to be on the safe side.

![Battery2](https://raw.githubusercontent.com/occino/enertion/master/battery/batterySetup.jpg)

![Battery3](https://raw.githubusercontent.com/occino/enertion/master/battery/pyramid.jpg)

![Battery4](https://raw.githubusercontent.com/occino/enertion/master/battery/pack_raw.jpg)

The BMS is a cheap 13S circuit usable for 12S as well. It is only used for charging and not for discharging. To prevent the battery from over discharge, I used the cut off setting of the FOCBOX UNITY.
As I mentioned before, I would like to use 12S3P and 10S4P battery packs in the battery compartment. In order to get the same dimensions, I printed a 2x2 dummy cell construction as your can see on the picture below.

![Battery5](https://raw.githubusercontent.com/occino/enertion/master/battery/pack_bms.jpg)

After adding all the wires, I added felt pads on all edges which should absorb shocks and keep the pack tight in the battery compartment.

![Battery6](https://raw.githubusercontent.com/occino/enertion/master/battery/pack_padding.jpg)

Finally I used a 200mm shrink tube and a hot air gun to close the battery pack.

![Battery7](https://raw.githubusercontent.com/occino/enertion/master/enclosure/IMG_20190126_150100.jpg)

After inserting the battery and connecting the XT60 and XT30, the only thing left was the bottom plate.

![Battery8](https://raw.githubusercontent.com/occino/enertion/master/enclosure/enclosure_bottom.jpg)

That's it. Just an easy, modular build :).

What do you think? Any suggestions for improvements?

If you have any questions please feel free to drop a message.

Cheers, Nico
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-01-29T10:59:30.031Z Reads: 405

```
this is really well done. would be a bit concerned about water ingress but apart from that you've done an awesome job.
```

---
## \#3 Posted by: mutantbass Posted at: 2019-01-29T11:17:49.388Z Reads: 385

```
that battery is beauiful :) good job
```

---
## \#4 Posted by: occino Posted at: 2019-01-29T11:22:40.907Z Reads: 385

```
Thanks Matt!
I used a lot of sponge rubber in order to keep water out auf the enclosure. The only place which is not sealed is where motor wires run into the focbox case. I'm already working on a solution for that :)
```

---
## \#5 Posted by: Winfly Posted at: 2019-01-29T18:44:23.198Z Reads: 351

```
Nice build!! I really like the compartments for electronics. Also, I'm worry about your battery. Afaik , the bamboo GT is quite flexible and the way you spot welded series connections with only nickel strip concerns me. Ignoring whether your spot welds are good or not. You will be pulling a alot of stress on these nickel strip and they might eventually give out.
```

---
## \#6 Posted by: occino Posted at: 2019-01-29T19:13:58.034Z Reads: 322

```
Hi @Winfly, thanks for your response. The bamboo GTX deck is not that flexible compared to Loaded decks for example. I literally jumped with my 90kg on the final board and it only sag about 1-1.5 cm in the center. To be honest, I'm a bit disappointed about the flex. With all the padding around the battery I think this should be fine.
```

---
## \#7 Posted by: rey8801 Posted at: 2019-01-29T19:26:14.024Z Reads: 309

```
On that spot you can internally add sugru or what I do is back sealant silicone. It cures in about 24 hours and became rather strong but really elastic so it will allow to the cable to move a bit while keep everything sealed. Plus you can always remove in case of intervention.
```

---
## \#8 Posted by: Superflim Posted at: 2019-01-29T19:35:22.145Z Reads: 293

```
does this work on blank pcbs too? or only on sealed off wires?
```

---
## \#9 Posted by: rey8801 Posted at: 2019-01-29T19:41:57.454Z Reads: 290

```
You can find it in the home depot. I prefer over sugro for sealing because you can always remove and doesn't leave any residues. Sugru is fantastic to hold parts in place, but I prefer the black silicon for those part where you have a hole with wires going through. In thst case the silicon can really fill up all the gaps and then became a rubber wall really elastic.
```

---
## \#10 Posted by: Superflim Posted at: 2019-01-29T19:44:58.147Z Reads: 278

```
my question was will it damage electronics?
```

---
## \#11 Posted by: gmurad Posted at: 2019-01-30T00:17:08.811Z Reads: 274

```
That's a cool way to build a battery case! Could be really cool and functional with a transparent bottom plate. I wonder if the *tongue and groove* would really stop water.

Also saw that you posted your build in Github. I guess you work in tech?
```

---
## \#12 Posted by: barajabali Posted at: 2019-01-30T01:01:55.481Z Reads: 268

```
Awesome build! Competition is getting good now :)
```

---
## \#13 Posted by: briman05 Posted at: 2019-01-30T02:54:42.770Z Reads: 268

```
This looks very thought out I am really liking the unity printed box.
```

---
## \#14 Posted by: landonkun Posted at: 2019-01-30T05:30:18.147Z Reads: 263

```
I'm curious about the PVC plate. Where did you get it? How was the shape cut that way?
```

---
## \#15 Posted by: occino Posted at: 2019-01-30T09:29:16.440Z Reads: 273

```
Hi @gmurad,
funny that you mention transparent bottom plate. I already played around with plexiglass before the 100x50x2mm PVC plate arrived. You are right, the post is hosted on github as well. Thanks to markdown the readme.md in github is perfect to prepare a longer post. And yes, I'm working as a software engineer (bachelor in electrical engineering and master in computer engineering).

Here's an old picture with plexiglass underneath the board.

![plexiglass](https://raw.githubusercontent.com/occino/enertion/master/enclosure/plexiglass.JPG)
```

---
## \#16 Posted by: occino Posted at: 2019-01-30T14:09:05.650Z Reads: 257

```
Hi @landonkun,
I bought it on [ebay](https://www.ebay.de/itm/323578072021  "ebay"). Unfortunately, the seller only ships within Germany. Maybe you find something similar in Canada. The material is pretty soft and not brittle as plexiglass. Therefore I used a jigsaw to cut the shape and a file for the finish.
```

---
## \#17 Posted by: Smithster Posted at: 2019-02-05T21:27:46.246Z Reads: 237

```
congrats nice build
```

---
## \#18 Posted by: dareno Posted at: 2019-02-05T23:18:56.153Z Reads: 225

```
Nice clean build that.  Love the simplicity and the thought that went into the enclosure.  Awesome stuff.
```

---
## \#19 Posted by: deucesdown Posted at: 2019-02-05T23:57:49.536Z Reads: 230

```
[quote="occino, post:1, topic:82469"]
kWeld by [keenlab ](https://www.keenlab.de/) powered by a high discharge lipo. The nickel strips are pure nickel (8mm x 0.3mm)
[/quote]

I tried welding 0.3mm strip with a kweld to some dead 18650. Gave up at 100joules, as the nickel, the cell, and hhe electrodes were very hot after just a few attempts. This was with a 3s 65c 6000mah graphene pack. I have the crimped XT150 electrodes. I also didnt like how things were going with 0.25mm strip.

Can you tell me your settings, setup, and how it went?

I like the cell holding jig. :)

And how are you finding 10s4p vs 12s3p? Not many people have been able to do direct comparisons.

Thanks for posting!
```

---
## \#20 Posted by: mikenyc Posted at: 2019-02-06T00:58:56.572Z Reads: 210

```
can that battery flex?
```

---
## \#21 Posted by: epss4 Posted at: 2019-02-06T03:19:14.080Z Reads: 184

```
What range and speed do you get ?? 
Really nice build!
```

---
## \#22 Posted by: Winfly Posted at: 2019-02-06T05:32:59.274Z Reads: 184

```
Tried my friend's bamboo GT again. can confirm that it flexes a lot. not as much as the boosted but it's not a stiff deck for your rigid battery pack.
```

---
## \#23 Posted by: occino Posted at: 2019-02-06T07:15:09.193Z Reads: 184

```
Hi @mikenyc,
yes the battery is a bit flexible. Because of the padding with felt pads around the battery, the battery do not need to be flexible as the deck anyway.
After a few rides I will inspect the weldings spots for any weaknesses.
```

---
## \#24 Posted by: occino Posted at: 2019-02-06T07:30:25.965Z Reads: 184

```
Unfortunately, the weather in germany really sucks lately. Therefore I have not tested speed and range. I expect a speed of > 50km/h (>31mph) and a range of at least 20km (12.5 miles) with the 12S3P pack. I will do a range test at the weekend but figuring out the max. speed will tricky I guess :smile:
```

---
## \#25 Posted by: occino Posted at: 2019-02-06T08:29:05.127Z Reads: 175

```
Hi @deucesdown,
I used a **Multistar High Capacity 6S 20000mAh** with 20C burst. I turned the kWeld to 15-20J and put a decent amount of pressure onto the welding spots to ensure a good conductivity with less sparks.

I also tested the kWeld with old 18650 cells and noticed significant differences. Welding VTC5 work fine but some old china cells dont. Even with higher joules the nickel don't stick to the cells.

Furthermore I had problems with nickel coated strips. I highly recommend to do a scratch test to ensure that you got pure nickel strips. Just scratch a piece of nickel and put it in water over night. If your see rust, you got steal with a nickel coat. This is bad for welding and no suitable for high current applications.

Welding 0.3mm nickel turned out a bit tricky but it's definitely possible. I did some breaks because the anodes and even the battery got hot.
```

---
## \#26 Posted by: mikenyc Posted at: 2019-02-06T09:48:53.998Z Reads: 165

```
Hmm, how can you inspect the welds under the shrink wrap and padding?
```

---
## \#27 Posted by: occino Posted at: 2019-02-06T09:56:51.201Z Reads: 168

```
I will open up the shrink tube and remove the padding. After inspecting I will close it up again ;)
```

---
## \#28 Posted by: Sn4pz Posted at: 2019-02-06T13:55:24.901Z Reads: 160

```
I feel like the nickle would pass his initial testing. and then the real world torture of *potentially*(not making fun of anyone, just thinking realisticsally) heavier people bouncing up and down on them.... I dunno if I would trust the check after just a few rides
```

---
## \#29 Posted by: mikenyc Posted at: 2019-02-06T14:08:46.856Z Reads: 166

```
yeah, that's going to break down over time. not criticizing the packs construction -- i just don't think it's appropriate for a deck with that much flex.
```

---
## \#30 Posted by: Sn4pz Posted at: 2019-02-06T14:22:50.097Z Reads: 169

```
Absolutely

😍:drooling_face: ![955bb3af03a55caf4feb6acd53550faa49cf72d8_1_666x500|666x500](upload://p9NKIzCYd8vkv4E2taneAWn6pUZ.jpeg)
```

---
## \#31 Posted by: mikenyc Posted at: 2019-02-06T14:30:53.257Z Reads: 166

```
show off! !
```

---
## \#32 Posted by: Sn4pz Posted at: 2019-02-06T14:47:19.150Z Reads: 164

```
I can't take credit haha, it's Hyperion2s work, great job Ben

Hopefully he finesses my pack like that huh? ;)
```

---
## \#33 Posted by: deucesdown Posted at: 2019-02-06T17:33:07.148Z Reads: 163

```
I worry about the wires that go between compartment -- seems like they're sandwiched between deck and enclosure and would be subject to rubbing.
```

---
## \#34 Posted by: Sn4pz Posted at: 2019-02-06T17:35:01.535Z Reads: 167

```
fair point, and to be honest its not mine :crazy_face:

I guess Ill ask Ben or Cory(whoever I guess) to ensure they wont wiggle or move
```

---
## \#35 Posted by: epss4 Posted at: 2019-02-10T02:59:32.680Z Reads: 155

```
![image|666x500](upload://weggrkLxeNtA3jVDK0VDVBcSN1n.jpeg) 
😁😁😁
```

---
## \#36 Posted by: occino Posted at: 2019-02-27T16:02:46.257Z Reads: 142

```
I tested the board in the last days and did some adjustments. Especially the acceleration curve needed to be soften at 12S. Otherwise the kick is too hard when pushing the throttle.
I made about 25km with the 12S3P pack and easiliy hit 45km/h but then I felt scared :smiley: 
Because of the battery frame the GTX deck is not that flexible anymore. Therefore the battery pack do not need to be flexible as well.

All in all I'm very satisfied with the result. Compared to my other builds I really have to learn to handle the power :sweat_smile:
```

---
## \#37 Posted by: epss4 Posted at: 2019-02-27T16:37:30.842Z Reads: 139

```
Will you mind sharing your acceleration curve :)?
```

---
## \#38 Posted by: occino Posted at: 2019-02-27T17:55:00.838Z Reads: 140

```
Sure ;) ![ui|236x500](upload://tGRx9dbt1VIMwesh1UX3SbT7VjU.png)
```

---
## \#39 Posted by: epss4 Posted at: 2019-02-27T18:07:43.652Z Reads: 137

```
Thanks man!
```

---
## \#40 Posted by: huntercasillas Posted at: 2019-04-05T07:40:40.604Z Reads: 106

```
Do you have a link to that battery percentage reader? Where did you connect it on the unity exactly?
```

---
## \#41 Posted by: occino Posted at: 2019-04-08T09:14:41.593Z Reads: 99

```
Hi, this is only a simple voltage display ([link](https://de.aliexpress.com/item/0-36-DC0-100V-LED-Mini-Digital-Voltmeter-Blue-red-green-LED-Display-Volt-Meter/32817252098.html)). For me the battery voltage is more meaningful than a percentage display.
Cheers
```

---
## \#42 Posted by: epss4 Posted at: 2019-04-08T17:22:32.206Z Reads: 91

```
Hi man! How does your build/hub is going? :) still working good??
```

---
## \#43 Posted by: TommyCnc Posted at: 2019-04-25T15:05:34.156Z Reads: 74

```
This unity holder looks perfect for my build, will stick your info up for full credit if I end up using it. Looks great  though either way . Well designed!
```

---
## \#44 Posted by: TommyCnc Posted at: 2019-06-27T19:06:08.934Z Reads: 49

```
![IMG_20190627_175925|374x500](upload://dwhIYLNZQLqJYd0nKlPPXBaYLcF.jpeg)  the 3d pronted enclosure seems to have done the job. I had to strengthen it and the wires once soldered and connected are too tight to squeeze in there but the bullet comnectors fit through the bottom OK if you've got the room.
```

---
