# How can I reduce VESC overheating?

### Replies: 31 Views: 5451

## \#1 Posted by: evoheyax Posted at: 2016-03-28T22:30:59.558Z Reads: 410

```
First off, I am not the normal. I have a good 5 mile each way route to my university that I take everyday. It involves no hills higher of a grade than 7%. However, on my way to class, I have 16 uphill blocks followed by 2 downhill blocks, followed by another 4 blocks uphill before it turns to mostly downhill and flat. I can get about 5 blocks before my vesc's start to shutdown from too much heat.

My first solution was a 20mm fan that blew air through the side where the vesc's are. This did not do much.

After trying the small fan, I decided to step it up to 2x 40 mm fans one that blows air directly down onto the FETs of each VESC, which from my research, seem to be the main component that over heats.

This works much better. However, I still can not make it the 16 uphill blocks without the board ramping my speed back to a standstill, and forcing me to take a break to let it cool down.

So what else can I do?

I bough little heatsinks that I could put into the FETs, but I'm afraid that the intense vibrations of San Franciscos poor quality roads along with the heat with kill the glue on the back of the heatsinks and knock them off, causing a short circuit somewheres.
```

---
## \#2 Posted by: treenutter Posted at: 2016-03-28T22:47:04.086Z Reads: 400

```
@evoheyax Would you pull less amps in these settings, and thusly produce less heat, if you increased voltage with a larger battery?
```

---
## \#3 Posted by: chaka Posted at: 2016-03-28T22:47:53.350Z Reads: 394

```
This sounds like a slow buildup of heat. Make sure you are getting fresh air into your enclosure/deck. 

Can we see a screen shot of your settings?

You can also adjust the temp settings a little higher 5 to 10 degrees higher isn't too bad.

Reducing motor current is another option that will help in tuning your board.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-03-28T23:30:11.922Z Reads: 384

```
These 2 40mm fans are pulling a lot of air directly onto the FETs, though I have to direction of airflow in and out, just really in and some holes for it to trickle out by the power button and charging port holes in my lid.

I debated between my own battery or a space cell for this exact concern. I was informed no one had heat issues with the VESC and space cell so I figured this would not happen. At this point, I can't afford to buy another battery right now to get to a higher voltage.

What settings in particular are you interested in? It's just that getting to the settings will be a pain as i don't have an external accessible USB port for them. But I need to get to the bottom of this, so it's ok. I just need to know what can cause higher heat and fix it as I need to do so ASAP. Leaving it open for a few days is not an option (at least until the weekend).
```

---
## \#5 Posted by: RunPlayBack Posted at: 2016-03-28T23:59:16.727Z Reads: 357

```
I've been using these settings on my dual. Ran it pretty hard this weekend on long trails with various flats and semi hills with no cutoffs.

Motor Max: 70.00 A
Motor Min: -60.00 A
Bat Max: 15.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A

Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V

Startup Boost: 0.040
```

---
## \#6 Posted by: evoheyax Posted at: 2016-03-29T00:40:14.276Z Reads: 342

```
I'm using almost the same (possibly the same) settings
```

---
## \#7 Posted by: chaka Posted at: 2016-03-29T00:51:02.419Z Reads: 338

```
I would focus on moving more air through your deck, its odd to have it overheat on flats. Are you sure you are overheating and not hitting the upper limit on your battery cut-off? Without knowing your settings it will be really hard to diagnose.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-03-29T01:15:31.838Z Reads: 335

```
Just curious abt how long is that? How long are you on the board?
```

---
## \#9 Posted by: evoheyax Posted at: 2016-03-29T01:39:20.052Z Reads: 331

