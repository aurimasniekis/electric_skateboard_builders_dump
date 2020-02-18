# The Orange Firefly &#124; Turnigy SK3 6374-192kv &#124; 10S3P 25R &#124; VESC 6 &#124; 3D-printed enclosure &amp; motor mount &#124; Custom deck

### Replies: 83 Views: 12992

## \#1 Posted by: solidgeek Posted at: 2017-04-23T21:57:21.545Z Reads: 880

```
Greetings from Denmark,

Last year I build my first electric longboard, with inspiration and information from you guys! Thanks for all the amazing builds and information avalible on this forum, its amazing :slight_smile:

I have been riding my board for a year now, and borrowed it to my cousin a few weeks ago. He road it for a few miles, and of course fried all the electronics :smile: That gave me a new opportiúnity to create something new and hopefully better.

So far my build will contain:

* 1 **Turnigy SK3 6374-192kv** motor
* 30 **Samsung 25R 2500mAh** (10S3P)
* 1 **40A 10S BMS**
* 1 Vedder **Antispark Switch** with 40A/50A fuse
* 4 **83mm ABEC 11** clones
* **Custom remote** with NRF24L01
* A **VESC 6.4**
* Custom deck
* 15T and 40T HTD pulleys and belt

The deck is designed in Inkscape, and milled out with my X-Carve from Inventables - a most usefull machine! The deck is made of some glulam I had in stock. 

<img src="/uploads/db1493/original/3X/3/4/34a89f490409ba90cae4285c6b490bda93eca888.jpg" width="375" height="500">

It came out pretty neat, here is a picture of it with some wheels and trucks mounted!

<img src="/uploads/db1493/original/3X/9/8/98f21d18b9c5b1107df2f957ecdda70da259dc07.jpg" width="458" height="500"> 

I plan to cut out a pocket for the batteries and all the electronics, and build a cover/lid that fits right on. All done on my X-carve of course :D

<img src="/uploads/db1493/original/3X/e/6/e618c2382b8da41e20a1689833b91f15092ccb7f.PNG" width="690" height="241">

I am planning to cut out som risers for the trucks in some high quality wood, and making a motor mount out of some 5mm aluminium profiles I have lying around. 

What do you think so far, anything I could improve? Looking forward to hear your opiones :slight_smile:
```

---
## \#2 Posted by: wmj259 Posted at: 2017-04-24T00:30:17.895Z Reads: 775

```
I'm interested in how the risers come out. I need me a pair also. And very nice design with following the grain of the wood. Also how thick is that board?
```

---
## \#3 Posted by: Luke Posted at: 2017-04-24T01:10:56.396Z Reads: 773

```
[quote="solidgeek, post:1, topic:21639"]
1 Turnigy G160 245kv motor
30 Samsung 25R 2500mAh (10S3P)
A VESC-X or VESC 6.0 (your thoughts on this would be very appreciated)
[/quote]
It may be advisable to set an Erpm limit of 60,000 when setting up your vesc if you go with the vesc-x
Using that high a kv motor with a 10s battery may otherwise lead to some issues.
```

---
## \#4 Posted by: solidgeek Posted at: 2017-04-24T09:51:46.019Z Reads: 759

```
[quote="wmj259, post:2, topic:21639"]
I'm interested in how the risers come out. I need me a pair also.
[/quote]

I will post a picture later today :slight_smile:

[quote="wmj259, post:2, topic:21639"]
And very nice design with following the grain of the wood. Also how thick is that board?
[/quote]

Thank you, I like it to! The board is 18mm

[quote="Luke, post:3, topic:21639"]
It may be advisable to set an Erpm limit of 60,000 when setting up your vesc if you go with the vesc-xUsing that high a kv motor with a 10s battery may otherwise lead to some issues.
[/quote]

Okay I will keep that in mind, doesn't the VESC 6.0 have these issues? A eRPM limit of 60,000 is quite a lot isn't it?
```

---
## \#5 Posted by: solidgeek Posted at: 2017-04-24T18:22:27.879Z Reads: 729

```
Just finished the risers. They are made out of some hard wood I found in my workshop. 

<img src="/uploads/db1493/original/3X/f/4/f4fe59b580f5045c21a9f016cbd6bcf71d77dfa2.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/d/6/d62286c6c9d803fadd38a7087de9979819a11f9f.jpg" width="690" height="388">

I also recieved my wheel pulley today, 3D-printed from 3DHubs.com. Not sure if PLA is strong enough though?

<img src="/uploads/db1493/original/3X/e/2/e2d5cce5184fa6a648cc76327cfc166cb90326b1.png" width="690" height="377">

I used this 3D-model http://www.thingiverse.com/thing:545345
```

---
## \#6 Posted by: Luke Posted at: 2017-04-24T19:02:06.378Z Reads: 690

```
[quote="solidgeek, post:4, topic:21639"]
Okay I will keep that in mind, doesn't the VESC 6.0 have these issues? A eRPM limit of 60,000 is quite a lot isn't it?
[/quote]

Can't comment on the vesc 6.0, I haven't looked at it. And it just depends on the kv of the motor and the voltage of the battery
```

