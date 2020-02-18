# Please review my first build &#124; Planning Phase &#124; Single Drive 12S VESC

### Replies: 10 Views: 1424

## \#1 Posted by: moistousness Posted at: 2016-08-04T01:01:09.060Z Reads: 136

```
Hey Everyone!

Been researching and looking to make a new board for the light commute! Wanting to make a single motor board with the option to add another motor later on. I'm a bit unsure on the compatibility of the electronics. If you see any problems, let me know.

<img src="/uploads/db1493/original/2X/9/9b4ea699b86b66c4e717202b4cc63d414ffc0a61.PNG" width="690" height="272">

https://docs.google.com/spreadsheets/d/1ed0rFbn3FAj8BUzO_tGEmVNpte9m-aaFfNFqn9SZGow/edit?usp=sharing
```

---
## \#2 Posted by: sl33py Posted at: 2016-08-04T01:16:32.951Z Reads: 127

```
looks like a solid list and build.  A couple suggestions and concerns.

if you want 12s you will want <200kv motor.  I know DIYes is getting a 190kv sensored motor option soon.  The R-Spec from enertion is another option, and there's always the SK3's from HK.

You should read up on the 60k ERPM limit to avoid damaging your VESC - might decide to go w/ a different motor setup and lower # series batteries?  I usually go 8-10s to be a bit more cautious and not push my VESC's.

Charger - that's for a SPACE cell - look at the iMax/SkyRC B6ACv2 if you want an inexpensive but good starting charger that doesn't need a AC to DC power supply.  Slower than an icharger or similar, but the non-clones are pretty nice!

Tx/Rx - i would go with the tried/true GT2b myself - $25, then print your own enclosure (badwolf, master cho, baby buffalo, etc.) or have one printed from 3dhubs for a few $ more.

BMS - i'd skip until you get going.  Use lipo or similar to start and upgrade later.

skip the battery meter as well.  Get a low voltage alarm instead to alarm/yell at you when voltage on any cell in the pack gets below 3.x volts (set in alarm where you want - i usually do 3.7 or 3.6v).
like this - http://www.hobbyking.com/hobbyking/store/__90762__Turnigy_Lipo_Battery_Voltage_Tester_2_8S_and_Low_Voltage_Buzzer_Alarm_AU_Warehouse_.html

Batteries - i personally like multiple thinner batteries w/ a harness to run in series vs a single big 6s/8s/12s battery.  cheaper, modular (if one has an issue) and lower profile under the deck.  so some 3s x 3 for 9s, or x4 for 12s.  i shoot for <30mm thickness on their "C" size on HK.

misc - i'd look at a loop key and pick a single type of battery connector.  I like XT90's, but just pick one as in the long run it'll help you a lot to simplify.

my .02 - HTH and GL!
```

---
## \#3 Posted by: moistousness Posted at: 2016-08-04T02:33:41.266Z Reads: 106

```
Thanks for the 2c.

Good advice. I might do a simpler battery set up and upgrade when I'm more knowledgeable. I've amended my build

What connectors and miscellaneous things would I need to put all the electronics together or missing?
```

---
## \#4 Posted by: torqueboards Posted at: 2016-08-04T02:42:40.720Z Reads: 103

```
Mid August  - 6355 170KV and 190KV motors will be in stock. Week of the 15th. Same time we have a huge stock of VESCs coming. We shouldn't ever be out of stock anymore :joy:
```

---
## \#5 Posted by: sl33py Posted at: 2016-08-04T05:41:17.581Z Reads: 93

```
[quote="moistousness, post:3, topic:7097"]
What connectors and miscellaneous things would I need to put all the electronics together or missing?
[/quote]


A good solder station if you don't have one is nice.  At least a good soldering iron w/ adjustable heat and swappable tips (you need hot and large tips for bigger wire).

Good silicone wire 12/10g or so.  Superworm and wet noodle i think are the easy ones to find on Amazon and not too $.

Heat shrink tube, and a standard connector - XT90's my preferred.  If you get some anti-spark xt90's they make great anti-spark loop keys!
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

Some small 22-24g silicone wire is also great for misc wiring - canbus between VESCs, Rx wires to VESC, small LCD power displays etc.  

And the regular skateboard stuffs - a good skate tool, some good bushings for your weight (i like the SHR venom/blood orange/ and similar).  Mounting hardware and risers or shock pads.  If not gripped already - some viscious griptape is great too - or similar coarse grip (preference).

A parallel charging board is great to have (still good to individually balance cells occasionally).  Buddy RC's paraboard is the best one i've found, but $$ - plenty of less $ on HK.
http://www.buddyrc.com/power-system/paraboard-parallel-charge-board.html

GL!
```

---
## \#6 Posted by: kortho Posted at: 2016-08-05T23:08:30.397Z Reads: 61

```
Why would you get a dual motor mechanical kit for a single motor setup?
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-05T23:29:21.755Z Reads: 57

```
> Wanting to make a single motor board with the option to add another motor later on.
```

---
## \#8 Posted by: mason Posted at: 2016-08-06T00:22:49.963Z Reads: 52

```
can I ask how you embedded the spreadsheet?

thanks lol
```

---
## \#9 Posted by: jrpwit Posted at: 2016-08-06T01:02:10.242Z Reads: 50

```
just paste a google drive spread sheet link
```

---
## \#10 Posted by: moistousness Posted at: 2016-08-06T01:03:06.984Z Reads: 49

```
what @jrpwit said
```

---
