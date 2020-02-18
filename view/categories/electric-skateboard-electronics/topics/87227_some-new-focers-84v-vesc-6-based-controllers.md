# Some New FOCers (84V VESC 6 based controllers)

### Replies: 109 Views: 3333

## \#1 Posted by: shaman Posted at: 2019-03-15T15:18:19.293Z Reads: 428

```
![TO247|690x342](upload://eTJFvahms1TQu13wwFKlLZpSNsi.jpeg) 
**Serious FOCer**. TO-247 version

![6%20FET%20angled|690x364](upload://1sNfGUKxty2SGqhnZ7cbK5Ygrrm.png) 
**Little FOCer**. vertical TO-220 version.

![TO220%20horizontal|690x306](upload://4Ny2Qyz0dyFZ21pGVfjz5FVcLW0.jpeg) 
**Flat Little FOCer.** horizontal TO-220 version for reduced overall height. Image for reference only. Layout does not yet accommodate horizontal TO-220 package.

![12%20FET%20angled|690x389](upload://acwUfglA9Denm8v7bzksCgE6odH.png) 
**Mother FOCer**. 12 TO-220 FET version.

**Announcing a new line of FOCing controllers**

Features:

* 15V to 84V operation

* Expected power of approx 5kW with TO-247 FETs and good heat sinking

* Has primary features of VESC controllers (FOC, configurable current/temperature limits, throttle response, dual motor operation, ect.)

* Different versions for different FET packages

* TO-247 FET and 12 TO-220 FET versions for higher current capability

* Single-sided dual-layer PCB

* Small 45mm x 101.5mm board size

* Each switch node has it's own bulk cap, pwr, gnd and phase cable holes. Reduces need for beefing up long traces for increased current handling capability

* Utilizes DRV8353RS to achieve higher operating voltage, superior fault detection, and small footprint. Also allows for tailored slew rate control to minimize ringing/spiking in the power stage

* Easy On/Off capability with switch of choice

* Wireless Bluetooth transceiver module can be easily added for wireless interface with VESC Android App. Allows for easy configurations of different speed/power profiles that can be selected at will.

* Design will be open sourced after verification

* Designed in KiCAD for flexibility and compatibility with the open source community

Donations:
Open Source R&amp;D isn't free! Any help is appreciated! 
https://www.paypal.me/shamansystems?locale.x=en_US

This is a higher performing controller in comparison to my Cheap FOCer controller that is about to go into beta testing. All lessons learned from the Cheap FOCer development has and will go into this new controller design. It will be a while before this is made a reality. new firmware will have be developed for the new DRV8353RS. Your patience will be appreciated on this one as I have other projects running parallel. In the mean time while we all wait for me to develop this, I am open to any suggestions that will help make this controller great for this community!

All this wouldn’t be possible without Benjamin Vedder’s hard work to build on. Please consider supporting him for his efforts through the link below.

https://vesc-project.com/donations
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-18T05:59:55.146Z Reads: 364

```
kind a missed that the last days...
I directly have some questions :sweat_smile:
As it´s gonna be vesc6 based esc, I can assume that it´s possible to run AS5047 encoder with that esc as well?
the voltage for the sensors is switchable between 3.3 and 5V or it will be set to one of thos values?
```

---
## \#3 Posted by: shaman Posted at: 2019-03-18T14:03:00.903Z Reads: 346

```
I haven't implemented a switch for the hall sensor voltage. The AS5047 needs 5V right? Most hall effect sensors in the e-bike world take 5V as well. What I can do is just make the hall sensor outputs permanently tied to 5V to accommodate this unless someone knows of hall sensors that need 3.3V.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-03-18T14:10:59.848Z Reads: 339

```
The AS5047 works with both depending on how you solder up the sensor pcb.
The noice seems to be less with 3.3V but if you use shielded cables 5V works as well.
I read somewhere that the AS5047 Encoder wouldn’t work with hw4.xx is that correct and does it mean that the encoder also not working with the cheap focer? 
Not an issue for me if not, just wanted to clearify for my personal understanding.
```

---
## \#5 Posted by: briman05 Posted at: 2019-03-18T14:24:38.098Z Reads: 308

```
I propose a name change and call it the mother FOCer
```

---
## \#6 Posted by: shaman Posted at: 2019-03-18T14:24:57.523Z Reads: 301

```
I'm not sure if the Cheap FOCer will work or not with that encoder. It will just have to be tested to find out for sure (task for Beta Testers). Personally I don't see why it wouldn't. 

Odd how 3.3V is less noisy than 5V. Generally higher reference voltages or Vcc voltages are less susceptible to noise.
```

---
## \#7 Posted by: shaman Posted at: 2019-03-18T14:27:18.990Z Reads: 290

```
I've reserved the name "Mother FOCer" for  a 12 FET or higher version. I decided this back on my Cheap FOCer thread. I like where your head's at though :slightly_smiling_face:
```

---
## \#8 Posted by: briman05 Posted at: 2019-03-18T14:29:43.681Z Reads: 282

```
Totally understand maybe the "Little FOCer".  The work so far looks really good I'm going to be watching this thread to see how it comes out when you have a working prototype.
```

---
## \#9 Posted by: shaman Posted at: 2019-03-18T14:33:27.306Z Reads: 271

