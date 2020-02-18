# DAVEga second batch

### Replies: 45 Views: 1845

## \#1 Posted by: janpom Posted at: 2019-01-25T21:42:06.936Z Reads: 344

```
DAVEga is a gadget that displays various data read from a VESC based controller, such as as speed, remaining battery capacity, and travelled distance. You can read more about it in [this thread](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509). Four display layouts are currently supported -- two graphical in vertical mode, one graphical in horizontal mode, and one text only with detailed information. It's possible to toggle between the layouts with a button.

![davega%20(1)|300x496](upload://myW3bJFXhv96XcxMERw5vpM31cH.jpeg) 

 ![IMG_1583|674x500](upload://8gVFPFNPItBvZGHclIsU3gRqMPC.jpeg) 

![DSC01711|690x460](upload://b5bwg2s8JPcZmUcxRyhaM8LEhe2.jpeg)

 ![IMG_1600|690x498](upload://r2aTmOSVA3bRBNF4AukIOcqONUo.jpeg)

DAVEga is fully open source and anyone is welcome to build their own. Or you can now get two pieces from me -- one assembled and one unassembled -- for more-or-less the cost of the parts and shipping.

## What's in the package

One assembled DAVEga with the following accessories:
- USB-UART adapter (for updating/configuring the firmware)
- buttons
- crimped wires and JST-PH connectors
  - 4 pin (DAVEga side)
  - 7 pin and 8 pin (VESC side; use the one that fits your controller)

![DSC01821|690x484](upload://k9b8V906bVMMt9bHxnH7FkrQuAk.jpeg) 

One unassembled DAVEga with the same accessories:

![DSC01824|690x413](upload://joN2WcdJPeAd9gn9QwjsEFicG3e.jpeg)

## What's NOT in the package

The display! There are various sources. I personally ordered several displays from [here](https://www.aliexpress.com/item/ILI9225-2-0-Inch-UART-TFT-LCD-Display-Module-SPI-Interface-Colorful-Screen-Serial-Port-176x220/32792711665.html) and all arrived and fully functional, so I can recommend this seller.

Note that there are many similarly looking displays that won't work with DAVEga. Make sure that the one you order is **2.0" TFT** using the **ILI9225 driver**.

Pro tip: You may want to order two. :smiley:

 ## Price

* **25 USD**
* or **22 EUR**
* or **550 CZK**

The price includes world-wide tracked shipping from the Czech Republic via the Czech Post.

## Ordering

To order, please PM me and specify the following:

* your full name
* your full address
* your preferred currency
* your preferred payment method (see below)

## Payment methods

PayPal is preferred. Friends & family is much appreciated but not required.

I can also accept payments on my [Revolut](https://www.revolut.com/) account. (May work best for those who don't have USD/EUR/CZK PayPal account since currency conversions on PayPal are expensive.)

## When do I pay?

When I receive your order, I'll send you back an estimate of when I will be ready to ship the Daves to you. Once ready, I'll PM you again with the payment information.

**Please don't send me any money unless explicitly asked for!** :smiley: 

## When will you ship?

I currently have parts for 50 DAVEgas and I have already assembled a few. I should be able to dispatch the first 25 orders relatively quickly (1-2 weeks). Then I need to order more stuff from AliExpress, which means about a month of wait. I will of course backorder prior to completely running out of parts if it looks like there's enough interest.

## Assembly tips
Use the assembled one as a template. 

When soldering the display headers (2x 5 pin header) to the PCB, you may want to plug-in the display first. That keeps the headers in the correct position with respect to each other. If you solder them one by one instead, it's slightly difficult to keep them in a straight line, which may then make plugging-in the display hard to impossible.

Make sure you have the MCU, the diode, and the electrolytic capacitor correctly oriented (there's a black arrow pointing to the negative side). For all other parts, the orientation doesn't matter.

If you don't have JST-PH crimps and/or crimping pliers, unpin the crimped wires from one of the 4 pin connectors and plug them into the 7 or 8 pin connector (depending on what VESC do you have). Then solder them to the wires on the other 4 pin connector (or add extension wires in-between if you need a longer harness).

(More detailed assembly instructions with pictures TBD.)

## Configuring firmware

See the [README](https://github.com/janpom/davega/blob/master/README.md) file in the [DAVEga firmware repository](https://github.com/janpom/davega/).

## Enclosures

Several printable enclosures are available on [thingiverse](https://www.thingiverse.com/search?q=davega) thanks to @mmaner, @lrdesigns, and @JonathanLau1983. 

## How do I ask questions?

If you have any questions about **ordering, shipping, or payments**, please ask in **this thread**.

If you have questions about **DAVEga (assembly, connecting to VESC, troubleshooting)**, please ask in the **[DAVEga thread](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509)**.

**Please do NOT PM me with questions.** I may not be able to respond back to everyone individually.

## FAQ

* Can I order just one?
  * No, sorry.
* Can I order more than two?
  * Not at the moment, sorry.
* I received your package but there was no display. WTF?
  * You may need to read the "What's in the package" and "What's NOT in the package" sections again.
* Are you making a lot of money on this?
  * No. :smiley:
```

