# Using 12 pin SP21 connector to avoid BMS

### Replies: 7 Views: 349

## \#1 Posted by: janpom Posted at: 2018-12-25T22:05:39.667Z Reads: 71

```
I don't like the idea of a charge-only BMS for the reasons [I mentioned here](https://www.electric-skateboard.builders/t/cheap-diy-12s-balance-charger-idea/76695?u=janpom). There are various alternatives to a charge-only BMS, but to do it right you need access to the balance wires.

I recently purchased the [Vera build](https://www.electric-skateboard.builders/t/first-build-vera-evo-36-dual-foc-6355-190kv-10s5p-30q-107mm-metr-pro/58551) from @brenternet, which included a cheap bypassed BMS that soon stopped working for an unknown reason. So I removed it and started working on the no-BMS setup that I have long thought about. This is a quick report on my progress so far.

I noticed that some people use the 2 pin SP21 waterproof connectors. They also come in the [12 pin version](https://www.electric-skateboard.builders/t/first-build-vera-evo-36-dual-foc-6355-190kv-10s5p-30q-107mm-metr-pro/58551), which is one pin short for 12S, but my battery is only 10S, so I thought I'd give it a go. The connector is rated 5A, which is enough for charging (at least for me). For 12S or for faster charging, one could use the 12 pin connector only for the balance wires and use a [2 pin SP21](https://www.aliexpress.com/item/SP2110-2-pin-waterproof-Connector-Male-Female-21mm-Panel-installed-connectors-LED-monitor-connector-IP68-Current/32650587083.html?spm=a2g0s.9042311.0.0.27424c4drMCRgU) in addition to that.

On to the process. I first soldered 22 AWG wires on the connector part that goes inside the enclosure. 22 AWG is the max gauge I would recommend. I used 20 AWG on the outside part (which has the same kind of wire connectors) and that's already a bit too much to solder on comfortably, though it still can be done (I only used 20 AWG because I ran out of 22 AWG; also for science, of course).

![DSC01723|690x460](upload://kB0OwuwP5SUbj2LjtdEROUlb7Nm.jpeg) 

![DSC01725|690x460](upload://dQUma8E5INupWm55rNJVA09E0WT.jpeg) 

Finished soldering, and put a sleeve and a plastic cover on the outside part. The plastic cover can waterproof the connector, which is of course redundant unless you plan to charge your board outside in rain. :smile: I only put it on since I thought it will be good to have something to hold on when plugging it in/out. It's really bulky though and there's a minor problem with that as you'll see later.

![DSC01759|690x460](upload://nQ2PCG0XmIQAuCVozMwhb1c34j6.jpeg)  

Before mounting the connector on the enclosure, I wanted to test if all is working as expected first. This is my temporary charging setup. 

![DSC01761|690x460](upload://8hLDFwyuUpjnZRQWtEBYn1CLIcm.jpeg)

![DSC01763|690x460](upload://503WAp17cwQUkWZTplXaKFkKtto.jpeg) 

I took a piece of perfboard and soldered the wires on such that I can connect the charger and easily check voltages of individual cells with a multimeter. (It would have been much simpler to use a 11 pin terminal blocks if I had one on hand.)

![DSC01760|690x460](upload://pNAKtx3vKIirRXpg2l4dnesGtPT.jpeg) 

The connector makes it somewhat difficult not to mess up the order of the balance wires. It would have been easier if I had more than two colors. Measuring continuity with multimeter helps. Also, it's of course a good idea to check for shorts before connecting the battery.

After checking that all works it was time to remove the original charge connector and do some drilling, which turned out to be a bit of a problem. The connector requires a hole with a diameter of 22 mm. The biggest drill bit I have is only 20 mm.

![DSC01764|690x460](upload://uxbSisvuA8GmqbEu7y0DVtpAKle.jpeg) 

Maybe it will still fit. (I also have a 2 pin connector which was easier to use to test fit since it had no wires on. It's exactly the same size as the 12 pin one.)

![DSC01765|690x460](upload://qcDxEzsbI2ipBsQvXZ03riR9JJy.jpeg) 

OK, you can't push a 22 mm thing through a 20 mm hole. Tested for you. :smile:

![DSC01766|690x460](upload://iaMdoLPVahWZg6e7yNa09qk4xs3.jpeg) 

Time to put into test this thing that I recently found in a hardware store.

![DSC01767|690x460](upload://uu3GC1a3cbP1rFu6AfZu9d87UsT.jpeg)

It worked!

![DSC01768|690x460](upload://tMvVy7XgFqvAyALOkGVKoHNYFrr.jpeg)

![DSC01770|690x460](upload://jIm785x38Tvj1VHPZjG9fIkynGO.jpeg) 

![DSC01774|690x460](upload://f5HaUuz4hL5bBDX6OgEdKDpwmZ2.jpeg) 

![DSC01773|690x460](upload://ddRYzJSg4YBwCqWW8EDhWyghlNB.jpeg) 

One problem is that the enclosure is not completely flat in that area so the connector doesn't align with it perfectly.

![DSC01772|690x460](upload://4Toaj3ssWHvpON3wqhm1BvTI43K.jpeg) 

I wondered whether the mount would still be waterproof. The connector comes with a rubber gasket for the mounting hole. So I closed the lid and sprayed on some water (after disconnecting the battery first). 

No water got in at first, so I sprayed it more aggressively. After that, a few drops leaked in, but surprisingly not through the big hole but rather through the small screw holes. I will have to fix that. No water got into the connector.

Here's one more picture of the charging cable connected. It's actually a hair too long to charge the board while standing on wheels. That's not a big deal though and could be fixed by removing the plastic cover.

I can't help thinking that it looks like I'm milking the board rather than charging it. :smiley: 

![DSC01775|690x460](upload://pgIfQgPSTrjs3V1opRfKm7rbllt.jpeg) 

So far so good. The next step is to figure out how exactly to go about charging. I considered using the two 6S iMAX B6 balance chargers that I already have or getting the 10S [iCharger 1010B+](https://www.icharger.co.nz/icharger-1010b), which is a bit expensive, or even the 12S [Chargery C4012B](http://www.chargery.com/C4012B.asp), which is crazy expensive. But I'm thinking I'll actually go without a balance charger at all. Jehu Garcia says in one of his videos that he uses no balance charger in his li-ion powered VW bus. He says that you do need a balance charger for li-pos, but not for li-ion as long as you keep an eye on individual cell voltages... and that's easy for me to do now that I have access to balance wires.

I would like to make a custom 10-12S battery monitor that shows individual cell voltages and triggers an alarm if any cell voltage gets above predefined threshold so that I know I should disconnect the charger. I will never charge my board unattended ever, so a display with individual voltages and some simple beeper is all I need. I can see a number of options how to do something like that, but more about that in some other post.
```

