# 12s5p 30Qs charge rate?

### Replies: 121 Views: 1723

## \#1 Posted by: deecept Posted at: 2018-12-17T14:50:34.554Z Reads: 286

```
I promise I have tried to search for this, but with no luck..

I'm doing my best in building a 12s5p battery with Samsung 30Qs. All info I find says I should be able to charge this pack with maximum 15A rate - but this seems really high, even for this size pack.
My BMS is 12s 60A version from eBay, and I'm looking at [this charger](https://www.aliexpress.com/item/50-4V-10A-charger-for-12S-Li-ion-battery-pack-4-2V-12-50-4V-battery/32851314532.html).
Any inputs? (pun intended)
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-12-17T14:57:18.763Z Reads: 275

```
look at the datasheet for samsung 30q
```

---
## \#3 Posted by: rsalmon Posted at: 2018-12-17T14:58:30.499Z Reads: 274

```
While 15A for the whole pack itself should indeed be fine, you need to make sure your balance wires can withstand that much current, even if you go with 10A.

There are some stories here on the forum of people melting their balance wires and BMSs while charging even at 8A.
```

---
## \#4 Posted by: deecept Posted at: 2018-12-17T15:10:02.655Z Reads: 269

```
Hmm - good point.They are very thin.
[This is the BMS](https://www.ebay.com/itm/44V-44-4V-48V-50-4V-60A-12S-Li-ion-ion-LiPo-Li-Polymer-BMS-PCB-For-18650-Battery) I got, it states in the text:
"Max Continuing discharge Current : 60A
Max Charge Current : 30A"

Sorta the reason I bought it, but china-ware isn't always very reliable. Any way to test this before hand?
```

---
## \#5 Posted by: accrobrandon Posted at: 2018-12-17T15:10:22.183Z Reads: 260

```
I got chargers... And details there about wiring... 4amp max per cell.. ×  5 = 20amp charging potential... But as others mentioned making sure the wiring can.handle it... Input charge port should be atleast 20awg.. And a proper connector =)

https://www.electric-skateboard.builders/t/f-s-5amp-and-8amp-10s-charger-and-12s-charger-42v-50-4-lith-ion/70480
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-12-17T17:24:53.903Z Reads: 231

```
generally speaking liion max charge rate is 0.5c, so 7.5a per cell for 30q.

that means your 5p pack should be able to accept a charge rate of 37.5a.  so if you can find a charger than can do 2000 watts (50.4v * 38amp) then go right ahead.

whatever your charge rate is in amps, divide that by 5. that's your per cell charge rate.
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-12-17T17:48:40.021Z Reads: 218

```
i think you used your numberpad wrong^^
```

---
## \#8 Posted by: pjotr47 Posted at: 2018-12-17T17:49:34.109Z Reads: 214

```
0.5c -> 0.5 * 3000mah=>1.5A each cell -> 1.5*5p= 7.5A 

7.5A*50.4=378watt
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-12-17T17:53:22.401Z Reads: 207

```
7.5a per cell * 5p = 37.5amp

37.5amp * 50.4v = 1890watt, round up 2000
```

---
## \#10 Posted by: taz Posted at: 2018-12-17T18:03:46.978Z Reads: 205

```
Not true.
Charging does not take place through the balancing leads.
In most BMSs the balance leads only bleed current to balance the cells.
Charging is done via the - and + poles of the whole pack so you just have to make sure your charging leads and BMS can withstand the charging current. eg If you are using a Bestech D140 your maximum charging current is 15A whereas with a D223V1 it is 20A provided all the other components (wires, connectors etc) can take it.
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-12-17T18:08:11.770Z Reads: 193

```
ehm....what? 
30Q has 4A Max Charge. So i don't know where you get those numbers from.
```

---
## \#12 Posted by: thisguyhere Posted at: 2018-12-17T18:24:04.466Z Reads: 195

```
oop, you're right.

official spec sheet says 4a

