# VESC FAQ &#124; Best Settings For Hub Motors

### Replies: 41 Views: 10639

## \#1 Posted by: elkick Posted at: 2015-09-17T06:57:07.717Z Reads: 545

```
For those who are using hub motors you need to adjust some values within BLDC tool (sensorless tab)  to start smoothly from a standstill according to Benjamin Vedder:

Minimum ERPM: 50
Minimum ERPM for integrator limit: 600

This is due to the fact that the hub motors won't give that much torque in general. Although I think it's more efficient to use as high voltage as possible. Made some first tests with the SPACE cell with 10s and pediglides V1 hub motors and I'm quite happy with the result. VESC's and motors are staying cool and reach has increased too.

This is a test with 7s (cracking nose at the end is due to the old wooden floor :smile: ):
https://youtu.be/G9nNrAn-ehw
```

---
## \#2 Posted by: onloop Posted at: 2015-09-17T08:17:28.685Z Reads: 507

```
I also suggest upping the startup boost.

<img src="/uploads/db1493/original/1X/9ed55279d89d9826b7d8966bb4f9cf0ae76ed22d.jpg" width="690" height="342">
```

---
## \#3 Posted by: onloop Posted at: 2015-10-07T12:17:18.700Z Reads: 480

```
Hub motors don't have the benefit of mechanical reduction, they don't spin at high rpm like with a satellite motor configuration, so they may end up having higher motor current peaks during start up and when climbing hills.

Therefore the potential problem with hub motors is over heating from high amp draw and heat losses. This could also permanently damage magnets if temps get over 100c for too long.

With hub motors having higher peak amp draws it could also damage some batteries or blow fuses if you have them installed in your system.

Therefore it is important to have the correct settings in the VESC to help protect the hub motors & batteries from too high currents.

This is a quote from Ben Vedder about managing battery & motor current:
> For the VESC you can configure different current limits for the motor and battery. You can for example set the motor current limit to 80A and battery current to 30A, which should work nicely with dual motors on a space cell. The motor current in each motor will then be able to reach 80A until you have reached 3/8 of the full speed. After that, the motor current will be more and more limited the faster you go.
```

---
## \#4 Posted by: kai Posted at: 2015-11-30T15:56:48.179Z Reads: 429

```
Does this also apply to carvon hub motors? The settings i mean?
```

---
## \#5 Posted by: elkick Posted at: 2015-12-01T19:23:43.389Z Reads: 421

```
Yes, I'm using both version of the CarvOn too with those values.
```

---
## \#6 Posted by: Tothpl Posted at: 2016-04-18T19:14:36.740Z Reads: 365

```
I am having a hell of a time setting up my new vesc to work with my carvon single hub. I can't seem to find any solid info on how to set the vesc up. I watched the vesc for dummies video and couldn't decipher much from it. The settings I have tried have only resulted in a top speed of 3mph and no torque. I need some help dumbing it down. I am clearly not as smart as all of you.
```

---
## \#7 Posted by: appelton Posted at: 2016-04-18T19:19:31.112Z Reads: 349

```
Check RUNPLAYBACK's topic on his Single Carvon build. He put his VESC's settings there.
```

---
## \#8 Posted by: Tothpl Posted at: 2016-04-18T19:24:40.795Z Reads: 347

```
Saw his as well. The one he has listed was foc. I used the settings he had for bldc but that was only for the one page. None of the other settings. I have used all of the setting he had listed on the other pages to no avail. It also doesn't explain why I have no power or torque. I shot him an email but am still waiting to hear back.
```

---
## \#9 Posted by: appelton Posted at: 2016-04-18T19:26:36.999Z Reads: 333

```
If you got your settings right please post them here. I'll be probably buying single carvon this summer so It would helpful.
Thanks!
```

---
## \#10 Posted by: mccloed Posted at: 2016-04-18T19:34:50.313Z Reads: 327

```
Need more info. How many volts are you running? RUNPLAYBACK is using a Space cell, which is 10s. I am running on 8s with the Carvon single.
```

---
## \#11 Posted by: Tothpl Posted at: 2016-04-18T19:43:38.127Z Reads: 321

```
I have a space cell as well. And as soon I get this thing working right, I'll post everything I did.
```

---
## \#12 Posted by: Tothpl Posted at: 2016-04-18T20:50:37.170Z Reads: 326

