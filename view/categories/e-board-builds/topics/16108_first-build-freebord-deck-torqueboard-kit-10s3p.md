# First build &#124; Freebord deck &#124; Torqueboard kit &#124; 10s3p

### Replies: 17 Views: 1932

## \#1 Posted by: mt37 Posted at: 2017-01-14T23:07:38.080Z Reads: 152

```
Hi folks,

After lurking on these forums for a while I decided on my first build.

The base is a freebord that has been sitting unused for a while.

I got the mechanical kit for 1 motor here [1] and a 6374 190kv sensored here [2]

I've started putting together the kit (which sadly comes with no instructions whatsoever), and I'm already hitting some issues.

It looks like the tolerances between the belt and the motor mount are very small, and I'm worried about it catching.
The tolerance between the motor pinion and the wheel is pretty tight too.
Is it something I should be concerned about, and try to space the motor mount more from the pulley ?

<img src="/uploads/db1493/original/3X/3/5/35d31c0db7cfd843ef0555c60114cd0b008f77be.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/5/45a7ce18139cf9db28b5bce7d7d61107e231753f.JPG" width="375" height="500">

[1] diy-electric-skateboard-kits-parts/torqueboards-single-motor-mechanical-kit/
[2] https://electric-skateboard.market/product/190kv-sensored-motor-6354-6374/
```

---
## \#2 Posted by: mt37 Posted at: 2017-01-14T23:11:21.597Z Reads: 145

```
@torqueboards your help would be greatly appreciated :blush:
```

---
## \#3 Posted by: torqueboards Posted at: 2017-01-14T23:25:45.938Z Reads: 146

```
@mt37 - It should be setup like this.

<img src="/uploads/db1493/original/3X/8/c/8c6c859baa11bd0e8c10550d4ac5315ab5355b08.jpg" width="590" height="500">

The truck clamp should be to the center of the truck.
The motor pulley hub is facing outside.

Hope that helps. Let me know if it doesn't. Thanks for tagging me :)
```

---
## \#4 Posted by: mt37 Posted at: 2017-01-14T23:30:04.140Z Reads: 140

```
"the motor pulley hub is facing outside" - could you clarify what that means ?

Mine has the wide end resting against the wheel, is that correct ?

Also it seems while torquing the plate on the other end it kinda bent into the wheel, but I don't think that would be a problem.
```

---
## \#5 Posted by: mortorojo Posted at: 2017-01-14T23:30:44.189Z Reads: 143

```
I have a set of the torqueboards motor mounts, they work great but i had to really torque them down to the trucks to stop them from moving. I'd recommend flipping 3/8" bracket that tightens down to the trucks to the other side of the motor mount bracket. Doing that should allow you to flip the motor pulley around and allow it to sit further on the motor shaft. Here is a pic for reference from the  site.<img src="/uploads/db1493/original/3X/5/b/5b1d9fb57bc85e06853fd072a3be0351ea22887a.jpg" width="456" height="304">
```

---
## \#6 Posted by: Guacamoleface Posted at: 2017-01-14T23:35:40.200Z Reads: 140

```
Your plate that holds the motor should sit on the other side of the mount mounted on the truck as on the pictures above :)
```

---
## \#7 Posted by: mt37 Posted at: 2017-01-14T23:37:30.233Z Reads: 140

```
Thank you all for your help!

It's already looking much tidier. I'm sure I'll be back for more noob questions (:

<img src="/uploads/db1493/original/3X/3/a/3a29985c0f186ae0c44b2248572e75f8f9dbf501.JPG" width="375" height="500">
```

---
## \#8 Posted by: mt37 Posted at: 2017-03-06T20:00:22.591Z Reads: 104

```
**Update** 
<br/>
Finished putting the battery pack together, here is the full kit ready to be mounted (still need to fabricate a tray) 
 
<img src="/uploads/db1493/original/3X/4/9/49ef6e52835c87ccab89fc18242d6ac817911e00.JPG" width="666" height="500">

<br/>
I salvaged the 18650 out of laptops, they're mostly all good. The reds don't seem as good, but I built a 10s3p for ~$60 including a BMS, can't be too picky

<img src="/uploads/db1493/original/3X/6/2/628639debec934eaffa6ad9a361fc286f9d7cd8f.JPG" width="281" height="500">

<br/>
I made a spot welder using : a junk microwave oven transfomer, a 40 amp solid state relay, and a bit of arduino code 

<img src="/uploads/db1493/original/3X/0/5/05b7aabba1e665cd1f7ae4112264c3f1df57eb81.JPG" width="666" height="500">

<br/>
My early attempts at spot welding, before tuning the arduino code (a little aggressive)

<img src="/uploads/db1493/original/3X/e/e/ee8049969c1ad643a58c6398d395667024f8ac56.JPG" width="281" height="500">
```

---
## \#9 Posted by: Maxid Posted at: 2017-03-06T20:05:18.646Z Reads: 94

```
Laptop cells in a 3P configuration are a bad idea - this will not work.
```

---
## \#10 Posted by: mt37 Posted at: 2017-03-06T20:07:08.212Z Reads: 94

```
Why is that ?

Edit: I'm not afraid of trying this out and failing. It was cheap enough to warrant the experience.
If it's a fail, I'll buy name brand 18650.
```

---
## \#11 Posted by: Maxid Posted at: 2017-03-06T20:10:14.363Z Reads: 92

```
Discharge rate is too low and overheating issues. With a little bad luck they will "explode" while riding or charging.
```

---
## \#12 Posted by: mt37 Posted at: 2017-03-06T20:13:57.735Z Reads: 90

```
I thought 18650 were robust enough to rarely explode, no matter their provenance.

Can I play it safe with VESC settings ? Like limiting battery amps to 25A, regen to -12A
Charging is done via a BMS and I'll monitor the amps carefully on the input. I think that should help.

Eventually I want to ditch my chinese BMS and do charging / monitoring system as described here [1]

ps. there seem to be a number of people using laptop batteries throughout these forums, and youtube videos.

[1] http://www.electric-skateboard.builders/t/please-help-me-confirm-a-faulty-bms/18548/5
```

---
## \#13 Posted by: Maxid Posted at: 2017-03-06T20:23:11.069Z Reads: 88

```
You'd have to limit battery amps to maybe 5A per cell - that will be no fun ride. 
Sure a lot of people are using them - but in much larger parallel configurations like 6P and up. 

18650 don't explode like Lipos but they do vent - I would not want this happen to me at home or next to my expensive VESC.
```

---
## \#14 Posted by: mt37 Posted at: 2017-03-06T20:26:36.141Z Reads: 83

```
That's a good point, thank you for that. Can I find more info on the science behind why a 6p would be better than a 3p for my "unknown cells" ?

At this point I feel like I just need to plow through with what I have and have hope in my odds. I've already invested all my budget for this, and a fair amount of time.
```

---
## \#15 Posted by: Maxid Posted at: 2017-03-06T20:30:43.565Z Reads: 77

```
In parallel you basically add the discharge current of your individual cells to get your true pack output current (in your case maybe 3x5A=15A) similar to what you do with voltage when you do series connections.
```

---
## \#16 Posted by: mt37 Posted at: 2017-03-06T20:31:55.627Z Reads: 80

```
I meant some links, youtube videos etc. To further my education on the matter, and understand all the risks so I can make an educated decision.

Edit: or at least how could I measure over time the quality of cells from unknown provenance, and possibly increase the 15 amp threshold.
```

---
## \#17 Posted by: Mark Posted at: 2017-03-23T22:08:46.527Z Reads: 67

```
Does the deck have bite?
```

---