---
## \#7 Posted by: rwxr Posted at: 2017-04-24T19:11:24.375Z Reads: 676

```
PLA is too brittle to use for pulleys. Nylon would be best.
```

---
## \#8 Posted by: OskarCastrone Posted at: 2017-04-24T20:10:08.193Z Reads: 669

```
Hi!

Good to see another Dane here! That's pretty rare! 
Where do you live? Maybe we can meet up some time? 

If you need any parts, I am about to launch an eskate website containing prebuild boards and spare parts. 

Du er velkommen til at sende mig en mail på oskar@castrone.dk :)
```

---
## \#9 Posted by: solidgeek Posted at: 2017-04-24T20:44:23.465Z Reads: 665

```
[quote="rwxr, post:7, topic:21639, full:true"]
PLA is too brittle to use for pulleys. Nylon would be best.
[/quote]

If the PLA version fits I will go for another material. However printing in Nylon is pretty expensive, maybe ABS could do the job? As far as I know ABS is much stronger than PLA :slight_smile: 

[quote="OskarCastrone, post:8, topic:21639"]
Hi!

Good to see another Dane here! That's pretty rare! Where do you live? Maybe we can meet up some time? 

If you need any parts, I am about to launch an eskate website containing prebuild boards and spare parts. 

Du er velkommen til at sende mig en mail på oskar@castrone.dk :slight_smile:
[/quote]

Hi Oskar, good to know that I am not alone on my electric longboard in Denmark! I live in Aalborg, how about you? Could be fun to meet :D

Lyder spændende med din webshop :) ! Hvis du har brug for noget hjælp med opsætning/udvikling må du sige til - jeg arbejder til dagligt med webudvikling/design :smile:
```

---
## \#10 Posted by: Deathjunior Posted at: 2017-04-24T21:54:19.794Z Reads: 668

```
It's looking oddly similar to my build so far. You might try and router out the edge of the deck a bit on the underside to give it kindof a wheel well. It's been working out really well on my. I've got 97mm wheels and only 1/4 inch risers <img src="/uploads/db1493/original/3X/8/a/8af25b98de809831b746c52ec28f31dd602bebdf.jpg" width="374" height="500">

As for printed pullys I'd have someone see about cnc milling some out of aluminum if it's anything like my motor and gear covers that shit will vibrate itself to pieces.
```

---
## \#11 Posted by: sl33py Posted at: 2017-04-24T23:27:27.764Z Reads: 648

```
[quote="solidgeek, post:4, topic:21639"]
doesn't the VESC 6.0 have these issues? A eRPM limit of 60,000 is quite a lot isn't it?
[/quote]

It seems like this has been addressed and fixed w/ the VESC 6.  Where the VESC 4.xx was pretty much guaranteed to kill the DRV chip over 60k ERPM's (thanks to @Chaka for calling out this limitation and sharing here).  

I just read [a pretty lengthy post by Ben on his forum](http://vedder.se/forums/viewtopic.php?f=6&t=590&start=10) regarding the VESC 6 Beta.  Getting close finally!  And some motors over 150k ERPM it seems w/o issue.  Much higher amps possible, and just seems a ton more robust!  

The possible downside if you were going to build your own (you made your own deck - i'm guessing you might try reflowing your own VESC) - Vedder's BOM/Gerbers aren't yet available during the "Beta" .  But you can see if there is room to join the beta group by contacting @trampa (Frank at Trampa) to get on the list.  Trampa being in the UK, and you in Denmark -  it should be a bit faster for you vs those of us in the states.  

HTH - GL!
```

---
## \#12 Posted by: sl33py Posted at: 2017-04-24T23:31:20.216Z Reads: 632

```
[quote="Deathjunior, post:10, topic:21639"]
As for printed pullys
[/quote]


If you go printed pulleys - you should go 15mm wide belts for more contact, and hopefully you are light.  Being in Denmark - i'm also guessing it's pretty flat where you ride?

I had a single 9mm setup w/ printed wheel pulley for my GF - worked OK.  Nylon IIRC, not PLA, but while she could ride it - it would skip terribly for me no matter how tight i ran the belt.  Not just at faster speeds...  So while it *can* work... I would still go w/ Aluminum if you can.  Look for @Titoxd10001's 15mm 15/40 setup if you want to gear down (less top speed, better accel and torque) w/ some nice aluminum gears that won't break the bank $ wise.  Unsure if shipping to EU will be prohibitively expensive though...

GL!
```

---
## \#13 Posted by: Titoxd10001 Posted at: 2017-04-25T01:11:35.936Z Reads: 589

```
Thanks for the tag. @Deathjunior I have aluminum 40t pulleys designed especially for 97mm flywheels. I also have steel 15t 15mm pulleys. They will be available for purchase today or tomorrow shipped directly from Europe at a very reasonable price.
```

---
## \#14 Posted by: solidgeek Posted at: 2017-04-25T06:46:21.184Z Reads: 639

