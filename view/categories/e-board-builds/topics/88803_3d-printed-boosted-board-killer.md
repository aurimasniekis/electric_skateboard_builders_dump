# 3D Printed Boosted Board Killer

### Replies: 178 Views: 15481

## \#1 Posted by: Pryside Posted at: 2019-03-30T19:00:57.452Z Reads: 960

```
[YOUTUBE LINK](https://youtu.be/C8n8ceZM9qY)

I love the Boosted Boards but wanted something more, so I created and designed this amazing 5000W almost completely 3D Printed electric Longboard. Check out my Video about it if you want to learn more!
This Thing combines everything I ever wanted from a good electric Longboard:

* Amazing Remote
* Flexy Deck for smooth ride
* High Power
* Fast Charging
* Smart BMS
* Nice Remote with percise and smooth control and great features
* Somewhat Waterproof
* Reliable

![DSC00644|690x460](upload://pMMyxMpyJ8JRoibdGRY0jOzCOKL.jpeg) ![DSC00645|690x460](upload://aC7ArNs7RDlpJyAzXLxJDBLT9nw.jpeg) ![DSC00646|690x460](upload://yPjFpO1mB7XyILOW12eYcKKLEEM.jpeg) ![DSC00648|690x460](upload://fczIXzpOzjLoUSTO8orM0FXC7Vo.jpeg) ![DSC00649|333x500](upload://dylkYaNY43UWbVqYeBefxgnNknY.jpeg) 

[THINGIVERSE FILES AND CAD](https://www.thingiverse.com/thing:3528728)

[PRE-CHARGE ANTI-SPARK SCHEMATIC](https://drive.google.com/open?id=1kMG3GBcZCPoe54R4nuCTkw7K1juGhK98)

[FIREFLY REMOTE MODDED FIRMWARE GitHub](https://github.com/Pryside/FireFly-Esk8-NRF24)

Specs:
* 5000W Power
* Peak 12Nm per Wheel (Dual Drive)
* 36Km Range
* 388Wh Battery
* 9,5Kg weight
* 40Km of Range per Hour charging
* Board Loaded Vanguard Flex 3 (same as Boosted Board V2 Deck)

Battery:
* 3D Printed BatteryCase that can be easily removed and swapped
* Hidden flat copper cables for clean look
* 12S3P 18650 Samsung 30Q Battery
Maximum Discharge per Cell: 35A peak
* SMART Bluetooth BMS [I made a Video about it](https://www.youtube.com/watch?v=QQW3uuzNnkg)
Smart BMS sounds awesome and it is!
* Pre charge Anti Spark that doesnt destroy itself, every other Anti Spark died on me
You need to precharge the capacitors of the vesc to have a reliable system (link to schematic is above)
* XT60 for charging
* 10mm hole for on off switch

VESC Case:
* 3D Printed Vesc Case
* 2x esk8.de hellray VESCs 4.12 with direct Fets on FW 3.4
* Added a 600W TVS Diode. Almost NO VESC except the Focbox and a few others have a TVS Diode!
* YOUR VESC WILL DIE ON 12S WITHOUT ONE! It saves your vesc against high Voltage trancients
(I have a pile of dead vescs and repaired a few, trust me!)
How to Install one on your vesc and more details in my video!
I used the P6KE56CA
* Arduino Nano with NRF24L01 controlling the VESC over UART

Drivetrain:
* 3D Printed Motor Guards for front and back, makes them practically waterproof
* 3D Printed Wheel Pulleys (currently 38T)
* 2x TorqueBoard 6355 190Kv Motors (run them on 70A because airflow is restricted by the splash guards)
!!dont recommend the Motors, magnets need to be glued, more info in my video!!
* 12mm Belts
* MBS All Terrain 100mm Wheels
* 15T gears on my Motor

Remote:
* FireFly Remote
* Modded the Firmware heavily, many Features added, full list on my GitHub (linked above)
Things like Battery Bar, Action Based information, Km and Energy tracker, full UART Support etc etc.
Currently made it for Vesc FW 3.4
Works great!

Current Km state of this Board 780Km, still works great!!
Hope you like it :)
```

---
## \#2 Posted by: pduck911 Posted at: 2019-03-30T19:12:47.811Z Reads: 738

```
Impressive, very nice work!
```

---
## \#3 Posted by: Indiangummy Posted at: 2019-03-30T20:07:50.602Z Reads: 729

```
This is a clickbait title if I've ever seen one. 😂
```

---
## \#4 Posted by: Pryside Posted at: 2019-03-30T20:25:13.726Z Reads: 695

```
hell yeah, but as long as there is actually something good behind the bait I think its okay :smiley:
```

---
## \#5 Posted by: BruSkater Posted at: 2019-03-30T20:27:57.304Z Reads: 671

```
Nice build! Would the firefly firmware work with the unity?
```

---
## \#6 Posted by: chickengun Posted at: 2019-03-30T20:46:59.125Z Reads: 613

```
Nice work :+1:
```

---
## \#7 Posted by: Pryside Posted at: 2019-03-30T21:10:56.797Z Reads: 568

```
should propably. Try it out and see if the library reads data from the vesc. I made this for Vesc firmware 3.4 so anything from 3.xx should work
```

---
## \#8 Posted by: BruSkater Posted at: 2019-03-30T21:20:54.946Z Reads: 540

```
I am not very familiar Uploading the FW to the remote, do you know any guide I can follow or point me briefly in the right direction?
```

---
## \#9 Posted by: Pryside Posted at: 2019-03-30T21:33:39.220Z Reads: 523

```
Hm, where did you even get your Firefly from? Did you buy it preassembled or why dont you know how to flash it...
I wount really recommend messing around with that If you dont know how to reprogram it, since you can mess things up and then nothing will be working. On mine I layed the Uart to the micro USB port for charging but I guess on yours you have to open it up and plug into the arduino on the inside. But you definitly should understand the basics of arduinos in the first place for that, just watch arduino tutorials on yt to get how the software works
```

---
## \#10 Posted by: LukePL Posted at: 2019-03-30T21:39:07.466Z Reads: 494

```
Super impressive @Pryside! I'm just curious can someone confirm your swich design and Vesc mod. It sounds to good to be true.
```

---
## \#11 Posted by: Vanarian Posted at: 2019-03-30T21:45:22.655Z Reads: 495

```
[quote="Pryside, post:1, topic:88803"]
Pre charge Anti Spark that doesnt destroy itself
[/quote]

[quote="Pryside, post:1, topic:88803"]
Added a 600W TVS Diode.
[/quote]

Got any pictures about these ? Thanks for sharing the schematic of the pre charge AS :beers:
```

---
## \#12 Posted by: rusins Posted at: 2019-03-30T21:59:47.267Z Reads: 458

```
If I understood correctly from the video, your diode will cause a short circuit if the voltage goes above 58V or so... couldn't that harm the battery or BMS? (I forgot if yours was discharge passthrough or not.)
```

---
## \#13 Posted by: NoobSk8t Posted at: 2019-03-31T10:39:09.916Z Reads: 434

```
could you link the BMS I couldn't find it anywhere
```

---
## \#14 Posted by: chickengun Posted at: 2019-03-31T14:42:28.062Z Reads: 415

```
@pryside can you please draw the schematic of your firefly receiver? Now that you use UART for reading and writing data you only need two pins RX,TX as well as CE and CSN? You don't need the 5V,PPM,GND wires from VESC?
```

---
## \#15 Posted by: Pryside Posted at: 2019-03-31T18:06:53.216Z Reads: 409

```
I have a video about it, where I also talk about how to find it https://www.youtube.com/watch?v=QQW3uuzNnkg

Literally google "Smart BMS 12S" for example. Aliexpress, BMSbattery.com Lithiumbatterypcb.com so many sites offer this... :slight_smile:
```

---
## \#16 Posted by: Pryside Posted at: 2019-03-31T18:11:13.037Z Reads: 411

```
Short circuit in the sense that It destroys the excess voltage trancients. It eats up the spikes created by your motors and vesc. A vesc makes switching mistakes all the time and creats constantly voltage and current spikes that vary in their peaks. So no current gets drawn from the Battery when a TVS Diode kills voltage spikes, thats why I said to mount them directly on the PCB of the Vesc, otherwise it wont work because of the inductance of the battery wires, the trancient of the vesc usually wont even reach the battery.
```

---
## \#17 Posted by: Pryside Posted at: 2019-03-31T18:18:54.548Z Reads: 409

```
Currently time a little rare, yes I can draw it out and all, but it's usually the same as every nrf24l01 arduino nano uart config. Just need to watch out to use the right CE CSN pins on the nano. These are defined in my Arduino code at the top.
Just use a normal NRF24L01 - Arduino Nano wiring diagramm and watch out that the CE and CSN pins match the ones I used in my code (or change them in the code later on) 
And use a normal Arduino Nano - Vesc Uart wiring.
Uart is only TX, RX, GND and 5V. Nothing more needed.
In the Vesc Tool its then Uart at 115200 as control and not PWM anymore.
Also as mentioned in my Git Vesc Firmware 3.4 is currently required for my Software
```

---
## \#18 Posted by: SeanHacker Posted at: 2019-03-31T19:01:18.143Z Reads: 403

```
Please make and send me an antispark that actually works @Pryside . I will love you so hard for the rest of your adult life.
```

---
## \#19 Posted by: NoobSk8t Posted at: 2019-03-31T19:33:25.384Z Reads: 403

```
I'm a new subscriber of yours and from Germany too. Do you know anything about what the laws are like in Germany rn?
```

---
## \#21 Posted by: Pryside Posted at: 2019-03-31T22:30:27.930Z Reads: 396