---
## \#2 Posted by: AxelF Posted at: 2019-01-25T23:03:36.575Z Reads: 252

```
Id love a unit!

But for clarification (since Im dumb), 2 units for a total of 22 EUR?

Sending a PM with my info. :)
```

---
## \#3 Posted by: janpom Posted at: 2019-01-26T00:09:23.870Z Reads: 237

```
Yes, that's correct. The price is for 2 units, one assembled and one unassembled.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-01-26T14:25:54.742Z Reads: 230

```
Will you release the code which work with your smart bms?
Really would like to have a second DaveGA for my smart bms to constant display the individual cell voltage.
```

---
## \#5 Posted by: janpom Posted at: 2019-01-26T14:30:23.644Z Reads: 219

```
I'll definitely do it, but I don't have it finished yet. Too much work, not enough time. I received so many orders yesterday that I had to staff up. :smiley: 

![DSC01829|635x500](upload://g8ZA5RQW6tpC89jrBfrwuyKA7DU.jpeg)  

![DSC01830|385x500](upload://o3nhi9qhjCE1SL6lhDs51w2Kn7.jpeg) 

We're starting the soldering training tomorrow. :smiley:
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-26T14:31:10.301Z Reads: 203

```
You upgraded your shop fast 😂👌
```

---
## \#7 Posted by: JonathanLau1983 Posted at: 2019-01-26T16:05:49.476Z Reads: 193

```
It's the main reason to have kids right!
```

---
## \#8 Posted by: Mich21050 Posted at: 2019-01-28T13:31:00.474Z Reads: 189

```
Is anybody interested in a 3d printed case?  :smile:
[poll type=regular public=true]
* Yes
* No
[/poll]
```

---
## \#9 Posted by: lrdesigns Posted at: 2019-01-29T01:54:23.231Z Reads: 184

```
@Mich21050 is quick! 

I will be making some SLA prints of my design if anyone is interested?

https://www.electric-skateboard.builders/t/davega-lrdesigns-sla-printed-case/82435
```

---
## \#10 Posted by: gmurad Posted at: 2019-04-09T12:00:56.877Z Reads: 148

```
@janpom Are you still taking orders for this? Last message here is from January so not sure. If so I will PM you with an order.
```

---
## \#11 Posted by: janpom Posted at: 2019-04-09T12:05:06.866Z Reads: 153

```
I am, but I only have parts left for one or two, so you'd better hurry up. :slight_smile:
```

---
## \#12 Posted by: legend27 Posted at: 2019-04-10T15:11:30.854Z Reads: 152

```
Just got mine! Looks awesome! Good job @janpom

Unfortunately the LCD I ordered more than a month ago has still not arrived so won't be able to test it... 

![image|666x500](upload://fyEPqCRK54c17uFxprAj5iN0zwC.jpeg)
```

---
## \#13 Posted by: deucesdown Posted at: 2019-04-21T17:08:32.417Z Reads: 138

```
@janpom if you got any left, I'll take them. I'm finally getting around to assembly, and realized I only have 1!
```

---
## \#14 Posted by: janpom Posted at: 2019-04-21T18:28:31.100Z Reads: 134

```
I'll PM you.
```

---
## \#15 Posted by: RedBaron Posted at: 2019-04-25T16:04:28.725Z Reads: 125

```
I would also like to order a set if and when available. Im not in a hurry and currently gathering parts for my new build.
```

---
## \#16 Posted by: deucesdown Posted at: 2019-04-25T17:45:37.425Z Reads: 124

```
I've arranged for 2 partial sets, but if you haven't sent them yet, I'll be happy to share with redbaron.
```

---
## \#17 Posted by: RedBaron Posted at: 2019-04-25T19:28:09.357Z Reads: 121

```
would much appreciate that! don't mind assembling one at all either.
```

---
## \#18 Posted by: janpom Posted at: 2019-04-25T22:32:39.571Z Reads: 116

```
I actually did send them a few days back. I just forgot to send you the tracking link, sorry. Will do tomorrow. I'm off to bed now.
```

---
## \#19 Posted by: janpom Posted at: 2019-04-25T22:34:06.984Z Reads: 118

```
I'll see what I can still find in my inventory. Will PM you.
```

---
## \#20 Posted by: legend27 Posted at: 2019-05-14T12:57:06.233Z Reads: 110

```
Finally got the screens! Assembly was really easy and basically just plug n’ play afterwards.

Just need a case and it will be ready!

@janpom Your work is just amazing!

![image|666x500](upload://iDj4hYTIDAUpJJgcmNSJK0BxMd8.jpeg)
```

---
## \#21 Posted by: gmurad Posted at: 2019-05-14T13:04:48.235Z Reads: 111

```
Soldering job looked really good on the assembled board. @janpom can you share a bit of your soldering technique? Did you use extra flux or just rosin core solder?
```

---
## \#22 Posted by: janpom Posted at: 2019-05-14T13:27:54.103Z Reads: 115

```
Thanks! No extra flux. (Would be extra work to clean afterwards. :smile:) Just a thin 0.5 mm leaded (60/40) solder with flux core. That with my TS100 soldering iron and the default conical tip and default settings (300 Celsius). I have done quite a few of them now, which was a really good soldering practice.

It's all pretty straightforward. You'll obviously want to start with the smallest components. I typically went in the following order:
- resistor
- diode
- USB-UART female header
- crystal
- 22p and 100n capacitors
- MCU
- 100u capacitor
- JST-PH
- display headers

The display headers are best soldered on with the display plugged in. It's easier.

The USB-UART header is best done by soldering only one pin first; then reheat it with right hand and adjust position with the left hand. Solder the remaining pins last. The same goes for the JST-PH though that one I usually managed to do without having to re-adjust the position after soldering the first pin.

I didn't use any helping hands. I just kept the PCB on a flat surface.

Edit: I recorded the assembly.

https://youtu.be/QPjD0Zebh9U
```

---
## \#23 Posted by: gmurad Posted at: 2019-05-14T13:30:05.970Z Reads: 111

```
Nice, thanks for the breakdown! My TS80 is arriving in the mail today, looking forward to making the second DAVEga using it.
```

---
## \#24 Posted by: briman05 Posted at: 2019-05-14T15:11:15.416Z Reads: 105

```
rosin core sucks only use leaded 60/40 or 62/36/2 silver bearing solder.
```

---
## \#25 Posted by: gmurad Posted at: 2019-05-15T12:17:58.960Z Reads: 100

```
@briman05 Interesting, the general advice on the internet is to use rosin core for electronics. So when you use 60/40 that doesn't have flux in the core right? You add the flux yourself?
```

---
## \#26 Posted by: briman05 Posted at: 2019-05-15T14:10:46.443Z Reads: 99

```
No it has a flux core.  The internet is probably telling you to use lead free rosin core because is it safer health wise but leaded solder is superior
```

---
## \#27 Posted by: gmurad Posted at: 2019-05-15T14:23:46.089Z Reads: 93

```
Makes sense. Leaded 60/40 with flux core. I figure for people that are not soldering every day a little bit of lead is ok, but I could be wrong...
```

---
## \#28 Posted by: briman05 Posted at: 2019-05-15T14:54:31.367Z Reads: 87

```
I have used leaded rosin core and silver bearing rosin core with no issues but non leaded is not as good for electronic work as leaded
```

---
## \#29 Posted by: deucesdown Posted at: 2019-05-15T14:56:10.423Z Reads: 89

```
63/37 is easier to work with. Kester is a good brand.
```

---
## \#30 Posted by: janpom Posted at: 2019-05-15T14:57:16.138Z Reads: 94

```
The fumes from the flux are actually more of a health problem than the lead. Keeping the temperature low reduces the fumes. For PCB soldering I usually do 300 Celsius but I tried going to 270 and that worked just fine as well. If possible, keep the window open while soldering and/or breath out when making a solder joint.
```

---
## \#31 Posted by: deucesdown Posted at: 2019-05-15T15:52:25.369Z Reads: 97

```
Found a monster summary post for solder wire at eevblog.

https://www.eevblog.com/forum/reviews/an-other-post-for-good-solderwire/msg655700/#msg655700
```

---
## \#32 Posted by: janpom Posted at: 2019-05-19T15:59:07.762Z Reads: 98

```
I have 5 last assembled DAVEgas that I'd like to let go. I won't be making any more kits. I also have 3 extra displays. Price:

- $16 - assembled DAVEga + USB-UART adapter + 4 simple buttons + parts for making a harness
- $7 - display
- $6 - shipping to EU, $7 to outside EU

![IMG_1961|666x500](upload://yhXJfSSLiz8bSHFrhLi2PNdvbqC.jpeg) 

@bonesaw @Ricco @MrFidgety @AlMcCal
```

---
## \#33 Posted by: PickSix24 Posted at: 2019-05-19T16:21:35.414Z Reads: 98

```
@janpom still working on a larger Dave ?
```

---
## \#34 Posted by: Mudders Posted at: 2019-05-19T16:25:46.937Z Reads: 96

```
Could I buy 2 please @janpom ?
```

---
## \#36 Posted by: janpom Posted at: 2019-05-19T17:15:47.019Z Reads: 98

```
Yes, I am. @LRDesigns designed a nice enclosure for it. We'll have it CNC-ed in aluminum and it will be super sexy. The bigger display won't be the only improvement. I'm completely rewriting the code for the ESP32 platform and adding a lot of new features. There's still a lot of work to be done though. I suppose it will won't be before 3-4 months until you can buy one. The price will be quite a bit higher than the current DAVEga but I hope we'll be able to keep it below $100 including the enclosure. No more spoilers for now. :slight_smile:
```

---
## \#37 Posted by: PickSix24 Posted at: 2019-05-19T20:06:43.219Z Reads: 92

```
Can’t wait !!
```

---
## \#38 Posted by: High-roller Posted at: 2019-05-20T05:34:32.156Z Reads: 92

```
Are there any more available with the screen?
```

---
## \#39 Posted by: janpom Posted at: 2019-05-20T05:55:54.425Z Reads: 95

```
No, sorry. I have last two without displays.
```

---
## \#40 Posted by: High-roller Posted at: 2019-05-20T06:03:05.463Z Reads: 94

```
Okay, I'll take one please. I'll PM you in a little bit.
Can you please link the correct screen again?
```

---
## \#41 Posted by: louwii Posted at: 2019-05-20T08:06:55.914Z Reads: 97

```
I'll get one if any left, assembled or not, screen or not. Will pay in USD via Paypal, shipping to Canada. :)
```

---
## \#42 Posted by: janpom Posted at: 2019-05-21T10:46:39.414Z Reads: 88

```
All sold out now, sorry.

Working hard to get the new, better and sexier Dave to you ASAP though. :slight_smile:
```

---
## \#43 Posted by: 0Z3M0 Posted at: 2019-05-27T19:43:38.096Z Reads: 82

```
Frick! found this thread too late :sweat_smile: I need this :grinning:
```

---
## \#44 Posted by: Okami Posted at: 2019-05-28T18:33:59.918Z Reads: 73

```
Flipsky is selling these for 35usd + shipping
```

---
## \#45 Posted by: Komamtb Posted at: 2019-08-16T09:13:53.105Z Reads: 47

```
would it be possible to buy a flipsky one, but make it work in horizontal orentation and use a case from our member?
```

---
## \#46 Posted by: bilkenter Posted at: 2019-08-29T06:11:41.701Z Reads: 43

```
I would like to order too. When it is going to be available?
```

---