```
Just got back from a test ride after matching @RunPlayBack 's settings, as well as the settings at the top of this page. I have zero torque. It takes me ages to get up to speed.  When I am at full throttle its nowhere near as fast as it was with my old setup using the carvon and 6s lipos with a car esc. not to mention, the hub motor was hot to the touch. This is the entire purpose I bought all this stuff, to keep the motor running cool and last. So far it has none of the above. I feel like I spent a crap load of money only to go backwards. 

The things I dont understand about the vesc are the multitude of options. While that makes it a great muti-use product, it makes trying to understand it impossible without a masters in electrical engineering. Simple things like setting my throttle points are baffling me. I have full throttle in the first 1/8th of trigger pull, and braking doesn't start until 2/3rds trigger. I tried playing with PPM pulsewidths, but that got me no change.

Maybe I should scrap the vesc and invest in a huge ass car esc...
```

---
## \#13 Posted by: barajabali Posted at: 2016-04-18T21:23:08.937Z Reads: 297

```
What do u guys think of hub motors on TB esc? 120amp opto 12s.
```

---
## \#14 Posted by: laurnts Posted at: 2016-04-18T21:42:52.842Z Reads: 294

```
I am using hub motor as well. Show me your bldc tool screenshot @Tothpl. Lets see what can I help you.
```

---
## \#15 Posted by: Tothpl Posted at: 2016-04-18T21:52:56.214Z Reads: 310

```
<img src="/uploads/db1493/original/2X/d/d6aa3b564af9942d071091c901f41e4710179f36.png" width="690" height="370">
<img src="/uploads/db1493/original/2X/3/310ce5a241e897507db2e2f08ac324c6263bf5e3.png" width="690" height="370">
<img src="/uploads/db1493/original/2X/1/1f6e1cc840b97fdd5e5b4474dd410431bef4f6b5.png" width="690" height="371">
<img src="/uploads/db1493/original/2X/e/e6a510d439fdda476018e7f30909aaab2e226bf3.png" width="690" height="372">
<img src="/uploads/db1493/original/2X/a/a4969461e0b9402c9afbf6b29a5128340af1b9ef.png" width="690" height="370">

this is every page that I made a change to. I am using a gt2b in a bad wolf case as a controller. let me know what you see. I appreciate the help.
```

---
## \#16 Posted by: elkick Posted at: 2016-04-18T22:00:31.532Z Reads: 278

```
You need to klick apply after motor detection on the BLDC page. Else the detected values are not saved and so it won't work. And after that "write configuration".
```

---
## \#17 Posted by: Tothpl Posted at: 2016-04-18T22:20:45.570Z Reads: 282

```
I had figured out the "write configure" and had been doing that to all my changes. I will give the "apply" button a go as well. Other than that, these settings look good for my setup?
Again, thanks for the help.
```

---
## \#18 Posted by: chaka Posted at: 2016-04-18T22:52:41.623Z Reads: 283

```
Be careful messing around with the settings, you have some of them in really dangerous territory. Revert back to default configuration and raise you motor and battery max up to 80 amps. You may want to run motor detection again after reverting back to default.
```

---
## \#19 Posted by: laurnts Posted at: 2016-04-18T23:29:44.902Z Reads: 295

```
@Tothpl I think you need to recheck this points.

Scr1Shot1 > Voltage Limits
Battery Cutoff Start (according to your bat settings)
Battery Cutoff End (according to your bat settings)

ScrShot2 > Sensorless - Commutation Mode
Minimum ERPM: 50 (Correct)
Minimum ERPM for integrator limit: 600 (Correct)
Integrator Limit: 135 (Check your motor detection param, the value is 134.54)
BEMF Coupling: 850 (Check your motor detection param, the value is 849.56)

ScrShot4 > Current Control
Startup boost (BLDC Only): 0.040 (I use 0.050 but 0.040 is enough)

Please check and apply your motor detection parameter, please read carefully :slight_smile: take your time!
```

---
## \#20 Posted by: Tothpl Posted at: 2016-04-19T01:37:50.989Z Reads: 286

```
Again, thanks for all the help. I won't be able to get to it tonight. I'll report back tomorrow with an update.
```

---
## \#21 Posted by: RunPlayBack Posted at: 2016-04-19T04:34:13.386Z Reads: 279

