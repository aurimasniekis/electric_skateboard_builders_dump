# New vesc user? Read This - COMPLETE WALKTROUGH OF THE VESC

### Replies: 176 Views: 90683

## \#1 Posted by: evoheyax Posted at: 2016-05-07T23:02:46.515Z Reads: 4462

```
Many new users may find the VESC confusing or not understand what they are doing. I will attempt to break this barrier down, and congregate all the VESC information across this forum here.

----------
**Background Information**
----------

First off, you need to understand the VESC is a speed controller, which is sorta like the brain of your electric skateboard. It's the middle man, between your input through a controller (also know as transmitter/reciever system) and your motors.

You should understand some basic terms too. I will give you an analogy so you can try to visualize it.

**Voltage** - Think of it like how big a muscle is
**Amps** - Think of it as how much energy you can send to that muscle

- You can have huge muscles, so moving something with that muscle takes less energy than someone who has smaller muscles (i.e. high voltage, low amps) (a good example of this is running at 10s and only 15 amps per motor)

**OR**

- You can have small muscles, which means to do the same as the big muscles, you need more energy. (low voltage, high amps) (a good example is 6s and 120 amps per motor)

Now that you have some background about voltage and amps, lets get to the VESC.

----------
**About the VESC**
----------

This speed controller has the ability to do many things a normal RC speed controller can not. One of those is limiting the amount of amps that come from your battery to your motors. An easy way to burn up a motor is by sending it more amps than it can handle for too long (often while riding up a hill). This means you should never burn up a motor with a vesc (unless you set this limit too high). There's also many other protections that can be set through limits, such as the max temperature you want the vesc to get to (so you can't burn up the speed controller), min and max input voltage (so you can't pull the voltage of your battery under a safe limit, which would brick your battery), and max regenerative break amps (protects battery from having too many amps sent back in to it). So you can protect your entire electronic system from making some of the most common user mistakes by setting these limits correctly.

----------
**Variations of VESCs**
----------

They're are many different VESC's on the market, and none of which are equal. Few actually use vedders BOM to the tee anymore, creating their own mods to increase stability. So buying a VESC 4.12 from one vendor is not the same VESC 4.12 of another vendor.

On top of that, some vendors, like Ollin Board Co (i.e. @chaka) offer direct FETs, which are thiner and deal with heat a little better.

Enertion took it's own route with the VESC-X (now named the FOCBOX, keep reading for more info), which seems to be based on the VESC 5 design. Again, direct FETs are used, and the max amp rating is much higher.

The VESC 5 was scapped for the VESC 6, which is not yet released, though prototypes exist showing it's increased max continuous amps and increased FOC stability.

The VESC 4.12 can do **27** amps continuous before going nuclear.
The VESC 6 can do **50** amps continuous before going nuclear.

The VESC-X is unknown at this time, though it's claimed to have a higher amp rating than the VESC 4.12.

The VESC 6 may be a good option for really powerful single drive or dual drive boards, but is an over kill for most. At this point, it looks to be better suited for electric bikes than electric skateboards, especially given the projected price tag.

----------
**Difference between VESC-X (i.e. FOCBOX) and VESC 4.12 (or lower VESC versions)**
----------

The VESC-X runs on a different tool than other VESCs. As a result, you should download those from enertions site.

- For windows, [Click Here](http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/).
- For Mac, [Click Here](http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-mac/).

----------
**Recent changes to the VESC**
----------
Vedder recently, with the help of Trampa, trademarked the VESC. This means only Trampa can sell the VESC under the name VESC anymore. Thus, companies are being forced to changed the name of their VESC based speed controllers.

- The VESC-X is now named the FOCBOX
- For Esk8.de, the VESC 4.12 is now called the ESK8 Controller
- For Torqueboards, i.e, diyelectric, the VESC 4.12 is called the Torque ESC

----------
**Downloading BLDC tool**
----------

Now, the first thing you should understand is when you get your vesc, you need to find the correct BLDC tool. There are mac/linux/windows versions, but **you need the bldc tool with the same firmware as the one pre installed on your vesc**. If you are unsure which firmware your vesc came pre installed with, ask the person you bought it from, or download any version, and when you attempt to connect your vesc to the bldc tool, you will get an error which will tell you which version of firmware you have. For instructions on connecting your vesc, read below.

You can update or downgrade the firmware to match the version of bldc tool you have, but this should be a last option solution if you really can't find the right tool. You can fry the drv chip on your vesc by doing a bad firmware update, which is very easy to mess up, and would make your vesc an expensive paper weight.

- To download the BLDC too for Mac or Windowsl, Please wait. There is no link at this time.
- To download the BLDC tool for Ubuntu, [Click Here](https://github.com/vedderb/bldc-tool) and follow the instructions in the README file.
- For information about upgrading firmware, [Click Here](https://www.electric-skateboard.builders/t/vesc-faq-firmware-upgrade-guide-windows-osx/852).

Now that you have the correct BLDC tool, you can connect your VESC to your usb type b cable to your vesc, and the other end to your computer. Now is a good time to talk about powering the VESC for configuration. Both Vedder (who is the guy that engineered this speed controller) and onloop (a prominent seller of the vesc) recommend using a lab rated regulated power supply to power the VESC during configuration. I use one I bought on amazon for around $45 USD. This however, may not be necessary. Chaka, another prominent seller of the VESC, suggests you only need to do this when powering up for the first time, and his have been powered before shipping, thus with his, this is not necessary. You can read more about Chaka's Low power recommendations [Here](https://www.electric-skateboard.builders/t/vesc-faq-when-to-use-low-voltage-vesc-configuration/1965). It's most important to use a regulated power supply if the VESC has never been powered up before. This is not an issue for those buying VESCs from any of the prominent VESC sellers like Torque Borads, Enertion, Axle, Esk8.de, or Chaka.

----------
**Connecting through BLDC tool**
----------

Now that you have it powered and physically connected, its time to make the software connection through the BLDC tool. Select the right port (not the bluetooth one). You should have only 2 options, the bluetooth and another. Click connect. And in the bottom right corner, you should see a green status with your current firmware version. This is the time that you will see an error message if the firmware on your vesc and the version of BLDC tool you have do not match. You can solve this mismatch by downloading an older version of BLDC (the one that matches your firmware version), or flashing the firmware (first option is much safer), as linked above.

----------
**Configuring your VESC**
----------

Now, onto the configuring itself. [Here](https://www.electric-skateboard.builders/t/easy-vesc-configuration-in-windows-mac-for-noob/2963) is an article explaining what you need to modify to get your vesc running.

To see how you make these change, Jaccobly has done a fabulous video found [Here](https://www.electric-skateboard.builders/t/vesc-faq-in-depth-video-how-to-program-your-vesc/2088).

----------
**For more specific segments**
----------

- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244) how to setup the receiver and brakes
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353) more info about setting up the Regenative breaks
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139) how to setup the Nyko Kama wii remote
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142)  how to setup dual motors through the canbus port
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-duty-cycle-vs-current-control-ppm-settings/1218) an explanation about the difference between Duty Cycle and Current Control
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500) an explanation of how to do motor detection
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-limit-output-voltage-according-to-motor-maximum-specs/683) information about limiting the voltage of your battery

----------
**Side Note**
----------

Please note, if you are configuring on a lab rate Regulated power supply, you will have issues controlling the motor after configuring the receiver and doing motor detection. Your motor will nudge a tad bit, if at all, and stop immediately. This is because the power supply is not giving the vesc enough amps. To get around this, when you think your settings are all good, test it using your battery.

----------
**Conclusion**
----------

Now that you have reach this point, you should now have working settings and allow you to run your motor through your controller. In theory, this can be your ending point, there is however, one last feature of the vesc that separates the vesc from other speed controllers, and this is a mode called FOC, or Field Orientated Control.

Instead of running in BLDC mode, you can run in FOC mode. For more information about what FOC mode is, [Read This](https://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419)!

For a comparision of BLDC and FOC, [Read This](https://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/)!

To configure FOC mode, Vedder himself has put together a youtube video, which is linked from [This Thread](https://www.electric-skateboard.builders/t/vesc-faq-bejamins-foc-tutorial/1178).

----------
**Watt Control Mode**
----------
A member of the community @Ackmaniac modified both the BLDC-tool and the VESC firmware to add a mode called watt control. Basically, instead of adjust amps like control mode does, it controls watts, which takes into consideration voltage. As a result, you can decrease the negative impact on performance of sag.

To read more about it and downloads, read his thread [Here](https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286).

----------
**PROBLEMS?!?**
----------

Now, you should hopefully have a working and correctly configured electrical system. If you don't, read [this article](https://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672). A lot of useful debugging information is there.

If anything in this guide seems misleading or inaccurate, or you feel points are missing, please post so below. This is th information I have gathered from my experience of using the VESC. I'm am not an electrical engineer, nor have I taken General Physics II with applied calculus, which focuses mostly on the physics behind electricity. So I have not the best person to ask technical questions to.

Thank you for reading and I hope this will help!
```

---
## \#2 Posted by: evoheyax Posted at: 2016-05-07T23:08:12.564Z Reads: 3055

