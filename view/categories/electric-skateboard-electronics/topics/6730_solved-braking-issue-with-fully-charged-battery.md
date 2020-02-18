# Solved! Braking issue with fully charged battery

### Replies: 127 Views: 10273

## \#1 Posted by: Mrmoonlight Posted at: 2016-07-27T23:12:24.240Z Reads: 556

```
So I got my board all set up and everything seems to be working fine except that my brakes don't work when my battery is fully charged. Once it's down to around 90%, everything works fine. 

If I put on my brakes at 100% and my batteries are full, nothing happens. If I put on my brakes at 50% and I'm going slow, I get some braking. Once my battery is at 90% the issue is gone. Any ideas on where to start would be of much appreciated.

I'm running a Space Cell 3, Carvon Hub, VESC, Enertion Remote.
```

---
## \#2 Posted by: mason Posted at: 2016-07-27T23:22:22.947Z Reads: 521

```
Your problem is regenerative braking and overcharge protection.
Your VESC is preventing the battery from being overcharged, and in order to do that it needs to disable breaks.
```

---
## \#3 Posted by: bbq870 Posted at: 2016-07-27T23:30:42.715Z Reads: 509

```
how did Mellow solve that problem?
with their boards you can break even with full batteries.
```

---
## \#4 Posted by: Mrmoonlight Posted at: 2016-07-27T23:31:20.450Z Reads: 498

```
Makes sense. Is there a setting on my VESC I can change to adjust this?
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-27T23:31:39.824Z Reads: 489

```
What's your battery regen set at?
```

---
## \#6 Posted by: Mrmoonlight Posted at: 2016-07-27T23:37:40.205Z Reads: 489

```
Here's a screen shot of my settings. Batt min is at -12A

<img src="/uploads/db1493/original/2X/d/d369dfc41494c85b9014188599cf1ac8c53a4901.png" width="690" height="363">
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-27T23:47:42.076Z Reads: 475

```
Could be a variety of things, but it does sound like what @link5505 mentioned. Though, I wouldn't imagine you need to go all the way to 90% to stop it from happening. Another possibility is that you're getting voltage spikes during regen that bring it over the max. Anyway you can plug it into your laptop and do active sampling to see if you get a fault code? You Might have to hold the brake down while turning the wheel during full charge to see it.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-07-28T00:10:52.982Z Reads: 462

```
It sound like some kind of Over Voltage, probably a fault from the BMS. Are the Brake working without any load ?

Edit : Also are you in bldc mode or foc ?
```

---
## \#9 Posted by: Mrmoonlight Posted at: 2016-07-28T00:15:08.905Z Reads: 463

```
Same thing happens in both BLDC and FOC. Brakes work fine once the battery is at 90%. Charging it up now. Gonna see if I can get a sample
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-07-28T00:29:09.753Z Reads: 454

```
Also, if can read the fault* in the BLDC Tool it would be great.
```

---
## \#11 Posted by: treenutter Posted at: 2016-07-28T00:55:38.944Z Reads: 448

```
[quote="link5505, post:2, topic:6730"]
Your problem is regenerative braking and overcharge protection.
[/quote]

I agree with @link5505 this is a common story with VESC.
 
[quote="bbq870, post:3, topic:6730"]
how did Mellow solve that problem?
[/quote]

They use a dual-drive system. They describe it (albeit in a very basic way) here:

http://www.mellowboards.com/faq/

The solution for most of us with single drive, is to reduce braking force in BLDC. Then less energy is created when regen is happening, so you're less likely to trip your VESC's cutoff threshold. You could charge the battery just below max. The problem with this is it is at max charge, for most BMSs, where balancing happens.

When I know my battery is full, I avoid heavy extended braking for the first few minutes. That's how I solve it personally, along with slightly reduced braking force settings.

@Mrmoonlight it sounds like you're regen settings are not configured well for you setup, thus the sensitivity you're experiencing. @onloop wrote a good post about it here, try manipulating the settings according to this post:

http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#12 Posted by: Mrmoonlight Posted at: 2016-07-28T01:02:05.275Z Reads: 423

```
Got an over voltage fault when I brake. I'm able to get it to brake when I push the throttle half way for a sec, then apply 50% brakes.<img src="/uploads/db1493/original/2X/e/e01bfe7bc4ffd48090ff97ae22ddaf4449f41ea4.png" width="690" height="383">
```

---
## \#13 Posted by: Jinra Posted at: 2016-07-28T01:19:09.543Z Reads: 399

```
Sounds like one or more of your cells might've gone bad causing the overvolt during regen.

@treenutter The reason I'm hesitant to go to that conclusion is because that he needs to go all the way to 90% for the issue to go away. This should stop happening even at 98-99%. The settings seem correct for battery Regen according to his screenshot.
```

---
## \#14 Posted by: anorak234 Posted at: 2016-07-28T02:08:52.571Z Reads: 382

```
I think maybe they use something to simply dissipate the leftover energy as heat?
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2016-07-28T02:10:42.006Z Reads: 386

```
It sound like a problem with the bms or the battery, I think you should contact @EnertionSupport or @onloop to take a look  into your problem.
```

---
## \#16 Posted by: Jinra Posted at: 2016-07-28T02:11:10.997Z Reads: 380

```
On the faq it says they have a secondary braking resistor to correct the problem. My theory is that the resistor reduces the voltage to prevent current from flowing back into the battery and it redirects the energy as heat to a sink.
```

