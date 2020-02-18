# Lipo Series Question

### Replies: 12 Views: 831

## \#1 Posted by: themegak Posted at: 2017-11-22T23:15:21.846Z Reads: 82

```
I have four 3s 5,000 mah Batteries.  I want to make a 10s Battery pack out of them.  I have already disassembled one of the lipos and separated one cell so I now have, three 3S Lipos and one 1S lipo all at 5000mahs.  My question is, do you think there is anything wrong with a config like this ?  Below is a crude diagram of what i am thinking of doing.  I will be adding a 10s BMS as well but I am curious if there are any issues with doing this.  I don't think there are, but I'd be interested in knowing your thoughts.

 <img src="/uploads/db1493/original/3X/8/3/83b30fb1178909f584e920b704e936ff9c0d6f5c.JPG" width="690" height="492">
```

---
## \#2 Posted by: wafflejock Posted at: 2017-11-22T23:24:02.881Z Reads: 78

```
Since they are the same capacity it's no different than having a 10S battery really aside from the extra resistance from the connections and wires between the cells.  Basically should work fine, main issue is just mixing different capacity cells or having ones with higher internal resistance in the set of cells in series (increasing the entire circuit resistance, effectively bringing down the max discharge rate and putting more stress on the one cell compared to the rest).  If all the cells are roughly the same capacity and IR though I don't see how this would be a problem really.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-11-22T23:44:13.962Z Reads: 74

```
As @wafflejock stated, No problem as long as all cells are the same brand, capacity and C rating.
Also, you could reduce the resistance by soldering the battery packs together in series instead of using connectors.
This will also make a less bulky wiring job.

<img src="/uploads/db1493/original/3X/a/0/a0f29cf98e6333ae09bf7f660d0bc35c20796ffd.png" width="329" height="500">
<img src="/uploads/db1493/original/3X/1/3/132ab44b4d9e7f4af27a659982ee06a4775019da.png" width="376" height="500">
```

---
## \#4 Posted by: themegak Posted at: 2017-11-22T23:50:19.222Z Reads: 62

```
Thanks but, my setup will be a little different from yours as one of my packs is 1cell from a 3s battery.  That is the thing I am unsure of even though it technically shouldn't be an issue.  What do you think about that?
```

---
## \#5 Posted by: Namasaki Posted at: 2017-11-23T00:30:11.199Z Reads: 60

```
I think it will not be an issue as long as it's from the same brand, capacity and C rating as the other packs.
```

---
## \#6 Posted by: themegak Posted at: 2017-11-23T02:40:58.226Z Reads: 52

```
Thanks  @wafflejock and @Namasaki  ..  Appreciate you thoughts..
```

---
## \#7 Posted by: Wilsonliang777 Posted at: 2017-11-23T19:13:54.454Z Reads: 49

```
I am doing the samething.  I have 3x 3s 7000mah lipo packs and a 1s 7000mah.   I noticed when I disassembled the lipo there is a circuit board in the 3s lipo pack.  What's that board for?    Does all lipo comes when bms built in?  The first time I ran the 10s battery I noticed the 1s had a higher voltage left over(1s 3.80v.  All other cells had like 3.67v.   I charged the pack up again and ran it for 20 min and the 1s has 4.08v and all other cells has around 4.12v.
```

---
## \#8 Posted by: themegak Posted at: 2017-11-23T22:14:15.475Z Reads: 42

```
Interesting, can u post a pick of the circuit board ? Also, did the single cell come out of an identical 3s 7000mah battery?
```

---
## \#9 Posted by: wafflejock Posted at: 2017-11-24T00:24:10.326Z Reads: 37

```
Haven't seen this on bigger packs but on some of the 1S lipos for micro quadcopters they have a built in low voltage cut off so you don't accidentally over drain the cells I'd guess it's the same thing, could also be charge circuitry but my guess would be low voltage cut off maybe cell level fusing of some sort.  If you take a pic sure someone will be able to tell you.  Also could post a link or the exact battery make/model and could see if it's in a manual or listing anywhere.
```

---
## \#10 Posted by: Wilsonliang777 Posted at: 2017-11-24T00:34:44.070Z Reads: 36

```
Yes. All the cells were from the same kind of batteries and purchased at the same times.  Actually the 3s were 6s 3500mah connected to make 3s 7000mah.   Right now I don't have a Bms so I am charging the batteries individually.   So I know they were somewhat balanced when I put it together.    I am thinking regenerate charging might be putting more voltage into the 1s  because it does not have a curicit board.  That might account for the extra voltage on the  first run.  My second run I did not break  at all there for no regenerative charge <img src="/uploads/db1493/original/3X/2/4/24f025eb91eeb2ca1c8db723eb8a04b573439167.jpg" width="375" height="500">
```

---
## \#11 Posted by: wafflejock Posted at: 2017-11-24T00:53:21.082Z Reads: 33

```
Just did some searching around and yeah appears it is just a BMS basically and does regulate both charge and discharge current http://www.batteryspace.com/protection-circuit-module-pcb-for-7-4v-li-ion-battery-pack-18a-limit.aspx  Your suspicion sounds pretty on point with this limiting the power going into those cells and therefore more regen going into the one without any such circuit.  Sure you could remove it but working with the lipo cells is always a nerve racking and tedious process.  Personally using 5S 5Ah batteries in hindsight think 3 4S or 4 3S or maybe even the 5 2S could be a better option.

I ended up making these trays for the LiPos so I can take them out to charge and figured I can buy more in the future and swap out the trays if I want more range keep a few in a backpack ready to go:

[Album](https://photos.app.goo.gl/KzDYcYYeHPuD4u5e2)

With something like that could have had more slots and just made it a little easier to push them out from the side they plug into but the concept could work for more batteries is the point.
```

---
## \#12 Posted by: Wilsonliang777 Posted at: 2017-11-24T03:15:21.108Z Reads: 28

```
I am not going to take all the lipo apart.   Once I am sure all the lipo is compatible I will install an bms and I hope the bms will  regurlate the charge and discharge.  Therefore will help the 1s stay balance when the other cells.
```

---
