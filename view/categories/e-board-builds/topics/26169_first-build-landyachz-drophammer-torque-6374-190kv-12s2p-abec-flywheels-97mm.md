# First build &#124; Landyachz Drophammer &#124; Torque 6374 190Kv &#124; 12s2p &#124; Abec flywheels 97mm

### Replies: 66 Views: 5679

## \#1 Posted by: tvidotto Posted at: 2017-06-25T23:36:23.535Z Reads: 539

```
Hey everyone!

I am new posting here but I have been lurking the forum for months trying to learn the most I can. I think I will never feel comfortable enough till I actually build one.

I used to ride skates 15 years ago but them moved to a bigger city for the university and never rode again. One year ago I moved to the US to work on a game company called Valve and decided to start riding again. The streets and sidewalks here are great for those small wheels so I think it is time to go a little further

Going to the build, here is a list

* Landyachtz deck, it is a drop through deck and I am not sure if will be any problem for the new trucks
* caliber truck II 50º
* abec wheels 97mm
* motor mount from Enertion (got on another site because apparently enertion is not doing Diy stuff anymore)
* nano remote 2.4ghz
* ESC VESC from Diyelectricskateboards.com 
* 12s2p battery pack from Diyelectricskateboards.com (with bms )
* motor 6374 190kv 3150W from Diyelectricskateboards.com
* 36T pulley
* 16T pinnion for the motor
* belt 255mm 12mmw wide also from Diyelectricskateboards.com

<img src="/uploads/db1493/original/3X/d/5/d5cc6de3f25b091fc2631e05b1b77952e3f318ca.png" width="690" height="392">

I read in multiple places that a battery not well wired can get fire, so I decided to go safe and get one already assembled  from Diyelectricskateboards.com, I always see really good feedback about them so I tough it was the best choice

I weight 205 pounds and the area that I live is mostly flat, but I would like to try some hills in Seattle, our neighbor city

I was calculating the speed with that RC app, and something feels wrong. I am using:
* internal gear ratio as 1
* pinion = 16
* spur = 36
* battery voltage as 44.4
* motor KV = 190
* Tire diameter = 97

And the output is 69km/h (43 mph)

This looks wrong but I don't know how much the air drag and my weight contribute to slowing it down.

Is there anything wrong with this build?
Am I missing something?
```

---
## \#2 Posted by: Decdog Posted at: 2017-06-25T23:54:30.953Z Reads: 474

```
according to [this](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":12,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":97}|), your unweighted top speed would be around 41 mph
```

---
## \#3 Posted by: wafflejock Posted at: 2017-06-26T00:06:18.823Z Reads: 477

```
[quote="tvidotto, post:1, topic:26169"]
to work on a game company called Valve
[/quote]

Humblebrag :slight_smile: can I get a VR thing called Vive

Think the pinion teeth if you go with 13 is going to give you more torque less top end and given the 190kv motor and your size (not being a wirey short type like me) that might be better for the hills out there.  With 13 tooth pinion on the motor shaft the calc says top end is 27mph weighted.  Think just the combo of high kv, pinion ratio, and tire diameter adds up to lots of speed but then probably not as much torque for acceleration or hill climbing.
```

---
## \#4 Posted by: tvidotto Posted at: 2017-06-26T00:43:01.811Z Reads: 461

```
[quote="Decdog, post:2, topic:26169, full:true"]
according to this, your unweighted top speed would be around 41 mph
[/quote]


great, this weighted value looks more realistic but I could not find on the site what is the math behind being weighted.
According to another post, the weighted value is pretty accurate, but still feels it is too much compared to other boards I see here with better electronics and less top speed 

<img src="/uploads/db1493/original/3X/3/7/37fc66a139e3432b32097080e7ecf14edca99dd6.png" width="314" height="200">

Maybe I should reduce the efficiency percentage
```

---
## \#5 Posted by: tvidotto Posted at: 2017-06-26T00:51:37.436Z Reads: 432

```
[quote="wafflejock, post:3, topic:26169"]
Humblebrag :slight_smile: can I get a VR thing called Vive
[/quote]

you can get free demos if you come by =], I gave a demo two days ago to a friend youtuber.

[quote="wafflejock, post:3, topic:26169"]
Think the pinion teeth if you go with 13 is going to give you more torque less top end and given the 190kv motor and your size
[/quote]

It makes sense to go more torque and less final speed since I will never want to reach it, but is the 13T ok in case it has too much torque? I heard that since it has fewer teeth in contact with the belt, it can lead to excessive stress and damage both. I was wondering if I could 3dprint a 40T for the wheels, but I don't know if the belt will be long enough, it may need to be a new one

Anyways, I am still learning so feel free to point any error
```

---
## \#6 Posted by: wafflejock Posted at: 2017-06-26T01:05:09.939Z Reads: 406

```
If I ever make it back out there I'll take you up on the demo :slight_smile:

Looks like you should be fine on adjusting the number of teeth up or down by a few since the motor mount has some wiggle room built in for getting the belt on there tight http://www.electric-skateboard.builders/t/free-enertion-simple-motor-mount-open-source/12846/31

About the wear on the teeth, that does sound likely seeing as how I did wear through one belt and have had my board for just over a year but the belts aren't that expensive and I ride pretty often so I just chalked it up as a small consumable.  The pinion itself hasn't shown any substantial signs of wear (just surface scuffing but nothing appearing to wear down).  I think most of that tearing was due to having the belt a bit too loose though and braking too hard more than anything, since I replaced it a while back and then also adjusted my wheel spacing by adding a washer to make sure the belt doesn't rub the screws holding the motor in and it seems all is well.

Think the 3D printed option is worth a shot too if you have an all metal hot end then nylon can be really good for things like this.  Makes a nice solid part and since the nylon tends to stay as a single thread instead of melting completely like abs or pla it makes the parts quite a bit stronger (beyond the material properties).
```

