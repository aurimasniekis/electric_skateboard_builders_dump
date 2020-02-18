# Sensored FOC setup

### Replies: 47 Views: 5019

## \#1 Posted by: Daan_vZon Posted at: 2017-04-30T13:13:39.632Z Reads: 481

```
Couldn't really find some detailed up to date information about this, so decided just to make a new topic. I wonder whether it is better to control your motor through FOC or sensored through BLDC (in hybrid mode probably). Although my motor does have a 6-pin sensor wire which should be compatible with the [Enertion VESC](http://www.enertionboards.com/electric-skateboard-parts/vesc-x-programmable-brushless-motor-controller/?setCurrencyId=3) I use, I have only used an FOC setup thus far, which worked quite well. If I increase the connector size on the motor's sensor wire it will fit the VESC so I can setup sensored/hybrid mode, but before doing so I hope someone's able to tell me whether this is preferable to do.
```

---
## \#2 Posted by: yaca Posted at: 2017-04-30T20:30:23.968Z Reads: 461

```
You say your FOC setup worked quite well, so why you want to change to BLDC? You can also try sensored motor with FOC.
```

---
## \#3 Posted by: Daan_vZon Posted at: 2017-05-01T11:24:55.127Z Reads: 448

```
Found out only yesterday in the BLDC tool that it is possible to use hall sensors with the FOC mode too. Always thought it was FOC ór sensored, but now know you can do both. Thanks for the respons.

However, during setup my Enertion VESC-X gave a 'fault' warning by a red flickering LED, after which a part of the VESC blew up, so unfortunately I'm not able to test it out anyway...
```

---
## \#4 Posted by: makevoid Posted at: 2017-05-01T11:54:58.196Z Reads: 423

```
which fault did you get? if it's a over/under voltage error you may need to change your voltage limit, for example max input voltage should be 57V.
```

---
## \#5 Posted by: Daan_vZon Posted at: 2017-05-01T12:10:47.805Z Reads: 411

```
@makevoid just made a new topic for it, hoping to get some input like yours. 
However I do not know what kind of error it was. The VESC features a small red LED specific for indicating a fault, which suddenly went blinking. I already set the maximum input voltage to 57V in the very beginning, so I think it couldnt't be that problem, or can it?
```

---
## \#6 Posted by: Daan_vZon Posted at: 2017-05-01T12:11:27.451Z Reads: 405

```
Topic about the problem is:
https://www.electric-skateboard.builders/t/enertion-vesc-x-failing/22136
```

---
## \#7 Posted by: Daan_vZon Posted at: 2017-05-10T20:13:23.770Z Reads: 388

```
I would like to set up my VESC(-X) sensored as soon as I have the time for it. However, the female 6 pin JST-connector on the sensor wire coming from the motor, is smaller than the male connector on the VESC. <img src="/uploads/db1493/original/3X/f/f/ffa1b8f45cc049805742095eb7efa3aea9453790.jpg" width="690" height="388">

I think the sensor wire is a "Standard RC Sensor Wire JST-ZH 6pin 1.5mm pitch". Not sure what kind of connector is on the VESC and what dimensions it is.

Can anyone please tell me the best way to connect the sensor wire to the VESC? Haven't yet been able to find the right female connector online to replace the sensor wire connector with.
```

---
## \#8 Posted by: yaca Posted at: 2017-05-10T21:07:29.032Z Reads: 371

```
search for JST-PH 6pin 2.0mm pitch. Maybe you try this adapter 
diy-electric-skateboard-kits-parts/vesc-sensor-wires/ 

or just find the right plug and solder it to your wire. If you want to solder the plug I could send this to you if you are in europe. I just ordered yesterday 10 plugs with wire, same like Jinra posted right now. It was just € 5,49 free shipping, but it comes from China and will need some time to arrive.
```

---
## \#9 Posted by: Jinra Posted at: 2017-05-10T21:10:35.095Z Reads: 361

```
This works perfectly

http://www.ebay.com/itm/JST-2-0mm-PH-6-Pin-Connector-with-Wire-X-10-Sets-TW-/141757606740?hash=item2101696b54:g:W9EAAOSwgQ9V3m4W
```

---
## \#10 Posted by: Daan_vZon Posted at: 2017-05-10T21:55:58.475Z Reads: 354