![image|690x346](upload://xodAS8eFTIDf114YtWnhvOnaacx.png) 

i got .5c from this: https://batteryuniversity.com/learn/article/charging_lithium_ion_batteries

so for 5p pack, at 4a per cell, max pack charge rate would be 20a.
```

---
## \#13 Posted by: rsalmon Posted at: 2018-12-17T18:24:14.693Z Reads: 188

```
[quote="taz, post:10, topic:78259"]
Charging does not take place through the balancing leads.
[/quote]

I didn't mean to imply that, but I can see why you interpreted this way.

I guess the takeaway is it's generally good practice to upgrade the balance wires if you intend to charge at high currents.
```

---
## \#14 Posted by: taz Posted at: 2018-12-17T18:35:56.081Z Reads: 181

```
[quote="rsalmon, post:13, topic:78259"]
I guess the takeaway is it’s generally good practice to upgrade the balance wires if you intend to charge at high currents.
[/quote]

Why? As I wrote the balance leads will only see the BMS discharge current which is 100-200mA for most BMSs
```

---
## \#15 Posted by: pjotr47 Posted at: 2018-12-17T18:41:19.040Z Reads: 175

```
[quote="thisguyhere, post:12, topic:78259"]
i got .5c from this:
[/quote]

0.5c means 0.5* the capacity. the capacity of a 30q is 3000mah=3Ah.... 0.5c * 3Ah stays still 1.5A


I know the 30q can take 4A, that is the fast charging.
```

---
## \#16 Posted by: thisguyhere Posted at: 2018-12-17T18:42:06.662Z Reads: 167

```
damn, i was wrong again.  i mistook C for discharge, but you're right, C is capacity.
```

---
## \#17 Posted by: psychotiller Posted at: 2018-12-17T18:48:23.445Z Reads: 164

```
Why do you need to charge at the max rate? A 4a 50.4v charger will charge a 12s5p pack in under 3 hours with 18awg wire. Working to charge faster than that you are asking for trouble and certainly a short pack life.
```

---
## \#18 Posted by: thisguyhere Posted at: 2018-12-17T18:49:53.147Z Reads: 162

```
i wouldn't charge at max rate.  hell, i still use a 2amp charger.

but i think the original question was max charge rate for 30q.

sup dave.
```

---
## \#19 Posted by: taz Posted at: 2018-12-17T19:00:50.651Z Reads: 164

```
Since the standard charge current for 30Q cells is 1.5A going to 5x1.5A=7.5A will not compromise cell life.
Of course finding the proper charger and connector is another story.
Personally I would like to have a 15A charger for those times I need to use the board at the last minute and as usually it sits at 50-70% charge. All the other times a slower charger will be the one I use.
```

---
## \#20 Posted by: Hummie Posted at: 2018-12-17T19:17:49.066Z Reads: 164

```
https://scitechdaily.com/new-sensor-reveals-lithium-ion-batteries-can-safely-charge-5-times-faster/


https://batteryuniversity.com/index.php/learn/article/ultra_fast_chargers

bet you can charge with very high current when the cells are at a low state of charge
```

---
## \#21 Posted by: Battosaii Posted at: 2018-12-17T20:30:46.202Z Reads: 150

```
Yeah make sure your BMS wires can handle it. Most BMS come with 22awg balance wires and that's not enough for 10a.  I have a 12s8p 30q battery and I use a 8a charger so I used 20awg silicone with for my balance leads nothing even heats up while charging takes about 3.5 hours to full charge from dead
```

---
## \#22 Posted by: Hummie Posted at: 2018-12-17T20:50:28.573Z Reads: 147

```
But as said the balance wires take barely any current when charging
```

---
## \#23 Posted by: b264 Posted at: 2018-12-17T20:56:13.824Z Reads: 146

```
[quote="taz, post:10, topic:78259"]
Charging does not take place through the balancing leads.
[/quote]

If you wire charge-only (bypassed BMS) it **does take place through the balance leads** in a lot of ways to wire it.  It all depends on how yours is set up.  There are certainly many ways to wire it up where charging does not happen through the balance leads but throwing statements out like that could cause someone to have a fire.  It's not true a lot of the time.  Even when it does charge through the balance leads though, it would typically only have the full charge current on the end two balance leads and the middle ones would typically be 100mA maximum
```

---
## \#24 Posted by: b264 Posted at: 2018-12-17T21:02:56.476Z Reads: 147

```
Minimum wire gauge for charging:

26AWG: 2.2A continuous
24AWG: 3.5A continuous
22AWG: 7A continuous &lt;-- usually this one
20AWG: 11A continuous
18AWG: 16A continuous
16AWG: 22A continuous
```

---
## \#25 Posted by: taz Posted at: 2018-12-17T21:10:10.379Z Reads: 140

```
[quote="taz, post:10, topic:78259"]
In **most** BMSs the balance leads only bleed current to balance the cells.
[/quote]

[quote="b264, post:23, topic:78259"]
There are certainly many ways to wire it up where charging does not happen through the balance leads but throwing statements out like that could cause someone to have a fire.
[/quote]

You mean like that?
Good job isolating one part of my post buddy. :+1:
```

---
## \#26 Posted by: b264 Posted at: 2018-12-17T21:14:48.774Z Reads: 140

```
It's better to be safer, and making a statement like that can lead someone that doesn't know better to have a fire.

Picture yourself as a noob not knowing what any of the parts do, and read your post.  See how you could wire it wrong?  That's why I interjected.

Also it has just as much to do with *what BMS* you use -- as with *how* you use it.  You can wire the BMS up to only the battery with the balance wires only -- a very popular way in esk8 -- and run the large-gauge wires straight to the ESC not even touching the BMS.  This is called bypassing the BMS or running the BMS "charge-only" and is very popular.  What you said is dangerous in that context mixed with noob skill-levels.
```

---
## \#27 Posted by: taz Posted at: 2018-12-17T21:33:14.569Z Reads: 138

```
Bypassing the BMS has nothing to do with charging. The charge function (from an external charger) of a charge/discharge BMS remains the same regardless if you bypass it or not.
However I am always happy to gain knowledge so could you please provide a typical diagram of a BMS wired in a way that the charge current would flow through the balance leads?
```

---
## \#28 Posted by: b264 Posted at: 2018-12-17T21:41:21.850Z Reads: 136

```
"charge-only" or bypassed BMS, the 10AWG doesn't touch the BMS or charge port, only the 22AWG & 24AWG balance wires
![20181003_155339|690x345](upload://8D58fpNfK4HGgzkggFKMykdkgjl.jpeg) 

There are a lot of diagrams in the diagram thread, here is [a similar one](https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/128?u=b264)
```

---
## \#29 Posted by: taz Posted at: 2018-12-17T21:47:54.713Z Reads: 138

```
I know very well how to bypass a BMS.
This is one of my batteries

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/e/5edc33114e149ed0134a431025e8a0953bd115c4.jpeg)

I still fail to see how current will flow through the balance leads while charging on the diagram you linked (which by the way is exactly how I have my BMS above setup)
```

---
## \#30 Posted by: pat.speed Posted at: 2018-12-17T21:54:48.800Z Reads: 133

```
His b- connection on the bms goes straight through the first balance lead so he doesnt need a large cable going to the bms
```

---
## \#31 Posted by: b264 Posted at: 2018-12-17T21:57:41.876Z Reads: 132

```
[quote="taz, post:29, topic:78259"]
I still fail to see how current will flow through the balance leads while charging on the diagram you linked
[/quote]

That diagram isn't correct (diagrams don't have to be functional or correct to be on the thread, and we can't flag for those errors....) but similar in most ways.

Considering how the large gauge wires don't even connect to the BMS, I'm not sure what there is to misunderstand. 

In the same way that spare wire in my desk drawer isn't carrying my charge current?  In the same way that wire at your house is not carrying my charge current here.
```

---
## \#32 Posted by: taz Posted at: 2018-12-17T21:59:14.449Z Reads: 132

```
Are you talking about the photo or the diagram? On the diagram the b- goes through the BMS.
If you are talking about the photo I can't see how it is wired under all the tape and fish paper.
```

---
## \#33 Posted by: pat.speed Posted at: 2018-12-17T22:01:11.825Z Reads: 129

```
Both, either is the same. @b264 has two battery negative wires, a thic 8awg and a small whatever awg. The small one goes to the bms and the big one goes straight to the vesc
```

---
## \#34 Posted by: taz Posted at: 2018-12-17T22:06:46.943Z Reads: 131

```
 If you are talking about this diagram (which you linked as an example by the way) it is correct.
![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/d/b/dbdb3ec9f9f9ede294573a056fb83f0f7b8fcb54.jpeg)

Again what do the large (discharge) leads have to do with what we are discussing here?
We are talking about high current charging with an external charger.
I say that even if you hook up a big ass charger, provided your charging wires (not discharge wires), port and BMS are suitable you will not have a problem. The small balance leads do not see the charging current.
You say this is not correct and that there is a way to wire a BMS that the balance leads will see the charging current.
I am still waiting on that diagram.

@pat.speed You are describing a bypassed BMS. I know how it works. Don't let the 12AWG charging wires fool you on my battery shown above. I used them because I had run out of 18AWG. The discharge wires are 10AWG and are completely separate from the BMS.
```

---
## \#35 Posted by: sayekim Posted at: 2018-12-17T22:10:24.650Z Reads: 123

```
Yeah I’m with the balance leads don’t see the charge current crew until proven wrong.

It’s in the name right? Balance leads. Not charge leads.
```

---
## \#36 Posted by: b264 Posted at: 2018-12-17T22:12:08.695Z Reads: 116

```
[quote="taz, post:34, topic:78259"]
If you are talking about this diagram (which you linked as an example by the way) it is correct.
[/quote]

It's not correct because the BMS does not know the voltage of the most-positive P-pack.
```

---
## \#37 Posted by: mmaner Posted at: 2018-12-17T22:15:21.298Z Reads: 116

```
[quote="b264, post:31, topic:78259"]
That diagram isn’t correct (diagrams don’t have to be functional or correct to be on the thread, and we can’t flag for those errors
[/quote]

Mine isn't correct?  Tell me whats wrong so I can fix it.
```

---
## \#38 Posted by: taz Posted at: 2018-12-17T22:15:48.212Z Reads: 119

```
Good catch, it is missing a balance lead on the positive pole of the last p-group.
It also has 2 balance leads between the + of the 6th p-group and the - of the 7th p-group which is also wrong.
The BMS bypassing section of it is correct though.
```

---
## \#39 Posted by: b264 Posted at: 2018-12-17T22:17:53.263Z Reads: 119

```
[quote="mmaner, post:37, topic:78259"]
Mine isn’t correct? Tell me whats wrong so I can fix it.
[/quote]

B12 is missing, only B0 through B11 are shown

I'd also put the balance wires on the - end of each P-pack except the last P-pack with B+ on it gets two balance wires
```

---
## \#40 Posted by: pat.speed Posted at: 2018-12-17T22:18:13.471Z Reads: 117

```
See that little b- wire. That is the one we are talking about that can’t handle the current. Because on some bmss they have a b- wire that plugs into the connector, that wire can be split so it goes to b- on the bms and the connector. But doing that means the full charging current passes through it so it have to be capable of the current
```

---
## \#41 Posted by: b264 Posted at: 2018-12-17T22:19:31.134Z Reads: 113

```
Yes, if you are bypassing the BMS for discharge, a lot of times you can leave B- unhooked on the BMS because it directly connects to B0 (if that BMS has a B0, not all do)
```

---
## \#42 Posted by: pat.speed Posted at: 2018-12-17T22:21:10.847Z Reads: 110

```
Yep, I like to just connect them together anyway, just in case it’s isolated. Pretty sure most Chinese bms use a b0 and b- most bestech and supower don’t if I recall
```

---
## \#43 Posted by: b264 Posted at: 2018-12-17T22:22:47.560Z Reads: 108

```
I just look at the PCB and if see they are connected on the copper and measure that they are connected on the copper, adding another wire is just one more thing that could rub and short out
```

---
## \#44 Posted by: pat.speed Posted at: 2018-12-17T22:25:00.926Z Reads: 103

```
The next problem with charging like that without the extra wire is the connector is rated for probs 4a max
```

---
## \#45 Posted by: taz Posted at: 2018-12-17T22:26:57.176Z Reads: 107

```
I can see how that can happen.
However all the manufacturer's diagrams I have seen, they show the b- connected (if the BMS is of a decent charge rating).
Guys I think you can agree that there are not many stupid BMS manufacturers that would rate their BMSs for 10-15-20A continuous charge current if the current went through the puny balance leads when wired according to their instructions.
Can you make it go through at least one balance lead? Probably yes, but in that case you are wiring it wrong.

![](https://memegenerator.net/img/instances/76892751/youre-holding-it-wrong.jpg)
```

---
## \#46 Posted by: b264 Posted at: 2018-12-17T22:27:10.061Z Reads: 100

```
I usually charge at 2A but sometimes I will juice at 4A if I'm not at home.  At home I always have another board charged anyway and would charge at 500mA if I could
```

---
## \#47 Posted by: b264 Posted at: 2018-12-17T22:28:09.983Z Reads: 102

```
[quote="taz, post:45, topic:78259"]
Can you make it go through at least one balance lead? Probably yes, but in that case you are wiring it wrong.
[/quote]

Wrong to you, for your needs -- maybe, I will give you that.  But that's about all.  Definitely not wrong in all situations.  Which is the whole thing I was saying about generalising.
```

---
## \#48 Posted by: pat.speed Posted at: 2018-12-17T22:28:39.894Z Reads: 99

```
I guess it depends how you looks at it. I actually wire mine properly anyway, I was just trying to show it can be wired in a way that the leads do handle current
```

---
## \#49 Posted by: pat.speed Posted at: 2018-12-17T22:30:21.641Z Reads: 97

```
No, just stop it. I’ve had enough. It’s time for change

Stop using a f’ing Z in your words, bloody Americans. Use a S from now on
```

---
## \#50 Posted by: b264 Posted at: 2018-12-17T22:30:55.540Z Reads: 94

```
[quote="pat.speed, post:49, topic:78259, full:true"]
No, just stop it. I’ve had enough. It’s time for change

Stop using a f’ing Z in your words, bloody Americans. Use a S from now on
[/quote]

This is something we can both agree on.
```

---
## \#51 Posted by: pat.speed Posted at: 2018-12-17T22:32:03.576Z Reads: 94

```
In Aus nowadays if you take an exam and use either spelling it is classed as correct as long as it’s consistent. Just shows nobody knows what the heck to use
```

---
## \#52 Posted by: b264 Posted at: 2018-12-17T22:33:05.567Z Reads: 94

```
[quote="b264, post:47, topic:78259"]
generalising
[/quote]

It's actually hilarious you pointed that out, because I typed an "S" then when I proofread it I changed it to "Z" because that's how my fellow 'Muricans do it.  But now I changed it back to "S" how it's supposed to be and I think of it in my head.
```

---
## \#53 Posted by: taz Posted at: 2018-12-17T22:34:33.624Z Reads: 92

```
Imagine what this does to a non native English speaker such as myself. I am confused.
Still calling it aluminium though 'cause it sounds cooler.
```

---
## \#54 Posted by: pat.speed Posted at: 2018-12-17T22:40:09.507Z Reads: 94

```
I hate it when people call it aluminum
```

---
## \#55 Posted by: mmaner Posted at: 2018-12-17T22:41:48.382Z Reads: 103

```
[quote="b264, post:39, topic:78259"]
> Mine isn’t correct? Tell me whats wrong so I can fix it.

B12 is missing, only B0 through B11 are shown

I’d also put the balance wires on the - end of each P-pack except the last P-pack with B+ on it gets two balance wires
[/quote]

I see the balance wire placement issue, I have resolved it in the image and replaced it in the linked post.  I don't know how that happened, its even correct in my work document.  I guess I had versioning issue.

The Bestech D140 doesn't have a B0, only a B- which is logically identical to B1.  I specifically created the illustration with the D140 in mind as it's become very popular as of late.

![D140%20-%2012S|541x500](upload://6cgg7NZ4txb8goVZXApkzwrBcGb.png) 


**Most importantly, if you see a diagram issue (and I'm not talking specifically to you @b264, rather to everyone) point it out.  Lots of people depend on these diagrams for construction and a defective diagram can cost somebody a lot of money and fingers.**
```

---
## \#56 Posted by: deecept Posted at: 2018-12-17T22:44:14.208Z Reads: 99

```
Hi all! Been a busy day. While this has been an interesting read, I'm not really any closer to answering the question of what amperage I should charge my pack at. Now I even have developed some degree of angst as too how to set up my BMS :b:
 
Yes, 2a is safest, and 4a is possible.. But if there is no consequences to using 6,8,10 or more, why not do it? Not too bothered about years of life out of the pack.
Actually I think a charger with adjustable amperage would be the sweet spot. No hurry? 0.5a. Busy day? BOOM, 12a. Know any of those? :) 

And thanks a bunch for being so detailed in answering, I learn so much from this forum! No generaliSing ;)
```

---
## \#57 Posted by: taz Posted at: 2018-12-17T22:44:30.785Z Reads: 102

```
Still wrong Mike. Gotta connect the B12 + pole to the BMS.
```

---
## \#58 Posted by: mmaner Posted at: 2018-12-17T22:45:53.922Z Reads: 101

```
From what point to what point?
```

---
## \#59 Posted by: pat.speed Posted at: 2018-12-17T22:47:23.918Z Reads: 100

```
You can make an adjustable charger using a boost converter, watt meter and 24v+ power supply. Or you can go reverse and buy a 48v psu and a buck converter, some have integrated watt meter type things too. Just make sure to get a cc/cv charger
```

---
## \#60 Posted by: pat.speed Posted at: 2018-12-17T22:47:58.998Z Reads: 102

```
The pos of the battery pack should be your last connection b12 if it’s 12s
```

---
## \#61 Posted by: taz Posted at: 2018-12-17T22:50:00.131Z Reads: 102

```
![Screenshot_20181218-004922_Chrome|243x500](upload://h89Z5RbOQkHmKwH1Kw7BSHyIhq1.jpeg)
```

---
## \#62 Posted by: mmaner Posted at: 2018-12-17T22:50:11.639Z Reads: 96

```
Isn't that only for discharge?
```

---
## \#63 Posted by: mmaner Posted at: 2018-12-17T22:51:48.110Z Reads: 97

```
So, move the B1 balance lead from cell group B1 to the Positive of cell group B12?  I'm just trying to make sure I am understanding this correctly, not being argumentative.
```

---
## \#64 Posted by: taz Posted at: 2018-12-17T22:56:15.423Z Reads: 98

```
No the B1 balance lead goes to the B1+ p-group.
Take a look a Bestech's diagram, it's all in there.
It's getting late here guys, I am going to sleep.
See ya...
```

---
## \#65 Posted by: pat.speed Posted at: 2018-12-17T22:56:55.155Z Reads: 97

```
Kinda, some bmss are meant to have that b0 (the balance lead on the negative of the pack) some are not. It just depends. If the bms has 12 wires you leave it off, if it has 13 you add it. The wire like @taz said however needs to be there as the b12
```

---
## \#66 Posted by: mmaner Posted at: 2018-12-17T22:59:26.704Z Reads: 95

```
OK, but I can't tell what the arrows on the pic @taz made are pointing at.  The manual for the D140 says the balance leads are NEG connections.  While it is technically a charge/discharge BMS in my illustration it is wired for charge only, which I understood meant the POS connection was NOT used.  Is that incorrect?  If so please just tell me what wire needs to move from which point to which point.
```

---
## \#67 Posted by: pat.speed Posted at: 2018-12-17T23:07:58.673Z Reads: 97

```
Ok sorry for the bad drawing I’m on mobile, but basically with your bms the b- or b0 doesn’t need to be connected to the balance wire connector. As can be seen in the bestech wire schematic if you read the PIN numbers on the board there is no wire going to b-. This means the balance lead that goes from the neg of the battery shouldn’t be there. However I don’t think it would pose a problem if it was connected. 

As I also drew the balance lead from the positive side of the battery was missing. This must be connected so that the last cell of the pack is monitored/balanced. It will be b12.

![image|690x304](upload://cMgETG6EJmoyZOkVKeGAwVZrGY9.jpeg)
```

---
## \#68 Posted by: mmaner Posted at: 2018-12-17T23:12:51.680Z Reads: 88

```
I am still confused, the X I see on the the drawing above is on B1 balance wire.  So you are saying that the B1 balance lead and the B- negative lead should not be there and that Balance wire B12 goes to the positive of cell group B12?
```

---
## \#69 Posted by: pat.speed Posted at: 2018-12-17T23:17:07.852Z Reads: 95

```
Ok, that wire that I crossed out is not b1. B1 is the positive side of the cell. I crossed out b0 which is not used in this case. In the diagram I put below you will see what I mean![image|281x500](upload://8hyN6ltqsdoz1QS9wlYx4vKi1fK.jpeg)
```

---
## \#70 Posted by: Sebike Posted at: 2018-12-17T23:33:01.357Z Reads: 94

```
no. you're wrong. the diagram clearly sais it's "discharge only", so I assume the charging and balancing wires are broken or not connected.
```

---
## \#71 Posted by: mmaner Posted at: 2018-12-17T23:54:25.626Z Reads: 91

```
Its charge only, apparently I fucked the whole thing up
```

---
## \#72 Posted by: mmaner Posted at: 2018-12-17T23:57:18.009Z Reads: 90

```
I would really appreciate it if someone would just draw whats its supposed or tell me the label(s) of the lead that needs to move and label(s) of where it needs to move too because I still do not understand.
```

---
## \#73 Posted by: b264 Posted at: 2018-12-18T00:02:06.835Z Reads: 88

```
[quote="Sebike, post:70, topic:78259, full:true"]
no. you’re wrong. the diagram clearly sais it’s “discharge only”, so I assume the charging and balancing wires are broken or not connected.
[/quote]

But there is no way for the BMS to know the voltage of the first P-pack, it is 100% wrong

Look at the red wire @pat.speed [put in there](https://www.electric-skateboard.builders/t/12s5p-30qs-charge-rate/78259/67?u=b264)
```

---
## \#74 Posted by: deltazeta Posted at: 2018-12-18T00:03:22.015Z Reads: 88

```
Functionally, the BMS has to compare voltages between two consecutive balance leads for any sort of protection to kick in. If you leave out any balance lead the protection circuits can't determine if there's an overcharge problem.
```

---
## \#75 Posted by: Sebike Posted at: 2018-12-18T00:07:22.525Z Reads: 89

```
aesthetically pleasing though :smiling_face_with_three_hearts:
```

---
## \#76 Posted by: Sebike Posted at: 2018-12-18T00:39:11.498Z Reads: 94

```
Tired and with a headache, but hopefully I managed to get it right. If not, let me know and I'll burn it, chop it and flush it.

Charge only. 

![DSC_0096-01|690x388](upload://nsOpn77Xa0IlCQVz4s61oRN6xD6.jpeg)
```

---
## \#77 Posted by: pat.speed Posted at: 2018-12-18T00:41:57.078Z Reads: 92

```
This, this is the correct wiring. Although some bmss will have an extra wire going from here into the connector for a total of 13 balance wires![image|281x500](upload://32Iw8GtOSgnAOC7XvMqAsK6UrzQ.jpeg)
```

---
## \#78 Posted by: lrdesigns Posted at: 2018-12-18T00:58:59.246Z Reads: 90

```
[quote="deecept, post:56, topic:78259"]
Actually I think a charger with adjustable amperage would be the sweet spot. No hurry? 0.5a. Busy day? BOOM, 12a. Know any of those? :slight_smile:
[/quote]

This? only up to 10a though. 
https://www.amazon.com/TekPower-TP6010E-Adjustable-Switching-Digital/dp/B015QHVJR4/ref=sr_1_3?ie=UTF8&qid=1545094633&sr=8-3&keywords=60v+power+supply+10a
```

---
## \#79 Posted by: mmaner Posted at: 2018-12-18T01:26:04.967Z Reads: 92

```
Thank you for that, I really do appreciate it.  I'm just trying to understand here, please just work with me.

I see this...
![image|82x100](upload://fFZ0krvg5c5vqxT6lOAH8BUHUbr.jpeg) 
Does that mean all the balance leads go to the positive side of the cell groups?

I see this...
![image|60x73](upload://q6pnCKWC23Hhe4q6cIoyNKobvmg.jpeg) 
Does that mean that Balance Lead B12 is functionally connected to both the Positive of cell group B12 and the  pack as a total?

Lastly this...
![image|197x100](upload://q3kaxTHftgp9xYqB6TZMyqcQEPL.jpeg) 
Does that mean that the charge port negative is connected to P- and the charge port positive is connected to cell group B12 as well as the balance lead B12 and the entire pack positive?
```

---
## \#80 Posted by: pat.speed Posted at: 2018-12-18T03:54:47.979Z Reads: 86

```
Yes, I am pretty sure that’s what it’s is meant to be. The reason b12 is on the positive is so that the bms can measure the last cells voltage. If there is no lead on the positive side it cannot do this as to measure voltage you need both the anode and cathode
```

---
## \#81 Posted by: mmaner Posted at: 2018-12-18T03:57:15.900Z Reads: 78

```
I'm glad to know it. I'll have to pull my packs and do some checking.
```

---
## \#82 Posted by: pat.speed Posted at: 2018-12-18T04:03:37.153Z Reads: 80

```
Oh, about the bit with the balance going to the positive side of the series connection, it doesn’t actually matter which side of the series connection as they are both connected together.

Essentially you should have one wire going to each side of every cell, except for you the main negative on some bmss
```

---
## \#83 Posted by: Sebike Posted at: 2018-12-18T06:37:16.368Z Reads: 78

```
What @pat.speed said ^^
```

---
## \#84 Posted by: taz Posted at: 2018-12-18T08:16:11.978Z Reads: 77

```
Does this help? I have added the difference in potential from B- (or B0) assuming 4.2V cell charge state.

    Battery        BMS     ΔV
    B1-              B-          0
    B1+             B1         4.2
    B2+             B2         8.4
    B3+             B3        12.6
     .
     .
     .
    B12+           B12      50.4

On the D140  you could also connect the B1- to the B0 in the BMS (since there is electrical continuity between these 2) using the balance lead but that would end up with the full charge current going through that lead.`Preformatted text`
```

---
## \#85 Posted by: b264 Posted at: 2018-12-18T08:39:17.167Z Reads: 80

```
It's usually marked 
```
B- -- 0V
B0 -- 0V  (not always present)
B1 -- 4.2V
B2 -- 8.4V
B3 -- 12.6V
B4 -- 16.8V
B5 -- 21V
B6 -- 25.2V
B7 -- 29.4V
B8 -- 33.6V
B9 -- 37.8V
B10 -- 42V
B11 -- 46.2V
B12 -- 50.4V
B+ -- 50.4V  (doesn't connect to BMS)
```

Connecting 13 balance leads to B0 through B12 allows you to charge through the balance leads without connecting B- or B+ to the BMS, in most but not all cases

If you did that, full charge current would flow through B0 and B12 and approximately 100mA maximum would flow through B1 through B11
```

---
## \#86 Posted by: mmaner Posted at: 2018-12-18T13:51:04.395Z Reads: 74

```
Functionally the only change I made was to move the B12 balance lead to the positive side of the CG12 from the negative.  Is that correct?  The B12 Balance lead, pack positive and charge positive are on the positive side of the CG12 now.

![Esk8%20Construction%20Diagram%20-%20battery%20only|690x299](upload://aHoT6YIuzTaEPNhZcYcD5JHpDn3.jpeg)
```

---
## \#87 Posted by: Sebike Posted at: 2018-12-18T14:18:26.449Z Reads: 73

```
In your diagram you don't have a balance lead (b11) between cell group b11 and b12. 

And you have battery negative connected to b1 on the bms. 

IF battery negative is supposed to be connected as a "balance lead" on your specific bms it should most probably be to b0, as the b1 should be connected inbetween cell group 1 (+) and cell group 2 (-)
```

---
## \#88 Posted by: mmaner Posted at: 2018-12-18T14:19:45.526Z Reads: 74

```
There's no B0 on the D140, so I assume I should move all of the balance leads to the positive side of the cell groups, correct?
```

---
## \#89 Posted by: Sebike Posted at: 2018-12-18T14:23:44.141Z Reads: 75

```
If you don't have b0, the least confusing way is to think balance lead - > positive side of cells.

As long as b1-b11 is connected between cell groups and b12 is on cell gr 12s positive side, it should be right.
```

---
## \#90 Posted by: taz Posted at: 2018-12-18T14:26:37.991Z Reads: 74

```
![Screenshot_20181218-162600_Chrome|243x500](upload://uo6LVPEHHStQ0g21ORo1vOcbhQi.jpeg)
```

---
## \#91 Posted by: mmaner Posted at: 2018-12-18T14:27:18.511Z Reads: 68

```
Copy that, I think I am understanding now.  Thank you so much for taking the time to explain this, not a lot of people would and I want you to know I appreciate it.
```

---
## \#92 Posted by: Sebike Posted at: 2018-12-18T14:28:14.426Z Reads: 69

```
Any time, any day 😊
```

---
## \#93 Posted by: b264 Posted at: 2018-12-18T16:23:55.537Z Reads: 74

```
[quote="mmaner, post:88, topic:78259, full:true"]
There’s no B0 on the D140, so I assume I should move all of the balance leads to the positive side of the cell groups, correct?
[/quote]

There is a B0 on the D140 image [you linked above](https://www.electric-skateboard.builders/t/12s5p-30qs-charge-rate/78259/55?u=b264), but other ones still have it on the PCB, but the connector does not go all the way to it.  It all depends on your specific unit.

![2b6fe483c2bb24d6089a9769e3c3be09d9fd05af%20(copy)|541x500](upload://23ijC6ObTNDgRHNMyKnmbpflfbI.jpeg)
```

---
## \#94 Posted by: mmaner Posted at: 2018-12-18T17:03:30.726Z Reads: 71

```
I have x5 D140's right now, none of them have the B0 even though the image does.  The image on the website still shows it but they don't actually come with it.
```

---
## \#95 Posted by: b264 Posted at: 2018-12-18T17:12:02.672Z Reads: 69

```
It should be electrically the same as the B- pad, just lower current (aka only suitable for charging)
```

---
## \#96 Posted by: taz Posted at: 2018-12-18T17:37:17.410Z Reads: 67

```
My D140 has a B0 on the balance connector but it is labelled B- like in the photo.
```

---
## \#97 Posted by: Indiangummy Posted at: 2018-12-18T17:42:44.228Z Reads: 65

```
Hey are your packs in balance? I wonder how it's doing that since the balance leads are connected to the - of the p packs. It wouldn't know what the voltage's of the packs would be right?
```

---
## \#98 Posted by: Friskies Posted at: 2018-12-18T18:00:37.774Z Reads: 68

```
I contacted bestech specifically asking about B0 when I was assembling my pack and they told me "do not connect B0 to the negative terminal". So I have assembled my pack according to the manufacturer specifications. it works very well and keeps I'm balance without issues.
```

---
## \#99 Posted by: mmaner Posted at: 2018-12-18T18:02:06.266Z Reads: 70

```
I checked 2 of them last night, one was built over a year ago using the previous illustration.  Its still perfectly in balance.  There's no cell group more than .01 volts off from the other cell groups.  I don't know what that means, as correlation doesn't equal causation, but I am glad it's the case.
```

---
## \#100 Posted by: Indiangummy Posted at: 2018-12-18T18:03:51.296Z Reads: 71

```
Don't fix what aint broken. 😂
But that's wired. Its like if you put one end of your multimeter on ground and the other on the - of the packs.
```

---
## \#101 Posted by: mmaner Posted at: 2018-12-18T18:04:55.700Z Reads: 68

```
I am going to re-wire all of them to make sure they are right.  I just wish someone had pointed out the schematic was wrong 3 weeks ago :slight_smile:.
```

---
## \#102 Posted by: pat.speed Posted at: 2018-12-18T21:08:13.289Z Reads: 66

```
It doesn’t matter which side the balance wire is on, it can be on the negative of each p group or the positive, they are both connected together anyway so it makes no difference
```

---
## \#103 Posted by: b264 Posted at: 2018-12-18T21:17:08.706Z Reads: 68

```
[quote="taz, post:96, topic:78259, full:true"]
My D140 has a B0 on the balance connector but it is labelled B- like in the photo.
[/quote]

B- and B0 are the same electrically but typically a small guage wire is B0 and a large gauge wire is B-
```

---
## \#104 Posted by: b264 Posted at: 2018-12-18T21:17:54.048Z Reads: 69

```
[quote="mmaner, post:101, topic:78259"]
I just wish someone had pointed out the schematic was wrong 3 weeks ago :slight_smile:.
[/quote]

I looked at it, and didn't notice.  Sorry :expressionless:
```

---
## \#105 Posted by: Indiangummy Posted at: 2018-12-18T21:38:03.576Z Reads: 69

```
Oh ok, that's counter intuitive to me atleast. But I didn't know that. Thanks.
```

---
## \#106 Posted by: taz Posted at: 2018-12-19T05:22:51.705Z Reads: 70

```
That is correct. I just pointed out that in the case of the D140 they are both labelled B-.
```

---
## \#107 Posted by: hyperIon1 Posted at: 2018-12-19T07:49:28.767Z Reads: 78

```
Hey Guys, 
I've been meaning to bring this to your attention. I know a lot of people have used the D140 too much success, myself included.
The one problem that we have had with it was its size and the absence of protection.
we have found an alternative that is self-contained and protected, smaller as well. 
the HCX-127 10s and 12s
the HCX-124 10s
pictured with the D140
![IMG_0990|663x500](upload://uFa7cQO63fcUOtnxmraeg8KA4t2.jpeg) 
![189FA7A1-4277-4C74-ADAB-D938B2A38C80|575x500](upload://8qUK1mU5G0qUNNiSO96NmgxC1uq.jpeg) 
![9E954FFB-C3C3-4F49-9868-186FB07AB7E7|353x500](upload://3C6aDBJ8nD4yO4hUnzM6DW5o5db.jpeg)
![1BD398DA-F755-47ED-AABB-8C19AB6BC352|690x258](upload://dbbRYanLFbUZYcXvhQGHseZh5Cw.jpeg) 
![1F723A25-E272-4433-86D0-38D53FB78B7A|422x499](upload://oAisaZN9FyiMoMj1Ie1RuGToLTP.jpeg)
```

---
## \#108 Posted by: b264 Posted at: 2018-12-19T08:06:33.308Z Reads: 78

```
**10S**:

The HCX-D239 looks great if you're using lipo instead of li-ion cells.  It's very, very similar to the HCX-D124 except can charge at 8A instead of 4A and has voltage settings slightly better for lipo.
```

---
## \#109 Posted by: hyperIon1 Posted at: 2018-12-19T08:10:38.797Z Reads: 79

```
and then, of course, the Cadillac of bms 
the tiny bms programable and communication 
![56%20AM|650x500](upload://3daEN6iY8HtCWkVtttJFKd3Y5zB.png)
```

---
## \#110 Posted by: b264 Posted at: 2018-12-19T08:11:30.519Z Reads: 79

```
To me, Cadillac that is not.  More things to fail.  Too many features.

When streetface is the failure mode, I don't want to take extra chances.
```

---
## \#111 Posted by: hyperIon1 Posted at: 2018-12-19T08:15:38.709Z Reads: 79

```
Cadillac in price for sure, one of the best bms units on the market for what it does. 
is it something esk8 friendly, no 
cost alone sends it down the road.....
I would like to see a bms that is durable with communication for pack diagnosis
```

---
## \#112 Posted by: b264 Posted at: 2018-12-19T08:23:11.688Z Reads: 74

```
A simple beep would be nice from a tiny piezo buzzer if there are non-critical problems
```

---
## \#113 Posted by: Sebike Posted at: 2018-12-19T08:27:43.405Z Reads: 76

```
And some magic smoke or flames if critical problems. Anything to keep you well informed of pack status.
```

---
## \#114 Posted by: DerelictRobot Posted at: 2018-12-20T06:34:54.222Z Reads: 71

```
Got a link? To this or the prior one you linked?
```

---
## \#115 Posted by: hyperIon1 Posted at: 2018-12-20T07:21:09.204Z Reads: 68

```
The tiny bms : https://www.energusps.com/shop/product/tiny-bms-s516-150a-750a-36
```

---
## \#116 Posted by: dareno Posted at: 2018-12-20T07:49:41.424Z Reads: 67

```
Too much information really.  I put a turbo boost monitor on my 4wd and then suffered from anxiety everytime it went above 18.  Took it off now I sleep again.  Don't do bluetooth, Don't do any of the other stuff that can interfere with me actually riding the board.  I don't need to know if hill B caused a voltage spike, I don't need to know if I drew 80 amps or 60 amps going up hill A.  What I don't want is something else that can fail while hurtling down a hill at 40mph.  Maybe reset my vesc or shut the battery down.  I know its charge only but seriously how much info do you really need? Keep it simple stupid safe. I like the external balancer that @SkaterBoy58 has come up with.  Go back to balancing outside the enclosure like rc.  More space for batteries equals more power  :sunglasses:
```

---
## \#117 Posted by: Hummie Posted at: 2018-12-20T08:05:00.897Z Reads: 65

```
having the bms on the outside seems safer. Don't want anything else that could possibly break and cause an accident.  that's a bigger worry for me than a fire.    I was looking at @SkaterBoy58 thing but its more than I want to do but like to make a simpler version.   was going to do a version with 12 little lipo chargers but was told it might blow up with the common ground.  I still don't know if I believe it! ahhhaaaha  Do it.
```

---
## \#118 Posted by: dareno Posted at: 2018-12-20T08:08:40.128Z Reads: 63

```
https://www.youtube.com/watch?v=FQRW0RM4V0k
```

---
## \#119 Posted by: hyperIon1 Posted at: 2018-12-20T08:13:38.633Z Reads: 65

```
HCX-127 bms 
http://litechpower.com/
Just a small note on li-tech power and bestech, they are the same company or sister companies.
```

---
## \#120 Posted by: pat.speed Posted at: 2018-12-20T09:10:29.250Z Reads: 64

```
Got a link to @SkaterBoy58’s bms? I think mine has carked it
```

---
## \#121 Posted by: dareno Posted at: 2018-12-20T09:46:33.656Z Reads: 63

```
On his build thread.  

https://www.electric-skateboard.builders/t/la-croix-long-range-cruiser-carving-machine/76960
```

---
