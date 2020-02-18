# Enertion FOCBOX Teardown &amp; Internals

### Replies: 29 Views: 3601

## \#1 Posted by: JdogAwesome Posted at: 2018-01-03T04:58:30.287Z Reads: 536

```
This is just a simple teardown and overview of the internals of the Enertion FOCBOX, its similar to my [Shred Lights Review](https://www.electric-skateboard.builders/t/shred-light-teardown-and-internal-review/). Starting off I ordered mine during the Cyber Monday sale like a lot of people on 11-26 and received them on 12-23 so just under a month from China which is pretty good being it was with the free shipping. However the tracking number I received was either wrong or didnt work because no tracking web service could find it. Im sure I could have contacted Enertion about this but I thought I would just give it some more time until eventually a box showed up with a different tracking number and I had my FOCBOX's. Overall the packaging was decent just some standard bubble wrap in a small box so no complaints there, pic below.
<img src="/uploads/db1493/original/3X/3/2/32457b31d4d58c21091909ebefe8970604d307c1.jpg" width="690" height="389">

The actual ESC's themselves look just beautiful compared to your normal bare board VESC with its plastic top and milled aluminum bottom. I also really appreciate the sticker labeling all the pins and LED's which is a nice touch especially for beginners, and the MICRO USB port is a wonderful change which I welcomed with open arms compared to the standard mini usb trash, I do however wish the port protruded out farther as its relatively hard to plug some cables into it. The addition of the servo cable coming right out of the box for connecting straight to a receiver is another nice touch especially for beginners as well. The housing is held together with three M3x8 screws which go through the top plastic housing, pcb and into the metal bottom. The ESC is designed to have all the FET's on the bottom side to dissipate all the heat through the metal heatsink and uses a piece of thermal tape in between. For the input it comes with a female XT60U-M which is just a slightly shorter version of your standard XT60 female plug and it works fine with normal XT60's. The motor phase wires are 3.5mm bullets which like others have stated are a weird size as most motors are 4mm bullets, but I just ordered some 3.5mm male bullets and soldered adapters together for my 4mm motors. Making adapters is usually far easier than trying to solder bullets onto copper wire. The FOCBOX also weighs in at 105 grams, which I cant compare to anything else as I never weighed my VESC's. On the bottom of the FOCBOX there are four M3x4 Mounting holes which are 30mm wide and 15mm tall which I suppose you could use for mounting to a larger heatsink or maybe an enclosure, idk.

<img src="/uploads/db1493/original/3X/c/5/c589147f857392643a638129e63c2672c4171d79.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/7/2/7219cbf9c3aacc5183bbfb0492f6801a151f0f97.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/0/f/0f1349c81c952b2596ecca045c22b0d00f93ccb9.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/b/e/be50bad4c02993255c90705634ec6208db1769a7.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/3/0/30f4c262782f9210d71ea3e01ab9d56a2b48acc2.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/9/e/9e3df15fa3e992749f77212f3aaac39a60e5ca3b.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/8/6/86156609a7f42f8ffe4e9d74e29712b6cc235ba1.jpg" width="690" height="389">

Moving onto the best part, the actual internals and electronics inside. To start the FOCBOX has two 680uF 63V Nichicon Caps compared to for example my Maytech VESC which has three 680uF caps, but I think that still 1360uF is plenty. For the most part everything's the same as the VESC 4.12 on the FOCBOX other than the shape and DirectFET's but there are still a few smaller changes. For example the TVS diode seems to be different though I cant find any information on the one in the FOCBOX, its labeled as GFZ 74A though if anyone can find any info on it. Other than that all the other parts seem the same [DRV8302](http://www.ti.com/lit/ds/symlink/drv8302.pdf), [STM32F4](http://www.st.com/content/ccc/resource/technical/document/datasheet/ef/92/76/6d/bb/c2/4f/f7/DM00037051.pdf/files/DM00037051.pdf/jcr:content/translations/en.DM00037051.pdf) MCU, [SN65HVD232](http://www.ti.com/product/SN65HVD232) Can Transceiver, etc. The MOSFET's are [IRF7749's](https://www.infineon.com/dgdl/irf7749l2pbf.pdf?fileId=5546d462533600a40153560445e71ca2) with a max Vdss of 60V which works though I would have prefered to see maybe the [IRF7759](https://www.infineon.com/dgdl/irf7759l2pbf.pdf?fileId=5546d462533600a40153560478171cb0) though it has a higher RDSon of 1.8mOhms compared to the 1.1mOhms of the 7749 so I can see why they went with it. Another thing to point out is the silicone all around the capacitors and main power leads which I actually like a lot because it seems to keep everything together quite well. You might also notice the white gunk on the TVS diode near the MOSFET's which its actually like on all my FOCBOX's or at least to some extent.
<img src="/uploads/db1493/original/3X/4/3/434a01c542c8eae6c2fe60fb5a5a973b66108159.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/3/c/3c1217d95c8be641a3110fbc59e6f409a5e68244.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/8/a/8ae2a7bec71756419554cba8d6ae19665a0f33f7.jpg" width="690" height="389">

Last but not least I heard some people talking about whether or not the FOCBOX has a conformal coating which I can confirm it does not. Its not a big deal as if water is getting into your enclosure you probably have bigger problems then messing up your ESC though it would have been a nice feature, nonetheless I added my own coating of MG Chemicals Acrylic Conformal Coating. First pics are the before with a blacklight and last pics are after the coating was applied.  
<img src="/uploads/db1493/original/3X/2/0/202e8c03036067ab88a9ecfb58297b353aba1eb6.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/e/6/e676cdf5d3a993887e9126ba201eb484c76f3b55.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/5/7/57544d8849fcff608a867d2cfe64a12349d2f1bc.jpg" width="690" height="389">
<img src="/uploads/db1493/original/3X/7/2/722a39466c729699a9d599d802a41e1141c34acb.jpg" width="690" height="389">

Overall the FOCBOX is a great ESC and I cant wait to test it out on my board once it gets a little warmer out, its currently about 5°F in Chicago right now, but once I do ill either update this post or add a reply. FOCBOX Schematics can be found [HERE](http://www.enertionboards.com/how-to-build-eboard/vesc-x-design-files/) on the Enertion website. Also if I missed anything or if there's anything you'd like added for example a feature or part I missed about the FOCBOX please let me know and I will add it!
```

