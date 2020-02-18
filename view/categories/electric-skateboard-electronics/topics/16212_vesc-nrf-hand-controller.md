# VESC NRF Hand Controller

### Replies: 44 Views: 7458

## \#1 Posted by: Duffman Posted at: 2017-01-17T14:26:32.101Z Reads: 538

```
Hi there, I wanted to show you my VESC NRF Hand Controller. It is based on Benjamin Vedders Nunchuk RF PCB and can be used with any VESC. In fact it is a NRF Nunchuk, put into a 3D printed case to get rid of this little thump stick and to convert it into a trigger.

All 3D data can be found here: http://www.thingiverse.com/thing:2027168

First of all a few pics to show you what I'm talking about:

<img src="/uploads/db1493/original/3X/1/3/1359a3ee571515bc77b73bb45ee5e62fadd352e7.jpg" width="690" height="323">
<img src="/uploads/db1493/original/3X/d/6/d6cabfe80423411ac87ed0a6b52c65786552dc6d.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/5/3/530ffbd177c9e8213e4c44b48e9c24006f01033e.jpg" width="690" height="323">
<img src="/uploads/db1493/original/3X/6/e/6e5ddc15be7ff2215976a342258f0e36b4a38b9c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/4/d48b5efec626e045b3d27cc15c907cd327c83266.jpg" width="690" height="323">

Thanks go out to @chaka, who documented his Nunchuk RF build in this thread: http://www.electric-skateboard.builders/t/vesc-nunchuk-rf/588/30 

So I ordered the PCBs at OshPark and assembled my NRF24 based Nunchuk RF.
<img src="/uploads/db1493/original/3X/d/0/d0fb35af04913c8a882f4848dad102492ab7fecc.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/1/4/14d5b1e578d16e22215a434f9a449b71b4e0ac0c.jpg" width="690" height="388">

This PCB is intended to be placed in a Wii Nunchuk.
<img src="/uploads/db1493/original/3X/6/f/6fa357e1b0a70dcfca04d000419a5f683e1ca138.jpg" width="690" height="388">

On the VESC side the NRF24 transceiver can directly be connected to the VESC.
<img src="/uploads/db1493/original/3X/7/4/7489508c57618b6ae3fab3f4a50120fc2a17db59.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/d/8/d8f2544d81a31d7c2abcf7d9306599c384f6703a.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/8/7/87d11b7682553af1c56e6b132aa70875f39c11d4.jpg" width="690" height="388">


Luckily things worked from the start, there were some things that bothered me:
- connection with NRF was better than with the standard nunchuk but still not 100% reliable
- soldering required to change the NRF ID
- this fiddly thumb stick...

So I started upgrading it with an 'Hex switch' for the NRF ID:
<img src="/uploads/db1493/original/3X/a/4/a404894fa043a7e081ddc41ab33fe15148884f34.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/5/15883e2aa8f24957a22f7f01024648f1a098e2b5.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/c/6c5388b88d40d3c4fd632b1fa5f179fad29434e1.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/9/6/9694c18303f4ea59ad842be20ac405229061c9dc.jpg" width="690" height="388">

A NRFL01PA 'long range' module for TX and RX:
<img src="/uploads/db1493/original/3X/c/f/cfdd1303034a0df53eeae2432abf6ea49e4d04ba.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/3/c/3cdcc779915f973873fb53b26e081a8e4e66da97.jpg" width="690" height="388">

And finally after a series of prototypes I put all of this into a nice case which converts the thump stick to a trigger:
<img src="/uploads/db1493/original/3X/3/6/36bf7a01a39cc100c56816801dc8ee4f405df940.jpg" width="690" height="388">

More details in the next post...
```

---
## \#2 Posted by: Duffman Posted at: 2017-01-17T14:43:59.057Z Reads: 447

