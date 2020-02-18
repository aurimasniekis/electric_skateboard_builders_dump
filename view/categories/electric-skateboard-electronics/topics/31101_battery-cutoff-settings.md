# Battery cutoff settings

### Replies: 61 Views: 3278

## \#1 Posted by: Jdubb121212 Posted at: 2017-08-20T13:58:15.793Z Reads: 372

```
I have a 12s2p battery 
6374 190kv motor
focbox
nano remote
This is my first time setting up a vesc so bear with me,
just wondering what my battery cutoff settings should be (start and end)?
```

---
## \#2 Posted by: darkkevind Posted at: 2017-08-20T14:18:15.519Z Reads: 358

```
Fully charged your batteries will be 4.2v per cell, so that's your max voltage. 

Fully discharged you shouldn't let them go below 3.2, some would say 3.1 is ok but remember 3.7 is the nominal voltage.

So.... 3.2v x however many cells you have is your absolute cut off voltage. 
Dependant on how much warning you want to have, raise that a fraction of a volt or two (per cell) for your cut off start.
```

---
## \#3 Posted by: Jdubb121212 Posted at: 2017-08-20T14:21:33.082Z Reads: 340

```
I actually bought the diyelectricskateboard battery pack and I'm not sure how many cells there are?
```

---
## \#4 Posted by: darkkevind Posted at: 2017-08-20T14:55:16.446Z Reads: 329

```
[quote="Jdubb121212, post:1, topic:31101"]
I have a 12s2p battery
[/quote]

You've already told us...

12s = 12 cells. 's' = cells in **s**eries.
'p' = cells in parallel.
```

---
## \#5 Posted by: rich Posted at: 2017-08-20T15:10:39.523Z Reads: 310

```
Also important is your Batt max setting because you have not much amp output from 12s2p.
I just looked at their Homepage, no info which cells are used but the BMS is rated for 30A Continuous Amp Output and 80A Peak Amp Output. If the cells are 20A cont. you have 40A max from battery, but the cells will get hot when used at their limits. Would be good if they have used 25A or 30A cells, maybe someone knows.
Batt regen would be about -8A, Motor regen (brake) should not be too far away from motor regen (maybe -30 to -40A).
```

---
## \#6 Posted by: Crossfire Posted at: 2017-08-20T15:24:29.092Z Reads: 303

```
3.2 V per cell is too low imho. You'll feel that after 3.7V they start to get sluggish and sag a lot more. That's because momentarily they're reaching even lower voltages (when accelerating for example) - like 3.3 or 3.2V. When you stop and check the voltage they get back up in voltage. Running them too low often, they'll degrade sooner. 

Under 3.5V they are starting to loose charge, voltage drops abruptly.
[https://i.stack.imgur.com/LV91V.gif](https://i.stack.imgur.com/LV91V.gif)
My opinion is that 3.6 V is absolute low if you want long term performance, reliability and safe operation. To reach 300-400 duty cycles, discharge them to 3.6V, rare to 3.5V.

My 8S setup gets me to over 12km when I discharge them to like 3.7V per cell. Which is more than enough.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-08-20T15:34:11.651Z Reads: 288

```
I have an 8s pack too, I kind of agree with you, if you're pulling they'll drop significantly at anything around 3.6v, but if you wanted the most out of your pack and wasn't too worried about pack longevity, you could go lower...
```

---
## \#8 Posted by: MontPierre Posted at: 2017-08-20T15:42:26.999Z Reads: 283

```
[quote="rich, post:5, topic:31101"]
Batt regen would be about -8A, Motor regen (brake) should not be too far away from motor regen (maybe -30 to -40A).
[/quote]

I have 10S zippy 8000mah which are rated 5C current charge.  Does it mean I can have 40A batt regen? I'm currently on 25A or 30A. 

Also - I think I should check if my Bestech BMS 10s 80A allows regen. I've heard it doesn't but board breaks fine. If your bms doesn't support regen I would only have motor min to play with ? That's regen also ... Or does bms just produce heat instead of feeding batteries with current? 

Edit 