```
Maybe 5 minutes tops before I first hit the heat limit.

Just to clarify I'm not hitting the heat limit on flats, only on hills, but some of the hills I'm hitting it on are only 2 or 3% grade, hardly a hill. It does seem residual, as I don't hit those limits the third hill of my route, which is my first 7% grade hill. But later on smaller hills.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-03-29T01:41:42.553Z Reads: 326

```
I'm not sure actually. That is possible but would that occur if I was to get off my board, wait for a few minutes, get back on and have no problems on he same hill that just caused problems? Wouldn't that more be an issue on super steep hills drawing high amps?
```

---
## \#11 Posted by: evoheyax Posted at: 2016-03-29T02:09:07.860Z Reads: 334

```
Now going up hill home from class just now, on a 3 or 4% hill. It cut off and now turning it back on, and reconnecting everything, nothing happens. I can't get any motor movement, despite having 30% of the battery left and fully charged enertion controller. I'm hopping I didn't blow something out with all the heat.

Getting fault code UNDER_VOLTAGE on my master vesc. Any idea what this means?

I have a min voltage set to 8v, and measuring my space cell with a multimeter shows 39.5v. I tried googling with no luck as to what that means.
```

---
## \#12 Posted by: trbt555 Posted at: 2016-04-10T17:11:42.878Z Reads: 310

```
Weather has been getting warmer where I live and I think I've been having overheating problems too, I think.
Mine also cuts out after some time on moderate hills.
It's one of @chaka's vescs with heat sinks.
```

---
## \#13 Posted by: laurnts Posted at: 2016-04-10T17:27:00.629Z Reads: 307

```
Add arctic silver thermal paste within the layer that connects vesc and mosfet. Helps heat transfer.

You can also replace the heat sink with larger ones from computer shop.

Another opt is to install a mini fan.

However I think this shouldnt happen in first place especially when you are already using 2 vesc setup.
```

---
## \#14 Posted by: trbt555 Posted at: 2016-04-10T18:08:19.477Z Reads: 296

```
I'm back to a single vesc, I didn't like the dual setup, too heavy, too noisy.
I guess I'll have to add a fan.
```

---
## \#15 Posted by: chaka Posted at: 2016-04-10T18:18:14.165Z Reads: 290

```
Can probably write some code to have one powered and controlled by the VESC that way it did not have to run all the time. I might even grease the wheels a little if someone was able to work it into the GUI and have Vedder include it in the next firmware update.
```

---
## \#16 Posted by: laurnts Posted at: 2016-04-10T18:47:27.038Z Reads: 288

```
Small fan is also noisy as hell especially those ezrun type of turbo fan. Bigger fan has less noise but doesnt improve cooling that much. Before I use to have a 3 channel remote with telemetry. So when i see the temperature increases beyond normal, I switched on the fan :)
```

---
## \#17 Posted by: trbt555 Posted at: 2016-04-10T19:41:26.763Z Reads: 280

```
You know what would be a nice product ?
A waterresistant VESC enclosure with external heat sinks, like commercial rc car esc's.
```

---
## \#18 Posted by: chaka Posted at: 2016-04-10T20:29:11.560Z Reads: 285

```
The VESC's I produce now are already water resistant. If you get them completely submersed they will stop working but they should go back to normal operation once they dry off. I could end up potting them in the future once v5 is released, they would be water proof if completely potted.
```

---
## \#19 Posted by: evoheyax Posted at: 2016-04-10T20:41:30.145Z Reads: 286

```
I don't think it's worth water proofing the components like Esc's. I think water proofing the enclosure would be better. You still need to need with the battery and any other electronics your using, like power switche or fans.
```

---
## \#20 Posted by: trbt555 Posted at: 2016-04-11T05:12:17.356Z Reads: 287

```
Yeah but then you can't put the vesc heatsinks outside the enclosure.
```

---
## \#21 Posted by: GhettoFab.rictation Posted at: 2017-11-26T11:00:01.055Z Reads: 161

```
What about running heat stinks and fans on each side of vesc. I'm going to do that tbh but idk if the vesc can take running two of these .02a fans on 5v?<img src="/uploads/db1493/original/3X/6/0/607680860bc0eb8d91d67fe9e9df3a1b33d9fbc7.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/9/4/9487070f2dbbf4717badebfcced0a52cb286a68c.jpg" width="281" height="500">
```

---
## \#22 Posted by: GhettoFab.rictation Posted at: 2017-11-26T11:02:09.777Z Reads: 160

```
7mm thin! <img src="/uploads/db1493/original/3X/e/4/e4b28da29c920da747b80ec207d49a96fd937754.jpg" width="281" height="500">
```

---
## \#23 Posted by: rok Posted at: 2017-11-26T15:41:53.101Z Reads: 160

```
I'm having the same problem with overheating vesc on flat grounds. I was running bldc with no problem but now i tried foc and it overheats. I thought its because of my longer wires under the grip tape. I will try heatsinks and bigger capacitor. Whatcha think?
```

---
## \#24 Posted by: Vanarian Posted at: 2017-11-26T15:49:48.513Z Reads: 164

```
Welp guys I'll help you out and wish you good luck with cooling it : 

