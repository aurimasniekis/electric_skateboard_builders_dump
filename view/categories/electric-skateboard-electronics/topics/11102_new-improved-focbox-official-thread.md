# NEW IMPROVED: FOCBOX &#124; Official Thread

### Replies: 571 Views: 43094

## \#1 Posted by: onloop Posted at: 2016-10-14T06:34:01.206Z Reads: 1785

```
FOCBOX is the newest an best version of the open source VESC project.

The VESC is an amazing Hardware & Software innovation, It was introduced to the esk8 community late in 2014. Not too long afterwards it became the preferred option for most esk8 builders due to it’s awesome features & most importantly the Creative Commons license making it freely available for esk8 builders worldwide to build, sell, use, share & improve upon.


----------


**QUOTE FROM BENJAMIN VEDDER VESC DESIGNER:**
> To me it is natural to share knowledge and information, and something that I enjoy doing.


----------

## Some of the key features that make the VESC platform so amazing:

* Supports higher voltage when compared to most hobby grade ESC
* Has current control functions & safety features to help protect your electrical system from damage.
* Supports many different motors via a motor detection function
* Amazing starting torque allowing non-sensored motors to work very well on esk8’s 
* It has very good regenerative brake function, an important feature for esk8
* It has a very advanced open source programming tool catering to many different use cases
* It is compact


----------


> Since 2014 many different VESC’s have been made worldwide, some of them are made according to Ben’s open source plans & other VESC’s are [completely reworked versions](http://www.electric-skateboard.builders/t/what-do-you-think-about-these-new-vescs/6080) or some simply have upgraded components, some vesc’s are very good & some not so good. Thankfully we all like to share our experiences, both good & bad, on the various open forums like this one. This allow users across the world to report bugs, faults & most importantly share ideas that will improve a design. Here lies the benefit of sharing, this process is a very organic way to drive innovations, the feedback from the community helps to constantly improve & build better products for everyone.

## So why do we need a new & improved VESC?

There are a few issues with the current version 4 VESC, these issues are mostly related to usability, reliability & manufacturability.

**DRV ERRORS:** The DRV chip is a sensitive component that can report errors for many different reasons. Some people have discovered ways to prevent this from happening and many experienced VESC vendors claim it is related to the other components that share the space around the DRV. There is some evidence that upgrading a few key components has shown to improve the reliability.

**SHORTING THE VESC:** The VESC doesn’t have a proper case to protect it & it has a separate Capacitor PCB with exposed pins & wires that can easily get placed in the wrong spot causing a short. 

**OVERHEATING:** The existing form factor doesn’t allow the end user to easily install heat sinks (or a proper case) to improve the thermal properties and allow passive cooling to occur. This is not an issue for most people, however it is a weak link that can be a problem for users who like to push the limits of the existing architecture. 

**SOFTWARE:** The BLDC tool is not the most user-friendly interface your will ever encounter, Personally I think it is fine & most people can learn it after watching a few videos online. But there is definitely room for improvement.

**MASS PRODUCTION:** The existing VESC & BOM were never designed to be made at scale in a large PCB production facility, it was designed to be ‘easy’ to hand solder by the hobbyist at home. This is a huge issue when doing large scale production as it increases the chance for manufacturing faults & increases the cost of production. Furthermore, The process of final assembly of the main PCB with a separate capacitor PCB as seen on the existing VESC made it difficult to perform testing in a timely & systematic manner. 

_If you wanted to be very critical you could probably bring to light a few other problems that need to be addressed, However, the general consensus overall is the existing VESC is very good for most people with some room for improvement._


**As you may all know by now, Benjamin Vedder has started working on VESC 6, it addresses the issues above & the new VESC TOOL looks great so far, except the graphic logo I would change that :)**

> ## So here lie the issues with VESC 6

> -	VESC 6 is not here yet & there is no delivery date. 
> -	There is a chance it might not be released under the same CC license as the original VESC
> -	VESC 6 will be costlier as it has RF module built in & More components in general.
> -	The improvements might not be required by most users who would otherwise be ok with the cheaper VESC 4 architecture, or just a cheaper & more reliable vesc like VESC-X



----------

## So why make the VESC-X?

It’s really simple, we just want to make a better VESC. We want esk8 builders to have a better, more reliable product at an affordable price. When I was a kid my mother told me if you want something Jason don’t expect anyone else to make it happen for you. Just do it.

So back in February 2016 I started working with a talented manufacturing engineer who specializes in PCB design & electronic system testing. We worked together for months testing the existing VESC hardware & investigating the various faults that where occurring. 

Our goal was to make the VESC more reliable, perform better under peak loads, improve the design for manufacturing & improve the testing process before shipping to the end user.

We soon realised the entire form factor had to change, separating the power and logic, use of directfets all on the same side…. This was all very logical, most engineers experienced in this field would agree, we believe this is the very same logic that steered ben down the path of changing the form factor for the NEW VESC 6.


----------


## Systematic Testing & Jig Design

The current VESC 4.12 we are selling are all tested before shipping, we have a custom made test Jig that serves two purposes, it loads firmware & spins up the motor on each unit before we ship.

https://www.youtube.com/watch?v=N9kbYnCEkjw

Testing before shipping is critical to identify faults and has definitely lowered the number of faults that have occurred at the end users home. However overall we were not completely satisfied with this process alone as we felt we could further improve results by having another separate stage for spinning the motor. 

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/c/9/c9bf49896b263a8603dfd4097e70ce994ac595f0_1_666x500.jpeg
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/0/104b5a745787d9b3664704f95acf70ff06104a44_1_666x500.jpeg
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/0/d/0d578cae9ef08ba4775af94fa9b5ad63bdd33d9f_1_666x500.jpeg

The NEW 2nd stage test will run higher currents & do more intensive motor spin testing. Our goal is zero faults leaving the factory. **We believe with the two-stage testing process we can achieve our target of zero faults shipped.**



----------

## A SUMMARY OF THE VESC-X FEATURES & BENEFITS

http://cdn1.bigcommerce.com/n-yp39j5/zad02/product_images/uploaded_images/vesc-x-info-graphic.jpg?t=1475820483


**UPGRADED DIRECTFET PACKAGE**
1. New form factor places all fets on one side allowing improved thermal management design.
2. The metal package of the fets allows a better heat transfer and increases the current carrying capacities.
3. Precision CNC aluminum heatsink will be used to improve thermal dynamics keeping the board much cooler preventing shutdowns caused by overheating
4. Lower gate charge which will make it easier for the DRV8302. Faster switching time and reduced load on the mosfet driver.
5. Compact footprint keeping the high current paths as short as possible for improved efficiency the efficiency.

**UPGRADED BOM COMPONENTS**
1. Some components in the original VESC BOM have been identified as a potential weakness that may lead to premature failures, components have been replace with higher tolerances.
2. Increased number of ceramic decoupling capacitors for improved reliability. 
3. Large TVS diode capable of handling large voltage and current spikes, giving regenerative breaking an alternative current path when the battery is fully charged.
4. Micro USB port to improve compatibility with the more common cables used with mobile phones. Easily accessible keeping all wires streamline.
5. Low ESR bulk capacitors, giving you power when it's needed most.

**NEW FORM FACTOR**
1. The new form factor drastically improves the manufacturability of the VESC, the VESC-X is faster & easier to produce with reduced chance of manufacturing faults.
2. The new layout keeps the logic & power separate, meaning traces are shorter and both ceramic and electrolytic capacitors are closer offering a more robust & reliable power system.
3. Integrated Bulk Capacitors, inside the hard case, help prevent accidental shorts occurring & make the footprint more manageable in tight enclosures.
4. This new PCB design with more accessible mounting holes makes installing a heatsink & hard case simple.
5. Place holder M3 holes for adding another heatsink for even more cooling power.

**NEW HARD CASE & HEATSINK INCLUDED**
1. A precision CNC aluminum heat sink not only improves the thermal properties of the vesc by dissipating the heat away from the board, it also protects from accidental shorts, accidental damage of vital components and provides a user-friendly mounting solution so you can install the vesc securely inside your components housing using common M3 screws.
2. The top side of the new VESC-X hard case is made from super strong impact resistance ABS material, The top shell is non-conductive material and covers all the exposed areas making it nearly impossible to short out your VESC accidently.
3. The impact resistant ABS shell design offers easy access to the various ports and has a window for monitoring the LED's which is useful for diagnostics.
4. With the built to last Aluminium Heatsink & Impact resistant tough case the VESC-X will be protected from accidental damage, whilst offering superior cooling performance during peak load draw.
5. Compact footprint of the VESC-X allows two of them to be mounted side by side and keep all your wires nice and tidy to offer the cleanest builds out there, while still having access to all the ports.



----------

## The CC License

We are communicating to Benjamin vedder about our intentions and happy to abide by his terms in accordance with the CC license. We are willing to discuss this matter publicly & share our ideas openly. 

The VESC-X design was based on open source schematic to ensure the firmware would be compatible. We will provide the VESC-X schematic in a downloadable format from our website. http://www.enertionboards.com/how-to-build-eboard/vesc-x-files/ 

* There have been no software or firmware changes made.
* The original source files and libraries provided by Benjamin Vedder were not used. 
* The VESC-X Hardware uses an unmodified open source Firmware.



----------

## The Development Process
For anyone who is interested in seeing how much work has gone into this project, here's some photos & info:

**This is one of the first hardware revisions, it had the same fets as the existing VESC 4.12 & the overall size was too big so we had to rework this totally.**
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/5/557b89bc7010ef719bd24d23bc7c700edd7233d4_1_525x500.png

**One of the very first working samples. Still trying to work out how to get a heat sink onto the fets & keep the package small.**
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/d/df0713c87c938286ab8112cf0e37bf82ad63c568_1_375x500.jpg
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/9/9634e5356ba70cca55930433b4c9c4cfe98e2528_1_524x500.png
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/d/d950c1d3e63307d7924f78e88680af72410d0ac3_1_513x500.png

**Our first look at the directfet package, this really made a big difference to the footprint and made total sense in terms of improving the thermal efficiency & the heat sink housing design would be better too. However, it meant weeks of layout work down the drain.**
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/a/a9634f28c7a8fc385610ad91d78dae4e5cd33bd7_1_690x382.png
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/c/c66d6371396333a897612aba626e8434c4b22ee5_1_375x500.jpg

**Changes were made to the number of the capacitors, instead of one big one we used lots of smaller ones increasing the capacitance & also putting them closer to the fets to better filter noise.**
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/0/08de20a7012dd36227abac339acb61a1ef34a2a3_1_509x499.png

**This is one of the first concepts for the heat sink & case**
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/5/535bfb36014001a85f8c0f2c87215f7e43528ac8_1_500x500.JPG
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/0/00b5c02b7d69214c08cf27ee96b27944f4dddadd_1_666x500.jpeg

**We didn't like it that much, so made some changes**
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/b/b47fc70de210ad10cbde71b122900e27d68d3697_1_500x500.JPG

**We realised fins won't do much inside an enclosure without much airflow & will increase machine time & cost, so we end up with this.**
http://cdn1.bigcommerce.com/n-yp39j5/zad02/products/176/images/1013/Enertion-VESC-1__31096.1475734962.1000.1000.JPG?c=2
http://cdn1.bigcommerce.com/n-yp39j5/zad02/products/176/images/1012/Enertion-VESC-2__19548.1475734962.1000.1000.JPG?c=2
https://www.instagram.com/p/BLXi08tA-KA/?taken-by=enertionboards




----------

----------

## Production Schedule & Pricing

##[BUY NOW & SAVE](http://www.enertionboards.com/electric-skateboard-parts/vesc-x-motor-controller/)

We are offering the VESC-X for sale right now for just $169USD for pre-orders, The price is discounted only during the production phase and will eventually settle at $199 once the production cycle has been finished & we have ample stock. 

**By early Novemeber 2016 we plan to have an early batch of units sent out to selected BETA testers from this forum for review.** _Note: we will do the beta tester selction so please don't email us_

**By late November 2016 we will have the first batch of 200 VESC-X ready to ship to early bird pre-order customers**

> To get the ball rolling we have created a further discount off the already discounted price of $169USD
> **THIS CODE CAN ONLY BE USED 20 TIMES - ENTER DURING CHECKOUT**
>
<img src="/uploads/db1493/original/3X/b/9/b9719f347a61e07dc668a9f1f20ddf8f7e991ec5.png" width="508" height="422">
> ##  VESCX$20OFF 
> _(approx $15usd discount)_
>



##[ORDER NOW & SAVE](http://www.enertionboards.com/electric-skateboard-parts/vesc-x-motor-controller/)

<img src="/uploads/db1493/original/3X/2/b/2be17e41e2ee81fe305b806c620f29e0fb79979f.png" width="445" height="500">





----------


----------


## AFFILIATE REWARD SYSTEM

**I’ll explain this in more detail in another thread, however here is a brief summary.**

The VESC-X is the first ever VESC version sold that will directly generate donations for Benjamin Vedder’s ongoing developments with VESC 6 & beyond. As of tomorrow, Ben can register to become an affiliate and refer people who are interested in purchasing the VESC-X. When the product is purchased via his referral link he will make a commission of $20AUD ($15USD) on each VESC-X purchase made.
```

---
## \#2 Posted by: rpn314 Posted at: 2016-10-14T06:37:05.360Z Reads: 1180

```
Looks great! A solid middle ground between the current 4.12 and the much anticipated VESC 6
```

---
## \#3 Posted by: Photorph Posted at: 2016-10-14T07:01:57.167Z Reads: 1170

```
I applaud the work you have done. Everything looks fantastic.

But what will happen when the VESC 6 is released?  There is no certain release date yet, but it may be here earlier than we expect.  Also why do you say it won't be released under the same CC license, I think Vedder will always keep this an open source project.

Edit: curious to know, who are the beta testers??
```

---
## \#4 Posted by: lox897 Posted at: 2016-10-14T07:03:37.340Z Reads: 1100

```
Bloody nice job Jason! If these prove to have no issues I'll definitely be ordering some! Will they have 1 year warranty no questions asked? @onloop
```

---
## \#5 Posted by: furryfrog Posted at: 2016-10-14T07:14:06.472Z Reads: 1025

```
Nice! looking forward to the results from the testing, and to see the capabilities of this improved version.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2016-10-14T07:19:59.818Z Reads: 982

```
looking good!
BUT the price! I see there are more components build in and a case and whatnot but on the other hand you said that this version is much better and faster to produce even in a bigger mass. So shouldn´t that drop the price a bit?
```

---
## \#7 Posted by: onloop Posted at: 2016-10-14T08:09:54.080Z Reads: 942

```
[quote="Photorph, post:3, topic:11102"]
But what will happen when the VESC 6 is released?
[/quote]

The VESC 6, if it is released as open source, will be a much higher price. So the VESC-X will be the alternative for those who don't need the costly extra features. There will be many people who don't want or need the integrated RF module which will add a substantial cost to the BOM
```

---
## \#8 Posted by: onloop Posted at: 2016-10-14T08:11:11.804Z Reads: 903

```
[quote="furryfrog, post:5, topic:11102"]
Nice! looking forward to the results from the testing
[/quote]

we already have fantastic test results, however, it will be good to get independent testers to give some feedback too.
```

---
## \#9 Posted by: Maxid Posted at: 2016-10-14T08:14:42.748Z Reads: 869

```
What does "fantastic" mean? Higher FOC reliability or just less heat under similar circumstances than v4?

Also what is a "substantial" cost increase in actual numbers? If it is 5 bucks it would still be substantial but well worth it for the added benefit. If it actually doubles the cost then that is a different story.
```

---
## \#10 Posted by: onloop Posted at: 2016-10-14T08:16:38.605Z Reads: 865

```
[quote="TarzanHBK, post:6, topic:11102, full:true"]
looking good!BUT the price! I see there are more components build in and a case and whatnot but on the other hand you said that this version is much better and faster to produce even in a bigger mass. So shouldn´t that drop the price a bit?
[/quote]

The upgraded components make the VESC-X more expensive, Plus the cost increases are also related to increased man hours due to two testing stages, but i assure you it is worth it. We have done everything possible to make the price low & maintain the best possible quality, improve reliability and make the product better.....
```

---
## \#11 Posted by: IDVert3X Posted at: 2016-10-14T08:28:37.886Z Reads: 828

```
400$ for ESCs ( dual motor setup ) is just too much imo.

Maybe you could design a version, that can drive two motors, so not all the components have to be doubled, which would result in lower price.
```

---
## \#12 Posted by: TarzanHBK Posted at: 2016-10-14T08:31:58.387Z Reads: 789

```
i hope one day will be the release-of-compact-dual-drive-vesc-day!
```

---
## \#14 Posted by: webst Posted at: 2016-10-14T08:49:03.465Z Reads: 782

```
Motors work independently and can be in different phases of rotation at any moment, that's why you cannot use single controller. It's like trying to see in 3d with one eye only.
```

---
## \#15 Posted by: webst Posted at: 2016-10-14T08:51:36.045Z Reads: 776

```
Will VESC-X support sensored motors?
```

---
## \#16 Posted by: Sion Posted at: 2016-10-14T08:56:29.706Z Reads: 801

```
[quote="onloop, post:1, topic:11102"]
The CC License

We are communicating to Benjamin vedder about our intentions and happy to abide by his terms in accordance with the CC license. We are willing to discuss this matter publicly & share our ideas openly. 

The VESC-X design was based on open source schematic to ensure the firmware would be compatible. We will provide the VESC-X schematic in a downloadable format from our website. http://www.enertionboards.com/how-to-build-eboard/vesc-x-files/ 


There have been no software or firmware changes made.
The original source files and libraries provided by Benjamin Vedder were not used. 
The VESC-X Hardware uses an unmodified open source Firmware.
[/quote]


Only the Schematics as a pdf are not the design files. I think you must upload the Altium files and the Gerbers to be CC license compatible.
I am not sure, but I think it is also not allowed by the CC license to be forced to create an account to download the files.
```

---
## \#17 Posted by: onloop Posted at: 2016-10-14T08:59:37.964Z Reads: 751

```
[quote="Maxid, post:9, topic:11102"]
What does "fantastic" mean?
[/quote]

YES, it supports sensored motors
```

---
## \#18 Posted by: dinodave Posted at: 2016-10-14T09:01:30.450Z Reads: 759

```
It's great to see you continuing to work to move this technology forward. Thanks for your efforts!

I noticed you mentioned software as a problem with the current VESC, that the current BLDC tool could be more user friendly. Are you working on something there? Just seemed a little odd to single that out then not announce anything.

Anyway I do agree the current software is fine for us hardcore enthusiast types for now :) keep up the good work, looking forward to seeing these in action.
```

---
## \#19 Posted by: Maxid Posted at: 2016-10-14T09:04:03.270Z Reads: 753

```
What has my quote to do with sensored motors?
```

---
## \#20 Posted by: onloop Posted at: 2016-10-14T09:05:55.636Z Reads: 785

```
[quote="Sion, post:16, topic:11102"]
Only the Schematics as a pdf are not the design files. I think you must upload the Altium files and the Gerbers to be CC license compatible.I am not sure, but I think it is also not allowed by the CC license to be forced to create an account to download the files.
[/quote]

The question has been raised with Ben Vedder, will abide by his instructions.

> forced to create an account to download the files.

you are not being forced to create an account. you can sign out as a guest.
```

---
## \#21 Posted by: onloop Posted at: 2016-10-14T09:07:47.269Z Reads: 751

```
somehow my response has been mixed up... lets try again
```

---
## \#22 Posted by: onloop Posted at: 2016-10-14T09:08:30.352Z Reads: 708

```
YES, it supports sensored motor
```

---
## \#23 Posted by: onloop Posted at: 2016-10-14T09:09:01.602Z Reads: 707

```
[quote="Maxid, post:9, topic:11102"]
What does "fantastic" mean?
[/quote]

Higher current draw, less heat.
```

---
## \#24 Posted by: XIII Posted at: 2016-10-14T09:09:45.117Z Reads: 710

```
435 euro's is what I paid for my dual vesc's 4.12 :D so not really
```

---
## \#25 Posted by: onloop Posted at: 2016-10-14T09:13:58.833Z Reads: 730

```
[quote="IDVert3X, post:11, topic:11102"]
400$ for ESCs ( dual motor setup ) is just too much imo
[/quote]

I agree, $400 is high, so buy it now for just $322.61

<img src="/uploads/db1493/original/3X/a/3/a316917f0c692c65f911f70b77019c64ca18a562.png" width="672" height="499">
```

---
## \#26 Posted by: Lukas Posted at: 2016-10-14T09:20:14.000Z Reads: 680

```
@onloop
If we preorder from Europe, will it be sent to your European warehouse first or would there be customs?
```

---
## \#27 Posted by: onloop Posted at: 2016-10-14T09:25:23.242Z Reads: 675

```
The first 200 at least will be from USA warehouse. 

Unless you EU guys organize a group buy of min 20pcs. Then it's 100% duty free guaranteed.
```

---
## \#28 Posted by: IDVert3X Posted at: 2016-10-14T09:45:08.062Z Reads: 680

```
320 usd is a fair price, but I'm scared of buying product that has not been tested over time. Your VESCs are known as not the best ( pretty much everyone recommends VESC from chaka instead ), so I would rather wait, I'm going to build my project in early 2017 anyway.
```

---
## \#29 Posted by: onloop Posted at: 2016-10-14T09:47:14.202Z Reads: 669

```
[quote="TarzanHBK, post:12, topic:11102, full:true"]
i hope one day will be the release-of-compact-dual-drive-vesc-day!
[/quote]

i don't think this will happen, as you need a way to swap parts quickly & cheaply, if one motor controller dies you need to swap two out for twice the cost.
```

---
## \#30 Posted by: webst Posted at: 2016-10-14T09:48:33.775Z Reads: 654

```
Problem with VESC-X is that it's almost the same price as your other offer:
http://www.enertionboards.com/electric-skateboard-parts/vesc-190kv-electric-skateboard-motor-bundle-sale/ 
I don't know how problematic is your previous VESC but this deal looks much better overall unless this is true:
http://vedder.se/forums/viewtopic.php?f=7&t=408
Please elaborate on this accusations. Is it even possible that you shipped that faulty product? Even if, is it possible that you would act like that with warranty?
```

---
## \#31 Posted by: IDVert3X Posted at: 2016-10-14T09:49:03.525Z Reads: 636

```
You can do two ESCs on a single board sharing some components, like the CPU, which would result in a smaller footprint and lower price.
```

---
## \#33 Posted by: webst Posted at: 2016-10-14T09:56:22.425Z Reads: 631

```
This makes sense when product is mature. Now the risk of burning one and ending up with both dead would be too much. I'd risk it if somebody would guarantee that his ESC is properly proofed for every possible scenario. Wrong polarity? No problem. Large voltage spike? Same. Check this link to know what I'm talking about:

http://www.rugged-circuits.com/10-ways-to-destroy-an-arduino/

We're not there with VESC yet I suppose.
```

---
## \#34 Posted by: onloop Posted at: 2016-10-14T10:00:52.718Z Reads: 615

```
[quote="webst, post:30, topic:11102"]
Please elaborate on this accusations. Is it even possible that you shipped that faulty product? Even if, is it possible that you would act like that with warranty?
[/quote]

The product that was shipped had an obvious manufacturing fault we are sorting him out under the terms of our warranty. No problem really. Of course, the guy is pissed off & so he should be.

The worker who assembled that batch lost his job too. That mistake is unacceptable. sometimes shit happens & that's is why we have a warranty.

Actually, this is one of the main reasons we are introducing two stages of testing. It will prevent the stupids mistakes from tired workers.
```

---
## \#35 Posted by: Maxid Posted at: 2016-10-14T10:02:22.624Z Reads: 595

```
Higher current-draw and less heat will not persuade me into buying this. The benefit I'd need to have to justify an order would be higher FOC reliability. If that is not the case the v4 is already good enough. Who uses "all the current" anyway? You are even limiting the Space cell to 40amps as far as I know with a fuse. That is well below the VESC v4 rated at continous 50A.

I am happy with my two v4.12 VESCs from you for my Jacob Hubs :thumbsup:
```

---
## \#37 Posted by: webst Posted at: 2016-10-14T10:11:30.028Z Reads: 588

```
This is exactly why my hand is more frequently hovering over this offer:

http://www.enertionboards.com/electric-skateboard-parts/vesc-190kv-electric-skateboard-motor-bundle-sale/

instead of VESC-X. I like VESC-X because of all the work that's been put into it, it finally looks like professional product, maybe some things I know about but never encountered in real life has been polished, but it's really hard to justify €250 more for set of two (when you add motors). Not to mention lack of 2 years warranty (something you get used to living in EU).
```

---
## \#38 Posted by: onloop Posted at: 2016-10-14T10:22:04.067Z Reads: 576

```
[quote="Maxid, post:35, topic:11102"]
If that is not the case the v4 is already good enough. Who uses "all the current" anyway? You are even limiting the Space cell to 40amps as far as I know
[/quote]

