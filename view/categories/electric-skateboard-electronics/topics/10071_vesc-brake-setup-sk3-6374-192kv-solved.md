# VESC brake setup / SK3 6374 192kv \[Solved\]

### Replies: 10 Views: 1158

## \#1 Posted by: Ferret99 Posted at: 2016-09-24T08:17:03.232Z Reads: 208

```
Someone know why the brake work only in low rpm ?<img src="/uploads/db1493/original/3X/3/4/3420403fcdde2fa2e90aee143a934647aa83f03f.jpg" width="690" height="371">
[https://youtu.be/Fcznk53Jte4](https://youtu.be/Fcznk53Jte4)
```

---
## \#2 Posted by: El_Cid Posted at: 2016-09-24T08:59:54.687Z Reads: 192

```
Try changing your batt min (regen) to -12.00 I read somewhere that thats the high rpm break. The low rpm one is the motor min (regen). Reason for the -12A was that its the max a raptor space cell can charge at. Was thinking maybe having it as high as you do may be causing your issue. Just bench test it first though dont want u getting hurt...
```

---
## \#3 Posted by: El_Cid Posted at: 2016-09-24T09:09:57.905Z Reads: 188

```
Also your max input voltage is set to 42v which if you're using a 10S batt is cutting it close to a full charge and if breaking with a full charge and dumping 80A into the battery it may be causing the vesc to "over voltage" I think thats also what the LED flashing like that means. Plug it all in to BLDC run the real time data tab and look at the fault code when you do your break bench test like on the video and see what the fault code is.
```

---
## \#4 Posted by: El_Cid Posted at: 2016-09-24T09:17:18.345Z Reads: 184

```
I wonder if with the battery being full if its the caps that are topping up and since they can hold 63v or so the vesc may see higher than 42v.. So maybe try 44.4v? I mean the vesc can handle 12s... So that should still be safe for the vesc.
```

---
## \#5 Posted by: Ferret99 Posted at: 2016-09-24T09:48:36.938Z Reads: 172

```
Thank you! I changed the max input voltage to 44.4v and now the brake work
I am using my e bike battery (36v) but I am going to use 8s lipo
```

---
## \#6 Posted by: flatsp0t Posted at: 2016-09-24T10:47:07.649Z Reads: 168

```
Just leave the min and max batt voltage on their default values, they are just there to protect the componets from more than they can handle.
```

---
## \#7 Posted by: Ferret99 Posted at: 2016-09-24T11:09:34.096Z Reads: 162

```
the vesc can handle up to 12s but I am going to use 8s so it will be fine
```

---
## \#8 Posted by: flatsp0t Posted at: 2016-09-24T11:47:25.267Z Reads: 156

```
you can do whatever you want, i just wanted to tell you what vedder and all the vesc vendors say about these values.
```

---
## \#9 Posted by: El_Cid Posted at: 2016-09-24T15:37:58.295Z Reads: 137

```
Max batt should be set according to how much your battery can discharge at or less if you'd like less torky acceleration. And battery discharge could also depend on the cutoff settings of your bms. For example some pf the original raptor batteries came.with a bms that would trip at 30A draw so if on a single vesc you would set your max batt to 30a if on a dual it should be set to15a each vesc. The newer raptor battery has a 60A max bms and so on a dual vesc it can be set to 30a each. Even just that is far from leaving an pff the shelf vesc default. So depending on the discharge rate of your lipos. Thats how you can figure out your batt max. Same goes for batt min regen. It dictates how much amperage the vesc will allow back into the battery which if its set higher than the battery can handle recharge wise you could over charge and blow a battery or bms or even fuse if there is one.

Defaults do not work for every setup...
```

---
## \#10 Posted by: elkick Posted at: 2016-09-24T15:47:15.973Z Reads: 134

```
@flatsp0t was talking about something else (min./max. voltage values the VESC can handle), but never mind. 

Since Jacob Bloy still have that false claim for max. voltage in his tutorial videos for setting up VESCs in BLDC tool he might help those who are facing problems with this settings in the future. But I doubt it.
```

---