```
Cool. There's a lot of interest in this model. I don't think anyone has open sourced anything like it. Stay tuned for the progress!
```

---
## \#10 Posted by: Andy87 Posted at: 2019-03-18T16:55:52.777Z Reads: 276

```
[quote="shaman, post:6, topic:87227"]
task for Beta Testers
[/quote]

I can have a look at this by my own than 😉
```

---
## \#11 Posted by: shaman Posted at: 2019-03-24T23:30:52.395Z Reads: 275

```
![12%20FET%20with%20Sink%20angled|690x342](upload://f6DnEDPJhWP9BXjmjO7he7MutTX.png) 
12 FET Version w/ Heatsink

![12%20FET%20with%20Sink%20side|690x394](upload://9DLkULHfui5RuwE2hm00d0x8H9x.png) 
12 FET Version w/ Heatsink side view

![12%20FET%20angled|690x389](upload://acwUfglA9Denm8v7bzksCgE6odH.png)
12 FET Version

 ![6%20FET%20angled|690x364](upload://1sNfGUKxty2SGqhnZ7cbK5Ygrrm.png) 
6 FET version proper

Did some more work on the variants of the Serious FOCer. Got the 12 FET and 6 FET design drafted. the 12 FET probably leaves the esk8 realm in power but I figure you guys would like to know about it anyways.
```

---
## \#12 Posted by: kalebludlow Posted at: 2019-03-25T02:32:17.094Z Reads: 251

```
I'm not a super big smarty nerd, so what are the real world differences between the 6 FET and 12 FET version?
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-03-25T02:52:17.838Z Reads: 250

```
I have a 13s build comming up, this would be great but the caps and fets are too tall 😫
```

---
## \#14 Posted by: shaman Posted at: 2019-03-25T12:22:32.247Z Reads: 235

```
Doubling the FETs double the the amount of current than can be handled and therefore increases power. Increasing the amount of paralleled FETs to achieve greater power is common practice for ebike controller designs. There are 18 and even 24 FET controllers out there.
```

---
## \#15 Posted by: shaman Posted at: 2019-03-25T12:26:58.024Z Reads: 235

```
Did you see the horizontal 6 FET variant? It's in my first post but it's just for reference. Also the black cylinders on the board are actually through hole inductors that can be replaced by SMD inductors for lowered height. The large bulk caps are actually laying down for this board, they just don't have a 3D model and are identified by the 3 white rectangles. 

The horizontal 6 FET version hasn't officially been layed out but it wouldn't take long. Your not the only one who wants reduced height for this controller :slight_smile:
```

---
## \#16 Posted by: linsus Posted at: 2019-03-25T12:28:32.890Z Reads: 230

```
How big is the price delta between direct FETs and dpak ones?
```

---
## \#17 Posted by: shaman Posted at: 2019-03-25T12:32:44.490Z Reads: 233

```
I don't know off the top of my head but dpaks are slightly more expensive if I remember right. The dpak or d2pak packages can handle a little more current. They just aren't great for easily attaching a heatsink to them.
```

---
## \#18 Posted by: linsus Posted at: 2019-03-25T12:38:39.675Z Reads: 223

```
Wouldn't the directFETs be prefered then? Isnt the entire fuss about them that they're preferable for heat dissipation?
```

---
## \#19 Posted by: shaman Posted at: 2019-03-25T12:47:47.266Z Reads: 233

```
Well let's compare directFETs to TO-220s(the ones I'm using) instead of dpaks. directFETs appear to be slightly more expensive than TO-220s according to infineon's website. TO-220 are through hole, have tab with a mounting hole for a heatsink, and can be easily replaced if damaged. Tons of manufacturers make TO-220 FETs and therefore one can find good ones for low cost.

directFETs are very small for the power they can handle, are surface mount, and can be cooled from either side. Still you can't just bolt on a heatsink to them or easily replace them if they blow up. They are also only available from Infineon to my knowledge.

I went for practicality and ease of replacement for my design and you can bolt on a monster heatsink to TO-220s fairly easily and for cheap.
```

---
## \#20 Posted by: linsus Posted at: 2019-03-25T12:55:13.531Z Reads: 215

```
They're not THAT hard to replace :P only time I had to solder them was on initial mounting tho. They just float into place thanks to the surface tension of the hot solder.  A thin film of insulation between the sink and FET and ur done :P They have never blown after beeing properly soldered, on 4 separate escs. So I have nothing but love for them, so I might be abit biased I guess.

Regarding through hole, wont that add unwanted trace length on the power stage? :face_with_monocle:
```

---
## \#21 Posted by: shaman Posted at: 2019-03-25T13:03:08.942Z Reads: 210

```
Yes they're easy if you have the capability to do reflow soldering. I do but many hobbyists don't have a reflow station. Just a regular solder iron. Yes a thin film of insulation is placed in between FETs and the heatsink but how are you actually applying mechanical pressure between the directFET and the heatsink? Is the custom(expensive) heatsink that is being used designed to do this somehow?