So I have researched and there is no clear answer ;) well as long as it works and breaks I'm happy ;)
```

---
## \#9 Posted by: Crossfire Posted at: 2017-08-20T15:53:25.315Z Reads: 265

```
Exactly ;)
```

---
## \#10 Posted by: Namasaki Posted at: 2017-08-20T16:32:48.769Z Reads: 263

```
[quote="MontPierre, post:8, topic:31101"]
So I have researched and there is no clear answer :wink: well as long as it works and breaks I'm happy :wink:
[/quote]


Here is a clear answer for you:

I tested the Bestech HCX-D223V1 (Not Bypassed) braking continuously downhill while monitoring pack voltage. And I am pleased to inform you that this bms in this configuration does support regen charging. And not only that.
I conducted the test with a full battery. My total pack voltage climbed to 42.8v but would not go any higher because the bms's overcharge detection is set at 42.8 from the factory to allow some headroom while charging(they feel that this is a safe threshold so I went with it). So it stopped climbing at 42.8 and as soon as I stopped braking, the bms quickly trimmed the voltage back down to 42v while supposedly balancing the cells.

During this test I experienced NO issues with the Vesc shutting off or any brake failure.
```

---
## \#11 Posted by: MontPierre Posted at: 2017-08-20T16:37:20.844Z Reads: 248

```
@Namasaki That's great news! Thanks ! If I was to put in batteries of 42.3V  charged with seperate charger and connect them to bms would it immediately start trimming them down? How long did it take to trim them down from 42.8 to 42? Just out of curiosity.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-08-20T16:40:18.747Z Reads: 243

```
[quote="MontPierre, post:11, topic:31101"]
If I was to put in batteries of 42.3V  charged with seperate charger and connect them to bms would it immediately start trimming them down?
[/quote]

Although overcharging less than 1v on the total pack voltage seems to be an acceptable amount, I would not recommend doing so intentionally.
It would be nice if the Vesc allowed adjustment of the regen braking voltage.
```

---
## \#13 Posted by: MontPierre Posted at: 2017-08-20T16:41:14.757Z Reads: 234

```
Noted! How long was trimming of excess voltage?
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-20T16:41:22.465Z Reads: 226

```
[quote="MontPierre, post:11, topic:31101"]
How long did it take to trim them down from 42.8 to 42? Just out of curiosity.
[/quote]