```
Hey Peter here's my latest settings on the Carvon single hub + Space Cell, everything else I left at default. Also, how much do you weigh? Are you kick pushing on startup or standing still?

Motor Max: 70.00 A
Motor Min: -60.00 A
Bat Max: 30.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A

Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V

Startup Boost: 0.040
```

---
## \#22 Posted by: Tothpl Posted at: 2016-04-19T19:27:35.321Z Reads: 271

```
I appreciate you posting your settings, they are a huge help. Are you running BLDC or FOC? Hows the start up torque? I always kick push a few times to get going before rolling the power on. I'm 6'4" 210lbs. I am comparing this all to the 6s lipos I had running on this hub before. On lipos, It felt just like the belt drive I built while waiting for parts for this.
```

---
## \#23 Posted by: laurnts Posted at: 2016-04-19T20:56:57.990Z Reads: 265

```
I am running sensorless BLDC mode as my hub doesn't seems to work with FOC.
I will try sensored BLDC and sensored FOC when I have my JST arrived.

The startup torque for me they are very similar belt and hub with belt slightly on top of hub motor especially starting on hills. On flat ground they are both responsive and agressive. I also do 1 kick push most of the time to get into balance, it's more natural to do just 1 push.

I am running all of my belt drive and hub drive with 6s lipo 30C 8000mah and 6s lipo 25c 10000mah. Both discharge are quite similar 240A - 250A. Very punchy!
```

---
## \#24 Posted by: Tothpl Posted at: 2016-04-19T21:31:28.314Z Reads: 262

```
I just got back from a speed run. The results are below. That is still within my comfort zone, but I feel I am maxing out the system due to my size. Also of note, I am seriously worried about the hub motor due to heat. I thought all these components would mitigate the heat. Another point of complaint, the space cell battery isnt lasting as long as I had expected. @onloop advertises 1.5hrs of playtime using a dual motor setup. From a fresh charge, I rode my single carvon for 1x 10min run, and, 1x 5min run. Both runs included plenty of full throttle. It now sits at 57%.
<img src="/uploads/db1493/original/2X/a/aa7b18a62d4c313195034cec159ad8d0d7568b70.PNG" width="281" height="500">

That all being said, I am still trying to figure out what is normal compared to my belt drive, lipo setup. The carvon hub still feels way less torquey than before. although with everyones help on the settings, I have noticed an definite increase in speed. I now want to make sure that they are operating within safe parameters of the hub to keep it from melting itself.
As far as the speed goes, Its not quite at the scary limit for me. I need to know I have that power, even though I cruise at 17-20mph. I like to live a little! I had that with the lipo setup, but I cooked the hub motor using 6s and too much full throttle. Theoretically, since I increased the voltage, shouldn't my available power increase as well?
```

---
## \#25 Posted by: Tothpl Posted at: 2016-04-19T21:48:58.301Z Reads: 239

```
@laurnts While changing settings prior to the test run, I noticed that every time I ran motor detection, a different value for Integrator Limit and BEMF Coupling would appear. It varied by about 50pts. I ended up just typing in one of the values and calling it a day. I dont really know what that does, and dont understand why it varies every time if I am to input it into a block?
```

---
## \#26 Posted by: laurnts Posted at: 2016-04-19T21:51:14.803Z Reads: 239

```
It's all about magnets and magnetic fields, so value might varies slightly for every detection (also depends on where does the motor starting position). Thats why Vedder sometimes does multiple detection to find the average value and if the value he have is correct. I also just round it to the nearest value.
```

---
## \#27 Posted by: Tothpl Posted at: 2016-04-19T21:53:30.708Z Reads: 233

```
As in the 135 and 850. That makes a little more sense now, thank you!
```

---
## \#28 Posted by: RunPlayBack Posted at: 2016-04-20T13:38:34.652Z Reads: 245

```
I'm running FOC at the moment because of the stealth. I typically don't have a need to hit top speeds when I'm commuting through downtown. Yes your height and weight are pushing the limits of the single hub which is why it feels less torquey. I have both a single and dual, both using a space cell, and I think if you want that high torque from the hubs, dual is the way to go. For me, I approach my single as a cruiser/coasting board, something that is easily transportable and I can use to get through the city as stealthy as possible - like a hybrid of a natural longboard and an electric. The dual is longer, bigger and heavier, but when I want to power through distances, it's what I like to use.
```

---
## \#29 Posted by: Tothpl Posted at: 2016-04-20T21:13:20.132Z Reads: 264