```


[quote="sl33py, post:12, topic:21639"]
If you go printed pulleys - you should go 15mm wide belts for more contact, and hopefully you are light.  Being in Denmark - i'm also guessing it's pretty flat where you ride?
[/quote]

It is indeed very flat in Denmark, however we got hills now and there :slight_smile: Maybe I should go with a steel or aluminium pulley instead. I just find the idea of 3D-printing parts very appealing :P 

[quote="sl33py, post:11, topic:21639"]
It seems like this has been addressed and fixed w/ the VESC 6.  Where the VESC 4.xx was pretty much guaranteed to kill the DRV chip over 60k ERPM's (thanks to @Chaka for calling out this limitation and sharing here).
[/quote]

Thanks, thats good to know! I have already contacted Frank, and I believe he added me to the mailing-list :slight_smile:! So I am waiting to recieve an e-mail from him!

[quote="Titoxd10001, post:13, topic:21639"]
I have aluminum 40t pulleys designed especially for 97mm flywheels. I also have steel 15t 15mm pulleys. They will be available for purchase today or tomorrow shipped directly from Europe at a very reasonable price.
[/quote]

@Titoxd10001 I am very interested in one of your kits, does it fit a 83mm flywheel? Thanks :slight_smile:

[quote="Deathjunior, post:10, topic:21639"]
It's looking oddly similar to my build so far. You might try and router out the edge of the deck a bit on the underside to give it kindof a wheel well. It's been working out really well on my.
[/quote]

Looks nice, do you have more pictures of your board? :smiley:
```

---
## \#15 Posted by: Deathjunior Posted at: 2017-04-25T07:25:52.431Z Reads: 643

```
I don't have many since I don't take many lol but sure<img src="/uploads/db1493/original/3X/0/0/00c8146fafd570b452936a430ff0c7f5871b8336.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/e/be110bdc65ea005e1bd83aabff9cb226f0b13d1d.jpg" width="374" height="500">
```

---
## \#16 Posted by: Deathjunior Posted at: 2017-04-26T15:39:34.982Z Reads: 605

```
I'm good lol I run cnc aluminum wheel pulleys I just use an abs 3d printed spacer to make them work on my 97mm flywheels. My motor pulleys are steel. I'm going to rework my motor covers and print them from pla in order to investment cast them in sand.
```

---
## \#17 Posted by: OskarCastrone Posted at: 2017-04-26T16:27:02.933Z Reads: 588

```
@solidgeek
I actually have a motormount set including pulleys and trucks. I am willing to sell it to you for  DKK600? It is about half of what I payed for them from DIY...
```

---
## \#18 Posted by: solidgeek Posted at: 2017-04-30T21:52:22.480Z Reads: 688

```
I have just recieved my 40T and 15T pulley from @Titoxd10001! Looks great, and fits my ABEC11 clones perfectly - thanks, you just saved me a lot of enginering :smile: !!!

[quote="OskarCastrone, post:17, topic:21639"]
I actually have a motormount set including pulleys and trucks. I am willing to sell it to you for  DKK600? It is about half of what I payed for them from DIY...
[/quote]

Thanks, but I have been working on a motor mount myself :slight_smile:! Just finished the 3D-sketches today, and been trying to carve the design in aluminium on my CNC. It came out very good, however I did not have the time to finish it completly. 

<img src="/uploads/db1493/original/3X/e/3/e38570e77fde22f1f1bc37be870b994d1fd5dd85.PNG" width="690" height="472"> 

<img src="/uploads/db1493/original/3X/0/5/058e5a54b1450af35c493104f454fd2848228b4c.jpg" width="690" height="388">

Looking forward to next weekend... :stuck_out_tongue:
```

---
## \#19 Posted by: solidgeek Posted at: 2017-06-03T13:35:47.087Z Reads: 670

```
So, it’s been awhile since I had the time to work with my board, however since the VESC 6.0 just has been released for Beta, I simple had to finish the mechanics (motor mount etc.). Instead of the aluminum motor mount I had been working on, I decided to try something new. I recently bought a 3D printer, so I thought it would be fun to try and make an all 3D-printed motor mount. And I came up with this design (inspired heavily by the one from DIY).

<img src="/uploads/db1493/original/3X/8/7/87309a6d63b1794bcb91b646840e4f4196bb9ab5.PNG" width="689" height="342">

<img src="/uploads/db1493/original/3X/f/5/f5195b5ed9dddd0fcf9d55e1db7d21a1f38a518f.PNG" width="690" height="472">

<img src="/uploads/db1493/original/3X/6/0/60ebbfc0da3755f59d34885eea167a2849207450.PNG" width="690" height="453">

It consists of to parts, heavily interlocked and reinforced. The locking ring fits perfectly on a caliber truck and is tightened by one 5mm bolt and locked in place with another 5mm bolt. The whole motor mount fits right over the caliber-ring, and is locked in place with 1-5 4mm bolts. To make sure the motor mount doesn't bend I have made room for two solid 3mm*80mm steel rods, that slides in from the tip of the motor mount.

Sooo... I printed it with some high quality carbonfiber reinforced PLA in about 4 hours, and it fits perfectly :smile:

<img src="/uploads/db1493/original/3X/4/4/4442673d317a4dc0724cae5fca0dba84cc07525f.jpg" width="690" height="230">

<img src="/uploads/db1493/original/3X/5/1/517b618560d00134812759d8db1339519cff3650.jpg" width="582" height="500">

<img src="/uploads/db1493/original/3X/5/d/5d5d5570ba226e628cea98602100b4d81970b412.jpg" width="595" height="500">

It feels incredibly stiff and robust, however if it will last more than a few miles, I do not know :stuck_out_tongue: Hopefully it works untill I learn to push myself ;)! I'm looking forward to recieving my VESC 6!
 
If anyone wants to try to 3D-print the motor mount themselves I would love to share the Autodesk Inventor / STL-files :slight_smile:
```