Yes the though hole packages cause a larger footprint for layout in the power stage but this isn't anything that can't be accounted for and managed. TO-220s and TO-247 packages are used in several professional controllers like the SEVCON or Adaptto and have proven themselves to be effective. The downside just tends to be that they're larger and cause the controller to be larger. Not a big deal for bikes but it is for esk8. The directFETs are small and are good for when small is needed.
```

---
## \#22 Posted by: linsus Posted at: 2019-03-25T13:07:26.016Z Reads: 201

```
[quote="shaman, post:21, topic:87227"]
Yes a thin film of insulation is placed in between FETs and the heatsink but how are you actually applying mechanical pressure between the directFET and the heatsink? Is the custom(expensive) heatsink that is being used designed to do this somehow?
[/quote]

The mechanical pressure is added from the PCB mounting holes. The sink doesn't have to be that complicated, Just enough that a small portion extrudes over the FETs. 
Simplest way would be a sandwich of two plates, one as big as the PCB (to mount on) and one ontop of it to make contact with fets, So essensially two squares of metal. One could go wild and make an encasing like the vesc6 tho. But its more expensive
```

---
## \#23 Posted by: shaman Posted at: 2019-03-25T13:14:57.787Z Reads: 195

```
Ah I see. Some BMS boards do this same thing for heatsinking. 

To each their own I suppose. Each type of FET has their advantages and disadvantages .Optimize for one thing and you stray from another. It wouldn't be too hard for one to spin my controller design to accommodate directFETs. Open sourcing this design will allow anyone to do this and create a controller better optimized for esk8. That's the beauty of open source :slight_smile:
```

---
## \#24 Posted by: Benjamin899 Posted at: 2019-03-25T15:42:34.234Z Reads: 190

```
@shaman i like your approach, there are enough powerfull small solution available, and yours isnt that much bigger.
I think your design has more advantages than not. This ESC will be epic in Pneumatic (bigger) Builds and other fun application, GoCart ect, that have room to spare.
```

---
## \#25 Posted by: banjaxxed Posted at: 2019-03-25T20:20:50.576Z Reads: 184

```
Roll over Beethoven 

droool. This is very cool. Does it require a massive forks of Vedder's code to acheive the end-goal?

Any plans for dual ESC variant given that is what is gets done, especially for the 12FET version

Looking forward to following the exploits on this
```

---
## \#26 Posted by: shaman Posted at: 2019-03-25T22:07:05.297Z Reads: 182

```
The changes to Mr. Vedder's code won't be too bad. There's one file that is particular to the DRV being used. That's the one that needs to be changed. There's already support for the DRV8323 which is very similar to the DRV8353. Changes will most likely be minimal.

There's no plan for a dual ESC at the moment. Just run two controllers together through CAN for the dual awesomeness.
```

---
## \#27 Posted by: banjaxxed Posted at: 2019-03-25T22:08:12.714Z Reads: 193

```
[quote="shaman, post:26, topic:87227"]
dual awesomeness
[/quote]

works for me. Particular to esk8 and ATB, there are many 80xx motors which reference 15s which fits in with the 12FET version. My knowledge on motor efficiency at Xv is pretty limited.

Wondering what happens theoretically as voltage increases, the current demand should be lower. At some point peak efficiency is reached depending on motor construction and materials used. 

Are the advantages worth shooting for? I know we are already stretching the 60v component rating most VESC based clones are geared towards with 13s builds..Trampa VESC 75/300 notwithstanding

motor examples
* Leopard LC8072 Voltage up to lipos 16s
* APS 8072S  MAX VOLT: 15S (63V)


Smaller motors like the ubiquitous 6374 afaik they do not normally get a higher voltage suggestion than about 13s. Perhaps something like the swissboard hub drive with silver windings could utilise.

I'm aware you can run pretty much any of these motors at 20s but things get dangerous and unless it's a motorbike/kickass MTB/car it does not seem to be a thing
```

---
## \#28 Posted by: linsus Posted at: 2019-03-25T22:30:33.937Z Reads: 164

```
Check for 15-30 kW bldcs on ali f.e, theyre quite pricy but its the "next step".

What happens with the smaller motors is that they eventually saturate @ magnetic flux. Which is bit mor connected to current then voltage. Sure bigger motor, step up in voltage, but also step up in current if you want the full potential of the motor.
```

---
## \#29 Posted by: banjaxxed Posted at: 2019-03-25T22:36:05.517Z Reads: 168

```
I hear you, but you're into serious danger power for something you can't sit in and control steering with apart from body weight.

The 80xx motors with big wheels and low kv more likely in 2019/20?

[quote="linsus, post:28, topic:87227"]
its the “next step”.
[/quote]
```

---
## \#30 Posted by: linsus Posted at: 2019-03-25T22:37:57.076Z Reads: 163

```
Your looking to change means of transportation your looking for more power. Id be more comfortable with that beast on a motorbike. But towards 20kW on an eskate? If u wanna tow cars I guess?

Sure the 80xx motors are out there, but i think its hard to keep the cogging and drag down the bigger you go. I guess on an mtb or AT setup but freewheeling would get close to minimal
```

---
## \#31 Posted by: briman05 Posted at: 2019-03-25T23:03:37.481Z Reads: 160

```
Every post makes this even more interesting
```

---
## \#32 Posted by: banjaxxed Posted at: 2019-03-25T23:19:37.458Z Reads: 161

```
How dangerous is 16s 160A DC to a mere mortal?
```

---
## \#33 Posted by: shaman Posted at: 2019-03-25T23:23:31.913Z Reads: 172

```
[quote="linsus, post:30, topic:87227"]
But towards 20kW on an eskate? If u wanna tow cars I guess?
[/quote]