hubs motors need more current to generate torque, they also run hotter, especially if they are big hubs... so we need a vesc that can handle it.

and what makes you think our batteries will always have a 40A fuse... maybe the next version won't :wink:
```

---
## \#39 Posted by: onloop Posted at: 2016-10-14T10:22:40.852Z Reads: 555

```
that is a one time deal & it's about to end.... so make your decision soon.
```

---
## \#40 Posted by: Sion Posted at: 2016-10-14T10:31:23.331Z Reads: 589

```
[quote="onloop, post:10, topic:11102"]
The upgraded components make the VESC-X more expensive, Plus the cost increases are also related to increased man hours due to two testing stages, but i assure you it is worth it. We have done everything possible to make the price low & maintain the best possible quality, improve reliability and make the product better.....
[/quote]
A first view looks more like it should be equally expensive or maybe less expensive. (Sure the case is expensive, but I wouldn't count this to the "upgraded BOM components".
The only more expensive part are the MOSFETS. 3,68€ (IRF7749) to 3,30€ (IRFS7530) for one FET. With the higher quantity the differences get lower.
You are saving a lot of money using a lot less capacitors. Like going from 15u100V to 4.7u100V, 2 63V Elkos instead of 3 Elkos and more capacitor "downgrade".

To the two testing stages. When they are as good as your old "spin up testings" which don't be executed like you can read here: [http://vedder.se/forums/viewtopic.php?f=7&t=408](http://vedder.se/forums/viewtopic.php?f=7&t=408) that brings nothing. 
But I think you will find enough people here which buy your new VESC-X and then see that they have major quality problems. Good luck. Then they can buy your warranty to get a new one. :smile:
[quote="onloop, post:20, topic:11102"]
The question has been raised with Ben Vedder, will abide by his instructions.
[/quote]
You expected chaka to upload his "upgraded components" but you are not willed to upload at least your BOM (to see the "upgrade") or the layout? Very contradictory.
[quote="onloop, post:20, topic:11102"]
you are not being forced to create an account. you can sign out as a guest.
[/quote]
Good to know. Thanks.
```

---
## \#41 Posted by: 2-alex-2 Posted at: 2016-10-14T10:35:51.967Z Reads: 552

```
I want to pre order one but I disagree with your warranty procedures and what make it worse is its a brand new item with probably limited testing. Vesc 4.12 has been out for a while now and still getting some small issues but this brand new vescx should be better but just not with out warranty to back the consumer for if there is any issues creep up with manufacturing or design issue. Wouldn't want to miss the deal and have to pay full whack either so is there not going to be any support for first batch buyers.
```

---
## \#42 Posted by: rmrf Posted at: 2016-10-14T10:53:39.934Z Reads: 554

```
Thank you for trying to download the files and pointing out they are not source files. And thank you for analysis of components and a link to **xlv** thread. Your post is more informative than this whole topic.
```

---
## \#44 Posted by: onloop Posted at: 2016-10-14T11:09:11.288Z Reads: 564

```
[quote="2-alex-2, post:41, topic:11102"]
with out warranty to back the consumer for if there is any issues creep up with manufacturing or design issue
[/quote]

The vesc-x has a 60 day limited warranty included. It covers manufacturer faults, which should be easily identified on receipt of the product. After two stages of testing we expect near zero DOA.

You also have a choice to purchase an instant replacement warranty. This is only $39USD. You get up to two replacements of VESC-X no matter what the fault is.
```

---
## \#45 Posted by: 2-alex-2 Posted at: 2016-10-14T11:47:27.374Z Reads: 529

```
Yea still don't think that is enough 60 days. And to pay for extra warranty that the bit I really don't agree with. You are now fairly settled business now and should offer a better warranty. There are people on this forum who sell vesc that off free warranty even if it was a user issue. Will contemplate it but think will probably wait for someone els to produce them with better warranty for probably same amount.
```

---
## \#46 Posted by: onloop Posted at: 2016-10-14T11:54:10.757Z Reads: 535

```
[quote="2-alex-2, post:45, topic:11102"]
Yea still don't think that is enough 60 days. And to pay for extra warranty that the bit I really don't agree with. You are now fairly settled business now and should offer a better warranty.
[/quote]

the decision is based on market research, see here: http://www.electric-skateboard.builders/t/vesc-faq-low-prices-vs-quality-service-user-poll/1652

The majority of people want lower price & less warranty, please understand that everything has a cost. The longer warranty has a cost, especially when you have a product that will be used in many experimental setups that we have no control over. People can literally destroy the VESC by changing the firmware settings incorrectly.....

So we have decided to offer the premium warranty for the minority & the lowest prices possible for the majority
```

---
## \#47 Posted by: onloop Posted at: 2016-10-14T11:57:40.181Z Reads: 512

```
.............
## Only 18 uses of the discount code now available
```

---
## \#48 Posted by: TarzanHBK Posted at: 2016-10-14T12:24:22.336Z Reads: 518

```
would be good to see other companies or even countries to use a 2 year warranty with all their stuff they´re selling, like we are use to here in the EU!
Lots of peops thinking about buying the vesc over an standart esc, we should get to a point where the price difference is insufficient. (which it is with the higher rated 12s esc i know).
But on the other hand, a bulletproof vesc, where people could put in strange numbers in the bldc tool and only getting a error instead of an blown DRV.

To summerize: It should be possible to produce a not so expensive, good to produce and really reliable vesc.
maybe in 2 years?! :monkey:
```

---
## \#49 Posted by: Pantologist Posted at: 2016-10-14T12:33:29.752Z Reads: 506

```
It's really not possible. There are just too many things that can go wrong especially if the person doesn't know what they are doing.
```

---
## \#50 Posted by: Maxid Posted at: 2016-10-14T12:47:43.481Z Reads: 524

```
[quote="TarzanHBK, post:48, topic:11102, full:true"]
would be good to see other companies or even countries to use a 2 year warranty with all their stuff they´re selling, like we are use to here in the EU!
[/quote]

Not sure why people keep on referring to this seemingly amazing warranty wonderland that is the EU. This is not the case. The 2 years guarantee is not meant to keep you from destroying a product by ensuring you get a new one. After only 6 months YOU are actually required to PROVE to the seller that the fault in the product already existed at the time of purchase. This is nearly impossible without expensive assessment by an expert. Everytime a seller gives you any form of refund or repair after those 6 months he does this purely out of goodwill and not because he is legally required to do so.

Explanation by the EU: http://europa.eu/youreurope/citizens/consumers/shopping/guarantees-returns/index_en.htm

This also means however that companies like esk8 (selling VESCs in Germany) are basically offering a 6 months no questions asked guarantee as they would have to prove to the buyer that the fault was NOT there from the beginning.
```

---
## \#51 Posted by: TarzanHBK Posted at: 2016-10-14T13:05:17.474Z Reads: 485

```
[quote="Maxid, post:50, topic:11102"]
offering a 6 months no questions asked guarantee
[/quote]


i know but thats great comparing to other countries isn´t it ? :slight_smile:

the point is to stand behind your product like esk8, chaka or others do and provide a great service if something is wrong!
```

---
## \#52 Posted by: SORRENTINO Posted at: 2016-10-14T13:49:22.934Z Reads: 466

```
Whats the constant amp rating on this esc?
```

---
## \#53 Posted by: jmasta Posted at: 2016-10-14T14:24:02.197Z Reads: 468

```
Will this be suitable for 12S @ 60A?
```

---
## \#54 Posted by: 2-alex-2 Posted at: 2016-10-14T15:18:45.046Z Reads: 467

```
I strongly believe that if the user is at fualt and no proof can be shown they yes more than in they're rights to refuse (I work in the cycle industry and this happens a lot). But more warranty for the newer unproven product as no one knows how this vesc will 6-12months time even if it's been correctly setup. And that's what's needed I think. Also a good detailed setup process as I built my 3D printer from scratch 3 years ago and have never needed to adjust any of the firmware since that original setup but then again the product had been tested for longer with lots or reworks. And I believe these new vesc won't be without their faults down the line.
```

---
## \#55 Posted by: IDVert3X Posted at: 2016-10-14T15:23:45.584Z Reads: 474

```
I live in Slovakia, Europe - warranty is pretty fair there both for the seller and the customer.
We have got 24 months warranty covering any issues excluding the ones caused by the user himself.
I have never had any problem and always got a replacement / free reprair / refund.
You just have to describe the problem in a detail, they will try to reproduce it and then fix it.
If they find out it was caused by the user ( for example mechanical damage etc. ), they will refuse to fix it.

It's really hard to provide warranty on something like VESC is.
Why? Because it's hard to find out if it was caused by the user or the unit itself.
It's quite easy with DOA products and seller should imediately replace it for free.
But if you are using something for let's say 12 months, settings are correct, runs stable and it fails for no reason, then you should have free repair / replacement.
```

---
## \#56 Posted by: 2-alex-2 Posted at: 2016-10-14T15:27:37.239Z Reads: 443

```
Yea that's all it needs is a 12month warranty subject to users setting and usage. For like myself I would research and research before running any firmware and then once setup take it for easy runs then return and check again. And yea if you successfully run a firmware for say 9 months and you have done nothing different then it's oviously a manufacturer issue or design.
```

---
## \#57 Posted by: evoheyax Posted at: 2016-10-14T15:33:44.654Z Reads: 449

```
It's basically impossible to prove whose fault it is when a vesc breaks (with out paying an expert more than the cost of a new vesc). So good luck getting your legally required warranties in the EU.

I finally found the cause of my first vesc failure, which was from the second enertion china batch. It was the infamous pin poking the positive wire between the caps and vesc. This occurred back in the beginning of the year, before this was a know problem, way before switching to the US factory.

@onloop, are these new ones made in the US? Glad to see you step up to the plate and deliver a better quality vesc.
```

---
## \#58 Posted by: rmrf Posted at: 2016-10-14T16:18:23.196Z Reads: 447

```
[quote="onloop, post:1, topic:11102"]
As of tomorrow, Ben can register to become an affiliate and refer people who are interested in purchasing the VESC-X
[/quote]
Just think for a second how impossible this is. No way he will do that. Instead it would be a good move to send him money automatically whether he registers or not, promotes you or not.
```

---
## \#59 Posted by: kovjanos Posted at: 2016-10-14T16:27:39.505Z Reads: 479

```
I'm not an expert in these but be careful: guarantee and warranty are different

Guarantee:

* EU defines minimal guarantee time-frames for some type of products, but not for all. Min is usually 1 year.
* Guarantee time-frame is defined by the seller, kind of voluntary offer (above the EU defined min. if applies). 
* Some sellers provide longer guarantee time for products for marketing reasons (e.g. 5y for cars). 
* Under the guarantee period the seller must prove that the product's failure came from a not-so-proper usage of the product caused by the buyer. 
* The product can have different guarantee time-frames for different parts of the product (like phone vs. battery). 
* Guarantee definitions could also move/rearrange responsibilities around wearing parts, maintenance required parts – in some cases even warranty is lost on these (e.g. you not change oil in your car periodically).

Warranty:

* Warranty is around the product liability, means the product has no hidden issues, and works as described. 
* Warranty period has two parts: in the first part the buyer is treated innocent..
* In the first part – usually 6 months – on complaints the seller has to prove that the buyer caused the failure - e.g. incorrect use. 
* In the rest of the full warranty period  – usually 2y – the buyer have to prove that the failure came from a hidden issue that was already in the product at the time of purchase. 
* Time-frames are defined by the law - for both new/used(refurbished) products and B-B/B-C/C-C deals. 
Covers all parts of the product.

Regarding the 6 months, 2 years and friends: 

* 6 months: this is usually the first period of warranty - the seller has to prove that the failure was caused the buyer. It covers all parts of the product.
* 2 years: this is usually the full period of the warranty. Some consumer goods, durables have 3y warranty period. Under the warranty period after the first “innocent buyer phase”, the buyer has to prove that the failure came from the product and the product had the source of the issue since it was purchased.
* 2-3-5 years: this is usually the voluntary guarantee. The seller agrees that issues will be covered unless the buyer caused the failure, this must be proven by the seller.

This even more complex based on how the product is sourced: 
 
* who buys it? - person or legal entity. e.g. does it requires CE so parts are well classified?
* from where? - outside of EU / EEC / EFTA / OECD...  All different European associations follow the EU regulations and also OECD country laws are quite similar.
* from whom? - person or legal entity? e.g. when you say EU warehouse - is it a single person or a company behind it?

Even if the seller is outside of EU, there are many cases when the EU or similar laws are enforced on the product and the deal.

R, J.
```

---
## \#60 Posted by: kovjanos Posted at: 2016-10-14T16:33:17.086Z Reads: 428

```
[quote="evoheyax, post:57, topic:11102"]
It's basically impossible to prove whose fault it is when a vesc breaks
[/quote]

Law defines, who is responsible - in the different phases of warranty and guarantee - to prove that the fault is by the other party. if it's not possible to prove than who can't prove is responsible to cover the issue. 
E.g. usually in the first 6 months the seller has to prove, if can't, seller must do repair / replace.

R, J.
```

---
## \#61 Posted by: guyguy Posted at: 2016-10-14T16:39:03.513Z Reads: 424

```
Since this does not look like an official Vedder product you may want to think about renaming this product or having Vedder give rights to his name being attached to this product. The VESC has a considerable amount of goodwill attached to it in this community and is a valuable trademark and calling it a VESC has already caused a lot of confusion as to Vedder's involvement in this product which can open you up to other issues as well.

Not trying to give you a hard time, just some advice that may save you trouble down the road since the more you invest marketing this now the more difficult it will be to rebrand later on.
```

---
## \#62 Posted by: evoheyax Posted at: 2016-10-14T16:53:54.659Z Reads: 425

```
Renaming it may cuase equal confusion. It runs the same software as the VESC, it's basically the same components as the VESC with a few upgrades and new FETs. Mostly new form factor and upgraded components. I think having VESC in the name is smart, some it is a VESC after all. Personally I think it should be called the VESC-V, since it's like the version 5 vedder is skipping.
```

---
## \#63 Posted by: guyguy Posted at: 2016-10-14T17:42:09.501Z Reads: 461

```
If I could name this product I'd name it S-ESC-X (Skateboard ESC-X) - super cheesy but a nod to Tesla and their Models S, 3 and X. 

I 100% agree with you that it's smart from strictly marketing and business standpoint to call this a VESC since by doing so he'll benefit from all the brand equity, goodwill and market understanding/knowledge of the VESC 4.12. I'm just saying he should either get Vedder's consent to call this a VESC (maybe he did, but from the context of the original post it doesn't seem to be the case) or call it something else; otherwise this becomes a bad decision in consideration of trademark infringement risks where he may be fined later on, be subject to deceptive practices, lose out on sunk cost marketing this as a VESC and then have to cover the expense of rebrand later on. 

When I'm talking about confusion, I'm speaking specifically in terms of brand confusion in the market (this is the only arena where trademarks exist) and not product quality or makeup. As to trademarks doesn't matter if two products are exactly the same; brand equity is brand equity, which is why you can sell two shoes of equal quality and the one with the Nike brand will sell for 2000% more. Another way to put this is say your company Rocket Boards started growing and you've earned yourself a great reputation on hollow-core completes. How would you feel if I then started selling a competing product called "Rocket Board-X by Evoheyax" and based it off your design -- I would be leveraging your marketing spend and reputation for myself. I'm also assuming you wouldn't want your name associated and I don't think it would be a good defense for me to say, hey I don't want the market to be confused about the underlying design and since it's based off of Evoheyax's Rocket Board (nice job btw) I'm going to name it after him.
```

---
## \#64 Posted by: E-Boarding Posted at: 2016-10-14T17:43:55.054Z Reads: 439

```
I do like the name VESC-V too, what stands this X for and what is the next version called VESC-XX?

I realy like your effort you put in the development of this new VESC and would really like to try them but about 330 Eur for a dual-setup for an untested product. Maybe I've to pay taxes...
And as the others mentioned before, you had serveral quality issues and manufactoring faults on the older VESCs and many people are not happy with your warranty and 2x40$ for platinum is not an option.
So for me the price and overal risk is too high, maybe in 2017 when this is tested,

And can you show me video of a dual-raptor that bombs a huge hill in FOC-mode serveral times without blowing DRV or other problems?
```

---
## \#65 Posted by: Blasto Posted at: 2016-10-14T18:12:43.607Z Reads: 434

```
[quote="E-Boarding, post:64, topic:11102"]
330 Eur for a dual-setup for an untested product.
[/quote]

[quote="onloop, post:1, topic:11102"]
Testing before shipping is critical to identify faults and has definitely lowered the number of faults that have occurred at the end users home. However overall we were not completely satisfied with this process alone as we felt we could further improve results by having another separate stage for spinning the motor.
[/quote]

[quote="onloop, post:1, topic:11102"]
The NEW 2nd stage test will run higher currents & do more intensive motor spin testing. Our goal is zero faults leaving the factory. We believe with the two-stage testing process we can achieve our target of zero faults shipped.
[/quote]



He has a 2 stage testing now, so even his manufacturing is being improved.

Great work!
```

---
## \#66 Posted by: E-Boarding Posted at: 2016-10-14T18:14:20.257Z Reads: 416

```
does he test FOC under high load? Seems not
```

---
## \#67 Posted by: JohnnyMeduse Posted at: 2016-10-14T18:15:20.160Z Reads: 417

```
http://www.electric-skateboard.builders/t/the-hubs-x-enertion-vesc-x-hummie-hubs-custom-10s4p-pack/11127?u=johnnymeduse

The fact is, I need to stop because the motor are Overheating before the VESC
```

---
## \#68 Posted by: kovjanos Posted at: 2016-10-14T18:38:48.378Z Reads: 427

```
[quote="onloop, post:1, topic:11102"]
The CC License

We are communicating to Benjamin vedder about our intentions and happy to abide by his terms in accordance with the CC license. We are willing to discuss this matter publicly & share our ideas openly. 
[/quote]

From the moment when Benjamin shared his work with the  Creative Commons Attribution-ShareAlike 4.0 International License, he gave the right to anyone to Adapt - remix, transform, and build - upon the material for any purpose, even commercially.


[quote="onloop, post:1, topic:11102"]
The VESC-X design was based on open source schematic to ensure the firmware would be compatible. We will provide the VESC-X schematic in a downloadable format from our website.
[/quote]
Will be there an update email for those who already downloaded the pack sent out when the non-PDF files are available?

R, J.
```

---
## \#69 Posted by: jmasta Posted at: 2016-10-14T18:41:53.831Z Reads: 407

```
@onloop Can you confirm if this will work with 12S voltage?  I'll buy one right now if it does.  Thanks!
```

---
## \#70 Posted by: Blasto Posted at: 2016-10-14T18:48:45.477Z Reads: 425

```
you are missing the share part, redistribute in any medium or format

meaning he could mail you a paper copie of the gerbers if you like. The format is paper and the medium is mail.

now he's sharing a pdf format of what was remixed, via his website. that conforms to the CC 4.0

<img src="/uploads/db1493/original/3X/2/4/2429f05ef16fad8d9dd8a817c004fdfdc8b7e129.png" width="559" height="181">
```

---
## \#71 Posted by: kovjanos Posted at: 2016-10-14T18:56:29.141Z Reads: 415

```
[quote="Blasto, post:70, topic:11102"]
you are missing the share part
[/quote]

You mean:
> ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

That's why I asked when the design files and BOM will be available as current files are only PDF...

R, J.
```

---
## \#72 Posted by: Blasto Posted at: 2016-10-14T18:59:05.258Z Reads: 404

```
Yes so someone can use the schematic of the VESC-X and remix it also. that's what the SareAlike is. Doesn't mean the format needs to be the same. Because it stays under the CC 4.0 license
```

---
## \#73 Posted by: kovjanos Posted at: 2016-10-14T19:02:52.709Z Reads: 400

```
[quote="Blasto, post:72, topic:11102"]
Doesn't mean the format needs to be the same.
[/quote]

Just try to prove the circuit and PCB designers work with PDF file format :laughing:

R, J.
```

---
## \#74 Posted by: Blasto Posted at: 2016-10-14T19:07:45.705Z Reads: 392

```
[quote="kovjanos, post:73, topic:11102"]
Just try to prove the circuit and PCB designers work with PDF file format
[/quote]

I don't understand what you mean? I work with altium on a almost daily basis, the pdf of the VESC-X is clearly sourced from altium. Now, there's no KIcad to Altium importer out there. So the designer of the VESC-X was probably using the pdf of the 4.12 as reference, starting from scratch.
```

---
## \#75 Posted by: rmrf Posted at: 2016-10-14T19:41:02.413Z Reads: 385

```
He means that @onloop did not share the source files and thus does not comply with the license. PDF is good, but if you want to create a new VESC-XY based on VESC-X, you have to do a lot of work. @onloop did this on purpose, to prevent others from doing say, I want just to take files, and manufacture PCBs on oshpark, and solder everything myself. I can't easily do this.
```

---
## \#76 Posted by: guyguy Posted at: 2016-10-14T20:09:07.880Z Reads: 398

```
A lot of people cite the creative commons licenses for hardware but it's not really applicable. The license is a copyright license which offers very little protection when it comes to software and no protection when it comes to hardware (normally you have to go the patent route for protection). The original intent of copyrights was to protect authorship and publication rights for books so these protections weren't ever really envisioned to protect objects like computer hardware. This is alluded to in their FAQ:

https://creativecommons.org/faq/#general-license-information
<img src="/uploads/db1493/original/3X/b/1/b113565e2e7257216c12de4d976c0f121200fc43.png" width="690" height="86"> 

Hardware can't be protected by copyright. Software can be, but it's easy to circumvent because functionality can't be copyrighted so, you can basically re-write a code and not be subject to copyright -- most likely have to go patent route to do anything. Onloop is only bound by the CC license insofar as it relates to work that is actually copyrightable, like the images or written materials that Vedder published. If it's just new hardware he's pushing out it doesn't really apply unless there's a patent.
```

---
## \#77 Posted by: kovjanos Posted at: 2016-10-14T20:12:37.300Z Reads: 375

```
What I'm saying is that PDF is not the standard file format of Altium.
Independently from where you start the work - from a paper document or importing the source files - and from the changes you apply - only conversion / transformation or changes like rerouting / BOM - you must share and distribute your contributions.
Altium format is not proprietary, so can't see how the fair use would prevent sharing design in the right format.

R, J.
```

---
## \#78 Posted by: kovjanos Posted at: 2016-10-14T20:14:11.261Z Reads: 382

```
[quote="guyguy, post:76, topic:11102"]
Onloop is only bound by the CC license insofar as it relates to work that is actually copyrightable
[/quote]

If he would be bound to those than he wouldn't complain on Chaka's BOM a few weeks ago.

R, J.
```

---
## \#79 Posted by: guyguy Posted at: 2016-10-14T20:19:22.868Z Reads: 380

```
lol right, not saying he's not hypocritical. 

I made this same point in the thread where he was going after Chaka.
```

---
## \#80 Posted by: JohnnyMeduse Posted at: 2016-10-14T20:24:30.063Z Reads: 381

```
Well, chaka did not share any of is information.... Not even is bom or is shematic... That was the point

Also as @Blasto said, you can reproduce de VESC-X, you just need to work for it.. all the information is available
```

---
## \#81 Posted by: kovjanos Posted at: 2016-10-14T20:25:34.487Z Reads: 387

```
I'm not sure if you are right with the statement that you can't apply copyright on software / hardware. - See Apple vs. Samsung :) 
The native file formats are also documents - like DOC or PDF - , just better to represent the content of it: circuits and PCB designs.  So the "protect authorship and publication rights" could apply.

R, J.
```

---
## \#82 Posted by: Pantologist Posted at: 2016-10-14T20:32:31.577Z Reads: 385

```
Chaka did not do a complete layout change that would require a BOM change. He simply had suggestions for upgraded components that he sent to Vedder. 

This is a complete PCB layout change and should have a BOM to show the newly designed layout of the similar and upgraded Vesc components.
```

---
## \#83 Posted by: guyguy Posted at: 2016-10-14T20:33:20.790Z Reads: 389

```
Those were patents infringement suits, not copyright. 

I do this for a living :)
```

---
## \#84 Posted by: JohnnyMeduse Posted at: 2016-10-14T20:34:56.912Z Reads: 388

```
Fyi.. Chaka did a complete bom change... He just the same layout and He just did not share is work.
```

---
## \#85 Posted by: Pantologist Posted at: 2016-10-14T20:40:44.298Z Reads: 372

```
Do you know what he changed? Because it looks identical to the original BOM.
```

---
## \#86 Posted by: onloop Posted at: 2016-10-14T21:31:38.962Z Reads: 385

```
[quote="guyguy, post:79, topic:11102"]
lol right, not saying he's not hypocritical.
I made this same point in the thread where he was going after Chaka.
[/quote]

I agree that thread got pretty messy. But it really didn't have to.

The point is chaka made claims (and so did many others) that his vesc was better due to upgrading parts. The claim was that the upgraded parts improved the vesc reliability and reduced the chance of drv errors. 