---
## \#20 Posted by: mmaner Posted at: 2017-06-03T14:53:05.734Z Reads: 625

```
That looks awesome, the way you reinforced the motor plate is inspired. I'd like to print one if these in ABS and give it a run, if you don't mind sharing.
```

---
## \#21 Posted by: rwxr Posted at: 2017-06-03T15:00:44.716Z Reads: 587

```
I would also like to try printing them :)
```

---
## \#22 Posted by: solidgeek Posted at: 2017-06-03T15:53:14.221Z Reads: 611

```
Thanks, I am happy you like it :smiley:  !
[quote="mmaner, post:20, topic:21639, full:true"]
That looks awesome, the way you reinforced the motor plate is inspired. I'd like to print one if these in ABS and give it a run, if you don't mind sharing.
[/quote]

 I have made an Google Drive folder with the original Inventor-files and the STL-files :slight_smile:

https://drive.google.com/open?id=0B5QG3s3e1xG8ajNGZ0hEUXVuY3M  

I am using a 295Mmm belt, because my pulley setup (40T/15T) is quite big. I am not sure it will work with a standard 265mm belt :) The distance between the motor and wheel axis is 77mm. Also the mount only works if you have a hollow wheel pulley, or some flat 4mm bolts - so the wheel pulley doesn’t collide with the 4mm bolts.
```

---
## \#23 Posted by: mmaner Posted at: 2017-06-03T16:07:30.265Z Reads: 578

```
Cool I'll give it a shot and let you know. Thanks for sharing.
```

---
## \#24 Posted by: solidgeek Posted at: 2017-06-03T19:14:02.240Z Reads: 571

```
I'm looking forward to see the result :slight_smile:
```

---
## \#25 Posted by: mmaner Posted at: 2017-06-04T17:31:18.080Z Reads: 589

```
@solidgeek I had a hard time finding this post 😀.
<img src="/uploads/db1493/original/3X/9/f/9f42b7590914a6fdda66a43d25f44082845d607e.png" width="281" height="500">
I still have these rods if you want some, just let me know the size you want.

I had some issues with my printer, it get out of level sometimes and my ABS slurry was too weak.  Re-election and re-add, printing now in blue ABS at 100% infill.  

I'll post the result tomorrow, gonna take 9 hours or so to print, but I'll install it in my beater board tomorrow and see how it does.
```

---
## \#26 Posted by: solidgeek Posted at: 2017-06-04T18:45:04.955Z Reads: 542

```
@mmaner funny how different people get the same ideas :P It seems to work great with the rods.

Well I salavage my 3mm steel rods from two old CD/DVD-drives I had lying around. Those old drives got some pretty neat and reusable components. So I probably don't need anymore, but thanks for the offer :slight_smile: !

Sounds like you got yourself a tiresome 3D-printer :confused: I have no experience in printed ABS using ABS slurry (juice?), do you think it is nessesary to print it in ABS? The carbon-fiber PLA seems very strong, and I think it would be easier to print with (if you have some of course)?. Looking forward to see the result!
```

---
## \#27 Posted by: mmaner Posted at: 2017-06-04T18:55:38.355Z Reads: 519

```
It's not the best printer, but it works pretty well.  I have a little  pla but no cf pla.  Abs is what I normally use, pretty strong stuff.
```

---
## \#28 Posted by: dedinski Posted at: 2017-06-04T18:57:09.817Z Reads: 513

```
Hows the carbon fiber mount holding up?
```

---
## \#29 Posted by: solidgeek Posted at: 2017-06-04T19:01:04.775Z Reads: 524

```
Well I'm still waiting for my new VESC6, so I haven't been able to do a real test-ride yet :( However I have tried putting quite a lot of stress on the mount, and it doesn't seem to bend at all (the steel rods probably adds some stiffness). So far I'm very impressed with the strenght :slight_smile: 

I will make an update on its performance as soon as possible!
```

---
## \#30 Posted by: Julmust Posted at: 2017-06-04T22:18:20.447Z Reads: 522

```
Hey, solidgeek! You've really got a cool build going on! I'm liking the 3d printing aspect to the board and think that I might end up doing something similar. Are the designs made to fit on the Caliber G II or are they for the Caliber IIs? Otherwise what trucks are you using?
```

---
## \#31 Posted by: lucasbuckleynz Posted at: 2017-06-05T02:05:04.127Z Reads: 518