---
## \#7 Posted by: Shahar9320 Posted at: 2017-06-26T06:26:37.509Z Reads: 356

```
I just bought a *very* similar board: 12s2p , vesc, 6374 190kv all from  diy but I bought an extra 13t besides the one that comes with the kit and also 83mm wheels.. I need torque more than speed but if there aren't a lot of hills where you live I think you'll be fine with the 97's and just buy a 13t pulley
```

---
## \#8 Posted by: SirDiff Posted at: 2017-06-26T07:06:04.030Z Reads: 356

```
[quote="tvidotto, post:4, topic:26169"]
feels it is too much compared to other boards I see here with better electronics and less top speed
[/quote]

Your speed is determined by teeth ratio, wheel diameter, battery voltage and motor kv. If you take a 245kv motor, 6s battery and the right ratio, you can get higher speed than much better boards. It's not the top speed that determines how good a board is. By the way, 190kv is a bit high for 12s, be sure to have the max rpm setting right (60k) in the vesc settings, otherwise you might fry your drv chip 
P.s. Right now in this thread there are 3 posts made by you. 3
**Half life 3 confirmed**???
```

---
## \#9 Posted by: tvidotto Posted at: 2017-06-27T05:21:42.243Z Reads: 343

```
[quote="SirDiff, post:8, topic:26169"]
be sure to have the max rpm setting right (60k) in the vesc settings
[/quote]

Great! tips like this are really welcome. I will be sure to get this done when I get the battery

[quote="SirDiff, post:8, topic:26169"]
P.s. Right now in this thread there are 3 posts made by you. 3
Half life 3 confirmed???
[/quote]
4 posts now!! 4!!
```

---
## \#10 Posted by: tvidotto Posted at: 2017-06-27T05:29:44.814Z Reads: 362

```
Updates:
I started 3dprinting a 40T pulley to see if the belt is long enough. If it doesn't fit, I can try going smaller with the wheel's pinion and go for a 13T instead of 16T.
<img src="/uploads/db1493/original/3X/9/2/920269735d76c6b63bd7198223a02b70367da4bc.png" width="690" height="383">
<img src="/uploads/db1493/original/3X/0/5/05bc0a7f9935a74fe08150c6391f25f2f876027b.png" width="690" height="368">

I also got some deliveries today, both miamielectricboard and diyelectricskateboards where fast with the shipping almost beating Amazon prime, which is impressive, I am only missing the battery now.

<img src="/uploads/db1493/original/3X/6/1/61f9fc6ab5cab9c734daaaa93578b58ddafa96b1.png" width="690" height="428">

I really want to start assembling everything but if I do, I cant use the board tomorrow =]
```

---
## \#11 Posted by: tvidotto Posted at: 2017-06-28T03:15:27.508Z Reads: 347

```
updating:
printed the 40T pulley (still with support material)
<img src="/uploads/db1493/original/3X/d/e/de2cfab9db81a64be25af1b8205db99202f67f33.png" width="690" height="428">

After the lye bath
<img src="/uploads/db1493/original/3X/0/8/08b1bed65c5e9b42344d8e10e4afaba9accccb6f.png" width="690" height="490">

bad news is that the belt is too short for 40T and 16T. I think I need an extra belt to try this ratio.
<img src="/uploads/db1493/original/3X/8/8/886a77b9314dcca2c6e4c4691f5bf9c72182f73e.png" width="690" height="394">

Another change of plans is that based on the size of the motor I will probably not be able to mount the truck as drop-thru.
But I also don't want the deck hole to be visible so I am looking into alternative solutions.
I found online some back plating for drop-thrus but did not find one that I like yet
```

---
## \#12 Posted by: wafflejock Posted at: 2017-06-28T03:41:30.132Z Reads: 328

```
Huh I thought from the other designs I'd seen with this motor mount the nut in the bottom left of your last photo was holding a screw that goes through a slot where you could adjust the spacing? Is that not true, or the slots just don't give enough play for the extra diameter pulley?  On the plus side the cleaned up print looks good.
```

---
## \#13 Posted by: tvidotto Posted at: 2017-06-28T03:47:40.869Z Reads: 319

```
[/quote][quote="wafflejock, post:12, topic:26169"]
of your last photo was holding a screw that goes through a slot where you could adjust the spacing
[/quote]
It does allow some movement but not enough.
I can also 3dprint the 13T wheel pulley, but I think it may be too much stress for a 3dprinted part. I will never know if I don't try it
On the meantime, I am trying to get in contact with diyelectricskateboards to see if they can ship another belt together with the battery
```

---
## \#14 Posted by: wafflejock Posted at: 2017-06-28T04:01:20.188Z Reads: 307

```
Bummer sorry for the crap advice I thought it would have been enough since I can get quite a bit of slack on the mount I got from DIY that I figured it would probably be the same kind of deal with that mount but guess I shouldn't have assumed.  Yeah they have been really accommodating with adjusting orders for me in the past so hopefully that works out.

Also curious what plastic did you end up printing it with (sorry if you mentioned it don't see it anywhere).
```

---
## \#15 Posted by: tvidotto Posted at: 2017-06-28T05:08:20.172Z Reads: 309

```
[quote="wafflejock, post:14, topic:26169"]
sorry for the crap advice
[/quote]

nothing to be sorry about, your logic was right

About the print, the printer name is "Dimension 1200es" and according to the internet it uses ABS

<img src="/uploads/db1493/original/3X/d/5/d52f1576fa04f58c3b6c40356c30a9fd1bbf0f04.png" width="391" height="204">

It took roughly 3 hours to print and around 10 hours on the lye bath to dissolve the support material.
```

