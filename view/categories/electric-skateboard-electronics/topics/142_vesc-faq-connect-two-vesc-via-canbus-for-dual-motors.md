# VESC FAQ &#124; Connect two VESC via CANBUS for dual motors

### Replies: 137 Views: 40639

## \#1 Posted by: onloop Posted at: 2015-08-26T05:45:06.301Z Reads: 1974

```
The VESC is designed to control dual motors from one input source. It also offers traction control!

1. In the picture below there is one remote control receiver connected via the Orange, Red & Brown Wires.
------------------------------------------------------------------------

https://cdn1.bigcommerce.com/n-yp39j5/zad02/product_images/uploaded_images/20150522-082329.jpg?t=1432249306


----------


2. You must connect two wires between the VESC's, Run the two wires connecting the two middle pins of the four pin connector. You may buy this connector and just use the two middle pins, its called a "JST-PH 2MM" connector. 
------------------------------------------------------------------------
<img src="/uploads/db1493/original/1X/fd512974e0f361a1edf6f33b492f868b9f2f18fa.jpg" width="669" height="499"> 


----------


3. You need to configure the Firmware using the BLDC tool on your computer. 
------------------------------------------------------------------------
- Go to "App Configuration" tab, 
- Choose input type. For RC controller choose "PPM tab" / For Nunchuck choose "Nunchuck"
- Select "Multiple ESC over Can" 
- Traction control is optional



<img src="/uploads/db1493/original/1X/eb23aa079be16ea4f352a855f33ad90f6a29c0af.jpg" width="690" height="398"> 


----------

4. Now bench test to see if the motors both spin together.
------------------------------------------------------------------------
```

---
## \#2 Posted by: sl33py Posted at: 2015-08-27T00:18:22.473Z Reads: 1620

```
On my to-do list.  Previous dual VESC setup used "Y" servo cable.

Don't forget to uniquely ID each controller.  There are problems if you don't give them different ID's (1/2, 0/1, etc.)
[img]/uploads/db1493/original/1X/4d2d70f9f3c1625375e27c4b7e4b69ff32c39cd4.JPG[/img]
```

---
## \#3 Posted by: onloop Posted at: 2015-09-03T05:44:24.023Z Reads: 1518

```
ALSO NOTE: You need to click this for the slave VESC


<img src="/uploads/db1493/original/1X/6bf4b822eb3f66c38b3e207c4c8f2d0cd7ec285a.jpg" width="690" height="383">
```

---
## \#5 Posted by: lowGuido Posted at: 2015-09-17T07:34:28.457Z Reads: 1410

```
Hey I was just thinking of this.. 
if you are connecting 2 VESC's together a lot of the electronics is probably wasted on the 2nd VESC. wouldn't it be possible to have a VESC daughter board made with basicly just the FETS and related electronics. so all the signaling is done on the main VESC and then the 2nd motor is run by a daughter board signaled from the first VESC.

I dunno.. again I'm just thinking out loud.
```

---
## \#4 Posted by: onloop Posted at: 2015-09-17T08:13:10.314Z Reads: 1389

```
I moved a post to a new topic: [VESC FAQ | Best Settings For Hub Motors](http://www.electric-skateboard.builders/t/vesc-faq-best-settings-for-hub-motors/212)
```

---
## \#6 Posted by: Mitch Posted at: 2015-10-19T08:42:48.782Z Reads: 1371

```
Hey if i connect my remote receiver directly to one of the VESC and then link the two as shown in this post will everything work fine, after programming it correctly of course?
```

---
## \#7 Posted by: Mitch Posted at: 2015-10-19T08:45:28.405Z Reads: 1329

```
Also does anyone know a good website in Australia that sells the the connecting JST-PH 2mm cable? I am struggling to find it
```

---
## \#8 Posted by: elkick Posted at: 2015-10-19T08:51:49.005Z Reads: 1303

```
@Mitch, yes your remote should work. About the connectors: I don't have a source for Australia, but could recommend this reliable guy from Germany shipping worldwide and fast, he has also the same for 4 Pin: http://www.ebay.com.au/itm/KIT-BUCHSE-STECKER-6-polig-pins-2-mm-JST-HEADER-Male-Connector-PCB-A648/262040524714?_trksid=p2045573.c100033.m2042&_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20131017132637%26meid%3D557c647a904e420bb98fff8961370645%26pid%3D100033%26rk%3D2%26rkt%3D4%26sd%3D371296458570
```

---
## \#9 Posted by: Moja Posted at: 2015-11-05T11:56:34.022Z Reads: 1248

```
 I had this setup running really nicely until yesterday. I have the same settings as shown in the above examples. Yesterday I was riding allot and a few times the slave motor wouldn't spin on startup, I restarted the board and things worked fine, then nothing at all. I've been troubleshooting all night and got the motor going a few times then it would stop responding and now I cant get anything from it. 
 I've checked and re-soldered the CANBUS connection, the VESC is on with blue lights (good) and the motor spins on the detection test in BLDC but I can't control the second motor using my GT2B which is connected to the master VESC, Im not getting any pulse width readings in the PPM app, however I do if I am connected to the master VESC. 

 I'd love to hear any suggestions so I can get this thing back up and running for the weekend, single drive sucks after you've experienced the wonders of dual rear :smile:
```

---
## \#10 Posted by: chaka Posted at: 2015-11-05T15:16:46.779Z Reads: 1179

```
While I think it is great that we can use this capability I think splitting the servo signal is still the most robust option.  I recently configured two vesc as a master/slave and encountered the same issues.

I wonder if it works more smoothly using the nunchuk instead of PPM?
```

---
## \#11 Posted by: elkick Posted at: 2015-11-05T18:19:06.894Z Reads: 1141

```
Did you check the motor cables? I had the same issues like you and they were caused by a broken solder spot on one motor connector.
```

---
## \#12 Posted by: Moja Posted at: 2015-11-05T20:39:00.234Z Reads: 1096

