# &ldquo;Mini Remote&rdquo; Thumb Drive

### Replies: 37 Views: 1659

## \#1 Posted by: jaatis Posted at: 2018-11-11T18:00:44.894Z Reads: 433

```
This mod let's you use the bulletproof internals of the legendary mini remote but in a thumb driven configuration. The mod only requires a few 3D printed parts and a few fasteners. Everything else can be taken from the donor remote.

**Disclaimers:**
- This mod has not been thoroughly tested yet. Use at your own risk.
- Depending on your 3D printer's capabilities the parts might or might not fit together properly.
- Soldering is required.
- This remote is **not** small. I advice to first print the parts and check if you are OK with the size.

That being said the parts I printed fit together perfectly and the remote feels ergonomic in my hand. Also it seems to work just fine with some initial testing. I have designed and printed over 10 prototypes and finally I'm happy to share the results.

![1|666x499](upload://qcn6Ei2SQgQwVPhVOfztuGcOkDt.jpeg) 
![20181111_141725|666x500](upload://nKE8Zi71127hPc6Hv93Z0sM8rUa.jpeg)
![4|667x500](upload://1AN00rLDwtZ0VAkosA8pLYe1JpW.jpeg) 
![20181111_141955|666x500](upload://qBTxHqOpWxEMUiexd6eiOWGesaw.jpeg)
![2|666x499](upload://aqEaFnZeTIQ2veOTNxRT43N7O7F.jpeg) 

******************************************************************************************************************

**Thingiverse link for the STLs:**

https://www.thingiverse.com/thing:3209308

Please notice that there are **two different versions of the "case_right"**.
The _case_right_insert.stl_ utilizes an **M3 brass insert** for the battery lid screw and the other one (_case_right_hexnut.stl_)  a **regular M3 nut**.

You can see the brass insert used in the instructions below. These inserts are very cheap and can be purchased e.g. from [here](https://www.banggood.com/100pcs-M34mm-H62-Brass-Knurl-Nuts-DIY-Accessories-p-971077.html?).

![image|690x207](upload://rYWx0svgEXzOSFFemFo4091nD7S.png) 

There are also three different options of the throttle wheel to choose from:

> throttle_wheel
> throttle_wheel_old_design
> throttle_wheel_large-tolerance

Try the “throttle_wheel” first.
If it doesn’t fit on top of the potentiometer then you can try the “throttle_wheel_large-tolerance”. This might be needed if you use a larger nozzle on your printer.
The “throttle_wheel_old_design” just has a different grip compared to the other two.

![image|690x255](upload://la8FtrrqlpSvdptS9o7iWaRuuiK.png) 


******************************************************************************************************************

**Instructions:**

You'll need a soldering iron, one 10-12 mm long M3 bolt and either an M3 brass insert or an M3 nut. Other parts can be printed and harvested from the mini remote.

Print all the parts and check that everything fits. The "case_right" needs to be printed with support for the battery lid cutout. Other parts don't need supports.

![11|690x467](upload://k12CMFy0Y1iLHZq5eJZIJZgNbfw.jpeg) 

This would be a good time to sand and paint the parts.

![20181110_165716|666x500](upload://nCP1FXmIWzhjPyzV1bzI45NW4yY.jpeg) 

Check which holes should be through holes. To ease the printing process I left a layer or two of material inside of some holes. You'll need to file them out but you should not have to enlarge the hole diameters. In total there should be six: Five in the "case_left" and one in the "case_right" for the battery lid screw. A few examples are highlighted in the picture below.

![image|690x345](upload://n1C02sbytjgfsPoqkVT3uUvIuNS.png) 

If you use a brass insert to hold the battery lid screw, you'll need to heat it up (with a lighter for example) and insert it to the case like in the picture below. Make sure that the M3 bolt goes all the way through the hole after this.

![20181110_171559|666x500](upload://PTUMUzKOgZldaAmO2XqUAaNvPV.jpeg) 

Next you'll need to remove the potentiometer assembly, PCB and battery contacts from the mini remote. At least the battery contacts need to be desoldered in order to be removed. I advise to desolder the potentiometer wires as well and solder them back facing the other direction. This helps mounting the potentiometer to the new case.

![20181111_133826|666x500](upload://aLGxUw5hDjqUyFnZB9bbQOJr6B2.jpeg) 

You also need to cut out the tab on the bottom battery contact (but only on this one!):

![20181111_134727|666x500](upload://mwMbcHUL6kOr8F15cdrwl2FJiUP.jpeg) 

Start mounting parts to the left case. I used a few drops of hot glue to mount the PCB and wires in place. Make sure the wires don't interfere with any moving parts and that the polarity on the batteries/contacts is correct!

![20181111_135847|666x500](upload://hbSHBHJNzB0nd1KBFD8m4j0lqB.jpeg) 

I used some grease on all joints and moving surfaces.

![20181111_140917|666x500](upload://zC52Aa9LQPk0gx0BZdIMvsKkBFP.jpeg) 

Using screws from the mini remote mount the two cases together. Check that the on/off switch moves as it should.

![20181111_141213|666x500](upload://3fIVm82xko6TJMFiFjB2YHBqAqg.jpeg) 

Insert batteries, attach a lanyard and put some adhesive foam on the inside of the battery lid to help with rattles.

![20181111_141456|666x500](upload://fkgkVCz2BY3b3OS76GzzDkLGCI6.jpeg) 

Lastly, don't forget to **re-calibrate the remote on the VESC tool**!!!

Enjoy :slight_smile: 

![20181111_141653|666x500](upload://9ZciR5gcxupRTGCbTP2wni567Kx.jpeg)
```

