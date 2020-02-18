# 12S battery configuration question

### Replies: 36 Views: 8015

## \#1 Posted by: LucidLunacy Posted at: 2016-05-10T19:50:53.745Z Reads: 436

```
1st off, can someone confirm the number of LiPo's below are actually accurate to give me the end result I came up with?

2nd, which setup would make more sense to buy?  

<img src="/uploads/db1493/original/2X/e/e8928690e357fd5a37492543f616c4b7a52e3600.png" width="598" height="500">
```

---
## \#2 Posted by: scrant Posted at: 2016-05-10T19:56:14.534Z Reads: 406

```
It's been a long day, but I believe you would need to multiply those numbers instead of add to get your desired results.
```

---
## \#3 Posted by: sl33py Posted at: 2016-05-10T19:57:27.118Z Reads: 400

```
In series you increase the voltage, but keep the same mAh rating - so each of your above x 4 and x3 would be 2200mAh and 3000mAh respectively.

In parallel you would keep the voltage 3/4s, but increase the mAh.

That make sense?  I would go with larger mAh packs 3/4s x #needed to get 12s and still have a decent mAh for range.

HTH - GL!
```

---
## \#4 Posted by: hexakopter Posted at: 2016-05-10T19:59:24.906Z Reads: 386

```
To point one:

Your calculations are not right. 
**Setup 1:** You will get 8 2200mAh batteries for dollar 109,84, but it is not possible to do 12S4p. For 12s4p you need 16 of these. 4 in series are needed to get 12s, but then they only have 2200mAh. With 8 batteries you can only build 12s2p, so 12s and 4400mAh.

**Setup 2:** Same failure. You will need 9 batteries to get 9000mAh with 12s. Six are just for 12s2p, so 12s and 6000mAh.
```

---
## \#5 Posted by: treenutter Posted at: 2016-05-10T20:08:06.513Z Reads: 356

```
Good question @LucidLunacy. @sl33py and @hexakopter have it right... you can either increase the voltage (the "S"), or the capacity (the mAh), but not both when you combine packs. You can still achieve what you're after, but you'll need different battery packs to get there.
```

---
## \#6 Posted by: sl33py Posted at: 2016-05-10T20:16:09.489Z Reads: 339

```
In general i would suggest something around 5000mAh (aka 5Ah).  if 3s packs x4 for 12s, or if 4s packs x3 for 12s.

I personally prefer the 3s packs for balance, and ability to run only 3 for 9s (great if you get a >200kv motor later or on another board and want to use these packs).  Plus 3s packs can usually be a bit smaller - i like thinner packs for better clearance.

So a setup of 4 x 3s packs 5000mAh would be a great start, and unless you need crazy range should give you a decent run time/range.  

GL!
```

---
## \#7 Posted by: sl33py Posted at: 2016-05-10T20:25:33.407Z Reads: 308

```
a favorite of mine for being super thin and light:
https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=11931

4500mAh (so a bit lower capacity), but only 21mm thick and 350g.  x 4 and about your 100'ish $.  

Even better for range would be the:
https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=9184 

23mm thick, 350g and 5000mAh.  again around $100'ish.

GL!
```

---
## \#8 Posted by: outsider Posted at: 2016-05-10T20:50:45.192Z Reads: 270

```
What kind of range would you get with 4x 3s packs at 5000mah? Thanks :)
```

---
## \#9 Posted by: Jinra Posted at: 2016-05-10T20:57:04.503Z Reads: 261

```
Approximately 22km based on conditions and setup. General rule of thumb is 10wh = 1km. This setup nets you 222wh (44.4v * 5 amps = 222wh).
```

---
## \#10 Posted by: LucidLunacy Posted at: 2016-05-10T21:05:53.118Z Reads: 253

```
[quote="sl33py, post:6, topic:3088"]
I personally prefer the 3s packs for balance, and ability to run only 3 for 9s (great if you get a &gt;200kv motor later or on another board and want to use these packs).  Plus 3s packs can usually be a bit smaller - i like thinner packs for better clearance.
[/quote]

Exactly why Im wanting to buy 3-4s packs.  

Thanks for the links.
```

