# 4wd evo build 12s6p

### Replies: 64 Views: 2770

## \#1 Posted by: Chase Posted at: 2018-05-15T04:02:18.052Z Reads: 487

```
So I’m building my V4 evo (RC version of course since XL is MIA). Here are my initial pics. I’ll end up putting in my 4p battery once it’s fixed. I just wanted to ask a quick question about my first focbox configuration. I posted it elsewhere but I figured this would be a better place.
Can anyone possibly answer this question regarding focbox configuration. When I do the app setup for the maytech remote setup, I do full throttle to enter maximum pulse. Then I do maximum brake to enter minimum pulse. When I go enable it to enable current reverse with brake the motor immediately starts up as if though I’m pushing the throttle. The only way I could get the motor not to spin without pushing on the remote was to set the minimum pulse to the number shows without pushing the throttle at all. So to reiterate max pulse is full throttle forward, minimum is not pushing throttle whatsoever. Shouldn’t I be able to set minimum to the full brake pulse without it automatically running when I enable it?
![image|375x500](upload://4Bkm2R0tms3MNs73VANsVxBYjHr.jpeg)![image|375x500](upload://nURHqhFhxBceJafA3SuspR05jZg.jpeg)

I ordered the XL as well back at the beginning of December, but if it doesn’t show progress of being released I’ll likely look into other options and sell my place in line. 

Any help is appreciated
```

---
## \#2 Posted by: Eboosted Posted at: 2018-05-15T05:28:25.256Z Reads: 437

```
1. Select no app and write
2. Turn on the remote
3. Click on the reset ppm button
4. Pull throttle to the max and brake to the max
5. Click apply
6. Select current no reverse with brake
7. Click write to ESC
```

---
## \#3 Posted by: Chase Posted at: 2018-05-15T05:39:08.636Z Reads: 420

```
Thanks. That’s actually the process I had been following. I played around with the minimum pulse and it turns out if you go back all the way with the throttle it passes the point where the display hit 0%. Releasing a little allowed me to see the exact pulse it hit zero. It foxed the issue
```

---
## \#4 Posted by: b264 Posted at: 2018-05-15T05:40:33.586Z Reads: 399

```
You can't sell your place in line.
```

---
## \#5 Posted by: Chase Posted at: 2018-05-15T05:41:22.511Z Reads: 385

```
Meant I would receive and send to the buyer
```

---
## \#6 Posted by: Eboosted Posted at: 2018-05-15T06:04:23.590Z Reads: 379

```
[quote="Chase, post:3, topic:55509, full:true"]
Thanks. That’s actually the process I had been following. I played around with the minimum pulse and it turns out if you go back all the way with the throttle it passes the point where the display hit 0%. Releasing a little allowed me to see the exact pulse it hit zero. It foxed the issue
[/quote]

That's impossible are you ussing the Wizard to set up the PPM?
```

---
## \#7 Posted by: Chase Posted at: 2018-05-15T06:16:20.068Z Reads: 353

```
I’m using the download from enertion
```

---
## \#8 Posted by: Eboosted Posted at: 2018-05-15T06:47:52.584Z Reads: 358

```
Install @Ackmaniac and forget about all the issues, it's way better
```

---
## \#9 Posted by: Chase Posted at: 2018-05-15T07:06:24.445Z Reads: 366

```
Thanks will do
```

---
## \#10 Posted by: Chase Posted at: 2018-05-27T01:48:27.352Z Reads: 352

```
![image|666x500](upload://i6FwtytOGEtoWkCfFV9ljpXnpgd.jpeg)![image|666x500](upload://Fna67WQl7XWUw0IKzPUZUe4olD.jpeg)
```

---
## \#11 Posted by: mikenyc Posted at: 2018-05-27T03:21:33.416Z Reads: 337

```
Hey what power button did you go with on that enclosure?
```

---
## \#12 Posted by: Chase Posted at: 2018-05-27T03:57:02.236Z Reads: 338

```
Just a typical switch.

![image|281x499](upload://rKGi8YxjkkDP58T6K6ru7lUiRDe.jpg)
```

---
## \#13 Posted by: mikenyc Posted at: 2018-05-27T12:22:24.563Z Reads: 323

```
Interesting placement. @Eboosted can you recommend a switch that will fit on the side near the electronics typically go?
```

