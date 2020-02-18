# Maytech MTES 120A 12S Sensor System with 6374-170KV Motors

### Replies: 45 Views: 5259

## \#1 Posted by: Nowind Posted at: 2016-09-22T05:02:09.304Z Reads: 405

```
Hey.

We have ordered 3 complete Sensor Setups in China from Maytech for testing this on E-MTB.
@squad : saw them on your tread, so first thanks for posting this mate.

<img src="/uploads/db1493/original/3X/b/e/be3b98a437e36b5536ae5b1ba589fd7e25fd0b14.JPG" width="666" height="500"> 

<img src="/uploads/db1493/original/3X/e/1/e1f19b06b2767e2fbdf48df012e3551c65cad99d.JPG" width="666" height="500">

Its in about 3 years riding E-MTB´s the first Sensored system i own. Really interrested how this will perform compared to unsensored Roxxys or MAX6 setups!

Ordered the USB-Links and the Progbox too:
<img src="/uploads/db1493/original/3X/7/0/70ce03e03d848bf79be0ada73cb264f92b48f051.JPG" width="666" height="500">

Motors are as labeled :
63mm diameter,
74mm long, 
817gramm wheight, 
8mm Motorshaft, 25mm long
2mm Keyway, 19mm long ... why not 3mm (-;
2 common bolting circles M4, 44mm and i guess 30mm
12AWG silicon Motorwires 

<img src="/uploads/db1493/original/3X/f/6/f6a176f2a3b6d4b191d22e2234338d3d7227bd3c.JPG" width="666" height="500">

Look from behind on Hallsensors:
<img src="/uploads/db1493/original/3X/0/f/0f893757f079deee60142f898ac65b95937e6cb2.JPG" width="666" height="500">

Front wire inlet:
<img src="/uploads/db1493/original/3X/a/1/a1569150bac2203ece75d5cbaca0579b0888b173.JPG" width="666" height="500">

The Hallwires were only shrinked with the phase wires, looks not really good IMO
Added some extra shrink in the outlet area:
<img src="/uploads/db1493/original/3X/b/c/bc26e1e7cb94c82a9d496f1cc6ca4d2270a9be8c.JPG" width="666" height="500">

One Hallwire were broken, fast fix but of course not nice by brandnew parts... 
<img src="/uploads/db1493/original/3X/8/2/828fdaeaebc99416ebc79b6a23790d38d5a63213.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/7/8/78174b56590b3e2c27352d33176673135c555d4f.JPG" width="666" height="500">

ESC´s : 
58mm X 86mm
186gramm wheight
similar footprint to the Roxxy, only the Elkos are relocated to get it slimmer.
Aluminium Heatsink, 2 pieces, screwed 

<img src="/uploads/db1493/original/3X/c/e/ce3f86dd44ad8b8aa49d30d0f0ab1e52d9e1e119.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/4/b4c5fcbeefe7dc685d6372cade58e48ef1234b1e.JPG" width="666" height="500">

Dont like that the hallsensor connector sits on the side, better IMO to locate it on phase wire side...

<img src="/uploads/db1493/original/3X/3/4/34813fab22cc2aff73a356d93c2060452e919d7d.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/6/867f7767013f45e3c6b83e8b4d4385b950e769b6.JPG" width="666" height="500">

Problems at the moment:
Cant set the " Throttle Calibrations" in the instructions they talk about a set button you should use to determine the endpoints.... but there is no set button (-:
seems to work correct but feels strange.... asked squad about and he confirm that he dont set it and it works ... he is probably right that they just copied the instructions from another ESC

The Program Box connects to ESC but not more ... i used the USB Linker instead and this works:
You can set the common parameters... will post some pics later

So hope to do some real life tests shortly.

Hang Loose 
Jenso
```

---
## \#2 Posted by: covert Posted at: 2016-09-22T06:16:27.454Z Reads: 342

```
Wow. They look awesome. Keen to hear the results of the testing.
```

---
## \#3 Posted by: kovjanos Posted at: 2016-09-22T06:47:01.972Z Reads: 338

```
I had two of these ESCs - one was faulty right out-of-the-box. Now support is silent since days.
<img src="/uploads/db1493/original/3X/2/3/232bd049f03ddddf62b66cd2321b66ab98d87215.jpg" width="484" height="500">


R, J.
```

---
## \#4 Posted by: squad Posted at: 2016-09-22T09:29:33.614Z Reads: 322