---
## \#17 Posted by: anorak234 Posted at: 2016-07-28T02:12:05.643Z Reads: 372

```
Sounds good to me. Wouldn't reduced voltage means that the board is slower at the start though?
```

---
## \#18 Posted by: Jinra Posted at: 2016-07-28T02:13:28.840Z Reads: 365

```
Braking resistor would mean it's lowering the voltage against current from flowing into the battery, not out.
```

---
## \#19 Posted by: anorak234 Posted at: 2016-07-28T02:14:17.526Z Reads: 365

```
Ah, got it. I wonder why other sellers with 'regen braking' don't do this...
```

---
## \#20 Posted by: Jinra Posted at: 2016-07-28T02:15:54.745Z Reads: 365

```
I think it's because it requires additional engineering due to it being a "**secondary** braking resistor" meaning it needs to have a primary one for actually regen braking when it's not full. I could be completely wrong though, so a bit of a disclaimer there :)
```

---
## \#21 Posted by: anorak234 Posted at: 2016-07-28T02:17:15.297Z Reads: 343

```
I think ur probably right. Either way, mellow defenitely packed more into their product than other sellers, so it's not surprising that they took the time to make sure braking is always available
```

---
## \#22 Posted by: Fababuba Posted at: 2016-07-28T02:27:24.295Z Reads: 338

```
I have the same OVER_VOLTAGE braking issue with the space cell. However, my display recently stopped working so I can't check at what percentage it fixes itself. Do you also get the OVER_VOLTAGE error when you rapidly press the throttle to full in short bursts?
```

---
## \#23 Posted by: Hummie Posted at: 2016-07-28T02:36:42.348Z Reads: 332

```
I thought the vesc and braking at full charge was a risk because you can over charge the batteries and blow them up but the brakes worked fine until that happens:grinning:
```

---
## \#24 Posted by: Mrmoonlight Posted at: 2016-07-28T02:41:14.753Z Reads: 325

```
Nope, just when I hit the breaks.
```

---
## \#25 Posted by: Mrmoonlight Posted at: 2016-07-28T02:48:01.779Z Reads: 318

```
I recall hearing somewhere that the SpaceCell had some protection against that and it would only pose an issue if you started your ride braking down a big hill. Otherwise, once you start off, you deplete the battery enough that it shouldn't pose an issue. 

So I messed with my settings a bit and at 97% charge, I needed to set my Motor Min -10A to get it to brake without any errors. Once I got down to 95%, I could up that to -25A.
```

---
## \#26 Posted by: Mrmoonlight Posted at: 2016-07-28T03:00:57.754Z Reads: 310

```
Just sent a message to Enertion. Thanks everyone for all the help. Definitely feel like I'm getting closer to figuring out all the issues with my setup.
```

---
## \#27 Posted by: Hummie Posted at: 2016-07-28T03:01:01.129Z Reads: 313

```
so it's a spacecell issue right because the vesc doesnt shut off the brakes when over charging from regen.  I think if you use just the vesc and at full charge slam on brakes on a mountain and you dont burst into flames you can eventually hit your max voltage limit and then that shuts the board down.  right?  there are voltage spikes so maybe it would shut off before what the battery voltage really is.
```

---
## \#28 Posted by: Mrmoonlight Posted at: 2016-07-28T03:03:50.360Z Reads: 307

```
Ha ha! Now I just need a mountain so I can test that theory out.
```

---
## \#29 Posted by: elkick Posted at: 2016-07-28T08:11:17.253Z Reads: 292

```
I have a space cell (the old one) here and my kids are using it since Sept. 2015, never had a single issue like this. Try to adjust the Motor min. (regen) to be -40 or lower.
```

---
## \#30 Posted by: chaka Posted at: 2016-07-28T12:59:42.820Z Reads: 293

```
It seems like you are having a problem with the vesc rather than the bms since you have recorded an "over voltage" fault. You should not be getting an over voltage fault since your max voltage is set to the default setting of 57 volts. Might have some faulty capacitors.
```

---
## \#31 Posted by: Mrmoonlight Posted at: 2016-07-28T13:37:43.668Z Reads: 293

```
Works to lower the motor min, but I have to bring it down to -10. I'm thinking this is not the norm. I sent a message to Enertion Support. I'm sure they will have more insight.
```

---
## \#32 Posted by: Hummie Posted at: 2016-07-28T15:45:54.629Z Reads: 287

```
Isn't that a huge amount of amps to be going back into the battery? Or maybe that's not where it goes. Is there somewhere yet that gives an expalanation of all the variables on the bldc program?
```

---
## \#33 Posted by: Jinra Posted at: 2016-07-28T15:48:06.033Z Reads: 284

```
battery Regen is the field that controls current going back into battery, not motor Regen
```

---
## \#34 Posted by: Hummie Posted at: 2016-07-28T15:54:06.889Z Reads: 286

```
So I can adjust the motor regen to what is comfortable as its not a risk while the battery side I should consider what my battery can take back?

It still seems a basic vesc guide isn't around
```

---
## \#35 Posted by: elkick Posted at: 2016-07-28T16:34:37.060Z Reads: 280

```
The initial problem is not a space cell issue but a VESC issue. And those parameters are not difficult to understand, motor in/out, battery in/out and both can be different limits, where battery values are to be aligned with the BMS capabilities. 

Since the the VESCs shows over voltage and the Volt limit is set to 57V it's obviously a VESC issue like chaka's mentioning, failing caps.
```

