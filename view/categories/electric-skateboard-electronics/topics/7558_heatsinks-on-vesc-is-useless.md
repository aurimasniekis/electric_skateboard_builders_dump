# Heatsinks on vesc is useless!

### Replies: 30 Views: 5212

## \#1 Posted by: Hummie Posted at: 2016-08-12T17:27:26.084Z Reads: 525

```
I was just reading adding heatsinks to the top of the fets almost does nothing.  According to Rew:

"Yes. Note that cooling the "top" of the fets (the side you can see without desoldering) is useless. I've found a datasheet that mentions 10x the thermal resistance to that side of the case than to the side that you're planning on cooling. Note that the high-side-FET drains are all connected to "VMOT". So you can easily solder all three of them to a big copper plate (connect to VMOT as well!) and a heatsink. 

On the other side, the three drains are connected to the motor phases. So you'd need an L-shaped copper conductor and then an insulated heatsink on that. Consider: There is also the IRFP7530. The problem is that it is a lot bigger: TO247."

Also the temp sensors aren't really on the fets just nearby and there's really only one sensor for all the fets for now
```

---
## \#2 Posted by: chaka Posted at: 2016-08-12T17:37:58.525Z Reads: 517

```
Common misconception.... I suggest you do some real world testing. While not ideal, they do indeed help dissipate heat away from the mosfets.
```

---
## \#3 Posted by: Blasto Posted at: 2016-08-12T17:46:23.669Z Reads: 520

```
I wouldn't say useless, it does help a lot. Just not optimal.
```

---
## \#4 Posted by: Nordle Posted at: 2016-08-12T17:54:31.305Z Reads: 510

```
Heatsink on VESC is not useless! makes it more bling bling
```

---
## \#5 Posted by: evoheyax Posted at: 2016-08-12T17:58:51.395Z Reads: 498

```
I showed you real world tests hummie... I have one right now with a heatsink and one with out (both chakas). The one with the heat sink draws more amps than the one without the heatsink. They both get to about the same temperature, but the one with the heatsink cools quicker, and thus can pull more amps than the one without the heatsink.

Without heatsinks, I had heating issues with my carvons. With heatsinks, the heating issues went away. My real world tests show me that the heatsinks do have a positive effect of dissipating heat.
```

---
## \#6 Posted by: Hummie Posted at: 2016-08-12T18:02:48.895Z Reads: 471

```
I haven't done any tests and I never get too hot but I thought it was worth noting what the resident expert on vedder's site said given so many people have problems. 
i know they have a plastic case and it's hard to really get to the source of the heat.
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-12T18:04:56.716Z Reads: 452

```
I think some people try to mask actual problems by adding heatsinks. I dont think it's to say heatsinks are useless, but rather they're not always the best way to solve a heat issue.
```

---
## \#8 Posted by: smurf Posted at: 2016-08-12T18:07:04.580Z Reads: 440

```
Do they make so much heat that they need venting or can you use a air/waterproof case?
```

---
## \#9 Posted by: Hummie Posted at: 2016-08-12T18:10:56.168Z Reads: 425

```
In my experience they can be pretty well contained but others have had problems and need to add heatsinks and get better airflow.  
I'm not saying a heatsink on the top does nothing just bringing a point of view from someone who knows a lot and we could maybe further benefit from what he's saying
```

---
## \#10 Posted by: Abdulz Posted at: 2016-08-12T18:23:33.794Z Reads: 408

```
I'm abit new to VESCs but do you think the voltage is a game changer as the higher the voltage the lower the amp draw?
```

---
## \#11 Posted by: smurf Posted at: 2016-08-12T18:31:27.718Z Reads: 406

```
For the same amount of work yes but mostly we are using more voltage for more work
```

---
## \#12 Posted by: sl33py Posted at: 2016-08-12T18:32:27.056Z Reads: 403

```
Yep - totally a game changer - higher voltage = lower amps!  But not one VESC or anything hardware has to do with.
```

---
## \#13 Posted by: chaka Posted at: 2016-08-12T18:37:50.993Z Reads: 397

```
This is something I have been intending to create once our mill is up an running. It will be interesting to see if it increases the capability of the VESC with a more direct connection to the base of the fets.

<img src="/uploads/db1493/original/2X/0/054fe0f85c5a38278fee37e556ead37e594288ba.png" width="690" height="291">
```

---
## \#14 Posted by: evoheyax Posted at: 2016-08-12T18:40:27.610Z Reads: 383

```
I think a low amp, high voltage system likely dose not need heatsinks if the motor/gearing is efficient. I needed them, because they way I was running my carvons was not efficient, I never got close to 85% of my no load speed, as that would be way too fast. With your motors even @Hummie, the heat sinks had a positive effect. You  never had issues because you have good airflow i.e. they are duct tapped to the bottom of your board. But if you enclose them, they will get hot.
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-08-12T18:55:36.405Z Reads: 369

```
[quote="evoheyax, post:5, topic:7558"]
Without heatsinks, I had heating issues with my carvons. With heatsinks, the heating issues went away.
[/quote]

good to know. I may have a carvon build in the pipe.
```

---
## \#16 Posted by: Hummie Posted at: 2016-08-12T19:05:02.134Z Reads: 359

```
actually theyre pretty contained in bubble wrap and tape these days and cant be seen.  wish my batteries were as well as they're all dying from shrapnel again.

the no-load speed is constantly changing based on your throttle and what percent it sends to the motor of the battery voltage and if your motors are big enough and the load not too big they will be near it.  the carvon are big and you probably were.  I think more the reason carvon get the vesc hot is because theyre such high kv it takes more amps for them to create torque.
```

---
## \#17 Posted by: Nordle Posted at: 2016-08-12T19:08:57.839Z Reads: 345

