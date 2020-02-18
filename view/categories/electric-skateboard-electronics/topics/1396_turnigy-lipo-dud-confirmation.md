# Turnigy LiPo dud confirmation

### Replies: 4 Views: 806

## \#1 Posted by: SpartanScrub Posted at: 2016-02-16T09:43:17.882Z Reads: 55

```
Finally got my board running and unfortunately wasted one of my LiPo batteries in the process. I'm using [ 2 Turnigy 5000mAh 5S 20C Packs][1] connected in series to a VESC. When I started the ride, both packs were brand new at about 20V each with no more than a 0.02V difference between each cell. After a little test riding, the board finally shutdown at 30V (which looking back was probably way too low, especially for testing). Excited/nervous to charge Lipos for the first time, I saw that one of them caught a case of the puffs. The dud had dropped to 12V (2.4V/cell) while the good battery was still over 18V. 

Is this just a case of a bad LiPo (from reading @onloop it does not seem to be uncommon) and not an issue with the VESC regen that I need to figure out? I had it set to the default, motor min -60A and batt min -20A.  

Here's how I connected the batteries just to make sure I didn't have a brain fart on something so trivial<img src="/uploads/db1493/original/2X/d/de146d0dd7abf53126b4775c639798ddedd79a2e.jpg" width="446" height="500">

The puffy battery also did start off about 2mm thicker than the good one when it arrived brand new, so that is sort of why I jumped to the conclusion that it was the battery's fault and not mine. Anyway, just though I'd ask now before I burn through some more crappy/cheap hobbyking batteries.

  [1]: https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=58990
```

---
## \#2 Posted by: laurnts Posted at: 2016-02-16T10:30:05.402Z Reads: 48

```
Well you just smoked out your lipo i guess. Over draining them to the end. Lipo needs to get recharged when they are 3.2V - 3.4V left. If you drain them below 3.0V then you might just finished that lipo life / cut down the lifecycle significantly.

The connection is ok, thats correct for setting it in series for getting 10s.
```

---
## \#3 Posted by: Kaly Posted at: 2016-02-16T10:59:41.625Z Reads: 47

```
Lipos are always a guessing game next time when receiving batteries perform a  proper inspection before using them. This should have been a red flag. 

[quote="SpartanScrub, post:1, topic:1396"]
The puffy battery also did start off about 2mm thicker than the good one when it arrived brand new
[/quote]

And this batteries for the 1-3 uses need to keep the load low in order to break them in. 

One more thing, Get rid of that pack, is too much of a fire hazard in you living place.
```

---
## \#4 Posted by: SpartanScrub Posted at: 2016-02-16T11:21:10.802Z Reads: 43

```
Yea I have it outside on some bricks by itself in a metal trashcan until I figure out what to do with it/where to dispose of it. I've see videos of what happens when  a cell phone lipo burst so I'm guessing the 5 cell going up in flames wouldn't be pretty. 

Thanks for the tip though, I'll be sure to go easy on the next pack to start off.
```

---