---
## \#36 Posted by: Jinra Posted at: 2016-07-28T16:44:39.467Z Reads: 272

```
Is it not possible that bad cells are causing a voltage spike in the VESC during regen?
```

---
## \#37 Posted by: Hummie Posted at: 2016-07-28T16:50:33.534Z Reads: 279

```
Ok let's say I want to make the brakes stronger what are my variables?  I dont necessarily think it's hard but it'd be nice if all the options were explained in one place. Maybe they are and I can read it.

Just increase either or both as long as I don't put more amps back to the battery than it can take?   Can I have a higher number going to the battery than from the motor?   If I have a huge battery can I have a huge back to battery number? Is there a limit on either variable?
```

---
## \#38 Posted by: Mrmoonlight Posted at: 2016-07-28T16:50:49.227Z Reads: 280

```
I'm also having a problem with losing power when putting stress on the motor after I've been riding for awhile. I was thinking that was a heat issue with my VESC. Installed some heatsinks, but I haven't been able to test it out yet. Without the heatsinks, with my board cold, I could go about a half mile on a 2.5% grade without issue, then power starts to cut out and my board will be limited to a crawl. If my board is already warmed up, it happens after a few blocks. Not sure if it's a related issue or gives any additional insight.

@Hummie, I agree. It would be nice to have a brief and basic explanation of each of the settings all in one place. I'm still trying to decipher what each setting affects. If there's nothing like that floating around, I'm sure, with a little input from everyone, it wouldn't be hard to create.
```

---
## \#39 Posted by: Hummie Posted at: 2016-07-28T16:55:01.115Z Reads: 276

```
Maybe u could ride with a laptop and see ur temps. Or adjust the temp limits. Are ur vescs sealed in?
```

---
## \#40 Posted by: Jinra Posted at: 2016-07-28T16:55:12.897Z Reads: 282

```
I'm not saying this is 100% how you should do it, but this is how I'm setting mine up. I know that both battery regen and motor regen affect braking ability. I'll be setting my battery regen to the max charge current supported by my pack (10s4p 25R cells) which is 16 amps. Since I'm running dual drive I'm setting each VESC to -8 battery regen. My motor regen will be set to -60A. Battery max is at 40A per VESC (80A total to match the pack).
```

---
## \#41 Posted by: chaka Posted at: 2016-07-28T16:57:01.295Z Reads: 266

```
Sounds like your VESC is overheating, your options are, switch to a smaller motor, add another large motor and run dual, or add an auxiliary fan and attempt to keep the VESC cool.
```

---
## \#42 Posted by: Mrmoonlight Posted at: 2016-07-28T17:33:55.538Z Reads: 260

```
I'm running a Carvon V2 single hub. I weigh 135, so I figure I would be fine with a similar setup as Runplayback and his single Carvon hub build. Not sure if he uses a heatsink on his VESC, but I'm hoping that I can get a similar level of performance without adding another motor or fan. 

I'll take my laptop today and see if I can get a temp read.
```

---
## \#43 Posted by: chaka Posted at: 2016-07-28T18:06:51.989Z Reads: 255

```
@RunPlayBack is in a relatively flat area so I am not sure if he has done much hill climbing but that is when things start to heat up. Maybe he can chime in with his experience on those hubs. 

FYI, I am not sue where you got your VESC but if you purchased from me at Ollin Board Company you can send it in for repair if it keeps giving you problems with the over voltage fault.
```

---
## \#44 Posted by: JohnnyMeduse Posted at: 2016-07-28T18:21:09.567Z Reads: 247

```
If the problem was related to the VESC, it will occur whatever the battery voltage were. So, because the problem stop when the battery reach around 90%, it most likely to be a BMS problem (probably a protection circuit when out, and now the BMS is unable to do it job properly). Also, it not because this is a DRV fault, that the problem is coming from the VESC. Problem on electronics circuit are often more complex that you might think.
```

---
## \#45 Posted by: Mrmoonlight Posted at: 2016-07-28T19:05:47.333Z Reads: 247

```
Just took a temp reading right after my board started to cut out. It was a couple minutes after and was at 75. So I'm sure I had passed 80 degrees and cut out. The heat sinks must be working. I was able to go a lot further without it cutting out and it's 91F out here. 

So is it safe to go any higher than 80? I also have a much bigger and better heats ink on order that should help even more.

Right about to go over a bridge, so giving it awhile to cool off. Last time I got about 1/8 mile before it cut out.

@chaka, got my VESC from Enertion.
```

---
## \#46 Posted by: chaka Posted at: 2016-07-28T19:26:23.123Z Reads: 236

```
If you have the space for it you can add a small fan off the 5v from the VESC and remove the heat from those heatsinks. Remember 80 C equals about 180 degrees Fahrenheit so it best to keep things cooler if you can.
```

---
## \#47 Posted by: Mrmoonlight Posted at: 2016-07-28T21:03:15.227Z Reads: 236