The reason I was "going after" him is he should have done the community the kind gesture to explain what parts he changed. Everyone wants a better vesc and he was keeping the changes secret for commercial gain.

Still to this date he has not published his BOM. All he said was read vedder forum to find the answers.... so we did exactly that. It made it harder but such is life. 

Now I have made a new product, I have made all the same changes as chacka and a few more very significant upgrades, I have also provided clear pictures of the changes, I have explained the changes in detail (without anyone  needing to "go after me") and I have published schematics for anyone who is interested.

But somehow I am still hypocritical? I really don't understand the logic. It's very biased.

All I want is to make better esk8's - leave the politics at the door.
```

---
## \#87 Posted by: kovjanos Posted at: 2016-10-14T21:37:02.663Z Reads: 370

```
[quote="onloop, post:86, topic:11102"]
All I want is to make better esk8's
[/quote]

Thanks for all your efforts!
Could you please then share the Altium file(s)?

R, J.
```

---
## \#88 Posted by: xxlv Posted at: 2016-10-14T21:41:36.460Z Reads: 366

```
I think the people here complaining about the fact that you are "only" publishing PDF files instead of the original Altium files. I think for the correct spirit of open source it would be nice if you'd published everything, but i personally can understand why you didn't. You do want to make better esk8, but you want to sell them and not be made by others. You spent many hours of work in your new layout and want to protect it. Just look how many hours Benjamin put into that project, without him.. what would you have? :slight_smile:
 
However, since i run a VESC-repair business, i'm very interested in your source files (like your altium files) because the repair is much easier off navigatable Layout files rather than using some JPG/PDF files. I'd very much appreciate if you publish it.
```

---
## \#89 Posted by: onloop Posted at: 2016-10-14T21:44:05.779Z Reads: 353

```
Waiting to hear instruction from vedder. Its Possible after vesc v6 is released we will do it. But really don't want to derail vedder vesc6 developments. 

The schematics are available now so you can see what we did.
```

---
## \#90 Posted by: kovjanos Posted at: 2016-10-14T21:50:17.252Z Reads: 354

```
[quote="onloop, post:89, topic:11102"]
Waiting to hear instruction from vedder.
[/quote]

What type of instructions? 
Are there any components from VESC that are not under CC BY-SA 4.0?
I thought - as how it is advertised - that VESC is fully open source. If it is, then can't see why would you have to wait sharing the content...

R, J.
```

---
## \#91 Posted by: Kaly Posted at: 2016-10-14T21:59:15.984Z Reads: 340

```
@onloop great man, to see you push the envelope once more.
```

---
## \#92 Posted by: onloop Posted at: 2016-10-14T22:09:07.910Z Reads: 348

```
[quote="kovjanos, post:90, topic:11102"]
then can't see why would you have to wait sharing the content...
[/quote]

because it's polite.... & because it's not required

Vedder doesn't necessarily want everyone's modified VESC hardware designs being made public right now, especially when he is looking to release the next major hardware change himself in the near future. It's a potential conflict and therefore we will wait.
```

---
## \#93 Posted by: kovjanos Posted at: 2016-10-14T22:23:20.886Z Reads: 371

```
[quote="onloop, post:92, topic:11102"]
because it's polite
[/quote]

Sure - I would even do this for the reputation. There are not too many out there contributing on this level.

[quote="onloop, post:92, topic:11102"]
because it's not required
[/quote]
You mean: sharing the changes? 
If yes, I just would like to point you to the very simple description of the CC BY-SA 4.0:
> If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

If not, could you please elaborate? 

[quote="onloop, post:92, topic:11102"]
It's a potential conflict
[/quote]
There are different VESC versions on the market - I couldn't think on better description on VESC-X what you made in this thread's OP. Plus you already started selling (pre-order) it, so on this level it's already making newbies (not reading these details) confused!
...but how would the source files make conflict? - those are not consumed by users who are not aware of what VESC is on this level.

The only conflict would be around the name itself - VESC - but I didn't find anything that would imply there there is a copyright / trademark on the name.

R, J.
```

---
## \#94 Posted by: Sion Posted at: 2016-10-14T22:28:47.466Z Reads: 377

```
[quote="onloop, post:1, topic:11102"]

I’ll explain this in more detail in another thread, however here is a brief summary.

The VESC-X is the first ever VESC version sold that will directly generate donations for Benjamin Vedder’s ongoing developments with VESC 6 & beyond. As of tomorrow, Ben can register to become an affiliate and refer people who are interested in purchasing the VESC-X. When the product is purchased via his referral link he will make a commission of $20AUD ($15USD) on each VESC-X purchase made.
[/quote]

@onloop I can understand that you will not say anything to my last post because it will maybe reflect badly to your VESC-X.
But I can not understand why we need to order over a special link to support Benjamins work. Why not sending him the money for every order? You generated a lot of money from his work and it would be fair to spend money for every single order like chaka did. I think that is a clear point that you are just profit oriented and not "make better esk8`s" like you always claim.
```

---
## \#95 Posted by: guyguy Posted at: 2016-10-14T22:30:01.931Z Reads: 366

```
I'm not saying you _are_ hypocritical either, I was only saying that I wasn't saying you're not hypocritical :wink:. Joking aside I apologies, hypocritical was not the correct word to use there and it's not my intent to cause drama. I think people were taking my comments on the non-relevance copyright/CC license as defending your your file format choice and I wasn't (I'm not qualified to have an opinion on that) so I was trying to distance myself from that separate issue. 

As for bias, I admire your work and everything you've done for the community - so, yes, I'm bias, only a little though.
```

---
## \#97 Posted by: onloop Posted at: 2016-10-14T23:28:10.198Z Reads: 370

```

**The referral program has started, sign up now & earn cash to help us promote the new VESC-X**

http://www.electric-skateboard.builders/t/get-paid-15-help-promote-the-new-improved-vesc-x/11154
```

---
## \#99 Posted by: torqueboards Posted at: 2016-10-14T23:44:10.977Z Reads: 367

```
Nice job Congrats! I like the innovation.
```

---
## \#100 Posted by: ArmandR Posted at: 2016-10-15T00:35:29.175Z Reads: 366

```
Will the new raptors have the VESC-X?
```

---
## \#101 Posted by: onloop Posted at: 2016-10-15T00:46:18.662Z Reads: 366

```
Eventually when the stock is available we will be using vesc-x  in all our pre built products.
```

---
## \#102 Posted by: jmasta Posted at: 2016-10-15T01:49:52.857Z Reads: 375

```
Is the VESC-X compatible with 12S?
```

---
## \#103 Posted by: Photorph Posted at: 2016-10-15T02:23:21.204Z Reads: 376

```
yea why not?? Even the previous VESC was.  I ran it on 12s at 30+ mph near the ERPM limit.  No issues.
```

---
## \#104 Posted by: jmasta Posted at: 2016-10-15T03:17:43.435Z Reads: 382

```
I only ask because on Enertion's site, the VESC is listed at 10S max, but other suppliers spec it to 12S.  This could just be a conservative value, or they could have optimized the component selection for 10S max in their build of the VESC
```

---
## \#105 Posted by: chuttney1 Posted at: 2016-10-15T04:06:23.370Z Reads: 381

```
Actually, running on 12S is half-reliable because it would result in a broken DRV8302 chip when it happens. Vedder design the VESC to have a max voltage of 60V and 60 amps. There's no one stopping you from doing so, but only the advice of picking which buyer should you choose to return a broken product for repairs.
```

---
## \#106 Posted by: Photorph Posted at: 2016-10-15T06:11:18.019Z Reads: 384

```
[quote="chuttney1, post:105, topic:11102"]
Vedder design the VESC to have a max voltage of 60V
[/quote]

So 12s should be safely below that?
```

---
## \#111 Posted by: guyguy Posted at: 2016-10-15T13:59:54.722Z Reads: 375

```
@onloop are there any manufacturing differences between the run coming out 11/10 and the vesc-x your beta testers have gotten? 

I'm wondering if those great results are coming from vescs built off of your scaled production line or if those betas were a small batch production. Would give me a better idea of what they're evaluating. 

Thanks!
```

---
## \#113 Posted by: Chicagojoshua Posted at: 2016-10-15T20:08:42.149Z Reads: 363

```
Whoa!!! WAY OUT OF PRICE RANGE!!! For the price of one vesc I can get two 4.12 Vesc plus a remote on Ali express! The real market price should have been 100 USD. Good luck with those crazy out lf equilibrium prices
```

---
## \#114 Posted by: Pantologist Posted at: 2016-10-15T20:46:24.439Z Reads: 362

```
Well... if it actually is a lot more reliable, I'd buy it. For now, I'm just going to sit and wait. 

Vesc 6 will probably be around the same price.
```

---
## \#115 Posted by: onloop Posted at: 2016-10-15T21:27:05.417Z Reads: 370

```
The vesc on aliexpress are made using components sourced from the Chinese electronics market. They will never be able to guarantee they are using genuine parts as specified by vedders BOM. I know because I used to make vesc in China and they need various parts to be imported. They certainly will not be using the upgraded high tolerance parts we are now using. there is no point making vesc with cheap parts they just don't stand up to the levels the majority of esk8 builders need.

If you are on a tight budget you can buy the old 4.12 version now for $89usd. It's made using genuine parts from BOM. It's made in the US. Tested before shipping & is in stock. http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/
```

---
## \#116 Posted by: Chicagojoshua Posted at: 2016-10-15T21:47:51.670Z Reads: 359

```
I get what your saying but I have yet to have issues with the Vescs I bought from Ali Express. Perhaps if your were to drop the price of the 4.12 to $80 and charge $115 for the new one and provide free shipping you would corner the USA Vesc market. The whole idea is to wipe out your VESC competitors. But what do I know, I am only simple business man with three successful startups.
```

---
## \#117 Posted by: Pantologist Posted at: 2016-10-15T21:51:20.424Z Reads: 358

```
Why would he have to drop the price of the old vesc even more? It is already priced competitively.

The new Vesc x will probably lower in price after awhile and much more after the vesc 6 releases. Besides he setup a way for people to get $15 through referrals.
```

---
## \#118 Posted by: DeathCookies Posted at: 2016-10-15T21:53:19.256Z Reads: 358

```
When do you think that our both comments will be flagged and deleted like @Hummie ? :D
It is nearly the same production as a normal VESC just with a BIG X ("name/brand/price") for a little difference in layout and some minor improved parts.....
```

---
## \#119 Posted by: whitepony Posted at: 2016-10-15T22:07:11.397Z Reads: 366

```
[quote="DeathCookies, post:118, topic:11102"]
When do you think that our both comments will be flagged and deleted like @Hummie ? :smiley:It is nearly the same production as a normal VESC just with a BIG X ("name/brand/price") for a little difference in layout and some minor improved parts.....
[/quote]

as much as I wonder about the product in the light of the upcoming vesc 6, its still a pretty neat work and many really useful changes. most of all I like the cooling/enclosure, the integrated caps and the form factor, which allows 2 vescs next to each other to have the typical width of an 18650 battery.
```

---
## \#120 Posted by: Pantologist Posted at: 2016-10-15T22:10:07.653Z Reads: 361

```
My comment about the referral program already got deleted....

I think @onloop did a great job. The minor improvements look promising. The direct FETs, heart sink and enclosure are just awesome.

I'll still be waiting for the Vesc 6. I'd rather wait for something completely new and specs my money on that.
```

---
## \#121 Posted by: guyguy Posted at: 2016-10-15T22:26:14.247Z Reads: 361

```
I just hope all these tweaks add up to a product with wider tolerances than 4.12, mainly around FOC and, more controversially, pairing it with larger larger motors that we usually see with mono drives -- don't really want to open that can of worms, just saying I'm waiting to buy this once I see a beta testers do a sustained hill climb (over .25 miles) with Raptor mono-drive (6372) with stock gearing, at top speed, with a 180lb + rider and not have vesc related issues. Even better if its in FOC.
```

---
## \#122 Posted by: onloop Posted at: 2016-10-15T22:33:20.330Z Reads: 353

```
This is not the place to discuss pricing structure or your success at business. Maybe you can create another thread about the science of price engineering. 

**Everyone please stay on topic or your posts will get flagged/removed.**
```

---
## \#123 Posted by: onloop Posted at: 2016-10-15T23:12:41.915Z Reads: 366

```
To help you all understand the rules of this thread (and forum)

**Examples of posts that may be flagged as off topic.**
1. Anything to do with cc license.
2. Anything to do with donations.
3. Anything that is abrasive, argumentative or offensive 
4. Anything that is related to other products or other vendors.
5. Anything that is about prices.
6. Defamation / unfounded accusations.

If you don't like seeing new innovations just don't look in this thread.


**Example of things that may be discussed openly.**
1. Engineering decisions.
2. BOM decisions / upgraded parts.
3. Design decisions.
4. Performance improvement. How/why
5. Why we made vesc-x.
6. Production methods, process.
7. Testing methods.
8. Beta testing and feedback.


Of course there are many more things that we can discuss. Just remember anyone (its not just moderators) on this forum can flag your post and if you get 3 flags your post is removed automatically. So please think before your post and try to be civil.
```

---
## \#124 Posted by: Hummie Posted at: 2016-10-15T23:55:03.379Z Reads: 354

```
I'm on ur side of whatever scuffle is going on. I empathize. Or for the rest of us who aren't I into dictionary nerdery sympathize.  It's a new age and the helm of the ship goes on the website. Talking as partially drunk. And a melodramatic.  Sentimental drink.  Please keep the forum free for everyone's crap and u will be revered and wealthy.
```

---
## \#125 Posted by: onloop Posted at: 2016-10-16T00:22:42.015Z Reads: 359

```
[quote="Hummie, post:124, topic:11102, full:true"]
I'm on ur side of whatever scuffle is going on. I empathize. Or for the rest of us who aren't I into dictionary nerdery sympathize.  It's a new age and the helm of the ship goes on the website. Talking as partially drunk. And a melodramatic.  Sentimental drink.  Please keep the forum free for everyone's crap and u will be revered and wealthy.
[/quote]

i am not sure exactly what you are saying hummie...  it seems my hummie-to-english translation app is not working. :slight_smile: 


_i think you are saying its a good idea to remove the off topic posts?_
```

---
## \#126 Posted by: Hummie Posted at: 2016-10-16T00:34:07.472Z Reads: 343

```
I think I'll just talk about my vacuum infusion.  

Whatever it is we are talking about.
```

---
## \#127 Posted by: Michaelinvegas Posted at: 2016-10-16T05:06:15.553Z Reads: 341

```
🍺🍻🍷🍸🍹🍾
.....
```

---
## \#128 Posted by: chinzw Posted at: 2016-10-16T05:37:49.388Z Reads: 358

```
[quote="onloop, post:115, topic:11102, full:true"]
they need various parts to be imported.
[/quote]

Wait what?
```

---
## \#129 Posted by: rmrf Posted at: 2016-10-16T06:52:50.721Z Reads: 369

```

http://imgur.com/1CAFALR
```

---
## \#130 Posted by: onloop Posted at: 2016-10-16T07:53:25.269Z Reads: 372

```
I can't tell if you are being a dick or have a really good sense of humour...

But I honestly like your post. It made me smile.. it's definitely off topic! but who gives a f when it's funny.

Seriously bro if you want to talk with me about this product and it's off-topic-related stuff just blast me via PM. It seems like you have some vested interest or something that you need to get off your chest.. Happy to chat about it.
```

---
## \#131 Posted by: E-Boarding Posted at: 2016-10-16T09:04:15.207Z Reads: 378

```
I'm not convinced by words, I need facts.

I might buy your new VESCs but before I do, I wan't a prove/guarantee that it's fully safe to run a dual-raptor-setup in FOC (under heavy load), I'm sure your team can test this easily.
```

---
## \#132 Posted by: Dedbny Posted at: 2016-10-16T09:55:04.251Z Reads: 357

```
Has the DVR chip been made more robust on these new Vecs as they seem to be the weak link to these things.
```

---
## \#133 Posted by: flatsp0t Posted at: 2016-10-16T12:11:31.822Z Reads: 368

```
There are already some guys who have it(Or at least a sample), who seem so be testing stuff like this in the moment.

@JohnnyMeduse is testing them with hubs:
http://www.electric-skateboard.builders/t/the-hubs-x-enertion-vesc-x-hummie-hubs-custom-10s4p-pack/11127/
```

---
## \#135 Posted by: onloop Posted at: 2016-10-16T14:19:15.775Z Reads: 356

```
The drv chip is the same chip. However the tolerances of the components surrounding it are upgraded over the normal vesc 4 BOM. 

We also added a tvs diode to protect the components from voltage spikes.
```

---
## \#136 Posted by: onloop Posted at: 2016-10-16T14:32:31.928Z Reads: 365

```
[quote="E-Boarding, post:131, topic:11102"]
I'm not convinced by words, I need facts
[/quote]

Other vendors have claimed that upgraded capacitors are the reason their vesc are more reliable. There is some clear evidence already that this is true and therefore being implemented in v6.

We are simply making the same changes plus adding a few other additional components that are designed to provide protection. Such as the tvs diode to stop voltage spikes.

We also separated the logic and power to minimise trace length and re postioning components to minimise noise. These are all known facts and it's why vedder is doing the changes in the same way on v6.

Everything we did was based on knowledge gained from evidence provided from vesc users across the globe.
```

---
## \#137 Posted by: rpn314 Posted at: 2016-10-16T14:56:45.767Z Reads: 361

```
https://thumbs.gfycat.com/CorruptFemaleCaterpillar-size_restricted.gif

Stay classy guys and gals. :slight_smile:
```

---
## \#139 Posted by: TheCheat Posted at: 2016-10-16T15:38:49.789Z Reads: 347

```
For any audiophiles here, this forum is turning into the e-skateboard equivalent of head-fi. Where constructive posts (meant to better the product or company) are being censored as a means to protect the company's interests. People here are bringing up legitimate concerns about the VESC-X and its development, only to get censored or shut down.
```

---
## \#140 Posted by: E-Boarding Posted at: 2016-10-16T16:17:46.934Z Reads: 344

```
I know and this is logical but it's just words, take your raptor go out and try hard to blow this fucking chip with r-specs. Because that's what I want to buy this VESC for and I don't want to waste my money. ;)
```

---
## \#141 Posted by: webst Posted at: 2016-10-16T16:31:47.894Z Reads: 338

```
Using both BLDC and FOC modes.
```

---
## \#142 Posted by: guyguy Posted at: 2016-10-16T16:48:59.204Z Reads: 348

```
[quote="onloop, post:123, topic:11102"]
Examples of posts that may be flagged as off topic.1. Anything to do with cc license.2. Anything to do with donations.
[/quote]

To better my understanding of the rules of this thread, whyare those items off topic? Both are of are subsections of your original post. I mean no offense in asking this question and I am grateful/impressed with your investments in pushing the community forward.
```

---
## \#143 Posted by: 2-alex-2 Posted at: 2016-10-16T17:05:45.289Z Reads: 350

```
[quote="onloop, post:136, topic:11102"]
Other vendors have claimed that upgraded capacitors are the reason their vesc are more reliable.
[/quote]

So why would we pay that different for a new untested component over say a v4.12 chaka made vesc with same upgraded components and proven pcb board. This is why I couldn't pay that extra as nothing to show its better. Would rather by Chaka vesc with the better warranty
```

---
## \#144 Posted by: Blasto Posted at: 2016-10-16T17:14:12.294Z Reads: 348

```
[quote="2-alex-2, post:143, topic:11102"]
new untested component
[/quote]

Untested by the masses true, but you can't expect to have hundres of reviews of a new product 3 days after it's launch.