```
I'm writing my exams very soon so I'll see how much time I have. Can sell you one for 30€+shipping. I'll contact you when I get it done. Give me your contacts in the DMs and I can send you one.
```

---
## \#22 Posted by: Pryside Posted at: 2019-03-31T22:31:33.201Z Reads: 365

```
Currently its completely illegal and will be propably even after the new laws for small electric vehicles will pass. Maybe some types will be allowed but propably never any board you actually want to ride. My tip (have been caught by the police before and they have let me go): Dont use any main roads. Stay away from them as good as possible and only use side roads, bike paths etc. basically anywhere where police cars dont drive. Stay aware of your surrounding and drive carefully. And watch out that no police is seeing you, if they do just push they are usually not interested in making a scene.
```

---
## \#23 Posted by: Pryside Posted at: 2019-03-31T22:34:06.868Z Reads: 357

```
Not really any detailed pictures right now. In my video there are a few scenes where you can see the anti-spark. And the tvs diode is just a normal diode.
```

---
## \#24 Posted by: SeanHacker Posted at: 2019-03-31T22:34:21.772Z Reads: 353

```
[quote="Pryside, post:21, topic:88803, full:true"]
I’m writing my exams very soon so I’ll see how much time I have. Can sell you one for 30€+shipping. I’ll contact you when I get it done. Give me your contacts in the DMs and I can send you one.
[/quote]

I love you. DM incoming...
```

---
## \#25 Posted by: Pryside Posted at: 2019-03-31T22:40:19.276Z Reads: 366

```
I can confirm you the switch design at least, I've used it in many way more high power applications with a 300A Kelly for example. And have let many EE review my design (I'm only EE first sem) and yeah as long as the R3 resistor which charges the Caps is beefy enough (thats why it says "use a wire resistor" in the schem) it works perfectly

And the TVS diode is the same thing, I noticed the missing TVS on the Vesc one day, talked to a few EE about it and they all said the same thing that this is very unsafe this way. Unscrewed a Focbox and saw that they added one and that confirmed the fact for me that you need one.
I destroyed 5 vescs in 1000Km (DRV8302 Errors, blown mosfets and caps) and after this mod my vesc never had any issues again.
```

---
## \#26 Posted by: SeanHacker Posted at: 2019-03-31T22:45:03.535Z Reads: 365

```
[quote="Pryside, post:25, topic:88803"]
Unscrewed a Focbox and saw that they added one and that confirmed the fact for me that you need one.
[/quote]

Yep...
![IMG_20190327_151436|659x500](upload://nt8IkMOntC9pSONZzQxa2Qmo3i1.jpeg)
```

---
## \#27 Posted by: LukePL Posted at: 2019-04-01T05:08:49.630Z Reads: 342

```
Great! Thank you for shareing your finds and design! 👍
```

---
## \#28 Posted by: City-Blade-101 Posted at: 2019-04-01T13:02:36.319Z Reads: 328

```
Nice one, Leo! 
Level up!
Fahr vorsichtig und kauf Dir bitte ein paar skateschuhe:wink:
Ist nicht böse gemeint, aber Eishockey spielt man auch nicht mit Eiskunstlauf Schuhen:wink:
EDIT: dear pilgrim,I totally love your way of building and learning from your first DIY board on.
This board you build is a rocket. A really nice weapon.I love it and you finally learned to apply grip tape the right way in the end (hahaha, just kidding).
Cant wait for future Skateboards or maybe high speed onewheel projects.
Enjoy riding this beast !
peace
```

---
## \#29 Posted by: City-Blade-101 Posted at: 2019-04-01T13:10:00.102Z Reads: 318

```
best ideas at the moment came from FDP, because they want to install 3 categories.
1. for kids under the age of 14 years with a speed limit up to 12kmh - free without any insurance and helmet.
2. for commuters at the age of 14 and above with a speed limit of 25 kmh - free without any insurance and helmet
3. for freaks(Sports) at the age of 18 i think and with a speed limit of 45 kmh - insurance and helmet is needed.

This law would be perfect for us and I think the electric skate community in germany would totally love if it would come through like this.But it sounds like a dream.
All best wishes.
peace
```

---
## \#30 Posted by: Bor.inc Posted at: 2019-04-03T06:17:29.865Z Reads: 306

```
I just saw your video and you did an amazin job I must say, you even made a better antispark and fixed the vesc problem with such a simple solution.

You can probably try to make a custom pcb for your antispark and sell it because you have made a more reliable antispark switch and I think everyone is tired of blowing theirs up haha
```

---
## \#31 Posted by: City-Blade-101 Posted at: 2019-04-03T14:14:51.033Z Reads: 295

```
Yeah, and if it works like @Pryside says, blowing VESCs or Flyskies at 12S setups should be no more. Sounds pretty.:smiling_face_with_three_hearts:
```

---
## \#32 Posted by: Bor.inc Posted at: 2019-04-03T14:21:42.078Z Reads: 296

```
Yes looks promesing!

For the antispark he can maybe also put the diode that will stop vescs being killed because if im right it just has to be on the power wires of the vescs
```

---
## \#33 Posted by: City-Blade-101 Posted at: 2019-04-03T14:23:47.114Z Reads: 294

```
Thats what he mentioned in his video i think. Im not familiar with the electronics so far like being a specialist, but I count on this boy!
```

---
## \#34 Posted by: Pedrodemio Posted at: 2019-04-03T14:39:47.209Z Reads: 307

```
Really nice board, and way better range than the original

Wish I can find someone with a Boosted or any other Vanguard board one day to try it 

I’m sorry but I have to post this 😁

![image|213x150](upload://mzCV6CbkZRxufjygMsGnTTnYixo.jpeg)
```

---
## \#35 Posted by: Pryside Posted at: 2019-04-04T15:21:37.233Z Reads: 290

```
I cant guarante that the TVS Diode makes the Vesc indestructable since its still pretty stupid to run 60V rated components on 51V with inductive loads. But a Vesc has never lasted me this long before on 12S. :slight_smile:
```

---
## \#36 Posted by: Pryside Posted at: 2019-04-04T15:24:23.498Z Reads: 287

```
Antisparks die from a completely different reason. The Mosfets Latch Up from the high current when connecting to the Caps of the Vesc. I even explained that in my Video. A TVS Diode, just prevents voltage surges, these are two completely different things.
```

---
## \#37 Posted by: Bor.inc Posted at: 2019-04-04T18:12:18.518Z Reads: 284

```
ah yes I get that, the modification on your antispark is to prevent the short circuit in the beginning. But what I mean is that if you plan on selling the antisparks you can maybe try to also add the diode on that same antispark so you also save the vescs :slight_smile: you know what i mean? 

And it is so awesome that you have probably fixed two common big problems just with such easy solutions, mad props
```

---
## \#38 Posted by: Bor.inc Posted at: 2019-04-04T19:03:24.375Z Reads: 291

```
Btw im not realy that much into electronics and im trying to find such diodes for my vesc but:

is a diode like the <small> **P6KE-51A** </small> also suitable for this application? I assume that it only can handle 5amps less than the p6ke-56a that you use but Im interested in your opinion!

I have also two others that maybe work?
 **P6KE-200CA**  (is bidirectional and what is tranzorb?) and **P6KE-47CA** (the same?) all state that it can handle max 600watt (just like your p6ke-56a) is this a problem?
```

---
## \#39 Posted by: FelixS_1 Posted at: 2019-04-05T14:16:00.928Z Reads: 286

```
hello leo can you tell me your motor mount that you use?
```

---
## \#40 Posted by: janpom Posted at: 2019-04-05T20:50:24.115Z Reads: 285

```
[quote="Pryside, post:1, topic:88803"]
40Km of Range per Hour
[/quote]

:face_with_monocle:
```

---
## \#41 Posted by: janpom Posted at: 2019-04-05T21:11:57.613Z Reads: 278

```
Nice build and nice video. Pretty impressive, especially for such a young fella.

Quick tip. If you stop saying things like "this GREAT XYZ that I designed" people will like your vids a lot better.
```

---
## \#42 Posted by: Lobbie Posted at: 2019-04-06T23:25:49.370Z Reads: 257

```
nice vid!!
```

---
## \#43 Posted by: relations99 Posted at: 2019-04-07T08:12:52.238Z Reads: 259

```
Hey just wondering, did you typo your receiver code?

    int counter_checksum=0;
    counter_checksum = ControlValues.ValY;
    if(ControlValues.upperButton == true) counter_checksum++;   <<<<
    if(ControlValues.upperButton == true) counter_checksum++;   <<<<
    if(ControlValues.checksum == counter_checksum)
    {
      recievedData = true;
    }
    
did you mean to check upper and lower button instead?
```

---
## \#44 Posted by: RedWeedGFX Posted at: 2019-04-07T12:31:21.100Z Reads: 260

```
Hello i would really like to make my own i just dont have the tools skills or time to do it would it be possible for me to buy one like this of of you i would really like to come in contact with u.you’re work is awesome and i really support you Best wishes: Addi
```

---
## \#45 Posted by: RedWeedGFX Posted at: 2019-04-07T12:37:15.233Z Reads: 251

```
How much it costed you to make
```

---
## \#46 Posted by: Friskies Posted at: 2019-04-07T14:30:30.824Z Reads: 250

```
It is impossible for your board to be 5000w with a 12s3p 30q pack unless you are planning on destroying cells running a 3P 30q pack at 100A + discharge...
```

---
## \#47 Posted by: danielz Posted at: 2019-04-07T14:46:38.439Z Reads: 250

```
Im not the only one thinking this then, they must be running very hot. :rofl:
```

---
## \#48 Posted by: superjoys Posted at: 2019-04-07T20:55:39.582Z Reads: 253

