# I&rsquo;m NEWBIE! First time building e-mtb. Tips &amp; Tricks are welcome

### Replies: 11 Views: 851

## \#1 Posted by: Ghrom Posted at: 2017-11-05T02:44:37.386Z Reads: 158

```
Hi everybody!

I reach here while looking for some info on how to build my own electric All Terrain Skate. Never heard about mountainboards before. In the beggining I tought I was the first one with this crazy idea, but seems it's been spining around for long time and there are lot of ppl enjoying them. So glad to be able to share the hobby :)

I have read a ton, but I'm still pretty newbie and there is too much info to consider, so any help or advice will be much appreciated.

The only thing I'm sure about is going for a Trampaboard 35ºLong 17ply.
Why this trampa deck? Cuz I'm BIG (1'96m / 100Kg) and think it will be the more confortable for me. 

When it comes to the electric stuff, I'm still completely lose:
	- Motor: I'm thinking on 2 x Turnigy SK3 149KV. I'm assuming less KVs means more Torque and I prefer power to climb easier rather than reaching top speeds. 
It's ok or am I getting wrong?  
	- Battery: After spending a few weeks reading, I think Li-ion is my way to go. They last longer than LiPo, are more safety and I'm taking this point as an inversion.  But still thousands doubts come to my head:
                First thing, does it worth it? Li-ion are much more expensive. I can try to build the battery for my own but still there is a huge price difference.
                If I skip the costs, there are still lots of enigms: 
		If one single cell performs 3,6v - 3000mAh - 15A (I'm thinking on a Samsung INR18650-30Q)...
		Then if I build a 12S4P battery, I'll get 36V - 12000mAh - 60A.
		Will that 12S4P battery be enough to power both motors? For how long? Any BSM recommendations? If that's not enough, and I'm going to need 2 x 12S4P, perhaps LiPo is the right choice. Are there any known formula to calculate this?
	- VESC: I know it's a very important part, but I didn't have time to take a look into this yet :( Thought It's better to have it clear about batterys first.
        - Motor mount: Seems like some ppl here are selling artisan stuff (@Idea), I will take into this later on. 
        - Motor pulley / Belt: 14t pulley and 15mm belt are enough? Or should I go for something stronger due to my size (13t and 20mm for example)?

What do you think?
I know there is too much on the air right now, but as said before any help and/or advice will be much appreciated.

Thanks in advance!
Ghrom
```

---
## \#2 Posted by: mmaner Posted at: 2017-11-05T02:48:16.963Z Reads: 147

```
Take a look at the MBS Comp 95, pretty beefy board and the bindings are a lot more comfortable.
```

---
## \#3 Posted by: Ghrom Posted at: 2017-11-05T10:56:50.327Z Reads: 129

```
Tnx for the info @mmaner. 
I will try to find where to test it, but seems it can satisfy my needs  

Any comment about the electronic parts?
```

---
## \#4 Posted by: mmaner Posted at: 2017-11-05T13:25:34.748Z Reads: 118

```
I personally use 10s, as 12s can be deadly to the VESC.  I just don't like running against the ERPM barrier.  Plenty of people use 12s but 10s leaves more room for experimentation.   Lipos will give you more amp delivery than most liion packs and are cheaper, but support less charge cycles. 

Talk to @korryh about MBS mounts, solid and not too expensive. If you want VESC's I would suggest FocBoxes right at the beginning and save some.mkney blowing up less robust controllers.
```

---
## \#5 Posted by: benjammin Posted at: 2017-11-06T06:20:32.645Z Reads: 91

```
Comp 95 is a solid choice. 

<img src="/uploads/db1493/original/3X/c/2/c287694097ada2394d7ba84c017c1f66d11393be.JPG" width="666" height="500">

Also, If you go Comp 95, make sure to get the new model w/Matrix2 trucks. Springs look cool and all, but imo there's really no comparison in performance. Max6 w/8s works great if you're not looking for a lot of top end (25-26mph or so, depending on how much torque you need). Beltdrive is from E-Toxx (contact Nowind). He also has a directdrive made for these that's supposed to be the shit.
```