---
## \#2 Posted by: Luuke Posted at: 2018-01-03T09:53:05.903Z Reads: 451

```
Thank you for the review! I am still waiting for mine...
I can't tell you which TVS is in the Focbox, but the VESC6 uses this one:
60V Shotkey
https://www.arrow.com/en/products/pmeg6020er115/nexperia
&
5V TVS
https://www.arrow.com/en/products/smaj5.0a/littelfuse

E: I am wrong! Seems like both are used for the 5V supply. Even the 60V one!
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2018-01-03T13:44:32.311Z Reads: 407

```
DID you put conformal coating over the Mosfet ???
```

---
## \#4 Posted by: mikenyc Posted at: 2018-01-03T13:52:31.554Z Reads: 391

```
:fire: 10char
```

---
## \#5 Posted by: longhairedboy Posted at: 2018-01-03T13:55:37.687Z Reads: 370

```
@JohnnyMeduse is right... you don't want that on the fets themselves. The fets should be in direct contact with the thermal tape.
```

---
## \#6 Posted by: Deckoz Posted at: 2018-01-03T14:46:35.909Z Reads: 355

```
Acrylic Conformal coating on fets does not prevent heat dissipation. It's also the only thing that can protect fets from water. Oil based sealants don't work for fets. 

Only use acrylic based conformal coating on fets, silicon conformal coating is to thick and will trap heat, and oil based(corrosionX) will not prevent water damage.

/Been conformal coating fets for over a decade.
```

---
## \#7 Posted by: shanewill1234 Posted at: 2018-01-03T15:28:27.709Z Reads: 333

```
You're lucky, I ordered a couple FocBoxs as well on Nov 28th and just got an email yesterday saying that they have to make more with a new manufacturer to fulfill all the backorders they have.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2018-01-03T15:51:39.703Z Reads: 325

```
Well... 

I don't want to say that conformal coating (event the acrylic one) won't work because it could work, but it could also reduce the thermal performance of the fet and heat sink. And since it hasn't been tested by Enertion over their product, if something blow up it could be seen as a void of waranty. 

http://www.circuitnet.com/experts/86511.html
```

---
## \#9 Posted by: PXSS Posted at: 2018-01-03T16:23:02.144Z Reads: 313

```
They are talking about something different there. 
The op on that link was asking about coating over the heatsink itself which is a bigger hindrance than between the heatsink and component. 

I agree though, there are a few thermally conductive conformal coatings but from my research acrylic isn’t one of them. MG chemicals doesn’t list the thermal conductivity of their stuff on the tds and I assume it’s not very high. 

I have never covered any component that is meant to dissipate heat.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-01-03T16:26:04.155Z Reads: 289

```
Sure, it could void the warranty. But your also talking about a coating applied properly should be less then 0.15mm thick.  Or 150microns. While the coating is low in heat conductivity, a few microns will be negligible when talking about percentages of a degree.