```
Hi solidgeek or anyone that knows, I really like the idea of 3D printing the motor mounts and was wondering what sort of motor it would fit (63mm or 50mm diameter) .... or the hole spacing. Also is there enough space to have a dual motor system?
```

---
## \#32 Posted by: solidgeek Posted at: 2017-06-05T14:02:21.701Z Reads: 567

```
[quote="Julmust, post:30, topic:21639, full:true"]
Hey, solidgeek! You've really got a cool build going on! I'm liking the 3d printing aspect to the board and think that I might end up doing something similar. Are the designs made to fit on the Caliber G II or are they for the Caliber IIs? Otherwise what trucks are you using?
[/quote]

Hey @Julmust :) Thanks, i'm glad you like the idea! I'm not excatly sure, the ones I bought came from a guy on eBay, this is the ones I bought:
http://www.ebay.com/itm/371926081730?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

@lucasbuckleynz the design is made for a 63mm motor or one with the same holespacing as the G160 from Turnigy :)  The mount is quite thick, so I'm not sure if it will work for a double motor setup.<img src="/uploads/db1493/original/3X/2/d/2dea3306c580855484f75c004ffa1dc086bcbde3.jpg" width="473" height="500">

At least you will need do use a little shorter motor than my G160 :stuck_out_tongue:  The holespacing is: 
<img src="/uploads/db1493/original/3X/8/e/8e371e7918a26bf6fdc7280b0bbd81b664f033bf.PNG" width="690" height="318">
```

---
## \#33 Posted by: Julmust Posted at: 2017-06-05T14:33:18.650Z Reads: 531

```
Okay, great @solidgeek . Looks like they are the same actually! Where did you buy your abec clones and how much were they?
```

---
## \#34 Posted by: solidgeek Posted at: 2017-06-05T20:40:42.183Z Reads: 537

```
Good! I also bought my ABEC clones on ebay: 
http://www.ebay.com/itm/161958552460?_trksid=p2057872.m2749.l2649&var=461260479372&ssPageName=STRK%3AMEBIDX%3AIT 

Very nice wheels to a good price and shipped with the Global Shipping Program, which is nice if you live in Europe :slight_smile:
```

---
## \#35 Posted by: solidgeek Posted at: 2017-06-19T11:13:35.302Z Reads: 550

```
I have been working quite a lot on my board the past few days. I have 3D-printed an enclousure for the electronics, and a riser with 3.5mm banana-plugs for the motor. Here is some pictures

<img src="/uploads/db1493/original/3X/6/c/6cb9e0c608cbbf970284a9244869179242108a25.jpg" width="690" height="350">

<img src="/uploads/db1493/original/3X/0/3/0374bfbe1ca48cab3277d55a229ea34fe823c005.jpg" width="690" height="350">

<img src="/uploads/db1493/original/3X/c/2/c21eaed2c75ff3ef25c3eb39a147b8a4f2c33773.jpg" width="690" height="350">

Next I plan to 3D-print the enclosure for the batteries and BMS. And then I only need to finish my remote.. :smiley:
```

---
## \#36 Posted by: solidgeek Posted at: 2017-06-27T00:30:38.170Z Reads: 537

```
So I just finished all the enclousere today :yum:

<img src="/uploads/db1493/original/3X/f/c/fc9e81f01de5ef4afd880b1c6bc6ff19a2222cb5.jpg" width="318" height="500">

It came out pretty neat I think, with the sleek and simple look :smile:

<img src="/uploads/db1493/original/3X/e/2/e2fbcbb71e291b21c45154327edd2a544d2221d3.jpg" width="690" height="378">

Can't wait to finish the remote!!!
```

---
## \#37 Posted by: BOB1 Posted at: 2017-07-07T05:07:17.148Z Reads: 512

```
Loving the design of that enclosure, I'm trying to design one for my board atm and I'm trying to do something similar. Would be great to have some more pics or an STL for better inspiration.
```

---
## \#38 Posted by: solidgeek Posted at: 2017-07-07T10:05:43.760Z Reads: 507

```
Hi Bob, Thanks I am glad you like it :smile:!  I will gladly share the 3D-files, however I am not at my computer at the moment, so you will have to wait a few more hours.

EDIT: I have uploaded the STL-files to the same Google Docs folder as my motormount: https://drive.google.com/drive/folders/0B5QG3s3e1xG8ajNGZ0hEUXVuY3M :-) !
```

---
## \#39 Posted by: solidgeek Posted at: 2017-07-10T22:17:29.909Z Reads: 497

```
I have made an Thingiverse account so I can share my 3D-designs with you guys! Just released my enclousure design https://www.thingiverse.com/thing:2423483 - hope you enjoy  :smile: 

My 3D-printed motor mount is doing surprisingly well so far, with some improvements I think it actually could be a permanent solution.
```

---
## \#41 Posted by: Chicagojoshua Posted at: 2017-07-11T03:20:37.427Z Reads: 496

```
hey,

    Great job, do you have an idea of where I can purchase the rod inserts for the mount?
```

---
## \#42 Posted by: solidgeek Posted at: 2017-07-11T09:53:36.745Z Reads: 498