---
## \#11 Posted by: outsider Posted at: 2016-05-10T21:32:09.977Z Reads: 237

```
How does that scale with 1 vs 2 motors? Thanks for the help! I thought if you put them in series, the capacity stays at 5000mah in total? Sorry still learning about batteries.
```

---
## \#12 Posted by: Jinra Posted at: 2016-05-10T21:36:20.597Z Reads: 241

```
You'll probably get slightly more mileage out of a single motor, but it heavily depends on your weight, amount and incline of hills, if there's heavy wind, etc. 1 or 2 motors shouldn't affect it too drastically (maybe 3~ km in this example). Take a look at the boosted dual+ with 7 mile range (2 motors) vs the single with 8 miles (1 motor).

And yes, series = increasingly voltage. Parallel = increasing capacity
```

---
## \#13 Posted by: outsider Posted at: 2016-05-10T22:02:54.139Z Reads: 236

```
I just have 2 more questions (hope that's alright)

* How much does the discharge rate matter? I see 1 pack with 20c and one with 30c.
* The same 2 packs, 1 is 4S and 1 is 3S1P - what will this effect in terms of building?

The 2 batteries 
http://www.hobbyking.com/hobbyking/store/__8587__ZIPPY_Flightmax_5000mAh_3S1P_30C.html
http://www.hobbyking.com/hobbyking/store/__9516__Turnigy_5000mAh_4S_30C_Lipo_Pack.html

Really appreciate the help!
```

---
## \#14 Posted by: lox897 Posted at: 2016-05-10T22:08:34.066Z Reads: 213

```
Get at least 20c continuous. It means that you times the mah of the pack by the discharge rate of the pack to get the continuous discharge.
```

---
## \#15 Posted by: Jinra Posted at: 2016-05-10T22:16:46.284Z Reads: 214

```
Depends on the current draw of the ESC to the motor. If you're going up hills, your ESC is going to be drawing a lot of current. I think 60A is the default Max current from the VESC. The 'C' rate is the battery's discharge potential, where 1C = complete discharge of the battery in 1 hour (2C would be complete discharge in .5 hours). To calculate the discharge rate in amp hours, multiply the C rate by the capacity of the battery (eg. 20C battery 2 5000mah = 100A discharge rate).
```

---
## \#16 Posted by: outsider Posted at: 2016-05-10T22:57:43.911Z Reads: 214

```
@Jinra and @lox897 Thanks for the help

Is there an easy way to charge all lipo's at once by plugging in 1 cable into a charger? Much like a consumer grade board.

And voltage meters can be used to find out battery capacity remaining?
```

---
## \#17 Posted by: sl33py Posted at: 2016-05-10T23:09:32.875Z Reads: 228

```
be cautious about "20c" is key statements - it's really C * Capacity of batteries - i would shoot for 100A discharge (normal not peak) to ensure you have overhead and don't damage your batteries.

While lipos aren't super expensive they aren't cheap either.  You shorten the life of the battery with heavy draw/demand.  So utilizing less of the discharge capability will give you longer battery life.  That's why i shoot for a minimum of 100A continuous (not peak) discharge batteries (5000mAh * 20C = 100A).  More is better but spending on 65C batteries is just throwing away money...  IMO.

Similarly charging is a big part of pack life.  Lower charging will get you more re-charge cycles (life), and not charging all the way to 4.2v will also help increase cycles/life.  That said - i want maximum range, and usually still charge to 4.2, but do try to slow charge when i can afford the time.

Charging multiple's @outsider - get a paraboard.  There are cheap knockoffs, but the original paraboard is what you are looking for solution-wise.  It allows you to connect 4-6 batteries (depending on which board and total amps combined charging) at the same time *and* balance charging them.
[img]/uploads/db1493/original/2X/0/0b53050b8623182c0a1bc26b634d06d1b5973bac.jpg[/img]
http://www.buddyrc.com/power-system/paraboard-parallel-charge-board/paraboard-v3.html

Just pick the connectors you need, or bare wire to solder your own (wish they would get xt90's!).  It's also helpful to get some balance lead extensions to make it easier to plug in 4 batteries at once.

If you get a decent charger (i like iCharger but $$ - iMax B6AC v2 is my budget recommended), it can show you mAh charged and some other battery testing (like Internal Resistance - great info to see if pack is spent/shot/deadjim).

HTH - GL!
```

