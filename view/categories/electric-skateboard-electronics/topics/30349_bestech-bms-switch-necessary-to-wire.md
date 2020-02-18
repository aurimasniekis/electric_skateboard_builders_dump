# Bestech BMS switch- necessary to wire?

### Replies: 60 Views: 4118

## \#1 Posted by: MontPierre Posted at: 2017-08-11T17:07:31.102Z Reads: 388

```
Hi!

Just got a delivery of my BMS 10s Beatech 80A.

I have vedder anti spark switch which works amazing. 

Do I have to wire switch on this BMS to have it working ? Or can I just have wires disconnected as they are and use my existing switch? I'm not sure if switch on BMS is currently on... and I can use it as it came. Otwerise I think they would add a switch by default like a balancing cable which came in the box.

Thanks
```

---
## \#2 Posted by: willpark16 Posted at: 2017-08-11T17:25:09.860Z Reads: 363

```
Which model?
```

---
## \#3 Posted by: MontPierre Posted at: 2017-08-11T17:28:18.452Z Reads: 364

```
@willpark16 I've seen remarks about switch but it isint clear to me

<img src="/uploads/db1493/original/3X/a/d/ad13ccd2fb07871b1631b88b3e81554b87194343.jpg" width="281" height="499">
```

---
## \#4 Posted by: willpark16 Posted at: 2017-08-11T17:37:24.867Z Reads: 328

```
U don't need the eswitch for that
```

---
## \#5 Posted by: MontPierre Posted at: 2017-08-11T17:38:40.114Z Reads: 327

```
Ohh cos remarks of "switch must be on during charging and discharging " threw me off. Have you got one of those BMS yourself?
```

---
## \#6 Posted by: willpark16 Posted at: 2017-08-11T17:40:10.248Z Reads: 322

```
Yea actually in the lab rn and it's 2 feet away from me
```

---
## \#7 Posted by: MontPierre Posted at: 2017-08-11T18:10:08.612Z Reads: 320

```
Lol! So I'll connect it as on their diagram and should work fine without switch being in on position? I don't have to solder switch wires together ? I'm just making sure as I don't want to burn it on fist day :D
```

---
## \#8 Posted by: willpark16 Posted at: 2017-08-11T18:17:03.601Z Reads: 321

```
<img src="/uploads/db1493/original/3X/3/c/3c270d2dac8353fae7063a170cd368936c6170af.png" width="664" height="500">
```

---
## \#9 Posted by: MontPierre Posted at: 2017-08-11T18:18:09.867Z Reads: 303

```
Cool! Thanks !
```

---
## \#10 Posted by: Lionpuncher Posted at: 2017-08-11T20:20:58.168Z Reads: 293

```
Ok. I'm still confused. Sorry to butt in. I have the same bms and still trying to get my head wrapped around the e switch situation. What are you doing with those wires then? I was led to believe that the e switch would nullify the need for a Vedder switch or similar Sps switch. Please help me out. :pray:
Do i need a vedder sw if i use it? Can i ignore this wires and use a Vedder instead? This is consuming me right now. Haha
```

---
## \#11 Posted by: mmaner Posted at: 2017-08-11T20:41:32.982Z Reads: 287

```
The switch on the Bestech BMS is not a +/-, it simply closes or opens a circuit to turn on the BMS.  If you dont want to use it, just solder the ends together and its always on.  Then use a Vede Anti-Spark switch right after the battery pack.
```

---
## \#12 Posted by: Lionpuncher Posted at: 2017-08-11T20:45:38.935Z Reads: 274

```
Thank you. Would it not be recommended to use this as the boards on/off switch? I thought I saw a thread where they did that...
```

---
## \#13 Posted by: mmaner Posted at: 2017-08-11T20:46:59.671Z Reads: 272

```
Its what I normally use, the BMS that is.  Lots of people like the pretty light up switch on vedder switches :slight_smile:.
```

---
## \#14 Posted by: Lionpuncher Posted at: 2017-08-11T20:51:14.757Z Reads: 270

```
Cool, thanks @mmaner! I think I'll go for a retro car switch maybe. Give it a night rider feel...
```

---
## \#15 Posted by: Namasaki Posted at: 2017-08-12T07:17:17.614Z Reads: 269

