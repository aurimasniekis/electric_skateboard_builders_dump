# Cell error lipo battery

### Replies: 44 Views: 3531

## \#1 Posted by: Samuele00 Posted at: 2018-01-27T12:32:04.828Z Reads: 121

```
I have a 30c 3s turnigy lipo battery and when I connect it to the charge it tells me "cell error invalid voltage", I have an imax b6, what can I do?
```

---
## \#2 Posted by: rojitor Posted at: 2018-01-27T12:34:25.147Z Reads: 122

```
Is the balance cable properly connected?
```

---
## \#3 Posted by: Samuele00 Posted at: 2018-01-27T12:39:52.043Z Reads: 121

```
Yes,it's correct
```

---
## \#4 Posted by: E1Allen Posted at: 2018-01-27T12:40:20.691Z Reads: 108

```
What's the voltage of each cell
```

---
## \#5 Posted by: E1Allen Posted at: 2018-01-27T12:40:36.457Z Reads: 105

```
Do you have a way to check it?
```

---
## \#6 Posted by: Samuele00 Posted at: 2018-01-27T12:44:33.926Z Reads: 96

```
3.18 3.19 2.45 , It's a problem...
```

---
## \#7 Posted by: E1Allen Posted at: 2018-01-27T12:46:47.906Z Reads: 96

```
Yeah. That cell is bad. Most likely trying anything at this point would just be a bandaid for that cell.  Only real safe choice is replace that battery pack.
```

---
## \#8 Posted by: Samuele00 Posted at: 2018-01-27T13:58:43.504Z Reads: 94

```
I havent any money .....
```

---
## \#9 Posted by: Blitz Posted at: 2018-01-27T14:11:15.658Z Reads: 91

```
Are you still under warranty?
```

---
## \#10 Posted by: Samuele00 Posted at: 2018-01-27T15:18:47.557Z Reads: 82

```
I bought it a fra mounth ago
```

---
## \#11 Posted by: Namasaki Posted at: 2018-01-27T16:15:26.204Z Reads: 77

```
[quote="Samuele00, post:6, topic:44788, full:true"]
3.18 3.19 2.45 , It’s a problem…
[/quote]

In reality, all 3 cells have been over discharged. 
You probably have some swelling at this point. 
The internal resistance of the lowest cell is probably very high now. 
The only safe and practical option now is to replace the pack. 
And avoid discharging below 3.6v
```

---
## \#12 Posted by: wafflejock Posted at: 2018-01-27T16:24:30.097Z Reads: 72

```
Agree just chalk it up as a loss not worth trying to recover at best it will work crappy for one or two more runs, at worst you have a near impossible to extinguish chemical fire.  Good side is you only killed a 3S, I did the same to a 6S.
```

---
## \#13 Posted by: Samuele00 Posted at: 2018-01-27T16:39:18.497Z Reads: 67

```
The cell didn't blow up. Is  there a way to bring it to a normal voltage?
```

---
## \#14 Posted by: xBRAZILx Posted at: 2018-01-27T16:39:31.476Z Reads: 64

```
i had the same issue last week.
1 cell of my 3s battery swelled as f...

i left cool down and the swell was gone,but the battery was all unbalanced.
i put to charge with 0.5A (normally i charge with 3.0A) and the battery come back working/charging normally.

i guess what happened to me was that i went to long and steep hill to test if the regenerative brakes really charge the battery. went that after this 2 min braking on this hill, 1cell get swelled, but this battery is also very old though.

but, the cell that i mentioned is a little puffy nowadays...
```

---
## \#15 Posted by: Samuele00 Posted at: 2018-01-27T17:02:11.795Z Reads: 59

```
How can i resolve the error on the charger? so that i can charge the cell
```

---
## \#16 Posted by: mmaner Posted at: 2018-01-27T17:03:17.168Z Reads: 58

```
Try what @xBRAZILx just suggested. If that doesn't work you need a new lipo.
```

---
## \#17 Posted by: Samuele00 Posted at: 2018-01-27T18:13:58.550Z Reads: 57

```
Could you tell me how can i set the recharge? I am not able to use the charger, and online i did't find nothing.
```

---
## \#18 Posted by: E1Allen Posted at: 2018-01-27T18:22:04.186Z Reads: 56

```
You either charge the one cell from the balance lead with tiny pins or instead of lipo balance charge you do lipo charge to attempt to get the low cell up near the others then balance charge should work
```

---
## \#19 Posted by: Samuele00 Posted at: 2018-01-27T19:04:48.737Z Reads: 53

```
Sorry  i'm Italian and i don't understand  :pensieroso:
```

---
## \#20 Posted by: leo Posted at: 2018-01-27T20:21:51.314Z Reads: 51