```
I just swapped over to all FOC settings. Just to be sure, I clicked the FOC button on the motor tab, as well as 'detect settings, apply, and write config.' on the FOC tab. those were the only settings I changed. I left all the others the same. After a quick test run, I topped out at 27mph even. It sounded ever so slightly more quiet, and just barely noticeably slower on throttling up. which would be evident in the slower top speed. 
I can't help but compare this to the mass amounts of torque I had when running this hub with 6s Lipos and a car esc. It was faster and had waaay more punch. Then again, I burned it out. (Which I cant say enough good things about Carvon's customer service!!) I am going to assume that the lipo setup was doomed to fail regardless of the results. That this is the way it should feel operating within the hubs safety parameters?
<img src="/uploads/db1493/original/2X/b/bab86865b01c06dfed0165277a4b8c0216e718ca.png" width="690" height="381">
```

---
## \#30 Posted by: davey8 Posted at: 2016-10-14T20:59:59.354Z Reads: 185

```
Should I do these ERPM settings with my VESCs on an R-spec motor to get a standing start as well?
```

---
## \#31 Posted by: leroy Posted at: 2016-12-31T02:41:56.413Z Reads: 159

```
I think it would help others a lot if folks posted their xml config files, rather than just one or two settings. 

I myself would love to see a full config on a 3000w hub motor with a 6s battery and vesc,
 I can't get past about 5 mph, 
and I am not that fat.... 

these pants just make me look fat. :)
```

---
## \#33 Posted by: leroy Posted at: 2016-12-31T02:49:11.279Z Reads: 162

```
http://stream0.net/5mph.xml

taking my own advice, here is my 5mph config 

http://stream0.net/5mph.xml
```

---
## \#34 Posted by: yaca Posted at: 2017-01-05T20:05:38.391Z Reads: 156

```
In my opinion it's easier to have a look on screenshots of bldc-tool as on xml files.
```

---
## \#35 Posted by: Ackmaniac Posted at: 2017-01-05T20:34:06.143Z Reads: 154

```
I think you can't get past 5 mph because of the kv of your motor. Which motor is it?
```

---
## \#36 Posted by: Hummie Posted at: 2017-01-05T21:09:02.286Z Reads: 151

```
It shouldn't matter if u use lipo or li-ion and I guess the old esc u used had a higher amp limit than the vesc. Likely has unknown limit.  U can still burn the motor out with the vesc if u over cook
```

---
## \#37 Posted by: leroy Posted at: 2017-01-05T21:41:21.788Z Reads: 148

```
Yeah, it is easier to read as a screenshot, good point.

However,  I do want to import settings using an xml, 
because I am new to the tool and don't want to accidentally miss a setting.
```

---
## \#38 Posted by: leroy Posted at: 2017-01-05T21:45:30.653Z Reads: 150

```
I have a 3000w hub motor with a 90kv, using a 6s battery, 
when I first hooked it to the vesc, it would not even push the board by itself, I got some help and then it started working a bit better, but I would like some more speed.
I have a 10s coming in this afternoon, and I will see if that helps.
```

---
## \#39 Posted by: leroy Posted at: 2017-01-05T21:51:25.080Z Reads: 150

```
If you have any advice, I am listening. 
I don't know what I'm doing with the vesc, 
or any esc for that matter. 

I'm sure I am making plenty of mistakes, 
point them out to me , please.
```

---
## \#40 Posted by: Ackmaniac Posted at: 2017-01-05T22:13:15.340Z Reads: 150

```
The settings seem to be OK. Which remote are you using and did you adjust the settings for the remote? And if you don't run with sensors then you always should give it a little push at the startup.

And Screenshots of the settings would be better. I can read 90% of the values by heart but the most others don't know what all the keys stand for.
```

---
## \#41 Posted by: leroy Posted at: 2017-01-06T21:58:29.666Z Reads: 137

```
I just plugged a 10s battery, and it's much much much better. 

I am using a benchwheel remote, 
I didn't even know you could adjust those. 
How do you adjust a remote? 

I am jazzed up now :)
```

---
## \#42 Posted by: Ackmaniac Posted at: 2017-01-06T22:39:28.819Z Reads: 135

```
Via these settings.

<img src="/uploads/db1493/original/3X/3/0/30808cf9e234835cf789fbdccea0281e56203acc.png" width="690" height="421">
```

---