```
@MontPierre @Multiple_Scoregasm 
The E-Switch has to be on when discharging or else you will have no output from the bms. 
  
The E-Switch has to be on during charging or else the battery won't charge. 

The E- switch doubles as a reset switch in the event a protection circuit is tripped.  So if you hard wire the switch on, you'll have to pull the enclosure and seperate the wires to reset the bms.
```

---
## \#16 Posted by: Lionpuncher Posted at: 2017-08-12T10:18:41.667Z Reads: 268

```
Ok perfect t that what i needed to know.  Clearly using the e switch as my on/off is a no brainer. Thanks for the additional info @Namasaki. Now to pick a switch.... :thinking:
```

---
## \#17 Posted by: MontPierre Posted at: 2017-08-12T10:23:22.387Z Reads: 274

```
Get a latching LED switch  - some are water proof.

https://www.ebay.co.uk/itm/122004041613 

This is what I have and it will go perfectly with my black enclosure ;) 

I'm getting rid of my vedder antispark- just takes too much precious space in the enclosure.

Here is wiring diagram to get switch LED working. Just need to calculate a resistor. 

http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/294?u=montpierre
```

---
## \#18 Posted by: Lionpuncher Posted at: 2017-08-12T10:32:53.466Z Reads: 259

```
Waterproof and dust proof would be ideal. Thanks for the suggestions and wiring help.
```

---
## \#19 Posted by: Silverline Posted at: 2017-08-12T11:28:48.188Z Reads: 257

```
Nice switch. But wouldn't be better to find a switch with a 5v led insted of 12/24v. So the led could be powered from the 5v output on the VESC.
```

---
## \#20 Posted by: MontPierre Posted at: 2017-08-12T11:38:47.781Z Reads: 254

```
This one has 6/12/24 voltage rating - for switch itself. I'll test it and see how bright it is under 5V from vesc and then I'll know. I might need to add resistor to limit current to led. 

I could not find any 5V that I liked. 6V will be fine ;)
```

---
## \#21 Posted by: Silverline Posted at: 2017-08-12T11:42:11.311Z Reads: 242

```
No need to limit the current :-) the current is only going to be as high as the LED needs. Do you have the switch already ? Nice if it can run on 6v voltage
```

---
## \#22 Posted by: MontPierre Posted at: 2017-08-12T11:53:47.974Z Reads: 240

```
Yeah I have it already but didn't have time to connect it yet. I'll try tonight. I think with 5V it might be a tad dimmer than with 6V which doesn't bother me at all ;)
```

---
## \#23 Posted by: Silverline Posted at: 2017-08-12T11:55:09.980Z Reads: 237

```
Nice..  can you report back 😃
```

---
## \#24 Posted by: MontPierre Posted at: 2017-08-12T12:13:17.543Z Reads: 232

```
Will do !!
```

---
## \#25 Posted by: MontPierre Posted at: 2017-08-12T21:43:18.859Z Reads: 233

```
Mission accomplished! 5V works well! 


<img src="/uploads/db1493/original/3X/0/7/071f4c25930767685b1bb9d4fa65a3e3719c935c.JPG" width="544" height="500">
```

---
## \#26 Posted by: Silverline Posted at: 2017-08-13T07:13:28.816Z Reads: 226

```
Perfect thanks. I order one..
```

---
## \#27 Posted by: MontPierre Posted at: 2017-08-22T16:39:48.894Z Reads: 212

```
FYI it also has same brightens over 3.3V :D
```

---
## \#28 Posted by: Luuke Posted at: 2017-11-03T22:14:01.565Z Reads: 204

```
[quote="Namasaki, post:15, topic:30349"]
The E-Switch has to be on during charging or else the battery won't charge.
[/quote]

Is there any option, that it is possible to charge when switch is off?
So the switch is just for discharging?
```

---
## \#29 Posted by: Namasaki Posted at: 2017-11-04T00:40:51.478Z Reads: 197

```
Bestech says the switch must be on. That's all I know.
```

---
## \#30 Posted by: Lambjr088 Posted at: 2017-11-04T03:07:56.386Z Reads: 192

```
I wonder if these will work with 5v even tho it says 12v.
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F182825054149
```

