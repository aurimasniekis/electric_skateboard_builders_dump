# Mounted LiPo Safety (Storage and Charging)

### Replies: 14 Views: 1862

## \#1 Posted by: dstnceswmer Posted at: 2016-12-14T16:39:29.824Z Reads: 198

```
So I'm still in the process of putting together my first eboard and through reading I have been doing I am becoming more and more concerned about LiPo safety. I live in a city apartment and as such do not have access to anywhere outdoors, or a cement floor, to store/charge my board. I am using two 6s batteries wired in series for a 12s configuration. I wanted to have an easy 1 port charging solution so I incorperated a 12s BMS in my design allowing me to just use a DC barrel plug bulk charger for charging. That being said the setup is such that I do not want to be taking apart my battery enclosure every time I want to charge my board. 

I have been trying to think of a safe way to store/charge my board in my apartment so as not too come home and have the whole building burned down (yes I know not to leave a charging battery untended, was referring more to storage in that case). 

I was wondering if I built a thick-ish (1/2")plywood box lined with some aluminum sheet metal that was big enough to store my entire board in, if that would be adequate protection against a 12s LiPo fire? Also do not have a ton of room or $ so didn't want anything as overkill as say a gun safe or anything.
```

---
## \#2 Posted by: Hummie Posted at: 2016-12-14T16:48:18.505Z Reads: 188

```
I haven't gotten a Lipo to burn up yet and don't know their potential but maybe pour a concrete box instead of wood.  Cheaper.
```

---
## \#3 Posted by: darkkevind Posted at: 2016-12-14T16:51:43.348Z Reads: 184

```
Get a tool safe that one might have in the back of a pickup. That said, you're pretty safe, as long as you're not abusing your batteries, they won't rebel.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-12-14T17:58:44.572Z Reads: 162

```
The lipo danger is a danger exacerbated by vendors who are profiting more from selling li-ion batteries. Lipos will NOT just blow up unless they were very poorly manufactured. Buy a respected brand's lipos (zippy for example) and they are not going to just blow up, unless you over discharge below 2.8v per cell and charge them again.

Lipos that blow up almost always blow up during charging, and it's always due to abuse or poor manufacturing. If you get cells, and charge and discharge them a few times, then they very likely don't have any manufacturing faults, and will only blow up if you abuse it.

Lipos from my testing are much better for electric skateboard use than li-ion. I think the li-ion trend is just a fad. It will blow over as people realize they can get far better performance (less sag, more range, high speeds for longer times (due to their better discharge curve)) from lipos. Lipos are better IMO until we get a better, high discharge battery.
```

---
## \#5 Posted by: Hummie Posted at: 2016-12-14T18:15:23.314Z Reads: 151

```
But occasionally lipo will blow up while not charging or discharging.  Just yesterday I was searching for incidences of this happening and there are at least a couple documented cases 

https://www.rcgroups.com/forums/showpost.php?p=34412643&postcount=44
```

---
## \#6 Posted by: dstnceswmer Posted at: 2016-12-14T18:23:48.453Z Reads: 148

```
yeah, I have seen a few as well in my searching, just want to be as safe as possible. I like the idea of puouring a thin walled concrete shell to put in a sort of decorative wooden box. As for a tool safe, those things are quite $$$ from what I've seen online.
```

---
## \#7 Posted by: Kaly Posted at: 2016-12-14T19:24:07.499Z Reads: 140

```
@dstnceswmer 
This will give you peace of mind 
 http://m.ebay.com/itm/30cal-M19A1-7-62mm-30-Caliber-Ammo-Can-Box-Military-Surplus-/291966653914?hash=item43fa9195da%3Ag%3AlXYAAOSw%7EoFXJN0S&_trkparms=pageci%253Aad7b969c-c232-11e6-bec7-74dbd1a08b97%257Cparentrq%253Afec95e641580a7873954a09effd6bd5a%257Ciid%253A14
```

---
## \#8 Posted by: smurf Posted at: 2016-12-14T19:42:20.724Z Reads: 126

```
Fire rated "purple plywood" is a option for use in a 1 hour firewalls. It should contain a battery fire. Add 2 layers of 5/8 drywall on the inside and it would take a thermite grenade to burn through.
```

---
## \#9 Posted by: dstnceswmer Posted at: 2016-12-14T19:43:08.850Z Reads: 130

```
thanks but remember, not looking to remove batteries from board, and don't think my whole board will fit in that sized box lol :)
```

---
## \#10 Posted by: i2oadsweepei2 Posted at: 2016-12-14T19:54:22.820Z Reads: 131

```
The next enclosure I make out of fiberglass I'm going to buy a few lipo safe bags from hobbyking and cut them up to line the bottom of the board and the inside of the enclosure with. In hopes of containing any potential fire. With that said I remove my lipos and inspect them after every use and to charge them too. Like said above I store them in lipo bags inside of ammo boxes. Just incase.

<img src="/uploads/db1493/original/3X/d/8/d8bbc68b7a211879da16403640741064d0117025.JPG" width="669" height="499">
```

---
## \#11 Posted by: treenutter Posted at: 2016-12-14T20:26:52.805Z Reads: 124

```
@dstnceswmer I store mine in a lipo bag removed from the board. Buy quality lipos, use a balance charger at the right settings, and make sure they don't get damaged by impact or puncture. Obviously don't over-charge or over-discharge. I've never had a problem, but stay cautious. 

<img src="/uploads/db1493/original/3X/f/5/f5008a5a56313417c32a38e0dd328ec2f53e1577.jpg" width="333" height="250">
```

---
## \#12 Posted by: jmasta Posted at: 2016-12-14T20:34:12.038Z Reads: 120

```
My LiPos permanently live in firesafe bags.  The bags are then velcroed to the board and encased with an aluminum enclosure.  With the addition of a BMS and conservative voltage cutoffs programmed into VESC, I have very little concerns of them causing problems.

Stop discharging at 3.5 or 3.4V/cell, and you should never have problems.  There is very little energy left in the lipos after 3.6V/cell, so you really are not losing much capacity at all by doing this.  It also recommended to only charge to 4.15V, instead of 4.20V
```

---
## \#13 Posted by: dstnceswmer Posted at: 2016-12-14T20:47:35.007Z Reads: 120

```
ok, yeah I have a 3d printed hard enclosure I designed right now. think I'll redesign it a bit larger to accommodate a LiPo bag in there as well. 

As for charging cuttoff, with the BMS I installed won't a bulk laptop style charger stop charging at the correct point or do I need to break out the DMM to monitor the cells?
```

---
## \#14 Posted by: kidcisco Posted at: 2017-06-10T01:53:19.856Z Reads: 80

```
Firesafe bags inside a fireproof document safe for charging. I also go the extra mile and make sure I wear this while I'm riding, just to be safe. 

http://www.macronsafety.com/media/catalog/product/cache/1/image/650x/c56438956073d445ecf1fb001fab99f6/c/p/cpa-aluminized-fire-proximity-suit.jpg
```

---
