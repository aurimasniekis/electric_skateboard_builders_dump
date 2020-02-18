# Flipsky anti-spark

### Replies: 17 Views: 1027

## \#1 Posted by: JasperM Posted at: 2018-08-23T05:12:02.768Z Reads: 296

```
Has anybody used the Flipsky anti-spark switches? If so how do they hold up.

Also what is the difference between the big and the little fuse apart from the size?

![Screenshot_20180823-150947_Chrome|243x500](upload://ln5kunPyxczc0SL2uG5SWjEd0fv.jpg)
```

---
## \#2 Posted by: AutoItKing Posted at: 2018-08-23T05:56:54.338Z Reads: 279

```
Haven't used one but looks similar to most others.
Big fuse (looks like ATC style) is easily replaceable if blown, Little Fuse (brand name) is soldered to the board and must be de-soldered for replacement.
```

---
## \#3 Posted by: Pimousse Posted at: 2018-08-23T06:34:17.670Z Reads: 270

```
IIRC, a french guy blew 2 of them in a really short time (normal use)
Those are Vedder's design after all, which proves to be unreliable (no precharge).
```

---
## \#4 Posted by: Nordle Posted at: 2018-08-23T07:41:03.639Z Reads: 248

```
Well vedder design has precharge, it does aprox. take 1sec to charge 4200uF of caps (on 10S).
I never failed mine built from mouser parts, but all i built with china mosfets failed at some point.
```

---
## \#5 Posted by: DavidC Posted at: 2018-08-23T08:47:28.237Z Reads: 236

```
I've got a similar LED switch and it's not reliable. When OFF sometimes it's ON anyway, making sparks when connecting Lipos… Unpredictable. Solution is to tap on it til it's really OFF… I had to add a XT90-S on the Lipo side to avoid sparks. So better to use a XT90-S alone.
```

---
## \#6 Posted by: JasperM Posted at: 2018-08-23T08:50:49.434Z Reads: 223

```
Ive got an XT90-S already but Ive seen plenty of the more powerful boards on here using switches that would be seemingly reliable.

Sounds like I'll be continuing with a loop key or buying a more expensive switch.
```

---
## \#7 Posted by: Kug3lis Posted at: 2018-08-23T11:04:53.549Z Reads: 210

```
It's not a pre-charge, its expanded time mosfet opening that's all.. Pre-charge means you charge capacitors through resistor to limit incoming current :)
```

---
## \#8 Posted by: Pimousse Posted at: 2018-08-23T11:12:44.663Z Reads: 204

```
[quote="Kug3lis, post:7, topic:65795"]
Pre-charge means you charge capacitors through resistor to limit incoming current
[/quote]
Regarding your statement, @Nordle is right, it's precharge.

See original thread which inspired Vedder to design his own :
https://endless-sphere.com/forums/viewtopic.php?f=3&t=40142&start=100
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-08-23T11:14:36.660Z Reads: 197

```
https://en.wikipedia.org/wiki/Pre-charge