---
## \#18 Posted by: sl33py Posted at: 2016-05-10T23:13:36.576Z Reads: 213

```
"consumer grade board" - you are asking about BMS.  A single barrel plug and done like on your laptop.

A Battery Management System allows you to charge and discharge all the batteries to max and min safely.  It likely (verify depending which you get) has a low voltage cuttoff, and will definitely have a balance/charge limit as well.  Complexity wise i've avoided, but do like the idea for simplicity.

There are a TON of them out there and i don't know enough to educate anyone, but hopefully someone will chime in or it can help you refine your search to good or suggested BMS's.

GL!
```

---
## \#19 Posted by: Jinra Posted at: 2016-05-10T23:15:21.783Z Reads: 219

```
hey sl33py, slightly off topic question. How come some lipos like [this one](http://www.hobbyking.com/hobbyking/store/__8932__Turnigy_2200mAh_3S_20C_Lipo_Pack.html) have a 3s configuration but have 4 balance leads? When I was looking up some BMS's they showed configurations for 1 lead per positive terminal in a series ([example](http://i1098.photobucket.com/albums/g378/lilianleung/12Slogo.jpg~original))
```

---
## \#20 Posted by: sl33py Posted at: 2016-05-10T23:27:26.923Z Reads: 215

```
every battery will have one more wire than number of cells on the balance plug.  3s - 4 wires, 4s - 5 wires, etc.

(EDIT - it's one power and the 3 grounds on a 3s)...  let me go double check.  I know they are in series, so you will see 4.2, 8.4, 12.6, etc.

uno momento

I had it backwards - one power wire, plus one ground x each cell.

here's a good overview:
https://www.youtube.com/watch?v=BtKhZ3NeEpE
```

---
## \#21 Posted by: Jinra Posted at: 2016-05-10T23:30:25.825Z Reads: 200

```
So if I were to make my own battery like the example pic shown, I wouldn't solder on that extra lead?
```

---
## \#22 Posted by: NNGG Posted at: 2016-05-11T00:12:03.979Z Reads: 191

```
Buy 3 4S zippy 5000mah lipos. $30 each.
```

---
## \#23 Posted by: Hummie Posted at: 2016-05-11T17:55:32.366Z Reads: 181

```
Bulk charging with power supply.  Meanwell or other brands. Doesn't monitor each cell and u have to do that on the side. I like this method way more than typical chargers
```

---
## \#24 Posted by: LucidLunacy Posted at: 2016-05-12T19:54:05.299Z Reads: 170

```
Can some one confirm the following:

You can combine any # of LiPo packs with different cell counts as long as the mAh and "C" rating is the same

ex-2s 5000mAh 20C in series with 3s 5000mAh 20C = 5s 5000mAh 20C
_______________________________________________________________________________________________

You can combine any # of LiPo packs with different capacity as long as cell count and "C" rating is the same

ex- 2s 4000mAh 20C in parallel with 2s 5000mAh 20C = 2s 9000mAh 20C

_______________________________________________________________________________________________
```

---
## \#25 Posted by: sl33py Posted at: 2016-05-13T15:20:19.967Z Reads: 166

```
@LucidLunacy - correct.  In Series, you are simply increasing voltage (2s - 7.4-8.4v (nominal to fully charged) + 3s - 11.1- 12.6v) so you will have 5s (19-21v).

Pairing brands might be wise and a battery monitor on each would be good to watch for the first cell reaching your cutoff/low-voltage.  So you don't overdraw and damage.

GL!
```

---
## \#26 Posted by: LucidLunacy Posted at: 2016-05-13T15:44:06.329Z Reads: 156

```
Right on man, Thanks for confirming!
```

---
## \#27 Posted by: Hummie Posted at: 2016-05-13T18:58:25.659Z Reads: 168

```
I'm using (9) 90c cells in series with (3) 35c. I'm watching the voltages and they stay balanced enough to keep everything within 4.2 and 3.6 and no not get warm or puffy.  Why don't I want to do this?
```

