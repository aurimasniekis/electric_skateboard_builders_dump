# FatBoy HV ESC - 18S 150A Electric Speed Controller

### Replies: 111 Views: 5468

## \#1 Posted by: Kug3lis Posted at: 2018-06-29T22:44:27.586Z Reads: 542

```
Hi guys, after designing, and redesigning the design we finally reached the point where we kinda have almost semi-final design which we will start testing soon on the boards :)

So let me introduce you to the new FatBoy family member **HV ESC**

# FatBoy HV ESC

<img src="https://www.electric-skateboard.builders/uploads/db1493/original/3X/c/e/cec862807a59313e1e019121580369258327ee51.jpg"/>

<img src="https://www.electric-skateboard.builders/uploads/db1493/original/3X/0/a/0a56f1e42abd3dd82bbab2640ce92a1f53b252fe.jpg"/>

## Hardware Features:

* STM32 microprocessor
* DirectFET mosfets
* Independent Gate Drivers / Current Amplifiers
* Hall / Rotary Encoder support
* CAN/UART interface
* Voltage 4S-18S (15V - 80V absolute maximums)
* Current up to 100A - 150A

This ESC will be available in single/dual configuration and will be using our CNC machined aluminium cases for outside/inside enclosure mounting with high-efficiency heat dissipation which allows us to provide higher constant currents.

## Software

At the moment it is still in development but several hints it will be based on FreeRTOS and motor control libraries which would allow more precise sensored / sensorless applications. 

For the prototyping and first devices, I have adapted VESC firmware to run on my hardware design.

https://github.com/aurimasniekis/fatboy-vesc

## Current project status:

Today we have received parts and PCB, soldered power and MCU stage everything looks fine will continue tomorrow and after we make aluminium cases for it I will begin testing in the field in my projects afterwards we will begin beta tests with several people and later on if everything is successful will be available to purchase from our online store.

<img src="https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/6/e/6edede8fc0045d5b6bf0bd989ccd922137f73f8e_1_375x500.jpg"/>

![image|375x500](upload://qyAJU1uQScIp1snpENxPpQu5Xqm.jpg)

![image|375x500](upload://tQWkhnl2sbfYLQmCDKOOhb3757I.jpg)

![image|375x500](upload://i2i0DqOzCKuqoyf4TCx7dao3Bvv.jpg)
```

---
## \#2 Posted by: Jc06505n Posted at: 2018-06-29T22:48:24.079Z Reads: 484

```
Looks awesome , what distinct advantages/ improvements will this have over VESC’s ? Will this be your “Jarvis/Friday” for your Mark 48?
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-06-29T22:52:44.268Z Reads: 478

```
One if the biggest I guess "DRV-less" design, independent power supply from gate drivers and etc. Higher voltage support. Software wise I am using industrial level software components with algorithms used in enterprise applications so it should be much smoother and better control loops.

Yes, I will be using these as 18S ESC on my Mark 48 as "booster controllers" :joy:
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-06-29T22:57:00.089Z Reads: 465

```
[quote="Kug3lis, post:3, topic:60463"]
Yes, I will be using these as 18S ESC on my Mark 48 as “booster controllers” :joy:
[/quote]

Can’t tell if this is a joke because you are an absolute madman. Been killing it in the innovate game. Excited to see you progress. Absolute great job man
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-06-29T22:58:37.365Z Reads: 451

```
I was nurturing this design since last October and just finally got moving on faster after I started working on Mark 48 project :) But because of my own lack of resources I transferred all prototyping work to my father who is assembling them now ;)
```

---
## \#6 Posted by: SeanHacker Posted at: 2018-06-29T23:01:54.295Z Reads: 432

```
@Kug3lis 

With the way you've come in here and done what you have so far, I have a strong feeling you're going to be the next Vedder. Thanks for everything you've brought to the table here so far! I'll buy whatever you come out with!
```

---
## \#7 Posted by: Blacksheep Posted at: 2018-06-29T23:03:28.648Z Reads: 427

```
Can I get on te beta testing?
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-06-29T23:03:48.943Z Reads: 432

```
Thanks for the kind words :) I just like to create things and with help with my father we make those ideas reality :)

P.S. Who don't remember first versions of this esc :smiley:

https://www.electric-skateboard.builders/t/daily-driver-v2-0-35-holypro-trampa-vertigo-trucks-aps-6384s-170kv-4kw-fatboy-inner-gear-direct-drive-12s-custom-esc/36560/9?u=kug3lis
```

---
## \#9 Posted by: E1Allen Posted at: 2018-06-29T23:09:02.477Z Reads: 422

```
Sign me up!

I will punish the ESC
```

---
## \#10 Posted by: rojitor Posted at: 2018-06-29T23:14:44.665Z Reads: 408

```
:heart_eyes: amazing!!!
```

---
## \#11 Posted by: Silverline Posted at: 2018-06-29T23:24:57.420Z Reads: 402