---
## \#16 Posted by: sl33py Posted at: 2017-06-28T05:09:28.045Z Reads: 314

```
Hey @tvidotto!  Welcome to esk8!  I'm just across the lake from you!

First off - gearing - if you want to avoid monster speeds on 12s, i'd stick to as low as you can go.  14/15t motor and 40t wheel.   Especially with the 97's on 12s!

Another way to keep speeds down is to go to 149kv or 170kv motor.  

I have spare belts a-plenty even if you want to test fit an assortment of sizes.  Not sure if you get down by the airport any time and want to get a helping hand just shoot me a PM.

With your 3d printer - i'd really suggest the GT2b vs nano.  I know i've had drops from tons of wifi 2.4 w/ others and no issues with GT2b.  Madmonkey, badwolf, baby buffalo, etc - tons of options.

I ride out at Alki pretty frequently too (play beach VB nearly every Fri during the summer), so if you want a chill ride some time we can get @smurf to join too when his build is finally done!

GL!
```

---
## \#17 Posted by: tvidotto Posted at: 2017-06-29T06:26:47.717Z Reads: 300

```
hey @sl33py ! thanks!

Oh nice, so you are around the Tacoma area-ish? I go there sometimes.

[quote="sl33py, post:16, topic:26169"]
With your 3d printer - i'd really suggest the GT2b vs nano
[/quote]
You mean getting that bulky controller and using another case to make it smaller? I will start researching about that, for sure the last thing I want is losing connection 

Alki looks amazing! I never been there, I dont think my board can get that far, but maybe I can find another way.
```

---
## \#18 Posted by: tvidotto Posted at: 2017-06-29T08:43:44.717Z Reads: 332

```
new updates:

I got the email that the battery was shipped so if it follows the same shipping days from last time I may be able to start the build this weekend.

I could not manage to get a new belt shipped with the battery in time,  so I decided to go for a shorter motor mount ( to fit the 40t pulley). I downloaded a bunch of mounts on Thinginverse but none of them was like I wanted, so I modeled a new in Maya ( the printscreen is not the final, it is missing the motor hole and some other minor adjustments )

<img src="/uploads/db1493/original/3X/c/3/c3809f456cf9046e264d81c725c20122f1a6f4f4.png" width="587" height="500">

Same for the pulley, I did not find a 13 teeth pulley for 12mm belt. I tried to be as precise as possible, but Maya is not the best program for that. I will discover if it works on the following days.
<img src="/uploads/db1493/original/3X/8/6/86f64f114375acd0bb8efef402a5067b2b7ce201.png" width="265" height="358"><img src="/uploads/db1493/original/3X/d/7/d785ec7e0fddd6e20f462162324af4a841883d96.png" width="430" height="500">
(looking really weird with the support material =] )

Also on another news, a friend that lives in the building got interested and it just bought a longboard, that may lead to another electronic board in this area.
```

---
## \#19 Posted by: wafflejock Posted at: 2017-06-29T17:45:05.499Z Reads: 318

```
Cool stuff thanks for sharing and keeping us all posted on the build so far.

Don't have a dual extruder setup here so I can't really do the support material as something aside from what I'm printing with... I guess it eliminates the lye processing dangers and time but don't end up with as clean of parts in the end.  Really makes me think adding another stepper to my 3D printer and dealing with the config might be worth it.

Thingiverse is great for simple/common stuff and inspiration but happens often that I end up browsing for a bit then deciding it's faster for me to model the part I need than try to find someones listing that is good.  That said things like the pulley are kind of a pain to model so I use the OpenSCAD file for pulleys on thingiverse for those:

https://www.thingiverse.com/thing:16627

Printed a battery enclosure last night that has a little actuating part (2 parts in one print) for locking it into a larger enclosure but I had a few issues printer skipping steps (reduced acceleration on the printer and tightened the belts) and some issues with the multiple parts in one print that I should be able to fix with little bridges that can be cut out after the print.  On the plus side even though it had issues printing I was still able to break the sliding part that I spring loaded free so it will lock into the outer container

http://storage8.static.itmages.com/i/17/0629/h_1498757783_5861991_ad946310bc.jpeg

Also need to flatten out one side of the moving part so it won't tend to pop itself out but can be popped into the slot... any other ideas or thoughts welcome.

---

Regarding your motor mount I think you're probably going to either need to go thicker with that or use Nylon or some other higher temp plastics (ABS or PLA probably won't cut it at that thickness, maybe at a really high infill % it can hold up but will be a pretty serious test of that plastic, ABS is more compliant to bending it a bit or mushing than PLA, Nylon or PTFE is stronger than both and can get variable types of flexibility or rigidity depending on what you want/need).  When the motor turns and pulls on the belt it really wants to spin the whole mount around the truck, the whole equal and opposite reaction thing, so the mount gets kicked around with a lot of force.... it might work but I'd probably go thicker or Nylon... just my .02
```

---
## \#20 Posted by: tvidotto Posted at: 2017-06-30T03:18:05.940Z Reads: 307

```
[quote="wafflejock, post:19, topic:26169"]
Don't have a dual extruder setup here so I can't really do the support material as something aside from what I'm printing with... I guess it eliminates the lye processing dangers and time but don't end up with as clean of parts in the end.  Really makes me think adding another stepper to my 3D printer and dealing with the config might be worth it.
[/quote]

I think the time spent on the lye bath is not that bad, it saves me a lot of work. The problem is that that thing is really strong. At work we have a room dedicated to those strong materials with an emergency washing system in case it spills in the face.
The nice description they gave me about the lye was: if you touch and feel your fingers sticky, it is fat melting.

Those parametric pulleys looks a great idea, I am downloading the program now.
[quote="wafflejock, post:19, topic:26169"]
Regarding your motor mount I think you're probably going to either need to go thicker with that or use Nylon or some other higher temp plastics
[/quote]

This is an excellent observation; it seems highly possible now that you mentioned that I will have issues with temperature, the print looks really thin now that you mentioned. I left it printing yesterday night so at least I can test it and adjust in case it fails.
```

