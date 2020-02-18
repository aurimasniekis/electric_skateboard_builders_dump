# HW6.4 based ESC - ESCape

### Replies: 997 Views: 54306

## \#1 Posted by: stewii Posted at: 2017-11-07T01:40:10.746Z Reads: 1364

```
Hi all.

To stop hijacking the VESC6 thread I am opening this one to talk about the ESC I have made based on the BV VESC6.4 schematics. The only change I have made was on the motion tracking chip. 

A few people already purchased it and almost finished them all, only waiting for the cover PCBs to arrive. So soon there will be some reviews.

This is how it looks like

<img src="/uploads/db1493/original/3X/b/1/b1dcbd2921401995acc7fe08c2410d8e0a7af7ae.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/c/f/cfb0fcf3f862023b09e431d93c4076195b66bdda.JPG" width="375" height="500">

Been using one on my esk8 with a small heatsink controlled by a nunchuck RF and an old laptops wifi antenna and it is great!

Any questions just hit me up
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-11-07T01:42:37.720Z Reads: 1192

```
What kind of differences does it have in performance with the different chip?  Is it not as responsive?  Also what kind of price difference is there?
```

---
## \#3 Posted by: scepterr Posted at: 2017-11-07T01:44:47.120Z Reads: 1174

```
any more for sale/testing? i have 95% of the components on hand, just need pcb
```

---
## \#4 Posted by: michaelcpg Posted at: 2017-11-07T01:51:57.178Z Reads: 1156

```
Looks awesome man. How much would I be looking at for a pair of these?
```

---
## \#5 Posted by: Jreamer Posted at: 2017-11-07T02:36:55.894Z Reads: 1132

```
Nice pics!
```

---
## \#6 Posted by: vishal_tejwani Posted at: 2017-11-07T02:37:22.450Z Reads: 1112

```
Post the video of it working, you shared with me iguess. People will be more intrested
```

---
## \#7 Posted by: Maxid Posted at: 2017-11-07T05:30:18.544Z Reads: 1086

```
Biggest questions: do you also have an enclosure (the direct FETs need one if I am not mistaken) and what's the price range?
```

---
## \#8 Posted by: stewii Posted at: 2017-11-07T12:44:26.938Z Reads: 1073

```
The difference is that I designed the PCB for the MPU-9250 instead of the 9150 (obsolete) but that chip doesn't come populated and it is not implemented in the firmware as far as I know.

I am selling at the moment at 130GBP  (without transfer fees) plus shipping and doesn't come with housing.
```

---
## \#9 Posted by: stewii Posted at: 2017-11-07T12:45:24.059Z Reads: 1054

```
I sell bare PCBs as well and provide BOM and stencil files.
```

---
## \#10 Posted by: egzplicit Posted at: 2017-11-07T12:50:47.223Z Reads: 1068

```
[quote="stewii, post:8, topic:37579"]
The difference is that I designed the PCB for the MPU-9250 instead of the 9150 (obsolete) but that chip doesn't come populated and it is not implemented in the firmware as far as I know.
[/quote]

Sorry to ask but how is the 9150 used in the firmware?


> I am selling at the moment at 130GBP (without transfer fees) plus shipping and doesn't come with housing

Any plans for a housing and heat sink? That’s a very good price.
```

---
## \#11 Posted by: scepterr Posted at: 2017-11-07T13:49:18.587Z Reads: 1012

```
How much for 2  bare PCBs and stencil's to NYC?
```

---
## \#12 Posted by: stewii Posted at: 2017-11-07T16:42:59.408Z Reads: 1008

```
7.5GBP (10USD) each plus shipping (8GBP). I don't sell stencils, only share the files so you can order one from your favourite stencil maker.
```

---
## \#13 Posted by: stewii Posted at: 2017-11-07T16:47:47.541Z Reads: 992

```
That 9150 is a gyro and accelerometer. It is not used in the firmware. 

I have a design for the housing, don't have a CNC mill though. I will sort something out soon.
```

---
## \#14 Posted by: akhlut Posted at: 2017-11-07T16:48:57.673Z Reads: 965

```
@scepterr want to split?  I'm down for a pcb or two.
```

---
## \#15 Posted by: Luuke Posted at: 2017-11-07T17:50:38.270Z Reads: 966

```
So your Hardware is compatible to the newest firmware (lightly modified cause of different chip)?
What about further updates? Will you implement that as well?
When are you ready to deliver?
```

---
## \#16 Posted by: JohnA Posted at: 2017-11-07T23:37:52.544Z Reads: 944

```
@akhlut and @scepterr if you guys are states side I would be in to get 2-3 of these to test out
```

---
## \#17 Posted by: scepterr Posted at: 2017-11-07T23:38:52.773Z Reads: 928

```
Sure
@JohnA we're getting just the PCB
```

---
## \#18 Posted by: JohnA Posted at: 2017-11-07T23:39:41.866Z Reads: 933

```
@scepterr yeah I’m aware, I wanna get better at smd soldering.
```

---
## \#19 Posted by: SORRENTINO Posted at: 2017-11-08T00:30:13.460Z Reads: 931

```
Reflow ovens about to be ordered lol
```

---
## \#20 Posted by: gogomrrobot Posted at: 2017-11-08T01:03:57.528Z Reads: 930

```
Here are the [STEP](https://www.dropbox.com/s/65w853vj7n660kk/HW64_housing.step?dl=0) and [STL](https://www.dropbox.com/s/525bmxqr6bk3vcy/HW64_housing.stl?dl=0) files @stewii is providing for the housing.  Can we find a cheap source to CNC machine these in A7075? Anyone?  I would be interested in (2)
```

---
## \#21 Posted by: Kug3lis Posted at: 2017-11-08T01:21:05.546Z Reads: 896

```
I could ask my father, he is making cases for VESC and other stuff. But it should be minimum like 10-20 qty to make
```

---
## \#22 Posted by: gogomrrobot Posted at: 2017-11-08T01:23:22.188Z Reads: 887

```
OK please let us know @stewii V6ESC (that's what I am calling it) will be shipping soon so maybe you can run a group buy -- you supply the units? Or list them on your webshop as that's what all the cool kids are doing now.
```

---
## \#23 Posted by: scepterr Posted at: 2017-11-08T01:48:58.546Z Reads: 873

```
Assuming I get the amount of PCBs I'm planning, hitting 10 won't be a problem
```

---
## \#24 Posted by: CamBo Posted at: 2017-11-08T05:09:54.630Z Reads: 861

```
Can anyone tell me the dimensions of the case?
I only have my phone.
```

---
## \#25 Posted by: Kug3lis Posted at: 2017-11-08T12:16:13.484Z Reads: 856

```
I talked with my father about machining the case here is some comments I received about it.

* The design contains 90º inside corners. (Not a single machine in world will be able to make it)
* There are no threads in holes

The price would be around 25€ per piece then making minimum 20 pieces. The price includes anodizing and 100mmX100mm logo engraving.
```

---
## \#26 Posted by: LukePL Posted at: 2017-11-08T13:26:00.541Z Reads: 826

```
EDM would do it 😁
```

---
## \#27 Posted by: karatektus Posted at: 2017-11-08T13:44:55.544Z Reads: 823

```
Just a few noob questions: 
Can you handsolder this? 
Do you need a hot air soldering station? 
Would a stencil be of any use without hot air?

Am i correct that the easiest way to assemble a pcb without an oven would be to apply solderpaste with the stencil -> place the parts by hand -> solder them via hot air -> repeat for the other side?
```

---
## \#28 Posted by: akhlut Posted at: 2017-11-08T13:56:56.093Z Reads: 804

```
With enough patience, planning, and skill the entire thing can be done by hand.  Honestly, I would skillet reflow the DRV/MCU side and do the other by hand.  The hardest part would be the GND pad under the DRV chip.

@stewii, do you have the physical dimensions of the PCB?
```

---
## \#29 Posted by: karatektus Posted at: 2017-11-08T13:58:38.301Z Reads: 791

```
well the ground pad under the chip pretty much means you need hot air ^^
I really am thinking about just doing it myself. it would dramatically decrease the cost :D
Edit: I just googled "skillet reflow".... thats ingenious xD
```

---
## \#30 Posted by: gogomrrobot Posted at: 2017-11-08T14:38:44.209Z Reads: 801

```
[quote="Kug3lis, post:25, topic:37579, full:true"]
I talked with my father about machining the case here is some comments I received about it.

* The design contains 90º inside corners. (Not a single machine in world will be able to make it)
* There are no threads in holes

The price would be around 25€ per piece then making minimum 20 pieces. The price includes anodizing and 100mmX100mm logo engraving.
[/quote]

Seems like a good price in am! @scepterr you in?
```

---
## \#31 Posted by: stewii Posted at: 2017-11-08T15:17:09.728Z Reads: 777

```
The PCB is 60x60mm and the internal dimensions of that housing is 64x62 mm.
We dont really need 90 degree angles, I can put fillets on the internal edges with 2mm radius, I just need to increase the internal size slightly. 
The threads don't show up on the step file because I didnt modeled them.
25 eur is a great price.
```

---
## \#32 Posted by: Kug3lis Posted at: 2017-11-08T15:22:02.170Z Reads: 761

```
I asked what best radius would be and he said that 4mm so he could machine it simpler without changing bits in one go
```

---
## \#33 Posted by: CamBo Posted at: 2017-11-08T18:45:25.324Z Reads: 768

```
@stewii is the PCB mounted to the 2 holes on the interior shelf?
If I can trim the corners of the design without affecting the functionality of the case I can mill it in my machine.
I am constrained to a 100mm diameter disc.  I think @Kug3lis came with an excellent price for production, but I may make a unit so we can test fit on a first article before running production.
```

---
## \#34 Posted by: HifuSk8 Posted at: 2017-11-08T20:59:16.094Z Reads: 776

```
<img src="/uploads/db1493/original/3X/1/7/1756f68b4f5d0d1b649e6594a7d21bd4026d1795.png" width="690" height="387">
```

---
## \#35 Posted by: karatektus Posted at: 2017-11-08T22:06:55.584Z Reads: 760

```
Where can i get the BOM? :> I would be interested in a few PCBs
```

---
## \#36 Posted by: CamBo Posted at: 2017-11-08T23:28:41.012Z Reads: 780

```
<img src="/uploads/db1493/original/3X/d/4/d4a40b9a4edb1732d01efc308b664e857c03c4ac.jpg" width="375" height="500">

I modified the cases external dimensions to fit in my machine and am running a prototype in plastic to see how it comes out.
```

---
## \#37 Posted by: stewii Posted at: 2017-11-09T00:20:49.083Z Reads: 801

```
[quote="Luuke, post:15, topic:37579, full:true"]
So your Hardware is compatible to the newest firmware (lightly modified cause of different chip)?
What about further updates? Will you implement that as well?
When are you ready to deliver?
[/quote]

Yes, 100% compatible.
I take a couple of weeks to deliver.

[quote="Kug3lis, post:32, topic:37579, full:true"]
I asked what best radius would be and he said that 4mm so he could machine it simpler without changing bits in one go
[/quote]

I have made some changes. Should be easier to make one, but I had to increase by 2mm the length, which means I will need to change the cover PCB as well.  :cry: 

https://www.dropbox.com/s/uai3mpn7pgraje0/HW64_housing_1.1.step?dl=0

[quote="CamBo, post:33, topic:37579, full:true"]
@stewii is the PCB mounted to the 2 holes on the interior shelf?
If I can trim the corners of the design without affecting the functionality of the case I can mill it in my machine.
I am constrained to a 100mm diameter disc.  I think @Kug3lis came with an excellent price for production, but I may make a unit so we can test fit on a first article before running production.
[/quote]

Yes, it is.
Thanks for doing that, I was thinking 3D print the design before we move to aluminium.

[quote="karatektus, post:35, topic:37579, full:true"]
Where can i get the BOM? :> I would be interested in a few PCBs
[/quote]

https://www.dropbox.com/s/kgdrnrdylf28ddw/HW64_BOM.ods?dl=0

[quote="CamBo, post:36, topic:37579, full:true"]
<img src="/uploads/db1493/original/3X/d/4/d4a40b9a4edb1732d01efc308b664e857c03c4ac.jpg" width="375" height="500">

I modified the cases external dimensions to fit in my machine and am running a prototype in plastic to see how it comes out.
[/quote]

looks good :) wish I had a CNC
```

---
## \#38 Posted by: ShutterShock Posted at: 2017-11-09T00:23:36.465Z Reads: 742

```
So what is the expected performance of this esc?  Would it be between the FOCBOX and the VESC 6 or would it be like the VESC 6
```

---
## \#39 Posted by: akhlut Posted at: 2017-11-09T02:13:47.608Z Reads: 773

```
Question!  How are you ensuring reliable direct connection between fets and case?  Looks like those mounting holes would lever the fets off of the heatsink if tightened down.  An additional mounting screw near the caps/power entrance tab would help eliminate this.  Alternatively, is there a clamping mechanism to hold the fets and pcb tight to the heatsink?

Also, that diode and cap look uncomfortably close to the fet and its heatsink.  

I think alot of these issues can be alleviated with minor changes to the heatsink.
```

---
## \#40 Posted by: CamBo Posted at: 2017-11-09T05:17:46.636Z Reads: 835

```
Do u know the appropriate height of the fets + solder? I would like to add a raised section around the screw holes to the model I’m working on to correct this.
```

---
## \#41 Posted by: Skifree Posted at: 2017-11-09T05:35:00.991Z Reads: 791

```
Would it be possible to make it watertight? It would be awesome if there was no need for an enclosure.
```

---
## \#42 Posted by: stewii Posted at: 2017-11-09T11:36:32.692Z Reads: 829

```
[quote="ShutterShock, post:38, topic:37579, full:true"]
So what is the expected performance of this esc?  Would it be between the FOCBOX and the VESC 6 or would it be like the VESC 6
[/quote]

Similar to VESC6.

[quote="akhlut, post:39, topic:37579, full:true"]
Question!  How are you ensuring reliable direct connection between fets and case?  Looks like those mounting holes would lever the fets off of the heatsink if tightened down.  An additional mounting screw near the caps/power entrance tab would help eliminate this.  Alternatively, is there a clamping mechanism to hold the fets and pcb tight to the heatsink?

Also, that diode and cap look uncomfortably close to the fet and its heatsink.  

I think alot of these issues can be alleviated with minor changes to the heatsink.
[/quote]

I use thermal tape on the FETs which does that job and stop them with shorting with anything else.  
I don't see any problem with cap and diode being there, parts don't move and there is thermal tape in between.

[quote="CamBo, post:40, topic:37579, full:true"]
Do u know the appropriate height of the fets + solder? I would like to add a raised section around the screw holes to the model I’m working on to correct this.
[/quote]

FETs and solder - 0.7mm
Thermal tape on top 0.3mm
```

---
## \#43 Posted by: karatektus Posted at: 2017-11-09T13:01:19.877Z Reads: 733

```
Can I already order PCBs from you? :)
```

---
## \#44 Posted by: akhlut Posted at: 2017-11-09T13:04:09.516Z Reads: 716

```
@stewii you have a link for the thermal tape?
```

---
## \#45 Posted by: qdxiatao Posted at: 2017-11-09T14:49:01.572Z Reads: 725

```
very good thanks!
```

---
## \#46 Posted by: stewii Posted at: 2017-11-09T17:51:18.106Z Reads: 774

```
[quote="akhlut, post:44, topic:37579, full:true"]
@stewii you have a link for the thermal tape?
[/quote]

Not sure why you want this but https://multimedia.3m.com/mws/media/122119O/3m-thermally-conductive-adhesive-transfer-tapes-8800-series.pdf

The new cover PCB arrived today, it might need some changes depending on the housing...

<img src="/uploads/db1493/original/3X/9/f/9f905646d6d547609ecbde2770d990358a3ae6f4.JPG" width="375" height="500">
```

---
## \#47 Posted by: CamBo Posted at: 2017-11-09T18:25:54.001Z Reads: 752

```
Here’s a pic of the case prototype I milled for science.
<img src="/uploads/db1493/original/3X/1/b/1b5ac02bf0c44bc4d12ff889ca386d3ed1e95924.jpeg" width="375" height="500">

I would need to change the clamping in the machine to fit the corners of the cover.  For the prototype I just rounded them to fit my system and moved the holes in 5mm.
```

---
## \#48 Posted by: karatektus Posted at: 2017-11-09T19:21:10.567Z Reads: 736

```
<img src="/uploads/db1493/original/3X/0/1/013e8b2bb625cb2726bd9755a3fd29bac63d4306.jpg" width="543" height="500">
```

---
## \#49 Posted by: Eboosted Posted at: 2017-11-10T07:08:45.521Z Reads: 715

```
Please @stewii make a video of your board running your VESC.

I know this is too much but if you could make a video of the VESC running on inclines and surpassing the 60k limit without frying the DRV, I and everyone i here would be pretty excited
```

---
## \#50 Posted by: scepterr Posted at: 2017-11-10T07:14:42.561Z Reads: 697

```
I've got PCBs on the way, will try it on my 6374s but ultimately going to my carvon v4xl build in January😋
```

---
## \#51 Posted by: Eboosted Posted at: 2017-11-10T07:39:55.116Z Reads: 678

```
Can't wait for it @scepterr. Those will go on my Trampa 12s 6384s
```

---
## \#52 Posted by: scepterr Posted at: 2017-11-10T07:42:19.945Z Reads: 670

```
What's awesome is I only need a handful of new components on top of 4.12 bom, and I have all the upgraded caps already too 😛
```

---
## \#53 Posted by: Fotherja Posted at: 2017-11-13T10:43:35.128Z Reads: 680

```
Hi stewii, please may I buy a PCB off you and the stencil files? I'd like to reflow up your board and have most of the components already from VESC4. I'm UK based. How can I PM you?
```

---
## \#54 Posted by: Youssless Posted at: 2017-11-13T11:10:38.131Z Reads: 674

```
to PM, click on his username and then click 'Message'.
```

---
## \#55 Posted by: Kug3lis Posted at: 2017-11-13T11:23:34.488Z Reads: 668

```
I dont think he will be able as he is new user lvl
```

---
## \#56 Posted by: stewii Posted at: 2017-11-13T19:04:58.288Z Reads: 674

```
You got PM
```

---
## \#57 Posted by: MontPierre Posted at: 2017-11-14T21:55:43.931Z Reads: 676

```
Can’t wait to see some reviews / videos!
```

---
## \#58 Posted by: ugothakd Posted at: 2017-11-17T04:07:57.213Z Reads: 686

```
What's the benefits of an enclosure vs an actual heat sink?
```

---
## \#59 Posted by: MysticalDork Posted at: 2017-11-17T04:10:07.545Z Reads: 710

```
easier to machine, cheaper in small volumes. Don't need a big finned heatsink unless you're running high continuous loads. For Esk8 applications, it's just not needed.
```

---
## \#60 Posted by: scepterr Posted at: 2017-11-17T05:57:59.227Z Reads: 723

```
Goodies came 😁
<img src="/uploads/db1493/original/3X/f/2/f22e33505bbe0af39902190f146b4db652087e28.jpg" width="666" height="500">
```

---
## \#61 Posted by: Eboosted Posted at: 2017-11-17T06:16:52.462Z Reads: 683

```
How long will you take to have one ready for testing? I can't wait for at least one review
```

---
## \#62 Posted by: chuttney1 Posted at: 2017-11-17T06:55:46.704Z Reads: 665

```
So are these two or 4 layer boards?
```

---
## \#63 Posted by: scepterr Posted at: 2017-11-17T07:40:30.584Z Reads: 657

```
As soon as components arrive

@chuttney1 dunno, didn't look, will check tomorrow
```

---
## \#65 Posted by: gogomrrobot Posted at: 2017-11-18T10:12:23.790Z Reads: 675

```
Mine are almost here I will fire them up... `In Transit to Destination`... USPS...


<img src="/uploads/db1493/original/3X/e/4/e47ed353d9ed69047023c39c42be725772c69b6e.png" width="690" height="387">
```

---
## \#66 Posted by: gogomrrobot Posted at: 2017-11-21T00:18:19.510Z Reads: 672

```
Just arrived my white label VESC6 need some CNC housing... and oh yeah a board to mount it on

<img src="/uploads/db1493/original/3X/4/2/42fc4f65177fea02bac2005088b0e529eed0f453.JPG" width="375" height="500">
```

---
## \#67 Posted by: Eboosted Posted at: 2017-11-21T05:33:04.063Z Reads: 666

```
[quote="Fotherja, post:53, topic:37579"]
u and the stencil files? I'd like to reflow up your board and have most of the components already from VESC4. I'm UK based. How can I PM you?
[/quote]

When are you going to test it, I'd like to see how it performs? Where are you getting your housings from?
```

---
## \#68 Posted by: gogomrrobot Posted at: 2017-11-21T06:42:04.379Z Reads: 663

```
[quote="Eboosted, post:67, topic:37579, full:true"]
When are you going to test it, I'd like to see how it performs? Where are you getting your housings from?
[/quote]

I have asked @stewii for the new STL files because I believe he has updated the cover.  I am hoping @Kug3lis will mill them for me but we need at least 20 people to commit to it.   Last resort I just may send it to 3dhubs which isn't a good idea to use plastic but it's something until we can get one milled proper.

Sorry I just can't get the testing done quickly -- I have (2) new boards coming but it will be a while. My existing boards, it's a pain to get the VESC's and wiring un-done and re-done. Maybe I can just solder on the motor leads though... hook it up to my lipos and show the motors run at full speed. Would that work?
```

---
## \#69 Posted by: Surfer Posted at: 2017-11-21T08:11:25.560Z Reads: 637

```
If @Kug3lis decide to make them I will be up for 2
```

---
## \#70 Posted by: Fotherja Posted at: 2017-11-21T09:37:08.082Z Reads: 639

```
Just waiting on the stencil and components. Hoping to have an assembled PCB by the end of the weekend. I'll do a review and try to upload a video then also. PCB from stewii looks excellent. For an enclosure, I'm just going to 3D print a box and clamp a lump of Aluminium over the FETs to buffer the heat spikes.
```

---
## \#71 Posted by: telnoi Posted at: 2017-11-21T11:01:13.802Z Reads: 630

```
remember reading somewhere that these direct fets are conductive. You'd need separate heat sink, or separate it with silicone(?) sheets.
```

---
## \#72 Posted by: JTAG Posted at: 2017-11-21T11:47:02.583Z Reads: 627

```
You absolutely need to insulate them :santa:!
```

---
## \#73 Posted by: ugothakd Posted at: 2017-11-21T12:46:21.854Z Reads: 630

```
One could just leave emtpty space in the case for the direct fets and mount seperate small heat sinks through the case https://www.amazon.com/gp/aw/d/B07217N5LS?psc=1
```

---
## \#74 Posted by: Kug3lis Posted at: 2017-11-21T13:20:28.256Z Reads: 641

```
not worth it... Just use insulation pads like vesc6 and focbox uses
```

---
## \#75 Posted by: Eboosted Posted at: 2017-11-21T16:06:47.303Z Reads: 643

```
[quote="Kug3lis, post:74, topic:37579, full:true"]
not worth it... Just use insulation pads like vesc6 and focbox uses
[/quote]

How are yiu going to use these insulation pads?
```

---
## \#76 Posted by: telnoi Posted at: 2017-11-21T20:53:49.941Z Reads: 637

```
they are sandwiched In between the case and the direct fets with a bit of thermal paste.
```

---
## \#77 Posted by: MysticalDork Posted at: 2017-11-22T04:00:07.013Z Reads: 645

```
They don't even really need the thermal paste.
```

---
## \#78 Posted by: telnoi Posted at: 2017-11-22T06:27:53.014Z Reads: 666

```
I guess it depends on how much room is in between the FET and the case.
The controller I have at least uses and needs thermal paste, otherwise the heat transfer would be far from optimal.
```

---
## \#79 Posted by: stewii Posted at: 2017-11-24T01:36:07.890Z Reads: 675

```
I use thermal tape for insulation and heat transfer and works great.
```

---
## \#80 Posted by: gogomrrobot Posted at: 2017-11-27T04:55:05.422Z Reads: 669

```
Updated STL files for housing...

https://www.thingiverse.com/thing:2666832
```

---
## \#81 Posted by: karatektus Posted at: 2017-11-29T11:39:37.069Z Reads: 685

```
[quote="Kug3lis, post:25, topic:37579"]
achining the case here is some comments I received about it.


The design contains 90º inside corners. (Not a single machine in world will be able to make it)
There are no threads in holes


The price would be around 25€ per piece t
[/quote]

Well I would be up for 4 of them :)
```

---
## \#82 Posted by: baxter Posted at: 2017-11-29T12:07:37.928Z Reads: 662

```
@stewii

