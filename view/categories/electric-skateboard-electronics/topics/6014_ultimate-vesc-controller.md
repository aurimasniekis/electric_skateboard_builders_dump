# Ultimate VESC Controller

### Replies: 71 Views: 12472

## \#1 Posted by: vitormhenrique Posted at: 2016-07-13T04:22:36.002Z Reads: 1104

```
After my initial [prototype](http://www.electric-skateboard.builders/t/custom-vesc-controller-prototype/1073/2) I finally worked out the bugs and got version two working.

<img src="/uploads/db1493/original/2X/5/568d92f8e07583b74e91bd312b9bde7a5cafc186.JPG" width="666" height="500">

After seeing the GT2b from @FLATLINEcustoms I knew that that design was the ultimate one, unfortunately I asked him to share the step files to modify it but until this date he didn't.  As editing STL files is a pain in the a** I recreated the design from scratch using Fusion 360, but I'm terrible at CAD designs and could not recreate the chamfers and few details that make his work much better. 

Functionalities: 
The remote use xbee radio to connect to another micro controller that handle the received data. I decided not connect the xbee directly to VESC's because I'm planing to add more stuff to the receiver, like GPS, LED's etc... So I don't want to create a bunch of custom applications on VESC.

The remote has 3 buttons, one is a cruise control, the other two can handle multiple or single clicks to different functionalities, for now: turn on and off lights, change mode from rabbit to turtle.

Few more pictures of the design, and build process

<img src="/uploads/db1493/original/2X/3/35f560e6256e4f2c3d057b7c9dcb21cfed6e55d4.png" width="560" height="500">
<img src="/uploads/db1493/original/2X/8/801c669deed492f15f65ac8e82afc763ab8e9d0c.JPG" width="666" height="500">
<img src="/uploads/db1493/original/2X/d/d26d1c1e7ca5ca9c0f299895301b476cbf38b29b.JPG" width="666" height="500">
<img src="/uploads/db1493/original/2X/2/23ee06e54dd2633600fa2c7d374beb73141fd3e5.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/8/82f83ed75e755a2e3e89b6932e8fbcb34ddd55e1.JPG" width="666" height="500">

As you can see the controller uses teensy-lc as the micro controller and a ST7735 based lcd to display information. I'll put the files on thing-verse together with the firmware of the remote, I can definitely help however wants to reproduce this but you need to have basic knowledge of electronics, I can not explain how to wire a potentiometer
```

---
## \#2 Posted by: Chris_KP Posted at: 2016-07-13T04:30:55.091Z Reads: 885

```
thats so freakin awesome!!
```

---
## \#3 Posted by: Blasto Posted at: 2016-07-13T04:31:56.372Z Reads: 874

```
Good job! Looks nice, will you make a pcb to get rid of all that hook up wire?
```

---
## \#4 Posted by: vitormhenrique Posted at: 2016-07-13T04:43:42.316Z Reads: 854

```
Yeap... 

Next step is to create a PCB and also design the trigger part to be 3d printed, I'm still using the trigger assembly removed from the gb2b controller. I'll also test using nrf24l01+ radios because xbee's are way to expensive, 23 bucks each, but they are very very reliable. 
Another problem is that nrf24l01 will need to share the SPI of the arduino*, not sure if the libraries (for the lcd and the radio) are already handle that, if not, I'm not very interested on updating them to make it happen, and I will leave xbee radios on the final version.
```

---
## \#5 Posted by: Ulfberht Posted at: 2016-07-13T05:48:05.507Z Reads: 789

```
This is the most amazing thing on the forum right now. IMO :astonished::thumbsup:
@vitormhenrique You are a true innovator!!
```

---
## \#6 Posted by: Pablo_702 Posted at: 2016-07-13T05:48:31.826Z Reads: 758

```
You should sell these
```

---
## \#7 Posted by: akira Posted at: 2016-07-13T05:57:03.689Z Reads: 742

```
@Pablo_702
If he plans to release the instructions and plans open source, it is much better than selling it. 

@vitormhenrique fantastic design ! Thus is truly amazing ! If you release the schematics and microcontroller code, I will surely give it a try !!
```