---
## \#21 Posted by: wafflejock Posted at: 2017-06-30T03:45:44.383Z Reads: 267

```
Cool yeah OpenSCAD is a bit of a clunky sort of UI but basically can put in the parameters you want for the pulley type and number of teeth and everything then hit F5 and it will remake the model, once you're happy with the parameters you hit F6 and it processes it into a mesh then there's a button for STL export.  There's also an openscad file for a rack and pinion setup I'm planning on using just really useful for simple parametric parts (especially when someone else already did the coding/scripting)
```

---
## \#22 Posted by: tvidotto Posted at: 2017-07-02T09:28:37.290Z Reads: 284

```
[quote="wafflejock, post:21, topic:26169"]
Cool yeah OpenSCAD is a bit of a clunky
[/quote]

A friend suggested me a program called Adobe fusion 360. I will do some more research about, but at first glance they look much better for the work I am doing.

----
I printed the shorter motor mount but I noticed some mistakes, the internal ring is too small and doesnt fit the truck, also the role for the screw could be better designed. So I will probably update the project and print again.

The 13T pulley came out almost perfect. The belt fits without any problem. The only downside is that the printer app closed some open holes and I will have to drill the shaft role again

<img src="/uploads/db1493/original/3X/6/4/64ce98b8adc79871eb49790adb5570ce6418c427.png" width="690" height="389">
```

---
## \#23 Posted by: wafflejock Posted at: 2017-07-02T17:21:23.225Z Reads: 274

```
Gotcha yeah plus side with ABS is it is workable sort of like a clay or something (guess you could say it's the aluminum of plastics).  Drilling shouldn't be much of a problem so long as the bit doesn't grab in too deep and crack the part.  Regarding OpenSCAD I kind of use it as a sledgehammer, that's to say it's a great tool but limited uses, basically if you need something that someone has already modelled in OpenSCAD or you need to model a lot of a thing that is similiar but with 1 or two variables that drive the model that change then it's great.  Basically I use it for generating one off parts like a gear or whatever and then export the STL and then pull it into something like OnShape or Blender where I can work on more complex models with UI that "makes sense" for the job.

I'm primarily a web dev but have been messing with various CAD software on and off for years.  Messed with AutoCAD as a kid on my Dad's computers and used to bother the computer graphics guys across the hall in college all the time to show me how to do stuff in 3DSMax.  More recently I'd been taught how to find my way around pretty quickly in Blender so I was using that for modelling 3D prints but it takes a lot of forethought to get things done in there that are pretty trivial in other programs and has some really crappy bugs with things like the boolean operator that make it frustrating to work with.

OnShape is a browser based tool and free to use for non-commercial purposes and is parametric, constraint based modelling (similar to Fusion360 from what I gather).  I've heard good things about Fusion as well but I'm a Linux die hard and so far they have no browser version of the software released (or linux version).  I wrote a big rant to Adobe like 5 years back about how they should get on Linux and that most people are using Windows and other shit proprietary systems because they are locked into the Adobe tools they learned and can't use those tools on Linux, hence no Linux adoption on the desktop... anyhow I'm going to get into my whole Linux thing so I'll just stop...  But yeah Fusion 360 :thumbsup: should be good if you want a cross platform browser based thing OnShape is pretty similar and free to use for us tinkerers.
```

---
## \#24 Posted by: tvidotto Posted at: 2017-07-05T06:22:54.268Z Reads: 276

```
[quote="wafflejock, post:23, topic:26169"]
I'm primarily a web dev but have been messing with various CAD software on and off for years
[/quote]

I used to love AutoCAD when I was in the architecture university, some year after I want to stay away from it as much as I could

This fusion 360 actually is really simple and powerful. Basically, you sketch all the dimensions you need and start extruding and chamfering as needed. Feels pretty good to model things precisely again.

After the suggestion of making the motor mount thicker, I decided to start it from scratch on Fusion to test it's workflow
the camera movement is really weird, doesn't look like any 3d program that I used before, but other than that is great

<img src="/uploads/db1493/original/3X/a/6/a68ef958a7d98309bc1565ee614c6ab68467ad02.png" width="689" height="473">

<img src="/uploads/db1493/original/3X/9/d/9d7d9f7f5bb0ce43cf106adcf26bd7d04877bfba.png" width="690" height="370">


 Now that the mount is thicker it will require new bolts for the motor and to lock the mount into the truck, I am thinking on getting m4 20 for the motor instead of the original m4 12 and m5 30 for the mount itself.

I also still need to figure out how I will attach the battery on the deck but I will wait for them to arrive first, it is expected by tomorrow since today was a holiday
```

---
## \#25 Posted by: raadio13 Posted at: 2017-07-05T12:30:56.836Z Reads: 245

```
can we borrow the 3d drawing lol :D
```

---
## \#26 Posted by: tvidotto Posted at: 2017-07-06T07:32:29.397Z Reads: 271

