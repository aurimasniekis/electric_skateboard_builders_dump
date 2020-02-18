# VESC Nunchuk RF

### Replies: 160 Views: 21562

## \#1 Posted by: chaka Posted at: 2015-11-26T13:36:33.814Z Reads: 604

```
There isn't much information on Vedder's nunchuk RF floating around so I think it's time we start a thread dedicated to the project. I made an order with OshPark and plan on documenting the build for everyone to follow.

Hardware: [vedderb/nunchuk_rf_hw
][1]


Firmware: [vedderb/nunchuk_mod
][2]


PCB's on OshPark: [NunchukRF_v51][3]

Tri Wing Screwdriver: [Google search][4]


<img src='/uploads/db1493/original/2X/c/caece645192dbd756e5dbe543b9cf2c6639dce22.png'> 

<img src='/uploads/db1493/original/2X/8/876687caf0a0a0208af2ed85e80d01163c426030.png'>




  [1]: https://github.com/vedderb/nunchuk_rf_hw
  [2]: https://github.com/vedderb/nunchuk_mod
  [3]: https://oshpark.com/shared_projects/GKeNqY7y
  [4]: https://www.google.com/search?q=tri+wing+screwdriver&client=ubuntu&hs=9ZV&channel=fs&biw=939&bih=639&source=lnms&sa=X&ved=0ahUKEwjw7bHbtr3JAhXFLogKHcyaAHwQ_AUIBigA&dpr=1.09
```

---
## \#2 Posted by: kai Posted at: 2015-11-26T13:52:33.596Z Reads: 514

```
So that board replaces the board already inside the nunchuck? I dont get what they are doing exactly. What is the point of this board? Sorry if this is a dumb question.... i just dont understand the project.
```

---
## \#3 Posted by: chaka Posted at: 2015-11-26T13:54:56.645Z Reads: 503

```
This pcb is designed specifically for the vesc so future developments will include an oled display, telemetry readout and other features.
```

---
## \#4 Posted by: monkey32 Posted at: 2015-11-26T14:03:44.952Z Reads: 487

```
Hells yea. This sound sick!!
```

---
## \#5 Posted by: tomtnt Posted at: 2015-11-26T16:22:12.911Z Reads: 479

```
Hi chaka, will you be selling these in the near future?
```

---
## \#6 Posted by: tomtnt Posted at: 2015-11-26T16:23:42.676Z Reads: 464

```
The nyko kama is also hit and miss for some people.  Frequent to intermittent to few random dropouts.  This replace sounds much more robust
```

---
## \#7 Posted by: chaka Posted at: 2015-11-26T17:50:11.007Z Reads: 453

```
Depends if we can get zero drops. Those drop outs are unacceptable. If I do sell them they will be really affordable. Around the same price as a gt2b remote.
```

---
## \#8 Posted by: treenutter Posted at: 2015-11-27T02:49:58.767Z Reads: 446

```
Thanks for sharing this @chaka I've hoped for more info on this development. I've recently (and reluctantly)  given up on my Nyko Kama(s) with VESC. I love the form factor of the nunchuck, and "perpetual steez" is wonderful. But my experience has been that the Kama receiver just isn't durable enough when connected to VESC. Both of mine have had intermittent dropouts after about 15 miles of ride time. It is zero fun to ride fearing that the connection will betray me at a critical moment! I'm hopeful that Vedder's replacement will be an improvement.
```

---
## \#9 Posted by: kai Posted at: 2015-11-27T17:52:21.312Z Reads: 419

```
@chaka do you sell the gt2b in the badwolf enclosure with receiver?
```

---
## \#10 Posted by: chaka Posted at: 2015-11-27T19:05:42.441Z Reads: 430

```
I do but it can be pricey for some. If you want to order a completed BadWolf mod from me it will cost $90.  I use Shapeways for the enclosure and it isn't cheap.
```

---
## \#11 Posted by: chaka Posted at: 2015-11-27T19:18:26.761Z Reads: 440

```
Have some black Nunchuks ordered. Should stay looking nicer longer than white. I am building 3 total for testing on this first round. 

The extra two have been spoken for already. If we get something useful I will consider building more for people who want one.

<img src='/uploads/db1493/original/2X/2/232141d2e6ad4e3a068835b330dddabec0f1e316.jpg'>
```

---
## \#12 Posted by: chaka Posted at: 2015-12-02T14:55:51.224Z Reads: 427

```
Don't forget to order a tri-wing screw driver!

<img src='/uploads/db1493/original/2X/2/2d4884208bb94a485f67905dd1d75fa03fd0fe2c.jpg'>
```

---
## \#13 Posted by: lowGuido Posted at: 2015-12-02T23:56:14.704Z Reads: 411

```
this remote control is it going to be a PPM type output? or something else?
```

---
## \#14 Posted by: torqueboards Posted at: 2015-12-03T01:33:10.216Z Reads: 407

```
Looks great.. Will be awesome once more people test it.

Nyko Kama + receiver itself seems to be the main issue. The 2.4ghz will be an awesome upgrade.

It's cool too since we can actually use Wired Wii Nunchucks for this hack versus Nyko Kama's not being as readily available anymore.
```

---
## \#15 Posted by: abadidea Posted at: 2015-12-03T01:53:42.418Z Reads: 404

```
i'm stoked, hoping you'll add these to your store soon enough chaka :) 

hoping you'll have just the board like vesc and completed with nunchuck
```

---
## \#16 Posted by: kai Posted at: 2015-12-20T13:49:08.174Z Reads: 394

```
so how did the testing go with the nunchucks you built?
```

---
## \#17 Posted by: chaka Posted at: 2015-12-20T16:37:53.735Z Reads: 399

```
I should have the rest of the BOM and stencils this coming week. If all goes well I will post a pre-order thread to get a larger batch going.
```

---
## \#18 Posted by: lox897 Posted at: 2016-01-09T21:42:46.168Z Reads: 401

```
How are you going with them?
```

---
## \#19 Posted by: chaka Posted at: 2016-01-09T22:05:44.105Z Reads: 418

```
I have successfully uploaded the firmware and have a single unit working and just received 9 more pcb's from oshpark this morning. I have been so focused on the VESC project that I have not had as much time as I would like to fully test the nunchuk-mod. I would like to try and design a FHSS pcb for the nunchuk that could utilize the GT2B receiver. FHSS transceivers are much more expensive than the AFH transceivers used by bluetooth style transmitters so it may be more cost effective to just pull components off the GT2B to make this happen.
```

---
## \#20 Posted by: NerijusM Posted at: 2016-01-09T22:35:21.879Z Reads: 417

```
Or you can use FRSKY telemetry system - http://www.hobbyking.com/hobbyking/store/__17205__FrSky_DHT_8ch_DIY_Telemetry_Compatible_Transmitter_Module.html
```

---
## \#21 Posted by: torqueboards Posted at: 2016-01-11T16:53:51.834Z Reads: 392

```
You can always just buy the receiver too. If that's all you need.
```

---
## \#22 Posted by: chaka Posted at: 2016-01-11T17:00:45.061Z Reads: 393

```
The transmitter is what I was referring to. I haven't looked into it to much but inexpensive FHSS transmitter modules are not as easy to come by as AFH.
```

---
## \#23 Posted by: treenutter Posted at: 2016-01-11T17:14:16.950Z Reads: 392

