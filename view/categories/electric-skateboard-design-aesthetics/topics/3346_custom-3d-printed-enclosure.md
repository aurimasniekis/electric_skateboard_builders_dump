# Custom 3D-printed enclosure

### Replies: 39 Views: 7126

## \#1 Posted by: mcfly777 Posted at: 2016-05-16T15:30:15.388Z Reads: 668

```
Hi There
I am planning my first build, and wanted to have a 2-part enclosure since my deck has some flex and I only have 2 batteries. So I started putting something together in Fusion 360. I thought about vacuum forming but since I have a 3D printer might as well use it. 

Goals: 
- Be able to print each part at once and not have to break it into multiple prints, so the design has to conform to the limits of my printer (230x150x150).
- thicker walls (3mm)
- stays in place with magnets

Comments appreciated. I am now printing the first one so I can test fit.

<img src="/uploads/db1493/original/2X/0/084af5610973496c3bb05af7046fbd95d14a0efe.png" width="690" height="283">

<img src="/uploads/db1493/original/2X/8/854ed63024173cc77d13cd841ba40d3594814f81.png" width="690" height="283">
<img src="/uploads/db1493/original/2X/b/bde2346617125b02c8f2963375e91fe35f4f50c3.JPG" width="690" height="455">
```

---
## \#2 Posted by: bbq870 Posted at: 2016-05-17T11:29:42.310Z Reads: 593

```
what kind of material are you planning to use?
```

---
## \#3 Posted by: mcfly777 Posted at: 2016-05-17T14:59:08.689Z Reads: 587

```
I printed it yesterday with ABS. It is very sturdy and feels solid. But the problem with ABS is its shrinkage, especially with long straight parts like this, so I got an area where the layers delaminated a bit. I ordered PETG as it is claimed that it has all the good properties of ABS but without the shrinkage (or smell).
Leo
```

---
## \#4 Posted by: MasterCho Posted at: 2016-05-17T16:40:03.527Z Reads: 558

```
Usually,the shrinkage happens when temperature changes too quickly,especially when you print Flat and  large object like this. Just make sure to cover all the openings of the case as much you can. Also, use ABS slurry to glue it down on the plate from the lift and keep the build plate temperature at 100c-110c.
```

---
## \#5 Posted by: mcfly777 Posted at: 2016-05-17T16:52:22.941Z Reads: 536

```
Indeed, I have a closed case and a heated bed. I can stick the first layer very well. Now that I looked at it some more it seems that maybe there was one layer that didn't print well so that may have caused the delamination. I'm hoping PETG works well, I like ABS but I wish it was as easy to print as it is with PLA. At least the price for PETG is roughly the same as ABS.
```

---
## \#6 Posted by: jeshua Posted at: 2016-05-19T05:00:29.360Z Reads: 510

```
To prevent lamination with abs I've found that increasing your hotend temp by 10C helps. You may also be able to increase the extrusion rate slightly depending on what software you're using. 

I'm very curious to see how well the magnets will work, I may steal that idea for mine. I was about to print but that would be really clean.
```

---
## \#7 Posted by: mcfly777 Posted at: 2016-05-19T15:23:52.178Z Reads: 499

```
Yes I'll try the magnets on a scrap piece of board with my prototype enclosure and see how it holds up. Note that I intend to affix the batteries/components to the deck, so all the magnets have to support is the weight of the enclosure itself.
```

---
## \#8 Posted by: mcfly777 Posted at: 2016-05-19T16:15:00.528Z Reads: 515

```
Ok, just I just did it an experiment with magnets this morning. Installed 6 8mm magnets, and attached the enclosure to a metal base (since I didn't have another 6 magnets for the other side). It did not stick as well as I wanted it to. I have some magnets ordered but it will take a while until I get it. Also have some clevis pins that I'll get later this week so I'll play with that as well.

<img src="/uploads/db1493/original/2X/1/1bfc483d6c23236157ca5ea8365f147a5aacfd26.jpg" width="666" height="500">
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-05-19T16:48:01.121Z Reads: 482

```
You have guide slots right? So the magnet force only has to worry abt one getting pulled off and not slide off right?

Edit and 6 magnets aren't enough based on the looks ...will need double at least
```

---
## \#10 Posted by: mcfly777 Posted at: 2016-05-19T17:11:30.874Z Reads: 464

```
Yes I will need to work on both: more magnets and stops so the enclosure doesn't slide.
Leo
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-05-19T17:12:52.945Z Reads: 452

```
Lol and if it don't work......velcro lol
```

---
## \#12 Posted by: mcfly777 Posted at: 2016-05-19T17:15:55.803Z Reads: 456

```
I have velcro + straps to fix the battery/components to the deck. And I think I might add a thin strip of velcro to the enclosure/deck interface as well.
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-05-19T17:22:40.519Z Reads: 452

```
Would best leave the Velcro option last since it will add distance to the magnets ... Making them less or ineffective 