```
The motor connections seem solid. From my inspections the hardware seems ok.
```

---
## \#13 Posted by: disastorm Posted at: 2015-11-05T20:40:42.253Z Reads: 1096

```
[quote="chaka, post:10, topic:142, full:true"]
While I think it is great that we can use this capability I think splitting the servo signal is still the most robust option.  I recently configured two vesc as a master/slave and encountered the same issues.

I wonder if it works more smoothly using the nunchuk instead of PPM?
[/quote]
Hi, what does splitting the servo mean ? Do you mean have the wireless receiver input to both of the vescs in parallel as opposed to having them connected via CANBUS ? Does that work ?
```

---
## \#14 Posted by: chaka Posted at: 2015-11-05T21:11:01.060Z Reads: 1035

```
Yes, you split the signal. You have to drop the positive on one so you will only pull power off of one VESC to power the receiver. I think this will disable any traction control though.
```

---
## \#15 Posted by: disastorm Posted at: 2015-11-05T23:19:45.264Z Reads: 1020

```
[quote="chaka, post:14, topic:142, full:true"]
Yes, you split the signal. You have to drop the positive on one so you will only pull power off of one VESC to power the receiver. I think this will disable any traction control though.
[/quote]

I see. What is traction control ? I'll be building mine soon so I want to know what I should do. The issue with CANBUS is that it stops working some time ??
```

---
## \#16 Posted by: chaka Posted at: 2015-11-05T23:25:21.845Z Reads: 986

```
I have only experienced this once so it could be an isolated incident. 

Traction control will sense one will spinning more than the other and reduce current to that motor until they get back in sync.
```

---
## \#17 Posted by: disastorm Posted at: 2015-11-05T23:27:43.689Z Reads: 1002

```
[quote="chaka, post:16, topic:142, full:true"]
I have only experienced this once so it could be an isolated incident. 

Traction control will sense one will spinning more than the other and reduce current to that motor until they get back in sync.
[/quote]
ah I see. I'll probably try to use CANBUS then and I'll switch if I encounter any issues.

Also the issue you describe is independent of the receiver itself? I will be using the Nyko Kama.
 Also just as a general question, if splitting the signals, the current into each VESC connector would be cut in half right? Does the VESC still work fine in that case?
```

---
## \#18 Posted by: chaka Posted at: 2015-11-05T23:31:16.993Z Reads: 956

```
You can wire the nyko kama dongle directly to the VESC and join them using the CANBUS.
```

---
## \#19 Posted by: disastorm Posted at: 2015-11-05T23:35:18.086Z Reads: 979

```
[quote="chaka, post:18, topic:142, full:true"]
You can wire the nyko kama dongle directly to the VESC and join them using the CANBUS.
[/quote]
Yes thats what I planned on doing. Was the issue you were referring to only applicable to the G2B controller ?
```

---
## \#20 Posted by: chaka Posted at: 2015-11-06T01:30:01.445Z Reads: 978

```
I had some issues using the PPM with communication enabled. You will be using the nunchuck option, might be more stable.
```

---
## \#21 Posted by: Moja Posted at: 2015-11-06T08:11:16.176Z Reads: 929

```
The GT2B is really reliable for build quality and signal connection but the nunchuck is awesome for cruise control and the form factor. When you are carving hard, the combination of cruise control and traction control makes for an awesome ride,  the power gets switched from motor to motor really intelligently making carving on flat ground feel very natural. 

Anyone got any ideas how I can sort out the communication error with CANBUS in PPM mode?
```

---
## \#22 Posted by: kai Posted at: 2015-11-10T21:52:03.951Z Reads: 909

```
Noob question. So the batteries just need to connect to 1 vesc and the canbus connection delivers power to the second one? Or does the battery need to be connected directly to both?
```

---
## \#23 Posted by: onloop Posted at: 2015-11-10T21:52:57.545Z Reads: 889

```
each vesc must have a power supply, canbus is just a data/communications conecction
```

---
## \#24 Posted by: kai Posted at: 2015-11-10T21:58:08.080Z Reads: 866

```
so i need a splitter from space cell with 1 female and 2 male xt60 connectors?
```

---
## \#25 Posted by: onloop Posted at: 2015-11-10T22:19:16.126Z Reads: 854

```
you don't really need extra XT60 just solder two vesc power leads together onto one xt60 connector (++) & (--)
```

---
## \#26 Posted by: kai Posted at: 2015-11-10T23:03:58.275Z Reads: 837

```
Never thought of that. Thanks @onloop
```

---
## \#27 Posted by: trbt555 Posted at: 2015-11-11T08:44:47.837Z Reads: 823

```
Slightly off-topic, I think you can get away with only one set of capacitors if you interconnect the VESC's locally and run only 2wires from the battery.
```

---
## \#28 Posted by: lowGuido Posted at: 2015-11-11T11:37:54.267Z Reads: 816

```
Im not sure that you can.

Edit. I mean you can. But its probably not recomended.
```

---
## \#29 Posted by: onloop Posted at: 2015-11-11T22:15:51.705Z Reads: 814

```
i think a single vesc could still be ok with just 500uf cap, it really depends how long/skinny your battery wires are.

If the battery is nice & close you can have lower. i think over 1000uf per vesc is a safe bet.
```

---
## \#30 Posted by: kai Posted at: 2015-11-30T12:47:19.902Z Reads: 803

```
Did you get that sorted out yet @moja ? Another noob question... do you do motor detection after you slave the vesc? Or do i do them indivisually and then slave the vesc?
```

---
## \#31 Posted by: Jeff Posted at: 2015-11-30T15:40:50.752Z Reads: 807

```
I have a dual VESC set up via CANBUS. I was experiencing some issues with the slave not connecting when I just used plug in connectors. However, I have had no issues whatsoever after I soldered the wires directly to the pins and put heatshrink in-between. 

I setup the XML file with the master VESC and simply copied it over to the slave making sure I changed the controller ID number. Works great.
```