---
## \#2 Posted by: mccloed Posted at: 2018-11-11T21:00:48.151Z Reads: 314

```
Nice! What were your print setting on this?
```

---
## \#3 Posted by: jaatis Posted at: 2018-11-11T21:18:18.452Z Reads: 315

```
I have a 0.6 mm nozzle on my printer, layer height 0.28 mm, 3 perimeters and maybe 40-50% infill. It's quite crude. Filament is Extrudr red PETG, prints very well but bad for the camera :smiley:  220 degC did the job on the E3D Volcano.

When I have the time I will properly sand the parts and paint them.
```

---
## \#4 Posted by: mccloed Posted at: 2018-11-11T21:26:56.637Z Reads: 306

```
Cool. Thanks.
```

---
## \#5 Posted by: jaatis Posted at: 2018-12-07T19:13:38.308Z Reads: 266

```
There doesn't seem to be much interest in this but nevertheless I though to post some updates.

Most important one that I forgot to include in the original post:
The logic of the remote is inverted to what some of you might gotten used to, i.e. accelerate is "down" and brake is "up".
![logic|690x296](upload://zy5aXf5KoJmjrs5rMiLpTtH5NBZ.png) 

Thanks to the cold northern winter, I haven't been able to test this remote more than a couple of times so far. But the times that I did, it worked perfectly. However I did not like the grip of the throttle wheel. So I drew up a different design which I like much more:

![20181207_201706|666x500](upload://pUg5SmqSBfQJHFLIEECrXjp9e7V.jpeg) 

I printed this new wheel with a smaller nozzle and better resolution than the other parts. That's where I noticed a problem. I have designed the tolerances of the holes etc. so that they work with the parts that my big nozzle printer produces.

[s]This means that for small nozzle and high resolution prints many of the tolerances are too big! For example in this case, the throttle wheel had quite a bit of backlash on the potentiometer, which is not good.[/s]

[s]I will go through the design and upload a second set of STLs with smaller tolerances for those who use max. 0.4 mm nozzle (on an accurate FDM printer).[/s]

Edit: Fixed files have been uploaded.
```

---
## \#6 Posted by: myreala Posted at: 2018-12-07T20:02:33.933Z Reads: 226

```
This is good stuff man, I might do this mod as I have a mini which is super reliable but the trigger design is kind of a loose cannon.
```

---
## \#7 Posted by: mmaner Posted at: 2018-12-07T20:17:26.207Z Reads: 227

```
I'm really impressed with this project.  I remember reading this thread when you first posted it, I even made a bookmark so I could back and re-read it but totally forgot.  This is actually something I've been looking for for a long time.  I've even spent time making a model myself, just haven't had time to finish it.

Would you mind if I remixed your model a little?  It would save me a ton of time finishing mine up.
```

---
## \#8 Posted by: jaatis Posted at: 2018-12-07T20:24:38.723Z Reads: 215

```
Of course! I can send you the step files if you want.
```

---
## \#9 Posted by: mmaner Posted at: 2018-12-07T20:28:00.160Z Reads: 219

```
That would be great.  I want to make the top nose a little longer to include a finger slot and add some finger grips to the front.  Essentially the same shape as the benchwheel remote with finger grips like the nano-x.
```

