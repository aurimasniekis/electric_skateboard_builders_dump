# Looking for VESC Heatsink kit

### Replies: 32 Views: 3661

## \#1 Posted by: roonydagoony Posted at: 2016-07-11T17:25:17.542Z Reads: 331

```
Hi,  Ollin Boards does not sell individual heatsink units, they only add it as an accessory for the vesc (if you buy that form them)

I was wondering if anyone has any spares (heatsink and bottom plate).
I'm willing to pay full prices

I'm in NYC
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-11T17:32:04.304Z Reads: 336

```
You can get some of these and throw them on the mosfets and DRV.

http://www.ebay.com/sch/i.html?_from=R40&_trksid=p2050601.m570.l1313.TR0.TRC0.H0.X5-pin+jst.TRS0&_nkw=raspberry+pi+heatsink&_sacat=0
```

---
## \#3 Posted by: Ulfberht Posted at: 2016-07-11T18:18:42.356Z Reads: 333

```
NIce! I bought some of those. I got these ones though. 
http://www.ebay.com/itm/30PCS-Aluminum-Heatsink-Cooler-Adhesive-Kit-for-Cooling-Raspberry-Pi-/141865269904?hash=item2107d43a90:g:xc4AAOSwa-dWl0Hl
There are a couple of sizes and they have 3m adhesive on the back. My only concern is that, under the vibrations that an ESK8 produces, they might come loose. I want to test how they hold up to heat and vibration before I put them on my factory fresh Ollinboardco VESCs.
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-11T18:26:03.963Z Reads: 307

```
I got the same ones! :smiley:
```

---
## \#5 Posted by: PB1 Posted at: 2016-07-11T18:32:55.819Z Reads: 303

```
Does any of you guys know if it is enough to put heatsinks on the mosfets? 
Which part of the VESC does actually get warm? 

Only the 6 mosfets or also the DRV?
```

---
## \#6 Posted by: Jinra Posted at: 2016-07-11T18:41:43.855Z Reads: 295

```
Depends heavily on your build and environment. Some people overheat their mosfets/drv, others run quite cool. I'd say most people don't have heatsinks on them.
```

---
## \#7 Posted by: roonydagoony Posted at: 2016-07-11T18:42:46.214Z Reads: 290

```
I've heard too many stores of ppl melting their vescs....so to be safe, I'd lik to heat sink this up. Especially because I'll be using 2 of them inside my space cell pro enclosure
```

---
## \#8 Posted by: Jinra Posted at: 2016-07-11T18:43:35.018Z Reads: 287

```
You're probably reading about a lot of people running FOC. If you want to be safe run in BLDC and you should be fine.
```

---
## \#9 Posted by: PB1 Posted at: 2016-07-11T18:45:22.636Z Reads: 282

```
I know as a fact that my VESC do get very warm (single SK3 6364 - see build thread 2F4M - BLDC). We have some nasty and loooong hills here. 
So I do want to heatsink my VESCs for the next build and have some GPU heatsinks already. Question is, do they only go onto the mosfests or also onto other parts, e.g. the DRV Chip?
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-11T18:47:05.490Z Reads: 269

```
@chaka sells his VESCs with a heatsink option and only has it on the 6 mosfets. You probably don't need one for the DRV, but I imagine it wouldn't hurt.
```

---
## \#11 Posted by: torqueboards Posted at: 2016-07-11T18:48:27.857Z Reads: 261

```
I'll have a heatsink for both the bottom and top. Not sure on the ETA just yet though. Kind of late though since who knows when the VESC 6 is gonna be out but would be a nice to have...
```

---
## \#12 Posted by: rotorguru Posted at: 2016-07-11T18:58:51.902Z Reads: 256

```
@torqueboards Add to your store ;)
```

---
## \#13 Posted by: torqueboards Posted at: 2016-07-11T19:33:18.672Z Reads: 253

```
@rotorguru - Not available yet :stuck_out_tongue:
```

---
## \#14 Posted by: chaka Posted at: 2016-07-11T20:42:16.095Z Reads: 239

```
Well you are half right. The bottom aluminum plate acts as the heat sink for the lower fets.
```

---
## \#15 Posted by: Jinra Posted at: 2016-07-11T20:43:40.981Z Reads: 241

```
Right, so 6 mosfets like i said right? :P
```

---
## \#16 Posted by: roonydagoony Posted at: 2016-07-11T20:44:39.970Z Reads: 242

```
Oh right, also need to get the bottom plate
```

---
## \#17 Posted by: Nordle Posted at: 2016-07-11T20:53:38.162Z Reads: 237

```
or another heatsink, or another plate on top, or copper coins even if they aren't actually copper
```

---
## \#18 Posted by: Lukas Posted at: 2016-07-11T20:55:10.230Z Reads: 243

```
@ chaka 
Do you put any sort of electrical isolator between the heatsinks/aluminum plate and the mosfets? If so does it affect the thermal conductivity much? 