![image|481x422](upload://erWWas3WiOSTrQrmNirLSivqBcj.jpg)
```

---
## \#10 Posted by: Pimousse Posted at: 2018-08-23T11:15:59.143Z Reads: 180

```
Did you even open the link I posted ?
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-08-23T11:28:59.915Z Reads: 180

```
Yes, but it is not a normal pre-charge it just limits current for specific type doesn't even care if capacitors are fully charged, and when gate opens it blews them as massive inrush current falls through them...

Simple example look at @jtag BMS he has separate circuit to charge the load via separate resistor, the same is in my new AS switch

If you don't believe me just run simple SPICE simulation with that schematic and you will see that it limits current and then spikes back on when mosfet turns on :)
```

---
## \#12 Posted by: Pimousse Posted at: 2018-08-23T11:41:05.889Z Reads: 178

```
I know how it works. Thanks. :slight_smile: 

You say : 

[quote="Kug3lis, post:7, topic:65795"]
Pre-charge means you charge capacitors through resistor **to limit incoming current**
[/quote]

Wikipedia says :

> Pre-charge of the powerline voltages in a high voltage DC application is a preliminary mode **which limits the inrush current** during the power up procedure.

What the original designer of Antispark (Fetcher) says :

> If the controller capacitors total 1,000uF, the current would be a constant **50mA** during precharge, for about 1 second.
If the controller capacitors total 10,000uF, the current would be **500mA.** 

SO, as good engineers we both are, we will conclude that **YES**, Antispark switch **has** precharge. :slight_smile:
And YES, @Nordle was right, and I was wrong few posts earlier until I read all along the thread I posted.

And YES, it's not as smart as a DieBieMS (or Battman which I know better bc I studied and wrote firmware for tens of hours). You're right.

Guess we're all right then. :smile:
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-08-23T11:44:37.397Z Reads: 169

```
Yes, I just don't want people mix the idea of full normal pre-charge with the same pre-charge from like vedder switch schematic...
```

---
## \#14 Posted by: longhairedboy Posted at: 2018-08-23T12:31:01.930Z Reads: 167

```
This is just a vedder switch, and flipsky certainly isn't the first vendor to have them. they're fine for 10S and below unless you swap the fets out with an IRFS7734 or better, but if you leave the switch unplugged from the pcb while its on you're likely going to find it stuck on forever. Regen braking from big motors on big thane at high speed has been known to float these on rare occasion for heavier dudes. 

I use vedder switches similar to these in mine but mine have the specific fets i mentioned. 

![electronics-eswitch-raw-01|666x500](upload://xTpin6TKvFa96kLNNBpnGTtk8cQ.jpeg)

I'd like a version with 5 fets and headers for LEDs along with solder pads for MIDI fuses.
```

---
## \#15 Posted by: JasperM Posted at: 2018-08-23T13:14:50.409Z Reads: 153

```
[quote="longhairedboy, post:14, topic:65795"]
but if you leave the switch unplugged from the pcb while its on you’re likely going to find it stuck on forever.
[/quote]

Do you mean if the board is on and you physically unplug the switch while its in the on position?

[quote="longhairedboy, post:14, topic:65795"]
Regen braking from big motors on big thane at high speed has been known to float these on rare occasion for heavier dudes.
[/quote]

Sooo a 110kg rider on dual sk3s with 100mm wheels will blow it up when breaking?

Also, would an on/off switch be more reliable from a BMS, I've seen a few people running them too.
```

---
## \#16 Posted by: longhairedboy Posted at: 2018-08-24T11:31:16.696Z Reads: 130

```
[quote="JasperM, post:15, topic:65795"]
Do you mean if the board is on and you physically unplug the switch while its in the on position?
[/quote]

Yes. I'm not sure how long it takes, but if you leave it on long enough after the rocker or pushbutton is disconnected, it will just get stuck on and you have to replace components. I use the little three conductor PPM leads on mine so i have several "jumpers" i've made to keep them in the off position while wiring them in. 

[quote="JasperM, post:15, topic:65795"]
Sooo a 110kg rider on dual sk3s with 100mm wheels will blow it up when breaking?
[/quote]

If they brake hard enough at a high enough speed, its possible. I can't account for the exact conditions it requires, i just know that I've seen it happen on rare occasion. 

[quote="JasperM, post:15, topic:65795"]
Also, would an on/off switch be more reliable from a BMS, I’ve seen a few people running them too.
[/quote]

that's not really an either/or situation and depends entirely on the build. If the BMS in your application has a built in power switch then you wouldn't need both. The BMSs i use don't, so most of the time i use the switch i mentioned above (sometimes i use 300 amp flier eswitches because they seem to be more resiliant to abuse). If you're using removable lipos and a loop key, you wouldn't need either.
```

---
## \#17 Posted by: Nordle Posted at: 2018-08-24T12:11:04.268Z Reads: 106

```
wich schematic are you using?
```

---