```
@chaka just a thought; It is excellent to consider cost in the design of the controller, but right now the "desired" controller options (full badwolf mod or enertion\carvon's new remote) are selling for $90-$110 usd. If you beat that price point at all for a complete reliable remote it will be a  win!
```

---
## \#24 Posted by: chaka Posted at: 2016-01-11T17:19:20.156Z Reads: 386

```
Looks like all I need is a top quality 3d printer if that is the case. I do like the small form factor of the wired nunchuk though.
```

---
## \#25 Posted by: Blasto Posted at: 2016-01-11T23:24:40.557Z Reads: 381

```
my small contribution for the Vedder nunchuk. Replaces the wire rubber shroud with a 3D printed one that mounts a mini USB, just like if it belongs there.

http://www.thingiverse.com/thing:1261253
```

---
## \#26 Posted by: torqueboards Posted at: 2016-01-23T02:52:35.097Z Reads: 379

```
Great contribution Blasto! That looks awesome.

Chaka have you tested the VESC Nunchuk RF yet? I wonder how well it does too..
```

---
## \#27 Posted by: purplearms Posted at: 2016-01-30T03:52:52.087Z Reads: 383

```
Thanks for the part! I'm going to try and print one on shapeways. What scale is the drawing in? mm?
```

---
## \#28 Posted by: Blasto Posted at: 2016-02-05T17:40:58.832Z Reads: 410

```
Added a little light pipe to the nunchuk, i like the results

<img src="/uploads/db1493/original/2X/5/5deed520361e37da3e852185b2c441c20fe0a3fd.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/7/711d6f394edad525cb00639ffb7fdc2501d6e469.jpeg" width="375" height="500">


Inside

<img src="/uploads/db1493/original/2X/b/b598b6faf2096c771addee39244785a78419f66f.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/2/2e50d990d92475349784a9dc7f22dd7d1c160edf.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/c/c1e26858f81100aec4953ca114fffe239dea15e0.jpeg" width="375" height="500">

Do not put to much hot glue on the back side of the pcb, i was stuck cutting it out with a knife right over all the cables
```

---
## \#29 Posted by: torqueboards Posted at: 2016-02-06T01:31:30.903Z Reads: 396

```
Looks great! Let us know how the connection goes..
```

---
## \#30 Posted by: Justin Posted at: 2016-02-07T11:00:34.716Z Reads: 400

```
This really looks like the perfect controller to me, but how do i get one/make one.
If i order the board from Oshpark, do i only have to wire up the battery and buttons from the Wii Nunchuck,
upload the firmware and its ready to roll? Hope someone can enlighten me or post a quick tutorial!
```

---
## \#31 Posted by: Blasto Posted at: 2016-02-07T12:22:28.607Z Reads: 404

```
I'll eventually post a "what i did" kind of thing. 

But basically 
Get a cheap wired nunchuck
Dismantle it and salvage the casing, buttons and thumbstick 
Order the pcb from osh park
Populate the pcb, your soldering skillz need to be spot on, there's a fancy qfn package with thermal pad
Print this usb shroud http://www.thingiverse.com/thing:1261253
Assemble the whole thing with the new pcb and battery.
Open ubuntu and program the firmware http://vedder.se/forums/viewtopic.php?f=7&t=44

Wire up the nrf transceiver to the vesc
Open the bldc tool, enable the nrf app, put the controller id according to the 4 populated id resistors on the nunchuck pcb

Test the thing out, hold C and Z, red led should on and stay solid.

Voilà.
```

---
## \#32 Posted by: chaka Posted at: 2016-02-07T14:48:21.657Z Reads: 386

```
I can help by providing populated pcb's if anyone needs them. Or maybe a few kits with all the chips and components to solder your own pcb?
```

---
## \#33 Posted by: kfarr Posted at: 2016-02-08T22:23:41.580Z Reads: 386

```
Hello!  

What batteries did you use?  It's a pretty tight fit in there.  They appear to be 3.7 240 mAH, but what dimensions?  

Nice work!
```

---
## \#34 Posted by: Blasto Posted at: 2016-02-08T23:30:53.591Z Reads: 383

```
I got these batteries 

http://m.ebay.com/itm/2PCS-3-7V-240mAh-20C-Lipo-Battery-For-SYMA-S107G-S105G-Helicopter-RC-Quadcopter-/351532196464?txnId=763149322022

I was planning on using only one, but i figured i was going to lose the spare one anyways. I just broke off a spline inside the nunchuck to fit both of them
```

---
## \#35 Posted by: laurnts Posted at: 2016-02-08T23:31:24.665Z Reads: 372

```
FYI for people who doesn't know what it's, it's basically a Nunchuck PCB design & components that is compatible with VESC. Since Nyko Kama is getting rare and the support for other brands are quite limited, Vedder and his friend are building their own version of "Nyko Kama" but only on the electronic side.
```

---
## \#36 Posted by: kfarr Posted at: 2016-02-08T23:34:29.778Z Reads: 364

```
Beautiful!  Thank you!

My board are here, components should be here soon.  For what it's worth, I'm an R2-D2 builder and will be using a pair of these with custom firmware to control my R2 unit.  I set out to make my own board like this (I'm an embedded firmware engineer) but this is just perfect.

Love the open-source community!
```

---
## \#37 Posted by: Justin Posted at: 2016-02-09T11:46:59.939Z Reads: 362

```
And it uses 2.4ghz radiofrequency in stead of bluetooth, so the Nyko Kama drop/signal issues should be fixed with this right?
```

---
## \#38 Posted by: chaka Posted at: 2016-02-09T14:24:41.917Z Reads: 362

```
It uses AFH, adaptive frequency hopping, also called bluetooth. It will have some of the same problems any other AFH controller.

Ideally we would have FHSS for throttle and braking and AFH for telemetry.
```

---
## \#39 Posted by: trbt555 Posted at: 2016-02-09T15:36:36.895Z Reads: 363

```
Personally I don't think the exact modus of transmission plays a great role in safety or reliability in general.
The logic (or lack of) between receiver and (V)ESC is of greater importance.
You could have an uber-reliable connection between transmitter and receiver, and still run run out of battery on your transmitter which -with wonky logic- could cause the board to go full throttle. Most RC receivers have a fail safe setting which makes the output go to neutral (or a pre determined setting) if the TX/RX connection is lost.
Does the Nunchuck RF solution offer this kind of fail safe logic ?
Information about this thing seems to be scattered all over the forums.
```

---
## \#40 Posted by: laurnts Posted at: 2016-02-09T16:15:09.571Z Reads: 366

```
My Ts3t trackstar remote has a fail-safe function build in when signal is lost. I could set it to return to specific value of PWM (1500 for example) when signal has lost. This will loosen the throttle power to the board. I don't know how this technology works, but I assume it sends presignal / prememory up to the receiver module when connection is lost set to 1500.

But from BLDC tool it's self, I believe I've seen also a VESC setting for fail-safe signal lost. This is useful for our Nunchuck remote to add 1 extra layer of security incase suddenly remote goes out of battery / slammed and destroyed due to fall.
```

---
## \#41 Posted by: chaka Posted at: 2016-02-09T16:18:43.930Z Reads: 349

```
@trbt555 It really does play a huge role. 

In simple terms AFH looks for a selective clean signal over a more narrow band. The goal here is getting a crystal clear signal, however, when encountering interference or sudden weakness in signal you can loose throttle/brake control.

FHSS takes the good with the bad with its frequency spectrum, and as far as I am aware not susceptible to dynamic interference like AFH is. The signal is not as clean but more then suitable for pulse modulated signals.

The biggest problem in using AFH for throttle or braking is the possibility of total signal loss due to dynamic interference. Might not be a huge issue at low speed but it can get ugly at 30+mph. If you have any kind of drag brake set it will send you into a fishtail.
```