The enclosure is the biggest feature here, even acts as a heatsink on a fet package that is designed to transfer it's heat the most efficient way.
```

---
## \#145 Posted by: 2-alex-2 Posted at: 2016-10-16T17:26:12.728Z Reads: 353

```
Yea the inclosure is good but I have a 3D printer and access to cnc which within a day or so could have something made to enclose a v4.12 . Yea I under stand beta testing as have been beta and alpha tester for computer game few years ago and yes you can't get huge amounts of reviews unless your willing to put the money into the testers. The more tester the better the result by seeing as this is still a small business there will be less money spent on testing compared to the larger companies. I do wish him all the best and hope that the launch goes well to encourage people to buy them but without the confidence in your own product to supply a 12 month warranty on manufacturing issues its hard to buy.
```

---
## \#146 Posted by: Blasto Posted at: 2016-10-16T17:41:16.588Z Reads: 359

```
The big problem with the 4.12 is that is was not designed with an enclosure in mind. While building my robots, i tried enclosing them, ended up either shorting the fets or the whole assembly became to bulky. (If you do a search with keyword "sumo" you'll find the threads)

It's totally respectable for one to wait and see how a product matures in to a tried, tested and reliable product. Other peep's will get their hands on one early on, beleive me they won't be dissapointed.

Personnaly i've been testing this thing for the last 3 months, tried all the revisions, haven't broke this one yet.
```

---
## \#147 Posted by: Blasto Posted at: 2016-10-16T18:00:13.989Z Reads: 373

```
Guess i can show these pictures now,

This is the first revision i received, my feedback was
"It's nice, but it's bulky, not easily mountable, no real advantages over the current 4.12"

<img src="/uploads/db1493/original/3X/3/4/34ac920ef93910de9f75b19e40eac7b020b4848b.jpeg" width="375" height="500">

My feedback was taken in to account, 3 revisions later, now you have the vesc-x
```

---
## \#148 Posted by: 2-alex-2 Posted at: 2016-10-16T18:27:41.700Z Reads: 369

```
Yea 4.12 was design to serve the needs at the time but people have developed and pushed the boundaries since. So things will need to change which is why people have developed 4.12 more to make it suitable within the designs but still limited. So then it's now been developed more to make v6 but doesn't mean the 4.12 can be pushed to the side as if configured correctly it's now a reliable vesc. Just we now need this new vesc to be tested with the mass if proven to work then brilliant I would buy. But bottom line is if you have tested something and you believe in the product you will support the people who buy from you and supply a warranty. Oviously were still working with people who don't understand the basics to coding and programming which is the key. If we can make a vesc that will work with majority of setups with basic setup then will be off and people will be happy to pay the extra. But for now we need the support from the seller to say yea we have tested and if configured right this product will work flawlessly.
```

---
## \#149 Posted by: akira Posted at: 2016-10-16T18:49:08.073Z Reads: 353

```
I would happily build one to test but the BOM and PCB files are not being made public ...
```

---
## \#150 Posted by: Kaly Posted at: 2016-10-16T22:38:01.114Z Reads: 354

```
Hello guys 
@onloop what are the overall dimensions  of the vesc-x ?
```

---
## \#151 Posted by: onloop Posted at: 2016-10-16T22:45:49.531Z Reads: 360

```
[quote="racidon, post:138, topic:11102"]
But I can't highlight how you don't honour your warranties? Thus your comment about a 60 day warranty isn't really correct?
[/quote]

When we do the installation of VESC into our own products we offer 12 months instant replacement warranties, raptor customers can attest to this. We will also have some new products coming soon that will have the VESC-X pre-installed inside, you will get 12 months warranty on those too.

If you decide to build your own esk8 and install the VESC & if it fails in 60 days you need to prove it was a manufacturing fault. If you have changed firmware settings or modified the VESC it voids the warranty.

If you cannot prove it was a manufacturing fault, or even if you destroyed the vesc from user error you can buy a Platinum warranty and we ship you a new VESC.
```

---
## \#152 Posted by: onloop Posted at: 2016-10-16T22:46:16.731Z Reads: 359

```

outside diemnsion 64mm X 64mm
```

---
## \#153 Posted by: onloop Posted at: 2016-10-16T23:02:29.130Z Reads: 378

```
## IT'S NOT CENSORSHIP

People can create a new thread to discuss any of the off-topic subjects, I just don't want this thread filling up with crap...

**I am all for open discuss, please just do it in the correct thread!**

**example;** 

_create a thread called_ "How much vendors should donate to Vedder"

_create a thread called_ "I am anti VESC-X & here is why"

_create a thread called_ "I am anti-innovation & here is why"

_create a thread called_ "Creative Commons License - Rules & Guidelines"

_create a thread called_ "VESC prices"

_create a thread called_ "VESC Vendors warranties & what is covered"

_create a thread called_ "I like to discredit everything enertion does because I have deep resentment & envy of their work"


**Please try to be reasonable & civil... & don't hijack threads with bullshit.**
```

---
## \#154 Posted by: ArmandR Posted at: 2016-10-16T23:03:06.444Z Reads: 364

```
[quote="onloop, post:151, topic:11102"]
some new products coming soon that will have the VESC-X pre-installed inside
[/quote]

How soon? Just wondering if I should lay off buying parts for my build and buy your "new" products.
```

---
## \#155 Posted by: lox897 Posted at: 2016-10-16T23:51:19.089Z Reads: 359

```
[quote="onloop, post:151, topic:11102"]
If you decide to build your own esk8 and install the VESC & if it fails in 60 days you need to prove it was a manufacturing fault. If you have changed firmware settings or modified the VESC it voids the warranty.
[/quote]

But aren't we supposed to change firmware settings? How should we prove it is a manufacturing fault? A video of setting it up? Thanks in advance.
```

---
## \#156 Posted by: JuniorPotato93 Posted at: 2016-10-17T00:00:22.561Z Reads: 354

```
[quote="onloop, post:151, topic:11102"]
If you have changed firmware settings or modified the VESC it voids the warranty.
[/quote]

Same question as @lox897, I'm genuinely confused on this one. If i purchase a VESC, whether it be the new VESC-X or a 4.12  and change the setting in the BLDC, like ERPM from 100,000 to 60,000 or change my battery cut offs to match the system I set up thats warrants voiding the warranty? Could you elaborate on this a little? 

you dont have to go into the modifying your hardware, that ones painfully obvious.
```

---
## \#157 Posted by: Kaly Posted at: 2016-10-17T00:00:25.387Z Reads: 338

```
What is the height?
```

---
## \#158 Posted by: chuttney1 Posted at: 2016-10-17T02:13:52.640Z Reads: 341

```
Im guessing no ask if Onloop will provide a version without the heatsink and case. Could drop the price by $40 I assume.
```

---
## \#159 Posted by: Blasto Posted at: 2016-10-17T02:17:27.075Z Reads: 354

```
[quote="Kaly, post:157, topic:11102, full:true"]
What is the height?
[/quote]

22mm high

These fets are designed to have a heatsink, i mean they must have a heatsink. @chuttney1
```

---
## \#161 Posted by: onloop Posted at: 2016-10-17T04:37:19.067Z Reads: 369

```
I understand you are frustrated, building electric skateboards can be tricky, that's why we offered you the option to have our technicians rebuild your board free of charge, you refused our offer. we can only do so much.

We also offer prebuilt boards that come with 12 months warranty. However we cannot offer warranty on your self made electric skateboard.

please stop posting off topic stuff.
```

---
## \#162 Posted by: onloop Posted at: 2016-10-17T04:40:00.445Z Reads: 374

```
Custom CNC Heat sinks being prepared.

<img src="/uploads/db1493/original/3X/d/8/d89042b555d4d361df81837c172bb1ff97b90e8a.jpg" width="617" height="499">
<img src="/uploads/db1493/original/3X/1/c/1cc6b3597cdec5faca8bdeec11d0ea8d3d473f59.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/8/d8afd613209810105912c290d13901887a5714f8.jpg" width="690" height="393">
```

---
## \#163 Posted by: AyyAyRon Posted at: 2016-10-17T04:42:26.198Z Reads: 359

```
So getting the warranty 1 year replacement warranty is good idea then
```

---
## \#165 Posted by: onloop Posted at: 2016-10-17T05:17:26.251Z Reads: 375

```
[quote="AyyAyRon, post:163, topic:11102, full:true"]
So getting the warranty 1-year replacement warranty is good idea then
[/quote]

Actually, most people don't buy the platinum warranty that we offer & most people "mathematically" don't need it. Failure rates are 2-3% 

I suppose it's like buying insurance for your car...... it's pretty costly especially if you never have a crash!!!
However, if you do crash you get a new car or repair done under insurance, so now you are glad that you have paid for insurance.

We offer the 1yr platinum warranty with vesc-x for just $39 at the time of purchase, this takes the total price to about $209USD.

The platinum warranty is good for up to 2 replacements in 1 yr. So if your luck is really bad & you suffer some accidents you basically get three vesc-x in the first year at a cost of just $69 each.

With our additional 2nd stage of testing using a motor with higher current there should be zero DOA. 

So it's your call. Maybe you plan to do some experimental stuff & will be changing the settings and messing around with different motors settings which can destroy a perfectly good vesc, so maybe the $39 is worth it.
```

---
## \#166 Posted by: OldAFGuy Posted at: 2016-10-17T16:46:09.062Z Reads: 370

```
Why are there no mounting holes???  In a custom machined enclosure it seems a crime not to include one single mounting hole.  

It clearly looks like this unit could be sealed and mounted without the fully enclosed VESC-X needing to be put into another enclosure.  Better cooling too.

Please consider sealing the unit with Silicone and mounting directly via mounting holes.

OldAFGuy
```

---
## \#167 Posted by: Blasto Posted at: 2016-10-17T16:47:49.830Z Reads: 357

```
[quote="OldAFGuy, post:166, topic:11102"]
Why are there no mounting holes
[/quote]

there are 4 blind holes at the back of the enclosure

@onloop should mention this, guess it got forgotten with all of this brouhaha
```

---
## \#168 Posted by: onloop Posted at: 2016-10-17T21:49:17.121Z Reads: 352

```
[quote="onloop, post:1, topic:11102"]
5. Place holder M3 holes for adding another heatsink for even more cooling power.
[/quote]

It got mentioned. I suppose the holes spacing dimensions wouldn't hurt... I'll work on updating the specs at enertion website.
```

---
## \#169 Posted by: xxlv Posted at: 2016-10-19T18:53:56.215Z Reads: 369

```
Do you think C102-107 (4.7µF 100V) will be sufficient as replacement for that more expensive C37 C51 (15uF, 100V) 810-CGA9P3X7S2A156M from the original VESC design?

Especially when using the VESC a high current, there will be short high current spikes which the big electrolytic Caps can't handle.
Whats your opinion on this?
```

---
## \#170 Posted by: onloop Posted at: 2016-10-21T00:22:40.147Z Reads: 366

```
These caps are physically placed at the source of the noise, across the fets. This will significantly reduce the propagation throughout the circuit. All decoupling caps, including electrolytic caps are stamped with a low ESR rating. Yes we believe it is sufficient.
```

---
## \#171 Posted by: Michaelinvegas Posted at: 2016-10-22T20:17:09.347Z Reads: 372

```
The Beta VESC-X has arrived 

----

Unboxing tonight 😉 - Video to follow 


<img src="/uploads/db1493/original/3X/4/6/46f412d12d8d1023ebfc11ee55bf98787b70b602.JPG" width="374" height="500">
```

---
## \#172 Posted by: guyguy Posted at: 2016-10-23T16:20:50.219Z Reads: 358

```
Nice, looking forward to seeing your vlog on it. :grinning:
```

---
## \#173 Posted by: Michaelinvegas Posted at: 2016-10-23T18:01:02.720Z Reads: 374

```
Here it is.... sorry I thought it uploaded last night...but seems there was an error....

Pardon the length (14 minutes of your life)....I wanted you guys to have a good look at it. 

Enjoy! 

https://youtu.be/2PS72Li29Jo


You know there are more videos to come
```

---
## \#174 Posted by: webst Posted at: 2016-10-23T20:58:21.246Z Reads: 365

```
You could easily cut first 7 minutes of this video where you just read the internet to people on the internet. To sum the rest, there are only two things worth noticing: 3d printed enclosure (7:52) and thermal tape on mosfets (11:10).
```

---
## \#175 Posted by: Michaelinvegas Posted at: 2016-10-23T21:27:34.917Z Reads: 362

```
Look forward to your version @webst
```

---
## \#176 Posted by: webst Posted at: 2016-10-23T21:52:07.332Z Reads: 352

```
Don't. I'm waiting for 6.0 or anything with proper vector control implementation. I did not mean no offense, I'm just not that good at talking politically correct which has it's good sides.
```

---
## \#177 Posted by: Pantologist Posted at: 2016-10-23T21:54:23.053Z Reads: 350

```
Are you referring to FOC?
```

---
## \#178 Posted by: webst Posted at: 2016-10-23T21:58:58.393Z Reads: 348

```
Yes, I am. If you want to say that VESC-X has it then I'd be positively surprised.
```

---
## \#179 Posted by: Blasto Posted at: 2016-10-23T22:02:05.835Z Reads: 365

```
Its been doing dam good so far!

http://www.electric-skateboard.builders/t/the-mule-i-mono-r-spec-big-boy-i-10s4p-i-zenit-freeride-deck-i-vesc-x-i-foc-enabled/11238?u=blasto
```

---
## \#180 Posted by: Pantologist Posted at: 2016-10-23T22:08:44.598Z Reads: 362

```
@JohnnyMeduse is also running FOC. No issues so far. 

http://www.electric-skateboard.builders/t/the-hubs-x-enertion-vesc-x-hummie-hubs-custom-10s4p-pack/11127

VESC 6.0 seems to be taking a long time. No doubt it is a huge overhaul, but I've been waiting since last Spring. :P
```

---
## \#181 Posted by: webst Posted at: 2016-10-23T22:31:23.416Z Reads: 358

```
Interesting. Do you guys use sensored motors?
```

---
## \#182 Posted by: Pantologist Posted at: 2016-10-23T22:44:12.400Z Reads: 360

```
Well Hummie Hubs are senorless hubs. @Blasto is using a RSPEC so it has no senors either. 

Sensorless FOC in both cases.
```

---
## \#183 Posted by: Michaelinvegas Posted at: 2016-10-24T02:32:56.512Z Reads: 370

```
<img src="/uploads/db1493/original/3X/6/0/60e291db2b6bc92f6ab2b002c0ac3a342b1be73c.JPG" width="333" height="500">
```

---
## \#184 Posted by: webst Posted at: 2016-10-24T10:33:13.699Z Reads: 359

```
@Blasto @JohnnyMeduse  Could you record and post a movie here how does sensorless start from 0km/h look like on VESC-X in FOC mode?

@Michaelinvegas Thanks for photos, this looks good.
```

---
## \#185 Posted by: JohnnyMeduse Posted at: 2016-10-24T12:40:03.119Z Reads: 357

```
I will try my best, but It's pretty rainy all week around here, Also starting from 0 in a sensorless FOC, is not as fast as starting from 0 in a BLDC, because the motor need to find is position, so it's is better to give it a little push. (but for testing purpose, who cares :wink:)
```

---
## \#186 Posted by: Monte Posted at: 2016-10-24T14:50:51.591Z Reads: 351

```
<img src="/uploads/db1493/original/3X/9/8/980445c377bd9ac80725db2ac296f3c087082140.png" width="587" height="76">
```

---
## \#187 Posted by: Michaelinvegas Posted at: 2016-10-24T15:00:04.207Z Reads: 365

```
Out of nowhere it rains in Vegas today  ...after months no rain ....

<img src="/uploads/db1493/original/3X/3/7/37ffeff5fee06b65adb6a20b79ed2cc4ade6f3fe.JPG" width="500" height="500">
```

---
## \#188 Posted by: Blasto Posted at: 2016-10-24T22:35:49.507Z Reads: 364

```
Here you go

http://www.youtube.com/watch?v=CdgAD3KyWuQ
```

---
## \#189 Posted by: Michaelinvegas Posted at: 2016-10-24T22:38:18.917Z Reads: 357

```
nice and silent
```

---
## \#190 Posted by: webst Posted at: 2016-10-24T22:45:01.378Z Reads: 352

```
Thanks. I expected it would stutter a little and there's no such thing. This is great.
```

---
## \#191 Posted by: Blasto Posted at: 2016-10-24T22:47:24.935Z Reads: 356

```
The wheel needs to turn about 1/4 turn for the vesc-x to know the motor position, when i turned the board around on the second go, there is a slight stutter but it quickly goes away.

Just get the board rolling and there will be no stutter at all
```

---
## \#192 Posted by: Michaelinvegas Posted at: 2016-10-24T22:53:23.218Z Reads: 357

```
<img src="/uploads/db1493/original/3X/a/b/ab3ead641f428b9382395066253d3b40bf462177.PNG" width="690" height="157">


Added just for you so your impatient brethren don't get all squirmy lol
```

---
## \#193 Posted by: deke997 Posted at: 2016-10-25T01:47:17.385Z Reads: 360

```
I just fried my VESC 4.12, so I need a new VESC now. I would love to beta test for you!! @onloop
```

---
## \#194 Posted by: Michaelinvegas Posted at: 2016-10-25T05:06:33.681Z Reads: 362

```
There are other VESC Gods in charge of the picking apparently
```

---
## \#195 Posted by: Michaelinvegas Posted at: 2016-10-25T10:06:32.191Z Reads: 376

```

!!!  This is a BETA Version of the VESC-X!!! Copying this process could VOID your Warranty!   So, please check the terms and conditions of your warranty before attempting to add conformal Coatings. 

Keep-out areas:
-Connectors, will create a bad electrical contact.
-mosfets, will affect the thermal transfer.
-thermal tape, will affect the thermal transfer.
-mounting points
-the heatsink has a very tight gap in between the heatsink and mosfets (0.4mm). This gap is very important for a controlled pressure on the thermal tape. If the gap is increased by the conformal coating, less pressure will be applied to the tape and it will affect the thermal transfer






https://youtu.be/5ZjktW68JXI
```

---
## \#196 Posted by: Mox Posted at: 2016-10-27T15:23:26.991Z Reads: 364

```
Preordered one because I think its a nice product. The warrenty thing is kind of odd but Im sure Jason will pay special attention on the units that roll out in the first batch ;)
@onloop I sent you a request for the screw hole mount thing(Simon on fb). Would be lovely if you could provide me with the necassary information.
```

---
## \#197 Posted by: onloop Posted at: 2016-10-27T20:48:58.538Z Reads: 367

```
The Facebook message will go to my support team. 

Maybe I can answer the question for you on here. Are you asking about the mounting holes on the bottom of heat sink?

They are rectangle 30mm x15mm spacing. M3
```

---
## \#198 Posted by: Mox Posted at: 2016-10-27T21:47:11.821Z Reads: 369

```
That would be great!
I want to build a board with a kydex enclosure with the vescx’s heat sink fastened to it inside the enclosure facing the ground. 
This got me thinking. The heat sink has 7 tread holes. This might be a great opportunity to build an additional heat sink that is outside the kydex case with 7 holes that perfectly aline with the ones from the vescx. Fastening the two together (with the kydex in between) would get some additional heat management going.
Bottom line is I would need exact measurements of the vescx's heat sink regarding the position of those thread holes to make that work. Since I don’t have the unit yet it would be lovely if you could provide me with these measurements. 
Bottom line is; I want to start building but I don’t have anything to work with yet. (first build and started ordering a week ago)
```

---
## \#199 Posted by: onloop Posted at: 2016-10-27T21:56:54.614Z Reads: 375

```
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/8/c/8c732a6069b0e963f0809da24ae8e9de242ae028_1_690x455.png
```

---
## \#200 Posted by: Mox Posted at: 2016-10-27T22:08:59.895Z Reads: 367

```
Thanks mate!
```

---
## \#201 Posted by: onloop Posted at: 2016-11-01T07:12:43.394Z Reads: 380

```
Some photos i got last week showing the heat sink & hard case. First batch of 20 will be ready soon installed inside these cases and then will get some VESCX sent out to more testers

<img src="/uploads/db1493/original/3X/c/c/cc01a89c5e8fa10e2e02d4c601575d2990859b66.jpg" width="607" height="500">

<img src="/uploads/db1493/original/3X/3/4/34110ae00aaaab7fad1bbf25f844118dc7bce269.jpg" width="618" height="490">
```

---
## \#202 Posted by: Mark Posted at: 2016-11-01T09:03:25.459Z Reads: 363

```
Wondering if I pre-order a vesc x right now when it would arrive?
```

---
## \#203 Posted by: Mox Posted at: 2016-11-01T09:10:15.739Z Reads: 361

```
I preordered a week ago and I just receved my tracking number
```

---
## \#204 Posted by: xxlv Posted at: 2016-11-03T11:51:54.599Z Reads: 368

```
I preordered mid Oct and i did not receive a tracking number :(
```

---
## \#205 Posted by: onloop Posted at: 2016-11-03T12:23:52.503Z Reads: 365

```
vescx hasnt shipped to anyone yet.
```

---
## \#206 Posted by: E-Boarding Posted at: 2016-11-03T12:36:48.154Z Reads: 368

```
Discount VESCX$20OFF still works, looks like less than 20 people have ordered them so far.
```

---
## \#207 Posted by: Michaelinvegas Posted at: 2016-11-05T23:35:37.893Z Reads: 374

```
VESC - X FOC
12s 
Carvon v2.5 85kv


https://youtu.be/SVSLEgBw7wI
```

---
## \#208 Posted by: Michaelinvegas Posted at: 2016-11-06T12:25:52.517Z Reads: 374

```
Setting up the VESC-X at 12s FOC


https://youtu.be/xgx3DE3hX24
```

---
## \#209 Posted by: JTAG Posted at: 2016-11-07T20:52:51.738Z Reads: 361

```
You received a proto / sample VESC-X and you need help configuring it? How does that compute xD?
```

---
## \#210 Posted by: Michaelinvegas Posted at: 2016-11-07T21:23:39.990Z Reads: 364

```
Hey if someone says I'll give you a hand...who am I to say No lol

Plus a opportunity to film the setup using 12s right off the bat with the carvons....
```

---
## \#211 Posted by: jct1212 Posted at: 2016-11-08T16:26:30.929Z Reads: 371

```
Are these on track to start shipping soon? No problem if they are not, just wondering.
```

---
## \#212 Posted by: onloop Posted at: 2016-11-12T04:45:44.295Z Reads: 382

```
our US based factory moved last week, so put us back a tad.

anyway, they now have a much larger production area & more staff.... which is great news!

latest news, we have the PCBS, the BOM is on hand, program& test JIGS are ready - we will have a pre-production batch made to double check everything is perfect - then we hit the bit green go button. By the end of November, 120 units will have shipped, this should cover all orders & from there-there will be ample stock ongoing for immediate shipping.

<img src="/uploads/db1493/original/3X/6/2/626eb73f3d5dffe90857aa2cc0c7f53a6e37207c.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/2/126ef51ca1edb8cc67571effd6673b65db73d396.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/e/9/e90bdab24da90fbf99e07332b214dd11d795fb5d.jpg" width="690" height="388">
```

---
## \#213 Posted by: onloop Posted at: 2016-11-14T22:16:29.381Z Reads: 372

```
https://www.instagram.com/p/BMyCBiUgrKR/?taken-by=enertionboards&hl=en
```

---
## \#214 Posted by: onloop Posted at: 2016-11-15T02:28:35.448Z Reads: 376

```
First VESC with i/o labels

https://www.instagram.com/p/BM0DHUEA1_L/?taken-by=enertionboards&hl=en
```

---
## \#215 Posted by: xxlv Posted at: 2016-11-15T10:07:02.715Z Reads: 372

```
Hey! 
in my order confimation is written "(Stock Available After 10th Nov 2016)". I'm wondering when exactly you will be shipping them? I cant wait! :)
```

---
## \#216 Posted by: Mark Posted at: 2016-11-15T10:12:56.719Z Reads: 357

```
Does the 15$ referal still work?
```

---
## \#217 Posted by: Stefan Posted at: 2016-11-15T10:19:04.020Z Reads: 366

```
<img src="/uploads/db1493/original/3X/8/a/8abf1ad0a91efbc9b4742389c0937aac4270bbe1.png" width="281" height="499">
```

---
## \#218 Posted by: SORRENTINO Posted at: 2016-11-15T14:16:59.520Z Reads: 350

```
So is the blue and black case the heatsink or only the blue part?
```

---
## \#219 Posted by: TarzanHBK Posted at: 2016-11-15T14:40:48.458Z Reads: 360

```
the blue part is the alu heatsink and the black part is just housing
```

---
## \#220 Posted by: onloop Posted at: 2016-11-22T04:50:57.778Z Reads: 369

```
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/2/3/2321c52bcfaf129eee8dc410b0a2c752af0e62d9_1_666x500.JPG


some vesc-x heading out to some folks
```

---
## \#221 Posted by: CaptainMerricka Posted at: 2016-11-23T05:45:00.881Z Reads: 357

```
oh man I can't wait to be some folks.
```

---
## \#222 Posted by: DeathCookies Posted at: 2016-11-23T12:48:02.796Z Reads: 355

```
Why dont you insert plugs for UART?
```

---
## \#223 Posted by: Smithster Posted at: 2016-11-23T13:13:37.488Z Reads: 358

```
Will the Vesc-x be available from the EU distributor?
```

---
## \#224 Posted by: Monte Posted at: 2016-11-23T15:04:33.912Z Reads: 358

```
Why do people not just wait for Vesc v6? It will be released in early 2017. You can say what ever you want but the vesx actually cant be better than the new version. Benjamin did much work on it to improve it. And i think its not that much hard to just wait 3-4 Months to get a Quality version of it from Someone like Chaka.

This post was flagged by the commu.....
```

---
## \#225 Posted by: darkkevind Posted at: 2016-11-23T15:09:32.211Z Reads: 348

```
I think when you want something, you want it now! At least that's how I feel anyway. I don't want to be waiting months to be able to best experience my board... just my 2p :slight_smile:
```

---
## \#226 Posted by: jujet Posted at: 2016-11-23T15:12:48.054Z Reads: 357

```
[quote="Monte, post:224, topic:11102"]
It will be released in early 2017
[/quote]

Vedder said he will try and setup a team to test it and will probably release it sometime in March 2017. That's 4 months from today

[quote="Monte, post:224, topic:11102"]
Why do people not just wait for Vesc v6?
[/quote]

Because you'd have to wait 4 months for it
```

---
## \#227 Posted by: TarzanHBK Posted at: 2016-11-23T15:23:37.860Z Reads: 345

```
and after that, someone has to build it (again a few months) to make it vendor reliable and tested
```

---
## \#228 Posted by: flatsp0t Posted at: 2016-11-23T16:25:08.862Z Reads: 354

```
It will be about 100$ more in pure component price, and not everyone needs the added features and capabilities.
It will be bulkier because of onboard communication modules that are not needed by Everyone.
This aside, the "release date" was announced Yesterday. Nobody wants to wait for something that will come "maybe soon".

You need to wait, if you want to use big motors(80XX or even larger), or if you have high current scenarios(EMTB, Hubs) or more reliable FOC(or a combination of this). 
But for every normal use case, these are very good, and there is no need to spend more money and wait months to get rolling.

just my 2 cents
```

---
## \#229 Posted by: CaptainMerricka Posted at: 2016-11-24T07:17:33.744Z Reads: 340

```
Cost. I am betting on the Vesc 6 being more expensive because of its increased features.
```

---
## \#230 Posted by: onloop Posted at: 2016-11-25T02:48:48.071Z Reads: 343

```
[quote="DeathCookies, post:222, topic:11102, full:true"]
Why dont you insert plugs for UART?
[/quote]

they will be there
```

---
## \#231 Posted by: onloop Posted at: 2016-11-25T02:51:14.221Z Reads: 357

```
[quote="CaptainMerricka, post:229, topic:11102, full:true"]
Cost. I am betting on the Vesc 6 being more expensive because of its increased features.
[/quote]

the VESC 6 will be much more expensive, we think it will retail around $300USD. It also seems the footprint is a bit larger so some people might need to rethink their enclosures.

the VESCX will be a more compact & more affordable option still with the benefit of high current throughput / improved cooling. Perfect for Hub motors.
```

---
## \#232 Posted by: xxlv Posted at: 2016-11-25T08:38:05.775Z Reads: 348

```
How do you come to 300USD? Most of the BOM is the same, you don't need to add the NRF on the Board. It can be around the same price as the current VESC.
```

---
## \#233 Posted by: rmrf Posted at: 2016-11-28T13:18:15.344Z Reads: 352

```
You forgot to take some things into account

• countless hours spent on R&D
• suffix X
• much innovation
• direct drive™
• science is curiosity™
• video with boy and girl on skateboard holding hands
```

---
## \#234 Posted by: JohnnyMeduse Posted at: 2016-11-28T13:44:08.550Z Reads: 350

```
300 is for the vesc 6.0, start to read the tread before bashing.... 300 is also the leak price from trampa... The price is also base on the licence, VESC will not be easy to market.
```

---
## \#235 Posted by: rmrf Posted at: 2016-11-28T13:53:50.929Z Reads: 343

```
Oh you know something we all don't know. Please shed some light on us. Tell us more about the license. I had a conspiracy theory about VESC6 dual license, is it true? Is it?
```

---
## \#236 Posted by: mmaner Posted at: 2016-11-28T13:56:45.680Z Reads: 344

```
@onloop I grew up in a family of Small Business owners. With the influx on corps like Wal-Mart & Costco small business in the US is essentially dead now.  That really sucks for the consumer as options are vastly limited.  Wal-Mart likes to see whats selling in an area, find a chinese knock-off, sell it for half the price to run small shops out of business.  They then raise the price higher than the small business to recoup the initial discounts, the only product change being a re-brand and dropping many accessories or versions.  Some people are not savvy enough to 'see behind the curtain' and get spoiled by the ease of purchase and fail to see the implications or lack of quality.

I write all of this because I don't know if its the same in Australia and I appreciate what you do for the community.  Having grown up in small business family I think I can safely assume you are just trying to make a living doing something you enjoy, just like the rest of us.  I can further assume you aren't getting lottery rich off this.  

To sum up, sometimes you just gotta wash your hands of the trolls and keep moving.  Good on you mate :)
```

---
## \#237 Posted by: Stefan Posted at: 2016-12-01T13:45:24.387Z Reads: 331

```
Any update on the VESC-X?
```

---
## \#238 Posted by: chuttney1 Posted at: 2016-12-02T03:13:49.617Z Reads: 333

```
VESC 6.0 cannot cost $300. If it did I go buy a PS4 Pro or something to make with for $300. I believe the max price would be $200, but $300 is way to much for the cost of good and some for profit.
```

---
## \#239 Posted by: CaptainMerricka Posted at: 2016-12-03T23:40:24.130Z Reads: 327

```
Are these shipping out? Cant wait to ride my first build!
```

---
## \#240 Posted by: lox897 Posted at: 2016-12-04T00:37:13.764Z Reads: 333

```
I got a reply from support saying they would ship from the manufacturer on 15th December. Hopefully in time for christmas.
```

---
## \#242 Posted by: CaptainMerricka Posted at: 2016-12-13T04:33:55.074Z Reads: 330

```
I got an update on the vesc-x today from enertion.