```
For this last one? Sure,  I can totally share it, I am only afraid if that the clamp system I did will hold it, now that I tested the motor the torque seems way higher than I was expecting and I believe it may rotate a little

I may need to add some teeth there or make it as two pieces instead of four.

---

updated
I printed the second version of the mount but I am afraid it will not handle the torque. I am not sure how much the motor tries to rotate so I may need to update the design. There is only one way to test.
<img src="/uploads/db1493/original/3X/4/7/471d6db1e96dfc53d6c9c3eb7f0a164917e2bd7e.png" width="690" height="383">

I also printed a cap with the logo of the game that I work for the drop-thru holes that are exposed on the deck, but again another mistake in the calculations. The trucks support both patterns of hole, but when I unassembled it I discovered that my deck doesn't. So it needs to be bigger and follow the old-school pattern.
<img src="/uploads/db1493/original/3X/8/5/85f24a3e41fe7d1875ca296b34af016f878bfc61.png" width="690" 
height="418">

Also, are those number correct?
<img src="/uploads/db1493/original/3X/b/1/b1295aedab84324286d8d9236051ad52269c84f3.png" width="690" height="347">

my battery is a 12s2p  6ah 44.4V 266.4wh
motor is 6374 190KV
```

---
## \#27 Posted by: wafflejock Posted at: 2017-07-06T07:48:30.355Z Reads: 262

```
You can use Acetone to "ABS weld" the parts together once you have everything aligned and tightened up as much as you can without cracking anything.  Just do it in a well ventilated area you basically just put some pure acetone in a glass and use a brush (not made of plastic or at least not ABS or something that will dissolve in the acetone) to brush a little acetone onto each part you're going to join then just clamp them together and let the acetone evaporate out.  The acetone will melt the top layer of the plastic and it will chemically bond into one part, it will be at least as strong as the print layers.

You can also make some "abs juice" or "abs slurry" by adding some abs scraps into the acetone in a jar and again keep it in a well ventilated area and sealed up (slightly exothermic reaction I guess so good to add the ABS kind of slowly or just do small quantities as you need it).  That way when you "paint" it on you are adding a little material as well since it will tend to sort of melt away.  Also the brush will likely be ruined once the acetone evaporates from it the plastic will harden in the bristles, if you let it sit in acetone for a minute or so it will soften up again though so it just becomes your plastic bonding brush.

---

Also think your battery cut off is pretty low what kind of batteries were you using again? need to do the low safe point * 12 to get your cut offs, 30-33 would be for 10S with li-ion I believe, LiPo better to stay in the 3.6-3.8 range on the bottom per cell.
```

---
## \#28 Posted by: tvidotto Posted at: 2017-07-06T07:59:38.850Z Reads: 251

```
[quote="wafflejock, post:27, topic:26169"]
You can use Acetone to "ABS weld" the parts together once you have everything aligned and tightened up as much as you can without cracking anything
[/quote]

this is actually a great idea, I will buy some acetone tomorrow

[quote="wafflejock, post:27, topic:26169"]
what kind of batteries were you using again?
[/quote]

it is from DiyElectricskateboard, it says " HHS Li Ion 18650"
```

---
## \#29 Posted by: wafflejock Posted at: 2017-07-06T08:15:00.144Z Reads: 257

```
Did some searching around looks like 3.0 is the absolute bottom I'd probably go with 3.2 - 3.5 as the per cell cut off limits and then check how many mAh actually go back into the battery.  You want to ideally only drain 80% or so of the charge just to maximize the life cycle and limit the chance of ever dropping any given cell below the 3.0 a which point it will degrade and will probably need to be replaced which usually means replacing more than the one cell.  So with 6Ah after you get back to recharge you should be putting about 4.8Ah, if it's more than that you might want to increase the cut offs, if it's less than that you can decrease the cut offs.

So 3.2 * 12 = 38.4V and 3.5*12 = 42V

Set those as the end and start cut off values, then it will reduce power when you get down to 42V and cut off power when it hits 38.4V.  If you want to be more conservative could cut off between 3.6-3.8 which is the safe range for run of the mill RC LiPo batteries.

---

You basically just want to be sure you don't ever get any cell going below the safe voltage level for any extended period of time but need to keep in mind there is voltage sag when you're drawing a lot of power out of the pack and you don't want that sag to ever go below 3.0V, so if you get a .5V dip whenever you're cruising then you'd want your low cut off at 3.5... hopefully that makes sense.  Could check with DIY on what they recommend for safe minimum voltage.
```

---
## \#30 Posted by: tvidotto Posted at: 2017-07-09T00:59:04.890Z Reads: 267

```
I went to a huge construction store here called Home Depot, and struggled trying to find the imperial sizes to the metric system. There is no progressive pattern on the numbers, and it is a mess how they name them.
The numbers are closer but they don't match, my 3dprinted mount cannot be used because I have no way to attach it to the motor. I tried screwing and they cant handle the torque because the holes are too tight.

<img src="/uploads/db1493/original/3X/7/8/78a54dd2905b0b50390bc10bfdbcc692e73494da.png" width="690" height="443">

This is me trying to take it off after the second one broke while I was complaining about the imperial system =]
<img src="/uploads/db1493/original/3X/f/f/ff8ca0ad8ca67e60c5afcdb1c42b6ffacab98b67.png" width="612" height="370">

So I went up with the original mount. When adding the motor pulley I faced couple issues, first there is a metal piece that comes with the motor and works as a lock mechanism for the pulley, that piece was too big for the space on the motor shaft, I don't know how this happened because it came with the motor on the same package, they were supposed to fit together. Anyways, 1 hour later after sanding, it ended up fitting.

The second issue was my fault; the screws that came with the pulley are not flush with the diameter, and they don't have enough clearance from my 97mm wheels. So I had to skip using them. The pulley got it so snug on the shaft that I doubt they will even be separated again.

<img src="/uploads/db1493/original/3X/8/b/8bb2ee16dbec30ac1e2d3caaa0e1dbdf3286163d.png" width="475" height="500">

The first attempts to roll the wheels I could hear some strange noises that were matching with the frequency of the spin, my guess was that the belt was too tight and after releasing the tension the noise disappeared.

I am using the nano remote and it is hard to keep a progressive acceleration, feels that the controller is too sensitive and it goes from zero to "trying to trow me away from the board" too fast.
I wonder if I can change the acceleration curve on the vesc or maybe swapping to those gt2b controllers and get a more smooth acceleration.
```