```
@onloop Could you pin this topic to the top of the forum? or at least for newer users. This connects the dots of information on this forum about the vesc together, and should eliminate most peoples questions about the vesc.
```

---
## \#3 Posted by: Bender Posted at: 2016-05-07T23:11:48.300Z Reads: 2927

```
This is great!
And for me the timing couldn't be better
I'm setting up my first VESC in 2 days
```

---
## \#4 Posted by: cmatson Posted at: 2016-05-08T02:31:03.593Z Reads: 2646

```
holy sh*t bro you are going all out with the starter/new user posts!!! this is great man!!
```

---
## \#5 Posted by: treenutter Posted at: 2016-05-08T03:01:35.887Z Reads: 2315

```
[quote="cmatson, post:4, topic:2980"]
holy sh*t bro you are going all out with the starter/new user posts!!!
[/quote]


@evoheyax these are a huge contribution thanks!
```

---
## \#6 Posted by: evoheyax Posted at: 2016-05-08T03:19:38.851Z Reads: 1995

```
thank you. I've been thinking about this for a while. The thing is, this forum has been a great place to learn stuff, but the information now is too far spread out. Its everywhere on this forum, and while searching can help, you will be weeding through a lot more than you would want to go through, especially if your a new builder whose already swamped with other things to learn, like what parts they should use, or how to solder correctly, or understanding enough about volts and amps to figure out what drive train ratio they should use and what parts to use with that system.
```

---
## \#7 Posted by: karma Posted at: 2016-05-08T15:31:33.418Z Reads: 1786

```
Really good post! This will save alot of time and headache. Just a small typo under "**About the VESC**",  "An easy way to burn up a motor is sending more amps than **is** can handle for too long (often while riding up a hill).", should be, "An easy way to burn up a motor is sending more amps than **is** can handle for too long (often while riding up a hill)."
```

---
## \#8 Posted by: evoheyax Posted at: 2016-05-08T17:33:41.806Z Reads: 1660

```
Thanks, I know I should re read it like, 10 more times. I've been fixing up the language. When I type, I tend to do that for some reason, haha.
```

---
## \#9 Posted by: Ulfberht Posted at: 2016-05-08T20:48:01.900Z Reads: 1594

```
@evoheyax You really hit it out of the park with this thread. Very complete and much appreciated. I've already learned and bookmarked all of this information, but I had to suffer to get it!! Thanks for condensing and making a great primer for anyone looking for the best info. You rock, Luke!! :v:
```

---
## \#10 Posted by: lilracerboi Posted at: 2016-05-12T00:16:22.051Z Reads: 1489

```
Just to get something straight, I can run the motor detection/setup everything using just the lipo batteries? Or do I need a separate power supply?
```

---
## \#11 Posted by: evoheyax Posted at: 2016-05-12T01:21:23.318Z Reads: 1414

```
You can use either a separate power supply or you normal lipo/lion battery to do the motor detection. The same applies to doing the FOC detections, if you choose to run FOC instead of BLDC
```

---
## \#12 Posted by: lilracerboi Posted at: 2016-05-12T03:03:45.080Z Reads: 1346

```
Alright cool. I don't have a separate power supply, so I was worried. I'm going to be running FOC tomorrow, when I get the VESC in the mail.
```

---
## \#13 Posted by: lilracerboi Posted at: 2016-05-12T19:12:54.009Z Reads: 1310

```
When it says "spin freely" does it mean off the ground or without a belt?
```

---
## \#14 Posted by: evoheyax Posted at: 2016-05-14T06:43:24.932Z Reads: 1272

```
define "it"? I'm not sure what context you are pulling that from :)
```

---
## \#15 Posted by: lilracerboi Posted at: 2016-05-14T07:49:37.251Z Reads: 1259

```
Sorry.

From http://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500
Step 1.
```

---
## \#16 Posted by: evoheyax Posted at: 2016-05-14T16:30:51.130Z Reads: 1252

```
That comment is saying you should put it in a position (off the ground) where nothing stops the motor from spinning. The belt is fine, if you can take your hand, and spin the wheel without great difficulty. The belt should make it slightly harder to spin, but not too hard to spin. You should run the detection with the belt attached. But most importantly, it should be able to spin without any load, as when you click on detect motor button, it will do a series of tests that will make the motor spin. If you have load or even if the wheel is touching the ground, it will fail detection, as the motor can't spin freely.

For me, I prop my boards up on foam blocks while doing detection. You could also just flip the board over.
```

---
## \#17 Posted by: lilracerboi Posted at: 2016-05-14T21:06:34.335Z Reads: 1197

```
I figured it was that way. Didn't know if there was a difference with or without the belt.

Thanks.
```

---
## \#18 Posted by: Bender Posted at: 2016-05-15T04:23:09.147Z Reads: 1173

```
I just did a test with and without the belt
Almost indistinguishable, just slightly lower ERPMs with belt on.
```

---
## \#19 Posted by: laurnts Posted at: 2016-05-15T12:12:45.700Z Reads: 1158

```
It doesn't or shouldn't change alot. Because what its detecting is motors stator & magnetic fields. It has nothing to do with load.
```

---
## \#20 Posted by: nfed163 Posted at: 2016-05-27T22:59:44.489Z Reads: 1203

```
[quote="evoheyax, post:1, topic:2980"]
Now that you have the correct BLDC tool, you can connect your VESC to your usb type b cable to your vesc, and the other end to your computer.
[/quote]

I ahvn't bought my VESC yet but can you elaborate on how the VESC is connected to the computer? Do I need to buy a separate cable? what is the input on the VESC? 

Super helpful post! Thank you!
```

---
## \#21 Posted by: Hummie Posted at: 2016-05-27T23:55:24.795Z Reads: 1119

```
Usb on computer to mini usb on vesc
```

---
## \#22 Posted by: LukeM Posted at: 2016-06-01T01:30:58.807Z Reads: 1108

```
Hey I just got my VESC and am trying to download the tool but the site appears to be down. Here is what I see:
<img src="/uploads/db1493/original/2X/d/d485fd275ff7164b1d705061629f11819b6b1e4b.png" width="690" height="388">
```

---
## \#23 Posted by: LukeM Posted at: 2016-06-01T01:32:25.662Z Reads: 1023

```
Is there any where else I can download the tool?
```

---
## \#24 Posted by: makevoid Posted at: 2016-06-01T06:12:27.815Z Reads: 984

```
@jacobbloy ping
```

---
## \#25 Posted by: evoheyax Posted at: 2016-06-01T06:31:53.139Z Reads: 977

```
I believe there's files for the tool floating around somewhere on the web. You have to compile it though in to a runnable file.
```

---
## \#26 Posted by: jacobbloy Posted at: 2016-06-01T06:35:37.580Z Reads: 960

```
sorry guys i sleep while your awake i was updating some stuff last night it is being fixed
```

---
## \#27 Posted by: LukeM Posted at: 2016-06-01T17:53:49.548Z Reads: 950

```
@jacobbloy Thanks! Do you have an estimate to when the site will be up again?
```

---
## \#28 Posted by: jacobbloy Posted at: 2016-06-01T22:42:20.763Z Reads: 943

```
It's been back up for some time now!
```

---
## \#29 Posted by: Justin Posted at: 2016-06-24T22:45:15.804Z Reads: 941

```
Unfortunately i am unable to download the BLDC-tool for Mac OSX. I entered my emailadres some time ago. But have not received the download link (i also sent you an email via your site). Is there another place where i can find the tool?

- Edit: Tried a different emailadres and now it works fine -
```

---
## \#30 Posted by: scisslehannd Posted at: 2016-07-01T20:39:17.851Z Reads: 940

```
Can someone please, for the life of me, tell me where to buy a VESC right now so I can receive it ASAP.

Meaning..... the VESC is in the warehouse ready to be shipped. It seems all the websites I find (enertion, diyelectricskateboard, etc) are producing VESC and if I order right now I will be waiting months.
```

---
## \#31 Posted by: CSN Posted at: 2016-07-01T20:48:16.868Z Reads: 944

```
http://www.ollinboardcompany.com/product/vedder-s-speed-controller

will be the quickest to receive and most reliable.

Might still be a week or two but much better than waiting for months to get beta product.
```

---
## \#32 Posted by: jacobbloy Posted at: 2016-07-04T16:30:09.670Z Reads: 928

```
https://www.youtube.com/playlist?list=PLICpQdAXJazT-ICMIgJuc2pl-w0-j1j9A
```

---
## \#33 Posted by: jacobbloy Posted at: 2016-07-04T16:30:57.800Z Reads: 881

```
try it again I'm having trouble with some emails servers so it will again direct download
```

---
## \#34 Posted by: Titoxd10001 Posted at: 2016-07-21T01:54:59.482Z Reads: 838

```
How do I connect a sensored motor?
```

---
## \#35 Posted by: Mandy Posted at: 2016-07-21T02:58:59.344Z Reads: 838

```
Alright cool.  I get more understanding on VESC. Thanks for your kindly sharing.
```

---
## \#36 Posted by: MicroRAsus Posted at: 2016-07-21T07:24:13.592Z Reads: 843

```
Nice tutorial! I wonder how to use vesc for head light? such as in this video:https://www.youtube.com/watch?v=G8f0xg7DNmM
```