It only took maybe 10 seconds.
```

---
## \#15 Posted by: MontPierre Posted at: 2017-08-20T16:44:09.049Z Reads: 224

```
Wow! That's quick! I'm thinking of investing in bench power supply to get my balancing working, at the moment my charger shuts off at 42V ;( and I have to balance lipos individually with separate balance charger. Doesn't take long but it's a pain in the butt ;)
```

---
## \#16 Posted by: Namasaki Posted at: 2017-08-20T17:00:03.542Z Reads: 225

```
[quote="MontPierre, post:15, topic:31101"]
at the moment my charger shuts off at 42V ;( and I have to balance lipos individually with separate balance charger. Doesn't take long but it's a pain in the butt :wink:
[/quote]

Are you using a bms?
The bms wil balance the cells but it will do so by trimming them down unlike a hobby charger which holds the full cells while bringing up the low cells.
IMO, nothing charges better than a hobby charger.

Understand that under charging is said to increase battery life and this is why Bestech designed their bms to trim the cells down to a voltage under full charge when balancing.

So using a brick charger with a bms instead of a hobby charger or power supply could increase the life of your battery.
So it's up to the individual users idea of whats more important. 
Maximum battery life or Maximum power and range. There's is always a trade off.

Let me clarify, charing to 41v instead of 42v is said to increase battery life substantially and honestly, the difference in range and power would be negligible.
```

---
## \#17 Posted by: MontPierre Posted at: 2017-08-20T17:29:15.875Z Reads: 207

```
Indeed I have bms 10s 80a. My brick charger ( 4 or 5A can't remember) charges up to 42V and then noting happens, some cells are undercharged and some overcharged and total is 42V. After I reach this 42V nothing happens, I left it for 45 min and no difference to individual cell voltage. What I'm currently doing is charging with brick charger to 40.9 ( quick charge ) or so and then finishing and balancing with hobby charger separately each lipo. As you said I'm happy with 41V rather than 42V.  Sometimes I would go to 41.5 on each cell. 

I'm not over the moon with bms being set up for 42V balancing start. Shame this value wasn't customisable. 

Balancing 0.2 volt of each lipo with 2A hobby charger isint a pain, takes 10 minutes each or so,  I just need to watch it so it doesn't go over voltage I aim for.

Bit tedious but manageable. Also I balance only every second charge, can't be bothered to do it every time. After non balanced charge I check each cell voltage. If they are more than 0.3 volt between highest and lowest I then balance manually with hobby charger to get it as close as I can.

I hope this makes sense, sorry for being so all over my post ;) I'm on mobile and at work haha
```

---
## \#18 Posted by: Jdubb121212 Posted at: 2017-08-20T17:42:19.456Z Reads: 202

```
Here is my current settings, see anything that needs addressed or corrected?.<img src="/uploads/db1493/original/3X/2/8/282a9cb54dd2aaeec608b3855c7bef23a4ff9b62.png" width="4" height="2"><img src="/uploads/db1493/original/3X/4/c/4c1902b9c74ebf4a51cf4931042ca7213e722595.png" width="507" height="238"><img src="/uploads/db1493/original/3X/1/1/112e1696e6146e5a50b15289430f77a25f028338.png" width="690" height="419"><img src="/uploads/db1493/original/3X/5/2/52de5e8937e3c944838535faa4bd10f2dfeaffb8.png" width="690" height="417"><img src="/uploads/db1493/original/3X/c/2/c2ff72c61f9d68810ea261ed005715a0a91a65d8.png" width="690" height="491">
```

---
## \#19 Posted by: MontPierre Posted at: 2017-08-20T17:44:26.902Z Reads: 193

```
Yeah, battery cut off ends I would put approx1-2v lower than the start. Otherwise you will damage cells with current settings.

Cut off start 35v
Cut off end 34V

Or even better 36v and 35v for longevity of your batteries
```

---
## \#20 Posted by: Namasaki Posted at: 2017-08-20T17:48:12.010Z Reads: 196

```
[quote="MontPierre, post:17, topic:31101"]
After I reach this 42V nothing happens, I left it for 45 min and no difference to individual cell voltage.
[/quote]


Are you charging with the bms E-switch turned on?
Are you leaving it on for 45min after charging?
```

---
## \#21 Posted by: MontPierre Posted at: 2017-08-20T17:51:32.713Z Reads: 184

```
@Namasaki E switch is on and left it for 45 min after it was 42V and charger LED went green.
```

---
## \#22 Posted by: Namasaki Posted at: 2017-08-20T17:54:17.526Z Reads: 183

```
can you post a specific wiring diagram of your bms and setup?
```

---
## \#23 Posted by: MontPierre Posted at: 2017-08-20T18:00:00.800Z Reads: 181

```
Same as here but 10s. I used this diagram to set mine up. 

Shall I leave it for longer? It quicker to do it with hobby charger ;) 

<img src="/uploads/db1493/original/3X/3/c/3c270d2dac8353fae7063a170cd368936c6170af.png" width="664" height="500">
```

---
## \#24 Posted by: MontPierre Posted at: 2017-08-20T18:01:38.849Z Reads: 160

```
I'll try it today again, one of my bms ( have two) is acting up lately.
```

---
## \#25 Posted by: Namasaki Posted at: 2017-08-20T18:09:17.891Z Reads: 158

```
I just pulled the lid off my battery and checked individual cells and found that the bms did not pull high cells down while trickle charging with power supply. And the bms did not balance cells down while it was turned off.
I've got my board on now to see if it trims them down.
```

---
## \#26 Posted by: darkkevind Posted at: 2017-08-20T18:11:24.927Z Reads: 157

```
Has no one noticed he's got 3.5v as cut off!?
```

---
## \#27 Posted by: MontPierre Posted at: 2017-08-20T18:13:34.035Z Reads: 155

```
I did 💪🏻 And advised better numbers
```

---
## \#28 Posted by: MontPierre Posted at: 2017-08-20T18:15:35.362Z Reads: 154

```
Ohhh let's see how long it will take.
```

---
## \#29 Posted by: scepterr Posted at: 2017-08-20T18:17:50.091Z Reads: 154

```
@Namasaki what BMS do you have ?
Most of I've seen only balance when charging and hit above 4.1-4.15
```

---
## \#30 Posted by: MontPierre Posted at: 2017-08-20T18:17:59.069Z Reads: 148

```
I wish in description of my charger there was trickle charge amperage 