---
## \#8 Posted by: sismeiro Posted at: 2016-07-13T08:59:41.361Z Reads: 703

```
This is the community answer to the more advanced Evolve and Stary remote controllers. Good work! :smiley:
```

---
## \#9 Posted by: torqueboards Posted at: 2016-07-13T09:19:21.970Z Reads: 694

```
Well done! @vitormhenrique

Well done...

:grin:
```

---
## \#10 Posted by: onloop Posted at: 2016-07-13T09:26:24.302Z Reads: 664

```
VERY COOL...  watch out evolve.
```

---
## \#11 Posted by: jrpwit Posted at: 2016-07-13T09:33:15.430Z Reads: 647

```
Holy crap!!! THAT IS SO AWSOME!!! By far the best remote in my opinion!:
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-07-13T11:14:02.667Z Reads: 639

```
Nice controller. I had the exact same idea....
I would say "current" and not "curret" ;)
What is this for a mode "rabbit"?
```

---
## \#13 Posted by: XvDarkVAngelvX Posted at: 2016-07-13T11:36:41.351Z Reads: 617

```
I had made an inquary about a system of this type about a week ago 👌 and here we are. I 🎼 must take my 👒 hat off to 😋 you. You are Dr. Frankenstein to my creation. This is a must have. When will we be ready for production?
```

---
## \#14 Posted by: lox897 Posted at: 2016-07-13T11:38:28.731Z Reads: 609

```
Rabbit = Fast and torquey
Turtle = Slow (for beginners)
```

---
## \#15 Posted by: laurnts Posted at: 2016-07-13T11:38:49.469Z Reads: 592

```
This is so epic. Telemetry data! I had it on my RC car remote this data, but the receiver is abit sensitive that it broke down easily. I'll be looking forward for this one!
```

---
## \#16 Posted by: bill_f Posted at: 2016-07-13T11:54:57.064Z Reads: 579

```
Sweet!  Thanks for posting this here and for putting CAD files on Thingiverse. New to VESC but this looks like a good project down the road.
```

---
## \#17 Posted by: vitormhenrique Posted at: 2016-07-13T14:10:06.267Z Reads: 613

```
[quote="akira, post:7, topic:6014"]
If you release the schematics and microcontroller code, I will surely give it a try !!
[/quote]

Yeah... I'll share, but I was planing to share once I have the pcb done (for the receiver and the remote). I'll start working on that tonight and I'm estimating two weeks to get it done. If you guys want the hacked version schematics I can do that too.

[quote="DeathCookies, post:12, topic:6014"]
I would say "current" and not "curret"
[/quote]

ops.... thanks! :)  rabbit and turtle are two different modes with different acceleration. Rabbit will push whatever throttle you give on the trigger, while turtle will slow down the acceleration.
```

---
## \#18 Posted by: akira Posted at: 2016-07-13T14:20:43.758Z Reads: 577

```
@vitormhenrique
I don't think I'll have time to try it before several weeks. If you route a PCB, I'll wait for that.
I still have to complete my "simple" GT2b.

I did not know the teensy microcontroler, there are some many out there now !!
Have you written your code in C or arduino-like ?

Anyway, great stuff here !!
```

---
## \#19 Posted by: vitormhenrique Posted at: 2016-07-13T14:46:49.468Z Reads: 580

```
[quote="akira, post:18, topic:6014"]
Have you written your code in C or arduino-like ?
[/quote]

arduino language is actually C with custom functions to access the hardware of the atmega microcontroller. Teensy is a arduino compatible micro, but the specs are much much better, form factor, speed, etc... But for the final version I think I'll stick with the atmega328 with the arduino bootloader.

I'm still not sure about the LCD size, 1.8" is cool, but it may be too big?
```

---
## \#20 Posted by: akira Posted at: 2016-07-13T14:50:33.521Z Reads: 577

```
@vitormhenrique

Thanks for the informations. I have played a bit with the arduinos ... (nano and uno mainly).