Someone needs to invent magnetic Velcro lol
```

---
## \#14 Posted by: mcfly777 Posted at: 2016-05-19T17:48:45.055Z Reads: 454

```
If I use Velcro I will recess it by about 3mm so that the magnets still touch :) I have to work on the design of the enclosure maybe later today.
```

---
## \#15 Posted by: mcfly777 Posted at: 2016-05-20T03:03:30.611Z Reads: 483

```
And here's the updated version
- 5 magnets on each side
- 2 holes on each side for clevis pins

To-do:
- holes for balance charging port and xt60
- hole for XT90 switch

<img src="/uploads/db1493/original/2X/a/a36e0f3ec8812864d76fea284c58731eb2a24c27.png" width="690" height="469">

<img src="/uploads/db1493/original/2X/f/f4056fbb6d33379661b3a862d93ed1b084169496.png" width="600" height="500">
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2016-05-20T03:36:18.055Z Reads: 454

```
Sweeeeeeeeeeetnesssssa
```

---
## \#17 Posted by: mcfly777 Posted at: 2016-05-21T01:48:53.951Z Reads: 467

```
New version
I made it so that there's a smaller part (the front) where all the cables will stay, and which will stay permanently connected to the deck, and a removable lid, that can be secured by either magnets OR clevis pins. I'm printing the first front part now. The  connectors are: XT60 and 6S balance charge connector.

To-do 
-voltmeter
-add curved deck outline so there's no gap when the enclosure is sitting close to the deck

<img src="/uploads/db1493/original/2X/4/4f17c77464f49a0833f51ac605d57cdedcc57a3d.png" width="690" height="322">
```

---
## \#18 Posted by: lox897 Posted at: 2016-05-21T02:34:14.842Z Reads: 460

```
Do you use Solidworks? Sorry if you have already said this.
```

---
## \#19 Posted by: mcfly777 Posted at: 2016-05-21T03:00:01.403Z Reads: 466

```
No, using Fusion 360.
```

---
## \#20 Posted by: mcfly777 Posted at: 2016-05-22T17:06:31.494Z Reads: 504

```
Current iteration. Now with space for a voltmeter, an XT60 port to charge and connect to VESC, a 6s balance port, and an XT90 loop. I'm printing the larger piece now and will test fit.

<img src="/uploads/db1493/original/2X/3/398604314944a1cfbd82de041896727f1d87ec1a.png" width="690" height="459">

<img src="/uploads/db1493/original/2X/0/045e42e14492694d1840f0cc7ec91662ab905afa.jpg" width="500" height="500">

<img src="/uploads/db1493/original/2X/a/a20a428a233c2dc414dd0259414ee3c79c3b6366.jpg" width="500" height="500">
```

---
## \#21 Posted by: jakobnator Posted at: 2016-05-25T05:27:20.103Z Reads: 489

```
Very cool, I also am working on a 3d printed enclosure (Not nearly as well designed). I solved the delamination issue with some ABS sludge on the heated bed, (mix of acetone and ABS filament). Magnets are very cool solution to mounting. Currently I am using threaded inserts that are used in furniture but I have no idea how long those will last. Do you plan to connect the two boxes with wires across the board or are you routing them a la boosted board style? My first enclosure had two 10 AWG wires that ran down it and I hated it, so I am just hoping that the ABS is flexible enough to bend as one box instead of two.

Here is the first generation, looking to reprint when I extend my 3d printer to a 300x200mm build size. 
https://dl2.pushbulletusercontent.com/dBhwrzrf8Zn2ocHeVsENFRxJUL9f8hdL/IMG_20160525_012252.jpg
```

---
## \#22 Posted by: mcfly777 Posted at: 2016-05-25T14:59:51.998Z Reads: 485

```
I haven't decided how I will route the wires between the battery and VESC. I have just made extensions to my box so if I need more space I can just print another one. Also, if the deck bends, the top of the boxes can  open a little bit.Note that no components will be fixed to the enclosure, everything is stuck to the deck itself. See below for diagram.

As for material, I have printed it using PETG which is fusing each layer very well and it doesn't have the shrinkage issue of ABS.

<img src="/uploads/db1493/original/2X/e/ebb79d0bb7b9e598698c53c5a24d9b8542b5348f.png" width="690" height="434">
```

---
## \#23 Posted by: jakobnator Posted at: 2016-05-25T16:26:53.541Z Reads: 453

```
Yea my deck flexes a bit too and the middle does seem to split if I stand on the middle of it. I have been toying with the idea of making a single enclosure with two halves that are connected with some flexible rubber so that the very middle of the enclosure is flexible yet still watertight.
```