36V 37V 42V 45V 5A Battery Charger For 10s 10x 3.6V/3.7V Lithium Li-ion Battery
https://banggood.app.link/r8c7ifyRLF
```

---
## \#31 Posted by: scepterr Posted at: 2017-08-20T18:19:28.194Z Reads: 148

```
Lithium isnt supposed to be trickle charged , it's CCCV. I've never seen a datasheet for a lithium cell that supports trickle/float charging
```

---
## \#32 Posted by: Namasaki Posted at: 2017-08-20T18:26:31.618Z Reads: 144

```
my power supply doesn't drop all the way to zero current. it only goes down to 50-40ma.
That could be because the Vescs and receiver are on while charging.
```

---
## \#33 Posted by: Namasaki Posted at: 2017-08-20T18:27:46.023Z Reads: 146

```
[quote="scepterr, post:29, topic:31101"]
what BMS do you have ?
[/quote]
 Bestech HCX-D223V1
```

---
## \#34 Posted by: scepterr Posted at: 2017-08-20T18:33:12.033Z Reads: 146

```
It's supposed to stop after a certain time, I don't remember the exact formula but I'm sure it's in the datasheet for your cells
```

---
## \#35 Posted by: Namasaki Posted at: 2017-08-20T19:04:20.324Z Reads: 146

```
**Results**

After leaving the E-switch on for apx 30 min voltages are as follows

Pack1
4.185
4.195
Pack2
4.198
4.192
Pack3
4.195
4.195
Pack4
4.195
4.195
Pack5
4.195
4.190
Rounded numbers
Pack1
4.19
4.20
Pack2
4.20
4.19
Pack3
4.20
4.20
Pack4
4.20
4.20
Pack5
4.20
4.19
I can't find the list now but some of the voltages where 4.204-4.206 before balancing.
I think these numbers are acceptable but I will let it balance for a while longer and check them again.
I have seen where even a hobby charger could not balance some packs perfectly.
```

---
## \#36 Posted by: MontPierre Posted at: 2017-08-20T19:11:31.227Z Reads: 136

```
This looks promising. Hmm I guess I need proper power supply as this one cuts out at 42V sharp. I guess you couldn't achieve balancing with your brick charger, right? 

How do boards like Boosted or Raptor work around this? Their BMS's must be set for lets say 41V balancing start and chargers to 42V cut off?
```

---
## \#37 Posted by: Namasaki Posted at: 2017-08-20T19:22:42.344Z Reads: 137

```
I'll have to test with my brick charger to see
```

---
## \#38 Posted by: MontPierre Posted at: 2017-08-20T19:24:18.839Z Reads: 137

```
I would be grateful if you can some time. I was hoping for plug and play set up and its fine apart of balancing part :/
```

---
## \#39 Posted by: Namasaki Posted at: 2017-08-20T19:44:02.195Z Reads: 143

```
after an additional 30 min with bms on the total pack voltage dropped from 41.90 to 41.85
After rechecking the cell voltages it seemed that there was no improvement to balance however after rounding the numbers there does appear to be a slight improvement.
Still, I would conclude that the original 30min balancing is adequate.
Note that differences in cell internal resistance will affect their ability to charge and discharge evenly
4.179
4.184
4.192
4.188
4.190
4.190
4.190
4.190
4.186
4.185
numbers rounded looks good.
pack 1
4.18
4.18
pack2
4.19
4.19
pack3
4.19
4.19
pack4
4.19
4.19
pack5
4.19
4.19

**Edit**
After rounding the numbers and seeing a  slight improvement to overall balancing after the additional 30 min of balancing.
This could imply that the bms is constantly balancing while on and not charging.  How great would that be?
```

---
## \#40 Posted by: Silverline Posted at: 2017-08-20T19:46:38.083Z Reads: 131

```
Hallo @Namasaki Nice info about the bestech 10s 80A BMS :-) Thanks

I`m building my 10s Trampa at the moment, with the same BMS. I know the E-switch have to be on when charging. But i don`t like that my focbox`s is powered on in several hours while charging. I notiched when no load on the BMS output, the voltage is nearly "vbat" level on the load pads. But do you think it`s okay, to ad a loopkey to the chain ? Between the bms and vesc`s. So while charging i could pull the loopkey, so the vesc`s is not powered while charging ?