---
## \#32 Posted by: chaka Posted at: 2015-12-11T19:45:27.839Z Reads: 817

```
I made a listing for the CANBUS link: [CANBUS Connector for Vedder's Motor Controller][1]
I have been getting tons of request for this item. .

<img src='/uploads/db1493/original/2X/5/5c36f0a4f7c2cab858f7b15ea6826bf982739bed.jpg'>


  [1]: http://www.ollinboardcompany.com/product/canbus-connector-for-vedder-s-motor-controller
```

---
## \#33 Posted by: jakeyb2525 Posted at: 2015-12-11T20:28:53.381Z Reads: 777

```
can you add one to my order please @chaka :+1:
```

---
## \#34 Posted by: torqueboards Posted at: 2015-12-13T05:59:22.888Z Reads: 778

```
Awesome connector! Well needed.
```

---
## \#35 Posted by: sgaana Posted at: 2016-01-10T23:54:51.083Z Reads: 809

```
@sl33py @EnertionSupport I have my Project Zephyr powered up (both VESC blue and green lights are on, Canbus properly placed, checked all wires).  But was able to spin only one motor? How do you identify each VESC ?  It seems that I can configure only one VESC ! I know that you should assign ID 0 to the master and 1 to the slave. After you configure the master, how to do save it and then move to the slave?
<img src="/uploads/db1493/original/2X/2/21228613a5ce463fab3252d09280d1b7b94912a8.png" width="690" height="417">
<img src="/uploads/db1493/original/2X/a/a5126c6017290147f3f5175163da57dbd45fa8d1.png" width="640" height="480">
```

---
## \#36 Posted by: trbt555 Posted at: 2016-01-11T06:08:54.973Z Reads: 774

```
You need to configure them individually via USB. You can't do it over CAN.
After that you can check CANbus communication by connecting to the master, clicking CAN FWD, entering the slave's ID on the upper right of your screen and checking if realtime data is coming back from the slave.
```

---
## \#37 Posted by: trbt555 Posted at: 2016-01-11T12:03:12.171Z Reads: 769

```
Oh yeah, and please put some tape or heat shrink on those capacitor boards. Unless you like sparks and smoke ;-)
```

---
## \#38 Posted by: sgaana Posted at: 2016-01-11T15:37:41.417Z Reads: 808

```
Thanks. This looks better. 
<img src="/uploads/db1493/original/2X/2/2a37f3be0b2813e90e4258d858a60d11c912dc41.jpeg" width="666" height="500">
```

---
## \#39 Posted by: NIK Posted at: 2016-01-13T11:07:44.829Z Reads: 835

```
When u say that it is better if we split the servo receiver cable, does it means that only one receiver wire going to just one vesc or splitting into 'y' servo wire? Thanks
```

---
## \#40 Posted by: NIK Posted at: 2016-01-13T12:45:38.573Z Reads: 892

```
Hi guys, what is the id that we must put in? Or do we have specific id or just randomly? Thanks
```

---
## \#41 Posted by: chaka Posted at: 2016-01-13T14:45:31.518Z Reads: 879

```
You are using a nunchuk so you will need to use the canbus to control the second VESC. I have not tried splitting the leads on a wii dongle yet but it may work. Better to use the canbus though.

If you where using a conventional FHSS transmitter you could split the receiver output leads and control both VESC through the ppm input. Be sure to only have the red wire coming from one vesc if you do this.
```

---
## \#42 Posted by: NIK Posted at: 2016-01-13T15:59:26.488Z Reads: 877

```
This is my setup. Actually I just want to try and see what happen if I didnt do the setting as previous comment. But yeah, I've encountered some problem such as one of the motor suddenly stuck or pause. Maybe because I didnt put any ID or set the slave or master. 

This is my dual setup picture and @chaka , that means I need to cut which wire? because im using a bit different color for the wire and got confused. Im also using 2.4ghz mini controller.

<img src="/uploads/db1493/original/2X/2/251d5a1451373f39fefda556bdc0dfeb1153b29e.JPG" width="429" height="500">
```

---
## \#43 Posted by: chaka Posted at: 2016-01-13T16:11:23.113Z Reads: 823

```
The center wire needs to be cut on just one. Leave it on your master vesc, it powers the receiver.
```

---
## \#44 Posted by: NIK Posted at: 2016-01-13T17:09:21.013Z Reads: 821

```
When @onloop says that we need to click the send status over CAN for the slave. Just to make it clear, u need to tick or no tick it? haha sorry for my bad English.
```

---
## \#45 Posted by: NIK Posted at: 2016-01-13T17:15:07.481Z Reads: 837

```
When I cut the slave, red wire, the receiver didn't get power at all. Maybe I'm doing it the wrong way. 

<img src="/uploads/db1493/original/2X/b/b711346968845b6427ca3753b56d3391434d00e4.JPG" width="375" height="500">
```

---
## \#46 Posted by: chaka Posted at: 2016-01-13T17:19:41.724Z Reads: 805

```
[quote="chaka, post:43, topic:142"]
Leave it on your master vesc,
[/quote] :confused: Unless you have a ubec/sbec around. The center wire powers the receiver and the power should come from only one source.
```

---
## \#47 Posted by: NIK Posted at: 2016-01-13T17:24:12.115Z Reads: 824

```
haha i dont know about BEC/SBEC. I have 2 VESC and 2.4GHz mini controller. 

and this is my BLDC setting for master and slave:

Master 1

<img src="/uploads/db1493/original/2X/a/abf4113660eb9046a0e655e257063fe98cd77e03.JPG" width="690" height="400">

<img src="/uploads/db1493/original/2X/5/53785b7349afe5f2517f9056ccb65a5673b25057.JPG" width="690" height="403">

Slave 

<img src="/uploads/db1493/original/2X/f/f0e175aecf2bb7444e24ecd8cfd172e2b954a459.JPG" width="690" height="401">

<img src="/uploads/db1493/original/2X/9/9357fb05f9e5bed31b91d66b66c95342618f484f.JPG" width="690" height="402">
```