---
## \#42 Posted by: lox897 Posted at: 2016-02-14T05:00:19.350Z Reads: 337

```
Quick question: You know how the nyko kama comes with a receiver and it's wireless. The corded one doesn't come with a wireless receiver does it? What receiver do we use on the vesc if we buy a corded one? Sorry if I've mis-understood how this works.
```

---
## \#43 Posted by: lowGuido Posted at: 2016-02-14T11:14:45.614Z Reads: 338

```
you dont actually use the wired nunchuck. you gut it and replace the insides with an RF tranmitter.
```

---
## \#44 Posted by: lox897 Posted at: 2016-02-14T19:18:30.948Z Reads: 333

```
And the VESC has a built in receiver?
```

---
## \#45 Posted by: lowGuido Posted at: 2016-02-14T19:26:14.994Z Reads: 328

```

no you have to also wire a receiver to the VESC.
```

---
## \#46 Posted by: lox897 Posted at: 2016-02-14T19:41:47.885Z Reads: 322

```
May I ask which receiver? Is it a NRF24L01?
```

---
## \#47 Posted by: lowGuido Posted at: 2016-02-14T19:42:47.378Z Reads: 329

```
I believe it is an NRF24L01 yes.
```

---
## \#48 Posted by: lox897 Posted at: 2016-02-14T19:46:30.487Z Reads: 335

```
Thanks for the help @lowGuido
```

---
## \#49 Posted by: Blasto Posted at: 2016-02-14T20:38:48.035Z Reads: 355

```
This is the connections from the vesc to the nrf. You need to add a decoupling capacitor on the 3.3v and gnd of the nrf, 2.2uF will do. Dont forget to jump the CE of the nrf to the vcc or 3.3v

Vesc Nrf
Clk. Clk
Mosi. Mosi
Miso. Miso
Ss. Ss
Vcc. 3.3v
Gnd. Gnd
Vcc. CE


Here are the receivers, made 2, one is with the mini nrf, i need to complete it, <img src="/uploads/db1493/original/2X/a/a7cdbe02a14eff70a28898349ca87f1864900164.jpeg" width="666" height="500">
```

---
## \#50 Posted by: purplearms Posted at: 2016-02-15T15:24:30.084Z Reads: 346

```
Thanks for sharing. I know you can get them cheap on ebay, but do you think this one from sparkfun with the antenna and auto retransmit feature would help with the dropped connections?

http://www.sparkfun.com/products/705
http://www.sparkfun.com/products/145
```

---
## \#51 Posted by: Blasto Posted at: 2016-02-15T17:30:32.139Z Reads: 335

```
Worth the try, don't forget that it would go on the receiving end, on the vesc. So i wouldn't put my hopes up on the auto-retransmit feature. But that antenna will be a big help.
```

---
## \#52 Posted by: Ulfberht Posted at: 2016-03-14T08:22:46.884Z Reads: 332

```
Would it be possible to use another Wii compatible nunchuck? 
LIke this one....
http://www.amazon.com/Afterglow-AW-2-Lightchuck-Wii-Blue-Nintendo/dp/B003ITY9XY
```

---
## \#53 Posted by: lowGuido Posted at: 2016-03-14T11:12:39.091Z Reads: 322

```
I dont see why not.

-------------
```

---
## \#54 Posted by: chaka Posted at: 2016-03-14T15:53:33.882Z Reads: 322

```
Finishing another batch of PCB's in the next few days. Anyone waiting on one can expect to see a tracking update as soon as I finish inspection and testing.
```

---
## \#55 Posted by: JohnyK Posted at: 2016-03-18T19:57:44.034Z Reads: 324

```
Hello skate builders,

my first post on forums, but I must say that i'm amazed with the forum.Lots of useful info. I'm also into building e-skate.

now back on topic. Check these cheap bluetooth controllers out:
http://www.aliexpress.com/item/New-Bluetooth-Remote-Control-Wireless-Selfie-Shutter-Game-Console-Gamepad-Joystick-Game-Controller-for-Android-Smartphone/32467870580.html
even smaller one: 
http://www.aliexpress.com/item/Wireless-Bluetooth-Game-Controller-Joystick-Gaming-Gamepad-for-Android-IOS-Moblie-Smart-Phone-for-iPhone-for/32565129038.html

the smaller one has arrived and is reaaally small and the joystick has small travel. waiting for the big one. it should be same as wii.
```

---
## \#56 Posted by: Michaelinvegas Posted at: 2016-03-18T22:00:40.743Z Reads: 317

```
Yes endless sphere sucks
```

---
## \#57 Posted by: monkey32 Posted at: 2016-03-19T10:15:00.643Z Reads: 315

```
Ease up there buddy. Endless doent suck. Endless sphere was the original forum where Onloop - the guy hosting this forum, started building and sharing how to build. There is still a $hit ton of information there- both in archives and currently being built. This forum does have better organization and is much more specific to e-skate but in terms of controler tech, batteries, and development across the spectrum of EV endless is unbelievable.
```

---
## \#58 Posted by: Michaelinvegas Posted at: 2016-03-19T11:35:32.715Z Reads: 311

```
You ease up buddy.... Didn't know there was and endless - cheerleader .... Thanks for the non needed lesson on what it is.... Fully aware kid
```

---
## \#59 Posted by: chaka Posted at: 2016-03-19T14:41:55.976Z Reads: 320

```
 Vegas sucks too, all the fancy lights just hide the piece of crap it really is but you don't hear any of us randomly spouting off like we have a case of mild turrets ;)

This is the type of attitude I commonly see on the sphere from a few bad actors. It is very counterproductive and I hope it will be moderated by the community as a whole over here. If you can't help yourself then at least do this in an appropriate thread and leave the technical threads alone.
```

---
## \#60 Posted by: Michaelinvegas Posted at: 2016-03-19T15:08:39.233Z Reads: 324

```
How did Vegas get involved and who has turrets? .... Only one comment abt end less.... ... No more abt this
```

---
## \#61 Posted by: Ulfberht Posted at: 2016-03-26T23:52:19.909Z Reads: 313

```
I'm rollin in a little late to the party, but I'd like to know if there are any more PCBs available! Sounds like a pretty cool upgrade to play around with.
```

---
## \#62 Posted by: jacobbloy Posted at: 2016-04-13T18:53:17.055Z Reads: 333

```
hey mate why have i never seem this usb mount of yours? your a ledge me and vedder have been making some design changes for the nunchuk rf remote i have done a batch with jason with imbedded nrf24lo1+ chips as the cheap nrf modules are half of the drop out issues but sadly that run didn't work!
so iv since made some design modifications and yet to test them as i don't have the money for new pcbs to be made maybe i can send the designs to @chaka for testing (The problem was the RF antenna is so hard to get right).<img src="/uploads/db1493/original/2X/d/da680025b8963fe260b0e108066c9ac373cba4e6.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/9/94b80aea54fbc199022b24a90845db8573fffa2b.jpg" width="375" height="500">

But iv been working on modifying the nunchuk_mod firmware to then allow a uart connection so you can plug in a BLE module instead to work with the same receiver as my iOS/android app

watch the video till the end or scroll through and you will find!
https://youtu.be/N98Oqr0WRG0
```