```
Dual esc with heatsink... i`m in....
This is next level..... Once again, DIY is raising the bar... Boosted, evolve and others, no thanks.... It`s just toys

Glad to se the "next Vedder" is actually on the forum, where everything happens.
```

---
## \#12 Posted by: Grozniy Posted at: 2018-06-29T23:31:03.369Z Reads: 389

```
Awesome idea ;) How much would dual cost?
```

---
## \#13 Posted by: Skunk Posted at: 2018-06-29T23:37:05.919Z Reads: 390

```
Was just about to order a set of focbox....
Maybe I'lll just wait.
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-06-29T23:41:08.164Z Reads: 390

```
I don't think it will see day light in 1-2 months for sure... Regarding the price I can tell it will be for sure more expensive than ESCapes as gate drivers and etc cost a bit more plus it will come with the case...

Also there are some discussion regarding making single unified connector based on XT90 design for motors and sensor wire :)
```

---
## \#15 Posted by: Cobber Posted at: 2018-06-29T23:57:22.329Z Reads: 378

```
(18*4.2v)*150a = 11340w :open_mouth:
```

---
## \#16 Posted by: E1Allen Posted at: 2018-06-29T23:59:26.229Z Reads: 378

```
More like 10kw at nominal if you account for voltage sag.  Still quite a bit.
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-06-30T00:00:41.811Z Reads: 389

```
Yeah, it should peak at around 10kW, but idea the higher voltage less current you need to consume to produce the same power :) That's it will be coming with fully fledged case so it could handle those currents without going into melting :D

For e.g. same 4kW would require only 50A @ 18S instead of 80A
```

---
## \#18 Posted by: Cobber Posted at: 2018-06-30T00:12:06.226Z Reads: 383

```
[quote="E1Allen, post:16, topic:60463"]
10kw... [per wheel] ...Still quite a bit
[/quote]

Ya think :joy:

[quote="Kug3lis, post:17, topic:60463"]
it should peak at around 10kW
[/quote]

What sort of constant wattage (amp/voltage) out put do you predict Kugy?
```

---
## \#19 Posted by: Kug3lis Posted at: 2018-06-30T00:13:10.568Z Reads: 373

```
Cant tell you nothing without real life testing :/
```

---
## \#20 Posted by: Cobber Posted at: 2018-06-30T00:25:50.521Z Reads: 377

```
What guage or cross section (mm2) wire are you going to use?
```

---
## \#21 Posted by: Kug3lis Posted at: 2018-06-30T00:28:38.677Z Reads: 356

```
Don't know yet, but it's not intention of making it full current capable out of the box I mean even xt90 will be problem short term runs of full current should be more than enough I personally can't get more than 3kW to be consumed no matter hills I tried...
```

---
## \#22 Posted by: E1Allen Posted at: 2018-06-30T00:49:41.824Z Reads: 343

```
U talking about with current vesc?
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-06-30T00:50:46.741Z Reads: 342

```
Yes

10char
```

---
## \#24 Posted by: E1Allen Posted at: 2018-06-30T01:07:00.415Z Reads: 340

```
I Hear ya.  On dual setup I've managed 5kw battery and almost 6.5kw motor.  Only for bursts because the acceleration is crazy.  18s with lower amp requirements will be nice.  Plus the extra rpm/v for the speeds.  I'm thinking burnouts...
```

---
## \#25 Posted by: pat.speed Posted at: 2018-06-30T01:25:09.730Z Reads: 341

```
Yes speed, this accompanied with @MoeStooge’s WR murder board and ngv will be left in smoke.

@Kug3lis is there a erpm limit with your design?
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-06-30T01:27:00.418Z Reads: 338

```
Dont know yet, have to try it out
```

---
## \#27 Posted by: JdogAwesome Posted at: 2018-06-30T04:16:36.237Z Reads: 345

```
Looks great man! Always nice to see new speed controllers on the market, we need some variety lol! Just curious though on what you think the continuous output current of these ESC's will be? Also any chance you could disclose what FET's your using, im assuming the IRF7769 as they are 100V rated and are DirectFET's, problem is there not in stock anywhere, how do you plan to address the high performance DirectFET stock shortages?
```

---
## \#28 Posted by: hyperIon1 Posted at: 2018-06-30T04:44:43.665Z Reads: 356

```
Excellent work, I really like your innovative approach. I think a variety of independent esc’s will keep the industry moving forward.
```

---
## \#29 Posted by: 3DServisas Posted at: 2018-06-30T09:28:34.784Z Reads: 353

```
![IMAGE%202018-06-30%2012%3A28%3A13|375x500](upload://xowsGrwMJTXEwewfoaDtaPY0hL.jpg)![IMAGE%202018-06-30%2012%3A28%3A16|375x500](upload://zlz1hK0WTwjQxvubuQlinp1YYbb.jpg)
```

---
## \#31 Posted by: Kug3lis Posted at: 2018-06-30T10:53:18.408Z Reads: 339

```
All higher voltage DirectFET's has no shortage problems ;)
```

