# Looking for help with piecing together a Frankenstein

### Replies: 8 Views: 322

## \#1 Posted by: MiniChopper4Me Posted at: 2018-10-12T02:55:29.834Z Reads: 113

```
Hello everyone, new user here.

I'm trying to rescue a failed kickstarter board without throwing the whole thing in the trash, but at the end of the day that may be the best option.  Looking for advice.

I have a Kuickwheel Serpent-W, which among all its issues, the biggest for me is the terrible lack of control.  There is delay from the remote and the motors, the braking is terrible, and sometimes it will keep accelerating when you are actually trying to brake.  Also it loses connectivity from time to time.

One of the biggest things I identified early was the battery.  It was poorly assembled using crap cells.  I made a replacement pack using 30Qs, doubled the capacity from 10S2P to 10S4P and managed to get the whole thing to fit in the original battery case.  This worked out like a charm, but the other issues remained.

Next, I cut a hole in the board using a waterjet (Its a solid metal deck) thinking the issue might be signal blocking.  This did not resolve the issues.

Finally, I tried buying a replacement ESC/remote from Ownboard.  Its one of the newer chinese cheap ESC/controllers.  I got all of this hooked up today finally but the motors only spin veeeeerrrryyyy slowly.

Incidentally, the motors look exactly like the Maxfind motors [linked here](https://www.maxfindboards.com/collections/accessories/products/skateboard-hub-motor).

I stupidly thought it would just work, but clearly something isn't right.  Could it be that the motors I have are wye and the ownboard ones are delta or vice-versa? Is there any way to modify/adjust the ownboard ESC?  Am I better off buying a set of motors and the truck for the ownboard or replacing the ESC/controller with something else?
```

---
## \#2 Posted by: MiniChopper4Me Posted at: 2018-10-12T03:05:05.254Z Reads: 100

```
![image|281x500](upload://y86xLewaEbvjzjNTMeQyGXztzx.jpeg) ![image|383x499](upload://wYmctYxSp8bCsCsXnC1OPFaRAMc.jpeg) ![image|375x500](upload://yiid2XehnKdgP5crgLeyQzxjedf.jpeg) ![image|281x500](upload://AqWHGX8NGjS83BV6YeK58lE9lr5.jpeg) ![image|375x500](upload://5xByq7hpVSAQcN3azZz2DDZ3I0h.jpeg) ![image|375x500](upload://zkN43f3QRioK57sPgXKfGSPAfRx.jpeg) ![image|666x500](upload://kxJ5fuFnl76eZDAWFotw41Mfb9j.jpeg) ![image|375x500](upload://hX9MGG9VNWDEh97rpmA7rnC4x1l.jpeg)
```

---
## \#3 Posted by: mynamesmatt Posted at: 2018-10-12T03:29:07.038Z Reads: 76

```
Use a vesc or focbox and test to see if the motors run faster at all
```

---
## \#4 Posted by: dareno Posted at: 2018-10-12T09:14:41.894Z Reads: 58

```
They look like the koowheel hubs.  Difficult to tell but they are similar and if so are not bad.  As my fellow aussie said don't mess about with the chinese bespoke esc's at all and bite the bullet with some proper vesc.  You don't need to go focbox with those just a decent 4.12 vedder based unit like a HK or TB version.  Then you can set everything up properly.  Use a benchwheel remote receiver too.  Vedder switch set up and the board will be ALIVE!   Its ALIVE!

ps that deck is full batman dude.  Theme it up
```

---
## \#5 Posted by: pat.speed Posted at: 2018-10-12T12:27:51.266Z Reads: 47

```
I’m hearing good things about the flipsky vescs too, which are currently the cheapest in the market
```

---
## \#6 Posted by: brenternet Posted at: 2018-10-12T12:59:41.176Z Reads: 40

```
Yes and no. 4.12 single and 6.6 dual and single are worth your money. 4.20 dual and single mini are not up to scratch at present.

Best bang for your buck by miles are the 4.12 singles, they can be had for so little on ebay through an offer to the seller.
```

---
## \#7 Posted by: MiniChopper4Me Posted at: 2018-10-12T20:46:19.270Z Reads: 33

```
I played around with it some more.  Turns out I needed to change the connectors around for the hall sensors.  The Kuickwheel ESC had the outputs with ground, 5v, then sensor sensor sensor.

Once I got the cables in the right order, the motors spin, but there's cogging, stuttering, all kinds of mess.

I ended up buying a flipsky 4.20 dual and the photon plus a flipsky power switch.  Guess I should've read the issues with the 4.20 before buying it.
```

---
## \#8 Posted by: MiniChopper4Me Posted at: 2018-10-23T18:15:24.170Z Reads: 19

```
With the 4.20 dual, everything works great so far, at least on the bench.  But after doing much more reading and spending, I'm now at a point where I'm planning on building 2 more decks, 1 out of the failed Serpent-W, and another custom board.

The Serpent-W will be rebuilt using the SkullboardVIP wheels once they get here with a 10S4P 30Q pack.  First I'm going to do it with the ESC/remote it comes with (I wanted to test the possibility for other Serpent-W owners who are not DIY inclined), but this implies not being able to use the lights the board comes with.  At the end, I plan to use these motors/wheels with the Flipsky 4.20 dual and hopefully a Photon remote so that I can also wire the lights.  I've also bought ceramic bearings for the motors to replace the crappy ones they come with.  I expect the very stiff deck to pair well with the airless tires.
```

---