---
## \#14 Posted by: Eboosted Posted at: 2018-05-27T18:18:32.733Z Reads: 320

```
16mm spdf latching switch, I think Mouser has them in stock. But I can't look right now as I'm travelling to DFW via México City with a big package

![15274451743619168530715137252983|374x500](upload://679lV0y2pBySaUdj62SRwjQdPrp.jpg)
```

---
## \#15 Posted by: Chase Posted at: 2018-06-03T23:17:33.728Z Reads: 310

```
Since this is my first carvon I wanted to check... is it supposed to sound like this? See video. I know I can make it quiet by changing the settings to foc. How much will this reduce the top speed? Just sounds so different then my other boards.

https://youtu.be/RRxOKl4rYns
```

---
## \#16 Posted by: deucesdown Posted at: 2018-06-04T00:50:58.895Z Reads: 302

```
I remember my v2.5 sounding like a tie fighter, loved it!
```

---
## \#17 Posted by: chris.hunt Posted at: 2018-06-04T01:05:39.723Z Reads: 296

```
from riding @Mikenopolis carvon board it sounds about right but thats just me
```

---
## \#18 Posted by: Deckoz Posted at: 2018-06-04T01:20:45.682Z Reads: 291

```
Lol that is an odd sounding board lol

Sounds like cards stuck in a wheel spoke even when you are coasting... That doesn't sound right to me lol especially for something with no drivetrain...
```

---
## \#19 Posted by: Chase Posted at: 2018-06-04T01:35:08.055Z Reads: 286

```
I think the reason it makes noise when I am coasting is related to the urethane that they started wrapping the motor cans in. I’m more wondering about the noise when I throttle and brake. I’ve seen a few videos but it’s just hard to hear on them.
```

---
## \#20 Posted by: Mikenopolis Posted at: 2018-06-04T01:38:08.546Z Reads: 282

```
I think you are thinking of the the dual 6355 BLDC Raptor. My CarvOn V4 Raptor is FOC and really quiet
```

---
## \#21 Posted by: deucesdown Posted at: 2018-06-04T03:05:11.367Z Reads: 268

```
Try foc v2.5 were silent on foc. See if it's the urethane sleeve.

I liked the bldc noise to warn pedestrians.
```

---
## \#22 Posted by: Chase Posted at: 2018-06-06T02:17:06.122Z Reads: 257

```
Guess I just didn’t realize how loud the BDLC is on these motors. It’s in foc now and nice and quiet.
```

---
## \#23 Posted by: Chase Posted at: 2018-08-02T01:14:32.198Z Reads: 251

```
Getting ready for it’s upgrade to 4wd. Gotta love a black board.

![image|666x500](upload://ZBwGkfM4TiAYAFGD7u4FSWdTOB.jpeg)
```

---
## \#24 Posted by: chris.hunt Posted at: 2018-08-02T06:53:12.784Z Reads: 241

```
is that the big evo?
```

---
## \#25 Posted by: Chase Posted at: 2018-08-02T06:59:01.147Z Reads: 239

```
Yes
10char
```

---
## \#26 Posted by: chris.hunt Posted at: 2018-08-02T07:10:34.083Z Reads: 233

```
nice what a beauty did you order an enclosure from alan?
```

---
## \#27 Posted by: Chase Posted at: 2018-08-02T07:23:22.561Z Reads: 237

```
Thanks! Yes, it had the regular sized eboosted enclosure, by now I have to upgrade to the double layer to fit the 12S6P I’m putting together.
```

---
## \#28 Posted by: Chase Posted at: 2018-08-02T23:33:17.131Z Reads: 243

```
I asked this on the noob questions but it got drown out before getting an answer. I’m building a 12s6p from 30q cells and if possible I want a bms that can discharge. I’ve seen a similar thread, but my question is different. 

I’ve seen a few videos where people stack the bms on top of the cells. The high discharge bms from supower have big metal plates on the bottom.

 Will stacking these high discharge bms on cells heat them too much?

 Their just too wide to fit in an enclosure otherwise.
```

---
## \#29 Posted by: Mikenopolis Posted at: 2018-08-02T23:49:12.952Z Reads: 244