```
Good idea. Plenty of space in there. It's 10s version and about 6" of the case is just foam. I can probably move that back a bit and make room for a fan and my larger heatsink. That should definitely take care of the heat issue. I was able to go 1/4 miles before it shut down. So twice as far as before. Plus it cooled off much quicker and I just had to push a few times to get up. Once I got onto a flat, it was fine again. Previously it would take a few minutes even after I came to a flat to get power back. 

Quick question. Would one of these fans work? Also, one has 3 cables, the other has 2. Do you know which of the 4 pins on the VESC I should connect to?

https://www.amazon.com/5015S-Turbine-Brushless-Cooling-Blower/dp/B00H6VM83I/ref=sr_1_2?ie=UTF8&qid=1469739202&sr=8-2&keywords=5V++fan+blower

https://www.amazon.com/uxcell%C2%AE-0-25A-Computer-Cooling-Blower/dp/B018TGYQF6/ref=sr_1_8?ie=UTF8&qid=1469739202&sr=8-8&keywords=5V++fan+blower
```

---
## \#49 Posted by: Hummie Posted at: 2016-07-29T00:20:22.766Z Reads: 228

```
i bet some vesc get hotter than others.  some people have them encased and also, more so, I think some of them are just made better.  Is this possible?  I know of people who are always being stopped and even have fans attached and I can completely seal my stuff up in bubble wrap and never get too hot despite having motors closely attached that will get up to 200f
```

---
## \#50 Posted by: Mrmoonlight Posted at: 2016-07-29T01:37:20.039Z Reads: 225

```
How hot do you let your MOSFET's get before you have them cut off? I have mine set to 80c, but I'm not sure how safe it is to let them get much hotter. 200f would give me and extra 13 degrees. That would definitely solve part of my issue. 

@onloop, any suggestions on max MOSFET and Motor Start + End temps?
```

---
## \#51 Posted by: evoheyax Posted at: 2016-07-29T01:55:01.717Z Reads: 229

```
I have this issue every time I ride. After a good push to full throttle for a seconds, the the problem goes away. I always assumed it's an over voltage protection by the VESC, stopping the breaking from occurring cause it would over charge the battery. This cuase me to fall last week, only the second times I've gone down on an eboard.
```

---
## \#52 Posted by: RunPlayBack Posted at: 2016-07-29T01:58:10.023Z Reads: 231

```
@Mrmoonlight I've never encountered that issue and I'm running the older Space Cell with @chaka VESC without heatsink. The only issues I've ever had with his VESC are user error because my phase wires came loose otherwise everything is working in tip top shape through all kinds of weather since last November. I weigh just under 130lbs so our build specs are pretty much identical. Here's my "city safe" settings:

Motor Max: 60.00 A
Motor Min: -60.00 A
Bat Max: 30.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A

Max ERPM: 60000.00

Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V
```

---
## \#53 Posted by: Jinra Posted at: 2016-07-29T02:03:27.285Z Reads: 213

```
Shouldn't your battery regen be less since, I'm assuming, you're running 3p on 4a max charge current cells. The max i would set battery regen at is -12A
```

---
## \#54 Posted by: RunPlayBack Posted at: 2016-07-29T02:08:42.830Z Reads: 207

```
Yup sorry that was a typo! I meant to put -12.00 just updated it :)
```

---
## \#55 Posted by: Mrmoonlight Posted at: 2016-07-29T02:08:48.605Z Reads: 218

```
Thanks! 
What effect does having the Max ERPM at 60000 do? Does in have any effect in FOC mode?

Couple questions:
Do your brakes work fine with a fully charged or even a 95% charged battery?
After your board is warmed up, can you take on a 2.5% grade for more than 600ft before the Temp limits start cutting power?
```

---
## \#56 Posted by: RunPlayBack Posted at: 2016-07-29T02:10:31.313Z Reads: 214

```
60,000 limits my top speed to around 23-25mph. Yup brakes work fine on flats, I don't really take many high grade hills around where I live but even on the occasional time where I pushed it hard up a hill it's never cut power off on me with these settings.
```

---
## \#57 Posted by: Mrmoonlight Posted at: 2016-07-29T02:20:52.337Z Reads: 220

```
Makes sense. I never need to go that fast. I'm fine with maxing out my speed around 20mph. 

My brakes won't work on flats or anything unless my Batt max is less than 10A if I'm close to a full charge.

If my board is warmed up and if I took off the heatsinks, it would cut power on even a 1% grade after a couple blocks. Once it cuts off, it won't even do flats for awhile until it cools off. With the heatsinks I can ride flats no problem and 1% grades are not much of an issue unless I'm going for a longer than a mile. Then I have to coast every so often for a few seconds to keep it going. 

How far do you usually ride? My usual ride is around 7 - 8 miles, but I start having issues after around a mile. 

Sounds like my board is not even close to performing the way it should. I'm hoping I can figure this out when Enertion Support gets back to me.

Thanks!
```

---
## \#58 Posted by: Mrmoonlight Posted at: 2016-07-29T02:25:59.583Z Reads: 209

```
Did you ever resolve your issue with power cutting when going up hill?
```

---
## \#59 Posted by: evoheyax Posted at: 2016-07-29T03:18:41.751Z Reads: 210

```
Yes, it was the VESC over heating. With chakas heatsinks, this issue went away. I believe the high kv created huge inefficiencies which heated the vesc's more than they should have.
```

---
## \#60 Posted by: joeadams101 Posted at: 2016-08-04T20:36:15.321Z Reads: 199

```
Yup you are having the same Issues I am. The brakes work fine after adjusting the max input voltage. Still having the loose of
Power issue. Will try again tonight with @onloop recommendation of bat max
```