```
is it possible to get a full partslist?
```

---
## \#49 Posted by: Winkelmann Posted at: 2019-04-08T17:59:49.414Z Reads: 249

```
Awesome build Pryside! i've got a lot of inspiration from your build and would love if you and everyone that reads this would give me some feedback!

https://www.electric-skateboard.builders/t/project-board-better-than-boosted/89825?u=winkelmann
```

---
## \#50 Posted by: Mitkah Posted at: 2019-04-09T07:49:07.482Z Reads: 239

```
Hey @Pryside, 
I have an ESV based on 4.12 in the standard design, where should i solder the tvs? Parallel on the back on plus and minus? 

[Picture from the back](http://vedder.se/wp-content/uploads/2015/01/pcb_back.jpg)
```

---
## \#51 Posted by: Mitkah Posted at: 2019-04-09T07:56:31.816Z Reads: 237

```
the motor mounts are from torqueboards

[https:///collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-set-only-black](https:///collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-set-only-black)
```

---
## \#52 Posted by: Mitkah Posted at: 2019-04-10T06:15:44.803Z Reads: 226

```
have a look at the other videos from him, there is a good descritpion
```

---
## \#53 Posted by: Pryside Posted at: 2019-04-10T10:44:42.398Z Reads: 224

```
sorry, forgot the "charging". Its the charging rate in Km. Because I have a quickcharger with 400W that charges the board in an hour. The charging rate is 40Km of range per hour
```

---
## \#54 Posted by: Pryside Posted at: 2019-04-10T10:47:12.538Z Reads: 217

```
jupp indeed, that is a typo. I will fix it. the upper and lower buttons dont get used anyway thats why I propably didnt notice it while testing. Thanks for the comment!
```

---
## \#55 Posted by: Pryside Posted at: 2019-04-10T10:49:17.098Z Reads: 219

```
A TVS on the Antispark wont work. The voltage trancients get created directly on the vesc and should be eliminated before even reaching the battery. Thats why I said in the video the tvs diode should be mounted directly onto the vesc pcb where the battery wires go in otherwise the tvs will have no effect
```

---
## \#56 Posted by: Pryside Posted at: 2019-04-10T11:01:29.663Z Reads: 219

```
Yeah propably that sounded a little full of myself, it wasnt inteded that way. I called a lot of stuff like the Firefly Remote from Solidgeek and a ton of other components awesome and great too. I think I called my own stuff one single time in the video great and I dont think its a bad thing to be proud of your own creation that I spend so much time for and to express that, its a very normal thing that people do. Be proud of your work.
```

---
## \#57 Posted by: Pryside Posted at: 2019-04-10T11:04:23.172Z Reads: 211

```
Not that easy. I could build one but that would cost 1300€ in parts with charger and all. And labor is around 80h to fully build one again so around 2500€ would be the cost of one.
```

---
## \#58 Posted by: Pryside Posted at: 2019-04-10T11:15:56.527Z Reads: 221

```
No its not healthy but also doesnt destroy them. The 30q cells can widthstand a 35A burst quite easily. They are capable of 22A constant discharge and in their lifecycle tests they run them with 22A constant. Many "30A" or "40A" cells out there have a similar internal resistance so other than faster degradation this doesnt really affect them negatively.
Its also a power that I almost never use only when accelerating on a hill. I usually stay below 1.5kW when riding and peak above 3kW for maybe half a second.
I also only charge to 4Volt/85% and discharge never below 3,4V/15%
And after around 40 cycles I still have full range and no cell is ever out of balance.
```

---
## \#59 Posted by: Pryside Posted at: 2019-04-10T11:18:47.204Z Reads: 209

```
jupp, right there where the cables meet the pcb. the body of the tvs can be right above the current shunt
also if you have some space, try maybe soldering a good low esr 62V cap directly on the board, also helps a lot.
```

---
## \#60 Posted by: Pryside Posted at: 2019-04-10T11:46:01.238Z Reads: 222

```
the P6KE-51A will maybe work with 11S and below but not 12S. It has a breakdown voltage starting at 48,5V this is no bueno when you have a battery voltage of 50,4V fully charged.
 
the p6ke-200CA has a breakdown at 200V and wont help anything with your 60V+ voltage spikes.

47CA has a breakdown at 47V also not usefull with 12S

really use the 56CA or 56A as I recommended in the video they are the only ones with a breakdown closest to your 50,4V
```

---
## \#61 Posted by: City-Blade-101 Posted at: 2019-04-10T12:04:09.876Z Reads: 214

```
You can be proud, Leo. At first I thought the same way like @janpom about you, but If you create or invent things you have to mention that it was your idea and your try.
Everyone does it and if not someone will steal your ideas and make them their own.
In this forum are so many very impressive builders who exchange themselfes  with others for building better boards and to eliminate possible mistakes for being save in the workspace and finally in the streets...
Im no specialist in electronics, but i learned a lot in here and i can tell you the only mistake you made is just to solder your batteries instead of spot weld them(i think i saw that in your videos). I know from the batterie freaks in here that soldering will damage your cells and the construction is not very reliable. Please look @pjotr47 ! He is a real Battery god and a specialist all the way for maximum power.
peace
```

---
## \#62 Posted by: Andy87 Posted at: 2019-04-10T12:07:57.636Z Reads: 203

```
[quote="Pryside, post:53, topic:88803"]
The charging rate is 40Km of range per hour
[/quote]

maybe i´m dumb, but would that mean if it´s windy outside the charger would charge more slowly because the range would be less? :thinking:
```

---
## \#63 Posted by: pjotr47 Posted at: 2019-04-10T12:21:37.700Z Reads: 189

```
Lol you make my laughing @Andy87
```

---
## \#64 Posted by: City-Blade-101 Posted at: 2019-04-10T12:21:48.892Z Reads: 190

```
lmao 10 char
```

---
## \#65 Posted by: Mitkah Posted at: 2019-04-10T12:44:00.091Z Reads: 192

```
in one hour, you can charge the battery enough for 40km driving
```

---
## \#66 Posted by: Andy87 Posted at: 2019-04-10T12:50:52.254Z Reads: 199

```
How your charger can calculate that? Your range depends on so much things. So if you have a ride after thanksgiving and it’s a windy day and you decide to go up the steepest hills in your village, than the range of your pack is maybe only 35km...would that mean next time I charge up my pack I would overcharge it because the charger charge 40km instead of 35km? ... 💁‍♂️
```

---
## \#68 Posted by: Mitkah Posted at: 2019-04-10T13:00:58.582Z Reads: 192

```
ist a unit for e-vehicles
```

---
## \#69 Posted by: Andy87 Posted at: 2019-04-10T13:01:59.931Z Reads: 197

```
and yes I fully understood what the OP mean with it. I just think it´s not necessary to click bait every feature, especially if it´s than not right anymore. 

He did a good job with the board and all the things he created by his own. No need to advertise it like  chinese clone board companies do it with there products.

He can just fully charge his battery in 1h that´s it.
```

---
## \#70 Posted by: Andy87 Posted at: 2019-04-10T13:03:37.078Z Reads: 202

```
I think you didn´t got it. maybe my last comment helps to understand that.
your charger charge up to a capacity but not to a range. how much range you get out of that capacity depends on different things and is never the same. 

Soooo, to say in one hour his charger is charging 40km range is just not correct.
```

---
## \#71 Posted by: pjotr47 Posted at: 2019-04-10T13:21:17.642Z Reads: 202

```
Fully correct @Andy87 

He can give better the amps off his charger. I think it is a 8A charger. 

There are some ”click baits” in this topic. He is talking about 5000watt off power. A Samsung 30q is rated for 15A. There are some guys who are rocking 20A from them. If I calculate with a fully charge: 4,2v * 12s *3p *20A, i have 3000watt. So I don’t know where those 5000watt comes from
```

---
## \#72 Posted by: rey8801 Posted at: 2019-04-10T16:52:29.960Z Reads: 192

```
Of yuu see the video it said 5000w comes from the battery being used at 35A since 20A is constant meaning that he can discharge way more for short period. So I guess he set 35A battery max. From there the 5000w
```

---
## \#73 Posted by: Pedrodemio Posted at: 2019-04-10T17:36:13.313Z Reads: 189

```
Don't forget the sag, the 30Q at 35A would sag 0,7V per cell

So (4,2-0,7)*12s*3p*35A = 4400 W

Or a 20A

(4,2-0,4)*12s*3p*20A = 2700 W
```

---
## \#74 Posted by: Pryside Posted at: 2019-04-11T09:59:26.323Z Reads: 189

```
The reason I said that is not to sound like a chinese company, but because people ask so often how fast my board charges and it is a very important factor that people should use when talking about charging rate. If I said my board can be charged in an hour, you could compare that to a Boosted board that also gets charged in an hour. But that would be way off, because I can charge at 450W and Boosted charges at less than 80W. So saying "it takes an hour to charge" is a bad comparison. And with saying how many watts my charges has also doesnt get the idea across of how fast you can charge.
Way better way is to calculate the range using the usual 11Wh/Km that you get when crusing at 30Kmh on a smooth road.

Now Tesla has been using "Km of range per hour charging" for a very long time, so why not use that. This actually tells you "My board has 40Km/h charge rate, so if I wait 30 Minutes I can ride 20 Kilometers again."
```

---
## \#75 Posted by: Pryside Posted at: 2019-04-11T10:03:17.063Z Reads: 173

```
you can easily pull 35A per cell from a 30Q without any problems for a very quick burst. U wont need the 5kW boost for more than a second anyway
```

---
## \#76 Posted by: Pryside Posted at: 2019-04-11T10:04:12.574Z Reads: 196