20kW is almost 27HP. That's motorcycle territory. Would probably rip you or the esk8 apart if you tried something like that on a small piece of wood.

[quote="banjaxxed, post:32, topic:87227, full:true"]
How dangerous is 16s 160A DC to a mere mortal?
[/quote]

Well I don't advise licking it. It's dangerous if you don't respect it but it can be handled in the proper medium. 16s 160A is about 9kW and roughly 12HP. Probably best applied in ebike or above.
```

---
## \#34 Posted by: banjaxxed Posted at: 2019-03-25T23:27:57.832Z Reads: 151

```
It’s interesting because there are quite a few 80xx builds out there. My understanding is change the ESCs to seriousFOCers, up pack series to 16s and enjoy better efficiency, more linear power delivery and of course higher ERPM, but not necessarily higher top speed/torque?

Speaking of ERPM, is there a limit in mind that you think would be achievable?
```

---
## \#35 Posted by: banjaxxed Posted at: 2019-03-25T23:31:28.229Z Reads: 154

```
[quote="shaman, post:33, topic:87227"]
I don’t advise licking it.
[/quote]

Only toads these days 😂
```

---
## \#36 Posted by: evoheyax Posted at: 2019-03-25T23:33:09.926Z Reads: 159

```
Love more options. Just trying to understand what applications your thinking this would be good for?

5kw would surely spin any wheel on acceleration unless your building some crazy large wheels.
```

---
## \#37 Posted by: shaman Posted at: 2019-03-25T23:33:15.515Z Reads: 174

```
[quote="banjaxxed, post:34, topic:87227"]
up pack series to 16s and enjoy better efficiency
[/quote]
While increasing voltage and decreasing current does generally yield higher efficiency, motors still have a sweet spot of rpm vs power that will be the most efficient. There are a lot of variables in that and more than I fully understand. All i know is that the sweet spot can be found by putting the motor on a dyno and conducting tests.

More voltage = higher rpm for motors. More current = more torque at least up to a certain point. 

[quote="banjaxxed, post:34, topic:87227"]
Speaking of ERPM, is there a limit in mind that you think would be achievable?
[/quote]
I'm assuming the ERPM limit will be the same as the VESC 6 since my design is the same from a controls standpoint. Only one real way to find out though. Hence beta testing :slightly_smiling_face:
```

---
## \#38 Posted by: shaman Posted at: 2019-03-25T23:36:04.864Z Reads: 169

```
The applications for the serious FOCer series of controllers are more geared for ebikes or above. I just figured you guys might be interested for shits and giggles. The 6 FET versions would be the most practical for esk8 and could be considered a high voltage version of my Cheap FOCer.
```

---
## \#39 Posted by: banjaxxed Posted at: 2019-03-25T23:39:11.617Z Reads: 165

```
And if you get a DRV error
Bad Mother FOCer
```

---
## \#40 Posted by: banjaxxed Posted at: 2019-03-25T23:41:53.878Z Reads: 168

```
Plenty of willing devotees of shit and giggles. Can I propose a master of ESC carnage and reviewer extrordinaire, @longhairedboy ?
```

---
## \#41 Posted by: FredrikHems Posted at: 2019-03-25T23:42:03.127Z Reads: 160

```
Is the 5kw power output the goal for the 6 FET or 12 FET version?
```

---
## \#42 Posted by: shaman Posted at: 2019-03-25T23:45:29.149Z Reads: 165

```
[quote="banjaxxed, post:40, topic:87227"]
Can I propose a master of ESC carnage and reviewer extrordinaire, @longhairedboy ?
[/quote]

Sure. I'll probably do another round of Beta Testing for this series of controllers. It just may not be as many.

[quote="FredrikHems, post:41, topic:87227, full:true"]
Is the 5kw power output the goal for the 6 FET or 12 FET version?
[/quote]

That's for the 6 TO-247 FET version. The 6 TO-220 FET version is more like 3.5kW. These numbers are approximations as I have no idea what the real life limits are for TO-247s. Gunna find out though :slight_smile:
```

---
## \#43 Posted by: banjaxxed Posted at: 2019-03-25T23:47:09.738Z Reads: 160

```
6/12FET models need naming delineation otherwise you will be crossing wires from here to eternity, jest but true

* 6FET: Serious FOCer
* 12FET: Mother FOCer

Our erstwhile naming combobulator @brenternet will be along shortly to rubber stamp @briman05’s witty denomer or trash it into oblivion.

If you’re familiar with DaveGA, you’ll understand, it’s a thing
```

---
## \#44 Posted by: Benjamin899 Posted at: 2019-03-25T23:47:12.648Z Reads: 157

```
Pneumatic direct drive, since we lose the gearing you will need a powerfull motor to run efficient.
```

---
## \#45 Posted by: shaman Posted at: 2019-03-25T23:49:54.912Z Reads: 158

```
Sure. 

* 6 TO-220: Little FOCer
* 6 TO-247: Serious FOCer
* 12 FET: Mother FOCer
* 18 FET: Serious Mother FOCer

