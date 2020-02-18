# Confirmation of my Wiring

### Replies: 50 Views: 1219

## \#1 Posted by: swimmydude Posted at: 2019-01-06T02:37:47.554Z Reads: 160

```
![GoblinGlider%20schematic|500x500](upload://eJ4zmTne1QrVQM24sNtkuuJ1Fro.png) 


Didn't want to clog up my build thread. I realized that I probably should have just drawn the schematic instead of scouring for a good program to draw this up on. Then I realized I would have to spend time to learn a new program, so opted for subpar paint. Anyway, I think everything is solid but I feel like I'm missing something or got something wrong despite constantly researching everything.

I know the loopkey is redundant but I know that is good when it comes to this type of thing. I didn't choose to go with an antispark because I already have a switch that came with the Unity and I don't have the antispark connectors for it anyway. (Took me forever to realize that anitspark loopkeys were made differently. I felt like I was missing something when I just couldn't understand how it worked despite knowing the theory behind it.) Is the loopkey in the correct spot? Maybe it should be on the negative side? Or somewhere else?

Instead of wiring in a voltage display. I am using a Firefly remote and DAVEga combo. Not entirely sure how I'm going to have both work but that's a problem for later. I know I can at least use at least one.

Last thing is the type of wiring. BMS wires will be of the wires they came with. 22 AWG for the wire with the fuse. As far as I'm concerned, then everything else is 10 AWG wiring? At least the wires that directly connect to the batteries? 

Thanks for any of the suggestions and input.
```

---
## \#2 Posted by: akhlut Posted at: 2019-01-06T02:42:39.278Z Reads: 133

```
![20180319014420808|480x500](upload://TEQcIFjFYU2swCdlDu7r4WZjlW.jpeg)

omit loop key, its kinda like an arming switch and is just an additional point if failure.

your balance leads go to the positive terminals of the batteries, not the negative terminals.
```

---
## \#3 Posted by: swimmydude Posted at: 2019-01-06T02:51:37.674Z Reads: 128

```
That's essentially what I have? Not sure what this tells me. I can confirm that is the bms I have. I came to the conclusion that the B- (which I have labeled as -B on accident) on the connector slot is functionally the same as the part on the side of the bms.

_edit:_ Oh, you made an edit. Okay, I can omit the loopkey. I realize that if I ever had the switch on and inserted the loopkey, I could be in trouble. Otherwise wouldn't it be fine though?

Isn't it the same thing basically since where I have it labeled on the negative portions of the battery cells the positive is directly in contact? I can change the labeling to make it easier to read/digest though.
```

---
## \#4 Posted by: monsterbuilder Posted at: 2019-01-06T03:03:39.290Z Reads: 121

```
Following.  Also need help with the same schematic.
```

---
## \#5 Posted by: swimmydude Posted at: 2019-01-06T17:54:37.545Z Reads: 119

```
![1|500x500](upload://2SaF64ZSuY4TdAoZFT3baSorOUj.png) 

I've updated. Took out the loopkey. Unless the wiring is actually wrong or the labeling is off, I'm leaving the bms wiring the same. Because the semantics of connecting it to positive or negative side is virtually the same. They are connected in series going in a snaking fashion. Maybe the labeling would make more sense if I connected to the "positive side" because then the last parallel group wouldn't look like it was 9 and 10. I do appreciate the feedback though. Anybody else have thoughts? I was hoping to finish up today.
```

---
## \#6 Posted by: ventisca1011 Posted at: 2019-01-06T18:35:49.062Z Reads: 106

```
Got thesame schematic but mine is a mess :smiley:
```

---
## \#7 Posted by: J0ker3366 Posted at: 2019-01-06T18:40:37.000Z Reads: 104

```
Why did you remove the loop key? Does the bms have a power switch with it?
```

---
## \#8 Posted by: ventisca1011 Posted at: 2019-01-06T18:40:52.187Z Reads: 104

```
They said you can add battery gauge in unity is that true?
```

---
## \#9 Posted by: J0ker3366 Posted at: 2019-01-06T18:41:58.916Z Reads: 105

