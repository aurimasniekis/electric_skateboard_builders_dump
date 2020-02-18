# FATboy anti-spark switch

### Replies: 117 Views: 4711

## \#1 Posted by: Kug3lis Posted at: 2017-11-21T00:47:59.341Z Reads: 418

```
Hi guys, today I was working on the anti-spark switch to use together with momentary push button with push to hold to turn on/off features and in the end created bit overpowered really small anti-spark switch.

<img src="/uploads/db1493/original/3X/7/5/75ed3793cecc4ca09f9c34d745103cae3bdff6d7.PNG" width="690" height="384">

<img src="/uploads/db1493/original/3X/3/8/38191428b5d2d26eb11053cb807111bd4a2561ef.PNG" width="690" height="326">

Main Electrical Features:

* Controller by MCU
* High Side switch
* FDBL86361_F085 Mosfets (300A 80V)
* 10-70V operating voltage (up to 16s)
* Theoretically it should withstand 100A constant current but have to test it out before I can give my word on this
* Any push button
* 5V led output
* Really small module (18mm x 50mm)

Possible Software Features:

* Push and hold for e.g. 5s to turn on/off (prevents accidental turns off/on)
* Programmable push hold button time
* Programmable low voltage shut down (somehow programmable with same push button)
* Battery level by dynamic led blinking times?
* Ability to disable current intake into the battery

Now have to cram all those software features into small memory footprint.

If anyone has any more suggestion, please comment :stuck_out_tongue_winking_eye:
```

---
## \#2 Posted by: evoheyax Posted at: 2017-11-21T00:50:54.258Z Reads: 357

```
Sounds good to me... We need more solutions. Just had a high speed spill today thanks to a failed vedder anti sparkswitch (direct fet version). Feel like xt90 loop switches are the only safe option now.
```

---
## \#3 Posted by: Kug3lis Posted at: 2017-11-21T00:51:50.317Z Reads: 348

```
What happened?
```

---
## \#4 Posted by: evoheyax Posted at: 2017-11-21T01:37:55.891Z Reads: 338

```
Was on the end of my route to my university, 5 mile trip, and on the last hill (15% grade), I got jerkiness from the motors. They lost power, regained power, lost power, regained power, that loop a few times, and finally lost it. Thanks to the v4 hummie hubs in 4WD, I can climb 20% grade hills even at over 30 mph. I was full throttling it up hill, made it half way, and this happened. Now the gate is stuck open, so the power switch is useless. It's now just a hazard, cause it could cause this again, so I just removed it and have everything directly soldered. Till someone comes up with a solution, my board stays on 24/7, lol.

After spending years of developing these motors with hummie, I finally feel they can't fail anymore and I haven't had any failures so far in the few hundred miles I've done on them so far. My chaka quad vesc is rock solid, a few problems with caps falling off due to vibration (after 1500-2000 miles of use i'll say), but that's all in great working condition now.

Just when you think everythings solid, something will fuck up your day. I landed on my 3k laptop, so now I have to deal with that. All because of a stupid power switch.

This is the same reason I don't like fuses in my circuits. They are another point of possible failure that I've personally seen friends eat it at 25+ mph. Simpler is safer...
```

---
## \#5 Posted by: Kug3lis Posted at: 2017-11-21T01:40:07.673Z Reads: 312

```
Hmm, have you been braking at that moment or something?
```

---
## \#6 Posted by: evoheyax Posted at: 2017-11-21T01:50:11.280Z Reads: 310

```
I was neither accelerating or braking. I was at a constant 25-30 mph.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-11-21T01:53:32.853Z Reads: 310

```
This is awsome :thumbsup:

Do you an idea of price point?
```

---
## \#8 Posted by: Kug3lis Posted at: 2017-11-21T01:56:36.249Z Reads: 306

```
Something like 40-70€ I guess, will see with parts, I will be ordering some PCBs and parts for the prototype by the end of the week if everything goes well will try to make a batch of them.
```

---
## \#9 Posted by: Blasto Posted at: 2017-11-21T02:29:35.437Z Reads: 301

```
This design as is, won't work.

there's a few things that don't seem right, but here is the most flagrant

<img src="/uploads/db1493/original/3X/e/b/eb6f6d44e45f68014e08079d5693cbabf85f423d.png" width="690" height="258">

you have no high current path on your ground, your tracks will blow at about 4-5A

Not sure what is U3, but if it's a linear regulator, that thing will get hot to the point of failling.
 
-no gate protection, no current limiter. will make U1 fail if it's a mcu
```

---
## \#10 Posted by: Kug3lis Posted at: 2017-11-21T02:37:06.793Z Reads: 280

```
U1 is not mcu, u2 is mcu, u3 is high voltage low current linear regulator ~50mA its rated for 3x higher voltages so shouldn't be a problem. I have already reconsidered ground plane.

The whole switching is based on high end BMS design
```

---
## \#11 Posted by: Blasto Posted at: 2017-11-21T03:02:49.648Z Reads: 278

```
[quote="Kug3lis, post:10, topic:38869"]
The whole switching is based on high end BMS design
[/quote]

ah that is why you have two fets drain to drain. (edit patata potato)

so in this case Q1 is not doing anything, except potentially blocking any regen, it's not contributing to switching the load. All the current will just go through it's diode.
```

---
## \#13 Posted by: Kug3lis Posted at: 2017-11-21T03:16:17.737Z Reads: 263

```
Wait what? They are not in series, they are back to back

It's full switching so if its turned off no current goes in or out
```

---
## \#14 Posted by: Cobber Posted at: 2017-11-21T04:06:16.917Z Reads: 247

```
I'd like some proven high Amp capable anti-spark switches. :pray:
100A cont. is minimum. 
160A cont. would be nice too, I know some one else who would buy a few as well  ;)
```

---
## \#15 Posted by: evoheyax Posted at: 2017-11-21T05:08:49.692Z Reads: 242

```
I agree. Now that I can do higher amps since I'm not using a power switch, I'm gona try 160 amps and see what happens :stuck_out_tongue: 