```
No real answer since I don’t know, but I was curious about the heat so I had the board on while charging. This board was dead cold in the office before I plugged it in. The temperature between the battery (bottom) and BMS (middle) is 10 degrees Fahrenheit 

![image|406x500](upload://e2ov7LPWzdipAJmEPeI0F5m9Ixn.jpeg)
```

---
## \#30 Posted by: Chase Posted at: 2018-08-03T01:29:58.178Z Reads: 236

```
To me that says no it isn’t a good idea to stack a high discharge bms on top of cells. Looks like a charge only is the only option unless anyone knows of a smaller that can handle at least 100A
```

---
## \#31 Posted by: mikenyc Posted at: 2018-08-03T22:27:50.112Z Reads: 226

```
what are the dimensions of the metal plate?
```

---
## \#32 Posted by: Chase Posted at: 2018-08-03T23:03:52.025Z Reads: 232

```
With the radiating plate on its Dimension: 200mm * 110mm * 20mm (L*W*T) - with Radiating Board
Im assuming without it would be like all the lower Amp ones at Size: 129mm * 53mm if the radiating board was removed.

https://www.ebay.com/i/322366720064?rt=nc&_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D2%26asc%3D20160908110712%26meid%3Dfe7168388c37496f807edc7d45369f6c%26pid%3D100677%26rk%3D8%26rkt%3D30%26sd%3D222353573658%26itm%3D322366720064
```

---
## \#33 Posted by: mikenyc Posted at: 2018-08-03T23:06:12.253Z Reads: 220

```
Interesting. Did you already order an enclosure?
```

---
## \#34 Posted by: Chase Posted at: 2018-08-03T23:11:32.172Z Reads: 220

```
Yeah I ordered a DS eboosted. I got a small 60mm charge only bms in the meantime but if I find a small enough that can handle a 4wd discharge from a 6p Ill swap it out
```

---
## \#35 Posted by: Chase Posted at: 2018-08-06T22:19:46.622Z Reads: 213

```
In the process of building my first 4wd from this deck. Looks like the safest method is to split the receiver signal over the 4 vesc or simply have 4 receivers. I really wanted to use the Bluetooth app to be able to control my vesc setting from my phone. Is the only way around this is to  buy 4 bluetooth receivers and then have to switch connections each time to change the settings? Or is there a different way around this without going the canbus route?
```

---
## \#36 Posted by: mikenyc Posted at: 2018-08-06T22:27:47.268Z Reads: 201

```
i made a canbus harness by making 2 Y-Cables. You can still use the bluetooth app to update your settings. @rpasichnyk's METR module works really well. And you only need 1 module
```

---
## \#37 Posted by: Chase Posted at: 2018-08-06T22:29:31.765Z Reads: 204

```
Yea and then set 3 as slaves? I thought I read somewhere that you can destroy the slave vescs if one gets disconnected?
```

---
## \#38 Posted by: mikenyc Posted at: 2018-08-06T22:56:25.474Z Reads: 202

```
yeah, if the power gets disconnected, you'll have a big issue, but if your parallel connectors are secure, you shouldn't run into problems.
```

---
## \#39 Posted by: Chase Posted at: 2018-08-06T23:20:28.459Z Reads: 207

```
I guess that’s the trade off I’ll have to take. Disconnection security with the split remote or the ability to change settings via Bluetooth for a can setup
```

---
## \#40 Posted by: Chase Posted at: 2018-09-10T00:15:09.849Z Reads: 221

```
Built my 12s6p battery with Bluetooth on my way to upgrading to 4wd.

![image|281x499](upload://W4KLzrWKLmRSPn5SGdOp0ImrZv.jpg)![image|666x500](upload://js4tOdKuHoItjcuHA2oofLgTvhq.jpeg)
```

---
## \#41 Posted by: trancejunkiexxl Posted at: 2018-09-10T00:28:26.720Z Reads: 200

```
Nice man, carefull with those speed controllers 😉
```

---
## \#42 Posted by: Chase Posted at: 2018-09-10T18:32:45.075Z Reads: 200

```
Not sure what the issue is but it took like 6 hours just to get to 50% with my 1.5A charger. Could this be the bms settings? I noticed that its trying to balance after 3.4V so it may be slowed because its trying to balance too early? This is my first time having a bms that can be adjusted in so many ways.
```

---
## \#43 Posted by: Chase Posted at: 2018-09-10T21:54:09.730Z Reads: 194