---
## \#61 Posted by: joeadams101 Posted at: 2016-08-05T06:08:02.070Z Reads: 195

```
where to buy chakas heatsinks?
```

---
## \#62 Posted by: DeathCookies Posted at: 2016-08-05T06:16:06.796Z Reads: 189

```
Just search in ebay or amazon "heatsinks" and you will find many!
```

---
## \#63 Posted by: Mrmoonlight Posted at: 2016-08-07T07:35:26.877Z Reads: 191

```
Not sure if you can tell from this. I couldn't make out the text on the side from my pic. I haven't seen many of these so, not sure.

<img src="/uploads/db1493/original/2X/6/61dcc5e9908782947aa1df5af29cc6f3fca817a6.jpg" width="431" height="500">
```

---
## \#64 Posted by: Jinra Posted at: 2016-08-07T07:36:54.489Z Reads: 185

```
Yea can't tell unfortunately :( Just post back when you find out.
```

---
## \#65 Posted by: Mrmoonlight Posted at: 2016-08-07T07:42:01.916Z Reads: 191

```
Will find out as soon as I get back to NY. 

Thanks for help! Always appreciated.
```

---
## \#66 Posted by: Mrmoonlight Posted at: 2016-08-07T17:14:46.709Z Reads: 191

```
So Enertion support just got back to me and said that my board's performance is common amongst Carvon V2 users and they can't find any issues. Their best solution was to upgrade to the Carvon V2.5 or upgrade to the VESC premium if I want to swap my VESC. Basically they're saying it's a problem with my setup since the Carvon V2 hub will cause these overheating issues with it's high KV. Am I missing something here essential for my setup to work? This is my first DIY build so It's definitely a possibility. 

Thanks all for the help!

My list of parts:

Carvon V2 
Enertion VESC
Enertion SPACE CELL 3
Enertion Steeze Remote

Here's my wiring diagram.

<img src="/uploads/db1493/original/2X/b/b138aea03974099df9eefff2a3d889f0c2f17e95.jpg" width="500" height="500">
```

---
## \#67 Posted by: Jinra Posted at: 2016-08-07T17:20:03.121Z Reads: 181

```
[quote="Mrmoonlight, post:66, topic:6730"]
Basically they're saying it's a problem with my setup since the Carvon V2 hub will cause these overheating issues with it's high KV.
[/quote]

That doesn't sound right to me, but i could be wrong.
```

---
## \#68 Posted by: elkick Posted at: 2016-08-07T17:53:03.984Z Reads: 179

```
So, 149kv with 10s is considered high kv? That's definitely a wrong argument and cannot be the cause of you issue at all.
```

---
## \#69 Posted by: Mrmoonlight Posted at: 2016-08-07T18:02:26.587Z Reads: 190

```
This is response I got. I'm pretty green when it comes to DIY boards since this is my first build, so maybe I'm reading something wrong if most other Carvon V2 users are having the same issue.

"After looking through your forum thread, and these screen shots I can't see anything out of the ordinary that would point to some fault of the VESC's- others have had over heating problems with carvon's hubs (due to the high KV I mentioned before) and solved the issue with heatsinks or fans. 

If you want to get the VESC platinum warranty we'd be happy to take a look at it, but in my honest opinion I don't think another VESC would solve these issues; it seems to run consistently with a couple other carvon users. Hopefully the lower KV v2.5's will solve the problem."
```

---
## \#70 Posted by: chaka Posted at: 2016-08-07T18:12:00.514Z Reads: 185

```
I have plenty of customers using Carvon hubs with the VESC and it works great! You probably have a faulty BMS. One way to check is by getting eyes on the VESC when the brakes cutout. If the vesc blinks three times then it is probably a DRV fault, if the vesc powers off then the BMS is giving out.
```

---
## \#71 Posted by: anon33082420 Posted at: 2016-08-07T18:18:28.588Z Reads: 177

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#72 Posted by: Mrmoonlight Posted at: 2016-08-07T18:53:13.339Z Reads: 172

```
I'll definitely try that when I get back to NY. Got some testing to do!

@LEVer, my heat sink is only covered on the edges to keep them on. That was an old shot. Now there's 4 heat sinks (2 on both sides) and the plastic wrap only goes around the very edges to hold it on. 2 caps. I checked the pins and cut them down.

Perhaps there are different types of VESC's out there with different specs that are optimized for different motors? Enertion's would obviously be optimized for Enertion motors. Would that make any sense?
```

---
## \#73 Posted by: Mrmoonlight Posted at: 2016-08-09T17:20:13.014Z Reads: 165

```
@chaka tested it and my VESC blinks 3 times. So DRV fault? Would that possibly mean a bad chip? I also took out and inspected my battery pack and found a loose connection. Soldered it. Solved a couple small intermittent issues, but still getting the fault.

@Jinra and @LEVer Checked my 2 caps. They are 63V.

Installed a much larger heatsink today. I'll test it and see if it makes any difference in my VESC overheating.
```

---
## \#74 Posted by: Jinra Posted at: 2016-08-09T17:21:56.576Z Reads: 156

```
anyway you can replicate the problem on the bench and see if you get a fault code in BLDC?
```

---
## \#75 Posted by: Mrmoonlight Posted at: 2016-08-09T17:22:50.709Z Reads: 154

```
Fault is Over voltage
```

---
## \#76 Posted by: Jinra Posted at: 2016-08-09T17:23:14.097Z Reads: 153