160a power switch would be nice. So would a bms though too...

The holly grail will be the bms + power switch, like j-tags bms. We need more though than just one option.
```

---
## \#16 Posted by: Kug3lis Posted at: 2017-11-21T09:36:04.122Z Reads: 226

```
I will start working on BMS these days, I have already made balancer part now just need main controller + power switches.

For higher current rating I can put 2x or 3x mosfets but first I want to see how single performs
```

---
## \#17 Posted by: Cobber Posted at: 2017-11-21T09:42:25.573Z Reads: 232

```
100A ill use as a pair... one for each esc, same as 160A
```

---
## \#18 Posted by: Kug3lis Posted at: 2017-11-21T22:53:28.910Z Reads: 238

```
Hi guys, I just updated the design, went from LDO to buck converter the LDO did not provide enough current for simple led. Because of the increase in size, I went double Mosfet's so it should be around ~200A but still, it's in theory. The new board size is 30x50mm

<img src="/uploads/db1493/original/3X/a/4/a4aca3cd529b25d527d2a636f7480c8dc2267d64.PNG" width="690" height="441">

<img src="/uploads/db1493/original/3X/f/d/fdc7f5a0276fbcfc27b875d7cc12fad57281110f.PNG" width="690" height="463">
```

---
## \#19 Posted by: Cobber Posted at: 2017-11-22T01:12:35.956Z Reads: 225

```
200A is a great idea. If you want to future proof the design as 2 x VESC6 stock can do 200A (100A ea.).
```

---
## \#20 Posted by: Kug3lis Posted at: 2017-11-22T01:13:05.167Z Reads: 224

```
If going by specs its 600A... But oh well...
```

---
## \#21 Posted by: Cobber Posted at: 2017-11-22T01:15:01.488Z Reads: 224

```
should be reliable then :thumbsup:
```

---
## \#22 Posted by: eLDoska Posted at: 2017-11-22T01:36:18.524Z Reads: 206

```
FDBL86361 without heatsink can handle max ~ 30A/mosfet
correct me if i am wrong - you have 2 layer pcb. with 2oz copper your traces could be max 30х0.07=2.1mm2. 
i doubt that 2.1mm2 copper will handle 200A current
```

---
## \#23 Posted by: Kug3lis Posted at: 2017-11-22T02:17:57.643Z Reads: 206

```
Who said I will not have a heatsink on the MOSFETs? The distance between wire (copper) and MOSFET input is small enough to handle this kind of currents, plus the MOSFET, and wire for 200A will also act as a heatsink for the heat transfer so as I say it theoretically after test runs I will be able to tell exactly it handles at which temperatures.
```

---
## \#24 Posted by: pshaw Posted at: 2017-11-22T02:46:54.778Z Reads: 196

```
Apologigizes dude. Your setup looks super promising I hope it comes together soon so I can get one :)
```

---
## \#26 Posted by: pshaw Posted at: 2017-11-22T02:51:23.205Z Reads: 194

```
10 characters
```

---
## \#27 Posted by: JdogAwesome Posted at: 2017-11-22T03:17:34.672Z Reads: 186

```
Alright so I'm confused. From what I can tell your using N-Channel MOSFET's that switch the negative side of a circuit, so how are you connecting the positive rail to the MOSFET'S then?
```

---
## \#29 Posted by: pat.speed Posted at: 2017-11-22T03:25:57.064Z Reads: 178

```
What? Two minutes ago you said you switch the negative side not the positive
```

---
## \#30 Posted by: Kug3lis Posted at: 2017-11-22T03:26:48.971Z Reads: 173

```
Sorry that messeg was to @pshaw changed message
```

---
## \#31 Posted by: JdogAwesome Posted at: 2017-11-22T03:35:27.909Z Reads: 172

```
So I'm still confused, are you switching the negative side of the circuit (low side) or the positive side (high side).
```

---
## \#32 Posted by: Kug3lis Posted at: 2017-11-22T03:36:25.532Z Reads: 163

```
positive side (high side)
```

---
## \#33 Posted by: JdogAwesome Posted at: 2017-11-22T03:39:44.979Z Reads: 170

```
Yeah but how, your N Channel MOSFET'S source is connected to the positive input of the battery, how does that work?
```

---
## \#34 Posted by: Kug3lis Posted at: 2017-11-22T03:41:10.967Z Reads: 171

```
It works as high side switch? Half bridges works the same
```

---
## \#35 Posted by: JdogAwesome Posted at: 2017-11-22T03:48:38.389Z Reads: 174

```
Ohh nevermind I was so confused lol was messing up my understanding of N-channels sorry man, thanks for your patience.
```

---
## \#36 Posted by: Kug3lis Posted at: 2017-11-22T03:52:50.624Z Reads: 174

```
No problem I was prepared for more detailed answer :D N-channel uses electrons to transfer current that's why they are better situated for this kind of application but minus that you need to drive gate higher voltage than source, so you need bootstrapped gate driver, then P-channel uses holes which is not really efficient way of transferring but the easiest
```

---
## \#37 Posted by: NAF Posted at: 2017-11-22T06:00:49.941Z Reads: 167

```
@evoheyax Just curious ..who made your switch ?
```

---
## \#38 Posted by: evoheyax Posted at: 2017-11-22T15:45:43.664Z Reads: 166

```
Golden Husky... Though I found another problem. My bluetooth module was causing some issues (sending a control signal it seemed like, which it shouldn't be). Not sure if the power switch caused the bluetooth module to fail or vice versa. Will do more digging today.
```

---
## \#39 Posted by: GrecoMan Posted at: 2017-11-22T15:52:24.557Z Reads: 166

```
aw shit now i’m scared my bluetooth is possessed
```

---
## \#40 Posted by: evoheyax Posted at: 2017-11-22T16:09:38.167Z Reads: 175

```
Well it is a risk I suppose. I've done hundreds of miles, probably closer to a thousand miles with my bluetooth module and never had an issue until now. Again, it'll be important to get the whole pictures. All I know at this point is I was going up hill, got jitters, and power switch stayed on (wouldn't turn off). I thought originally that the vesc's weren't getting power, but they were. Just the receiver wouldn't turn on. I then noticed a buzzing sound coming from the vesc's. I unplugged the bluetooth module, and that sound went away and receiver powered up. Power switch is still broken. Not sure if the bluetooth module is also broken or if it's the VESC. I also notice at the same time, a busted capacitor (the big tube ones) on the master vesc.

So:
- Broken power switch
- Possibly broken bluetooth module
- Possibly broken vesc (unlikely, but possible)
- Busted capacitor

This is going to be puzzle to solve though.

The bluetooth module is capable of interfering with the control signal (since they can send their own control signal while the ppm sends its normal control signal). That could cause jittering.

The power switch could of been opening and closing the mosfets (a short somewhere maybe), which could of caused the jittering.

The capacitor is a prime suspect of the jittering. If that blew, I would be left without enough capacitance, and the voltage would fluctuate under high load, like I was at the time.

Too many possibilities, but I'll try to dig more see what I can rule out.
```

---
## \#41 Posted by: Kug3lis Posted at: 2017-11-22T16:19:15.457Z Reads: 161

```
Check if components on switch has not micro breaks on solder joints because of vibrations
```

---
## \#42 Posted by: LukePL Posted at: 2017-11-22T18:47:09.286Z Reads: 178

```
Guys I have a OT question but maybe close to switch subject. This BMS https://pl.aliexpress.com/item/12S-120A-version-D-lipo-lithium-Polymer-BMS-PCM-PCB-battery-protection-board-for-12-Packs/32799811707.html?spm=a2g17.search0104.3.80.KiDH80&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10151_10065_10344_10068_10345_10342_10343_10340_10171_10341_10541_10562_10084_10083_10304_10307_10301_10539_10312_10059_10313_10314_10534_10533_100031_10103_10073_10594_10557_10596_10595_10142_10107,searchweb201603_25,ppcSwitch_4&btsid=f93fe07b-7595-44f7-8e71-4c6b53f2c88f&algo_expid=d5e4b878-c9b7-47af-9c32-d901f527abb0-10&algo_pvid=d5e4b878-c9b7-47af-9c32-d901f527abb0&rmStoreLevelAB=3
has temperature switch. Can I hook up some standard switch and do you think it's possible that will work this way?
```

---
## \#43 Posted by: longhairedboy Posted at: 2017-11-22T18:58:39.102Z Reads: 190

```
@evoheyax for high amp loads you can run the vedder switches in parallel. 

<img src="/uploads/db1493/original/3X/9/4/94ee54fe91718a5339d047411aaefe88c759c783.jpeg" width="667" height="499"><img src="/uploads/db1493/original/3X/7/0/704199c237cfa6904b97374c5e4266975d638f8d.jpeg" width="375" height="500">

these are modified with 75v fets and when used with a 60 amp BMS they basically never blow at all. But when we went full discharge on Tattu lipo packs it was time to spread it around a little. Phoned a freind and we discussed how to wire this properly without draining the wrong drain. It works like a champ.
```

---
## \#44 Posted by: Kug3lis Posted at: 2018-01-10T10:28:38.772Z Reads: 172

```
Is anyone still interested in this?
```

---
## \#45 Posted by: bimmer Posted at: 2018-01-10T10:31:06.265Z Reads: 173

```
I'm honestly in talks of having the DieBieBms made at a factory and it will make all sparkswitches obsolete.
```

---
## \#46 Posted by: Kug3lis Posted at: 2018-01-10T10:36:31.067Z Reads: 172

```
It doesn't matter where the board is made, the design is the key element here. This one also would make everything obsolete. This has microprocessor so I can do like hold to turn on/off battery level on led blinking speed and etc. Plus this board disconnects positive wire not negative like all others.

P.S. It would also had a aluminium case to cool down those mosfets, and etc.
```

---
## \#47 Posted by: bimmer Posted at: 2018-01-10T10:41:59.346Z Reads: 174

```
![687b83287560d0d4d5ab3bb2d80b59668e9fb60f_1_666x500|666x500](upload://3DjPRk40ElXw1JhiIBHh6tcikG7.jpg)
Jtag has opensourced this bms and it can be  made as low as 60$ in the right  quantity wich is  the price of a  decent bms and sparkswitch,
```

---
## \#48 Posted by: SimosMCmuffin Posted at: 2018-01-10T10:44:34.147Z Reads: 169

```
I can create a sparkswitch with just two pieces of wire :grin:
```

---
## \#49 Posted by: Kug3lis Posted at: 2018-01-10T10:46:03.117Z Reads: 166

```
Yes, but current wise it's the same as other spark switches, just two MOSFETs without any heatsinks so no more than 40A could be pulled continuously.
```

---
## \#50 Posted by: lock Posted at: 2018-01-10T12:04:45.515Z Reads: 163

```
Well he’s working on that [MoreAmpsSheild](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/230) that apparently handles 240A, and does a bunch of other neat stuff you’d probably want if you were running that much current.

Still, get the feeling some people would still like to forgo the complexity of a BMS. So a good switch, is still a good idea.
```

---
## \#51 Posted by: fedestanco Posted at: 2018-01-10T12:08:28.699Z Reads: 160

```
[quote="bimmer, post:47, topic:38869"]
60$ in the right  quantity
[/quote]

No matter the quantity it's impossible to go that low. Seriously have a look at the BOM.
```

---
## \#52 Posted by: Kug3lis Posted at: 2018-01-10T12:10:12.502Z Reads: 159

```
On his more amps shield I do not saw any more mosfets to handle more current so I don't know how he is going to get more current from that PCB...
```

---
## \#53 Posted by: Kug3lis Posted at: 2018-01-10T12:11:07.082Z Reads: 161

```
Plus my switch uses the same logic as his board for switching power, its kind the best solution you can get. Just I use more powerful mosfets and mcu ;)
```

---
## \#54 Posted by: SimosMCmuffin Posted at: 2018-01-10T12:20:35.822Z Reads: 166

```
[quote="JTAG, post:230, topic:2639"]
By a customer's request; a shield that adds 6 temperature sensors, a DC - DC converter (for 12V on the can bus), 4 fans with rpm control, buffered IO, relay driver, additional pre-charge method a**nd shunt to allow currents up to 250A** :heart_eyes:.
[/quote]

It would seem that there aren't more transistors on the board, but rather more parallel/lower resistance shunts so they can measure currents up to 240 A, without melting their current shunt resistors. Or so I would understand from his quoted sentence and the linked pictures in the reply.

I also have to wonder with @Kug3lis how they plan to keep their transistors from escaping into the atmosphere at such high currents.
```

---
## \#55 Posted by: Kug3lis Posted at: 2018-01-10T12:33:15.030Z Reads: 166

```
That's why I am really curious how they handle the current, because current does not divide equally between paths so I am bit sceptical...

Plus the IRFS7530 has some high heat output at that current...

250A through 0.0014 Ohm dissipates 87.5W of power, P = I^2 * R. 87.5W x 313 K/W gives a junction rise above ambient of 27387 K, or 3500C.... :joy: (can be really wrong calculation as I don't remember correct formulas) and it's only for single mosfet.
```

---
## \#56 Posted by: longhairedboy Posted at: 2018-01-10T12:43:32.263Z Reads: 158

```
[quote="bimmer, post:47, topic:38869, full:true"]
Jtag has opensourced this bms and it can be  made as low as 60$ in the right  quantity wich is  the price of a  decent bms and sparkswitch,
[/quote]

Where? and in what quantity? That deal sounds like a shenzen bait and switch to me. 

[quote="fedestanco, post:51, topic:38869"]
No matter the quantity it’s impossible to go that low. Seriously have a look at the BOM.
[/quote]

That's what i was thinking. Maybe under $100 is possible.. somewhere...

[quote="Kug3lis, post:49, topic:38869, full:true"]
Yes, but current wise it’s the same as other spark switches, just two MOSFETs without any heatsinks so no more than 40A could be pulled continuously.
[/quote]

why is it rated for a 100amp fuse then? I run twin IRFS7730 mosfets at well over 50 amps all the time and they're fine. They seem to start having issues right around 60 amps under 200+ pound loads and the speeds associated with those amps, which for my weight class is above 40mph. Are 7530s that much different?
```

---
## \#57 Posted by: Kug3lis Posted at: 2018-01-10T12:45:06.761Z Reads: 145

```
The load of skateboard is not continues, as I am saying for continues load max 40A, but for longboard 50-60A should be enough but not 250A as he states in his message...
```

---
## \#58 Posted by: Kug3lis Posted at: 2018-01-10T12:46:33.396Z Reads: 146

```
On my board I will just put several SOT227B style mosfets on big ass aluminium plate and will not have any problem even with 200A :D
```

---
## \#59 Posted by: SimosMCmuffin Posted at: 2018-01-10T12:48:41.850Z Reads: 156

```
Also, I'd like to give you some constructive input on your anti-spark switch design.

You really lose the pro of using more powerful MOSFETs if you use them in the fully blocking setup, because you actually end with more dissipated power overall compared to the 2 parallel IRFS7530s in one direction. Your overall Rds(on) will be higher due to the current having to run through 2 silicon dies in series (even in the parallel version). Now if you plan on making a heatsink for it, then you might make up for the increased heat production by being able to pull the heat away more effectively due to more surface area to move the heat off of the packages to the heatsink, but overall wouldn't it still run hotter, at least power dissipation wise?

IMO, MCU seems a bit overkill. I (personal opinion) believe that most people would want their e-switch to be as simple as possible. AKA it's either on or off. They want to disconnect their battery from their motor controller by holding a switch down for a couple of seconds and connect it back by doing the same again. I doubt they want to start faffing about with firmware and flashing it to the MCU. How are they supposed to flash the firmware again? are you going put a header to the board, which they can use? How many people have the programmers and the know-how needed to do this? Are you going to flash every board yourself you plan to sell? I really don't think the MCU is the best choice in this case, but rather more simple logic gate based one, which's output is toggled by holding down a momentary pushbutton.

Just my two cents.
```

---
## \#60 Posted by: Kug3lis Posted at: 2018-01-10T12:56:43.621Z Reads: 155

```
I use them in the fully blocking way just to prevent burning the battery with a current running in from VESC or etc then the board is off. Either way, its how normal BMS looks, this whole switch is just a part of professional grade BMS just the switching part, the same design is in jtag version of BMS too. The MCU will be one time programmed because I saw saying that vibrations can make button switch and turn off the board while riding if anyone wants it can be a simple toggle switch. You will not need to program it or do anything related to it.

On the other note about fully blocking mode is like to prevent inbound current to battery then the battery is fully charged, or etc. It would work partially as BMS without balancing. Turn off the load then minimum voltage is reached or etc.
```

---
## \#61 Posted by: SimosMCmuffin Posted at: 2018-01-10T13:01:31.308Z Reads: 159

```
Are you sure about the mosfet arrangement in the DieBieBMS being in fully blocking arrangement?

![MosfetArrangement_diebie|690x339](upload://85sfeEkyfTdc9t5Kv59ibfADzhW.png)
```

---
## \#62 Posted by: Kug3lis Posted at: 2018-01-10T13:02:07.981Z Reads: 156

```
Yeah I just opened and saw he is using two different paths. My bad but if you look in other reference design of bms and etc you will see ;)
```

---
## \#63 Posted by: Kug3lis Posted at: 2018-01-10T13:02:45.829Z Reads: 161

```
![24 PM|418x268](upload://oiliv1Lcjww6MittEObmzUPb4as.png)
```

---
## \#64 Posted by: SimosMCmuffin Posted at: 2018-01-10T13:10:31.134Z Reads: 157

```
I would also then bring into question about how useful the fully blocking arrangement is still going to be, because I _assume_ that most(?) esk8 motor controllers are VESC based, in which you can set the max DC bus voltage limit, so you can disable regen brakes if your battery voltage rises too much, making the fully blocking setup needless.

Then in the case that you're going downhill braking and the VESC cuts out, because the DC bus voltage rises too high. then you're still going to be in some trouble, because now you can't brake, your speed is increasing, your motor is producing higher BEMF and your MOSFET Vdss is still 60V at which point it will experience breakdown and the current will then go through it and then through the body diode of the other MOSFET into the battery, again making the fully blocking setup seem a bit... useless.

We need to dump energy somewhere if we want to slow down. So in a dangerous scenario as pictured above, I would say that it's better to ruin a battery, then be out of control.
```

---
## \#65 Posted by: Kug3lis Posted at: 2018-01-10T13:14:22.823Z Reads: 155

```
I mean yes, I was talking more case then power is switched and you push the board and then motor acts as generator and leaks current :D But I mean if there is a need for simple switch without blocking I can change the design, I just wanted to make simple fully disconnect switch on positive path not negative and only half disconnecting. The whole closing charging and etc was just an Idea what I can do with MCU in place. I am doing this module for the community, not for myself so I am up for suggestions and ideas.
```

---
## \#66 Posted by: SimosMCmuffin Posted at: 2018-01-10T13:20:05.920Z Reads: 156

```
I fully agree that having the N-channel FET on the ground side is not ideal and I would much rather see the e-switch being a high-side solution. I have also done some idea work on how to make it high-side, higher current with simple IC solution (no programmables).

What I would like to know is, what's the failure mode of the Vedder anti-spark switches, because many people seem to be breaking them, but I want to know _why_ they are breaking, so it could be remedied if I or somebody else were to make a high-side e-switch.
```

---
## \#67 Posted by: Kug3lis Posted at: 2018-01-10T13:23:24.511Z Reads: 154

```
For the high side, you need only high side MOSFET driver IC and that's all... Nothing special, I can adapt this design to not be fully blocking, and be only one side and other side diode will leak current pack to pack, the MCU can be replaced with simple toggle switch if that's the case and that's all...
```

---
## \#68 Posted by: JTAG Posted at: 2018-01-10T13:30:59.887Z Reads: 159

```
I seem to have missed this discussion and the questions that were raised here. Ill elaborate on some points shortly, for now let me just state that the MoreAmpsShield is not capable of switching the high currents, it is just capable of measuring (which I still have to validate trough, I^2 is a bitch) it. Switching happens trough a relay:

![IMG_20180104_112715|666x500](upload://uLR7rX64lzrmzHVNOcZJVOzUE0U.jpg)

Eventually ill make it solid state, fully blocking with a shitload of FET's and a heat sink, this will also be a real challenge :sweat: .
```

---
## \#69 Posted by: SimosMCmuffin Posted at: 2018-01-10T13:32:26.042Z Reads: 152

```
Which switch type would be safer, a pushbutton with hold down time or a toggle switch? 

Toggle switch would make the circuitry super simple and you could then do the MOSFET drive with only 
the BQ76200 making the BOM super small, because you don't need a step-down regulator.

Pushbutton implementation would need more complex circuitry, but would also be doable with relatively low cost...

I think staying with MOSFET for the switching transistor type is still more sensible than going to an IGBT, because most of the time we're still operating in lower current range when cruising. IGBTs would only have the smaller power dissipation advantage in the high currents, but would run hotter in the lower currents... Anyway heat dissipation becames relevant at higher currents regardless of transistor type.
```

---
## \#70 Posted by: Kug3lis Posted at: 2018-01-10T13:33:29.294Z Reads: 141

```
Hehe, sorry I did not follow the discussion on your thread about it. You should definitely think about SOT227B and big ass aluminium plate if you are making only single unit as those are like 20-30$ each
```

---
## \#71 Posted by: Kug3lis Posted at: 2018-01-10T13:34:55.772Z Reads: 146

```
Yes, toggle would be super easy.

Where did you get the "IGBT" idea? IGBT are only liable from 200V+
```

---
## \#72 Posted by: SimosMCmuffin Posted at: 2018-01-10T13:38:48.298Z Reads: 149

```
[quote="Kug3lis, post:70, topic:38869"]
You should definitely think about **SOT227B** and big ass aluminium plate if you are making only single unit as those are like 20-30$ each
[/quote]
I couldn't find anything but IGBTs with that package type
```

---
## \#73 Posted by: Kug3lis Posted at: 2018-01-10T13:39:37.133Z Reads: 150

```
https://octopart.com/search?category_ids=4229&start=0&specs2.20.values=Chassis%20Mount&specs2.2.values=SOT-227-4&specs2.2.values=Module&specs2.2.values=SOT-227&specs2.2.values=SOT

500+

I am going to use this ones in my project. 3 in parallel https://octopart.com/ixfn360n10t-ixys-19075359?r=sp&s=J-ouvTuVQzOMVXv7MIETyA and one for charging path
```

---
## \#74 Posted by: SimosMCmuffin Posted at: 2018-01-10T13:51:06.574Z Reads: 146

```
Ah, my bad.

Space conscious design is still not reasonable with that hunky package, because their Rds(on) on still higher than the FDBL86561-F085 so the heat problem still persists. In your case they are most likely better because you mentioned mounting them to a heatsink and that big package can transfer heat so effectively.

E-switch:
Just 2 FDBL86561-F085 in parallel would still be a direct upgrade compared to 2 IRF7530 in parallel Rds(on) wise and with a very similar sized package. But I'm still wondering if it's the heat that is killing these anti-spark switched or some drain (battery) side inductive voltage spikes...
```

---
## \#75 Posted by: Kug3lis Posted at: 2018-01-10T13:54:37.526Z Reads: 141

```
I am using SOT-227 because I will be using copper bus bars on multiple xt90 connects I have 4 x 4 configuration so I don't want to do 16 cables lying around. Then using SOT-227 I can just screw copper bars to it and attach it to the aluminium lid of my battery case I know its overkill but its better than dealing with small tracks and etc.

Regarding the problems, I have big suspicious of Vgs voltage being the case on high temperate and causing MOSFET's to not open fully.  Which makes Rds supper high and it burns the metals inside which makes them open or etc. But in any case I think switching part is a problem there...
```

---
## \#76 Posted by: SimosMCmuffin Posted at: 2018-01-10T14:03:22.286Z Reads: 140

```
http://www.electric-skateboard.builders/uploads/db1493/original/3X/5/c/5caf3aad4cfb0f20cecc538920acef64bc97fd6d.png

Not sure if this is the original schematic, but wouldn't the Mosfets be only for a short-time in the ohmic region while the gate charges through the 1M ohm resistor once the switch is closed and then the zener clamps the voltage to some sensible level?

Do the gates charge too slowly and the VESC is used too soon to power a load, while the Mosfets are still in the ohmic region causing them to burn almost instantly??

This could be easy to test with a oscilloscope, but I don't have those anti-spark switches...
```

---
## \#77 Posted by: Kug3lis Posted at: 2018-01-10T14:09:33.580Z Reads: 134

```
The problem is not vesc but capacitors, have you tried to plug in lipo pack without XT90S connector have you heard the pop sound just from connecting the connectors? The inrush current is so big that I guess mosfets just pops instantly open or etc.
```

---
## \#78 Posted by: SimosMCmuffin Posted at: 2018-01-10T14:14:06.894Z Reads: 140

```
I did think about the caps for a moment, but dismissed the idea, because the capacitance isn't huge, but they do pull quite a wallop of current in the beginning... And if the gate voltage rises even slightly slowly, that might cause quite the power spike over the drain and source... Could be the cause...

Use a pre-charge FET with the BQ76200, because it supports it?
connect the switch directly to precharge_enable with a zener clamp and then wire the discharge_enable via RC circuit to give it some delay and use a zener clamp?
```

---
## \#79 Posted by: longhairedboy Posted at: 2018-01-10T14:17:13.872Z Reads: 133

```
[quote="Kug3lis, post:77, topic:38869, full:true"]
The problem is not vesc but capacitors, have you tried to plug in lipo pack without XT90S connector have you heard the pop sound just from connecting the connectors? The inrush current is so big that I guess mosfets just pops instantly open or etc.
[/quote]

this issue has led to a very specific order of operations when building my boards. I've popped open perfectly good eswitches before, ones with 100s, even 1000s of miles on them, just by doing things in the wrong order. 

eswitch needs to be fully assembled and OFF when connecting to the VESC after connecting it to the battery. This means using a shorted jumper to keep it off during assembly since the rocker or pushbutton will just get in the way of everything. 

if the switch is ON when connecting things it has a small chance of staying on forever.
```

---
## \#80 Posted by: SimosMCmuffin Posted at: 2018-01-10T14:38:02.143Z Reads: 139

```
Well, aren't there essentially 3 possible failure modes on the Mosfets?

Vgs limits: +-20 V on gate. Is something weird happening to the gate voltage when it's charged to the zener clamping voltage and we connect the VESC's capacitive load and we have some inductance in the wiring. causing the Vgs voltage to cross it's absolute max rating?

Vdss limit: Do we have a breakdown on the drain-source gap, due voltage spike caused by the current spike and wiring inductance?

Heat death: Too slowly climbing gate voltage leaves the Mosfet in the ohmic region and current spike then heat kills the silicon die? Unlikely I would say, because  

[quote="longhairedboy, post:79, topic:38869"]
if the switch is ON when connecting things it has a small chance of staying on forever.
[/quote]

Surely the gate voltage has already reached the zener clamping voltage at this point, meaning that the Mosfet should be fully conductive...

These cases should be probed with oscilloscope while connecting to a load in both OFF and ON states and see what's going on at the Mosfet's gate, drain and source.
```

---
## \#81 Posted by: longhairedboy Posted at: 2018-01-10T14:56:25.666Z Reads: 143

```
i don't understand why we're still here. 

i was able to vastly improve the vedder spark switch simply by changing the mosfet out with a better part number. ITs fucking magical compared to most of the ones out there that aren't built into a BMS. 

Yet that design is still flawed. I have fried every eswitch there is. I even bought an $80 direct fet switch from austria and it died on connection. 

what the fuck is so damned complicated about building an eswitch that can handle 60-80 amps and not fry on or blow up? Do we need to use relays? I'm not really interested in experiencing the effects of the vibrational forces of an esk8 on a traditional servo-thrown type relay, so what, heftier solid-state-ier ones? 

Even the ones i'm trying to make myself as an experiment have some dumb fucking issue with the 12v for the LED in the pushbuttons, so i now have to see how reliable they are when not using that 12v rail. 

its fucking retarded.
```

---
## \#82 Posted by: JTAG Posted at: 2018-01-10T14:57:41.054Z Reads: 139

```
![image|690x126](upload://zG23iKDz8gpkpIugihxZEYCoCF2.png)

Yep this function saved me a couple of times replacing the FET's xD.
```

---
## \#83 Posted by: Kug3lis Posted at: 2018-01-10T15:00:36.905Z Reads: 141

```
Thats why i want to use mcu with this ;)
```

---
## \#84 Posted by: Pimousse Posted at: 2018-01-10T15:34:23.664Z Reads: 140

```
So if I understand correctly, you activate precharge and you wait for the output voltage to reach a percentage of the pack voltage to switch to discharge state ?

I'm coding the firmware of Raphael Chang BMS (as we have the HW but the project has been stopped before having the FW) and I'd like to check that this feature has been coded as well (but it sounds familiar to me).
```

---
## \#85 Posted by: SimosMCmuffin Posted at: 2018-01-10T17:30:10.389Z Reads: 139

```
![e_switch-schema|690x384](upload://qC4MWeZpW9nPeSdRxVwoQ4RbT13.png)

How about doing it with only passives like this?

When switch is turned on, Pre-charge is immediately turned on and the P-channel FET starts charging load capacitance via high impedance path. Meanwhile a RC circuit slowly raises the DSG_EN pins voltage and it will after some time turn the big N-channel FETs then on, giving us a low impedance pathway for high currents.

the RC circuit can be used to tune the pre-charge time.

Just noticed btw, that the P-channel FET is the wrong way around, but throwing this out here as an idea.
```

---
## \#86 Posted by: Kug3lis Posted at: 2018-01-10T17:33:16.107Z Reads: 131

```
those en pins are like 1V high or something so you will need I don't know :D

Digital high is 1.2V
```

---
## \#87 Posted by: SimosMCmuffin Posted at: 2018-01-10T17:40:29.681Z Reads: 131

```
That's why there is the 50k resistor and then the 5V zener to clamp the voltage. The voltages on the EN-pins should rise to around 5V or am I missing something?
```

---
## \#88 Posted by: Kug3lis Posted at: 2018-01-10T17:41:56.716Z Reads: 129

```
Never mind I did not saw that RC was on DSG not on PCHG.

P.S. You don't need to enable CP_EN
```

---
## \#89 Posted by: SimosMCmuffin Posted at: 2018-01-10T17:42:28.679Z Reads: 133

```
Don't I need to enable the charge pump so I can drive the N-channel gates high?
```

---
## \#90 Posted by: Kug3lis Posted at: 2018-01-10T17:44:17.790Z Reads: 135

```
http://www.ti.com/lit/ds/symlink/bq76200.pdf

> Charge pump enable (internally logic ORed with CHG_EN and DSG_EN
signals)

> Note that when either the CHG_EN or DSG_EN is enabled, the charge pump will be automatically enabled even
if the CP_EN is in the disable state. It is recommended to enable the charge pump via CP_EN pin during system
start-up to avoid adding the tCPON time into the FET switching time during normal operation.
```

---
## \#91 Posted by: SimosMCmuffin Posted at: 2018-01-10T17:45:16.901Z Reads: 123

```
Ah, yes. Well, even simpler then :D
```

---
## \#92 Posted by: Kug3lis Posted at: 2018-01-10T17:47:00.813Z Reads: 117

```
I also incorporated some protections on mosfet gates similar to @jtag schematic
```

---
## \#93 Posted by: b264 Posted at: 2018-01-10T17:51:22.430Z Reads: 129

```
[quote="SimosMCmuffin, post:69, topic:38869"]
Which switch type would be safer, a pushbutton with hold down time or a toggle switch?
[/quote]

5s hold time momentary

flying sticks won't power off board
```

---
## \#94 Posted by: Kug3lis Posted at: 2018-01-10T17:52:03.193Z Reads: 127

```
:joy: :joy: :joy: :joy:

10char
```

---
## \#95 Posted by: SimosMCmuffin Posted at: 2018-01-10T17:55:40.217Z Reads: 130

```
You know what @Kug3lis, just go for the MCU.

What micro were you planning on? ATtiny?
```

---
## \#96 Posted by: Kug3lis Posted at: 2018-01-10T17:56:22.169Z Reads: 123

```
I spent same time trying to make it mculess but then said fuck it and went with mcu :D
```

---
## \#97 Posted by: Kug3lis Posted at: 2018-01-10T17:57:12.558Z Reads: 130

```
Hm, dont remember now :D maybe atmel or maybe st

I think its Attiny I guess, because I don't use st8 and stm32 doenst have 8 pin case

Ahh yes, it's attiny because I thought of programming chips off board and then just soldering them in ;)
```

---
## \#98 Posted by: SimosMCmuffin Posted at: 2018-01-10T17:59:30.310Z Reads: 134

```
an ARM MCU might be a bit overkill :grin:
Although ARM does have the SWD programming interface, less pins needed
```

---
## \#99 Posted by: Kug3lis Posted at: 2018-01-10T17:59:49.647Z Reads: 136

```
Trust me arm cost cheaper than avr...
```

---
## \#100 Posted by: SimosMCmuffin Posted at: 2018-01-10T18:00:49.718Z Reads: 141

```
![tiiny4|690x267](upload://9waFQaYjL4KjRM0D9nE16eMXw87.png)
```

---
## \#101 Posted by: Kug3lis Posted at: 2018-01-10T18:02:04.015Z Reads: 141

```
I see you like challenges and you want to code a program for 512-byte flash? :joy: :joy: :joy: :joy:
```

---
## \#102 Posted by: SimosMCmuffin Posted at: 2018-01-10T18:02:57.192Z Reads: 141

```
When in doubt, whip out the assembly :D
```

---
## \#103 Posted by: SORRENTINO Posted at: 2018-01-10T18:03:18.218Z Reads: 138

```
@Kug3lis be nice to have an automatic off after a certain amount of hours. I know a few people that left there boards on for a while and came back to dead batteries :smile:
```

---
## \#104 Posted by: Kug3lis Posted at: 2018-01-10T18:04:04.753Z Reads: 140

```
Sorry but this project will definitely not worth whipping out assembly :D

@SORRENTINO yep like I said possibilities is endless then you have MCU with button, led and voltage of pack

I even had idea to code like you program cell count and it can blink according battery percentage :D
```

---
## \#105 Posted by: SimosMCmuffin Posted at: 2018-01-10T18:08:39.997Z Reads: 142

```


[quote="Kug3lis, post:104, topic:38869"]
I even had idea to code like you program cell count and it can blink according battery percentage :smiley:
[/quote]

"Rough estimate of battery percentage". Voltage only, is not the best thing to go on estimating how much juice is left, especially when we have very different sized batteries and chemistry.
```

---
## \#106 Posted by: bimmer Posted at: 2018-01-10T21:23:05.241Z Reads: 143

```
Sorry my bad at 200 untis the Price is 95$
```

---
## \#107 Posted by: SimosMCmuffin Posted at: 2018-01-16T10:27:23.294Z Reads: 146

```
I have a very strong hunch about the vedder's anti-spark switches failure mode.

I was looking at possible MOSFETs for work related project on digi-key and looked at the search filter "input capacitance" and just thought: "I should perhaps figure out what the input capacitance does for it to be an available filter on MOSFETs"

Well, quick google search lead to this stackExchange question: https://electronics.stackexchange.com/questions/83712/gate-capacitance-and-miller-capacitance-on-the-mosfet

And the approved answer's relevant part had the following:

> Consider the MOSFET above switching a 10A load from a supply voltage of 50V. If you drive the gate to turn the device on the drain could be expected to fall from 50V to 0V within a few hundred nano seconds. Unfortunately the rapidly falling drain voltage (as the device turns on) removes gate charge via the miller capacitance and this can begin to turn off the device - it's called negative feedback and can result in less than ideal switching times (on and off).
.
The trick is to ensure that the gate is over-driven slightly to accommodate this. Look at the following picture taken from the FQP30N06L data sheet: -

Could it be, that if the capacitive load is connected while the e-switch is turned on, the weak 1M pull-up resistor is not enough to keep the gate voltage high, because the miller capacitance causes the gate voltage to dip momentarily and this with the big in-rush currents causes the MOSFET to burn out due to the increased Rds(on)?

Thoughts on this? Would be pretty easy to probe the gate and see what the voltage does on load connection.
```

---
## \#108 Posted by: Kug3lis Posted at: 2018-01-16T10:46:21.596Z Reads: 144

```
That can be, I am not much into analogue electronic science but it sounds like it can be. Something with bad turn on/off of mosfets. I never understood how good plain circuit can be for controlling mosfets for such high voltage and load...
```

---
## \#109 Posted by: squishy654 Posted at: 2018-02-13T17:57:14.591Z Reads: 123

```
Why are you guys not using high amp relays and making them antispark??
```

---
## \#110 Posted by: Kug3lis Posted at: 2018-02-13T18:02:54.056Z Reads: 123

```
High current relays sometimes can stick together which will be useless if you want to turn them off ;) Plus the price of relay and mosfets ;)
```

---
## \#111 Posted by: squishy654 Posted at: 2018-02-13T18:06:37.398Z Reads: 124

```
Seems the price tag of a pile of burned out mosfets costs a lot more than one sound functional relay made to handle the power..
```

---
## \#112 Posted by: Kug3lis Posted at: 2018-02-13T18:13:22.220Z Reads: 125

```
Plus you will need 12v to drive it :D
```

---
## \#113 Posted by: squishy654 Posted at: 2018-02-13T18:14:30.276Z Reads: 127

```
I have a 12v bus on many of my boards for LED lighting and tunes..simple to fix by adding a cheap regulator..you could even integrate such a regulator into any relay design...it's just a chip
```

---
## \#114 Posted by: b264 Posted at: 2018-02-13T18:18:21.463Z Reads: 128

```
[quote="squishy654, post:111, topic:38869, full:true"]
Seems the price tag of a pile of burned out mosfets costs a lot more than one sound functional relay made to handle the power…
[/quote]

I'd be super nervous that the sidewalk ka-dunk ka-dunk ka-dunk ka-dunk would vibrate loose the mechanical relay contacts causing arcs and heat and failures and ESC reboots
```

---
## \#115 Posted by: squishy654 Posted at: 2018-02-13T18:22:26.079Z Reads: 130

```
That's why I ride Avenue trucks on my electrics, lol...helps keep them in one piece and my feet feeling good..
```

---
## \#116 Posted by: PXSS Posted at: 2018-02-14T00:38:52.289Z Reads: 122

```
https://www.digikey.com/product-detail/en/crydom-co/D06D60/CC1521-ND/353616
Here, solved
```

---
## \#117 Posted by: Kug3lis Posted at: 2018-02-14T01:32:17.728Z Reads: 122

```
These needs like real massive heatsinks for full load :D
```

---
## \#118 Posted by: PXSS Posted at: 2018-02-14T01:59:57.431Z Reads: 125

```
No they dont. If you run full load, even at 8P, your battery heats up faster than the switch. (I have 2 and one $150 heatsink on a shelf somewhere). 

Anyone who runs 100A+ for longer than 5 minutes needs to rethink something
```

---
## \#119 Posted by: squishy654 Posted at: 2018-02-14T02:37:14.183Z Reads: 121

```
If they do, who cares..sounds like an excuse for some functional bling! I like the idea..now find a tiny regulator to trigger it and put it on a board..come on inventors, nessissity is your mother!
```

---
## \#120 Posted by: PXSS Posted at: 2018-02-14T03:04:11.750Z Reads: 119

```
Voltage divider to gate with a switch on the high side so that the gate is pulled low when off.

Use a switch for the switch!!!!
```

---