```
These are the 3D printed parts:
<img src="/uploads/db1493/original/3X/f/b/fbe1de89304d5b87f88f43a9bece9494efab491c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/2/8/285cdbc6c5d39f7966a409ba63322986b3a0344c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/9/b/9b1417deeda3f719956ca8b6346c04d263316da2.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/0/0/00f2c7b3ee30c1c2d846f8b6cda936977f3ff6ae.jpg" width="690" height="388">

The top of the case holds all PCBs, the trigger, the USB port, some switches and some LEDs:
<img src="/uploads/db1493/original/3X/2/c/2c2ec46c08ca22690dd22afdba481df4c5bd0cf8.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/9/a/9a61db279f103600d5a16bd6eb4f33da941a8147.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/9/2/92964c9753c61906d329d77a73f59b5c096cd073.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/6/e/6e495c42dc2f343e176b8273528fad0f3ee0320d.jpg" width="690" height="388">

The battery and the C + Z buttons are located in the lower halves of the case. The connector at the bottom is for a safety leash which shuts down the electronics if you loose the hand controller. If configured right, the VESC goes into brake mode with configurable braking current when the connection drops.
<img src="/uploads/db1493/original/3X/c/4/c45871cd4909076c030e2d4b0b2b3ce826fc0d79.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/a/1/a1a9305c38e6ebcf422ed419cd9e7aafbaad4288.jpg" width="281" height="500">

The buttons on the top are for the LED light and an hardware beginner mode. Two resistors can be switched in the line of the thumb stick to limit acceleration and braking power to 50% and stretch this 50% to the full mechanical trigger move.
(Yes it is really this simple and works perfect...)
<img src="/uploads/db1493/original/3X/b/f/bf0b31c0c1f9933caa9e0679739b7cb5766fd44c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/f/d/fd86b6e7e55ec935cb4b5e87faaec42e10161997.jpg" width="690" height="388">


Feel free to copy or remix this and build your own :slight_smile: 
<img src="/uploads/db1493/original/3X/d/6/d6cabfe80423411ac87ed0a6b52c65786552dc6d.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/3/6/36bf7a01a39cc100c56816801dc8ee4f405df940.jpg" width="690" height="388">
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-01-17T15:15:25.623Z Reads: 402

```
well this reminds me of the Halo-Alien-Spark-Thingy-Pistol :D
<img src="/uploads/db1493/original/3X/6/c/6c8784c07f05913780e4aea1c4085d05310adb6e.jpg" width="480" height="358">
```

---
## \#4 Posted by: Okami Posted at: 2017-01-17T15:48:15.152Z Reads: 395

```
Nice remote build!

I had a few questions:

1) **How did you make the surface of the 3d printed material so smooth?** Did you just sand it down and then applied some coating? I know there are a few methods but it seems you can get mixed results based on what material and what paper/aceton etc you use.. 

So would be cool to find more details about the nice finish of the 3d printed material!

2) **Is this the right resistor value you used - 4.7k Ohms 5% ?**

I might say you are a genius lol who knew it could be so simple as just wiring a resistor(s) in the line with wires..

Also - **in which 2 wires the resistors should be wired in** ? Im not that familiar with resistor basics anymore, so a little hint would be helpful..

** Extra question **

Do you think the same value resistors will work for any potentiometer? Could you give some details what value pot you had, so others could compare, if they have the same?

3) It looks like you also made a **''dead man'' switch** :) **Which type of connector you used for that?**

It looks something similar to these JST connectors but im not sure :slight_smile:

This is probably the least significant question from all but non the less, would be glad to know which one worked good for you, as I assume the connector has to snap out easly, to really work as a ''dead man's switch'' :slight_smile:

Nice work.. :)
```

---
## \#5 Posted by: mmaner Posted at: 2017-01-17T15:50:30.379Z Reads: 361

```
Very nice build, I like the LED's in the front too.
```

---
## \#6 Posted by: wmj259 Posted at: 2017-01-17T16:41:51.282Z Reads: 366

```
Thats the Needler :blush:

@Duffman, btw are those MNKE 18650s? I missed my luck at the clearance sale for liion :/
```

---
## \#7 Posted by: okp Posted at: 2017-01-17T16:50:29.543Z Reads: 372

```
nice one ! still a bit "big" too me as I prefer stealthy remote. I had Vedder NRF in the nunchuck in testing two years ago on my Busted board build; It was great, but I has some really weird behaviors time to time. It seems the NRF has some issues but then I moved to GT2B as I cannot afford to get this issues in Paris downtown.

https://youtu.be/CoG-N0z3H5w
```

---
## \#8 Posted by: Eboosted Posted at: 2017-01-17T22:00:27.505Z Reads: 351

```
Is it really dangerous to ride in Paris downtown?, how strict are airport security officers and airlines in regards to flying with an e-Board?
```

---
## \#9 Posted by: The_Dude Posted at: 2017-01-17T22:21:01.153Z Reads: 342

```
Perfect as usual, Heisenberg :sunglasses:

I already made some test prints, results are not good as yours but I will try to adjust better printing parameters. What kind of buttons did you use on the top and on the sides of the controller and can you you give some details on the antenna mod of the NRF? I know you already told me in Hasloch but unfortunately I can't remember :sweat:

Dude
```

---
## \#10 Posted by: Duffman Posted at: 2017-01-18T07:08:03.772Z Reads: 316

```
@Okami:

1. As I used PLA, I couldn't use acetone vapor to smooth the part. It is just roughly sanded, afterwards a bit ground with steel wool and afterwards spray painted with matte paint. I use to spray the last layer(s) from a too far distance to get some extra matte speckles which cover printing and sanding artifacts better.

2. Yes you are right, 4,7kOhm. But it does not have to be exactly this value, you could even use variable resistors and trim them to the value that gives you the percentage you like. The potentiometer in the thumb stick has 10kOhm. So in line with 5+5kOhm you shrink the trigger range to 50%. They are connected in the 'outer' both wires of the pot and get shorted to 0Ohm (each) by the switch to get 100% power again.

3. The connectors are called 'Losi Connectors' / Micro-T/B/DT. They do NOT snap out easily as I want the remote to shut down only when I go down so hard that I loose it. The second purpose of this is to simply switch off the remote, whitch does not work properly with any switch I had, because the charging electronics on the PCB is very sensitive to any resistance in the connection to the battery. 

Btw: You need to disconnect and connect power when you change the NRF ID, because it is only read at startup... This got me some grey hairs...


@wmj259:
I've no idea what type or brand these 18650s are. I put new cells in my cordless drill and used the old weak ones for this NRF remote.


@unik:
I'm riding nunchuks since the beginning and I'm so addicted to the reverse and cruise control buttons that I can't imagine something else. With the original Kama nunchuks I had always connection problems and dropouts at higher currents. With the original SMD NRF remote this got much better but was still not perfect. Finally the bigger long range with antenna work perfect and reliable up to 50m. 

Very important is to lower the 'Timeout when no control signal is received' from 1s to 100ms. Else it is possible, that the VESC keeps the last received command for 1s when the signal drops out, which happens mostly when you command full throttle... Don't ask how I know... Ouch...

The next important value is 'Timeout Fault stop time', which should be lowered from 1s to 100ms. Else the VESC needs 1s to recover after a short cutout which leads you to give even more throttle and tends to knock you off the board if the VESC powers up again.
```

---
## \#11 Posted by: Duffman Posted at: 2017-01-18T07:22:14.138Z Reads: 302

```
@The_Dude:

These are the components used:

Latching 6mm Push-Button-Switch for LED and Mode:
http://www.ebay.de/itm/50Pcs-6-Pin-Mounted-10mmx5-8mmx5-8mm-Locking-White-Push-Button-Tact-Switch-/191677440869?hash=item2ca0dda365:m:mi9xE5ww9D6bHTb0bB74krQ

Non Latching Push-Button-Switch for reverse and cruise control:
http://www.ebay.de/itm/25-x-DPDT-Momentary-6-Pin-DIP-Blue-Pushbutton-Flashlight-Switch-8mmx8mm-/291534361607?hash=item43e0cd5407:m:mzhqdg6JaTdOMfRkuNNMNdg

Thumb Stick without dead zone in the center: 
https://www.conrad.de/de/joystick-12-vdc-kunststoffhebel-print-alps-rkjxp-1224002-1-st-700620.html

NRF Long Range Module:
http://www.ebay.de/itm/NRF24L01-Wi-Fi-Modul-mit-Antenne-2-4-GHz-Funkmodul-Arduino-kompatibel-56-/122034562710?hash=item1c69d3a696:g:W8sAAOSwEzxYZBOF

Hex coded switch 0-F:
http://www.ebay.de/itm/Elma-07-0153-Horizontal-Hex-Coded-Switch-16-Position-0-F-6-Pin-Kodierschalter-/271767135206?hash=item3f469563e6:g:fWkAAOSwxYxU1LN8