---
## \#48 Posted by: NIK Posted at: 2016-01-13T17:25:28.736Z Reads: 726

```
and I am planning to make the VESC on the right my master and left is my slave VESC
```

---
## \#49 Posted by: BigAl Posted at: 2016-01-14T03:50:51.246Z Reads: 748

```
What @chaka is saying is that you cut the red wire coming from one of the VESC and leave the other connected.  You see, the red wire is what feeds power to the receiver.  You only need the power to come from one of the VESC, it doesn't matter which VESC the power comes from but the receiver should only receive power from one of the VESCs.

Hope that helps.
Al...
```

---
## \#50 Posted by: trbt555 Posted at: 2016-01-14T06:25:49.336Z Reads: 760

```
If you're using CAN bus in a master/slave configuration, the receiver should only be connected to the master.

First you need to make sure both VESC's are working properly by connecting each one to the BLDC tool and using the arrow keys on your keyboard to run the motor. Once you're sure they are both OK, you can set up CAN bus:

 - Connect master to BLDC, give the master ID 0, configure the PPM settings (write conf) for your receiver and test to see if your motor runs. Don't connect the slave to the master yet. Put your transmitter aside.
 - Connect the slave to BLDC and give it ID 1 and tick " send status over CAN" - (write conf).
 - Disconnect the slave from BLDC.
 - Connect both VESC's with the CAN bus cable.
 - Cycle the power on both VESC's off an on.
 - Reconnect the master to BLDC and tick "CAN Fwd" on the upper right of your screen, enter ID 1 To receive data from slave.
 - Goto the realtime data tab, tick "activate sampling" and verify there's data coming back from the slave. You should see the graphs move. If they don't, there's no communication.
 - Now take your transmitter and pull the trigger to see if both motors spin.

Hope this helps
```

---
## \#51 Posted by: Evan Posted at: 2016-03-20T08:54:56.925Z Reads: 714

```
<img src="/uploads/db1493/original/2X/e/e46ae5f2c131abcc5707cd2d3db557b03d2007f1.jpg" width="690" height="388">


So according to Raptor board, the dual vesc setup with non-Nyko Kama (or NunChuck) receiver should be like this?

No need to connect both vesc's receiver side? Then how to know or decide which side is master one?
```

---
## \#52 Posted by: Evan Posted at: 2016-03-20T09:14:05.206Z Reads: 704

```
<img src="/uploads/db1493/original/2X/a/a6f92a220f603e89f567125f88dac21922b44893.jpg" width="666" height="500">

[enter link description here][1]


  [1]: https://www.youtube.com/watch?v=Vg8-nZlSeDY



Another proof which shows only need one side connecting to receiver?!
```

---
## \#53 Posted by: trbt555 Posted at: 2016-03-20T12:23:55.737Z Reads: 680

```
Correct, If you're using CANbus, the receiver is connected to the master only.
The app for the receiver is configured only in the master.
The master takes care of the control of the slave.
```

---
## \#54 Posted by: Evan Posted at: 2016-03-21T09:45:50.529Z Reads: 679

```
Thanks, that means WITH the CANbus setup, the one connected to the receiver becomes the master one?

So is that possible to do a different way on dual Vesc which like old esc setup that "without CANbus then connected both receiver side with the 'Y' bridge then take one side's middle wire out"

Learned those setup from : http://2bfly.com/knowledgebase/electronic-speed-controls/multi-engine-esc-wiring/
```

---
## \#55 Posted by: lowGuido Posted at: 2016-03-21T18:58:33.910Z Reads: 669

```
you have to program the master and slave in the BLDC tool software.

or you can set them up as 2 individual ESCs and use a Y if you prefer that.
```

---
## \#56 Posted by: Evan Posted at: 2016-03-22T05:42:57.662Z Reads: 654

```
[quote="lowGuido, post:55, topic:142"]
or you can set them up as 2 individual ESCs and use a Y
[/quote]
Okay! So there are not big differences, are they? I mean these two setup.
```

---
## \#57 Posted by: trbt555 Posted at: 2016-03-22T06:17:08.317Z Reads: 661

```
If you use a Y connection You won't have traction control but I'm pretty sure you wont miss it. 
You won't be able to get realtime data from both vescs over the same usb connection either, you'll need to plug into each vesc separately to look at realtime data.
It will make config straightforward though, you can set both vescs up identically.
```

---
## \#58 Posted by: Evan Posted at: 2016-03-22T06:56:12.679Z Reads: 652

```
Very helpful info mate. Thank god I've asked those question. Didn't even know that before. Then now I know what setup I'm going to run in future. Cheers!
```

---
## \#59 Posted by: deadlyrobot310 Posted at: 2016-03-29T01:56:31.185Z Reads: 659

```
Hello Everyone,

I heard that the VESC is open source which raises the questions.
1) does the VESC have extra I/O pins available, and if so is there a way to program these pins.
2) does anyone have a schematic for the VESC, would like to take a look at the hardware
```

---
## \#60 Posted by: torqueboards Posted at: 2016-03-29T04:53:17.059Z Reads: 668

```
@deadlyrobot310 - http://vedder.se/2015/01/vesc-open-source-esc/ Check here...
```

---
## \#61 Posted by: lowGuido Posted at: 2016-04-08T14:08:22.347Z Reads: 629

```
I have noticed with my dual VESC's (via canbus) that if I'm on cruise control and I load up one wheel the motor spins up harder to try and overcome the load, but if I load the other wheel it just stops.
I have tried turning on and off traction control option and it doesn't seem to make a difference.
its the motor attached to the slave VESC that stops under load.

is there some sort of setting that I'm missing?
```

