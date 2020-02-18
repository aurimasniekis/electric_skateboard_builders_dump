# Soldering a 10s2p Samsung 30Q

### Replies: 22 Views: 2059

## \#1 Posted by: florensvb Posted at: 2017-10-10T15:46:44.939Z Reads: 269

```
Hey guys,

I am in the process of ordering everything that I need to build my first 10s2p and am looking for some last minute advice.

I was planing to use copper braid for the parallel connections and then 8 awg wire for the serial connections:

http://www.ebay.de/itm/1m-Kupfergeflecht-PRO-POWER-FB-Erdungsband-30A-2-26mm-Breite-5mm-/232282931721?hash=item3615244209:g:~~cAAOSw2gxY1rji

http://www.ebay.de/itm/Silikonkabel-8AWG-Silikon-Kabel-Farbe-Rot-Schwarz-8-25-qmm-180-Ampere-/152146448420?var=&hash=item236ca29024:m:mILiKCZVJr4-sfD8jaPrWKw

Are these good copper braids and wires to use? Am I correct in using copper braid for parallel and wires for series? 

Most importantly: The description of the copper braid claims that it can handle 30A current- is that enough for my 10s2p?

Also, where the heck do I get heat shrink sufficiently large to wrap around my pack? 

Do I need anything else to make a good pack??

Please dont hesitate to give me more advice on this. 

I do have a 100W soldering iron that should get the heat in and out quickly enough.

And as always: Cheers guys! :)
```

---
## \#2 Posted by: barajabali Posted at: 2017-10-10T16:01:19.138Z Reads: 251

```
Are you running a dual or singly setup? Either way i think this pack may be too small for the output needed.
```

---
## \#3 Posted by: florensvb Posted at: 2017-10-10T16:02:02.176Z Reads: 250

```
Planning on building a single 6364 190kv. You're saying 2p isn't enough?

Advice on the 10s2p comes from the master:
http://www.electric-skateboard.builders/t/need-10s-bms-40a-w-e-switch/34483/18?u=florensvb
```

---
## \#4 Posted by: willpark16 Posted at: 2017-10-10T16:06:54.799Z Reads: 242

```
He uses Baden cells
```

---
## \#5 Posted by: barajabali Posted at: 2017-10-10T16:07:41.266Z Reads: 239

```
https://www.imrbatteries.com/samsung-30q-18650-3000mah-15a-flat-top-battery/

Only 30 amp cont rating for a 2p. I'm not guaranteeing you'll have issues but you may.  I have had problems in the past with 30amp discharge on a single drive 6374
```

---
## \#6 Posted by: florensvb Posted at: 2017-10-10T16:15:03.733Z Reads: 233

```
Yeah i was planning on setting my motor max and battery max to 30A. What kind of problems did you have?
```

---
## \#7 Posted by: barajabali Posted at: 2017-10-10T16:16:58.870Z Reads: 229

```
Cutouts under high acceleration sometimes.
```

---
## \#8 Posted by: florensvb Posted at: 2017-10-10T16:17:47.114Z Reads: 225

```
Where do those cutouts come from?
```

---
## \#9 Posted by: barajabali Posted at: 2017-10-10T16:19:31.562Z Reads: 220

```
Heavy sag from either going up hill or acceleration causes the cells to sag so much that the vesc goings in to low voltage
```

---
## \#10 Posted by: florensvb Posted at: 2017-10-10T16:23:33.710Z Reads: 220

```
Hmhm... well at least it will perform better than my 8s1p lipos :D 

Can you give advice as to wether the copper braid and silicon wire i posted are adequate?
```

---
## \#11 Posted by: barajabali Posted at: 2017-10-10T16:40:03.881Z Reads: 211

```
Yea the silicone wire will be a better option :)
```

---
## \#12 Posted by: florensvb Posted at: 2017-10-10T16:41:51.129Z Reads: 202

```
So just use the 8 awg silicon wire for all of the connections and just remove the insulation wherever needed?
```