---
## \#31 Posted by: rpn314 Posted at: 2017-07-09T18:21:47.196Z Reads: 245

```
[quote="tvidotto, post:30, topic:26169"]
I wonder if I can change the acceleration curve on the vesc or maybe swapping to those gt2b controllers and get a more smooth acceleration
[/quote]

Check out @Ackmaniac's firmware
```

---
## \#32 Posted by: tvidotto Posted at: 2017-07-10T07:43:10.715Z Reads: 243

```
Will do. Just need to learn how to do it and if it is possible to revert if I don't like

I tried today reducing the motor max and motor min by half and it worked, made the acceleration and brake much more smooth, but the board felt weak to the point that could not stop going down on a hill.
```

---
## \#33 Posted by: tvidotto Posted at: 2017-07-15T09:20:10.156Z Reads: 243

```
changed the firmware to @Ackmaniac 's and tomorrow will start testing it.

I also started tearing apart my GT2E controller and I was wondering: Are those functions necessary?
<img src="/uploads/db1493/original/3X/9/6/96fd4a0874a6943236bed06bf2ab45a57210a48c.png" width="390" height="473">

I guess only the binding, power and led lights are useful. Anything else?
```

---
## \#34 Posted by: tvidotto Posted at: 2017-07-17T03:36:45.767Z Reads: 238

```
the vibration of the road untightened the motor mount and messed with the alignment.
I had to come back home carrying the board =]

<img src="/uploads/db1493/original/3X/b/4/b4e6299b3fe4afe4eff6e3c3106e4ba65e9d5e8c.png" width="690" height="492">
```

---
## \#35 Posted by: Eboosted Posted at: 2017-07-17T03:52:10.231Z Reads: 232

```
Motor mount bolts should be installed with Loctite always!, I see your motor mounts are abs, I'm not sure if that's going to hold though
```

---
## \#36 Posted by: tvidotto Posted at: 2017-07-18T06:00:39.607Z Reads: 243

```
The one I was using are the Enertion, they had Loctite but I think the problem was something else, they were mounted too close to the middle of the truck and that part is not flat enough, so the contact area with the truck was reduced. I filed that part it apparently this plus the loctite fixed the issue
This is where I started filing
<img src="/uploads/db1493/original/3X/7/e/7e409fcd1be2c931878dc2c9f5e0f0ac53eef2ff.png" width="690" height="411">

I still want to try the 3d printed mount, but I am getting into multiple issues. I used Loctite on the motor pulley screws and I cant take them off now... I tried warming up them with a soldering iron and only worked for 1, the other three doesn't want to move.
Apparently acetone works, that will be my next test

On the meantime I decided to design new wheel pulleys to my wheels

so I modeled the wheels and made the pulley no a way that it fits exactly the shape
<img src="/uploads/db1493/original/3X/7/3/7348701a5ed9c940f7074e0de33a2b39c1e657a6.png" width="540" height="500">

<img src="/uploads/db1493/original/3X/a/1/a11833f2e9e4ada490915389c6a9b3418dc9b262.png" width="477" height="500">

I am not sure if going that high with those "pillars" inside of the wheel are a good idea.I will have to test
```

---
## \#37 Posted by: tvidotto Posted at: 2017-07-19T06:04:23.595Z Reads: 233

```
I designed the pulley to have nuts inserted and utterly failed; the nuts are big enough to hit the truck and don't allow it to spin.
I will try next without the bolts and see if the pastic can hold the screws.
<img src="/uploads/db1493/original/3X/5/8/589b139a67989131313c7c3c1c95041696df440a.png" width="690" height="490">
```

---
## \#38 Posted by: tvidotto Posted at: 2017-07-25T04:45:38.207Z Reads: 232

```
I updated the design without the nuts but I made the screw holes not tight enough. 
After a week it got a little eccentric and broke

<img src="/uploads/db1493/original/3X/7/6/7600a85dc5423be156c2cae34572ffdba930a014.png" width="536" height="384">
```

---
## \#39 Posted by: tvidotto Posted at: 2017-07-30T19:24:49.793Z Reads: 224

```
updated the design with screw threads and more contact to the teeth area

<img src="/uploads/db1493/original/3X/0/3/03b046ebb6e4a9d193ed6db0041a699c2465e39a.png" width="690" height="389">
```

---
## \#40 Posted by: wafflejock Posted at: 2017-08-11T22:46:57.665Z Reads: 212

```
Looks good if you still have problems with delamination (breaking across layers) you may want to consider doing a mold of this (3d printed part) in silicone and pouring the urethane plastic part out of a mold, gets rid of the possible delamination issue and you can get different types of urethane plastics that are tougher or more flexible depending on what you need here.  I've been playing with this for the last few weeks and it works well for certain shapes, with this one could do a two part mold pretty easily since all the holes and parts that stick out go in one direction could mold in the orientation you have it on the table.  Also once you have a mold of a good part can re-use the mold 30-50 times from what I've read (have used one at least 15 times without any issue yet).  Initial cost for some silicone sampler pack an urethane plastic will be pretty high (like $50-60 for both) but should be able to probably make 10 or so of them with the sampler size of urethane plastic that gets poured into the mold so if they are good enough can probably get rid of them for $5 a piece and recoup your money.
```

