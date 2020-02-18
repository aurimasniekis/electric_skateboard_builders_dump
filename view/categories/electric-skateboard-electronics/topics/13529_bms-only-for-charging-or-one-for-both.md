# BMS - Only for charging or one for both?

### Replies: 19 Views: 2332

## \#1 Posted by: fraannk Posted at: 2016-11-23T10:05:22.657Z Reads: 218

```
Hey guys. I'm not sure whether or not to choose a BMS for charging or one for charging AND discharging. Can you explain the advantages with using a BMS for discharging as well? I use a VESC, and they have low voltage cut-off, so I don't know what would be the best solution. :) I do not have much space available. :P
```

---
## \#2 Posted by: jujet Posted at: 2016-11-23T10:10:15.544Z Reads: 221

```
Here you go mate, have a read here

http://liionbms.com/php/wp_cccv_charging.php

http://liionbms.com/php/wp_lovtg_cutoff.php
```

---
## \#3 Posted by: IDVert3X Posted at: 2016-11-23T11:56:53.196Z Reads: 210

```
If you have a VESC, BMS for discharging is pointless. The only thing it would be good for is short circuit protection. But you can use fuse for this ( which is much cheaper and smaller than 80A BMS ).

BTW, some BMSs offer e-switch as well, so that may be the reason to buy one.
But it's generally cheaper to make an e-switch ( ~ 25 euros ), buy BMS for charging only ( ~ 10 euros ) and use fuse. It's smaller compared to 80A+ BMSs and size matters when you are doing split encloser design for flexy boards ( Vanguard for example ).
```

---
## \#4 Posted by: Jakeii Posted at: 2016-11-23T12:09:13.391Z Reads: 200

```
I relied on the VESC to protect my batteries, cutoff set at 33V I think. But after one long ride, it started to slow, and then stop, I thought yay, good vesc saving my batteries. But upon getting home almost all the cells were ruined.

The VESC can't see the individual cell voltages so it won't cut off if one cell goes below the point of no return but the total voltage seems alright. Possibly you could get away with using a lipo voltage alarm?
```

---
## \#5 Posted by: IDVert3X Posted at: 2016-11-23T12:17:21.506Z Reads: 188

```
[quote="Jakeii, post:4, topic:13529"]
it won't cut off if one cell goes below the point of no return but the total voltage seems alright.
[/quote]

Well, that happens when you use crappy packs ( like Multistar ) which usually have 1 or more weaker cells.
Never happened to me while using blue Turnigy batteries or quality Li-Ion cells.
Actually, I don't use BMS for li-ion at all in one of my projects, I just programmed high and low voltage cutoffs and it's still balanced after a year and ~ 400 cycles.

[quote="Jakeii, post:4, topic:13529"]
Possibly you could get away with using a lipo voltage alarm
[/quote]

Yup, that's what people flying aircraft use.
```

---
## \#6 Posted by: Jakeii Posted at: 2016-11-23T12:21:41.056Z Reads: 175

```
Well I used Turnigy packs so I'm not sure what went wrong then!

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/b/d/bdd4c2ba00afa241508429dcfc3702ec9d9ff0c8_1_666x500.jpg
```

---
## \#7 Posted by: IDVert3X Posted at: 2016-11-23T12:25:47.137Z Reads: 168

```
You said almost all the cells were ruined, so the total voltage has to be below the cutoff limit as well.
Doesn't sounds like a balancing issue. 
More like a failure of VESC cutoff ( never used this function personally ).

LiPo shouldn't be discharged below 3.3V under load.
Did you measured the total voltage of the pack after this happened?
```

---
## \#8 Posted by: Jakeii Posted at: 2016-11-23T12:45:40.145Z Reads: 166

```
Yea you could be right, and/or a faulty pack, it was 10S so shouldn't have kept going below 33V. I did check with a low voltage alarm, and alarms were blaring over the cells being anywhere from 3.3V to 1.7V, and my balance charger refused to charge them.
```

---
## \#9 Posted by: jujet Posted at: 2016-11-23T14:42:20.516Z Reads: 161

```
[quote="IDVert3X, post:3, topic:13529"]
If you have a VESC, BMS for discharging is pointless
[/quote]

No. You cannot protect individual cells with just the total voltage! 

You may feel comfortable using a Li Ion pack with a VESC with a low-voltage cut-off of let's say 25 V, a full 5 V above the 20 V minimum. But, in reality, you may be damaging the most discharged cells and not know it!

You MUST have a BMS to:

Stop charging if any individual cell is at the max voltage
Stop discharging if any individual cell is at the min voltage
Stop the battery current in case of overcurrent

Read links I posted above and decide for yourself if you'll use a BMS or not. I know some people don't use BMS and it works, in the end it's all about managing risk (I think)
```

---
## \#10 Posted by: fraannk Posted at: 2016-11-23T17:41:57.981Z Reads: 154

```
Thanks for the links. My current setup is 2x 5S Turnigy (blue) batteries, Vedder Switch and a VESC. Right now, I take my batteries out every time they need a charge. (I've always known when to charge them, based roughly on kilometers and feel) I'm looking for an easier way of charging, that's why I started looking into BMS's. 

So it seems like a BMS doesn't do much in the discharging department other than balancing. Since I already discharge without a BMS (and know the "dangers"), adding a "mini-BMS" for charging might be the easiest/cheapest/smallest route, am I right? Or did I miss something other than the things stated by you guys, and the info in the links? :)

Thanks for the help guys, I appreciate it a lot!
```