I guess that the main constrain is the ergonomy of the controler in your hand.
Does it fit well with this big screen ?
I have not yet tried the original version of Flatline but I am a bit worried that my hand is too small for this big design.
```

---
## \#21 Posted by: vitormhenrique Posted at: 2016-07-13T15:01:04.781Z Reads: 515

```
my hands are pretty small, actually, maybe too small =/ 

And the controller still fell good, I need to improve the design a little bit and increase the chanfers to get closer to @FLATLINEcustoms design.
```

---
## \#22 Posted by: cmatson Posted at: 2016-07-14T02:59:01.215Z Reads: 508

```
so many people would buy this a remote like this..

if there is one thing the DIY community lacks, it's a solid remote that is reliable yet still remains compact with cool features. This guy is the ticket!
```

---
## \#23 Posted by: mishrasubhransu Posted at: 2016-07-14T03:21:06.683Z Reads: 521

```
Awesome job! 

I happen to have all the components lying around it my lab. Actually, I have a sparkfun lcd instead. If you could share the hacky schematics and the arduino code, I might be able to replicate it in a week or so.
```

---
## \#24 Posted by: Michaelinvegas Posted at: 2016-07-14T03:35:38.216Z Reads: 519

```
👍🏻 .

--------------
```

---
## \#25 Posted by: vitormhenrique Posted at: 2016-07-15T02:01:16.578Z Reads: 551

```
Due to the very good feedback I'm already working on the final version, I'll test few different radios on the first PCB, including the nrf24l01, some lora radios and maybe bluetooth.... 

I spend the last two nights learning how to design a more organic form using the sculpturing part of fusion 360, I'm pretty pleased with the new design...

The curves are much more smooth and it should have much better grip on the hand....

<img src="/uploads/db1493/original/2X/0/0854b58ab659da8d1688247bc77bb108cc30b719.png" width="388" height="499">
<img src="/uploads/db1493/original/2X/9/923686781b0c888ac5c7fab5af2fdfad3186bf40.png" width="637" height="500">
<img src="/uploads/db1493/original/2X/c/ccbb5e7cc6280801d7cd852b27fbb07337f1f974.png" width="668" height="499">
```

---
## \#26 Posted by: MasterCho Posted at: 2016-07-15T02:56:35.114Z Reads: 512

```
Great job!  If you need any help, please let me know I am familiar with fusion 360 as well.
```

---
## \#27 Posted by: Eboostin Posted at: 2016-07-16T03:03:11.612Z Reads: 505

```
Any chance you'd consider a slide potentiometer version?

Otherwise this remote is perfect! 

The Ego and Marbel remotes are so nice to use with the slide.
```

---
## \#28 Posted by: jmasta Posted at: 2016-07-21T19:08:42.442Z Reads: 490

```
This is awesome!  I would love to help out and make one myself. I have access to 3D printing
```

---
## \#29 Posted by: vitormhenrique Posted at: 2016-07-21T19:42:50.902Z Reads: 504

```
I'm working on the final design and the PCB.... 
I ordered a bunch of different components and different radio modules..

My goal is to design a controller that is reliable, I started the pcb design and will be testing few radio units this weekend.

I also have a friend that is mechanical engineer and very good with cad and industrial design, today we will have a session and try to finalize the design.

Once I finish the pcb, I'll order from OSHPark and test it out, if it proves to work as the prototype, I'll share the code, design and pcb. 

@Eboostin this is already a potentiometer version :stuck_out_tongue: as the thrigger is connected to a potentiometer but I see what you mean, you want a slide potentiometer... I'll only consider that after finishing this version.
```

---
## \#30 Posted by: Blasto Posted at: 2016-07-21T19:47:04.498Z Reads: 477

```
check out pcbway for protos, I find them faster and cheaper. haven't seen an issue in pcb quality

