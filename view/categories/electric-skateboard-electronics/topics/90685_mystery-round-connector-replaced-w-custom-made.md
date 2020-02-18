# Mystery round connector \[replaced w/ custom made\]

### Replies: 9 Views: 305

## \#1 Posted by: bluegreen Posted at: 2019-04-16T00:37:46.562Z Reads: 94

```
Hello I've spent some hours unsuccessfully searching for this connector. The close I've got is some kind of amphenol connector but I don't think that's right it's from a chinese board so probably in metric? These measurements are approximate.

If anyone even just knows what these kind of connectors are called or help narrow my search, I guess something like this would be on digikey...

The replacement battery I ordered came with a 4 pin version and I need to a 3 pin version.

![connector|563x500](upload://lY12TPikWg8T6Pe0fIzStlzmRql.png) ![20190415_173131|666x500](upload://7REyOiWwhqt2Z5teljbBkkQPxTL.jpeg) ![20190415_173144|666x500](upload://s0Dnt1bVmAQvVaLLl5r42hbyPbL.jpeg) 

This is an example of the 3 pin connector I need. If anyone has any ideas, thanks!
```

---
## \#2 Posted by: b264 Posted at: 2019-04-16T00:38:24.672Z Reads: 89

```
It's a GX16-3
```

---
## \#3 Posted by: bluegreen Posted at: 2019-04-16T00:47:03.025Z Reads: 83

```
That for sure gets closer! I think the pinout is compatible but all my searches online seem to show the inverted gender, and slightly different style keyway.

![image|505x321](upload://aNRJSPInefPuEeIeApEMAb5vRFB.jpeg) 

The keyway probably isn't important but finding a panel mount female connector is the trick I guess.

Thanks for the quick reply!
```

---
## \#4 Posted by: b264 Posted at: 2019-04-16T00:48:32.583Z Reads: 77

```
Yes, upon closer inspection, it *appears* to be a

"GX16-3 that's been modified to be proprietary and not obtainable anywhere else so you have to pay up"
```

---
## \#5 Posted by: b264 Posted at: 2019-04-16T00:50:07.303Z Reads: 75

```
I would just change it all over to actual GX16-3 and be done with it.
```

---
## \#6 Posted by: bluegreen Posted at: 2019-04-16T00:51:55.728Z Reads: 73

```
Probably good advice, I'm going to continue the search now that I at least know the pinout it should match.
```

---
## \#7 Posted by: Namasaki Posted at: 2019-04-16T00:55:38.143Z Reads: 69

```
Good advice from @b264
You'll probably be trying to find a match for the proprietary version until the cows come home.
Best option is to replace both connectors with the generic version.
```

---
## \#8 Posted by: bluegreen Posted at: 2019-04-16T01:47:38.738Z Reads: 59

```
Ordered some GX16-3 I think I might be able to retrofit the female part to the inside of the part I already have. It appears to be held in place with a set screw so if the diameters are compatible I just need to drill out the current guts, replace it with this and then drill in a place for a set screw.

If it doesn't work I'll just give up and focus on building my own board instead of repairing crappy Chinese ones. :slight_smile:
```

---
## \#10 Posted by: bluegreen Posted at: 2019-04-18T20:12:53.640Z Reads: 27

```
![20190417_151957|666x500](upload://5UCCzEzFCePxhBz0lNycEDNiF2p.jpeg) 

Drilled out the old connector.

![20190417_152557|666x500](upload://6ZFfwB139Nq7QK6ooXiTc7LTzV6.jpeg) 

Left plastic on the internal diameter to match the insert. Had the perfect size drill bit already, hooray!

![20190417_153713|666x500](upload://66MH3HOcgDa5by2i5u6PrcA7Mzt.jpeg) 

Drilled the hole for the lock screw (in the wrong place, had to do it again).

![20190418_124423|666x500](upload://xwVy2aCGpMWfCXdCRWgnZnKKx3r.jpeg) 

And... voila! The connector is a bit fussy to get on/off compared to the "original" one that uses a rubber surround. But it works!

Anyways if anyone is curious this was because I bought an Onan x2/x3 battery thinking it would work for the x1, but after ordering it found out the connector was different. Don't be like me.
```

---