As well the manufacturer warranty is only good for 60 days, the purchasable year long warranty supports all user modifications with the exception of SMD component changes according to the wording.

It's the same argument as electrically insulating your packs with kapton. Protection > negligible temp variance.
```

---
## \#11 Posted by: JdogAwesome Posted at: 2018-01-03T17:13:21.616Z Reads: 280

```
Hey @JohnnyMeduse @longhairedboy @PXSS I did cover the FET's in a thin layer of the coating but I tried to keep it thin and only did one coat unlike how I do two coats on some areas, ie DRV and MCU. I have coated MOSFET's and other components connected to heatsinks before with thermal compound in-between and I haven't seen any noticeable difference. I will however test this out because it's a good point so I'll let everyone know with my findings! And the main reason I covered the top of the FET'S was for corrosion resistance because they are metal unlike normal D2PAK's which are plastic.
```

---
## \#12 Posted by: Quiles Posted at: 2018-01-03T22:20:45.866Z Reads: 265

```
what's the big difference from a TB VESC for example, in your perspective. Why FOCBOX is so realiable compared to others...
```

---
## \#13 Posted by: b264 Posted at: 2018-01-03T22:28:08.748Z Reads: 266

```
[quote="JdogAwesome, post:1, topic:42633"]
the TVS diode seems to be different though I cant find any information on the one in the FOCBOX, its labeled as GFZ 74A though if anyone can find any info on it.
[/quote]