```
You can add a battery gauge to any setup. Just have to wire in line somewhere.
```

---
## \#10 Posted by: swimmydude Posted at: 2019-01-06T18:48:33.757Z Reads: 102

```
Because my first reply said I should. I didn't have a reasonable response to say yay or nay and no one else commented. So I went with it. I do have an antispark switch that came with the Unity. It's just placed through the Unity. I would assume any incoming current goes through that first before anything else in it.
```

---
## \#11 Posted by: J0ker3366 Posted at: 2019-01-06T18:52:03.201Z Reads: 97

```
Put the loop key back in. You can put it on the negative side or after your charge port and you'll be able to charge without turning on the board. If you put it in between the 🔋 and bms, you'll have to turn the board on when charging.

That loop key is your saving grace. Always keep it. Unless they put out a antispark that can uphold to our abuse.
```

---
## \#12 Posted by: J0ker3366 Posted at: 2019-01-06T18:54:01.254Z Reads: 96

```
Also, you don't need two positive wires off the battery. Main wire should be 12 or 10awg to xt60. Your charge wire can be 14-18awg but you can just solder the two together @ connection.
```

---
## \#13 Posted by: thisguyhere Posted at: 2019-01-06T18:58:51.676Z Reads: 93

```
U forgot b- coming off bms, that goes to pack main negative

Also why omit a loopkey, how's it going to be switched on and off?

Put voltmeter after loop key and before unity so u get voltage reading when loopkey is in
```

---
## \#14 Posted by: akhlut Posted at: 2019-01-06T19:11:00.847Z Reads: 90

```
the unity has a switch built into it, no need for loopkey.  why would you need to turn on board to charge?  why u need meter?  unity has bt built in, just use app.  if u want hardwired meter use antispark to monitor unity 5v rail and make contact for meter leads.  its just a fancy switch.
```

---
## \#15 Posted by: J0ker3366 Posted at: 2019-01-06T19:12:45.850Z Reads: 89

```
[quote="akhlut, post:14, topic:80063"]
the unity has a switch built into it, no need for loopkey.
[/quote]
Newly educated lol.
```

---
## \#16 Posted by: akhlut Posted at: 2019-01-06T19:15:22.292Z Reads: 90

```
![Screenshot_20190106-141445_Chrome|243x500](upload://7BPTiVoQPnWdRCQ9butlQ0Hco91.jpeg)
```

---
## \#17 Posted by: swimmydude Posted at: 2019-01-06T19:16:53.091Z Reads: 86

```
It's not built in. It comes with a switch that you connect to your system. As I noted in my first post. I realize it's redundant but isn't that what we want? Extra failsafes?

_edit:_ Is it not an antispark? I was led that it was. Regardless I don't have antispark connectors, so building an antispark loopkey is out of the question. At least for now.
```

---
## \#18 Posted by: J_Dizzle Posted at: 2019-01-06T19:19:35.661Z Reads: 88

```
The unity has a push to start feature and auto shut off after a few minutes
```

---
## \#19 Posted by: akhlut Posted at: 2019-01-06T19:20:31.035Z Reads: 87

```
the antispark is built into the unity.  you just need a way to physically turn it on - thats the physical switch.
```

---
## \#20 Posted by: swimmydude Posted at: 2019-01-06T19:42:50.943Z Reads: 88

```
![1|500x500](upload://iTZoQvGBEmWYNs1GlWvosCttMCo.png) 

Okay, I realized I don't have any 20awg wires but I do have 16awg. Which would might be fine but doesn't really match up with what I'm trying to have with my fuse. Is 12awg enough for the battery wires instead of 10? The difference between 41a and 55a?

@akhlut Thanks, now I know the distinction. Still though, you don't believe the extra failsafe is worth the chance of extra failure? Even if at worse it's just making a new loopkey?

@thisguyhere I didn't though? I labeled it wrong but fixed it in this iteration. Also is voltmeter needed? I will have reading on DAVEga and/or Firefly. And can't the Unity app read it too, like akhlut said? I dunno if the Unity app can read it while the board is off though.
```