---
## \#24 Posted by: JLabs Posted at: 2016-05-25T16:47:28.509Z Reads: 439

```
That's a nice enclosure! I designed something similar in 123d and am working on a F360 version... This is very well done. How long have you been modeling?
```

---
## \#25 Posted by: mcfly777 Posted at: 2016-05-25T17:17:27.139Z Reads: 448

```
hey @JLabs thanks, I am new to modeling. Have designed only small items so far, but watching a lot of youtube videos and trying a lot of stuff. I guess Fusion 360 really made sense for me so that's what I'm using. And it's free :slight_smile:

Still my biggest question is how to attach this to the deck. I think I'll use 6-32 brass wood inserts. But I need to modify this design so that if I want to add more of the middle sections the holes will continue to line up. But I have printed already what you see there and I'm lazy to do all the calculations for this...but I think I'll have to do it so that I only have to drill the deck once and at regular spacing....
```

---
## \#26 Posted by: JLabs Posted at: 2016-05-25T17:22:01.340Z Reads: 421

```
I used shoulder head cap acres, they are flush with the deck and I have nuts on the other side of the enclosure
```

---
## \#27 Posted by: jakobnator Posted at: 2016-05-25T17:29:11.748Z Reads: 422

```
Although it is nice to have threaded inserts on one side, from my experience go with the T-nuts like JLab uses, brass sheers really easily and when screwing mine in about half of them snapped and they almost go through the thickness of the board anyways.
```

---
## \#28 Posted by: mcfly777 Posted at: 2016-05-25T18:47:14.702Z Reads: 426

```
thanks @JLabs and @jakobnator. I have no experience with inserts but if they are not enough then the T-nuts are my next choice

Leo
```

---
## \#29 Posted by: mcfly777 Posted at: 2016-05-30T18:10:41.213Z Reads: 424

```
Continued at my build topic http://www.electric-skateboard.builders/t/untitled-sector-9-faultline-torqueboards-trucks-tb-motor-230kv-torqueboards-v4-mount-6s-vesc/3085
```

---
## \#30 Posted by: LAVAMAN Posted at: 2016-12-31T18:41:19.251Z Reads: 318

```
Good job on the 3-D printed enclosure. Doing it in sections so it will flex a little as well as being able to lengthen it in the future is a great idea. You could also add some sort of O-ring or rubber gasket to keep water out. I want to do something very similar for my build. How long does it take you to print the enclosure? 

I have been also looking for a solution for fastening enclosure to the bottom of the board. I was thinking of the "DZUS" fastener. They are used for quick panel access in racing applications like motorcycles, airplanes, etc. No tools necessary. Just a spring loaded knob. I provided a link below.

http://www.southco.com/en-us/d9
```

---
## \#31 Posted by: dedinski Posted at: 2017-02-21T15:56:50.723Z Reads: 286

```
Any chance you could share the file so i can print it? My design looks like crap :)
```

---
## \#32 Posted by: dedinski Posted at: 2017-03-05T15:58:57.464Z Reads: 267

```
Wow, that would be really nice to pop that baby open quickly.
```

---
## \#33 Posted by: taycro Posted at: 2017-08-12T01:17:36.516Z Reads: 212

```
Hey man, that looks awesome! I was wondering if you could share the CAD files with me. I am currently designing my own enclosure, but I am struggling with the slots in the wall for the various items. I was thinking that I could just look at your files and copy the ports. That is all I want. If you could do that for me, I would really appreciate it. Thanks.
```

---
## \#34 Posted by: mcfly777 Posted at: 2017-08-12T02:45:15.338Z Reads: 201

```
Hey!
Here's the download link

https://u109281.dl.dropboxusercontent.com/u/109281/enclosure.zip
```

---
## \#35 Posted by: taycro Posted at: 2017-08-12T20:35:01.344Z Reads: 190

```
Is all of you stuff going in this enclosure? Also, how thick are the walls of you enclosure?
```

---
## \#36 Posted by: jm.riviere Posted at: 2017-11-06T14:28:21.465Z Reads: 156

```
Hey Mate, I'm a bit late to the game and the link doesn't seem to work anymore (file not found)! Would you mind putting your model back online? Thanks! :blush:
```

---
## \#37 Posted by: taycro Posted at: 2017-11-20T03:45:38.909Z Reads: 147

```
Hey could you possibly send me your F360 model? Thanks!
```

---
## \#38 Posted by: pvcaesbroeck Posted at: 2018-01-21T11:27:00.099Z Reads: 126

```
Hello mcfly777, thank you for sharing your model. Would you mind activating the link again? It doesn't seem to work anymore.
Thanks again.
```

---
## \#39 Posted by: D_Sk8 Posted at: 2018-02-03T22:37:13.911Z Reads: 112

```
Any chance you can re-activate?
```

---