```
@nowind I hope they will work fine for You, with 63mm motors there is huge difference with sensored vs sensorless operation from my personal experience :)

@kovjanos I guess it's just infamous chinese quality control... sorry to hear that mate, too bad they didn't sort this out right...

Maybe it's salvageable, it seems like mosfet's failed, it would require someone with smd soldering skills and hot air soldering station, I think it may work again with those faulty mosfets changed.
```

---
## \#5 Posted by: kovjanos Posted at: 2016-09-22T09:44:57.570Z Reads: 318

```
Yep, I hope somehow it will work - but would be more happy to have it replaced. 
With sensors connected the other ESC makes the motor clogging (very rare) on slow speed even if it has a smooth start (doesn't have this issue with VESC).
If it won't work out the right way I'll wait for VESC 6 before investing into another pair of Maytech ESCs as there is no way back to non-sensored configs :) 

R, J.
```

---
## \#6 Posted by: JLabs Posted at: 2016-09-22T10:16:39.811Z Reads: 310

```
Curious to hear your results, because I am planning an MTB build. How much did u pay for each unit? If u don't mind me asking.
```

---
## \#7 Posted by: squad Posted at: 2016-09-22T15:28:59.829Z Reads: 292

```
You may need to change sensor wires arround, probably Your hall sensor order is not corresponding to phase wires.

[Check this out](https://endless-sphere.com/w/index.php/Determining_the_Wiring_for_a_Brushless_Motor)
```

---
## \#8 Posted by: michaeld33 Posted at: 2016-09-22T16:46:24.557Z Reads: 280

```
Wow awesome. I'm planning on picking up some of these, good to see someone else is using them!
```

---
## \#9 Posted by: kovjanos Posted at: 2016-09-22T18:05:54.519Z Reads: 281

```
I tried all the possible variations to find the one which worked. ...but even the best one is clogging sometimes (very rare).
Actually I kept the sensor fixed and played with the phase wires - my understanding that this is OK.

R, J.
```

---
## \#10 Posted by: squad Posted at: 2016-09-22T20:18:52.368Z Reads: 273

```
If so, then maybe one of Your hall sensors has failed? It's simple to check with voltmeter, it should give 0 then 5V and then again 0 etc. as You slowly turn the motor by hand.

Sorry Jenso for highjacking Your thread.
```

---
## \#11 Posted by: Nowind Posted at: 2016-09-23T05:19:01.436Z Reads: 269

```
No its all good, it was thought to discuss this sensor system, your input is really apreciated :kissing_heart:
I´m in rush right now, will give some updates later.
```

---
## \#12 Posted by: Nowind Posted at: 2016-09-24T19:34:44.889Z Reads: 280

```
[quote="kovjanos, post:3, topic:9973"]
I had two of these ESCs - one was faulty right out-of-the-box. Now support is silent since days.
[/quote]

Sorry to hear, you dont get any reply from the seller? Since how long?
We have emailed him because the wrong documentation and get instantly an reply.

[quote="JLabs, post:6, topic:9973, full:true"]
Curious to hear your results, because I am planning an MTB build. How much did u pay for each unit? If u don't mind me asking.
[/quote]



Maytech sends us new instruction for the ESC, and told us that the throttle calibration is not needet with this "special skateboard ESC"... So its like @squad said.
Dont know if its possible to upload PDF, if so i could share the actuall instructions !

I got both ESC´s and Motors now soldered and programmed.
Both work in sensored Modus, just have to change one phase wire on one ESC.
Programming via USB LInk is easy, but the Progbox still not working.

Machined a Rc plate for mounting:
<img src="/uploads/db1493/original/3X/a/d/add798f9b8534ad20488b6c3e6cb5603a4064728.JPG" width="666" height="500">

Mount one ESC upside down to have the hallconnector on the outside:
<img src="/uploads/db1493/original/3X/0/2/02f8593513026d21ad338023a5d4d497b3c272ca.JPG" width="666" height="500">

I used for the first time the "SUGRU"  to secure the Hall wires on connector.
Thanks to @whitepony for mention this stuff on one of his posts. 
Lots of possibilities ... like it

<img src="/uploads/db1493/original/3X/6/a/6a8528e656d77628338c8f58a3d7bd1d53bee857.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/e/8ed47aa12e9789344a9ecd5ab96b421cf7ffc146.JPG" width="666" height="500">

Now actually waiting for the 2mm Keys to complete the buildup and go for real life test.

<img src="/uploads/db1493/original/3X/3/5/3521c58777079b3482d492258c154197d8081d1c.JPG" width="666" height="500">
```