---
## \#62 Posted by: lowGuido Posted at: 2016-04-18T01:03:23.625Z Reads: 602

```
found the issue, it looks like it was a faulty canbus cable.
```

---
## \#63 Posted by: jacobbloy Posted at: 2016-05-06T09:41:38.039Z Reads: 589

```
Traction control if found doesn't work as well for hub motors any way!
```

---
## \#64 Posted by: laurnts Posted at: 2016-05-06T10:05:13.120Z Reads: 588

```
I thought so too, but it think the setting needs to be changed from 3000 erpm differences to lower number I suppose.
```

---
## \#65 Posted by: lowGuido Posted at: 2016-05-06T10:15:09.389Z Reads: 577

```
Yeah i hadn't put traction control on, I did have a faulty canbus cable though.
```

---
## \#66 Posted by: jacobbloy Posted at: 2016-05-06T10:54:31.450Z Reads: 581

```
good job you fixed it
```

---
## \#67 Posted by: laurnts Posted at: 2016-05-11T19:29:08.271Z Reads: 588

```
Does anyone know if its okay to have slightly different parameters in motor integrator limit as well as BEMF coupling on dual motor configuration.

After running detection, I have 2 results

Left motor:
Integrator Limit 95
BEMF Coupling 650

Right motor:
Integrator Limit 90
BEMF Coupling 600

Should be left and right motor configuration the same? or should it be different according to the uniqueness of each motor?
What re the implications if they are different? or if I average them and have them on the same value?
```

---
## \#68 Posted by: Nordle Posted at: 2016-06-01T05:33:58.409Z Reads: 577

```
Just give this a little push, cause I would like to hear the answer to Laurnts question.
And say hello to this community:)
```

---
## \#69 Posted by: Riako Posted at: 2016-06-02T13:45:05.243Z Reads: 582

```
https://monlongboardelectrique.files.wordpress.com/2016/01/setup_emtb_cablage_b.jpg?w=1000
... if it could help ...
```

---
## \#70 Posted by: flatsp0t Posted at: 2016-06-02T14:12:07.728Z Reads: 579

```
No, this is perfect, no motor is like the other and the values are near enough.
```

---
## \#71 Posted by: treeme Posted at: 2016-06-04T17:40:20.446Z Reads: 581

```
Hi All,

I seem to be running into an issue with the dual motor setup I've changed using the BLDC Tool. 

I'm using an Enertion Dual Raptor, so I've got two VESCs (4.12) controlling it. My goal is to change it to FOC mode. For that reason, I got the BLDC tool (V2.15), and changed the firmware on the VESCs from 2.16 (default) to 2.15 (compatible with 2.15, couldn't find firmware 2.17 or 2.18). I managed to change 1 to FOC mode, but the other one seems to be unresponsive. When I try measuring the motor configuration settings for FOC, it doesn't do anything at all. Some of the strange things I notice are the resistance is about 300x as much on the motor that doesn't do anything than the one that functions (.02 vs 6.3). The strange part is I can connect using CAN forwarding (set master to one, slave to 2, can connect from either to the other. 

As for settings for the app, I set the master one to send status over CAN (if slave sends status over can, the one motor that does work gets conflicting signals). In PPM mode (since I'm using a steez remote), I set the multipl escs over can on both, then I tried disabling control on the slave, then enabling multiple over can. Nothing seems to work. Any one have a suggestion what I should try next?
```

---
## \#72 Posted by: flatsp0t Posted at: 2016-06-04T17:55:11.773Z Reads: 552

```
Does the other still work with bldc mode?

Sometimes there occur some problems on firmware flashing.
```

---
## \#73 Posted by: treeme Posted at: 2016-06-04T22:38:29.136Z Reads: 556

```
Just uploaded the VESC enertion 6355 firmware on the "bad" VESC.. Every time I try reading the configuration from the motor, I get a bad detection code:

<img src="/uploads/db1493/original/2X/b/b56559f39deb2b754b80d5b664ec774dcbd855ad.png" width="690" height="315">
```

---
## \#74 Posted by: treeme Posted at: 2016-06-04T22:40:17.189Z Reads: 549

```
And the other one can be read without problems:

<img src="/uploads/db1493/original/2X/4/46a2f0c5981eb4d8c2c8762cf08d5c51d4b65e45.png" width="517" height="500">
```

---
## \#75 Posted by: treeme Posted at: 2016-06-04T23:01:57.175Z Reads: 553

```
To add more detail, I know there's the VESC faq posted [here](http://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672?u=treeme) that talks about what to do, but in making the board, there this black epoxy sort of stuff that prevents me from checking the wire connections to the motor.

That being said, here is the current/duty graph which makes me convince it's a bad motor/bad motor connection:

<img src="/uploads/db1493/original/2X/d/d91612ebaee8a9d0fbf8e835f8c535bc9dedc6a6.png" width="690" height="361">
```

---
## \#76 Posted by: trbt555 Posted at: 2016-06-05T16:02:11.379Z Reads: 549

```
Switch the motors, if the problem follows the suspect motor, it's the motor.
Otherwise it's the vesc.

Go back to bldc mode.
Manually Copy the settings from the good vesc to the suspect vesc and see if it still runs in bldc.
```

---
## \#77 Posted by: treeme Posted at: 2016-06-05T16:39:03.500Z Reads: 557

```
I would, but there's this black epoxy that's on the board that prevents me from doing anything: <img src="/uploads/db1493/original/2X/6/6abb27781a1e9730e2298603d97a41bbdc619672.png" width="281" height="500">

@EnertionSupport, Do you have suggestions on how I can  unglue this or maybe have it sent in to be checked on if you have to have special tools for this?
```

---
## \#78 Posted by: flatsp0t Posted at: 2016-06-05T16:47:52.262Z Reads: 534

```
it is just hot glue
```

---
## \#79 Posted by: Strawbs Posted at: 2016-06-20T22:39:25.967Z Reads: 550

