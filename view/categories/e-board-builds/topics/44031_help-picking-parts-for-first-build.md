# Help Picking parts for first build

### Replies: 23 Views: 1222

## \#1 Posted by: Acklavidian Posted at: 2018-01-18T18:20:52.569Z Reads: 158

```
Got a boosted board a while back, and I have really been enjoying the experience so far. However, I really like to tinker, and build things which my boosted board doesn't facilitate very well. I do have some 3d printed wheel hacks that I'm waiting to receive parts for, but this isn't enough. I've been lurking for a while, and doing a lot of research but feel a little overwhelmed with options and don't know which direction to go and how to meet my specification requirements. 
Use case:
* Daily commute 4 miles one way.
* Road quality varies wildly from smooth to astrological impact event.
* Body weight 230lbs

Desired specs:
* flexy deck
* 25mph+ crusing speed
* range 10mi+ 
* skate or AT wheels

I've been trying to decide between Trampa or Loaded Icarus. Leaning toward Icarus right now. This parts list  was largely inspired by: [This](https://www.electric-skateboard.builders/t/1250-build-36-mph-and-15-20-mi-range/36815) build by @Mattmccrary8  
Prospective parts:
* deck - Loaded Icarus - $215
* trucks - TB 218mm - $65
* motors - TB 6374 190KV x2 - $240
* mounts and pulleys - TB SINGLE BOLT ON MOTOR MOUNT W/ DRIVE WHEEL KIT 16/36 x2 - $216
* wheels - abec 11 - already own
* Nano remote - $25
* Male to male service - $3
* TB VESC 4.12 - x2 - $200
* VESC canbus - $2
* Vesc connector - $7 

Still trying to figure out how to accommodate a 12s4p battery on a flexy board. This is the most intimidating part for me as I don't have a spot welder, but I suppose if need be I can get one. However, the N.E.S.E. packs seem like a viable option. So for the battery I have:
* Samsung 25r 18650 2500mAh 20A x 48 - $240
* NESE module x 12 - $132
* Custom fiber-glass enclosure

What do y'all think so far? What am I missing?
```

---
## \#2 Posted by: Colson003 Posted at: 2018-01-18T18:36:55.478Z Reads: 124

```
Where are you getting your cells? $5 a cell for 25R is very high. You can get the 30Q from nkon for about $4 per cell.
```

---
## \#3 Posted by: Acklavidian Posted at: 2018-01-18T18:58:00.268Z Reads: 119

```
Literally just googled it and used the first link. I'm not trying to do super cheep, but always happy to save.
```

---
## \#4 Posted by: PredatorBoards Posted at: 2018-01-18T19:04:36.602Z Reads: 119

```
2 **very different** decks. If you ask me, I suggest looking into the DB Longboards Coreflex decks. They're wider than the Icarus, which makes for better/easier turning and carving. The trampa is a completely flat deck that will make your feet slide off really easily when you hit bumps. I personally believe the only way to use those decks is with bindings. Otherwise you have no business using them.


You are also overpaying for your 25R cells. Might as well get 30Q cells for the that price/budget.
```

---
## \#5 Posted by: Mathias Posted at: 2018-01-18T20:05:43.716Z Reads: 104

```
[quote="Acklavidian, post:1, topic:44031"]
Still trying to figure out how to accommodate a 12s4p battery on a flexy board.
[/quote]

This ia definitely a tricky thing to do. The two options are either a segmented enclosure, or making short, thick enclosures sitting close to the trucks. But be careful: flex and battery don't mix very well. We got a few examples here of power cutting out, or even batteries catching fire. 

I got a vanguard with split enclosures: 
https://www.electric-skateboard.builders/t/first-build-vanguard-dual-tb-6355-190kv-tb-vesc-10s4p-lg-hg2-alien-mounts-paris-195mm-alien-remote/24295/41

And I am really happy with the flex! On the Icarus and this type of enclosures you'll probably get into trouble with the ground clearance unless you don't drop-through your trucks. 

Another thing to keep in mind is that split enclosures come with long battery cables, which is a problem for FOC or for unreliable VESCs, and at the moment a lot of people count TB's VESCs among them. I recently blew two of them in BLDC mode. You might want to get FOCBOX instead. I now regret that I didn't.
```

---
## \#6 Posted by: PredatorBoards Posted at: 2018-01-18T20:10:38.253Z Reads: 86

```
As long as the VESC is using the proper caps as designed by Vedder, there shouldn't be too much of an issue with surges. I'd just stay off of FOC altogether, as it's just another thing to potentially cause problems down the line.
```

---
## \#7 Posted by: Mathias Posted at: 2018-01-18T21:42:42.019Z Reads: 82