---
## \#31 Posted by: MontPierre Posted at: 2017-11-04T08:44:00.080Z Reads: 185

```
I’m pretty sure yes. I think the 12V is the upper range. Give it a try ;)
```

---
## \#32 Posted by: Acido Posted at: 2017-11-05T11:31:06.164Z Reads: 182

```
the power for the switch is 12v?
```

---
## \#33 Posted by: Acido Posted at: 2017-11-07T07:05:39.840Z Reads: 179

```
What voltage us in the wires for the switch 12 or battery voltage in my case 42v?
```

---
## \#34 Posted by: MontPierre Posted at: 2017-11-07T10:56:21.666Z Reads: 175

```
@Acido I just measured the switch connected to Bestech bms and when switched off it is at approx 7.5V. When I switch on my board it goes down to 0V ;)

That’s connected via Bestech bms switch cables which come with it as standard bare without a switch. 

Led is connected to 5V output on vesc.
```

---
## \#35 Posted by: Acido Posted at: 2017-11-07T13:57:20.570Z Reads: 173

```
Cool thanks will bookmark your message :)
```

---
## \#36 Posted by: Lambjr088 Posted at: 2018-02-28T06:12:33.805Z Reads: 165

```
@MontPierre. How has the switch been doing connected to the vesc? Do u have any pics?
```

---
## \#37 Posted by: MontPierre Posted at: 2018-03-10T15:53:35.240Z Reads: 165

```
Hi! Its' been fine. To VESC I only connected LED wires from the switch ( to 5V on VESC) rest is connected to BMS switch. Unfortunately, I don't have the board with me to take pics at this moment.This should help.

http://www.electric-skateboard.builders/t/led-button-for-vedders-antispark-switch/15787/40?u=montpierre
```

---
## \#38 Posted by: bevilacqua Posted at: 2018-03-10T16:08:40.666Z Reads: 161

```
does the BMS still balance at 42V (10s) when the switch is off? 

With the metr app its kinda practical as you can set up a notification when the battery reaches its target voltage, letting you know when your board is ready...
```

---
## \#39 Posted by: Namasaki Posted at: 2018-03-10T17:30:13.794Z Reads: 160

```
[quote="bevilacqua, post:38, topicI:30349"]
does the BMS still balance at 42V (10s) when the switch is off?
[/quote]
Can’t say for sure. 
 The bms has to be on during charging per the manufacturer but it does appear to continue trimming after the charger and bms are turned off.
```

---
## \#40 Posted by: bevilacqua Posted at: 2018-03-10T17:48:34.764Z Reads: 155

```
thanks :) It should continue balancing...  
I'll email besetech. If I know anything else I'll let it know in this thread
```

---
## \#41 Posted by: webst Posted at: 2018-05-02T08:59:46.083Z Reads: 135

```
Should it be momentary or latching switch?

Edit:
I found @mmaner post suggesting that it is latching one.
 
[quote="mmaner, post:11, topic:30349, full:true"]
The switch on the Bestech BMS is not a +/-, it simply closes or opens a circuit to turn on the BMS.  If you dont want to use it, just solder the ends together and its always on.  Then use a Vede Anti-Spark switch right after the battery pack.
[/quote]
```

---
## \#42 Posted by: Caydenfish Posted at: 2018-06-03T03:05:17.689Z Reads: 118

```
So is it an okay idea to just Solder these wires together and then use a antispark switch elsewhere? Or should an antispark switch be used to connect the wires?
```

---
## \#43 Posted by: Namasaki Posted at: 2018-06-03T21:47:13.715Z Reads: 120

```
It’s not a good idea to solder the E-switch wires together because the E-switch also serves as a reset switch when the bms goes into protection mode. 
There is no need for an antispark switch with this bms
```

---
## \#44 Posted by: Caydenfish Posted at: 2018-06-19T03:44:21.632Z Reads: 118

```
Question, putting everything together right now, but how do you turn the BMS on/off? I understand that the wires must be together during both charging and discharging, but so you disconnect them during storage?
```

---
## \#45 Posted by: ervinelin Posted at: 2018-06-19T04:01:55.506Z Reads: 110