```
I got mine from two old CD drives I salvaged, however a quick search on ebay for "3mm steel rods" gives tons of results :slight_smile: 

http://www.ebay.com/itm/5-Pcs-RC-Airplane-Stainless-Steel-Round-Rods-Axles-Bars-3mm-x-150mm-BT-M0K7-/282434753580?epid=872598568&hash=item41c26c542c:g:M~MAAOSwtZJY8s4N

You would just have to cut them to the right lenght etc. 

I am glad you like my design :-)
```

---
## \#43 Posted by: solidgeek Posted at: 2017-07-11T15:38:38.507Z Reads: 495

```
https://www.youtube.com/watch?v=5cW0p8VKpxI

https://www.thingiverse.com/thing:2429445
```

---
## \#44 Posted by: solidgeek Posted at: 2017-07-12T23:22:37.209Z Reads: 479

```
My build is complete, remote is done and I have crashed a couple of times! Great fun :smile: (I made a little video)

https://www.youtube.com/watch?v=XwxYdglf3o0
```

---
## \#45 Posted by: Chicagojoshua Posted at: 2017-07-13T04:23:46.289Z Reads: 470

```
Dude, that remote is awesome! Looks just like my boosted remote. Can you share the details of that remote cause it looks like its 3d printed? I would be curious to build a remote just like yours! Awesome job !
```

---
## \#46 Posted by: solidgeek Posted at: 2017-07-13T09:58:52.194Z Reads: 480

```
Thanks! Well I was heavily inspired by the design of the Boosted remote, its a very nice design. And you are right it is 3D-printed, in the same material as my motor mount :slight_smile:

It uses an Arduino Nano, a Hall sensor (throttle), a NRF24-modul and a few other easily availble components. I am planning to make a build thread/video within the next week. Would be awesome to make it open source, and develop it further!  

<img src="/uploads/db1493/original/3X/a/8/a8f23afd07fcb40966b8cf39c5b1208a62d3ea9d.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/9/29af7afe89d0ee0af802ed1b2bf083c3064c8ba3.jpg" width="375" height="500">
```

---
## \#47 Posted by: Chicagojoshua Posted at: 2017-07-13T15:50:10.744Z Reads: 454

```
dude that remote build thread is going to be awesome! Does it also give you the battery capacity like the real one? Wow, you even built the trigger activation which is so essential for safety. I have several boards but the boosted boards remote is by far the best one. The only thing I would change on the remote is the thumb wheel,,,,I would add a slight knob to the middle of the thumb wheel just like the winning remote. When its hot outside and my hands are sweaty the thumb wheel slips and when its cold outside I cant feel the thumb wheel with my gloves. This could easily be improved with a slight nipple in the middle of the thumb wheel.
```

---
## \#48 Posted by: oskuro Posted at: 2017-07-13T19:11:31.172Z Reads: 443

```
Wow amazing eboard, great job!! how much did you spend more or less?
```

---
## \#49 Posted by: solidgeek Posted at: 2017-07-13T22:18:20.383Z Reads: 451

```
@Chicagojoshua I hope so :slight_smile:! At the moment it doesn't have a way of knowing the battery capacity of the board itself, because I am using UART on my VESC for another purpose - Bluetooth. It is however easily done as many have done it before me (copy-paste no time to waste), and I believe I could make it work with only a few software changes :wink:

The cool thing about 3D-printing is that you easlisy can modify the thumb wheel with a knob! I will try to implement this in the next version :slight_smile:

@oskuro I wonder.... Well here it comes
**Batteries**: 900DKK (140$)
**ESC** (VESC 6): 2000DKK (310$) 
**Motor**: 600DKK (92$)
**Wheels & trucks**: 500DKK (76$)
**Drivetrain** : 180DKK (28$)
**Electronics**: 500DKK (76$)
**Misc**: 200DKK (30$)

More or less: 4880DKK or **748USD**. And it was quite a fun process to build it :P
```

---
## \#50 Posted by: HTownBomber Posted at: 2017-07-13T22:30:40.277Z Reads: 431

```
Great build! I'm a huge fan of that hex grip tape. Did you buy it pre-cut or laser cut it yourself?
```

---
## \#51 Posted by: IsTalo Posted at: 2017-07-13T23:47:52.857Z Reads: 421

```
I need that tutorial, plz plz plz, if you can, put the code in the description of the video
```

---
## \#52 Posted by: solidgeek Posted at: 2017-07-14T00:21:19.374Z Reads: 420

```
@HTownBomber I am not sure what hex grip tape you are talking about? :P I am just using regular grip tape, but thanks :joy:
 
@IsTalo I will make a topic about it as soon as I got the time. I am also waiting for a few components - so it will take a few days :)
```

---
## \#53 Posted by: IsTalo Posted at: 2017-07-14T00:26:50.663Z Reads: 410

```
Do it now and them you update with the new parts, I really loved it. Does it have a Fail Safe? And could I modify the Stl to fit a oled display?
```

---
## \#54 Posted by: demayod Posted at: 2017-07-14T00:28:34.068Z Reads: 403

```
Looks like he's talking about @Deathjunior s board.
```