The antenna mod was really simple: I pulled the antenna apart, desoldered the brass tube from the shielding and replaced it with a piece of wire of similar length. Additionally I cut the SMA connector and soldered the coax wire directly to the NRF PCB.
```

---
## \#12 Posted by: wmj259 Posted at: 2017-01-18T07:25:00.349Z Reads: 254

```
Have you had any drops?
```

---
## \#13 Posted by: Duffman Posted at: 2017-01-18T07:36:24.476Z Reads: 245

```
No, with those 'long range modules' it works perfect.
```

---
## \#14 Posted by: Okami Posted at: 2017-01-18T07:37:09.747Z Reads: 255

```
@Duffman Thanks for your response! I assume that spray paint finish on top of the smooth surface really makes the plastic stand out from the ''unrefined 3d prints'' :slight_smile:

Other than that - will have to probably play with pots some day and see how the values change, so thanks for going in detail with this one and mounting a little pot instead of resistor might be a good idea, at least till the ''perfect'' value is met :slight_smile:
   
----
[quote="Duffman, post:10, topic:16212"]
because the charging electronics on the PCB is very sensitive to any resistance in the connection to the battery.
[/quote]

Well, this is something interesting I have not heard of.. is it original nunchucks pcb which is sensitive or you meant your own etched pcb? (It looks like you made your own , sorry I I skipped something)

---

From your posts it looks like it is possible to overcome the nunchuks ''finickies'' / difficulties, if you plan ahead.. otherwise a feature rich remote, if you get it working properly.. which it seems you did in the end :)
```

---
## \#15 Posted by: Duffman Posted at: 2017-01-18T07:47:03.419Z Reads: 229

```
The PCBs were manufactured by OshPark and self assembled.

The charging circuit in combination with the voltage regulator on Benjamin Vedders Nunchuk RF PCB are sensitive to the resistance in the battery cable. If it is soldered directly or connected with a low resistance connector it works without problems, but when you put a switch in the power line, the submitted throttle value swings by some ten percent around the actual value.
```

---
## \#16 Posted by: Okami Posted at: 2017-01-18T08:12:28.573Z Reads: 224

```
@Duffman Ok, so from you I understand you get an ''interference'' for the throttle value.. just from the switch alone.. 

that''s something I have not heard of but I assume sensitive electronics does get interference more easly..

Might as well measure resistance of my dc switch Im using for the board.. who knows, perhaps it is eating up a few watts without me knowing :)

--

Anyways, at least now I know the reason why you had to go the ''connector as a switch'' route.. that was one of the first things I saw interesting that you had developed such a refined circuitry (wiring), just to accomodate the physical connector..
```

---
## \#17 Posted by: Duffman Posted at: 2017-01-18T08:17:42.621Z Reads: 222

```
I've tried several switches and just the bigger/better/bulkier ones worked, so I took the dead mans switch approach...
```

---
## \#18 Posted by: Duffman Posted at: 2017-01-27T06:41:16.556Z Reads: 239

```
A bit off topic, but this is how I post process my 3D printed parts. The shown are not realted to this remote and were actually printed on a professional 30k€ printer, which also suffers a bit from Z wobble and blobs. 

First I roughly sanded the print to get rid of the printing artifacts:
<img src="/uploads/db1493/original/3X/3/6/3698d80baea52506e1381904335310d0c4e9131e.jpg" width="690" height="388">

Then I smoothed the sanding marks with steel wool:
<img src="/uploads/db1493/original/3X/b/c/bc333cc33caaca2a14319bcc9f91924bcccb290c.jpg" width="690" height="388">

Then I just sprayed the parts with matte black paint:
<img src="/uploads/db1493/original/3X/b/c/bcccaf109a8a1ecf6273dcd9a7836dc936b4f42a.jpg" width="690" height="388">

After drying there were still some artifacts and scratches:
<img src="/uploads/db1493/original/3X/e/5/e588e8530ee616dfa222cc871bf57a0c870d0b59.jpg" width="281" height="500">