```
I didn't realise this, I bought an anti-spark switch so now it's just lying around for my next build.

I use a latching push button switch with external LEDs (https://www.electric-skateboard.builders/t/rolling-fortress-lacroix-prototipo-dual-focbox-6374-diy-mbs-geared-drive-12s4p/59021)
```

---
## \#46 Posted by: Namasaki Posted at: 2018-06-19T05:21:12.585Z Reads: 111

```
Use a latching on/off switch connected to the 2 white wires.
```

---
## \#47 Posted by: Namasaki Posted at: 2018-06-19T05:22:48.973Z Reads: 114

```
Your board looks amazing!
Nice job👍
```

---
## \#48 Posted by: XTLA Posted at: 2018-06-19T13:21:00.705Z Reads: 108

```
So the e-switch wire from bms are not +/- , just connect them to the switch that has 2 pin, just like that?
```

---
## \#49 Posted by: Namasaki Posted at: 2018-06-19T20:45:53.936Z Reads: 104

```
[quote="XTLA, post:48, topic:30349, full:true"]
So the e-switch wire from bms are not +/- , just connect them to the switch that has 2 pin, just like that?
[/quote]


yes you are correct
```

---
## \#50 Posted by: Namasaki Posted at: 2018-06-19T23:27:58.405Z Reads: 98

```
Also, any 12v automotive switch will work as long as it is not a momentary switch.

A toggle switch will work and a Latching push button switch will work.
```

---
## \#51 Posted by: Trdolan03 Posted at: 2018-06-24T19:03:26.247Z Reads: 92

```
Is it an anti-spark of sorts of would it be advisable to solder those two wires together and put an anti-spark in the build?
```

---
## \#52 Posted by: XTLA Posted at: 2018-06-28T06:53:43.996Z Reads: 88

```
I think this will work, it’s waterproof, but the size...

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F173351231625

![image|537x500](upload://s1QOFFD5QhTd8rridHGdqd3ht4G.jpeg)
```

---
## \#53 Posted by: shark78921 Posted at: 2019-06-15T12:24:38.749Z Reads: 41

```
Where is it i can buy that switch?
```

---
## \#54 Posted by: mattfink Posted at: 2019-07-07T17:12:51.167Z Reads: 34

```
Hi wonder if anybody can help me.

Trying to work out where on the Bestech 10S BMS i wire the eswitch, ![15625193989355264262873033711855|281x500](upload://rOubFGlAKaBgl5sEXoPuMsZaTsU.jpeg) 

Is it the connectors next to B- labelled D4, D5 or somewhere else.
```

---
## \#55 Posted by: vortek Posted at: 2019-07-07T18:11:05.433Z Reads: 33

```
There are two white wires that go from there check the image:
![image|281x500](upload://6UxyvWspWdrEyfixTvzQeCdXjDy.jpeg) 

If they are joined it is ON. Just use whatever switch you would like.
```

---
## \#56 Posted by: mattfink Posted at: 2019-07-07T19:14:12.376Z Reads: 32

```
So the 2 white wires that are attached to the heat sink, i plugged the thing in and it seems to be on, so i need to detach them and link them to a switch?
```

---
## \#57 Posted by: vortek Posted at: 2019-07-07T23:30:14.532Z Reads: 31

```
Using a multimeter you can see if current travels between B- and C- or P- and verify that those wires are indeed the switch. Just use a JST plug and put a on/off switch. 
![image|463x463](upload://9fTaESba1HULSwHmCDwKJvHx2Js.jpeg)
```

---
## \#58 Posted by: XTLA Posted at: 2019-07-08T07:55:58.652Z Reads: 29

```
I think that 2wires goes to temperature sensor which is attached to the heatsink. He need to find another switch wires.
```

---
## \#59 Posted by: vortek Posted at: 2019-07-08T11:37:10.860Z Reads: 24

```
I have the exact same BMS and on mine the two wires come from the heatsink and go down that hole and out the side as this picture:

![image|450x338](upload://N9S7UjrBPoXeYjdLSjLdYiunqh.jpg)
```

---
## \#60 Posted by: XTLA Posted at: 2019-07-08T12:19:23.496Z Reads: 23

```
Yea that one.
![image|450x338](upload://fCNSgRS7mXQ852FPS3cXPd32e1i.jpeg)
```

---
