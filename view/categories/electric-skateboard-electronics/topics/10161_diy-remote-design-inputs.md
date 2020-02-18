# DIY remote design inputs

### Replies: 53 Views: 4695

## \#1 Posted by: B4Me Posted at: 2016-09-26T12:36:29.899Z Reads: 412

```
Hi guys
I'm fidling with a new design for a remote..
I have so far planned on using the following parts:
Arduino mini pro
0.96" OLED with i2c or spi
HC05 (bluetooth module)
18650 (single cell)
some sort of lithium charging circuit (ebay have some cheap)


My current design looks like this:
<img src="/uploads/db1493/original/3X/d/2/d2ecf032cba3a7190805ecd5c77f2a2d5052c449.PNG" width="134" height="500"><img src="/uploads/db1493/original/3X/9/b/9bca39c75803c6a0a4dcdf5749f2527cd486e05c.PNG" width="266" height="500"><img src="/uploads/db1493/original/3X/e/7/e7e68d84dbf4bb61dffa3bbb21c5707812ed78e2.PNG" width="208" height="500">

It is missing the dead-man-switch...


What would you like to have on a remote, if you could add things ?
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-09-26T13:30:43.920Z Reads: 384

```
Please do not use bluetooth for the transmission of the control signal, it has proven to be unreliable.
A remote that drops out and tries to kill you is not what we need in a sport this dangerous.
If you can fit a 2.4ghz transmitter (e.g. the NRF24L01), it would be more reliable.

EDIT:
Maybe you wanto to refer to this thread:
http://www.electric-skateboard.builders/t/what-products-solutions-do-you-want-for-electric-skateboards-designing-a-remote/9423

100% Realiability is the No.1 requested "Feature"
```

---
## \#3 Posted by: Stevemk14ebr Posted at: 2016-09-26T13:41:34.535Z Reads: 364

```
If i designed a controller it would have two 2.4ghz radio modules, both paired all the time and they would act as redundant radios so even if one radio disconnects the other is fine. I would also add a small spring actuated switch to the front that would control turn signals, and one button on the side for headlights.
```

---
## \#4 Posted by: chinzw Posted at: 2016-09-26T19:43:40.110Z Reads: 340

```
You dont need 2 radio modules, just a receiver that handles dropouts properly
```

---
## \#5 Posted by: Stevemk14ebr Posted at: 2016-09-26T21:31:25.887Z Reads: 322

```
since when is redundant design a bad idea? Especially when i'm trusting my life to a board, i'll keep my two radios.
```

---
## \#6 Posted by: Mrmoonlight Posted at: 2016-09-26T22:18:56.503Z Reads: 311

```
Yup, well beyond everything else is reliability. I'd pay twice the price in a heartbeat for a more reliable remote. 

Besides that, I like the thumb slider switches and a battery level indicator.
```

---
## \#7 Posted by: Pantologist Posted at: 2016-09-26T22:20:15.110Z Reads: 306

```
Battery level for the board? 

That would need Bluetooth. 

I am thinking, a Bluetooth and 2.4ghz transmitter. So you can easily integrate data and have a reliable remote.
```

---
## \#8 Posted by: Mrmoonlight Posted at: 2016-09-26T22:29:30.092Z Reads: 301

```
Battery level for the remote only. I'm fine with just the level on the board. My EGO has an indicator and it comes in handy. 

So far, my favorite remote has been the EGO remote. I don't need the sport/rabbit modes of flash light, but I like the slim design. So far, I've never had a single drop out on that remote.
```

---
## \#9 Posted by: Pantologist Posted at: 2016-09-26T22:45:58.931Z Reads: 293

```
We might as well make a smart remote if we are going to spend the time making a custom one anyways. I am going to try and mod my Mini Remote into a thumb one with bluetooth.
```

---
## \#10 Posted by: chinzw Posted at: 2016-09-27T01:31:10.814Z Reads: 281

```
Then you'll need 2 receiver modules too...
```

---
## \#11 Posted by: Stevemk14ebr Posted at: 2016-09-27T05:23:16.617Z Reads: 268

```
ok so then i need two receivers. A 2.4ghz radio chip is like 4 dollars. The electronic guts of a remote could be under $30 even with dual radios if you did a custom circuit. When i'm done with college this summer i will be making my own.
```

---
## \#12 Posted by: B4Me Posted at: 2016-09-27T06:36:14.318Z Reads: 260

```
I have NRF24L01 aswell, but why do you think its more reliable ?
I think 2.4Ghz is still 2.4Ghz... is it the BT handshake thats to slow to recover well ?
```

---
## \#13 Posted by: mrpj Posted at: 2016-09-27T06:38:10.836Z Reads: 277

```
@B4Me