---
## \#37 Posted by: jrpwit Posted at: 2016-07-21T10:24:44.539Z Reads: 835

```
I always wondered the same thing after seeing that video by vedder. Really loved the turn signals cause I use the nunchuk.
```

---
## \#38 Posted by: Skitzor Posted at: 2016-07-26T11:37:53.231Z Reads: 828

```
I join these guys above me. That setup though is with a colorcoded LED bar. I just need an output, maybe three I can toggle for brake, left and right. But turn signals are optional for me...
```

---
## \#39 Posted by: petmakris Posted at: 2016-08-09T19:14:44.270Z Reads: 820

```
See the custom firmware post by vedder
```

---
## \#40 Posted by: t1m0007 Posted at: 2016-08-10T21:22:19.713Z Reads: 886

```
Link for the lazy http://vedder.se/2015/08/vesc-writing-custom-applications/
```

---
## \#41 Posted by: webst Posted at: 2016-10-15T11:20:50.278Z Reads: 755

```
Is it better to first config VESC with usb cable or bluetooth? Can you point me to best, most reliable tutorial on how to connect bt module and use it? Preferably at the same time as  remote. I plan dual vesc setup.
```

---
## \#42 Posted by: JohnnyMeduse Posted at: 2016-10-15T14:45:57.015Z Reads: 735

```
try to search using the keyword VESC FAQ, and you will find most of the tutorial you need, also you need to connect via usb first (I don't think there a way to connect and change parameter via Bluetooth)
```

---
## \#43 Posted by: lamjiasheng Posted at: 2016-10-20T17:12:24.791Z Reads: 727

```
I have a question here
Enertion vesc and other vesc have a 3 tube like connector to connect motor with vesc and a 2 wire to connect vesc and the battery right ?

So my main concern is every battery vesc and motor we get will be have the same connector to install easilly right or there are many types of connector ?

Like somehow a battery only comes with 2 wire and fhe vesc have 3 ports
```

---
## \#44 Posted by: evoheyax Posted at: 2016-10-20T18:17:10.924Z Reads: 695

```
I would suggest you read about rc connector types, since most of the connectors we use on eboards started in the rc hobby world. there are xt60, xt90, 3mm bullet, 4mm, 5.5mm bullet, 8mm bullet (super high amp), servo, and more. 

There's many many different types of ports, just like with any other electronic. Cell phones, for example, have many different plugs. In the cell phone world, most are using micro usb these days (besides the iphone, which uses the lighting), but usb mini and some other ports pop up on phones from time to time. And similarly, in eboards, the xt60 or xt90 is usually used for battery connections, and the 4mm bullet connector or 5.5mm bullet connector is used for motor wires. 

You should know the names of the ports, their amp ratings, ect. You need to understand what's going on with your electronics, or you will waste a lot of money blowing up parts (and possibly injury yourself).

If you did a simple search on hobby king for batteries for example, you would see that batteries have different connectors. A lot of hobby grade batteries use 5.5mm bullets for the battery. But bullet connectors are not anti-spark plugs, so you get a big pop noise every time you plug it in. Reaserch before you buy stuff! You can get convertor cables to so you don't have to solder.
```

---
## \#45 Posted by: Spek Posted at: 2016-10-21T03:40:10.120Z Reads: 636

```
Also some sellers like ollinboards allow you to select your connector types. In my case, I just matched my motors' and batteries' connectors on my vesc order.
```

---
## \#46 Posted by: lamjiasheng Posted at: 2016-10-21T09:04:04.301Z Reads: 633

```
I'm planning on the enertion vesc-standard
Its xt and mm type are self custom ?
Or whats the xt type and the mm of the vesc
```

---
## \#47 Posted by: im-done Posted at: 2016-10-21T13:21:55.685Z Reads: 623

```
You may want to post about the .004 glitch thing
```

---
## \#48 Posted by: webst Posted at: 2016-10-22T01:59:40.486Z Reads: 630

```
Why don't you post about it? All I found out is that "there's a glitch on most BLDC tools that will mutliply the value by 10 every time you write in the motor config tab. The default value is .04 which is why you want to set it to .004 before you write."

source: http://www.electric-skateboard.builders/t/update-not-enough-power-or-lost-of-it-enertion-build/7104/32?u=webst
```

---
## \#49 Posted by: evoheyax Posted at: 2016-10-22T20:02:46.134Z Reads: 618

```
This would be a good question to ask enertion. I'm 90% sure they are using 5.5mm bullets for the motor phase wires, and xt60 for the battery side. But I can't confirm 100%, because I don't own one, nor do I work for enertion, and they don't even have it listed on their site.
```

---
## \#50 Posted by: im-done Posted at: 2016-10-22T20:58:24.750Z Reads: 608

```
I didnt post about it becuase i simply did not know much about the glitch. I just remeber that i had to change a value to .004.
```

---
## \#51 Posted by: tommyjamez Posted at: 2016-11-26T01:34:53.705Z Reads: 596

```
My welder gets here in a few days, and I'll be building my own 18650 packs with BSM and VESC thanks to the info on here!  The money I'm saving and the maintenance that needs to be done in the future are things that I can't thank you enough for. You guys rock!!
```

---
## \#52 Posted by: nmagz3 Posted at: 2016-12-09T08:03:45.242Z Reads: 569

```
@evoheyax  Hey, this is exactly what I've been looking for!  As a noob you try your best to search and take pieces of information from different posts to create an understanding of a particular topic.  I've been able to do that very well for most things concerning my board.  However, the VESC is a hurdle I didn't want to take lightly and finding information on it was confusing.  I found threads that talked about the VESC and FOC in depth.  I also found threads that had debates about how things should be done.  But, this is the first post I've read that really spelled it out and that basic straight forward approach is what I needed for my first VESC "install".  Thanks so much for taking the time to put this together.
```

---
## \#53 Posted by: Osogeetchie Posted at: 2016-12-13T21:06:54.647Z Reads: 535

```
Can someone PLEASE Please help me. I'm looking for a VESC for 6s batteries for an electric longboard I'm trying to create, I want to connect a Bluetooth transmitter to the vesc and I want the boats to travel around 7-9 miles at around 20mph, I know I'm sort of asking for a lot but I've been looking for so long and just stumbled upon this forum. Thank you.
```

---
## \#54 Posted by: Fatch Posted at: 2016-12-16T13:11:22.544Z Reads: 520

```
Hey man I'm thinking about building a simple board but it's my first and I could use a hand can you message me for some tips and stuff thanks
```

---
## \#55 Posted by: laikiux Posted at: 2016-12-22T17:36:36.500Z Reads: 517

```
Hi,
I bought 4.12 VESC from Enertion. I downloaded BLDC tool from here http://vesc.net.au/ . Now I have 10s Li-ion Batttery with 36.6 V. Can I connect VESC with this battery for the first time or power supply is necessary? Will I need to upgrade firmware?
```

---
## \#56 Posted by: yaca Posted at: 2016-12-22T21:13:51.501Z Reads: 528

```
When I connected my 4.12 VESCs from Enertion the first time I used a 3s Lipo for to make motor detection but since them I always use my 10s battery for to change values. I'm not sure if it's a problem to use 10s at the first connection. I recommend to use the BLDC Tool and firmware 2.52 from @ackmaniac but if you want to use firmware 2.18 you have to look about "Max current ramp step" in Motor config - Advanced. The value should be 0,04. If this value is changing (it multiplies per 10) after every write and read you have the bug version of 2.18 firmware wich I had on my vescs when I got them in july.
```

---
## \#57 Posted by: LAVAMAN Posted at: 2017-01-03T22:40:06.049Z Reads: 520

```
Thanks for combining all this info. in one place. I will be working on this in the near future and will use this resource "before" I start asking a million questions.
```

---
## \#58 Posted by: thallazar Posted at: 2017-01-06T13:39:55.141Z Reads: 512

```
I'm really confused as to how the VESC connects to whatever controller you've got. Does it require a seperate device if you want to connect to an RC remote?
```

---
## \#59 Posted by: rwxr Posted at: 2017-01-06T14:22:16.932Z Reads: 524

```
You need the specific receiver that comes with your controller. The receiver is powered by the VESC and then you need to follow your controllers bind instructions.
When that is done, you need to configure min and max pulsewidth for your controller in BLDC-tool before you can use it.
```

---
## \#60 Posted by: sensationalsalmon Posted at: 2017-01-07T23:26:24.816Z Reads: 519

```
So i jut put together my skateboard and have a 4s battery with 16000 mah and a 10C discharge. I only have one and am pretty much getting no power to the motor and I don't know what my options are to fix this. I have a turnigy 245kv motor on it. Help?
```

---
## \#61 Posted by: JohnnyMeduse Posted at: 2017-01-07T23:58:13.811Z Reads: 499

```
[quote="sensationalsalmon, post:60, topic:2980"]
4s battery
[/quote]

4s battery is pretty low, specially if you're using a Vesc.... You need at least 6s or more
```

---
## \#62 Posted by: sensationalsalmon Posted at: 2017-01-08T00:10:43.493Z Reads: 497

```
i ordered two 42 5200 mah batteries and perhaps in the future i will get another 42 to go along with the one I already have.
```