So here is the trick: For the last layer I sprayed from a too far distance to get little blobs and speckles on the surface, which hide little imperfections:
<img src="/uploads/db1493/original/3X/3/a/3a86d6878d78243ea9d0f12c8c155d7212693c06.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/2/a/2a99e9a3aee46337623ba91a4505dbaf1983dc7a.jpg" width="690" height="388">
```

---
## \#19 Posted by: Maxid Posted at: 2017-01-27T07:35:59.618Z Reads: 222

```
I am actually a little disappointed with the print quality when this was in fact a 30k€ printer.
A uPrint SE gives you basically the same level of quality (you can look at my prints) and costs like a third of that.
But nice trick to get the surface smooth. Did you ever try acetone vapor?
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-01-27T07:44:59.849Z Reads: 219

```
why didn´t you just use some spray filler?
```

---
## \#21 Posted by: Duffman Posted at: 2017-01-27T08:22:50.518Z Reads: 210

```
@Maxid: Yep, this is reality. 

Ok, the printer is a 6 year old Dimension Elite, so maybe the newer generations offer better quality. But the main difference and justification for the price is usability. You can send every part and every geometry in every orientation to this printer, it will automatically generate dissolvable supports and just print it without any need for tuning.

For these ABS parts I could have used acetone vapor, but at home I normally print PLA which can only be mechanically smoothed.

@TarzanHBK: Filler is on my 'have to try list' since since a long time but I always came over it... Any recommendations??
```

---
## \#22 Posted by: TarzanHBK Posted at: 2017-01-27T08:33:23.591Z Reads: 208

```
I´d go with Spraymax products. Especially this one for plastic parts:
http://www.spraymax.de/index.php?id=871
```

---
## \#23 Posted by: Maxid Posted at: 2017-01-27T08:35:44.669Z Reads: 220

```
[quote="Duffman, post:21, topic:16212, full:true"]
Ok, the printer is a 6 year old Dimension Elite, so maybe the newer generations offer better quality. But the main difference and justification for the price is usability. You can send every part and every geometry in every orientation to this printer, it will automatically generate dissolvable supports and just print it without any need for tuning.
[/quote]
Just like the uPrint. Actually the uPrint is the "workhorse" at work because it will simply never fail and will print everything you throw at it. We also have two leapfrog printers (a Xeed and Bolt) which supposedly have a way lower layer thickness of just 10um (uPrInt has 250um) - reality though is that they often struggle and the final result is worse than on the uPrint.
We just recently had to upgrade to the uPrint SE when our original uPrint from 2007 died - quality wise I have not noticed any difference between the two - well the support material is a little easier to break off and dissolve but that is about it.
Next time you need a new printer might give this one a shot ;)

Edit: Just looked the dimension elite up and it is also from Stratasys :D - I guess the actual difference is then more in the lines of printable size and speed. The Dimension Elite seems to be a bit more polished and faster than the uPrint.
```

---
## \#24 Posted by: Duffman Posted at: 2017-01-27T08:48:52.836Z Reads: 206

```
Yep, you're right. I guess they use pretty much the same technology and mechanics. It looks like the uPrint is the little brother of the Dimension.

@TarzanHBK: I'll take a closer look, but I will go with 1K filler, because I usually have small parts.
```

---
## \#25 Posted by: TarzanHBK Posted at: 2017-01-27T09:03:27.107Z Reads: 196

```
yah you´re right with only one of these housings you´re better with 1k. Should go too with Spraymax :slight_smile:
```

---
## \#26 Posted by: The_Dude Posted at: 2017-02-05T18:14:09.805Z Reads: 194

```
Hi Duffman,
how did you get the pins of the hex switch facing vertically? Did you cut the hex switch in the middle to get inner access and then bend them upwards.
```

---
## \#27 Posted by: Duffman Posted at: 2017-02-05T19:11:31.035Z Reads: 191

```
Yes, I cracked the back cover off, sanded the plastic down, cut the pins and bent them to shape.
```

---
## \#28 Posted by: The_Dude Posted at: 2017-03-14T20:49:25.217Z Reads: 211

```
Hey man from Albuquerque,
5-Star-Rating for your build. Finally I made my own one, thanks.
<img src="/uploads/db1493/original/3X/a/3/a3b3955c44dacb5d011d53637bc59ce8f125cbea.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/9/9937686d11b1f2606528e73bb037929aa9ec95f7.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/3/d3d428d45bc2dc8607afb35a681a0eec87cdf297.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/5/350791bce98d447f620eb9becd005edf11ad38df.JPG" width="375" height="500">
```

---
## \#29 Posted by: Duffman Posted at: 2017-03-15T08:42:48.380Z Reads: 195