I've been working on a custom remote myself - but from a different angle so far. I have focused on the schematics and electric side. I am looking for other people that might be interested in teaming up and working together on the remote. 
On my side, the main schematics (with charging circuit, usb2mc connection and other things) is done, but I haven't had the time (and skill) to start with a case. I'd like to have the case first, in order to fit in the pcb (and create a layout on top of it)

Anyhow - if you are interested let me know.

Per your design - some suggestions from what I have gathered myself:

- dead man`s switch (from what you already noted)

- some menu button(s) to navigate and change settings

- you might think of moving the display further down / towards the bottom. Most oled display have a fairly large pcb themself (usually around 3x3cm) and thus your display would most likely be taking space from the throttle system

@flatsp0t @Stevemk14ebr @Mrmoonlight @Pantologist

All your solutions mentioned work in the 2.4 ghz spectrum (actually 2400Mhz - 25xx Mhz) and they would all be prone to the same problems in urban areas. Just because you name it differently and have a different specification, doesn`t mean that there is suddenly more "space" in the medium. They all have to share the 2.4Ghz band ([see wiki](https://en.wikipedia.org/wiki/List_of_2.4_GHz_radio_use)). So even if you include a second radio, you will need to deal with interferences. Your everyday 2.4 GHZ hobby remote is not built to be used in highly con-quested areas - and on top of that - the protocols are fairly simple and will not deal with packet loss / re-transmissions (/ encryption). 

So where to go from here? 

- choose a different frequency band: go for 433MHZ or 868/933MHZ ISM bands. Even though you will have lower bandwith - it is vastly sufficient for realtime data from the vesc and from the remote. (100hz for controls and 10hz or less for displaying information is more than sufficient - assuming that control data is ~10 bytes (one axis, 1 button) and vesc information ~300 byte - we would need less than 5kb/s constant data connection ;-))
The benefits are, that these frequencies are less common and used - so less prone to con-question and other problems

- choose a specification that handles packet collisions, re-transmissions, con-question, channel/frequency switching reasonably well (from all mentioned actually wifi has the best specifications - highest transmision power (compared to bluetooth), low latency transmissions, encryption with wpa(2) etc.) 

- write your own protocol on top of a low level protocol (i.e. most 2.4 GHZ transceivers) to deal with mentioned issues

- write your application to actually account for packet loss, re-transmissions and include proper safeguards. 

Whatever you do, I can only recommend not to neglect the security issue with transmitting unencrypted data for your boards. Even if your data is encrypted, you should also account for packet replay attacks and other malicious attacks - it is your life you are dealing with here. And creating a harmful device is fairly easy. (Even if it is just to jam signals .... )
```

---
## \#14 Posted by: B4Me Posted at: 2016-09-27T06:39:18.940Z Reads: 234

```
I like the idea, but if you want redundancy, it should NEVER be on the same frequency.. then you would want 2.4G and 5Ghz.. or 868Mhz, you get where I'm going.. having the same frequency, will make matters worse for both radios... and if the 2.4ghz is flodded due to wifi or some other thing.. everything is dead now
```

---
## \#15 Posted by: B4Me Posted at: 2016-09-27T07:02:40.488Z Reads: 261

```
You are a very gifted guy ! I must say..
I am my self a civil engineer, mechatronic master degree (software, mechanical and electronics)..
You have some excellent points in the things you are saying.. I have decided on NOT to make the PCB's from scratch (atm).. I design PCB at work, so at home I mostly rely on ebay and kits, there are so many dev boards out there :slight_smile:
Hope you get what I mean.. I dont dislike the PCB design, but it is not necessary unless you are thinking about mass production, or like the finished feeling of a PCB :slight_smile:
If you can come up with a case design idea, and measurements or step files for internal components, I will definitely help designing your case :) 

I actually have some RFM12 modules (433Mhz), every car owner will hate me driving by (should use that frequency on car locks :D )
But maybe thats the way to go, or on the skateboard I could have both BT and 433, then I could get more info on BT and less for the 433 remote :slight_smile:
But as stated by you, security is key, and fall back strategies.. 
eg. slow down and stop if signal is lossed, some encryption, or and incrementing number so playback attacks cant happen as easy that is..

But on the OLED I want things like:
Batt level
Watt (in or out and amount)
Wh used/left
Kmt or RPM (same same if you know the gearing and wheel dia)
remote battery level
```

---
## \#16 Posted by: B4Me Posted at: 2016-09-27T07:06:40.889Z Reads: 241

```
The display position is indeed where it needs to be atm :slight_smile:
 ... or maybe I will make the remote 5 mm higher, to push battery and oled down, as I have some hard time to place the counter part for the rotating rod in the top cover