```
@Jinra @yaca thanks
That adapter would have been perfect. Wish I knew they had it when I ordered the motor from them. Shipping alone from diyelectricskateboard costs $40 however, so that's a bit too pricey to go for though. The best option will indeed probably be one of these connectors like Jinra just sent. Would only need 1 though and according to Ebay shipping will be between Fri. May. 26 and Tue. Jun. 20, a bit long... Yaca, when do you think your plugs will arrive? I would be really glad if you could just send me one, I live in the Netherlands. But do you think shipping costs from you to me be worth it?
```

---
## \#11 Posted by: Daan_vZon Posted at: 2017-05-10T22:36:50.617Z Reads: 356

```
Decided to just order the connector wires Jinra showed. Will have to wait until they arrive for some time, but it's worth the money just ordering, it might also come in handy in the future. Will use sensorless control first and switch to sensored when they arrive. Let's see it in a positive way: I will be able to enjoy the improvement the more.

Also ordered an HM-10 BLE Bluetooth module today to connect the VESC to my phone and will look further for some suitable front- and backlights for using in addition to the RGB LED-lightning I placed under the board.
```

---
## \#12 Posted by: Daan_vZon Posted at: 2017-06-07T17:33:29.261Z Reads: 352

```
After finally receiving the needed JST-PH 6pin 2.0mm connector wires I started setting up my board sensored instead of unsensored, which I used before. However, after pressing 'Detect Hall Sensors' in the FOC tab I get the notification 'Bad Detection Result Received' in the down right corner. Could anyone tell me how I can fix this problem?

The motor I use is [this](diy-electric-skateboard-kits-parts/6355-260kv-epower-motor/) one from .
In the description of their motors, the following is stated, which I used for connecting the wires:

Sensor Wire: Standard RC Sensor Wire JST-ZH 6pin 1.5mm pitch
Red = 5v
White = Temp
Blue = A
Yellow = C
Green = B
Black = GND

I use the FOCBOX (previously called the VESC-X), on which characters are written next to each port for the Hall-sensors. From one side to the other these are:
5V
H3
H2
H1
T
GND

So I cut off the 1.5 mm pitch from the sensor wire coming from the motor and replaced it with the new 2.0 mm one, in such a way that the wires were connected in the following way if I put the 2.0 connector in the FOCBOX/VESC:
Red = 5v             --> 5V
White = Temp      --> T
Blue = A              --> H1
Yellow = C           --> H3
Green = B            --> H2
Black = GND        --> GND

These combinations seemed the right ones to me, but maybe some need to be switched? Hopefully, someone can help me out. Thanks in advance.
```

---
## \#13 Posted by: yaca Posted at: 2017-06-07T18:03:16.492Z Reads: 327

```
At 4.12 VESC the temperature pin is next to the red 5V+ pin. It seems at the focbox it's next to the GND pin. Is this correct @onloop? I'm not sure how you connected it. Maybe a picture?
```

---
## \#14 Posted by: Daan_vZon Posted at: 2017-06-07T19:03:03.562Z Reads: 329

```
@yaca  A sort of sticker on the FOCBOX gives the following pinsequence (the left one for the not knowing people), which is the one I listed above.
<img src="/uploads/db1493/original/3X/9/d/9d9f9a3cc53ab34195aa4947861c15c7f1c8a217.jpg" width="690" height="388">

That makes it seem indeed that the 5V+ pin is next to the GND pin, so conform to this I connected my wires. However if I take of the plastic cover and watch the backside of the board I can read the following pinsequence (again the one in the left), which is much different and is more like the normal VESC pinsequence as far as I know: <img src="/uploads/db1493/original/3X/b/6/b6835909899769858eb0350c304bcc63bb3fe6d3.jpg" width="690" height="388">
```

---
## \#15 Posted by: yaca Posted at: 2017-06-07T19:35:36.089Z Reads: 315

```
On the cover the temp pin is next to the GND pin and on the board the temp pin is next to 5V+!? So I think they printed it wrong on the cover. It would be clear if @onloop or somebody else can confirm this before you continue.
```

---
## \#16 Posted by: Daan_vZon Posted at: 2017-06-07T23:59:06.018Z Reads: 307