```
but you get the v2.5? the lower kv should run fine, speaking from experience
```

---
## \#18 Posted by: chaka Posted at: 2016-08-12T22:33:02.974Z Reads: 333

```
Its coming back to me now why I abandoned the custom heat sink. I didn't want such a large positive terminal exposed in my system. :confused:
```

---
## \#19 Posted by: Heavy1 Posted at: 2016-08-13T01:45:49.591Z Reads: 324

```
Is there a non conductive material that could still be used to dissipate heat or at least as a transitional material to the heat sink?
```

---
## \#20 Posted by: Hummie Posted at: 2016-08-13T02:36:43.196Z Reads: 320

```
i think heat and electricity conductibility go pretty hand in hand except for some fancy pastes and silicones.  

chaka is that dangerous is that why you dont want that?  to touch?  what on the board is dangerous to touch at 12s?  Have you touched 12s!?  I mean possibly shorted across something with 50v. had your body in circuit with that and you dont zing
```

---
## \#21 Posted by: cjoliver Posted at: 2016-08-13T02:37:53.300Z Reads: 286

```
Lol someone should make a water cooled system for the VESC :joy:
```

---
## \#22 Posted by: Randyc1 Posted at: 2016-08-13T02:45:55.590Z Reads: 294

```
If the Vesc Enclosure itself was the Heatsink, then it would be directly exposed to the wind for superior cooling, ...seperate from the battery enclosure.
```

---
## \#23 Posted by: evoheyax Posted at: 2016-08-13T16:34:03.100Z Reads: 279

```
thought about it, but you don't want liquid in your board, waiting to be spilled.
```

---
## \#24 Posted by: chaka Posted at: 2016-08-13T17:13:19.837Z Reads: 278

```
i think we will need it if we start racing eboards competitively. I have had some excellent results cooling 18650's with embedded cooling line. It wasn't pretty but it worked really well. The challenge is fitting everything inside a deck. ;)
```

---
## \#25 Posted by: Randyc1 Posted at: 2016-08-13T18:08:00.000Z Reads: 278

```
Can't we build a Heat Sink "Evolve style" , which is exposed to the wind ??

Just having Wind cooling the Fins,... seems to me would make a big difference?
```

---
## \#26 Posted by: Hummie Posted at: 2016-08-14T01:55:17.505Z Reads: 272

```
Chaka didn't mean to step on your heatsink progress with the over-the-top title.  I thought it might lure more people.   When u say u don't want to heatsink the bottom of the fets because of the large positive terminal are u afraid people would short the board?  I'm looking to get the most cooling possible as I'll be running one hub motor and anticipate a lot of amps and heat
```

---
## \#27 Posted by: Jinra Posted at: 2016-08-14T01:57:45.848Z Reads: 274

```
Yea having one giant exposed positive terminal is never a good idea. Super easy to short. When I rode with  you last time it didn't seem that your VESC got that hot. Given, you were on a dual setup, but I don't imagine it'll get that much hotter on a single especially running 12s. I have some raspberry pi heatsinks you can throw on the mosfets if you want. Since you don't run an enclosure the wind hitting the sinks directly should help control temperatures pretty well.
```

---
## \#28 Posted by: JdogAwesome Posted at: 2016-08-14T04:35:49.607Z Reads: 268

```
On the original post, @Hummie mentioned the IRFP7530 MOSFET which happens to be the exact MOSFET im using in my [EBoard Switch](http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738) and doing the math the 7530 wouldn't need a heatsink at 30A continuous in a 63°C environment at its max RDSON which is usually around 1.65Miliohms not 2 which is what I based the calculations off of. Anyways the 7530 would be a great substitute for the VESC fets if it ever becomes necessary to increase the max VESC amperage. Also people where worried about heatsinks possibly shorting out things because they would be live connections, but you could just use non conductive thermal past to fix that problem, thats what most people do for adding heatsinks to fets because the flange is usually a drain as well. [IRFP7530PbF Datasheet](http://www.infineon.com/dgdl/irfp7530pbf.pdf?fileId=5546d462533600a40153562caf372027)

*EDIT: just realized that the MOSFET's used on the VESC currently are 7530 versions though there actually better, or at least have a lower RDSON of only 1.4mOhms and a C/W of 40. So yeah pretty much disregard what I said about the 7530 as a replacement for the current fets. Though the 7530 is still a great mosfet for other applications.
```

---
## \#29 Posted by: racidon Posted at: 2016-08-14T05:03:59.581Z Reads: 269

```
[quote="Hummie, post:9, topic:7558, full:true"]
I'm not saying a heatsink on the top does nothing just bringing a point of view from someone who knows a lot and we could maybe further benefit from what he's saying
[/quote]

I guess he doesn't work for the motherboard companies that have been doing this now for about 15+ years with all the added research they've done in the field?



[quote="chaka, post:18, topic:7558, full:true"]
Its coming back to me now why I abandoned the custom heat sink. I didn't want such a large positive terminal exposed in my system. :confused:
[/quote]

Hey bud you can get non-conductive thermal compound to separate the heatsink from the conductive material.

Edit:
Something like this:
http://www.ebay.com.au/itm/like/182063660930?lpid=107&chn=ps
```

---
## \#30 Posted by: Heavy1 Posted at: 2016-08-23T12:44:16.789Z Reads: 222

```
Yes this isn't a Vesc, but I think it does support the notion that heatsinks can be beneficial.

I know you cant read much into this because there is nothing to suggest they are the same esc but I can only conclude the HV160 and HV160 lite are identical besides cases and heatsinks. Hv160 requires 5mph airflow for rating, Hv160 lite 20mph airflow for its rating.

http://www.castlecreations.com/products/phoenix-ice2-hv.html
```

---