```
charge for 60 seconds nicad instead of lipo then interrupt and load normally lipo balance sorry my english is italian
```

---
## \#21 Posted by: leo Posted at: 2018-01-27T20:25:24.722Z Reads: 50

```
se vuoi scrivimi privato ti spiego sono italiano anche io
```

---
## \#22 Posted by: louwii Posted at: 2018-01-27T21:00:17.601Z Reads: 48

```
So you recommend setting the cutoff voltage at 3.6 in the VESC ?
Mine is set at 3.3 right now :confused:
```

---
## \#23 Posted by: Namasaki Posted at: 2018-01-28T03:07:23.089Z Reads: 49

```
Yes because the Vesc will monitor the total pack voltage not individual cells.
So to protect against out of balance cells going too low, you have to use conservative limits.
3.6 or 36v on a 10s pack is fairly safe.
```

---
## \#24 Posted by: wafflejock Posted at: 2018-01-28T06:29:45.186Z Reads: 51

```
I've had mine at 37V-35V (for 10S) as the soft-hard cut off limits for a while now and haven't had issues but better to start at 38V-36V at first and see when the VESC does hard cut off what the individual cells are at and how far off they are from each other then make the call from there if it's worth bumping it any lower to get those last drops of juice (probably not).

Need to keep in mind when the batteries have current flowing there is also a corresponding dip in voltage (if your cells go over the voltage cliff there is no real return to 100%).

https://www.rctech.net/forum/attachments/electric-road/398648d1229845264-smc-40c-c-max-7-4v-hardcase-lipos-5000mah-pro-race-40c-cell-discharge-curve-graph.jpg

---

Note not my actual battery but just a generic lipo discharge graph, results vary depending on the specifics of the cell.
```

---
## \#25 Posted by: louwii Posted at: 2018-01-28T07:59:35.490Z Reads: 38

```
Thanks guys, the weather is really crappy here, I didn't have the "chance" yet to run my board until the battery is flat. I'm gonna raise the cut-off limits to be safe.
```

---
## \#26 Posted by: pat.speed Posted at: 2018-01-28T11:12:05.704Z Reads: 37

```
I have over discharged a cell to 2.9v before and was able to recharge it but the pack was never very good after that. If you really don't want to buy a new one you can charge it without the balance plug until all cells are above 3v just do it slowly, around 0.5amps. 

If you don't understand some of the words very well you can try using google translate although it's not very accurate.

Bouna Fortuna e essere sicura
```

---
## \#27 Posted by: rojitor Posted at: 2018-01-28T11:13:47.526Z Reads: 35

```
Once any cell is discharged beyond 2.7v the damage is permanent. That lipo is very dangerous even if you manage to charge it and use again.
My advice is to dispose of it.
```

---
## \#28 Posted by: pat.speed Posted at: 2018-01-28T11:14:49.709Z Reads: 35

```
I agree it is best not to use the same pack but if you must it is possible although there is a good chance of it going boom
```

---
## \#29 Posted by: Namasaki Posted at: 2018-01-28T17:12:41.878Z Reads: 34

```
[quote="pat.speed, post:28, topic:44788, full:true"]
I agree it is best not to use the same pack but if you must it is possible although there is a good chance of it going boom
[/quote]

Safety First!
Trying to resurrect a battery like that one is not worth the risk.
```

---
## \#30 Posted by: Blitz Posted at: 2018-01-28T18:00:07.773Z Reads: 33

```
What about using a 0.1" header to charging port and charge through balance lead would the cell go up
by any chance?
```

---
## \#31 Posted by: wafflejock Posted at: 2018-01-28T18:08:07.623Z Reads: 33

```
Yes but this is a bad idea.  Suggested above already but that's what namasaki is saying is dangerous (also the cell will still drift/drop in voltage more quickly than the others still so chance of permanent failure and a worse situation are very likely).  I "recovered" my cell for maybe  3 more rides before it just couldn't charge at all anymore, especially at 3S worth it to just replace the damaged battery chalk it up as an experience and don't let your cell voltage get so low again.  There is nothing to do now except figure out how to safely dispose of the lipo and find a new replacement one.
```

---
## \#32 Posted by: Blitz Posted at: 2018-01-28T20:42:25.809Z Reads: 30

```
OH yeah that makes sence,

What do you count as healthy voltage cutoff,
and how long did you lipos last?
```

---
## \#33 Posted by: Namasaki Posted at: 2018-01-28T22:39:38.649Z Reads: 28

```
[quote="wafflejock, post:31, topic:44788"]
chalk it up as an experience and don’t let your cell voltage get so low again.
[/quote]


Well said @wafflejock

I learned my lesson about over discharging the hard way with my first build.
I ruined 2 brand new 6s packs because I just wanted to ride a little more.
Wound up having to trash them.
```

