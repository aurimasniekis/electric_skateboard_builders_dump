# Custom 10s4p Evolve Battery Issue

### Replies: 11 Views: 1140

## \#1 Posted by: Kit Posted at: 2018-05-06T04:52:03.724Z Reads: 207

```
Hi Guys,

I built a 10s4p (Samsung 18650 30q's) for my Evolve CGT and it was working for about 75 miles; however, after every ride now, I get a message on my remote stating "battery maintenance" and most recently "battery drain"...the last one occurred after the battery was reading as at 70%, which suddenly dropped down to 0%.

So far, I suspect that the BMS is overheating...each cell reads as at ~4000mah each. The wiring shows no damage & each battery is connecting properly to the leads. They are reading as 4v, 8v, 12v, 16v, 20v, 24v, 28v, 32v, 36v, and 40v sequentially. The cause should have been isolated by now, so the BMS is my current suspicion.
```

---
## \#2 Posted by: Naysh Posted at: 2018-05-06T07:27:47.731Z Reads: 188

```
you need battery help battery expert @barajabali should be able to help you out
```

---
## \#3 Posted by: ARetardedPillow Posted at: 2018-05-06T08:04:14.751Z Reads: 180

```
How did you measure the mah of each cell?
```

---
## \#4 Posted by: Kit Posted at: 2018-05-06T15:01:42.796Z Reads: 157

```
The evolve remote has a menu that displays the mah of cells 1-10. Atm the board isnt powering up, despite it powering up after 2 other rides that gave off the "battery maintenance" message, so it's difficult to tell what the current mah is. I got my last reading before the "battery drained" message.
```

---
## \#5 Posted by: ShutterShock Posted at: 2018-05-06T19:37:33.486Z Reads: 123

```
Honestly even though you said you checked it still sounds like a connection issue.. Maybe a spot weld is coming loose occasionally or there is  wire that is internally split?  Check over every connection very closely.

Also you should pull out a multimeter and check the voltage of every cell just to be sure one isnt bad.  While you're at it, use the continuity tester and check for any loose welds.
```

---
## \#6 Posted by: Kit Posted at: 2018-05-06T20:23:22.531Z Reads: 117

```
True...looks like I'll have to cut up the shrink wrap to get a closer look at things
```

---
## \#7 Posted by: Jinra Posted at: 2018-05-06T21:41:12.735Z Reads: 108

```
Could be inadequate series connection. Do you have pictures of the pack?
```

---
## \#8 Posted by: Kit Posted at: 2018-05-07T00:30:07.963Z Reads: 101

```
I do not have older ones showing the issue unfortunately, as I had opened up the pack, addressed the most likely issue, then shrink-wrapped it back together before hopping back on the forums and seeing your reply. However, I believe you are 100% right on this Jinra; I originally connected my series via magnets. 3 sets of 2; so 2 magnets connecting the last 3 batteries together, in order to connect the two series. I forgot to mention it due to my stoner lifestyle thanks to some California Kush lol. 

While they were not disconnected when I opened up the pack, the magnets still slid around the first time I wrapped the pack up. I suspected that they were disconnecting suddenly due to riding around/vibrations; it would explain the sudden "battery drain" message at a 0% charge despite being at a 70% charge just before. 

So this time, in order to ensure that it is not a possible point of connection failure, I removed the magnets and soldered 14 awg wire to connect the series together. I also confirmed that all cells are reading properly, and did a quick 10 mile test ride with no issues so far. Here is a picture of it currently with the soldered connection (please note, the last 3 batteries on the right have clear-wrap, as the original pink wrap was damaged by me): 

EDIT: I noticed the older pic was my 10s5p, here is my 10s4p when I first finished it but before I wrapped it. I have already replaced the magnets with soldered wire.
![20180404_213959|375x500](upload://2u3clojtpz5gPB0yxqRbRPaIyG2.jpg)
```

---
## \#9 Posted by: Kit Posted at: 2018-05-08T00:54:30.812Z Reads: 77

```
Whelp it looks like the issue is still occurring; did a 2 mile ride and the board just shut down. It wont take a charge (red led isnt lighting up when the charging brick is plugged in) but I think the issue may be the connections still...time to remove the final layer of tape...
```

---
## \#10 Posted by: b264 Posted at: 2018-05-08T04:43:46.978Z Reads: 77

```
[quote="Kit, post:4, topic:54537"]
The evolve remote has a menu that displays the mah of cells 1-10.
[/quote]

I assume you mean mAh, and it does not have this.  It shows the voltage or V of each parallel pack.

Are those all the same cells?

Please show photos of the battery welds and connections.
```

---
## \#11 Posted by: Kit Posted at: 2018-05-09T00:59:32.580Z Reads: 72

```
![20180508_115317|666x500](upload://sGSewG6jNPF7U0PBTXOmLRtuCfR.jpg)![20180508_115031|374x500](upload://sr8McMmrI3Lra5619ehFf0F4qw7.jpg)

Looks like the true issue lies in the connections like you guys said; as soon as I cut open the shrink wrap I saw that there was a hole on the side of it, with this metal strip sticking out. I did not see any damage on the CGT housing which was a relief. I removed the strip (this one bridges two cells together), and soldered on a new connection in its place. I did this for 2 other strips that I found to be just as weak as I inspected the rest of the pack. After packing it all up, I did a test ride for about 11 miles and no issues occurred. I plan on doing more "test" rides but I am more confident in the packs ability to handle the mileage. 

This is my very first pack so I expected some issues I suppose. My second pack is already much more properly built than this one (and minus the caps). Only kapton tape is now used to cover the endcaps, rather than electrical tape. Direct solder for the series connection, rather than magnets. Kapton to cover exposed soldering points on the BMS as well, as a precaution. 

This is the final product as of now, w/shrink wrap:
![received_10155685113217106|690x388](upload://1OwJk2WPgyFcSdy3cMBPkro1QmI.jpeg)
```

---