---
## \#63 Posted by: chaka Posted at: 2016-04-13T19:43:32.184Z Reads: 308

```
@jacobbloy I can do a small run, let me know ;)
```

---
## \#64 Posted by: Blasto Posted at: 2016-04-13T21:51:23.334Z Reads: 310

```
If you have the gerbers with a nrf24lo1+ chipintergrated i'll gladly test it out

I already have this for the receiver end 

https://www.sparkfun.com/products/691
```

---
## \#65 Posted by: jacobbloy Posted at: 2016-04-14T00:58:13.860Z Reads: 310

```
Yea cool! At one point I was using https://www.sparkfun.com/products/705
With a 5dbi antenna on both RX and TX I could go a good 300meters away!

If you don't mind soldering 3 wires on to your pcb I can also send you the code for the Uart connection
Then u can use the HC-05 modules that you have or the HM-10 modules when you get them
```

---
## \#66 Posted by: Blasto Posted at: 2016-04-14T01:08:40.821Z Reads: 305

```
3 little barnacles never hurt anyone, pretty sure I can pull that off

Edit: sorry I think I misunderstood, on which pcb? nunchuckRF V5,1?
```

---
## \#67 Posted by: jacobbloy Posted at: 2016-04-14T01:09:59.487Z Reads: 305

```
Sorry 4<img src="/uploads/db1493/original/2X/4/4ec8ff5dd9696353c720877f2371c326de01806b.jpeg" width="374" height="500">
```

---
## \#68 Posted by: Blasto Posted at: 2016-04-14T01:11:36.220Z Reads: 297

```
Ah gotcha, I have two blanks left. I'll build a new one
```

---
## \#69 Posted by: jacobbloy Posted at: 2016-04-14T01:11:45.259Z Reads: 308

```
<img src="/uploads/db1493/original/2X/e/eb2dfdd3dd95eafb5b46ad4fc2e75be0f7093783.jpeg" width="375" height="500">

On this board I moved the VCC and GRD as they short in that location, you do not actually have to remove the nrf module.
```

---
## \#70 Posted by: Blasto Posted at: 2016-04-14T01:31:35.172Z Reads: 311

```
[quote="jacobbloy, post:69, topic:588"]
On this board I moved the VCC and GRD as they short in that location, you do not actually have to remove the nrf module.
[/quote]

is that an earlier version of the nunchuck RF, V5.0?? The brown wire is in the way. 

this is what I have
<img src="/uploads/db1493/original/2X/c/cb0ef557f1debb76784504960160688a38b93e91.jpeg" width="375" height="500">
```

---
## \#71 Posted by: jacobbloy Posted at: 2016-04-14T02:10:35.436Z Reads: 301

```
The first one is the same as your version, the second image is the pcb with inbeeded nrf chip.
```

---
## \#72 Posted by: Sk8on Posted at: 2016-05-16T21:29:11.989Z Reads: 300

```
Dear Community,

I am recently finishing my eboard and got aware of the nunchuck control unit. Is someone of you still selling some Nunchuck PCBs for a shipment to Germany? A price information would also be handy. 

I would be glad to get my hands on 1 or 2. 

yours Sk8on
```

---
## \#73 Posted by: fertito Posted at: 2016-06-03T12:18:19.825Z Reads: 290

```
Hello everyone,
is there a way to have one of these pcb?
I'm trying to make the code to work with a stm32f103 board of mine (which is basically the same chip than the stm32f100 with more features), I plugged a nrf24l01, some buttons, ... compiled the code for my chip model, flashed it, and it seems to work. I can see spi signal on every lines (including miso), but I can't make it to talk with the VESC, despite I can also see that there is som data on spi lines, the leds are not indicating anything...
I'm using hardcoded address : 05.
The deep low power feature make it very difficult to debug, could you tell me where to disable it in chibios?
the same goes for VESC, the debugger is loosing connection very soon, so I can't see if there is some data received, 
Thank you very much for any help.
Roman
```

---
## \#74 Posted by: jacobbloy Posted at: 2016-06-04T06:25:57.137Z Reads: 272

```
I do have some very old code that works with the 103 chip but it's not up to date ill see what I can do!
```

---
## \#75 Posted by: fertito Posted at: 2016-06-04T07:18:07.627Z Reads: 281

```
Hello Jacob, thank you very much.
Normally à f100 code is working out if the box on a f103, I did it several time.
The main difference between these two chip is the USB on the f103.
I'll try to get m'y hand on a f100 and on some pcb, do you still have some?
Thanks again.
```

---
## \#76 Posted by: fertito Posted at: 2016-06-08T11:43:33.950Z Reads: 284

```
Hello there,
my nrf module was not working, I changed them and now it is working nicely.
I confirm that the STM32F100 code is working flawlessly on a STM32F103.
I ordered some pcb at seeedstudio, I'll give some if someone is interrested.
```

---
## \#77 Posted by: hexakopter Posted at: 2016-06-10T20:26:56.435Z Reads: 294

```
Also had a problem with not working NRF modules. Don't use the ones with the NRF package into this black dot of glue. (Don't know how to describe them)

Here a picture of my nunchuk if anybody is interested.
<img src="/uploads/db1493/original/2X/d/dee908f214126b090a1ee9b08593d703ab175f8e.jpg" width="375" height="500">
```

---
## \#78 Posted by: fertito Posted at: 2016-06-13T14:03:44.656Z Reads: 285

```
There is a reason why they put a drop of black glue on the chip... my guess is that is is not a nrf24L01 but a substitute without all of the functionality...

here is some other nice things to read : http://hackaday.com/2015/02/23/nordic-nrf24l01-real-vs-fake/
```

---
## \#79 Posted by: hexakopter Posted at: 2016-06-13T20:18:26.818Z Reads: 293

```
It looks like they are using SE8R01 instead of NRF24L01. Same pinout on the module, but a little different protocol. This should be the problem why they are not working.
```

---
## \#80 Posted by: hexakopter Posted at: 2016-06-14T12:54:33.235Z Reads: 307

```
Is the reverse function with the z-button working by someone? I am on V2.18 right now and when enabling "Current with reverse" in the nunchuk tab that is not changing anything. Pushing the z-Button has no effect. Now I want to know if that is normal or something with my hardware/software is wrong.
```

---
## \#81 Posted by: mishrasubhransu Posted at: 2016-06-24T18:28:44.188Z Reads: 325

```
Does anyone have an assembled board that I can buy?
```

---
## \#82 Posted by: hexakopter Posted at: 2016-06-24T19:12:22.886Z Reads: 328

```
Maybe I should talk about it here also.
[http://vedder.se/forums/viewtopic.php?f=6&t=248](http://vedder.se/forums/viewtopic.php?f=6&t=248)

Long story short: On wednesday I had trouble with the VESC Nunchuk RF. It was like a normal skateboard run, but abruptly the nunchuk was not working anymore. All stick inputs don't affected anything on the VESC and it was driving with full speed without a chance to stop it. Not just that I wasn't able to stop with the motor the VESC was spinning the motor like on full throttle. The last attempt to stop it with sitting down failed and the board throw me of on 52kmh (around 32mph). Not a good feeling at all.
Fortunately I was wearing a helmet, but that doesn't protect the rest of the body... :disappointed_relieved:
```

---
## \#83 Posted by: philipp Posted at: 2016-06-26T07:49:29.730Z Reads: 318

