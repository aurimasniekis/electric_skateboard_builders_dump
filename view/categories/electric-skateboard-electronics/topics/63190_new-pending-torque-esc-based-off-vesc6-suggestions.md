# NEW PENDING TORQUE ESC based off VESC6 - Suggestions

### Replies: 42 Views: 1103

## \#1 Posted by: torqueboards Posted at: 2018-07-29T00:22:19.666Z Reads: 331

```
Have a new ESC that's based off of VESC6 with a few protection modules added so it comes in a bit too big IMO.

It's about 82mm wide, 70mm length, 25mm height. For a DUAL it would be 164mm or 6.45" inches wide.

I can follow through with the current size and start testing although I personally think it's too wide for a single ESC. I'd rather not follow through with it if the width of the ESC is way too long for others as well.

There's two options.
OPTION 1 - Re-do the PCB and change the size and make it longer vs wider.
OPTION 2 - Since we're redoing the PCB may think about splitting it up and having a 2 layer board to possibly get more space/room but overall should be smaller can probably increase power output as well.

The question for everyone...

**What's the maximum width you'd want for an ESC for your build/setup? Ref to a single esc.**

**What added features would you like to see in an ESC?**
```

---
## \#2 Posted by: chris.hunt Posted at: 2018-07-29T00:27:20.183Z Reads: 320

```
[quote="torqueboards, post:1, topic:63190"]
What’s the maximum width you’d want for an ESC for your build/setup? Ref to a single esc.
[/quote]

I think the FOCBOX is perfect possibly a little smaller

[quote="torqueboards, post:1, topic:63190"]
What added features would you like to see in an ESC?
[/quote]

not sure if this exist or not but the ability to control led's from the ESC for example how a motherboard on a computer has a rgb header to control the lights maybe we can make one that will control a front headlight, and a break/reverse light as well as a side light
```

---
## \#3 Posted by: torqueboards Posted at: 2018-07-29T00:34:23.755Z Reads: 291

```
Also switching the board to a 2 layer..  will add more time to R&D and need another round of testing.

But the benefit would be logic and power would be different so we could have a higher spec power board for those running more power.

Current PCB is 60x80 but with the enclosure it's about 70x82.
```

---
## \#4 Posted by: akhlut Posted at: 2018-07-29T00:34:51.658Z Reads: 276

```
Two 2 layer boards.  HV/LV simplifies routing and PCB's can be 2 layer instead of 4.  Double stack should get a v6 down to about the size of a v4, maybe slightly wider.  DRV exposed for replacement.  Also, not hard soldered but a daughter board ala RAMPS1.4.  Port headers facing down so they don't melt when replacing drv (which should be top of stack for easy replacement).

Modular replacement should be easier to hotswap as well as troubleshoot.

+1 for 2oz HV and 1oz LV
```

---
## \#5 Posted by: pat.speed Posted at: 2018-07-29T00:35:29.482Z Reads: 256

```
160mm doesn’t sound too bad, I run lipos on both my boards so my cases have to be that wide to accommodate the lipos anyway. But I guess the majority run Li-ion which is only about 130-140mm
```

---
## \#6 Posted by: torqueboards Posted at: 2018-07-29T00:36:23.754Z Reads: 256

```
[quote="pat.speed, post:5, topic:63190"]
160mm doesn’t sound too bad
[/quote]

Yeah, sounds bad too that's why I posted it lol. Batteries are only about 140-150mm wide.

I sorta want them the same size but just checking what other people think about it.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-07-29T00:38:23.061Z Reads: 247

```
Would it be possible to just make it one dual esc? that would surely save some space
```

---
## \#8 Posted by: torqueboards Posted at: 2018-07-29T00:41:10.541Z Reads: 247

```
[quote="pat.speed, post:7, topic:63190"]
Would it be possible to just make it one dual esc?
[/quote]