---
## \#13 Posted by: kovjanos Posted at: 2016-09-25T11:40:45.464Z Reads: 252

```
[quote="Nowind, post:12, topic:9973"]
Sorry to hear, you dont get any reply from the seller? Since how long?We have emailed him because the wrong documentation and get instantly an reply.
[/quote]

4 days - but this is constant. Got now 2 replies but always had to wait that much...

R, J.
```

---
## \#14 Posted by: kovjanos Posted at: 2016-09-25T11:42:13.030Z Reads: 249

```
[quote="Nowind, post:12, topic:9973"]
Machined a Rc plate for mounting:
[/quote]

Are you sure that these ESCs have the same environment sealing like your other car ESCs? I'm not sure...

R, J.
```

---
## \#15 Posted by: Nowind Posted at: 2016-09-25T16:53:35.498Z Reads: 242

```
They are labeled as "splashwaterproof" but i will not test this (-;
Its not a board i will run in the rain.
But dust and debris will not be a problem, so i see no need for a extra housing.
```

---
## \#16 Posted by: kovjanos Posted at: 2016-09-27T14:29:08.476Z Reads: 226

```
They are far away from being splash-proof. The case doesn't seal the cables, cap bank is almost full open plus the sensor connector and led hole is wide open.
The works is around the phase wires, those SMDs are placed too close to the openings. 
Actually those are placed too close to the cable soldering points and the positions of the fets' metal heat--pipe-leafs are also quite risky.

I got some replies and updates but still not a big step forward.

R, J.
```

---
## \#17 Posted by: Nowind Posted at: 2016-09-27T18:35:40.537Z Reads: 221

```
Yes you are right. As i said i will not ride the setup in the rain.

Today i mounted the Gears and do a Benchtest on 12S.
Both ESC are working but with at least half the power they should delivers.
I´m sure that this has to do with throttle calibration, maytech told us that its not needet by this ESC (and also not possible) but its like only half throttle.

Same effect by my friend !!!

What let me think thats has to do with Throttle calibration : 
If i give full throttle i can increase RPM by turning the "throttle poti" this is IMO a proof for missing throotle calibration. I dont get full RPM but more.

My friend tested two different Remotes, one is the original Maytech Throttle Remote.
I used the common 2.4ghz Miniremote, will test with my DX3R Pro Remote also this evening.

We contacted Maytech also, hope on fast reply.

Cheers
```

---
## \#18 Posted by: DeathCookies Posted at: 2016-09-27T18:45:44.424Z Reads: 212

```
Maybe you can try the following trick:

Full throttle --> turn on the esc
wait till it beeps and then go neutral
wait till it beeps and go full brake

after it it will be configured. Well it is just a guess :D My YEP helicopter esc is working like that ;)
```

---
## \#19 Posted by: kovjanos Posted at: 2016-09-27T18:53:41.783Z Reads: 213

```
I'm wondering if you have the Maytech MTES120A Users Manual.pdf which is really for the 120A version as my PDF is sh*t. Looks like a mix of EZFUN and 120A.

I'm also wondering if you get the programmer working as the PC software they sent over is a bit "unfinished" - you can set the battery type, the cell level cutoff value but you can't set the number of cells in series :) 

R, J.
```

---
## \#20 Posted by: kovjanos Posted at: 2016-09-27T19:01:13.360Z Reads: 223

```
[quote="Nowind, post:17, topic:9973"]
I´m sure that this has to do with throttle calibration, maytech told us that its not needet by this ESC (and also not possible) but its like only half throttle.
[/quote]

I got a doc from them because I had the same issue. The doc doesn't look like the right one but has the following for calibration:

> Throttle Range Calibration:
> Note: For the first time using transmitter or changing the transmitter you must set Throttle Range Calibration.
>
> ◆ Switch off the ESC, connect it with battery pack, then turn on transmitter, set the direction of the throttle channel to REV; set the throttle trim to "0"; set the  EPA/ATV value of the throttle channel to 100%, and disable the ABS function of your transmitter.
>
> ◆ Hold the "Set" button and switch on the ESC, wait for about 2 second until the Green LED begins to flash and the motor emits continuous ''Beep-beep-'' sound. then release the ''Set" button and pull the throttle trigger to the neutral point at the same time, then you will hear a continuous "Beep" sound and see the Red LED continuous blink, then click on the "Set" button, hear "Beep" the sound of the motor.
> 
> ◆ Push the throttle trigger to end position of forward, press "Set" button for one time, you will hear motor ''Beep-beep-".
>
> ◆ Now push the throttle trigger to the end position of backward, press "Set"  button for one time, you hear motor "Beep-beep-beep", both of the Red LED and Green LED turned off simultaneity, the Throttle Range Calibration is confirmed , the motor can be started after 2 seconds for battery cells detecting program.

R, J.
```

