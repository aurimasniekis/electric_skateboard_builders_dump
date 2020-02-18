# BMS caught on fire. What did I do wrong?

### Replies: 23 Views: 1375

## \#1 Posted by: Ethanstone Posted at: 2018-04-30T19:41:37.791Z Reads: 230

```
Hi,
I wired up my BMS to the batteries and a few minutes later it was in flames. What did I do wrong?
Here is the diagram that followed to wire up the BMS:
![IMG_0669|375x500](upload://caGFtgNw6rEVEnNpCnrMjpiUwHq.JPG)
Here is the sechamtic of the BMS I used:
![22 PM|690x239](upload://aDhCel1fnUspoHBgA8zF2G710iP.png)
Thanks for your help
```

---
## \#2 Posted by: Blasto Posted at: 2018-04-30T19:43:19.166Z Reads: 224

```
![image|352x500](upload://bFiG4gcDKSvJmS42aajVum9MPOo.jpg)
```

---
## \#3 Posted by: Ethanstone Posted at: 2018-04-30T19:46:39.148Z Reads: 214

```
Ohh. 
Thanks. 
Then how much power do I need to give the BMS to charge the batteries? 12v 2000mA? 12 500mA?
```

---
## \#4 Posted by: Blasto Posted at: 2018-04-30T19:51:23.068Z Reads: 210

```
[quote="Ethanstone, post:3, topic:53948"]
Then how much power do I need to give the BMS to charge the batteries? 12v 2000mA? 12 500mA?
[/quote]

the way you have it setup, you would need a 20-22V charger (6S, dont know if lipo or liion)... I can't really say more, lack of information
```

---
## \#5 Posted by: banjaxxed Posted at: 2018-04-30T20:03:19.814Z Reads: 207

```
@Acido hairy carpet
```

---
## \#6 Posted by: Mikenopolis Posted at: 2018-04-30T20:19:06.470Z Reads: 195

```
[quote="banjaxxed, post:5, topic:53948"]
hairy carpet
[/quote]

Celebrity Jeopardy?
![image|690x441](upload://wykNDSu42KA7Jo0SFPCEcx3Bq7L.jpeg)
```

---
## \#7 Posted by: b264 Posted at: 2018-04-30T20:21:18.944Z Reads: 179

```
You can't charge lithium cells with a power supply.  You need a lithium charger.  They operate in constant-current mode for a while until they switch to constant-voltage mode
```

---
## \#8 Posted by: Acido Posted at: 2018-04-30T20:22:55.025Z Reads: 169

```
A spark wont start a fire for sure on anything
But anyways its not the safest place to work with possible sparks...
```

---
## \#9 Posted by: Ethanstone Posted at: 2018-04-30T20:46:05.363Z Reads: 163

```
I have lipo batteries.
Also I forgot to put in the charger into the diagram here is the new drawing:
![54681374022__7B3FF22D-E418-489F-B0F6-8E033EFC61A3|375x500](upload://niQbRTPLI7IQ3R1pwVzExmfgoyj.JPG)
```

---
## \#10 Posted by: banjaxxed Posted at: 2018-04-30T20:52:35.919Z Reads: 150

```
That is fire started by the incorrect wiring of a bms, now if the rig above was wired up lke the thread we were dscussing, this one
https://www.electric-skateboard.builders/t/bms-wiring-issues/53892/5?u=banjaxxed

..then the carpet would go on fire, it's a case in point which coincidentally was posted after we posted on the other thread earlier today

I understand what you are sayng but there are a number of ways you can incorectly wire a bms, some ways a spark or two dead bms & like above a fire.

I think it's more of a problem then spontaneously combusting lipos or alien abductions.

@Mikenopolis you filthy bugger, love it.
```

---
## \#11 Posted by: pixelsilva Posted at: 2018-04-30T21:43:57.124Z Reads: 136

```
When the time comes to assemble my enchilada, I will definitely call some of you guys. This battery/vesc/bms thing is scary s...! I'll stay miles away from accidentally torching down this building with one of 'em custom batteries. Here 'am surrounded by carpets and wood all over the place, from floors to ceilings. These dang buildings are old, dating back just after the big quake of 1906. Even the rats here are centenary!!
```

---
## \#12 Posted by: TowerCrisis Posted at: 2018-04-30T21:52:34.020Z Reads: 126

```
What? People use bench power supplies to charge their packs all the time. I've never seen one that doesn't operate on CC and CV.
```

---
## \#13 Posted by: b264 Posted at: 2018-04-30T21:57:52.254Z Reads: 123