---
## \#63 Posted by: Rollbrett Posted at: 2017-01-15T23:39:33.841Z Reads: 506

```
@evoheyax Please add a special note for the "Max Current Ramp Step" bug to prevent peeps from blowing their DRVs like I did!
http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#64 Posted by: Cazbuilds Posted at: 2017-01-18T03:20:31.461Z Reads: 472

```
Quick question for you guys. For some reason when I click to download the tool, it says that the "This service is temporarily unavailable!" and I can't go to the website. Anyone else having this problem or is it from my ISP?
```

---
## \#65 Posted by: NickTheDude Posted at: 2017-01-18T03:23:46.906Z Reads: 456

```
Down for me as well. You can use this site to check: http://www.isitdownrightnow.com/
```

---
## \#66 Posted by: evoheyax Posted at: 2017-01-18T06:12:16.804Z Reads: 458

```
For some reason, I am unable to modify the original post. I want to add info about alternate firmwares also, such as @Ackmaniac's firmware.
```

---
## \#67 Posted by: lox897 Posted at: 2017-01-18T06:16:21.958Z Reads: 458

```
It's because it is too old. Only moderators can edit it. If you write it up in a word doc or whatever and email it to me I'll change it for you
```

---
## \#68 Posted by: Hylke59beare1913 Posted at: 2017-02-03T11:54:05.044Z Reads: 456

```
i have the new vecs-x from Enertion, but no cable to connect to the receiver where can i bay this cable Enertion dont have.
```

---
## \#69 Posted by: jujet Posted at: 2017-02-03T12:16:27.253Z Reads: 451

```
You can use your phone's data cable
```

---
## \#71 Posted by: SeanHacker Posted at: 2017-02-03T17:13:44.218Z Reads: 454

```
The cable you're looking for is called a servo cable. You can pick them up at your local hobby shop or anywhere on the internet.
```

---
## \#72 Posted by: NICOMUTTER Posted at: 2017-04-10T10:11:00.693Z Reads: 465

```
<img src="/uploads/db1493/original/3X/c/f/cf18913fd58b7b8df88395d924d2f9d26db14f1e.JPG" width="373" height="500"><img 

Hello, 

How do I connect my receiver to my VESC :o 
need help ty :)
Image 2 just behind
```

---
## \#73 Posted by: NICOMUTTER Posted at: 2017-04-10T10:11:36.641Z Reads: 458

```
<img src="/uploads/db1493/original/3X/5/d/5da75fc8ca7834e9a7f9a68edcfe15215eb2b749.JPG" width="373" height="500">
Image 2
```

---
## \#74 Posted by: JohnnyMeduse Posted at: 2017-04-10T12:45:28.961Z Reads: 445

```
@NICOMUTTER

I think this thread might be helpful to you

https://www.electric-skateboard.builders/t/vesc-receiver-connection-questions/6558
```

---
## \#75 Posted by: rwxr Posted at: 2017-04-10T13:41:01.758Z Reads: 423

```
Also, that rug is probably not the best placement of electronics due to static electricity.
```

---
## \#76 Posted by: NICOMUTTER Posted at: 2017-04-11T08:03:16.577Z Reads: 425

```
It's was just for the pic ;p
```

---
## \#77 Posted by: mptrs Posted at: 2017-05-09T21:08:18.333Z Reads: 397

```
Link to BLDC tool died :frowning:
```

---
## \#78 Posted by: evoheyax Posted at: 2017-05-09T21:14:38.602Z Reads: 409

```
yes, and theres not a new one either.

I had a hell of a time downloading it yesterday.

If your using linux, you can download the github repository from vedders github, and compile it yourself, which is what I did. It's a bit of a pain though and you need to know how to navigate directories through the command prompt.

Windows and mac, you can try this, though IDK if it works: https://drive.google.com/drive/folders/0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU

You will be limited in the firmware versions you can run though. Jacob seems to have completely disappeared.
```

---
## \#79 Posted by: mptrs Posted at: 2017-05-09T22:42:39.051Z Reads: 400

```
Thanks!

@jacobbloy was online 22 hours ago, hope he can everything up and running. Maybe it's cheaper for him to share all version on github? You can host the site there as well.
```

---
## \#80 Posted by: evoheyax Posted at: 2017-05-09T22:44:15.948Z Reads: 424

```
IF anyone has any good versions please share them. I know theres a lot out there with the tool and since Jacob was the only one really hosting it, we're left in a bind...
```

---
## \#81 Posted by: yaca Posted at: 2017-05-10T11:00:41.359Z Reads: 465

```
Why not ackmaniacs version? Just for  Maytechs without  bootloader it is more difficult.
```

---
## \#82 Posted by: evoheyax Posted at: 2017-05-11T15:29:56.651Z Reads: 452

```
That is a possibility... I will research his firmware more this summer and try it out.
```

---
## \#83 Posted by: Cole935 Posted at: 2017-06-06T21:36:28.195Z Reads: 442

```
So where can I download the VESC software for windows?
```

---
## \#84 Posted by: SpeedyGornzallez Posted at: 2017-06-07T07:08:58.716Z Reads: 450

```
@Cole935 
I got mine off Enertion but I'm sure there are many others, the Enertion software may only work specifically for the Enertion VESC but idk haha I'm a bit of a noob
http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/
```

---
## \#85 Posted by: thetechtrader Posted at: 2017-06-23T11:21:04.225Z Reads: 404

```
Im new to the forum, this is my first post and im pumped to learn about my new VESC coming in the mail!
QUESTION: Will my motor have more power/torque if I program VESC to allow my 12S volts to flow 44.4v for big muscle, and limit the amps to 50A? Or would it be the same if I used my required 8S with 29.6v and limit to 50A?
```

---
## \#86 Posted by: Challlsss Posted at: 2017-06-23T13:37:34.367Z Reads: 436

```
Hi @thetechtrader! Welcome to the forum! You are about to learn a lot more than you expected if you spend some time here! The more you read the easier your first build will be!

That being said: You will not "program" the VESC for Voltage. The VESC controls current being delivered to the motor and does not change voltage. So what voltage you use is %100 based on the battery. Changing the voltage on a board changes the top speed it can go at... if you had a 6S board that could do 10 mph and you changed the battery to a 12S it would then go roughly 20 mph. The torque would not change in this situation.

__HOWEVER__ more voltage in "real world" almost always means more torque, and this is because of gear ratios. When selecting your motor you will notice a spec called kv. This is essentially the gear ratio inside the motor and when going from 6S to 12S, or any other voltage you will likely have to change the kv of the motor. This is because VESC usears are limited to 60,000 erpm. And as a result you will change the top speed and torque output of the board.
```

---
## \#87 Posted by: evoheyax Posted at: 2017-06-23T20:18:39.323Z Reads: 461

```
@lox897 @laurnts @treenutter @Michaelinvegas @lowGuido @barajabali

Can one of you guys update the original post of this thread to the code that's below (I'm assuming if you click edit on this, you be able to see the code (text with formatting), and not just the text. I would do it my self, but I can't edit this topic anymore since Jason demoted me from Regular to Member last year. After the line below please!

----------



Many new users may find the VESC confusing or not understand what they are doing. I will attempt to break this barrier down, and congregate all the VESC information across this forum here.

----------
**Background Information**
----------

First off, you need to understand the VESC is a speed controller, which is sorta like the brain of your electric skateboard. It's the middle man, between your input through a controller (also know as transmitter/reciever system) and your motors.

You should understand some basic terms too. I will give you an analogy so you can try to visualize it.

**Voltage** - Think of it like how big a muscle is
**Amps** - Think of it as how much energy you can send to that muscle

- You can have huge muscles, so moving something with that muscle takes less energy than someone who has smaller muscles (i.e. high voltage, low amps) (a good example of this is running at 10s and only 15 amps per motor)

**OR**

- You can have small muscles, which means to do the same as the big muscles, you need more energy. (low voltage, high amps) (a good example is 6s and 120 amps per motor)

Now that you have some background about voltage and amps, lets get to the VESC.

----------
**About the VESC**
----------

