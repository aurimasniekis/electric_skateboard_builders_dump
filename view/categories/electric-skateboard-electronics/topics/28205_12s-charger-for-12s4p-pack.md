# 12S charger for 12s4p pack

### Replies: 33 Views: 4272

## \#1 Posted by: pshaw Posted at: 2017-07-21T15:06:55.238Z Reads: 559

```
Gents,

Looking for some charger options for a 12s4p battery. If possible I'd like to have 12A charging capability but I feel those might get expensive. 

This is the one that has been recommended to me which can do 4A but there but the minimum shipping cost to the USA IS 75 dollars! 

http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html


Thanks!
```

---
## \#2 Posted by: jmasta Posted at: 2017-07-21T15:55:57.590Z Reads: 543

```
12A?  Holy amperes, batman.  That equates to 600W!

12A is going to put a significant stress on your cells, if you could even find a charger that huge. It is better to charge at a slower rate. Generally it is recommended to charge at 1C or less (e.g., charge a 5Ah pack at 5A or less)

I charge my 12S battery at 4A and that is plenty
```

---
## \#3 Posted by: pshaw Posted at: 2017-07-21T15:56:44.786Z Reads: 529

```
My 12S4p pack will be 12A. So it WILL be 1C charge :)
```

---
## \#4 Posted by: jmasta Posted at: 2017-07-21T16:01:29.407Z Reads: 511

```
If you really want a 12A charger (...you don't), here's a bad idea on how to make one:

1. Buy three identical 4A chargers
2. Wire the DC outputs in parallel (4A x 3 = 12A)
3. Plug the three AC inputs into a power strip
4. Charge at 12A!
5. Destroy battery
6. Profit?
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-07-21T16:02:04.276Z Reads: 487

```
yea i just don't know if an off the shelf 12amp / 50.4v charger really exists.

your best bet will be a 12s balance charger, my 10s balance charger goes up to 10amp.  or some scientific / industrial grade constant volt / amp power source, but that'll probably super expensive.
```

---
## \#6 Posted by: pshaw Posted at: 2017-07-21T16:03:07.389Z Reads: 486

```
@jmasta You didn't read my post. I won't be charging over 1C


@thisguyhere I have a BMS so balance charger wouldn't work right?
```

---
## \#7 Posted by: jmasta Posted at: 2017-07-21T16:21:30.840Z Reads: 481

```
@pshaw Just because the cells _can_ be fast charged at 1C doesn't mean it is good for them.  A standard charge is 0.5C. Higher charge rates adversely affect the life of the cell

I would recommend charging your 4p pack at **6A or less**   (=4x 1.5A)

Assuming these are your batteries:

<img src="/uploads/db1493/original/3X/d/b/dbad81c68e33e9b492d0b29956a3fe439b9357da.png" width="460" height="499">
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-07-21T16:40:45.893Z Reads: 445

```
[quote="pshaw, post:6, topic:28205"]
I have a BMS so balance charger wouldn't work right?
[/quote]

yea you've got a bms, no balance charger then.

like @jmasta said, you shouldn't be charging at any more than 0.5c so...just stick with a 4amp charger.

i've been charging my 12s4p pack with a 2amp brick charger, and while it takes a while, you can just plug it in and forget about it since you've got a bms.
```

---
## \#9 Posted by: jaykup Posted at: 2017-07-21T20:19:49.081Z Reads: 433

```
Go with a MeanWell LED driver.  Fanless, waterproof, metal construction - 

HLG-600H-48A - $170
 - Adjustable voltage 40.8 to 50.4v
 - Adjustable Amperage 6.2A to 12.5A
 - Charging Power - 600 watts

HLG-600H-54A - $170
 - Adjustable voltage 45.9 to 56.7v
 - Adjustable Amperage 5.6A to 11.2A
 - Charging Power - 600 watts

http://www.meanwell.com/webapp/product/search.aspx?prod=hlg-600h

I have the 185 watt version HLG-185H-48A (4A charger @ $45 USA shipped) and it works awesome.  I like it because you can slightly undercharge the cells for much longer cycle life, or crank it up to the full 4.2v per cell.  Would take 2.5 to 3 hrs to charge your pack.

It charges at CC then CV to float it off.

All sizes:

http://www.meanwell.com/product/led/LED.html
```

---
## \#10 Posted by: pshaw Posted at: 2017-07-21T21:14:18.106Z Reads: 393

```
Fantastic! Any idea if there is a place in the US I can buy a BMS that supports 12S too? That would be super helpful!
```

---
## \#11 Posted by: smurf Posted at: 2017-07-21T21:35:45.771Z Reads: 379

```
http://ebay.com/itm/44V-48V-50-4V-12S-60A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System-/221644780045
```

---
## \#12 Posted by: pshaw Posted at: 2017-07-21T22:21:29.864Z Reads: 367