---
## \#41 Posted by: Mattmccrary8 Posted at: 2017-10-10T13:43:42.613Z Reads: 184

```
What are you vesc settings I’m having problems with mine
```

---
## \#42 Posted by: tvidotto Posted at: 2017-10-17T03:10:42.656Z Reads: 176

```
sorry the huge time not showing around.
The problem with the gear, was indeed excentric rotation. after that I printed multiple gears and they never had any problem

@Mattmccrary8, what problems are happening on yours? 
I keep changing my settings, since I keep messing with gear rations, belts and motors. will do it again today
```

---
## \#43 Posted by: tvidotto Posted at: 2017-11-04T05:14:23.221Z Reads: 160

```
Damn, burned my third vesc in 6 months

2 riding FOC and 1 riding on BLDC
```

---
## \#44 Posted by: tvidotto Posted at: 2017-11-15T06:08:10.919Z Reads: 151

```
I am having some issues with FOC
When I am going really slow, the breaks tend to lock.
I tried messing with all the configuration but even with a **Motor min** and **Bat min**, I can still feel the motor locking.

Tried with the same config on BLDC and the issue is gone

I was getting into the silence of FOC...

My config right now is:
**Motor Max 70**
**Motor Min -60**
**Batt Max 60**
**Batt min - 20**

Any idea what it could be?
```

---
## \#45 Posted by: Colson003 Posted at: 2017-11-15T06:35:59.237Z Reads: 148

```
What fw is your VESC running?
```

---
## \#46 Posted by: cwazy1 Posted at: 2017-11-15T06:44:42.149Z Reads: 148

```
I've had awful luck with TB VESCs. If you're insistent on riding FOC, ditch the TB VESC and grab a FOCBOX. 

Let me know if you're ever up in Seattle. We should get a group ride going when the weather turns better.
```

---
## \#47 Posted by: Colson003 Posted at: 2017-11-15T06:51:26.925Z Reads: 141

```
I've been running FOC sensored on 6s with 3.31fw and haven't had any issues. Super smooth and no "boost effect" with the 3.31 fw either. I really like my TB vesc
```

---
## \#48 Posted by: cwazy1 Posted at: 2017-11-15T07:02:24.596Z Reads: 142

```
I cannot attest to the new 3.x FW, I've heard its made FOC a bit more reliable.
```

---
## \#49 Posted by: Eboosted Posted at: 2017-11-16T20:31:00.106Z Reads: 140

```
I'm having the same issue I was thinking about decreasing the motor min from - 65A to - 55A to test it. I. Might go back to BLDC as well as FOC is nice but it's like riding a Toyota Prius, sometimes you want to ride a V8 with full exhaust
```

---
## \#50 Posted by: tvidotto Posted at: 2017-11-17T05:12:29.229Z Reads: 144

```
[quote="Colson003, post:45, topic:26169, full:true"]
What fw is your VESC running?

I've been running FOC sensored on 6s with 3.31fw and haven't had any issues. Super smooth and no "boost effect" with the 3.31 fw either. I really like my TB vesc
[/quote]

The firmware is 4.12. It is the torque boards vesc updated to that firmware that comes with the Watt mode

I dont remember having this issue before... Well, BLDC is working great and smooth right now but I miss the silence

[quote="cwazy1, post:46, topic:26169, full:true"]
I've had awful luck with TB VESCs. If you're insistent on riding FOC, ditch the TB VESC and grab a FOCBOX. 

Let me know if you're ever up in Seattle. We should get a group ride going when the weather turns better.
[/quote]

Oh nice! I am actually in Bellevue but I could get to Seattle no problem.
I was thinking about the FocBox but I actually dont know if they are better and if they will fit my enclosure, they look bigger and my enclosure is already packed
(could be a good excuse to make a new board =] )

[quote="Eboosted, post:49, topic:26169, full:true"]
I'm having the same issue I was thinking about decreasing the motor min from - 65A to - 55A to test it. I. Might go back to BLDC as well as FOC is nice but it's like riding a Toyota Prius, sometimes you want to ride a V8 with full exhaust
[/quote]

I tried reducing to -10A, same thing...
I am starting to guess is the Firmware for the Watt mode, I used FOC before and it was fine ( till I blew off the vesc messing with a new controler :) )
```

---
## \#51 Posted by: Eboosted Posted at: 2017-11-17T05:27:15.976Z Reads: 116

```
It's not the firmware, as I'm using Vedder original current mode, not Watt mode from ackmaniac as you, and I still get the wheel locking
```

---
## \#52 Posted by: cwazy1 Posted at: 2017-11-17T06:24:12.261Z Reads: 131

```
[quote="tvidotto, post:50, topic:26169"]
Oh nice! I am actually in Bellevue but I could get to Seattle no problem.
I was thinking about the FocBox but I actually dont know if they are better and if they will fit my enclosure, they look bigger and my enclosure is already packed
(could be a good excuse to make a new board =] )
[/quote]

I'll send you a pm with my contact. Lets go ride sometime. My gf lives right across the street from MS, so I'm over there quite often! 

Focboxes are actually about half the size of 4.x VESC. They're TINY.
```

---
## \#53 Posted by: tvidotto Posted at: 2017-11-17T06:40:28.181Z Reads: 135

```
[quote="cwazy1, post:52, topic:26169"]
Focboxes are actually about half the size of 4.x VESC. They're TINY.
[/quote]

oh really? I guess I got it wrong from the pictures.
They look much more sturdy. I think I will try them
```

---
## \#54 Posted by: tvidotto Posted at: 2017-11-17T06:42:57.913Z Reads: 137