```
Well, I even added two large caps plus I left the ones that the two TB VESCs shipped with in place untouched. FOC blew one within seconds. Seitched to BLDC since. One one of them kept holding up, two more blew after quite a short time. I'm not even alone with the problem. At the point when I started my build I had the impression that TB VESCs are just fine. But recently there have been lots of reports of TB VESCs blowing for no apparent reason. So I don't know... Now I've been running one Ollin and the one working TB VESC for a long time, nothing changed in my config or my setup. But 2/3 failure rate is not exactly great (not even counting the one blown in FOC, which was supposed to work with 10s and the extra caps!).
```

---
## \#8 Posted by: Acklavidian Posted at: 2018-01-18T21:52:20.182Z Reads: 92

```
> The trampa is a completely flat deck that will make your feet slide off really easily when you hit bumps. I personally believe the only way to use those decks is with bindings. Otherwise you have no business using them

I would definitely do bindings with a trampa.

> You are also overpaying for your 25R cells. Might as well get 30Q cells for the that price/budget.

I don't know the difference between 30q and 25r
```

---
## \#9 Posted by: mmaner Posted at: 2018-01-18T21:53:59.571Z Reads: 91

```
Here are the best binding available for a street deck...
https://store.freebord.com/s2-bindings/
```

---
## \#10 Posted by: Acklavidian Posted at: 2018-01-18T21:56:57.360Z Reads: 87

```
@Mathias FOCBOX it is. Do I run 2 of those as well? What are caps?
```

---
## \#11 Posted by: PredatorBoards Posted at: 2018-01-18T22:01:35.996Z Reads: 87

```
30Q cells have 500 mah more capacity. In a 4P setup like yours, that's another 2000mah of extra capacity or roughly 5 more miles of range. The 30Q cells also hold their voltage better versus the 25R at higher discharge rates.
```

---
## \#12 Posted by: Mathias Posted at: 2018-01-18T22:04:38.928Z Reads: 80

```
Yes. FOCBOX is an upgraded version of the VESC 4.12. You can replace it 1:1, exept it's less prone to failure and can run more current.
```

---
## \#13 Posted by: Acklavidian Posted at: 2018-01-18T22:09:29.716Z Reads: 75

```
@PredatorBoards DB Longboards Coreflex decks put me at the very edge of their weight spectrum 😑.
```

---
## \#14 Posted by: Acklavidian Posted at: 2018-01-18T22:11:43.916Z Reads: 75

```
Are 30Q physically larger? Where do you look for cells in the US?
```

---
## \#15 Posted by: Colson003 Posted at: 2018-01-18T22:13:36.666Z Reads: 73

```
ru.nkon.nl or liionwholesale.com

30q and 25r are the same size.
```

---
## \#16 Posted by: Acklavidian Posted at: 2018-01-18T22:27:12.390Z Reads: 71

```
Would the 30Q be too much for the nese modules?
```

---
## \#17 Posted by: Mathias Posted at: 2018-01-18T22:49:20.359Z Reads: 70

```
[quote="Acklavidian, post:10, topic:44031"]
What are caps?
[/quote]

Capacitors. The hight currents paired with high inductance (e.g. from long battery cables) lead to voltage spikes that can your electronics when the motor controller changes the current. That's why the vesc needs protective capacotors that short out fast current fluctuations. FOC produces more spikes and is therefore much more dangerous to blow your vesc. That's why for long battery cables (like I got it with the split enclosures) it's a good idea to put extra caps/larger ones than the ones that your VESC ships with. Especially in FOC. With FOCBOX you should be fine without extra caps, at least in BLDC mode. FOC on FOCBOX with extra long battery cables might be a different story, though. I don't know what's the limit there...
```

---
## \#18 Posted by: Colson003 Posted at: 2018-01-18T23:29:03.040Z Reads: 71

```
What do you mean too much? Too many amps? 

https://youtu.be/93JBo87LJiU
```

---
## \#19 Posted by: Acklavidian Posted at: 2018-01-19T15:15:11.703Z Reads: 59

```
Too much anything
```

---
## \#20 Posted by: Acklavidian Posted at: 2018-01-19T15:49:44.907Z Reads: 59

```
Just don't want to over load it electrically.
```

---
## \#21 Posted by: Acklavidian Posted at: 2018-02-16T16:03:20.135Z Reads: 48

```
![IMG_20180215_224547|374x500](upload://n1Usb4Dru8qpG6L0Jhai29PkMKn.jpg)
Finally getting some parts.
```

---
## \#22 Posted by: Acklavidian Posted at: 2018-02-23T03:06:48.989Z Reads: 40

```
Mechanical stuff is all in. Time to start the intimidating part. ![IMG_20180222_210204|666x500](upload://8zK8arCw2hp2l0Un7uiAEkzUN0i.jpg)
```

---
## \#23 Posted by: Acklavidian Posted at: 2018-02-23T03:07:30.045Z Reads: 38

```
![IMG_20180222_210259|374x500](upload://m8avfmhTxSqVHV1VPPGsSjXi0xF.jpg)
```

---