And do i need to leave my charger connectet in 45min after end charged to ballance my cells, or is it okay to remove the charger after the LED turns green, and then let the E-switch being on for 45min ?
```

---
## \#41 Posted by: MontPierre Posted at: 2017-08-20T19:51:50.240Z Reads: 122

```
I still have some juice left if my pack, I will charge it with the brick on Tuesday and I will leave it to balance for 45 min or so. I wish I had cell checker so I could keep an eye on each cell while is charging and balancing. Let me know how it preforms balancing with your brick. I'm curious.
```

---
## \#42 Posted by: MontPierre Posted at: 2017-08-20T19:59:57.963Z Reads: 116

```
Shouldn't balancing only commence once individual cells reach 4.2V ? Above values are below 4.2.
```

---
## \#43 Posted by: Namasaki Posted at: 2017-08-20T20:01:39.289Z Reads: 121

```
[quote="MontPierre, post:41, topic:31101"]
I wish I had cell checker so I could keep an eye on each cell while is charging and balancing
[/quote]


That wouldn't work anyway because you have to turn the switch off and disconect the bms balance leads in order to plug in the cell checker.
```

---
## \#44 Posted by: Namasaki Posted at: 2017-08-20T20:02:22.038Z Reads: 116

```
[quote="MontPierre, post:42, topic:31101, full:true"]
Shouldn't balancing only commence once individual cells reach 4.2V ? Above values are below 4.2.
[/quote]


Please go back and read edit
```

---
## \#45 Posted by: MontPierre Posted at: 2017-08-20T20:04:39.262Z Reads: 110

```
[quote="Namasaki, post:43, topic:31101"]
That wouldn't work anyway because you have to turn the switch off and disconect the bms balance leads in order to plug in the cell checker.
[/quote]

I could use parallel balance leads, someone here recommended this kind of set up.
```

---
## \#46 Posted by: Namasaki Posted at: 2017-08-20T20:10:10.187Z Reads: 109

```
It would be fine to add a loop key as long as it downstream from the pos charge wire. So that the loop key doesn't disconnect the pos charge wire.
After the your charger goes green, turn it off and unplug it and leave the bms e-switch on for balancing.
```

---
## \#47 Posted by: Namasaki Posted at: 2017-08-20T20:10:53.965Z Reads: 109

```
[quote="MontPierre, post:45, topic:31101"]
I could use parallel balance leads, someone here recommended this kind of set up.
[/quote]


Ok, yes, that would work.
```

---
## \#48 Posted by: scepterr Posted at: 2017-08-20T20:14:04.526Z Reads: 112

```
@Namasaki it could just be the power draw of the BMS bringing them down, not any balancing function.
```

---
## \#49 Posted by: Namasaki Posted at: 2017-08-20T20:15:19.387Z Reads: 113

```
@scepterr 
After turning my bms on for the 3rd time, it brought the total pack voltage down to 41.8v
Some numbers rounded up and some rounded down.
4.18
4.18
4.19
4.19
4.19
4.19
4.19
4.19
4.18
4.18
```

---
## \#50 Posted by: Namasaki Posted at: 2017-08-20T20:18:41.815Z Reads: 108

```
[quote="scepterr, post:48, topic:31101"]
it could just be the power draw of the BMS bringing them down, not any balancing function.
[/quote]

Hard to say for sure.
Still even the original balancing is adequate in my opinion.

And this concludes my testing session for today.
```

---
## \#51 Posted by: Silverline Posted at: 2017-08-20T20:20:47.033Z Reads: 99

```
So you would not put the the loopkey in series between P- on the BMS, and - in the vescs ? You would take the positive Wire to the VESC after the charge wire
```

---
## \#52 Posted by: MontPierre Posted at: 2017-08-20T20:21:47.152Z Reads: 94

```
[quote="Namasaki, post:49, topic:31101"]
After turning my bms on for the 3rd time,
[/quote]