Is there any risk to produce a short by adding the aluminum parts?
Everything looks so close together :sweat_smile:
```

---
## \#19 Posted by: chaka Posted at: 2016-07-11T21:04:42.399Z Reads: 238

```
This is the main reason I do not sell this as a kit. If you install it incorrectly with the wrong type of thermal adhesive you ruin you VESC.
```

---
## \#20 Posted by: KMeyerson Posted at: 2016-07-12T00:22:45.687Z Reads: 229

```
I tend to go with adhesive free thermal pads when I can, but the VESC gets as toasty as the AMD 290x so pads are not going to work.
```

---
## \#21 Posted by: Jebe Posted at: 2016-08-15T00:27:26.080Z Reads: 192

```
be careful with the adhesives they use - make sure they aren't using insulating adhesive tape.
```

---
## \#22 Posted by: sl33py Posted at: 2016-08-15T00:54:20.865Z Reads: 196

```
[quote="torqueboards, post:11, topic:5916, full:true"]
I'll have a heatsink for both the bottom and top. Not sure on the ETA just yet though. Kind of late though since who knows when the VESC 6 is gonna be out but would be a nice to have...
[/quote]


Hey @Torqueboards - i'd buy a few to put on my existing VESCs - never bad to have better cooling.  And i'll be getting the v6 VESC as soon as it comes out too!  Hope you and @Chaka have those available once finalized.
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-15T00:58:11.045Z Reads: 193

```
You can buy the heat sink kit from @chaka right now on his site too.
```

---
## \#24 Posted by: Kaly Posted at: 2016-08-15T01:23:25.751Z Reads: 196

```
@Jinra that is a add-on item only

On a related matter.
Does anybody knows where to get the spacer use in the heat sink kit from ollinboards ?
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-15T01:26:41.882Z Reads: 192

```
Just thought he'd sell it stand-alone. If not, I bought these myself for my Enertion Vescs.

http://www.ebay.com/itm/30PCS-Aluminum-Heatsink-Cooler-Adhesive-Kit-for-Cooling-Raspberry-Pi-/141865269904?hash=item2107d43a90:g:xc4AAOSwa-dWl0Hl

They come with 3m thermal pads so they stick on the mosfets pretty well. I imagine you can get the nylon standoffs at digikey.
```

---
## \#26 Posted by: Kaly Posted at: 2016-08-15T01:30:27.748Z Reads: 191

```
Thank you I'll try you way :-)
```

---
## \#27 Posted by: abenny Posted at: 2016-08-21T17:51:24.845Z Reads: 178

```
im looking at adding heatisnks to my vesc aswell. i already have my aluminum but am wondering how do secure them to the board? is there anything i could get from a hardware store that would work? i thought of pc thermal paste but it isnt adhesive so id still need a way to fasten the aluminum.
```

---
## \#28 Posted by: fottaz Posted at: 2016-08-21T18:05:24.850Z Reads: 179

```
Hi guys, You could make an heat sink for your Vesc at home recycling an old Graphics Card.

<img src="/uploads/db1493/original/2X/a/ad75f3dec0983d8845e9506f52e936816a59485f.jpg" width="377" height="500">
<img src="/uploads/db1493/original/2X/b/b149709940a25ac2a509ee7a6f39ebd757264ea8.jpg" width="662" height="500">
```

---
## \#29 Posted by: abenny Posted at: 2016-08-21T18:18:38.576Z Reads: 171

```
im doning something similar. just cant decide on how to fasten the heatsink to the board. probably gonna do zip ties and thermal paste lol. i dont really have any other ideas, the aluminum i have isnt possible for me to drill through it with my shit tools
```

---
## \#30 Posted by: fottaz Posted at: 2016-08-21T18:42:54.907Z Reads: 170

```
I've used plastic screws and the zip tie, modified to let It pass throught the heat sink. You only need a Dremel to modify the piece and a drill for the holes, obviously with thermal past.
```

---
## \#31 Posted by: evoheyax Posted at: 2016-08-22T04:32:12.427Z Reads: 165

```
What thermal adhesive should I use? I'm not using anything right now on the replacement heat sink you sent me, and I don't want any vesc issues.
```

---
## \#32 Posted by: Mrmoonlight Posted at: 2016-08-22T06:38:55.022Z Reads: 160

```
I use standard silver thermal paste. Does the job just fine. There's also the adhesive paste, but I'm a little worried that it might cause some issues with all the vibrations and the heatsink being so much larger than the chips. I used shrink tube over the whole thing and cutout holes around the Heatsink just leaving the edges and corners. Holds it in there pretty well. 

Here's a pic of my heatsink before I shrink wrapped it. Picked up the heatsink and paste off ebay for a few bucks

http://www.ebay.com/itm/381103432358?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

http://www.ebay.com/itm/131459510613?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

<img src="/uploads/db1493/original/2X/2/21df23bbef7cb306dfc8b53d85550a9037be7652.JPG" width="640" height="480">
```

---