```
I'm having trouble finding these connectors in any store or online without buying 20+

I found these at hobby people (see below)

I bought (2) Female JST connectors and plan to solder them together to create the female to female connection.

Will this work?

<img src='https://mail.google.com/mail/u/0/?ui=2&ik=3f013a4819&view=fimg&th=1556feedec91ea78&attid=0.1&disp=emb&attbid=ANGjdJ93OXoPd2lhEVdVaztzvvaiL6YK4TQaomfLrAva3jxu4a8Kq-eftx_C2Us3XhPUQP7nQmr9MjKGeRAGiX0iIMhG4KOHLY21z1xGDyVEE2aEWUvHLlWNpxI9Q_Y&sz=s0-l75-ft&ats=1466461928311&rm=1556feedec91ea78&zw&atsh=1'>
```

---
## \#80 Posted by: Jinra Posted at: 2016-06-20T22:50:51.299Z Reads: 554

```
You can get one of these and cut/ignore the last cable

http://www.getfpv.com/male-to-male-servo-extension-cable-26awg-jr-style-5-pcs.html

BTW, your picture is broken.
```

---
## \#81 Posted by: Strawbs Posted at: 2016-06-20T23:02:53.420Z Reads: 548

```
Sorry,  How about this one...

<img src="/uploads/db1493/original/2X/1/19bc36f27e6abdea7f875d07da9a4b2cb3bc9abf.jpg" width="640" height="480">
```

---
## \#82 Posted by: Jinra Posted at: 2016-06-20T23:05:29.003Z Reads: 526

```
yea that'll work too
```

---
## \#83 Posted by: Strawbs Posted at: 2016-06-20T23:10:57.365Z Reads: 517

```
Cool thanks!
```

---
## \#84 Posted by: Adam0311 Posted at: 2016-07-18T06:23:45.768Z Reads: 512

```
Have the dual raptor and had the slave VESC go down on me. Replaced bad enertion VESC with new Ollin VESC. The older master VESC is firmware 2.8, new Ollin VESC is 2.17...do I need to update firmware on older VESC before I can connect via canbus?
```

---
## \#85 Posted by: trbt555 Posted at: 2016-07-19T08:09:10.477Z Reads: 510

```
It makes sense to have them both on the same firmware version given the fact one will be controlling the other.
```

---
## \#86 Posted by: Adam0311 Posted at: 2016-07-19T15:32:43.457Z Reads: 508

```
It actually seems to be working ok, but I think I'll update the old VESC just to make sure.
```

---
## \#87 Posted by: Titoxd10001 Posted at: 2016-07-20T01:11:58.069Z Reads: 501

```
Once they're connected via canbus how do I make changes in bldc tool?
```

---
## \#88 Posted by: xxlv Posted at: 2016-07-25T21:13:41.970Z Reads: 501

```
Here is a detailed howto:
http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/
```

---
## \#89 Posted by: JTAG Posted at: 2016-07-25T21:31:15.288Z Reads: 515

```
You can configure a CAN adres uniquely for each ESC in the "app" tab. For the master ESC (the one that receives the signal from the remote) I set the adres to 0, for the slave ESC I set the adres to 1. 

Once the above settings are applied you can acces both esc's trough the single USB port on for example the master ESC (the one with adres 0):

To connect to the master ESC, uncheck "CAN Fwd" (default mode) and click connect -> you are now configuring the master ESC.

If you want to connect to the other ecs over the CAN simply set the box left to the "CAN Fwd" checkbox to 1 and then check the "CAN Fwd" box. BLDC tool should now give the green connected notification.

You can now switch between both esc's by checking and un-checking the "CAN Fwd" box. Be not to write the same app config to both esc's, then you'll have to reconfigure the CAN addres again to make them different again.
```

---
## \#90 Posted by: Titoxd10001 Posted at: 2016-07-26T22:29:45.258Z Reads: 481

```
@JTAG thanks for the explanation I went back to a y cable due to frustration and found out I was having trouble due to over voltage on my slave vesc so I increased my max voltage to 57v for 12s. I will go back to can bus now that I see it's easy to make changes in bldc tool.
```

---
## \#92 Posted by: MicroRAsus Posted at: 2016-08-13T04:44:08.855Z Reads: 458

```
Do I need to do motor detection on slave vesc?
```

---
## \#93 Posted by: Skitzor Posted at: 2016-08-13T12:48:29.640Z Reads: 453

```
yes on both vescs !
```

---
## \#95 Posted by: wilsonrott Posted at: 2016-09-03T01:03:05.127Z Reads: 440

```
Hay gays I just got a vesc (from enertion)and i set it up with 10s lipo 5000mah sk3 245kv motor and it work for a little bit but know when I pull the throttle the vesc flashes red three (3) times in two (2) groups so like --- ---. dose any one know what this error code is and know how to fix it.
```

---
## \#96 Posted by: ed713 Posted at: 2016-09-03T02:47:21.600Z Reads: 439

```
Hey man. You're going to have to plug your VESC into the computer and check using the BLDC tool.
```

---
## \#97 Posted by: wilsonrott Posted at: 2016-09-03T03:49:57.459Z Reads: 452

```
thank you for your response.

check what?
```

---
## \#98 Posted by: ed713 Posted at: 2016-09-03T04:13:38.915Z Reads: 471

```
Go into the terminal tab and type "faults", and then enter.
```

---
## \#99 Posted by: Daniel Posted at: 2016-09-18T19:43:03.774Z Reads: 464

```
I plugged as on pictured.
I have a problem with the settings.
I was looking at forum but no concrete and my english language is poor
Can I please about photos correct settings for: VESC 1 (PPM), VESC 2

<img src="/uploads/db1493/original/3X/a/b/abf434a994f3560287859e7da1454e58f29bf58d.jpg" width="600" height="499">
```

---
## \#100 Posted by: Daniel Posted at: 2016-09-18T19:59:03.725Z Reads: 455