```
@EnertionSupport could you please help me out?
```

---
## \#17 Posted by: Jinra Posted at: 2017-06-08T00:12:25.361Z Reads: 308

```
I'd trust the PCB over the cover as they're likely from two different suppliers
```

---
## \#18 Posted by: Daan_vZon Posted at: 2017-06-08T09:00:43.578Z Reads: 305

```
In that case, I'll try to resolder them the way the PCB indicates. Did I assume correctly that for the Hall sensors H1 corresponded with A, H2 did with B and H3 with C?
```

---
## \#19 Posted by: Jinra Posted at: 2017-06-08T14:10:14.675Z Reads: 295

```
Order of the sensors doesn't matter as long as you do detection.

why do you have to resolder? You can use a pin to remove the wires from the jst header
```

---
## \#20 Posted by: Daan_vZon Posted at: 2017-06-08T15:12:17.758Z Reads: 293

```
Hmm, didn't think of that. I just resoldered/switched the second and the fifth wires, so it corresponded with the pinsequence written on the PCBA. It seems that Enertion didn't put the right markings on their sticker. I just redetected the Hall sensors in the BLDC tool and it works now. Thanks @Jinra and @yaca! Gonna try out the difference with sensors hopefully tonight.
```

---
## \#21 Posted by: Wolfcola Posted at: 2017-06-08T15:41:02.299Z Reads: 273

```
Holy shit I was having problems with this and gave up. I'm going to try this.
```

---
## \#22 Posted by: Daan_vZon Posted at: 2017-06-08T15:47:35.773Z Reads: 273

```
Haha, great. That's partly why I posted it in the thread. You should just follow the indications on the PCBA instead of the ones on the topsticker. You could use the photo I posted or open the case yourself if that is easier for you. Hope it works out!
```

---
## \#23 Posted by: Wolfcola Posted at: 2017-06-09T17:47:57.415Z Reads: 260

```
Damn yo. It worked. Can't believe that was the problem. FOC is way more juicy. Stoked thanks dude!
```

---
## \#24 Posted by: NAT-Frank Posted at: 2017-06-10T03:50:50.114Z Reads: 256

```
Holy shit dude. I have been trying to figure this out too. So glad I ran into this thread.
```

---
## \#25 Posted by: Stef Posted at: 2017-06-11T21:26:30.101Z Reads: 249

```
Thank you so much for pointing this out! I switched pins and am now running sensored FOC. Now starting from standstill is butter smooth and the general throttle/braking response seems more fluid in general.
```

---
## \#26 Posted by: yaca Posted at: 2017-06-12T08:04:04.895Z Reads: 244

```
@onloop did you read this thread?
```

---
## \#27 Posted by: TranxFu Posted at: 2017-06-14T22:16:52.409Z Reads: 239

```
Mhmmm.. I tried sensored on the FOCBOX. Also switched the pin sequence as seen on the PCB. I get failed hall sensor detection on BLDC and FOC. I'm using APS motors. Any way I can check what is not working correctly ?
```

---
## \#28 Posted by: Jinra Posted at: 2017-06-14T22:21:24.554Z Reads: 245

```
pics of setup with sensor wires?
```

---
## \#29 Posted by: TranxFu Posted at: 2017-06-16T14:06:16.923Z Reads: 247

```
<img src="/uploads/db1493/original/3X/1/5/15dbbe3f97e3a5f44355303e6438e74063bceb12.JPG" width="375" height="500">

Orange=blue. Extended the sensor wires as per color. It's a aps motor
```

---
## \#30 Posted by: Blasto Posted at: 2017-06-16T14:43:17.011Z Reads: 233

```
just as a test, make your motor go in the reverse direction (flip two phases) and try again
```

---
## \#31 Posted by: TranxFu Posted at: 2017-06-17T10:59:07.715Z Reads: 230

```
Tried and got the same results :/ @Daan_vZon did it work out for you ?
```

---
## \#32 Posted by: Daan_vZon Posted at: 2017-06-17T13:44:59.836Z Reads: 227

```
Yeahh, it worked out perfectly for me! I just connected the wires like the PCB described and it couldn't start up smoother. Even going from driving forward to going in reverse goes 100% smoothly.
```