---
## \#21 Posted by: Sebike Posted at: 2019-01-06T22:18:22.399Z Reads: 76

```
For safety reasons I would definately not build a board without physically being able to cut the circuit in case of whatever might happen and fail, as in "loop key". +1 on putting it back. :slightly_smiling_face:
```

---
## \#22 Posted by: akhlut Posted at: 2019-01-06T22:50:08.657Z Reads: 75

```
yup.  keep the loop key and omit the switch.  might have to jump some pins on the unity to make that happen, but not 100% sure.
```

---
## \#23 Posted by: thisguyhere Posted at: 2019-01-06T23:13:34.493Z Reads: 72

```
My bad, @akhlut has a point tho, totally forgot switch built into unity. Deeply ashamed 

Also no need nfor voltmeter, i just like a quick visual check without having to open app and all that
```

---
## \#24 Posted by: Indiangummy Posted at: 2019-01-06T23:18:34.770Z Reads: 75

```
If you want to use a loop key you will have to short the pins on the unity. Not plugging in the led switch is the same as installing it and never pressing the button. 

Edit: yeah, what @akhlut said.
```

---
## \#25 Posted by: ventisca1011 Posted at: 2019-01-07T00:10:54.158Z Reads: 73

```
is it necesary to put fuse in this schematic? i got same wiring but i didnt put one :slight_smile:
```

---
## \#26 Posted by: swimmydude Posted at: 2019-01-07T04:07:03.551Z Reads: 73

```
It adds an extra layer of safety. Helps breaks the connection if it gets too crazy for whatever reason. From what I gathered, there's several places you can put it depending on what you're looking for. I won't go into it because I'm not experienced enough to state them confidently right now. My intention for the fuse is if anything happens while charging, it won't catch my house on fire. 

@akhlut Alright, lol. I'm under the impression that the switch is just not going to do it. I can look into what I need to alter but you wouldn't happen to have any starting points on that do you? I guess I can't just not plug in the switch and it work like that?
_edit:_ oops, I know see that @Indiangummy stated that not plugging it in is the same as having it in and not turning it on. So I will have to do some manipulation.
```

---
## \#27 Posted by: Indiangummy Posted at: 2019-01-07T04:08:57.549Z Reads: 72

```
no you have to make the connector shorted and then plug it in. someone in the unity thread did it. im not sure who but someone has.

Edit: if you do this then unity will be in always on mode and then you can use a loop key to turn on and off.
```

---
## \#28 Posted by: Indiangummy Posted at: 2019-01-07T04:12:04.167Z Reads: 70

```
@swimmydude found it 
https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/48?u=indiangummy
```

---
## \#29 Posted by: swimmydude Posted at: 2019-01-07T04:15:12.781Z Reads: 69

```
Okay, thank you. I shall bookmark and reference that in the next few days. Since the Unity apparently has antispark built inside, I'm more comfortable not using the switch. Still going to be weird since switch is so much more elegant than a damn loopkey. 

Other than that, would you say the schematic is fine? Wire gauges and all?
```

---
## \#30 Posted by: Indiangummy Posted at: 2019-01-07T04:16:52.547Z Reads: 69

```
[quote="swimmydude, post:29, topic:80063"]
spark built inside, I’m more comfortable not using the switch. Still going to be weird since switch is so much more elegant than a damn loopkey.

[/quote]

yeah im using the unity with the switch. no problems so far. not many miles on it though. but i trust it. :grinning:
```

---
## \#31 Posted by: swimmydude Posted at: 2019-01-07T04:18:41.631Z Reads: 68

```
oh jeeze, apparently you'll lose push to start and auto turn off function. Sigh. I mean this is my first build so it's not like I'm losing anything I had previously. I won't have to butcher my switch wires and such. Since I do have blank jst pins I bought recently. I have learned that I actually hate crimping though.
```

---
## \#32 Posted by: akhlut Posted at: 2019-01-07T04:19:04.073Z Reads: 67