---
## \#13 Posted by: barajabali Posted at: 2017-10-10T16:46:01.514Z Reads: 199

```
Yea that would be recommended  you could use the copper braid too.  Its just not as ideal
```

---
## \#14 Posted by: florensvb Posted at: 2017-10-10T16:47:01.606Z Reads: 200

```
Oh ok. I thought it would be more ideal, as its so thin and more like a nickel strip. I only got the idea from reading on the forum. Guess going with silicon wire is easier for me anyways :D Thanks @barajabali for the help
```

---
## \#15 Posted by: barajabali Posted at: 2017-10-10T16:48:17.140Z Reads: 192

```
My pleasure :) good luck and post pictures
```

---
## \#16 Posted by: banjaxxed Posted at: 2017-10-10T20:50:25.549Z Reads: 188

```
The parallel connections can be thin it's the series that throughput the real power
```

---
## \#17 Posted by: florensvb Posted at: 2017-10-10T21:06:27.517Z Reads: 180

```
ah ok i was taking it from here

http://www.electric-skateboard.builders/t/soldering-iron-for-18650-packs/18626/10?u=florensvb

Do you recommend that I'll be fine using 8 awg wire or maybe i could even go with 10?
```

---
## \#18 Posted by: Jinra Posted at: 2017-10-10T21:08:44.118Z Reads: 174

```
You can set the 30Q's for 40A total discharge
```

---
## \#19 Posted by: Namasaki Posted at: 2017-10-11T03:02:16.650Z Reads: 164

```
@barajabali  is the expert when it comes to batteries, So take his advice.

And the 10s2p pack that I built with Basen cells was actually a disappointment for me. It had good range on flat ground at moderate speeds but when climbing hills, it had excessive voltage sag and it's range was cut in half.
That is why I pulled it and replaced it with the Lipo build.
```

---
## \#20 Posted by: jaykup Posted at: 2017-10-11T03:21:18.735Z Reads: 164

```
I agree on the 10s2p being a bit on the lite side... the board is not going to have much of a personality... but if you go that route the amperage requirements are much less.  If we consider the 30Q batteries being 20A batteries (even through they are rated at 15A), you are only moving 40 amps.  That puts you safely in the 10-12 gauge range.  8AWG wire is hard to work with in any form.  I originally tried using 8AWG silicone wire for the short 1" connections between series, and failed miserably.  It was also hard to keep 1" of silicone wire that was stripped of it's insulation together during the soldering process.  It's basically 50 tiny strands not attached to each other.  The braided wire holds together nicely in short sections.

The other problem was the wire would suck up all the solder and become hard, not allowing the battery to fold over.  If you don't need to fold the battery, it may work OK.  It basically creates a solid solder bridge though.  That's why I ended up buying the 12awg flat braided wire after failing with the silicone wire.

I did use the 8awg silicone wire successfully on the battery to VESC connections without an issue.  Since the wire was longer, it didn't matter that it was sucking up some solder and the insulation held it together without issue.

You could probably use 12awg braid for all the series and parallel connections (instead of nickle strips), then use 10-12 awg silicone wire from the battery to the VESC.
```

---
## \#21 Posted by: Ulfberht Posted at: 2017-10-11T03:48:43.039Z Reads: 153

```
[quote="jaykup, post:20, topic:35247"]
8AWG wire is hard to work with in any form
[/quote]

I totally agree with this. The only way to make it a little easier with stranded wire is to actually cut off some of the strands before soldering. Cut down to about 10awg or so. This works good if you are soldering to a connector/plug and you can't get the whole wire in there. (such as an XT-90)  If all you have is 8AWG you can make it work is what I'm trying to say.
```

---
## \#22 Posted by: florensvb Posted at: 2017-10-11T06:16:35.582Z Reads: 142

```
I havent ordered any wires yet- so i am happy for your advice! I also want to make it easier on myself to get the soldering done. so i guess i will make the entire pack with 10awg wire
```

---