```
Here is a full calculation of how much power you can actually get using my setup:

Fully charged Battery at 50,4V. IR per cell is 20mOhm (DC iR from Datasheet), 3 in paralell is 6,3mOhm, 12 in series is 75mOhm
Lets calculate the theoretical maximum. I currently have a 75A Current Limit, but lets assume I set this to 90A say I go full throttle:
My Vescs pull 180A
180A * 0,075Ohm = 13,5V voltage drop inside my Battery
50,4V-13,5V= 36,9V Voltage going to my VESC (still above 3V per cell)
36,9V * 180A = 6642W so thats the amount of Power getting eaten from my vesc.
Thats where usually everybody stops and says that this is the power, but since there are a ton of losses at this current here is the real mechanical power that you would be measuring on a dyno:
Resistance of my vescs: 0,0011Ohm Resistance of Motors: 0,0225Ohm
(0,0011Ohm+0,0225Ohm)*180A²= 764,64W of Power loss in Motors and ESC
6642W-764,64W= 5877W MECHANICAL POWER
so yes, the 5kW is easily possible.﻿
```

---
## \#77 Posted by: Pryside Posted at: 2019-04-11T10:06:50.623Z Reads: 178

```
Yeah range depends on a lot of things but just like on electric cars we use a typical consumption that is 11Wh/Km. Almost every single eBoard company uses this consumption.
```

---
## \#78 Posted by: Andy87 Posted at: 2019-04-11T10:08:57.229Z Reads: 178

```
[quote="Pryside, post:76, topic:88803"]
I set this to 90A say I go full throttle: My Vescs pull 180A
[/quote]

You want to say you run the esk8.de with 90A batt max? Just to get that right for me.
```

---
## \#79 Posted by: Andy87 Posted at: 2019-04-11T10:15:13.392Z Reads: 182

```
[quote="Pryside, post:77, topic:88803"]
typical consumption that is 11Wh/Km. Almost every single eBoard company
[/quote]

Which means your board is the same as any e board which use that 11Wh/km. Not faster not better. Maybe I get something wrong but with the same average power consumption you get the same average result out of different boards. 

With it i assume you don’t use super secret new motor technology or a gear drive which reduced all losses or wheels and bearings that spin for ever.
```

---
## \#80 Posted by: pjotr47 Posted at: 2019-04-11T10:36:36.910Z Reads: 199

```
Yeah I know but that is in burst that is not real power you always have. 

In my free time I also work as a DJ. With the speakers you also have peak and rms capability. the Chinese companies advertise their speakers with the peak power and the good quality speakers companies always talk about rms power. you can also bring this back to the esk8 world. Many Chinese companies turn out with their peak power, which means that people fall for it.
I challenge you to ask the peak power of your board for 2 minutes and then we talk again.

That 5000watt off power is just a clickbait shit.

And like @Andy87 said not each board is the same, the 10 wh/km rule is a rule of thumb. The real consumption depends much on the rider (weight), rider style (acceleration), weather (much wind). I know guys who do 6wh/km and also guys who do 25wh/km.

[quote="Pryside, post:76, topic:88803"]
I currently have a 75A Current Limit, but lets assume I set this to 90A say I go full throttle: My Vescs pull 180A 180A *
[/quote]

Wait a second, If you tell me that you do 35A form a 30q so 3*35A=105A.

How can your vesc pull 180A :face_with_raised_eyebrow:
```

---
## \#81 Posted by: Pryside Posted at: 2019-04-11T11:49:58.506Z Reads: 178

```
yes this works, have done that before quite a few times on eBikes. The Fets are rated for almost 300A peak. Absolutly no problem with the right thermal paste and not done for too long. Even 100A still works, temperature ist the only problem at this current. Air cooled they thermal throttled after like 10 seconds full throttle.
```

---
## \#82 Posted by: Pryside Posted at: 2019-04-11T11:56:54.226Z Reads: 188

```
"peak power" "2 minutes" you are contradicting yourself

Yeah obviously its clickbait. "Boosted Board Killer" is also a clickbait title. Thats how you get the attention of people.

But 5kW is a true value that can be achived for quite a few seconds.
My VESCs can easily pull 180A together. Its a Dual Drive, I have two Motors, two vescs and they split the current between each other. One pulls 90A the other also 90A.

Next video I can show my BMS Log that shows that I can pull 120A if you want some proof. :)
```

---
## \#83 Posted by: Pryside Posted at: 2019-04-11T12:05:23.232Z Reads: 166

```
not percisely calculated but around 1200€ with Charger an everything.
```

---
## \#84 Posted by: Andy87 Posted at: 2019-04-11T12:08:05.556Z Reads: 186

```
[quote="Pryside, post:82, topic:88803"]
Next video I can show my BMS Log that shows that I can pull 120A if you want some proof
[/quote]

Not digging the proof, just really interested how you get those esc set up with that settings running stable. I have two of them as well. One fucked pretty fast after some over current faults I still can’t explain where they where coming from and after that I run one in single at 40A bat max which took me exactly 2min till the esc shut down because of over temperature. The broken one is on repair at the moment and I really would like to use them on one of my other builds, but if I can’t even run them with 40A bat max it will just not work for me. 

So what you would recommend. Change the heat paste to other one and mount the vescs on a bigger heat sink?
```

---
## \#85 Posted by: Pryside Posted at: 2019-04-11T12:16:05.754Z Reads: 187

```
are you using the esk8 vescs with direct fets? The 1.7mOhm direct fets? Because the hardware I use is basically somwhat of a VESC6 when it comes to the mosfet / capacitors at least.
I also blew one up on an eBike that had almost no thermal paste between the pads and the case. I also set the slow maximum amps to 150A for this experiment with 90 motor amps.
They ran fine for almost a minute on 70A foc_openloop and for around 10 seconds on 90A openloop before throtteling down. But never any errors just cutting down the amps.
```

---
## \#86 Posted by: Pedrodemio Posted at: 2019-04-11T12:32:54.031Z Reads: 196

```
So you set 90A battery in each vesc? You can do what you want, but the data sheet exists for a reason

You are heating each cell at 40W, at that level, even just a peak has the potential to take the core of the cell to a really high temperature, there is not enough conductivity for the heat to flow out

If you manage to do some logs of acceleration from dead stop, maybe in a heavy hill I would love to see if you manage to hit the 180A
```

---
## \#87 Posted by: Andy87 Posted at: 2019-04-11T12:59:42.481Z Reads: 199

```
I have this one 
![image|438x500](upload://o1aRpRPrUTAFaZpI3wBiHIa0oAe.jpeg)
```

---
## \#88 Posted by: Pryside Posted at: 2019-04-14T10:29:24.678Z Reads: 203

```
jupp thats the one I used too. On the mosfets put some good thermalpads like the EYGA series (A is important because they are not conductive) like the EYGA091203A for example on there and add some good thermal paste on top and this thing should easily get 90A as long as the metal is cool
```

---
## \#89 Posted by: City-Blade-101 Posted at: 2019-04-14T16:09:23.277Z Reads: 203

```
Sorry Leo, i ve seen your vid again and saw you finally spot welded your batteries.
It was on your first build you soldered them. 
My fault.
peace
```

---
## \#90 Posted by: noi Posted at: 2019-04-15T13:15:02.728Z Reads: 204

```
Can please someone confirm that I have to solder the TVS Diode there, see picture? Or does it goes on the other side, where the cables from the batterie are?

![IMG_5640|375x500](upload://jO0XkQrGe55xThyH0F4XAuQ2nyM.jpeg)
```

---
## \#91 Posted by: Llama Posted at: 2019-04-21T05:03:12.789Z Reads: 195

```
Hey i saw you would see the pre change anti-spark circuit for €30. I was wondering how i could message you about this.

I would like to start getting everything ready to make something like this during the year.
```

---
## \#92 Posted by: relations99 Posted at: 2019-04-21T06:05:48.833Z Reads: 193

```
Just wondering, the TVS diode is supposed to be reversed biased? Does that mean the voltage spikes / surges are opposite polarity? Or is it in forward biased with respect to the battery polarity?

Edit : does that also mean that if I choose a bidirectional one, it'll constantly drain the battery?
```

---
## \#93 Posted by: Friskies Posted at: 2019-04-21T06:17:09.517Z Reads: 183

```
Just use a loopkey.....
```

---
## \#94 Posted by: matiller Posted at: 2019-04-24T14:15:35.750Z Reads: 188

```
Hello, if I am using 2 ESC, do I need to use 2 recievers?
```

---
## \#95 Posted by: matiller Posted at: 2019-04-24T14:16:36.783Z Reads: 181

```
Could you please take picture from the other side?
```

---
## \#96 Posted by: Mainsedora Posted at: 2019-04-24T14:50:21.990Z Reads: 180

```
no, you can solder the wires coming from the two vescs in parallel to one wire going into your receiver. It will work
```

---
## \#97 Posted by: matiller Posted at: 2019-04-24T14:55:34.868Z Reads: 177

```
Thank you sooo much.
```

---
## \#98 Posted by: matiller Posted at: 2019-04-24T15:04:40.429Z Reads: 182

```
Do you know where to find schematic how to use UART port of flipsky ESC with arduino? It is my first time using Arduino, so I do not really see it in code files. On https://solidgeek.dk/docs/firefly-remote/receiver/schematic/ webside it is connected via 3 pin servo connector (writing to ESC)
```

---
## \#99 Posted by: noi Posted at: 2019-04-24T16:32:49.928Z Reads: 199