```
[quote="hexakopter, post:82, topic:588"]
but that doesn't protect the rest of the body
[/quote]
 Pics or it didn't happen!
```

---
## \#84 Posted by: hexakopter Posted at: 2016-06-26T10:38:08.005Z Reads: 313

```
<img src="/uploads/db1493/original/2X/0/0dd844ef6d34d63b5675cfccccb593c60f958b1d.PNG" width="533" height="500">
```

---
## \#85 Posted by: torqueboards Posted at: 2016-06-26T10:55:47.182Z Reads: 319

```
@hexakopter. That's when you gotta do a flip the deck trick or crash. lol

<img src="/uploads/db1493/original/2X/1/17a409a679ca6d54e488078a40b5e7492a5fbb02.png" width="225" height="224">
```

---
## \#86 Posted by: Sk8on Posted at: 2016-10-12T12:59:39.636Z Reads: 252

```
Dear Skaters!

I am still searching for a working pcb for the wii Nunchuck. I did something wrong soldering the chip i think. Is there someone who is having some left over? I will buy it then for a shipment to Germany. Would be perfect, thanks!
```

---
## \#87 Posted by: rpn314 Posted at: 2016-10-12T13:34:18.708Z Reads: 240

```
I can have one by the end of the week if you want. I have 2 extra blank PCBs, I'd just have to order a few of the components I'm missing and solder them together.

Edit: It looks like a few of the components I don't have are on backorder at Mouser and won't be in stock for another month or two, so I may have to rescind that offer. Sorry.
```

---
## \#88 Posted by: faithfulpuppy Posted at: 2017-02-17T13:47:35.971Z Reads: 211

```
is anyone still making these?
```

---
## \#89 Posted by: rpn314 Posted at: 2017-02-18T19:09:03.106Z Reads: 213

```
I've the PCBs and it looks like the parts are all in stock on mouser. If you're interested I can look into timing and cost a bit more.
```

---
## \#90 Posted by: Bender Posted at: 2017-02-18T21:21:32.981Z Reads: 212

```
I'd be interested in one if your going to make a few
```

---
## \#91 Posted by: deepsilence Posted at: 2017-02-19T01:41:14.615Z Reads: 210

```
I'd also be interested in one. Maybe two, but definitely one.
```

---
## \#92 Posted by: rpn314 Posted at: 2017-02-19T02:47:40.582Z Reads: 204

```
@Bender and @deepsilence are you guys looking for the full nunchuck or just a finished (assembled/soldered/programmed) PCB?
```

---
## \#93 Posted by: Bender Posted at: 2017-02-19T04:13:17.015Z Reads: 203

```
I good with the finished PCB.
But I'd take either, whatever is easier for you.
I'd even take 2 if you had em.
```

---
## \#94 Posted by: rpn314 Posted at: 2017-02-19T06:04:00.169Z Reads: 206

```
Well I'm happy to do as much or as little as you'd like.
What I have currently (just checked): 
- 1 Blank PCB
- most of the discrete components
- 2 small li-po batteries (they came in a 3-pack and I used 1 in mine)
- Female micro-USB connectors (I used micro instead of mini)
- Ability and tools to make them

What I'd need to have a finished PCB
- A few of the components, like the processor and LEDs, that I don't have
- the RF Transmitter

What I'd need to get after that to have a fully working unit
- Nunchuck shell (with the joystick and C-Z buttons)

So at a minimum I'd probably need a week and a half to get the 1 PCB I have up and running (order the parts, assemble, etc). If there's enough demand, I can certainly order more of everything, including more PCBs from oshpark, then assemble, test, and get them to those who'd like one. I love mine :)
```

---
## \#95 Posted by: deepsilence Posted at: 2017-02-19T11:59:22.405Z Reads: 191

```
Just as Bender, I'd be good with just the PCB.
I already have some nunchucks laying around. Besides, as much as I appreciate your help, I wouldn't want you to do all the fun ;) 

I'm currently building my second board but wont have it ready for another two or three months, so I'm not really in a hurry. So if you're planning on ordering more PCBs and do a small run or something I could definitely wait for that.
```

---
## \#96 Posted by: boards Posted at: 2017-02-19T16:57:35.852Z Reads: 191

```
I just ordered 3 pcbs and at least 3 copies of every part. 

I'll probably sell 1-2 kits when everything arrives.
```

---
## \#97 Posted by: Bender Posted at: 2017-02-19T21:10:49.832Z Reads: 187

```
could you give us a price for both options
Thanks for doing this!

Are you using the Bluetooth version like Jacob's?
```

---
## \#98 Posted by: hexakopter Posted at: 2017-02-19T23:31:12.398Z Reads: 187

```
Maybe that would be interesting for you also. Benjamin says on his forum:

> The beta VESC also has an NRF and antenna, and we are trying to make a kit for the nunchuk as well that you can assemble yourself soon.

http://vedder.se/forums/viewtopic.php?f=6&t=590

So it looks like there is a kit coming from the "right" source someday and when I am not mistaken the NRF IC will also be soldered on the PCB directly, so you can use an original NRF IC and not the cheap ones on the china modules.
```

---
## \#99 Posted by: rpn314 Posted at: 2017-02-20T18:06:20.710Z Reads: 183

```
I just have the standard ones (I used the OshPark link at the top of this thread). To my understanding Jacob's nunchuckRF w/ bluetooth has pretty much died. If you can find the hardware and firmware files somewhere, I'd be happy to work on it (I'd love to make myself one as well!), but I couldn't find much more than a few pictures and upset people.

For a finished PCB (major soldering done) I could do a small run for about $25+shipping. If more people want them (larger run), I could probably get it down closer to $20
You would just need to get and attach (solder) a battery, USB, the C-Z buttons, and the joystick and then put it in the shell.

Edit: I can't seem to find a US reseller for the NRF24L01+ module, which means I'd have to get it from China so it'd be a few weeks out.
```

---
## \#100 Posted by: Bender Posted at: 2017-02-20T20:39:28.659Z Reads: 179

```
That sounds reasonable to me.
What would you want for a finished nunchuck?
And what type of reciever do we need?
```

---
## \#101 Posted by: rpn314 Posted at: 2017-02-20T22:30:43.799Z Reads: 172

```
For a full unit it would be closer to $40, most of which goes for a new/gently used Nunchuck.

[quote="Bender, post:100, topic:588"]
And what type of reciever do we need?
[/quote]

To plug into the VESC? I used [one of these](http://www.ebay.com/itm/NRF24L01-PA-LNA-SMA-Antenna-Wireless-Transceiver-Communication-Arduino-US-Seller-/172051152184?hash=item280f0c3d38:g:JnIAAOSwFqJWixLf), however you can you a smaller one (without an antenna and amplifier).
```

---
## \#102 Posted by: deepsilence Posted at: 2017-02-21T08:29:20.569Z Reads: 172

```
When (if) you decide to do a run please let me know. I already have everything else I need to complete the controller and to connect it on the VESC side, just missing the PCB.
```

---
## \#103 Posted by: boards Posted at: 2017-03-03T17:54:31.539Z Reads: 174

```
Got my 3 copies of everything, assembled one last night, lost a mosfet. Everything seems good but I can't get it to recognize the uart chip :/ Reflowed it a few times at 250c, even tried one of the other chips. Verified all the resistors etc are not shorted / ok too.
```

---
## \#104 Posted by: natn0 Posted at: 2017-04-24T20:42:50.903Z Reads: 157

```
Hey that's awesome! What light pipe did you use?
```