<img src="/uploads/db1493/original/3X/e/2/e2bb7178e89a1561d33b7cb0c1262bb4b4aa4ed5.PNG" width="690" height="374">
```

---
## \#17 Posted by: mrpj Posted at: 2016-09-27T07:32:23.352Z Reads: 239

```
Thanks for the compliments - everyone has something he likes to dive into when doing things. That`s why I like communities - people get together to exchange ideas and discuss and then something will evolve from that.

So anyhow - just a short response:

I understand where you are coming from in regards of pcb design - to be honest - these days ordering pcb prototypes (in small quantities) from china is quite reasonable. I like to tailor things to my needs (luckily I am not doing this at work - so I guess that is why I like to do them in my free time). I feel that the remote will be a "tight fit" and thus I thought about creating a PCB (also allows for choosing components ;-) )

And it doesn`t need to be mass production - but if there are more people interested in the pcb - there is always the option of doing a group buy (but people will need to assemble themselves). 

Even your 433Mhz is plenty of bandwith - the data from the vesc to the remote doesn`t have to be very frequent (10hz or less is enough) - in my concept, I was planning to let the remote "stay dumb" when it comes to sending the information. From my point of view, just sending the position and state of the trigger is sufficient and requires just a few bytes -> low bandwith. It adds the benefit that the receiving controller (or the controller on the vesc) will be able to deal smoothly with dropped/lost packets and act accordingly to safeguard. It might be again overkill to have both bluetooth and 433 in the remote. (On the receiver side there it might be an option to connect via smartphones/laptops for changing vesc settings) 

Looking at the exploded view, I can see why you moved the display to the top section. My take on this: don`t make the case too thick - it will feel more heavy in the end, than it actually is. Is there any particular reason for going with 18650 cells over a lipo flat pack? (Having a good charging ic (i.e. max1555), and a protection/undervolt circuit you can keep them in safe operating zones)
```

---
## \#18 Posted by: mrpj Posted at: 2016-09-27T07:34:19.759Z Reads: 236

```
Oh and forgot to say: you might consider going up from 433 mhz to 868/933 mhz - 433mhz antennas will be quite large - that's whats keeping me from choosing 433 so far
```

---
## \#19 Posted by: B4Me Posted at: 2016-09-27T07:37:39.592Z Reads: 241

```
Is it like 12CM long ? it dosnt need to be a wip antenna, it could be pig tail design (coiled wire)
Or a pcb antenna .. lay it down aside the hand 

<img src="/uploads/db1493/original/3X/e/1/e1ff422bd205de47f855a545122847c6c81b2c41.jpg" width="601" height="500">
```

---
## \#20 Posted by: B4Me Posted at: 2016-09-27T08:16:39.598Z Reads: 239

```
I will admit the fealing of your own PCB is awesome ! but sparetime is key.. and there exist so many dev boards where only the wires between is missing :D
Maybe I will design a pcb if the prototype works :slight_smile:

I also think 433-868 is a good choice after the 2.4ghz discussion, as the frequency is NOT flooded, at least in europe, I think both a illegal to transmit over 1-2% duty, so it's like a change of 1-2% to get noise from other sources on these frequencies :)

The idea with BT and 433 was just to have the remote ONLY 433, but my phone of home could get diagnostics out of the board.. and should the remote fail, an app could get the board running the way home :D

18650 was due to the easy access, go to a dumbster, grab nearest laptop battery, 5-7 good cels out of 6-8 batteries
I have a lumber hand (some would say.. :P )
So I dont wont to make the remote to flat, it will end giving me some pain in the hand (hard to explain in english.. but if you hold on something flat and thin for a long time, my fingers/palm is in pain..)
Therefor the 18650 was good capacity and size when I anyways want the fat grip (it is only 20mm thick 18mm battery dia + 2x1mm plastic)
```

---
## \#21 Posted by: mrpj Posted at: 2016-09-27T08:49:20.202Z Reads: 219

```
In regards to antenna length - you got to check if you are going for 1/2 or 1/4 length and test. I just know that a good 868 mhz antenna (with coils) would be around 6cm. Just something that has to fit in the case ;-)

It`s true that there are plenty of developer boards out there - for a prototype it's definately sufficient - I just like to make it into something clean in the end. But as it is with most prototypes - they stay like they are right? ;-)  - so I started designing them from the start already into the direction haha

Ah I get why the 18650 - I honestly wouldn't worry so much about pricing for a battery. (lipo is 3-4 euros) - if it is easier to fit things into a case. I do get what you mean with your palms - I have rather normal hands and thus 2cm is the max that feels comfortable for me. 

Anyhow - if you like and want - we can have further discussion and share our results - and/or work together on a prototype.
```

---
## \#22 Posted by: B4Me Posted at: 2016-09-27T08:57:38.593Z Reads: 217