---
## \#2 Posted by: mmaner Posted at: 2018-12-25T22:11:30.198Z Reads: 56

```
I've tried connectors similar to this one in the past, for the same reason. I wanted to use an external charger to charge and balance. Of the 3 I tried, all 3 broke in some way within 100 miles. I ended up using a JST 2.0 11 pin connector that I pulled out of the enclosure when I needed to charge. I eventually got away from that as it was time consuming. 

I'm not saying don't do it, just passing along my experience. Good luck.
```

---
## \#3 Posted by: janpom Posted at: 2018-12-25T22:15:37.156Z Reads: 53

```
That's good to know, thanks. How exactly did your connectors break? Did they wear out due to plugging in/out or did it have to do with riding/vibrations?
```

---
## \#4 Posted by: mmaner Posted at: 2018-12-25T22:19:54.245Z Reads: 50

```
I theorize the body can't handle the vibrations. The body, all 3, just sort of crumbled.  It cracked in multiple places along the wide part of the body, center wise. 

I had imtedee to coat a new one in epoxy, install it and then pool epoxy around the exposed positions, both inside and outside, but I got tired of having to work on it before I could ride or out the board up. 

I ended up settling in using the Bestech D150 charge only BMS and a 5a rated 2.5mm DC jack.
```

---
## \#5 Posted by: janpom Posted at: 2018-12-25T22:28:49.882Z Reads: 47

```
That sounds bad. That's actually pretty dangerous since if the connector cracks the pins can touch and short the battery. Well, thanks for the heads up. I'll definitely keep an eye on the connector. Maybe even disconnect it from the battery for a few test rides.

A BMS is surely a simpler option. I just don't like the idea of a dumb charge-only BMS since (1) you're always carrying in your enclosure something that's only used for charging and (2) you don't get to know if there's something wrong with the battery.
```

---
## \#6 Posted by: mmaner Posted at: 2018-12-25T22:34:18.210Z Reads: 45

```
I agree wholeheartedly. I just never found a better solution that a BMS and checking cell group voltage with a multimeter every month or so. 

At least I never found a usable solution using available components. I actually modeled a connector using 1mm wide 10g copper blades that would be incredible for charging using an external balance charger. 

Unfortunately to get it made was going to cost about 40k for 1000 of them, minimum order, which left then at 40 bucks a piece so not very sellable.
```

---
## \#7 Posted by: Surfer Posted at: 2018-12-25T23:52:04.318Z Reads: 32

```
I really like the idea to use something like this, a BMS Bluetooth where you can check all data coming from your pack in your phone, I think it's awesome, just too big!!
https://s.click.aliexpress.com/e/bTdyAIdS
But also the experience is telling me quality batteries usually don't drift, I didn't find any liion pack on all of I used hard any kind of drift. By that I would like just a small foot print device to monitor the cells in my phone, no balance, no charging, not nothing more than cell monitor and then I can decide when to balance them.
```

---