---
## \#21 Posted by: mccloed Posted at: 2016-09-27T19:26:41.904Z Reads: 192

```
Looks like the instructions on an ESC with a program switch, which, I assume, these do not have. 

To anyone using the Maytech or FVT 12s 120a ESC: **Make sure no throttle input is given on start up**. I have fried several of these by accidentally giving a little throttle while turning the ESC on.
```

---
## \#22 Posted by: Nowind Posted at: 2016-09-27T21:25:08.968Z Reads: 199

```
[quote="DeathCookies, post:18, topic:9973"]
Maybe you can try the following trick:

Full throttle --&gt; turn on the escwait till it beeps and then go neutralwait till it beeps and go full brake

after it it will be configured. Well it is just a guess :smiley: My YEP helicopter esc is working like that :wink:
[/quote]



I tried this already, my Roxxy is programmed this way. Thank you mate.

[quote="kovjanos, post:20, topic:9973"]
I got a doc from them because I had the same issue. The doc doesn't look like the right one but has the following for calibration:
[/quote]

I got a newer one on request, there is completely nothing about calibration, all say say "its not needet" :grin:

[quote="mccloed, post:21, topic:9973, full:true"]
Looks like the instructions on an ESC with a program switch, which, I assume, these do not have. 

To anyone using the Maytech or FVT 12s 120a ESC: Make sure no throttle input is given on start up. I have fried several of these by accidentally giving a little throttle while turning the ESC on.
[/quote]

Holy Shit, you killed several this way? Oh man thanks for advice. I will be carefull.

And yes you are right, the old instruction manuel is talking about a switch which is not there.
```

---
## \#23 Posted by: JLabs Posted at: 2016-10-01T16:18:02.045Z Reads: 177

```
Hey, do you know which wire is A, B, and C? How did you wire them properly or dosnt it matter?

Thanks!
```

---
## \#24 Posted by: Nowind Posted at: 2016-10-01T18:36:25.035Z Reads: 199

```
Hey.
No there is no identification on the wires.
Just hook them up and try... have to change on one side the two of the phase wires.

For detailed informations on testing hall connection check out the link from @squad  : 

[quote="squad, post:7, topic:9973, full:true"]
You may need to change sensor wires arround, probably Your hall sensor order is not corresponding to phase wires.

Check this out
https://endless-sphere.com/w/index.php/Determining_the_Wiring_for_a_Brushless_Motor
[/quote]
```

---
## \#25 Posted by: Lukaszlisc Posted at: 2016-10-01T20:30:48.426Z Reads: 196

```
Would be not better use Alien 6374 Sensored Outrunner brushless motor 170KV 3200W? any one test them on E-MTB? 
<img src="/uploads/db1493/original/3X/4/e/4ef719f7f8a94d041eacf0c9c0ad3de694bcdc15.jpg" width="400" height="400">
```

---
## \#26 Posted by: JLabs Posted at: 2016-10-01T23:16:18.154Z Reads: 191

```
So, I got 2 of these for testing. The wire closest to the sensor port is A, middle is B, and the furthest is C. I am overly impressed with this speed controller. I just have one problem. The brakes are progressive when I brake, but after about 1 second they go to full brake. Do you have any pointers?
```

---
## \#27 Posted by: Lukaszlisc Posted at: 2016-10-01T23:42:22.199Z Reads: 185

```
@JLabs what ESC are you using?
```

---
## \#28 Posted by: JLabs Posted at: 2016-10-01T23:58:16.787Z Reads: 183

```
The 12s 120a sensored.
```

---
## \#29 Posted by: Lukaszlisc Posted at: 2016-10-01T23:59:46.009Z Reads: 180

```
What model?
```

---
## \#30 Posted by: JLabs Posted at: 2016-10-02T00:00:25.759Z Reads: 181

```
They are from FVT. They're are the same as the Maytech, I think.
```

---
## \#31 Posted by: smudgeUK Posted at: 2016-10-02T01:25:54.080Z Reads: 180