---
## \#33 Posted by: TranxFu Posted at: 2017-06-17T14:40:00.676Z Reads: 225

```
Mhmm all right. Maybe I'll check the solder spots again. Is yours plugged in in the same sequence as the one posted above ?
```

---
## \#34 Posted by: Daan_vZon Posted at: 2017-06-18T13:07:58.305Z Reads: 218

```
Which one posted do you mean? Yours? Unfortunately, I won't be able to tell you if the wires are in the same sequence, since I don't know the sequence of the sensor wires coming for your motor.
```

---
## \#35 Posted by: flywithgriff Posted at: 2017-08-07T03:09:21.243Z Reads: 200

```
I'm happy to have found this thread as I am about to set up my first FOC build. I will be running 10s and dual 6374 190kv with dual FOCBOX. Can anyone go a bit more in depth with the steps to setup FOC?
```

---
## \#36 Posted by: Jinra Posted at: 2017-08-07T03:10:26.198Z Reads: 201

```
Use ackmaniacs fw and it has step by step numbers to show you exactly how to configure
```

---
## \#37 Posted by: flywithgriff Posted at: 2017-08-07T03:11:21.246Z Reads: 209

```
Awesome! Thank you. I'll have to search his thread on how to upload the firmware.
```

---
## \#38 Posted by: flywithgriff Posted at: 2017-08-07T04:01:57.344Z Reads: 208

```
Does it matter wether I'm using a split servo vs canbus for his fw?
```

---
## \#39 Posted by: Jinra Posted at: 2017-08-07T05:56:02.582Z Reads: 201

```
nope either will work.
```

---
## \#40 Posted by: Lionpuncher Posted at: 2017-09-01T23:47:09.654Z Reads: 195

```
Had a gander at the PCB in my new focbox. The 5v and the GND are swapped on the sticker for the motor sensor connector. 
Great thread!
```

---
## \#41 Posted by: flywithgriff Posted at: 2017-09-02T00:33:28.650Z Reads: 189

```
Please post pictures of your FOCBOX. The T and H3 should be swapped. If your G and 5V are swapped that's a new issue.
```

---
## \#42 Posted by: Lionpuncher Posted at: 2017-09-02T20:36:37.406Z Reads: 190

```
OK guys. Totally derped that. Upon a recheck at a more decent hour of the day, I can see my issue is the same as the others. It's defo the H3 and T not the 5V and GND. 
My bad.
```

---
## \#43 Posted by: crustyxpunk Posted at: 2017-09-15T13:48:30.858Z Reads: 174

```
Kind of lame that enertion or onloop never responded to this thread...
```

---
## \#44 Posted by: Mikenopolis Posted at: 2017-09-15T16:43:15.621Z Reads: 168

```
I'm finally starting my new build and wanted to be sure on this issue. So basically I just have to swapped these two wires on the **sensor wire connector**, Blue wire goes to T and Brown wire goes to H3 correct?
<img src="/uploads/db1493/original/3X/b/b/bbf8b871cd708025735b18048469c4553bd2b8ab.jpg" width="498" height="500">
```

---
## \#45 Posted by: Jinra Posted at: 2017-09-15T16:44:57.875Z Reads: 162

```
Yes you can use a little needle or pin to lift the plastic retainer on the JST header and pull out the cable really easily. The convention for the TEMP wire is white, so you could move that to the correct position if you want, but not required. 

When in doubt check the PCB, but the picture looks right.
```

---
## \#46 Posted by: Mikenopolis Posted at: 2017-09-19T18:17:19.973Z Reads: 156

```
I swapped the two wires on the JST header but BLDC tools was unable to measure the hall sensor. after a bit of thought, I realized it didn't make sense to swap the wire because the LABEL was made wrong, but the PCB is correct, which means ignoring the label, the wires from the motor to the board would still be connected to what it should be. I swapped it back and everything worked like a charm.

Am I crazy here or does it not matter unless you are putting together your own sensor and own wiring?
```

---
## \#47 Posted by: Lionpuncher Posted at: 2017-09-22T16:58:26.942Z Reads: 136

```
 Not crazy at all. 
The sensored motor i bought had a different connector than the connector on the esc. So i had to solder a different end on the motor side. Was very important to know where to put the wires on the new connector.
```

---