I could but then running a single motor setup would be more costly.
Enertion is doing that anyways.
I think the benefit is having more options vs less options.
For now, I don't see a need for a specific dual esc. Makes sense for Enertion since they only sell dual motor setups.
```

---
## \#9 Posted by: torqueboards Posted at: 2018-07-29T00:54:32.672Z Reads: 244

```
[quote="chris.hunt, post:2, topic:63190"]
not sure if this exist or not but the ability to control led’s from the ESC for example how a motherboard on a computer has a rgb header to control the lights maybe we can make one that will control a front headlight, and a break/reverse light as well as a side light
[/quote]

Probably looking into that a bit later that way it can be tied to a remote or something.
```

---
## \#10 Posted by: pat.speed Posted at: 2018-07-29T01:02:10.887Z Reads: 238

```
You could have both could you not? This one that you have designed now for single motor as it won’t matter since there will only be one and then make a dual motor one
```

---
## \#11 Posted by: torqueboards Posted at: 2018-07-29T01:03:26.636Z Reads: 238

```
[quote="pat.speed, post:10, topic:63190"]
You could have both could you not?
[/quote]

You could but then if you wanted to go from a single motor to dual motor setup. You would need to buy an entirely new ESC. I'll look into a dual setup and see how much more cost effective it would be but last I remember I don't think there was a huge benefit.
```

---
## \#12 Posted by: briman05 Posted at: 2018-07-29T01:30:26.457Z Reads: 216

```
I would want to see being able to run in foc reliably
```

---
## \#13 Posted by: torqueboards Posted at: 2018-07-29T01:34:21.687Z Reads: 215

```
[quote="briman05, post:12, topic:63190, full:true"]
I would want to see being able to run in foc reliably
[/quote]

Yeah, I want FOC reliable also. We'll continuously upgrade it to make it more reliable. Would be great to buy it once and not ever need another one. I actually have a few engineers working on it so any damaged ones we'll take them back for more testing.
```

---
## \#14 Posted by: briman05 Posted at: 2018-07-29T01:39:56.617Z Reads: 210

```
Also maybe a integrated switch.
```

---
## \#15 Posted by: mmaner Posted at: 2018-07-29T03:25:43.412Z Reads: 200

```
As long as it's no more than 70mm wide, can handle 80a, reliable FOC and has an available 5v port it's perfect.
```

---
## \#16 Posted by: onepunchboard Posted at: 2018-07-29T03:38:25.811Z Reads: 198

```
I don't care about more amp as my current set up never pass 40A. (12s battery woohoo)BUT Small print def be more useful. Included switch and Bluetooth would nice feature. I really like changing setting on the fly these days

Also USB port need to be face up not side it's hard to get to sometimes
```

---
## \#17 Posted by: lock Posted at: 2018-07-29T03:46:58.798Z Reads: 200

```
VESC Firmware v3.39 added support for an AUX pin; currently only seems to be supported in the 'super' VESC Vedder is working on. Would be nice to have this on other VESCs too for lights/etc.
```

---
## \#18 Posted by: chuttney1 Posted at: 2018-07-29T03:50:12.957Z Reads: 203

```
I hope you've taken note of past forum posts not including this one. You need to add diodes in series with the 5v and 3V3 rails for external connectors. Simple but allows connections to other 5V or 3V3 powered devices, battery or not. You can look at old MacBook schematics on this as it's easily seen. Called ORing diodes.
```

---
## \#19 Posted by: dareno Posted at: 2018-07-29T09:25:56.284Z Reads: 212

```
You just continue to find new ways of parting me with money lol 
  There are far more educated people on here that can help with the technical bits but coming from a rc background all I really want is a product that doesn't pop at the first sign of trouble.  Over engineer the thing please.  If it makes the form factor larger then so be it but make it reliable whatever that takes and we can accommodate it and allow for the size in the easy bit of the build.  
Good v4's work in most of the configurations people employ but when you want to push the boundaries then you need a v6 and right now they are either crazy money or untested.  
Features I would like to see