```
http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/   very good
```

---
## \#101 Posted by: Alexander Posted at: 2016-09-18T20:09:36.091Z Reads: 461

```
How does one tackle hot glue? My gut says heat but better safe than sorry lol I ask as I'm about to swap out the receiver from a new Raptor and it's also got this black glue securing things in place..
```

---
## \#102 Posted by: Daniel Posted at: 2016-09-19T22:53:10.241Z Reads: 457

```
I dont know whats wrong
I made a film https://www.youtube.com/watch?v=hjYoYlA6ETw
```

---
## \#103 Posted by: JCribb Posted at: 2016-10-08T03:39:23.727Z Reads: 422

```
can you run 2 vest's over can if they ere different version, 4.10 to a 4.12, something must have happened to one of my vests when putting it inside the enclosure, am using 2x 4.10 but since one doesn't turn on I might have to get a new one. I heard a spark nothing major and now only one of the vesc turns on, is there something I could have blown? I m running dual motor 12s 12ah custom cnc ali board.
```

---
## \#104 Posted by: jehugarcia Posted at: 2016-10-17T06:05:56.241Z Reads: 407

```
Is it possible to kill both your VESCs by connecting the CAN bus cable before setting one to Master and the other to Slave?   Both motors spun up for a moment and then the slave stopped.  So I power cycled both VESCs  and they DO NOT POWER UP anymore.   NO lights but they do provide power the receiver.   Using 12S currently at 47V
```

---
## \#105 Posted by: ralphy Posted at: 2016-10-17T20:05:48.342Z Reads: 396

```
is this the only way to do it?
```

---
## \#106 Posted by: Tuomalar Posted at: 2017-01-27T23:30:51.315Z Reads: 353

```
Any idea where I can find these jst ph canbus connectors with 4 pins from EU?
```

---
## \#107 Posted by: rwxr Posted at: 2017-01-27T23:41:26.480Z Reads: 362

```
I have a spare one I can send you on monday from sweden if you pay postage
```

---
## \#108 Posted by: Tuomalar Posted at: 2017-01-28T00:16:37.818Z Reads: 364

```
Sent you PM
```

---
## \#109 Posted by: Jebe Posted at: 2017-03-03T09:22:13.824Z Reads: 350

```
any answer to this?
was this an enertion vesc?
```

---
## \#110 Posted by: tonystark Posted at: 2017-03-03T18:01:52.818Z Reads: 357

```
do i have to power 2 vesc to do that or only one of them?
```

---
## \#111 Posted by: Blasto Posted at: 2017-03-03T18:21:57.529Z Reads: 384

```
[quote="jehugarcia, post:104, topic:142, full:true"]
Is it possible to kill both your VESCs by connecting the CAN bus cable before setting one to Master and the other to Slave?   Both motors spun up for a moment and then the slave stopped.  So I power cycled both VESCs  and they DO NOT POWER UP anymore.   NO lights but they do provide power the receiver.   Using 12S currently at 47V
[/quote]

If you short the CAN bus, it will destroy U401 (can bus transceiver) on both vesc. U401 tends to die short, putting the buck converter in to an OVC (over current state)... result, no leds on both vesc.

solution: replace U401, DO NOT try to solder directly on to the CAN bus, no mater how good you think your soldering skills are, if the wires touch, silent death for U401. 

Do it proper and make a cable:

[you need 2 JST PH housing](http://www.digikey.com/product-detail/en/jst-sales-america-inc/PHR-4/455-1164-ND/608606)

[2 pre-crimped JST PH wires](http://www.digikey.com/product-detail/en/jst-sales-america-inc/APAPA22K152/455-3085-ND/6009461)
```

---
## \#112 Posted by: Mike_Lemon Posted at: 2017-06-22T18:26:53.423Z Reads: 329

```
I'm also having problems with this thing had the CAN bus destroyed on both and got replaced with this IC 
https://www.aliexpress.com/item/5pcs-VP232-SN65HVD232D-SOP8-100-new-original-IC/32739398720.html?spm=2114.13010608.0.0.xovMCA

Now when I check that CAN Fwd after connecting from the Master and set  the CAN ID to 1(Slave's can id)
It just disconnects from the BLDC tool.
Also nothing manages to sync

What should I do?

Is there a good way to check if the can bus ICs are good?
```

---
## \#113 Posted by: Stefan Posted at: 2017-06-22T20:53:12.863Z Reads: 320

```
Maybe you have send status over can enabled on both vescs. This was the problem for me when i tried to connect to the second vesc over can fwd.
```

---
## \#114 Posted by: Mike_Lemon Posted at: 2017-06-22T23:24:16.578Z Reads: 312

```
Actually I've confirmed that it's not several times and still...
```

---
## \#115 Posted by: Stefan Posted at: 2017-06-22T23:40:31.670Z Reads: 311

```
Did you double check the have different IDs?
```

---
## \#116 Posted by: Mike_Lemon Posted at: 2017-06-23T00:17:34.128Z Reads: 308

```
Yes
(just filling it up so I can post it)
```

---
## \#117 Posted by: Stefan Posted at: 2017-06-23T00:19:51.862Z Reads: 304

```
Doesn't sound good to me..
```

---
## \#118 Posted by: Macmak Posted at: 2018-02-14T23:36:44.425Z Reads: 230

```
[quote="chaka, post:16, topic:142"]
I have only experienced this once so it could be an isolated incident.
[/quote]

Please elaborate. I'm having a similar problem: 2-motor setup connected via can bus working fine and suddenly the slave went dead. The can bus tested fine. 

As a work around, I split the remote signal which now goes to both VESCs and got both motors working again.
```

---
## \#119 Posted by: Riako Posted at: 2018-02-15T03:05:19.549Z Reads: 237