http://www.pcbway.com/
```

---
## \#31 Posted by: vitormhenrique Posted at: 2016-07-21T19:48:19.409Z Reads: 464

```
faster shiping from china to USA than oshpark?
```

---
## \#32 Posted by: Blasto Posted at: 2016-07-21T19:50:43.687Z Reads: 470

```
well to be fair i'm in canada, osh park uses usps-canada post for the free shipping option, usually takes 2-3 weeks once shipped.

pcbway uses dhl, usually takes 4 days to get here

anyways you can get accurate quote from both companies
```

---
## \#33 Posted by: vitormhenrique Posted at: 2016-07-21T19:53:34.771Z Reads: 478

```
I'll check it out.... I'm lucky using oshpark and most of my orders were upgraded to "Super Swift Service" for free... 

But I'll compare both services :)  

Thanks for the tip!
```

---
## \#34 Posted by: Ulfberht Posted at: 2016-07-21T20:11:32.629Z Reads: 482

```
[quote="vitormhenrique, post:29, topic:6014"]
Once I finish the pcb, I'll order from OSHPark and test it out, if it proves to work as the prototype, I'll share the code, design and pcb.
[/quote]

That is remarkably generous of you! Thank you @vitormhenrique!!
Are you going to share the BOM with the design information? This is a very exciting build!
```

---
## \#35 Posted by: nicolasgod Posted at: 2016-07-23T15:01:57.664Z Reads: 460

```
That's a really nice work, respect to you for designing with fusion360, that's the worst soft for CAD, not convenient to use to design mechanical parts.
```

---
## \#36 Posted by: jmasta Posted at: 2016-07-25T15:44:38.887Z Reads: 445

```
I'm proficient in both Pro/E (Creo) and SoildWorks,  Let me know if you want any help with the CAD
```

---
## \#37 Posted by: boards Posted at: 2016-07-25T16:11:44.729Z Reads: 470

```
I have a teensy 3.0 that I've already connected to an RF module and a nunchuck (using nunchuck connections, not direct). It still fits into the nunchuck even though I haven't made custom pcb. Just need to get to making the software portion...
```

---
## \#38 Posted by: Dedbny Posted at: 2016-07-29T23:56:18.274Z Reads: 476

```
Keep up the good work.  Maybe you could do something with Enertion.  Your remote with a Raptor would be great.
```

---
## \#39 Posted by: alexmarin99 Posted at: 2016-07-31T16:39:31.300Z Reads: 514

```
Hi, very nice work you did there!

I've also made a remote similar to yours.

I've created my own PCB that includes a charger for 18650 lithium battery, arduino nano, adafruit screen and bluetooth HC-05.
I don't use any GT2B or anything else.

The receiver is another arduino with bluetooth module.

PM me, maybe we could do something even nicer!

<img src="/uploads/db1493/original/2X/b/b4e50b708ae293abe1a8a3513c9e96ee07ae2f41.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/9/9e9bf4f316e4989713917208fab7b6b2c26d869c.jpg" width="375" height="500">

Sorry for all the wires, will be better in version 2.0 :P
```

---
## \#41 Posted by: Workaround Posted at: 2016-07-31T17:03:19.464Z Reads: 499

```
Where is the arduino code you used for this. I want to make my own controller similar to this.
```

---
## \#42 Posted by: cjoliver Posted at: 2016-07-31T18:40:33.839Z Reads: 479

```
Does your controller ever cut out mid-ride? Have been considering bluetooth but worried about interference
```

---
## \#43 Posted by: alexmarin99 Posted at: 2016-07-31T19:11:11.546Z Reads: 485

```
I created my own code for this,  because I'm using my own hardware.

So my code won't work for you, unless you have the exact same PCB as me :/
```

---
## \#44 Posted by: alexmarin99 Posted at: 2016-07-31T19:14:16.947Z Reads: 501

```
It never cut out mid-ride. I've never had a problem with this bluetooth module (HC-05, around 4$/piece). 

I'm considering building my own bluetooth module and to integrate it with the other electronics, to save some space.

Also, range is 20m line-of-sight.
```

---
## \#45 Posted by: Workaround Posted at: 2016-07-31T19:14:27.381Z Reads: 491

```
I just need to look at an example that i can play so I can start on my project. I'm doing something similar.
```

---
## \#46 Posted by: alexmarin99 Posted at: 2016-07-31T19:29:30.645Z Reads: 503

```
I'll release the code and other files when everything will be finalized. 