```
Figured it out. It was a problem with the app. I used the one that was made for it for Android and it showed the accurate values. It’s weord because I tried the iOS app right before and it was way off valtage. Then when I tried it again after using the android app, it all the sudden started showing the correct values.

Edit: neither of the apps are accurate when the pack is charging
```

---
## \#44 Posted by: Chase Posted at: 2018-09-12T05:41:41.118Z Reads: 202

```
Switch wired up. Now just have to mount the enclosure and put in the vescs

![image|375x500](upload://nDXJWolRRJZVfHKITlZQN20XxsK.jpeg)
```

---
## \#45 Posted by: Chase Posted at: 2018-09-17T06:25:10.386Z Reads: 191

```
It’s got a gut but I’m sure it’ll fly. Just needs to be grip taped and then it’s 4wd time

![image|690x220](upload://7OlGhUvF8oIbKynZO4LGyd8sQOF.jpeg)

If a mod sees this post please change the thread title to something more appropriate like 4wd evo build.
```

---
## \#46 Posted by: Chase Posted at: 2018-09-23T00:05:00.756Z Reads: 185

```
First impressions:

Has the torque and brakes that I missed with the 2wd v4. 

Fast as hell. Couldn’t pull the throttle down much at all. Daytime on a Saturday here in San Francisco with too much foot and street traffic so come nightfall I plan on doing some faster runs.

Double stacked batteries on these drop down evo decks require enclosures that you don’t mind scratching up. Even the slightest bump can do some damage. I’ll be buying some six shooters soon for cross city trips. The 107mm will have to be reserved for mostly speed trials on flat roads.
```

---
## \#47 Posted by: Riako Posted at: 2018-10-13T14:57:22.495Z Reads: 170

```
Would love to try this freaking badass killer formula board ! Plus it is an absolute beauty/beast man !!!
Enjoy, show us more pic and vid pleeaaase :P
```

---
## \#48 Posted by: Skunk Posted at: 2018-10-13T15:08:35.604Z Reads: 172

```
Yeah more updates on this. 
I wanna see it go.
```

---
## \#49 Posted by: Chase Posted at: 2018-10-14T02:41:33.829Z Reads: 172

```
Thank you for your comments. I had taken the enclosure off to smooth some of the paint out and add a clear coat and accidentally blew the antispark switch carelessly reassembling it. It’s a fast beast that’s for sure. I’ll make a nice update in a few days when I get it back up and running. I have some six shooters so to test out as well.

![image|375x500](upload://eVH54PULT8wDjyaAOcgV3icjIiP.jpeg)
```

---
## \#50 Posted by: Jake2k17 Posted at: 2018-10-14T03:42:30.627Z Reads: 162

```
Looks good bro! Why don’t you add some risers on there to give it some more space with 107s? Overall it’s FOCing sweet, 4wd might be be sexiest builds on the forum
```

---
## \#51 Posted by: trancejunkiexxl Posted at: 2018-10-14T15:17:01.681Z Reads: 157

```
amazing board man. what motor/batt settings you running? im using 40/30. feels like plenty of power so i havent changed anything yet.. :smiley: although i went conservative as im stuck on 12s4p atm..:unamused:
```

---
## \#52 Posted by: Chase Posted at: 2018-11-10T07:51:11.869Z Reads: 153

```
Got so busy with work that I’m just now getting this repainted/gripped and ready to go. Unless I’m too hungover, I plan to make the group ride tomorrow to finally make a long trip with it. 

![image|666x500](upload://xpAkYUUganq2HtJqxANarEsnfXL.jpeg)
```

---
## \#53 Posted by: Chase Posted at: 2019-01-26T00:13:43.400Z Reads: 136

```
Just bought another AWD vehicle to go with it.

![image|375x500](upload://6mQQ01gJuQjJJJwAkaM6BHU6yjW.jpeg)
```

---
## \#54 Posted by: Mobutusan Posted at: 2019-01-26T02:54:11.438Z Reads: 122

```
Dope! Details? Still loving my 04 WRX wagon that I've modded just about everything I can get my hands on. I would love to make it electric one day though. :money_mouth_face:
```

---
## \#55 Posted by: Chase Posted at: 2019-01-26T04:04:32.932Z Reads: 120