---
## \#105 Posted by: boards Posted at: 2017-04-26T01:17:40.197Z Reads: 156

```
Been using this for some time now. Can't see why anybody would use another remote (minus maybe a screen). You don't need to turn it on, with the stick from an legit nunchuck it's so smooth, no dropouts, plus you can connect the nunchuck to bldc tool and view info from your VESCs.

Highly recommend people to make these.
```

---
## \#106 Posted by: rpn314 Posted at: 2017-04-26T13:41:30.272Z Reads: 164

```
I asked him the same thing :)

[quote="Blasto, full:true"]
I just drilled a 1/8" hole and pushed this guy in

http://www.digikey.com/product-detail/en/51513010125F/350-3721-ND

I tried to align it withe the middle led, the other are visible through it also
[/quote]

@boards Can you elaborate on this? I wasn't aware the BLDC Tool could connect directly to the nunchuck. 
[quote="boards, post:105, topic:588"]
plus you can connect the nunchuck to bldc tool and view info from your VESCs.
[/quote]
```

---
## \#107 Posted by: boards Posted at: 2017-04-26T14:41:29.314Z Reads: 162

```
Plug it in via the usb, go to bldc tool and connect to the new serial interface. The terminal and data views work, but configuration does not.
```

---
## \#108 Posted by: rpn314 Posted at: 2017-04-27T18:39:44.625Z Reads: 162

```
[quote="boards, post:107, topic:588, full:true"]
Plug it in via the usb, go to bldc tool and connect to the new serial interface. The terminal and data views work, but configuration does not.
[/quote]

When I connect it says "Connected" in the corner for a second, but then it just says, "No Firmware Read Response" and disconnects again. What am I missing?
```

---
## \#109 Posted by: boards Posted at: 2017-04-27T19:53:20.585Z Reads: 148

```
Make sure the VESCS are on and that the remote can connect normally.
```

---
## \#110 Posted by: Nordle Posted at: 2017-04-27T19:57:54.703Z Reads: 149

```
Some one selling these?
```

---
## \#111 Posted by: rpn314 Posted at: 2017-04-27T23:05:44.958Z Reads: 151

```
[quote="boards, post:109, topic:588, full:true"]
Make sure the VESCS are on and that the remote can connect normally.
[/quote]

Oh got it. I misunderstood what you meant by connecting the nunchuck to bldc tool.
```

---
## \#112 Posted by: natn0 Posted at: 2017-04-28T00:51:37.058Z Reads: 149

```
Maybe later, I've bought enough parts to make 3 but I'm probably only going to keep one. But first I've got to build them and do some testing with different transceivers so this is maybe a few weeks or months away.
```

---
## \#113 Posted by: rpn314 Posted at: 2017-04-28T01:19:25.661Z Reads: 151

```
[quote="Nordle, post:110, topic:588, full:true"]
Some one selling these?
[/quote]

I can put one together for you. I posted a few posts up about it.

[quote="natn0, post:112, topic:588"]
do some testing with different transceivers
[/quote]
Are you testing a new nunchuck or the original one that vedder made (which started this thread)?
```

---
## \#114 Posted by: Nordle Posted at: 2017-04-28T05:15:07.202Z Reads: 143

```
Nice, pm me pls i'll take one!
```

---
## \#115 Posted by: natn0 Posted at: 2017-04-28T18:13:19.506Z Reads: 147

```
[quote="rpn314, post:113, topic:588"]
Are you testing a new nunchuck or the original one that vedder made (which started this thread)?
[/quote]

No it's Vedder's. The one mentioned in this thread with different transceiver modules (at both ends) and one with the nRF24L01 directly on the PCB is also in the works.

The goal is to find completely reliable setups as some people have been having problems with drop-outs.
How has yours worked in this regard?
```

---
## \#116 Posted by: rpn314 Posted at: 2017-04-28T18:52:48.804Z Reads: 148

```
Until lately I've had very good luck with the mini module on the PCB in the nunchuck and the long range module (with the external antenna) on the vesc side. 2 weeks ago I think my receiver module got fried. It cut out and I haven't been able to get it to connect again (2 weeks later...so not just an intermittent signal drop).
```

---
## \#117 Posted by: boards Posted at: 2017-04-28T21:10:10.435Z Reads: 149

```
I've found the non antenna module sensitive to placement. Right above the vescs results in very poor range but if you move it even a few inches away from the motor wires and vescs it's great.
```

---
## \#118 Posted by: TeleRando Posted at: 2017-04-28T22:15:26.384Z Reads: 145

```
I'm about to build a couple of these but I'm unsure about how to upload the firmware. Can anyone with experience chime in and write up a basic how-to?
```

---
## \#119 Posted by: rpn314 Posted at: 2017-04-29T03:59:30.984Z Reads: 149

```
I have done quite a few now. In my experience, Ubuntu is the only real option. I know the program he (vedder) uses to flash the firmware (it's called stm32flash) works on Windows, but there's a bunch of other dependencies that I only really know how to do on ubuntu. I basically just  follow the instructions outlined by vedder for his speed controller (http://vedder.se/2015/01/vesc-open-source-esc/ starting at "Software Installation and Configuration Tutorial") combined with some posts on his forum (http://vedder.se/forums/viewtopic.php?f=7&t=44&sid=a0a9ad1a784307f48f455fd389b84a2c).

After getting all of those dependencies in place, the basics of it is you download the firmware (https://github.com/vedderb/nunchuk_mod) and stm32flash (https://sourceforge.net/projects/stm32flash/), unpack stm32flash, then unpack the firmware package into a folder in the stm32flash folder. Then you open terminal, cd to that nunchuck directory, and run "make upload"

It's tough to remember exactly what all I did, so I'll have to go through with a fresh copy of ubuntu and make a video. Probably won't have time this weekend, but I probably can next week sometime.
```

---
## \#120 Posted by: TeleRando Posted at: 2017-05-12T16:07:20.265Z Reads: 140

```
A video would be fantastic if you have the time. I know I would really appreciate the effort and I'm sure others would as well. I was away from home for a few weeks... I'll be starting the assembly of my NRF Nunchuck today.
```

---
## \#121 Posted by: TeleRando Posted at: 2017-05-13T23:28:19.416Z Reads: 146

```
I made a thing...

<img src="/uploads/db1493/original/3X/1/f/1faf1e21fcb201d5c0536c2bff20f08707e4c6cc.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/5/058c989117722793e22eb10c55ac78ee1962f769.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/f/ef3751245ef504dd1e650c4c4df4e8aa5a96916f.jpg" width="666" height="500">
```

---
## \#122 Posted by: Sander Posted at: 2017-05-14T16:44:48.199Z Reads: 137

```
What is the range you get?
```

---
## \#123 Posted by: TeleRando Posted at: 2017-05-14T19:08:57.582Z Reads: 136

```
I haven't finished it yet. I have a generic Wii nunchuck on its way to me now. I should have it assembled by the end of the week.
```

---
## \#124 Posted by: Sander Posted at: 2017-05-14T20:07:03.945Z Reads: 134

```
Well not to be rude the ranges you get from the nrf smd's are terrible... Atleast for me. Thats why I asked what range you get? But there is a simple solution another nrf smd with the long range edition, in built antenna with PA and LNA. I have not tested it yet but I will confirm it in the end of the next month.
```

---
## \#125 Posted by: TeleRando Posted at: 2017-05-14T20:10:21.939Z Reads: 133