---
## \#6 Posted by: Ghrom Posted at: 2017-11-17T11:26:12.983Z Reads: 63

```
Taking your advices in mind and after testing it, I have purchased an used MBS Comp 95x.
Seems its been used very few times. I'm attaching some pics ^^
<img src="/uploads/db1493/original/3X/7/c/7cd1098a71e3113e300603fbaeb9719ef62faf73.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/9/398b6666ba013464bfc2bbe8b2d0ae66e5e75fa2.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/0/60ce162fec2483450dfbb4ff7c2de317d4d44002.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/3/13d283bfe8fd726b544a9d0806c39ecdb796449f.JPG" width="666" height="500">

All for less than 200€. Hope I get a good deal. 
Trucks aren't the recommended ones, but could be a good start point for a newbie. What do you think?

I have also ordered 2x Turnigy SK3 149kv motors from hobbyking.
That's all I'm sure for now xD

I'm still looking for some more info about the other components. Didn't realize how deep is this world till now. So much info to process and learn about.

Thanks @mmaner and @benjammin for your comments and help!

I'll keep you guys up to date.

As always, any comments are welcome
:slight_smile:
```

---
## \#7 Posted by: mmaner Posted at: 2017-11-17T12:57:33.104Z Reads: 55

```
That's a good deal, good looking board. Talk to @korryh, he might have or can make some motor mounts for you.
```

---
## \#8 Posted by: benjammin Posted at: 2017-11-17T16:13:09.111Z Reads: 54

```
Nice, yeah good deal! Just saw the same board someone posted on YouTube (think your bindings are better). Actually like the look of this one over mine.

https://m.youtube.com/watch?v=iLUzqO6Xrw4
```

---
## \#9 Posted by: DilatedPupils Posted at: 2017-11-17T19:33:20.793Z Reads: 55

```
If you're going to go with Li-ions you would want at least 5p. I just recently switched from lipo to li ion on my Trampa. And at 12s5p I feel like the lipos are still better. The charging is just more convenient.
I running 149kv, 12s , 12 tooth motor gear, 60 spur and  to speed is about 23mph and 8mile range on 8000mah lipo with a few hill climbs. Haven't tested the range of my li ion, but should be double that.
Good luck with your build. I'm also looking for motor mounts for those trucks for my second emtb.
```

---
## \#10 Posted by: Ghrom Posted at: 2017-11-17T22:28:57.523Z Reads: 54

```
Hi @DilatedPupils 

I've heard the same from different ppl about Li-ions vs Lipos. 
Thoug I will go for Lipos at the beggining, and if I see I'm using the mountainboard as much as I pretend to, build a second one with better components.

Lot of questions come to my head:
- What specs had your previuos Lipo? 8miles with just 8Ah sounds pretty good to me.
- Also, are you going with single motor or 2 motors? Model?
- Why did you decide 12s5p on your Li-ion battery? 
- Did you try 10s6p instead 12s5p?
- Which cells are you using?

As @mmaner said, talk to @korryh. I've contact him last week and he aswer me really fast :)
I'm waiting to see if I can get other motor mounts from Spain (where I live) but if it's not possible I will definetly ask @korryh for them.

Thanks for sharing!
Regards!
```

---
## \#11 Posted by: DilatedPupils Posted at: 2017-11-18T02:38:43.032Z Reads: 52

```
3x 4s turnigy 8000mah 25c lipos. I got them on sale, would recommend getting 2x 6s instead for more convenient charging. 
IMO if you're thinking about switching you li ions later, you should just go with them from the beginning. 

Sk3 6374 149kv. Sk3s are awesome.  Even more with sensors. And for offroading, dual is the only way to go. I started with single, and I could only ride it on pavement.

I went with 12s because 149kv at 10s won't be enough. More power is what you want specially on an emtb.  I'm using 30Q without bms. I made 2x 6s packs so I could balance charge them on my hobby charger every once in awhile.
```

---