Just for clarification - power adapter wasn't on/connected, just board itself including Vesc?
```

---
## \#53 Posted by: Namasaki Posted at: 2017-08-20T20:26:23.233Z Reads: 88

```
[quote="Silverline, post:51, topic:31101, full:true"]
So you would not put the the loopkey in series between P- on the BMS, and - in the vescs ? You would take the positive Wire to the VESC after the charge wire
[/quote]


Oh your right, what was I thinking? Yes put it on the negative main between the P- and Vesc negative.
```

---
## \#54 Posted by: Namasaki Posted at: 2017-08-20T20:27:47.500Z Reads: 99

```
[quote="MontPierre, post:52, topic:31101"]
Just for clarification - power adapter wasn't on/connected, just board itself including Vesc?
[/quote]

If by power adapter you mean the charger then yes, it was off and disconnected.
```

---
## \#55 Posted by: Silverline Posted at: 2017-08-20T20:39:03.258Z Reads: 103

```
Thanks
I very appreciate your help.

I just did a test charge for the very first time, and all seems to be working fine. I could monitor all the cells voltage with my multimeter and temporary connectors. And they all seems to charge pretty equally 😃
Without any load on P- and plus from the battery, with the E-switch off. I measure close to bat voltage between plus on the battery and P-. I have not received my focboxes yet. Do you think it's gonna drain my battery over time ?
<img src="/uploads/db1493/original/3X/f/a/fa95d3a189fe2a40f1f871aaf96a888513df6eb1.jpg" width="690" height="388">
```

---
## \#56 Posted by: Jdubb121212 Posted at: 2017-08-20T20:43:31.961Z Reads: 102

```
I knew it was wrong thats why I posted pictures. I read/watched videos but got different numbers thats why I asked.
```

---
## \#57 Posted by: darkkevind Posted at: 2017-08-20T20:45:21.514Z Reads: 98

```
I wasn't mocking you mate, I was mocking everyone else for not seeing it or mentioning it to you ;)
```

---
## \#58 Posted by: Namasaki Posted at: 2017-08-20T20:46:44.332Z Reads: 97

```
[quote="Silverline, post:55, topic:31101"]
with the E-switch off. I measure close to bat voltage between plus on the battery and P-. I have not received my focboxes yet. Do you think it's gonna drain my battery over time ?
[/quote]


It's still reading full pack voltage because there is no load to pull it down. As long as the bms is off your battery should not drain down.
```

---
## \#59 Posted by: Silverline Posted at: 2017-08-20T21:00:05.807Z Reads: 96

```
Actually i dont think you are right. After 45min, the voltage has dropped 0.02v. I had an old car bulb laying arround, and now the voltage dropped to 0v. And the voltage seems stable for now.
```

---
## \#60 Posted by: rich Posted at: 2017-08-20T21:24:05.224Z Reads: 97

```
Sorry, fell asleep :sleeping:
[quote="MontPierre, post:8, topic:31101"]
I have 10S zippy 8000mah which are rated 5C current charge.  Does it mean I can have 40A batt regen? I'm currently on 25A or 30A.
[/quote]

True, you can increase your batt regen to 40A max, for safety maybe 35A. I have 10s1p Lipo 10Ah with 5c and my setting is 40A. 

@Jdubb121212 your Motor min setting is -60A, I would decrease it to -40A or less. Batt max 25A seems very safe, maybe you can increase it a bit if you need more power sometimes (if you don't push full throttle too often or climb epic hills). I guess your max cont. battery output is 40A, the cells get warm above 20A and hot when they reach 40A.
I'm not sure about your batt min setting, now it's -20A, theoretically your 12s2p can handle about 8A only but I've read several times that in real world the regen power isn't that high as in settings, so it could be OK.

My battery cut off settings are (Lipo and Li-ion):
Cut off start 35v
Cut off end 32V

I try to reach home above 36V but sometimes I go down to 32V. But anyway the time frame is very tiny from 35V to 32V, some blinks of an eye
```

---
## \#61 Posted by: Namasaki Posted at: 2017-08-20T23:23:29.681Z Reads: 89

```
[quote="Silverline, post:59, topic:31101, full:true"]
Actually i dont think you are right. After 45min, the voltage has dropped 0.02v. I had an old car bulb laying arround, and now the voltage dropped to 0v. And the voltage seems stable for now.
[/quote]

I'm not sure what your saying here
```

---