```
![IMG_3223|666x500](upload://5jC7cgs5B39RhX67ewKUvuZ0UGz.jpeg) 

@Indiangummy got it.  short mom1 and mom2 on the unity
```

---
## \#33 Posted by: Indiangummy Posted at: 2019-01-07T04:19:28.642Z Reads: 66

```
[quote="swimmydude, post:29, topic:80063"]
would you say the schematic is fine? Wire gauges and all?
[/quote]

you need a wire from Battery negative to the B- on the bms. since its a charge only setup you can use 22-24 AWG wire. besides that i think you're good. may want some on more experienced check it though.
```

---
## \#34 Posted by: akhlut Posted at: 2019-01-07T04:22:27.568Z Reads: 63

```
it doesnt hurt to use a heavier gauge wire from B- to the negative battery terminal.  i used 14awg for P and B.
```

---
## \#35 Posted by: swimmydude Posted at: 2019-01-07T04:24:58.899Z Reads: 66

```
and @Indiangummy  Okay. On the schematic, I DO have negative terminal to B-. Just for simplicity, I opted for the B- on the connector rather than the B- on the side of the bms. BUT if you think I should use a heavier gauge wire for it. Then that will be enough for me to go the extra effort to solder to the side of the bms rather than just using the connector. 
Just to clarify, it's the first connection on the bms before B1. I dunno why the bms decided to have two spots for B-.
```

---
## \#36 Posted by: akhlut Posted at: 2019-01-07T04:55:19.827Z Reads: 64

```
![Wiring|500x500](upload://yPGM7AQuQrdIwm6OksnjncpfTpy.jpeg)
```

---
## \#37 Posted by: swimmydude Posted at: 2019-01-07T05:37:54.921Z Reads: 61

```
oops. I didn't update it one last time. Thanks. I guess I should have stated that it was connected like that. I just assumed it was implied, haha.

![parallel%201|666x500](upload://optMJNslqYxSqT5PwXsLYUojqpI.jpeg) 

![parallel%202|666x500](upload://zlrbSJqcjgc2ApfudmHUYcQCU4s.jpeg) 

![battery|375x500](upload://1wZ2TNIzUVsGO14aih0ngwpV6o0.jpeg) 

![batteryy|666x500](upload://s3qGJkP0z2LrblMf1wN8bQMRNUu.jpeg)

Definitely not the cleanest or neatest but it is my first build and I think it will hold.
```

---
## \#38 Posted by: b264 Posted at: 2019-01-07T06:40:06.758Z Reads: 62

```
If you remove the balance wires for brevity, you're doing yourself a disservice.  The balance wires *have to be* correct.
```

---
## \#39 Posted by: Scream Posted at: 2019-01-07T06:52:32.230Z Reads: 63

```
I don’t mean to add further confusion here... but why do you need to short the unity switch just because you have a loop key?

Why not just have both? I have the unity and no loop key, but I can’t see why you couldn’t just add a loop key to the circuit, and keep it connected. Only disconnect the loop key for longer periods of inactivity or in an emergency.

Loop key should be between the positive side of the battery and everything else. That way when you remove the key everything is grounded, not “live”. I guess you could have the loop key after the charger circuit so you can charge without it attached... but if you’re only removing the loop key for storage or emergency I’d just make it so removing the key kills everything.

You should snip the corners off your nickel strips 👍

Edit: my bad you definitely snipped the corners for the positive ends
```

---
## \#40 Posted by: Jcullinan09 Posted at: 2019-01-07T07:06:04.477Z Reads: 61

```
Just to clarify, should balance wires stem outwards to BMS from cell groups on positive or negative side of the cells?
```

---
## \#41 Posted by: b264 Posted at: 2019-01-07T07:19:31.577Z Reads: 61

```
It's better to run them off the negative sides and one will need to come off the positive side on the end.  Electrically, it makes no difference.  Mechanically, shorts are more likely on the positive ends so keep those simpler.  Less stuff = less stuff to short under vibration
```

---
## \#42 Posted by: swimmydude Posted at: 2019-01-07T07:52:10.332Z Reads: 61