```
Well, I mean if you [type "power supply" into a popular search engine](https://www.google.com/search?hl=en&q=power%20supply), the entire first page of results are all things that don't do CC/CV and won't work to charge lithium packs, so I'm really not sure what you're talking about.   Perhaps you could give an example.
```

---
## \#14 Posted by: TowerCrisis Posted at: 2018-04-30T22:08:23.648Z Reads: 119

```
I'm talking about one of [these.](https://www.google.com/search?q=lab+power+supply&client=ms-android-google&biw=412&bih=604&tbm=shop&prmd=sivn&tbas=0&tbs=vw:l,price:1,ppr_max:100,mr:1&ved=0ahUKEwjG95_8gOPaAhXSo1kKHboYDO8QsnMIwQM&ei=T5PnWoaUH9LH5gK6sbD4Dg)

Most people who regularly work with electronics will have at least a cheap one
```

---
## \#15 Posted by: b264 Posted at: 2018-04-30T23:00:26.346Z Reads: 113

```
That linked one will work, but suggesting that any power supply will work and having this here for folks to read who don't know the diffrerence, so they can accidentally burn down a building, is possibly a tad foolish.  I think it's better to say "some" power supplies will work, but it's better to use a lithium charger.  Because if they know enough about electricity to know which power supply will work, and which won't, then they probably won't be needing advice on this subject in the first place.

We should err on the side of caution to prevent noob accidents.
```

---
## \#16 Posted by: TowerCrisis Posted at: 2018-04-30T23:15:32.982Z Reads: 103

```
Realistically, nobody is going to see "power supply" and go ahead and plug in their batteries into any of the 6+ types of connectors on a desktop supply without asking how to or questioning if its the right thing to do.
```

---
## \#17 Posted by: b264 Posted at: 2018-05-01T00:17:07.660Z Reads: 103

```
I disagree.  Someone will ALWAYS find a way to break something.  That's why it's good to be helpful -- and not assuming they will do the correct thing by default.
```

---
## \#18 Posted by: green-creeper Posted at: 2018-05-23T22:36:59.559Z Reads: 78

```
Hello,
As a new member, I can't start a topic, but maybe you could help me here.
I fired two BMS. I think I realized the first problem, but not the second one.

I have 3x4s batteries, trying to connect BMS. I checked all wires and detected the sequence.
Each 4s battery pack has 5 wires, 1 red and 4 black. 3 of black are PLUS, one red is the last MINUS. I used only PLUS wires. I soldered everything, then connected a battery minus to B- and checked voltage with voltmeter. Everything seemed OK. 
After couple of minutes, my wires startes to smell. 
I had no choice, but to cut them all.
I checked voltage three times before soldering, have no idea what's happened.
Could you help me? Any Ideas?
![merge_from_ofoct|142x500](upload://8H71D6r0lS2qwHK44h3oY60JEeQ.jpg)
```

---
## \#19 Posted by: Ethanstone Posted at: 2018-05-23T23:11:25.785Z Reads: 65

```
Hi,
I just want to clarify, there are two types of things you can do with the BMS. One, you can use it for discharging or two, you can use it for charging. I don't know anything about using the BMS for discharging but I know a little bit about using your BMS to charge. Here is the diagram I was refereed to by @banjaxxed for charging my BMS. ![32 PM|690x411](upload://aBU2Faeg2SpIGXNuHQ2Ti3KbNuX.jpg)
Hope that helps.
```

---
## \#20 Posted by: TowerCrisis Posted at: 2018-05-24T01:12:51.549Z Reads: 57

```
That diagram is using the BMS in a charge AND discharge scenario.
```

---
## \#22 Posted by: green-creeper Posted at: 2018-05-24T08:34:43.591Z Reads: 46

```
How you detect which of balance wires you should connect?
I use voltmeter, connect minus wire to voltmeter and check all the wires, the first one should be 3.70V and each next wire should have +3.70V more then previous one.
```

---
## \#23 Posted by: b264 Posted at: 2018-05-24T08:35:20.424Z Reads: 48

```
[quote="TowerCrisis, post:20, topic:53948, full:true"]
That diagram is using the BMS in a charge AND discharge scenario.
[/quote]

This is for using the BMS for charge only (BMS bypassed)

![32 PM|690x411](upload://5yHUi8z6fpEO8i0tayPLjo7LpOC.jpg)

Also, the extra balance wire connection (if there is one) is USUALLY on the negative end but you must check the balance lead voltages with a multimeter and read the BMS pcb or documentation.
```

---
## \#24 Posted by: Ethanstone Posted at: 2018-05-24T15:32:24.886Z Reads: 35

```
Ohh. Thanks. My bad.
```

---