An integral switch 
  
A remote programming port    -   the ability to mount a socket on the outside of the enclosure 

A low voltage port/ports to accommodate accessories; lights cooling fan etc

Also a data sheet on purchase.  It shocks me how many manufacturers sell a product without any paperwork at all. Take it to the next level and provide some basic settings info for the most popular configurations especially for the products that you sell.  

Decent back up   -   If a problem is flagged within the community then act on it and fix the issue, don't continue to sell it to new users who are unaware.

Provide a repair service for the product that we can utilise when we've been stupid.

Great news though and stop messing around on here and get on with building this thing :stuck_out_tongue_winking_eye:
```

---
## \#20 Posted by: DAddYE Posted at: 2018-07-29T13:53:54.751Z Reads: 194

```
I would like 13mm to 15mm tops wide. 
I’d like a budget dual vesc; isn’t possible to save some space/money having a single pic handeling them both? 
An integrated Bluetooth would be too much to ask? :slight_smile:
```

---
## \#21 Posted by: Andy87 Posted at: 2018-07-29T14:25:47.789Z Reads: 174

```
80a const. current
Safe FOC 
5V power output (for lights etc)
Plug for powerswitch
Integrated Bluetooth (for iOS and Android)
2.4 ghz Receiver which can be paired with gt2b remote
Dual setup via Bluetooth module instead of CAN
Different options for heatsink (single, dual housing)
Would be a dream...no lose connections anymore, no extra cables and modules flying around...and FOC😍
```

---
## \#22 Posted by: mikenyc Posted at: 2018-07-29T14:34:59.853Z Reads: 174

```
[quote="torqueboards, post:8, topic:63190"]
For now, I don’t see a need for a specific dual esc. Makes sense for Enertion since they only sell dual motor setups.
[/quote]

hmm. maybe send out a poll or something to your mailing list to see if more people are interested in running dual set up vs. single. huge benefits with everything in a single unit.
```

---
## \#23 Posted by: mmaner Posted at: 2018-07-29T14:53:49.691Z Reads: 168

```
I don't understand the desire for a dual esc in the current market. The reason you combine systems is to save power, space and/or money. 

Currently it won't be significantly smaller, it will use the same voltage and won't be any cheaper. 

The risk is you replace the entire system instead if half (said half the money) when it breaks. 

I wish someone would explain to me why duals are attractive.
```

---
## \#24 Posted by: Mikenopolis Posted at: 2018-07-29T15:41:29.361Z Reads: 171

```
The only single unit dual esc I’m attracted to is the Unity. Is there a need? Obviously not since we’ve been running separate vescs all this time. The things I like about it is:

1.) One XT60 connector
2.) Single programming
3.) Integrated switch plug

None of these are needed but it’s nice to have if it’s dependable (that’s a big IF) the space saving is welcomed. 

I guess what I’m saying is that I’m too lazy to manage my mess of cables or make a smaller XT splitter and the unity is my way out of 10 minutes of work 🤷‍♂️
```

---
## \#25 Posted by: akhlut Posted at: 2018-07-29T15:48:22.760Z Reads: 169

```
Less complexity, simpler is better.

Strip features away, don't add extras - no integrated switch, no bluetooth, no nothing.  Stick with core functionality and remove everything else.
```

---
## \#26 Posted by: Silverline Posted at: 2018-07-29T15:51:31.175Z Reads: 169

```
I like my dual heatsink for both my Escapes and focboxes... They sit nicely in the enclosure, with greate cooling, looks dual, but i can still switch one if necessary
```

---
## \#27 Posted by: Acido Posted at: 2018-07-29T16:34:58.222Z Reads: 167

```
If you would put a e switch inside that wouldnt fail that would be a dealbreaker, and possibly some mini bluetooth solution with an app developed from you or someone to make it look fancy
```

---
## \#28 Posted by: torqueboards Posted at: 2018-07-30T04:29:12.286Z Reads: 155

```
Cool.. Thanks for everyone's feedback.