```
Thanks for having a look at the pictures. Its the normal 4.12 TB VESC.
![IMG_5683|375x500](upload://suY6o0DisnWQNEcCPpf5hZgWWeH.jpeg) ![IMG_5682|375x500](upload://iOCZ3VcSOsshs2GfQa9j87Mieun.jpeg) ![IMG_5681|375x500](upload://pVp1Z0MQk8VK8OW0TfYoANjIbrX.jpeg)
```

---
## \#100 Posted by: Mainsedora Posted at: 2019-04-24T17:04:51.191Z Reads: 187

```
I personally use the ppm port of my vesc with a rc remote. Are you going to build a firefly remote?
```

---
## \#101 Posted by: Dr.Octogon Posted at: 2019-04-24T17:18:27.879Z Reads: 191

```
If anyone needs this printed. I have a large fully enclosed printer that print this without issue. 

My setup is posted below.

https://www.electric-skateboard.builders/t/3d-printing-resource-whats-new/88585/8
```

---
## \#102 Posted by: matiller Posted at: 2019-04-24T17:55:25.854Z Reads: 185

```
yeah, I already builded the transmiter... I have got a problem with this UART port
```

---
## \#103 Posted by: matiller Posted at: 2019-04-24T17:58:21.567Z Reads: 186

```
Well, it goes there :) Just be careful not to short those two... Are you planning to use firefly Controller?
```

---
## \#104 Posted by: matiller Posted at: 2019-04-24T18:06:58.992Z Reads: 190

```
![Sn%C3%ADmka|369x500](upload://iIIIQ7QMYi7Qp7Apsgz7ZSpKzjV.png) It is way easier to put it in here, as there is nothing to short
```

---
## \#105 Posted by: noi Posted at: 2019-04-24T18:59:35.760Z Reads: 183

```
Awesome, thank you very much. I have a GT2B transmitter, no firefly.
```

---
## \#106 Posted by: Mainsedora Posted at: 2019-04-24T19:31:03.637Z Reads: 181

```
@solidgeek @matiller You could ask himself :smile:, coz I don't really know a solution for that
```

---
## \#107 Posted by: WolffXIII Posted at: 2019-04-27T17:57:38.885Z Reads: 179

```
Thanks @Pryside for this build, been watching your YouTube videos, learning lots! Looking to do my first build this month :slight_smile:
```

---
## \#108 Posted by: matiller Posted at: 2019-05-01T13:26:32.743Z Reads: 176

```
Can I use 57v power supply with that smart bms? (12s)
```

---
## \#109 Posted by: curtis Posted at: 2019-05-03T03:09:33.452Z Reads: 172

```
I watched your You Tube video a few times and you went into detail on alot. I want to know how you might change your board if you are using hub motors   Would you still recomend doing a 12s 2p system? or less power because the motors don't have to turn a gear.
```

---
## \#110 Posted by: Andy87 Posted at: 2019-05-03T05:14:20.499Z Reads: 166

```
@matiller no! [](http://)
```

---
## \#111 Posted by: Andy87 Posted at: 2019-05-03T05:16:34.125Z Reads: 165

```
@curtis his battery is a 12s3p and will work with hubs perfectly fine as well. Don’t go 12s2p.
```

---
## \#112 Posted by: matiller Posted at: 2019-05-03T14:41:26.027Z Reads: 165

```
well... can I use 52? or what is the safe voltage? Does it have to be 50.4 or can it be 51? Thanks
```

---
## \#113 Posted by: Andy87 Posted at: 2019-05-03T14:43:43.640Z Reads: 169

```
Get a charge which fit to your battery 12s battery means 12s Charger. You probably will not have issues if you use a charger with lower voltage besides that it will never charge up 100%, but don’t use a charger with higher output voltage than your pack. A smart bms is not a wonder box. It’s still just a bms.
```

---
## \#114 Posted by: Pryside Posted at: 2019-05-04T00:14:52.776Z Reads: 167

```
The bms might save you from blowing up your battery but the only save way to charge it is to get a "50,2V 12S charger". There are a ton of them on aliexpress
```

---
## \#115 Posted by: matiller Posted at: 2019-05-06T19:08:09.924Z Reads: 159

```
What size nickel stips did you use? As I am reading 10mm by 0.15 is not enough... Thanks
```

---
## \#116 Posted by: Pryside Posted at: 2019-05-06T19:09:54.562Z Reads: 158

```
depending on how many cells paralell you have. If the current only has to go less than 20mm there wont be any problems. Otherwise just weld another sheet on top if you want to cross a bigger distance
```

---
## \#117 Posted by: farnamweb Posted at: 2019-05-11T04:46:18.327Z Reads: 172

```
Hi @Pryside, 

1) Can I use this ESC instead? It's cheaper 
https:///collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller

2) I understand that you don't recommend TorqueBoard motors. What motor do you recommend? 

3) Is the belt 265mm or 280mm ? 

4) I have a drone with a 6S 4in1 ESC, does installing a TVS  diode help protecting the esc? 

5) There is always a spark when plugging in the battery. Drone is powered through the ESC board. Should I also install anti spark?
```

---
## \#118 Posted by: rusins Posted at: 2019-05-11T16:26:48.803Z Reads: 178

```
1. Many on this forum use that ESC, should be fine, but will require the diode trick if you intend to run it at 12s voltage
2. TB motors have been updated recently to make them stronger and more reliable, I don't see why you wouldn't go with them
3. belt length depends on the pulleys and mounts used, someone might know a good calculator for it
4. don't know
5. sparks when plugging in a battery is normal, most people here use loop keys as switches instead of anti-spark ones.
```

---
## \#119 Posted by: Pryside Posted at: 2019-05-11T22:20:18.646Z Reads: 168

```
Just received the first PCBs I made of my precharge Antispark. Will solder them and do some intensive testing next week this should be very nice.
![20|690x389](upload://yqmhO9xWAYn8rjU6xjChZBNqxbd.jpeg)
```

---
## \#120 Posted by: SeanHacker Posted at: 2019-05-11T23:01:39.555Z Reads: 163

```
Nice. Love what I'm seeing here dude!
```

---
## \#121 Posted by: farnamweb Posted at: 2019-05-12T12:04:39.945Z Reads: 160

```
I have a few more questions. Thank you in advance! 

1) Isn't it better to print the battery/VESC case with TPU instead? It's more durable and it can flex when the board flexes.

2) I already have a 1000W 12V server PSU. Should I get a voltage booster like below and rely on BMS to balance charge the battery pack?
https://www.amazon.com/dp/B00E8D7XYG/?coliid=I3MVENO2EUVXXT&amp;colid=2NAX0GX2GD9J1&amp;psc=0&amp;ref_=lv_ov_lig_dp_it

3) Do I need to buy LONGBOARD SHOCKPAD RISERS 3MM ? 
https:///products/longboard-shockpad-risers-3mm?variant=712549924887&gt
```

---
## \#123 Posted by: Pryside Posted at: 2019-05-12T13:39:10.665Z Reads: 157

```
1. No. Solder joints, nickel welded batterys and in general all pcbs dont like flex. You can split up the battery into smaller parts and spread them across the board and have them connected with some silicone wire but you will run into ton of loose connections if you print this thing in tpu and ride it for a while.
2. yes that works. I used a Boost Converter from ebay (300W 80V boost converter) to charge my old board with. But these days I perfer to have a small power brick with 90W (12S Liion charger) from aliexpress with me so I can charge wherever I go and dont have to think if Its worth carrying this brick.
3. You can but they only protect your deck and dont have any ride quality improvements since you will squish them anyway when screwing them in. Ride quality only gets improved by softer and bigger wheels and a softer deck
```

---
## \#124 Posted by: farnamweb Posted at: 2019-05-12T14:14:13.299Z Reads: 163

```
Thank you very much for the help. I also made a list of components for the anti spark board. Do you mind taking a quick look at it @Pryside ? 

*  Power switch >> not sure what to get. please help!
* 4X 1M Ohm Resistors (R1,2,4,5)  >> Metal Film Resistors - Through Hole 1M ohm 1% 0.4W

https://www.mouser.com/ProductDetail/Welwyn-Components-TT-Electronics/MFR3-1M0FC?qs=sGAEpiMZZMtlubZbdhIBIJtQxnYsq7hXit92tIgpI8A%3D

* 1X 15 Ohm Resistor(R6) >> Wirewound Resistors - Through Hole 3W 15 Ohm 5%

https://www.mouser.com/ProductDetail/Yageo/PNP300JR-73-15R?qs=sGAEpiMZZMtlubZbdhIBINt%2Ft6Hry3%2FBZn3Gyw1qhA0%3D

* 1X 1 OHM Resistor ( R3) &gt;&gt; Wasn't able to find a wire resistor. What is the part number that you used?

* 3X 12V Zener Diodes(D1,2,3) >> Zener Diodes 12V 3W

https://www.mouser.com/ProductDetail/ON-Semiconductor/1N5927BRLG?qs=sGAEpiMZZMtQ8nqTKtFS%2FJ7m6e1KBCgub6c2uyKgC%252BY%3D

* 1X 16V 4.7μF Capacitors(C1) >> Aluminum Electrolytic Capacitors - Radial Leaded 16volts 4.7uF

https://www.mouser.com/ProductDetail/Nichicon/USP1C4R7MDD?qs=sGAEpiMZZMsh%252B1woXyUXj7onzYv6nMPCw8k8X5hq4n8%3D

* 2X IRFS7530 Transistors(T1)

https://www.mouser.com/ProductDetail/Infineon-Technologies/IRFS7530TRL7PP?qs=sGAEpiMZZMshyDBzk1%2FWi%252BDdTe3kt8oihq%2FEFTk6nI%252BSM6z%252BASO6Fg%3D%3D

* 1X IRFB3006 Transistor(T2)

https://www.mouser.com/ProductDetail/Infineon-Technologies/IRFB3006GPBF?qs=sGAEpiMZZMshyDBzk1%2FWi5%252BqVgN3%252BWS8frDEDJEFm2A%3D
```