```
Well I still have two unpopulated boards so maybe I'll give that a try too. Do you know of a source for the long-range smd NRF?
```

---
## \#126 Posted by: Sander Posted at: 2017-05-14T21:36:22.852Z Reads: 134

```
Well I havent recieved it yet and not confirmed it works.
But here is the link:
https://www.aliexpress.com/item/Free-Shipping-SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in/2022127731.html?spm=2114.40010508.4.27.OGF00a
```

---
## \#127 Posted by: Quezacotl Posted at: 2017-06-20T07:52:11.460Z Reads: 131

```
Hello!
I just built this NunchukRF 5.1. I have had problems. And i need some clarifications if someone can answer.

When i upload the code, (make upload) that's pulled from git, it goes ok. But then it is all dead.
It starts to work after i have "activated" it by connecting to Windows machine or by pressing "connect" on BLDC Tool. Even then it can't connect to VESC.

Another scenario; everything the same except i upload this mystery code that i found on this german site: http://www.elektro-skateboard.de/forum/eigenbauten-95/nunchuk-rf-5092.php and it actually connects to VESC and functions ok.

It would be alright with this solution, but it deactivates randomly, or when i disconnect(desolder) the battery. Sometimes middle of a ride, or when i let it be after a long ride. I have confirmed that the issue is not the battery. Then it works happily again when i do the activation with computer. But sadly i don't have a computer with me when i ride...

This is my second nunchuk, and it functions exactly the same. The previous got kinda broken, because i shorted the regulator and a battery trace burned. I replaced the regulator and all seem to work, it uploads the code without problems. But instead of red light flashing the green is flashing. And obviously it doesn't connect to VESC.

So... What are your experiences with this? Do you need to activate the nunchuk? What does the green LED mean?

My VESC PCB is 4.12 and firmware 2.18.
```

---
## \#128 Posted by: The_Dude Posted at: 2017-06-20T08:03:42.576Z Reads: 122

```
Where did you get your NRF modules from, China? As far as I remember I also had some weird behaviour. Then I  bought 6 (or more) of the modules and tried until git one which worked fine. The mystery code you found on the elektro-skateboard forum is fine - think there is only error in the LED red/green activation corrected.
```

---
## \#129 Posted by: Quezacotl Posted at: 2017-06-20T08:45:57.847Z Reads: 119

```
Yea, China, through eBay. Those original looking, not blob. And chip says nrf24l01+. But how the NRF modules could affect to this mysterious activation i need to perform?
Anyhow, i just ordered more of those.

While you have a fully functional nunchuk, do you need to activate it the same way i do?
And can you get the original code to work?

Funny, while i'm using the mystery code or the original, all the LED behavior is the same. The pairing is flashing red until solid when it connects.

I need facts, so i don't need to chase unexisting things.
```

---
## \#130 Posted by: trampa Posted at: 2017-06-20T10:01:11.240Z Reads: 123

```
The cheap china ones do not really work. There is a lot of luck involved if you get one working fine straight away.
Benjamin also bought some china clones and they are all in the bin. Just not reliable!

Frank
```

---
## \#131 Posted by: The_Dude Posted at: 2017-06-20T10:35:14.441Z Reads: 125

```
Yep, both codes work fine for me. You can check the differences by comparing the sources. My initial problems where
1. related VESC 4.7, so not of interest for you
2. bad quality nrf24l01 modules - this is not visible from the outside so you just have to try

Setup process:
1. upload the firmware
2. activate nrf in BLDC tool, make sure you set the address correctly, depending on the resistors (binäry coded, 1111 hex = 16 dec) you soldered on the pcb
3. establish connection by pressing c+z button

Don't know everything about the meaning of the LED's is, but what I I know so far is:
- blue LED is used for charging, when the battery is fully charged it blinks slowly
- while connecting, the green LED is blinking, after connecting it's on (in your case ist might be the red since it is assigned not correctly in the original source)
```

---
## \#132 Posted by: rpn314 Posted at: 2017-06-20T11:01:43.929Z Reads: 118

```
I'm not sure what this "activate nunchuk" or deactivate process you're referring to.
```

---
## \#133 Posted by: Maxid Posted at: 2017-06-20T11:23:55.996Z Reads: 121

```
is there a reputable source for the nrf modules in Germany?
```

---
## \#134 Posted by: Quezacotl Posted at: 2017-06-20T11:58:25.823Z Reads: 117

```
Rpn314: The activating i'm referring is that when there is no power, and i connect the battery, it is still dead, no c+z are working until i connect it to computer. I need to awake the nunchuk with Windows, bldc tool or maybe anything that tries to talk to the nunchuk, except the programming application.

The_Dude, there is no source code for the mystery firmware unfortunately. It would have to be asked from the person who posted it.

Seems that i need to try and see if the nunchuk awakens without computer, when i desolder the NRF module. That's all i can think of.
```

---
## \#135 Posted by: The_Dude Posted at: 2017-06-20T12:25:41.279Z Reads: 119

```
[quote="Quezacotl, post:134, topic:588"]
Rpn314: The activating i'm referring is that when there is no power, and i connect the battery, it is still dead, no c+z are working until i connect it to computer. I need to awake the nunchuk with Windows, bldc tool or maybe anything that tries to talk to the nunchuk, except the programming application.
[/quote]

OK, this is definitely NOT how it is supposed to be!
```

---
## \#136 Posted by: The_Dude Posted at: 2017-06-20T12:39:28.552Z Reads: 121

```
Puhh, as I said I ordered a whole bunch and tested them. Maybe Farnell, Mouser, ...
I would just check where they come from and ignore the offers from China :smirk:
```

---
## \#137 Posted by: The_Dude Posted at: 2017-06-20T12:41:06.726Z Reads: 122

```
If you want I can put the complete files including the compiled firmware and the makefile with the command for uploading the firmware on the pcb on my dropbox.
```

---
## \#138 Posted by: Quezacotl Posted at: 2017-06-20T12:54:52.278Z Reads: 120

```
That would be great. Then i would see what is the difference between those firmwares.
```

---
## \#139 Posted by: The_Dude Posted at: 2017-06-20T18:50:42.861Z Reads: 121

```
Here you will find the sources:
[https://www.dropbox.com/sh/5rwq2u1h83tnqbc/AABitDwG0UPnjqippgnFCq-Sa?dl=0](https://www.dropbox.com/sh/5rwq2u1h83tnqbc/AABitDwG0UPnjqippgnFCq-Sa?dl=0)
```

---
## \#140 Posted by: Quezacotl Posted at: 2017-06-20T21:05:15.706Z Reads: 127

```
I desoldered the NRF module, but my problem still persists, i need to "activate" the nunchuk. So it is not related to NRF module any way.
Next thing that i can think of is that if i have some wrong component on board. Something that is related to stm chip booting. I'm using the right BOM, V5.

And i quickly tried that source you posted, it is different than what i found, since it behaves like you said, red and green is swapped. But i need to look more into it.
```

---
## \#141 Posted by: The_Dude Posted at: 2017-06-20T21:14:50.813Z Reads: 128

```
Maybe your "activation" thought was misleading, when searching for the error. When you connect to a usb-port you also switch to a different power source ... namely your computer! I would really take a closer look to U3 and U4. Is one of them getting hot, you did not swap them accidentally, are the "looking" all right?
```

---
## \#142 Posted by: Quezacotl Posted at: 2017-06-20T21:38:36.082Z Reads: 132