---
## \#32 Posted by: uigiroux Posted at: 2018-06-30T11:21:53.515Z Reads: 341

```
Is this about the same size as an ESCape? Love what your doing here!! :heart_eyes:
```

---
## \#33 Posted by: Kug3lis Posted at: 2018-06-30T11:34:16.221Z Reads: 338

```
It's bit bigger 65x70
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-06-30T13:34:53.943Z Reads: 340

```
Got the software running :slight_smile:

![05%20PM|690x440](upload://kpDqlPCblJK8RCQLmkO9mjM30bC.png)
```

---
## \#35 Posted by: uigiroux Posted at: 2018-06-30T13:46:19.199Z Reads: 337

```
Able to post any video of it working with 18s battery? Or is that a ways away?
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-06-30T13:47:11.224Z Reads: 335

```
light years away :D We are just getting into trying to connect motor
```

---
## \#37 Posted by: uigiroux Posted at: 2018-06-30T13:55:15.091Z Reads: 339

```
Damn bro you are so brilliant with all your Esk8 products!!! You gonna be making a MCU for everything to connect too that'll basically run and coordinate everything?
```

---
## \#38 Posted by: Surfer Posted at: 2018-06-30T14:17:53.671Z Reads: 342

```
That's is awesome!! And you too!
```

---
## \#39 Posted by: JdogAwesome Posted at: 2018-06-30T15:05:50.807Z Reads: 339

```
Will you look at that your right lol! I dont know what I was looking at where I was seeing that they where out of stock, woops. Anyways you have any idea on the continuous current output of the ESC? And how much heat do you think the heatsink this will be enclosed in will be able to sink? Also do you plan to go the FOCBOX route of more thermal mass vs surface area, and will there be a fan or a mount for one? I know a lot of questions im just curious!
```

---
## \#40 Posted by: jens_c Posted at: 2018-06-30T15:10:30.257Z Reads: 330

```
this would be perfect for an ebike
```

---
## \#41 Posted by: Pedrodemio Posted at: 2018-06-30T15:23:25.562Z Reads: 327

```
Nice project @Kug3lis

I think you should advertise this on ebike fóruns, this solve the VESC problem of low voltage compared to what is usually used. It will be the holy grail for them, really small and more power than most controllers that are much bigger, it even beats the compact controller from ebikes.ca I think
```

---
## \#42 Posted by: uigiroux Posted at: 2018-06-30T16:10:45.173Z Reads: 322

```
@Kug3lis you could also advertise this towards the e-foil forum where they make electric powered surf boards and foils.  Would be so perfect for those since they really could benefit from the use of properly powered 80mm motors...
```

---
## \#43 Posted by: banjaxxed Posted at: 2018-06-30T16:12:24.878Z Reads: 314

```
Oh dear, up to my neck in 4.12, Focboxes & ESCapes & you do this? Shame on you

Sign me up
```

---
## \#44 Posted by: AgileCow Posted at: 2018-06-30T16:28:09.109Z Reads: 313

```
Looks sick! :slight_smile:

Sign me up for when the testing begins, if it is in a couple of months that would be perfect to test on my offroad board  in the autumn :slight_smile:


Good job!
```

---
## \#45 Posted by: uigiroux Posted at: 2018-06-30T16:58:38.338Z Reads: 309

```
Same, I'll be down for 2 for sure!
```

---
## \#46 Posted by: Ebisane9 Posted at: 2018-06-30T17:14:11.094Z Reads: 309

```
you're never gonna start your build lmao.
```

---
## \#47 Posted by: Kug3lis Posted at: 2018-06-30T17:15:22.569Z Reads: 299

```
I need this for my build so... :D Plus I have already many parts coming in ;)
```

---
## \#48 Posted by: Ebisane9 Posted at: 2018-06-30T17:15:57.005Z Reads: 306

```
lmao not you! talking about @uigiroux
```

---
## \#49 Posted by: uigiroux Posted at: 2018-06-30T17:56:44.106Z Reads: 310

```
Lol well it's taken awhile but I've already started my build, I'll start a build thread once I'm closer to finishing it.

And just FYI, I'd of finished a long time ago, but many parts that I'm using are taking forever to get made.  I don't complain about it as it seems to be just a part of doing things DIY, but I hardly think that because I am taking my time and making sure to order the best parts only,  that I should be a punch line in a joke about never getting a Esk8 built.  I easily could have built a pos with cheap parts by now, but I'm one who researches tremendously about items before purchase, and many items are only offered from members of the forum, so I'm waiting for quality.
```

---
## \#50 Posted by: Ebisane9 Posted at: 2018-06-30T18:33:10.417Z Reads: 301

```
sweet. 4WD?
```

---
## \#51 Posted by: uigiroux Posted at: 2018-06-30T19:10:50.113Z Reads: 297

```
Not for this build.  I've decided to take others advice and build a 2WD first.  I may go 4WD some day, but I don't want to spend that much extra for a 4WD build at the moment..
```

---
## \#52 Posted by: karma Posted at: 2018-06-30T20:48:03.338Z Reads: 303

```
[quote="Kug3lis, post:1, topic:60463"]
At the moment it is still in development but several hints it will be based on FreeRTOS and motor control libraries which would allow more precise sensored / sensorless applications.
[/quote]
What motor control libraries are we talking about?
```

---
## \#53 Posted by: Rinzler Posted at: 2018-07-01T09:10:55.760Z Reads: 291

```
The e-foil people will go crazy for this, maybe try making a thread at http://efoil.builders/ if you want to. The e-foil people cash out a lot more on esc and their builds in total, so that might help you when you are taking your first batch orders to keep the cost down. Just made a profile there, i now know how a beginner feels on this forum :joy: Also super pumped about innovation on this forum, the e-foil forum is kinda dry.
```

---
## \#54 Posted by: AreaKruzer Posted at: 2018-07-01T15:03:43.190Z Reads: 284

```
Looking really good and promising.
```

---
## \#55 Posted by: banjaxxed Posted at: 2018-07-01T17:08:48.959Z Reads: 277

```
That’s very true, hey @Msk8 this could be a game changer for efoil
```

---
## \#56 Posted by: SeanHacker Posted at: 2018-07-01T17:14:53.017Z Reads: 279

```
I forgot to mention before @Kug3lis. You have a really cool Dad! Mine would just tell me to fuck off and show him the money first. Haha. You guys are perfect for this industry (and many others).
```

---
## \#57 Posted by: Msk8 Posted at: 2018-07-01T19:08:17.572Z Reads: 275

```
Absolutely, thanks for mentioning. We need high power ESCs for the electric hydrofoils. Since we are in water, many of us salt water, we don’t want to go much above 12S for saftey reasons. But we need ESCs that can handle high load. We draw high amps at start before foiling, many of our builds well over 100A, especially with direct drive systems we are experimenting with, like jet drives or low kV propped motors without gears. Please join us at efoil.builders if you are interested and let’s make sure we cross references these threads. Thanks.
```

---
## \#58 Posted by: ducktaperules Posted at: 2018-07-01T19:24:25.455Z Reads: 276

```
[quote="Kug3lis, post:14, topic:60463"]
single unified connector based on XT90 design for motors and sensor wire
[/quote]

I need this in my life.
```

---
## \#59 Posted by: sk8l8r Posted at: 2018-07-01T20:30:25.780Z Reads: 274

```
[quote="Blacksheep, post:7, topic:60463, full:true"]
Can I get on te beta testing?
[/quote]

@Kug3lis me too!  :slight_smile:

Edit: my 16s madness can become reality lol
```

---
## \#60 Posted by: banjaxxed Posted at: 2018-07-01T22:50:16.395Z Reads: 273

```
Paging @Deckoz, come in @Deckoz 

Sooooo, what motors could use say 14s more effectively than 12s, safety concerns? 

The efoil guys do go for these bigger voltages which can be dangerous in salt water since with dc it’s not possible to break the shock and you can drown

a/c as anyone who has done something dumb at home; and I’ll include myself in that, you can break the shock pretty easy
```

---
## \#61 Posted by: PredatorBoards Posted at: 2018-07-01T22:59:46.817Z Reads: 274

```
Was wondering when I was gonna hear more news about this project after you posted that teaser in the picture only thread. Congrats! Is there going to be a programming tool that you developed on your own? Do you think there will be an alternative VESC firmware fork available?
```

---
## \#62 Posted by: Kug3lis Posted at: 2018-07-01T23:21:58.604Z Reads: 272

```
Yes, there will be one browser based so you will not need any drivers / tools to download. For VESC to be able to work with it, it would need to change the way it communicates with computer :) VESC at the moment uses USB Virtual Serial Port which is not available at the moment to use with WebUSB standard as nobody implemented way to simulate serial port communications via raw usb packets while in my firmware I am using direct USB communication for which I use WebUSB to communicate to it.
```

---
## \#63 Posted by: PredatorBoards Posted at: 2018-07-02T00:54:51.412Z Reads: 271

```
Sounds really promising! What directFETs are you using to meet these power figures?
```

---
## \#64 Posted by: Deckoz Posted at: 2018-07-02T01:00:08.049Z Reads: 283

```
[quote="banjaxxed, post:60, topic:60463"]
Sooooo, what motors could use say 14s more effectively than 12s, safety concerns?
[/quote]

14s not much more than 13s.. 6374 would be fine in fall/spring with sub 65 temps..but heat in higher temps needs mass, I'd probably say 8072 or 80100 for summer high voltage high kv wind or some type of inrunner water-cooled in a smaller format...

That is if you are planning to use the entire speed envelope of your gearing... If not 6374 do just fine for summer cruising
```

---
## \#65 Posted by: banjaxxed Posted at: 2018-07-02T05:58:03.447Z Reads: 279

```
[quote="Kug3lis, post:17, topic:60463"]
same 4kW would require only 50A @ 18S instead of 80A
[/quote]

Thanks for this info, possible then to make smaller packs with less current, interesting possibilities here.

I’m thinking ATB dual 6384 direct drive 5:1 with 9” tires, that’s my destination.

...And an ehovercraft
```

---
## \#66 Posted by: banjaxxed Posted at: 2018-07-02T06:28:36.121Z Reads: 276

```
Funnily enough heat is becoming a problem where I am at the moment, I like the idea of using an overvolt to overcome a lack of amps that could be an interesting thing in the hill climb stakes with a smaller parallel pack
```

---
## \#67 Posted by: blezalex Posted at: 2018-07-02T16:30:47.622Z Reads: 270

```
@Kug3lis, I have a perfect application to try your controller. I'm building  a large version of self-balancing one-wheeled board. My first version is using VESC, but 60v is a big limitation for larger version. Motor tracking under heavy load was also a problem with VESC. That is where your improved algorithms could shine. 

I've been looking for a controller that could handle 72v and have very fast tracking and current control + foc. 

Self balancing requires at least 100hz control loop and I could not find any controller meeting those criteria on the market. https://www.roboteq.com/index.php/component/virtuemart/369/rgbl1896-detail?Itemid=970 the only thing i could find. it is huge, heavy and too expensive. 

Here is me riding my v1 https://www.youtube.com/watch?v=4-E7deaGyFs
The next version is a lot bigger https://photos.google.com/share/AF1QipPO78TzYYgQhJqzmjaNSFoXNritETvh-AQ7qblW5T9r_-F3rVFOC8KurQlnfdjCbA?key=U2hEZVhLbFhpRjYxeG1Zc0UtbFNEWGViY3lHVmdB 

:)
```

---
## \#68 Posted by: PredatorBoards Posted at: 2018-07-02T17:12:46.216Z Reads: 256

```
Not to detract, but do you have a build thread? Would love to read about how you went about the design phase. 

Edit: Forgot to add. The A200S VESC might be a good stepping stone until the Fatboy HV becomes available. It's 16S 200A. I think it's available for 500-600 ish.
```

---
## \#69 Posted by: E1Allen Posted at: 2018-07-02T17:17:01.978Z Reads: 255

```
A200s is pre-order for the second 20, it's probably going to be 480GBP with shipping.  It can also handle 18s
```

---
## \#70 Posted by: Holyman92 Posted at: 2018-07-02T17:41:59.906Z Reads: 264

```
i feel like @MoeStooge could benefit from this....
```

---
## \#71 Posted by: b264 Posted at: 2018-07-02T18:04:00.349Z Reads: 266

```
[quote="banjaxxed, post:65, topic:60463"]
direct drive 5:1
[/quote]

If it's 5:1 then it's not direct drive.  You might be thinking of a gear drive
```

---
## \#72 Posted by: banjaxxed Posted at: 2018-07-02T19:03:22.278Z Reads: 260

```
Well there is that old potato to keep digging up true
```

---
## \#73 Posted by: blezalex Posted at: 2018-07-02T20:53:42.005Z Reads: 268

```
I did not do a build thread. I posted some info in intro thread some time ago: https://www.electric-skateboard.builders/t/new-member-introduce-yourself-here-tell-us-your-plan/216/814?u=blezalex
It has links to github and some more pictures. 

Thanks for pointer to The A200S VESC . Does it run the same VESC firmware? I need FOC and current control.
```

---
## \#74 Posted by: hexakopter Posted at: 2018-07-02T21:27:54.317Z Reads: 281

```
[quote="PredatorBoards, post:61, topic:60463"]
Do you think there will be an alternative VESC firmware fork available?
[/quote]


When you are asking if his own motor control firmware will be open source then the answer will be yes I think. That is what @Kug3lis wrote in the past. 

[quote="Kug3lis, post:49, topic:40375"]
I have been OS developer for over a decade now…
[/quote] 

[quote="Kug3lis, post:81, topic:40375, full:true"]
Your all this talk makes me want to go fork the code rewrite from scratch (I was intending to do because there are newer chips which are cheaper) Make it completely MIT proof and then release to the public and then I would like to see what your TM branded bullshit will look like against completely open source project?
[/quote]

So I guess it will be available for sure.

[quote="Cobber, post:18, topic:60463"]
What sort of constant wattage (amp/voltage) out put do you predict Kugy?
[/quote]
When comparing the drain to source on-resistance of the VESC 6 MOSFET (IRF7749) to the one of the FatBoy ESC (IRF7769) I expect a constant current output of the FatBoy around 33A with a heatsink like the VESC 6 has with no airflow at room temperature. (RDSon around 1.08 mOhm@80A/VGS=10V for IRF7749 and RDSon around 2.93 mOhm@80A/VGS=10V for IRF7769) Also notice that the given 18s (75.6V for a full LiPo) is to close to the 80V hardware limit for a save operation in my opinion, so when using regenerative braking I would not use more than 16s. (Same why the A200S save limit is 16s also)
So I would say the real constant power of the FatBoy HV ESC uncooled will be around 2kW. So a lot less than the 10kW target. :sweat_smile: But keep in mind that in our applications we don't use constant wattage for several minutes.
```

---
## \#75 Posted by: Kug3lis Posted at: 2018-07-02T22:03:53.213Z Reads: 266

```
I haven't yet figured out or decided according to the licensing as libraries have own licenses which I need to follow...

@hexakopter where did I mentioned what MOSFET's I am using? Also please don't discuss about specs if you don't even know what is going to be in the end ;) In the tests with casing, I was running over 100A for a good amount of time without air flow it felt same as laptop charger or etc didn't have thermometer at hand :) Plus where did you brought out 80V as hardware limit? Also if talking hardware limits VESC6 runs with 60V mosfets at 51V voltages so it has higher chance to fail than 100V mosfet at 76V ;)

EDIT: 80V was mentioned as maximum working voltage (for the crazy people who likes to live on the edge) hardware limit voltage is higher than that :)
```

---
## \#76 Posted by: PredatorBoards Posted at: 2018-07-02T22:31:21.089Z Reads: 256

```
Do make a build thread detailing the software portion of it! I would love to build one of these myself. The A200S definitely has FOC and current control. It should be compatible with the VESC tool, although I think custom firmware is a given.
```

---
## \#77 Posted by: hexakopter Posted at: 2018-07-03T14:40:26.478Z Reads: 273

```
[quote="Kug3lis, post:75, topic:60463"]
@hexakopter where did I mentioned what MOSFET’s I am using? Also please don’t discuss about specs if you don’t even know what is going to be in the end :wink:
[/quote]


There are pictures in this thread available were you can see that IRF7769 MOSFETs are used. I discussed about specs because I am also interested in a higher power/voltage VESC and some people were asking about the constant current your design will handle. So I just shared my calculations I did for myself looking at a picture showing a PCB with the labeling "FATboy HV ESC V1.0-Beta 18s 150A". So I calculated what would be possible with this current design ("normal" aluminum case without airflow) and not the end product which maybe looks totally different. No offense.

[quote="Kug3lis, post:75, topic:60463"]
In the tests with casing, I was running over 100A for a good amount of time without air flow it felt same as laptop charger or etc didn’t have thermometer at hand :slight_smile:
[/quote]
When the same physics apply to you that apply to me then this is not possible. ("normal" aluminum case without airflow) :D The VESC 6 can handle around 55A constant current (constant is >15 minutes for me) and as I stated before it uses MOSFETs with a superior RDSon than what is used in your design. So there is no way you can push 100A constant current for 15 minutes with the FatBoy HV ESC. ("normal" aluminum case without airflow) You should also be aware that case temperature ≠ MOSFET temperature.
You are now saying that you did the tests with the FatBoy ESC yourself but a few posts back that your father living in an other country assembled the board. It would be nice when you (your father or you) can proof me wrong and do a video showing 100A constant current ("normal" aluminum case without airflow) for >15 minutes.

[quote="Kug3lis, post:75, topic:60463"]
80V was mentioned as maximum working voltage (for the crazy people who likes to live on the edge) hardware limit voltage is higher than that :slight_smile:
[/quote]
How is it possible to have a hardware limit voltage higher than 80V when using INA240 current amplifiers with a 80V limit? And before you ask again where you mentioned using them it is also noticeable from the pictures. :grinning: So in my comparison spreadsheet the save operation of the FatBoy ESC is still at 16s max voltage.
```

---
## \#78 Posted by: Kug3lis Posted at: 2018-07-03T15:12:48.033Z Reads: 261

```
Oh boy... Please take your science back to your backyard :) Based on your science it's impossible to dissipate (I^2 * Rds = 100 * 100 * 0.0028 = 28W) of heat, which is nothing with the full aluminium case compared to VESC6 "case". Also with over 100A constant current not the MOSFETs are the problem but the power delivery is a much bigger problem.

You can't compare only because some other device is not capable of doing anything else. that's why we are going to sell this is esc with case only to provide enough cooling to run it at high currents.

I am not uploading any testing videos because it is not the final design and still modifications happening. Like now I am changing design of final board as it has some minor flaws.

Also, I am developing this ESC since last October, I have made many prototypes and etc, my father is assembling the final product so that's why he is doing it.

Regarding INA240 you know that motors are not driven at bat voltage because of current limiting? I have tested it with even 21S using 7 x 3S my graphene packs and it was still functioning just bit warm so please keep your paper knowledge to yourself :slight_smile:

P.S. I am building this for my own project to use with 18S as a proof of concept that it works
```

---
## \#79 Posted by: Kug3lis Posted at: 2018-07-03T15:30:00.960Z Reads: 248

```
Also no one talks about constant currents on ESC as there technically impossible without braking or blocking motor to make it consume same high amount of current for long amount of time. I was using nichrome wire as water heater to test out current handling of the phases. Later on we are going to build dyno stand for testing motors and drive trains to test out power capabilities and etc. So I will be able produce high loads on motors by simulating resistance, that's why I am not talking about constant current handling yet, just maximum allowed.
```

---
## \#80 Posted by: MoeStooge Posted at: 2018-07-03T16:12:07.150Z Reads: 246

```
Pardon me if I read over this and missed it while skimming info.  E-rpm limits?
```

---
## \#81 Posted by: Kug3lis Posted at: 2018-07-03T17:06:33.465Z Reads: 256

```
Haven't yet tried out, at the moment with vesc firmware it should be the same as VESC6. On my own firmware don't know yet anything as it is still in development and code is not the best quality to do benchmarks.

P.S. If you looking for high rpm FOC, FOC is not really suitable for high kv motors... iirc fastest one I saw was like 20k rpm but it was using >200Mhz mcu or etc and still struggled.

E-RPM is mostly limited by MCU performance and software. How long does it take to calculate next step values in between steps. For high speed motors compators are needed to detect zero crossing of BEMF and etc...
```

---
## \#82 Posted by: b264 Posted at: 2018-07-03T18:26:02.077Z Reads: 245

```
To get faster performance, sometimes you can use lookup tables instead of calulating the floating-point numbers.  

_sometimes..._
```

---
## \#83 Posted by: jens_c Posted at: 2018-07-03T18:28:05.466Z Reads: 242

```
add a 32 core cpu to your system
```

---
## \#84 Posted by: Kug3lis Posted at: 2018-07-03T18:35:56.700Z Reads: 246

```
It's not the problem of cpu performance, adc, pwm they all have maximum speeds :) I mean yes you can build fucking monster with oscilloscope level ADC, external PWM generator which uses freaking LVDS connections :D But who will want to pay several K for speed controller to drive 60$ motor :D
```

---
## \#85 Posted by: jens_c Posted at: 2018-07-03T18:47:08.840Z Reads: 247

```
the day i have to much money
```

---
## \#86 Posted by: LAVAMAN Posted at: 2018-07-03T20:07:09.656Z Reads: 251

```
If this turns out to be plug and play by simply inputting a few basic parameters and is dependable, you will be an e skate hero! Sign me up!
```

---
## \#87 Posted by: Minim Posted at: 2018-07-03T20:31:09.174Z Reads: 254

```
Why so humble?
```

---
## \#88 Posted by: hexakopter Posted at: 2018-07-03T20:53:27.048Z Reads: 266

```
I edited my post to be clear I talk about an uncooled aluminium enclosure like mentioned in my first post. So no airflow and sitting in room temperature. I also said that constant current for several minutes isn't used in our application, but it is a good benchmark because it is easy to reproduce with different hardware at same conditions and it is not dependent from riding speed and mounting for an example. (different airflow)
On my ESC I am also using 150A motor current without a problem, but not for several minutes and with good airflow cooling the case. So I never said 100A are not possible. Just not with your FETs, a normal aluminium case without airflow at room temperature and running it continuous for >15 minutes.
https://metr.at/r/2jHdL
Good luck with your project and I am out now.
```

---
## \#89 Posted by: Holyman92 Posted at: 2018-07-18T02:15:49.504Z Reads: 238

```
@Kug3lis I am eagerly waiting to buy a dual setup of these for my board... I was gonna buy some of stewii's controllers in September, now these are what's going in my monster... we have a race track, drag strip and I have obtained permission to take my board on it... I'm gonna try and top out an 18s and get it clocked lol
```

---
## \#90 Posted by: Kubbur Posted at: 2018-07-18T17:38:48.733Z Reads: 233

```
i need this for my upcoming setup
```

---
## \#91 Posted by: Friskies Posted at: 2018-09-24T02:46:38.696Z Reads: 206

```

Any updates?
```

---
## \#92 Posted by: Kug3lis Posted at: 2018-09-24T09:32:27.557Z Reads: 204

```
Still a shit load of work on firmware so don't expect without end of year or next year spring :)
```

---
## \#93 Posted by: Skunk Posted at: 2018-09-24T09:35:08.913Z Reads: 203

```
So what you're saying is, we should start the pre-order Group buy thread. LOL
```

---
## \#94 Posted by: Kug3lis Posted at: 2018-09-24T09:37:23.418Z Reads: 207

```
Oh no not yet :) I am still working on firmware level stuff, afterwards I will be deciding what hardware to make as logic (mcu and firmware) will be used the same on all hardware configs ;) I have achieved motor spinning, now I need to implement PPM, configuration, usb, uart, can and other stuff :)
```

---
## \#95 Posted by: Skunk Posted at: 2018-09-24T09:39:36.237Z Reads: 207

```
[quote="Kug3lis, post:94, topic:60463"]
Oh no not yet
[/quote]

Oh I know, was more a joke on people and thier impatience for new products.

Plus we need time to design body armor to Keep Us Alive at 19s
```

---
## \#96 Posted by: Kug3lis Posted at: 2018-09-24T09:50:53.625Z Reads: 206

```
Plus I am evaluating DRV for 100V operation from TI :O Maybe it will go into production at the same time I will finish my firmware :)
```

---
## \#97 Posted by: Wraith Posted at: 2018-09-24T09:59:05.288Z Reads: 207

```
You almost got me there on the pre-order thing lol
```

---
## \#98 Posted by: Blitz Posted at: 2018-10-08T10:55:16.587Z Reads: 184

```
Would our standard 6374 motors handle your 18s esc (at say 16-18s), or would we need different motors?
```

---
## \#99 Posted by: Kug3lis Posted at: 2018-10-08T13:21:22.309Z Reads: 180

```
Each motor has maximum RPM or Voltage allowed :) Its mainly for beefier motors like 80**
```

---
## \#100 Posted by: ElskerShadow Posted at: 2018-10-08T13:23:59.688Z Reads: 187

```
@Kug3lis Do you think your ESC will be suitable for more powerfull electric vehicules, like scooter, motorcycles, powerfull ebikes ? 

I am looking for other ESC than chinese ones
```

---
## \#101 Posted by: Kug3lis Posted at: 2018-10-08T13:28:58.399Z Reads: 188

```
Well I am making new main brain of esc which I can reuse on mostly any hardware stage. so from mini version for 6s 30a max up to bus motor controller but I doubt I will make something for bigger vehicles as there are better options :)

Bike has already nice controller :slight_smile:

http://adaptto.com/Products/Controllers/

P.S. this design in topic is dead so no more like this as I am using different mcu and etc things :)
```

---
## \#102 Posted by: ElskerShadow Posted at: 2018-10-08T13:36:35.831Z Reads: 181

```
I've heard of the adaptto but 470 dollars for a 4 kw controller seems like a lot ! 
Sabvoton are bigger but half the price for similar function
```

---
## \#103 Posted by: Kug3lis Posted at: 2018-10-08T13:37:27.282Z Reads: 187

```
Well those 4kW are real constant 4kW not vesc 1min max :)
```

---
## \#104 Posted by: ElskerShadow Posted at: 2018-10-08T13:39:38.935Z Reads: 192

```
yeah I bet they are, well I have never tried those so when I have spare money i'll try these controller. 

according to you even adding thermal mass for dissipation would not help ? 

I have been spoiled with open source software i think :stuck_out_tongue:I'd love to have some VESC like ESC for bigger applications
```

---
## \#105 Posted by: lrdesigns Posted at: 2018-10-09T00:38:51.513Z Reads: 198

```
[quote="Blitz, post:98, topic:60463"]
Would our standard 6374 motors handle your 18s
[/quote]

Yes, with some provisions. 

There is no hard voltage limit for the brushless motors we use. You will reach the RPM limit and destroy the motor before voltage becomes a problem. I dont think you could even reach that RPM on a skateboard. Hobby grade motors become sketchy above 50,000 rpm. While our skate motors are spinning 8-10,000 rpm. 

The max power the motor can handle in watts is still the same though, if you increase voltage you need to decrease amps / load or risk overheating the motor. The easiest way to do that would be a higher gear ratio. Going 4wd would do that too. :joy: 

Limit the amps in vesc is one way but your also limiting acceleration. 

Heat is the main issue motors face, bigger motors handle more heat. More load = More heat.
```

---
## \#106 Posted by: Blitz Posted at: 2018-10-09T15:58:03.279Z Reads: 182

```
Yeah, I wouldn't try put 18s on my motors, and just match the wattage not without solid research but thanks for the answer!
```

---
## \#107 Posted by: Holyman92 Posted at: 2018-10-09T16:16:11.561Z Reads: 190

```
@Kug3lis rememebr when u asked me why i need 80mm motors... this is why, the build i referenced that will be using the 80mm im designing to be used with ur ESC but for the mean time ima be using it w/ the 6.6 from FlipSky
```

---
## \#108 Posted by: b264 Posted at: 2018-10-09T18:53:08.116Z Reads: 186

```
I wouldn't use 18S, but I would love to have equipment rated 18S and using it only for 12S.  Never failures!
```

---
## \#109 Posted by: Surfer Posted at: 2019-04-17T12:00:06.605Z Reads: 125

```
Hi are you still working on this or is a rip project?
```

---
## \#110 Posted by: b264 Posted at: 2019-04-17T16:15:20.547Z Reads: 107

```
He's stepped away from esk8.
```

---
## \#111 Posted by: Surfer Posted at: 2019-04-17T17:36:32.457Z Reads: 103

```
I don't think so :slight_smile:
This is not a easy nor quick project , maybe not with this one, but he keeps building and selling killer stufffs
```

---
## \#112 Posted by: Andy87 Posted at: 2019-04-17T19:19:44.760Z Reads: 94

```
Maybe have a look here instead 
https://www.electric-skateboard.builders/t/some-new-focers-84v-vesc-6-based-controllers/87227?u=andy87
```

---