---
## \#125 Posted by: farnamweb Posted at: 2019-05-12T23:13:30.903Z Reads: 162

```
I'm totally building this board. I got more questions for you @Pryside . I wish you would update the post with more details. That would be nice to share the complete part list. 

1) Is 60 AMP enough for BMS? Should I buy one with higher or lower current? 
I found a smaller version that supports 20A and found another with 100A. 
https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/
This question was answered and I went with the 60A BMS:
https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/6937?u=farnamweb

2) Are you using the following motor mount ? Is there a cheaper alternative? 
https:///collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-set-only-black

3) What is the belt length? 265? 


4) I can buy LG HG2 for $3.5/cell. Same capacity and extra 5 AMPs ( 20A) . Should I get HG2 instead?
This was answered here: https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/6950?u=farnamweb

    Will buy 30Q
```

---
## \#126 Posted by: Pavlo_H Posted at: 2019-05-14T00:16:45.005Z Reads: 160

```
Has anyone modified the code so it will work with the "TTGO LORA32 868/915Mhz ESP32" 128x64 screen? I'm trying to build the Firefly nano remote but I would love to have features like an Odometer and cruise control on it.
```

---
## \#127 Posted by: relations99 Posted at: 2019-05-14T00:54:00.476Z Reads: 168

```
I'm using an I2C 128x64 Oled. Not ready to share yet tho. Never tested. ![IMG_20190422_231351|375x500](upload://lKvc4rBTlYQCi2I5h1gnnePdDRF.jpeg)
```

---
## \#128 Posted by: matiller Posted at: 2019-05-15T19:50:28.840Z Reads: 159

```
Can you send gerber files? Thanks (What is that 8 pin for? next to Q3...) I guess 3 pin Mosfet could be used right?
```

---
## \#129 Posted by: Pryside Posted at: 2019-05-17T17:02:31.969Z Reads: 153

```
[quote="farnamweb, post:124, topic:88803"]
Wasn’t able to find a wire resistor. What is the part number that you used?
[/quote]

just use another wirewound resistor like r6, should be fine, with a quite high power rating. Dont really remember wich one I picked and on my PCB there will be some changes and a quite different precharge fet and resistor to save space.
```

---
## \#130 Posted by: Pryside Posted at: 2019-05-17T17:12:56.770Z Reads: 149

```
1. Ignore these stupid current ratings. The 60A BMS can handle pulsed up to 1500A but thats not the reason. You want to buy something that is somewhat in the range of what you will be using. 60A * 3,6V on a 10S is 2.2kW you will never ever use that much power for more than a few seconds so 60A is pretty save. I calculated the losses at 60A and they were around 7W so no problem there.

2. Yes, they are quite terrible and took me like a week to set up correctly. Would propably try the electricboardsolutions.com

3. nope, running on the MBS AT 100mm and 38T there and 15T on the motor so I had to use 280 HTD 5M 12mm wide belts.

4. yeah any cell would work, just take a look at their internal resistance and you can pull a lot more pulsed power than what they are rated.
```

---
## \#131 Posted by: Pryside Posted at: 2019-05-17T17:13:52.640Z Reads: 146

```
Will publish all Antispark stuff very soon :)
```

---
## \#132 Posted by: farnamweb Posted at: 2019-05-17T17:23:20.293Z Reads: 146

```
Thanks man

I got this mount and belt . The mount has an idler which is interesting . The seller calculated the belt length for me. It's 320
https://boardnamics.com/product/motor-mount-for-electric-skateboard-v2-0-w-idler-gear/?attribute_version=Stealth+Edition
https://boardnamics.com/product/two-replacement-timing-belts/?attribute_belt-length=320mm
```

---
## \#133 Posted by: farnamweb Posted at: 2019-05-17T17:29:54.334Z Reads: 149

```
@matiller helped me find the resistor 
https://www.mouser.com/ProductDetail/Ohmite/TUW5J1R0E?qs=sGAEpiMZZMtbXrIkmrvidMPY4i6h3AHP%252BV%252BE2e384xE%3D 

I'm way to excited to finish the board. Do these changes affect the performance of the board or are they just saving space?
```

---
## \#134 Posted by: matiller Posted at: 2019-05-18T10:41:31.323Z Reads: 144

```
What are your VESC settings for breaking?
```

---
## \#135 Posted by: Pryside Posted at: 2019-05-21T14:43:26.807Z Reads: 145

```
putting a tvs so high up there will destroy its purpose, most transcients wont even reach the caps since you have some inductance from the wires. Put it directly on the pcb as in noi's picture
```

---
## \#136 Posted by: Pryside Posted at: 2019-05-21T14:46:19.207Z Reads: 147

```
-75Amps on the Phases and -10A on the battery are my max settings. May seem high but again pulsed this is perfectly acceptable. Safety is more important then getting 2 more cycles out of your battery.
```

---
## \#137 Posted by: TroyMclure Posted at: 2019-05-22T09:53:05.066Z Reads: 148

```
is it possible to buy a anti spark from you? would love to build your board as well :slight_smile:
```

---
## \#138 Posted by: farnamweb Posted at: 2019-05-24T01:24:05.122Z Reads: 152

```
![Capture|417x205](https://www.electric-skateboard.builders/uploads/db1493/original/3X/8/f/8fe2c196e7e7bb2d05b27ae3e119237c2f316b8e.jpeg)

Please verify the wiring.

BAT - &gt;&gt; BMS B -   
BMS P- &gt;&gt; not connected to anything  
BMC C- &gt;&gt; charger port & Anti Spark’s B-
```

---
## \#139 Posted by: farnamweb Posted at: 2019-05-24T01:28:49.947Z Reads: 160

```
1) I just got my Loaded Vanguard Deck. The top has a clear grip coating. Do I still need to install a grip tape? 

btw, Loaded is selling new factory blemished decks for $148

https://www.amazon.com/gp/offer-listing/B075NQGJJ8/ref=dp_olp_all_mbc?ie=UTF8&condition=all

2) There is one XT60 on the battery case for charging. What is the purpose of the other XT60 on the VESC case?

3) What size/length bolt and nuts do I need to attach the wheel pulley to the wheel ? 

I'm assuming that I need to place a nut on the wheel pulley and bolts on the retainer. In that case, there is no room in the wheel pulley hole to hold down the nut using a nut driver.
```

---
## \#141 Posted by: Bor.inc Posted at: 2019-05-28T14:24:11.759Z Reads: 144

```
So just to be sure: if you solder a diode that has a polarity you need to solder it with the minus side of the diode to the + of the vesc and the other on the - ?
```

---
## \#142 Posted by: evoheyax Posted at: 2019-05-28T15:14:13.793Z Reads: 151

```
Nice work. Clean, looks a lot like a boosted but much better I'm sure.

But... I will pick you on your numbers, haha.

5000w/50.4 = 99 amps needed. But here's the catch... at 20a, 30q's will drop from 50.4v to 46v while under power. At 35a, I can't imagine what your dropping down to. With a 12s3p, the most power you can physically get from it is 60a at 46v (which is a full charged 12s3p 30q pack under load) = 2760w for more than .1 of a second. In that .1 of a second, the massive amp draw has little effect on operations, so it's a useless number to say you peak 99a. Thus saying you peak 5000w is kinda misleading, none the less advertising 5000w and not stating it as a peak number. Everyone defines peak and continuous differently. So you can twist the definitions so your not technically wrong. But the reality is your more likely using around 2500w max, which is high powered by the premade board market, but it's a very common watt number for a DIY board.

The problem with everyone misusing peak and continuous numbers is they make it hard to compare boards. I actually pull 10,000 watts for .5 seconds, which is significant in my case as I'm already at 15 mph in that half of a second. So I feel 10,000 watts peak is actually a fair statement. Do I just adjust my settings to 20,000 and say 20,000 peak? I'm sure I could hit close to that for .1 of a second, defiantly not the entire half second it takes me to do 0-15 mph as before.

It's gritting in to the details, I know. But trust me, if you put a lipo in there that actually could do 100a and not sag into a black hole, you would still say your at 5000w and the acceleration would be night and day different, at least 30% faster acceleration. So because there's no standard as to what these numbers are defined as and the lose definitions we have are bent so often, it's unfortunately really hard to compare one board to another without riding both (which is not possible 90%+ of the time on the forums).

Still love your design though. Just get a smaller 12s lipo for shits and giggles (like, $150 usd or less), and you'll see a large power increase.
```

---
## \#143 Posted by: farnamweb Posted at: 2019-05-29T02:46:07.901Z Reads: 146

```
yes connect it in reverse . but if you use a bidirectional diode like the one below, then you are good either way.
https://www.mouser.com/ProductDetail/Taiwan-Semiconductor/P6KE56CA?qs=sGAEpiMZZMvS4F1mNSR4OnsH6NOyMirV
```

---
## \#144 Posted by: farnamweb Posted at: 2019-05-29T02:47:00.663Z Reads: 147

```
I can't get the remote working. I have uploaded the firmware for RX and TX.TX LCD lights up but I see the Voltage as 0. I also can't control the motors. 

1) I have selected UART under "APP to Use" and UART is set to 115200 under the UART tab. Do I still need to follow the "Input Setup Wizard" ? If not, how do I pair TX and RX ? 
2) I can enter the remote menu by holding down the switch and powering on the remote, but I don't know how to change settings there.
3) Do I need to power on the TX first and RX second? 

Vesc : 4.12 with FW3.40  
firmware : https://github.com/Pryside/FireFly-Esk8-NRF24/blob/master/libraries  
VescUart Lib : https://github.com/SolidGeek/VescUart
```