```
Oh right, sorry. Keeping up with too many threads lately.
```

---
## \#77 Posted by: Mrmoonlight Posted at: 2016-08-09T17:59:35.078Z Reads: 156

```
No apologies needed. Thanks for all the help!
```

---
## \#78 Posted by: Mrmoonlight Posted at: 2016-08-09T19:57:04.812Z Reads: 161

```
So no impovement with he larger heat sink. If this didn't help the heat issue, I'm not sure how much difference even a fan would make.
```

---
## \#79 Posted by: Jinra Posted at: 2016-08-09T20:01:57.620Z Reads: 157

```
Your VESC shouldn't be getting that hot that quickly in the first place. Adding more cooling will only be masking the real problem.
```

---
## \#80 Posted by: Mrmoonlight Posted at: 2016-08-09T20:17:14.388Z Reads: 152

```
Enertion was saying this was pretty normal for their VESC's when paired with a 149kv motor and that heat sinks and fans usually takes care of the problem.
```

---
## \#81 Posted by: Jinra Posted at: 2016-08-09T20:18:27.427Z Reads: 151

```
maybe if you're riding for a long time and up a bunch of hills, but otherwise not normal.
```

---
## \#82 Posted by: Mrmoonlight Posted at: 2016-08-09T21:21:56.498Z Reads: 148

```
For flats if I'm riding for around 15 -20min I overheat with a heatsink. Without the heatsink, I overheat after around 5min. Enertion is saying my best bet is to upgrade to the Carvon V2.5 with the 85KV motor, add heatsinks+fans, and I should be good to go for my overheating and braking issues. 

My question is, if 149KV is too high for my VESC and Enertion's motors are 190KV, wouldn't their motors also have issues with over heating and braking? or does the belt + pulley eliminate this?
```

---
## \#83 Posted by: Jinra Posted at: 2016-08-09T21:23:09.054Z Reads: 148

```
Oh I forgot you're using Carvons. Hub motors generally draw more current than belt drives so running a 190kv motor with reduced gearing should be less stressful.
```

---
## \#84 Posted by: Mrmoonlight Posted at: 2016-08-09T21:40:37.955Z Reads: 142

```
Makes sense. 

So is what Enertion is saying sound right? That a 149KV hub motor would make my VESC overheat like this?
```

---
## \#85 Posted by: Jinra Posted at: 2016-08-09T21:44:32.156Z Reads: 140

```
I guess it depends on current draw, but overheating in 5 minutes on flats doesn't sound right to me. The fact that there's an overvolt error is peculiar itself. I suspect there's something more than just an incompatible motor.
```

---
## \#86 Posted by: sl33py Posted at: 2016-08-09T21:49:12.230Z Reads: 135

```
where do you live?  wonder if you tried another un-heatsinked VESC if the issue would persist.  It would simplify the discussion w/ Enertion...
```

---
## \#87 Posted by: Mrmoonlight Posted at: 2016-08-09T21:56:31.831Z Reads: 136

```
I live in NYC. I just ordered another VESC to test from DIY. Should be here in a week or so. Enertion is saying everything looks normal, but I'm questioning that given what I'm hearing from everyone here. Especially since Runplayback (I basically duplicated his setup and settings) is getting much better performance. Or it may just be Enertion's newest crop of VESC's being optimized to work with Enertion's setup. That would makes sense too. I wouldn't expect them to make a VESC with Carvon hubs in mind.
```

---
## \#88 Posted by: Jinra Posted at: 2016-08-09T22:00:44.851Z Reads: 140

```
VESCs aren't custom tailored to any specific motor hardware-wise. You configure the software per motor in BLDC tool. I still think it's something wrong with the battery or VESC.
```

---
## \#89 Posted by: Mrmoonlight Posted at: 2016-08-09T22:50:30.157Z Reads: 143

```
That's what I thought, but it seems that some VESC's perform different than others. I imagine the type of hardware used could make a difference in performance? I know some VESC's have 3 caps and other's have 2. Maybe the numbers work out to be the same? Not sure what hardware other VESC's have.
```

---
## \#90 Posted by: sl33py Posted at: 2016-08-09T23:01:14.367Z Reads: 142

```
[quote="Mrmoonlight, post:87, topic:6730"]
I basically duplicated his setup and settings
[/quote]


Did you run your own motor detection and adjust the settings to reflect your detection settings in BLDC?  Vs just plugging in someone else's values and skipping those detection steps in your setup.  Just want to confirm.
```

---
## \#91 Posted by: sl33py Posted at: 2016-08-09T23:03:39.951Z Reads: 137

```
[quote="Mrmoonlight, post:89, topic:6730"]
some VESC's have 3 caps and other's have 2.
[/quote]


I like the 3 smaller caps better for compact form and easier to fit, but i *still* only run a single bigger cap on my 4.7hw VESC's.  It's not about the # of caps (but more does help marginally) - but really the total capacity of the cap to smooth the power to VESC.
```

---
## \#92 Posted by: Mrmoonlight Posted at: 2016-08-09T23:20:42.850Z Reads: 130

```
Yup, ran the motor detection and plugged in the appropriate settings. 
With the caps, I figured it didn't make much of difference as long as the total capacity was equivalent. I'm just not sure what other VESC's come with.
```

---
## \#93 Posted by: Tomkav Posted at: 2016-08-15T09:56:07.913Z Reads: 121