---
## \#28 Posted by: rodriguejoe1 Posted at: 2016-09-04T20:23:52.783Z Reads: 150

```
Long question. I am having a full blown BRAIN FART deciding what battery configuration to order for this..
www.trampaboards.com/emtb-holypro-deck-with-vertigo-trucks-8-inch-superstar-wheels-ratchet-bindings-twin-motor-mount--motor--529e-p-12669.html
I want a 12S 10A configuration on dual ollin boards. So is it better to run (2) 6s1p like these www.hobbyking.com/hobbyking/store/__8590__ZIPPY_Flightmax_5000mAh_6S1P_30C.html then put them in series with this series connector www.hobbyking.com/hobbyking/store/__10264__XT60_Harness_for_2_Packs_in_Series_1pc_.html?strSearch=xt60 series then to ONE vesc and repeat for the other side? That would give me 12S2p 10A
or ...(4) 3S like these http://www.hobbyking.com/hobbyking/store/__14057__ZIPPY_Flightmax_2800mAh_3S1P_30C.html
using the the xt60 harness x2 then a parallel connector like this one http://www.hobbyking.com/hobbyking/store/__64402__XT60_Harness_for_2_Packs_in_Parallel_1pc_AR_Warehouse_.html?strSearch=parallel to get 12S 10.A plus?
```

---
## \#29 Posted by: Hummie Posted at: 2016-09-05T00:35:59.395Z Reads: 136

```
Don't understand u with he 10a 

.im not sure I understand al, ur asking but I like the serial connection method give the host two options. 

 U can put ur batteries in series or parallel either way no problem ans determines the voltage.  Everyone puts their escs in parallel and I think it's the only way.  Seperate batteries for each esc is doable 

Esc is series?
```

---
## \#30 Posted by: rodriguejoe1 Posted at: 2016-09-05T00:39:44.122Z Reads: 129

```
I MEANT 10,000 mAh  for distance.. sorry..
```

---
## \#31 Posted by: Hummie Posted at: 2016-09-05T00:43:13.100Z Reads: 131

```
I'm not sure what ur asking but if the motors are on either side there will either be long battery or motor wires.  The esc will be better with the long motor wires.   I'd do a series connection for the batteries to the two paralleled escs and one with reall long wires.
```

---
## \#32 Posted by: rodriguejoe1 Posted at: 2016-09-05T02:20:38.546Z Reads: 135

```
so let me see if this is clearer...battery pack 1
6S1P
         +SERIES CONNECTOR EQUALS 12S1P THEN A PARALLEL CONNECTOR EQUALS 12S2P TO VESC #1
6S1P
_____________________________________________________________________________________________
battery pack 2

6S1P
        +SERIES CONNECTOR EQUALS 12S1P THEN A PARALLEL CONNECTOR EQUALS 12S2P TO VESC #2 
6S1P
```

---
## \#33 Posted by: Hummie Posted at: 2016-09-05T03:32:08.398Z Reads: 135

```
A picture would do it all.  Easiest is just make ur 12s battery, all in series, and have ur two escs coming off in a parallel circuit.   And I have an xt90s plug at the beginning of the escs. 
<img src="/uploads/db1493/original/2X/4/4ffe692801975c9f2b5c19e0731afedc59c61669.jpeg" width="375" height="500">

Words are confusing. 

This is charging but then I plug it into the plug coming out of the two paralleled escs to go
```

---
## \#34 Posted by: Mobutusan Posted at: 2016-09-05T06:47:58.065Z Reads: 126

```
@Hummie What type of charger are you using that can charge the 12s in series?
```

---
## \#35 Posted by: Hummie Posted at: 2016-09-05T13:39:43.790Z Reads: 121

```
A Meanwell 48 volt adjustable power supply with a wattmeter I soldered on.   Not the easiest out of the box or in use but will do 400 watts to 50.4 or more.  You can get easier to use bulk chargers with more features if you look for ebike chargers but mine can put out a lot. 


I balance charge with little 6s balancers for 10$ on the side.
```

---
## \#36 Posted by: rodriguejoe1 Posted at: 2016-09-05T16:05:34.166Z Reads: 115

```
Thank you.. That answers my question..
```

---