"Just a quick update on the progress of the VESC-X production. 

Our manufacturer has advised today that they will commence shipments after 23rd December. Please note that there may be delays with receiving your order due to the Christmas holiday period.

We really appreciate your patience whilst the manufacturer has been completing the production of this exciting, new product. "
```

---
## \#243 Posted by: lox897 Posted at: 2016-12-13T04:39:06.111Z Reads: 328

```
I was told 15th December it would ship. Now they are saying 23rd... I was hoping to have this by christmas for my little bro, unfortunately not. Hopefully enertion will ship by DHL so it can get there by his birthday...
```

---
## \#244 Posted by: Stefan Posted at: 2016-12-24T13:00:49.825Z Reads: 319

```
Any updates on shipping?
```

---
## \#245 Posted by: SeanHacker Posted at: 2016-12-24T17:22:33.459Z Reads: 323

```
It's supposed to be shipping early January now.
```

---
## \#246 Posted by: Stefan Posted at: 2016-12-24T17:32:12.435Z Reads: 326

```
Why is shipping delayed again and again? I don't get why there are actually even any dates set for shipping when they get cancelled as soon as we pass that day?
```

---
## \#247 Posted by: willpark16 Posted at: 2016-12-24T19:30:59.711Z Reads: 313

```
It's enertion so always plan for three months after that date
```

---
## \#248 Posted by: ThomasLefort Posted at: 2016-12-25T18:23:26.291Z Reads: 311

```
There is zero communication. Too bad. Surely the last time I ordered at Enertion because of that. Do not give a date if it is to repel it 4 times then. This is not correct with regard to your customers.
Good evening and merry Christmas to all
```

---
## \#249 Posted by: E-Boarding Posted at: 2016-12-25T21:16:59.568Z Reads: 304

```
the Enertion webside says "Stock Shipping After 23rd Dec 2016"
```

---
## \#250 Posted by: lox897 Posted at: 2016-12-26T01:36:50.216Z Reads: 306

```
The delivery date is now the 27th. First 15th, then 23rd, then 25th, now 27th.
```

---
## \#251 Posted by: kptheinventor Posted at: 2016-12-26T05:23:19.376Z Reads: 310

```
@lox897 Is the delivery date the date Enertion expects to receive them or the date we should expect to receive them?
```

---
## \#252 Posted by: lox897 Posted at: 2016-12-26T05:34:32.896Z Reads: 308

```
That is the date that MacroFab will ship them. @kptheinventor
```

---
## \#253 Posted by: 2-alex-2 Posted at: 2016-12-26T11:48:16.951Z Reads: 310

```
Looks like tipical enertion delays are you guys even surprised it been delayed.
```

---
## \#254 Posted by: E-Boarding Posted at: 2016-12-26T16:57:02.243Z Reads: 305

```
no, it would suck a lot if it would be summer, but it's winter so not a big deal, I knew there will be 1-2 montths delay when I bought this.
```

---
## \#255 Posted by: kptheinventor Posted at: 2016-12-26T20:59:49.846Z Reads: 308

```
@2-alex-2 Hahah this is my first build, I didn't realize Enertions reputation :/
```

---
## \#256 Posted by: mmaner Posted at: 2016-12-26T22:19:43.124Z Reads: 306

```
Eneetion reputation is very good.  They make great products.  There's just quit a few trolls around here that like to start crap.
```

---
## \#257 Posted by: lox897 Posted at: 2016-12-26T22:48:44.934Z Reads: 310

```
[quote="E-Boarding, post:254, topic:11102, full:true"]
no, it would suck a lot if it would be summer, but it's winter so not a big deal, I knew there will be 1-2 montths delay when I bought this.
[/quote]

But it's summer where I live... @E-Boarding
```

---
## \#258 Posted by: willpark16 Posted at: 2016-12-27T00:49:13.543Z Reads: 313

```
How many vesc delays were there? I'm just saying his mechanical components are grade A but anything electrical I wouldn't hold my breath on. He even put cheap bypassed bms in his new space cell so u can pay 350 for cheap components
```

---
## \#259 Posted by: monkey32 Posted at: 2016-12-27T01:48:50.714Z Reads: 321

```
Enertion has a great rep and can produce great products, over  200,000 raised for the new complete board without even a V2 prototype being evidence of this.

 However  they/ he often sells products prior to having goods in hand ( normal with small business) and as such have seemingly now, as in past, committed to deadlines he/ they can't meet due to circumstances they can't control. 

They/ he  hopefully improve with this as they/ he continue to grow. It's not all trolls commenting. I have been a staunch supporter (still rock the gold motor mount ) and will continue to be. But the pattern still exists as with any budding company.....chalk it up to growing pains
```

---
## \#260 Posted by: Esrapp21 Posted at: 2016-12-27T02:53:52.495Z Reads: 321

```
I think enertion should trademark the term "Delay" :slight_smile:
```

---
## \#261 Posted by: onloop Posted at: 2016-12-27T11:26:26.669Z Reads: 317

```
Will ship any day now. Everything slows down during holiday period.

Sorry for the delays.
```

---
## \#262 Posted by: ZachNYC Posted at: 2016-12-31T04:55:59.179Z Reads: 315

```
@onloop hope all is well, but the vesc and charger are pretty much the only things I'm waiting on, and I'm really anxious to see my board in action, any updates? Either way, happy holidays and new year.
```

---
## \#263 Posted by: lox897 Posted at: 2017-01-17T05:44:09.857Z Reads: 304

```
I didn't receive a confirmation email but I received a text message from DHL. If you haven't heard about your shipment yet, try registering for a MacroFab account or DHL to get a tracking number
```

---
## \#264 Posted by: onloop Posted at: 2017-01-17T06:13:05.264Z Reads: 308

```
MacroFab having lots of problems with fullfilment at the moment. It seems they are shipping out orders and not pushing data to our systems.

Also, Some orders have been duplicated. Please notify us if you have received a duplication or error with your order.

We will be emailing everyone who has been affected by these issues.

Thanks for your understanding.
```

---
## \#265 Posted by: ThomasLefort Posted at: 2017-01-18T12:14:12.005Z Reads: 309

```
I finally received mine. Is it possible to have some documentation about the electronic ? I'm working on a DIY remote and I can't read pin designation on my VESC.
Thanks by advance
```

---
## \#266 Posted by: Blasto Posted at: 2017-01-18T13:57:09.736Z Reads: 319

```
<img src="/uploads/db1493/original/3X/9/c/9cc0a294ccb47fe6cb14e070bc1978c53443b27c.JPG" width="500" height="500">
```

---
## \#267 Posted by: SeanHacker Posted at: 2017-01-20T02:41:33.298Z Reads: 318

```
<img src="/uploads/db1493/original/3X/3/8/38d93f7ff62b2c4389dbe82e394459593b022b65.jpg" width="281" height="499">
```

---
## \#268 Posted by: onloop Posted at: 2017-01-20T04:11:01.828Z Reads: 321

```
<img src="/uploads/db1493/original/3X/9/a/9a34fd7ebaf8c5a1c595ad77aef6754a607c2c2a.png" width="497" height="500">
```

---
## \#269 Posted by: Okami Posted at: 2017-01-20T10:57:26.053Z Reads: 304

```
Can someone quickly tell what current capability these guys have?
(over a standard vesc) ?
```

---
## \#270 Posted by: Stefan Posted at: 2017-01-20T12:52:20.614Z Reads: 305

```
Jason mentioned that the VESC-X should be able to cope with 60A constantly.
```

---
## \#271 Posted by: lox897 Posted at: 2017-01-20T18:08:06.733Z Reads: 313

```
Setup in BLDC Tool in 10 minutes and slapped it onto my bro's new board. Working perfectly with 4x 3s lipos in series and a 170kv motor.

Top speed:45-50km/h
Range: 17km
```

---
## \#272 Posted by: Okami Posted at: 2017-01-20T18:25:50.663Z Reads: 316

```
@lox897  What battery capacity / how much wh? 17km seems cool

---
@Stefan 80A seems quite a lot.. I wonder does just heatsink alone can do this.. im not sure if Jason did that direct fet thing chaka or someone else who is dealing with vesc's told about..

I understand current limit is about 50a for standard one, so if this one can do 60-65, that would still be an improvement.. some video would be cool to see that this vesc-x is really capable of 80A..

@lox897 I assume your buddy wont be ready to push the limits of vesc-x ? Do you know someone who would be willing to give it a try? :D of course that person also needs metr.at or some other vesc bluetooth app ;)
```

---
## \#273 Posted by: lox897 Posted at: 2017-01-20T18:27:37.221Z Reads: 299

```
My mistake, I meant 22km range. 12 x 3.7 =44.4v

44.4v x 5 = 222wh

222 / 10wh (per km) = 22.2km range
```

---
## \#274 Posted by: Randyc1 Posted at: 2017-01-20T19:39:28.069Z Reads: 297

```
What gearing you have to reach 50kph on a 170 kv ?
```

---
## \#275 Posted by: lox897 Posted at: 2017-01-20T19:53:15.800Z Reads: 303

```
15/36 gearing. I'm also 45kg. I haven't tested full speed yet but I got to 38kmh with about 2/5 more throttle
```

---
## \#276 Posted by: Stefan Posted at: 2017-01-21T00:04:16.207Z Reads: 308

```
I'm sorry, I looked it up again and it was 60A. I will edit this in my last post so no one can get confused.
```

---
## \#277 Posted by: mptrs Posted at: 2017-01-21T11:23:41.106Z Reads: 307

```
@onloop any chance this can be shipped from the warehouse in Europe?

Or is anyone already starting a group buy for this?
```

---
## \#278 Posted by: IDVert3X Posted at: 2017-01-21T11:32:56.640Z Reads: 327

```
EU group buy for these would be nice, Enertion also offers nice bulk discounts.
Maybe @ajaynagra could include these in his next GB? 

> Buy 5 - 10 and pay only €147.55 each
> Buy 11 - 20 and pay only €143.32 each
> Buy 21 - 30 and pay only €138.38 each
> Buy 31 - 40 and pay only €110.84 each
> Buy 41 - 50 and pay only €103.08 each
> Buy 51 or above and pay only €83.31 each

But as we all know Enertion, it's going to take at least 3 forevers for it to be shipped :D
```

---
## \#279 Posted by: onloop Posted at: 2017-01-21T11:39:12.087Z Reads: 340

```
[quote="IDVert3X, post:278, topic:11102"]
it's going to take at least 3 forevers for it to be shipped
[/quote]

VESC-X in stock now in USA warehouse.

<img src="/uploads/db1493/original/3X/7/2/72472beea87dc297b8fbce915e14402b108c16f3.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/1/4/14486565c36345a2ec6fa3cb41a09df2aea01b9c.jpg" width="374" height="500">
```

---
## \#280 Posted by: ZachNYC Posted at: 2017-01-22T19:07:11.922Z Reads: 311

```
Just got mine!! Wish I was prepared and had finished getting everything else though.
```

---
## \#281 Posted by: willpark16 Posted at: 2017-01-22T23:06:59.790Z Reads: 306

```
I'f i buy a vesc x today what would be the estimated arrival time to california
```

---
## \#282 Posted by: dylantrygg Posted at: 2017-01-22T23:26:27.457Z Reads: 305

```
I just receieved my VESCX and it looks very well built and sturdy. I also have the enertion 190kv motor. I put it in my build and it spun at full rpms. I strapped everything up and set the board down to ride and the board has no torque at all. Literally not enough torque to pull the board by itself. I'm running 8s which should be very well in the high range of torque. Any suggestions?
```

---
## \#283 Posted by: JohnnyMeduse Posted at: 2017-01-22T23:34:21.819Z Reads: 298

```
Did you setup the vesc in the bldc tool before trying to ride it...?
```

---
## \#284 Posted by: dylantrygg Posted at: 2017-01-22T23:36:57.154Z Reads: 298

```
I did try connecting via micro usb, but nothing would show up on the tool.
```

---
## \#285 Posted by: JohnnyMeduse Posted at: 2017-01-22T23:48:44.244Z Reads: 298

```
Well.... VESC are NOT PLUG AND PLAY... you need to configure them by using the bldc tool... If you have any problem configure it you can use the key word VESC FAQ in the search bar or if you don't found what youre looking for start a new topic, and it will be a pleasure to help you 😉

Edit: quick tip... try to press the refresh arrow... left to the connect button 😉
```

---
## \#286 Posted by: dylantrygg Posted at: 2017-01-23T00:05:47.209Z Reads: 295

```
Okay, it wasn't connecting on my mac so I booted up windows and it connected to the vesc from there. Thank you for your help.
```

---
## \#287 Posted by: willpark16 Posted at: 2017-01-23T00:19:26.559Z Reads: 301

```
I thought with enertion product like his motor and batter they were
```

---
## \#288 Posted by: JohnnyMeduse Posted at: 2017-01-23T00:25:37.456Z Reads: 300

```
Each motor and each VESC are different... And even if a motor detection has been made in the testing process it won't alway correspond to another motor.
```

---
## \#289 Posted by: willpark16 Posted at: 2017-01-23T00:35:36.220Z Reads: 298

```
True I was just saying that on loop previously stated his 4.12 vesc could be paired with any of his spacecells or motors
```

---
## \#290 Posted by: lox897 Posted at: 2017-01-23T13:21:37.604Z Reads: 296

```
I believe you have to install an Arduino driver to get it working on the Mac.
```

---
## \#291 Posted by: themegak Posted at: 2017-01-23T16:36:53.746Z Reads: 297

```
I just got my VESC X in the mail a couple of days ago.  First of all congratulations @onloop .  This thing is a beauty.  I love the design, the direct fets, the chasis and the clear labeling of every pin.  Kudos my man, you have outdone yourself.  I've got one question, I'm hoping someone can answer for me.  I opened the case and noticed a tan colored piece of tape on top of the fets.  The tape is thick enough to prevent the chasis from sitting on the board evenly, I'm wondering if i can simply remove the piece of tape and tighen the case properly.  Just not sure if there is a reason for the tape to be there.  Can someone please let me know.  I will upload some pictures later.
```

---
## \#292 Posted by: JohnnyMeduse Posted at: 2017-01-23T16:45:24.658Z Reads: 293

```
DON'T TOUCH THAT TAPE... It is a thermal conductive tape and need to be place there, or else you will short every mosfet together

Also the gap need to be there in other to prevent the heatsink to short every component
```

---
## \#293 Posted by: themegak Posted at: 2017-01-23T17:17:21.050Z Reads: 301

```
got it thanks. so there will be a small gap between the case and board.  Was hoping for a nice flush case for the board to keep debris out but if that is how it needs to be than all good.  Still the nicest VESC I've ever seen.
```

---
## \#294 Posted by: JohnnyMeduse Posted at: 2017-01-23T17:20:15.238Z Reads: 307

```
You shoudn't get too much debris inside... but you still can seal it with some silicone around the gap (not on the board but on the cover) maybe... 😉
```

---
## \#295 Posted by: themegak Posted at: 2017-01-23T17:20:50.383Z Reads: 321

```
sounds good.  Thanks for the quick reply.  You are a gentlemen of the the highest order.
```

---
## \#296 Posted by: willpark16 Posted at: 2017-01-23T17:21:21.869Z Reads: 333

```
do you know the wait time for a vesc x in the us if ordered today? also would you reccommend the warranty?
```

---
## \#297 Posted by: JohnnyMeduse Posted at: 2017-01-23T17:22:39.480Z Reads: 337

```
As Jason said earlier last week, I think they are in stock rigth now...
```

---
## \#298 Posted by: willpark16 Posted at: 2017-01-23T17:28:13.426Z Reads: 339

```
tried tagging him but he bumped over it..... thanks tho
```

---
## \#299 Posted by: Hylke59beare1913 Posted at: 2017-02-04T11:59:04.616Z Reads: 335

```
does it mather how i connect the new vesc-x on the motor there are three wirrels.
and i dont know how i connect the three wirrels from the receiver to the vesx-x
on youtube are the old vesc and can not see wich wirrel on what pin
```

---
## \#300 Posted by: nitt Posted at: 2017-02-04T16:05:41.086Z Reads: 334

```
Hello everyone I have just recieved a vescx and it states V1.3 on the outside and inside of the case What version of software do I use. I cannot afford to melt to many of these. All help is appreciated.
```

---
## \#301 Posted by: jct1212 Posted at: 2017-02-04T16:38:56.941Z Reads: 322

```
Just connect them any way. If the motor spins the incorrect direction (it goes backwards when it should be moving forwards), switch any two of the wires and it should be good!
```

---
## \#302 Posted by: jct1212 Posted at: 2017-02-04T16:39:25.108Z Reads: 322

```
I just set mine up with the BLDC tool and didn't have to update or change the firmware at all. It is 4.12 I believe
```

---
## \#303 Posted by: nitt Posted at: 2017-02-04T17:48:37.613Z Reads: 319

```
Thank you for the advice , all I am getting is com3 the software is not able to find the hardware. No hurry snow for a month at least.
```

---
## \#304 Posted by: ThomasLefort Posted at: 2017-02-06T09:45:20.421Z Reads: 328

```
Hi,
I was wondering if I can get the 5V output to power an Arduino on the JST 7pin connector. The 5V pin is able to power an external component ?
Thanks in advance
```

---
## \#305 Posted by: Ackmaniac Posted at: 2017-02-06T10:00:31.450Z Reads: 329

```
You can power external components via the 5V pin. Arduino, ESP8266 or Bluetooth modules are no problem.
```

---
## \#306 Posted by: Pedrodemio Posted at: 2017-02-06T11:53:10.054Z Reads: 331

```
I always had problem with the VESC interfering with the radio module connected to the arduino, a low pass filter on the 5v line solved the issue but I never understood why this happened
```

---
## \#307 Posted by: Lambjr088 Posted at: 2017-02-08T17:55:07.991Z Reads: 325

```
Is anyone doing a groupbuy for these vesc-x i would be down for 4 of them if any is. Gotta hit up the groupbuy gurus for this
```

---
## \#308 Posted by: willpark16 Posted at: 2017-02-08T20:46:21.643Z Reads: 318

```
Down if we can get 10 people
```

---
## \#309 Posted by: Tarzan Posted at: 2017-02-08T22:15:11.048Z Reads: 323

```
Speaking of gurus 
@Michaelinvegas is famous for organizing group buys
```

---
## \#310 Posted by: Michaelinvegas Posted at: 2017-02-09T04:50:25.012Z Reads: 315

```
What are we talking abt?
```

---
## \#311 Posted by: willpark16 Posted at: 2017-02-09T06:50:29.892Z Reads: 316

```
Vesc x group buy at least 5
```

---
## \#312 Posted by: dylantrygg Posted at: 2017-02-12T21:50:09.961Z Reads: 311

```
I have had the new VESC-X for a couple of weeks and also the bigger enertion motor. I've been running 4s in series (8s) and I love the torque/speed right off a full charge, but when my battery drains to around 95%, torque and speed decrease by a lot. Definitely still rideable but very annoying. Any suggestions?
```

---
## \#313 Posted by: Ackmaniac Posted at: 2017-02-12T22:05:51.564Z Reads: 311

```
What Battery do you have and what is your Battery cutoff start and cutoff end. the best would be if you post screenshots of your settings.
And please check in the realtime tab if the voltage that is shown there fits with your actual battery voltage.
```

---
## \#314 Posted by: dylantrygg Posted at: 2017-02-12T22:32:00.434Z Reads: 322

```
Just posted my own thread and put it on there. I'm running 2x 4s (8s) at 5000mah.
```

---
## \#315 Posted by: ArmandR Posted at: 2017-02-13T03:18:51.849Z Reads: 332

```
@onloop Is the performance much better compared to regular vescs?
```

---
## \#316 Posted by: onloop Posted at: 2017-03-08T08:22:19.544Z Reads: 347

```
Was noticing lots of universities ordering the VESC-X, so ran a report of all the universities that have ordered.



----------


----------


----------


http://cdn1.bigcommerce.com/n-yp39j5/zad02/images/stencil/original/products/176/1207/universities-vescx-x__97234.1488961056.jpg?c=2





----------


----------


----------



**WE HAVE OVER 500 IN STOCK IN USA - ORDER NOW**

http://www.enertionboards.com/electric-skateboard-parts/vesc-x-programmable-brushless-motor-controller/
```

---
## \#317 Posted by: akira Posted at: 2017-03-08T09:04:17.170Z Reads: 330

```
And if a guy working as receptionnist at NASA buys a VESC-X, would you also say that NASA is endorsing VESC-X for its next space shuttle ?
```

---
## \#318 Posted by: onloop Posted at: 2017-03-08T09:57:17.854Z Reads: 331

```
Actually I think I do have orders from nasa. 

Also, a guy from tesla ordered one the other day, I emailed him and asked if he could confirm if it was for personal use or for company / research etc. He said it was personal.

How about this my little space cadet friend, when I have a collection of 10 or more space agencies who have purchased a vescx, I'll do a special space one for you.
```

---
## \#319 Posted by: akira Posted at: 2017-03-08T10:39:21.148Z Reads: 327

```
Little space cadet friend ??
Your arrogance is really limitless ...
```

---
## \#320 Posted by: Nemesis Posted at: 2017-03-08T11:43:28.538Z Reads: 330

```
I'm not charging towards anyone on a trusted steed :racehorse: while wealding the sword of justice and truth :crossed_swords: and i know its not really that important to the context but...i just have to let the nerd in me say.... only six space agencies,
```

---
## \#321 Posted by: monkey32 Posted at: 2017-03-08T11:43:55.442Z Reads: 332

```
It is telling of the great work you do Jason....Well done it is great to see such reputable buyer. Congrats. I really hope you are prototyping a 6.0 now though cause yesterday's inovations are tomorrow's paper weights.....................I still have a V 1.0 VESC from you ............ Again awesome job and it's been really cool watching you build and grow but don't stop improving. stuff can always get better.
```

---
## \#322 Posted by: onloop Posted at: 2017-03-08T11:58:43.211Z Reads: 337

```
[quote="akira, post:319, topic:11102"]
Your arrogance is really limitless ...
[/quote]

https://usercontent2.hubstatic.com/7436639_f520.jpg
```

---
## \#323 Posted by: mmaner Posted at: 2017-03-08T16:09:11.117Z Reads: 329

```
[quote="onloop, post:316, topic:11102"]
Was noticing lots of universities ordering the VESC-X, so ran a report of all the universities that have ordered.
[/quote]

[quote="akira, post:317, topic:11102"]
if a guy working as receptionnist at NASA buys a VESC-X, would you also say that NASA is endorsing VESC-X
[/quote]

I dont see where he said anyone was endorsing anything...why be a dick?
```

---
## \#324 Posted by: Stevemk14ebr Posted at: 2017-03-08T16:15:48.546Z Reads: 320

```
It was implied by his graphic. You cannot deny that. *Plays Bob Marley on way out*
```

---
## \#325 Posted by: mmaner Posted at: 2017-03-08T16:17:44.090Z Reads: 328

```
I absolutely CAN deny that, that's not what I got from it, hence my confusion.
```

---
## \#326 Posted by: willpark16 Posted at: 2017-03-08T16:43:09.948Z Reads: 322

```
he was in a way but not in anyway that harmed anyone or justified that response. Nice job though @onloop
```

---
## \#327 Posted by: Stevemk14ebr Posted at: 2017-03-08T16:43:28.037Z Reads: 324

```
Bottom right: "Universities across the globe choose vesc-x" should be "Individuals at these universities choose vesc-x" the former implies that it is the university orderering these. If you don't agree that statement is misleading or could be misleading to others you are kidding yourself

Go lookup ethos, by associating images of these universities with the image of his vesc-x he builds off their reputation of quality. It is clever marketing, however it is misleading
```

---
## \#328 Posted by: E-Boarding Posted at: 2017-03-08T17:50:22.427Z Reads: 322

```
I would like to order but you removed the PayPal option, so I cannot order from Enertion anymore (without a credit card)