In the meantime, I suggest that you look at serial communication between two arduinos.
The addition of bluetooth is simple, because it's the same thing as having a wire between the two arduinos, except it's wireless :stuck_out_tongue:

Here are some links:

http://projectsfromtech.blogspot.ca/2013/05/arduino-serial-communication-between.html 
https://www.arduino.cc/en/Tutorial/MasterWriter

edit:
Code for the Adafruit screen is given by them, so it's also pretty straightforward. I've managed to make it running in less than 10 minutes.
```

---
## \#47 Posted by: Hillso Posted at: 2016-08-02T14:51:39.122Z Reads: 480

```
this is pretty cool: https://www.youtube.com/watch?v=1jJkVAt6YOw
```

---
## \#48 Posted by: cesargrimmelprez Posted at: 2016-08-10T12:49:21.991Z Reads: 464

```
Awesome dude! Please try to sell it
```

---
## \#49 Posted by: Heavy1 Posted at: 2016-08-22T21:49:01.545Z Reads: 469

```
any updates on this amazing project ?
```

---
## \#50 Posted by: vitormhenrique Posted at: 2016-08-25T15:31:44.463Z Reads: 482

```
Quick update!

Things were a little slow on the development, due to few issues, mainlyI had my electric skateboard stolen, so I did not had anything else to test and I wanted to ride a sk8, I had no spare VESC and I prioritized building a new esk8 first, and you guys know how difficult is to get VESC's especially. So I finally got to a point that my esk8 is working, few minor things to add but I can work on both the remote and my esk8 at the same time.

Pictures of the new ride.... 

<img src="/uploads/db1493/original/2X/f/f81233e2ec830068151d96dbd39fe54f8e7f4904.JPG" width="666" height="500"><img src="/uploads/db1493/original/2X/a/ab3207686104c2d328b55952f0bd1a3187664dc5.JPG" width="666" height="500">
```

---
## \#51 Posted by: Raf Posted at: 2016-08-25T15:35:21.801Z Reads: 465

```
what wheel are those?
```

---
## \#52 Posted by: vitormhenrique Posted at: 2016-08-25T15:43:44.805Z Reads: 466

```
[quote="Raf, post:51, topic:6014, full:true"]
what wheel are those?
[/quote]

http://shop.mbs.com/accessories-488/mountainboard-wheels/mbs-all-terrain-longboard-wheels.html
```

---
## \#53 Posted by: cesargrimmelprez Posted at: 2016-08-25T18:25:04.048Z Reads: 454

```
What battery do you use?
```

---
## \#54 Posted by: vitormhenrique Posted at: 2016-08-25T18:40:28.465Z Reads: 465

```
[quote="cesargrimmelprez, post:53, topic:6014, full:true"]
What battery do you use?
[/quote]

I'm guessing you are asking what is battery of the skateboard, not the controller. The eSK8 uses custom batery made of [a123 cells](http://www.a123systems.com/lithium-ion-cells-26650-cylindrical-cell.htm) on a 12S2P configuration. I'll make a post of my sk8 on a separete thread.
```

---
## \#55 Posted by: cesargrimmelprez Posted at: 2016-08-25T18:41:26.010Z Reads: 463

```
Ow hahah yes, indeed, ill check out build thread
```

---
## \#56 Posted by: Heavy1 Posted at: 2016-08-26T20:10:39.907Z Reads: 458

```
Would there be the ability to add in cell monitoring to the controller?
```

---
## \#57 Posted by: hackeralf Posted at: 2016-10-21T06:46:01.552Z Reads: 376

```
How much is it?
```

---
## \#58 Posted by: webst Posted at: 2016-10-25T13:41:43.759Z Reads: 367

```
[quote="Workaround, post:45, topic:6014, full:true"]
I just need to look at an example that i can play so I can start on my project. I'm doing something similar.
[/quote]