```
I dont think the antenna atleast should be the reason to go ghz ;)

You are so right there sir ! If it works.. why use time perfecting it.. thoe.. it feels great to have a finished product like yoours ;)

My current remote:
https://www.aliexpress.com/item/F01719-3-Flysky-FS-GT3B-2-4G-3CH-Gun-Transmitter-Receiver-RC-Car-Boat-FS-GT3B/32339629939.html

Is way thicker.. it lays great in the hand.. but I think 20mm is where it goes from nice laying in the pocket all day.. to 25mm where it felt awefull (atleast with my first prototype design print)
(do you have access to a 3d printer ? could send a stl file, then you could try to feel it in your hand)
Maybe I change to flat lithium cells, the 18650 is just the start :slight_smile:
I just like the cell I think :blush: 

I would love to work with you !
Whats your geographic location on this planet ?
Mine is Denmark
```

---
## \#23 Posted by: B4Me Posted at: 2016-09-27T10:48:13.283Z Reads: 202

```
Seems as if RFM69 is the new player intown.. it can be 433-868-915Mhz, så plenty of options, for about 2£ only :smiley:
```

---
## \#24 Posted by: mrpj Posted at: 2016-09-27T16:58:23.080Z Reads: 220

```
I have access to a 3d printer at a fablab closeby - but unfortunately don`t own one myself :cry:

Don`t feel obliged to change anything - I like to bounce of ideas and discuss them - sometimes I have an idea and I don't realize it's actually not good/feasible until some tells me ;-)

Yes the RFM69HCW modules are great - they have quite robust protocol already - and they offer hardware encryption with aes128 (that should be sufficient to not be harmed by someone/something just poking around ;-) )

There is a development board called "moteino" with a really [great forum](https://lowpowerlab.com/forum/moteino/)  - there is a lot of information in regard to that developer board an to rfm68 modules in general.

I am from the south of Germany - so not to far apart ;-). btw I just noticed that we started talking about vesc (and vesc 6.0) beforehand :flushed: - didn`t realize it until now.
```

---
## \#25 Posted by: B4Me Posted at: 2016-09-27T18:11:41.176Z Reads: 218

```
<img src="/uploads/db1493/original/3X/e/4/e48764145b0c8347a5d6533e69e3676803da3b9a.jpg" width="317" height="500">
Version 4 of the case :D
```

---
## \#26 Posted by: karma Posted at: 2016-09-27T19:42:18.274Z Reads: 212

```
This topic is really interesting and fun to read! Keep it up! :smiley:
```

---
## \#27 Posted by: B4Me Posted at: 2016-09-27T20:45:23.640Z Reads: 217

```
<img src="/uploads/db1493/original/3X/9/8/98e5890793f6e985b043982abacb88a5bf54b97f.jpg" width="375" height="500">
```

---
## \#28 Posted by: B4Me Posted at: 2016-09-27T20:52:48.761Z Reads: 209

```
I will keep it running, until the remote is a working finished device :D
maybe others want one at that time :smile:
```

---
## \#29 Posted by: B4Me Posted at: 2016-09-27T21:38:27.733Z Reads: 206

```
Fablabs are great ! but if you one day get the possibility, buy one, especially if you like designing custom electronics.. its awesome to make the perfect casing for your projects :D (wall mounted tablets, rc remotes, custom fan for motors, battery compartment for esk8-boards)

just keep the ideas flowing, I will if possible try to incorporate the ones I can apply :smiley:

The RFM manufacturer are really good, also when it comes to documentation, eventhough they gave me a hardtime in 2011 trying to get rfm12's to work :stuck_out_tongue:

Awesome ! I will give the forum a look later in the project then :smiley:

South of Germany, south of Denmark, awesome ! :smiley:

I know ;) and the VESC assembly is most properly starting within two weeks :)
```

---
## \#30 Posted by: nico_civic5 Posted at: 2016-09-28T09:38:06.587Z Reads: 198

```
Dear i have a question for you. 
I recently lose my remote control for my electric skateboard 800w zles. And i cant find the same. I buy a new one with the reciver buy the plug has 3 cables and the reciver of my board has 4 white cables. And u dont know how to pair it. I can pair the newcontrol with the old reciver?  I have to change the reciver? I send you some pics for you to see.
If you can help me i really apreciete because in my country no body knows so much for electric skateboards.
```

---
## \#31 Posted by: mrpj Posted at: 2016-09-28T11:12:19.783Z Reads: 200

```
I had a quick look for small size antennas:

I found a couple of helical antennas for cheap on aliexpress 