---
## \#10 Posted by: jaatis Posted at: 2018-12-10T17:45:14.389Z Reads: 211

```
I have noticed a problem in the right side case which causes some minor alignment issues with the throttle wheel. I'm working on fixing it and will upload new files with correct tolerances to Thingiverse soon.
```

---
## \#11 Posted by: jaatis Posted at: 2018-12-12T20:04:30.650Z Reads: 212

```
The files have now been updated and uploaded to Thingiverse. If you downloaded and/or printed the files before today, I recommend to discard them and use the newest versions instead. Only the battery lid remained unchanged.

https://www.thingiverse.com/thing:3209308

There are now three different options of the throttle wheel to choose from:

> throttle_wheel
> throttle_wheel_old_design
> throttle_wheel_large-tolerance

Try the "throttle_wheel" first.
If it doesn't fit on top of the potentiometer then you can try the "throttle_wheel_large-tolerance". This might be needed if you use a larger nozzle on your printer.
The "throttle_wheel_old_design" just has a different grip compared to the other two.

You also need to choose one of the two options for right side case:

> case_right_insert
> case_right_hexnut

Make your decision based on which kind of a nut you want to use for the battery lid screw, a brass insert or a regular nut. The hexnut version has now been tested as well and works nicely:

![20181212_201223|666x500](upload://3Uwo2V1DhdBXny2svBKKfbOTiyH.jpeg) 

I recommend either gluing or melting the nut to place just to be sure.
```

---
## \#12 Posted by: J0ker3366 Posted at: 2018-12-12T20:19:30.402Z Reads: 191

```
&lrm; Following
```

---
## \#13 Posted by: peter97silva Posted at: 2018-12-26T16:02:45.523Z Reads: 180

```
This is great! Awesome job, I'm going to print this soon, maybe next week, I was full of the mini remote being to big on the pocket and the thumb drive looks much better too! Thanks so much!
```

---
## \#14 Posted by: jaatis Posted at: 2018-12-26T18:29:23.005Z Reads: 181

```
I hope you try the mod and like it, but I have to warn you that this is only marginally smaller than the original remote.

If you really are after a smaller alternative, I'd suggest to try @nuttyjeff's Avio remote. It's still a trigger style remote though.
```

---
## \#15 Posted by: Allofyoush Posted at: 2019-01-14T01:18:06.889Z Reads: 162

```
Do you want to upload your version?
```

---
## \#16 Posted by: mmaner Posted at: 2019-01-14T01:25:21.329Z Reads: 165

```
Haven't had time to do anything yet.
```

---
## \#17 Posted by: Allofyoush Posted at: 2019-01-14T01:34:13.049Z Reads: 168

```
Gotcha. The mini remote seems to be the best deal, so turning it into an even better deal would be awesome
```

---
## \#18 Posted by: Niak Posted at: 2019-03-30T05:12:37.826Z Reads: 139

```
Great design, nice job. i would like to make a version that takes a lipo. Is it possible to send me the step files?
```

---
## \#19 Posted by: jaatis Posted at: 2019-03-30T15:11:42.874Z Reads: 138

```
Sure, shoot me a pm.
```

---
## \#20 Posted by: Niak Posted at: 2019-03-30T15:50:46.047Z Reads: 134

```
Hey man,

I’ve just finished one for trigger style.

I also want to check what you ended up with the trigger assembly.![image|509x500](upload://bz77xIdbjViwEtuVqAKcss2fNfF.jpeg)
```

---
## \#21 Posted by: SanderG Posted at: 2019-05-16T17:03:07.371Z Reads: 111

```
Hey looks good! is there a way to reverse the remote? up is throttle and down is brake? Also can you share the  cad file? I wanna make some changes (adding a 18650 cell)
```

---
## \#22 Posted by: pat.speed Posted at: 2019-05-16T21:42:03.888Z Reads: 102

```
You can’t reverse throttle with a switch like you can with gt2b. You however might be able to modify the hardware to make this happen
```

---
## \#23 Posted by: SanderG Posted at: 2019-05-16T21:42:52.831Z Reads: 99

```
Yea thats why i wanna get the cad assembly file :)
```

---
## \#24 Posted by: Marksmoura Posted at: 2019-05-16T22:31:08.855Z Reads: 101

