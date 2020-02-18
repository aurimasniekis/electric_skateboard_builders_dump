# Super simple DIY remote headlights

### Replies: 4 Views: 980

## \#1 Posted by: Static Posted at: 2018-09-09T03:55:09.266Z Reads: 165

```
In my search for an easy highbeam headlight option from [this thread](https://www.electric-skateboard.builders/t/long-throw-headlights-what-has-worked-best-for-you-shredlights-etc-bike-lights-flashlights-custom/63944/7) I tried a few different variants of cheap led flashlights. Mounting them to the trucks with rubber "c" clamps was easy and secure. However, all of them eventually began to fail. Usually a flicker in which the battery was likely loosing contact. 

I decided that I wanted to make something more reliable and permanent. This led me to [ebay bike lights](https://www.ebay.com/itm/SolarStorm-15000Lm-3xXML-T6-LED-Head-Bicycle-Bike-Lamp-Light-Rear-Light-16000mAh/322656749160?ssPageName=STRK%3AMEBIDX%3AIT&var=511675710648&_trksid=p2060353.m2749.l2649):



![image|361x298](upload://oohhVoK4Jiwp06PeUvTU8JP9DjB.jpg)

I tested this model in particular for a while with it simply taped to the board. It held up to the vibrations well and was brighter than anything else I tested. The entire body is metal as well as the internals. At under $20 USD it seemed like a good purchase.

I could have just 3D printed a mount and battery case for the underside of the board and finished there, but I wanted this light to be remote controlled so I decided to experiment. 

This model runs off a 2s2p battery pack of 18650 cells. So the voltage range is somewhere between 6.8-8.4 volts. I happened to see a cheap remote relay switch [on Amazon](https://www.amazon.com/gp/product/B0762HH45G/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1) that operated at this voltage so I thought I'd give that a try.
![image|558x496](upload://84lO6qI9Yu6f8SiAc53f58dQSlb.jpg)

Easily enough it works. I wanted this to be simple and reliable so I didn't keep the lights original PCB. Instead I opted to use a couple of resistors with a switch for brightness control. Not too experienced with circuits, but I've managed in the past through experimentation and this couldn't get much simpler.

This is the basic wiring diagram, except I used a switch and two resistors before the leds for high and low beam.
![image|663x346](upload://7oA1hOEA68FYA93ivLcCuxJ5poS.png)
Looking up the data sheet for the LED's used in my light it seems that they consume a bit more current than I assumed:

(XM-L T6 )
![image|690x229](upload://b2krmaDFErSeZJZ73BvzsuNr1uK.png)

I went through my scrap parts bin and found a couple of hefty resistors (10ohm and 2.7ohm) that I figured wouldn't get to hot. After testing them for a while they don't, but I'm still a little concerned about [power dissipation.](http://led.linear1.org/led.wiz) 

![image|690x497](upload://2rllRkuOkxLTyJT8bIsFpWyS3jd.jpg)

Anyway now that it's tested I'll print an enclosure for everything and mount the light. The remote should be pretty easy to take integrate into my boards remote.

![image|690x393](upload://awCyu71J7E8mtO4fSECKGJ3cShE.jpg)

Thanks for reading. Comments, ideas, or suggestions are welcomed.
```

---
## \#2 Posted by: High-roller Posted at: 2018-09-09T04:26:24.312Z Reads: 130

```
I was looking at buying a couple of these for my next build, thanks for confirming their brightness.
Right now I'm doing what you did, I have a small separate battery pack for the lights, but it would be nice if I could just draw from the main pack. Are you planning on trying that?
```

---
## \#3 Posted by: Static Posted at: 2018-09-09T04:33:13.909Z Reads: 121

```
The bike light I purchased came with that battery pack. I'm basically drawing directly from the battery pack with a resistor before the led.
```

---
## \#4 Posted by: Static Posted at: 2018-09-29T01:12:24.231Z Reads: 69

```
Made a quick test run and it works great. I really like the ability to turn the lights off via remote. It also came in handy to signal people. Unfortunately as I expected there is passive drain on the battery so it dies if I leave it plugged in. 

Anyone know how I could improve this? I feel this could be a really easy project for most and be comparable to something like shredlights except remote controlled.

![image|374x500](upload://ceCZbnagwnEcaAkwGkx7GMDYPFu.jpeg) 
![image|374x500](upload://73tk1xAx0s6d8oW96lmujp2lVFy.jpeg)
```

---