- [433 MHZ](https://www.aliexpress.com/item/10Pcs-433MHz-Helical-Antenna-2-5dBi-32mm-for-Remote-Contorl/32608690665.html?spm=2114.30010308.3.100.T4ezj9&ws_ab_test=searchweb201556_10&aff_platform=aaf&sk=QFEEaUzZF%3A&cpt=1475059263424&aff_trace_key=bacc8e7902b044eca115efb719facc4f-1475059263424-02317-QFEEaUzZF)
- [868 MHZ](https://www.aliexpress.com/item/10Pcs-868MHz-Helical-Antenna-2-15dBi-13mm-for-Remote-Contorl/32610707134.html?spm=2114.30010308.3.44.Q55h8h&ws_ab_test=searchweb201556_10&aff_platform=aaf&sk=7yNjiEMZ7%3A&cpt=1475059261870&aff_trace_key=bacc8e7902b044eca115efb719facc4f-1475059261870-02220-7yNjiEMZ7)
- [915 MHZ](https://www.aliexpress.com/item/10Pcs-915MHz-Helical-Antenna-2-15dBi-12-5mm-for-Remote-Contorl/32608721336.html?spm=2114.30010308.3.10.Y4kw9g&ws_ab_test=searchweb201556_10&aff_platform=aaf&sk=QrV3Ja2FM%3A&cpt=1475059265019&aff_trace_key=bacc8e7902b044eca115efb719facc4f-1475059265019-05408-QrV3Ja2FM)

I guess it would be best if we can fit the antenna (16 - 30mm) in the upper part of the casing - next to the speed throttle? 

During my search for a throttle I was actually planing to use a [joystick potentiometer](https://www.aliexpress.com/item/2-Sets-3D-Analog-Joystick-3-Pin-Sensor-Module-Potentiometer-with-Thumb-Sticks-for-Playstation-4/32728004271.html?ws_ab_test=searchweb201556_8,searchweb201602_1_10065_10068_112_10069_110_111_418_10017_109_108_10060_10061_10062_10057_10056_10055_10054_10059_10058_10073_10070_10052_10053_10050_10051,searchweb201603_7&btsid=f09bfc6e-29b5-42fb-b518-1e10d76952b7) and either just guide the axis of the throttle to be solely y bound. Or take it apart and create a different mount.

Another option would be to go down the hall sensor route (similar to [boosted board remote](http://puu.sh/q0H0b/ccfb3e1047.jpg)

I unfortunately haven`t had much to do with electronics (in form of communication technology) to asses if the magnets however would interfere with the antenna - will ask some people who actually studied that to see if they have any remarks.

Do you have some measurements of the case for me? Then I would start with designing a PCB in the next weeks
```

---
## \#32 Posted by: B4Me Posted at: 2016-09-28T12:05:07.399Z Reads: 185

```
I would try to contact the manufacture, as 4 white cables dosnt tell much :(
```

---
## \#33 Posted by: B4Me Posted at: 2016-09-29T06:41:30.154Z Reads: 192

```
I think at least that the antenna is best suited with being in the top, outside the hand, else you could interfer..
The small joystick or potentiometer ideas are really good, but I think hall effect is the simplest and smallest footprint to build
It shouldnt interfer, aslong as the halleffect sensor is sub-mhz, and the antenna is mid-high Mhz range :slight_smile:

Which ECAD software are you using ?
Can it import step og DXF files ?
```

---
## \#34 Posted by: mrpj Posted at: 2016-09-29T08:36:27.097Z Reads: 186

```
I am not yet completely sure about the hall sensor as throttle - have no experience with using a hell sensor so far. And any design implications that a setup like this requires. I am just hesitant in regards to any interference - also in relation to the hall sensor. Probably will order some sensors and test/play around with them to see how they behave and react ;-)

I am using Cadsoft Eagle - it is actually the one ECAD I`ve grown up with and am by now the most comfortable. It seems that it [supports dxf imports](https://todbot.com/blog/2011/06/06/from-illustrator-to-eagle-vector-graphics-in-circuits/comment-page-2/) but I haven't used them yet ;-)

Maybe it is time to move to a different ECAD software - heared great things about KiCad?
```

---
## \#35 Posted by: B4Me Posted at: 2016-09-29T13:59:29.907Z Reads: 174

```
Try to order some S49E, they are pretty cheap on ebay, and works down to 3V, and are NOT a hall effect switch ;D

Actually I havent used anything else than Altium, mainly due to me line of work ;)

But KiCad seems really awesome!
I'll try to export some DXF of a cut section, then you know the envelope of your board, if you want the same shape, that is ;)
```

---
## \#36 Posted by: mrpj Posted at: 2016-09-29T14:38:16.206Z Reads: 184

```
[quote="B4Me, post:35, topic:10161"]
Try to order some S49E, they are pretty cheap on ebay, and works down to 3V, and are NOT a hall effect switch ;D
[/quote]

I was looking at Hall Sensors from [AllegroMicro](http://www.allegromicro.com/en/Products/Magnetic-Digital-Position-Sensor-ICs/Hall-Effect-Unipolar-Switches/A1120-1-2-5.asp) to already deal with the behavior of SMD versions

[quote="B4Me, post:35, topic:10161"]
I'll try to export some DXF of a cut section, then you know the envelope of your board, if you want the same shape, that is
[/quote]

The general shape is great - just don't know how you feel about a "dead mans switch"?
Different question in that regard: would there be enough space in the upper part to place the RF69HCW module (16x16mm) and the antenna? 

There is no need to rush the DXF files - I'll probably don't get around doing the pcb layout before early october.
```

---
## \#37 Posted by: B4Me Posted at: 2016-09-29T22:55:48.525Z Reads: 191

```
the link was broken :frowning:
[http://www.allegromicro.com/en/Products/Magnetic-Digital-Position-Sensor-ICs/Hall-Effect-Unipolar-Switches/A1120-1-2-5.aspx](http://www.allegromicro.com/en/Products/Magnetic-Digital-Position-Sensor-ICs/Hall-Effect-Unipolar-Switches/A1120-1-2-5.aspx) 

If you run the pcb under, then smd is the way to go ;) 

I'am planning to design a trigger switch, for the index-finger, but should I do ON/Off or analog switch ? 

See this picture, its the RFM12 module, but I think its the same factor, as this also is 16x16
<img src="/uploads/db1493/original/3X/7/2/72f4ab64657201c7653a3a52ca3f2b009b07f13e.PNG" width="298" height="500">
But We'll just change the shape to the parts and back :slight_smile:

The following is only preliminary design.. but the basic shape is defined :)
DXF and PDF file:
http://www.fileconvoy.com/dfl.php?id=gd0da7c288b53d0189998803219660930ca3687026

And this drawing is at the center, of the remote
```

---
## \#38 Posted by: mrpj Posted at: 2016-09-30T06:58:00.174Z Reads: 189

```
Going to post a couple of thoughts and findings ;-)

[quote="B4Me, post:37, topic:10161"]
I'am planning to design a trigger switch, for the index-finger, but should I do ON/Off or analog switch ?
[/quote]

If we have the throttle at the thumb, I think a ON/OFF switch for the index-finger (as trigger / dead man`s switch) is suffice. Will keep the design simpler and I don't see any usage scenario for also doing this part analog (i.e. with a hall sensor). 

Some thoughts on the thumbwheel:

- For the hall sensor to be more precise, allego micro propose a [push-pull](http://www.allegromicro.com/en/Design-Center/Technical-Documents/Hall-Effect-Sensor-IC-Publications/Hall-Effect-IC-Application-Guide.aspx#Q41) combination. That would require having 2 magnets and the hall sensor would need to be inbetween those two
- I propose to make the thumbwheel "more solid" - as I think the "dust guard" might break easily. Also this would provide more space for magnet configurations - what do you think?
- What mechanism do you propose to have the thumb return to neutral? (I was thinking that the thumbwheel is similar to the wii controler, that the movement is for acceleration/deceleration - or do you see it differently?)

I've tried to inform myself a bit more on antenna designs and the RFM module and found some [interesting notes](http://wireless.murata.com/media/products/apnotes/antenna.pdf?ref=rfm.com)

On page 7:
> When the coil runs near and parallel to ground, maximum gain is only -18 dBd. When the loose end of the coil was pulled away from ground, as shown in the alternate version drawing, gain increased to -5.5 dBd, and the null became deeper.

and

> The big problem with this antenna is the mechanical construction and it's bulky size. It can be easily de-tuned by nearby objects, including a hand, so it may not be good for hand-held use. 

So I wonder if it would be good to keep the current space of the RFM module just for the antenna and move it further down? Also the note on the application with a hand nearby worries me slightly :-(

On a different note - since you switched to lipos, wouldn't it make sense to also move the OLED display closer to the bottom in order to not overlap with the center point of the thumbwheel?

On the topic in relation to communication, I've found a couple of interesting products/implementations. Most interestingly was [OpenLRS](https://openlrsng.org/). An open source RC implementation using 433 / 868 / 916 mhz modules, offering encryption, frequency hopping and other interesting features. It has been widely used by a lot of people for drones/rc planes. 
When I find the time, I will evaluate this firmware and see if/how it could be used for our remote. As far as I could tell though, it offers quite a lot of features (including telemetry). 

There are also "commercial" OpenLRS products  based on Atmega328P ([example](http://www.hobbyking.com/hobbyking/store/__27096__OrangeRx_Open_LRS_433MHz_9Ch_Receiver.html), [example 2](http://www.hobbyking.com/hobbyking/store/__40032__OrangeRX_Open_LRS_433MHz_Transmitter_100mW_compatible_with_Futaba_radio_.html)) available.
```

---
## \#39 Posted by: B4Me Posted at: 2016-09-30T08:30:34.498Z Reads: 172

```
I will reply more thoroughly later.. but for now take a look on this guys design

https://www.radicalcreation.com/forums/viewtopic.php?f=6&t=35&sid=1657148f8f9f4948887332cdcd84c904

thats my inspiration for the thumb controll, push pull and return, everything is shown in his videos :)
```

---
## \#40 Posted by: B4Me Posted at: 2016-10-01T16:48:57.340Z Reads: 177

```
You really did some research here ! :D like it !
I dont think you should be so worried about the hand at the antenne, remember these devices are used for ranges upto 0,5km .. we "only" need 2-10 meters :)
I actually think.. if we dont give a f.. about the PA stage in the module, we could do it with out antennas on :stuck_out_tongue:
 
That stack, or what its called.. openLRS, is really awesome ! but is it maybe over complicating the software ?
I mean, I want encryption, and telemetry, but if the code still needs to be edited by the users, arduino ide ?.. then a simpler setup could maybe do the stuff

What do you think ?
```

---
## \#41 Posted by: mrpj Posted at: 2016-10-02T15:20:30.142Z Reads: 171

```
[quote="B4Me, post:39, topic:10161"]
https://www.radicalcreation.com/forums/viewtopic.php?f=6&t=35&sid=1657148f8f9f4948887332cdcd84c904
thats my inspiration for the thumb controll, push pull and return, everything is shown in his videos :slight_smile:
[/quote]

That design looks great. Though I would place all switches/components on the pcb (like it is done in the boosted remote). 
I've been thinking what the easiest/best approach to move from your the case design to the pcb shape (with drill holes, and proper cutouts for certain mechanics (i.e. the thumbwheel)). Any suggestions? (the DXF only has a hole for the center of the thumbwheel, but I am not sure how much space is needed and if I could fully populate everything else ;-) )

[quote="B4Me, post:40, topic:10161"]
I dont think you should be so worried about the hand at the antenne, remember these devices are used for ranges upto 0,5km .. we "only" need 2-10 meters :slight_smile:I actually think.. if we dont give a f.. about the PA stage in the module, we could do it with out antennas on :stuck_out_tongue:
[/quote]

I would not omit the antenna - especially considering that we don't have a clear line of sight from the remote to the board receiver (i.e. board, human body etc. will dampen the signal). Also when testing some RF modules in the past, without antenna I had significant packet loss even if the modules where just couple of centimeters apart. :sweat:

[quote="B4Me, post:40, topic:10161"]
That stack, or what its called.. openLRS, is really awesome ! but is it maybe over complicating the software ?I mean, I want encryption, and telemetry, but if the code still needs to be edited by the users, arduino ide ?.. then a simpler setup could maybe do the stuff
[/quote]

I mostly looked at Open LRS for the protocol and the features - having a frequency spread spectrum (via channel hopping) is desirable for reliability. Almost all rm69 libraries I found, don't have channel hopping included. Somehow it also seems that the rfm22/23 had this feature directly on the module. Will see if I can find more information.

For OpenLRS there are toosl (similar to the bldc tool) to configure the remote. So it shouldn't be that hard - generally I see it the same as with the vesc - here people also need to adjust settings

In the end we can see if the open lrs firmware itself can be easily modified for our needs, or if it is feasible to port features over, or to write a custom solution. But I'd rather investigate already existing solutions (and learn the features/limitations) before starting from scratch
```

---
## \#42 Posted by: brun Posted at: 2016-10-02T18:00:19.282Z Reads: 155

```
I've built several remotes using both 433mhz and Nrf2401.  My experience with the nrf was good in terms of range and reliability but the biggest problem was that they interfaced the VESC  via its ppm/pwm 'app' that lacks all of the nice throttle ramping controls, instant torque after coasting that the nunchuck 'app' has which makes the riding experience so much better 

Does anyone know the protocol that the nunchuck uses to communicate with the vesc?
```

---
## \#43 Posted by: mrpj Posted at: 2016-10-02T20:32:33.827Z Reads: 160

```
Please share a bit more about your experience and your design

[quote="brun, post:42, topic:10161"]
Does anyone know the protocol that the nunchuck uses to communicate with the vesc?
[/quote]

There are different implementations - but for the one that is provided by benjamin vedder check his forums http://vedder.se/forums/index.php and the nunchuck app for the vesc

additionally check [this github repository](https://github.com/RollingGecko/VescUartControl) - it provides an uart -> vesc interface for "nunchuck commands"
```

---
## \#44 Posted by: brun Posted at: 2016-10-02T21:59:04.076Z Reads: 158

```
Great...I'll start digging there.  

I've been posting our whole project to hackaday...lots of stuff on both the board and remote hardware, electronics and software.  Some stuff on how we handled NRF2401 challenges.
Project log is here:
https://hackaday.io/project/12123-electric-longboard
```

---
## \#45 Posted by: B4Me Posted at: 2016-10-06T09:21:59.608Z Reads: 159

```
So sorry for the long away time..
(A lot of shit hit the fan lately :-/ )
I will try to design a pcb for you, with the envelope you can design within.
As to mounting screws I havnt really planned this out yet.. But I will soon, else if yoo decide on some holes, I can also incorporate these into the design.
For the case, would you mostly like screws or you glueing it together ?

It some time since I played with these modules, and ofc we should not remove the antenna, but I hope we will get good range still, but we just need to test it out, move stuff around in the case until there is a good signal :slight_smile:

 Do the modules actually just do the channel hopping in hardware or maybe not at all ?
Still it is a good thing that we are away from most noise sources not using 2.4Ghz

Its always a good idea to steal parts of code when needed, no reason to reinvent something simular
```

---
## \#46 Posted by: brun Posted at: 2016-10-09T20:27:11.271Z Reads: 151

```
Looking at the VESC UART interface and other VESC GIt Hub references....these seem to be mainly concerned with how to communicate diagnostics or set/get values for things like the BLDC tool.  

I found a good [Wii-Nunchuck I2C protocol.](http://www.robotshop.com/media/files/PDF/inex-zx-nunchuck-datasheet.pdf)   It seems pretty easy to implement.  It's a simple I2C slave with 2 commands and a 6 byte payload and a bit of CRC. 

Still I think the next thing to try is moving the receiver very far from the VESC, maybe supply an independent 3.3V to it.  I'll be outlining my attempts at doing this and some other things on my [Hackaday log.](https://hackaday.io/project/12123-electric-longboard/log/47339-wii-mote-cut-outwork-in-progress)
```

---
## \#47 Posted by: WrinklyWink Posted at: 2016-10-14T08:51:48.519Z Reads: 144

```
nice theory creation and testing! This sort of thing with the nunchuck receiver has been on my mind a lot lately because I want to implement a topside location for the receiver, This means the receiver will have to be given a longer wire. Obviously wondering of ways to shield from interference. But if its a 3.3 volt problem then theres an easy fix.. Looking forward to option 3 test.
```

---
## \#48 Posted by: julian46 Posted at: 2016-12-02T14:24:21.769Z Reads: 128

```
what do you guys think of the nRF24L01 compared to bluetooth in regards to handing interference? - had some issues with my early November Evolve Bamboo GT - just wondering if a different radio may work better. (its intermittent - some times ok - other times not - trying to determine if its a hw defect with my remote/board controller or if the nature of the beast with this radio) - I don' think the nRF24L01 has frequency hopping or similar built in - whereas pretty sure all versions of bluetooth do (they are using similar frequencies) - thanks
```

---
## \#49 Posted by: tueboard Posted at: 2016-12-02T16:26:00.159Z Reads: 121

```
@B4Me i would pay for a controller like yours with some buttons more:
- speed acceleration (noob, pro)
- cruise control
```

---
## \#50 Posted by: B4Me Posted at: 2016-12-13T07:52:23.272Z Reads: 116

```
Hi julian, its the same issue.. you need to move away from 2.4Ghz if you want less interference.. 2.4ghz is so populated with everything :-/
```

---
## \#51 Posted by: WawiKirsinger Posted at: 2017-08-20T23:24:48.203Z Reads: 73

```
Hi! i`m new here im i just looking for some really good looking remote... so how is you Project going? if i can add somthing i think it need to be more "heavy" adding weight it would createe the "expensive remote" LOL and the ring wherer to put the finger would be great!
```

---
## \#52 Posted by: Deckoz Posted at: 2017-08-23T04:42:49.385Z Reads: 59

```
lol at everybody arguing you need two receiver modules...its called a diversity receiver... diversity receivers are typically two transceivers that can both trans and receive, one is used for signal, one used for telemetry with packet health. both antennas can receive during packet degredation... 

if your looking for multichannel capability, small receivers/transceivers. look into FrSky SBUS ie OpenTX. Its open source, supports upto 16 channels, and you can use SmartPort telemetry if you desire(ie send VESC data back for an OLED screen)


realizing now this was a dead bumped thread^ lol
```

---
## \#53 Posted by: B4Me Posted at: 2017-08-23T06:48:51.571Z Reads: 57

```
dead, maybe, but the info is still valuable for me and the others following :slight_smile:
My time is the issue, else this remote would long be in the marked
```

---