...or something
```

---
## \#46 Posted by: banjaxxed Posted at: 2019-03-25T23:51:43.560Z Reads: 153

```
It works any way you do it, ingenious 😀
```

---
## \#47 Posted by: shaman Posted at: 2019-03-25T23:54:20.913Z Reads: 158

```
Catchy isn't it? And they say design engineers can't market :grin:
```

---
## \#48 Posted by: briman05 Posted at: 2019-03-26T00:09:03.166Z Reads: 155

```
18 fet should be holy mother FOCer or grandmotha FOCer
```

---
## \#49 Posted by: shaman Posted at: 2019-03-26T00:10:38.289Z Reads: 153

```
Gotta save something for the 18 TO-247 FET FOCer. That's my prospect controller for my e-motorcycle conversion. That's a league of it's own though and will be designed differently
```

---
## \#50 Posted by: banjaxxed Posted at: 2019-03-26T00:11:29.388Z Reads: 151

```
Holy Mother FOCer 😂
```

---
## \#51 Posted by: lrdesigns Posted at: 2019-03-26T01:30:29.159Z Reads: 151

```
Hey man just donated to the R&D effort. Have a :beer:, :hamburger:, :burrito: or :coffee: on me. Whatever floats your boat? 

Is there any plans to do a run of these where the surface mount components are already on then the through holes can be added by ourselves? That should make them buildable by most DIYers.
```

---
## \#52 Posted by: shaman Posted at: 2019-03-26T01:39:37.714Z Reads: 157

```
gunna very much enjoy my :beer: Much appreciated!

Yes I am definitely considering offering boards that have the SMD components, or at least the hard ones, pre-soldered leaving the rest to the DIYer. This sort of thing was discussed back on my Cheap FOCer thread. 

So here's my master plan:

1. Start LLC and webstore

1. Design and sell cool open source stuff

1. ???

1. Profit...or something
```

---
## \#53 Posted by: lrdesigns Posted at: 2019-03-26T01:43:30.624Z Reads: 155

```
:beers: Cheers!
```

---
## \#54 Posted by: Andy87 Posted at: 2019-03-26T04:47:51.192Z Reads: 159

```
[quote="shaman, post:33, topic:87227"]
Would probably rip you or the esk8 apart if you tried something like that
[/quote]

Sound great 😊 definitely down for beta testing that 😌
```

---
## \#55 Posted by: linsus Posted at: 2019-03-26T08:49:28.078Z Reads: 159

```
[quote="shaman, post:45, topic:87227, full:true"]
Sure.

* 6 TO-220: Little FOCer
* 6 TO-247: Serious FOCer
* 12 FET: Mother FOCer
* 18 FET: Serious Mother FOCer

…or something
[/quote]