```
Ships from China. :p @smurf
```

---
## \#13 Posted by: pshaw Posted at: 2017-07-21T22:49:40.476Z Reads: 362

```
@jaykup is that a power supply or only a charger. It has 3 wires coming out of the output it looks like.  Sorry but exactly sure how this works haha
```

---
## \#14 Posted by: jaykup Posted at: 2017-07-22T00:50:14.367Z Reads: 358

```
It's technically a power supply but works great as a charger.

**EDIT: post below doesn't apply to the 600w version, only the 80-320w versions**

**see http://www.electric-skateboard.builders/t/12s-charger-for-12s4p-pack/28205/27 for the 600w explanation**

One end is for AC 110v input, so it has 3 wires.  Hot, Neutral and Ground.  Just cut an extension cord or old computer power cord and solder/join together.

<img src="/uploads/db1493/original/3X/d/9/d990b68232814f88229d747b2b6b5307d1f15ee1.jpg" width="281" height="500">

The other end is the DC Out and just has two wires, positive and negative.  Solder a connector that can plug into your battery (in this case I used an XT90).

<img src="/uploads/db1493/original/3X/6/3/63653967e9dff7708eab4cbcc8243d83f018ebb5.jpg" width="281" height="500">

Plug it in and measure the DC Out with a volt meter.  Turn the V Adjust screw on the top (under the rubber plug) until the volt meter reads the desired voltage (50.4 for 12s charging to 4.2v per cell).

Then plug it in and let it charge!
```

---
## \#15 Posted by: pshaw Posted at: 2017-07-22T01:12:52.816Z Reads: 325

```
Exactly what I needed to know. Thanks!
```

---
## \#16 Posted by: Titoxd10001 Posted at: 2017-07-22T02:09:43.674Z Reads: 321

```
What would be the difference between the models. Someone has a clg-150-48 and they mentioned it gets hot. Is the hlg model better? Trying to get a charger for 12s
```

---
## \#17 Posted by: pshaw Posted at: 2017-07-22T02:16:06.959Z Reads: 323

```
@Titoxd10001 a charger getting hot isn't necessarily a bad thing.
```

---
## \#18 Posted by: Titoxd10001 Posted at: 2017-07-24T20:41:19.622Z Reads: 313

```
About to purchase a charger either hlg-185h-48 or hlg-240h-48. They should both work for 12s correct? Also can I charge without bms, the charger will shutoff automatically if I set it to 4.1v per cell?
```

---
## \#19 Posted by: jaykup Posted at: 2017-07-24T22:13:16.402Z Reads: 309

```
Correct both will work.  Both will shut off at the max voltage set on the charger. So for 4.1 at 12s set to 49.2v.  Will work without bms, should work with it.
```

---
## \#20 Posted by: Titoxd10001 Posted at: 2017-07-25T00:46:13.458Z Reads: 305

```
Awesome thanks
```

---
## \#21 Posted by: DilatedPupils Posted at: 2017-07-25T06:35:11.605Z Reads: 283

```
Oh just what I'm looking for. 5a sounds good.
Where are you getting yours from @Titoxd10001?
```

---
## \#22 Posted by: Titoxd10001 Posted at: 2017-07-25T16:08:03.430Z Reads: 274

```
Looking at a couple places but it's hard to figure shipping/taxes. The 185h, there's some cheap ones on eBay. I'm thinking of even getting the 240h or 320h tho
```

---
## \#23 Posted by: DilatedPupils Posted at: 2017-07-25T17:25:50.472Z Reads: 275

```
I was thinking of getting the 240 for 5a charging. I'll be using it for 10Ah lipo so the 185 would take a longer to charge.
```

---
## \#24 Posted by: Titoxd10001 Posted at: 2017-07-25T21:19:30.696Z Reads: 265

```
Yeah I'm thinking between 240 or 320 for 12AH pack. Make sure you use bms for lipo
```

---
## \#25 Posted by: DilatedPupils Posted at: 2017-07-25T22:03:22.476Z Reads: 260

```
Yeah. I have bestech bms coming.
```

---
## \#26 Posted by: jaykup Posted at: 2017-07-26T01:58:53.952Z Reads: 267

```
I created this spreadsheet a while back when deciding which charger to go with for a 12s4p pack, 2500 mah cells, 480 watt hours.

<img src="/uploads/db1493/original/3X/d/a/dac48c0b1ed922ff6de047b665eaa046a2bcb43f.png" width="690" height="102">

The 185 is quite a bit lighter than the 240 and the 320 is much heavier.  I was thinking I wanted portability, so I could throw it in a backpack.  Ive done that a few times, but found it wasn't as important.

I have enough range I really only charge overnight, so speed wasn't as critical as I originally thought.

Just things to consider when selecting a charger.
```

