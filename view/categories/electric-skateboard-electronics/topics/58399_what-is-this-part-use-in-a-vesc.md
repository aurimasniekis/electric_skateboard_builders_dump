# What is this part use in a VESC?

### Replies: 9 Views: 302

## \#1 Posted by: Tomer Posted at: 2018-06-10T07:43:54.100Z Reads: 83

```
Does any one know what it's doing?

![image_01|374x500](upload://lUpzYNthi7VCTKdoqcwcFj5Z3cJ.png)

How bad is it if a half of the cover of it is broken?
```

---
## \#2 Posted by: pat.speed Posted at: 2018-06-10T07:54:54.149Z Reads: 79

```
What part is broken? The plastic or the wire
```

---
## \#3 Posted by: CHAINMAILLEKID Posted at: 2018-06-10T08:22:45.016Z Reads: 68

```
I think its an inductor coil, and the material is part of the ferrite core.

They're usually part of power management as I'm familiar with them, but I'm not sure what it'd be doing here.

I've had things with chipped ferrite cores before w/o any issues. I think its fine so long as the windings are still all covered.
```

---
## \#4 Posted by: LittleSheepz Posted at: 2018-06-10T08:48:06.836Z Reads: 61

```
> Blockquot

[quote="Tomer, post:1, topic:58399"]
Does any one know what it’s doing?

[![image_01|374x500](//www.electric-skateboard.builders/uploads/db1493/optimized/3X/9/9/998e2319a45cec54d6b2053ded0a1ecc8ed5eb69_1_374x500.png)
image_01.png1574x2100 524 KB
](//www.electric-skateboard.builders/uploads/db1493/original/3X/9/9/998e2319a45cec54d6b2053ded0a1ecc8ed5eb69.jpg)

How bad is it if a half of the cover of it is broken?
[/quote]


That is a 22uH Inductor. I cant really see the broken part though. As long as the golden wire coiled around the  housing (the center part) is still intact, it should not affect much.

From the VESC Schematics, its connected to the DRV chip pin 50,51 and pin 52 in series with 100n capacitor.   The other end is connected to the 5v rail. So im guessing it's used for power filtering of some sorts.

Link for the inductor:
https://www.mouser.sg/ProductDetail/Bourns/SDR0805-220ML?qs=y9m3SKnhpLMnaY53wPhSdA%3D%3D


Cheers mate!
```

---
## \#5 Posted by: Tomer Posted at: 2018-06-10T08:48:38.288Z Reads: 60

```
[quote="pat.speed, post:2, topic:58399, full:true"]
What part is broken? The plastic or the wire
[/quote]

The plastic part is broken.

![image_01%20(1)|375x500](upload://ji83hPlt29QHJtWuln5FyX8cbdA.jpg)

I opened a FOCBOX that I bought for the first time because I read many FOCBOX's thermal pads are not aligned(I didn't even powered it yet), and I saw that this part is broken.

[quote="CHAINMAILLEKID, post:3, topic:58399, full:true"]
I think its an inductor coil, and the material is part of the ferrite core.

They're usually part of power management as I'm familiar with them, but I'm not sure what it'd be doing here.

I've had things with chipped ferrite cores before w/o any issues. I think its fine so long as the windings are still all covered.
[/quote]
Thanks.
The plastic is 1/4 broken. :disappointed_relieved:
```

---
## \#6 Posted by: LittleSheepz Posted at: 2018-06-10T08:50:27.363Z Reads: 57

```
[quote="Tomer, post:5, topic:58399"]
The plastic part is broken.

[![image_01%20(1)|375x500](//www.electric-skateboard.builders/uploads/db1493/optimized/3X/8/7/8735f40e98c93202651db5ce4bce863afc6fe036_1_375x500.jpg)
image_01 (1).jpg1815x2420 1020 KB
](//www.electric-skateboard.builders/uploads/db1493/original/3X/8/7/8735f40e98c93202651db5ce4bce863afc6fe036.jpg)

I opened a FOCBOX that I bought for the first time because I read many FOCBOX’s thermal pads are not aligned,
(I didn’t even powered it yet) and I saw that this part is broken.

![|20x20](//www.electric-skateboard.builders/user_avatar/www.electric-skateboard.builders/chainmaillekid/40/57919_1.png) CHAINMAILLEKID:

> I think its an inductor coil, and the material is part of the ferrite core.
>
>
>
> They’re usually part of power management as I’m familiar with them, but I’m not sure what it’d be doing here.
>
>
>
> I’ve had things with chipped ferrite cores before w/o any issues. I think its fine so long as the windings are still all covered.

Thanks.
The plastic is 1/4 broken. :disappointed_relieved:
[/quote]

Looks like the housing have broken off. It wouldn't really concern me. The windinds are still intact.
```

---
## \#7 Posted by: Tomer Posted at: 2018-06-10T09:08:35.681Z Reads: 49

```
Thanks for the informative answer! I'll plug it to power today and will test it.
```

---
## \#8 Posted by: CHAINMAILLEKID Posted at: 2018-06-10T09:12:34.912Z Reads: 46

```
I would still expect it to work, but behavior might not be consistent.

Should be easy to replace.
https://www.ebay.com/itm/CHOKE-SMD-220UH-Part-WURTH-ELEKTRONIK-744774222/352000302051
```

---
## \#9 Posted by: pat.speed Posted at: 2018-06-10T09:29:13.519Z Reads: 37

```
I’d just plug it into a low power 12v supply and see how it goes, maybe try and run a motor detection too
```

---