```
I'm getting the same thing but it then starts randomly doing its own thing.  Is this related? It stops after discharging below 90% and runs perfectly thereafter.  Help needed.
```

---
## \#94 Posted by: Mrmoonlight Posted at: 2016-08-15T11:27:01.761Z Reads: 123

```
What's ur set up? Also take a screenshot of your VESC settings.
```

---
## \#95 Posted by: Tomkav Posted at: 2016-08-15T13:30:46.071Z Reads: 120

```
How do I get the vesc settings?

Enertion trucks, pro drive+ motor, space cell pro 4 and Enertion Vesc ( recent batch)
```

---
## \#96 Posted by: Mrmoonlight Posted at: 2016-08-15T13:45:46.138Z Reads: 115

```
Have you done your motor detection on your VESC?
Once you're on your main BLDC tool screen, take a screenshot.
```

---
## \#97 Posted by: Tomkav Posted at: 2016-08-15T13:58:54.722Z Reads: 116

```
How do I connect? Is there a cable?
```

---
## \#98 Posted by: Mrmoonlight Posted at: 2016-08-15T14:15:04.128Z Reads: 133

```
Have you read through this thread?

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#99 Posted by: onloop Posted at: 2016-08-15T14:45:34.553Z Reads: 145

```
[quote="Mrmoonlight, post:87, topic:6730"]
Or it may just be Enertion's newest crop of VESC's being optimized to work with Enertion's setup. That would makes sense too. I wouldn't expect them to make a VESC with Carvon hubs in mind.
[/quote]

our vesc do have some preinstalled settings for r-spec motors, it saves our customers some stuffing around when they get their kits... also prevents some of the silly mistakes that can occur during the initial bench testing / setup phase...

here are some more things to try....

- Turn down the motor regen current, get it as close to the battery regen current as possible whilst still having some suitable brake force. (maybe -18 to -20)
- Bypass the BMS for discharge, if the problem still occurs it might be BMS related.
- Try a new VESC, do you have VESC platinum? if so email support@enertionboards.com and we will send a new one.
- Try some other motors, maybe a belt drive and see if problem remains.
```

---
## \#100 Posted by: Mrmoonlight Posted at: 2016-08-15T15:03:12.930Z Reads: 137

```
Thanks for the input!

I updated all my VESC settings to match up with my system. Consulted Carvon and Runplayback. I turned down my brake regen and it doesn't work unless I'm under -10. When my battery gets under 90% charge braking works fine. It's just when it's over 90%. 

I have a new VESC and another motor on order. Enertion support suggested I try Carvon V2.5 with the lower KV and that should solve my problem. I should have both of them in within the next week or so. Then I can swap parts and narrow down what part is causing my issue.

How do I bypass the BMS of discharge?

Thanks!
```

---
## \#101 Posted by: Tomkav Posted at: 2016-08-16T04:09:10.592Z Reads: 139

```
Thanks mate. I'll give it a go.
```

---
## \#102 Posted by: Mrmoonlight Posted at: 2016-08-17T18:58:52.948Z Reads: 136

```
UPDATE: 
solved the braking issue. Not sure exactly what I did that fixed it, but I re-soldered a loose connection on one of my batteries and I accidentally charged my battery to 100% which caused my board not to respond to my remote. At the advice of @Blasto I messed around with my max voltage settings to get my board to respond again and after I did that, my brakes started working fine. 

The only issue left is how to keep my VESC from overheating.
```

---
## \#103 Posted by: Jinra Posted at: 2016-08-17T18:59:37.401Z Reads: 135

```
Wasn't your max input voltage already at 57v?
```

---
## \#104 Posted by: Mrmoonlight Posted at: 2016-08-17T19:13:18.788Z Reads: 142

```
Yup. I had it at 57v, but I also tried some other settings too. Didn't make a difference for the braking until this last time. It could have been that or something else. For the past couple weeks I've been keeping my board under 90% charge, but I've changed a lot of other settings in the meantime to try an resolve my overheating issue.
```

---
## \#105 Posted by: Mrmoonlight Posted at: 2016-08-26T00:19:36.643Z Reads: 150

```
So I ordered another VESC from DIYelectricskateboards and popped it in last night. Took a ride today and the board performed great! I had full power over all flats and only overheated when going over the bridge. I actually had power for a good part of it and I didn't even stop to let it cool off first. I couldn't even go up a 1blk 3% grade without it instantly cutting power and had to wait around 10min before going over the bridge just to get a 1/4 of the way up before I had to start pushing. Before I had to start pushing on flats after around 20min.  