---
## \#27 Posted by: jaykup Posted at: 2017-07-26T02:34:19.348Z Reads: 257

```
Sorry I didn't answer this question correctly the first time.

I took a closer look at the 600w version and it's setup different than the other versions (80-320w versions).  

The 3 wires coming out of the output: 
 - Two of them are DC output cables each with their own positive and negative.  They are 14awg wires so they should be able to handle 20a each.  The lower voltage chargers output a lot more amps, so maybe both are needed in parallel, but on the 48v version is only 12a so one should be enough.  However, It's unclear if this unit is essentially two power supplies in one case.  If that's true, both DC output lines need to be attached in parallel.  I would recommend testing this with an amp meter to verify one line can give 12a before doing a parallel configuration.
 - The third wire is an RC+/RC- input and is specific for LED lights.  This can be ignored and not attached to anything.

http://www.meanwell.com/webapp/product/search.aspx?prod=hlg-600h

Finally, make sure to get the HLG-600H-48A model.  The "A" at the end stands for adjustable.  The models without the A, or with the B are either not adjustable or have dimming features that are not necessary for bulk charging.
```

---
## \#28 Posted by: pshaw Posted at: 2017-07-26T02:54:39.062Z Reads: 240

```
Thanks for all the help guys! I actually just ended up going the easy route and bought the 4A charger for liek 50 bucks. I figure 3 hours to charge isn't terrible when you have 20mi range :stuck_out_tongue:

I a pinch I could charge an hour and still have 8 miles that quick
```

---
## \#29 Posted by: Titoxd10001 Posted at: 2017-11-18T05:10:44.582Z Reads: 214

```
Ended up getting the hlg-320h-48a. It doesn't have any leds so was wondering how do you know the charge is done? Was thinking of adding voltmeter just to know it's on lol. It reached end voltage but seemed to stay on until I unplugged it. If I leave it plugged it say overnight it should still be okay right. Still need to try upping to the rated 6.7A
```

---
## \#30 Posted by: jaykup Posted at: 2017-11-19T01:05:31.620Z Reads: 208

```
Yeah the charger is just a bulk "brute force" type of charger.  It doesn't have any intelligence for these batteries specifically.  Leaving it charging overnight is no issue, it will charge to the max voltage you have the power supply set to then just sit there, slowing dropping amperage along the way until it reaches 0.  It does charge the way lithium ion batteries like to be charged (CCCV).

I just feel the charger, if it's cool I know it's done.  I've also calculated how long it should take to charge (~3hrs) so I know roughly when it will finish.  Most of the time, however, I just leave it on overnight.

Side note, and not a big deal - If you plan is to regularly charge overnight, reduce the amperage to get longer battery cycle life (total lifetime in years).  If you want to charge it quickly then max the amperage.
```

---
## \#31 Posted by: Titoxd10001 Posted at: 2017-11-19T03:04:00.043Z Reads: 201

```
Okay good to know. Might get a voltmeter/ampmeter someone suggested on different thread to also monitor amps. Seems like a solid "charger "
```

---
## \#32 Posted by: Ronny_CTS Posted at: 2017-11-19T09:20:31.816Z Reads: 197

```
@jaykup i have a question i hope you can answer me. 

I was looking at the [data sheet](http://www.mouser.com/ds/2/260/HLG-320H-spec-226092.pdf) for these Meanwheel chargers and i see that the depending on the model the constant current range varies. 
Example: 
HLG-320H-48 - CONSTANT CURRENT REGION - 24 ~ 48V
HLG-320H-54 - CONSTANT CURRENT REGION - 27 ~ 54V

So if i want to charge a 12S battery to 49.2V (4.1V per cell) with the HLG-320H-48 charger, it will only charge to 48V at CC and then switch to CV. 

Shouldn't the battery be charged all the way up to to 49.2V at CC and then switch to CV to finish charging?
```

---
## \#33 Posted by: jaykup Posted at: 2017-11-19T13:40:21.586Z Reads: 198

```
My understanding:

These chargers are meant for full amperage at 48v.  If adjusted to their max voltage of 52v, it will still perform in CC to 52v then CV mode to maintain 52v, but the output amperage won't be as high as the rated amperage beyond 48v.

For example:

321W (Rated) / 48V (Rated) = 6.7A (Rated)
321W (Rated) / 52V = 6.17A

As the battery pack voltage goes beyond 48v you are going to want to/have to limit current anyway to "top off" the pack, so I didn't see this as a major issue.  The reason I went with the 48v version was that I wanted to build a second board that was 10s and use the same charger.  I think if you were dedicated to 12s only (or higher for ebikes) then the 54 makes more sense.

Somewhat relevant data, though not everyone in that thread is clear on what the original question really is:
https://electronics.stackexchange.com/questions/285359/question-about-constant-current-region-and-voltage-adjustment
```

---