<img src="/uploads/db1493/original/3X/4/e/4e861c3de9bf34bb0fa5fc79594bd928775d8b79.jpg" width="570" height="499">

Active cooling with fan on these areas works too.
```

---
## \#25 Posted by: rok Posted at: 2017-11-26T19:34:09.153Z Reads: 158

```

Where to?

<img src="/uploads/db1493/original/3X/7/1/713a1d108d998ef04f02aef537bf297d245d6c0c.jpg" width="375" height="500">
```

---
## \#26 Posted by: GhettoFab.rictation Posted at: 2017-11-27T04:11:45.265Z Reads: 156

```
 My heat  sink is going to be shaped like this and have fans on both sides sucking air in from shrink wrap then out battery lead side with shrink wrap closed on motor wires  side!  <img src="/uploads/db1493/original/3X/6/e/6ebd18554af4f3a2947aaa25bf47843a03d8aeec.jpg" width="281" height="500">
```

---
## \#27 Posted by: GhettoFab.rictation Posted at: 2017-11-27T04:24:10.599Z Reads: 150

```
Obviously not as big, flush to the mosfet unit
```

---
## \#28 Posted by: Kug3lis Posted at: 2017-11-27T04:28:26.784Z Reads: 150

```
I don't want to advertise in this forum too much, but in my opinion is cheaper just to buy a case witch would act as heatsink and solve most of the problems you have...
```

---
## \#29 Posted by: Vanarian Posted at: 2017-11-27T10:45:45.294Z Reads: 143

```
They have HW 4.xx so cases won't resolve it like HW 6.4 with Alu case (and the standard case is only decent IMHO : raw alu lump + thermal pad with limited temp dissipation is better than nothing but still...). 

Looking forward to see this cooling tunnel!
```

---
## \#30 Posted by: Kug3lis Posted at: 2017-11-27T10:53:59.893Z Reads: 149

```
http://www.electric-skateboard.builders/t/single-vesc-cnc-machined-aluminium-case/38203/
```

---
## \#31 Posted by: GhettoFab.rictation Posted at: 2017-12-28T23:41:05.258Z Reads: 132

```
Alright I'm waiting on my other flat heat sink set to come in. Copper dissipates heat better than aluminum and I have made two heat sink for my antispark switch mosfets! I will also have another heat sink on the top of these as shown with a fan on each side of my vesc pulling air in the shrink wrap onto the mosfet heat sinks. then the air flow will exit out of the switch end with the shrink wrap sealed at the motor wire end. <img src="/uploads/db1493/original/3X/8/3/8366b1174532483613065b310b797a38ea177ec6.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/7/8/7826df73f42289dea7adef37d14e72d13e55a8bf.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/e/3/e3e0fd3144b17924b404a109c1d853df1f535102.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/e/e/ee8c8fa8a95425152a0ade969d24e3c76607c760.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/7/3/736b72fb97184426b9a8fda5034fafce32e7f18b.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/3/5/353f0c6530f1d3671d6b1c167da590762936075e.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/e/9/e9546c14e7c6a0e3a74bec6067c5041966fa5353.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/1/6/163c9308f1b0c3411337ad1fe00f50d709aefab5.jpg" width="690" height="388">
```

---