This speed controller has the ability to do many things a normal RC speed controller can not. One of those is limiting the amount of amps that come from your battery to your motors. An easy way to burn up a motor is by sending it more amps than it can handle for too long (often while riding up a hill). This means you should never burn up a motor with a vesc (unless you set this limit too high). There's also many other protections that can be set through limits, such as the max temperature you want the vesc to get to (so you can't burn up the speed controller), min and max input voltage (so you can't pull the voltage of your battery under a safe limit, which would brick your battery), and max regenerative break amps (protects battery from having too many amps sent back in to it). So you can protect your entire electronic system from making some of the most common user mistakes by setting these limits correctly.

----------
**Variations of VESCs**
----------

They're are many different VESC's on the market, and none of which are equal. Few actually use vedders BOM to the tee anymore, creating their own mods to increase stability. So buying a VESC 4.12 from one vendor is not the same VESC 4.12 of another vendor.

On top of that, some vendors, like Ollin Board Co (i.e. @chaka) offer direct FETs, which are thiner and deal with heat a little better.

Enertion took it's own route with the VESC-X (now named the FOCBOX, keep reading for more info), which seems to be based on the VESC 5 design. Again, direct FETs are used, and the max amp rating is much higher.

The VESC 5 was scapped for the VESC 6, which is not yet released, though prototypes exist showing it's increased max continuous amps and increased FOC stability.

The VESC 4.12 can do **27** amps continuous before going nuclear.
The VESC 6 can do **50** amps continuous before going nuclear.

The VESC-X is unknown at this time, though it's claimed to have a higher amp rating than the VESC 4.12.

The VESC 6 may be a good option for really powerful single drive or dual drive boards, but is an over kill for most. At this point, it looks to be better suited for electric bikes than electric skateboards, especially given the projected price tag.

----------
**Difference between VESC-X (i.e. FOCBOX) and VESC 4.12 (or lower VESC versions)**
----------

The VESC-X runs on a different tool than other VESCs. As a result, you should download those from enertions site.

- For windows, [Click Here](http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/).
- For Mac, [Click Here](http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-mac/).

----------
**Recent changes to the VESC**
----------
Vedder recently, with the help of Trampa, trademarked the VESC. This means only Trampa can sell the VESC under the name VESC anymore. Thus, companies are being forced to changed the name of their VESC based speed controllers.

- The VESC-X is now named the FOCBOX
- For Esk8.de, the VESC 4.12 is now called the ESK8 Controller
- For Torqueboards, i.e, diyelectric, the VESC 4.12 is called the Torque ESC

----------
**Downloading BLDC tool**
----------

Now, the first thing you should understand is when you get your vesc, you need to find the correct BLDC tool. There are mac/linux/windows versions, but **you need the bldc tool with the same firmware as the one pre installed on your vesc**. If you are unsure which firmware your vesc came pre installed with, ask the person you bought it from, or download any version, and when you attempt to connect your vesc to the bldc tool, you will get an error which will tell you which version of firmware you have. For instructions on connecting your vesc, read below.

You can update or downgrade the firmware to match the version of bldc tool you have, but this should be a last option solution if you really can't find the right tool. You can fry the drv chip on your vesc by doing a bad firmware update, which is very easy to mess up, and would make your vesc an expensive paper weight.

- To download the BLDC too for Mac or Windowsl, Please wait. There is no link at this time.
- To download the BLDC tool for Ubuntu, [Click Here](https://github.com/vedderb/bldc-tool) and follow the instructions in the README file.
- For information about upgrading firmware, [Click Here](https://www.electric-skateboard.builders/t/vesc-faq-firmware-upgrade-guide-windows-osx/852).

Now that you have the correct BLDC tool, you can connect your VESC to your usb type b cable to your vesc, and the other end to your computer. Now is a good time to talk about powering the VESC for configuration. Both Vedder (who is the guy that engineered this speed controller) and onloop (a prominent seller of the vesc) recommend using a lab rated regulated power supply to power the VESC during configuration. I use one I bought on amazon for around $45 USD. This however, may not be necessary. Chaka, another prominent seller of the VESC, suggests you only need to do this when powering up for the first time, and his have been powered before shipping, thus with his, this is not necessary. You can read more about Chaka's Low power recommendations [Here](https://www.electric-skateboard.builders/t/vesc-faq-when-to-use-low-voltage-vesc-configuration/1965). It's most important to use a regulated power supply if the VESC has never been powered up before. This is not an issue for those buying VESCs from any of the prominent VESC sellers like Torque Borads, Enertion, Axle, Esk8.de, or Chaka.

----------
**Connecting through BLDC tool**
----------

Now that you have it powered and physically connected, its time to make the software connection through the BLDC tool. Select the right port (not the bluetooth one). You should have only 2 options, the bluetooth and another. Click connect. And in the bottom right corner, you should see a green status with your current firmware version. This is the time that you will see an error message if the firmware on your vesc and the version of BLDC tool you have do not match. You can solve this mismatch by downloading an older version of BLDC (the one that matches your firmware version), or flashing the firmware (first option is much safer), as linked above.

----------
**Configuring your VESC**
----------

Now, onto the configuring itself. [Here](https://www.electric-skateboard.builders/t/easy-vesc-configuration-in-windows-mac-for-noob/2963) is an article explaining what you need to modify to get your vesc running.

To see how you make these change, Jaccobly has done a fabulous video found [Here](https://www.electric-skateboard.builders/t/vesc-faq-in-depth-video-how-to-program-your-vesc/2088).

----------
**For more specific segments**
----------

- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244) how to setup the receiver and brakes
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353) more info about setting up the Regenative breaks
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139) how to setup the Nyko Kama wii remote
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142)  how to setup dual motors through the canbus port
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-duty-cycle-vs-current-control-ppm-settings/1218) an explanation about the difference between Duty Cycle and Current Control
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500) an explanation of how to do motor detection
- [Here's](https://www.electric-skateboard.builders/t/vesc-faq-limit-output-voltage-according-to-motor-maximum-specs/683) information about limiting the voltage of your battery

----------
**Side Note**
----------

Please note, if you are configuring on a lab rate Regulated power supply, you will have issues controlling the motor after configuring the receiver and doing motor detection. Your motor will nudge a tad bit, if at all, and stop immediately. This is because the power supply is not giving the vesc enough amps. To get around this, when you think your settings are all good, test it using your battery.

----------
**Conclusion**
----------

Now that you have reach this point, you should now have working settings and allow you to run your motor through your controller. In theory, this can be your ending point, there is however, one last feature of the vesc that separates the vesc from other speed controllers, and this is a mode called FOC, or Field Orientated Control.

Instead of running in BLDC mode, you can run in FOC mode. For more information about what FOC mode is, [Read This](https://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419)!

For a comparision of BLDC and FOC, [Read This](https://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/)!

To configure FOC mode, Vedder himself has put together a youtube video, which is linked from [This Thread](https://www.electric-skateboard.builders/t/vesc-faq-bejamins-foc-tutorial/1178).

----------
**Watt Control Mode**
----------
A member of the community @Ackmaniac modified both the BLDC-tool and the VESC firmware to add a mode called watt control. Basically, instead of adjust amps like control mode does, it controls watts, which takes into consideration voltage. As a result, you can decrease the negative impact on performance of sag.

To read more about it and downloads, read his thread [Here](https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286).

----------
**PROBLEMS?!?**
----------

Now, you should hopefully have a working and correctly configured electrical system. If you don't, read [this article](https://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672). A lot of useful debugging information is there.

If anything in this guide seems misleading or inaccurate, or you feel points are missing, please post so below. This is th information I have gathered from my experience of using the VESC. I'm am not an electrical engineer, nor have I taken General Physics II with applied calculus, which focuses mostly on the physics behind electricity. So I have not the best person to ask technical questions to.

Thank you for reading and I hope this will help!
```

---
## \#88 Posted by: Michaelinvegas Posted at: 2017-06-23T20:21:27.723Z Reads: 339

```
@evoheyax wow dude
```

---
## \#89 Posted by: evoheyax Posted at: 2017-06-23T20:23:03.026Z Reads: 339

```
I'm trying to create as much info as possible as the market is getting crazier. I'm far from down with this thread. Just for now, I'm done, lol. Next up, I want to tackle remotes and remote technology.
```

---
## \#90 Posted by: Michaelinvegas Posted at: 2017-06-23T20:24:20.938Z Reads: 329

```
I'll defer to the other guys that are prob on a computer at some point during the day to fix it as you requested
```

---
## \#91 Posted by: lox897 Posted at: 2017-06-24T10:38:03.171Z Reads: 328

```
Took me a while but I did it on my phone lol. Tell me if anything needs to be changed and will fix it
```

---
## \#92 Posted by: evoheyax Posted at: 2017-06-25T04:15:11.754Z Reads: 321

```
The text I made has links and styling. Is there a way for you to get the code + text, not just the text?
```

---
## \#93 Posted by: lox897 Posted at: 2017-06-25T11:33:11.756Z Reads: 310

```
Will do on laptop tomorrow.
```

---
## \#94 Posted by: TarzanHBK Posted at: 2017-06-25T11:55:20.831Z Reads: 309

```
Nice write up dude!
Found something:
[quote="evoheyax, post:87, topic:2980"]
Torque Borads, Enertion, Axel, Elkick, or Chaka
[/quote]
it´s "Axle" not "Axel" and "Esk8" at the moment, "Elkick" is currently off the forum (both are Esk8.de)
```

---
## \#95 Posted by: evoheyax Posted at: 2017-06-25T16:48:11.111Z Reads: 297

```
ahh, thanks, I'll fix thse two things!
```

---
## \#96 Posted by: thetechtrader Posted at: 2017-06-26T14:32:51.084Z Reads: 307

```
Yes the more I read on this site the more I learn in many different areas... AMAZING!

Base on my above questions, and your reply, here is my next question which may or may not have the same answer you just gave me, but gotta ask to learn :slight_smile:

Would my setup have more torque, and/OR draw less current if I used:
12S, limited eRPM to a max rotation and limit VEST amps to 50A

 - VS - 

10S, limited eRPM to same max rotation, and limited VESC to 50A

Im sure they are newbie questions but once I wrap my head around the fundamentals I will NEVER ask again :)
```

---
## \#98 Posted by: thetechtrader Posted at: 2017-06-26T15:13:31.976Z Reads: 294

```
Ok, that more or less has me understanding the relationships between volts, amps, kv, greatly appreciated
```

---
## \#99 Posted by: wafflejock Posted at: 2017-06-26T15:31:26.632Z Reads: 307

```
The higher voltage is also going to be more efficient since higher amperage is what causes power loss through anything with resistance (everything) and power delivered to the motor is a product of the amperage and voltage.  That said I setup a 12S at first but was too much for me personally so stepped it down to 10S when my batteries started showing some wear and made a better case to protect the lipos I'm using.  Personally use the board for transportation to local shops and the grocery store and stuff so I'm not looking for a speed demon ride just something safe and fun to get around without a car.
```

---
## \#100 Posted by: thetechtrader Posted at: 2017-06-26T18:07:25.171Z Reads: 302

```
In general do lower KV motors like 170kv use up more battery power/life/run time vs day 500kv?
```

---
## \#101 Posted by: Challlsss Posted at: 2017-06-26T18:27:11.470Z Reads: 307

```
@thetechtrader In general... yes. I can go more into depth but just realized we are completely hijacking this thread. It needs to stay specifially for New VESC users. These are more battery and motor related questions. If you would make a new thread or find one that matches your questions and tag me ill be happy to post more there.
```

---
## \#102 Posted by: lowGuido Posted at: 2017-06-26T18:36:47.242Z Reads: 319

```
sorted.
10
```

---
## \#103 Posted by: Snowi Posted at: 2017-07-09T05:05:09.379Z Reads: 295

```
what exact vesc is he talking about? is all vesc's the same and can use the same software and modification and etc?
```

---
## \#104 Posted by: evoheyax Posted at: 2017-07-09T18:15:57.599Z Reads: 290

```
At the time this article was written, the VESC 4.1x (replace x with 0, 1, or 2) was the only VESC we had. Enertion has since created the FOCBOX that uses it's own firmware and tool, which is why I recently updated this. If it's not a FOCBOX (aka VESC-X), then you don't need special firmware or software. Most apps should still work with the FOCBOX. Other wise, you need firmware for your particular VESC version and software for your particular firmware version. They do need to match.
```

---
## \#105 Posted by: Blasto Posted at: 2017-07-09T19:41:17.073Z Reads: 284

```
@evoheyax where did you get this that the focbox runs it's own custom fw? As far as i know they come with fw 2.18 on them
```

---
## \#106 Posted by: evoheyax Posted at: 2017-07-10T15:46:46.300Z Reads: 275

```
Really? I've been talking to @Ackmaniac and he said something about working on the enertion firmware for their FOCBOX.

From looking at their BLDC tool, it's a fair bit different looking at places. So I assumed between the 2 that the firmware is different.
```

---
## \#107 Posted by: Jinra Posted at: 2017-07-10T15:49:04.764Z Reads: 268

```
I do recall someone saying something about version 1.x f/w on the focboxes.
```

---
## \#108 Posted by: Blasto Posted at: 2017-07-10T16:07:09.041Z Reads: 277

```
Ah ok, i think he meant the focbox that are used in the raptor2 has custom fw. 

Other than that they come with fw V2.18 on them
```

---
## \#109 Posted by: evoheyax Posted at: 2017-07-10T16:31:41.640Z Reads: 283

```
Ahhh! That makes more sense then. Thanks for the clarity!
```

---
## \#110 Posted by: thetechtrader Posted at: 2017-07-24T23:45:21.918Z Reads: 266

```
Has anyone ever coated their VESC in Plasti-Dip to waterproof it? Please share your thoughts and/or process/tips.
Thanks in advance!
```

---
## \#111 Posted by: Jinra Posted at: 2017-07-24T23:47:04.362Z Reads: 272

```
That will thermally insulate the vesc and make it near impossible to repair. I know @hummie has potted stuff before, i think vesc as well.
```

---
## \#112 Posted by: thetechtrader Posted at: 2017-07-25T00:19:51.828Z Reads: 268

```
Yes, my concern is it getting too warm.
Fixing it... I dont know how, and a $99 board cant cost much more than paying someone to fix it.
@hummie and insite on waterproofing a vesc?
```

---
## \#113 Posted by: Jinra Posted at: 2017-07-25T00:31:26.327Z Reads: 273

```
I'm saying the plasti-dip will make it near impossible (if at all) to repair. I doubt anyone would even want to try as it's more trouble than it's worth. While it doesn't water-proof the VESC, using simple shrink wrap will protect the VESC from most situations involving water, when it's in an enclosure.
```

---
## \#114 Posted by: Hummie Posted at: 2017-07-25T01:05:47.572Z Reads: 285

```
U should get the best thermally conductive stuff u can. Think it's silicone.  Compare before and after temps on the Vesc data log and tell us!  I planned to pot the Vesc in some special expensive 3m "electronics potting" with some nice copper little heat sinks for each fet I got but it all still sits undone waiting for the future.  Supposedly not much heat generated elsewhere.  

I more so than waterproofing was interested in sticking it to the board.  Potting it to the board!  Damn I want to do this still. Waterproof and more important to me vibration/bang proof
```

---
## \#115 Posted by: thetechtrader Posted at: 2017-07-25T13:09:00.369Z Reads: 274

```
what part is the FET? and did you make heat sinks for them?
What 3M stuff were you going to use?
```

---
## \#116 Posted by: thetechtrader Posted at: 2017-07-25T13:37:02.706Z Reads: 271

```
does the VESC have a built int AntiSpark resistor or do we need an XT90-S anti spark plug?
```

---
## \#117 Posted by: TarzanHBK Posted at: 2017-07-25T13:52:29.168Z Reads: 273

```
no, you need an anti spark plug or switch
```

---
## \#118 Posted by: thetechtrader Posted at: 2017-07-25T15:56:49.746Z Reads: 286

```
Thank you.
How do I wire in an on/off switch like this?
<img src="/uploads/db1493/original/3X/f/2/f286216d3d28eaca2560c387737f3b55349d6e5c.JPG" width="375" height="500">
```

---
## \#119 Posted by: Hummie Posted at: 2017-07-25T16:55:36.503Z Reads: 284

```
The 3m stuff I looked for in my pile but will look again buy there's surely a bunch of options: You could just do the "conformial coating" instead of fill potting an that might suit u better. 
 The fets are the 6 bigger bits just before the motor wires with the flat surface. I just found small copper heat sinks that were a bit bigger than the Fets that stick on.
```

---
## \#120 Posted by: wafflejock Posted at: 2017-07-25T17:16:46.472Z Reads: 286

```
@lrdesigns <-- didn't you plastidip your VESC? how'd that turn out?
```

---
## \#121 Posted by: Jinra Posted at: 2017-07-25T17:18:44.694Z Reads: 303

```
you can check out what happens to a computer when you plastidip it. Thermal throttling everywhere!

https://youtu.be/JO4Zope7I84
```

---
## \#122 Posted by: lrdesigns Posted at: 2017-07-26T00:51:03.824Z Reads: 312

```
[quote="wafflejock, post:120, topic:2980, full:true"]
@lrdesigns &lt;-- didn't you plastidip your VESC? how'd that turn out?
[/quote]

No I used a spray on conformal coating that is silicone based. http://hken.rs-online.com/web/p/conformal-coatings/0831141/  I needed 100% water proof and don't have heat issues as I have a dual with total power limited to 1000w so the vescs get warm but not hot. You can get thermally conductive conformal coatings though. Seems to have worked so far. I went to extra level with heavy shrink wrap and hotglued the ends so its sealed. 2X water proof! The connectors have been removed as I didn't want the chance for water to get under them. Repairing them would be very hard, it can be scraped off but is resistant to most solvents. 

More extreme than most are willing to do :stuck_out_tongue_closed_eyes:
<img src="/uploads/db1493/original/3X/9/b/9b4198a0da274be719ae55a924d406a1f4e4f3be.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/e/ae1a6f3c3e56e5a6d66295a287acb61f6754c40c.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/3/c/3c99859bbee7c032bc05d7dcb729f45edf9b2bf6.jpeg" width="666" height="500">

https://www.youtube.com/watch?v=DfcbYbrS4TQ
```

---
## \#123 Posted by: Lionpuncher Posted at: 2017-07-26T17:00:18.182Z Reads: 298

```
Just wanted to thank you. Your explanations have made all the difference for me to get my head wrapped around the info needed to do a first build. Haven't really had to post any redundant questions on the forum because the info was so easy to find and understand. 
Chur bro.
```

---
## \#124 Posted by: thetechtrader Posted at: 2017-07-29T12:48:29.271Z Reads: 287

```
[quote="lrdesigns, post:122, topic:2980"]
conformal coatings
[/quote]

I searched for conformal coatings, amazon $61 CAD plus shipping, plus 3-5 week wait.... I I just went to a local hobby shop and go the exact bottle for $14.97. silicone conformal coatings is what I learned is best for reducing heat as well.
```

---
## \#125 Posted by: evoheyax Posted at: 2017-08-01T17:42:40.831Z Reads: 294

```
Just throwing this in here, since it's related.

http://www.electric-skateboard.builders/t/devins-vesc-settings-calculator-for-2-16-2-18-firmware/29020
```

---
## \#126 Posted by: nw-esk8 Posted at: 2017-08-16T19:54:32.042Z Reads: 293

```
Asked this over in the 'noob questions' thread, but didn't get any bites.  I thought it might be better to try over here:

----------------------------


Is it possible to wire up dual vescs in parallel for increased current to a single motor?

IE: dual motor setup w/ chained canbus'ed quad vescs with each motor having a master/slave (master=power+pwm+sensor, slave=just power).

If not, why? +Is this something that could be available via firmware in the future?  It seems like amps are the limiting factor w/ vescs, especially w/ 63mm, but that could be a potential stopgap solution until vescs catch up re: amp ratings... Just imagine >100a cont+FOC.  I haven't seen any evidence this is currently doable, but I don't know enough about VESCs to come up w/ a reason why it couldn't be.

If so, any info/examples on this?  I haven't had any luck and usually my google fu is strong.

edit:
it'd look exactly like this rendering:
<img src="/uploads/db1493/original/3X/8/e/8e378ec3b18f16c8c771df61aa8ca012898ad5f8.png" width="690" height="253">

...but w/ a canbus connection
```

---
## \#127 Posted by: nw-esk8 Posted at: 2017-08-17T04:45:27.131Z Reads: 271

```
Also, if VESCs support up to 60v, what is preventing people from running 13s (...or even 14s)?
```

---
## \#128 Posted by: onepunchboard Posted at: 2017-08-17T05:22:29.664Z Reads: 267

```
one vesc interrupt the other for current measuring for motor. so no it won't work. probably fry both vesc
```

---
## \#129 Posted by: onepunchboard Posted at: 2017-08-17T05:23:33.487Z Reads: 267

```
could be voltage spike prevention headroom. I'm just assumming tho
```

---
## \#130 Posted by: nw-esk8 Posted at: 2017-08-17T05:28:42.256Z Reads: 262

```
Thanks for the reply, but if it's not possible currently, I'm still not clear on why it couldn't be possible (if there was a master/slave canbus configuration for managing the current?  how would the current be interrupted?)
```

---
## \#131 Posted by: onepunchboard Posted at: 2017-08-17T05:37:04.917Z Reads: 260

```
I'm not expert on this but sensor in the motor only good upto first 1000 rpm after that esc have to measure current draw to calculate rotor position and predict for next current draw. if u put 2, well one or the other will detect abnormalities in measuring and try to correct it. I won't work
```

---
## \#132 Posted by: nw-esk8 Posted at: 2017-08-17T05:38:14.239Z Reads: 248

```
I can't think of anything pre-ESC that could cause a spike like that (except maybe a BMS that's catastrophically malfunctioning?)... especially at just 13s.  

If it wasn't so expensive to test... :slight_smile:
```

---
## \#133 Posted by: onepunchboard Posted at: 2017-08-17T05:39:35.120Z Reads: 243

```
same I really want to try erpm limit for my vesc but can't afford another one😥
```

---
## \#134 Posted by: nw-esk8 Posted at: 2017-08-17T05:40:10.019Z Reads: 245

```
...but isn't that kinda what CANbus is for?
```

---
## \#135 Posted by: onepunchboard Posted at: 2017-08-17T05:47:55.542Z Reads: 262

```
cuz 2 motor 2 vesc can draw exact math for rotor position and canbus is communication line. but if u use 1 motor there is no answer for vesc to draw out. unless some magic code or math can fill in the caos for two. I'm  just assumming from what I read bldc basics from Ti. so I could be wrong.
```

---
## \#136 Posted by: nw-esk8 Posted at: 2017-08-17T05:57:21.346Z Reads: 267

```
Did those other ESCs you read about support CANbus though :) ?  I'm guessing they may have also said you have to split the receiver PPM signal for multiple ESCs? 

AFAIK canbus can transfer 1 MB/s AND I believe it supports full duplex communication... which seems like it would be **_more_** than enough to allow the master VESC recieve/calculate/send instructions to the slave (based on both ESCs current...receiver input, etc, etc).

I know I keep poking, but I am hoping to know definitively if it isn't possible... even if it hasn't been supported in the past.
```

---
## \#137 Posted by: onepunchboard Posted at: 2017-08-17T06:03:44.581Z Reads: 263

```
it sounds plausible. but I haven't  seen one yet
```

---
## \#138 Posted by: HubBoard Posted at: 2017-08-18T15:49:54.407Z Reads: 269

```
I have read about vesc and could't find any information on how to connect more than 2 motors.

I am building 4WD configuration, already got 4 Vesc's. There are information how to connect 2 motors by 2 vesc controllers in parrarel connection, one Master, one Slave with BLDC tool, but I was wondering how to connect 4 of them?

One of them as master and 3 slaves? And how to connect 4 vesc with just both, two-way can bus connector?
```

---
## \#139 Posted by: evoheyax Posted at: 2017-08-18T20:08:54.496Z Reads: 278

```
It's the same concept as 2wd.

VESC 1: controller id = 0, under ppm, multiple vesc's over esc is enabled.
VESC 2: controller id = 1, under app, send status over can is enabled.
VESC 3: controller id = 2, under app, send status over can is enabled.
VESC 4: controller id = 3, under app, send status over can is enabled.

This is how I ride with no issues. All is great!
```

---
## \#140 Posted by: wmj259 Posted at: 2017-09-16T19:23:00.609Z Reads: 270

```
Can't find the link for the old bldc tool software. Anyone know the link? Not the FOCBOX or VESC6 tool.
```

---
## \#141 Posted by: raven Posted at: 2017-11-12T06:49:05.403Z Reads: 257

```
I used my 3s pack to power my vesc. It didn't work unfortunately. Then I took out my 10s from Enertion. Straight away kicked into action but I have some firmware problems so need to fix that
```

---
## \#142 Posted by: Blitz Posted at: 2018-01-21T20:54:57.057Z Reads: 252

```
[quote="evoheyax, post:1, topic:2980"]
sellers like Torque Borads, Enertion, Axle, Esk8.de, or Chaka.
[/quote]

Iv'e bought focbox from a group buy. Could that mean that it has not been powered on?
```

---
## \#143 Posted by: MannyM0E Posted at: 2018-01-22T03:32:31.958Z Reads: 241

```
So does the vesc keep tracks of distances or like hour use ? Reason asking because I would like too know how much mile I've put into the board..
```

---
## \#144 Posted by: evoheyax Posted at: 2018-01-22T04:28:48.600Z Reads: 237

```
You can use the vesc to do this. You will need to use either a smart phone app or create your own app of some sort to display it. It's all open source, so it's all up to you.
```

---
## \#145 Posted by: evoheyax Posted at: 2018-01-22T04:29:17.359Z Reads: 236

```
All focboxs have been powered on and tested. That's just part of their process.
```

---
## \#146 Posted by: Ingvarjedi Posted at: 2018-02-02T08:21:11.972Z Reads: 223

```
Hi people.
I used VESC  from diyelectricskateboard. 

VESC BLDC ELECTRIC SKATEBOARD ESC FEATURES
Built in 5V BEC (Used to power your receiver.)
Voltage: 8V to 60V (Up to 14S LiPo Voltage)


This is realy 14s LiPo?? 
What safety voltage Li-Po can I use to not fry VESC with used motor 192kv-12s?
```

---
## \#147 Posted by: b264 Posted at: 2018-02-02T08:31:42.924Z Reads: 218

```
[quote="evoheyax, post:144, topic:2980"]
It’s all open source, so it’s all up to you.
[/quote]

None of the software [from the enertion web app](http://www.enertionboards.com/FOCBOX-speed-controller.html) is open-source.
```

---
## \#148 Posted by: TarzanHBK Posted at: 2018-02-02T08:34:19.109Z Reads: 221

```
For 192kv safe is 10s
12s gets critical and could cause drv errors with this motor with a standard 4.12.

12s with a standard vesc is as high as you should go, 13s is possible, but should only be used if you really know what you´re doing, have all settings in the right place and know how to properly cool everything.

14s will pop, as soon as you have the first voltage spike with a little bit of braking for example.

If you´re new to Vescs, you should go the safe 10s spot to save your components.
```

---
## \#149 Posted by: Ingvarjedi Posted at: 2018-02-02T08:40:08.138Z Reads: 229

```
Ok. Then this motor will not work fully efficiently? Can be used 245kv-10s motor with 10s Li-Po?

Yes. I'm new in  VESC. I'm in the process of studying.))

