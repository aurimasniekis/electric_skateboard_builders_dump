# Help My Supower BMS E-Switch Doesn&rsquo;t Work!

### Replies: 36 Views: 2734

## \#1 Posted by: NickTheDude Posted at: 2017-05-16T18:09:57.344Z Reads: 207

```
So I got a BMS for my lipos, but I'm not sure about a few things.

<img src="/uploads/db1493/original/3X/5/8/588c2c1e52dc8438c69494d09e7b3ca6439d20f2.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/2/c/2c422748d647fa10395cae426058f6a399921751.jpg" width="666" height="500">

The instructions are pretty straightforward, but I was wondering how I could tell which balance lead on the lipos corresponded to whichever pin on the balance connector. Right now I have 2 6S lipos wired in series.

<img src="/uploads/db1493/original/3X/6/5/65dd64c91fe81b67562cf6d69679ce8bd224f5dc.jpg" width="666" height="500">

Also, The charging port I got doesn't list which pin is negative or positive, their simply numbered 1, 2 and 3. So I'm not sure which ones I need to solder to.

<img src="/uploads/db1493/original/3X/9/6/96479ffee6e197b6936a8275caa1a7f0657f3380.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/9/b954c26346f067599ed5d662a6b9899a8e5e294d.jpg" width="666" height="500">

Any help is greatly appreciated. :grin:
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-05-16T18:54:34.285Z Reads: 198

```
I checked the voltages of each cell and I can see how they're ordered, does that mean the first cell (3.7V) would get wired to pin 1, and the last (44.4V) to pin 12? I assume I could just cut the ground off as well.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-16T19:01:05.827Z Reads: 198

```
Here is a diagram for 10s to Bestech bms. 
In principle, it's the same. 

<img src="/uploads/db1493/original/3X/1/1/114862db65428a120932667e3e27bc9b51a33674.PNG" width="664" height="500">
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-16T19:05:12.688Z Reads: 192

```
[quote="NickTheDude, post:2, topic:23220, full:true"]
I checked the voltages of each cell and I can see how they're ordered, does that mean the first cell (3.7V) would get wired to pin 1, and the last (44.4V) to pin 12? I assume I could just cut the ground off as well.
[/quote]

You are correct. 
You eliminate the ground wires on both plugs.
Lowest voltage to pin 1
Highest voltage to pin 12
```

---
## \#5 Posted by: NickTheDude Posted at: 2017-05-16T21:22:48.729Z Reads: 182

```
Alright, so I wired everything and now I'm even more confused...

<img src="/uploads/db1493/original/3X/e/4/e40e1179866a74c4e74b615ae66a2e9bc9397d7a.jpg" width="666" height="500">

The negative battery lead is going to B-, the positive battery lead is going to the VESC positive leads, P- is going to the VESC negative leads and all the balance wired are connected.

For some reason, the VESCs are constantly blinking blue and the switch doesn't seem to work. Occasionally, at seemingly random moments the VESCs will stop blinking and turn on. So far this has only happened with the switch in the ON position. Then if I use the switch while the VESCs are powered, they turn off as intended. However after that I cannot reliably turn them on again and they go back to blinking.

I checked the voltage and this is what I got.

B- and Battery+

<img src="/uploads/db1493/original/3X/0/8/0853c8863a4f8b707b822a75a1ec40cdcf49fe1b.jpg" width="666" height="500">

P- and Battery+

<img src="/uploads/db1493/original/3X/1/3/13a79a09d869dd5558cb6de340a0d1a8fbb02be8.jpg" width="666" height="500">

Then for some reason, when I plug in the receiver, the voltage from P- and Battery+ goes down and the VESCs stop blinking. Is this simply the idle voltage that the circuit has? Would lowering the VESC minimum input voltage fix the blinking?

<img src="/uploads/db1493/original/3X/1/d/1dce62b10e28d0ae1e3d8ed228a562c06869f2a9.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/d/6/d616dc3a48e8bd3038087e66604166f842358bc7.jpg" width="666" height="500">


I have no idea what's happening :cry:
```

---
## \#6 Posted by: jmasta Posted at: 2017-05-16T21:25:30.335Z Reads: 173

```
[quote="NickTheDude, post:1, topic:23220, full:true"]

<img src="/uploads/db1493/original/3X/5/8/588c2c1e52dc8438c69494d09e7b3ca6439d20f2.jpg" width="666" height="500">


[/quote]

Did you add that switch?  I have this same BMS and it does not have an e-switch functionality
```

---
## \#7 Posted by: NickTheDude Posted at: 2017-05-16T21:27:09.029Z Reads: 170

```
I asked them to include and e-switch when I ordered it and that's what they sent.
```

---
## \#8 Posted by: jrpwit Posted at: 2017-05-16T22:20:42.251Z Reads: 171

```
This is how I hucked mine up and works perfect. <img src="/uploads/db1493/original/3X/c/7/c7c7f438ab785da4a315fdf5a8b8e9fe95e5a7c9.png" width="500" height="500">