Is there someone in EU who can order them for me and sell me 2 VESC-X that I can pay with PayPal?
```

---
## \#329 Posted by: onloop Posted at: 2017-03-08T21:35:01.440Z Reads: 320

```
Get a debit card.
```

---
## \#330 Posted by: onloop Posted at: 2017-03-08T22:15:41.658Z Reads: 334

```
[quote="Stevemk14ebr, post:327, topic:11102"]
implies that it is the university orderering these.
[/quote]

**The Universities did order the VESCX....**

Mostly with an address specifically stating "robotics" or "engineering" etc

The university of Saskatchewan order was addressed directly to the  "University of Saskatchewan Space Design Team"

[MIT Lincoln Laboratory](http://www.ll.mit.edu/). Have also ordered, but they are not a university so didn't make the cut....
```

---
## \#331 Posted by: boards Posted at: 2017-03-08T23:09:01.864Z Reads: 333

```
Brushless ESCs suitable for robotics were really expensive before. I've seen quite a few projects using VESC at CMU recently.
```

---
## \#332 Posted by: JohnnyMeduse Posted at: 2017-03-09T00:26:58.516Z Reads: 340

```
Not only the VESC-X can be use in robotics, but also the Nano-X  😝


https://m.youtube.com/watch?v=rIoLBx3oHDY
```

---
## \#333 Posted by: Stevemk14ebr Posted at: 2017-03-09T00:31:31.615Z Reads: 347

```
Congrats then, I am mistaken and apologize.
```

---
## \#334 Posted by: KenTw Posted at: 2017-03-09T15:45:57.519Z Reads: 358

```
question
can i use the second channel on the nano x remote for a different speed curve?
if so, how can i do it on the vesc X?
```

---
## \#335 Posted by: Blasto Posted at: 2017-03-09T15:52:43.823Z Reads: 368

```
[quote="KenTw, post:334, topic:11102, full:true"]
questioncan i use the second channel on the nano x remote for a different speed curve?if so, how can i do it on the vesc X?
[/quote]

The second channel is a TTL 0-5V latching signal that could be used for leds. Controlled by a momentary switch on the remote

There's a switch on the nanoX to limit the ppm signal (beginner mode). 

If you want to have a full throttle curve control, you can get @Ackmaniac's bldc tool and firmware that will allow that.  The vescx come stock with fw 2.18 (latest from vedder)
```

---
## \#337 Posted by: SeanHacker Posted at: 2017-03-09T19:35:41.842Z Reads: 364

```
Feel better?
```

---
## \#339 Posted by: E-Boarding Posted at: 2017-03-09T22:06:49.145Z Reads: 360

```
Getting a credit card only to buy stuff from Enertion? Europe is not US.
I bought from you for a few k$ in the past with PayPal, very easy, why putting up barriers to give you my money?

In you Q&A you said, PayPal do not allow Preorders, ok fine, but the VESCX is not on preorder anymore, and what about BankTransfer, Stripe, Bitcoins, ...?

Can I buy some VESCs from your European Warehouse guy directly?
```

---
## \#340 Posted by: onloop Posted at: 2017-03-09T22:21:54.401Z Reads: 351

```
Debit card is not credit card. Do you have this option in Europe? Allows spending cash from bank on websites.
```

---
## \#341 Posted by: onloop Posted at: 2017-03-09T22:23:15.465Z Reads: 357

```
[quote="E-Boarding, post:339, topic:11102"]
PayPal do not allow Preorders,
[/quote]

If we turn on PayPal people will use it for raptor2 we cannot limit it to one product.
```

---
## \#342 Posted by: Jamy Posted at: 2017-03-09T23:20:00.768Z Reads: 354

```
Europe is a bit weird, yeah. It's getting better, we're finally getting prepaid cards for a decent rate. And now with N26 in some countries even debit mastercards.

@E-Boarding You're in Germany? Get an [N26 bank account](https://www.n26.com) for online purchases, it's free and they give you a Mastercard :)
```

---
## \#343 Posted by: E-Boarding Posted at: 2017-03-10T23:51:41.333Z Reads: 358

```
I see, so you can turn it on when the Raptor 2 is out?
I don't know what the difference between a debit and a credit card is, this is not very common in Germany, most websites do use banktransfer (where you put in your IBAN) or PayPal
```

---
## \#344 Posted by: JLabs Posted at: 2017-03-11T02:06:38.495Z Reads: 366

```
Just the small amount of business I have been doing I have realized that PayPal is not the best payment option, and has drawbacks. They charge more in fees, and its way to easy for people to create a claim and PayPal almost always sides with the customer. Also, if you start to do a lot more business the my freeze everything (look at what happened to Prusa). They may have done the same thing to Jason with the Raptor 2 launch. 

Stripe/Credit Card gateways are much easier in my opinion.
```

---
## \#345 Posted by: IDVert3X Posted at: 2017-03-12T00:23:41.265Z Reads: 360

```
@Jamy, @onloop

I live in Slovakia, **Europe**. The test place for all the banking stuff. We are small country, so it's easy to test it there, which is great, always the latest technology available :D

Debit card is basically a direct access to your account. If you pay using a debit card, money is charged directly from your account, if you don't have enough money, they will "borrow" you some ( there is a limit ). Your account will be -200 euros then for example. Once you get a salary of 800 euros for example ( typical salary there in Slovakia ), you will have +600 ( -200 + 800 ). If you can't get to "green numbers" fast enough ( usually one month ), they will charge you some money according to their rates, otherwise it's free. Credit cards are not used there. We use our debit cards everywhere including restaurants, supermarkets, hotels, all kinds of shops, public transport, gas stations... Yeah, it's actually hard to find a place where you can't pay using your debit card ( then you have to use cash, taverns are a good example ). You can use contactless payments almost everywhere as well. There is a limit for contactless payments tho. 20 euros per transaction if I'm correct. You can even use your smartphone instead of a card for contactless payments ( NFC support required ). If you need to pay more, you just insert your card into the terminal, type in your pin and you are good to go. It's the same, just slower. And of course you can use your debit card to pay for stuff on the internet. All the limits can be usually set in the internet banking.
```

---
## \#346 Posted by: E-Boarding Posted at: 2017-03-12T14:46:22.764Z Reads: 335

```
True, debit cards is most common non-cash-payment, but debit is not credit card, this is mainly an US-thing.
I know Enertion is focused on Amerika first, but can we say Europe second and let us pay with our debit cards?
```

---
## \#347 Posted by: Jamy Posted at: 2017-03-12T15:48:00.726Z Reads: 331

```
There are Mastercard and visa debit cards too though. (for example N26)
```

---
## \#348 Posted by: Maxid Posted at: 2017-03-12T18:13:22.187Z Reads: 335

```
DKB Visa is a free debit card. Might be worth a try for you.
```

---
## \#349 Posted by: kampfhahn Posted at: 2017-03-12T20:56:12.790Z Reads: 339

```
The DKB Visa is a real (free) Credit Card, i use it for five years now. You can also charge money to it if you don't want to use the credit function. But yes, they provide a V-Pay debit card as well.
```

---
## \#350 Posted by: Maxid Posted at: 2017-03-12T21:08:52.815Z Reads: 334

```
After having problems collecting a rental car with the DKB Visa I can say that it is not a real credit card. It is categorized as a Charge Card - which is NOT a traditional credit card.
```

---
## \#351 Posted by: kampfhahn Posted at: 2017-03-12T21:36:37.056Z Reads: 336

```
Don´t wanna start a discussion here but the DKB Visa is definitely a real credit card. As long as your limit is at least as high as the amount of money that the vendor wants to charge/block, you **shouldn't** get any problems with it. I never charge money on my DKB Visa and didn't get into trouble so far. In addition to a few hundred payments i also used it to block deposits for Apple´s express replacement service and at Sixt without problems. I´m pretty sure you just had bad luck but of course it sucked anyway.
```

---
## \#352 Posted by: Jamy Posted at: 2017-03-12T22:03:52.508Z Reads: 324

```
Rental car companies generally lock/authorize double the total price and then release half of it after the rental is over.
```

---
## \#353 Posted by: E-Boarding Posted at: 2017-03-13T21:20:30.737Z Reads: 336

```
[quote="onloop, post:329, topic:11102, full:true"]
Get a debit card.
[/quote]
In Germany 40mio people do have a credit card, this is 50% of the population. In the retail sector only 6% is payed with credit cards.

But 95% of the germans (like me) do have a debit card, usually a girocard (ec-card)

I may get myself a credit card, this sucks ass but you have a great unique product with your VESC-X

But for Enertion there is a potential of maybe double the sales from germany...
```

---
## \#354 Posted by: onloop Posted at: 2017-03-13T21:32:25.096Z Reads: 334

```
We have very good bulk prices on VESCX. I am surprised there are no German (or EU) entrepreneur who want to make a little business.
```

---
## \#355 Posted by: E-Boarding Posted at: 2017-03-14T16:58:28.292Z Reads: 345

```
On the german forum there is much talking about the VESC 6.0 (and nearly nothing about VESC-X)
And many people prefer the cheaper VESC 4.12 standard.
I don't understand that, germans are weird.
I think, VESC 6 can be bought soon without taxes and maybe a good warranty but VESC-X is still a bit cheaper.
```

---
## \#356 Posted by: thisisjaye Posted at: 2017-03-18T04:38:50.063Z Reads: 356

```
Any chance you can release the CAD files? I'll be ordering 30+ of these next week and would like to get a head start on my design.
```

---
## \#357 Posted by: TarzanHBK Posted at: 2017-03-20T11:50:00.851Z Reads: 356

```
Do you have Vescs in EU stock?
I need two more and don´t like import taxes so much ;)
```

---
## \#358 Posted by: onloop Posted at: 2017-03-20T13:46:14.527Z Reads: 360

```
Only in US. 

Some Talk of a europe GB. But not happened yet.
```

---
## \#359 Posted by: TarzanHBK Posted at: 2017-03-20T14:33:10.282Z Reads: 366

```
aaaand there we go:

http://www.electric-skateboard.builders/t/eu-group-buy-vesc-x/19354
```

---
## \#360 Posted by: bluetree70 Posted at: 2017-03-23T14:17:04.350Z Reads: 376

```
I recently brought VESC-X and Space battery pro from enertion and I was wondering I need to get a regulated power supply in order to configure the VESC-X for the first time. In the VESC guide, it was highly recommended to do so, but as I recall Chaka thinks that you only need to do this when powering up for the first time. I believe onloop said all the VESC-X have been tested before shipping. So does this mean I can use the space battery to power up the VESC-X for configuration without bricking it?

Also on the VESC-X it says "V1.3". Is this the firmware version or just the version number of the VESC-X? If so where can I find the firmware version of the VESCX I have?
```

---
## \#361 Posted by: Blasto Posted at: 2017-03-23T14:21:00.947Z Reads: 395

```
[quote="bluetree70, post:360, topic:11102"]
I need to get a regulated power supply in order to configure the VESC-X for the first time.
[/quote]

Very first thing you want to do is to solder your motor lead connections and ISOLATE them properly with heat shrink.

You should be ok to just power it up with your SCP4.

[quote="bluetree70, post:360, topic:11102"]
Also on the VESC-X it says "V1.3".
[/quote]

That is the hardware version

[quote="bluetree70, post:360, topic:11102"]
where can I find the firmware version of the VESCX I have?
[/quote]

download the BLDC tool, connect it to your computer, it will be firmware 2.18
```

---
## \#362 Posted by: bluetree70 Posted at: 2017-03-23T14:25:47.734Z Reads: 392

```
Thanks for the help!
```

---
## \#363 Posted by: Titoxd10001 Posted at: 2017-04-06T03:35:08.164Z Reads: 397

```
How are you guys connecting the receiver wires. With the connector I have it doesn't fit in my enclosure
<img src="/uploads/db1493/original/3X/4/3/43d93d7b81d291e491025aa74e32c08996cb6d89.jpg" width="666" height="500">
```

---
## \#364 Posted by: makevoid Posted at: 2017-04-06T03:42:12.037Z Reads: 410

```
you could solder directly to the pins, bend them a bit or use an angled connector like [these ones](http://www.ebay.co.uk/itm/50PCS-1x6Pin-Header-2-54mm-Pitch-Right-Female-Angle-Single-Row-Socket-Connector-/272263550286?hash=item3f642c154e:g:td4AAOSwubRXLCUA)
```

---
## \#365 Posted by: Titoxd10001 Posted at: 2017-04-06T04:30:03.419Z Reads: 441

```
Thanks, ill solder them on
```

---
## \#366 Posted by: Stef Posted at: 2017-04-06T04:32:04.805Z Reads: 442

```
Be careful to properly apply heatshrink, I recall someone shorting the pins and ruining his vesc.
```

---
## \#367 Posted by: Titoxd10001 Posted at: 2017-04-06T04:33:37.126Z Reads: 450

```
Thanks for the tip
```

---
## \#369 Posted by: Blasto Posted at: 2017-05-08T23:00:20.841Z Reads: 448

```
it does not have bluetooth directly, but it as UART, so you can use a bluetooth-serial dongle to connect to your phone. there's a few threads about this. check it out in the search bar
```

---
## \#370 Posted by: lox897 Posted at: 2017-05-14T20:50:05.082Z Reads: 443

```
Why are the VESC-X files not available anymore?
```

---
## \#371 Posted by: Blasto Posted at: 2017-05-14T20:52:17.872Z Reads: 438

```
http://www.enertionboards.com/how-to-build-eboard/vesc-x-design-files/
```

---
## \#372 Posted by: lox897 Posted at: 2017-05-14T20:54:46.657Z Reads: 433

```
You can't add it to cart

LOL LIVE CHAT TRANSCRIPT:

Lachlan:
I'd like the vesc x files please

Jessica M
I am sorry but we are sold out on that item

Lachlan:
Sold out? It's a downloadable file?
```

---
## \#373 Posted by: flywithgriff Posted at: 2017-05-14T20:59:45.900Z Reads: 425

```
HAHAHAHA Sorry but we are sold out of all the free stuff!
```

---
## \#374 Posted by: TranxFu Posted at: 2017-05-29T21:24:15.958Z Reads: 410

```
Hey guys :) Just received a couple VESC-X. Immediately wired it up and I'd want to try FOC now. No other reason besides that for getting them. 

Whats the general consensus on this ? Is this FOC Proof if you don't fk up the BLDC-Tool Setup ? I couldn't find any threads regarding FOC failure and VESC-X
```

---
## \#375 Posted by: Stefan Posted at: 2017-05-30T00:07:25.565Z Reads: 409

```
Runs smoothly for me since about January, on two vescs since march or so
```

---
## \#376 Posted by: Jebe Posted at: 2017-06-12T09:45:44.678Z Reads: 400

```
can someone please tell me what the pinouts are for the uart - the stickers are faded on mine.
```

---
## \#377 Posted by: rwxr Posted at: 2017-06-12T09:52:40.641Z Reads: 418

```
<img src="/uploads/db1493/original/3X/3/c/3c012b7f5d87d5fa7af7e58373d151d413459922.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/a/0a33b919d4ec47883254c7a23a0221a9dfec49aa.jpg" width="375" height="500">
```

---
## \#378 Posted by: rwxr Posted at: 2017-06-12T09:53:37.307Z Reads: 406

```
@lox897: do you have the design-files still?
```

---
## \#379 Posted by: Jebe Posted at: 2017-06-12T10:08:35.942Z Reads: 403

```
awesome - thanks bud.
```

---
## \#380 Posted by: lox897 Posted at: 2017-06-12T20:55:15.123Z Reads: 392

```
The VESC-X files? Yeah someone on here emailed them to me and I have them. PM your email and I can send them. Haha the Enertion support person never got back to me
```

---
## \#381 Posted by: Vieo Posted at: 2017-06-19T21:49:32.505Z Reads: 379

```
Would you mind positing publicly. Can't download them from website?
```

---
## \#382 Posted by: miguelop24 Posted at: 2017-07-20T11:15:15.069Z Reads: 364

```
@lox897 I have been searching these files online for a time now, if you still have them, could you send it to me? I will ask you for PM you when I can (this account is rly young :joy: ) if you dont mind
```

---
## \#383 Posted by: lox897 Posted at: 2017-07-20T11:28:06.304Z Reads: 367

```
I'll PM you
```

---
## \#384 Posted by: marcdecator Posted at: 2017-07-21T00:56:11.777Z Reads: 361

```
@lox897, could you also PM me? I would also really like to have a copy of the VESC-X design files. Thanks so much.
```

---
## \#385 Posted by: jbruce Posted at: 2017-07-21T04:39:20.127Z Reads: 350

```
@onloop Why the new design with 14awg wires?
```

---
## \#386 Posted by: onloop Posted at: 2017-07-21T04:43:22.100Z Reads: 354

```


14AWG is actually plenty.... we are running 80a motor currents with this.....  having thicker wire than a bundle of phase wires doesn't help performance.
```

---
## \#387 Posted by: TarzanHBK Posted at: 2017-07-21T06:22:50.965Z Reads: 360

```
isn´t 14 AWG only rated for 60A max continous?
Why underbuild and risking to lose power due to too much resistance and heat?
14 AWG is of course cheaper :smiley:
```

---
## \#388 Posted by: lox897 Posted at: 2017-07-21T08:46:57.762Z Reads: 361

```
@onloop can you please fix the VESC-X files on your store?

I'm going to upload them to media fire because I've had 10 people ask me today and it's kinda hard to remember them all. Everyone who wanted it please reply to this comment and I will tag you once I have them uploaded.

@Kaly
@miguelop24
@Surfer
@Alanhunt123
@marcdecator
@themegak
@The_Dude
@Martinsp
@DavidBanner
@JohnnyMeduse
@Mobutusan
@Ronny_CTS
```

---
## \#389 Posted by: Surfer Posted at: 2017-07-21T08:58:14.655Z Reads: 342

```
Hi, I would love to have that files if they provide info about repair it. Thanks in advance!!!
```

---
## \#390 Posted by: jbruce Posted at: 2017-07-21T09:18:38.410Z Reads: 350

```
It seems that at this amperage the wire would be dissipating around 2.5 watts of heat which will really heat up your wire. What do you mean by bundle of phase wires and how does that change things? 12awg wires would half the heat output and keep everyhting cooler.
```

---
## \#391 Posted by: onloop Posted at: 2017-07-21T09:28:42.760Z Reads: 363

```
Feel free to swap the wires... 

Or alternatively if ever the 14awg melts/combusts send us an email we'll send you some 12awg for free.

Also, please be sure to send a video showing your esk8 motors pulling 60a cont current through phase wires when riding.

We only run 30a battery current into each FOCBOX in the Raptor 2 and it is destroying everything on the street at the moment...
```

---
## \#392 Posted by: jbruce Posted at: 2017-07-21T09:31:10.697Z Reads: 353

```
Will swapping the wires void the warranty?

Also I see you point for dual motor boards, but for single motor boards you can easily pull that current somewhat continuously.
```

---
## \#393 Posted by: Alanhunt123 Posted at: 2017-07-21T11:36:57.583Z Reads: 345

```
Hi Lox! I'd love to have the files as well.

Thanks!
```

---
## \#394 Posted by: willpark16 Posted at: 2017-07-21T14:06:18.685Z Reads: 343

```
A single should actually pull less with a belt drive system mine pulls 3-5a cont including hills
```

---
## \#395 Posted by: JohnnyMeduse Posted at: 2017-07-21T14:16:11.221Z Reads: 342

```
The motor curent isn't continious... it is alternative Current... in simple term, the job of a esc is to convert dc into ac... so 14awg is more than enough 🤔
```

---
## \#396 Posted by: themegak Posted at: 2017-07-21T14:22:30.065Z Reads: 335

```
hello, please hook me up.  Would love to have.
```

---
## \#397 Posted by: The_Dude Posted at: 2017-07-21T14:26:28.332Z Reads: 340

```
Me too! 10chars
```

---
## \#398 Posted by: jbruce Posted at: 2017-07-21T17:52:54.002Z Reads: 342

```
I thought these motors are still running on dc current, the three wires is just to control the phases. 
Does a square wave count as ac?
```

---
## \#399 Posted by: JohnnyMeduse Posted at: 2017-07-21T18:09:15.151Z Reads: 358

```
Sorry I've been a little vague about it... Yes BLDC motor are DC motor, but each phase work by commutation. So you actually don't have a full dc current running trough each phase for long period of time. 

Explication is better on wikipedia. 

"Brushless DC electric motor (BLDC motors, BL motors) also known as electronically commutated motors (ECMs, EC motors) are synchronous motors powered by DC electricity via an inverter/switching power supply which produces an AC/bi-directional electric current to drive each phase of the motor via a closed loop controller. The controller provides pulses of current to the motor windings that control the speed and torque of the motor."

https://en.wikipedia.org/wiki/Brushless_DC_electric_motor

The switching power supply in our case is the ESC
```

---
## \#400 Posted by: jbruce Posted at: 2017-07-21T19:55:14.777Z Reads: 341

```
Ahh I see, thanks for explaining!

In this case, wouldn't each phase wire have current running through it for 2/3 of the time?
```

---
## \#401 Posted by: DavidBanner Posted at: 2017-07-21T20:10:58.766Z Reads: 338

```
awesome explanation! it all clicked once read that.
```

---
## \#402 Posted by: Martinsp Posted at: 2017-07-21T20:25:36.554Z Reads: 333

```
Hey! Add me to the list please. :) Thank you in advance.
```

---
## \#403 Posted by: DavidBanner Posted at: 2017-07-21T21:11:55.268Z Reads: 322

```
please add me to the list as well...
```

---
## \#404 Posted by: JohnnyMeduse Posted at: 2017-07-21T23:12:05.685Z Reads: 310

```
@lox897 look like I'm missing the party... count me in as well..
```

---
## \#405 Posted by: Mobutusan Posted at: 2017-07-22T05:53:06.231Z Reads: 310

```
Please add me too. Thanks
```

---
## \#406 Posted by: Ronny_CTS Posted at: 2017-07-22T07:22:36.397Z Reads: 308

```
Please count me in too. Thanks!
```

---
## \#407 Posted by: Vieo Posted at: 2017-07-22T11:43:16.490Z Reads: 320

```
[quote="lox897, post:388, topic:11102"]
reply to this comment and I will tag you once I have the
[/quote]

Me too please! +1
```

---
## \#408 Posted by: SilentException Posted at: 2017-07-22T11:55:54.124Z Reads: 318

```
Heck, don't even know what it is but now I want it too. +💯 !
```

---
## \#409 Posted by: scepterr Posted at: 2017-07-23T02:20:39.088Z Reads: 318

```
Does the Focbox work fine with the extended bldc tool and modified firmware?
```

---
## \#410 Posted by: TranxFu Posted at: 2017-07-23T02:27:06.582Z Reads: 316

```
Yes it does. Behaves just like a normal VESC
```

---
## \#411 Posted by: scepterr Posted at: 2017-07-23T05:52:50.835Z Reads: 324

```
Installed and running great on focbox, running FOC on Yuneec E-Go2 motor. Android app is awesome. Props and thanks to the developer.
```

---
## \#412 Posted by: onloop Posted at: 2017-07-23T06:43:55.813Z Reads: 326

```
@lox897 I'll have one too man, sign me up.
```

---
## \#413 Posted by: lox897 Posted at: 2017-07-23T06:55:15.836Z Reads: 329

```
Lol you want the VESC-X files? Can you please fix them on your website?
```

---
## \#414 Posted by: lox897 Posted at: 2017-07-23T09:45:59.883Z Reads: 345

```
Here we go boys:
https://www.mediafire.com/?rw3zfgei82t63lc
https://www.mediafire.com/?axtj1757l13o177

@Kaly
@miguelop24
@Surfer
@Alanhunt123
@marcdecator
@themegak
@The_Dude
@Martinsp
@DavidBanner
@JohnnyMeduse
@Mobutusan
@Ronny_CTS
@Vieo
```

---
## \#415 Posted by: Martinsp Posted at: 2017-07-23T10:29:26.217Z Reads: 329

```
Thank you!

It seems like the only thing that is different in the schematic is the big diode and the FETS, right?
```

---
## \#416 Posted by: Ronny_CTS Posted at: 2017-07-23T10:41:22.360Z Reads: 326

```
Thanks a lot mate! I just bought 2 focboxes so this might come in handy if i ever need to do a repair...although the version i bought are more recent version than these files...anyway thanks!
```

---
## \#417 Posted by: lox897 Posted at: 2017-07-23T10:54:09.058Z Reads: 323

```
[quote="Ronny_CTS, post:416, topic:11102"]
although the version i bought are more recent version than these
[/quote]
Only person that can give the latest files is @onloop :slight_smile:
```

---
## \#418 Posted by: DavidBanner Posted at: 2017-07-23T19:35:47.363Z Reads: 309

```
thank you @lox897
```

---
## \#419 Posted by: miguelop24 Posted at: 2017-07-28T15:59:45.590Z Reads: 308

```
Thanks you so much! I want to make some of these by my own, so this is really helpful
```

---
## \#420 Posted by: trancejunkiexxl Posted at: 2017-07-28T16:31:01.900Z Reads: 299

```
my focbox are coming any day now!!! so excited, just need a new soldeing iron.. i am really looking forward to a safe ride now that im almost healed up.... yeaaa progress!!
```

---
## \#421 Posted by: Martinsp Posted at: 2017-07-28T18:41:17.111Z Reads: 296

```
But you dont have the PCB design files. Or do you? :O :3 :D
```

---
## \#422 Posted by: miguelop24 Posted at: 2017-07-29T14:30:19.108Z Reads: 291

```
I dont, but I will try to get them from here. I have the layout, the basic connections and an open source license so I dont see why it couldnt be possible, a little of work required tho :v:

Obviusly it would still be nice if the source releases the schematics as the license invites them to share the files
```

---
## \#423 Posted by: monkey32 Posted at: 2017-07-29T17:38:19.556Z Reads: 291

```
I have Euro group buys happening for any interested parties. I am about to open a second GB.
```

---
## \#424 Posted by: solarcross Posted at: 2017-07-29T18:59:23.642Z Reads: 297

```
Just received my FOC..Im using 3 wire twist throttle..
So...can I still connect bluetooth etc...

thnx
```

---
## \#425 Posted by: flywithgriff Posted at: 2017-07-30T00:21:33.662Z Reads: 293

```
I have just ordered 2 FOCBOX and plan to run them in FOC on my MTB build. I can mount them in the battery enclosure or near the motors. Which is better?? Longer battery cables or longer phase wires?
```

---
## \#426 Posted by: trancejunkiexxl Posted at: 2017-07-30T00:26:40.126Z Reads: 295

```
JUST GOT MY FOCBOX's HOT DAMN they look sweeettt!!!
```

---
## \#427 Posted by: flywithgriff Posted at: 2017-07-31T01:28:28.093Z Reads: 290

```
I have found the schematics for the width of the FOCBOX but cannot find the height. Anyone know?
```

---
## \#428 Posted by: trancejunkiexxl Posted at: 2017-07-31T05:51:09.149Z Reads: 295

```
close to 3/4 and inch tall @flywithgriff  just shy of one inch
```

---
## \#429 Posted by: dannyboy Posted at: 2017-08-01T11:44:01.032Z Reads: 298

```
This may be too late, perhaps you have your answer already. Also I'm no expert so will humbly accept correction, but:
- Long battery wires can be bad as more inductance leads to more back emf and those spikes can shorten the life of the ESC. That's why there are big capacitors in parallel to the inputs from the battery and you can compensate for long battery wires by adding some more. There is a ton of advice out there, (low serial resistance, close to the ESC as poss etc.), but you can just buy little boards with appropriate caps on them, boards with natty holes and tabs such that you can get them really close to the ESC.
- Long motor cables (phase wires) are less of an issue and tend to just introduce more loss. There is a limit of course, you don't want massively long cables, but actually inductance on those ones is apparently slightly helpful. You may get less mileage as wasted energy heating the longer cables but performance and durability shouldn't suffer too much.
Those are generalizations, quite possibly wrong (really) and everything has it's limits. But I would err on shorter battery cables if you are forced to make a decision, and if the battery leads are still over 10cm then bolstering the source capacitance might be a good idea anyway especially with the giant currents an MTB is likely to draw. Caps are usually a lot cheaper and easier to get than new ESCs, (especially swanky VESCs) and having it break when out and about would suck.
```

---
## \#430 Posted by: adrianenertion Posted at: 2017-08-01T23:48:56.455Z Reads: 287

```
Swapping the wires does technically void your warranty, as any modifications to our product will. Don't worry though - you can always purchase the platinum warranty on the FOCBOX which covers user modifcations too!
```

---
## \#431 Posted by: Jinra Posted at: 2017-08-01T23:55:52.741Z Reads: 296

```
Just FYI Adrian, your focbox has had the wrong labeling for the sensor wires since the vesc-x. Including the new batch.
```

---
## \#432 Posted by: adrianenertion Posted at: 2017-08-02T00:12:14.392Z Reads: 320

```
Thanks for letting us know Jinra - we've just been made aware of this issue too. I'll try to get something posted today so we can clarify the issue (unless one of you awesome, knowledgeable community members beats us to the punch, of course).
```

---
## \#433 Posted by: Jinra Posted at: 2017-08-02T00:30:52.536Z Reads: 325

```
Yep, your +5v and GND wires are correct, but your temp wire label is in the wrong place.

<img src="/uploads/db1493/original/3X/c/f/cf66cb31d8b8eca16b468325e3cd16bc3fd93ab2.png" width="590" height="500">

The highlighted label "T" should be next to "5V" and H1, H2 H3, should be next to GND.
```

---
## \#434 Posted by: adrianenertion Posted at: 2017-08-02T00:37:06.769Z Reads: 309

```
Damn, that's inconvenient! Thanks so much for dropping some knowledge for us to help out our customers. We'll update the FOCBOX Help Guide using this info. 

How's the FOCBOX working for you otherwise?
```

---
## \#435 Posted by: Jinra Posted at: 2017-08-02T00:38:07.048Z Reads: 305

```
No idea! They'll be going on my hub build whenever I get around to buying those. I will say the FOCBOX build quality is very nice with the matte plastic enclosure and metal heatsink.
```

---
## \#436 Posted by: trancejunkiexxl Posted at: 2017-08-02T00:46:08.716Z Reads: 301

```
FOCBOX is working spiffy, just went for a nice run... quiet as a church =)
```

---
## \#437 Posted by: JohnnyMeduse Posted at: 2017-08-02T00:55:54.662Z Reads: 304

```
[quote="trancejunkiexxl, post:436, topic:11102"]
quiet as a church =)
[/quote]

I just hope your not referring to a gospel church :grin: :joy:
```

---
## \#438 Posted by: flywithgriff Posted at: 2017-08-02T01:03:34.254Z Reads: 302

```
I have a distance of about 16" between between my batteries and my FOCBOX. I want to run FOC, which wires should be the longest?
```

---
## \#439 Posted by: adrianenertion Posted at: 2017-08-02T01:06:24.984Z Reads: 300

```
Awesome trancejunkie! Glad to hear it's working well!
```

---
## \#440 Posted by: flywithgriff Posted at: 2017-08-02T01:35:58.267Z Reads: 301

```
@adrianenertion Could you shed some light on my previous question as to suggested wire length?
```

---
## \#441 Posted by: trancejunkiexxl Posted at: 2017-08-02T01:38:53.397Z Reads: 295

```
the motors are the choir!
```

---
## \#442 Posted by: adrianenertion Posted at: 2017-08-02T01:42:04.719Z Reads: 303

```
Unfortunately, I don't have that information on hand flywithgriff, but i've forwarded it to my tech guys so we can try to get you an answer ASAP. Please bear with us.
```

---
## \#443 Posted by: flywithgriff Posted at: 2017-08-02T01:48:27.366Z Reads: 298

```
Awesome, Thank you! This is my first venture with Enertion and I hope it is as great as others have said it can be.
```

---
## \#444 Posted by: adrianenertion Posted at: 2017-08-02T02:09:05.459Z Reads: 293

```
@Flywithgriff Here's what our engineer had to say:

16" on the power cable is fine. The FOCBOX has large bulk decoupling capacitors, so closer is always going to be better though
```

---
## \#445 Posted by: flywithgriff Posted at: 2017-08-02T02:11:22.049Z Reads: 294

```
Perfect, FOC should be just fine as long as the power wires from vesc to FOCBOX are 16" or shorter. Thank You
```

---
## \#446 Posted by: adrianenertion Posted at: 2017-08-02T02:12:55.223Z Reads: 294

```
You're most welcome!
```

---
## \#447 Posted by: leonsc Posted at: 2017-08-06T22:12:02.350Z Reads: 280

```
Sorry if this is the wrong place for this question but could I use a nyko kama with the focbox ? Cheers
```

---
## \#448 Posted by: flywithgriff Posted at: 2017-08-07T03:45:03.033Z Reads: 281

```
Running Dual FOCBOX in FOC. Canbus or split servo/y cable??
```

---
## \#449 Posted by: Blasto Posted at: 2017-08-07T04:02:53.722Z Reads: 280

```
CAN bus, to keep the transceivers safe and sound, while connected in CAN ALWAYS power to both controllers
```

---
## \#450 Posted by: Maxid Posted at: 2017-08-07T07:57:55.937Z Reads: 283

```
yes you can
```

---
## \#451 Posted by: leonsc Posted at: 2017-08-07T08:42:00.027Z Reads: 288

```
Thank you very much.
```

---
## \#452 Posted by: Michaelinvegas Posted at: 2017-08-08T21:40:55.892Z Reads: 294

```
Intelligent esk8 humor at it's finest 


https://www.instagram.com/p/BXjFGhABxf4/
```

---
## \#453 Posted by: notger Posted at: 2017-08-10T00:48:40.081Z Reads: 292

```
@onloop

Hi,

So, the FOCBOX is based on VESC4 Hardware and firmware.
But did you actually implement Motor-Temperature readout and reglementation ?

cause i read that sind 2.18 is was never implemented on the "Standard-Vescs"
```

---
## \#454 Posted by: JohnnyMeduse Posted at: 2017-08-10T01:09:36.626Z Reads: 289

```
The Implement is only firmware related... The hardware was already able to cope with a temps sensors.
```

---
## \#455 Posted by: Jinra Posted at: 2017-08-10T01:18:34.787Z Reads: 291

```
I'm actually surprised there hasn't been any official f/w updates since 2.18. I guess Vedder's been too busy with the VESC tool. On that note I wonder why @Ackmaniac's f/w goes to 2.54
```

---
## \#456 Posted by: JohnnyMeduse Posted at: 2017-08-10T01:21:36.276Z Reads: 297

```
I think the big updated is going to be the new VESC-tool...

And Niko has probably just ask a drunk guy a number between 0 and 100
```

---
## \#457 Posted by: notger Posted at: 2017-08-10T09:35:22.017Z Reads: 289

```
Hmm, but will the new VESC-Tool also update the "old" VESC4-Firmwares ??
or maybe just the VESC6 FW.

could be that VESC4 developement is history now i guess, if not anyone here does it ? But it is for sure not me .
```

---
## \#458 Posted by: Silverline Posted at: 2017-08-10T10:08:24.726Z Reads: 286

```
The new vesc tool should Work on 4,12 HW All so 😃
```

---
## \#459 Posted by: notger Posted at: 2017-08-10T13:44:59.706Z Reads: 282

```
Are there any "Release - Rumors" on the new VESC Tool.
```

---
## \#460 Posted by: trampa Posted at: 2017-08-10T16:13:47.842Z Reads: 276

```
Release is in sight. When im back from holidays I'll have a chat about the release with Benjamin. Some users reported issues with the FOC-BOX. We haven't tried that out ourselves. 

Frank
```

---
## \#461 Posted by: scepterr Posted at: 2017-08-11T04:26:37.452Z Reads: 273

```
Hey guys, make sure not to flash any firmware on the FOCBOX as that will void your 60 day warranty regardless of failure. Mine died in the first month and no warranty because the firmware was flashed, told to pay $80 for plat. warranty for replacement. 

@onloop Would've been nice if that was specifically mentioned on the product page, as any product running opensource firmware, flashing new firmware is quite common practice and expected.
```

---
## \#463 Posted by: num3a Posted at: 2017-08-11T22:35:55.692Z Reads: 267

```
Is this possible to connect make a dual setup with a focbox and a Vesc 4.12?
```

---
## \#464 Posted by: flywithgriff Posted at: 2017-08-12T01:36:39.166Z Reads: 268

```
Does this mean I cannot run @Ackmaniac fw??
```

---
## \#465 Posted by: scepterr Posted at: 2017-08-12T01:49:58.708Z Reads: 269

```
I did and it voided my 60 day warranty, so wait till after included 60 day warranty is up. From what I've learned don't change any settings without getting written approval from enertion, because if anything fails and you admit to changing anything your warranty is void. I was educated to this by Mike Schmeller from Enertion who pointed out that T&C states "any software modification will void warranty" With such vague wording Enertion can void your warranty for doing anything other than plugging the focbox in properly.
```

---
## \#466 Posted by: flywithgriff Posted at: 2017-08-12T01:51:03.803Z Reads: 265

```
What was the cause of your failure?
```

---
## \#467 Posted by: scepterr Posted at: 2017-08-12T02:01:23.912Z Reads: 275

```
DRV fried running yuneec ego2 battery and motor FOC sensored. My whole interaction with enertion about this is here  https://drive.google.com/file/d/0B8LrLknwWHGEQjVkbXAzUGhuZFE/view?usp=drivesdk

On a sidenote replaced the DRV today and its working, will be selling shortly
```

---
## \#468 Posted by: flywithgriff Posted at: 2017-08-12T02:04:32.999Z Reads: 269

```
I'm totally not attacking you or taking merit away from your case, just to make sure that clear. 

I was under the assumption they FOCBOX was virtually DRV Fault proof. I have heard several guys say they have had the built in failsafe kick in to avoid burning the DRV. This is a major concern as I have two brand new FOCBOX that will be running FOC and Sensored.
```

---
## \#469 Posted by: scepterr Posted at: 2017-08-12T02:05:24.826Z Reads: 265

```
That's exactly why I bought it
```

---
## \#470 Posted by: flywithgriff Posted at: 2017-08-12T02:05:47.685Z Reads: 262

```
What battery setup were you running?
```

---
## \#471 Posted by: scepterr Posted at: 2017-08-12T02:07:07.368Z Reads: 266

```
Stock yuneec ego2 battery 7S3P Panasonic 18650 fused for 30A, motor is 400watt.
```

---
## \#472 Posted by: flywithgriff Posted at: 2017-08-12T02:08:25.765Z Reads: 261

```
Can anyone advise if 7s could have been the problem here? @EnertionSupport @onloop
```

---
## \#473 Posted by: JohnnyMeduse Posted at: 2017-08-12T02:48:20.364Z Reads: 265

```
[quote="flywithgriff, post:468, topic:11102"]
I was under the assumption they FOCBOX was virtually DRV Fault proof
[/quote]

It's faults proof... except if you don't run a proper motor detection...
```

---
## \#474 Posted by: JohnnyMeduse Posted at: 2017-08-12T02:49:34.886Z Reads: 260

```
Before you blame anyone... could you at least show your parameter from the bldc tool.
```

---
## \#475 Posted by: flywithgriff Posted at: 2017-08-12T02:49:45.899Z Reads: 263

```
Ahh this is good to know! So @Ackmaniac fw will be fine if followed properly?
```

---
## \#476 Posted by: JohnnyMeduse Posted at: 2017-08-12T02:53:05.954Z Reads: 272

```
Yes Niko firmware is working fine on focbox, I've been running is firmware on every focbox I've got, since Alpha 1
```

---
## \#477 Posted by: SeanHacker Posted at: 2017-08-12T03:34:14.673Z Reads: 276

```
@Ackmaniac firmware + FOCBox = <img src="/uploads/db1493/original/3X/4/6/46c0ad45a3fc7cf53196fabedd33a23bc9aeeb91.jpg" width="690" height="388">
:smile:
```

---
## \#478 Posted by: scepterr Posted at: 2017-08-12T07:14:10.464Z Reads: 291

```
I dont blame anybody other than myself for deciding to purchase a focbox.

<img src="/uploads/db1493/original/3X/1/8/1867a748545bf2e3019a5f11dfd686ffc7338300.png" width="690" height="389"><img src="/uploads/db1493/original/3X/c/5/c53c4f5450c94bb641df191a2892e67a251635fd.png" width="690" height="389">
Guess it's the first focbox with replaced DRV
<img src="/uploads/db1493/original/3X/6/6/66a14f092eed23b4ae12e76c222b27eadaa15889.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/e/ae51f14a5f0a07d33cb6cd7f080791338705dc74.jpg" width="666" height="500">
```

---
## \#479 Posted by: adrianenertion Posted at: 2017-08-12T08:14:32.650Z Reads: 286

```
Hi @scepterr, 

Just to be clear, the wording of our warranty is hopefully far from vague. Here it is: "If any Electronic part has had hardware or software modifications the warranty is void."

This is written as part of our Terms and Conditions, because we, unfortunately, cannot guarantee that your purchased unit will work if you perform modifications on it. 

I might also point out that this is similar to Apple's stance on jailbroken phones. You can read about it on their support page here:

https://support.apple.com/en-au/HT201954

This is quite a common condition in the industry due to the precise nature of these types of parts. Don't forget, if you change things irreversibly and need a new unit, you can simply purchase a Platinum Instance Replacement warranty, and we'll send you out a new FOCBOX!
```

---
## \#480 Posted by: Maxid Posted at: 2017-08-12T10:28:02.081Z Reads: 282

```
That is BS though - you are using the same firmware for your Raptor2 - doing the upgrade yourself should not void anything. it is not like there are 100 firmwares around that might fry something
```

---
## \#481 Posted by: MontPierre Posted at: 2017-08-12T10:29:53.014Z Reads: 284

```
I think they mean modified firmware like @Ackmaniac not Vedder firmware. Anyway still not fair :/
```

---
## \#482 Posted by: Maxid Posted at: 2017-08-12T10:33:48.000Z Reads: 292

```
They are using @Ackmaniac's firmware - otherwise their BT connection would not work.
http://www.enertionboards.com/new-raptor-2-electric-skateboard/raptor-2-boostpack/
Just look at the screenshot of the app - looks familiar doesn't it ;)
```

---
## \#483 Posted by: MontPierre Posted at: 2017-08-12T10:38:08.808Z Reads: 296

```
Cheeky! I wonder if @Ackmaniac is aware of it...  @scepterr can you confirm above post?
```

---
## \#484 Posted by: Maxid Posted at: 2017-08-12T10:40:50.135Z Reads: 301

```
He is:
http://www.electric-skateboard.builders/t/raptor-2-most-powerful-direct-drive-electric-skateboard-kickstarter/12694/1801?u=maxid

"Also today sent one R2 unit to our software engineer in Germany to do the final firmware tweaks to maximize efficiency and performance."
```

---
## \#485 Posted by: scepterr Posted at: 2017-08-12T14:39:48.438Z Reads: 302

```
So using the focbox, voids the warranty?

What nobody at Enertion seems to get this isnt about money. It's about reputation. I spent over $80 to overnight the replacement IC so I can fix it myself. Maybe I got the 1 out of 1000 focbox that are bad. That's what I thought the warranty is for, not extorting more money. <img src="/uploads/db1493/original/3X/6/a/6a5ad45ee7d4ac4680a61b3754642ab28bd6f24c.jpg" width="281" height="500">
```

---
## \#486 Posted by: scepterr Posted at: 2017-08-12T14:41:34.096Z Reads: 286

```
Yes I was using @Ackmaniac 's firmware
```

---
## \#487 Posted by: JohnnyMeduse Posted at: 2017-08-12T16:57:35.252Z Reads: 286

```
[quote="Maxid, post:480, topic:11102"]
That is BS though - you are using the same firmware for your Raptor2
[/quote]

No, they are using a custom firmware for the raptor 2
```

---
## \#488 Posted by: Maxid Posted at: 2017-08-12T17:09:15.503Z Reads: 280

```
AFAIK without making it public that would be illegal. It is still based on the VESC open source project. So where is that firmware @EnertionSupport @adrianenertion?

Also the raptor is officially shipping now. That means the firmware should have already been made available to all including the source if it is indeed a custom firmware besides the 2.54
```

---
## \#489 Posted by: JohnnyMeduse Posted at: 2017-08-12T17:20:19.678Z Reads: 285

```
The firmware is base on Niko firmware... but Enertion are the one uploading it into the VESC not the customer... so the warranty apply.


[quote="Maxid, post:488, topic:11102"]
AFAIK without making it public that would be illegal
[/quote]

It's not illegal if they don't use the ORIGINAL firmware
```

---
## \#490 Posted by: Maxid Posted at: 2017-08-12T17:21:36.776Z Reads: 279

```
Doesn't matter - it is either the published 2.54 or a new one and then they need to make it public asap.

And you want me to believe they wrote a completely new version that has no vedder code inside? You just said yourself that it is based on the 2.54 - and the 2.54 is based on Vedder's firmware
```

---
## \#491 Posted by: JohnnyMeduse Posted at: 2017-08-12T17:24:39.924Z Reads: 274

```
And all the change made to obtain the 2,54 firmware are available.... so what your point ?
```

---
## \#492 Posted by: Maxid Posted at: 2017-08-12T17:25:54.894Z Reads: 274

```
You said that they don't use 2.54 but a differemt custom firmware. That custom firmware and all changes to the source would need to be made public just like 2.54 was. That is my point.
```

---
## \#493 Posted by: JohnnyMeduse Posted at: 2017-08-12T17:31:03.942Z Reads: 271

```
[quote="Maxid, post:492, topic:11102"]
You said that they don't use 2.54 but a differemt custom firmware.
[/quote]

They are using a custom version of the 2,54. So it's not really the 2.54 but it's at the same time.
```

---
## \#494 Posted by: Maxid Posted at: 2017-08-12T17:33:06.115Z Reads: 272

```
If there is even the slightest difference between the two versions they still need to make all the files available separately. The amount of change does not matter. Removing or adding one line of code is enough.
If it is only miniscule then the warranty argument is BS and if it is a big change then I am looking forward to seeing what changed.

This whole argument is so weird to have - you know perfectly well what is going on and you also know about the open source requirements.
```

---
## \#495 Posted by: scepterr Posted at: 2017-08-12T17:37:52.527Z Reads: 266

```
Any idea why its not sold with this firmware preloaded?
```

---
## \#496 Posted by: JohnnyMeduse Posted at: 2017-08-12T17:41:41.041Z Reads: 279

```
It's probably easier to upload Vedder firmware with the bootloader integrated on mcu alone, than Niko firmware, also the regulars BLDC tool is more common and easier to find (It's on Enertion website), and easier to support.
```

---
## \#497 Posted by: Jamy Posted at: 2017-08-12T19:16:30.197Z Reads: 291

```
@Maxid According to BLDC tool, the firmware on my Raptor 2 is 2.80, so I can't read any more of the settings without having a BLDC tool that supports 2.80.

But it's safe to say that it's based on the normal VESC firmware, otherwise, it'd be unlikely that BLDC tool can give me a firmware version... So since that's GPL v3, they [must release source under a GPL v3 compatible license](https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3))
```

---
## \#498 Posted by: JohnnyMeduse Posted at: 2017-08-12T19:20:40.360Z Reads: 281

```
@Jamy have you try @Ackmaniac software or just the regular BLDC tool ?
```

---
## \#499 Posted by: Jamy Posted at: 2017-08-12T19:27:33.097Z Reads: 279

```
@JohnnyMeduse Tried Ackmaniac's one and the one from Enertion's website. Both say they don't support 2.80 and bail out early. Would need to compile one for 2.80 and that might not even work if they added or removed preferences.
```

---
## \#500 Posted by: Maxid Posted at: 2017-08-12T19:30:29.825Z Reads: 275

```
They know exactly that they are not allowed to do this - I hate these games...
@onloop
```

---
## \#501 Posted by: trampa Posted at: 2017-08-12T19:38:30.527Z Reads: 277

```
If its not public you can simply request the entire software, since its GPL code. Easy... The added code has to be under the same GPL license, so the changed BLDC-Tool and FW is OS and public. 

Anything else is a violation of the GPL license Benjamin gave. Benjamin is the only person who doesn't have that duty, since he is the originator of his code. Anyone offering code, based on his code, has to use the GPL. The GPL is viral, it infects any code incorporating GPLed code.

Frank
```

---
## \#502 Posted by: Blasto Posted at: 2017-08-12T19:42:39.871Z Reads: 279

```
The 2.80 fw is compatible w @Ackmaniac bldc tool. The different version number is only to differentiate the raptor2 default settings.

@Jamy tried dl'ing the latest bldc tool
```

---
## \#503 Posted by: Jamy Posted at: 2017-08-12T19:44:22.294Z Reads: 280

```
I did, but the bldc tool won't allow me to configure. This is a design of the bldc tool so you don't damage the configuration by using an incorrect bldc tool for the firmware version. I could manually buid @Ackmaniac 's BLDC tool for v2.80 but that's effort which I shouldn't have to go through (plus risky, because I can't be sure they didn't adjust the config).
```

---
## \#504 Posted by: Maxid Posted at: 2017-08-12T19:50:00.880Z Reads: 283

```
So we are back to the BS warranty argument. If they can use @Ackmaniac's firmware everyone should be allowed to.
```

---
## \#505 Posted by: trampa Posted at: 2017-08-12T19:56:13.103Z Reads: 283

```
By law its public and you can request it and publish it, if not public.
You want to be able to change your settings. Warranty is a totally different thing. If you have access to the BLDC-tool and FW, it's hard to tell if you made changes while using the product. You can always play the original settings back onto the device. XML export-import.