I've decided on splitting it up into 2 layer stack since we're re-doing the PCB anyways to make it smaller. Overall easier and can replace boards easier down the road.

Will take a few extra weeks to finish the PCBs but better off in the long run. Still needs another round of testing and then a beta test batch.

Hopefully, that will bring it down to 60x60 and under 25mm height.

For now, we're sticking to a single ESC but we'll look into a dual option with more customized programming in the future.
```

---
## \#29 Posted by: Pedrodemio Posted at: 2018-07-30T09:37:24.704Z Reads: 140

```
What about making all the connections to the side? CAN bus, PPM etc

25mm is a bit tall but ok, but 25mm plus connectors on top can easily become 30mm or more
```

---
## \#30 Posted by: Acido Posted at: 2018-07-30T12:59:32.604Z Reads: 135

```
There are L shaped jst connectors available to buy i think
```

---
## \#31 Posted by: torqueboards Posted at: 2018-07-30T14:52:37.698Z Reads: 127

```
@Pedrodemio Yeah, I plan on putting the connectors on the side.
```

---
## \#32 Posted by: deucesdown Posted at: 2018-07-30T19:17:25.888Z Reads: 123

```
More protection for stupid failures like canbus, hall sensors.

Maybe a way to attach resistive load for regen braking when pack is full?

XH connector for halls? I find the PH is so delicate...

Built in bluetooth?
```

---
## \#33 Posted by: akhlut Posted at: 2018-07-30T19:55:05.346Z Reads: 123

```
+1 for CANBUS upgrade.

TJA1052i would be nice, but would need external circuitry for isolated power.
```

---
## \#34 Posted by: torqueboards Posted at: 2018-07-30T22:00:21.353Z Reads: 119

```
Since we're doing a single ESC. External bluetooth will probably be better will keep a lower price for the ESC in general.

Will probably be switching to lock connectors so nothing falls out.
```

---
## \#35 Posted by: akhlut Posted at: 2018-07-30T22:15:32.976Z Reads: 116

```
What kind of connectors?  Part #?
```

---
## \#36 Posted by: torqueboards Posted at: 2018-07-30T23:49:59.627Z Reads: 110

```
Haven't decided yet but should be similar to the current.
```

---
## \#37 Posted by: Mobutusan Posted at: 2018-07-31T02:51:49.417Z Reads: 101

```
How about an optional external heat sink that attaches to the ESC case and can be easily installed and sealed to an enclosure for external cooling?
```

---
## \#38 Posted by: torqueboards Posted at: 2018-07-31T03:23:00.273Z Reads: 102

```
@Mobutusan - Yeah, was thinking about it. It would be best. I'll see what I can do.
```

---
## \#39 Posted by: lrdesigns Posted at: 2018-07-31T04:18:58.438Z Reads: 100

```
[quote="Mobutusan, post:37, topic:63190, full:true"]
How about an optional external heat sink that attaches to the ESC case and can be easily installed and sealed to an enclosure for external cooling?
[/quote]

For dual setups. Like the ones for focbox or ESCape that are on the forum now.
```

---
## \#40 Posted by: torqueboards Posted at: 2018-07-31T04:26:03.313Z Reads: 101

```
I was thinking we should have a waterproof dual esc. Everything stored inside the dual ESC would need space for a bluetooth, receiver, wires from ESC1 to ESC 2.

The only thing harder to waterproof would be the end connectors especially if people are using it for custom DIY setups. But I'm sure, everyone could manage.

Entire Dual ESC block can just be bolted to the deck.
```

---
## \#41 Posted by: Andy87 Posted at: 2018-07-31T05:19:41.121Z Reads: 93

```
Waterproof housing with place for Bluetooth and receiver 😍
```

---
## \#42 Posted by: dareno Posted at: 2018-07-31T07:04:29.681Z Reads: 73

```
Now you're talking!
```

---