when I brake, does the voltage rises?
```

---
## \#150 Posted by: TarzanHBK Posted at: 2018-02-02T08:48:01.324Z Reads: 238

```
Here you´ll find the matching motors to cellnumbers:

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

And yes, during regenerative braking, the voltage rises above battery level, so you have to make sure your components are rated high enough and have a bit of play to handle these spikes
```

---
## \#151 Posted by: Ingvarjedi Posted at: 2018-02-02T08:55:50.558Z Reads: 231

```
I read it. there are many contradictions. this is confusing 😂😂😂😂
```

---
## \#152 Posted by: TarzanHBK Posted at: 2018-02-02T08:56:57.622Z Reads: 237

```
Just get a 10s with 190kv motor and you´ll be fine ;)
Also take your time to read through some of the buildsthreads and you´ll find out what other people are running.
```

---
## \#153 Posted by: amitbt69 Posted at: 2018-02-04T06:31:05.401Z Reads: 244

```
Great post! thanks
```

---
## \#154 Posted by: buckhr Posted at: 2018-02-14T14:54:13.533Z Reads: 258

```
I'd like to add some more info to the Windows configuration and setup details:

Here's a public link to the BLDC tool for Windows: [link](https://drive.google.com/file/d/0B86q1vsoI_CCd0RZMGlYSmF0c0E/view?usp=sharing)
Here's a public link to software containing the necessary drivers: [link](https://drive.google.com/file/d/1ExPn1c8RwVzrUD6KLfN9CuYYhuIXOlom/view?usp=sharing)