---
## \#34 Posted by: wafflejock Posted at: 2018-01-28T22:40:49.740Z Reads: 29

```
First ones I got were the multistar 6S 10Ah ones (huge, basically a regular masonry brick worth of lithium) they only lasted a couple of weeks though due to the overdischarge and just bad mounting attempts leading to things being scraped along the pavement etc.  I went from 12S down to 6S to not be using the one that was overdischarged and rode with that for like a week but really hard going from 12S to 6S feels like the thing is barely moving.  After that I got two 5Ah 5S 20C (hooked in series for 10S) Turnigy batteries and I've been using those for the last year or so (when the weather is nice was riding daily when it's crappy I ride like once a week still when a dry day appears).  Haven't done real close monitoring of them just checking the cells when I go to charge and things stay +/- .1V cell to cell so think things are still in good condition.  Would have to do more rigorous testing to see how much charge they are still holding now though.  Just based on feeling I'd say they are starting to wear some but it's not like I'm down to 50% capacity or anything.  If things are kept above the drop for voltage for the given cells then you should get about 150-200 cycles (full discharge/charge cycles) before starting to see a serious drop in capacity:

https://www.rcgroups.com/forums/showthread.php?1492938-How-many-cycles-should-we-get-from-a-good-lipo-battery

From what I gather the two most important things for longevity is 1 keep the cells above the minimum voltage and 2 don't store the cells fully charged (I typically charge and go cruise to bleed off some power, that's what I tell myself)

https://www.rcgroups.com/forums/showthread.php?403523-Storing-Lipo-Batteries-Fully-Charged!

---

With 185Wh I can get around 10-12 miles comfortably (flat land in Chicago and I'm like 115lbs or so) without pushing things to the limit, and since I generally am only making a few mile trips I can basically charge, then ride 2 or three times and then have to charge again (12 miles is the longest I've cruised on a single trip).  I setup my batteries so they are in trays that slide in and out and lock in with xt-90s to connect them to the rest of the circuit so I can at some point here throw down on some more 5Ah packs and swap between them if I need/want the extra range when just straight cruising with others or whatever (as is it's just used as a commuter board).
```

---
## \#35 Posted by: pat.speed Posted at: 2018-01-28T23:46:48.797Z Reads: 24

```
Oh yeah I also forgot to say that those lipos I had wouldn't charge past 4v lol. I just use the less damaged 3s for other things now like powering low current 12v devices
```

---
## \#36 Posted by: Hansg Posted at: 2018-01-29T17:27:16.318Z Reads: 21

```
I charged my lipo in mode NiCd to 1.3a![P_20180129_122409|281x500](upload://lMg4Tit3wvhE1iMQvsBHpwGdq05.jpg)![P_20180129_122403|281x500](upload://dDo6OFjIp8rLkMvKJwDHxf8genO.jpg)
```

---
## \#37 Posted by: Samuele00 Posted at: 2018-01-29T18:16:29.029Z Reads: 21

```
And does it function?
```

---
## \#38 Posted by: Hansg Posted at: 2018-01-29T19:19:03.236Z Reads: 21

```
Yes, is necessary only connected the cable xt60.
```

---
## \#39 Posted by: wafflejock Posted at: 2018-01-29T19:29:33.004Z Reads: 21

```
Don't do this... If you hook up the xt-60 you are pumping power into all the cells not just the ones that are too low, also different batteries use different charge profiles.  At best your battery will work for another week and you're creating a fire hazard to save $30

---

Sell some lemonade, mow a lawn, shovel a driveway or two and you should be able to replace it without risking burning your house down.
```

---
## \#40 Posted by: Samuele00 Posted at: 2018-01-29T21:32:20.066Z Reads: 18

```
the battery with shipping is € 50
```

---
## \#41 Posted by: Blitz Posted at: 2018-01-29T21:39:45.229Z Reads: 18

```
Dude If you really want to give the battery the best shot then charge the weak cell trough the balance port and keep an eye on the battery and keep checking to see if it is overheating and do this experiment in a fire safe area.
```

---
## \#42 Posted by: pat.speed Posted at: 2018-01-29T21:48:12.004Z Reads: 16

```
HobbyKing now has free shipping and a 20c 3s 5000mah lipo cost €18
```

---
## \#43 Posted by: E1Allen Posted at: 2018-01-30T05:12:13.437Z Reads: 14

```
He could remove the bad cell if he is going to try and keep using the battery. But he charged them all low either way
```

---
## \#44 Posted by: pat.speed Posted at: 2018-01-30T05:21:35.350Z Reads: 14

```
Yeah I ended up doing that to one cell
```

---