```
Cześć Lukasz!
I have two of these motors on my EMTB but i am waiting on my ESCs to be able to test them. Unfortunately i wont be able to use the sensors as the ESCs i am getting do not support sensored motors. Once i have tried them out i will let you know how they are
```

---
## \#32 Posted by: mccloed Posted at: 2016-10-02T02:43:44.508Z Reads: 170

```
Hey @JLabs, there is no way to set the brakes differently. The only thing you can do is change the delay time when it goes to full brake. 
Another reference for the phase wires: The one across from the positive lead is A, middle, B, and the one across from the negative lead is C. According to FVT.
```

---
## \#33 Posted by: JLabs Posted at: 2016-10-02T02:58:51.085Z Reads: 169

```
Really? That's odd.. Can you change the delay time with the programming card?
```

---
## \#34 Posted by: mccloed Posted at: 2016-10-02T03:11:06.858Z Reads: 165

```
Yup. If you have the right version. I've only had the USB link work for me. If you change the break percentage it changes the delay, on certain firmware versions. Some make no difference. That and the throttle at start-up death are the reasons I am not running one of these anymore.
```

---
## \#35 Posted by: Lukaszlisc Posted at: 2016-10-02T07:53:50.778Z Reads: 169

```
Siema:) i got dual 6355 motors sensoredless on VESC and 16cLiFepo4 setup. But the starting is annoying the motors just shaking but when it start is accelerating no problem. I was thinking to try sensor system and bigger motors. Waiting for news from you how they work thanks
```

---
## \#36 Posted by: Nowind Posted at: 2016-10-02T08:44:27.263Z Reads: 172

```
[quote="JLabs, post:30, topic:9973, full:true"]
They are from FVT. They're are the same as the Maytech, I think.
[/quote]

Are this the ones you are selling in your portal?
I thought the 12S ESC you have there is sensorless ?
Maybe i missunderstood?
```

---
## \#37 Posted by: JLabs Posted at: 2016-10-02T14:10:39.529Z Reads: 169

```
I am selling the 12s sensorless and bought 2 sensored versions for testing.
```

---
## \#38 Posted by: Mikeomania12 Posted at: 2016-10-02T15:58:31.859Z Reads: 172

```
So now you agree they are the same?
```

---
## \#39 Posted by: JLabs Posted at: 2016-10-02T16:12:11.984Z Reads: 166

```
**NO THEY ARE NOT.** The 12s **WITHOUT** sensors are different. The 12s **SENSORED** are the same. Why do you keep doubting me? I know what I am talking about.
```

---
## \#40 Posted by: Mikeomania12 Posted at: 2016-10-02T17:12:18.036Z Reads: 164

```
I doubt you because I know others that have told me they are the same. But thanks for being more clear about the sensors.
```

---
## \#41 Posted by: smudgeUK Posted at: 2016-10-02T17:50:45.709Z Reads: 158

```
I believe the vesc should work well without sensors.
I also have two vesc but have decided not to use them due to people here saying they are not very well suited to EMTB, but better for skateboard. I will try my motors on the MAX6 ESC's without sensors when i get them and let you know how they perform. maybe I will try the vesc on it one day.
@Nowind has used vesc on his with no problems in the past
```

---
## \#42 Posted by: Nowind Posted at: 2016-10-25T05:33:52.142Z Reads: 156

```
Short Update:

Problems with Programbox are solved, it was my fault. Dont plug it in correct :kissing_closed_eyes:

But the other problems are still there :disappointed_relieved:
We are in contact with Maytech, still hoping for updates.

Cheers
Jenso
```

---
## \#43 Posted by: Lukaszlisc Posted at: 2016-10-25T06:38:33.609Z Reads: 156

```
Did u test motors with different esc or vesc to see if where the problem is? If low power is motors foult or esc?
```

---
## \#44 Posted by: Nowind Posted at: 2016-10-27T18:36:24.208Z Reads: 151

```
Hey.
No i dont swapped to other motors or ESC.
I thought about but was to frustrated to spend more time with this, send the hole System back to Seller.
They wants to and IMO let them find the bug (-;
```

---
## \#45 Posted by: Lukaszlisc Posted at: 2016-10-27T19:09:26.039Z Reads: 150

```
Im using sensoredless 6355 motors just now but was thinking to upgrade to Alien 6374 Sensored Outrunner brushless motors 170KV 3200W and try it with vesc or alien 12s sensord esc. Wonder if any one got setup like that?
```

---