Looks like a [SMCG51A](https://www.mouser.com/ProductDetail/Vishay-Semiconductors/SMCG51A-E3-57T/?qs=cuN208rz%2FQ%2F9o%252bWPZPtznw%3D%3D) possibly
```

---
## \#14 Posted by: JdogAwesome Posted at: 2018-01-03T22:56:41.918Z Reads: 262

```
You can find all the main differences on the thread by Onloop [HERE](http://www.electric-skateboard.builders/t/new-improved-focbox-official-thread/). It states that the main differences are DirectFET package MOSFET's which greatly improve thermal transfer and make it so the FOCBOX can handle higher currents than a VESC. Increased number of decoupling capacitors, which you can see on the top of the PCB near the shunts, to improve reliability in FOC I assume as well as a Micro USB port and some other changes. And I think maybe the biggest difference is the device itself, it really feels like an actual product and not some DIY raw PCB that has so many exposed pads. The metal and plastic case really gives it a lot of protection and like Enertion said makes it far more manufacturable than your normal VESC.
```

---
## \#15 Posted by: Quiles Posted at: 2018-01-03T23:52:41.960Z Reads: 244

```
great review! Thanks for the link.
```

---
## \#16 Posted by: JdogAwesome Posted at: 2018-01-07T05:11:08.557Z Reads: 256

```
@JohnnyMeduse @longhairedboy @PXSS @Deckoz

Alright guys so finally got around to testing the thermal conductivity of the Acrylic conformal coatings! Let me start by saying that a single layer of the coating does absolutely nothing to the thermal transfer. To test this I used a internally shorted IRLZ44N MOSFET attached to a small heatsink drawing 12.5W. I first tested without any coating at all just screwed together and recorded the temps at different time intervals of 15s, 30s 1m, 2m and 2m 30s. The second test was with a single normal thickness coat that was thick enough to electrically isolate(tested with multimeter probes). I was planning on doing 2 coats as well as 3 and so on until I started seeing a difference, until my MOSFET suddenly stopped being shorted so I need to find a different way of testing this. I plan to figure out a new method of testing tomorrow and start again. Anyways below is my test data, pics are of the simple setup and measurements where taken from the center of the back of the heatsink.

ACC Thermal Transfer Test: 

Power: 12.5W 
Control Temp: 28C 

No Coating: 
15 seconds: 35.5c 
0-15s: +7.5c
30 seconds: 50.5c 
15-30s: +15c
1 minute: 73c
30-60s: +22.5c 
2 minutes: 104.8c
60-120s: +31.8c
2 min 30 sec: 115c
120-180s: +10.2c 

1 Coating: 
15 seconds: 39.5c
0-15s: +11.5c
30 seconds: 51.5c
15-30s: +12c
1 minute: 75c
30-60s: +23.5 
2 minutes: 106c
60-120s: +31c 
2 min 30 sec: 115c 
120-180s: +9c

<img src="/uploads/db1493/original/3X/4/c/4c227c6117dfef5c03d81fb2dcdbaf19ae3a7e09.jpg" width="690" height="389"><img src="/uploads/db1493/original/3X/4/5/45120eca12c1f9a94f7b5263506ca4f9f55dd58c.jpg" width="690" height="389">
```

---
## \#17 Posted by: Deckoz Posted at: 2018-01-07T13:32:42.240Z Reads: 227

```
[quote="JdogAwesome, post:16, topic:42633"]
Let me start by saying that a single layer of the coating does absolutely nothing to the thermal transfer.
[/quote]

Exactly as I said it would be fine ;)
You have the tests well laid  out too!
```

---
## \#18 Posted by: longhairedboy Posted at: 2018-01-07T18:29:56.026Z Reads: 222

```
based on what i'm reading here this test proves that a thin coating limits the heat transfer by as much as a full 2 degrees C in some situations over the same time interval. So while the final temps are the same, the transfer rate is indeed throttled.

It does do more than exactly nothing.  Little more, but more.
```

---
## \#19 Posted by: JdogAwesome Posted at: 2018-01-07T18:35:06.299Z Reads: 226

```
Well looking at the 0-15S interval the coated transfer is 4c higher, the 30-60s interval is also higher with the coating as well. This is why I'm going to redo all the tests again and do them multiple times because this premlinary test seems a little odd.
```

---
## \#20 Posted by: SOICDIP Posted at: 2018-01-07T18:54:08.020Z Reads: 227

```
[quote="JdogAwesome, post:19, topic:42633"]
This is why I'm going to redo all the tests again and do them multiple times because this premlinary test seems a little odd.
[/quote]

What were you using to measure the temperature?

Also, can you test with a thermal bad between the FET and the heatsink to replicate conditions of the FOCBOX?
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2018-01-07T19:39:23.124Z Reads: 212

```
[quote="JdogAwesome, post:19, topic:42633"]
This is why I'm going to redo all the tests again and do them multiple times because this premlinary test seems a little odd
[/quote]

And Maybe It could be a good Idea to add a gad pad between the Mosfet and the heatsink, like the scenario inside the focbox. Because I think the gap pad doesn't transfer 100% of the heat, so by adding some conformal coating, it could restraint the heat transfer ability of the Gap Pad.
```

---
## \#22 Posted by: JdogAwesome Posted at: 2018-01-07T19:56:54.657Z Reads: 203

```
@SOICDIP @JohnnyMeduse Yep I was planning on doing that as well, its going to be very in depth and probably gonna make a thread about it separate from this.

@SOICDIP Im currently using a handheld infrared thermometer which seems to be quite accurate and have very repeatable results, though im going to test out using a thermocouple and thermistor as well.
```

---
## \#23 Posted by: louwii Posted at: 2018-01-20T10:21:42.872Z Reads: 185

```
What's the JST sensor connector pitch ? 2mm? 2.5mm?
I have a motor with a JST sensor connector but it's super tiny, 1.25mm pitch I believe. I wonder why they used one that small if VESCs don't use connectors that small.
```

---
## \#24 Posted by: scepterr Posted at: 2018-01-20T10:50:45.295Z Reads: 185

```
Why not just cut little squares of kapton or any masking tape to just cover the top, this way you can coat everything necessary still. Get tape the width of the fet so you only have to cut the length.
```

---
## \#25 Posted by: Jumpman Posted at: 2018-01-20T11:03:32.037Z Reads: 186

```
Yep, JST PH 2.0mm 6pin.  I guess most motors aren’t designed for the Vesc, maybe it is more common on RC speed controllers.

One good thing is you can you use the jst ph 2.0mm 6 pin cable for wiring a Bluetooth module, although 7 pin is ideal.
```

---
## \#26 Posted by: stormboard1 Posted at: 2018-01-22T21:59:23.981Z Reads: 178

```
is corrosion x good for a conformal coating?
```

---
## \#27 Posted by: Deckoz Posted at: 2018-01-22T23:57:59.046Z Reads: 174

```
corrosionX is a hydrophobic antioxidation oil. It's good but it won't do anything to protect FETs from shorting. 

Also corrosionX x never dries it's always a liquid

Conformal coatings(silicon and acrylic) harden and make a physical barrier where corrosionX is a hydrophobic barrier
```

---
## \#28 Posted by: Kug3lis Posted at: 2018-01-23T00:48:09.168Z Reads: 167

```
I just saw this and just wanted to tell to try it out with DirectFET package before making decision, I read in DirectFET case application notes they have really specific requirements as they don't have any heat body buffer like your to220 which has massive case compared to DirectFET, and I think this can cause some problems, so I suggest to try it out :slight_smile:
```

---
## \#29 Posted by: pixelsilva Posted at: 2018-01-23T18:57:42.236Z Reads: 146

```
Say again?
```

---