---
## \#145 Posted by: Adam80bush Posted at: 2019-05-31T01:34:30.795Z Reads: 128

```
Interested in how the battery performs after continuous braking downhill. I'm aware of some issues that other boards have with this. Would love to hear about your own personal experience :grinning:
```

---
## \#146 Posted by: evoheyax Posted at: 2019-05-31T02:17:45.092Z Reads: 137

```
This is because you can only put 12amps back into the battery. If your on a 10% grade hill with 200 lb, your brakes will feel weak as you Don’t have anywhere to put the power your motors generate. So you have to generate less braking.

You have to remember you motor has to sets of magnets. You can send power to the stator electro magnet, which pushes your rotators permenant magnets (ie acceleration) or vice versa (ie regen braking). Your motor generates power, but with no wheels to put it, it can’t turn it in to braking.

Smaller lion batteries have this issue, which is why most regular members are turning to 12s6p or higher these days. I think I had one of the smallest batteries in the Vegas meetup for example which was basically a 12s3p in size.
```

---
## \#147 Posted by: farnamweb Posted at: 2019-06-01T12:50:57.087Z Reads: 133

```
![20190601_084519|281x500](upload://6O0KJQoQWUqrQr9FLUBsnUtUdyl.jpeg) 

Anti Spark is working great. Let me know if you need help. I may even build a few more and sell it with @Pryside 's permission.
```

---
## \#148 Posted by: matiller Posted at: 2019-06-01T17:48:41.726Z Reads: 128

```
Did anyone try using Pryside´s remote? How did you set it up in vesc tool?
```

---
## \#149 Posted by: Pryside Posted at: 2019-06-05T09:16:32.450Z Reads: 121

```
Will sell my own pcb soon, want to make some small changed, so in 2-3 weeks an ebay page should go up
```

---
## \#150 Posted by: Pryside Posted at: 2019-06-05T09:18:22.200Z Reads: 121

```
Set it up as uart/nunchuck 115200 baud. Needs vesc FW 3.x, will not work on the old FW 2.18 altough I can easily make a alternative reciever version if some want this.
```

---
## \#151 Posted by: Pryside Posted at: 2019-06-05T09:19:08.982Z Reads: 121

```
ebay page will come soon :)
```

---
## \#152 Posted by: Pryside Posted at: 2019-06-05T09:20:38.153Z Reads: 128

```
Had it configured for my pins on my reciever board. now changed it to the more common
RF24 radio(9, 10); where pin 9 and 10 get used for spi

If it was a connection issue that should fix it.
```

---
## \#153 Posted by: Pryside Posted at: 2019-06-05T09:25:50.861Z Reads: 133

```
sry for late answer. (I'll write here the same as I wrote in DMs so everybody knows)
1.  nope not needed, but If you want to hide your flat copper wires, you should definitly do so.
2. Main Idea was for 12V leds and phone charger with a small dc dc on the inside, but not used yet and just left it there for creative ideas
3. M5, and I just screwed them in the way it is currently but would recommend just using some 2k epoxy and put a bit around the nut place it in there and let it dry, that should do the job.
```

---
## \#154 Posted by: Pryside Posted at: 2019-06-10T16:50:49.871Z Reads: 127

```
Due to the strong censorship on this website, and many great builders getting banned I created the same thread over here. I will stay active on both for now, but looks like this forum will die soon.
https://forum./t/3d-printed-boosted-board-killer/2247
```

---
## \#155 Posted by: KranzeKake Posted at: 2019-06-13T22:55:19.549Z Reads: 121

```
Did you ever think about sending the UART data from your BMS over to your firefly remote?
Also, did  you disable the bms for discharge?
```

---
## \#156 Posted by: Pryside Posted at: 2019-06-22T20:09:48.595Z Reads: 117

```
Hm... what exactly do you have in mind, because other then soc theres not much interesting data to read from a bms. And soc is currently indicated by a voltage bar on the remote... so no real need for that i think
```

---
## \#157 Posted by: Philipp6 Posted at: 2019-06-23T15:01:17.316Z Reads: 116

```
Hey Pryside can I use your anti spark with a voltage of 22.2V (6s).Or must I use other mosfets.
```

---
## \#158 Posted by: Daniel_Kievit Posted at: 2019-06-27T11:45:40.260Z Reads: 111

```
Hi Leo,

How did you open your torqueboards motor and which waterproofing agent did you use?


Greetings,

daniel
```

---
## \#159 Posted by: Daniel_Kievit Posted at: 2019-06-27T11:46:21.401Z Reads: 108

```
I would not do that, because the voltage must be very high because of the voltage spikes
```

---
## \#160 Posted by: Rebuild Posted at: 2019-06-27T15:28:58.505Z Reads: 108

```
@pryside does your antispark design have any current draw when off?   Do you have a link for your eBay store so we can watch for when it becomes available there?  🤓
```

---
## \#161 Posted by: Daniel_Kievit Posted at: 2019-07-08T19:24:00.843Z Reads: 111

```
Hi leo, I have a couple of questions for you:

- Which glue did you use to fix the magnets in the motor?
- How did you open up the motor?
- Which waterproofing agent did you use for all of the circuit boards?

- Should I use a TVS diode for my torqueboards esc running on 10s, and if so, which one would you remommend, or which breakdown voltage should it have?

- Can I charge my 10s4p battery pack with a 10s 30A BMS, or is it recommended that you charge batteries separately from the BMS with a balanced charger?

Does anyone else maybe know any answers to my questions? 

Any help would really be appreciated!
```

---
## \#162 Posted by: farnamweb Posted at: 2019-07-11T03:27:39.913Z Reads: 104

```
* Which glue did you use to fix the magnets in the motor? IDK
* How did you open up the motor? 
There are a few tiny screw on the side of the motor. take those off and you should be able to pull the bottom side. Magents are strong so, pull it hard. make sure you put loctite on the screws when you are putting them back in. 
* Which waterproofing agent did you use for all of the circuit boards?  
not sure what he used, but this is a good one. 
https://www.amazon.com/gp/product/B008O9YIV6/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1
* Should I use a TVS diode for my torqueboards esc running on 10s, and if so, which one would you remommend, or which breakdown voltage should it have?  
yeah TVS diode can help 10s as well. Get one with a breakdown voltage higher than 42 but close. search mouser.com 
* Can I charge my 10s4p battery pack with a 10s 30A BMS, or is it recommended that you charge batteries separately from the BMS with a balanced charger?  
The bms that he is using does balance charging so there is no need to use a separate charger, However, you need to input 10s voltage using a power supply. I would get a 60A BMS because BMS is gonna handle discharge as well.   
https://www.lithiumbatterypcb.com/product/14s-bluetooth-lithium-e-bike-battery-pcb-board-with-30a-constant-charge-and-discharge-current-2/
```

---
## \#163 Posted by: Daniel_Kievit Posted at: 2019-07-13T15:56:33.054Z Reads: 97

```
Hi,

I have seen you on the other forum for the firefly remote to lol :) 

I am also going build the antispark system from leo. Is yours already finished? How high was the wattage of your wire resistor? 

And Leo, what do you mean by "a quite high power rating" for your wire resistor?
```

---
## \#164 Posted by: farnamweb Posted at: 2019-07-13T16:03:59.151Z Reads: 107

```
* yep, I have been using it for a while now. It works great. Here is the updated list 

* • 1X Veroboard
* • Power switch 
* https://www.amazon.com/gp/product/B0713QRSZN/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1
* • 4X 1M Ohm Resistors (R1,2,4,5) 
* https://www.mouser.com/ProductDetail/Welwyn-Components-TT-Electronics/MFR3-1M0FC?qs=sGAEpiMZZMtlubZbdhIBIJtQxnYsq7hXit92tIgpI8A%3D
* • 1X 15 Ohm Resistor(R6) 
* https://www.mouser.com/ProductDetail/Yageo/PNP300JR-73-15R?qs=sGAEpiMZZMtlubZbdhIBINt%2Ft6Hry3%2FBZn3Gyw1qhA0%3D
* • 1X 1 OHM Resistor ( R3) >>  
* https://www.mouser.com/ProductDetail/Ohmite/TUW5J1R0E?qs=sGAEpiMZZMtbXrIkmrvidMPY4i6h3AHP%252BV%252BE2e384xE%3D
* • 3X 12V Zener Diodes(D1,2,3) 
* https://www.mouser.com/ProductDetail/ON-Semiconductor/1N5927BRLG?qs=sGAEpiMZZMtQ8nqTKtFS%2FJ7m6e1KBCgub6c2uyKgC%252BY%3D
* • 1X 16V 4.7μF Capacitors(C1)
* https://www.mouser.com/ProductDetail/Nichicon/USP1C4R7MDD?qs=sGAEpiMZZMsh%252B1woXyUXj7onzYv6nMPCw8k8X5hq4n8%3D
* • 2X IRFS7530 Transistors(T1) 
* https://www.mouser.com/ProductDetail/Infineon-Technologies/IRFS7530TRL7PP?qs=sGAEpiMZZMshyDBzk1%2FWi%252BDdTe3kt8oihq%2FEFTk6nI%252BSM6z%252BASO6Fg%3D%3D
* • 1X IRFB3006 Transistor(T2)
* https://www.mouser.com/ProductDetail/Infineon-Technologies/IRFB3006GPBF?qs=sGAEpiMZZMshyDBzk1%2FWi5%252BqVgN3%252BWS8frDEDJEFm2A%3D
```