Also could u tell me if your switch works? I have the same brand but didn't ask for a switch. So far I have been using a spark connects but I would prefer a switch.
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-05-16T22:22:02.995Z Reads: 169

```
No, the switch randomly turns on and mostly doesn't work at all. Mine is wired in the same way except I haven't attached the charging port yet.
```

---
## \#10 Posted by: jrpwit Posted at: 2017-05-16T22:22:59.360Z Reads: 163

```
Bestech BMSs are hucked up slightly differently I believe
```

---
## \#11 Posted by: Jinra Posted at: 2017-05-16T22:24:40.352Z Reads: 162

```
You should probe each balance lead to make sure you get the expected voltage. I burned a couple BMS's because I failed to do this :'(
```

---
## \#12 Posted by: jrpwit Posted at: 2017-05-16T22:32:45.462Z Reads: 167

```
Also this is how lipos are assembled. Your balence leads could potentially not be wired correctly
<img src="/uploads/db1493/original/3X/9/0/9006c80b962599a6e111a6990a8062813d42397b.jpg" width="640" height="480">
```

---
## \#13 Posted by: NickTheDude Posted at: 2017-05-16T22:48:49.468Z Reads: 159

```
I just checked the balance wires again and they seem to be in the correct order. pin one is ~3.7 and it increases by ~3.7 each succeeding pin.
```

---
## \#14 Posted by: NickTheDude Posted at: 2017-05-17T15:00:18.384Z Reads: 156

```
So the switch functionality still isn't working... Does anyone actually have a Supower BMS with a working eswitch?

The voltage is staying around 2.8V which from what I've read seems to be fine. Presumably that means the BMS hasn't exploded yet. This leads me to believe that it could be the switch itself that's broken, unless anyone has any other ideas.

Also, I took apart the charger jack and found out which ports were positive and negative.

<img src="/uploads/db1493/original/3X/7/4/746937e21b7cba34ae3667def83a4094232e2a31.jpg" width="666" height="500">
```

---
## \#15 Posted by: jmasta Posted at: 2017-05-17T16:49:52.163Z Reads: 152

```
I've never seen that BMS with an e-switch. I have the same one, but use a separate anti-spark switch instead

PS. You could have figured out the pos/neg terminals on your charger, without taking it apart, by using your multimeter. A positive voltage reading between two pins means you have correctly identified the (+) and (-) pins. A negative voltage reading means they need to be flipped.  No connection, or "0L", means one of the pins is not used
```

---
## \#16 Posted by: NickTheDude Posted at: 2017-05-17T17:54:17.943Z Reads: 150

```
Ohhh good point I hadn't thought of that :stuck_out_tongue: But yeah if I can't figure out what's going on I'll probably end up using an anti-spark.
```

---
## \#17 Posted by: Fabian287 Posted at: 2017-05-17T18:26:53.980Z Reads: 149

```
i had a similar problem ... the problem was that the current to activate the discharge mosfets is to low.So i bridged the activation wire from the charge mosfets to the discharge for 3 sec. So you need 2 switches 1 normal and 1 to bridge the wire for some seconds to activate the mosfets.<img src="/uploads/db1493/original/3X/e/3/e35438f5b5060174b0d0236f0a680b1fa0480e46.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/4/1/41fc0210f18e8e89f3ad9060522cf826ad2fe562.jpg" width="666" height="499">
```

---
## \#18 Posted by: Fabian287 Posted at: 2017-05-17T18:38:44.627Z Reads: 136

```
Its a switch just like in a car to start the motor. but DONT let the switch all the time on.
```

---
## \#19 Posted by: NickTheDude Posted at: 2017-05-17T18:46:12.716Z Reads: 134

```
Hmmm, so would I still need to do that if I somehow bypassed the switch on the board and used an anti spark instead?
```

---
## \#20 Posted by: Okami Posted at: 2017-05-17T19:24:22.386Z Reads: 130

```
Cool discussion.. I would have initially suggested to connect the 2pins the 'smart switch' is connected to.. but @Fabian287 has even more knowledge.. and I didnt know the thing about mosfets he mentioned.. something totally new.
```

---
## \#21 Posted by: NickTheDude Posted at: 2017-05-17T19:29:28.241Z Reads: 122

```
[quote="Okami, post:20, topic:23220"]
I would have initially suggested to connect the 2pins the 'smart switch' is connected to..
[/quote]

Yeah, I tried that earlier today but it didn't work :frowning:
```

---
## \#22 Posted by: jmasta Posted at: 2017-05-17T19:29:30.561Z Reads: 122

```
Honestly, I would take whatever Supower says/claims with a grain of salt

For example, they say the BMS has "balancing function", but it can't actually balance my pack. It is still useful because it provides under- and over-voltage protection at the individual cell level. But the balancing is nonexistent. And I would not trust their "e-switch"

/$0.02
```