Considering the trademark issues that have been publicised with the latest version of this ESC (which I won't go into), what name will you be giving your product? 

StewiiESC 6.4?
```

---
## \#83 Posted by: Deckoz Posted at: 2017-11-29T21:47:50.197Z Reads: 672

```
Let the building begin

<img src="/uploads/db1493/original/3X/1/2/12b30f78037e298b2bfa7cda166276b7429c5396.jpg" width="375" height="500">
```

---
## \#84 Posted by: b264 Posted at: 2017-11-29T21:49:22.281Z Reads: 646

```
[quote="Deckoz, post:83, topic:37579"]
Let the building begin
[/quote]

Do you have the source for that pcb?
```

---
## \#85 Posted by: Deckoz Posted at: 2017-11-29T21:58:25.152Z Reads: 652

```
Nope.

But the way I look at it. Stewii provided
-the bom
-stencil files
-STP for the case

The cost of a single PCB through him are maybe $2 more then it would be having the files and ordering through a company like OSHPark.

The guy took the time to design them, is selling them, has extremely quick shipping. I'll let him have the miniscule upcharge for his time invested. The schematics are open source so anyone could design a board if they so desire...
```

---
## \#86 Posted by: stewii Posted at: 2017-11-30T02:55:10.563Z Reads: 629

```
I am still not sure, I have put ESCape on the cover PCBs, I thought it was cool.
```

---
## \#87 Posted by: stewii Posted at: 2017-11-30T03:43:49.454Z Reads: 657

```
By the way, I have managed to connect an LED strip WS2812B to the ESC, I had to change a couple of files on the firmware tho, because BV forgot to change a few things from the version 4 so it would work on version 6.  If anyone is interested I can make a small tutorial. [ Video](https://www.dropbox.com/s/dqx0vlx4e9nqq21/IMG_4659.MOV?dl=0)

https://www.dropbox.com/s/dqx0vlx4e9nqq21/IMG_4659.MOV?dl=0
```

---
## \#88 Posted by: gogomrrobot Posted at: 2017-12-03T17:46:32.569Z Reads: 663

```
Demo'ing this build this weekend...stewii vesc6 of course...

<img src="/uploads/db1493/original/3X/2/a/2addf7182cdb51a023b5f8917d13f1bebf2d5e07.JPG" width="666" height="500">

https://youtu.be/gYsyd69rbE4
```

---
## \#89 Posted by: Eboosted Posted at: 2017-12-04T04:21:12.998Z Reads: 640

```
Did you figure out what was the problem with the sensors?
```

---
## \#90 Posted by: gogomrrobot Posted at: 2017-12-04T04:40:38.041Z Reads: 642

```
Not yet ... but i think it's the order of the pins. One thing i noticed on @stewii vesc6 ppm wires the servo and ground are opposite of Trampa vesc6.  I mean they are correctly labeled on his white cover but opposite of Trampa's.

What Trampa manufactured and the openly released schematics by BV seem to have a few minor differences like this.
```

---
## \#91 Posted by: scepterr Posted at: 2017-12-04T04:44:26.108Z Reads: 640

```
I should have all the components in by the end of the week to have 2 running 😁
```

---
## \#92 Posted by: gogomrrobot Posted at: 2017-12-04T04:55:43.396Z Reads: 658

```
Yep... lol solved the mystery... he soldered on the connector in reverse for the sensor wires.

Again he does have it correctly labeled on the white cover... so no error there but you will have to reverse the wires in your adapter or flip his plug around.

Look closely....

<img src="/uploads/db1493/original/3X/7/5/752aa59f5336db6f2a29d7e836689089ac01aa16.JPG" width="375" height="500">
```

---
## \#93 Posted by: Eboosted Posted at: 2017-12-04T05:08:43.197Z Reads: 621

```
Would you be able to connect a high kv motor and make a test to see if the ERPMs could at least reach 100,000 on the bench?

Sorry, I think i might asking for too much 😂
```

---
## \#94 Posted by: gogomrrobot Posted at: 2017-12-04T05:17:41.762Z Reads: 618

```
No it's fair to ask but unfortunately I don't have any high KV motors. I had some 6355 230kV motors but sold them on forum as i kinda am not a speed demon but prefer the torque.  Even with those i was highly limiting the amps to about 60A and got only to about 52,000 rpm.

All my motors are max now at 170kV :frowning:

High KV motors are growing less popular around here. I mean i get the use case we definitely need them to test the 100k limit of the DRV.

But i don't have. Maybe @scepterr, @Pimousse, @Vanarian, @Surfer ? There are lot of owners out there now.
```

---
## \#95 Posted by: scepterr Posted at: 2017-12-04T05:43:39.546Z Reads: 608

```
I only have 160,170,190 test with
And these escs will ultimately be going on my carvon v4xl build I think those are around 100
But one interesting thing I think to try will be running both motors off one ESC..
```

---
## \#96 Posted by: Eboosted Posted at: 2017-12-04T05:49:14.288Z Reads: 591

```
How would you connect them? Y connection on phase wires and then to both motors? 

How would you perform motor detection?
```

---
## \#97 Posted by: scepterr Posted at: 2017-12-04T05:51:13.512Z Reads: 587

```
Yeah just y spit, assuming motors are close enough together , would do detection individually and compare, don't think that'll be an issue. Keeping them "synced" would be the issue. They would be running sensorless.
 Maybe keeping them synced isn't an issue I dunno, as long as they're spinning at the same rate even if one starts before the other should be ok
```

---
## \#98 Posted by: Eboosted Posted at: 2017-12-04T05:55:18.053Z Reads: 588

```
What would happen on close turns when the outside wheel needs to spin faster?

Traction control won't work, you will put a lot of stress on the vesc as you would have double the amp limits for both motors. 

How about regen, you will need accept current from both motors, a huge amount for 1 controller
```

---
## \#99 Posted by: scepterr Posted at: 2017-12-04T06:00:42.311Z Reads: 586

```
Lol yes mostly valid points, not something I'm planning doing long term, just wanna see how/if it works. Current draw and regen should be identical, considering you set limits, it's as if you're running 2*40A motors or ,1*80A motor, if you set motor max to 80A.
```

---
## \#100 Posted by: Eboosted Posted at: 2017-12-04T06:07:31.089Z Reads: 594

```
Do it for science man! I'd love to see the results
```

---
## \#101 Posted by: MysticalDork Posted at: 2017-12-04T06:58:48.544Z Reads: 605

```
it should work, as long as the motors are in phase. I think you'll run into problems when you corner though, because the controller will be trying to drive one motor "ahead" of its phase, and one motor "behind". I think it'll work fine on straights, but either stutter, lock up or throw an error on turns.

Also it probably won't start two motors unless they're positioned exactly the same way to begin with.

TL;DR it would work great if there were two motors sharing a single shaft, and they had been "timed" together so the phases/magnets line up. Outside of that, I think you're gonna have problems. How large those problems will be, I dunno.
```

---
## \#102 Posted by: scepterr Posted at: 2017-12-04T07:03:23.167Z Reads: 559

```
Yeah that's the syncing issue I'm concerned about. I'm wondering if theres some clever way to solve that on carvons vs belt drive..
Already sharing single shaft technically..just the timing issue
```

---
## \#103 Posted by: MysticalDork Posted at: 2017-12-04T07:10:10.006Z Reads: 558

```
You might have better luck driving the left/right pairs rather than front/back. As in, front left and rear left as one, front right and rear right as one. That should solve the sync loss on turning, but I still don't know what you'd do with sync on startup.
```

---
## \#104 Posted by: Vanarian Posted at: 2017-12-05T22:12:20.462Z Reads: 584

```
Plop, sorry I too have low kv motors ! 85Kv and 130 respectively. Maybe one is 170 like yours.

BTW received my VESC6 (don't remember if this was posted) so big thanks to @Pimousse and @stewii again !

Maybe someone wanna test this, I'm looking to resolder the cap on other side of PCB (it leverages the cover PCB but it diminish overall  thickness by fw millimeters. I'll report back how it went, my soldering skills are making me mad hahaha
```

---
## \#105 Posted by: Eboosted Posted at: 2017-12-06T05:30:52.562Z Reads: 574

```
So, still no one has tested the hardware with high current?
```

---
## \#106 Posted by: Kug3lis Posted at: 2017-12-11T19:54:17.393Z Reads: 608

```
Here is the final prototype made just now. The minimum order quantity is 20 and the price is 25 eur each + shipping.

<img src="/uploads/db1493/original/3X/b/5/b5533469ebc58f852467389d9e90387dd3c8de65.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/a/c/ace55b716475db51b913bf022a97d91bedcb3595.jpg" width="375" height="500">
```

---
## \#107 Posted by: scepterr Posted at: 2017-12-11T20:00:22.970Z Reads: 580

```
@JohnA @akhlut
We down for 6?
```

---
## \#108 Posted by: akhlut Posted at: 2017-12-11T20:25:58.893Z Reads: 578

```
Yeah, I'm in for two.
```

---
## \#109 Posted by: Surfer Posted at: 2017-12-11T20:53:42.614Z Reads: 574

```
Me two... We are almost there!!
```

---
## \#110 Posted by: SORRENTINO Posted at: 2017-12-11T20:55:24.727Z Reads: 567

```
@Deckoz 

10char
```

---
## \#111 Posted by: karatektus Posted at: 2017-12-11T21:32:14.403Z Reads: 559

```
Count me in for four(4) :>
```

---
## \#112 Posted by: gogomrrobot Posted at: 2017-12-11T21:49:35.087Z Reads: 549

```
two here .........
```

---
## \#113 Posted by: karatektus Posted at: 2017-12-13T11:03:08.634Z Reads: 538

```
so we are at 12?
```

---
## \#114 Posted by: uigiroux Posted at: 2017-12-14T16:51:10.059Z Reads: 550

```
I'll be wanting 2.  Will this have a cover plate or will it be open?
```

---
## \#115 Posted by: karatektus Posted at: 2017-12-14T23:15:12.317Z Reads: 559

```
you can get the cover plate from stewii its a pcb.
```

---
## \#116 Posted by: gogomrrobot Posted at: 2017-12-15T00:19:59.488Z Reads: 571

```
He includes the white cover plate in his price.

@Kug3lis is making the CNC aluminum housing for the bottom -- 25 euro is very cheap.  You can also 3D print an ABS or PLA housing... the STL files are linked on this thread.
```

---
## \#117 Posted by: Boardnamics Posted at: 2017-12-15T01:51:32.625Z Reads: 571

```
Count me in for 1, not just the PCB but the whole thing.
```

---
## \#118 Posted by: Deckoz Posted at: 2017-12-15T01:53:26.114Z Reads: 573

```
[quote="Boardnamics, post:117, topic:37579"]
whole thing.
[/quote]

Pm @stewii directly... He'll ship you the hardware..

You'll have to message @Kug3lis for the aluminum case 

Two separate things you'll need to make whole on your own ;)
```

---
## \#119 Posted by: telnoi Posted at: 2017-12-15T10:29:54.713Z Reads: 558

```
would recommend sticking to PETG, ABS or equivalent cases. 
PLA starts to deform at 50 degrees C.
```

---
## \#120 Posted by: akira Posted at: 2017-12-15T12:19:35.854Z Reads: 558

```
I ordered PCBs from @stewii at the very beginning (first version of the PCB). 
Will the case also fit my PCBs or do they only fit the second iteration of the design ?
```

---
## \#121 Posted by: stewii Posted at: 2017-12-15T17:27:19.263Z Reads: 569

```
Can you PM me in order to make arrangements so I can test fit this and make adjustments if needed?
```

---
## \#122 Posted by: stewii Posted at: 2017-12-15T17:35:37.535Z Reads: 553

```
It will fit, but you need a different cover PCB which I already have made.
But bare in mind I still need to test fit this housing first.
 [quote="akira, post:120, topic:37579, full:true"]
I ordered PCBs from @stewii at the very beginning (first version of the PCB). 
Will the case also fit my PCBs or do they only fit the second iteration of the design ?
[/quote]

By the way, in case you are interested in a ESCape can you please use this [FORM](https://goo.gl/forms/6KqTij6iPoSegpUK2)?
```

---
## \#123 Posted by: akira Posted at: 2017-12-15T19:22:37.406Z Reads: 543

```
Well, I am not sure I fit in the Form. I would like two housings without the PCB (which I already have ...). 
Is that possible ?
```

---
## \#124 Posted by: Minim Posted at: 2017-12-23T15:54:14.862Z Reads: 545

```
How much is it for a set of ESCs and what is the ETA on a set? Where are you shipping from? 

Btw, do you have a 3d model of the boards with components fitted to make it easier to design a case.
```

---
## \#125 Posted by: leonsc Posted at: 2017-12-24T23:29:19.566Z Reads: 522

```
Has anybody run these yet would love to see some really world test not just bench. Also a cheeky set up vid wouldn't go a miss thanks and keep up the good work.
```

---
## \#126 Posted by: GrecoMan Posted at: 2017-12-24T23:53:30.194Z Reads: 518

```
99% sure @gogomrrobot used one
```

---
## \#127 Posted by: gogomrrobot Posted at: 2017-12-25T02:02:55.078Z Reads: 545

```
i will get something out soon tomorrow double motor and double stewii vesc6 (escape) with hm-10 ... post a vid on big here

stuffing my face atm... merry xmas!
```

---
## \#128 Posted by: gogomrrobot Posted at: 2017-12-26T08:42:11.026Z Reads: 564

```
So here is the double ESCape on 80A. It is like a rocket. I added the hm-10 but still haven't configured it. Need to finish that and the bms wiring.

<img src="/uploads/db1493/original/3X/5/7/57037efa57df150cabe16c2ca9145fe5db161aed.JPG" width="666" height="500">

Video up a 20% hill... 25% throttle:

https://youtu.be/Xa_DpN8LmOA


I will go really fast once i finalize the build.
```

---
## \#129 Posted by: Acido Posted at: 2017-12-26T11:05:13.882Z Reads: 540

```
Where can I get one and for how much!!!
```

---
## \#130 Posted by: LukePL Posted at: 2017-12-26T11:27:33.291Z Reads: 531

```
PM @stewii he's the man :)
```

---
## \#131 Posted by: Vanarian Posted at: 2017-12-26T11:41:49.846Z Reads: 530

```
**SICK** and here I have two babies like this one, your run made me happy !
```

---
## \#132 Posted by: gogomrrobot Posted at: 2017-12-26T16:03:13.387Z Reads: 548

```
haha... it was nothing I was going so slow like 15mph maybe because no protective gear on and batteries on by a bungie cord.  It can fly up that hill on full blast.

https://youtu.be/pIIOgt7yk-g
```

---
## \#133 Posted by: Eboosted Posted at: 2017-12-31T06:01:46.179Z Reads: 546

```
Building mine ATM

<img src="/uploads/db1493/original/3X/d/3/d31aa493d6bd8e9cbce90fe22e49479dcb80f406.jpg" width="666" height="500">
```

---
## \#134 Posted by: Boardnamics Posted at: 2017-12-31T06:11:51.504Z Reads: 525

```
How thick is the copper tracing on these pcbs? Just curious
```

---
## \#135 Posted by: wmj259 Posted at: 2017-12-31T06:33:32.742Z Reads: 523

```
Let us know if you have any aha moments in making the escape. I'm gonna try it also.
```

---
## \#136 Posted by: scepterr Posted at: 2017-12-31T06:58:43.486Z Reads: 522

```
Looking good 👍
I have the bom sitting around for 2....I really should stop procrastinating 😋
```

---
## \#137 Posted by: Vanarian Posted at: 2017-12-31T16:44:27.089Z Reads: 523

```
Just get the build started :japanese_ogre:
```

---
## \#138 Posted by: SpeedyGonzales Posted at: 2017-12-31T17:35:22.043Z Reads: 542

```
This is fantastic build. Once I get hold of one of these babies I will make case with heatsink for it. 
Similar to the one I made for VESC 4.12 that was a brain cramp.
I think that this will work well with ESCape.<img src="/uploads/db1493/original/3X/b/f/bf354b71a96a6acb79d68fda335bee35eee089e3.JPG" width="690" height="388">
<img src="/uploads/db1493/original/3X/8/f/8fedaf60e14789687b04ccc7828d63d520f1adc0.JPG" width="690" height="388">
```

---
## \#139 Posted by: banjaxxed Posted at: 2017-12-31T18:32:35.068Z Reads: 548

```
Ah man I wanna play too but seem to be in the 'no homers' club<img src="/uploads/db1493/original/3X/4/4/445cf2a87f4c11ddda7c584f0ffc8a744f240881.JPG" width="365" height="500">
```

---
## \#140 Posted by: Stevemk14ebr Posted at: 2017-12-31T18:40:21.773Z Reads: 546

```
If you're mounting directly to the trucks i'd add some rubber, vibrations can wreak havoc on electronics.
```

---
## \#141 Posted by: SpeedyGonzales Posted at: 2017-12-31T19:35:43.208Z Reads: 555

```
That new ESCape will be going on an e-bike. At this point I have it running on standard VESC and 6374 motor and getting 30 mph out of it. I'm hoping for 40 mph with 8072 motor.<img src="/uploads/db1493/original/3X/2/b/2bad958cd01e8afe8b0acb139c5e9773461f364d.JPG" width="690" height="388">
```

---
## \#142 Posted by: wmj259 Posted at: 2017-12-31T19:37:09.454Z Reads: 540

```
That's nice. How (if you have) did you fix the issue with having the motor "assist" such that you can also pedal?
```

---
## \#143 Posted by: bigben Posted at: 2017-12-31T19:38:44.060Z Reads: 530

```
Complete non Ebike persons question here, but is that a kit or is it all home built?
```

---
## \#144 Posted by: SpeedyGonzales Posted at: 2017-12-31T19:43:28.688Z Reads: 532

```
@wmj259 Two freewheels. One on the chainring; the other on the transmission of the motor.
This is standard for a mid-drive ebike.
@bigben All home built.
```

---
## \#145 Posted by: wmj259 Posted at: 2017-12-31T19:44:50.292Z Reads: 524

```
That is really nice. Good work! How much would you say it cost?
```

---
## \#146 Posted by: SpeedyGonzales Posted at: 2017-12-31T19:49:45.106Z Reads: 523

```
Tools and components about 2k.
I machined parts myself. It took me a long time but it was tons of fun.
```

---
## \#147 Posted by: Lionpuncher Posted at: 2017-12-31T20:34:29.452Z Reads: 515

```
That's an absolute beauty! Great work. I hope to be able to build a sweet e bike one fine day.
```

---
## \#148 Posted by: mikenyc Posted at: 2017-12-31T21:54:53.503Z Reads: 515

```
sweet bong dude lol
```

---
## \#149 Posted by: gogomrrobot Posted at: 2017-12-31T22:27:01.523Z Reads: 510

```
ahh shoot good eye ~~ need to edit better :slight_smile:
```

---
## \#150 Posted by: Okami Posted at: 2018-01-01T16:30:18.315Z Reads: 531

```
@SpeedyGonzales  Did u also make this "star / snowflake" shaped battery holders? 

Look really nice. Would be interesting to see the battery closer
```

---
## \#151 Posted by: SpeedyGonzales Posted at: 2018-01-02T02:55:21.957Z Reads: 544

```
@Okami
Yes, this is one of the kind battery build. I designed it for very specific purpose. 
I'm planning to take my e-bike with me to other countries by an airplane and I can't take battery with me, so I built it so I can take the case with all the stuff with me. I will buy cells locally and put it all together without welding or soldering. That will take about 30 minutes.
BTW: I call it gatling gun barrel shape. <img src="/uploads/db1493/original/3X/b/6/b6330fecdf7fdd06249eac4bf0341c9a6e935a51.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/1/5/15bf609779ebeea56064a1b8efee27a370b6f685.JPG" width="281" height="500">
```

---
## \#152 Posted by: bimmer Posted at: 2018-01-02T05:36:03.839Z Reads: 528

```
impressive
```

---
## \#153 Posted by: Minim Posted at: 2018-01-02T05:48:28.952Z Reads: 525

```
Love that idea. I guess this could work for a flat pack also?
```

---
## \#154 Posted by: bimmer Posted at: 2018-01-02T06:01:18.078Z Reads: 539

```
Ordered a couple pcb's gonna 3d print this and chop down some aluminum heat sinks with a miter saw and insert them with epoxy then add a layer of non conductive thermal adhesive.
Also I added posts for a 25x25mm fan incase someone needs some extra cooling. It could use these https://www.amazon.com/Gdstime-Small-Plastic-Brushless-Cooling/dp/B01DA3OFZE/ref=sr_1_2?s=electronics&ie=UTF8&qid=1514873849&sr=1-2&keywords=5v+25mm+fan
<img src="/uploads/db1493/original/3X/c/b/cb6bc9849ab74777533a8d568b9266489e39d9b2.jpg" width="690" height="345"><img src="/uploads/db1493/original/3X/e/e/ee86a5664cae3b45bba360c5e1cf41a4d2b5a23b.jpg" width="690" height="345">
Stl no fan https://drive.google.com/open?id=1ZR4IiuZeFCTZgsCBcaUjrzg024h5d4Uo
Stl with fan https://drive.google.com/open?id=16S6ADTb8RXN95BlpL8WluroiPIRqbnT5
```

---
## \#156 Posted by: Okami Posted at: 2018-01-02T11:02:54.247Z Reads: 510

```
Now that u show it in close up, it does resemble guns barrel :) looks very cool / stylish non the less.

I suppose it took quite some time to design the holder and then later on machine all the parts. Otherwise really impressive indeed
```

---
## \#157 Posted by: stewii Posted at: 2018-01-02T16:43:48.751Z Reads: 522

```
[quote="Boardnamics, post:134, topic:37579, full:true"]
How thick is the copper tracing on these pcbs? Just curious
[/quote]

It is 1oz on all the layers.
Might do 2oz on the next batch but not sure if it is worth it.


[quote="SpeedyGonzales, post:141, topic:37579, full:true"]
That new ESCape will be going on an e-bike. At this point I have it running on standard VESC and 6374 motor and getting 30 mph out of it. I'm hoping for 40 mph with 8072 motor.
[/quote]

That looks amazing!


For all those who filled the google form I will contact you directly.
```

---
## \#158 Posted by: stewii Posted at: 2018-01-02T16:49:06.772Z Reads: 506

```
Where can I buy a kit like that ? :smiley:
```

---
## \#159 Posted by: Kug3lis Posted at: 2018-01-02T16:50:29.249Z Reads: 514

```
@stewii I wrote you a message last year regarding the case situation did you received it?
```

---
## \#160 Posted by: FredrikHems Posted at: 2018-01-02T16:53:18.420Z Reads: 525

```
It it possible to buy the whole esc, ready to use? Or do you just sell the pcb's?
```

---
## \#161 Posted by: stewii Posted at: 2018-01-02T17:00:22.246Z Reads: 532

```
sorry I missed it, I replied now.

[quote="FredrikHems, post:160, topic:37579, full:true"]
It it possible to buy the whole esc, ready to use? Or do you just sell the pcb's?
[/quote]

I also sell the whole ESCape, ready to use.
```

---
## \#162 Posted by: FredrikHems Posted at: 2018-01-02T19:14:38.133Z Reads: 525

```
What is the price for the ready to use one?
```

---
## \#163 Posted by: Sparc Posted at: 2018-01-02T19:50:01.190Z Reads: 507

```
@stewii I submitted a request using the form you provided.  I'm interested in 2 complete units if possible.
```

---
## \#164 Posted by: SpeedyGonzales Posted at: 2018-01-02T21:09:58.044Z Reads: 534

```
So far it is one of a kind prototype. It runs great, but I think that more power would make it more fun. That's why I'm interested in using your new board. Once I have it running with 8072 motor I will beef-up mechanical components and go from there.
BTW: Is your board preloaded with firmware and tested with motor before being shipped?
Will it work with BLDC tool and/or VESC tool?
Will I be able to run 70A continuous with a good heatsink?
```

---
## \#165 Posted by: stewii Posted at: 2018-01-03T16:48:52.396Z Reads: 568

```
It is £150 but it might change depending on the PCBA prices.

[quote="FredrikHems, post:162, topic:37579, full:true"]
What is the price for the ready to use one?
[/quote]


[quote="SpeedyGonzales, post:164, topic:37579, full:true"]
So far it is one of a kind prototype. It runs great, but I think that more power would make it more fun. That's why I'm interested in using your new board. Once I have it running with 8072 motor I will beef-up mechanical components and go from there.
BTW: Is your board preloaded with firmware and tested with motor before being shipped?
Will it work with BLDC tool and/or VESC tool?
Will I be able to run 70A continuous with a good heatsink?
[/quote]

Yes it is programmed with firmware and tested.
Yes, it works with VESC tool, I havent tested with BLDC tool but it should work too.
It is all about temperature, expect similar behaviour to VESC6, it depends on the heatsink, active heatsink even better. 


Here is some photos, housing is now being tested.

<img src="/uploads/db1493/original/3X/4/0/40e140637eda8a7fca0c63b3fceb1adf57db8a5d.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/b/db5d2ae4659180ac933e61e0e0818c0dcb537a95.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/f/dfe4e9f2650b3ab606d9ced4163c90cd5473c977.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/c/8/c82254137963eb7e142a73ebb2fe8e242ee89dc3.JPG" width="375" height="500">
```

---
## \#166 Posted by: squishy654 Posted at: 2018-01-03T17:22:57.175Z Reads: 516

```
Take my money please!
```

---
## \#167 Posted by: SpeedyGonzales Posted at: 2018-01-03T22:04:31.102Z Reads: 505

```
Great! Once you are ready to ship please PM me your PayPal account and I will shoot money your way.
```

---
## \#168 Posted by: Minim Posted at: 2018-01-04T23:55:35.857Z Reads: 503

```
How long is the current lead time?
```

---
## \#169 Posted by: youyoung21147 Posted at: 2018-01-06T01:30:23.589Z Reads: 504

```
Hi and congrats for this advanced ebike build ! I'm admirative with your patience at machining work and the excellent design of the battery pack ! Add cell-level fuses and it's good for NASA missions !

Did you know you can ship an unlimited amount of 100Wh batteries in cabin luggage ? Separately packing your 6-cell modules would qualify for air transport in cabin luggage.

This way you can buy the cells and take them wherever you need :)
```

---
## \#170 Posted by: SpeedyGonzales Posted at: 2018-01-06T03:42:50.862Z Reads: 513

```
Thank you dude. You are very kind.
I think that if I try to fly with these batteries I would be arrested, sentenced and executed. :grinning:
I don't think that I will have a chance in hell with 60 pcs. of 18650s. These are not your typical consumer batteries. You might even have a point but try to tell that to one of TSA guys. They will probably think that it is big caliber ammo. :confused:
 
Batteries Allowed in Carry-on Bags:
•Dry cell alkaline batteries; typical AA, AAA, C, D, 9-volt, button sized cells, etc.
•Dry cell rechargeable batteries such as Nickel Metal Hydride (NiMH) and Nickel Cadmium (NiCad).
•Lithium ion batteries (a.k.a.: rechargeable lithium, lithium polymer, LIPO, secondary lithium).
•Consumer-sized lithium ion batteries [no more than 8 grams of equivalent lithium content or 100 watt hours (wh) per battery]. This size covers AA, AAA, 9-volt, cell phone, PDA, camera, camcorder, Gameboy, and standard laptop computer batteries.
•Up to two larger lithium ion batteries (more than 8 grams, up to 25 grams of equivalent lithium content per battery) in their carry-on. This size covers larger extended-life laptop batteries. Most consumer lithium ion batteries are below this size.
•Lithium metal batteries (a.k.a.: non-rechargeable lithium, primary lithium). These batteries are often used with cameras and other small personal electronics. Consumer-sized batteries (up to 2 grams of lithium per battery) may be carried. This includes all the typical non-rechargeable batteries for personal film cameras and digital cameras (AA, AAA, 123, CR123A, CR1, CR2, CRV3, CR22, 2CR5, etc.) as well as the flat round lithium button cells.
```

---
## \#171 Posted by: stewii Posted at: 2018-01-07T01:14:53.798Z Reads: 477

```
It is 2-3 weeks.
```

---
## \#172 Posted by: SpeedyGonzales Posted at: 2018-01-07T16:31:04.868Z Reads: 478

```
Great! Looking forward to putting your creation to work.
```

---
## \#173 Posted by: qdxiatao Posted at: 2018-01-09T00:48:32.327Z Reads: 475

```
thanks for your work
```

---
## \#174 Posted by: bimmer Posted at: 2018-01-09T02:14:52.894Z Reads: 474

```
Got mine today look great but the fets are sold out  in the US :smiley:
```

---
## \#175 Posted by: Maineo Posted at: 2018-01-09T09:42:04.051Z Reads: 473

```
@stewii I submitted the form for the esc a while ago, but just in case it didn't go though. I'm interested in one esc with the housing.
```

---
## \#176 Posted by: stewii Posted at: 2018-01-09T10:47:22.352Z Reads: 483

```
not only in the USA, irf7749l1trpbf and irf7749l2trpbf out of stock everywhere! :frowning: 

[quote="bimmer, post:174, topic:37579, full:true"]
Got mine today look great but the fets are sold out  in the US :smiley:
[/quote]


Hi, sorry for the delay, trying to find a source for the FETs, factory lead time is huge. And also housings are a bit delayed too. But I will contact you all who filled the form.


[quote="Maineo, post:175, topic:37579, full:true"]
@stewii I submitted the form for the esc a while ago, but just in case it didn't go though. I'm interested in one esc with the housing.
[/quote]
```

---
## \#177 Posted by: bimmer Posted at: 2018-01-09T11:43:06.395Z Reads: 461

```
Bought the last 16 and now have to wait 26 weeks to finish the other 2 boards :confused: who bought all the fets just days ago there were literall thousands available
```

---
## \#178 Posted by: bimmer Posted at: 2018-01-09T11:54:51.917Z Reads: 451

```
Would these work? AUIRF7749L2CT-ND
```

---
## \#179 Posted by: SimosMCmuffin Posted at: 2018-01-09T12:24:29.025Z Reads: 473

```
You should able to use those. I just checked the available parts on digi-key with the search term "irf7749l" and it would seems that the "AUIRF7749L2CT-ND" is just the automotive grade version of the standard "IRF7749L"1/2"TRPBFCT-ND" FET and that's why it's a bit more expensive as well. Performance should be identical or maybe even marginally better.

https://www.digikey.fi/product-detail/en/infineon-technologies/AUIRF7749L2TR/AUIRF7749L2CT-ND/6559910
```

---
## \#180 Posted by: Kug3lis Posted at: 2018-01-09T12:38:52.827Z Reads: 486

```
[quote="bimmer, post:178, topic:37579"]
IRF7749
[/quote]

https://octopart.com/search?q=IRF7749
```

---
## \#181 Posted by: bimmer Posted at: 2018-01-09T14:45:54.015Z Reads: 496

```
Yes I was aware of octopart  but if you click on the ones that  say stocked on the actual websites they are all sold out.
```

---
## \#182 Posted by: Kug3lis Posted at: 2018-01-09T14:51:17.704Z Reads: 501

```
I dont know what are you talking about but here is first link:

<img src="/uploads/db1493/original/3X/0/2/0202fe8fff856f095852b0fdbdc49444f857a148.png" width="690" height="402">
```

---
## \#183 Posted by: stewii Posted at: 2018-01-09T15:08:43.871Z Reads: 476

```
I haven't tried those ones but they should work. They are a touch higher on power dissipation and drain current and higher Vgs max, they should perform marginally better as SimosMCmuffin said.
```

---
## \#184 Posted by: bimmer Posted at: 2018-01-09T23:40:22.340Z Reads: 462

```
Sorry I was thinking more along the lines or US based sellers. But I do appreciate the help and effort.
```

---
## \#185 Posted by: bimmer Posted at: 2018-01-09T23:40:41.608Z Reads: 459

```
Well I bought them.
```

---
## \#186 Posted by: notepad Posted at: 2018-01-09T23:43:31.557Z Reads: 448

```
anyone tested the max erpm yet?  Got lots of cash for these if we can get specs for how far they go before they pop.
```

---
## \#187 Posted by: bimmer Posted at: 2018-01-10T02:18:32.067Z Reads: 445

```
Mine will be ready next week gonna try and push  one or 2 to the breaking point before I commit to making a couple dozen I'll update you.
```

---
## \#188 Posted by: notepad Posted at: 2018-01-10T03:47:40.615Z Reads: 445

```
cheers,  cant wait to see!
```

---
## \#189 Posted by: Boardnamics Posted at: 2018-01-10T03:53:21.616Z Reads: 465

```
[quote="bimmer, post:178, topic:37579"]
AUIRF7749L2CT-ND
[/quote]

I also am interested in the erpm. I really want one for an rc car application but the erpm would be in the 150k ish range.
```

---
## \#190 Posted by: bimmer Posted at: 2018-01-10T23:30:47.530Z Reads: 483

```
Finished a case today my parts are still like a day or 2 out though.![20180110_162742|690x388](upload://nVRqi4yxrDuXgPgwhS0xgeyivQ8.jpg)![20180110_162736|690x388](upload://rEDuRcMQ5BQraGErXljEKrkOTuX.jpg)![20180110_162729|690x388](upload://ghTCMlWSpchV3UXaJPoICKF0yRt.jpg)`
```

---
## \#191 Posted by: Cobber Posted at: 2018-01-10T23:32:19.326Z Reads: 466

```
[quote="Boardnamics, post:189, topic:37579"]
I really want one for an rc car application but the erpm would be in the 150k ish range.
[/quote]

how many pole pairs is the motor?
```

---
## \#192 Posted by: Boardnamics Posted at: 2018-01-11T02:01:27.692Z Reads: 461

```
It's 4 pole, 4 magnets. So 2 pole pairs.
```

---
## \#193 Posted by: Cobber Posted at: 2018-01-11T02:06:45.947Z Reads: 464

```
So if erpm = number of pole pairs multiplied by rpm

You are going to be running your inrunner at 75,000 rpm?

Get that on video dude!
```

---
## \#194 Posted by: Boardnamics Posted at: 2018-01-11T02:23:01.626Z Reads: 465

```
Many inrunners can do it. They will get crazy hot though. I am running 12s on a motor that is either 1200kv or if I am pushing it, 1500kv. Keep in mind that's unloaded rpm. The way I gear it, it will not reach even close to 75k rpm. More like 50k
```

---
## \#195 Posted by: SOICDIP Posted at: 2018-01-11T03:26:27.580Z Reads: 467

```
How was the 60k ERPM limit on the VESC 4 solved on this version?
```

---
## \#196 Posted by: Hummie Posted at: 2018-01-11T03:57:00.319Z Reads: 480

```
@stewii any chance of a group buy?  the thread is long and haven't read it.
```

---
## \#197 Posted by: bimmer Posted at: 2018-01-12T01:52:04.604Z Reads: 488

```
Santa came today ![20180111_184605|690x388](upload://oLBhl9ljXLF6ImaGNHpfCwD2uGp.jpg)
```

---
## \#198 Posted by: stewii Posted at: 2018-01-12T02:18:42.105Z Reads: 481

```
Absolutely.
So far I've got 21 responses on the google form with a total of 39 ESCapes. 
I enquired a factory for production and if we get at least 40 units I will be able to sell each for £150 plus shipping with alu housing.
(since a good part of you will run dual motors I am working on a dual fully enclosure housing as well)

Of course this will be a big investment and you will need to pay in advance. Lead time 6-7 days plus 18-25 days.
```

---
## \#199 Posted by: Hummie Posted at: 2018-01-12T02:25:43.411Z Reads: 463

```
any chance of cutting off some of the components and making a bare bones double FOC machine that would be cheaper?  Only thing want is reliable foc.  even the high amp ability is overkill for me with a double and never hit an over-temp shut-down.
I imagine you have youre own plans but if you could make that...they will come.  you could get a lot more money and momentum.  Even the many white plugs and ports seem more than almost anyone uses.  just a mini usb for me please
```

---
## \#200 Posted by: stewii Posted at: 2018-01-12T02:42:11.632Z Reads: 453

```
If it is me assembling it  like I have been doing (slowly) I can customise it and make it cheaper for the buyer but will be marginal savings, ie: could not solder the wireless components or the jst connectors, switch, but that is only about £5. And of course if I go with a PCBA all the boards would have to be the same and we all want different things, so it might be difficult.
```

---
## \#201 Posted by: Hummie Posted at: 2018-01-12T02:46:58.349Z Reads: 452

```
so if it were a double barebones design cutting out everything but FOC and a reasonable amppplitude...still not much cheaper?  how do places like maytech do it?  cant we get some place that's good to do all the soldering cheaper or something?
```

---
## \#202 Posted by: Eboosted Posted at: 2018-01-12T05:18:12.290Z Reads: 492

```
Hello @stewii:
I went to try my new board today on FOC, I pressed the thottle pretty generously and it rode AMAZING for the first 10 miles, almost at the end of my ride I started to get cutouts on my slave ESCape, it was the dreaded FAULT_CODE_DRV :persevere:

I cycled the battery power on the board and remote, whent to ride again and it cutted out every 100mts throwing the same fault, I think my DRV is fried, but I don't know how could this happen on a HW6.4.

Have you got this issue?, how did you fix it?
Should I go back to BLDC to avoid it?
Is the DRV the same found on hardware V4.12? I have some DRV8302 laying around in my desk so I could change them tomorrow

[img]https://i.imgur.com/eRXF4iJ.png[/img]
[img]https://i.imgur.com/Z9ArEoe.png[/img]
```

---
## \#203 Posted by: SOICDIP Posted at: 2018-01-12T05:27:54.063Z Reads: 470

```
[quote="Eboosted, post:202, topic:37579"]
I have some DRV8302 laying around in my desk so I could change them tomorrow
[/quote]

Just letting you know, DRV8301 and 8302 are not compatible.
```

---
## \#204 Posted by: Eboosted Posted at: 2018-01-12T05:29:07.565Z Reads: 473

```
What's inside of the ESCape? DRV8301?

https://www.mouser.com/productdetail/595-drv8301dcar

Did anyone else had this DRV fault?
```

---
## \#205 Posted by: SOICDIP Posted at: 2018-01-12T05:36:30.664Z Reads: 469

```
[quote="Eboosted, post:204, topic:37579"]
What’s inside of the ESCape? DRV8301?
[/quote]


Yup, SPI controlled.
```

---
## \#206 Posted by: stewii Posted at: 2018-01-13T01:42:47.415Z Reads: 460

```
I have messaged you.
```

---
## \#207 Posted by: Stevemk14ebr Posted at: 2018-01-13T01:47:26.810Z Reads: 459

```
I've filled out the form for the group buy, will payment and such be soon?
```

---
## \#208 Posted by: Eboosted Posted at: 2018-01-13T01:47:37.351Z Reads: 461

```
Thanks @stewii I'll take the pictures and send them over to you
```

---
## \#209 Posted by: scepterr Posted at: 2018-01-13T01:50:08.495Z Reads: 464

```
I don't remember what quantity I filled out, I'll take 2 with housing, should I resubmit form?
I would also take an additional 2 single housings with PCB cover
```

---
## \#210 Posted by: SpeedyGonzales Posted at: 2018-01-13T13:40:52.373Z Reads: 459

```
What is ERPM and size of your motor?
```

---
## \#211 Posted by: Eboosted Posted at: 2018-01-13T16:41:50.126Z Reads: 458

```
I have dual 6374s 170KV motor from APS, my eRPM limit was left at 60000.
```

---
## \#212 Posted by: notepad Posted at: 2018-01-13T16:56:13.412Z Reads: 451

```
could be a simple silicone lottory faliure.  hope you get this sorted. feels bad man.
```

---
## \#213 Posted by: SpeedyGonzales Posted at: 2018-01-13T17:06:28.344Z Reads: 456

```
It looks like you were well within limits.
That sucks.
```

---
## \#214 Posted by: banjaxxed Posted at: 2018-01-13T17:48:03.396Z Reads: 453

```
Vesc 6k limit is 150k...could it be a reason elsewhere?
```

---
## \#215 Posted by: Eboosted Posted at: 2018-01-13T17:55:49.589Z Reads: 464

```
[quote="banjaxxed, post:214, topic:37579"]
uld it be a reason else
[/quote]

I switched to BLDC mode, no more cutouts, evetything working perfect. Miss FOC a little bit just for launches.

Stewii sent me some procedures to pinpoint the issue but I still need to find time to open up the enclosure
```

---
## \#216 Posted by: bimmer Posted at: 2018-01-14T07:14:27.159Z Reads: 471

```
Just finished  my first one... some parts didnt come so I borrowed them from an old vesc...while flashing the firmware there was smoke....*sigh* I'll report back when my 2. iteration of parts arrives...![20180114_001423|281x500](upload://gcOt8uOUe4rLM0nBHEEkyx6uSs7.jpg)
```

---
## \#217 Posted by: SOICDIP Posted at: 2018-01-14T07:36:17.831Z Reads: 464

```
[quote="bimmer, post:216, topic:37579"]
while flashing the firmware there was smoke
[/quote]

Can you get a closeup of the DRV?
```

---
## \#218 Posted by: bimmer Posted at: 2018-01-14T07:37:31.132Z Reads: 466

```
I just did that to the drv. :D![15159155169211645602575|281x500](upload://d0Y65K74HLJRmqaGrdFQXr55jNK.jpg)
```

---
## \#219 Posted by: scepterr Posted at: 2018-01-14T08:21:35.695Z Reads: 472

```
Is that flux or solder?
It should really be cleaned up to properly inspect, solder balls floating around

![IMG_20180114_032209|419x499](upload://25VGSgYi7iHZnJxliN2AamYH8SE.jpg)

And what's going on here
![IMG_20180114_033013|631x500](upload://nY9D6oQFD09QkviZrvsr8ekwYTT.jpg)
```

---
## \#220 Posted by: bimmer Posted at: 2018-01-14T10:02:19.595Z Reads: 467

```
To be honest this is the first smd soldering I've ever done. So its learning by doing so this was a 80$ lesson so far....
```

---
## \#221 Posted by: stewii Posted at: 2018-01-14T21:06:50.131Z Reads: 471

```
I have an inrunner 5000kv and tested it with a 3S battery (specs says 2S max) and got about 100k erpm.
Here is a printscreen, top is BLDC and bottom FOC.
![eRPM|501x500](upload://cRR9hpUptN5NWgtxuXLp2U8HH2e.png)
```

---
## \#222 Posted by: banjaxxed Posted at: 2018-01-14T21:14:19.407Z Reads: 463

```
That will buff right out
```

---
## \#223 Posted by: notepad Posted at: 2018-01-14T23:22:25.337Z Reads: 463

```
absolutly wonderful!  great to see its bullet proof at high erpm
```

---
## \#224 Posted by: bimmer Posted at: 2018-01-15T01:52:48.097Z Reads: 474

```
If I aquire a new skill im the process I'm okay with ruining s couple boards :smile: I also learned to never order the exact BOM since parts cost fractions of pennies sometimes.
```

---
## \#225 Posted by: willpark16 Posted at: 2018-01-15T02:12:44.318Z Reads: 478

```
I just taught myself an $80 lesson yesterday trying to make a carvon fiber deck it's all in the game brother
```

---
## \#226 Posted by: SpeedyGonzales Posted at: 2018-01-15T02:55:49.504Z Reads: 475

```
Yes, but by ordering not exactly the same parts (lower quality for fewer pennies) you might add one extra "O" to the BOM.:laughing:
```

---
## \#227 Posted by: bimmer Posted at: 2018-01-15T02:56:57.917Z Reads: 469

```
I meant order more than exactly them BOM because the little parts are never to be found once dropped and dont break the bank to order 50 instead of 4.
```

---
## \#228 Posted by: SpeedyGonzales Posted at: 2018-01-15T03:00:51.707Z Reads: 461

```
That makes sense.
```

---
## \#229 Posted by: SimosMCmuffin Posted at: 2018-01-15T06:45:09.403Z Reads: 453

```
@bimmer Are you doing hand soldering or hot air soldering?
```

---
## \#230 Posted by: bimmer Posted at: 2018-01-15T07:12:39.162Z Reads: 457

```
Hot air I think my stencil was too thick and added  to much solder paste...
```

---
## \#231 Posted by: ThierryGTLTS Posted at: 2018-01-15T08:25:32.369Z Reads: 460

```
Hi Stewii,

At those high erpm, are there still any noise differences bewteen BLDC and FOC?!

Thierry
```

---
## \#232 Posted by: JayReyez Posted at: 2018-01-19T20:17:53.478Z Reads: 453

```
Off topic here @stewii but can you please pm me, I would love to purchase some of your boards.
```

---
## \#233 Posted by: stewii Posted at: 2018-01-19T20:30:41.213Z Reads: 453

```
Yes there are,[ I recorded it](https://www.dropbox.com/s/qsh3tb6t0wxbdqj/New%20Recording%208.m4a?dl=0), first is BLDC then FOC.
```

---
## \#234 Posted by: SpeedyGonzales Posted at: 2018-01-20T02:20:11.244Z Reads: 459

```
Thank you for the recording. It sounds like a little lower frequency on FOC.
stewii are you making any progress? 
Looking forward to putting it to work.
```

---
## \#235 Posted by: Eboosted Posted at: 2018-01-21T03:44:00.667Z Reads: 473

```
[quote="Eboosted, post:215, topic:37579"]
I switched to BLDC mode, no more cutouts, evetything working perfect. Miss FOC a little bit just for launches.

Stewii sent me some procedures to pinpoint the issue but I still need to find time to open up the enclosure
[/quote]

Update:

With the help of @Stewii, I was able to fix  the DRV error.

Everytime I moved the USB plug from the slave ESC a DRV error was stored, at first I thought the cause was a bad DRV or USB plug solder joint.

https://www.youtube.com/watch?v=oIHRrCGi6AU

When I disassembled the ESC I found the temperature wire crooked against all electronics the screws were compresssing it even more against the motherboard.

Once I routed that wire correctly and bolt the ESC back again, BOOM! no more DRV error.

I'm running BLDC at the moment but tomorrow I'll go back to FOC.

Sorry to all you guys for throwing wrong information about the blow DRV chip.

ESCapes are working amazing so far.
```

---
## \#236 Posted by: bimmer Posted at: 2018-01-21T03:58:54.610Z Reads: 475

```
I'd like to anounce that she's alive.![15165071001792041630417|281x500](upload://n1KqOm8XSh8p1pVFQTsQTFYcJAx.jpg)
Update!
Thanks stewie for such a great product.
I whipped up a quick and dirty battery to bench them and they run great.![15165276106441122986251|281x500](upload://2AZ3hK44kD8JSyLj7pxVnltthJ2.jpg)![15165276721081676717930|690x388](upload://q4A3BS4eVa0PiF1OuEtaZBajKqC.jpg)
Ran a 245KV outrunner at fully charged 12S on FOC. full speed, stop, full speed, reverse, back and forth nothing cogging or weird noise and most of all no DRV error.
```

---
## \#237 Posted by: wmj259 Posted at: 2018-01-21T04:00:38.690Z Reads: 456

```
Did you solder it all yourself?
```

---
## \#238 Posted by: bimmer Posted at: 2018-01-21T04:24:31.826Z Reads: 464

```
![15165086316631502401422|690x388](upload://wG5u1YjwIiYRSLPkqPlYnAjkakv.jpg)
Yeah I bought all this stuff just to make it too.
```

---
## \#239 Posted by: ThierryGTLTS Posted at: 2018-01-21T10:35:03.332Z Reads: 462

```
Thanks.

Thierry
```

---
## \#240 Posted by: SpeedyGonzales Posted at: 2018-01-23T04:06:27.817Z Reads: 454

```
That is impressive. :clap:
```

---
## \#241 Posted by: scrapheap Posted at: 2018-01-24T18:41:21.596Z Reads: 442

```
Filled out and submitted the google form.

I hope I'm not too late to jump in on this.
```

---
## \#242 Posted by: Eboosted Posted at: 2018-01-25T05:39:31.957Z Reads: 444

```
Another update:

I'm back at FOC the ESCapes are working pretty good after temporarily fixing the flexing of the mother board, not a single fault, pretty reliable and fun to run it in FOC.

Highly recommended this ESCape
```

---
## \#243 Posted by: koralle Posted at: 2018-01-25T06:11:35.474Z Reads: 440

```
[quote="Eboosted, post:242, topic:37579"]
fixing the flexing of the mother board
[/quote]

can you please elaborate?
```

---
## \#244 Posted by: Eboosted Posted at: 2018-01-25T06:19:47.220Z Reads: 442

```
The first case design made the motherboard flex inside it, too much flex mixed with road vibrations caused the board to develop issues over time, the last version of the case is way better no more flexing of the electronic board and 100% more reliable.
```

---
## \#245 Posted by: LukePL Posted at: 2018-01-28T11:16:06.035Z Reads: 453

```
:D :D :smiley:![IMG_20180122_131411|666x500](upload://PMMo3tlP31rJGosM2RgV8X9eF9.jpg)![IMG_20180122_130544|666x500](upload://m7oNmvc0IEGlc01uWu22DwtyKoM.jpg)![IMG_20180128_120956|666x500](upload://rysZgmbN6SdRGtvIngsZGvjbUcH.jpg)
```

---
## \#246 Posted by: notepad Posted at: 2018-01-28T11:36:32.153Z Reads: 437

```
what guage wires are they.  they look a little thin for such a high performasce machine?

other than that. looks bloody sick
```

---
## \#247 Posted by: LukePL Posted at: 2018-01-28T11:41:46.657Z Reads: 437

```
It's 14AWG. I have Racestar BRH-5065 140KV so for now it's more than enough ;) Battery wires are 10AWG.
```

---
## \#248 Posted by: notepad Posted at: 2018-01-28T11:42:22.569Z Reads: 434

```
fair enough,  just my eyes playing tricks on me again :D
```

---
## \#249 Posted by: LukePL Posted at: 2018-01-28T11:47:57.489Z Reads: 434

```
Those cellphones cameras are quite wide angle so they play trick on everybody ;)
```

---
## \#250 Posted by: FredrikHems Posted at: 2018-01-28T12:10:18.068Z Reads: 428

```
Did you solder the whole thing yourself, or?
```

---
## \#251 Posted by: LukePL Posted at: 2018-01-28T13:04:35.510Z Reads: 418

```
No, got the whole thing from @stewii
```

---
## \#252 Posted by: scrapheap Posted at: 2018-01-28T13:08:16.389Z Reads: 414

```
If I may ask, how long was the wait time?

Thanks.
```

---
## \#253 Posted by: LukePL Posted at: 2018-01-28T13:13:21.230Z Reads: 406

```
Can't tell exactly because I'm not in rush but as I remember from time when I said ok I want it it was quite fast.
But you should contact @stewii because I have no idea on how many pcs he's working on currently.
```

---
## \#254 Posted by: scrapheap Posted at: 2018-01-28T13:24:20.193Z Reads: 410

```
I might have to...I filled out the form a few days ago and I still haven't had any contact from him as of yet, to know if it went through. Because I thought it was required to pay upfront...

I'll wait a few more days though, to give him some more time. Looks like he's a bit busy.
```

---
## \#255 Posted by: H_man Posted at: 2018-01-29T01:59:54.003Z Reads: 420

```
@stewii 
Im from Auckland, New Zealand I would like to know the cost of a single PCB and cost of shipping to Auckland, New Zealand

Thanks.
```

---
## \#256 Posted by: SpeedyGonzales Posted at: 2018-01-29T03:17:25.620Z Reads: 420

```
Your ESCape logo looks fantastic.
Correction: that ESCape logo looks fantastic :grinning:
```

---
## \#257 Posted by: Ps6ch0d0gg Posted at: 2018-01-29T09:50:56.837Z Reads: 428

```
Hi guys, I ordered 2 Escape from @stewi I would have them this week normally. the delay is about a month. For my part I write to him privately. as I have in my possession I would share the photos.
```

---
## \#258 Posted by: LukePL Posted at: 2018-01-29T10:14:22.699Z Reads: 427

```
Thank you but it belongs to @stewii ;)

@Ps6ch0d0gg that's the way it is sometimes. I'm kind of use to wait because I order stuff from Banggood and Aliexpress. ESCape is great hardware and comparing prices to Trampa it's definitely worth to wait
```

---
## \#259 Posted by: H_man Posted at: 2018-01-29T10:16:22.486Z Reads: 416

```
Is there a way to get in contact with him privately? an email address?
```

---
## \#260 Posted by: LukePL Posted at: 2018-01-29T10:31:59.627Z Reads: 416

```
Just send him a private message.
```

---
## \#261 Posted by: Ps6ch0d0gg Posted at: 2018-01-29T10:52:15.530Z Reads: 415

```
you just have to click on its name and choose private message option😉
```

---
## \#262 Posted by: Ps6ch0d0gg Posted at: 2018-01-29T10:53:35.701Z Reads: 427

```
for my part I am like a child waiting for his lollipop 😂😉
```

---
## \#263 Posted by: Nordle Posted at: 2018-01-29T11:20:57.538Z Reads: 410

```
Get some other candy meanwhile;)
```

---
## \#264 Posted by: banjaxxed Posted at: 2018-01-29T12:36:01.753Z Reads: 411

```
I'd say @stewii has too many PMs asking the same thing, me-when-how much-me-me-me :clown_face:
```

---
## \#265 Posted by: SpeedyGonzales Posted at: 2018-01-29T16:33:39.170Z Reads: 411

```
Good thing happen to those who wait.:sunglasses:
```

---
## \#266 Posted by: H_man Posted at: 2018-01-30T04:12:29.237Z Reads: 421

```
Thanks guys
```

---
## \#267 Posted by: b264 Posted at: 2018-01-30T04:26:22.337Z Reads: 489

```
[quote="SpeedyGonzales, post:265, topic:37579"]
Good thing happen to those who wait.:sunglasses:
[/quote]

Username does not check out
```

---
## \#268 Posted by: stewii Posted at: 2018-02-02T01:00:25.643Z Reads: 493

```
So, I finished the first few full ESCape with alu housing.
I have been receiving a lot of messages, so sorry for taking so long answering them.
Here is two of them: (I might change the cover PCB to black)

![IMG_4913|375x500](upload://3efDX0C5qUpENgY04RqJYsixqDb.JPG)

Also a dual full enclosed housing is under work:

![dualESCapehousing|689x349](upload://g3abgQExJnhjiD1IrEvbUmJCqXG.png)

I will do a pre-order through a website that is going to be up soon.

stay tuned
```

---
## \#269 Posted by: uigiroux Posted at: 2018-02-02T20:09:11.519Z Reads: 466

```
Is that for the housing only, or 2 VESC and the dual housing?  I already filled out the form for 2 of them, so would I need to fill out the new form to get on the wait list for them?
```

---
## \#270 Posted by: Florian_emtb Posted at: 2018-02-02T20:15:16.847Z Reads: 454

```
Hello,  how much is the max motor amps?
```

---
## \#271 Posted by: SeanHacker Posted at: 2018-02-03T03:29:56.758Z Reads: 455

```
Max motor amps depends on your motors dude. ;)
```

---
## \#272 Posted by: Ps6ch0d0gg Posted at: 2018-02-03T08:26:31.620Z Reads: 471

```
Hi same design that trampa so normally advertised up to 120 A ... but I saw jenso de etoxx make them run higher in no limit mode ...![Screenshot_20180203-092452|281x500](upload://y3N2sarYLKh9x55c7fcw3wucWOr.jpg)
```

---
## \#273 Posted by: Ps6ch0d0gg Posted at: 2018-02-03T08:28:39.602Z Reads: 457

```
after it seems that the leopard is not resisted but at the same time they are announced at 90 A max.
```

---
## \#274 Posted by: banjaxxed Posted at: 2018-02-03T10:41:03.081Z Reads: 459

```
They are real purdy, glad you're swamped I've yet to recover from the wallet bash @scepterr @Rithblu gave me this month, I will have those two we talked about 😃
```

---
## \#275 Posted by: Vanarian Posted at: 2018-02-03T17:08:21.149Z Reads: 451

```
That's nice, so the ESC has become stronger than Leopard motors ? It's good news ! No erpm limit worries, no DRV worries and able to pull high amps.
```

---
## \#276 Posted by: Hummie Posted at: 2018-02-03T18:00:01.298Z Reads: 456

```
[quote="SeanHacker, post:271, topic:37579"]
Max motor amps depends on your motors dude. :wink:
[/quote]
max motor amps is more limited by what the esc can do.  Even a small motor can do many amps for a short period of time

whats the max motor amps this esc will do?
```

---
## \#277 Posted by: Ps6ch0d0gg Posted at: 2018-02-03T18:41:46.704Z Reads: 463

```
it depends on the firmware you want to use if you use 6.4 firmware even that trampa limited to 120 A max if you use nohw version. limit you can climb higher but at your risk...

this is what stewie told me:![Screenshot_20180203-193657|281x500](upload://AtVGtqWSBUOcFsq8qVDcPwI9dk1.png)
```

---
## \#278 Posted by: Ps6ch0d0gg Posted at: 2018-02-03T18:46:41.696Z Reads: 440

```
yes and if I understood it currently used 2 × alien motor 8085 announced at 150A max and it works too.
```

---
## \#279 Posted by: Surfer Posted at: 2018-02-03T18:50:04.549Z Reads: 442

```
With such amount of processing power, we need soon 2170 or going back to lipos to get the vesc warm up!
```

---
## \#280 Posted by: Hummie Posted at: 2018-02-03T20:01:39.620Z Reads: 444

```
i'm confused by what you last said to vanarian: are you saying you run it at 150 motor amps or is the 150 the motor's claimed amp limit?
```

---
## \#281 Posted by: Ps6ch0d0gg Posted at: 2018-02-03T20:12:40.059Z Reads: 444

```
excuse me my english not very good. I said @nowind (= jenso = E-toxx) was driving with leopard and killed the engine then it is currently rolling with motor alien and it works ... now not sure that is last limit.
```

---
## \#282 Posted by: Ps6ch0d0gg Posted at: 2018-02-03T20:25:19.061Z Reads: 469

```
hello, here is a link to the post I'm talking about. and it's not me but nowind I'm talking to you about.
http://www.electric-skateboard.builders/t/e-toxx-directdrive-vs-trampa-vesc6-vs-leopard-8072-170kv-vs-nowind/30822/399
```

---
## \#284 Posted by: Exiledd_Top Posted at: 2018-02-04T04:53:40.639Z Reads: 466

```
Suggest u read the entire thread and not just ask something as in am lazy, trampa sells "vesc6" this thread is about wanting to make there similar or better  vesc's as trampa just not calling it vesc6 since it's trademark read first please ...@matwoSvK
```

---
## \#286 Posted by: Ps6ch0d0gg Posted at: 2018-02-05T17:16:26.347Z Reads: 478

```
Hi everyone, I just received my 2 ESCape they are just wonderful ... they are a little bigger than my roxxy esc I should change the support but too happy. thanks again to @stewii 😉![20180205_180626|374x500](upload://5MaD4ZVsyyxQMgBAiBka0QQnASy.jpg)![20180205_180635|374x500](upload://fyBDLYapdVSZEE2gCfivGmJ5r5H.jpg)![20180205_180653|374x500](upload://j2CPcNj6mZoDEcaE4mgelUlxlN1.jpg)
```

---
## \#287 Posted by: Nowind Posted at: 2018-02-05T21:31:19.803Z Reads: 454

```
Whats not good with the Roxxy ?
:joy:
ah i remember its the fkn break ...
:kissing_heart::joy:
```

---
## \#288 Posted by: benjammin Posted at: 2018-02-05T21:49:32.295Z Reads: 454

```
And the fire 🔥
```

---
## \#289 Posted by: stewii Posted at: 2018-02-07T17:54:28.658Z Reads: 467

```
Been doing the ESCapes slowly, but steady :slight_smile:
Apologies if I forget or take too long answering people.

Got a new batch of PCBs and from now on the PCBs have 2oz copper thick and ENIG. 

![IMG_4935|375x500](upload://yoJ4zvgGej2fNytybGi2Y4duVO4.JPG)
```

---
## \#290 Posted by: banjaxxed Posted at: 2018-02-08T08:18:31.525Z Reads: 453

```
Hey @stewii these pcb look great, is the price the same? What effect if any on continuous amps? 

[quote="stewii, post:289, topic:37579"]
2oz copper thick and ENIG
[/quote]
```

---
## \#291 Posted by: gogomrrobot Posted at: 2018-02-08T10:21:11.838Z Reads: 475

```
Just got my latest ESCapes —- now if those Carvon would just ship i could post two new builds :slight_smile:

 ![image|375x500](upload://2FnHu7ZfwJyQdqQgCbFEXCXJMnn.jpeg)

I like the smooth corner of the aluminum casing.. definitely a distinct look...

![image|375x500](upload://4ezYJoujFtVOTTj0NSUZdj5a60t.jpeg)
```

---
## \#292 Posted by: anorak234 Posted at: 2018-02-14T06:05:59.707Z Reads: 446

```
Just ordered mine. First VESC after all this time... now I'm truly an esk8 junkie. Time to go out and spend more money on bluetooth modules etc XD
```

---
## \#293 Posted by: wmj259 Posted at: 2018-02-14T06:56:22.204Z Reads: 444

```
A lot of the parts in the BOM have a minimum order. Especially the drv8301.
```

---
## \#294 Posted by: Eboosted Posted at: 2018-02-14T07:26:27.142Z Reads: 446

```
[quote="gogomrrobot, post:291, topic:37579"]
Just got my latest ESCapes
[/quote]

Can't wait to get mine, they are in ATL ATM
```

---
## \#295 Posted by: ArnhemAnt Posted at: 2018-02-14T08:34:45.112Z Reads: 441

```
Just found this thread. Wish I came across it earlier, rather than throwing my cash at the Focbox and waiting, waiting, waiting for shipping. 

I'll be keeping a very close eye on this thread from now on as I am super keen to see the dual ESCape with enclosure.
```

---
## \#296 Posted by: Manu39 Posted at: 2018-02-14T10:24:35.894Z Reads: 441

```
Bravo Stewii for designing the VESCape, the great job.
Is it possible to just get 2 Alu box?
If yes can you me by email to communicate me the price with delivery in France ....
Thank you Manu
Good ride
```

---
## \#297 Posted by: Riako Posted at: 2018-02-14T11:00:06.433Z Reads: 458

```
Hi e-riders :slight_smile:

1st - Thanks a lot @stewii !! Awesome work, they looks sooo great !
https://monlongboardelectrique.files.wordpress.com/2018/02/rps20180211_145302.jpg

But also, I came with **a question : did someone work on something like @Kug3lis Fox one case ?**
https://cdn.shopify.com/s/files/1/2408/6975/products/IMG_0488_grande.jpg?v=1516825140

Should be perfect to set on the build ... :yum:
(if not I may be in the same ask as @Manu39 )
```

---
## \#298 Posted by: LukePL Posted at: 2018-02-14T11:04:22.303Z Reads: 428

```
Yeah @stewii show that.  http://www.electric-skateboard.builders/t/hw6-4-based-esc-escape/37579/268
```

---
## \#299 Posted by: Riako Posted at: 2018-02-14T11:09:06.671Z Reads: 433

```
Thanks Luke !  :blush: haha I forgot that I already liked the pic ...

So Stewii, you could already count me in ;) :+1:
```

---
## \#300 Posted by: stewii Posted at: 2018-02-14T12:10:42.740Z Reads: 426

```
Yes I’ve an untested dual housing design but not sure if I can get enough people interested ( around 20).
```

---
## \#301 Posted by: banjaxxed Posted at: 2018-02-14T12:13:45.395Z Reads: 424

```
I'm in @stewii...with ESCapes too
```

---
## \#302 Posted by: stewii Posted at: 2018-02-14T12:15:33.689Z Reads: 427

```
Yes I can put you down for the 2nd batch
```

---
## \#303 Posted by: longhairedboy Posted at: 2018-02-14T12:32:27.087Z Reads: 428

```
sweet deck :slight_smile:
```

---
## \#304 Posted by: Riako Posted at: 2018-02-14T12:51:18.154Z Reads: 436

```
ok, thanks stewii, perfectly understandable. So I will wait (I got time, its for my esk8 build for the spring season)
Maybe I can try your housing (I try with a thingiverse link around here, not give much attention but it doesn't fit the version I got ^^..) in 3d print then to do cnc it ? If you could share your model I could try  to do some here for frensh guys ... :blush:
```

---
## \#305 Posted by: Manu39 Posted at: 2018-02-14T13:44:21.702Z Reads: 414

```
is it possible to contact you by mail or PM please thanks
```

---
## \#306 Posted by: Cobber Posted at: 2018-02-14T20:55:52.814Z Reads: 406

```
What are the dimensions of the single and duel housings (I'm down for 4 escapes and enclosures using the form since early last month).
```

---
## \#307 Posted by: scepterr Posted at: 2018-02-14T21:00:29.300Z Reads: 419

```
Do I have 2 coming?
I filled out something some time ago... 😋
```

---
## \#308 Posted by: ArnhemAnt Posted at: 2018-02-14T21:39:31.661Z Reads: 431

```
I'd certainly take a dual ESCape in the housing.
```

---
## \#309 Posted by: Surfer Posted at: 2018-02-14T21:43:27.237Z Reads: 437

```
Someone has been nice!!
![IMG_20180214_224055|666x500](upload://rnzTM17MFOZeTe7v8nvctp50u7G.jpg)
 Happy San Valentín!!
They look so premium 😎!
Thanks a lot @Stewii
```

---
## \#310 Posted by: Sippahodge Posted at: 2018-02-15T01:57:04.115Z Reads: 414

```
Where can i purchase?
```

---
## \#311 Posted by: MontPierre Posted at: 2018-02-15T07:02:45.291Z Reads: 397

```
@stewii Just filled out the form. My papypal email is different so one again I completed form ticking “existing customer” and made a note to contact me for different email address for PayPal.
```

---
## \#312 Posted by: MontPierre Posted at: 2018-02-15T07:05:37.427Z Reads: 402

```
@Surfer any chance for dimensions? I would like to see if it will fit my enclosure
```

---
## \#313 Posted by: Surfer Posted at: 2018-02-15T12:16:52.553Z Reads: 412

```
Hey that's the measures:
70x77x20mm
Weight:
225gr
I bit heavy compared with 4.12 without housing, almost half kilo extra on the board.
Maybe the b-box is lighter,I have to check it out.
```

---
## \#314 Posted by: stewii Posted at: 2018-02-15T15:57:19.687Z Reads: 421

```
[quote="Cobber, post:306, topic:37579, full:true"]
What are the dimensions of the single and duel housings (I'm down for 4 escapes and enclosures using the form since early last month).
[/quote]

Dual is 137 x 72.2 x 24 (mm) 

[quote="Riako, post:304, topic:37579, full:true"]
ok, thanks stewii, perfectly understandable. So I will wait (I got time, its for my esk8 build for the spring season)
Maybe I can try your housing (I try with a thingiverse link around here, not give much attention but it doesn't fit the version I got ^^..) in 3d print then to do cnc it ? If you could share your model I could try  to do some here for frensh guys ... :blush:
[/quote]

That thingiverse version is a very early design, the current version  is 2mm longer and corners rounder.


I am working down on my list, I will message you guys.
```

---
## \#315 Posted by: MontPierre Posted at: 2018-02-16T10:29:33.558Z Reads: 414

```
Wicked! So slightly larger than the FOCbox - awesome! It should fit in my enclosure.
```

---
## \#316 Posted by: Surfer Posted at: 2018-02-16T12:05:12.372Z Reads: 420

```
Seems like the race of V6 just started
Focbox V6
https://imgur.com/a/h5KNK
```

---
## \#317 Posted by: stewii Posted at: 2018-02-16T12:29:23.961Z Reads: 413

```
That is just the same old focbox with a number 6 lol
```

---
## \#318 Posted by: Surfer Posted at: 2018-02-16T12:32:48.789Z Reads: 399

```
Probably you right, just I saw the comment on top of the picture from enertionboards " vescsix? Yep"
```

---
## \#319 Posted by: stewii Posted at: 2018-02-16T12:34:48.751Z Reads: 395

```
When they release the focbox6 I will have the ESCape 22S :smiley:
```

---
## \#320 Posted by: Surfer Posted at: 2018-02-16T12:36:23.415Z Reads: 396

```
You talking about shipping?
🤣🤣🤣!!
```

---
## \#321 Posted by: LukePL Posted at: 2018-02-16T12:40:06.477Z Reads: 403

```
I belive about voltage :D
```

---
## \#322 Posted by: stewii Posted at: 2018-02-16T13:37:06.832Z Reads: 410

```
I just created an account on thingiverse and will share the 3D file here, it takes 24h.
```

---
## \#323 Posted by: Cobber Posted at: 2018-02-16T14:02:36.258Z Reads: 407

```
All good bro, as long as I have not fallen through the gaps doing a new jenso-emtb and a cantelated tesseract with ollin ronin mounts after I get through my current builds.

I have plenty of time if i'm in the que :D
```

---
## \#324 Posted by: moon Posted at: 2018-02-16T14:22:21.678Z Reads: 407

```
Are PCB files available?

Or to buy?
```

---
## \#325 Posted by: stewii Posted at: 2018-02-16T14:32:19.225Z Reads: 386

```
Just to buy. Send me a message.
```

---
## \#326 Posted by: KeivanM Posted at: 2018-02-16T15:12:36.606Z Reads: 384

```
I just signed up on the google sheet and sent a question, GREAT work you’re doing here!
```

---
## \#327 Posted by: KeivanM Posted at: 2018-02-16T15:13:11.579Z Reads: 389

```
I’ll buy 2 from you if they’re cheaper than the “b-box” ones in total
```

---
## \#328 Posted by: Riako Posted at: 2018-02-16T15:29:13.406Z Reads: 387

```
Wow ! so effective Stewii :facepunch::star_struck: Thanks a lot again and again for all your work and services !!
```

---
## \#329 Posted by: stewii Posted at: 2018-02-16T15:57:39.599Z Reads: 398

```
Thanks. I appreciate it.
b-boxes might be cheaper, not sure if bimmer has a final price.
If I could afford buying components for 100 units I could make them cheaper but I cant.

[quote="KeivanM, post:327, topic:37579, full:true"]
I’ll buy 2 from you if they’re cheaper than the “b-box” ones in total
[/quote]
```

---
## \#330 Posted by: Cobber Posted at: 2018-02-16T15:59:19.510Z Reads: 394

```
i'd pay stewii more, b-box is kind of stewii clone with some changes. stewii has a all aluminium case, double case offered... b-box stewii case/pom/alloy.

b-box is stewii re-design re-designed...

how hard do you want to go?
```

---
## \#331 Posted by: KeivanM Posted at: 2018-02-16T17:43:18.951Z Reads: 383

```
Okay awesome, thanks man :slight_smile:
```

---
## \#332 Posted by: bimmer Posted at: 2018-02-17T01:09:27.298Z Reads: 379

```
Yeah I am charging 160$ because I only made 50 aswell.
```

---
## \#333 Posted by: Deckoz Posted at: 2018-02-17T01:12:46.407Z Reads: 382

```
Hey @stewii I purchased 4 pcbs from you and built them up and milled out the cases...  Do your top plate pcbs actually have anything on them? As I'm thinking of just laser cutting some ABS or bare silicate board for case covers...since I didn't order cover pcbs(you hadn't completed them yet)

Thanks
```

---
## \#334 Posted by: banjaxxed Posted at: 2018-02-17T01:16:13.915Z Reads: 377

```
OMG Are they real VESC9?
```

---
## \#335 Posted by: stewii Posted at: 2018-02-17T01:17:02.815Z Reads: 388

```
Cover pcb has a printed 2.4Ghz antenna for the nRF IC and the layout of all the connections, that's it.
```

---
## \#336 Posted by: Deckoz Posted at: 2018-02-17T01:19:31.153Z Reads: 392

```
Ah ok thanks man. I'm didn't populate the nrf and not worried about silk screen. 

Thanks dude.
```

---
## \#337 Posted by: stewii Posted at: 2018-02-17T01:23:47.639Z Reads: 404

```
No problem, stl file will be here tomorrow if you want to use it.
```

---
## \#338 Posted by: stewii Posted at: 2018-02-17T01:35:38.551Z Reads: 414

```
Another 3 almost finished. Housings will take a couple of weeks tho. So if anyone is after one without housing let me know.
![IMG_4953|375x500](upload://5HZ0xQnlJI7All4QGdYpuWFlD1K.JPG)
```

---
## \#339 Posted by: moon Posted at: 2018-02-17T01:38:15.446Z Reads: 386

```
Whats your soldering setup like? any pics?
```

---
## \#340 Posted by: stewii Posted at: 2018-02-17T01:50:52.998Z Reads: 388

```
No pics, it is a reflow oven mostly and a 100W soldering iron for the cables. I only use the hot air station if I need to desolder something and that doesnt happen often.
```

---
## \#341 Posted by: Riako Posted at: 2018-02-17T13:44:39.789Z Reads: 388

```
ok, super !! Thanks Stewii, hope you take some time or find some to enjoy your WE still.
I'm not pressed for time (sorry don't know if this expression exist in english ...) but again, thanks for your work ! I will test it at once tomorow for sure ;)
```

---
## \#342 Posted by: Surfer Posted at: 2018-02-17T14:36:18.113Z Reads: 391

```
I should say that the soldering work is so beautiful props @stewii
```

---
## \#343 Posted by: GrecoMan Posted at: 2018-02-17T14:49:42.156Z Reads: 389

```
he gets some practice 😉
```

---
## \#344 Posted by: stewii Posted at: 2018-02-17T16:54:45.632Z Reads: 390

```
https://www.thingiverse.com/thing:2796140
```

---
## \#345 Posted by: Riako Posted at: 2018-02-17T17:04:03.448Z Reads: 393

```
Stewii ...
https://media1.tenor.com/images/df296dce4faf15ddf048e1dc0e79a032/tenor.gif?itemid=5170581
dl > on print !
```

---
## \#346 Posted by: Maineo Posted at: 2018-02-17T17:04:34.238Z Reads: 391

```
Hey stewii, I wanted to message you about the ESCape but I cant figure out how to message you on this forum :(
```

---
## \#347 Posted by: Riako Posted at: 2018-02-17T17:05:21.628Z Reads: 402

```
clic his name and > messages
https://monlongboardelectrique.files.wordpress.com/2018/02/sans-titre-1.jpg
```

---
## \#348 Posted by: Maineo Posted at: 2018-02-17T17:07:22.249Z Reads: 383

```
Thats what I expect to see, but I dont see any message tab or option. Is it some like new member limitation?
```

---
## \#349 Posted by: Cobber Posted at: 2018-02-17T17:10:39.970Z Reads: 383

```
get your read time up bro. contribute, like some posts...
```

---
## \#350 Posted by: Maineo Posted at: 2018-02-17T17:13:55.469Z Reads: 382

```
lol, it looks like that one like fixed it o.0  Thanks for the help
```

---
## \#351 Posted by: scepterr Posted at: 2018-02-17T19:11:54.798Z Reads: 383

```
Hey, I'm down to take 2 without housing, I believe I put down for 2 with, 2 without
```

---
## \#352 Posted by: Riako Posted at: 2018-02-17T20:35:29.128Z Reads: 391

```
https://monlongboardelectrique.files.wordpress.com/2018/02/rps20180217_213125.jpg
Perfect Stewii !
Any advice to make the two in one ? You let the space between them open or separated ?
```

---
## \#353 Posted by: Jobbel Posted at: 2018-02-18T20:05:54.982Z Reads: 391

```
![IMG_3173|375x500](upload://vmj43tpSBwTkYyz9kjVDG57wlhq.JPG)
Your ESCape is doing nicely
```

---
## \#354 Posted by: FredrikHems Posted at: 2018-02-18T20:37:26.288Z Reads: 381

```
Someone need to set up a competition in performance between the ESCape and the VESC6!
```

---
## \#355 Posted by: scepterr Posted at: 2018-02-18T20:50:07.736Z Reads: 381

```
There shouldn't be a measureable performance diff...it is identical
```

---
## \#356 Posted by: ArnhemAnt Posted at: 2018-02-18T21:40:54.333Z Reads: 396

```
Just scrolled back up and found the link to the form. All completed. Thanks @stewii for providing this service to the community here.
```

---
## \#357 Posted by: stewii Posted at: 2018-02-18T23:41:47.007Z Reads: 403

```
I am asked quite often if a housing is necessary, so I've done a quick comparison with alu housing and nothing over the FETs:


![thermal_comparison|690x405](upload://5mFlzasA2WF2gjbkYGPQUa6mqON.png)

notes:

-I had to stop the 60 amps test a bit earlier because my motor which is rated 50A max was starting to smell funny.
-the housing was about 20-30 degrees C lower than the FETs
-Once the FET temp cutoff kicked in which made the amperage go lower I stopped the test, it only happened in the tests without housing.
```

---
## \#358 Posted by: ATLesk8 Posted at: 2018-02-18T23:51:24.933Z Reads: 384

```
Are these available still? If so how do I order? Sorry if this has already been stated a billion times...
```

---
## \#359 Posted by: Manu39 Posted at: 2018-02-18T23:53:40.243Z Reads: 393

```
the differences in temperature rise are quite obvious on the test ... or the utility of a heat sink ...
Thanks for thé test
```

---
## \#360 Posted by: stewii Posted at: 2018-02-18T23:57:33.711Z Reads: 400

```
Yes, they are, I keep making them, sometimes can take up to 2 weeks, depending how busy I am and if I need to wait for parts to arrive. Just message me if you want to order.
```

---
## \#361 Posted by: scepterr Posted at: 2018-02-19T00:03:14.583Z Reads: 397

```
If the ones without housing are still available I'll take 2
Planning to put them on a dual mount plate
```

---
## \#362 Posted by: scrapheap Posted at: 2018-02-21T04:14:36.671Z Reads: 386

```
Got mine today, and holy cow this thing is awesome!

Thanks again @stewii!
```

---
## \#363 Posted by: banjaxxed Posted at: 2018-02-21T11:23:47.267Z Reads: 388

```
Lifespan of the FETs should be longer if ran cooler
```

---
## \#364 Posted by: sunbeachfun Posted at: 2018-02-21T15:24:24.881Z Reads: 389

```
I would like 1 with the aluminum case. Please inform me how to contact you.  not sure if this is pm or not.
```

---
## \#365 Posted by: banjaxxed Posted at: 2018-02-23T10:45:30.474Z Reads: 399

```
Thanks for sharing, what is the difference between the housing stewii made and your rendition?

Left-Right we have
Orig Stewii design | Gogomrrobot rendidtion | v.2 stewii design. I like the rounded corners on the orig. stewii design for cable routing but not sure what the extra indentations are in the revision that stewii made, any clarifications folks?

![image|690x423](upload://nim7eEXwJ5ztFcRO6Ow0zm8VR3y.jpg)

In case (sic) it was missed stewii left his v2 design on thingiverse as well
https://www.thingiverse.com/thing:2796140
```

---
## \#366 Posted by: banjaxxed Posted at: 2018-02-23T11:41:12.631Z Reads: 393

```
Ok, trying to answer my own question ;)

The 'dint' in the stewii v1.02 design is for L2 inductor_smd_8x8mm.
![image|391x322](upload://r2SeNTS3T8OsGr77HXldEac5uJg.jpg)

It appears stewii redesigned to leave more alloy inside the casing providing additional cooling to the componentry..nice one since lost metal is lost thermal wicking and it never costs more $$$ to leave metal in place.

Will have to see about changing the design to get back the rounded wire holes which allow for rubber grommets and some water protection. I'm not aware of square gommets but maybe they exist
```

---
## \#367 Posted by: LukePL Posted at: 2018-02-23T11:56:14.281Z Reads: 381

```
Are you going to use pcb as top cover? If so there's no point to use grommets. To use the the whole thing should be redesigned. All the top connectors should be inside the case and go out through side wall with grommet. 
Are you going to 3D print that?
```

---
## \#368 Posted by: gogomrrobot Posted at: 2018-02-23T13:50:07.179Z Reads: 380

```
Don’t use that anymore that was actually @stewii he sent me the STL and i shared it here but based on his final pcb its 2mm short. That case did work with the original escapes he sent me. Also now he is selling Vesc fully with aluminum rounded case.

TLDR; Going forward PM @stewii for the STL file for the housing or a link from him he shared on the forum.
```

---
## \#369 Posted by: Riako Posted at: 2018-02-23T14:12:31.586Z Reads: 368

```
Yes, the last one I try, sharing here by stewii is perfect !
```

---
## \#370 Posted by: banjaxxed Posted at: 2018-02-23T15:05:21.736Z Reads: 379

```
No there is a separate cover for the open side of the case which comes with the pcb. 

On top of the pcb cover a rubber gasket or 3D printed flexible grommet for keeping any water coming into the case with enough height to space any connectors from being pushed against the deck.

...loosely thought about probably flaws, enlighten us

**edit:** done
https://www.thingiverse.com/thing:2804101

@Riako thanks, I think are confirming that @stewii's thingiverse published housing is the corret size? that's what I made this change against
```

---
## \#371 Posted by: LukePL Posted at: 2018-02-23T15:32:51.654Z Reads: 365

```
That would be good idea If you have that designed already.
```

---
## \#372 Posted by: banjaxxed Posted at: 2018-02-23T15:54:47.872Z Reads: 365

```
Yes I guess the holes should be closed out some more to allow for fully sealed cables and enclosure height increased to give deck clearance...up to my tits atm
```

---
## \#373 Posted by: Pimousse Posted at: 2018-02-23T18:41:45.568Z Reads: 372

```
Hey @stewii, do you have a SLPDRT file of your case ?
The STEP file makes Solidworks crash evrytime, don't know why. :neutral_face:
```

---
## \#374 Posted by: LukePL Posted at: 2018-02-23T20:16:36.020Z Reads: 393

```
Ok so I have a offer for you guys. I can make a enclosure for ESCape for you. 
Price is 25euro plus shiping cost. Good thing is that I don't need minimum amount so everyone that is interested let me know (PM).![IMG_20180223_211650|666x500](upload://hhcfYJPZupenAokKTq6fqfxo4P6.jpg)
Guys... @scepterr @JohnA @akhlut @Surfer @karatektus @gogomrrobot @Boardnamics @banjaxxed  stil want some? ;)
```

---
## \#375 Posted by: Riako Posted at: 2018-02-23T20:35:10.109Z Reads: 374

```
ho ok, I print the stewii folder to hold gently the two ESCape waiting a dual cnc case offer or stewii folder :blush:
But it fit correctly, I didn't notice anything wrong.
I see your folder change a bit to the motor phase wires. but you also make changement in depth ?
```

---
## \#376 Posted by: scepterr Posted at: 2018-02-23T20:41:45.790Z Reads: 367

```
Good to know, I'll be using a dual plate for the ones I'm getting atm, for the next ones maybe
```

---
## \#377 Posted by: bigben Posted at: 2018-02-23T20:51:54.647Z Reads: 368

```
And a dual version??
```

---
## \#378 Posted by: banjaxxed Posted at: 2018-02-23T20:56:47.136Z Reads: 361

```
I only rounded the wire cutouts
```

---
## \#379 Posted by: Surfer Posted at: 2018-02-23T20:57:13.722Z Reads: 365

```
Oh that's awesome! Actually I have the ESCape housing, and is really good, just I think a lighter version could be interesting, almost half kilo for two, in a normal e-longboard is a lot!
```

---
## \#380 Posted by: LukePL Posted at: 2018-02-23T22:48:14.007Z Reads: 368

```
Should have some info next week.
```

---
## \#381 Posted by: LukePL Posted at: 2018-02-23T22:48:53.238Z Reads: 370

```
Dual will be lighter.
```

---
## \#382 Posted by: scepterr Posted at: 2018-02-23T22:50:45.600Z Reads: 367

```
Honestly if it's going in a sealed enclosure, you don't need more than a cooling plate
```

---
## \#383 Posted by: pixelsilva Posted at: 2018-02-23T23:19:17.541Z Reads: 374

```
This is awesome!
```

---
## \#384 Posted by: anorak234 Posted at: 2018-02-23T23:29:18.264Z Reads: 392

```
The normal ESCape comes with housing right? Mine is due to arrive this afternoon, I guess ill find out...
```

---
## \#385 Posted by: scrapheap Posted at: 2018-02-24T04:07:40.147Z Reads: 374

```
How much did you pay?

With housing, it's 150 GBP + shipping + paypal fees (if using goods and services)
Without housing, it's 130 GBP + shipping + fees
```

---
## \#386 Posted by: anorak234 Posted at: 2018-02-24T07:18:00.200Z Reads: 369

```
I paid the full 150, so I’m glad that means I’ll get the case. My package didn’t arrive though... and USPS is still saying “technical difficulties” on the tracking page. I want this thing to arrive already!
```

---
## \#387 Posted by: scrapheap Posted at: 2018-02-24T12:42:33.854Z Reads: 383

```
USPS was weird with mine as well. It's suppose to be signed for, I checked tracking and it kept saying "OUT FOR DELIVERY". Came home from work at 8PM expecting the little paper saying I missed a delivery but I don't see it and I check the mailbox instead. THERE IT WAS and the online tracking said it was still out for delivery. It still says it doesn't know if it was delivered and posted an alert saying it's not updated lol.

Check your mailbox if you haven't already.
```

---
## \#388 Posted by: Minim Posted at: 2018-02-24T22:08:13.296Z Reads: 384

```
Is this cut on a DIY router Luke?
```

---
## \#389 Posted by: anorak234 Posted at: 2018-02-25T16:15:19.633Z Reads: 404

```
Ok so my ESCape arrived last night, and I opened it this morning. First impressions are that it looks fantastic, with some scratches and messy wire due to what I assume is the result of a few thousand miles of shipping. ![image|666x500](upload://ccHZ8XgYX2Cx5NzkeZMD8nh8Fnh.jpeg)![image|375x500](upload://5DtUlnQPYtLAKwI1g0Ygm9tuqdq.jpeg)![image|666x500](upload://3TIRnybkr0ZMS9J98RpYI6mHR1Y.jpeg)![image|375x500](upload://kImW6FdL5fofSJ2gkJm6GMQNFou.jpeg)
As far as I’m concerned I can fix and solder the wires pretty easily, and the scratches aren’t a big deal because it’ll all be enclosed anyways. The only thing I’m worried about is how short the positive and negative wires are, as I’m not the fastest at soldering and it’ll get hot quickly. 

Anyways, this is my first VESC, so today is research day before I even think about starting this thing up. 
#1 mission: no drv chips blown.
```

---
## \#390 Posted by: Pimousse Posted at: 2018-02-25T16:21:56.454Z Reads: 370

```
Be sure to use a high power soldering iron (80W minimum) and follow every stp in VESC Tool to avoid bad things.
```

---
## \#391 Posted by: sMATTEr Posted at: 2018-02-25T16:26:58.631Z Reads: 369

```
80w? Is that really necessary?  It’s not likes he’s soldering directly on the VESC.

I would say there is zero risk of melting the solder on the vesc. Just don’t solder drunk and pretin the wires.

Edit: maybe zero risk is a overstatement :roll_eyes: :grin:
```

---
## \#392 Posted by: Silverline Posted at: 2018-02-25T17:34:01.373Z Reads: 372

```
No... My old 50 watt Weller station , can do this all day Long. The most important thing, is to use the right solder tip for the job.
```

---
## \#393 Posted by: stewii Posted at: 2018-02-25T18:34:03.420Z Reads: 378

```
[quote="anorak234, post:389, topic:37579"]
The only thing I’m worried about is how short the positive and negative wires are, as I’m not the fastest at soldering a
[/quote]

Sorry about the scratches :S 
The wires are like that messy probably because I connected them to my power supply and motor to do tests.

No worries about the battery wires getting too hot during soldering, my soldering iron is 100W and never gets too hot on the other ending of the wire to the point to melt the solder.
```

---
## \#394 Posted by: anorak234 Posted at: 2018-02-25T18:37:09.317Z Reads: 385

```
Got it all soldered up! You were correct, I don’t use 10awg very often and it kept very cool while adding the connector. I can already tell this thing with the heat sink will run wayyyy cooler than my Torqueboards esc.
![image|666x500](upload://4LHPOG03T5EA0tgx6CEdwfNIRJy.jpeg)
btw the black on the end of the XT90 is sharpie, not burns
```

---
## \#395 Posted by: ElskerShadow Posted at: 2018-02-25T18:58:57.092Z Reads: 377

```
This looks so great ! Maybe it’s time to dump foboxes and jump on these
```

---
## \#396 Posted by: ATLesk8 Posted at: 2018-02-26T02:25:00.910Z Reads: 375

```
Yeah how do we order these? Are they currently available? Take my 💰 💰 💰
```

---
## \#397 Posted by: Silverline Posted at: 2018-02-26T10:59:53.961Z Reads: 376

```
I want to buy 2pcs as well, with housing ??
```

---
## \#398 Posted by: stewii Posted at: 2018-02-26T15:39:14.445Z Reads: 386

```
Just message me. The few I make I sell immediately, so I don't have any in stock but I keep making them.

[quote="ATLesk8, post:396, topic:37579, full:true"]
Yeah how do we order these? Are they currently available? Take my 💰 💰 💰
[/quote]

[quote="Silverline, post:397, topic:37579, full:true"]
I want to buy 2pcs as well, with housing ??
[/quote]


Sorry, I dont think I have that file format on fusion360

[quote="Pimousse, post:373, topic:37579, full:true"]
Hey @stewii, do you have a SLPDRT file of your case ?
The STEP file makes Solidworks crash evrytime, don't know why. :neutral_face:
[/quote]
```

---
## \#399 Posted by: anorak234 Posted at: 2018-02-26T17:25:07.893Z Reads: 373

```
@stewii maybe it'd be beneficial for you to make a website? Sales don't look like they're slowing down any time soon, and you're going to get a hell of a lot of purchases if people look at a picture on a website of an ESCape marked for half the price of Trampa's VESC. I've also heard rumors of another ESC that you're working on, so it would help to have both organized for purchase in one online location.
```

---
## \#400 Posted by: pixelsilva Posted at: 2018-02-27T08:44:44.449Z Reads: 367

```
....the focbox killer is here. The focbox is dead, long live the ESCape.
```

---
## \#401 Posted by: ElskerShadow Posted at: 2018-02-27T08:47:06.746Z Reads: 376

```
This name disturb me B-Box is the name of my internet router lol :stuck_out_tongue:
```

---
## \#402 Posted by: pixelsilva Posted at: 2018-02-27T08:49:16.412Z Reads: 381

```
There...:point_up:
```

---
## \#403 Posted by: b264 Posted at: 2018-02-27T08:54:32.759Z Reads: 382

```
This is the ESCape, the [B-box has its own thread](https://www.electric-skateboard.builders/t/hw6-4-based-esc-b-box/44375) over yonder

Though they are closely related and both FOCBOX KILLERS :smirk:
```

---
## \#404 Posted by: ArnhemAnt Posted at: 2018-02-27T09:00:22.932Z Reads: 391

```
[quote="ElskerShadow, post:395, topic:37579, full:true"]
This looks so great ! Maybe it’s time to dump foboxes and jump on these
[/quote]

Exactly what I have done. I contacted Enertion and asked for them to refund the money I paid earlier this year for a product that they can't deliver.
```

---
## \#405 Posted by: ElskerShadow Posted at: 2018-02-27T09:10:48.866Z Reads: 374

```
I tought the B-box used the ESC-cape pcb ?
```

---
## \#406 Posted by: b264 Posted at: 2018-02-27T09:19:49.327Z Reads: 379

```
It does!  But it has its own thread, may or may not have the same BOM, and it's a different manufacturer in a different part of the world ;-)
```

---
## \#407 Posted by: ElskerShadow Posted at: 2018-02-27T09:23:52.465Z Reads: 379

```
Yup it makes sense anyway I’m in europe so i will stick to Esc-cape
```

---
## \#408 Posted by: stewii Posted at: 2018-02-27T17:22:28.671Z Reads: 383

```
Just wondering what is the favourite colour for the cover PCB solder mask for the ESCape, white, black or other?

[poll type=regular max=20 public=true]
* White
* Black
* Green
* Yellow
* Red
* Blue
[/poll]
```

---
## \#409 Posted by: Manu39 Posted at: 2018-02-27T17:59:06.051Z Reads: 365

```
Dual color...RED for the master ESCAPE and black for the slave ESCAPE...;-)
in the color of the FORAKER red and black ...;-)
```

---
## \#410 Posted by: Nordle Posted at: 2018-02-27T18:05:31.265Z Reads: 358

```
Black and white are best

what is the price for these? have to kill some older vesc's before i buy new ones but curious and a bit to lazy to read trough over 400 posts^^
```

---
## \#411 Posted by: Manu39 Posted at: 2018-02-27T18:11:14.686Z Reads: 355

```
In the last news:
150 GPB unit with aluminum case and cover ... Without shipping charges
```

---
## \#412 Posted by: Nordle Posted at: 2018-02-27T18:16:49.995Z Reads: 351

```
That seems fair:) you know without case?

in that case i hope to burn my 4.12's soon :man_farmer::fire:
```

---
## \#413 Posted by: Manu39 Posted at: 2018-02-27T18:22:12.119Z Reads: 355

```
From memory it seems to me that I read that the box alone is 20 GPB ... but  I'm not sure. Request @stewii
```

---
## \#414 Posted by: stewii Posted at: 2018-02-27T19:15:48.239Z Reads: 360

```
Manu39 is correct.

Black is indeed the favourite 2/3 of the votes, none for yellow? :D 
Ordering black cover PCBs then.
```

---
## \#415 Posted by: b264 Posted at: 2018-02-27T19:20:04.432Z Reads: 352

```
Black won because you didn't put "blinking indigo" as an option ;-)
```

---
## \#416 Posted by: H_man Posted at: 2018-02-28T08:28:44.226Z Reads: 353

```
Hi guys, I understand that this has been discussed before as the MOSFET IRF7749L1TRPBF is sold out until August-September. The alternative AUIRF7749L2TR was suggested. My question is are there any other alternatives for this MOSFET?
```

---
## \#417 Posted by: stewii Posted at: 2018-02-28T09:07:14.767Z Reads: 351

```
IRF7749L2TRPBF

Mouser had a few thousands a few days ago, but not anymore, Enertion must have bought them all :laughing:
```

---
## \#418 Posted by: bimmer Posted at: 2018-02-28T09:55:22.746Z Reads: 343

```
Yeah...enertion....😉
```

---
## \#419 Posted by: stewii Posted at: 2018-02-28T09:59:48.138Z Reads: 355

```
wait... was it you? :open_mouth:
```

---
## \#420 Posted by: bimmer Posted at: 2018-02-28T10:05:23.061Z Reads: 361

```
Not all of them :smiley: just a couple 100
```

---
## \#421 Posted by: Minim Posted at: 2018-03-01T21:15:35.681Z Reads: 366

```
I sent in a request through the google system a few days ago. Is there any other way of checking price/order these now? 

Also is there demand for alu cases or is this all handled?
```

---
## \#422 Posted by: stewii Posted at: 2018-03-01T21:47:50.390Z Reads: 367

```
@Minim There is a small delay with the aluminium housings , but I should get 40 soon so everything will be provided and sold as a unit if you want. 
You can PM me if you interested.
```

---
## \#423 Posted by: Minim Posted at: 2018-03-01T22:50:14.781Z Reads: 372

```
I was just wondering if there was a demand for machining them :) I just picked up 4meters of 100x30mm alu stock from my supplier. Looks like it would fit the box pretty good so I will machine my own housings but if there is demand I could look into making more of them.
```

---
## \#424 Posted by: banjaxxed Posted at: 2018-03-01T23:19:48.591Z Reads: 369

```
Norwegian cases! Well I have yet to get a price on 5 😎
```

---
## \#425 Posted by: LukePL Posted at: 2018-03-02T08:37:28.257Z Reads: 370

```
No. Does it look like made on DIY CNC? New batch is made on Brother RX450 X1
![IMG_20180301_153250|375x500](upload://nhLqtjjweQviMbdyh5xv2cu6H7k.jpg)
```

---
## \#426 Posted by: banjaxxed Posted at: 2018-03-02T16:04:24.650Z Reads: 356

```
Yeah could be down, anything designed for dual? what about rounding out those wire slots like my revision of stewii's?
```

---
## \#427 Posted by: LukePL Posted at: 2018-03-02T17:44:29.867Z Reads: 356

```
You mean round? Look at last picture.
```

---
## \#428 Posted by: Manu39 Posted at: 2018-03-02T18:22:15.066Z Reads: 373

```
why do axes of fixings of different diameters escape M4 and VESCsix M5 ... and different distances also of a few milimetres ....
![image|666x500](upload://ucsm7XE3ls6IA4SMxZyITTWXNBW.jpg)
A=71mm
B=38mm
M=4
![image|375x500](upload://vwzWK0otldFCckFXyZz7JH1uY7K.jpeg)
A=67
B=39
M=5a

ok just a few mm but a few mm important when the support is already operational ...
```

---
## \#429 Posted by: LukePL Posted at: 2018-03-02T18:33:02.211Z Reads: 347

```
I believe that no one though that it might be important to do that.
```

---
## \#430 Posted by: stewii Posted at: 2018-03-02T18:38:46.830Z Reads: 343

```
When the ESCape was made I didnt have the VESC6 dimensions, never thought of it to be exactly the same and didnt know there was advantages (being compatible with pre drilled mounting holes, boxes, etc ). Maybe on the next iteration of the housing if people really want it to be like that.
```

---
## \#431 Posted by: Nordle Posted at: 2018-03-02T18:49:43.259Z Reads: 338

```
What are overall dimensions of the case? Or are there even 3d files?:)
```

---
## \#432 Posted by: LukePL Posted at: 2018-03-02T18:56:15.641Z Reads: 344

```
It's 77x70x16,5 mm plus pcb cover on top
```

---
## \#433 Posted by: Manu39 Posted at: 2018-03-02T19:19:47.615Z Reads: 350

```
no problem stewii it was just a personal remark .... you were great in conforming to my request ...
sorry for throwing a pave into the pond
```

---
## \#434 Posted by: pixelsilva Posted at: 2018-03-02T21:29:00.839Z Reads: 342

```
This is awesome. We will stop reading stupid nonsense from down under with these lame "China closed for the new year this.." "when China that.." "China blah, blah, blah..."  :nauseated_face: :face_vomiting:
```

---
## \#435 Posted by: pixelsilva Posted at: 2018-03-02T21:31:27.666Z Reads: 336

```
Kudos @stewii !! :+1: :grinning:
```

---
## \#436 Posted by: banjaxxed Posted at: 2018-03-03T10:51:48.890Z Reads: 334

```
Interested in a dual version, any makers?
```

---
## \#437 Posted by: LukePL Posted at: 2018-03-03T13:18:01.276Z Reads: 334

```
Working on it. ;)
```

---
## \#438 Posted by: Riako Posted at: 2018-03-03T13:45:07.098Z Reads: 346

```
Yes ! Cool :+1: 
I'm in with @banjaxxed
```

---
## \#439 Posted by: banjaxxed Posted at: 2018-03-03T14:20:30.858Z Reads: 356

```
It would be nice to do something like this so as to enclose/seal to deck, 7mm rubber gasket, 6mm phase holes, 13mm long power hole

![image|545x330](upload://8wpDsom0h2tJ5Tu0EZZIbJbRQVy.jpg)
```

---
## \#440 Posted by: Nemesis Posted at: 2018-03-03T14:36:43.246Z Reads: 362

```
Deffo would be nice to have a heavy duty rubber case/mount, i've been looking at 9cm-10cm square rubber bench blocks and thinking.. i wonder if its possible to hand cut or even mill out a snug sleeve.. 

![rubber|666x500](upload://wiBXkhukpc7Fz34X4OY3bLWtvDH.jpg)
```

---
## \#441 Posted by: banjaxxed Posted at: 2018-03-03T14:38:15.702Z Reads: 348

```
The alloy is needed for heat dissipation, apart from that would need milling
```

---
## \#442 Posted by: Nemesis Posted at: 2018-03-03T14:38:41.845Z Reads: 352

```
It would be "in my tiny and somewhat poor quality low rez imagination" open topped showing the ally off and allowing it to cool and be cool... :slight_smile:
```

---
## \#443 Posted by: banjaxxed Posted at: 2018-03-03T14:39:51.091Z Reads: 349

```
That gasket could be 3d printed with ninjaflex
```

---
## \#444 Posted by: scepterr Posted at: 2018-03-03T14:53:22.818Z Reads: 354

```
You need the additional mass and thermal contact to aluminum for good heat dissipation, open air isn't really enough as @stewii charted
 https://www.electric-skateboard.builders/t/hw6-4-based-esc-escape/37579/357
```

---
## \#445 Posted by: Nemesis Posted at: 2018-03-03T15:06:36.276Z Reads: 345

```
From above the phase/power wires it "ally" would be exposed only a couple of mm  of the edge and the flat ally surface on top so kind of not fully enclosed, almost like a rubber band/gasket around the edges tho, you are correct would be better naked as most things are..  :wink:
```

---
## \#446 Posted by: LukePL Posted at: 2018-03-04T00:04:12.448Z Reads: 348

```
So you want to put it outside your enclosure? May I ask why?
Those closed holes would require 2 more fixings in CNC process and that is problematic (but possible of course) and will increase the price.
```

---
## \#447 Posted by: Eboosted Posted at: 2018-03-04T04:51:20.695Z Reads: 338

```
I haven't seen anyone runing over the 60k ERPM limit on these ESCapes.

I just got two more and I will test them with 200kv motors on 12S and maybe a 230kv motors at a later time, I'll run them in FOC from the start.
```

---
## \#448 Posted by: LukePL Posted at: 2018-03-04T11:47:39.567Z Reads: 344

```
Ok, guys tell me what you think?
[dual case](http://a360.co/2t9rR8E)
```

---
## \#449 Posted by: Riako Posted at: 2018-03-04T11:56:53.144Z Reads: 341

```
looks great !
```

---
## \#450 Posted by: Riako Posted at: 2018-03-04T12:31:33.671Z Reads: 353

```
to see more clearly, the idea of this genius (but expensive) design is the following ?
![Sans titre-1c|690x406](upload://6LFgVftjYkEXpylSi8dcdnTtON8.jpg)
```

---
## \#451 Posted by: banjaxxed Posted at: 2018-03-04T13:56:15.240Z Reads: 347

```
I like it with some possibilities of improvement maybe.

I'd like those phase/battery holes to be enclosed within the sidewall rather then simply being routed completly out, I like to run things in the open and this design would require copious amounts of sugru, silcone and swearing. And yeah want a big rubber gasket on top but can take care of that here anyway.

The idea behind your big flange (fnarrrr!) is what? that's a bigger piece of stock(more stock is more expensive, more machining is more expensive and time consuming) to acheive no discernable extra cooling and a larger size!?
```

---
## \#452 Posted by: LukePL Posted at: 2018-03-04T18:07:11.136Z Reads: 377

```
![Dual 1|690x432](upload://6Afxc0yGCA5t0pv4jyczf8jSvs9.jpg)![Dual 2|690x432](upload://qsWEFw9dDcDfqOXdCaq4SqpAqMy.jpg)![IMG_20180304_190309|666x500](upload://wX8nGcwXQyc7vPVzgLi9Lr4ON0Y.jpg)

Dimensions with flange 145,5mm x 79,5mm and 2 x single would be 140mm x 77mm.
I can always do it without flange and than it will be 136,5mm x 67,5mm.

@Riako I think I showed all now but you were right in most cases. PCB cove will be recessed so it should look quite nice.

@banjaxxed Again to drill those holes on CNC I would have to turn the enclosure each time to face proper plane for drilling. That requires precise fixture or calibration each time. You can print your gasket and put between flange and enclosure (see my hand drawing). I believe that gasket can be cut like a paper from from thin material. Look at dimensions, without flange it can be really small. I will use for it the same extrusion that I'm use for single so no problem here and milling it is less complicated that turning it to different positions to have round holes. If you are not into cooling it more than what's the point to put sealed enclosure outside main one? I get it in mountain board build (Trampa style) it might be helpful but in street build it's not. Maybe I should wrote it at beginning.... There's no single design that will suit all needs. I just think that this one is most universal. 
On a mountain board it can be done like that .... http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/d/edf47877c14a02fee336e1ed0b393b5becc9342e_1_541x500.jpg  and on a mountain board you could use a better cooling.
```

---
## \#453 Posted by: banjaxxed Posted at: 2018-03-04T20:53:13.630Z Reads: 338

```
[quote="LukePL, post:452, topic:37579"]
Again to drill those holes on CNC I would have to turn the enclosure each time to face proper plane for drilling
[/quote]



ah ok good point with 3 axis cnc, does the loss of the flange help with pricing? the sugru and swearing I can live with, depending on price could be down for 2 x dual and 1 single
```

---
## \#454 Posted by: LukePL Posted at: 2018-03-04T21:01:29.844Z Reads: 344

```
Well sure 3 axis but when someone have 5 axis its working time is probably more expensive :) 
The flange not really. Without it I have to make final contour on whole depth and with it i just leave 2mm.
However those fins on the bottom for sure will. 
I'm trying to see here what people thing and decide which way to go.
```

---
## \#455 Posted by: GrecoMan Posted at: 2018-03-04T21:03:07.231Z Reads: 332

```
can you mill aluminum pulleys?
```

---
## \#456 Posted by: LukePL Posted at: 2018-03-04T21:06:50.077Z Reads: 332

```
Technically sure I can and maybe will do for my Kegels. What you have in mind?
```

---
## \#457 Posted by: GrecoMan Posted at: 2018-03-04T21:08:16.527Z Reads: 324

```
i’ll pm you. don’t wanna derail this thread
```

---
## \#458 Posted by: banjaxxed Posted at: 2018-03-04T21:09:58.479Z Reads: 334

```
Right makes sense the flange is part of the fixture as such and also used for mounting flush with the ouside of an enclosure, pretty multipractical actually

The bottom fins are nice.
```

---
## \#459 Posted by: LukePL Posted at: 2018-03-04T21:24:44.106Z Reads: 336

```
Yes I believe it's a good solution. Hope that others will also she an opinion ( thank you @banjaxxed ;) )
I'll start to do CAM so I'll be able to give you pricing.
```

---
## \#460 Posted by: Mobutusan Posted at: 2018-03-04T22:02:39.649Z Reads: 338

```
I like the design, but where do the sensor cables go?
```

---
## \#461 Posted by: banjaxxed Posted at: 2018-03-04T22:36:28.824Z Reads: 339

```
Jesus christ no more slots, next someone will mention the shagging receiver 😂

Seriously though no problem to get a 'blank' in order to drill my own holes? A no problem option perhaps. I have a 5 axis arm 💪🏻 It's cheap too
```

---
## \#462 Posted by: Riako Posted at: 2018-03-04T23:56:42.231Z Reads: 344

```
in any case I'm in with your dual design !! Like the idea with flange here guys !
Like Banjax said, we could easily finish the drilling at home if it save time, fixture, calbibrate etc ...
:+1:
maybe we should start to make a special topic for that ^^ ...
```

---
## \#463 Posted by: Minim Posted at: 2018-03-05T00:17:58.891Z Reads: 337

```
No it didn’t look like it. Kinda hard to tell without holding the part :) Just genuinely interested in machining.. Need to give these cases a try in my VMC also.
```

---
## \#464 Posted by: LukePL Posted at: 2018-03-05T06:33:47.737Z Reads: 335

```
On top. Goes trough pcb cover like in single one. Look at my hand drawing.
```

---
## \#465 Posted by: LukePL Posted at: 2018-03-05T08:17:53.872Z Reads: 334

```
Thank you for your support :) I believe that no drilling will be required. I think I'll just 3D print it to show everyone how it could work ;)
```

---
## \#466 Posted by: pixelsilva Posted at: 2018-03-05T09:09:12.788Z Reads: 337

```
Good job @LukePL. Looking forward the final product.
```

---
## \#467 Posted by: LukePL Posted at: 2018-03-05T10:13:06.700Z Reads: 353

```
![Dual with PCB cover|690x432](upload://wl20BcgRVRsJGBvt55G6jBSxOzw.jpg)
Printing time 8,5 h :astonished:
```

---
## \#468 Posted by: Riako Posted at: 2018-03-05T12:38:54.269Z Reads: 348

```
https://2girls1mag.files.wordpress.com/2014/03/y8sqt.gif?w=640
outch, patience !! If I could help ...
```

---
## \#469 Posted by: LukePL Posted at: 2018-03-05T18:49:56.492Z Reads: 366

```
![IMG_20180305_194710|666x500](upload://xAZlYl2EQztsuEU0iBg0LmY3T1a.jpg)![IMG_20180305_180904|666x500](upload://aEAVbShSDU4PnLRKCbRIAyl2Yup.jpg)![IMG_20180305_194311|666x500](upload://dtUAdfdM7gfFzX5lmW0wg32EemZ.jpg)![IMG_20180305_181313|666x500](upload://4VJPdTIZxnMrz3b3MIcMOYc9MTH.jpg)![IMG_20180305_180806|375x500](upload://tPxkzSaN5qsm6lhgtb2t6IMFCt6.jpg)![IMG_20180305_195102|666x500](upload://v8Zn2PLi5ZFQ3Io6nFu8HwMs38L.jpg)
```

---
## \#470 Posted by: Riako Posted at: 2018-03-05T19:09:59.884Z Reads: 354

```
https://i.imgur.com/MtZiKJ3.gif?noredirect

yes yes, I want it !!!
```

---
## \#471 Posted by: Manu39 Posted at: 2018-03-05T19:13:51.911Z Reads: 351

```
Whaouuu good  work...
```

---
## \#472 Posted by: banjaxxed Posted at: 2018-03-05T20:57:05.589Z Reads: 354

```
Shwing, very nice @LukePL...no need to print after the proto...worth doing :slight_smile:
```

---
## \#473 Posted by: Surfer Posted at: 2018-03-05T21:10:14.113Z Reads: 348

```
Already looks beautiful!! 
Weight of the print please?
```

---
## \#474 Posted by: lrdesigns Posted at: 2018-03-06T00:16:24.389Z Reads: 356

```
This is it guys, the case / controller we have all been waiting for. :drooling_face:
![image|690x396](upload://8Nx6200gBpiNr8ok1JhidRR5Iex.jpg)
```

---
## \#475 Posted by: Mobutusan Posted at: 2018-03-06T02:23:53.909Z Reads: 346

```
That looks sooo good! Any interest in making these for FOCBOX's, but compatible with the existing FOCBOX cases, so there's no disassembly and it's plug and play? I'll be your first customer as long as they don't cost an arm AND a leg. (I need my legs to skate.)
```

---
## \#476 Posted by: eb1925 Posted at: 2018-03-06T03:56:01.686Z Reads: 352

```
You have all the magical 3d printed/CAD powers. You know de wae. ![de wae|480x480](upload://iiOhe40e5q2wto7ndd04D0aN15l.jpg)
```

---
## \#477 Posted by: bevilacqua Posted at: 2018-03-06T07:50:30.194Z Reads: 345

```
Is a black anodised option planed? 
Because matte black everything ;) 

Loos really good!
```

---
## \#478 Posted by: pixelsilva Posted at: 2018-03-06T08:17:08.701Z Reads: 336

```
Mannnn.... please, no more Focbox crap. Sick of that thing from down under. Is ESCape time now. :wink::rofl:
```

---
## \#479 Posted by: notger Posted at: 2018-03-06T09:05:52.943Z Reads: 341

```
[quote="pixelsilva, post:478, topic:37579, full:true"]
Mannnn… please, no more Focbox crap. Sick of that thing from down under. Is ESCape time now.
[/quote]

Don't get it, i ride dual Focboxes for >2000km now without proplems and can alos not read any major often appearing Problems here in the Forum.

So what is it about that makes you Sick ?
```

---
## \#480 Posted by: pixelsilva Posted at: 2018-03-06T09:47:49.526Z Reads: 339

```
Here, (@stewii, @bimmer & others), are making great efforts to part ways from traditional (and expensive) VESCs like Trampa or Enertion. There are many treads here where you can read about them. Lets stick to ESCape in this one. No need to keep associating this project to those. Enough of VESC6 and Focboxes.:roll_eyes:
```

---
## \#481 Posted by: Silverline Posted at: 2018-03-06T10:46:31.643Z Reads: 339

```
I just bought two Escape... And looking forward to receive when they are made. But damn i would love that dual housing in alu....  Who sell me one 😃
```

---
## \#482 Posted by: bimmer Posted at: 2018-03-06T10:53:55.423Z Reads: 340

```
I am just buying pcb's from stewie and having them assembled. He is the brains behind all of this.
```

---
## \#483 Posted by: Nordle Posted at: 2018-03-06T11:47:02.171Z Reads: 344

```
Can some1 lead me to the BOM list for the escape? This may become my first smd project :fire:
```

---
## \#484 Posted by: Manu39 Posted at: 2018-03-06T12:39:08.217Z Reads: 346

```
look at the first post ...
[https://www.dropbox.com/s/kgdrnrdylf28ddw/HW64_BOM.ods?dl=0](https://www.dropbox.com/s/kgdrnrdylf28ddw/HW64_BOM.ods?dl=0)
```

---
## \#485 Posted by: LukePL Posted at: 2018-03-06T13:03:48.171Z Reads: 346

```
@Surfer estimated weight in aluminium is 193g

 @Mobutusan it can be done and wouldn't bo so dificult. When I finish that I'll think about it and see if there's a interest.

@eb1925 :joy:

@bevilacqua I can check that once prototype is done but main goal is to be affordable  

@Silverline @stewii will have them to ;)

Thank you all for good words ;)
```

---
## \#486 Posted by: Nordle Posted at: 2018-03-06T13:16:34.987Z Reads: 335

```
I did, and now i did again. Can't find it. But thank you sir.
```

---
## \#487 Posted by: Silverline Posted at: 2018-03-06T15:50:43.116Z Reads: 340

```
@LukePL  Nice.

I contact him :slight_smile:

Sorry if it has been mentioned before, but what are the dimensions for the cut outs, i need to make in my enclosure :-) ?
```

---
## \#488 Posted by: Jc06505n Posted at: 2018-03-06T16:15:28.898Z Reads: 349

```
Is it really a part way though? As i understand this is just a cheaper but same Quality VESC 6. It's still prone to any failures that Focboxes or VESC6 have. Unless there's been improvements that I haven't caught aside from MPU. 

An amazing alternative to current ESC that I'm about to hit stewii up for ? Hell Yea. But a partway ? Eh.
```

---
## \#489 Posted by: stewii Posted at: 2018-03-06T16:36:05.827Z Reads: 357

```
This is how it looks like in black (need to get different screws)

![IMG_5050|375x500](upload://v9NZFXm1pQX8eDYK6DrAo6RRUgC.JPG)
```

---
## \#490 Posted by: pixelsilva Posted at: 2018-03-06T19:25:32.381Z Reads: 350

```
Don't worry..... 'Jason', it'll be an alternative anyway. Better than expensive (twice the price) or impossible to get (China shipment gremlins) VESCs.
```

---
## \#491 Posted by: Jc06505n Posted at: 2018-03-06T19:33:21.674Z Reads: 355

```
[quote="pixelsilva, post:490, topic:37579"]
Don’t worry… ‘Jason’, it’ll be an alternative anyway
[/quote]

Close but the 'a' and 's' are different letters .And oh yea no doubt. Far better than Trampa (i don't understand how they're not shitting their pants with these cheaper just as good alternatives) and the stock unavailability of Focboxes. I'm just saying that theyr'e all these are , alternatives. Not next step. Next step would be a VESC 7.
```

---
## \#492 Posted by: Acido Posted at: 2018-03-06T19:41:13.405Z Reads: 352

```
I don't think the  care much, they are making a shit ton of money on their other stuff, also they maybe ordered a batch of 100 or so that's like less than a 800$ or so.
```

---
## \#493 Posted by: b264 Posted at: 2018-03-07T00:41:20.668Z Reads: 347

```
How do you know they don't have color-changing pants?  They might...
```

---
## \#494 Posted by: gbutcher Posted at: 2018-03-07T02:06:31.490Z Reads: 351

```
If running 12S on these, do we still need to be mindful of the 60k ERPM limit and use a lower KV motor?
```

---
## \#495 Posted by: scepterr Posted at: 2018-03-07T02:11:17.244Z Reads: 359

```
Nope, 100-120k erpm is ok
```

---
## \#496 Posted by: Cobber Posted at: 2018-03-07T02:16:37.398Z Reads: 352

```
Scepy you are confident at 120k erpm, do you think a 540kv 10 pole (5 pole pairs) @12s will survive?
```

---
## \#497 Posted by: scepterr Posted at: 2018-03-07T02:17:52.100Z Reads: 347

```
What would be the erpm on that, too lazy to do the math myself 😛
```

---
## \#498 Posted by: Cobber Posted at: 2018-03-07T02:19:36.231Z Reads: 347

```
without any weighting it would be 23,976rpm, 119,880erpm.
```

---
## \#499 Posted by: scepterr Posted at: 2018-03-07T02:20:00.905Z Reads: 342

```
Oh, yeah that should be no problem
```

---
## \#500 Posted by: Nordle Posted at: 2018-03-07T08:05:25.575Z Reads: 336

```
Is there another BOM list? cant open this dropbox file on my phone:/
```

---
## \#501 Posted by: webst Posted at: 2018-03-07T08:07:28.242Z Reads: 345

```
It opens in Safari on iOS but you could try to download AndrOpen Office if on Android.
```

---
## \#502 Posted by: Nordle Posted at: 2018-03-07T08:10:00.077Z Reads: 346

```
It does not open in safari for me, i even download the dropbox app, no luck.
```

---
## \#503 Posted by: Acido Posted at: 2018-03-07T08:15:10.781Z Reads: 352

```
Try WPS office
```

---
## \#504 Posted by: Nordle Posted at: 2018-03-07T08:38:27.212Z Reads: 346

```
Wps office also doesn't work. Format not supportrt in both apps...
Someone got another BOM list?:)
```

---
## \#505 Posted by: b264 Posted at: 2018-03-07T09:02:31.904Z Reads: 330

```
Open it on a computer and not on the phone
```

---
## \#506 Posted by: Nordle Posted at: 2018-03-07T09:08:47.140Z Reads: 335

```
Just no, and i assume you don't have what i'm looking for, else you probably just would have linked it.
So can't really give you a thanks or a like for this useless post...
```

---
## \#507 Posted by: b264 Posted at: 2018-03-07T09:36:26.167Z Reads: 338

```
I have it, but it only lets me put images on here is the problem.  It's the forum doing that, which is probably why it was originally linked from a dropbox in the first place.  I also used a computer to open it on though, too and not a phone.

I can't really thank you for being rude when I suggested the best possible course of action for you.  Next time I will ignore you.
```

---
## \#508 Posted by: webst Posted at: 2018-03-07T09:42:09.731Z Reads: 353

```
There you have it:
https://docs.google.com/spreadsheets/d/1eYtcOQ3qFSzKLLraEMxRk_Ek-uDgsGqHRAEkxtAuPJM/edit?usp=sharing

I just imported dropbox file to google spreadsheets for you, don't know if the contents are up to date etc.
```

---
## \#509 Posted by: Nordle Posted at: 2018-03-07T10:20:43.336Z Reads: 353

```
[quote="b264, post:507, topic:37579"]
Next time I will ignore you.
[/quote]
I appreciate that. That saves me a lot of read time.

Really thank you @webst, now i can fill my shopping cart. And in the evening when i get closer to my pc i can do things there wich i really could not do on a phone.
```

---
## \#510 Posted by: chsknight Posted at: 2018-03-10T05:14:08.333Z Reads: 347

```
Does anyone have extra "06035C104JAT2A"  they can sell to me?  My order got backordered and most vendors look out of stock.
```

---
## \#511 Posted by: b264 Posted at: 2018-03-10T06:11:57.490Z Reads: 352

```
[quote="chsknight, post:510, topic:37579"]
06035C104JAT2A
[/quote]

It's better to use 100V capacitors anyway
```

---
## \#512 Posted by: scepterr Posted at: 2018-03-10T06:14:18.833Z Reads: 365

```
If you guys missed it in the pics thread testing out a dual plate from @akhlut
 
![IMG_20180309_173033__01|690x398](upload://zAPHYzkw12BC4mm0b5zKxNeKsFu.jpg)

![IMG_20180309_125223|375x500](upload://32j0ITzeq4VObBVSEIhnGzA5umJ.jpg)
```

---
## \#513 Posted by: Jc06505n Posted at: 2018-03-10T06:31:55.927Z Reads: 356

```
What iOS are you running?


Edit: Ah nvm you got it. Didn’t have to be a dick about It though.
```

---
## \#514 Posted by: stewii Posted at: 2018-03-10T11:49:55.881Z Reads: 360

```
this is the automotive equivalent and in stock: 06035C104J4T2A
[quote="chsknight, post:510, topic:37579, full:true"]
Does anyone have extra "06035C104JAT2A"  they can sell to me?  My order got backordered and most vendors look out of stock.
[/quote]



Nice job. How are you going to mount it ?


[quote="scepterr, post:512, topic:37579, full:true"]
If you guys missed it in the pics thread testing out a dual plate from @akhlut
[/quote]
```

---
## \#515 Posted by: scepterr Posted at: 2018-03-10T12:00:34.141Z Reads: 366

```
It's sitting on some closed cell foam and will be siliconed to the enclosure
![IMG_20180309_181358__01|690x368](upload://isxZ6FSWjnAmNkKz7nAs3CYmjHo.jpg)
![IMG_20180309_181608|375x500](upload://7fDzB5DSZSf958LkIxpYEOlWS8D.jpg)
```

---
## \#516 Posted by: Mikenopolis Posted at: 2018-03-10T12:03:23.279Z Reads: 355

```
just wondering...do you sleep?! it's 4 am here, so 7am there.
```

---
## \#517 Posted by: scepterr Posted at: 2018-03-10T12:04:03.824Z Reads: 370

```
Eventually...not sure when I'll let you know if it happens 😋

This is what I'm doing right now...looking at sexy holes
![Screenshot_20180310-064634~2|405x500](upload://hjWNAUuey86fH1c707jFWRTs0I5.jpg)
![Screenshot_20180310-064625~2|416x500](upload://1GPlUaE9fFzG9il8NmH0fiJ16ud.jpg)
```

---
## \#518 Posted by: Mikenopolis Posted at: 2018-03-10T12:06:23.419Z Reads: 358

```
damn addict :syringe::pill:

I'm just getting ready to leave the office, been here for like 20 hours
```

---
## \#519 Posted by: LukePL Posted at: 2018-03-10T12:08:25.352Z Reads: 358

```
Wait.... You are putting ESCape on a plate to improve cooling and than you insulate the whole surface with foam? Am I missing something? :face_with_raised_eyebrow:
```

---
## \#520 Posted by: scepterr Posted at: 2018-03-10T12:09:31.375Z Reads: 364

```
The surface that matters is the one facing the ESCapes, the foam is on the backside for vibration absorbing
```

---
## \#521 Posted by: stewii Posted at: 2018-03-10T12:13:09.224Z Reads: 362

```
it is not ideal, but in that case the plate will "store" the heat, it will take longer to cool itself down but will still relief the mosfets from the heat.
```

---
## \#522 Posted by: scepterr Posted at: 2018-03-10T12:15:07.931Z Reads: 361

```
It's a nice chunk of aluminum, and I don't plan running anywhere near limits for long 😋
```

---
## \#523 Posted by: Mikenopolis Posted at: 2018-03-10T12:16:27.535Z Reads: 360

```
in this for a Trampa? 

I'm wondering about the dual focbox case I have, not sure if I wanna cut a hole in the enclosure to vent the heat out.
```

---
## \#524 Posted by: scepterr Posted at: 2018-03-10T12:16:40.744Z Reads: 358

```
Nah it's the Zenith
```

---
## \#525 Posted by: Mikenopolis Posted at: 2018-03-10T12:17:51.707Z Reads: 364

```
so this thing will be fully enclosed within the enclosure?
```

---
## \#526 Posted by: scepterr Posted at: 2018-03-10T12:20:47.918Z Reads: 373

```
Yeah I don't foresee it being an issue but if it becomes one can add an external facing heatsink. 
One of these
![IMG_20180226_232221|541x500](upload://xX2W36LvImullDIU8mGxuKjktki.jpg)
```

---
## \#527 Posted by: LukePL Posted at: 2018-03-10T12:25:06.713Z Reads: 361

```
This is a very good solution! I was inspired by it making this dual enclosure ;)
```

---
## \#528 Posted by: bevilacqua Posted at: 2018-03-10T16:26:15.367Z Reads: 359

```
@stewii could I order this cap: 
MM035C104KCZ2A 
instead of this one in your BOM 06035C104JAT2A

only difference I found was the tolerance, 10% instead of 5% 

Thanks for your help.

(Buying on mouser.de)
```

---
## \#529 Posted by: stewii Posted at: 2018-03-10T16:41:01.765Z Reads: 344

```
yes that's fine but the one i suggested (06035C104J4T2A) is 5% and cheaper :)
```

---
## \#530 Posted by: Nordle Posted at: 2018-03-11T07:27:55.033Z Reads: 343

```
But it's out of stock in many places. ;)
C0603C104J5RACAUTO ->seems to be the same
```

---
## \#531 Posted by: stewii Posted at: 2018-03-11T07:46:57.837Z Reads: 347

```
You obviously didn’t search for that part ...

[quote="Nordle, post:530, topic:37579, full:true"]
But it's out of stock in many places. ;)
C0603C104J5RACAUTO ->seems to be the same
[/quote]
```

---
## \#532 Posted by: Nordle Posted at: 2018-03-11T08:42:24.796Z Reads: 347

```
Sure i did, or it was out of stock the other day, or i made an error. If i would have found it to be in stock i wouldn't have searched for a substitute at all.

Now having trouble finding this diode: PMEG6020ER,115
Can i just look for one with higher voltage and/or current rating in the same package, or are there other important values?
```

---
## \#533 Posted by: notepad Posted at: 2018-03-11T23:23:36.810Z Reads: 338

```
Damn dude. that black cover is amazing. your making me regret getting my Focboxes (since one is already dead)
```

---
## \#534 Posted by: michaelcpg Posted at: 2018-03-11T23:34:25.404Z Reads: 342

```
I'm in the same boat except my focboxes are still on order. Tempted to see if I can cancel the order and get a pair of these instead. Particularly seeing as the rest of my build is nearly done and it doesn't seem like the focboxes are going to be in stock for a while yet
```

---
## \#535 Posted by: notepad Posted at: 2018-03-11T23:37:33.746Z Reads: 344

```
If you paid by card or paypal, just cancel. TBH its a bit of a farce that its taken so long. especially since it seems like the QC has gone down for them to push out more boxes.
```

---
## \#536 Posted by: michaelcpg Posted at: 2018-03-11T23:56:22.177Z Reads: 340

```
@stewii sorry if you've mentioned this already somewhere recently but what is the current lead time on a pair of these prebuilt with aluminium enclosures?
```

---
## \#537 Posted by: Apolo Posted at: 2018-03-12T04:40:12.558Z Reads: 337

```
@stewii I also got lost in reading through this thread, I think you should make a separate thread strictly for purchasing prebuilt ESCapes. 

Are they still 125GBP each for prebuilt?
```

---
## \#538 Posted by: moon Posted at: 2018-03-12T04:40:47.685Z Reads: 334

```
He probably should have a website at this point
```

---
## \#539 Posted by: scrapheap Posted at: 2018-03-12T04:46:38.774Z Reads: 351

```
[quote="scrapheap, post:385, topic:37579"]
With housing, it’s 150 GBP + shipping + paypal fees (if using goods and services)

Without housing, it’s 130 GBP + shipping + fees
[/quote]

10 days ago, he stated there was a little delay with the aluminum housings. Once the 40 he has ordered come in, he'll be able to fill orders that asked for them.
```

---
## \#540 Posted by: rickyd Posted at: 2018-03-12T07:44:35.275Z Reads: 341

```
Do you also sell kits, i.e. all parts unsoldered?
```

---
## \#541 Posted by: bimmer Posted at: 2018-03-12T09:17:58.655Z Reads: 353

```
Is that something people would like?
```

---
## \#542 Posted by: sMATTEr Posted at: 2018-03-12T09:21:27.810Z Reads: 354

```
I would atleast buy two kits :sunglasses:
```

---
## \#543 Posted by: sMATTEr Posted at: 2018-03-12T09:22:24.000Z Reads: 360

```
Well. If it’s not 120$ that is.
```

---
## \#544 Posted by: bimmer Posted at: 2018-03-12T09:22:57.273Z Reads: 379

```
Just the PCB or the whole thing?![1520846684216732762194|281x500](upload://9suq1XXdjQKOsENAYK19MCoDrhT.jpg)This + smd parts being the whole thing.
```

---
## \#545 Posted by: sMATTEr Posted at: 2018-03-12T09:26:36.184Z Reads: 357

```
If you by the whole thing mean housing. Then no, only PCB with all the components. This is diy after all :wink:
```

---
## \#546 Posted by: Nordle Posted at: 2018-03-12T10:12:32.978Z Reads: 348

```
I would buy one set probably, just to starting into smd soldering. Later i would buy more:)
```

---
## \#547 Posted by: webst Posted at: 2018-03-12T10:23:47.463Z Reads: 357

```
Don't you also need to program it before using?
```

---
## \#548 Posted by: Nordle Posted at: 2018-03-12T10:34:22.555Z Reads: 367

```
Sure you have to. Not sure how its done however, but can't immagine that being harder than the soldering job.
```

---
## \#549 Posted by: Ps6ch0d0gg Posted at: 2018-03-13T12:33:48.252Z Reads: 377

```
Hi, finally all the pieces ... editing in progress ... again thanks stewii![20180313_132900|666x500](upload://1f0vSTrBdPSpzWhXi6PykHNXypi.jpg)
```

---
## \#550 Posted by: Manu39 Posted at: 2018-03-13T12:46:39.844Z Reads: 368

```
Nice man very Nice ...
I look forward to receiving my vescape 😜
```

---
## \#551 Posted by: rickyd Posted at: 2018-03-13T13:19:52.100Z Reads: 359

```
Where did you get this nice mount for the XT-connector?
```

---
## \#553 Posted by: rickyd Posted at: 2018-03-13T14:36:24.590Z Reads: 366

```
No, I mean the red aluminium thing that mounts the XT-connector to the case.
```

---
## \#554 Posted by: Ps6ch0d0gg Posted at: 2018-03-13T15:06:45.518Z Reads: 383

```
oups ok désolé j'ai eu du mal à comprendre. Voici le lien pour ...

http://s.aliexpress.com/uMreeIZ3?fromSns=Mé

![Screenshot_20180313-160616|281x500](upload://xoXQFJAck5umcmpSsjuFPb0lU2x.jpg)
```

---
## \#555 Posted by: rickyd Posted at: 2018-03-13T15:07:32.976Z Reads: 372

```
Nice! Thanks!
```

---
## \#556 Posted by: Cobber Posted at: 2018-03-13T22:11:59.428Z Reads: 377

```
That is awesome, I don't know why more people are not on this!

https://ae01.alicdn.com/kf/HTB1kUgjOpXXXXbHXpXXq6xXFXXXW/220122052/HTB1kUgjOpXXXXbHXpXXq6xXFXXXW.jpg?size=63164&height=474&width=555&hash=385aac6f2b9fc3505d25077eeda4ac0f
```

---
## \#557 Posted by: ArnhemAnt Posted at: 2018-03-13T22:36:28.724Z Reads: 378

```
[quote="michaelcpg, post:534, topic:37579, full:true"]
I’m in the same boat except my focboxes are still on order. Tempted to see if I can cancel the order and get a pair of these instead. Particularly seeing as the rest of my build is nearly done and it doesn’t seem like the focboxes are going to be in stock for a while yet
[/quote]

I also had two Focbox on order initially. Got sick of waiting. Emailed them, cancelled the order, got a refund and then sent my cash to stewii.
```

---
## \#558 Posted by: Ps6ch0d0gg Posted at: 2018-03-13T23:10:08.115Z Reads: 387

```
tomorrow last cable between the two and programming. I do not know why but I feel like I'm going to fly.![20180314_000532|374x500](upload://pDZZOpT5SsWzvGf9WR2siAl1nl9.jpg)
```

---
## \#559 Posted by: scepterr Posted at: 2018-03-14T06:14:41.334Z Reads: 378

```
If you need to pair 2x10awg, save space and want to be able to disconnect, 8mm bullets 😋
![IMG_20180313_145154__01|566x500](upload://DcLYSGTg9MnTsNbhbWSj1RWxVT.jpg)
```

---
## \#560 Posted by: Exiledd_Top Posted at: 2018-03-14T06:42:19.329Z Reads: 375

```
I was berly available to solder 10awg wire and with a solder gun i  cant imagine trying to heat up 2 10awg wires together into a 8mm bullet connector what solder iron or gun do u use
```

---
## \#561 Posted by: scepterr Posted at: 2018-03-14T06:46:33.188Z Reads: 374

```
Lol for that I used the Aoyue 9378
https://www.amazon.com/dp/B00BSW69LI/ref=cm_sw_r_cp_apa_eumQAbZAKVAG4
```

---
## \#562 Posted by: zblad Posted at: 2018-03-14T13:44:03.758Z Reads: 365

```
I have two questions about the Bill of Materials.  What is the Switch for at the very bottom (P8)?  Also is the wireless and motion tracking stuff in the Place column required?
```

---
## \#563 Posted by: b264 Posted at: 2018-03-14T14:03:29.328Z Reads: 368

```
set at what temperature?
```

---
## \#564 Posted by: scepterr Posted at: 2018-03-14T18:17:38.814Z Reads: 376

```
435c
10cha
```

---
## \#565 Posted by: Ps6ch0d0gg Posted at: 2018-03-15T08:00:15.834Z Reads: 387

```
Hi after a little test on the road I would only say one thing ... roxxy esc for sale! next board will be with stewii Escape.
 ps: if you emit sticker Escape could see me send it.![20180314_211101|666x500](upload://2QOKwj6JiRsEaZDH5i18KSMJujC.jpg)
```

---
## \#566 Posted by: stewii Posted at: 2018-03-15T21:06:27.962Z Reads: 385

```
Ok so the housings finally arrived and should ship a few controllers tomorrow. 

![image|375x500](upload://os0pQjztSjIof0FC29oFY54LWMK.jpeg)
```

---
## \#567 Posted by: Silverline Posted at: 2018-03-15T21:09:29.848Z Reads: 374

```
So freaking gorgeous :heart_eyes::heart_eyes::heart_eyes:

Do you know if i´m one of the lucky ones, whos EsCape going to be send out tomorrow ?
```

---
## \#568 Posted by: scepterr Posted at: 2018-03-15T21:11:19.334Z Reads: 388

```
Did a slight tweak on my dualplate, more heatsink which will double as wire channel 😋
![IMG_20180315_143706__01|690x305](upload://1LIt5xIPBH57bPUPEdANwLjgxeF.jpg)
```

---
## \#569 Posted by: stewii Posted at: 2018-03-15T21:19:54.343Z Reads: 388

```
yours will be send out saturday :)
```

---
## \#570 Posted by: Manu39 Posted at: 2018-03-15T22:00:06.500Z Reads: 385

```
hoboho noel is not finished .... beautiful in black @Stewii ....
```

---
## \#571 Posted by: bigben Posted at: 2018-03-15T22:00:40.293Z Reads: 381

```
You know you can beat the focboxes to my door...
```

---
## \#572 Posted by: bimmer Posted at: 2018-03-15T22:02:17.832Z Reads: 377

```
Anyone could do that. :D
```

---
## \#573 Posted by: ATLesk8 Posted at: 2018-03-15T22:34:36.741Z Reads: 372

```
That's hilarious that someone could garage design a working product and have it in customers hands in the span of a single shipping delay.
```

---
## \#574 Posted by: bimmer Posted at: 2018-03-15T22:38:01.073Z Reads: 378

```
When you have Websites, employees and point of sale to pay you can't just take a cut on margins.
We could and did.
```

---
## \#575 Posted by: rickyd Posted at: 2018-03-16T07:45:57.633Z Reads: 376

```
What is the current wait time from order to delivery?
```

---
## \#576 Posted by: stewii Posted at: 2018-03-16T08:12:33.623Z Reads: 381

```
At least 2 weeks till I can ship the ESCs. Have a lot of orders coming.
```

---
## \#577 Posted by: ron Posted at: 2018-03-16T13:23:34.011Z Reads: 390

```
Where did you get the stencils?
```

---
## \#578 Posted by: Acido Posted at: 2018-03-17T17:19:17.867Z Reads: 382

```
These are soldered using machines or by hand
```

---
## \#579 Posted by: Cobber Posted at: 2018-03-17T21:20:02.441Z Reads: 382

```
I am waiting for a few ESCapes...

Have we got a technical diagram of the current alloy case?

specifically the bolt hole pattern, I want to make sure it bolts up to my heatsink.
```

---
## \#580 Posted by: pixelsilva Posted at: 2018-03-17T23:24:39.623Z Reads: 383

```
> @ATLesk8
>  
> That’s hilarious that someone could garage design a working product and have it in customers hands in the span of a single shipping delay.

...is yellow, you fried it, and chicken lays it... what it is?
```

---
## \#581 Posted by: Riako Posted at: 2018-03-18T12:37:34.023Z Reads: 372

```
:grinning: Hey Luke ! **Is that great 3D model still on work ?**
Spring in a few days, I start to purchase my missing parts :blush:
```

---
## \#582 Posted by: LukePL Posted at: 2018-03-18T13:29:17.523Z Reads: 379

```
I had hard time to make some corrections but I send it to @stewii like an hour ago for final check. After a confirmation from him I'll start making alu prototype.
```

---
## \#583 Posted by: Acido Posted at: 2018-03-18T15:57:32.903Z Reads: 371

```
@stewii are you planning to produce them in a factory like 100-300pcs batch?
```

---
## \#584 Posted by: stewii Posted at: 2018-03-18T17:18:11.116Z Reads: 370

```
Yes I am :)
```

---
## \#585 Posted by: FredrikHems Posted at: 2018-03-18T17:19:04.613Z Reads: 375

```
Any thoughts on what the price will be then?
```

---
## \#586 Posted by: Acido Posted at: 2018-03-18T17:24:41.175Z Reads: 370

```
Probably same as @bimmer
```

---
## \#587 Posted by: Acido Posted at: 2018-03-18T17:24:55.658Z Reads: 373

```
Thats great!
Do you maybe know when?
```

---
## \#588 Posted by: Manu39 Posted at: 2018-03-18T17:27:08.738Z Reads: 371

```
certainly if the price goes down it will be only one more ... but it is already very honest ...
```

---
## \#589 Posted by: Silverline Posted at: 2018-03-18T18:05:19.681Z Reads: 377

```
Take my money :-)
```

---
## \#590 Posted by: ducktaperules Posted at: 2018-03-18T18:08:26.309Z Reads: 379

```
i would switch to this so quick if this was avalable with 2 vesc pre-installed without having to void any warranty
```

---
## \#591 Posted by: LukePL Posted at: 2018-03-18T18:34:45.869Z Reads: 374

```
It's going to happen guys we are finalizing the design ;)
```

---
## \#592 Posted by: Silverline Posted at: 2018-03-18T19:02:59.847Z Reads: 378

```
When can we sign up :-)
```

---
## \#593 Posted by: Lambjr088 Posted at: 2018-03-19T05:46:51.075Z Reads: 374

```
I think a new sale thread should be started just for this product. Just a thought
```

---
## \#594 Posted by: ron Posted at: 2018-03-19T10:54:14.566Z Reads: 370

```
Are you going to sell not assembled kits with all the bells and whistles (Case/Parts/PCB)?
```

---
## \#595 Posted by: ervinelin Posted at: 2018-03-19T14:11:25.765Z Reads: 378

```
How do I place an order and how much are we talking about?
```

---
## \#596 Posted by: Manu39 Posted at: 2018-03-19T14:14:51.117Z Reads: 380

```
post a private message @stewii
😉
```

---
## \#597 Posted by: Acido Posted at: 2018-03-19T16:00:12.613Z Reads: 381

```
whats the current price?
```

---
## \#598 Posted by: chickengun Posted at: 2018-03-19T18:41:05.515Z Reads: 398

```
And pray for a reply within this year :sweat_smile:
```

---
## \#599 Posted by: Manu39 Posted at: 2018-03-19T18:50:07.736Z Reads: 452

```
🙏....the price is indicated in the post number 8 and has not changed it seems to me ...😉
```

---
## \#600 Posted by: stewii Posted at: 2018-03-19T23:07:42.717Z Reads: 467

```
Sorry guys, been so busy doing the last orders. 

1.Very soon there will be a group buy so I can order a big batch from a factory. 

2.Might have to change the design because apparently Frank owns the IP of almost all the possible design variations and emailed (threaten) me about this.

3.I don't plan selling kits.

4.Current price is £150. But I am holding up new orders (i have too many-- see point 1)

5.Dual housing is LukePL domain.

6. i'm sure i'm forgetting something :)
```

---
## \#750 Posted by: uigiroux Posted at: 2018-03-20T18:05:14.309Z Reads: 458

```
@stewii do you plan on releasing this enclosure, and would it be possible to have it made from aluminum as well? 
![Screenshot_20180320-130326|690x362](upload://lmo3EVCQAqJHNcEi3ZgBmMS9Dxe.jpg)
```

---
## \#752 Posted by: stewii Posted at: 2018-03-20T18:06:56.214Z Reads: 446

```
LukePL will. I think he is doing the CAM programming. The debate is do we want symmetry? Remember that some OCD people :) wanted that.
```

---
## \#753 Posted by: stewii Posted at: 2018-03-20T18:08:15.548Z Reads: 443

```
Your housings look premium but people want cheap ESCapes and will have to have them made in China to cut on costs.
```

---
## \#754 Posted by: uigiroux Posted at: 2018-03-20T18:08:52.171Z Reads: 442

```
Lol, I think that's perfect it's so small!
```

---
## \#756 Posted by: uigiroux Posted at: 2018-03-20T18:14:03.280Z Reads: 435

```
So in the first post it says it's $130 for complete ESCape, then I think I saw it was now £150, can you confirm the price for the complete package of HW, enclosure, and PCB?
```

---
## \#757 Posted by: Deckoz Posted at: 2018-03-20T18:15:57.324Z Reads: 432

```
I think that was without housing... and the second with housing..
```

---
## \#758 Posted by: Acido Posted at: 2018-03-20T18:20:14.374Z Reads: 440

```
yea, thats the price i got about a month ago
```

---
## \#759 Posted by: Kug3lis Posted at: 2018-03-20T18:34:49.497Z Reads: 448

```
We talked before about the pricing, the prices are for single units in our store. But you can buy bulk at a lower price for e.g. Same design without fins as Single Focbox

https://shop.3dservisas.eu/products/single-focbox-case-without-cooling-fins

Can be made cheaper:

* 50 units 20€/ea
* 30 units 22€/ea

So if you are interested let me know.
```

---
## \#760 Posted by: b264 Posted at: 2018-03-20T18:49:15.635Z Reads: 429

```
[quote="stewii, post:753, topic:37579, full:true"]
Your housings look premium but people want cheap ESCapes and will have to have them made in China to cut on costs.
[/quote]

TB VESC serves the "cheap" market.  I don't think that statement makes sense.  A FOCBOX would be for them.
```

---
## \#761 Posted by: stewii Posted at: 2018-03-20T18:50:16.387Z Reads: 430

```
Cheap was probably the wrong word.
```

---
## \#776 Posted by: Namasaki Posted at: 2018-03-20T22:50:55.648Z Reads: 420

```

```

---
## \#788 Posted by: bimmer Posted at: 2018-03-20T23:12:31.545Z Reads: 433

```
http://www.electric-skateboard.builders/t/the-legitimacy-of-a-trademark-on-an-opensource-design/49671
```

---
## \#790 Posted by: Namasaki Posted at: 2018-03-20T23:19:05.803Z Reads: 423

```

```

---
## \#712 Posted by: Namasaki Posted at: 2018-03-20T23:58:26.812Z Reads: 328

```
44 posts were merged into an existing topic: [The legitimacy of a trademark on an opensource design](/t/the-legitimacy-of-a-trademark-on-an-opensource-design/49671)
```

---
## \#791 Posted by: Namasaki Posted at: 2018-03-21T00:06:25.894Z Reads: 415

```

```

---
## \#792 Posted by: scepterr Posted at: 2018-03-21T01:29:44.313Z Reads: 435

```
Took R1 off on mine, seems a bit too risky, might be better leaving it off in the future
![IMG_20180320_203218|666x500](upload://5VV9z6abn4K0AZkdpCF0Ff0Qh3n.jpg)
```

---
## \#793 Posted by: ArnhemAnt Posted at: 2018-03-21T04:17:17.569Z Reads: 419

```
R1 ?? Sorry for the 'silly' question but what is R1?
```

---
## \#794 Posted by: scepterr Posted at: 2018-03-21T04:26:55.723Z Reads: 416

```
R1 is 0 ohm resistor, that when populated allows you to draw power from USB
The issue is when you have both usb and battery connected you are feeding 5V from 2 sources
```

---
## \#795 Posted by: ArnhemAnt Posted at: 2018-03-21T04:31:09.620Z Reads: 419

```
Thank you kind Sir, for clarifying this.
```

---
## \#796 Posted by: pixelsilva Posted at: 2018-03-21T04:43:18.969Z Reads: 419

```
https://media.giphy.com/media/Rt23MIHkCJwdy/giphy.gif
```

---
## \#797 Posted by: webst Posted at: 2018-03-21T06:05:28.116Z Reads: 422

```
That is not the issue but cause. What’s the issue? Is this layout error?
```

---
## \#798 Posted by: scepterr Posted at: 2018-03-21T06:08:25.608Z Reads: 418

```
It's not a layout error, it's an optional component, it is useful for initial flash before even hooking up a battery, but I think poses too much risk leaving on. I had strange behavior on my windows tablet when connected to vesc tool and a battery, when I spun up the motor and applied breaks my touchscreen would stop working normally for a few seconds
```

---
## \#799 Posted by: webst Posted at: 2018-03-21T06:25:02.652Z Reads: 420

```
Isn’t it the way this was designed? I’m asking to know if it’s isolated case. Isn’t it the way everybody uses it? Maybe the fault is on a tablet side? Have you connected it to pc with same results? Has anyone also had this problem?
```

---
## \#800 Posted by: scepterr Posted at: 2018-03-21T06:26:08.464Z Reads: 413

```
Only the ESCapes come with R1 populated as far as I'm aware all other vesc4/6 don't

I first troubleshooted the issue by cutting the 5V line on one of my USB cables and it went away then I removed R1 and can use any cable now, ESCapes no longer connected to 5V usb
```

---
## \#801 Posted by: webst Posted at: 2018-03-21T06:30:44.602Z Reads: 416

```
I guess custom cable is easiest option, you can just block two middle pins with some tape on pc side
```

---
## \#802 Posted by: scepterr Posted at: 2018-03-21T06:34:21.047Z Reads: 432

```
It's really dead simple to take that resistor off, its not surrounded by components, just put a blob of solder on iron tip, apply to resistor and lift, resistor gone
![Screenshot_20180321-023344__01|499x500](upload://kDScPDeUcnJA847bTmdCKQO9CJC.jpg)
```

---
## \#803 Posted by: webst Posted at: 2018-03-21T06:40:12.600Z Reads: 424

```
And that’s how we went from too risky to dead simple. I like it :slight_smile:
```

---
## \#804 Posted by: scepterr Posted at: 2018-03-21T06:45:07.453Z Reads: 435

```
My babies all setup 😍
![IMG_20180321_024344|666x499](upload://oO2OoaXt7loLwA4nwADZRq9hHKx.jpg)
https://youtu.be/Q2HLkSGuEBY
```

---
## \#805 Posted by: Silverline Posted at: 2018-03-21T09:34:32.560Z Reads: 428

```
Look what showed Up today :slight_smile:
![IMG_20180321_103012|690x388](upload://rBJkE6p54E2K4wB7KWOXC9fvHe4.jpg)
```

---
## \#806 Posted by: AndyBigD Posted at: 2018-03-21T09:36:39.102Z Reads: 432

```
[quote="stewii, post:600, topic:37579"]
2.Might have to change the design because apparently Frank owns the IP of almost all the possible design variations and emailed (threaten) me about this.
[/quote]

Hey @stewii,

If you do have to change the design and want any modelling help or just some ideas and/or options, I'd be glad to help out if you need/want it...
I have already looked at an option or two as I was originally thinking of getting just the controller and making my own case (have access to CNC machines and a decent 3D Printer at work).

Hows this for an option (more FOCBOX style)?:
- Rather than an Aluminium enclosure with PCB cover, have an Aluminium baseplate/heatsink with a plastic enclosure.
- Smaller block of Aluminium and less machining required - should be cheaper.
- Plastic enclosure could be 3D Printed for prototyping, potentially injection molded if going to China with a large enough batch size?
- Silicone (or even 3D Printed TPU) cable gromets would be easy to integrate.

![image|690x397](upload://hcihctzojoulrpLOMp5gTlBlLGa.png)

![image|411x500](upload://cvQX52Mx2HsKVpY39eOAcRvnIgB.png)
```

---
## \#807 Posted by: Cobber Posted at: 2018-03-21T09:57:49.235Z Reads: 419

```
so jelly dude!

https://youtu.be/ym1yBIVfBtM
```

---
## \#808 Posted by: scepterr Posted at: 2018-03-21T10:12:29.523Z Reads: 420

```
First roll on dual ESCape 11S 😍
https://youtu.be/Y1Rlk1HEVZU
```

---
## \#809 Posted by: AndyBigD Posted at: 2018-03-21T10:23:58.506Z Reads: 426

```
Another option I was thinking I could try with 3D Pinted TPU, but would ideally be done with molded silicone...

- Even more compact Aluminium baseplate/heatsink
- Flexible enclosure/cover slips over baseplate/heatsink, retained by undercut on plate and lip on cover
- No fasteners needed (apart from 2 to hold down PCB
- Smaller footprint
- With the cover being flexible, wires could just be poked through during assembly.

![image|690x383](upload://d8q9OHoxPfGUawzBEG9R23nGKsp.png)

![image|432x500](upload://yiNTOg70yBsgOhOYI6bW1Rsiz8J.png)

![image|690x370](upload://rwEg90xKMeTNcAY0z1lOOIFzs8M.png)

I can keep the ideas coming @stewii, just let me know your thoughts or if you've got it all sorted.
I just want to help ensure this product remains available for all of us!
```

---
## \#810 Posted by: Surfer Posted at: 2018-03-21T10:40:55.838Z Reads: 404

```
Yeah!! keep your ideas coming, they are really good!
```

---
## \#811 Posted by: stewii Posted at: 2018-03-21T11:37:23.289Z Reads: 401

```
Wow amazing work! 
I still need to digest all this info.
```

---
## \#812 Posted by: stewii Posted at: 2018-03-21T11:40:09.699Z Reads: 401

```
I no longer populate R1. Again I have never encountered any issue, but I guess that depends on the PC/laptop.
```

---
## \#813 Posted by: uigiroux Posted at: 2018-03-21T12:24:11.442Z Reads: 400

```
Those enclosures you came up with look fantastic!
```

---
## \#814 Posted by: webst Posted at: 2018-03-21T12:26:03.615Z Reads: 399

```
Cables are too stiff to put through holes like this. I think that slots should be better. Also most rounded aluminium edges in your project means more cnc work. Nevertheless great job!
```

---
## \#815 Posted by: ducktaperules Posted at: 2018-03-21T12:45:05.163Z Reads: 401

```
i like this idea as an added extra level of splash protection is never a bad thing

EDIT : carfeull tho there might be existing IP around this http://www.trampaboards.com/vesc-6-external-splash-proof-silicone-seal-for-cnc-heat-sink-box-p-24845.html
```

---
## \#816 Posted by: baxter Posted at: 2018-03-21T12:48:51.300Z Reads: 398

```
Its a shame that the apparent solution to this problem is aesthetics! That being said, it appears to be a solution which its appealing, if somewhat unwarranted.
```

---
## \#817 Posted by: Riako Posted at: 2018-03-21T14:46:39.082Z Reads: 394

```
I love your last design ! Almost let me forgot the dual enclosure, but a mix of this and the @LukePL dual looks like an evidence !
So many good idea there ! Keep going :+1:
```

---
## \#818 Posted by: uigiroux Posted at: 2018-03-21T15:20:41.122Z Reads: 407

```
@stewii if you do decide to change your enclosure, I like this one the most.  Regardless, I'll buy them anyway you choose, you could put it in between two slices of bread and I'll be happy, lol.  :wink:

 ![Screenshot_20180321-102109|690x387](upload://2ohAUA4c0a2CERNl5LEM3b0fiAR.jpg)
```

---
## \#819 Posted by: moon Posted at: 2018-03-21T16:06:35.808Z Reads: 396

```
I prefer the other one, fight me
```

---
## \#820 Posted by: uigiroux Posted at: 2018-03-21T16:08:12.114Z Reads: 391

```
Haha, challenge accepted!
```

---
## \#821 Posted by: Mikenopolis Posted at: 2018-03-21T16:34:15.678Z Reads: 402

```
[quote="stewii, post:600, topic:37579"]
Might have to change the design
[/quote]

if this happens, how hard would it be to move things around and get the phase wires to be in the center for us OCD people? would that be enough change to bypass the BS...I mean IP issue
```

---
## \#822 Posted by: webst Posted at: 2018-03-21T16:38:13.510Z Reads: 397

```
1. There is no IP BS issue. 
2. Pretty hard and pointless work if you ask me. How frequently do you see it?
```

---
## \#823 Posted by: Mikenopolis Posted at: 2018-03-21T16:47:29.192Z Reads: 414

```
1.) the BS is Frank being an ass hat. If Ben actually was the one talking, it would be a different story.

2.) like I said, OCD. I see every annoyance of all things all the time. The following image is an example of something that drives me nuts. It's a personal problem.
![new-light-switch-final|666x500](upload://1785pzQRdozaNMo10Q7Hd9wgyEw.jpg)
```

---
## \#824 Posted by: Deckoz Posted at: 2018-03-21T16:53:20.064Z Reads: 408

```
Throw it in an Enclosure and make the wires come out of the center of the enclosure. Problem solved. ;)

Can't complain about something you only see while assembling.
```

---
## \#825 Posted by: webst Posted at: 2018-03-21T16:54:20.008Z Reads: 403

```
Or reroute [this](https://vesc-project.com/sites/default/files/Benjamin%20Posts/VESC_6.pdf) thing any way you want  :slight_smile:
```

---
## \#826 Posted by: Cobber Posted at: 2018-03-21T16:56:19.978Z Reads: 392

```
there is no IP issue
```

---
## \#827 Posted by: Mikenopolis Posted at: 2018-03-21T16:57:33.035Z Reads: 393

```
I actually solder on longer wires to one focbox because when I angle the existing ones it "shortens" the end when it comes out of the enclosure and the left and right isn't even.

Anyway. I asked if the change was possible just because IF he had to change the design, I thought that was something that could be done.
```

---
## \#828 Posted by: Mikenopolis Posted at: 2018-03-21T17:03:15.135Z Reads: 393

```
[quote="webst, post:825, topic:37579"]
Or reroute this thing any way you want  :slight_smile:
[/quote]

If I was to make that it's would be a vesc the size of a desk!

Sorry getting way off topic
```

---
## \#829 Posted by: LukePL Posted at: 2018-03-21T17:10:37.836Z Reads: 394

```
Ok Guys this is very nice looking design but to be so pretty in real life it requires a mold for plastic injection that cost a lot and you would have to lie to the factory about amount of parts because when they would hear even 300pcs it would be nothing for them. Probably you could find a lowest quality maker in China that would do for what? 2-3k$? But for the scale of sales it's not worth those money. Would it boost sales if at the same time have to be more expensive? The cheapest way would be 3D print but in cheap version is going to be terrible and better ones expensive. Even the worst 3D print is more expensive that PCB cover that is now in the use. There could be some savings on heat sink part but mostly on material because main part for milling is still there.  Frank achieved here what he wanted. Change the design to produce it more expensive. 
In the en of the day we will throw it into enclosure and not see so often.
```

---
## \#830 Posted by: Cobber Posted at: 2018-03-21T17:17:33.702Z Reads: 392

```
waasss up dude?
no enclosure?

stand alone price, i liked your work :money_mouth_face:
```

---
## \#831 Posted by: uigiroux Posted at: 2018-03-21T17:25:08.302Z Reads: 399

```
Frank didn't achieve that.  It was pretty much proven he was lying about everything and you could continue to sell the ESCape with the same enclosure and PCB as before and he can't do shit.  Nothing needs to change.  Also like I said earlier, you could just see say the HW and then separately we could buy the enclosure and PCB from others and he could hardly try and enforce anything there.  As was made clear, he wasn't saying the HW 6 was a problem.  And buying a piece of milled aluminum from someone else, well there's certainly nothing he could do with that in its own, and the same with the PCB.  Regardless of what you decide to do.  Definitely do what you want to do, not what you are going to do to try and shut that douche up..
```

---
## \#832 Posted by: LukePL Posted at: 2018-03-21T17:32:19.250Z Reads: 405

```
@Cobber who me? :) working on the dual but I have hard time to get my hands on CNC :( Maybe during weekend a prototype will be born ;)

@uigiroux yes I know that. I can mill the part I want :)
```

---
## \#833 Posted by: pixelsilva Posted at: 2018-03-21T22:30:22.279Z Reads: 411

```
> @Silverline 
> 
> Look what showed Up today :slightly_smiling_face:
> ![image|690x388](upload://sQiaxUshjPooUAWaySnWbacslRF.jpg)

Very subliminal by the way. (Red X) :sunglasses:
```

---
## \#834 Posted by: uigiroux Posted at: 2018-03-21T22:52:25.525Z Reads: 409

```
Haha that's great!
```

---
## \#835 Posted by: L3chef Posted at: 2018-03-22T12:08:36.452Z Reads: 401

```
Choose your weapon
```

---
## \#836 Posted by: pixelsilva Posted at: 2018-03-23T07:47:57.693Z Reads: 396

```
Bullet's in the chamber, hammer is mounted, and your finger playing with the trigger.
```

---
## \#837 Posted by: ArnhemAnt Posted at: 2018-03-23T07:58:24.043Z Reads: 397

```
I'm interested, what is the issue with the image you showed us?Is it that the screws don't all 'line up'? That's what annoys me about that image..............
```

---
## \#838 Posted by: scepterr Posted at: 2018-03-23T08:00:04.966Z Reads: 393

```
Lol I'm guessing it's the 1 regular switch followed by the 2 dimmer switches, instead of dimmer, regular, dimmer or all dimmer or all regular 😋
```

---
## \#839 Posted by: webst Posted at: 2018-03-23T09:04:01.806Z Reads: 389

```
Is this "ESCape from reality", forum for drug users that cannot handle daily irregularities and imperfections of real world? Well, then nice too meet you gentlemen! What's for dinner? :smiley:
```

---
## \#840 Posted by: telnoi Posted at: 2018-03-23T09:29:40.522Z Reads: 391

```
It would just call it/rebrand the ESCape to NoBox...and still make it rectangular in shape/keep the original design.
```

---
## \#841 Posted by: lazerusrm Posted at: 2018-03-23T09:54:42.121Z Reads: 392

```
Posted this in the wrong section.
```

---
## \#842 Posted by: Cobber Posted at: 2018-03-23T10:15:55.798Z Reads: 402

```
Keep this in the other topic dude, vesc has been a community OS project for years, lots of people have put lots of time and testing in to vedders OS baby, so passion runs deep and to some it is personal.
This topic is for @stewii to share his development of his HW 6.4 esc

and the following topic is to discuss such questions as you possed...

http://www.electric-skateboard.builders/t/the-legitimacy-of-a-trademark-on-an-opensource-design/49671?u=cobber
```

---
## \#843 Posted by: Acido Posted at: 2018-03-23T10:47:30.550Z Reads: 394

```
I burned my motherboard while applying throttle on my pc
Do not do anything than motor detections while your connected IMO
```

---
## \#844 Posted by: Manu39 Posted at: 2018-03-23T13:04:04.492Z Reads: 390

```
ha shit ... 🤬with the arrows of the keyboard or with the telco ... because for the arrow of the keyboard there is indeed an icon on the right on VESC tools to activate or not the arrows...
and what does IMO mean ....:relaxed::relaxed:
```

---
## \#845 Posted by: webst Posted at: 2018-03-23T13:22:58.964Z Reads: 391

```
http://www.smart-words.org/abbreviations/text.html
```

---
## \#846 Posted by: Acido Posted at: 2018-03-23T13:25:37.900Z Reads: 392

```
In my oppinion
Moving the motor by keys or remote
Probably a spike of power comes thru the usb port somehow and can do damage
Just plug it out and then do tests
```

---
## \#847 Posted by: Manu39 Posted at: 2018-03-23T13:28:03.402Z Reads: 399

```
Yes thanks @webst
```

---
## \#848 Posted by: Manu39 Posted at: 2018-03-23T18:34:03.556Z Reads: 400

```
@Acido : the motherboard burned when you had already made your engine detection or after setting through the Input Configuration Wizard ...
```

---
## \#849 Posted by: Silverline Posted at: 2018-03-23T19:14:59.284Z Reads: 399

```
So remove R1, we must 🤔
```

---
## \#850 Posted by: Kug3lis Posted at: 2018-03-23T19:43:50.542Z Reads: 406

```
It's like common practice when you work with MCU, and it has separate power supply, so you only use data lines and ground or if it relates high voltage even simple USB isolation chip to complete isolate your computer from device. I have experienced several burnt motherboard because of it even apple ones ;)
```

---
## \#851 Posted by: webst Posted at: 2018-03-27T10:52:41.050Z Reads: 393

```
Do you advise disconnecting USB power lines when operating from battery?
```

---
## \#852 Posted by: koralle Posted at: 2018-03-27T11:38:31.572Z Reads: 397

```
![de für_ usb isolator|421x241](upload://dediST1q8178yG8nCRkvF9CduAc.png)

Not cheap for such a small piece of china pcb
```

---
## \#853 Posted by: Kug3lis Posted at: 2018-03-27T11:46:06.255Z Reads: 398

```
Yeah, cause those have Power also isolated, as you don't need power on those devices you just need to isolate signals.
```

---
## \#854 Posted by: banjaxxed Posted at: 2018-03-27T12:29:16.125Z Reads: 405

```
That looks to be a complete BS price yeah, on phone eBay 10seconds beat
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F273008451559
```

---
## \#855 Posted by: Nordle Posted at: 2018-03-27T12:40:56.616Z Reads: 396

```
Or just cut the 5v wire from your usb wires
cost.. 0$
```

---
## \#856 Posted by: Kug3lis Posted at: 2018-03-27T12:42:38.942Z Reads: 391

```
and then for e.g. 48V comes up you are D+/D- lines because your regulator fucked up :D
```

---
## \#857 Posted by: webst Posted at: 2018-03-27T12:42:55.359Z Reads: 390

```
That was what I was asking for. Should I leave the ground intact?
```

---
## \#858 Posted by: Kug3lis Posted at: 2018-03-27T12:43:25.645Z Reads: 393

```
Yeah, ground and data pins is enough if device is self powered ;) and does not have USB detect logic
```

---
## \#859 Posted by: Nordle Posted at: 2018-03-27T12:43:50.196Z Reads: 398

```
Yes.

That would result in the same as removing r0, cause it‘s 0ohm, its just a bridge, an option
```

---
## \#860 Posted by: webst Posted at: 2018-03-27T12:56:16.887Z Reads: 403

```
I guess it's easier to batch program it with no motor connected when it's there. I mean when you have to program 100 vescs with same config.
```

---
## \#861 Posted by: stewii Posted at: 2018-03-27T17:58:49.358Z Reads: 404

```
So much overreacting about this.
There isnt overvoltage on the 5V rail.  
PC motherboards should handle over current on the USB, just like if you short it.
Latest ESCapes come without R0.
No way you can get 48V over D+/D- .


Will stop making these myself. So if you want to grab one check out here: http://www.electric-skateboard.builders/t/escape-group-buy-professional-pcb-assembly/49720
```

---
## \#862 Posted by: Kug3lis Posted at: 2018-03-27T18:08:30.040Z Reads: 399

```
Try put 12V on usb :) tell me later how your motherboard handled it ;)
```

---
## \#863 Posted by: b264 Posted at: 2018-03-27T18:13:10.865Z Reads: 410

```
[quote="Kug3lis, post:862, topic:37579"]
Try put 12V on usb :slight_smile: tell me later how your motherboard handled it
[/quote]

Why waste time?  Just go [straight for the heart](https://usbkill.com/products/usb-killer-v3?variant=44776085642) the first time.
```

---
## \#864 Posted by: stewii Posted at: 2018-03-27T18:21:03.794Z Reads: 398

```
Why would you have 12V on the 5V ESC rail? 
And I said overcurrent not overvoltage :)
```

---
## \#865 Posted by: JohnnyMeduse Posted at: 2018-03-27T18:33:23.677Z Reads: 396

```
Well... If the Ground on the DRV is badly solder you can get 8V or more on the 5V circuit, Also any defective part could create unique problem over the 5V
```

---
## \#866 Posted by: stewii Posted at: 2018-03-27T19:03:24.955Z Reads: 396

```
It is pointless to play what if games. 
If you have 8V on the 5v rail then your ESC wouldnt work for sure. Why connecting it to a PC?
```

---
## \#867 Posted by: JohnnyMeduse Posted at: 2018-03-27T19:07:55.613Z Reads: 397

```
Well... I’ve repaire over a few hundred of ESC, so I’m just a dumb shit who don’t know what he is doing 😉. If you want to close your eye on a known issue that up to you man.
```

---
## \#868 Posted by: stewii Posted at: 2018-03-27T19:15:04.560Z Reads: 383

```
Who said you are a dumb shit? 
What known issue? I am not populating R0 no more, my ESC have R0, never had an issue. 
Nothing to see here, move on.
```

---
## \#869 Posted by: bigben Posted at: 2018-03-28T22:15:44.300Z Reads: 375

```
Just plugged in my 2 new ESCapes and ran motor detection.
All good, worked exactly as expected. So excited to get them up and running on the mountain board, or should I use them on the Tesseract? Decisions decisions.
```

---
## \#870 Posted by: trancejunkiexxl Posted at: 2018-03-28T23:24:23.160Z Reads: 379

```
imho tesseract.. then again you can always just move em around :smiley:
```

---
## \#871 Posted by: Schulerbible Posted at: 2018-03-28T23:33:37.113Z Reads: 380

```
How much did you pay for the two? I'm too lazy going thru the whole thread ... *sorry*
```

---
## \#872 Posted by: pixelsilva Posted at: 2018-03-28T23:42:21.398Z Reads: 376

```
No man, the ESCapes are @Silverline 's
```

---
## \#873 Posted by: fraannk Posted at: 2018-03-29T03:27:18.897Z Reads: 385

```
Nothing would happen if I put 12V on the USB line...... My computer would just think it had a charger attached! #usbcmasterrace

and also, I've put more than 12V on USB... nothing happened...
```

---
## \#874 Posted by: bimmer Posted at: 2018-03-29T03:32:23.860Z Reads: 378

```
Saaame
10 char
```

---
## \#875 Posted by: Schulerbible Posted at: 2018-03-29T04:32:53.720Z Reads: 379

```
Uups sorry, wrong person :slight_smile:
```

---
## \#876 Posted by: H_man Posted at: 2018-03-30T11:59:43.921Z Reads: 386

```
Hi, is there anyone that would have these 2 components spare on hand they wouldn't mind shipping to New Zealand. I don't mind paying a little extra on top of the cost plus shipping, these components are out of stock and will become available near the end of the year I'm just too impatient. 

Components:
1 * LQM21PN2R2MGHL
1 * PMEG6020ER,115

Thanks
```

---
## \#877 Posted by: Kug3lis Posted at: 2018-03-30T12:04:24.093Z Reads: 385

```
LQM21PN2R2MGHL is 2.2uH inductor in 0806 package ~1.3A

https://www.digikey.co.uk/products/en/inductors-coils-chokes/fixed-inductors/71?k=&pkeyword=&FV=400006%2Cmu2.2%C2%B5H%7C2087%2Cffe00047%2Cmu1.3A%7C2088%2Cmu1.4A%7C2088%2Cmu1.5A%7C2088&quantity=0&ColumnSort=0&page=1&stock=1&pageSize=25

PMEG6020ER,115 is Schottky diode min 60V min 2A and SOD-123W package

https://www.digikey.co.uk/products/en/discrete-semiconductor-products/diodes-rectifiers-single/280?k=&pkeyword=&umin2071=60&rfu2071=V&pv914=19&pv914=18&FV=ffe00118%2C4034bf%2C1800018&quantity=0&ColumnSort=0&page=1&pageSize=25
```

---
## \#878 Posted by: bimmer Posted at: 2018-03-30T14:22:51.622Z Reads: 383

```
I'll check my spare parts box when I'm home.
```

---
## \#879 Posted by: H_man Posted at: 2018-03-31T02:21:13.649Z Reads: 386

```
Thanks, @brimmer. appreciate it!
```

---
## \#880 Posted by: H_man Posted at: 2018-03-31T02:48:30.540Z Reads: 397

```
Hi @Kug3lis I'm really bad with electronics forgive my questions, If i get a 60V 3A instead of a 60V 2A Schottky diode would that still work?? 

For example:
https://nz.mouser.com/ProductDetail/ON-Semiconductor-Fairchild/SS36FA?qs=%2fha2pyFadugJwW%252bgHSbajooq73VofB2m0AKhC5xQKuM%3d

Thanks.
```

---
## \#881 Posted by: b264 Posted at: 2018-03-31T05:58:00.579Z Reads: 403

```
It should work, yeah
```

---
## \#882 Posted by: Toglia Posted at: 2018-04-06T02:44:17.610Z Reads: 386

```
Where can I purchase a pair of these? Btw this is mindblowing!
```

---
## \#883 Posted by: Toglia Posted at: 2018-04-06T02:45:44.283Z Reads: 385

```
Where can I purchase a pair of these? And where can I see the specs? Would be nice if they where 300A :)
```

---
## \#884 Posted by: Colson003 Posted at: 2018-04-06T02:49:18.400Z Reads: 387

```
@Toglia

 http://www.electric-skateboard.builders/t/escape-group-buy-professional-pcb-assembly/49720/71
```

---
## \#885 Posted by: Toglia Posted at: 2018-04-06T04:46:00.240Z Reads: 383

```
Sorry that Im so late but can I ask what is the peak amps and how kuch the continuous? Thank you
```

---
## \#886 Posted by: Cobber Posted at: 2018-04-06T04:59:35.341Z Reads: 384

```
as stewii's ESCape is based on the open source hardware software VESC 6.4, it shares similar ampacity.

Try using "search" with terms like "vesc 6"
```

---
## \#887 Posted by: Minim Posted at: 2018-04-06T15:51:13.324Z Reads: 372

```
I replied to your payment email but I didn’t get any response @stewii . Can I buy it without the alu housing? What would the amount be to transfer if so?
```

---
## \#888 Posted by: stewii Posted at: 2018-04-06T16:49:23.214Z Reads: 380

```
You can, just order as normal, on the comments say you don't want housing, then on the final payment it is going to be  £10 cheaper per ESC.
```

---
## \#889 Posted by: Minim Posted at: 2018-04-06T17:17:35.549Z Reads: 386

```
Good. I sent the payment now for two units but I’ve never used TransferWise before. Do you send some kind of confirmation to oldies like me so I don’t miss the deadline if I did smt wrong.
```

---
## \#890 Posted by: Pimousse Posted at: 2018-04-12T16:20:23.797Z Reads: 392

```
Hi @stewii,
With @Manu39, we're trying to troubleshoot a serial communication issue.
I made a PCB with an arduino and a LED gauge communicating through UART.
Mine is working flawlessly with a VESC 6, FW3.37. I tested his gauge board with a VESC 4.12, no problem.
However, with the ESCape, the communication is established only when he's accelerating.
In idle, the Tx LED of the Arduino blinks but not the Rx one.
We checked parameters together, AFAIK everything is set up correctly.
So I'm stucked.

Any throughts ?
Thanks !
```

---
## \#891 Posted by: stewii Posted at: 2018-04-12T18:23:59.995Z Reads: 376

```
weird, bluetooth works fine though through uart. Can you DM with info about that arduino PCB?
```

---
## \#892 Posted by: Pimousse Posted at: 2018-04-12T20:17:16.199Z Reads: 377

```
This an Arduino nano communicating through uart (voltage divider on arduino Tx) abd display battery gauge on a WS2812 ring, plus button and luminosity sensor Arduino side.
@Manu39 tried to supply the Arduino through VESC 5V and by an UBEC on the main battery.
```

---
## \#893 Posted by: webst Posted at: 2018-04-12T20:24:58.701Z Reads: 388

```
I have similar problem with @rpasichnyk Perimetr app and bluetooth module. There is communication error and following message, possibly connected to @Pimousse case.
![image|690x318](upload://dtdkukEKmptmEIC4ovPn2PtMTKa.jpeg)

Vesc tool shows that software version is in fact 3.37.

Edit: I'm going to swap TX with RX and see if it helps.
Edit 2: It didn't
```

---
## \#894 Posted by: Minim Posted at: 2018-04-12T20:26:31.538Z Reads: 378

```
what blouetooth module are you using so I can order one I know is working for when mine gets here :D
```

---
## \#895 Posted by: stewii Posted at: 2018-04-12T23:42:42.793Z Reads: 399

```
I just tried with to connect an arduino nano I got here and Rx blinks and all works normal. I can try to replicate what you trying to do if you tell me what arduino program you have there.

[quote="Pimousse, post:892, topic:37579, full:true"]
This an Arduino nano communicating through uart (voltage divider on arduino Tx) abd display battery gauge on a WS2812 ring, plus button and luminosity sensor Arduino side.
@Manu39 tried to supply the Arduino through VESC 5V and by an UBEC on the main battery.
[/quote]



Can you take a pic of the connections on vesc and bluetooth module sides?


[quote="webst, post:893, topic:37579, full:true"]
I have similar problem with @rpasichnyk Perimetr app and bluetooth module. There is communication error and following message, possibly connected to @Pimousse case.
![image|690x318](upload://dtdkukEKmptmEIC4ovPn2PtMTKa.jpeg)

Vesc tool shows that software version is in fact 3.37.

Edit: I'm going to swap TX with RX and see if it helps.
Edit 2: It didn't
[/quote]


[quote="Minim, post:894, topic:37579, full:true"]
what blouetooth module are you using so I can order one I know is working for when mine gets here :D
[/quote]

I have a HM-10 and a NRF51822 both work perfectly.
```

---
## \#896 Posted by: Devilmycry Posted at: 2018-04-13T03:28:54.624Z Reads: 367

```
Hi everything 
I want to know 
For the escape can I make 100000 erpm and can I go to 80a each motor 
Thank you
```

---
## \#897 Posted by: Pimousse Posted at: 2018-04-13T04:14:23.704Z Reads: 377

```
@stewii, I have a pair of ESCape, I'll test with them.
```

---
## \#898 Posted by: Manu39 Posted at: 2018-04-13T06:24:41.318Z Reads: 386

```
hello @stewii , as I said @Pimousse  have the led fixed Rx: led lightly on...and the Tx LED is blinking.
the Rx will start blinking when I'm zooming in and the Tx stops blinking.
a pict  of the connections the escape and the arduino
![image|666x500](upload://mb6AsTOYTN5cdQZ18fe7sDZQuqb.jpeg)
it's the same thing on the slave and the master ...
```

---
## \#899 Posted by: rickyd Posted at: 2018-04-13T07:16:01.855Z Reads: 377

```
Are the Arduino and the ESCape on common ground?
```

---
## \#900 Posted by: Pimousse Posted at: 2018-04-13T08:31:56.472Z Reads: 371

```
Yes. The PCB is powered by the 5V and GND from the CANbus JST.
```

---
## \#901 Posted by: stewii Posted at: 2018-04-13T08:34:30.609Z Reads: 370

```
I dont use a voltage divider because most IO pins on the STM are 5V tolerant. Where can I get that PCB?
```

---
## \#902 Posted by: Pimousse Posted at: 2018-04-13T09:33:49.688Z Reads: 378

```
Well, I'll tell @Manu39 to try bypassing the voltage divider.

[quote="stewii, post:901, topic:37579"]
Where can I get that PCB?
[/quote]
That was only a small batch for french guys.
I need to sort PCB design (like this one) issues before going further.
```

---
## \#903 Posted by: webst Posted at: 2018-04-13T12:52:54.305Z Reads: 390

```
Are there any HW/SW differences between V6 and Escape that might cause Metr module to not recognize it’s proper software version?
Cable connection seems to be ok. Module is visible in app but cannot establish communication due to allegedly unsupported SW version, this looks like communication is after all working properly but doesn’t get proper firmware information back. 
![image|666x500](upload://mHVw4jXtAKMtORmZRdmmcmoDSAt.jpeg)
```

---
## \#904 Posted by: Manu39 Posted at: 2018-04-13T13:55:00.407Z Reads: 382

```
Strange with an HM-10 (aliexpress) and @emmaanuel  eskate apps the module is recognized and connect immediately ... i also ordered a module metr.at i will not fail to make a return on the problems or not...
did you set baudrate on 115200 bps  in VESC TOOLS?
```

---
## \#905 Posted by: stewii Posted at: 2018-04-13T13:57:36.115Z Reads: 378

```
No, there isn't differences. What kind of module is that used for metr.at? I dont have one. looks like an HM10. Is the ESC correctly configured? Are you on firmware 3.37? Why metr doesnt work with older firmwares?
```

---
## \#906 Posted by: webst Posted at: 2018-04-13T14:19:23.880Z Reads: 386

```
I don't really know, it works with hw 4.2 as well as with vesc 6. Esc is configured according to instructions at (https://metr.at/setup). I'll check one more time tonight and let you know, hopefully I managed to misclick something and it'll work.

@Manu39 I believe I did set everything right at least three times in a row :slight_smile: I'd appreciate if you check if yours work properly.

Edit: I started to believe I had missed something even though I checked it 3 times yesterday. Well, I checked everything one more time, it was all as it should be so I open Perimetr and of course it finds module in a blink of an eye. The only thing that changed is that I connected PPM remote (for the first time) before running Perimetr but I guess it's nothing to do with it. I don't know what happened but I strongly suspect that I missed something and lack of experience doesn't allow me to realize what. Thanks for suggestions!
```

---
## \#907 Posted by: Jobbel Posted at: 2018-04-15T16:28:08.231Z Reads: 385

```
After several weeks of use I am now running into an Issue with the ESCape
if i accelerate or break hard an OVER VOLTAGE fault occurs:

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -134.7
Current filtered : -30.2
Voltage          : 59.60
Duty             : 0.917
RPM              : 46392.3
Tacho            : 3489
Cycles running   : 4054
TIM duty         : 4259
TIM val samp     : 2081
TIM current samp : 4405
TIM top          : 4647
Comm step        : 3
Temperature      : 83.41


The Voltage value is not true. The most notable thing is, it does not happen if I connect the ESC to a Computer over USB. Because my R1 is still in place i thought that maybe the DC-DC converter is the source of the problem. I also found out that the Arduino connected to the 5V pin of the vesc performs a reset every time the fault happens.

btw I am using a 10s system.

It does not matter whether I use FOC or BLDC.
Maybe some noise or drops on the 5v are messing with the ADC of the STM 
Help would be appreciated
```

---
## \#908 Posted by: Exiledd_Top Posted at: 2018-04-15T16:31:28.385Z Reads: 369

```
Check your battery inspect it maybe a cable is loose. Also are you encounter this problem only at full charge or random because u could be regening to much at full battery causing vesc to reboot
```

---
## \#909 Posted by: Jobbel Posted at: 2018-04-15T16:34:37.866Z Reads: 368

```
I am currently checking for a loose cable. It started occuring with a battery at 50% i have not yet charged the battery since then
```

---
## \#910 Posted by: TarzanHBK Posted at: 2018-04-15T16:37:40.285Z Reads: 366

```
Looks like an extremly high braking current.
So maybe check on your motor too, to make sure the windings are not shorting.
```

---
## \#911 Posted by: Jobbel Posted at: 2018-04-15T16:42:35.882Z Reads: 366

```
As soon as I connect it to the computer the measured currents are no where near the stated above, that's why it does not run into a fault if the 5V line is stable.
I dont belive that a breaking current this high is true.

I just soldered the vesc directly to the battery without a switch and the error persists
```

---
## \#912 Posted by: stewii Posted at: 2018-04-15T16:56:17.049Z Reads: 356

```
That is the reg braking. It charges the battery , and  with -134 A the voltage goes too high and throws a fault code. That’s normal. Can you put here your motor settings.
```

---
## \#913 Posted by: Jobbel Posted at: 2018-04-15T16:57:16.112Z Reads: 368

```
![sasdasd|690x260](upload://5NEASfTmAdfL5GEPhfzs4NGXq2P.PNG)
```

---
## \#914 Posted by: Jobbel Posted at: 2018-04-15T16:57:57.568Z Reads: 378

```
It does also happen if i accelerate hard so breaking is not the only source for the issue
```

---
## \#915 Posted by: JohnnyMeduse Posted at: 2018-04-15T17:20:36.189Z Reads: 392

```
Can you check to see if those capacitor are still properly solder. 

![image|375x500](upload://dfwij8Gt3eMg1COgCkwSekw37JQ.jpg)
```

---
## \#916 Posted by: Silverline Posted at: 2018-04-15T17:32:11.367Z Reads: 383

```
Do you run single or dual setup ? If dual, is it both Escapes then ??
```

---
## \#917 Posted by: Pedrodemio Posted at: 2018-04-15T20:26:43.192Z Reads: 373

```
metr only works with the modules @rpasichnyk sell. Even if they are HM10, the app checks the MAC address
```

---
## \#918 Posted by: Eboosted Posted at: 2018-04-15T20:33:39.709Z Reads: 384

```
[quote="JohnnyMeduse, post:915, topic:37579, full:true"]
Can you check to see if those capacitor are still properly solder.
[/quote]

I had those broken on both of my escapes, I had to order new ones from Mouser but when I installed them back in, one escape did not turn on anymore, unfortunately I had to replace them with FocBoxes as they one is no longer working and shipping it back takes a lot of time.
```

---
## \#919 Posted by: Jobbel Posted at: 2018-04-15T20:53:43.998Z Reads: 401

```
![02(1)|375x500](upload://95OKQwn1tBBglHkzWGEBQrQHacY.jpeg)



Thanks a lot mr. Medusa wizard, apparently both contacts of one and one contact of the other capacitor managed to wiggle free.

I think after fixing it I'll add some silicon
```

---
## \#920 Posted by: banjaxxed Posted at: 2018-04-15T21:08:44.868Z Reads: 385

```
That is an impressive eye you have Sir
```

---
## \#921 Posted by: b264 Posted at: 2018-04-15T21:11:27.272Z Reads: 395

```
[quote="banjaxxed, post:920, topic:37579, full:true"]
That is an impressive eye you have Sir
[/quote]

I'm not sure if he saw the problem or deduced what it was likely to be from the symptoms.  That photo was of a different ESCape
```

---
## \#922 Posted by: JohnnyMeduse Posted at: 2018-04-15T21:26:26.544Z Reads: 402

```
[quote="banjaxxed, post:920, topic:37579, full:true"]
That is an impressive eye you have Sir
[/quote]

@Eboosted got the same problem a few weeks ago... I just have a good memory and these issues are prone to happen with a design like this one, especially in a high vibration environment.

[quote="b264, post:921, topic:37579"]
That photo was of a different ESCape
[/quote]

 True that a picture I took from above.
```

---
## \#923 Posted by: Deckoz Posted at: 2018-04-15T21:41:16.354Z Reads: 396

```
[quote="Jobbel, post:907, topic:37579"]
Voltage value is not true.
[/quote]

It probably is true... because your battery probably has a broken series connection....or you have a broke cap..
```

---
## \#924 Posted by: Eboosted Posted at: 2018-04-15T21:48:48.922Z Reads: 392

```
This is a design problem, @stewii is now using hot glue to avoid the cap legs from breaking.
```

---
## \#925 Posted by: b264 Posted at: 2018-04-15T21:51:39.360Z Reads: 383

```
If the caps stop pissing-off the gangsters down the street, maybe they won't keep having their legs broken.
```

---
## \#926 Posted by: Minim Posted at: 2018-04-15T21:54:28.232Z Reads: 385

```
Inboard had the same issue on their board with a heavy component in their board (“spole” in Norwegian.. don’t know the English word). I fixed it with resoldering and applied glue to it so it didn’t shake loose again. I think they also glue it in now ^^ Easy spot to miss before something breaks :)
```

---
## \#927 Posted by: Sebike Posted at: 2018-04-15T22:03:16.570Z Reads: 385

```
an inductor maybe?
```

---
## \#928 Posted by: Jobbel Posted at: 2018-04-16T00:17:27.993Z Reads: 381

```
I think I'll add an external Cap Board from a VESC 4.12 to the Escape and keep the 2 spots inside the aluminium housing empty.
This way it cannot happen again. I do not trust hotglue or silicon to be honest.
```

---
## \#929 Posted by: Minim Posted at: 2018-04-16T04:38:48.399Z Reads: 396

```
Keep the wires short then. The voltage spikes amplifies with cable lenght and the main reason for those caps is protecting the components from those spikes if I’m not mistaken.
```

---
## \#930 Posted by: GloStix Posted at: 2018-04-16T22:08:12.459Z Reads: 402

```
Exactly, prevents voltage sagging, but I prefer to install a short circuit preventor myself as any issues like a break in a capacitor line above if not discharged correctly will cause spike when re soldering.
```

---
## \#931 Posted by: Manu39 Posted at: 2018-04-18T18:46:07.487Z Reads: 407

```
I come back to my Smart Ring problem number 709 post and actually after shining the voltage divider bridge the smart ring works at the top. Thank you @Pimousse and @stewii for advice.
https://vimeo.com/265188386
```

---
## \#932 Posted by: Minim Posted at: 2018-04-18T18:59:21.047Z Reads: 395

```
I’m more concerned with the spikes than the sag. These small caps can’t prevent sag but they can even out the peak the esc pwm generates when going off. This is my understanding of it so it might be way off :D
```

---
## \#933 Posted by: rpasichnyk Posted at: 2018-04-18T19:59:39.212Z Reads: 393

```
@Manu39 @Pimousse where can I read more about Smart Ring? Very interesting stuff!
```

---
## \#934 Posted by: Manu39 Posted at: 2018-04-18T20:08:29.255Z Reads: 396

```
@pimousse is the creator of the SR, an intelligent gauge based ARDUINO that informs in real time and choice of battery percentage, speed or temperature of the engine (s).
here is the link of the project on the french forum:
[http://www.e-sk8.fr/forum/viewtopic.php?f=25&t=2731](http://www.e-sk8.fr/forum/viewtopic.php?f=25&t=2731)
```

---
## \#935 Posted by: Charles_Chan Posted at: 2018-04-19T15:30:12.251Z Reads: 394

```
For  nRF2.4 receiver on the PCB, Is it can meet all of the remote that sale on the market or just suitable for specify remote? thanks
```

---
## \#936 Posted by: GloStix Posted at: 2018-04-20T01:01:10.946Z Reads: 386

```
You are right Sir, I stand corrected. Too small size, see https://www.helifreak.com/showthread.php?t=435335
```

---
## \#937 Posted by: Manu39 Posted at: 2018-04-21T10:20:21.711Z Reads: 392

```
@webst: to receive Roman's Metr.at module. I made it plugged and set up as explained by Roman. at first it did not work on my iphon but worked on my ipad .... actually on my iphone CanFwd was ON ... and not on ipad. so I put on OFF and the miracle works ...
I am in double motor 130 kV / double ESCAPE / Lipo 12s 12A.
```

---
## \#938 Posted by: Minim Posted at: 2018-04-21T18:53:43.872Z Reads: 385

```
are there a 3d model of these vesc? Waiting on my preorder but want to design a small dual case for them
```

---
## \#939 Posted by: Manu39 Posted at: 2018-04-23T13:23:54.228Z Reads: 407

```
little review of ESCape by stewii:
Saturday 21/04 the FORAKER finally ready to do its first turn of the wheel. I decided to make a night out of 12 km including 2 of mountain road ... no problem during these 12 kms except a disconnection of metr.at that does not allow me to detail more this first exit.
![image|666x500](upload://qLR9Wtnmi5u4MSuOfiKgmQUjiCP.jpeg)
```

---
## \#941 Posted by: b264 Posted at: 2018-04-23T19:06:09.219Z Reads: 401

```
[quote="Minim, post:938, topic:37579, full:true"]
are there a 3d model of these vesc? Waiting on my preorder but want to design a small dual case for them
[/quote]

They're not vesc.  They are based on VESC and compatible with VESC.  VESC is a trademarked name
```

---
## \#942 Posted by: Minim Posted at: 2018-04-23T19:19:49.939Z Reads: 395

```
Ok... Are there a 3d model of this VESC based VESC?
```

---
## \#943 Posted by: Manu39 Posted at: 2018-04-23T19:34:56.437Z Reads: 383

```
ESCape....
```

---
## \#944 Posted by: b264 Posted at: 2018-04-23T20:26:31.274Z Reads: 387

```
[quote="Minim, post:942, topic:37579"]
VESC based VESC
[/quote]

VESC-based ESC.  It's called ESCape.  The "V" is trademarked.
```

---
## \#945 Posted by: Minim Posted at: 2018-04-23T20:29:48.291Z Reads: 386

```
Wow did trampa trademark V™ now? From now on we have to use the TM mark ev™ery time we use the letter V™? He's on a strike!
```

---
## \#946 Posted by: MyCampGround Posted at: 2018-04-23T22:04:29.069Z Reads: 384

```
i now have everything officially purchased for my new build except @stewii two ESCapes! :smile:
```

---
## \#947 Posted by: MyCampGround Posted at: 2018-04-29T22:50:51.505Z Reads: 375

```
Does anyone know the dimensions of two of these side by side?
```

---
## \#948 Posted by: b264 Posted at: 2018-04-30T03:49:09.853Z Reads: 392

```
[quote="MyCampGround, post:947, topic:37579, full:true"]
Does anyone know the dimensions of two of these side by side?
[/quote]

Nope; I sure don't.  But two B-Box side-by-side should be very, very similar and are 140 x 77 x 21mm

The 140mm is hard

The other two will need extra space for wires and connectors.  Cheers
```

---
## \#949 Posted by: LukePL Posted at: 2018-04-30T09:13:04.724Z Reads: 406

```
![IMG_20180430_110955|666x500](upload://75ikUi2n8BOWUOS7K9Fy26DuVQA.jpg)
by 77x18 so yeah @b264 is correct ;)
```

---
## \#950 Posted by: SORRENTINO Posted at: 2018-04-30T15:55:14.541Z Reads: 395

```
The group buy with the dual case has not yet happened correct?
```

---
## \#951 Posted by: LukePL Posted at: 2018-04-30T19:24:04.307Z Reads: 388

```
It happen. Do you need it? ;)
```

---
## \#952 Posted by: SORRENTINO Posted at: 2018-04-30T19:44:55.514Z Reads: 388

```
The ESCape and case group buy?
```

---
## \#953 Posted by: SORRENTINO Posted at: 2018-04-30T19:45:47.394Z Reads: 391

```
I saw Stewi say something about a big group buy so he can get the escs manufactured instead of soldering by hand.
```

---
## \#954 Posted by: LukePL Posted at: 2018-04-30T19:47:05.853Z Reads: 405

```
http://www.electric-skateboard.builders/t/escape-group-buy-professional-pcb-assembly/49720
It;s all there. Singe and dual ;)
```

---
## \#955 Posted by: SORRENTINO Posted at: 2018-04-30T19:53:19.723Z Reads: 386

```
damn looks like i missed it :frowning:
```

---
## \#956 Posted by: webst Posted at: 2018-04-30T19:56:16.941Z Reads: 385

```
Is there anywhere 3d file of single or dual aluminium enclosure?
```

---
## \#957 Posted by: LukePL Posted at: 2018-04-30T21:14:25.364Z Reads: 382

```
Single is available somewhere in the beginning of this thread. Dual is not.
```

---
## \#958 Posted by: Minim Posted at: 2018-05-01T10:16:19.418Z Reads: 387

```
I will make a dual case for mine as soon as they arrive.. can make one more if you need it. I think @LukePL designes one so if he still makes them it might be quicker to ask him.
```

---
## \#959 Posted by: AndyBigD Posted at: 2018-05-01T11:31:32.023Z Reads: 387

```
Can anyone confirm what size bullet connectors these have on the phase wires?
```

---
## \#960 Posted by: webst Posted at: 2018-05-01T12:09:35.371Z Reads: 388

```
Thank you! I want to put some more input capacitance and anclose them in housing. Thanks to @LukePL I found single vesc 3d file so I’ll manage to start from here.
```

---
## \#961 Posted by: bigben Posted at: 2018-05-01T12:13:56.321Z Reads: 387

```
Mine came without bullets.
```

---
## \#963 Posted by: JayReyez Posted at: 2018-05-03T20:17:59.043Z Reads: 378

```
Hey @stewii, nice to see you! Check your pm and drop me a note. Thanks 
-J
```

---
## \#964 Posted by: mmaner Posted at: 2018-05-03T21:03:03.086Z Reads: 377

```
do the ESCapes use the same CAN bus cable as v4 VESC's, using only the 2 inside leads?
```

---
## \#965 Posted by: SammiHuang Posted at: 2018-05-15T09:08:21.906Z Reads: 372

```
looks nice.
```

---
## \#966 Posted by: Pimousse Posted at: 2018-05-15T09:13:10.979Z Reads: 372

```
Yes.
10 chars
```

---
## \#967 Posted by: webst Posted at: 2018-05-15T11:35:14.915Z Reads: 377

```
I couldn't properly setup sensored [TorqueBoards 6355](products/electric-skateboard-motor-6355-190kv) with Escape. Wire configuration is as stated on their site, don't know the reason. Has anyone had such a problem? Unsensored FOC is pretty good though, except for no standing start.
```

---
## \#968 Posted by: banjaxxed Posted at: 2018-05-15T11:56:04.828Z Reads: 396

```
Not sure is the pin out printed on the  Maybe like APS motors you have to switch the leads heres how
products/vesc-sensor-wires?variant=712409808919

Wire configuration:
Red = 5v
White = Temp
Blue = A
Yellow = C
Green = B
Black = GND
```

---
## \#969 Posted by: webst Posted at: 2018-05-15T12:06:45.866Z Reads: 389

```
Pin names are also printed on escape. I've seen this converter but it was too late so I just remade it by hand with new JST 2.0 connector, just like you're suggesting. I even tried to switch ACB cables thinking it would finally catch on. No success. I've read somewhere that some hall sensors' signal levels are lower than others and that might be the case here but I'd like someone to confirm.
```

---
## \#970 Posted by: banjaxxed Posted at: 2018-05-15T12:33:35.118Z Reads: 389

```
maybe try this to see if it's a hall problem
https://www.electric-skateboard.builders/t/unknown-hall-error-255/37058/14?u=banjaxxed
```

---
## \#971 Posted by: ElskerShadow Posted at: 2018-05-23T07:24:52.435Z Reads: 376

```
Guys when will we be able tu buy dual Escape with heatsink?
```

---
## \#972 Posted by: bigben Posted at: 2018-05-23T07:54:44.968Z Reads: 372

```
@LukePL is making them I believe?
```

---
## \#973 Posted by: Silverline Posted at: 2018-05-23T18:04:53.855Z Reads: 369

```
We are All waiting on the dual housing. I think @LukePL will tell when they are ready. Hopefully this week :-)
```

---
## \#974 Posted by: LukePL Posted at: 2018-05-23T18:21:45.204Z Reads: 368

```
Yeah guys I feel the pressure and I'm bombarding guys from anodizing every day....
```

---
## \#975 Posted by: Minim Posted at: 2018-05-23T21:17:39.091Z Reads: 362

```
Are there any do/don’t do with the vesc6? I’ve heard many said they killed 4.12 vescs with user error in the settings. Kinda want to avoid doing that :D
```

---
## \#976 Posted by: moon Posted at: 2018-05-23T21:19:48.313Z Reads: 363

```
Also looking for advice around this I want to be careful
```

---
## \#977 Posted by: Minim Posted at: 2018-05-25T22:38:27.604Z Reads: 363

```
Maybe @stewii has some inputs on how to not produce magic smoke? 😂
```

---
## \#978 Posted by: ron Posted at: 2018-05-26T17:48:58.818Z Reads: 364

```
Can someone scale down the pads a little bit on the Stencil File so when etching the stencils the holes arent etched too large in size!?.

I tried with 3 EDA Programs and I couldn't get it scaled down to lets say 90% or 95% regarding the PAD size.

Thank you very much in advance.
```

---
## \#979 Posted by: webst Posted at: 2018-05-26T18:38:28.362Z Reads: 363

```
[quote="Minim, post:975, topic:37579"]
Are there any do/don’t do with the vesc6? I’ve heard many said they killed 4.12 vescs with user error in the settings. Kinda want to avoid doing that :smiley:
[/quote]

As far as I know VESCs 4.12 blew mainly because of exceeded erpm limit which was around 60000, now it's 150000 if I recall correctly. Benjamin tried to fry this thing really hard on his youtube videos with no luck. I, myself got them up to 50A on 10S while I was pushing my friend on a bike up pretty steep hill for a minute or so with no sweat. Temperature didn't even rise above 50°C (122°F). Just connect them and ride I guess.
```

---
## \#980 Posted by: deucesdown Posted at: 2018-05-26T20:10:27.359Z Reads: 369

```
The reasons I see often:
- motor phase wires disconnected or touched
- short somewhere, maybe leads penetrated the silicone wires
- that particular vesc was not well built
- canbus for duals
- bad/intermittent connections
- random mystery (lots of these)
- motor blown

I don't think there are that many erpm based failures.
```

---
## \#981 Posted by: Minim Posted at: 2018-05-26T21:23:25.468Z Reads: 364

```
Canbus with dual? I thought that was the preferred way?
```

---
## \#982 Posted by: Jc06505n Posted at: 2018-05-26T22:21:20.503Z Reads: 368

```
A sum of members prefer spilt PPM as opposed to canbus because with canbus you lose 2 ESC’s while POM you only lose one. 

I would use Canbus with Focboxes and Solit PPM with -$100 ESC, but that’s just me
```

---
## \#983 Posted by: Jc06505n Posted at: 2018-05-26T22:22:03.908Z Reads: 371

```
I wonder how many VESC6’s are out there as opposed to VESC4.12 to truly say that ESC6 solves all of these issues.
```

---
## \#984 Posted by: district9prawn Posted at: 2018-05-26T23:22:07.586Z Reads: 366

```
My ebike is running off my self built ESCape. I've been doing lots of full throttles starts at 12s and 100a battery, so over 4kw. This is on foc too at 30khz switching frequency.
```

---
## \#985 Posted by: Minim Posted at: 2018-05-26T23:30:24.125Z Reads: 369

```
I think @trampa stated in a vesc thread that canbus was the way to go when splitting. It does make sense since gnd potential can be different and cause ground loops that fck stuff up. Might be an other reason here tho but groundloops can make many funny results :X
```

---
## \#986 Posted by: philvanzu Posted at: 2018-05-27T11:28:48.873Z Reads: 380

```
[quote="Jc06505n, post:983, topic:37579, full:true"]
I wonder how many VESC6’s are out there as opposed to VESC4.12 to truly say that ESC6 solves all of these issues.
[/quote]

http://www.electric-skateboard.builders/t/vesc-hardware-firmware-branches-market-shares-survey/52517

Not that many. looking at the figures it looks like the Focbox did solve a lot of these issues though, considering it was released roughly in the same time period as the VESC6.

would be nice to get more data once the group buy ESCapes are out though.
```

---
## \#987 Posted by: Manu39 Posted at: 2018-05-29T10:16:43.846Z Reads: 363

```
hello @stewii , here is 100 kms done with the vescape on the foraker and no problem to report. I wanted to thank you again for the great work you did.
```

---
## \#988 Posted by: Silverline Posted at: 2018-05-29T15:30:11.649Z Reads: 363

```
Was it R0 or R1 that should be removed ?

@LukePL is this week, the big "dual housing week" :smile:
```

---
## \#989 Posted by: webst Posted at: 2018-05-29T17:13:14.426Z Reads: 365

```
R1, should not be present in new batches
```

---
## \#990 Posted by: Silverline Posted at: 2018-05-29T17:22:26.830Z Reads: 365

```
I have two of the first Escapes ever made...
```

---
## \#991 Posted by: LukePL Posted at: 2018-05-29T19:00:46.950Z Reads: 378

```
Yep 😁![IMG_20180529_205812|375x500](upload://5B2Co62ESiH13nIU83RjixlDUms.jpg)
```

---
## \#992 Posted by: Silverline Posted at: 2018-05-29T19:14:13.688Z Reads: 367

```
OMG..... Dips on two double housing 😍😍😍😍😍
```

---
## \#993 Posted by: Minim Posted at: 2018-05-29T21:56:16.954Z Reads: 398

```
Made one of the enclosures as a test today. They do look great but I have one concern and that is how the PCB is only fixed by two M3 screws in one end. I can’t really torque them down either since the insulator pad is sitting under it. Do you use some kind of silicone to seat the rest and make sure vibrations doesn’t kill it @stewii ? 

![image|374x500](upload://203gskDMwWRjPZb6L6suOHRLB6j.jpeg)![image|666x500](upload://2cog6Xotaoac5m7SiOnWFh9w4YT.jpeg)![image|374x500](upload://nfV2RafWvwUjgME1fDTOECZsaX4.jpeg)
```

---
## \#994 Posted by: Minim Posted at: 2018-05-29T21:59:28.279Z Reads: 396

```
The picture I wanted to add didn’t get in so I’m trying a separate post. This is the M3 screws I’m worried about.

![image|374x500](upload://6Vutv34uE0KvHADQkb4htpOk4zr.jpeg)
```

---
## \#995 Posted by: Cobber Posted at: 2018-05-30T02:03:37.695Z Reads: 389

```
At the least you need to put a mess of neutral cure silicone (some use hot glue although it softens with heat) between the caps and the positive/negative 10AWG wires running in to the esc so vibration doesn't kill them.
```

---
## \#996 Posted by: stewii Posted at: 2018-05-30T09:16:52.130Z Reads: 390

```
You can put paper washers (1mm height, depending the thickness of the thermal pad) between the housing and the PCB on those 2 internal M3 screws so the height will be the same as the FETs + thermal pad, that way you can torque the screws.

And also don't forget what Cobber said.
```

---
## \#997 Posted by: Minim Posted at: 2018-05-30T09:35:59.335Z Reads: 392

```
Thanks guys. And to be clear this is me doing things I don't know howto do so the vesc with case comming from @stewii will prolly be mounted as it should be :D
```

---
## \#998 Posted by: Minim Posted at: 2018-05-31T04:42:23.172Z Reads: 397

```
What is the name of the plugs the board uses? I ordered various connector and now I don’t recall the name of the one that does fit on the balance connector. Need to order smt that fits the other ports as well ^^

Edit:
From the bom it looks like Micro JST. Ordered these to see if they fit.  

JST PHR, 2mm Pitch, 3 Way, 1 Row Female Connector Housing
JST PHR, 2mm Pitch, 5 Way, 1 Row Female Connector Housing
JST PHR, 2mm Pitch, 4 Way, 1 Row Female Connector Housing
JST PHR, 2mm Pitch, 8 Way, 1 Row Female Connector Housing
JST PHR, 2mm Pitch, 6 Way, 1 Row Female Connector Housing
JST PH Crimp Terminal Contact, Female, 0.05mm² to 0.2mm², 30AWG to 24AWG, Tin Plating
```

---
## \#999 Posted by: quitzu Posted at: 2018-05-31T22:15:24.851Z Reads: 393

```
Are there still some ESCape available as PCB Bare or fully assembled?
```

---
## \#1000 Posted by: Minim Posted at: 2018-05-31T22:32:09.758Z Reads: 396

```
Made a short "making of" movie for my ESCape cases. Design is by @stewii . 

 https://www.youtube.com/watch?v=G-xif0AYjOg
```

---
## \#1001 Posted by: new Posted at: 2018-06-08T11:36:31.797Z Reads: 389

```
[quote="quitzu, post:999, topic:37579, full:true"]
Are there still some ESCape available as PCB Bare or fully assembled?
[/quote]

I got the same question but can't PM @stewii to order. Is this a new user limitation?
```

---
## \#1002 Posted by: Cobber Posted at: 2018-06-08T11:59:14.324Z Reads: 386

```
@new @quitzu The only ESCape's available now are the ones that were pre-ordered, if you have a ESCape coming your way some months ago you would have paid 85 pounds for each one and again recently you would have made a second payment.

If non of that applies to you, **you missed the "group buy"** and will need to wait for the next opportunity to arise. To all of the guys who desperately want one, think for a moment. **PM'ing stewii will not get you one and will just make more work for stewii so it will take longer for him to fulfill this delivery and it will take even longer before he begins the next.**
```

---
## \#1003 Posted by: bevilacqua Posted at: 2018-06-08T12:05:40.444Z Reads: 388

```
Got 2 PCBs and no Time/Parts thanks to Bimmer. EU (DE) Located
```

---
## \#1004 Posted by: chuttney1 Posted at: 2018-06-09T02:33:32.145Z Reads: 388

```
Just create a wait list without taking any money so you at least have a conservative number of people who would buy.
```

---
## \#1005 Posted by: Willyfan Posted at: 2018-06-13T10:33:53.538Z Reads: 376

```
@stewii : I'm interested to use a vesc 6 for a cablecam, how I can contact you? Sorry but I'm new in this forum and I don't found link or other info. If someone can help me...
```

---
## \#1006 Posted by: Jc06505n Posted at: 2018-06-13T10:56:32.710Z Reads: 382

```
Read the thread to understand the current status of obtaining an escape.
```

---
## \#1007 Posted by: AreaKruzer Posted at: 2018-06-13T10:57:50.610Z Reads: 379

```
The group buy for now has ended. Have to wait for stewii to set up for the 2nd group buy. But that is only if he can gather enough interests
```

---
## \#1008 Posted by: Minim Posted at: 2018-07-06T22:14:45.714Z Reads: 363

```
What firmware are you guys running on the Escapes? Is the stock 3.38 the goto firmware?
```

---
## \#1009 Posted by: ron Posted at: 2018-07-07T07:16:58.449Z Reads: 362

```
Does anyone have stencils for the PCB or knows where I can order them cheap? The cheapest offer I found was something for 40USD and this for the Kapton Version and not steel/aluminium version!.

Would be thankful if someone could offer them or lead me in the right direction.

Thanks in advance
```

---
## \#1010 Posted by: chuttney1 Posted at: 2018-07-08T05:20:17.833Z Reads: 353

```
Try jlcpcb.com. For cheap PCB, quality is very good from some of the youtube videos.
```

---
## \#1011 Posted by: banjaxxed Posted at: 2018-07-08T12:42:47.196Z Reads: 355

```
https://www.electric-skateboard.builders/t/b-box-kit-groupbuy/49972/148?u=banjaxxed
```

---
## \#1012 Posted by: Holyman92 Posted at: 2018-07-08T15:05:15.888Z Reads: 359

```
if you can get me a vector of the stencil i could try and make u a kapton stencil for material cost and shipping... I would pretty much use my vinyl cutter
```

---
## \#1013 Posted by: Pimousse Posted at: 2018-07-09T07:52:22.696Z Reads: 356

```
Yes.
10char
```

---
## \#1014 Posted by: ron Posted at: 2018-07-09T23:23:01.818Z Reads: 353

```
Thanks for the offer. Do you live in Europe?

I will provide you the vector files. Are you sure the plotter can make such tiny holes?
```

---
## \#1015 Posted by: Holyman92 Posted at: 2018-07-09T23:24:40.191Z Reads: 357

```
I live in the US and I'm not sure.. I was going to cut it on vinyl 1st then if it worked cut it on the kapton
```

---
## \#1016 Posted by: ron Posted at: 2018-07-09T23:28:22.586Z Reads: 358

```
jlcpcb couldn't provide me an offer. They are unable to open the GBP and GTP files. SO they asked me if I could upload the whole GERBER Files of the PCB which I don't have.

So I didn't bother with jlcpcb anymore.
```

---
## \#1017 Posted by: SammiHuangabc Posted at: 2018-07-12T06:12:29.283Z Reads: 347

```
Very nice, what is the prices?
```

---
## \#1018 Posted by: ElskerShadow Posted at: 2018-07-12T14:38:58.977Z Reads: 345

```
Anyone using these with a Gt2b? When I connect my receiver on channel 2 it's not ON, only on Channel 1 and VCC I have a light...
```

---
## \#1019 Posted by: Pimousse Posted at: 2018-07-12T14:58:03.170Z Reads: 347

```
Maybe you fried the receiver with wrong wiring ?
Replace the Rx or try to power it up through another channel (CH1, CH3) while using the CH2 for signal.
```

---
## \#1020 Posted by: Silverline Posted at: 2018-07-12T15:37:39.642Z Reads: 355

```
Gt2b and escape... Works perfect for me
```

---
## \#1021 Posted by: Taliesin Posted at: 2018-08-05T21:43:22.326Z Reads: 346

```
Can someone explain all the plug ins for me?

I know where the motor sensor wire plugs go, and I assume the micro usb is for hooking it up to your computer and running vesc tool, but are the rest used for?

![image|375x500](upload://hj3526ne6jVsxJZWLRVoNP6YDv9.jpeg)
```

---
## \#1022 Posted by: Silverline Posted at: 2018-08-05T21:52:47.720Z Reads: 344

```
Vesc 6 manual, page 3 : http://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-24166.html#manuals
```

---
## \#1023 Posted by: briman05 Posted at: 2018-08-12T19:11:22.912Z Reads: 342

```
Can is for can bus and the ppm is for the remote
```

---
## \#1024 Posted by: louwii Posted at: 2018-08-12T20:29:44.617Z Reads: 339

```
comm is often used to plug-in a bluetooth module.
```

---
## \#1025 Posted by: Riako Posted at: 2018-08-28T06:53:50.996Z Reads: 329

```
We are all with you ! Courage Stewii :muscle: :stuck_out_tongue_winking_eye:
https://media.giphy.com/media/xUA7b9po1wawZ5c2zK/source.gif
```

---
## \#1026 Posted by: Andy87 Posted at: 2018-08-28T07:05:41.502Z Reads: 325

```
hope it´s not too late, or you already found out by your own.
Don´t forget that you need to change the wire order in every plug. They turned around 180*  compared with the standard VESC6 plug pins.
```

---
## \#1027 Posted by: mmaner Posted at: 2018-08-28T16:30:47.231Z Reads: 313

```
what's the price of a fully assembled ESCape now?
```

---
## \#1028 Posted by: uigiroux Posted at: 2018-08-28T19:54:16.541Z Reads: 310

```
It's £240 which currently is $308 :slight_smile:  That's for dual with dual enclosure, so half that for single with enclosure I believe.
```

---
## \#1029 Posted by: SpeedyGonzales Posted at: 2018-10-08T15:40:36.951Z Reads: 295

```
[quote="stewii, post:861, topic:37579"]
Latest ESCapes come without R0.
[/quote]

Do you mean without R0 or R1?
I'm assuming it is R1.
I'm finally going to use your ESCape and it still has R1 (000) on it.
Do I need to desolder it and nothing else?
```

---
## \#1030 Posted by: SpeedyGonzales Posted at: 2018-10-09T14:43:37.652Z Reads: 292

```
@stewii
Do you still sell bare PCBs and provide BOM and stencil files?
```

---
## \#1031 Posted by: SpeedyGonzales Posted at: 2018-10-15T15:58:36.022Z Reads: 281

```
Is @stewii still alive?
Anybody?
```

---
## \#1032 Posted by: bevilacqua Posted at: 2018-10-15T17:34:54.284Z Reads: 277

```
I have 2 pcbs that I could sell. The plan was to make my own, but I got scammed by Bimmer :/ 
PM me if you are interested.
```

---
## \#1033 Posted by: SpeedyGonzales Posted at: 2018-10-16T02:33:53.538Z Reads: 274

```
I just bought 4 from other member. Thanks anyways.
Now I'm looking for some answers:
My ESCape still has R1 (000) on it.
Do I need to desolder it and nothing else?
After that can I set it up on the VESC tool just like any other VESC6?
Should I expect any surprises?
```

---
## \#1034 Posted by: Pimousse Posted at: 2018-10-17T12:01:01.102Z Reads: 267

```
Yes, desolder it.
Yes, program it as a VESC 6
No, no surprises.

Anything else ? :slight_smile:
```

---
## \#1035 Posted by: Andy87 Posted at: 2018-10-17T12:04:09.698Z Reads: 265

```
Wowowo, just came up to it.
What would be the problem if I let the r on the pcb? Gona be a Problem?
```

---
## \#1036 Posted by: Pimousse Posted at: 2018-10-17T12:06:10.862Z Reads: 262

```
Potential issue is that 5V from USB will fight against 5V from VESC.
```

---
## \#1037 Posted by: Andy87 Posted at: 2018-10-17T12:07:40.965Z Reads: 265

```
I thought I read before that stewii didn’t have had any issues with it.
Or did somebody till now fried one of the escapes?
```

---
## \#1038 Posted by: Pimousse Posted at: 2018-10-17T12:10:40.240Z Reads: 270

```
Well, it may depends on your computer and its USB power.
If your computer USB voltage is less than VESC one and have protection on its USB ports, well no problem.
In any other case, you may fry the VESC or the laptop (at least a part of it).
```

---
## \#1039 Posted by: Andy87 Posted at: 2018-10-17T12:12:52.388Z Reads: 261

```
Good that I didn’t set them up yet 😅
Will get rid of the r1. Thx!
```

---
## \#1040 Posted by: pat.speed Posted at: 2018-10-17T19:42:21.632Z Reads: 263

```
I’m pretty sure you can also just not power the vesc while programming as it will use the computers 5v
```

---
## \#1041 Posted by: Andy87 Posted at: 2018-10-17T19:46:32.825Z Reads: 265

```
I remember I read something about it and that stewii said I use both without issues...just don’t want to risk to fry them.

If I use the 5V from the usb, how to run motor detection without battery connected? 5V is enough for it? 🤔
```

---
## \#1042 Posted by: Silverline Posted at: 2018-10-17T19:48:47.103Z Reads: 260

```
I removed R1 as well. You need power on the vesc to spin Up the motors in motor detection :wink:
```

---
## \#1043 Posted by: pat.speed Posted at: 2018-10-17T19:57:03.824Z Reads: 254

```
True, forgot about that
```

---
## \#1044 Posted by: Andy87 Posted at: 2018-10-17T20:01:56.592Z Reads: 250

```
Ok so i will remove it better.
Thx for your info
```

---
## \#1045 Posted by: Nemesis Posted at: 2018-10-17T22:31:43.409Z Reads: 257

```
Do all of the escapes have the R1? i got my singles from the second batch (GB group buy 2).
```

---
## \#1046 Posted by: Riako Posted at: 2018-10-17T22:41:40.632Z Reads: 265

```
No, it was before the professionnal production. I have done the same on the 1st back from Stewii.
The 2nd GB come WO the R1 ;) 
https://www.instagram.com/p/BnlS2mvghzo/?hl=fr&taken-by=riakobonito
```

---
## \#1047 Posted by: SpeedyGonzales Posted at: 2018-10-17T23:31:48.115Z Reads: 255

```
Thanks a ton dude. I really appreciate it.
It looks like in the process we revived the thread.:sweat_smile:
Yes, I have more questions, but I will go easy.:grinning:
At this point I'm using VESC 4.12 and hall effect throttle on my e-bike and it works great.
Is it possible to set up second throttle to control regen / brake?
```

---
## \#1048 Posted by: ArnhemAnt Posted at: 2018-10-18T05:23:52.628Z Reads: 256

```
[quote="Andy87, post:1035, topic:37579"]
What would be the problem if I let the r on the pcb? Gona be a Problem?
[/quote]


My two ESCapes were from the 'original' order. I didn't make any changes to the ESC and was able to use the USB to computer and power the ESC's to run the motor detection, etc. No problems and all is working perfectly. I guess it is your call as to whether you remove R1 (whatever that is?) or not.
```

---
## \#1049 Posted by: Andy87 Posted at: 2018-10-18T05:45:44.390Z Reads: 255

```
so the usb 5V were enough to run the motor detection?
or you mean you had both connected at the same time without issues?
```

---
## \#1050 Posted by: ArnhemAnt Posted at: 2018-10-18T06:02:44.245Z Reads: 257

```
[quote="Andy87, post:1049, topic:37579"]
you had both connected at the same time without issues?
[/quote]


Correct. USB and 12s4p connected at the same time and no issues. I recall reading about this R1 'thing' but I chose to ignore it and had no issues setting things up. In all honesty, I still have absolutely no idea what R1 is.
```

---
## \#1051 Posted by: eb1925 Posted at: 2018-10-18T06:53:52.343Z Reads: 254

```
Could someone fully explain this R1 business? I have 2 original ESCapes and don't want to destroy things
```

---
## \#1052 Posted by: Andy87 Posted at: 2018-10-18T07:25:54.233Z Reads: 258

```
@ArnhemAnt and @eb1925 if you look somewhere more up in the threat, everything should be explained.
didn´t have had a time to look to all this 880 messages...so I will try to remember it right :sweat_smile:
but basically it´s like that, the R1 is a resistor which takes the voltage form your USB to power the vesc. The problem is that your USB power supply has a different potential than your battery power supply. Depending on how big this difference it can cause a defect of electric components.
I think it would be the same if you run a Y-Split ppm with the 5V wire connected on each of your ESC.  

If somebody can explain it more detailed, please feel free to correct me ;)
```

---
## \#1053 Posted by: Pimousse Posted at: 2018-10-18T07:53:24.282Z Reads: 253

```
Yes, you can use ADC1 for throttle and ADC2 for brake.
Then you have to select it in ADC tab (don't remember exactly the label).
```

---
## \#1054 Posted by: ArnhemAnt Posted at: 2018-10-18T08:12:50.679Z Reads: 261

```
[quote="stewii, post:812, topic:37579, full:true"]
I no longer populate R1. Again I have never encountered any issue, but I guess that depends on the PC/laptop.
[/quote]


Found this quote back on the 21st of May, by the man himself.
```

---
## \#1055 Posted by: eb1925 Posted at: 2018-10-18T16:17:51.794Z Reads: 258

```
Thank you!
```

---
## \#1056 Posted by: Silverline Posted at: 2018-10-18T18:20:50.740Z Reads: 272

```
It seems that @stewii is not here very often. So i'm asking here instead.

I suspect that my two big caps , is the source for my problem with "over current" fail i get from time to time. 

 The caps is only soldered on one side, is this okay ? Or could this be my problem ?

Finally , where do i find these "heat pads" to transfer the heat from the fets ?
![IMG_20181018_202345|690x388](upload://l47iaV2rSVqO69ss7OOirUVemkQ.jpeg)
```

---
## \#1057 Posted by: SpeedyGonzales Posted at: 2018-10-18T19:31:39.796Z Reads: 267

```
You might want to resolder caps.
You can use thermal conductive tape like this:
https://www.amazon.com/dp/B01MSL64XG/?coliid=I2W9CXAGHYLB91&colid=15U3DHO46KQSC&psc=0&ref_=lv_ov_lig_dp_it
```

---
## \#1058 Posted by: ArnhemAnt Posted at: 2018-10-18T20:32:56.399Z Reads: 258

```
@Silverline - what is the product (black in colour) that you have between the two caps? Have you checked to make sure it isn't conductive or corrosive? This may not be directly related to your current issue, but it may cause problems later on.
```

---
## \#1059 Posted by: Nordle Posted at: 2018-10-18T20:45:33.291Z Reads: 256

```
the black thing is hot glue or silicone i assume, and also it should be totally fine if each capacitor lead is properly soldered to the other side of the pcb, a pic maybe, but i don't think that's your problems source
```

---
## \#1060 Posted by: Silverline Posted at: 2018-10-18T20:57:53.255Z Reads: 246

```
Yes it's just silicone
```

---
## \#1061 Posted by: SpeedyGonzales Posted at: 2018-10-19T03:25:37.117Z Reads: 251

```
So, I desoldered R1 (000) resistor, hooked everything up and have my 8072 motor running on FOC with NO drama. Thank you all.
Next will be test under load.
```

---
## \#1062 Posted by: Riako Posted at: 2018-10-19T09:02:38.699Z Reads: 250

```
Yeah good, let us know about your teste ride :v: ;) enjoy & good ride !
```

---
## \#1063 Posted by: Kug3lis Posted at: 2018-10-19T09:06:59.374Z Reads: 246

```
ABS_OVER_CURRENT is then motor consumes a shit load but esc didn't managed to catch up and says that it even when it climbs over max limit :) I am getting this constantly right now :) with currents like 200A :D
```

---
## \#1064 Posted by: Andy87 Posted at: 2018-10-19T09:21:27.968Z Reads: 246

```
this doesn´t result in cut outs?
```

---
## \#1065 Posted by: Kug3lis Posted at: 2018-10-19T09:39:34.788Z Reads: 242

```
It does but that cut off doesn't feel on these motors like literally just today I felt that it was cuting out :D
```

---
## \#1066 Posted by: Silverline Posted at: 2018-10-19T09:43:31.907Z Reads: 244

```
I'm not pushing my motors at all when the fault is triggered. It often happen when only going around 10km/h, without much loade. Thats why i think it's maybe my caps.
```

---
## \#1067 Posted by: Kug3lis Posted at: 2018-10-19T09:48:23.041Z Reads: 239

```
Check also ur leads.. and solder stuff :)
```

---
## \#1068 Posted by: Silverline Posted at: 2018-10-19T10:00:36.726Z Reads: 244

```
Do you know if "abs-over-current" could be triggered from a defective receiver , or loose connection between receiver and vesc, or maybe conflicting RF signals. ? The funny thing is, that im only getting abs-over-current, when riding with other. Never when i'm just riding alone ?
The motors brake , not very funny :-(
```

---
## \#1069 Posted by: Kug3lis Posted at: 2018-10-19T10:02:39.950Z Reads: 238

```
abs_over_current means esc saw current reading higher than absolute max current limit ;)
```

---
## \#1070 Posted by: Silverline Posted at: 2018-10-19T10:04:08.182Z Reads: 240

```
Yes i know that. But when the fault is triggered, and the motor brakes down, i'm not pulling anything near that.

Going Up a steep hill, no problem at all. But going 10km/h, while riding with others, sometimes give me abs-over-current, and the motors brakes, almost sending me flying.
```

---
## \#1071 Posted by: lrdesigns Posted at: 2018-10-19T10:08:43.580Z Reads: 242

```
That is weird. Which remote you have?
```

---
## \#1072 Posted by: Silverline Posted at: 2018-10-19T10:10:04.639Z Reads: 246

```
Yes it is :-(  i'm using Gt2b, the same does those I'm driving with.
```

---
## \#1073 Posted by: Kug3lis Posted at: 2018-10-19T10:12:00.259Z Reads: 246

```
Maybe u remote send impulses or etc..
```

---
## \#1074 Posted by: Silverline Posted at: 2018-10-19T10:14:50.293Z Reads: 249

```
Now you are talking. Like conflicting impulses , could be a theory, or "out of the range" impulses. I have tried with a new Gt2b remote and receiver. But still same problem..... :-(
```

---
## \#1075 Posted by: Kug3lis Posted at: 2018-10-19T10:15:49.761Z Reads: 241

```
Have u tried not Gt2b?
```

---
## \#1076 Posted by: lrdesigns Posted at: 2018-10-19T10:16:18.025Z Reads: 242

```
In that case it can’t be the gt2b. It’s the most reliable remote you can have for esk8. The mystery deepens!
```

---
## \#1077 Posted by: Silverline Posted at: 2018-10-19T10:17:08.833Z Reads: 243

```
Nope, not yet. Because first i wanted to know, if it's even possible that at receiver/remote could give that sort of fault.

@lrdesigns yes exactly, thats why i use it 😀
```

---
## \#1078 Posted by: Kug3lis Posted at: 2018-10-19T10:18:13.939Z Reads: 244

```
Well VESC code is not perfect so everything is possible :) But first I would try different remote :) It can be that sometimes it sends short impulse of full throttle and then it overshoots limits.

Do you have fault report text with variables?
```

---
## \#1079 Posted by: Silverline Posted at: 2018-10-19T10:19:20.586Z Reads: 272

```
@Kug3lis yes... They look like this.  And both the Escapes get this faults (they run can bus )

![Screenshot_20181012-175415|281x500](upload://cCxoKgjVsDEAfYROZHqFgaMhuj0.png)

![Screenshot_20181012-175308|281x500](upload://9dM8YM3FM94nQt2ibvQIUo56JGc.png)
```

---
## \#1080 Posted by: Kug3lis Posted at: 2018-10-19T10:21:27.691Z Reads: 248

```
What is you are minimum current limits? Looks like it brakes and maybe overshoots braking currents
```

---
## \#1081 Posted by: Silverline Posted at: 2018-10-19T10:22:49.736Z Reads: 265

```
![IMG_20181012_202345|281x500](upload://a57bh9IEZU0enl0dO4ndAbTkWIk.jpeg)
```

---
## \#1082 Posted by: Kug3lis Posted at: 2018-10-19T10:28:50.443Z Reads: 274

```
Went into source code and ABS_OVER_CURRENT gets only triggered then the current is over abolsute maximum current value and nowhere else:

https://github.com/vedderb/bldc/blob/a20c35b33863b85bc5a11b80d30e4df3d8066cc3/mc_interface.c#L1130

So it looks like it reads higher current than the limit 150... which is interesting. Try maybe turn off slow abs current limit
```

---
## \#1083 Posted by: Kug3lis Posted at: 2018-10-19T10:31:20.992Z Reads: 263

```
Did some more review, I am thinking that then error is record it reads current again and looses the value it read at the fault time...
```

---
## \#1084 Posted by: Silverline Posted at: 2018-10-19T10:36:31.928Z Reads: 259

```
But dont you think, that defective caps or a loose connection in the caps, could give some sort of jitter / peake amps, and trigger the over-current ?
```

---
## \#1085 Posted by: Kug3lis Posted at: 2018-10-19T10:38:45.309Z Reads: 260

```
I would first thing with high current impulses suspect the motors, can be maybe some windings are shortening which makes the current shoot and because that stuff doesn't really depend on speed that would explain the error.
```

---
## \#1086 Posted by: Silverline Posted at: 2018-10-19T10:42:39.908Z Reads: 254

```
Yeah.. but the thing is, that i had the exact same problem with my old motors. And since it's both the vesc's, i dont think it's my motors
```

---
## \#1087 Posted by: Kug3lis Posted at: 2018-10-19T10:57:33.860Z Reads: 261

```
I filled the issue on vesc for wrong info in faults because the logic fails if your ABS current limit is 150 and in fault its -15A :smiley:

https://github.com/vedderb/bldc/issues/66
```

---
## \#1088 Posted by: Silverline Posted at: 2018-10-19T11:04:23.348Z Reads: 254

```
Cool thanks....

I have pm'd Benjamin as well, but dont expect an answer anytime Soon.
```

---
## \#1089 Posted by: SpeedyGonzales Posted at: 2018-10-19T18:04:40.537Z Reads: 253

```
I'm running my ESCape with Hall throttle by using COMM 5V ADC1. Unfortunately, VESC tool can map only up to 3.3V, so I can't use full range of my throttle. On my other setup with VESC 4.12 and BLDC tool I can map and set Max. V to match my throttle at about 3.85V and use full range. 
It looks like VESC tool is limited in that respect. Any thoughts on that?
```

---
## \#1090 Posted by: julian_esk8 Posted at: 2018-10-21T16:31:59.160Z Reads: 247

```
Hello,
Is there anyone how can help me? I got myself an ESCape Vesc and I am triing to connect it to my computer. The blue LED shines. Current from my power supply is also normal. I am not an expert with the Vesc 6 but is it possible that I got a Vesc without bootloader or firmware? The USB cable is also in best condition. Thanks in advance!
Best Regards
Julian
```

---
## \#1091 Posted by: Kug3lis Posted at: 2018-10-21T16:33:32.362Z Reads: 248

```
Processor is running on 3.3V you can't supply more than it is operating, change it to 3.3V supply its just pot or get voltage divider 5v to 3.3V
```

---
## \#1092 Posted by: Andy87 Posted at: 2018-10-21T16:55:09.576Z Reads: 256

```
Try different cables. If it’s a charge only cable you can’t connect. If that’s not work, check if you have the right usb driver installed.
```

---
## \#1093 Posted by: SpeedyGonzales Posted at: 2018-10-21T23:55:06.277Z Reads: 255

```
Thank you for the info. I'm surprised to hear that.
Assuming that you are correct and the processor can handle only up to 3.3V, then why 5V power is provided? That is not good. VESC 4.12 provides both 3.3V and 5V. and obviously can handle both. VESC 6 is step backwards in that respect. I understand that I can use couple of resistors to divide voltage, but that is half-assing. On the other hand, the majority of hall sensors are running on 4.5-20V and you don't need 3.3V on that connector, but it is there. It all doesn't make sense.
I guess nothing is perfect, but I can live with that.
```

---
## \#1094 Posted by: Kug3lis Posted at: 2018-10-21T23:59:20.204Z Reads: 264

```
Digital pins are compatible with 3.3V/5V. Processor uses 3.3V supply in both version. Hall sensors already has voltage divider with voltage selection on pcb. You doing not intended behaviour to use processor ADC which works by measuring voltage from 0 to REF which point is MCU power supply 3.3V. So you have to supply exact the same range 0 to 3.3v if you want to have full throttle range. or use voltage divider circuit like hall sensors do.

EDIT: hall sensors are not like potentiometers they work differently ;)
```

---
## \#1095 Posted by: SpeedyGonzales Posted at: 2018-10-22T01:57:31.020Z Reads: 279

```
What I'm only saying is this...
Motor hall sensors don't need voltage divider because a great majority, if not all of them, work on 4.5-20V, They are not designed to work at 3.3V, so 5V only will do just fine. That divider and switch on the motor halls connector is not needed, so why bother?
From what you are saying, a processor that handles COMM pins needs 3.3V or less for processing, so a 3.3/5V divider and a switch would be great to have on a COMM plug. A 5V supply only is a step backwards, considering that VESC 4.12 has both.
It is just common sense. 
I know that hall sensors operate on different principles than potentiometers.
That's a kindergarten stuff.
it looks like there is no way around, so I will live with that.
But, just in case I posted it on the VESC PROJECT forum, so if I know more I will be back.
Persistence is my middle name.
Right now I will focus on installing hall sensors in two of my 80mm motors.![80mm%20motor%20hall%20sensors%201|690x388](upload://a3qbnCxjkmxLOgr3G6IL4NHH388.jpeg) 
![80mm%20motors|690x388](upload://x4hJVDkMntG3XcZ3j8TR86rTtqg.jpeg)
```

---
## \#1096 Posted by: Kug3lis Posted at: 2018-10-22T07:25:30.707Z Reads: 276

```
Well I looked at your post at vesc forum and I can tell that you probably kindergarten level mindset if you think that changing code will change how microprocessor internals work... Go read how adc works in stm32 page...

And 4.12 and 6 mcu side and comm port is same. You hade 3.8V because of shitty vreg on your 4.12
```

---
## \#1097 Posted by: SpeedyGonzales Posted at: 2018-10-22T18:20:48.799Z Reads: 279

```
I just solved that problem despite or maybe because of my kindergarten level mindset :-)))
Also with the same mindset I designed and built a very efficient and compact, first of its kind transmission for an electric bicycle. (I attached photo so no BS here)
You don't stop digging into those codes. Let's hope that you will find what you are looking for there.![Cycloid%2019-1%202|690x388](upload://htjivrul7cHiR8WAe11ZaTqbUj5.jpeg)
```

---
## \#1098 Posted by: Riako Posted at: 2018-10-22T18:43:06.496Z Reads: 278

```
I want that masterpiiiiiiiiece !!!! :crazy_face: !!! :exploding_head: !! :heart_eyes: !
```

---
## \#1099 Posted by: julian_esk8 Posted at: 2018-10-23T10:57:47.477Z Reads: 271

```
I tested with different cables, that works fine with my phone. And my USB driver is also the newest version. My PC works fine with every VESC 4.10 or 4.12. Also VESCs with different firmware versions work great. Only the VESC 6 won´t show any sign of life. I am helpless.
```

---
## \#1100 Posted by: Andy87 Posted at: 2018-10-23T11:07:20.849Z Reads: 278

```
Try an other computer just to be sure it can only be the escape.
If that not work you need to get an st v2 link and load the bootloader and firmware on this way.
Strange as I thought @stewii is checking all of them before sending them out
```

---
## \#1101 Posted by: eb1925 Posted at: 2018-10-23T21:22:30.476Z Reads: 279

```
I had the same problem with my pc.....used my roommates and it worked fine
```

---
## \#1102 Posted by: 2small Posted at: 2018-10-26T20:20:48.980Z Reads: 284

```
Just got 2 ESC from @stewii  look good
```

---
## \#1103 Posted by: SpeedyGonzales Posted at: 2018-10-27T21:45:09.225Z Reads: 287

```
So far ESCape is working great. I tested it with two 80 mm motors. 
In order to get more startup torque I will be installing hall sensors in my two motors. I made  a few 120 deg mounting boards and I need only two . So, if you want to do something like that I have 3 extra boards that I can donate to the community for free. They are pre-drilled for .050" and .100" hall legs spacing. Five holes total, but you will need only three for each sensor.![Hall%20sensors%20holders%202|640x360](upload://hplbB4ZQlSJdp3d9LsNPHXLjDbn.jpeg) 
I have two that are .030" thick and one .060" thick. Either thickness works fine.
```

---
## \#1104 Posted by: SpeedyGonzales Posted at: 2018-11-01T05:17:12.413Z Reads: 274

```
I was setting up my motor and without any drama ESCape stopped working. No sign of life except DRV chip and one component next to it are getting hot. I assume that DRV is dead. Can you guys recommend someone that can bring my board back to life?
```

---
## \#1105 Posted by: Andy87 Posted at: 2018-11-01T07:00:04.911Z Reads: 268

```
@Martinsp maybe
```

---
## \#1106 Posted by: pat.speed Posted at: 2018-11-01T10:22:06.149Z Reads: 277

```
@JohnnyMeduse
```

---
## \#1107 Posted by: SpeedyGonzales Posted at: 2018-11-01T14:06:52.369Z Reads: 279

```
Thank you guys.
I PMed.
```

---
## \#1108 Posted by: SpeedyGonzales Posted at: 2018-11-27T22:34:45.451Z Reads: 262

```
Hi guys,
I just want to let you know that JF aka. JohnnyMeduse fixed my Escape and he is absolute pro.
IMHO he is the best man for the job.
```

---
## \#1109 Posted by: Sn4pz Posted at: 2018-11-27T22:43:22.603Z Reads: 262

```
Would those who have dual escapes in their boards stick with them over a unity?

I know one is two single escs, thats not my point, im just asking if you would change or not :)
```

---
## \#1110 Posted by: sayekim Posted at: 2018-11-27T23:40:29.364Z Reads: 262

```
I have yet to use mine on more than one ride. If it proves to be reliable to me I will ride them untill they break.
I’ll try a unity after that if that proves to be reliable.
```

---
## \#1111 Posted by: Sn4pz Posted at: 2018-11-28T22:51:11.484Z Reads: 258

```
Well if you ever have two you want to get rid of because your unity is too cool, I'll take them :smile:
```

---
## \#1112 Posted by: Minim Posted at: 2018-12-03T21:29:06.029Z Reads: 257

```
I wouldn't change them. Unity is prolly not ready before 2024 at enertions pace and by then there is prolly something else new out there :P
```

---
## \#1113 Posted by: Sn4pz Posted at: 2018-12-03T22:16:35.899Z Reads: 262

```
all right :sweat_smile::sob:

x2 :rofl:
```

---
## \#1114 Posted by: Vanarian Posted at: 2018-12-03T22:19:46.760Z Reads: 270

```
Need two physically separate ESCs, so Unity bundled ESC can't do for me 😆 so I'll stick with my ESCapes too haha
```

---
## \#1115 Posted by: Ingvarjedi Posted at: 2018-12-20T07:10:28.408Z Reads: 257

```
Hi people.
There are any news about the resumption of sales ESCape?
```

---
## \#1116 Posted by: rojitor Posted at: 2018-12-20T11:58:34.814Z Reads: 254

```
Don't think so
```

---
## \#1117 Posted by: uigiroux Posted at: 2018-12-20T15:31:59.751Z Reads: 253

```
I have two ESCape's from the last batch.  Is there an issue with them that needs to be fixed or is this just an isolated case? Was considering getting a Unity and selling the ESCape's...
```

---
## \#1118 Posted by: bigben Posted at: 2018-12-20T16:28:10.522Z Reads: 258

```
@ethel might buy your escapes if you decide to sell them?
He’s stateside too.
```

---
## \#1119 Posted by: uigiroux Posted at: 2018-12-20T16:51:20.574Z Reads: 260

```
Well I'd prefer to keep them, unless they have some issue I'd need to get fixed like @SpeedyGonzales had.  If that was just an isolated incident then I'm happy to keep mine, but if there's am issue that I'll need to get fixed, then I'd prefer to get a Unity.  I have both enclosures for the ESCape's also; one dual, and two singles.
```

---
## \#1120 Posted by: linsus Posted at: 2018-12-20T18:07:27.269Z Reads: 256

```
I sudgest to use them and find out ^^
```

---
## \#1121 Posted by: uigiroux Posted at: 2018-12-20T20:06:12.724Z Reads: 250

```
Good idea, lol :smile:
```

---
## \#1122 Posted by: ethel Posted at: 2018-12-20T22:18:01.490Z Reads: 254

```
Or sell them to me.
```

---
## \#1123 Posted by: chocol4te Posted at: 2019-03-08T14:09:17.000Z Reads: 230

```
Hey, I accidentally put 5V across VCC, and now isn't detected by either an ST Link or Black Magic Probe. I looked at all the schematics and most components should be at least 5V tolerant, but the MCU is definitely toast. Is it worth ordering a new STM32F405 and replace it, or do I need to get a new VESC?
```

---
## \#1124 Posted by: Pimousse Posted at: 2019-03-11T12:58:43.405Z Reads: 223

```
For someone with good SMD soldering skill (and a reflow station), changing the MCU shouldn't be that hard.
It's worth the effort, a MCU costs like 10€.
```

---
## \#1125 Posted by: chocol4te Posted at: 2019-03-18T17:39:49.490Z Reads: 224

```
Chip replacement went well, it’s happily updating and talking to the VESC tool, but I’ve got a new issue: phase A isn’t working. The motor exhibits the usual stuttering and jittery behaviour when one phase is missing. When phases B or C are disconnected it only buzzes and doesn’t move, when A is disconnected there is not change in behaviour. I’m going to swap 2 the AD8418s to see if it’s one of those that died, is there anything else I should look into?
```

---
## \#1126 Posted by: pat.speed Posted at: 2019-03-18T20:23:53.539Z Reads: 221

```
It may sound silly but just check there isn’t a loose bullet connector or wire
```

---
## \#1127 Posted by: district9prawn Posted at: 2019-03-18T23:41:14.277Z Reads: 216

```
Measure output voltage of the current amplifiers before you try replacing. Should read 1.65v with no current through the motor.

I've blown them with vcc transients and had them stuck at odd voltages.
```

---
## \#1128 Posted by: chocol4te Posted at: 2019-03-19T07:02:54.883Z Reads: 213

```
Unfortunately not, I checked thoroughly, and tested with a multimeter, thanks though :/
```

---
## \#1129 Posted by: chocol4te Posted at: 2019-03-19T07:05:44.434Z Reads: 218

```
Ahh, okay, I'll test now. Thanks! :)

Edit: I swapped the chips last night (I didn't read your post till this morning), and when I plugged it in just now my phase C current amplifier gave out the magic smoke. When I power the board now, I get blue and green LEDs for a few seconds, then just red blinking, no serial. I'm measuring 0.96V on the remaining two current amplifiers. I think I messed up the orientation of the chip on the C phase. :/
```

---
## \#1130 Posted by: chocol4te Posted at: 2019-03-21T13:40:42.088Z Reads: 212

```
Okay, so I've replaced the blown AD8418, then replaced the dead 3.3V DCDC converter with a large linear regulator, and now I'm back to where I started. It connects to the VESC tool, doesn't report any errors, but the A phase is dead. I'm going to hook an oscilloscope up to the gates of the FETs next to see if the issue is there :man_shrugging:

EDIT: Aaaand, DRV error. Great. I don't know whether to keep replacing parts, or just buy a new one :/
```

---
## \#1131 Posted by: district9prawn Posted at: 2019-03-23T11:47:45.121Z Reads: 211

```
Since you already replaced everything else you may as well do the DRV as well. Nothing else preventing it from working right?

I thought these weren't available any more. Have missed a lot in this thread.
```

---
## \#1132 Posted by: chocol4te Posted at: 2019-04-01T13:35:48.657Z Reads: 202

```
I've replaced the DRV8301, still getting the DRV error. It says "GVDD_UV" normally, then "GVDD_OV" when I try to run the motor. I measured AVDD to be 6.5V and GVDD to be 11V, neither changes when I try to run the motor :(
```

---
## \#1133 Posted by: AlanZhou Posted at: 2019-04-01T13:43:33.455Z Reads: 203

```
Drv error dosdent exactly mean the drv is dead, it's like a car check engine light, it can be multiple things, for example shorted fets durning detection will give out drv errors
```

---
## \#1134 Posted by: linsus Posted at: 2019-04-01T13:49:15.720Z Reads: 206

```
Best guess its one of the FETs then, measure between gate drain and source between em all and see if one sticks out
```

---
## \#1135 Posted by: chocol4te Posted at: 2019-04-01T19:17:52.187Z Reads: 201

```
All outputs had the same 8K ohm between them, and no FET had any shorts. I replaced both phase A FETs, and cleaned the whole board thoroughly (just in case flux being mildly conductive was the cause of issues), but no luck. I can't find any components that are unique to phase A that I haven't replaced now :/
```

---
## \#1136 Posted by: district9prawn Posted at: 2019-04-01T23:08:48.061Z Reads: 199

```
Do you have access to an oscilloscope to check the gate signals?
```

---
## \#1137 Posted by: chocol4te Posted at: 2019-04-02T05:57:05.154Z Reads: 202

```
I do, I’m going to check today. I’ll look at everything I can think of, but apart from the gates, where else should I focus?

Thanks for you help :)
```

---
## \#1138 Posted by: linsus Posted at: 2019-04-02T06:34:07.234Z Reads: 206

```
Guess check all voltage rails. Check for short between ground and vcc. Look for any empty pads on the pcb. Try resolder that drv. Not sure what else there is
```

---
## \#1139 Posted by: chocol4te Posted at: 2019-04-04T09:25:00.287Z Reads: 209

```
Done, everything as expected.

I’m getting two faults, I don’t understand GVDD_OV, as GVDD never hits the 16v required to trigger that fault, but FETHA_OC results in that phase being disabled by the DRV, so that explains why I wasn’t getting any output. 

When set the overcurrent mode to “report only”, duty cycle gets stuck at -95% with no input, and phase A is always high, then oscillates when I use the arrow keys, I’ve attached pictures of the scope on phase A and B to show the difference.

Phase B (normal operation)
![image|690x415](upload://m1oVGdc3miSYfto91qDwQQruRQc.jpeg) 

Phase A (always high)
![image|666x500](upload://e4r6hEp09tAbjiBjLg2xESkYQj3.jpeg)
```

---
## \#1140 Posted by: Manu39 Posted at: 2019-05-21T07:43:03.641Z Reads: 186

```
Hello guys
I have my vesc master that no longer has the green light on, after having updated to FW 3.57... an idea, on vesc tool the slave connects but impossible to connect to the master neither via the usb nor via the can bus it is no longer recognized...
When I try to connect it marks me NOT FIRMWARE READ RESPONSE
Thanks
```

---
## \#1141 Posted by: bevilacqua Posted at: 2019-05-21T07:46:04.526Z Reads: 185

```
Try flashing a new bootloader and downgrading the FW. I had issues with 3.57 too (motor detection)
```

---
## \#1142 Posted by: Manu39 Posted at: 2019-05-21T07:47:53.483Z Reads: 187

```
Thanks but what is the method to make the boot loader...now I'm in the unknown
```

---
## \#1143 Posted by: bevilacqua Posted at: 2019-05-21T08:23:55.760Z Reads: 192

```
https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#1144 Posted by: bevilacqua Posted at: 2019-05-21T08:28:31.947Z Reads: 188

```
you would need the Vesc6 .hex file, maybe @linsus has one (I only got 4.XX HW)
```

---
## \#1145 Posted by: linsus Posted at: 2019-05-21T08:41:44.917Z Reads: 186

```
https://github.com/vedderb/bldc

(easier to follow vedders instructions if you have a linux machine)

You'll need a discoverboard or ST-programmer if you want to upload a new bootloader. You're s'posed to be able to use the functioning vesc to fix the bricked one, I havn't tried this yet tho. Maybe @trampa can assist you
```

---
## \#1146 Posted by: Pimousse Posted at: 2019-05-21T09:03:58.857Z Reads: 174

```
We tried using the working one to flash the bricked one thanks to Black Magic Probe tool (SWD prog in VESC Tool).
However, no luck to discover the bricked VESC microcontroller. (CLK, IO and GND connected).
Next move : STLink :pensive:
```

---
## \#1147 Posted by: linsus Posted at: 2019-05-21T09:31:49.995Z Reads: 174

```
Hopefully u got a spare MCU so you can just do a swap :smile:
```

---
## \#1148 Posted by: Pimousse Posted at: 2019-05-21T09:47:30.725Z Reads: 182

```
Hopefully, we won't need to go that far ! :smile:
Anyway, there is seriously something to do. Bricking a VESC just because a bluetooth connection wasn't reliable enough is pretty scary !

This is really not eh first time I see that happening (I had the same with old Metr module and cheap Android phone).
```

---
## \#1149 Posted by: linsus Posted at: 2019-05-21T09:53:00.061Z Reads: 176

```
that does sound scary, never had any problems with my small cheap modules :open_mouth:
```

---
## \#1150 Posted by: Manu39 Posted at: 2019-05-21T10:46:33.070Z Reads: 176

```
You scare me....
```

---
## \#1151 Posted by: Pimousse Posted at: 2019-05-21T11:25:31.552Z Reads: 184

```
It has always happend when dealing with motor/app conf write.
Maybe it lacks of integrity check before sending it into internal registers, doesnt it ?

Now, we're looking for a stable FW version that Metr app can deal with.
@Manu39 was on FW 3.40, and everyhting was perfect. But we needed to move to 3.48+ for the use of COMM_GET_VALUES_SETUP_SELECTIVE.

So any FW version advice from 3.48 would be welcomed ! :slight_smile:
```

---
## \#1152 Posted by: linsus Posted at: 2019-05-21T12:06:42.284Z Reads: 182

```
Havn't done any update since november maybe :thinking:

Not sure which verision Im running, can check
```

---
## \#1153 Posted by: pookybear Posted at: 2019-05-22T05:04:56.789Z Reads: 178

```
This happened to me too. Vesc6. I tried changing POS ramp parameter using "expert settings" on metr pro. It would try to write the new parameters but it won't stick. Then eventually fails. After that my motor would spin so slow and cog badly.

I had to reload ackmaniac fw to clear it. I'm still using the metr module but using the ack app instead.
```

---
## \#1154 Posted by: Pimousse Posted at: 2019-05-22T10:34:46.140Z Reads: 172

```
What VESC FW ?
```

---
## \#1155 Posted by: bevilacqua Posted at: 2019-05-22T12:03:37.440Z Reads: 171

```
does someone have the BOM and schematics? links dont work any more

(I have 2 bare PCBs that I would like to use sometime in the near future) 

Thanks
```

---
## \#1156 Posted by: pookybear Posted at: 2019-05-22T13:49:30.582Z Reads: 166

```
I'm using @skatardude10 compiled Vesc fw that has the brake fix. Vesc6.

Here is the  [link.](https://github.com/skatardude10/bldc/commit/010b7ea4e0e7424e313f9b3373eeefdf78820717)
```

---
## \#1157 Posted by: Pimousse Posted at: 2019-05-22T14:05:47.369Z Reads: 170

```
Whatns the brake fix ?
Does he has a github repo where I can check it ?
```

---
## \#1158 Posted by: pookybear Posted at: 2019-05-22T14:09:55.970Z Reads: 169

```
The link is the github. Brake fix was done by deodand. He just merged it w ack FW.
```

---
## \#1159 Posted by: Pimousse Posted at: 2019-05-22T14:50:53.178Z Reads: 173

```
Sorry, I had a (too) quick look and didn't see sources.
What's the improvement in your ride feeling ?

AFAIK, Vedder considered to bring @Deodand code improvement into official firmware.
But IDK if it has been applied in the end.
```

---
## \#1160 Posted by: pookybear Posted at: 2019-05-22T14:53:17.995Z Reads: 173

```
The only real difference is the low speed braking. It doesn't lock up. Well what I read here in the forums, vedder has merged this fix into his official fw. Or he may have just made a fix based on deodands fix. Not sure. I haven't seen the code.

I really like ack FW. Just a better linear ride feel for me.
```

---
## \#1161 Posted by: Surfer Posted at: 2019-05-22T14:54:46.572Z Reads: 167

```
Yes, the deodand brake fix was implemented 3 or 4 iterations before last official firmware
```

---
## \#1162 Posted by: pookybear Posted at: 2019-05-22T14:59:26.781Z Reads: 169

```
Some user was able to compare data between ack and vedders official fw. Based on his findings, better ride control and better battery consumption. 

I'm gonna have to look for that post. Once I find it, I'll post it here.
```

---
## \#1163 Posted by: Pimousse Posted at: 2019-05-22T15:12:05.820Z Reads: 169

```
Ok, I found back where it has been discussed with Benjamin :
https://github.com/vedderb/bldc/pull/69

This has been integrated in official FW since FW 3.48. :+1:
```

---
## \#1164 Posted by: pookybear Posted at: 2019-05-22T15:20:05.411Z Reads: 165

```
Found it. [Here](https://www.electric-skateboard.builders/t/all-new-2019-vesc-tool-release/83619/370?u=pookybear) we go.
```

---
## \#1165 Posted by: skatardude10 Posted at: 2019-05-22T15:29:19.580Z Reads: 175

```
Vedder's fix is similar but different than deodand's fix, if I remember it has something to do with trying to not overload the MCU with 32bit operations or something, and be more compatible with a wider range of motors. 

The choice is obvious if you prefer either Acks or official FW, but otherwise I hear the two fixes feel different, with vedder preferring 'some cogging' or something, dunno. I'd love to hear if anyone has tried both and can compare the feeling. Personally, I think Jeff's fix feels great on Acks but at some point I might swap back to official FW (maybe).
```

---
## \#1166 Posted by: Pimousse Posted at: 2019-05-22T15:34:03.473Z Reads: 176

```
These last weeks, a lot a pull requests have been submitted by different contributors and have been merged. Check the lastest commits, this is huge !
So now the VESC Project tends to be more and more a collective work and we can already see a lot of benefits.
```

---
## \#1167 Posted by: abenny Posted at: 2019-06-06T22:19:42.708Z Reads: 159

```
hey guys, if i were looking to buy a connector for the PPM cable that fits the escape side, what would i google search?
```

---
## \#1168 Posted by: trampa Posted at: 2019-06-07T15:59:47.920Z Reads: 155

```
Benjamin takes his time to work things in. Usually he needs to re-code stuff and improve it, so it's not always a simple merge and therefore consumes some time his end.
Brake FIX suggestion as been implemented some months back. 
Benjamin changed the code, since he found the original implementation do have some "imperfections".
```

---
## \#1169 Posted by: webst Posted at: 2019-11-21T17:49:19.971Z Reads: 98

```
Guys, is there a way Vesc Tool sees MPU9250 gyro data? I checked **App settings** / **General** / **App to use** to No app but IMU app shows no data. Is this because of differences between VESC6 and ESCape? I used VescTool 1.19 which is the latest I could find on MacOS.
```

---
## \#1170 Posted by: Surfer Posted at: 2019-11-21T22:04:07.164Z Reads: 97

```
I solder the mpu in my ESCape and it doesn't show any data, I probably tried every setting available on the last vesc tool, but no success.

Post your findings please , maybe I missed something
```

---
## \#1171 Posted by: webst Posted at: 2019-11-21T22:58:05.610Z Reads: 97

```
Maybe @stewii can shed some light on it?
```

---
## \#1172 Posted by: webst Posted at: 2019-11-22T09:35:37.143Z Reads: 96

```
It just came to me that you soldered it by yourself, Isn’t that already soldered? Stewii up there says he’s using MPU9250 in place of obsolete 9150.

Edit: 
Found it, I was wrong. Seems like question to Benjamin Vedder now. 
[quote="stewii, post:8, topic:37579"]
The difference is that I designed the PCB for the MPU-9250 instead of the 9150 (obsolete) but that chip doesn’t come populated and it is not implemented in the firmware as far as I know.
[/quote]
```

---
## \#1173 Posted by: LukePL Posted at: 2019-11-22T19:38:18.200Z Reads: 92

```
@stewii is long gone and I don't think any one knows what happen
```

---
## \#1174 Posted by: itsrow Posted at: 2019-11-24T22:57:01.326Z Reads: 91

```
Makes me cry everytime I think about it, probably the most successful VESC manufacturer in terms of failure %, disappeared without a trace.
```

---
## \#1175 Posted by: Pimousse Posted at: 2019-11-25T17:17:00.318Z Reads: 86

```
Vesc 6+ and VESC 6 (= ESCAPE) don't share the same pins for IMU.
IMU integration is made for VESC 6+.
So it's impossible to have it working with official FW and VESC Tool.
```

---
## \#1176 Posted by: webst Posted at: 2019-11-25T19:57:56.614Z Reads: 84

```
It certainly is not exclusive to 6+, you can use external IMU with FW 3.60 and VESC Tool 1.18. Not as elegant as I hoped though.
```

---
## \#1177 Posted by: Pimousse Posted at: 2019-11-25T21:08:39.671Z Reads: 82

```
Oh yes, I meant Internal IMU.
```

---
## \#1178 Posted by: Fungineers Posted at: 2020-02-13T11:13:15.107Z Reads: 37

```
hey guys (if anyone is here), does anyone happend to have stewiis BOM? The dropbox link he shared is dead. Thanks!
```

---
## \#1179 Posted by: bigben Posted at: 2020-02-13T20:35:13.598Z Reads: 34

```
There should be the info you need here. 
https://forum.esk8.news/t/escape-comp-sale/18850
@AgressivStreetLamp should have the updated BOM
```

---
## \#1180 Posted by: AgressivStreetLamp Posted at: 2020-02-14T02:19:10.973Z Reads: 31

```
https://www.dropbox.com/s/9tjrxl914y4kfa8/ESCape_files.zip?dl=0
```

---