---
## \#55 Posted by: solidgeek Posted at: 2017-07-14T00:39:45.490Z Reads: 409

```
Don't worry it wont take long :P The receiver has a timeout limit, so if the transmitter (remote) fails the board will slow down within half a second. The remote got the "kill switch"-function with a button that needs to be pushed down in order to transmit, is that what you where asking about? 

And sure, if you could find a way to fit a bigger OLED display in the remote, it would be possible. At the moment I am using a 128x32px OLED display, which is plenty of space for basic information :slight_smile:
```

---
## \#56 Posted by: IsTalo Posted at: 2017-07-14T00:52:59.384Z Reads: 410

```
[quote="solidgeek, post:55, topic:21639"]
The receiver has a timeout limit, so if the transmitter (remote) fails the board will slow down within half a second.
[/quote]

Yeah, this is what I was asking, my remote controller have a fail safe that brakes totally, so it's not that good
```

---
## \#57 Posted by: Deathjunior Posted at: 2017-07-14T00:53:25.003Z Reads: 432

```
My hex grip tape was about 3 hours of hand cutting many many hexagons out of black diamond grip tape with a razor blade. It was very very time consuming. <img src="/uploads/db1493/original/3X/a/0/a07d7dbdcc0afd2cc87050bbde09985676951984.jpg" width="494" height="500"><img src="/uploads/db1493/original/3X/6/9/696a7c722f539440714d2ee897f6d81b9f2bf1a1.jpg" width="500" height="500">
```

---
## \#58 Posted by: Pantologist Posted at: 2017-07-14T01:00:00.102Z Reads: 408

```
This is awesome. Looks just like a Boosted remote. You think I could use the housing and mechanism of a real Boosted remote? Same Hall sensor design right?
```

---
## \#59 Posted by: solidgeek Posted at: 2017-07-14T01:06:44.755Z Reads: 411

```
Thanks :-) The inner mechanism of the thumb wheel is also heavily inspired by the Boosted remote, with magnets and a Hall sensor. However I am not sure if the Boosted remote is big enough to fit the custom electronics, it will be a tight fit I believe... but maybe possible if you scrap the OLED, or not :P 

I am not sure if it will be an upgrade or downgrade of the Boosted remote's electronics :joy:!
```

---
## \#60 Posted by: BenL Posted at: 2017-07-15T01:27:44.001Z Reads: 399

```
What 3D printer do you have? Even in two parts, the surface area of each piece of the enclosure looks pretty large.
Looks great!
```

---
## \#61 Posted by: Tampaesk8er Posted at: 2017-07-15T20:58:34.010Z Reads: 391

```
I also have 3D printed wheel pulleys, PLA, been using them 4months now, no cracks yet, just print at 100% and just check them after every ride.
```

---
## \#62 Posted by: solidgeek Posted at: 2017-07-15T23:16:07.285Z Reads: 392

```
I am using a CR-10 (called an Afinibot A31 in Europe). It has a build volumen of 30×30×40 cm :slight_smile: . The small enclosure for the electronics could be printed on most 3D printers I believe, however the battery enclosure is quite large :smile:  I am glad you like it !
```

---
## \#63 Posted by: Ubbiedude Posted at: 2017-07-15T23:54:44.349Z Reads: 394

```
How did you make your battery pack if i may ask
```

---
## \#64 Posted by: Tampaesk8er Posted at: 2017-07-16T04:08:14.248Z Reads: 420

```
This video shows both my builds:

https://youtu.be/isTE92hvvGU

This video is of my motor while in motion at ground level: 

https://youtu.be/iuFEmG7W8cQ
```

---
## \#65 Posted by: Tampaesk8er Posted at: 2017-07-16T11:48:43.308Z Reads: 401

```
Do you have a file you can share for the belt, motor cover?
```

---
## \#66 Posted by: solidgeek Posted at: 2017-07-16T23:01:16.605Z Reads: 394

```
It is 3D-printed, in two parts. Just gave it a few coats of paint, and some light sanding :slight_smile:
```

---
## \#67 Posted by: lucasbuckleynz Posted at: 2017-07-27T06:17:27.474Z Reads: 389

```
hi @solidgeek, where did you get the 15t pulley? I also have the turning SK3 motor and wanted to make sure I get a pulley that fits properly. im not really sure what ones will work I am very new to making electric long boards.
```

---
## \#68 Posted by: luis99945 Posted at: 2017-08-01T22:08:19.040Z Reads: 380

```

Where did you buy your pulleys and your band
```

---
## \#69 Posted by: solidgeek Posted at: 2017-08-01T22:55:43.551Z Reads: 400

```
Sorry for the late answer, I have been busy working on my custom nRF24 remote :slight_smile: @lucasbuckleynz I bought mine from @Titoxd10001, however, I don't know if he got any left :slight_smile: I bought my belt in a local shop :)

http://www.electric-skateboard.builders/t/europe-1x-15mm-steel-motor-pulley-remaining/21733

However if you got a Turnigy SK3 motor the shaft diameter is 8mm, so you would just have to find a pulley with the same shaft diameter :slight_smile:

If you are interested in my remote build you can follow my progress in this thread:

http://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543
```