---
## \#165 Posted by: Daniel_Kievit Posted at: 2019-07-13T17:52:46.849Z Reads: 94

```
Hey,

I found a lot of TVS diodes, but I'm not sure which one to choose. What precise voltage would be recommended for my 10s (42V) longboard? I can choose from 42.1 to approx 80v. 

And are there also demands for the:
- Peak pulse current
- current
- Peak pulse power dissipation
- Power dissipation?

And what is the difference between the clamping voltage and the breakdown voltage, because I can only choose from clamping voltage. Mouser is too expensive with shipping costs for me.
```

---
## \#166 Posted by: Philipp6 Posted at: 2019-07-13T20:20:43.222Z Reads: 92

```
Hey Leo Pryside
I have found mosfets like the IRFS7530-7PPBF and the IRFB3006PBF .The datasheet says that the mosfets have a maximum Gate to Source voltage of 20V.Can I power the Anti Spark with a voltage of 25,2V with fully charged battery(6S) and 18-19V when discharge??
```

---
## \#167 Posted by: farnamweb Posted at: 2019-07-14T00:27:04.181Z Reads: 96

```
This is a good one for 10S  
https://www.mouser.com/ProductDetail/Taiwan-Semiconductor/P6KE47CA?qs=sGAEpiMZZMvS4F1mNSR4OiB1XnQ6vcFb

If I understood it correctly, breakdown voltage is the voltage that the diode starts clamping the voltage spikes and clamping voltage is when the diode restricts voltage past this number.

Just get a diode with the breakdown voltage higher than 42V for 10S (10X4.2 ) and also close to 42V. something around 70V for clamping voltage should be fine too.  I don't think the other values matter.
```

---
## \#168 Posted by: Philipp6 Posted at: 2019-07-24T12:32:45.955Z Reads: 88

```
The code from the Firefly work fine but the receiver code dont work 
Arduino: 1.8.8 (Windows 10), Board: "Arduino Nano, ATmega328P (Old Bootloader)"

sketch_jul24b:6:1: error: 'VescUart' does not name a type
```

---
## \#169 Posted by: Daniel_Kievit Posted at: 2019-08-03T22:05:57.633Z Reads: 84

```
Hey man,

How many amps does the switch for the antispark need to be able to handle?
```

---
## \#170 Posted by: farnamweb Posted at: 2019-08-03T22:54:25.157Z Reads: 82

```
I'm not sure. @Pryside designed the circuit
```

---
## \#171 Posted by: Pryside Posted at: 2019-08-03T23:56:26.042Z Reads: 82

```
around 200A peak for sure and 30 amps constant. But you will always have to prechage the esc otherwise you will destroy any contactor or mosfet
```

---
## \#172 Posted by: sdoerflinger Posted at: 2019-09-13T07:57:29.404Z Reads: 74

```
@Pryside Hallo Leo, vielen Dank für die Pionier Arbeit, ich bin gerade auch dabei mein Board zu bauen. Da ergeben sich einige Fragen:

-Beim Anti-Sparkswitch, Kühlkörper braucht man da keine für die MOSFET oder?
-R3 also den 1 Ohm Widerstand, weißt du wieviel Watt der aushalten muss, bzw. reicht ein 5W Metalloxid Widerstand oder soll ich mir einen 10/25W Metallgehäuse Hochlast widerstand besorgen?

-Bei der Programmierung vom Receiver und Fernbedienung ist im Code die Nunchuck geschrieben bzw. auch mit upper und lower button, hattest du nicht auch die Firefly remote?  

Vielen Dank für deine Hilfe :slight_smile:

Gruß 
Stefan
```

---
## \#173 Posted by: jmasta Posted at: 2019-09-13T21:37:37.137Z Reads: 77

```
5000W on 3D printed pulleys and 12mm belts :face_with_raised_eyebrow:

[quote="Pryside, post:76, topic:88803, full:true"]
Here is a full calculation of how much power you can actually get using my setup:

Fully charged Battery at 50,4V. IR per cell is 20mOhm (DC iR from Datasheet), 3 in paralell is 6,3mOhm, 12 in series is 75mOhm
Lets calculate the theoretical maximum. I currently have a 75A Current Limit, but lets assume I set this to 90A say I go full throttle:
My Vescs pull 180A
180A * 0,075Ohm = 13,5V voltage drop inside my Battery
50,4V-13,5V= 36,9V Voltage going to my VESC (still above 3V per cell)
36,9V * 180A = 6642W so thats the amount of Power getting eaten from my vesc.
Thats where usually everybody stops and says that this is the power, but since there are a ton of losses at this current here is the real mechanical power that you would be measuring on a dyno:
Resistance of my vescs: 0,0011Ohm Resistance of Motors: 0,0225Ohm
(0,0011Ohm+0,0225Ohm)*180A²= 764,64W of Power loss in Motors and ESC
6642W-764,64W= 5877W MECHANICAL POWER
so yes, the 5kW is easily possible.﻿
[/quote]

You're not taking into account the limitations of your mechanical drivetrain.  Even if your electrical system was somehow capable of 5000W like you claim, your belts cannot physically transmit that much power, especially when using 3D printed pulleys

Cool looking build though!
```

---
## \#174 Posted by: careyer Posted at: 2019-09-22T09:07:22.581Z Reads: 68

```
Hi Leo!  I hope you can help me really quickly... I am DIYing my own E-Longboard right now and would like to add a TVS diode to my seltup as well. I am running on a 10S2P (18650)  Setup with a Dual VESC 4.20. Can you please give me advice what TVS diode I should use? I think you run on a 12S setup right? Do the diode specs need to be any different between 12S and 10S? Thank you so much! 

Cheers!
P.S:I posted this question in the YT comments as well. I really hope this reaches you!
```

---
## \#175 Posted by: Pryside Posted at: 2019-09-22T18:57:34.024Z Reads: 70

```
Please in english so others can understand you.
You cant really cool the mosfets on the antispark, thats not really possible and not required, it can easily handle 50A constant in my tests

I have a old version of my antispark in my board with a normal metal film resistor that works fine
But I would recommend something with a rating of maybe 10W just to be on the safe side. But generally decent THT Resistors will work

Thats just because benjamin vedder called the normal 0-255 current control "nunchuck" and thus everybody now calls it that. Has nothing to do with what the physical apperance of your remote is
Lower and upper button allow you to do reverse and cruise control. which I tried before but found both useless
Reverse is simply never practical in day to day use.
and cruise control is not required, since the firefly scroll wheel design makes it easy to just keep the throttle in the same position for hours nonstop
```

---
## \#176 Posted by: Pryside Posted at: 2019-09-22T19:01:39.967Z Reads: 73

```
that is simply wrong. There is a belt calculator for other belts online and I calculated this a while ago and it came out that my belts can widthstand around 15Nm, with a 16-42T HTD 5M transmission. And the 3D printed PLA pulleys are not a issue at all, they could easily carry 40Nm
Its a very strong plastic and the belt applies torque on all the sides
I do in fact get issues if I go full throttle often because my belts will get weakened and strart slipping 200Km into every new belt but other then that this drivetrain is well capable of bringing down the 12Nm on these 100mm wheels to the ground
```

---
## \#177 Posted by: Pryside Posted at: 2019-09-23T07:50:17.086Z Reads: 64

```
I havent opened a Shopsite yet but will do that soon. If you want to buy a Pre Chage Antispark from me just write me pryside.business@gmail.com

Price is 40€ incl. Shipping

It can easily handle 130A Peak (10 seconds) and around 60A constant

Its rated for 60V max (12S)

Have friends excessively test it already on eBoards and I have benchmarked it hard on my eBike with a 150A Battery Amps Controller and it works perfectly.

![image|690x388](upload://4nxkctPQJef7yj9b0LpXBghwnsU.jpeg)
```

---
## \#178 Posted by: mugnog Posted at: 2019-11-16T07:09:38.811Z Reads: 49

```
HI farna,

could you make a picture from above and below of yout anti-Spark? Thx
```

---
## \#179 Posted by: farnamweb Posted at: 2019-11-16T10:28:28.859Z Reads: 50

```
![20190608_103015|690x388](upload://gxuvL6I23HscWLA8qUVGXfq15Xb.jpeg) ![20190608_103009|690x388](upload://fUKZhtyWJe2hH8YqzRxyejbdAM0.jpeg) ![20190608_103003|690x388](upload://i9dQUx8lUAG0MS605bG43pF5Tnk.jpeg) ![20190608_102941|690x388](upload://8w631VOYOM2tjxf8XErZLsYuQgE.jpeg) ![20190608_102938|690x388](upload://7PSmOR3djP4MZi6PkGYwkvODBxk.jpeg) ![20190608_102935|690x388](upload://56fQfWCLZLrfDhgSrk8KUUxe039.jpeg) ![20190531_230612|281x500](upload://6ZLIouoW0JUlfMlqdQmL50n2p1O.jpeg)
```

---
## \#180 Posted by: mugnog Posted at: 2019-11-16T16:00:05.452Z Reads: 46

```
Superb!!!
Thx farnamweb!!!
Is it still working???
```

---
## \#181 Posted by: THERW Posted at: 2019-11-20T01:24:36.890Z Reads: 41

```
Not sure if it was already mensioned but what is the estimated cost of this, I currently own a v2 dual plus but now have a longer commute and range is becoming an issue, I am considering building a DIY or buying an evolve bamboo gt and swapping out the ESC as I am not a fan of the jerky movement and the prefer the thumb wheel remote any advice?
```

---
## \#183 Posted by: MadPatch Posted at: 2019-11-30T20:03:35.059Z Reads: 29

```
Hey is your remote compatible with vesc 6 hardware?
```

---