---
## \#11 Posted by: IDVert3X Posted at: 2016-11-23T17:47:01.264Z Reads: 148

```
You are right.
The main function of the BMS is proper balance charging.

But if you need to be 100% safe, over-discharge protection by moitoring individual cells can be archieved by much cheaper way. Just put in a $0.99 mini voltage alarm and when it starts to beep, you know you reached the critical level and shoudln't run it any longer. Just set it to 3.3V, so if any of the cells hits 3.3V, it starts to beep.

http://www.ebay.com/itm/NEW-RC-Lipo-Battery-Low-Voltage-Alarm-1S-8S-Buzzer-Indicator-Checker-Tester-LED-/172219837874?hash=item28191a2db2:g:NtwAAOSwfZhXNTzo
```

---
## \#12 Posted by: fraannk Posted at: 2016-11-23T17:48:38.599Z Reads: 147

```
Thank you. I might wait and see the results of @raphaelchang's epic BMS and ESC project. That seems pretty small and handles both charging and discharging. :) Thanks for the help!
```

---
## \#13 Posted by: IDVert3X Posted at: 2016-11-23T17:50:16.699Z Reads: 142

```
Yep, raphael's BMS and ESC projects looks really promissing.
Always good to have an alternatives.

VESC 6 also looks great!
```

---
## \#14 Posted by: longhairedboy Posted at: 2016-11-23T18:23:41.110Z Reads: 140

```
[quote="IDVert3X, post:3, topic:13529"]
If you have a VESC, BMS for discharging is pointless. The only thing it would be good for is short circuit protection. But you can use fuse for this ( which is much cheaper and smaller than 80A BMS ).
[/quote]

It is indeed not at all pointless. 

The VESC isn't going to shut your whole board down and completely cut power to the pack when LVC cuts in. Its not going to shut down the pack when one of the P groups goes too high or too low but the rest are fine. Its not going to protect the pack when there's a short in the VESC or anywhere else in the board. The VESC has those convenient features but they are absolutely no substitute for a proper BMS set up for charge and discharge.
```

---
## \#15 Posted by: IDVert3X Posted at: 2016-11-23T18:45:24.687Z Reads: 137

```
[quote="longhairedboy, post:14, topic:13529"]
The VESC isn't going to shut your whole board down and completely cut power to the pack when LVC cuts in
[/quote]

I though VESC will cut off itself when it hits LVC end limit. Noted.

[quote="longhairedboy, post:14, topic:13529"]
Its not going to shut down the pack when one of the P groups goes too high or too low
[/quote]

If one of the P groups gets **too** low ( which means battery is aging, can't keep the balance ) and others are just fine, it's time to replace it. Never a good thing to have weaker cell ( P group ) in your pack. Also, low voltage alarm can tell you this by beeping loudly and it's much cheaper.

[quote="longhairedboy, post:14, topic:13529"]
Its not going to protect the pack when there's a short in the VESC or anywhere else in the board
[/quote]

Fuses. Fuses. Fuses. There are only 2 types of people: those, who use them and those, who will.
No matter if you have BMS with short circuit protection, it may or may not fail, ALWAYS use fuses.

And after all, RC models with LiPo packs, which are much more prone to loose balance, don't use a BMS for discharging at all. Many people use those low voltage alarms and it's good enough.

But if you have a lot of free space in your encloser and don't mind spending more money, go for it.
```

---
## \#16 Posted by: IDVert3X Posted at: 2016-11-23T18:54:42.469Z Reads: 127

```
Let's talk about the benefits of having BMS **only for charge**:
- smaller
- cheaper
- less heat ( current don't have to go through the BMS, less losses )
- it's up to you when you want to shut off the board, you will **get warned**, but it won't just kick you off in the worst possible situation, you can safely stop and shut it down yourself.

Now, about the BMS **for discharging** as well:
- you don't have to switch off your board manually after a warning, it will shut down immediately
- you have short circuit protection ( in case you fuck it up, you don't have to change the fuse ).
```

---
## \#17 Posted by: overclocker_kris Posted at: 2016-11-24T20:55:26.675Z Reads: 120

```
just for charging.
```

---
## \#18 Posted by: Namasaki Posted at: 2016-11-25T07:24:00.459Z Reads: 115

```
@fraannk 
There is one point that has not been mentioned.
When your using a Vesc, you have regenerative braking so there is a possibility of over charging your batteries if your not using a BMS for Discharge because the charge current will go straight back into the batteries with no limitation.
Over discharging a pack can ruin it but over charging a pack can cause a fire.
A quality BMS that protects during discharge will prevent the batteries from overcharging by regenerative brakes because it monitors the min and max voltage limits continuously.
This may not be an issue if you live in the flat lands. For those who go up and down a lot of hills, it is.
I use a Bestech 80a bms. It was inexpensive compared to the rest of the electronics.
I ran my Li-ion pack down until the BMS shut off. Not one single cell was damaged.
The other day I was out riding with my 10s lipo/bms setup using five 2s Lipo packs in series.
The main positive wire on pack 5 broke loose and caused an intermittent connection.
My Bms shut down. 
When I got home and opened the enclosure I found that the wire was arcing.
A fire could have started from the arcing wire. if not for the bms. A fuse would not help in this situation.
```

---
## \#19 Posted by: rtasca Posted at: 2016-11-25T11:51:56.134Z Reads: 111

```
Can the versed PPL here link to a good + cheap charging only BMS up to 12s ?
```

---