Well, did you find some kind of workaround? Pun intended ;)
```

---
## \#59 Posted by: julian46 Posted at: 2016-12-02T14:17:13.788Z Reads: 327

```
Did you try the nRF24L01 radio module ? - just wondering what you thought of it...
```

---
## \#61 Posted by: lox897 Posted at: 2016-12-05T11:16:44.307Z Reads: 314

```
Is this project still going? @vitormhenrique
```

---
## \#62 Posted by: Fabian287 Posted at: 2016-12-10T19:15:17.697Z Reads: 321

```
COOL!!
How is it going on with you projekt?
I cant wait to make it :heart_eyes: or can you send your codes to me?:stuck_out_tongue: @vitormhenrique
```

---
## \#63 Posted by: Okami Posted at: 2017-01-14T14:23:57.691Z Reads: 291

```
I'd like to find out more about this project, too!

@vitormhenrique so did you happen to improve the remote with other communication protocol / device other than xbee?
```

---
## \#64 Posted by: JdogAwesome Posted at: 2017-01-14T15:51:34.614Z Reads: 285

```
Definetly a very interesting project, now if I only had a VESC lol. You might want to look into using a ESP8266 module for the wireless communication as well, the normal model has two GPIO's which you could use to communicate with the receiver, but you may need more GPIO's to communicate with the VESC. The ESP8266 ESP-03 has 7 GPIO's so I think that would definitely be enough. This would eliminate the need of having a second microcontroller on the board.
```

---
## \#65 Posted by: Ackmaniac Posted at: 2017-01-14T15:56:22.311Z Reads: 284

```
Only disadvantage with the ESP8266 is that it consumes around 100mah when Wifi is active. No problem for the board side but a bit much for the remotes battery.I recommend to use UDP as communication protocoll. And the Wemos mini D1 is very very nice and small device. Cheap as well.
```

---
## \#66 Posted by: JdogAwesome Posted at: 2017-01-14T17:06:02.007Z Reads: 283

```
Good point @Ackmaniac, I've actually heard it can draw a lot more current, around 500mA so that would suck lol. I think then the HC-05 Bluetooth module would be a better idea because I'm pretty sure it draws far less current.
```

---
## \#67 Posted by: JdogAwesome Posted at: 2017-01-15T01:32:22.607Z Reads: 288

```
Actually I just found [this](http://bbs.espressif.com/viewtopic.php?t=133) article that highlights ESP current draw and it seems like working current would be more around 120mA because it's not like it's going to be transmitting a lot of data. And if you can fit, let's say a 1.5Ah battery in the remote then you would get around 12 hours of battery life, which is pretty good considering an average board only has a battery that would last around an hour.
```

---
## \#68 Posted by: brun Posted at: 2017-02-05T21:32:41.578Z Reads: 281

```
What hardware are you using on the VESC side?  Are you connected via PWM or I2C slave (i.e. the Nunchuck interface)
```

---
## \#69 Posted by: delduked Posted at: 2017-03-05T20:18:17.903Z Reads: 251

```
Has there been anymore progress on this project? I'd like to see if I could get it one to work with the Torque Rocket Dual.
```

---
## \#70 Posted by: massive-attack Posted at: 2017-05-19T11:04:14.289Z Reads: 203

```
This is what jason @EnertionSupport should be doing . Make an upgrade vesrion to the vescx remote . I would buy it in a heart beat . Bet everyone else will to . Like evolve sells an upgraded lcd one for for 120$.
```

---
## \#71 Posted by: lox897 Posted at: 2017-05-19T13:19:01.858Z Reads: 200

```
I'm working on it currently. Search ultimate vesc controller with OLED. Still prototyping though.
```

---
## \#72 Posted by: Fabian287 Posted at: 2017-05-19T13:59:30.037Z Reads: 202

```
ArduBoardControler  by RollingGecko is just my Favorit with  some small changes.
```

---
## \#73 Posted by: Highwon Posted at: 2017-07-07T14:55:26.547Z Reads: 154

```
Is it ready???
```

---