```
I just checked them again, and they are the right way. And also smd markings match what they should be. They are not heating. And they look alright.
Power sources are the right way. When i plug USB, the blue LED lights. And the markings are all clear where the battery goes and where USB.

What else i could call it than activation. software power switch triggered by data? :slight_smile: 

When i look at the schematic, it looks that only thing that could be causing this problem would be the USB-bridge. Counterfeight chip with some pins swapped or something... that forces the nunchuk to be in some specific mode on boot... But that doesn't explain why the original code doesn't work and that ws2812 edition works.
But i can test that option by desoldering the USB-bridge off.

EDIT: Yeah! The booting problem(aka. activating) is solved!
I desoldered the CP2102 from the other nunchuk that i thought was broken. I applied power, and i needed to pair it only once, and whenever i connect the battery(actually lab power supply), it is automatically paired! So apparently now it works normal way. Except i can't connect it to computer obviously...

Only two questions remain now... Will the original firmware work now, and were the problem counterfeit CP2102, or just bad soldering.
The soldering appeared to be ok, but i need to wire the chip with thin enameled wire to the pcb so it is 100% every needed pad soldered.
```

---
## \#143 Posted by: The_Dude Posted at: 2017-06-21T05:26:32.540Z Reads: 120

```
Original firmware works too, just red and green switched. You used a heat gun to solder the grounding underneath the CP2102? If not, you can not connect as you already have experienced. 
Why do you have to use a wire??? Give me a photo!
```

---
## \#144 Posted by: Quezacotl Posted at: 2017-06-21T06:46:43.934Z Reads: 126

```
I soldered it the same way i solder all of the same kind of packages. pre-tinning, flux and heat gun. Including the ground plane.
Wires this time just to make sure all the pads are connected. To confirm if the chip(s) are fake or just bad soldering.
```

---
## \#145 Posted by: The_Dude Posted at: 2017-06-21T06:57:10.331Z Reads: 132

```
I also had some problems regarding the proper connection of the CP2102, since there are no visible pins, just some sort of corners underneath. After using the heat gun I re-soldered every "pin" with a very fine tin solder and a very, very fine solder tip. After that I had no more problems, connection was good and so far reliable.
```

---
## \#146 Posted by: Quezacotl Posted at: 2017-06-21T07:42:09.288Z Reads: 138

```
Okay, i tested with wires. Exactly the same behavior as before. So the chips are either counterfeit of partially broken.
Here's some pictures.

IC removed, device working perfectly:
<img src="/uploads/db1493/original/3X/9/5/9583451d3bfc0502d144d44ff052cf90730b94c6.jpg" width="666" height="500">
IC soldered with wires: (ground looks bad on picture. it's not)
<img src="/uploads/db1493/original/3X/b/c/bc2f2d6452b191fabab19ab94529c436c4d2d859.jpg" width="375" height="500">

EDIT: So far it is working good.
Now i have another problem, longboard battery died, i need to wait for new batteries to arrive. The current cells are already bad, used for testing purposes, to be replaced with better ones. But that's another story.

But about the CP2102. What i have read on internet, the problem may be related to RTS and DTR pins. What i'll try, is to control those two pins with switches and see what happens.
EDIT: Okay. When i disconnect the RTS signal, it starts working. So i need just one switch for RTS.

EDIT: The original firmware is still not working...
```

---
## \#147 Posted by: hexakopter Posted at: 2017-06-22T22:24:02.814Z Reads: 126

```
Are you compiling the newest version from Benjamins github? I think he has changed some pieces in the software (using STM32s ID) in his last commit.
I would try the software before that last commit. Maybe that will work for you.
```

---
## \#148 Posted by: Quezacotl Posted at: 2017-06-23T15:17:49.184Z Reads: 125

```
Yea, newest from github.
Now i had the time to compare those sources. The difference (most likely) why they are not working straight away is that some values on rf.c are different and need to be changed on BLDC Tool.
Newest --- other version:
NRF_RETR_DELAY_1000US --- NRF_RETR_DELAY_250US
NRF_SPEED_2M --- NRF_SPEED_250K

I don't have now time to test those settings, but some day next week i will.
```

---
## \#149 Posted by: rpn314 Posted at: 2017-06-23T22:13:34.968Z Reads: 127

```
@Quezacotl Do a full revert back to the pre-December 2016 version. He changed a lot more than the speed and delay settings. Vedder also added some capability to have the nunchuck auto-pair with a VESC (even changed the communication packet/protocol on it) but the VESC code does not have any similar features that I am aware of (so I suspect this is a feature we'll only see in the VESC6). This change also means that the resistors are not longer used to make the address, so the 198.199.(resisotr binary values) we've been using don't work. He completely deleted that code.
```

---
## \#150 Posted by: Quezacotl Posted at: 2017-06-24T08:26:23.219Z Reads: 122

```
Oh, true. Seems that it relies on STM32 chip's unique ID. Apparently it will be in next VESC firmware, not only in VESC6 i hope.
```

---
## \#151 Posted by: trampa Posted at: 2017-06-25T21:27:59.369Z Reads: 127

```
With VESC-Tool that will be sorted. My VESC 4 with external NRF module does the automatic pairing just fine.

Frank
```

---
## \#152 Posted by: rpn314 Posted at: 2017-06-26T10:33:55.107Z Reads: 127

```
I figured as much. But us laymen don't have that VESC firmware or code base yet, and we don't have a release date for that, so we have stick to reverting to a previous version.
```

---
## \#153 Posted by: trampa Posted at: 2017-06-28T17:35:13.237Z Reads: 126

```
True, but it won't be long until its released.

Frank
```

---
## \#154 Posted by: Nordle Posted at: 2017-06-28T18:38:23.284Z Reads: 123

```
Damn i like that dead bug style soldering! Respect
```

---
## \#155 Posted by: WrinklyWink Posted at: 2017-07-12T05:49:25.037Z Reads: 120

```
perhaps its too late but alcohol works wonders at breaking down hot glue..
```

---
## \#156 Posted by: Quezacotl Posted at: 2017-07-25T08:48:58.179Z Reads: 115

```
Now i soldered a presumably genuine CP2102 chip. I ordered it from Mouser when i got some other parts aswell.
The "activation" problem i was talking earlier still exists. So the problem is not in the USB chip.
I have made even a third remote, which has the same problem.
I have confirmed that all the components have right values, and they are on right places.
Still the only "solution" i have is to put a switch between BOOT0-signal.
```

---
## \#157 Posted by: rpn314 Posted at: 2017-07-25T10:58:50.036Z Reads: 114

```
I am still quite baffled by your issue. All the one's I've made (5 or so now) wake up perfectly when you press (and hold for a second) the Z and C buttons....
```

---
## \#158 Posted by: Quezacotl Posted at: 2017-07-25T12:34:08.789Z Reads: 116

```
Yea, very strange problem. I need to inspect carefully every single part including the PCB next time i bother to dig into this again.

But today i noticed that while the BOOT0 signal is cut, the databridge works still through BLDC-tool. I didn't even test that feature when i saw that programming won't work. I just assumed that databridge wouldn't work either.
So actually the BOOT0-signal is only for programming.
```

---
## \#159 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-05T07:41:47.144Z Reads: 108

```
Do you Still make them? I'd like to buy a populated board if you do!
```

---
## \#160 Posted by: rpn314 Posted at: 2017-08-05T15:56:08.816Z Reads: 102

```
Sure! I just sent you a PM.
```

---