```
I forgot to post updates here.

I was having some issues with the breaks making the belt skip some teeth on the motor pulley, so I decided to add a little more tension. It increased a lot the breaking power, but those 3dprinted wheels ended up breaking after two weeks of usage.


<img src="/uploads/db1493/original/3X/4/2/42c3f2b49a2c5783d9539890ee15c895da6c00c5.png" width="690" height="389">
```

---
## \#55 Posted by: tatze Posted at: 2017-11-17T21:10:33.472Z Reads: 122

```
Maybe you can try to use just the bearings (two next to each other) than you have to do a some adjustment but i think they dont wear out.
```

---
## \#56 Posted by: tvidotto Posted at: 2017-11-18T03:00:48.124Z Reads: 118

```
[quote="tatze, post:55, topic:26169, full:true"]
Maybe you can try to use just the bearings (two next to each other) than you have to do a some adjustment but i think they dont wear out.
[/quote]

that is probably a better solution, I will try again
```

---
## \#57 Posted by: tvidotto Posted at: 2017-11-18T03:07:19.338Z Reads: 122

```
Two weeks ago I had an accident where my motor stopped for no reason. I was pushing it really hard, and at some point it just cut, and I went flying forward. I hit my knee on the ground and after days of pain I ended up going to a doctor.

At that day I had adjusted the Motor max to 80A so I thought that I stressed too much the motor and it got too hot.
I ended up changing the motor and replaced for two 6374 and reduced back to 70A

Today on the same hill, I forced again, and the same thing happened, I was more aware this time and did not fall, but I am starting to lose confidence in the motors.

Any idea what it could be? Could it be the TB Vescs? Maybe the motors getting too much rpm?
```

---
## \#58 Posted by: louwii Posted at: 2017-11-18T05:45:11.644Z Reads: 116

```
Isn't your VESC that's just stopping because it's over-heating ? Or your trying to pull out too much amps ?
```

---
## \#59 Posted by: cwazy1 Posted at: 2017-11-18T05:52:33.138Z Reads: 113

```
the 12s2p TB pack has a max of 20A. IMO you're pulling too many amps and probably hitting overcurrent and/or overheating as lou said.
```

---
## \#60 Posted by: tvidotto Posted at: 2017-11-18T18:13:48.619Z Reads: 112

```
[quote="cwazy1, post:59, topic:26169, full:true"]
the 12s2p TB pack has a max of 20A. IMO you're pulling too many amps and probably hitting overcurrent and/or overheating as lou said.
[/quote]

[quote="louwii, post:58, topic:26169, full:true"]
Isn't your VESC that's just stopping because it's over-heating ? Or your trying to pull out too much amps ?
[/quote]

wait, so should I be only using 20A on the Motor Max? it seems too low compared to the other vescs configurations I saw here on this forum.
```

---
## \#61 Posted by: Lionpuncher Posted at: 2017-11-18T19:58:06.399Z Reads: 99

```
Not an expert. But i believe your battery max is more what determines what your battery will draw. Not sure if you need your motor max to be so high. Have you experimented with the 60amp range? Probs still plenty of power.
```

---
## \#62 Posted by: willpark16 Posted at: 2017-11-18T21:32:39.059Z Reads: 96

```
The other configurations probably had more juice available in the battery, I'm not sure what cells he uses in his 12s2p packs but i would say 20a max
```

---
## \#63 Posted by: cwazy1 Posted at: 2017-11-18T23:21:01.345Z Reads: 100

```
Unless your battery pack was order within the last month, you have the panny pf cells, which are 10A constant. 

Set battery max at 20A. Thats the capacity of your battery. You can keep motor max at 70A. 

Your battery min is also too high. 4A per 1P, so with you 2P pack, you should set battery min at -8A.
```

---
## \#64 Posted by: tvidotto Posted at: 2017-11-19T21:52:07.388Z Reads: 98

```
I use this configuration for months before and never had a problem... 

Today, same hill, same issue with the cut on trottle.
On the way back, it stopped working on a flat, at a walking speed and never came back

Two more Vescs to the graveyard. I am moving to focboxes and will try those specs


<img src="/uploads/db1493/original/3X/0/7/0714c540c9b699616b8290fd4a67acafca86be27.png" width="690" height="391">
```

---
## \#65 Posted by: tvidotto Posted at: 2017-11-27T07:59:48.148Z Reads: 85

```
I was checking my battery connectors and there is some black powder on the xt90 connector.
The battery is still working, but maybe that was the reason the two Vescs fried at the same time

Any idea what caused this? could it be some short circuit?

<img src="/uploads/db1493/original/3X/9/d/9d34ad82e3d65fb2dc3724296234e10c56946df4.png" width="617" height="331">



Also, I decided to upgrade my enclosure. Having only one is really annoying when you need to do some maintenance.

<img src="/uploads/db1493/original/3X/2/f/2f1f1f359f4c45da153f13cb118bb2c292722d44.png" width="690" height="390">

<img src="/uploads/db1493/original/3X/5/4/540b4bc220f6fda14648ce35a6369aff82c7386a.png" width="690" height="386">
```

---
## \#66 Posted by: wafflejock Posted at: 2017-11-27T08:21:30.914Z Reads: 83

```
Do you use an antispark loop key or switch when hooking up the batteries or do you get a spark when connecting them?  Never seen that particular funk in the plugs but would get some charring and a slightly frightening spark whenever connecting my batteries (never caused issues with the VESCs themselves though).  Appears you may have found the basic ingredients to life there or something.  Bummer to hear on all the dead VESCs probably worth sending those over to the DRVWizard if they are just blown DRV chips he can probably revive and you can resell or maybe he'll take them off your hands to resell himself (I dunno).
```

---