```
Great build and nice finish! I love the mod with the thread inserts.

Did you already take it out for a ride? How do you like the feeling of it?
```

---
## \#30 Posted by: The_Dude Posted at: 2017-03-15T16:14:58.940Z Reads: 194

```
Ride outside is on my list ... follows soon.
```

---
## \#31 Posted by: Duffman Posted at: 2017-03-16T13:18:27.989Z Reads: 196

```
Hey @unik, did just out of curiosity a size comparison of my NRF remote and your Sparkle. Could have bet, that there was more difference in size:

 <img src="/uploads/db1493/original/3X/7/0/70805a90ff7b825d7c2a97d833ca9bcbe61a2e04.jpg" width="300" height="250"><img src="/uploads/db1493/original/3X/3/8/3822eb29c1143640bcae86761452e0f37f7a06d8.jpg" width="300" height="250">
<img src="/uploads/db1493/original/3X/3/4/3415a7ee174f101c02dc1b049ea7e0ce9499e1ae.jpg" width="300" height="250"><img src="/uploads/db1493/original/3X/a/2/a291cf4156454fc65c0a9de35b2a22b89ae4b012.jpg" width="300" height="250">
```

---
## \#32 Posted by: bimmer Posted at: 2018-02-08T05:03:07.198Z Reads: 129

```
would this work with the vesc-6?
```

---
## \#33 Posted by: ZackoryCramer Posted at: 2018-02-08T05:11:49.220Z Reads: 130

```
I would think VESC 6 has the same UART communication protocol, but I am not 100% confident.
```

---
## \#34 Posted by: bimmer Posted at: 2018-02-08T09:43:24.590Z Reads: 124

```
I mean it has an nrf chip I want to know if that works.
```

---
## \#35 Posted by: rpn314 Posted at: 2018-02-08T15:51:09.956Z Reads: 121

```
This is literally just a shell for the NunchuckRF that Benjamin built, which I believe is compatible with VESC6
```

---
## \#36 Posted by: Duffman Posted at: 2018-02-08T17:47:05.788Z Reads: 122

```
The new firmware that runs on the VESC6 uses a new pairing method, so you need the newest firmware on the NunchukRF.
I still have not tested it, because I like the pairing via hex switch, but it should run perfect with VESC6.
```

---
## \#37 Posted by: bimmer Posted at: 2018-02-09T04:56:22.077Z Reads: 116

```
Thanks I might look into having those made then.
```

---
## \#38 Posted by: Nordle Posted at: 2018-02-09T08:08:09.530Z Reads: 117

```
I would like to have a source for the nunchuck-pcb's, would be nice if you could sell them seperate;)
```

---
## \#39 Posted by: stewii Posted at: 2018-02-09T09:02:58.339Z Reads: 113

```
I use a nunchuckRF with ESCape and it works as it should except the ws2812 light controls ( you need to change the firmware )
```

---
## \#40 Posted by: Duffman Posted at: 2018-02-09T09:15:57.434Z Reads: 118

```
@chaka posted a link to osh park where you can get the pcbs cheap and easy:
http://www.electric-skateboard.builders/t/vesc-nunchuk-rf/588/30
For all other parts check the first post in this thread.
```

---
## \#41 Posted by: Nordle Posted at: 2018-02-09T11:00:51.676Z Reads: 114

```
I have shaky hands;) i ment assembled pcb's. @bimmer looks like he's starting a buisness or doing us a favor
```

---
## \#42 Posted by: bimmer Posted at: 2018-02-09T11:34:04.867Z Reads: 117

```
I am making hw 6.4 esc's based on vesc 6 and would like a easy remote option without additional receivers that why I'll make them.
```

---
## \#43 Posted by: Duffman Posted at: 2018-02-09T21:11:11.176Z Reads: 113

```
Honestly I have no idea why this remote only got such a little bit attention. Everyone is selling vescs but no one is selling the remote that was developed for the vesc??
I have no intention and no capacity to produce those but I could help out with 3d printed parts and instructions...
```

---
## \#45 Posted by: relations99 Posted at: 2019-03-30T05:22:24.138Z Reads: 48

```
@Duffman did you use custom firmware in the vesc to do this? (connecting nrf straight to vesc) and what config do I need to setup on the vesc?
```

---
