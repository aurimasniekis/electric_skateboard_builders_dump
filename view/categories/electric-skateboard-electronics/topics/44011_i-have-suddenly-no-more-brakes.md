# I have suddenly NO MORE BRAKES

### Replies: 63 Views: 1608

## \#1 Posted by: ElskerShadow Posted at: 2018-01-18T11:55:49.298Z Reads: 226

```
Afraid AF to ride now. 
Thi morning i changed the BMS of my last board. I haven’t touched anything FOCBOX / TX side yet now i can only accelerate with the throttle and I have absolutely NO BRAKES anymore. I haven’t touched anything on the BLDC sofware i ve checked again and I don’t see the problem. 
![image|666x500](upload://7f9O39BXwJVHUqm0qYa6PxANUFb.jpg)
![image|666x500](upload://4ez6tzFYXP4KoP48QUjKidmOksu.jpg)
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2018-01-18T12:10:41.663Z Reads: 202

```
I would point to the BMS being the logical culprit.
Care to share some info on what BMS you have and how it's hooked up and what the overall change was?
```

---
## \#3 Posted by: krloz Posted at: 2018-01-18T12:13:37.212Z Reads: 201

```
Also... your BLDC tool is upside down....


Just kidding.  Hate when that happens to my uploads too
```

---
## \#4 Posted by: Ishayc Posted at: 2018-01-18T12:15:04.267Z Reads: 199

```
Is the battery charged to full?
The BMS might cut off in this case.
```

---
## \#5 Posted by: ElskerShadow Posted at: 2018-01-18T13:46:33.686Z Reads: 187

```
No the battery is charged to 80 %
```

---
## \#6 Posted by: ElskerShadow Posted at: 2018-01-18T13:47:07.440Z Reads: 181

```
It’s exactly the same BMS i had before it’s a Bestech 100A 12S
```

---
## \#7 Posted by: Martinsp Posted at: 2018-01-18T13:50:47.129Z Reads: 175

```
If you can, just remove the BMS and try to connect battery directly if that helps, if not it might be easiest to redo the settings (unless you have a spare remote laying around) and if still no change try a different remote.
```

---
## \#8 Posted by: ElskerShadow Posted at: 2018-01-18T15:03:54.144Z Reads: 154

```
I don’t wan’t to remove the BMS since i used my last shee of heatshink. I m pretty sure i did everything right for the BMS ( it’s just 2 negative wires not rocket science ) 
I tired to apply default configuration in the app config menu and not any changes.... 
when i hit the throttle i works flawlessly but there’s absolutely no brakes and sometimes the throttle don’t work it’s such a weird behavior. Why would a bms would make my vesc act like that ?
```

---
## \#9 Posted by: ElskerShadow Posted at: 2018-01-18T15:12:29.693Z Reads: 151

```
![image|375x500](upload://hi2CCvriU9A6MWDFLJMTYldAFzg.jpeg)![image|374x500](upload://z5sr22zyz3eha91F4L7L6AuA3rL.jpeg)I have typed faults and this resulted : i dunno what i means
```

---
## \#10 Posted by: GrecoMan Posted at: 2018-01-18T15:13:39.305Z Reads: 143

```
yup. ‘‘‘tis the bms. don’t fully charge your battery and you’ll be fine.
```

---
## \#11 Posted by: Deckoz Posted at: 2018-01-18T15:25:33.391Z Reads: 139

```
Either that or a cold joint on the new BMS from his wires...if nothing else changed(cold joint, high resistance low current capability either direction) could cause your faults or broken series connections
```

---
## \#12 Posted by: krloz Posted at: 2018-01-18T15:26:23.976Z Reads: 137

```
I think he said he is only charging the battery up to 80%. Full  battery shouldn't be the issue then. But I agree it looks like your bms is not allowing your vesc to dump power to the batteries thus not allowing it to do regen braking
```

---
## \#13 Posted by: GrecoMan Posted at: 2018-01-18T15:27:27.745Z Reads: 135

```
oh yea didn’t see that.  i think @Deckoz is right
```

---
## \#14 Posted by: krloz Posted at: 2018-01-18T15:29:43.088Z Reads: 136

```
Measure each cell voltage.  Maybe the bms is not balancing well and you have one cell near 4.2v while the rest are at 80%. This could trigger an over voltage protection on the bms also cutting regen braking
```

---
## \#15 Posted by: darkkevind Posted at: 2018-01-18T15:37:49.756Z Reads: 131

```
Also, check the style of BMS you have doesn't require you to use the C- for discharge as well as charge or the other way round P- for charge aswell as discharge..?
```

---
## \#16 Posted by: ElskerShadow Posted at: 2018-01-18T15:39:51.205Z Reads: 134

```
That’s what i tought but i ve been very carefull with soldering sinc i already had issues with cold joints in the past. I what you say is right i shouldn’t have any power to accelerate either ? I can accelerate as much as before can even reach 65 kph i just can’t break, so it’s returning the energy the problem i think
I have to admit i m clearly lost on this one spent almost the day on this one and no results so far
```

---
## \#17 Posted by: Deckoz Posted at: 2018-01-18T15:44:08.480Z Reads: 127

```
[quote="ElskerShadow, post:8, topic:44011"]
sometimes the throttle don’t work it’s such a weird behavior
[/quote]

[quote="ElskerShadow, post:16, topic:44011"]
I can accelerate as much as before
[/quote]

Can you clarify this as the two conflict.

-your throttle works normal and the brakes don't work
-your throttle is janky and your brakes don't work

Clarify this too
-your BMS is used for discharging
-your BMS is bypassed for discharging

Your bestech BMS
-has an eswitch
-does not have an eswitch
```

---
## \#18 Posted by: Deckoz Posted at: 2018-01-18T15:48:47.813Z Reads: 122

```
[quote="darkkevind, post:15, topic:44011"]
C- for discharge as well as charge or the other way round P- for charge
[/quote]

Fyi that's backwards

BMS Labels(not all are on every BMS but they all are the same meaning)
-P is discharge negative (on every BMS)
+P is discharge postive (rare)
-B is battery negative (always on every BMS)
+B battery postitive (rare)
-C or -Ch is charger negative (on most BMS, if not available use -p)

There is no +C as the postitive side of the charger either connects to directly to the battery positive, or the B+ on the BMS. On BMS with no C ports. Negative charger goes to -P, postitive still goes on battery positive or b+ BMS terminal
```

---
## \#19 Posted by: ElskerShadow Posted at: 2018-01-18T15:50:05.255Z Reads: 122

```
Sorry i m not clear enough. 

The throtle is normal but janky 1 time out of 3 and no brakes 

I’m afraid i can’t answer this question. 

I don’t use the integrated e switch because the last one failed so i use an antispark. With 80A fuse
```

---
## \#20 Posted by: ElskerShadow Posted at: 2018-01-18T15:50:51.345Z Reads: 119

```
The soldering on BMS ![image|281x500](upload://vO5kDz4A4ZJV21dZzR7FBuG259u.jpeg)
```

---
## \#21 Posted by: Deckoz Posted at: 2018-01-18T15:52:15.898Z Reads: 112

```
Your -B looks mostly flowed.

But the -P looks like it was tinned, and is mostly sitting on top of the tinned solder pad. Could you reflow that pad?
```

---
## \#22 Posted by: Deckoz Posted at: 2018-01-18T15:54:06.462Z Reads: 109

```
[quote="ElskerShadow, post:19, topic:44011"]
The throtle is normal but janky 1 time out of 3 and no brakes

I’m afraid i can’t answer this question.

I don’t use the integrated e switch because the last one failed so i use an antispark. With 80A fuse
[/quote]

Cool so it looks like your discharging through the BMS. And that -P joint could be the culprit
```

---
## \#23 Posted by: ElskerShadow Posted at: 2018-01-18T15:54:07.863Z Reads: 104

```
Heating the iron right now
```

---
## \#24 Posted by: darkkevind Posted at: 2018-01-18T15:54:55.428Z Reads: 104

```
I have a BMS where C- is used for charge AND discharge...
```

---
## \#25 Posted by: ElskerShadow Posted at: 2018-01-18T15:55:38.500Z Reads: 101

```
I soledred into P- because it was already like that with the old BMS
```

---
## \#26 Posted by: Deckoz Posted at: 2018-01-18T16:00:53.408Z Reads: 107

```
[quote="darkkevind, post:24, topic:44011"]
C- is used for charge AND discharge
[/quote]

That's a first for me

[quote="ElskerShadow, post:25, topic:44011, full:true"]
I soledred into P- because it was already like that with the old BMS
[/quote]

Oh that's fine man. Was just trying to understand why this could be happening. If it is not that -P joint, then it is the BMS itself limiting current. If the BMS is limiting current it can only be one of a couple things

-BMS is improperly rated(amps)
-series connection in the battery pack is weak causing a voltage spike
-one of the parallel packs is weak, is not balanced and the BMS cuts off because of the I'm balance for safety, or has very bad(high) internal resistance.

After you reflow that -P can you put a meter on each of your cell connections on the BMS JST plug and verify each series connection reads the same voltage or within 0.02 volts of one another?
```

---
## \#27 Posted by: ElskerShadow Posted at: 2018-01-18T16:02:46.414Z Reads: 102

```
![image|375x500](upload://42BCpkCt2vMikQ9U8GyiKP4F3pa.jpg)![image|375x500](upload://5jVTHQzdGcFm7imrqY2QIWdAD3c.jpg)

I think there’s enough tin :stuck_out_tongue:
Yet i still get over voltage fault
```

---
## \#28 Posted by: ElskerShadow Posted at: 2018-01-18T16:05:09.909Z Reads: 94

```
Will need to buy a multimeter to do that, i will check all connections and voltage tomorrow. 

It’s weird the thing that bother me the most is that i used my last sheet of heatshrink for nothing hahah
```

---
## \#29 Posted by: Deckoz Posted at: 2018-01-18T16:06:16.659Z Reads: 96

```
Yea looks fine now


At this point I would suspect it is either a weak group or a bad series connection... verify voltage for me and tag me when you do. Well get it figured out I'm sure.
```

---
## \#30 Posted by: ElskerShadow Posted at: 2018-01-18T16:08:17.330Z Reads: 93

```
Will do. Thanks for your help, it’s much appreciated !
```

---
## \#31 Posted by: ElskerShadow Posted at: 2018-01-18T16:17:28.216Z Reads: 94

```
Something you wanna know maybe is that i replaced the BMS because last one had 3 mosfets burning during a ride 
The battery pack is brand new
When the bms fried I visually checked all the 18650’s connections and they seemed fine to me but i’m not an expert
```

---
## \#32 Posted by: darkkevind Posted at: 2018-01-18T16:26:24.755Z Reads: 94

```
[quote="Deckoz, post:26, topic:44011"]
That’s a first for me
[/quote]

![Screenshot_20180118-162546|243x500](upload://eHKiWtKDFbBwZw3SPb6z2AmYeuU.jpg)
```

---
## \#33 Posted by: Deckoz Posted at: 2018-01-18T17:48:38.356Z Reads: 89

```
Ah yeah. It's essentially the same as connecting to the -P, the pad is probably shared trace.
```

---
## \#34 Posted by: TarzanHBK Posted at: 2018-01-18T19:31:43.089Z Reads: 81

```
Do you have a link to your BMS?
```

---
## \#35 Posted by: ElskerShadow Posted at: 2018-01-19T14:18:19.119Z Reads: 75

```
No i don’t. It’s weird because i can still charge the battery no problem
```

---
## \#36 Posted by: ElskerShadow Posted at: 2018-01-19T14:27:56.822Z Reads: 78

```
![image|375x500](upload://fp82PMoWbVetVYkASFEKiSPhtif.jpeg)![image|375x500](upload://qsOwSpi8aqVPVrRMy1hnfkz5xSK.jpeg)![image|375x500](upload://91jPUOxsZBiyVLw9bItZtnzHguK.jpeg)

More pics in case it can help
```

---
## \#37 Posted by: SOICDIP Posted at: 2018-01-19T16:07:04.323Z Reads: 75

```
Get a BT module or a UART data logger to pinpoint the error if this happens again.
```

---
## \#38 Posted by: ElskerShadow Posted at: 2018-01-19T19:15:33.785Z Reads: 70

```
Yeah i will try with meter app to see... 
i don’t even know if the battery is the problem eveything seems in perfect shape. I have no clue of what is causing the problem,maybe it’s because i m using 12S ? Never had a single issue with a 10S battery
```

---
## \#39 Posted by: scepterr Posted at: 2018-01-19T19:46:18.614Z Reads: 68

```
Btw since you are not using -C I think youre bypassing the balancing function

Unless -C ,-P is the same trace
```

---
## \#40 Posted by: ElskerShadow Posted at: 2018-01-19T21:00:43.818Z Reads: 68

```
I can’t tell. Maybe if i solder it into C- it will change something ?
```

---
## \#41 Posted by: scepterr Posted at: 2018-01-19T21:18:50.242Z Reads: 65

```
I would connect -C and charge it a bit, the BMS might be in some protection mode...that might release it
```

---
## \#42 Posted by: ElskerShadow Posted at: 2018-01-20T12:47:03.849Z Reads: 59

```
Charge it by how much ? 
I will try it
```

---
## \#43 Posted by: Deckoz Posted at: 2018-01-20T13:10:54.396Z Reads: 58

```
Wow nice catch @scepterr I didn't even notice his -C wasn't connected. You could be right about the BMS in a protection mode, as if he's not changing via -C it may not ever be hitting balance kick off - which could lead to an Imbalanced pack putting the BMS in protection mode

@ElskerShadow have you measured the volts of each series group yet to verify balance?
```

---
## \#44 Posted by: ElskerShadow Posted at: 2018-01-20T13:24:42.417Z Reads: 55

```
Unfortunately i've been busy AF and couldn't find the time to grab a multimeter i ll buy one on amazon prime so i'll have it tomorrow. But i have to admit that i d like to find an easier solution because the pack is completely taped/ sealed it's gonna be a pain in the ass to remove all that 

But my last BMS ( wich was the same ) had no wire connected to -C, wich cable should be connected to -C ? there's only two connected to the PCB not including balance leads
```

---
## \#45 Posted by: Deckoz Posted at: 2018-01-20T13:34:33.948Z Reads: 55

```
You don't need to remove the tape to check the cells...just check the voltage at the JST connection

-C is for the negative side of the charger plug

![IMG_20180120_083253|666x500](upload://8e0L4cvwSbwNHq5BSrU7wt78eNk.jpg)
Measure from the backside of the balance JST legs on the BMS... No untaping involved

Plus not having a multimeter and building batteries... Seems silly don't ya think :)
```

---
## \#46 Posted by: ElskerShadow Posted at: 2018-01-20T16:39:35.223Z Reads: 52

```
@Deckoz @scepterr 
![image|375x500](upload://qF4uIhp3xxwHX4wVrAjvOUoFGo4.jpg)

B- is connected to the XT90 out and P- goes all the way back to the bottom of battery 
![image|375x500](upload://bHHbV1GVdeDJNOMsZHQOkuCw0iN.jpg)

My negative charger lead goes into this tiny BMS i dunno what it does 
![image|375x500](upload://l9H3FChYog3iO7uNTwNecTMBV6n.jpg)

So should i still move the p- into c- if it’ not the charging ?
```

---
## \#47 Posted by: Deckoz Posted at: 2018-01-20T16:46:07.707Z Reads: 49

```
Um

-B goes to the battery negative terminal
-P goes to the xt90/whatever connector to your load.


You've wired it backwards

I'm so confused why do you have two BMS...

Lol

The way your big BMS should be wired

Postive from charger jack to positive battery terminal
Negative charger jack to -C on BMS
Postive battery terminal to xt90/barrel out
-P (negative of the postive out) to xt90/barrel out
-B to battery negative

Vs what you have now
-some random extra BMS for charging??? 
-big BMS has -B and -P backwards
```

---
## \#48 Posted by: ElskerShadow Posted at: 2018-01-20T17:10:22.225Z Reads: 45

```
In dunno it’s always been like that, one Bms with white balance and a tiny BMS with red balance..

So maybe if i switch B - and P- it will be good tho ?
```

---
## \#49 Posted by: ElskerShadow Posted at: 2018-01-20T17:15:06.912Z Reads: 42

```
![image|375x500](upload://kALQFxsESjRQAYDlWjQt4r1ozeb.jpg)

I just did it and now the battery won’t go ON so i guess it’s not the solution...
```

---
## \#50 Posted by: Deckoz Posted at: 2018-01-20T17:15:12.218Z Reads: 41

```
To me it looks like you can remove the tiny one with red balance.

And then just stick the negative side of the charger plug to -C on the other BMS

And reverse the -B and -P


If you didn't build the board...it looks like the person who did didn't have the concept that a single BMS can be used for charging and discharging....
```

---
## \#51 Posted by: ElskerShadow Posted at: 2018-01-20T17:15:58.624Z Reads: 42

```
I built the board just i had to buy the battery, it’s from eskating.eu and built in china I think
```

---
## \#52 Posted by: Deckoz Posted at: 2018-01-20T17:18:56.290Z Reads: 42

```
Also your positive side of the charger is connected to the -ch on that second BMS  with red balance wires....

I think you have alot of things backwards..and possibly shorting...
```

---
## \#53 Posted by: ElskerShadow Posted at: 2018-01-20T17:21:19.280Z Reads: 43

```
Apprently the tiny bms is for LCD readout

I hope nothin is shorted
```

---
## \#54 Posted by: ElskerShadow Posted at: 2018-01-20T17:23:16.816Z Reads: 42

```
I will try now what you say
```

---
## \#55 Posted by: ElskerShadow Posted at: 2018-01-20T17:26:11.688Z Reads: 43

```
![image|375x500](upload://jbl0CtRmdkiDmclwcIKJaz9oWIU.jpg)
Positive charger cable goes directly into battery it’s normal ? 
 ![image|375x500](upload://wOzW0g8oZl7xp81j6Pt0RXUGBpK.jpg)

Big cable : goes back to battery 
Litle cable : negative charge input
```

---
## \#56 Posted by: ElskerShadow Posted at: 2018-01-20T17:30:36.685Z Reads: 41

```
I just did what you told me, SWapped B- and P - and switched black charging cable to C- now the battery won’t turn ON.
```

---
## \#57 Posted by: Deckoz Posted at: 2018-01-20T17:31:30.757Z Reads: 41

```
Sorry was looking at your last pictures this one is what I was coming confused about

![9446321933469bc46ec8c592c078552c997f5067_1_375x500|375x500](upload://c75niNzaLKOT3Vqer7ZCL6n8kAf.jpg)

This is how I would have wired it

![IMG_20180120_123022|374x499](upload://eg97c9Kq7zX8llDnodhnd6WwcJ.jpg)
```

---
## \#58 Posted by: ElskerShadow Posted at: 2018-01-20T17:33:32.420Z Reads: 38

```
Right now it’s wired like that and no power at all
```

---
## \#59 Posted by: scepterr Posted at: 2018-01-20T17:34:08.320Z Reads: 37

```
I'm beyond confused with your wiring and multiple BMS lol
```

---
## \#60 Posted by: ElskerShadow Posted at: 2018-01-20T17:37:01.327Z Reads: 37

```
Believe me you can’t be more confused that I am now
```

---
## \#61 Posted by: akhlut Posted at: 2018-01-20T17:38:35.830Z Reads: 38

```
Simplify?  Get one bms setup known-good then move on?
```

---
## \#62 Posted by: ElskerShadow Posted at: 2018-01-20T17:41:09.746Z Reads: 39

```
That’s obviously what I will do, excuse me man to try easier way to repair my battery, if i can try something before replacing the BMS i will do it.
```

---
## \#63 Posted by: SeanHacker Posted at: 2018-01-20T18:29:08.780Z Reads: 37

```
I would definitely do the obvious thing then and get rid of all the unnecessary complications (multiple bms's). One thing you don't want is an unsafe eboard. They're crazy enough as is and with only one BMS. ;)
```

---