[![](https://media1.tenor.com/images/84ca83814ebd9688b1d386070b32db65/tenor.gif?itemid=9413605)](https://tenor.com/view/funny-shit-gif-9413605)
```

---
## \#56 Posted by: lrdesigns Posted at: 2019-03-26T09:33:36.951Z Reads: 161

```
![image|554x500](upload://8Jgldfkv5WxQITK365MsZjALPDR.jpeg) 

![image|581x363](upload://r3rEBCO81nBiokUq7hGbeqLYd8o.jpeg) 

https://media.giphy.com/media/MA7x0Zcqjf1x6/giphy.gif
```

---
## \#57 Posted by: Vanarian Posted at: 2019-03-26T10:58:58.867Z Reads: 159

```
[quote="shaman, post:11, topic:87227"]
![12 FET with Sink angled.PNG](https://www.electric-skateboard.builders/uploads/db1493/original/3X/6/9/69e09ed74ec38fe042f3c99bf753ef1e77990231.png)

12 FET Version w/ Heatsink

![12 FET with Sink side.PNG](https://www.electric-skateboard.builders/uploads/db1493/original/3X/4/3/439240e9f8be8adc284b6a7b2a5ff809f91fb50b.png)
[/quote]

Rant mode On/
I wish some people around here saw your work to improve their own... Now that's proper heatsinking FETs instead of putting useless metal on the plastic part. And yet people still buy their shit hahaha that's sickening.
/Rant mode Off.

On topic, I'm looking forward to your controllers prowess man !! How big will the footprint be btw ?  Looks perfect for drift trike / e-bikes / superfast boards / e-karting?
```

---
## \#58 Posted by: shaman Posted at: 2019-03-26T12:01:37.667Z Reads: 156

```
The board for the 12 FET is about 53mm x 101mm (2.1" x 4"). Relatively small compared to other 12 FET controllers out there.
```

---
## \#59 Posted by: shaman Posted at: 2019-03-26T12:34:43.581Z Reads: 153

```
Really liking the Samuel L. Jackson reference here. While Bad Mother FOCer was suggested as a name for when a fault happened, I'm leaning toward that being the name of the 18 TO-247 FET controller for my e-motorcycle. I might even put a silk screen outline of Samuel on the board.
```

---
## \#60 Posted by: linsus Posted at: 2019-03-26T12:45:07.501Z Reads: 154

```
I propose sam L's face printed in the silkscreen. Maybe in diffrent degrees of smiling between how much FOCer are in them.

Edit: actually read your comment now, lol, great minds think alike.
```

---
## \#61 Posted by: shaman Posted at: 2019-03-26T12:56:44.588Z Reads: 142

```
It's official. Putting silk screen Samuel on the back of the boards with varying degrees of intensity based on the type of FOCer. This kind of shit makes engineering fun :grin:
```

---
## \#62 Posted by: Pedrodemio Posted at: 2019-03-26T13:02:28.614Z Reads: 140

```
That will be epic 

Really interested on this e-motorcycle version
```

---
## \#63 Posted by: shaman Posted at: 2019-03-26T13:06:15.132Z Reads: 141

```
Me too. The Bad Mother FOCer (150V 300A controller) is just a concept right now. galp on the endless sphere has laid the foundation for something like this called the BESC. I'm waiting for him to release the schematics so that I can apply my own FOCery to it.
```

---
## \#64 Posted by: Pedrodemio Posted at: 2019-03-26T13:14:36.514Z Reads: 142

```
I’m following it there, now I just need a donor bike, and batteries, and a motor, and a bike driving license. Easy
```

---
## \#65 Posted by: banjaxxed Posted at: 2019-03-26T15:13:33.568Z Reads: 143

```
Try and arrange the position of the screen so the leds look like gleams in his grin
```

---
## \#66 Posted by: shaman Posted at: 2019-03-27T01:50:55.639Z Reads: 146

```
![image|500x500](upload://yizE6jIphNHYiCTxGRvNHlOkrO8.png) 

So I got some Samuel L. Jackson bitmaps prepared. KiCAD makes you create a custom footprint just for the graphics. I'll get to it sometime soon.
```

---
## \#67 Posted by: kuphjr Posted at: 2019-03-27T02:08:49.431Z Reads: 143

```
This would be a great addition to my electric unicycle build! Do you have an itemized parts list with approximate costs?  I'll send a $50 donation as long as someday I can either build one myself using your open source plans or buy one from you if you ever produce these for resale!
```

---
## \#68 Posted by: shaman Posted at: 2019-03-27T02:15:59.576Z Reads: 144

```
I don't have a BOM yet for this line controllers. They're still in development but I do intend to offer them for sale at least partially assembled sometime after I verify the design. The schematics, gerbers, and KiCAD project files are guaranteed to be released after verification. Check out my "master plan" in a recent post on this thread. 

The Cheap FOCer is my first controller design that is closer to being completed. Check out that thread if you haven't already.
```

---
## \#69 Posted by: kuphjr Posted at: 2019-03-27T02:33:58.593Z Reads: 150

```
Will do! Its awesome to see more speed controller development in the community.
```

---
## \#70 Posted by: shaman Posted at: 2019-03-31T21:40:10.610Z Reads: 150

```
![thumbnail|666x500](upload://aURqZ6rixxToKWcR9xT9lwMKo1I.jpeg) 

On a unrelated note, I got my first CNC machine up and running. Might be good for making custom heatsinks or enclosures.
```

---
## \#71 Posted by: banjaxxed Posted at: 2019-04-01T06:29:00.064Z Reads: 143

```
Dickbutt is not welcome here, ask me how I know
```

---
## \#72 Posted by: Bobby Posted at: 2019-04-01T07:16:32.304Z Reads: 142

```
@banjaxxed How do u know?
```

---
## \#73 Posted by: linsus Posted at: 2019-04-01T07:25:19.179Z Reads: 137

```
I smell directFET design
```

---
## \#74 Posted by: banjaxxed Posted at: 2019-04-01T07:53:01.845Z Reads: 137

```
![image|690x155](upload://DzVWj1DwAZl8Eugh2dYJsx0cIY.png)
```

---
## \#75 Posted by: shaman Posted at: 2019-04-01T12:17:46.159Z Reads: 131

```
Well enjoy it while it lasts I guess...
```

---
## \#76 Posted by: shaman Posted at: 2019-04-01T12:20:41.864Z Reads: 138

```
Let's not get too excited! :slightly_smiling_face: Maybe I'll do some enclosures with some CNCed graphics to start.
```

---
## \#77 Posted by: banjaxxed Posted at: 2019-04-01T12:25:27.826Z Reads: 143

```
Here's food for thinks, maybe down the road a dual bad Mother FOCer
![image|315x183](upload://rKHThhunMdEVWOCoDE9CKBUJjt7.png)  

Best keep to a sticker in case Miramax bother you
```

---
## \#78 Posted by: banjaxxed Posted at: 2019-04-01T12:26:27.363Z Reads: 142

```
Mine was much much worse, you'll have to use your imagination
```

---
## \#79 Posted by: shaman Posted at: 2019-04-03T23:53:48.533Z Reads: 135

```
Anyone have some good information on FCC, NRTL, or CE certifications when it comes to ESCs and such? I figure a DIY kit wouldn't need it but a fully assembled controller might?
```

---
## \#80 Posted by: district9prawn Posted at: 2019-04-04T06:42:36.613Z Reads: 126

```
Sell a 95% assembled controller?
```

---
## \#81 Posted by: shaman Posted at: 2019-04-04T12:08:07.125Z Reads: 126

```
Yeah. There might be a loophole here. I may hit up some certification facilities to try and find out what does and doesn't apply to motor controllers.
```

---
## \#82 Posted by: linsus Posted at: 2019-04-04T12:21:43.711Z Reads: 136

```
You're fine, Enertion dsnt have a single EMC cert, nor does Trampa, CE stamp is on the official VESC6 tho. But its usually selfcertifiable. 

Legally, no. You're not in the clear if this is a commercial profiting product.

Send one to me and I'll do the basic EN55xx for you. If it passes that you've come a long way.

Dont think I've posted this anywhere but here is the one i did on 4.12 hardware: 

![image|395x441](upload://aB0jtXBXSqz2EXySTs0Qqh9NRLq.jpeg)
```

---
## \#83 Posted by: shaman Posted at: 2019-04-04T13:33:15.080Z Reads: 127

```
I really appreciate the info and this offer! Things definitely are easier if I don't have to worry about expensive certifications. The 4.12 seems to do decently well under the basic EN55xx test. I may add a few more caps in choice places on the new controller designs to minimize radiation.
```

---
## \#84 Posted by: linsus Posted at: 2019-04-04T13:34:39.042Z Reads: 125

```
The biggest peak is the MCU at 168mhz if I remember correctly. Can't really do without it so :stuck_out_tongue:
```

---
## \#85 Posted by: shaman Posted at: 2019-04-04T13:46:06.735Z Reads: 127

```
True. Eventually shielding would be the way to reduce radiation. I assume that putting the controller in an aluminum enclosure would help reduce overall emissions.
```

---
## \#86 Posted by: shaman Posted at: 2019-04-04T14:03:22.296Z Reads: 124

```
[quote="linsus, post:82, topic:87227"]
Legally, no. You’re not in the clear if this is a commercial profiting product.
[/quote]

So what draws the line for considering something a commercial profiting product? I'm guessing no VESC or VESC derivative on the market has crossed into this threshold?
```

---
## \#87 Posted by: linsus Posted at: 2019-04-04T14:07:53.474Z Reads: 129

```
All of them have, if you accept money for it, you're obligated to be able to produce evidence of your stuff passing EMC compliances, in Sweden anyone can ask to see these documents and if the seller doesn't have them/Its not a ok product you can get hefty fines and even be asked to pull back all sold units if its hurtful enough. 

Part of this is the sole reason vedder doesn't want to sell it on his own.

The "hobby" sector usually doesn't draw this attention. But since the controller is finding its way into prebuilt stuff, I'm abit surprised noone got investigated yet.
```

---
## \#88 Posted by: shaman Posted at: 2019-04-04T14:10:45.093Z Reads: 127

```
[quote="linsus, post:82, topic:87227"]
Enertion dsnt have a single EMC cert, nor does Trampa, CE stamp is on the official VESC6 tho
[/quote]

[quote="linsus, post:87, topic:87227"]
obligated to be able to produce evidence of your stuff passing EMC compliances,
[/quote]

So these companies are currently taking a risk without these certs?
```

---
## \#89 Posted by: linsus Posted at: 2019-04-04T14:22:02.130Z Reads: 119

```
Very much so. Could even be calculated in the price ;)
```

---
## \#90 Posted by: shaman Posted at: 2019-04-04T14:24:43.754Z Reads: 116

```
hmmm...I may not take that risk. FCC "unintentional radiator" testing can run $1,000USD to $1500USD. Probably less costly than the consequences of an investigation. Yes the price tag could help compensate for such things without inflating the price beyond reason.
```

---
## \#91 Posted by: linsus Posted at: 2019-04-04T14:29:45.676Z Reads: 123

```
The fine in Sweden was 10 000 euro few years ago, if investigation would show that your product did not comply with the EMC standards + you pay for the test. If extreme enough you'd have to recall all products. So yea...

Sad truth is that even though we have these controlling organs run by our government together with EU. They dont have time to do more then a few random tests on products by huge commercial chains buying bulks of thousands. By the time they get tested they're usually taken out of the sellers current merchendise and replaced by something very similiar (that then needs a new test) and so on...

And the companies living of cheap chinese stuff of course uses this system to thier benefit. Once in a while they get nailed tho, but can afford the consequences.

The big risk is actually selling to different locations in the world.. Since different parts have different rules, USA and FCC beeing the strictest on radio emissions. You could get into some deep trouble xD.
```

---
## \#92 Posted by: shaman Posted at: 2019-04-04T14:34:17.835Z Reads: 121

```
Yes I can see how some just simply play the system. I'd rather do it right though. Especially since my controller design doesn't have any wireless communication devices. This makes getting these certifications cheaper and easier. Users can always add cheap modules if they want wireless. 

I'll need at least NRTL, CE, and FCC certifications to properly sell worldwide. There my be some I missed there. Some can simply be declared like CE. I think its worth the trouble in the long run. I won't be conducting business in constant fear of an investigation.
```

---
## \#93 Posted by: linsus Posted at: 2019-04-04T14:41:37.973Z Reads: 132

```
Start with one market to begin with and an EMC chamber that does pre-compliance (isn't 
accredited). Its alot cheaper and good enough. Not sure if you noticed, but you cant buy the VESC6 from trampa with the NRF module if you're in America.

Which I personally think is a good business practice by Trampa. 
https://media1.tenor.com/images/99e59449b7554b81bd40770ce32aa322/tenor.gif?itemid=7723689
```

---
## \#94 Posted by: shaman Posted at: 2019-04-04T14:46:01.172Z Reads: 126

```
Ah. I see there are some tactics here. It appears there are different ways to approach this. I really appreciate the advice. This information is hard to come by and may usually not be free. 

Regardless of certs, I still have to make something that works in the first place. It will be full steam into the New FOCers after the Cheap FOCer beta testing.
```

---
## \#95 Posted by: linsus Posted at: 2019-04-04T14:50:48.428Z Reads: 125

```
Its a very smaaaall department of nerds like me that work with this kind of shite. 
We're friendly and kind but dont like direct sunlight; .www.shortlink.se/en/
```

---
## \#96 Posted by: shaman Posted at: 2019-04-04T14:53:04.995Z Reads: 125

```
Yes...a familiar web page  :wink:
```

---
## \#97 Posted by: longhairedboy Posted at: 2019-04-09T18:50:48.448Z Reads: 123

```
84V FOC controllers? Holy shit. 

We have a test platform that could handle that. it has 10" pneumatic wheels, brushless inrunners, and 20mm belts, it just needs the ESC and a repacking of a drawer full of evolve cells.
```

---
## \#98 Posted by: banjaxxed Posted at: 2019-04-09T19:00:35.196Z Reads: 128

```
I wanna see a CAN-bused pair of Bad MF FOCer

@Martinsp has my address if you want to see it mated Gimp style to a set of these

 https://shop.electric-skateboard.net/diy-tuning/wheels-tyres-rims/367/beba-intermediate-eversion-10-x-4.00-5-offroad-e-boards-tyres

But only beach...we are very much talking about a serious e-vehicle & I am running out of body parts

Maybe @moon can encourage some carnage
```

---
## \#99 Posted by: moon Posted at: 2019-04-09T19:02:17.114Z Reads: 124

```
what the hell is that and what the hell is that site lol
```

---
## \#100 Posted by: shaman Posted at: 2019-04-09T19:13:31.589Z Reads: 127

```
Yep. Hope you guys got some low kV motors around.
```

---
## \#101 Posted by: banjaxxed Posted at: 2019-04-09T19:17:25.089Z Reads: 134

```
They are tubeless front kart wheel wheels 11" X 4", I think they mount to these
https://shop.electric-skateboard.net/diy-tuning/wheels-tyres-rims/575/a.m.v.-aluminium-rim?number=ESK8B10573.1

I think @Duffman has run something similar 

It would require a custom gear drive winky winky

Motor-wise, a pair of 130kv 80100, something like this

https://frchobby.en.alibaba.com/product/60481041439-803193582/MP_80100_KV130_RC_Outrunner_Brushless_Motor_for_E_Bike.html?spm=a2700.icbuShop.41413.10.487d7e15qVI6Na

Not Overkill, probably roadkill
```

---
## \#102 Posted by: Andy87 Posted at: 2019-04-09T19:22:12.505Z Reads: 129

```
😂😂😂

I was at one point some time ago close to order this wheels 😂
But the thing which hold me off was that I have no access to any cnc work shops and for now also no idea how I could get all the parts done I would need for it.
```

---
## \#103 Posted by: banjaxxed Posted at: 2019-04-09T19:33:20.176Z Reads: 130

```
Yeah, I think community-wise we are getting closer with various mounting options.

Duffman overcame that challenge by...well being able to custom make anything he wanted

Apart from a gear drive which supported the mounting points which is possible with the right person, the only thing needed is a custom standoff from the hub to the drive plate, that should be it.

Maybe we should take it to a new thread & not  FOC up Shaman's thread here, sorry about that old sport
```

---
## \#104 Posted by: moon Posted at: 2019-04-09T19:37:08.496Z Reads: 135

```
My gear drive uses an adapter to attach to  wheels. I imagine the adapter could be 3d printed out of nylon or something strong for testing

So it's probably possible

At the same time this thing looks like it needs some mad ratio

@banjaxxed pm me if you want to chat about this lolz
```

---
## \#105 Posted by: FredrikHems Posted at: 2019-04-09T22:20:25.687Z Reads: 129

```
@banjaxxed @moon I am literally designing a gear drive for these and the even bigger Mefo go kart tires right now. Aiming for a ratio of ~1:7 and helicals :yum:
```

---
## \#106 Posted by: shaman Posted at: 2019-05-31T17:58:38.931Z Reads: 102

```
Alright everyone. I’ve made a new thread in the esk8 news forum. Please redirect your attention over there if possible. The new thread is where I’ll be posting updates, answering questions, and receiving suggestions.

I am not actively deleting this thread on the esk8 builders forum. It will remain as a reference for all as long as it exists.

https://forum./t/some-new-focers-84v-vesc-6-based-controllers/1513
```

---
## \#107 Posted by: Gijs.wh Posted at: 2019-06-01T16:57:14.713Z Reads: 85

```
http://teamtriforceuk.com/a200s-v2/
I know you wil pay more but i think this is a way better option, way more output power
```

---
## \#108 Posted by: telnoi Posted at: 2019-06-01T17:09:15.407Z Reads: 84

```
What use is 200a? 80a at 12s is already enough to blow your socks off, at least with esk8. Wonder what motor size would be required to make full use of 200a continuous.
```

---
## \#109 Posted by: Gijs.wh Posted at: 2019-06-01T18:11:31.717Z Reads: 77

```
Wel ppl can finaly make use of there 80100 motors, and btw i draw 100a on 12s somtimes and i stil feel the need for more power
```

---