Frank
```

---
## \#506 Posted by: Maxid Posted at: 2017-08-12T19:59:06.207Z Reads: 284

```
Sure you can - I just don't like the hypocrisy of them telling people they are jailbreaking when enertion is doing it themselves on a product they sell.
```

---
## \#507 Posted by: trampa Posted at: 2017-08-12T20:02:29.243Z Reads: 289

```
You just need to request it, that's it. Easy! 
You should get the code within a short period of time. Read the GPL. It's quite short and doesn't require a lot of time.

Frank
```

---
## \#508 Posted by: Maxid Posted at: 2017-08-12T20:09:03.681Z Reads: 287

```
I don't need the code personally. For me this is all just a bad publicity thing from enertion and I want people to see that. You can't tell people upgrading their firmware is not covered because the firmware might be faulty but then use it on the Raptor 2.
```

---
## \#509 Posted by: Jamy Posted at: 2017-08-12T20:11:44.104Z Reads: 301

```
Well, I personally don't like the whole jailbreaking point either, since you're not actually circumventing any security to upload this firmware. 

Now since they have a custom firmware on the R2 you can't say they used Ackmaniac's firmware, since it's a custom one, which they might have validated for FOC and DRV faults.

Finally, I have had FOC on my old original VESC and never had a DRV fault. I'd say it's highly likely this was a user configuration fault, but I can't verify that so I'm not going to point fingers. They are allowed to deny warranty based on their Terms and Conditions, which you agreed when you purchased the product...

> If any Electronic part has had hardware or software modifications the warranty is void. If you do not have a protection circuit, such as a fuse connected to your battery the warranty is void.

EDIT: @trampa I'll be requesting the firmware and BLDC tool from Enertion shortly :)
```

---
## \#510 Posted by: JohnnyMeduse Posted at: 2017-08-12T20:16:55.835Z Reads: 295

```
[quote="Jamy, post:509, topic:11102"]
Now since they have a custom firmware on the R2 you can't say they used Ackmaniac's firmware, since it's a custom one, which they might have validated for FOC and DRV faults.
[/quote]

[quote="Blasto, post:502, topic:11102"]
The 2.80 fw is compatible w @Ackmaniac bldc tool. The different version number is only to differentiate the raptor2 default settings.
[/quote]

They're the same Firmware....

@Maxid the problem is to know which file he use.... since last year, remember the Jacob fault where he output a bad firmware a people have broke there VESC because of that. Since Then the Firmware is validated before putting it in the VESC. The problem is how can they be sure that the file updated in the vesc is the original from @Ackmaniac and as not been temper with.
```

---
## \#511 Posted by: Maxid Posted at: 2017-08-12T20:17:13.242Z Reads: 284

```
In my opinion this is not a software modification when the seller is doing the same thing. Apple does allow you to upgrade the phone to a new version they offer. Let us know what they say about the new version.
```

---
## \#512 Posted by: Maxid Posted at: 2017-08-12T20:18:57.462Z Reads: 282

```
They could offer it on their website (which they will need to do soon anyway because of the raptor2). Also it is not like there are 100s of firmware versions around. This is a way to make a good impression with customers - not drive them away with a nonsensical statement on this being a jailbreak and apple also forbidding it.
```

---
## \#513 Posted by: Jamy Posted at: 2017-08-12T20:22:51.639Z Reads: 291

```
[quote="JohnnyMeduse, post:510, topic:11102"]
They're the same Firmware....
[/quote]

Fair enough. But that still leaves the actual configuration settings, which has broken DRV's in the past. Again, according to their ToS they can void your warranty if you modify the software, which he has :/
```

---
## \#514 Posted by: JohnnyMeduse Posted at: 2017-08-12T20:25:18.969Z Reads: 300

```
[quote="Maxid, post:512, topic:11102"]
They could offer it on their website (which they will need to do soon anyway because of the raptor2)
[/quote]

Don't forget that the Raptor is a completely different product... and if a firmware is available for the R2 it doesn't mean that it will be supported on the FOCBOX alone.
```

---
## \#515 Posted by: onepunchboard Posted at: 2017-08-14T23:48:01.032Z Reads: 309

```
@onloop 
HI Jason, I have a question for erpm of focbox. some say 60k cuz it's based on 4.12, but other says it goes beyond since your design reduced load on drv and direct fet is faster.  I actually seen it reached 86k and even 100k without problem. what would you say to this?
I need this info to safely design my board that can go 60km/h.
I know you r busy in china but if you can reply that would be awesome
```

---
## \#516 Posted by: Maxid Posted at: 2017-08-18T13:51:19.131Z Reads: 300

```
Did enertion get back to you?
They have been eerily quiet in this conversation.
```

---
## \#517 Posted by: Jamy Posted at: 2017-08-18T14:22:50.406Z Reads: 304

```
Only emailed them on Wednesday, they forwarded it to someone and I'm awaiting response. Jason said on reddit that they're planning on releasing their bldc tool soon tho.
```

---
## \#518 Posted by: notger Posted at: 2017-08-18T14:29:20.884Z Reads: 310

```
So if id like to use the hopefully soon released new VESC-tool i have to change the firmware to a no-warranty firmware then, right.
Anyone actually experience if the new vesc-tool and the new FW is compatible to the FOCbox ?

greets Notger
```

---
## \#519 Posted by: deucesdown Posted at: 2017-08-21T14:20:22.838Z Reads: 307

```
Link? or which sub? I'm trying to stay on top of enertion news...
```

---
## \#520 Posted by: Jamy Posted at: 2017-08-21T14:22:41.253Z Reads: 325

```
[here](https://www.reddit.com/r/ElectricSkateboarding/comments/6tx1er/raptor_2_bldc_mode_can_anyone_explain_what_it_is/dlp0cyn/)
```

---
## \#521 Posted by: Deakbannok Posted at: 2017-09-01T18:45:07.099Z Reads: 328

```
I have received a new FOCBOX and comparison to the VESC-X which I bought it back on DEC 2016
So what are the improvement between these two here?
Also I have noticed the motor wires are 14; the old VESC-X are 12
 <img src="/uploads/db1493/original/3X/3/2/328660348f8d66894ea3fd75670dadbe54872d1e.jpg" width="281" height="500">
```

---
## \#522 Posted by: onepunchboard Posted at: 2017-09-02T04:09:46.726Z Reads: 324

```
interesting. big capped are different numbers and tiny registers and cappy have different numbers. wire is probably to cut the cost down. but still works I guess. I read somewhere more copper mass in esc wire can lead to loss in signal power and intro noise, but sounds bs
```

---
## \#523 Posted by: Deakbannok Posted at: 2017-09-02T04:45:11.397Z Reads: 331

```
And the cover case is slightly thicker. the normal micro USB cannot reached in. Have to remove the top cover case to connect to the BLDC tools
```

---
## \#524 Posted by: onepunchboard Posted at: 2017-09-02T13:43:05.850Z Reads: 333

```
I dint have any problem with USB
```

---
## \#525 Posted by: MaozK Posted at: 2017-09-28T06:25:53.869Z Reads: 315

```
Thats not enough, theres two dimensions missing.
What is the distance between those 4 holes to the outer contour?
```

---
## \#526 Posted by: telnoi Posted at: 2017-11-20T10:24:03.217Z Reads: 281

```
does anybody know if two of these will fit inside of a 206 ultrabox?
```

---
## \#527 Posted by: Riako Posted at: 2017-11-23T02:22:44.620Z Reads: 274

```
yes, and a bit more easier than with 2 v6 :blush:
```

---
## \#528 Posted by: telnoi Posted at: 2017-11-23T07:03:58.021Z Reads: 282

```
Awesome. Drag & drop :grin:
Taking half the day off. UPS faster than expected.
```

---
## \#529 Posted by: telnoi Posted at: 2017-11-23T16:00:44.203Z Reads: 281

```
is there a known issue with the focbox and the vest-tool firmware?

Motor detection in bldc fails. I have tested two different motors and two different focboxes. Same result. 
Motors spin up fine, but after it slows down it stutters (a bit more loudly than I am used to compared to the ESK8 controller) and I receive the status message ''motor detection fails.'' No error codes in the terminal.

Motors are 100% ok. Working fine with other brands controller and the vesc tool firmware.

I have the latest version of the focbox with soldered ppm connector.
```

---
## \#530 Posted by: Blasto Posted at: 2017-11-23T16:06:20.344Z Reads: 276

```
[quote="telnoi, post:529, topic:11102"]
Motors spin up fine, but after it slows down it stutters (a bit more loudly than I am used to compared to the ESK8 controller)
[/quote]

you may need to play with your detection parameters, what is your motor Kv and battery setup?
```

---
## \#531 Posted by: telnoi Posted at: 2017-11-23T16:07:30.898Z Reads: 262

```
sk3 149kv, 10s. Default settings worked fine with the other controller, but not the focbox.
```

---
## \#532 Posted by: Blasto Posted at: 2017-11-23T16:10:48.868Z Reads: 273

```
lower your min ERPM to 500

<img src="/uploads/db1493/original/3X/e/5/e5fd927b05f06735e3c8a3b42815d1cbf9c8ea0a.png" width="489" height="146">

could also increase your low duty  to 0.1

could also double check your battery voltage for funsies
```

---
## \#533 Posted by: telnoi Posted at: 2017-11-23T16:13:59.284Z Reads: 277

```
battery voltage is ok.
these are the default values. ERPM is set to 150 by default. Increased D to 0,10. No difference. Motor still stuttering at the end.

<img src="/uploads/db1493/original/3X/7/4/7479f0020feea375224b7b132d7551cd5a215c61.png" width="490" height="256">
```

---
## \#534 Posted by: telnoi Posted at: 2017-11-23T16:28:08.935Z Reads: 270

```
motor detection worked with higher A and ERPM, but it still stutters at the end of the sequence. Normal?
```

---
## \#535 Posted by: Blasto Posted at: 2017-11-23T16:29:21.630Z Reads: 277

```
[quote="telnoi, post:534, topic:11102"]
still stutters at the end of the sequence. Normal?
[/quote]

yeah that is the D value, you can play with it to get to to run smoother. but if you get the detection working, IMO, not worth it

Didnt realize that the default values on the vesctool TM were so low
```

---
## \#536 Posted by: telnoi Posted at: 2017-11-23T16:31:05.302Z Reads: 275

```
ok, moving on with ppm. Fingers crossed.
```

---
## \#537 Posted by: Blasto Posted at: 2017-11-23T16:32:17.258Z Reads: 293

```
[quote="telnoi, post:536, topic:11102"]
moving on with ppm. Fingers crossed.
[/quote]

go with the wizard, i wasted a lot of time trying to set it up manually, never worked... to this day don't know what i am missing
```

---
## \#538 Posted by: caprabianca Posted at: 2017-11-24T08:01:01.717Z Reads: 294

```
Hi guys, I am a newbie and I have a question for this product: I want to use a single Hub motor on my esk8, and I need to program the esc (I want to implement a sort of AI. Is this the right product for me? Do I need to use an Arduino to send speed signals or I can use just the FOCBOX? Thanks
```

---
## \#539 Posted by: telnoi Posted at: 2017-11-24T08:35:02.240Z Reads: 311

```
Up and running. Tried FOC, but the brakes do not appear to be progressive. Back on BLDC and had a good 9 km run. 
Thanks for your help.
```

---
## \#540 Posted by: MrDude_1 Posted at: 2017-12-11T05:19:26.354Z Reads: 302

```
Quick FOCbox question. 
According to the spec page on enertions website:
> 5V 1A Output for external devices

soo.. without going into the whole project, is that 1A actually available for me to use with external devices, or is some of that 5v power actually used internally, on the 5v bus, and its just a 1a converter?

The reason I ask is I am modding a scooter, and the OEM LED lights are 5v and when all are maxxed out, its .92 amps. This is worse case, brake light and running light on all at once. unlikely to happen, but I dont want to kill the 5v bus, or have it suddenly not work and lose primary braking.
Along with the LEDs, I also run an arduino, and 2 hall effect throttles. The arduino takes the two throttles (one gas, one brake) and outputs a servo signal for the FOCBOX. 

So... is this too much for the 1A bus, or is the 1A rating accurate? because If it is, I will be using .95a of it...
```

---
## \#541 Posted by: Hummie Posted at: 2018-02-03T18:01:47.204Z Reads: 269

```
whats the most "motor amps" the focbox will do?  Does it have an override limit built in despite what you program it to do similar to vescs?
```

---
## \#542 Posted by: zwrtw Posted at: 2018-02-07T20:28:05.933Z Reads: 272

```
I use 120A max motor amp (as a setting), but only 40A battery amp. That gives a good start, but as the motor speeds up, the max motor current is reduced due to the max battery current.
 
I have a FocBox with a 2mm thermal pad (older ones seem to have 1 mm pads). For my application (electric converted moped) I added a heatsink to the FocBox. The heatsink got hardly warm but the motorcurrent was reduced due to the fets getting hot. I replaced the original thermal pad with a 8W/mK thermal pad. Now the fets are cooled much better and the motorcurrent is not reduced anymore. 

So if you want to use somewhat higher continuous motorcurrents, a heatsink seems to be effective if the thermal pad is replaced by better heat conducting material.
```

---
## \#543 Posted by: b264 Posted at: 2018-02-08T09:44:11.274Z Reads: 257

```
Do you have a link to the 8W/mK thermal pad?
```

---
## \#544 Posted by: zwrtw Posted at: 2018-02-08T22:45:03.638Z Reads: 261

```
I used "T-Grizzly Minus Pad 8 Thermal Pad".
[https://www.highflow.nl/watercooling/koelpasta-pads-cleaners/t-grizzly-minus-pad-8-thermalpad.html?sl=en](https://www.highflow.nl/watercooling/koelpasta-pads-cleaners/t-grizzly-minus-pad-8-thermalpad.html?sl=en)
```

---
## \#545 Posted by: E1Allen Posted at: 2018-02-09T03:54:17.910Z Reads: 255

```
Anyone have issues with their FocBox returning to default settings on a ride?
```

---
## \#546 Posted by: uigiroux Posted at: 2018-02-10T15:04:54.972Z Reads: 247

```
I just came across this FOCBOX and wanted to know how it compares to the Enertion FOCBOX?

http://store-en.tmotor.com/mobile/category.php?id=59

I imagine the Alpha 80A HV would be the one closest to compare.

Here is a list of all there ESC's, also curious if any of these are worth considering. 

http://store-en.tmotor.com/mobile/category.php?id=5
```

---
## \#547 Posted by: JohnnyMeduse Posted at: 2018-02-10T15:24:54.387Z Reads: 253

```
Look like thos esc are build to be use with specific motors.
```

---
## \#548 Posted by: uigiroux Posted at: 2018-02-10T16:31:17.212Z Reads: 259

```
Oh right on, that makes sense, thank you!
```

---
## \#549 Posted by: Hummie Posted at: 2018-02-10T19:23:37.584Z Reads: 257

```
But seems they could match up.  Look nice.  Sine wave n not expensive.
```

---
## \#550 Posted by: scepterr Posted at: 2018-02-10T19:30:46.814Z Reads: 267

```
Yeah seems to obey the same erpm limit as the vesc, likely drv driven
That 180A HV would make an insane directdrive/hub board though 😍 would go well with pnuematic hubs 6-8"
![Screenshot_20180210-142859__01|527x500](upload://e6yOsx6jQryYZMcYaE778l2KcbK.jpg)
```

---
## \#551 Posted by: Kug3lis Posted at: 2018-02-10T19:56:36.318Z Reads: 259

```
http://store-en.tmotor.com/images/image/81161510297189.gif

The image inside is backwards :D
```

---
## \#552 Posted by: uigiroux Posted at: 2018-02-10T20:02:13.903Z Reads: 248

```
Would it go well with Carvon's?
```

---
## \#553 Posted by: scepterr Posted at: 2018-02-10T20:02:31.788Z Reads: 249

```
It would max out the carvons
```

---
## \#554 Posted by: uigiroux Posted at: 2018-02-10T20:05:42.878Z Reads: 253

```
So that's a yes?
```

---
## \#555 Posted by: scepterr Posted at: 2018-02-10T20:07:11.200Z Reads: 258

```
It would max out the carvons without itself being maxed out
Though I haven't looked at how/if they work in dual configurations beyond ppm split
```

---
## \#556 Posted by: uigiroux Posted at: 2018-02-10T20:08:45.336Z Reads: 262

```
So between this, a FOCBOX, and the ESCape (VESC 6), which would be best for Carvon's?
```

---
## \#557 Posted by: scepterr Posted at: 2018-02-10T20:09:28.843Z Reads: 261

```
Escape, then focbox, this is an unknown quantity, I have no idea how well it actually works for esk8...
```

---
## \#558 Posted by: uigiroux Posted at: 2018-02-10T20:13:41.716Z Reads: 269

```
Yeah... Well I'm happy getting the ESCape already..  Just gotta get the rest of the board haha.  Def going with a Photon remote, that is so sweet!
```

---
## \#559 Posted by: Eboosted Posted at: 2018-02-10T21:46:43.578Z Reads: 275

```
I'm runing ESCapes and they are pretty good, I purchased  two more and will be runing FOC 12S 200KV motors that's gonna be 61k ERPMs
```

---
## \#560 Posted by: Deckoz Posted at: 2018-02-11T00:18:41.762Z Reads: 276

```
Fyi TMOTOR is probably one of the best ESC manufacturer out there for multirotors. 

No idea about them in the skate game. But if they built it it's more then likely quality. Just not sure about throttle features. @uigiroux
```

---
## \#561 Posted by: PXSS Posted at: 2018-02-11T17:21:34.397Z Reads: 277

```
Their firmware is built for aircraft so I don't think it would work since you'd have no brakes
```

---
## \#562 Posted by: Hummie Posted at: 2018-02-11T18:20:30.319Z Reads: 285

```
says it has "active braking" that works when slowing down.   don't know what that would mean though.  wish someone would get one a try it out or find out
```

---
## \#563 Posted by: louwii Posted at: 2018-02-14T03:45:53.685Z Reads: 295

```
I'm quite lost with the Focbox, I couldn't find a convincing answer about updating it.

Should I use the VESC Tool and update my FOCBOX with it ?
Should I use the BLDC Tool available on Enertion website ?
Should I use @Ackmaniac custom BLDC tool with custom firmware ?

I'd like to use the VESC Tool and update it but people in that thread http://www.electric-skateboard.builders/t/vesc-tool-on-focbox/33352 says that it doesn't work in FOC with the last firmware ?
```

---
## \#564 Posted by: telnoi Posted at: 2018-02-14T11:00:30.155Z Reads: 297

```
Supposedly you loose your warranty if you install anything other than what is available on their website, though I can't find a mention of that on their website.

Other firmware is a personal choice. Ackmaniak's firmware is based on the vesc-tool and offers additional options. The FOC issues have been resolved a while ago/that thread contains old info.
```

---
## \#565 Posted by: rene Posted at: 2018-02-14T11:03:30.134Z Reads: 304

```
I used the VESC-Tool from Vedder and also from Ackmaniac because he has this nice breaking / reverse function. Firmware 3.1000
```

---
## \#566 Posted by: rene Posted at: 2018-02-14T11:06:22.039Z Reads: 316

```
Dont forget the FocBox is just a normal "Vesc Version 4" with a heatsink and two caps.
Has the same hardware design flaws (ground loop on the CAN chips) as all copy cats version 4.
```

---
## \#567 Posted by: louwii Posted at: 2018-02-14T20:45:10.252Z Reads: 325

```
We'll that would be stupid, why would you create a product based on open hardware but don't trust the open source firmware for it ?
Anyway, I used the BLDC tool from enettion website to set it up and it went fine, a bit scary at first when coming from the Vesc tool but not super hard in the end.
```

---
## \#568 Posted by: admiralackbar Posted at: 2018-07-31T14:25:50.628Z Reads: 218

```
is a 3d model available? I need it to figure out the spacing of components and dimensions for an electronics compartment & diy eboard I am 3D modeling in inventor / solidworks / fusion
```

---
## \#569 Posted by: onloop Posted at: 2018-11-28T00:31:58.744Z Reads: 172

```
![image|614x384](upload://cm9qvUiNZJ4ZmcWEBXxvagdCYrs.jpeg)
```

---
## \#570 Posted by: Itsmedant Posted at: 2018-11-28T02:43:04.095Z Reads: 160

```
Sad to see it go. Still not sure if I'm completely sold on a dual VESC. Its a big chunk of change to fork back over if something fails on it. My build now is 2 singles, I got a Unity on order so I guess I'll form my opinion then!
```

---
## \#571 Posted by: Andy87 Posted at: 2018-11-28T13:24:28.023Z Reads: 143

```
Are you sure?
the title of this thread is "NEW IMPROVED" ... time to step on with a new product ...
there is always something to improve (or a V2 ;) )
```

---
## \#572 Posted by: Sn4pz Posted at: 2018-11-28T13:35:43.515Z Reads: 139

```
I thought for a split second that there actually was a 2.0... now I'm sad again 😭😭😂
```

---
## \#573 Posted by: CarlCollins Posted at: 2018-11-28T13:36:52.573Z Reads: 137

```
Unity is the evolve form of FOCBOX, so you can say V3 as FOCBOX got updated twice before :slight_smile:
```

---
## \#574 Posted by: Sn4pz Posted at: 2018-11-28T13:37:36.948Z Reads: 136

```
Ah you know what I meant 😂

Maybe someday
```

---
## \#575 Posted by: CarlCollins Posted at: 2018-11-28T13:38:25.087Z Reads: 134

```
I can understand :stuck_out_tongue:
```

---
## \#576 Posted by: Bjork3n Posted at: 2018-11-28T13:49:05.064Z Reads: 133

```
@CarlCollins can you tell me what was updated on the recent focboxes with the v 1.7 label on the pcb?
```

---
## \#577 Posted by: Andy87 Posted at: 2018-11-28T13:51:49.978Z Reads: 131

```
You can disconnect the can bus while powered on without to fry the can port
```

---
## \#578 Posted by: Andy87 Posted at: 2018-11-28T13:59:25.724Z Reads: 134

```
Than v3.1 and call it split unity 😂🤷‍♂️
```

---
## \#579 Posted by: Tamatoa Posted at: 2018-11-28T16:03:13.096Z Reads: 130

```
Is there anyway for you guys to consider doing another run like in a group buy? Probably not right now but later next year. How many is the minimum quantity to do a run of singles?
```

---
## \#580 Posted by: briman05 Posted at: 2018-11-28T16:19:11.221Z Reads: 129

```
If they throw in free shipping and at the black friday price they would probably have a line of people waiting.  I almost snagged 2 focbox over the weekend but I needed to give me credit card a break.
```

---
## \#581 Posted by: banjaxxed Posted at: 2018-11-28T16:56:55.463Z Reads: 127

```
Loony tunes, my favorite and on point
```

---
## \#582 Posted by: Jreamer Posted at: 2018-11-28T17:03:15.200Z Reads: 135

```
These black friday 99 dollar sales are as close as we will ever get to a group buy thing.
```

---
## \#583 Posted by: Tamatoa Posted at: 2018-11-28T17:04:35.559Z Reads: 138

```
That would be great, although, free shipping might be a bit of a stretch i think 😁 but I won’t complain if they did. I have been thinking about grabbing a couple of those for a long time but I thought I had time and I am broke AF these days.  Now it is too late 😭
```

---
## \#584 Posted by: evoheyax Posted at: 2018-11-28T17:05:47.308Z Reads: 139

```
@onloop can you confirm when these Black Friday focbox's will ship? Would love to grab 4 at this price. But don't want to wait until April.
```

---
## \#585 Posted by: briman05 Posted at: 2018-11-28T17:26:35.239Z Reads: 134

```
Did you order them already cause they are sold out
```

---
## \#586 Posted by: evoheyax Posted at: 2018-11-28T17:28:45.869Z Reads: 141

```
Oh danm... I was waiting till I get paid on friday. But I guess no more focboxes...
```

---
## \#587 Posted by: briman05 Posted at: 2018-11-28T17:29:43.436Z Reads: 143

```
Yep if you go on the site it doesnt even come up
```

---
## \#588 Posted by: akhlut Posted at: 2018-11-28T17:31:12.253Z Reads: 146

```
I'm hoping they ship in a reasonable amount of time.
```

---
## \#589 Posted by: Andy87 Posted at: 2018-11-28T20:12:52.778Z Reads: 137

```
Took exactly 6 days with my last order.
To Russia 😅
```

---
## \#590 Posted by: Chupacabra Posted at: 2018-12-08T10:29:11.981Z Reads: 126

```
I’m down for one as well
```

---
## \#591 Posted by: MatrixWriter Posted at: 2019-01-15T23:38:00.470Z Reads: 88

```
I was wondering if anyone has the bill of materials for the FOCBOX, otherwise I could pretty much just pick and choose my own brand from the schematics - ie the resistors and caps?

I'm planning to make a different form factor for one of my build later on.
```

---