```
got same pb this summer with the v6 beta,... under bldc mode, the slave dead some times (1 time every 10 ride approx. ). I notice that it happened after stop (or long stop), want to start up and ... hummm it feel less powerefull sudently ! I turn it off and on and is good, sometime it do nothing ... and rework after 2 or 3 times switching ...
I have report that this summer when it happened but no feedback about that ...
I upgrade the fw and now I doesn't happened seens a while ...
Try to reput and reconfigure your setup maybe if it happened again.
Sorry for the poor help :blush:
Good luck !
```

---
## \#120 Posted by: Bjork3n Posted at: 2018-04-14T16:19:57.691Z Reads: 207

```
If you are connected with canbus and you get a fault on the slave vesc would you see this in the app if Uart is connected to the master?

And if i write in terminal "faults" will it search for faults just on the master or both?
```

---
## \#121 Posted by: Redfire1 Posted at: 2018-04-19T19:05:11.191Z Reads: 195

```
@chaka I have 2 mayteck vesc and cannt used the BLCD tool,so I was sent one mayteck tool,I connect t he can bus only one motor spin so i used a Y connector cause I dont have any clue will it cause and damage to my vesc.
```

---
## \#122 Posted by: briman05 Posted at: 2018-04-19T22:05:04.017Z Reads: 196

```
@chaka is not on here anymore technically he posted something about it around Christmas time because Ollie Boards was so busy.
```

---
## \#123 Posted by: Redfire1 Posted at: 2018-04-20T04:30:34.737Z Reads: 179

```
@briman05 do have any idea about my problem please ?.
```

---
## \#124 Posted by: briman05 Posted at: 2018-04-20T11:53:28.121Z Reads: 170

```
Will it not connect to the computer? I’m not understanding what the issue is. It could be that the firmware on your version of bldc tool is not compatible with your vesc
```

---
## \#125 Posted by: Redfire1 Posted at: 2018-04-20T12:56:14.884Z Reads: 165

```
Maybe my vesc is from mayteck and she said I should use vesc tool but I can’t connect my vesc with the can bus cable it don’t work so I am using a Y connector
```

---
## \#126 Posted by: briman05 Posted at: 2018-04-20T13:07:28.983Z Reads: 165

```
So maybe you blew out your can port if it was connected wrong. Download the bldc tool from Vedders website
```

---
## \#127 Posted by: Redfire1 Posted at: 2018-04-20T15:06:49.664Z Reads: 163

```
When I connect them there is light in both but only one turn,I used the can bus  cable from the supplier.how could I connect them wrong ?.
```

---
## \#128 Posted by: briman05 Posted at: 2018-04-20T15:17:46.052Z Reads: 166

```
When you are configuring then in the bldc tool you do each one separate with a id of 0 for the master and 1 for the slave and then you disconnect plug them both in with can bus connected and then power them on both at the same time.
```

---
## \#129 Posted by: Berlad180 Posted at: 2018-04-22T10:44:37.239Z Reads: 168

```
Could you please show what you mean by adding a heat sink between them ? you mean on the Vesc Mosfet ?
```

---
## \#130 Posted by: luis99945 Posted at: 2018-04-22T12:49:02.691Z Reads: 173

```
it is not possible for my two engines to spin even if I put that configuration
```

---
## \#131 Posted by: ramon Posted at: 2018-04-24T13:35:39.340Z Reads: 171

```
Hi, I was thinking on adding a second vesc to my board since I have two motors (motors are the same model), but the vesc I bought back then is not for sale anymore. Do you know if using different vesc's would be possible (as long as they are both vesc's and they both suppor CANBUS connexion)?
```

---
## \#132 Posted by: rey8801 Posted at: 2018-04-24T13:37:44.763Z Reads: 180

```
it's always better to have same vesc but it is possible. Keep the same hardware.
```

---
## \#133 Posted by: Benjamin899 Posted at: 2018-06-03T00:52:40.426Z Reads: 155

```
I am thinking to do the same as @ramon , i bought a focbox and now i want to go dual with a second vesc from maytech/flipsky, would that work if they have the same firmware? Since the hw on focbox is 4.12 anyway right? or did i get that wrong?
```

---
## \#134 Posted by: rey8801 Posted at: 2018-06-03T06:30:33.903Z Reads: 157

```
As far as I know it's possible. Of course better to have the same one for full compatibility. Make sure you have same firmware on both and should be fine. I do not know if in this case it's better to use split signal instead of can bus connection. I think can bus should work just fine. Of course you need to limit the spec based on the weaker vesc.
```

---
## \#135 Posted by: Benjamin899 Posted at: 2018-06-03T12:12:45.867Z Reads: 154

```
ty for the answer. good thing is there are not a lot of hills where i live, i am quite light so the shared load will never rly be a problem even for the weaker vesc.
```

---
## \#136 Posted by: rey8801 Posted at: 2018-06-03T12:18:02.517Z Reads: 158

```
No but it's important that you set the current limit based on that. So for instance all the maytech, TB vesc work fine with a battery max at 30A (at most) while FOCBOX can handle more. You will have plenty of power with dual vesc at 30A, do not worry about it
```

---
## \#137 Posted by: jackluis Posted at: 2018-08-12T20:08:05.796Z Reads: 120

```
Did ever get this fixed? I'm having exactly the same problem. Thanks!
```

---
## \#138 Posted by: ciscotory Posted at: 2018-11-07T21:19:31.184Z Reads: 85

```
Hi Lowguido
I'm facing a smilar problem just like yours with motor connected via slave vesc, pressing on cruse control and it spins up rabedly and some times just slwoly constant speed.
my setp up (fist time build) is dual vesce 4.12 with two 190kv's with 10s3p 
how (did you fidn it / or whre distinguishit it) was a faulty canbus cabele? buy testing using vesc tool or other mithode?
thanks..
```

---
## \#139 Posted by: lowGuido Posted at: 2018-11-08T14:06:50.035Z Reads: 84

```
I just replaced the cable.
```

---