---
## \#70 Posted by: lucasbuckleynz Posted at: 2017-08-02T09:31:51.412Z Reads: 360

```
yea unfortunately i am in New Zealand .......... so no one ever posts to here. It looks like i will have to try to source one. thanks all the same.
```

---
## \#71 Posted by: nmiller14 Posted at: 2017-08-09T20:32:52.528Z Reads: 352

```
Did any one ever find out if Solid Geeks Motor Mount design works for a 265 belt?? I want to give it a try but that is the belt I have right now.
```

---
## \#72 Posted by: Genex Posted at: 2017-08-09T20:45:46.428Z Reads: 357

```
Not true, PLA works perfectly for pulleys. ABS works best in high temp situations due to its thermal properties, but PLA works just as well for pulleys. Pulleys don't see the high temps ABS is traditionally used for.  I've made and shipped 20+ sets of pulleys for people are not one has ever complained about durability.  I have a single pulley that I put around 600 miles on in 8 months and it still worked perfectly ( it had to deal with a 6374 on high voltage for those 8 months too).  They are far cheaper than nylon, and do just as good of a job.  I would never recommend anyone to spend extra $$ on any material other than high quality PLA.

EDIT- Sick build bro, got yourself a better boosted board for half the price :P
```

---
## \#73 Posted by: solidgeek Posted at: 2017-08-09T21:08:55.634Z Reads: 360

```
Hi @nmiller14 it depends on your gearing ratio. I used a 15/40T gearing, and because of that I needed a longer belt. If you use lets say a 14/30T gearing, a belt lenght of 265-270 would work. What is your gearing? 

<img src="/uploads/db1493/original/3X/4/f/4f565f7c2ade4ca782dbe6cc3f5438e74feb699e.PNG" width="690" height="383">

(this is the calculator I have used: https://www.bbman.com/belt-length-calculator/) 

The center distance is the distance between the truck axle and the motor axle :) 

<img src="/uploads/db1493/original/3X/6/b/6b6e3a3288028704893cf25559b96e84579a591a.PNG" width="690" height="399">
```

---
## \#74 Posted by: nikoli280 Posted at: 2017-08-09T21:16:42.354Z Reads: 332

```
Great design of the remote. Can we get a parts list maybe some STL files
```

---
## \#75 Posted by: nmiller14 Posted at: 2017-08-09T21:18:56.130Z Reads: 326

```
It looks like I can get it to work with my 12T/32T 265. Thanks, as per the calculator I will have only 5 teeth in the mesh. Do you think that is sufficient? I was also thinking of doing slight modifications to it. Could you share the file in a format that is AutoCAD friendly. All of this is much appreciated. Thank you.
```

---
## \#76 Posted by: solidgeek Posted at: 2017-08-09T21:48:36.376Z Reads: 333

```
@nikoli280 Thanks! I have made a seperate build-thread for the remote, with a parts list and the STL files :) 

http://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543
 
@nmiller14 I "only" got 6 teeth in the mesh, however, it works great. My belt is 15mm, which works great for a single motor setup. I am not sure if AutoCAD can open and modify Inventor files? PM me, I am sure we can find a solution :slight_smile:
```

---
## \#77 Posted by: Sk8Board Posted at: 2017-10-14T04:13:16.973Z Reads: 291

```
You could do a diagonal setup, one in the front and one in the back
```

---
## \#78 Posted by: WhySpace Posted at: 2017-10-19T18:18:47.280Z Reads: 291

```
What is the flex of your board.
```

---
## \#79 Posted by: Nandox7 Posted at: 2017-12-11T15:09:37.638Z Reads: 267

```
Curious about the way you connecting the motor to the truck risers.
Did you found right angle bullet connectors or you just soldered the wires sideways into normal ones?

Cheers!
```

---
## \#80 Posted by: solidgeek Posted at: 2017-12-22T00:50:23.109Z Reads: 264

```
I soldered the wires sideways :P It was a little messy, but it works!
```

---
## \#81 Posted by: buip Posted at: 2018-01-12T03:40:08.224Z Reads: 246

```
Hey I like your mount design and was wondering if I could have the AutoCAD file?
```

---
## \#82 Posted by: moronicity Posted at: 2018-01-22T21:44:15.905Z Reads: 223

```
is there any way you can share the 3D files for the battery case. Thanks!
```

---
## \#83 Posted by: Sapphirinia Posted at: 2018-01-29T15:27:13.191Z Reads: 215

```
Hi, I love your progress. I'm working on a new enclosure for my board since I busted my spacecell mounting holes due to my Concave deck. I'm wondering if you have any suggestions on creating an enclosure 3d printed/fiberglass that would work with a flexy, Concave deck. A few people mentioned you from some of my questions. I made a 3d nylon wheel pulley, hoping it works out. I haven't been able to use it yet as my board was hit by a car and I haven't found a belt that fits my new wheel setup yet. All suggestions are appreciated.
```

---
## \#85 Posted by: Boarder Posted at: 2018-09-20T06:04:11.523Z Reads: 102

```
hey @solidgeek could you put that riser model on the drive plz?
```

---