```
That's a good point. Alright, I won't shortcut on that. Before I wire them up, I will have another drawing just for extra clarification. I feel like there was a time you said that you need to wire them in a certain order or no?

@Scream Yea, that was my thought process too. I'm not fully convinced otherwise, but it doesn't matter to me in the end. I don't have enough experience to say nah that's wrong. I trust it. I won't be butchering my switch's wiring though. I can make a short with some 5-pin jst I have somewhere.

I grinded the corners of all my strips. Took me forever because I don't have a motor grinder at home. I was mortified that you didn't think it was enough until I read your edit. Haha. I'm glad it's sufficient.
```

---
## \#43 Posted by: swimmydude Posted at: 2019-01-07T08:29:08.913Z Reads: 61

```
![2|500x500](upload://lJrvBT6c7YnoyQsDpgKvR1N9X3T.png) 

Meh, still not a super clean drawing but I think it has everything now. Now these are my reasoning for what I'm going for.

* BMS wiring is connecting to negative side due to me already having tabs on my battery pack. But refer to b264's comment about that two messages up.
* The loopkey can be either negative or positive side apparently. Preference will be the deciding factor. This NOT an antispark loopkey.
* Fuse is rated 7.5 amps and 58v due to b264's suggestion in many other threads.
* I already have my battery put together for the most part. Parallel groups are spot welded to pure nickel. Series are connected by tinned copper braids. 
* My wiring choices is mainly due to what I have but it's close to what is the norm. My 12 awg should preferably be 10awg though. My bms came with its own wiring which is 22 awg. The other wiring is 20 awg.

That should clarify everything and hopefully help future thread searcherslooking for info. Thanks for the input guys.
```

---
## \#44 Posted by: b264 Posted at: 2019-01-07T09:11:56.896Z Reads: 52

```
Looks good.  Make sure the series connections in the battery are at least 12AWG but for a dual motor drive I would recommend 10AWG for those and the power wires, but 12AWG will work

12AWG is awesome for single-motor builds and it works fine for dual; I just prefer 10AWG
```

---
## \#45 Posted by: janpom Posted at: 2019-01-07T09:26:06.563Z Reads: 50

```
The charger should go into C-, not P-. The P- is for discharge.

Edit: ... if there is a C-, which is apparently not the case for D140. Thanks @akhlut for correction.
```

---
## \#46 Posted by: akhlut Posted at: 2019-01-07T11:51:16.746Z Reads: 47

```
There is no C- on D140, just B- and P-.
```

---
## \#47 Posted by: janpom Posted at: 2019-01-07T11:56:59.797Z Reads: 47

```
I see. Sorry. If there was a C- though... :smiley:
```

---
## \#48 Posted by: Sebike Posted at: 2019-01-07T11:59:52.531Z Reads: 48

```
I, myself, would put a ~10A fuse in series with the charge port, but not on the discharge side.
```

---
## \#49 Posted by: ventisca1011 Posted at: 2019-01-07T12:25:14.829Z Reads: 48

```
https://www.unikboards.com/en/boutique/12s-60a-battery-bms/ im using this bms i think im okay without a fuse ?.?
```

---
## \#50 Posted by: Sebike Posted at: 2019-01-07T13:33:52.986Z Reads: 47

```
As long as nothing fails you're ok without a fuse :thinking:

If your charger or charging port is shorted out, your BMS will fry plus you might end up with a battery fire. This is where I believe a fuse would make a (positive) difference. 

I wouldn't put a fuse on the discharge side, as that would unable me to control the board if the fuse would burn during a ride. I wouldn't trust a fuse there, and I'm not sure if it would add safety or make the board less safe. (Opinions differ regarding this though, and some ppl might put fuses on the discharge side as well or cell level fuses)

The BMS would probably cut the over-current coming from the battery, so that would hopefully save my ESCs. If battery is shorted through the balancing cables, a discharge fuse won't save me anyways. 

Use good cells, insulate well (shrink wrap and fish paper), proper routing of cables, well built battery, make sure nothing moves around and monitor your cells regularly so you know your battery is healthy!
```

---