```
Thanks. It’s a 19 WRX. I wish I could have afforded the STI but it’s almost 40K! This one is still pretty quick though. 2.0L Turbo charged AWD with 268 HP.
```

---
## \#56 Posted by: Mobutusan Posted at: 2019-01-26T05:11:50.816Z Reads: 120

```
Nice. I didn't know the WRX has a 2.0L again. Sounds like a pretty good powerplant compared to the 2.0L I have. Having the 6 speed and 2.5L are the only things I really wish I had from the STI. But mine is paid off, and still so fun to drive that I can't bring myself to get even a newer used one and have car payments again. I still drool over the new ones though. Are you gonna mod it at all? Not sure how these new models respond to just an exhaust upgrade and retune, but in my experience, it's totally worth it for the improved throttle/turbo response and daily driveability. Love these cars.
```

---
## \#57 Posted by: Chase Posted at: 2019-01-26T05:29:01.044Z Reads: 115

```
This one is actually a 6 speed. I was actually just reading about some aftermarket options. An article claims I can add 17 hp and 21 pounds of torque with the right air intake. A decent exhaust might help a little. I used to have a nice Borla on my 06 GTO back in the day. It was a fun ride too but I raced a STI once and was left in the dust. It’s what made me want one so much.
```

---
## \#58 Posted by: Mobutusan Posted at: 2019-01-26T06:45:10.678Z Reads: 110

```
Very cool. I don't know how things have changed over the years, but on my car, smoothing out and opening up the exhaust a bit, e.g. uppipe, downpipe w/hi-flow cat, catback, and a custom retune made the biggest difference. Not just adding a decent bump in power, but maybe more importantly, improving throttle response and reducing turbo lag for daily driving.

I won't derail your thread any further, but before stumbling into this bottomless ESk8 hole, modding my WRX and Rallycross racing was my obsession. So, I have a very soft spot for these cars.

BTW, very nice Evo build. Looks like tons of fun.
```

---
## \#59 Posted by: Chase Posted at: 2019-02-24T03:36:34.023Z Reads: 98

```
Damn. The board sat idle for a month while I wait on this drive to be dealt with.

The battery is almost dead. It was fully charged last time it was on. Cells were at just under 3.1. All balanced. I think this pricey ass bms drained all of them for some reason. I noticed that it always says it’s balancing in the app.
```

---
## \#60 Posted by: Deckoz Posted at: 2019-02-24T03:57:30.654Z Reads: 93

```
I've left my 13s5p for weeks, with no change in voltage. Its most definitely your bms or switch.

If its a programmable bms you should set it to only kick off a balance above 4.15-4.17/cell. Balancing all the time is bad.
```

---
## \#61 Posted by: Chase Posted at: 2019-02-24T04:29:14.340Z Reads: 92

```
I thought I had it set that way, but for some reason the it always says it’s balancing the cells.

![image|281x499](upload://lpBAiaydMMZNv0qOpDZW5lQMARX.png) 

![image|281x499](upload://d90KnbURzjxnAe7hZs7gs1kTZdn.png)
```

---
## \#62 Posted by: youseekcota Posted at: 2019-02-24T05:07:35.895Z Reads: 86

```
Would love more comments about coordinating all the vescs. Having four masters, or wiring all the CANs together don't look like good choices, and having multiple receivers seems like just adding more that can go wrong. What do you think?
```

---
## \#63 Posted by: Chase Posted at: 2019-02-26T19:28:03.855Z Reads: 83

```
Well damn it looks like I’m gonna have to change it to a different bms. I can’t get this one to stop balancing.
```

---
## \#64 Posted by: Chase Posted at: 2019-08-23T21:00:32.149Z Reads: 59

```
God so sick about this car(19 wrx). Has less than 3000miles on in and it’s been sitting for months only start for the battery. Just drove it 30 miles. The clutch appears to be going out. Bad oil burning type smell and then it stalled out. Was right around the corner so I took it home.

Been driving stick for 15 years. Never stalled, scratched a gear or had any problems. I’m seriously the guy who always thinks about avoiding riding the clutch.The clutch warranty is 36k or three years but they add in only for wear and tear. When I called they said they rarely claim clutch under warranty since “I likely didn’t know how to drive a stick”. 

Completely shocked, like Im so careful driving stick and always getting compliments
```

---