---
## \#23 Posted by: NickTheDude Posted at: 2017-05-17T19:31:43.615Z Reads: 121

```
[quote="jmasta, post:22, topic:23220"]
they say the BMS has "balancing function", but it can't actually balance my pack.
[/quote]

Whaaaat really? I bought it for that reason... I might just order one from Bestech and call it a day.
```

---
## \#24 Posted by: Okami Posted at: 2017-05-17T19:41:44.143Z Reads: 117

```
I will let @jmasta answer to that.. but i heard some powersupplies cut off power, when the balancing should start, since the balancing action happens at the very end of the charge.
```

---
## \#25 Posted by: Okami Posted at: 2017-05-17T19:44:01.612Z Reads: 121

```
[quote="Fabian287, post:17, topic:23220"]
bridged the activation wire from the charge mosfets to the discharge for 3 sec. So you need 2 switches 1 normal and 1 to bridge the wire for some seconds to activate the mosfets.
[/quote]

@NickTheDude I would then follow his advice and try what he suggested.

Though you need to find the same mosfet path as he had found and bridge it to the output (battery terminal) directly I believe...

Havent done this myself, but probably wait till @Fabian287 can explain this procedure better.. unless u really know your thing with bms and mosfets :D
```

---
## \#26 Posted by: IsTalo Posted at: 2017-05-18T10:47:12.584Z Reads: 111

```
Wait, if it provide the over voltage it balancea, Right? The Bms put every cell as 4.2, so it is balancing, or not?
```

---
## \#27 Posted by: Eboostin Posted at: 2017-05-18T15:01:34.530Z Reads: 106

```
I have the 10S 60A and it balances my 10S6P pack fine. Been using it for about 6 months
```

---
## \#28 Posted by: Fabian287 Posted at: 2017-05-18T15:23:54.736Z Reads: 106

```
Can you please send me some detailed pictures from all sides? So i can mark you where you have to conect them. The problem is that the BMS dont previde enought power to activate the mosfets. So by connecting the two wires the discharge mosfets will be activate because now there is the power from the discharge and from the charge mosfets = activation Power x2. 

Sry for my English im german
```

---
## \#29 Posted by: NickTheDude Posted at: 2017-05-18T18:19:44.247Z Reads: 104

```
<img src="/uploads/db1493/original/3X/d/e/de8f0b6dc7583381cca8b3f6da0b4324d0a1e9f9.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/1/71c5783a4aaac0d23eb352cb2cf0a8fcaacb6afe.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/e/1e08ffd4f421405e1b99820846d3ad5c19d7ed24.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/4/e44899e18ebb4171cb3a4c7df25c3533ccd602af.jpg" width="666" height="500">


If you need a closeup of anything in particular let me know. Thanks!
```

---
## \#30 Posted by: Fabian287 Posted at: 2017-05-18T18:36:12.379Z Reads: 98

```
can you take a picture from under?
```

---
## \#31 Posted by: anorak234 Posted at: 2017-05-18T18:39:56.041Z Reads: 99

```
@NickTheDude time for a brush-up on those soldering skills - those connections look like they'll break off the first bump you hit
```

---
## \#32 Posted by: Fabian287 Posted at: 2017-05-18T18:45:09.802Z Reads: 97

```
For me the look fine. The mosfets are soldered from the backside.
```

---
## \#33 Posted by: NickTheDude Posted at: 2017-05-18T18:52:26.964Z Reads: 98

```
<img src="/uploads/db1493/original/3X/2/f/2f5c5dbcf4235b29800556aba08fe5e7ba020c97.jpg" width="666" height="500">

@anorak234 yeah I'll definitely re do them later, I just wanted to be able to test it out quickly.
```

---
## \#34 Posted by: Fabian287 Posted at: 2017-05-18T19:17:25.871Z Reads: 97

```
<img src="/uploads/db1493/original/3X/9/e/9ebc36ac99aa6e78588ec59c2dd97c350c3f82fa.jpg" width="666" height="500"> can you check if all the marked pins are all conected together? So all orange and all blue. I cant see it good. Normaly that is right.
```

---
## \#35 Posted by: Jebe Posted at: 2018-02-26T03:36:02.946Z Reads: 55

```
Having a problem where the voltage is not fully switching off as well . Under load the voltage drops near zero when switching the BMS off, unloaded it sits around 33 volts.
This is the second supower bms ive had which has done this. :( thought i had messed up with too much heat soldering first time. This time  I was very careful. Should those fet pins be connected?

Cell 10 also was charged to 4.7 volts, all others 4.1 to 4.2 volts. 42.5 volts coming from that, now binned, charger
```

---
## \#36 Posted by: i2oadsweepei2 Posted at: 2018-07-08T19:25:05.824Z Reads: 43

```
I thought I would share this here as well to see if anyone had any thoughts on the switch.

 [E-switch on BMS](https://www.electric-skateboard.builders/t/e-switch-on-bms/13484/89):

**** Edit **** It didn’t work.
```

---