```
Great project! Thumbs up man, great job.
This is exactly what I am looking for. 

I would make some changesfor example  I would like to have a small prismatic lithium battery instead of AA batteries.

About the inverted acceleration we can just rewire the potentiometer and the problem should be solved. Did you try this? Just inverting the + and - on the potentiometer should solve this issue. 


Would you by any change share the original CAD files? It would be great! And again nice job man.
```

---
## \#25 Posted by: jaatis Posted at: 2019-05-17T05:33:21.024Z Reads: 96

```
Yep I realized the potentiometer wire trick later but in the end kept this "inverted" function since actually I learned to prefer it.

I'm currently working on a smaller variant using a lipo battery but I've been busy doing other things so it's not even close to ready yet. The current form factor is holding back the design quite a bit.

I can share the step files and will do later once I have the access and the time. I'd love the idea that other people would help optimize this design and get more options for everyone!
```

---
## \#26 Posted by: TinnieSinker Posted at: 2019-05-17T07:34:23.241Z Reads: 88

```
this remote looks great! simple yet effective. cant wait to see the extra versions people are working on.

Im wondering can the unused steering channel can be used as an aux channel with a momentary switch?
```

---
## \#27 Posted by: Ariehh Posted at: 2019-05-17T08:59:54.064Z Reads: 90

```
I have a simple arduino code that when you turn that wheel left it turns a ledstrip on or off, if ou turn right you toggle between always on, 50% brightness and blinking. I haven't put it on my board yet because I need to find sturdy led lights first.
```

---
## \#28 Posted by: TinnieSinker Posted at: 2019-05-18T07:17:50.939Z Reads: 81

```
thats pretty cool! good to know the channel works as normal, I dont know much about potentiometers but if i can replace that with a switch it'll be just fine
```

---
## \#29 Posted by: Ariehh Posted at: 2019-05-18T07:32:41.691Z Reads: 81

```
Pots are quite easy. They all have a range between 0 and lets say 2000. So neutral position for the wheel is ~1000. In your arduino code you could make it so that when the value goes below 500 by turning left it triggers an action just like a button would do. Same goes for turning right and the value gettjng bigger than 1500. The deadspot in the middle would be ideal because of incidentally touching the wheel.
```

---
## \#30 Posted by: pat.speed Posted at: 2019-05-18T09:43:09.102Z Reads: 78

```
Problem is Arduino a don’t measure resistance, they work on voltage. So you would need to program in less than 2v does this and more than 4v does this etc.

Or that’s at least how I remember it working
```

---
## \#31 Posted by: Ariehh Posted at: 2019-05-18T10:56:28.787Z Reads: 72

```
I printed the value in the serial monitor and I got values between 0 and 2000
```

---
## \#32 Posted by: jaatis Posted at: 2019-05-18T15:15:42.190Z Reads: 74

```
The CAD files are now on [Thingiverse](https://www.thingiverse.com/thing:3209308) in step format (only the printable parts).\
@Marksmoura  @SanderG
```

---
## \#33 Posted by: SanderG Posted at: 2019-05-18T22:21:05.509Z Reads: 74

```
Thanks man! Do you maybe have the file for the potentiometer assembly? I wanna re design it a bit and would help to have that part lol :p If possible would help me allot!
```

---
## \#34 Posted by: Shadowfax Posted at: 2019-05-18T22:59:07.082Z Reads: 73

```
Thought I might add my little mini remote dirty hack here. 

When I got mine, I didn't have any AA's and didn't like the idea of it not being rechargable anyways. So on a whim I cut out the battery sled and litterally soldered in a 18350 cell I had laying around, then I added a micro USB charge board a found in a pile of old crap and it worked. The controller seems to have no issue running at 4.2v and I'm assuming it would run down to the batteries cut off, though I've never let it go that far. 

So yeah, for those that just want it easy to charge and last for freaking ever, it's not pretty, but it'll all hidden and it works!!
```

---
## \#35 Posted by: Wilsonliang777 Posted at: 2019-05-20T18:16:56.160Z Reads: 69

```
I want to convert my mini remote to this one but don't have access to a 3d printer.  Can anyone help me print a copy.   I will pay.   Ty
```

---
## \#36 Posted by: Z408 Posted at: 2019-09-05T02:51:06.921Z Reads: 45

```
Printing one this week.  If I am successful, I can print you one.
```

---
## \#37 Posted by: Wilsonliang777 Posted at: 2019-09-05T06:35:31.779Z Reads: 39

```
Thank you for the offer.  I ended up buying a cheap 3d printer and was able to print one.  But I ended up not using it becasue it was too thick.
```

---