Not sure what is different about the Enertion VESC, but this one works infinitely better on the same settings. I think I can tweak it a bit to make it work even better.
```

---
## \#106 Posted by: Eboosted Posted at: 2017-01-29T04:52:00.135Z Reads: 115

```
So, you fixed the issue by setting your Maximum input voltage from the original 57V to what value?
```

---
## \#107 Posted by: Luke Posted at: 2017-01-29T08:30:16.760Z Reads: 113

```
The original value is usually 42v, he changed it to 57v :)
```

---
## \#108 Posted by: Eboosted Posted at: 2017-01-29T18:03:50.558Z Reads: 112

```
My original value has always been 57V and I have the same exact problem. Has anyone tried to increase this value more than 57V in order to avoid the cutting off?
```

---
## \#109 Posted by: Mrmoonlight Posted at: 2017-01-29T19:42:04.315Z Reads: 114

```
Is your issue brakes cutting out or power cutting out?
```

---
## \#110 Posted by: Alextech Posted at: 2017-01-29T19:55:17.048Z Reads: 116

```
You really shouldn't exceeded the 57V level. After that you are exceeding the VESC Threshold and can really just start burning up DRV chips like myself.
```

---
## \#111 Posted by: Eboosted Posted at: 2017-01-29T21:51:07.371Z Reads: 117

```
The VESC is reseting itself when I'm on 100% charged battery and I brake, regenerative braking puts curebt into the battery but as it's already fully charged VESC cuts off.
```

---
## \#112 Posted by: Mrmoonlight Posted at: 2017-01-30T04:31:49.400Z Reads: 115

```
Whenever the battery is 100% charged, your brakes won't work because of regenerative breaking. It's basically the motor feeding power back into he battery. If the batt is full, no place for the power to go. Try running your board down to 98% before breaking.
```

---
## \#113 Posted by: Eboosted Posted at: 2017-01-30T04:36:23.292Z Reads: 112

```
That's what I'm currently doing but this solution is just a bandaid. I don't think people would be at the side of the board waiting to be 98% and unplug it afterwards.

How are do all eboards brands have a work around this?
```

---
## \#114 Posted by: Mrmoonlight Posted at: 2017-01-30T08:49:32.639Z Reads: 109

```
The only solution is limiting the charge. It can be done electronically so you don't have to, but when it comes to regen brakes, it's what it is.
```

---
## \#115 Posted by: Eboosted Posted at: 2017-01-30T14:07:36.063Z Reads: 107

```
In order to. Limit the charge at 98% o guess you should use a specific custom charger, I'm I right?
```

---
## \#116 Posted by: PXSS Posted at: 2017-01-30T14:40:03.950Z Reads: 110

```
Cant you set your charger to charge to 4.1V/cell instead of 4.2V
```

---
## \#117 Posted by: Eboosted Posted at: 2017-01-30T15:29:07.839Z Reads: 120

```
No, I just have a regular brick similar than the Evolve Charger.

<img src="/uploads/db1493/original/3X/c/8/c85f5c37b479ea5608a0877805b3caa6a7604424.jpg" width="500" height="500">
```

---
## \#118 Posted by: PXSS Posted at: 2017-01-30T17:00:07.146Z Reads: 116

```
Open it up! I think @whitepony has that charger and said there's a pot inside you can adjust
```

---
## \#119 Posted by: whitepony Posted at: 2017-01-30T17:34:09.626Z Reads: 120

```
nope, not in the evolve charger! 

http://www.electric-skateboard.builders/t/cheap-chargers-with-customizeable-end-of-charge-voltage/6902
```

---
## \#120 Posted by: Mrmoonlight Posted at: 2017-01-30T20:07:22.469Z Reads: 118

```
I know it's been done, but I'm not exactly sure of the details. I deal with it by running my motor on my way out the door if I'm at 100%. Then brake gently for the first minute or so of my ride. At what percentage does your board start working properly?
```

---
## \#121 Posted by: Kaden56 Posted at: 2017-01-30T20:19:25.137Z Reads: 118

```
I didn't read through the entire thread but I thought I'd mention that this happens with my board too. I have dual vescs and DIY's 10s4p pack. However it's only when the battery is right at 100% on my board. After riding for just 1 minute or so I can brake just fine. I have always just chalked it up to the vescs making sure my pack doesn't get over charge with regen braking. I just keep it in mind when I take the board out after fully charging it and I've had no scary situations.
```

---
## \#122 Posted by: Eboosted Posted at: 2017-01-30T20:57:30.676Z Reads: 108

```
What setting you have on max amp regen?
```

---
## \#123 Posted by: Mrmoonlight Posted at: 2017-01-30T21:15:34.052Z Reads: 109

```
Motor Max 60A
Motor Min -60A
Batt Max 30A
Batt Min -12A
```

---
## \#124 Posted by: Eboosted Posted at: 2017-01-30T21:52:23.609Z Reads: 117

```
Are those settings for a single or dual ?
```

---
## \#125 Posted by: Mrmoonlight Posted at: 2017-01-30T23:57:28.653Z Reads: 123

```
Single

oooooo
```

---
## \#126 Posted by: Eboosted Posted at: 2017-02-14T21:12:23.105Z Reads: 117

```
You need to apply this wiring to fix the issue

http://www.electric-skateboard.builders/t/vesc-bms-cutting-out-at-full-charged-battery-solved/16714/25?u=eboosted
```

---
## \#127 Posted by: eitan Posted at: 2017-02-18T23:32:58.926Z Reads: 111

```
Fascinating! thanks for posting your conclusions
```

---
## \#128 Posted by: jippijuk Posted at: 2018-10-30T02:36:06.095Z Reads: 42

```
I read hours and its very helpful. My decision is to keep the electronic simple at my board and bought a fancy Turingy Balance charger( charging outside of my board).

Question: since i have a balance charger i decided not to have a BMS between my Lipos ( 2 X 5S 40C 5000mAh in series), so I go directly through a spark safety switch into my motor controller ( waiting for the Focbox unit) During braking and down hill there is current going back to my Lipos - does this damage my Lipos ?
Do I need a BMS in between? or can I choose special settings with the BLDC-tool. Or this back flowing current is not critical?
```

---