Install both of the above applications.  The Teensyduo program is actually an arduino-based tool (which isnt really necessary) but it contains the right drivers necessary for the BLDC tool to be recognized as a COM port via USB.

Once both applications are installed, power up your VESC (via battery or power source) and plug it in using a mini USB _which can carry data_ ([like this one on Amazon, $5](https://www.amazon.com/gp/product/B00NH11N5A/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1)).  I struggled with three different mini USB cables for a while trying to understand why computer wouldnt recognize the VESC or COM port, and it was because I was using old, generic mini USB cables that I had from previous devices which only carried a charge and couldnt handle data transfer.  If you're using the right cable, when the VESC is plugged in and powered on you should see a new COM connection in device manager:

![image|682x500](upload://8UrpCW1TnwjZc9kyApyIeBmcaGY.png)

The STMicroelectronics Virtual COM Port is the VESC.  You need to note the (COM#) at the end of the title  because that is the COM port you will use to connect to through the BLDC tool.

Now that your VESC is recognized by Windows as a virtual COM port, all you need to do is go into the BLDC tool and select the COM port identified above and you should be able to connect!

![image|690x407](upload://ofOEk2lfoO8TWtumbbfUQnywYu7.png)

You can also change the COM ports for the virtual COM in the Device Manager if there is a conflict or if you just want to:

Right click COM port in Device Manager -> Port Settings -> Advanced -> COM Port Number -> Change to whatever you want

I hope this helps someone else!
```

---
## \#155 Posted by: MaxMaker Posted at: 2018-05-25T09:15:59.418Z Reads: 194

```
Hi all, 

I have a real problem with my brandnew VESC 6.4. It shuts down after connecting to VESC Tool over USB. It establishes a connection and displays its firmware in green at the bottom right corner, but then it kinda shuts down a few seconds later. The LEDs turn off completely, and only by powering it on and off come back to live. 

Any ideas how to solve this? I tried with 0.92, 0.94 and on two computers, MAC and PC.
```

---
## \#156 Posted by: TarzanHBK Posted at: 2018-05-25T09:48:08.587Z Reads: 198

```
I´m sure @trampa helps you out with it, i don´t know what should cause that if you don´t have any trouble with your power supply
```

---
## \#157 Posted by: MaxMaker Posted at: 2018-05-25T10:09:34.258Z Reads: 200

```
My power supply is set to 30V and maximum 3A. I am in contact with them. I hoped there would be an easy solution instead of sending it back.
```

---
## \#158 Posted by: TarzanHBK Posted at: 2018-05-25T10:14:00.913Z Reads: 204

```
If it behaves strange like that, it´s better to get it checked by them.
```

---
## \#159 Posted by: trampa Posted at: 2018-05-25T11:30:21.355Z Reads: 199

```
Try a battery please. A 3S Lipo would be good.

Frank
```

---
## \#160 Posted by: MaxMaker Posted at: 2018-05-25T12:12:08.085Z Reads: 206

```
Hey, I tried. Same thing. I took a video. First with and then without USB.

http://www.youtube.com/watch?v=CGZxkgRnqNs
```

---
## \#161 Posted by: trampa Posted at: 2018-05-25T12:25:16.609Z Reads: 196

```
Try a simple setup, batteries directly to VESC, only a fuse in between.
```

---
## \#162 Posted by: MaxMaker Posted at: 2018-05-25T12:59:11.661Z Reads: 190

```
Thats what it is. There is only a fuse between the batteries and the VESC and the giant relay. The Arduino, Buttons and Display are only there to control the Relay.  

I also tried connecting the power supply straight to the short cables on the VESC last night without any other electronics attached. I got the same result. The bench power supply can output up to 32V at 5 A, but it doesn’t even come close to that current.
```

---
## \#163 Posted by: JohnnyMeduse Posted at: 2018-05-25T13:00:54.173Z Reads: 190

```
Can you check the 5v rail
```

---
## \#164 Posted by: MaxMaker Posted at: 2018-05-25T13:34:24.915Z Reads: 197

```
How? I don’t feel like opening up the case for fear of breaking the heat sink connection.
```

---
## \#165 Posted by: trampa Posted at: 2018-05-25T14:33:49.757Z Reads: 207

```
You can measure the voltage on the 5V pins and on the 3.3V pins if you have a voltmeter.

We do a full spin-up test with each device. 12S Voltage + USB connectivity checked + automatic motor setup wizard + FOC and BLDC motor spin-up. Our test bench compares all values to reference values to see if there are any deviations from the norm. If the firmware is on the device, it has passed all tests and should work just fine. If you can't spot the issue, please get back to us via mail. We will sort it out for you and make sure you will get a working device. 

Frank
```

---
## \#167 Posted by: MaxMaker Posted at: 2018-05-25T17:32:54.832Z Reads: 208

```
I measured 2.8V on the PPM and on the CAN ports (each separately). It says 5V on the screen print though.
```

---
## \#168 Posted by: JohnnyMeduse Posted at: 2018-05-25T17:40:02.655Z Reads: 216

```
Look like something is wrong with the Drv or over the 5v leg...
```

---
## \#169 Posted by: MaxMaker Posted at: 2018-05-25T18:52:44.990Z Reads: 216

```
Can I replace that at home? Send it to Trampa?
```

---
## \#170 Posted by: Travo Posted at: 2018-07-15T20:32:53.025Z Reads: 193

```
Could someone help me, I think I bricked my vesc some how? I've tried 2 computers and two USB cables one long one short and nothing happens. The vesc connects to the PC and "installs hardware" but you cannot locate it under the PC icon and when using the vesc tool it says no ports found. The lights on the vesc light up so I wasn't sure if I screwed something up or my cables or PC is bad
```

---
## \#172 Posted by: BarbaraZ Posted at: 2018-07-16T03:24:16.236Z Reads: 189

```
Hi Travo, maybe you can try to check if your computer lacks some driver, just like stmicroel viritul drive. :wink:
```

---
## \#173 Posted by: Skunk Posted at: 2018-07-16T03:46:00.486Z Reads: 195

```
Oh boy. Another thread i need to read 4 times.
```

---
## \#174 Posted by: Travo Posted at: 2018-07-16T16:20:08.027Z Reads: 197

```
Okay will do
```

---
## \#175 Posted by: MD84 Posted at: 2018-10-25T03:08:13.695Z Reads: 152

```
I have a question about the receiver input. I have a typical hobby receiver.  Do I plug the servo cable into the throttle channel for pwm or the bat bind channel for ppm?

What other types of control inputs are available?
```

---
## \#176 Posted by: aidandf Posted at: 2018-12-24T03:14:15.124Z Reads: 133

```
Is there an esc that is can be programed with the FOCBOX BLDC Tool that is compatable with a 12s motor at 110A?
```

---
## \#177 Posted by: Lincon Posted at: 2019-05-24T02:25:28.456Z Reads: 81

```
Hello everyone,,,
The belt is fine, if you can take your hand, and spin the wheel without great difficulty. The belt should make it slightly harder to spin , but not too hard to spin. You https://xvideos.onl/ should run the detection with the belt attached.https://xnxx.onl/  But most importantly, it should be able to spin without any load, as when you click on detect motor button, it will do a series of tests that will make the motor spin. If you have load or even if the wheel is touching the ground, it will fail detection, as the motor can’t spin freely.
```

---
## \#178 Posted by: Namasaki Posted at: 2019-05-24T02:32:59.875Z Reads: 83

```
I have always believed that it is best to do motor detection without belts or without wheels on a direct drive. 
This is how I have always done mine and never had an issue. 
I have always thought that added drag on the motor could alter the outcome of the detection.

Would anyone else care to voice your opinion on this?
```

---
## \#179 Posted by: UnoTheHippo Posted at: 2019-07-04T09:45:45.343Z Reads: 61

```
Hi,
What would it mean if my voltage reading on my vesc is unstable. It keeps flacuating. Which messes up with a lot of readings as you could imagine. I used a multimeter, but its reading is stable. 
Thanks, 
Sam
```

---
## \#180 Posted by: DanielJohn Posted at: 2019-10-28T09:28:30.434Z Reads: 30

```
Hey,

Does anyone have any experience connecting the Flipsky VX1 with the Tourqueboards VESC?

I'm not usre which connector to use when attaching the reciever.

Cheers!

![73524504_403198637257902_7858116501708996608_n|373x500](upload://px5rlbvamANbUyVQ7Nf7cv86vDn.jpeg)
```

---
