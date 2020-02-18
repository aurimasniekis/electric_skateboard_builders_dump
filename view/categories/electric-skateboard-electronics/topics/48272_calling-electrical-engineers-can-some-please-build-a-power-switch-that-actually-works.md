# Calling Electrical Engineers: Can some please build a power switch that actually works?

### Replies: 105 Views: 3359

## \#1 Posted by: evoheyax Posted at: 2018-03-06T02:46:53.989Z Reads: 434

```
I really need some help to figure out why things fail, and fail, and fail, regardless of the design.

It seems like more people than I can count tried the torqueboards anti spark switch with bad results, including myself. There was even a thread created about them failing and many many others chimed in to share their experience. I tried multiple myself, some died a day later, some died within seconds of getting hooked up (not shorted).

I thought maybe it was just this design, so I tried @JdogAwesome's power switch. Everything worked good again for a day and then, same issue. So he found a problem, fixed it, and sent me another one. This one died almost instantly.

With @goldenHusky working on upgrades of the vedder anti-spark switch, I decided to try a 3x direct fet version. All was good for over a month. I used it day in and day out, no issues, until one day, the power switch, a capacitor, and my bluetooth module suddenly blew out at the same time on a steep hill at moderate speed.

So I sent it to the drv wizard, @JohnnyMeduse, to get fixed along with some vescs. Got ti back, and all was good. And now while setting up a new complete with one of my sample decks, before I could even get all of the electronics working (including new motors I'm currently winding),  it blew again.

6 power switches, 3 designs, and running everything within specification, and still... Can't get a power switch that works. And I don't see anyone publicly working on a solution.

My only option at this point is an xt90 loop key. But an led power switch can drastically change a product like mine, where one of the main goals has been to stream line the board into looking more like a normal longboard.

Are there any engineers in the community who want to take on building a power switch?

If someone wants to build it on their own: great.
If someone wants to work with me, we can work out a deal.

The goal though is to get rid of this problem that I and many others have had that really takes away from what builders can create.

Thoughts, comments, and onions are welcomed below!

P.S. Not trying to put either of your 3 on blast. Thank you all for your work on attempting to bring anti spark  power switches to the community. I wish we could find the problem, tweak the design, and get rid of the bugs, once and for all.
```

---
## \#2 Posted by: anorak234 Posted at: 2018-03-06T03:09:10.784Z Reads: 402

```
Best antispark switch:
https://www.amazon.com/XT90-S-Female-Connector-Battery-Charge/dp/B00RVM8U5W/ref=sr_1_1/132-5237862-0097560?ie=UTF8&qid=1520305711&sr=8-1&keywords=xt90s

Never failed anybody who knows how to solder since day one (unless your wire is too long... don't do that).
```

---
## \#3 Posted by: Lospalaz Posted at: 2018-03-06T03:11:39.354Z Reads: 395

```
But the guy specifically wants to make an anti-spark switch with the reliability of an XT-90-S loop key...
```

---
## \#4 Posted by: ZackoryCramer Posted at: 2018-03-06T03:16:10.214Z Reads: 390

```
Yea right. Burned up the internal resistor and male plug the second I connected them on 13s, half-charged. :triumph: Maybe it depends on where you got them from; mine was from amz too in a pack of 5.
```

---
## \#5 Posted by: mmaner Posted at: 2018-03-06T03:17:44.440Z Reads: 386

```
I think the answer is a solid state transformer that automatically removes itself from from the circuit when the optimal amperage load is achieved, but it's above my pay grade. 

As of now I mostly use xt90s loop keys. I use Bestech BMS's with an E-Switch when I can get them.
```

---
## \#6 Posted by: Lospalaz Posted at: 2018-03-06T03:20:59.324Z Reads: 375

```
This is above my pay grade too.  
When you say "solid state transformer," I think, "If it's solid state, how does Optimus Prime turn into a truck?"
```

---
## \#7 Posted by: b264 Posted at: 2018-03-06T03:22:11.686Z Reads: 371

```
[quote="ZackoryCramer, post:4, topic:48272"]
Burned up the internal resistor
[/quote]

That's caused by running it when it's not fully, 100% inserted.  99% is not enough
```

---
## \#8 Posted by: ZackoryCramer Posted at: 2018-03-06T03:23:22.273Z Reads: 358

```
Before I could even push it in entirely, it burned. No load. :dizzy_face:
```

---
## \#9 Posted by: mmaner Posted at: 2018-03-06T03:23:25.403Z Reads: 359

```
Lol, that's great 😀.  I've been thinking if a slideing half deck so you could have a short board or a long board by popping a section out and pushing the 2 halve together using some carbon rails, but haven't had time to anything other than think about it. 

Anyways, I was gonna called the Optimus Grind 😀
```

---
## \#10 Posted by: b264 Posted at: 2018-03-06T03:25:58.821Z Reads: 348

```
How much would one be worth to you that didn't fail?
```

---
## \#11 Posted by: evoheyax Posted at: 2018-03-06T03:28:48.551Z Reads: 343

```
Maybe the most reliable but not the prettiest either...

I have to sacrifice looks for performance as it is to a greater degree than most want, so I need to balance out with good looking parts where I can. A power switch should be one of them...
```

---
## \#12 Posted by: Jebe Posted at: 2018-03-06T03:30:21.649Z Reads: 333

```
Solid state relay
```

---
## \#13 Posted by: ZackoryCramer Posted at: 2018-03-06T03:34:05.731Z Reads: 334

```
@b264 
10$ :joy:

I think, more importantly, we should look at why they fail. From the looks of the electrical industry, we probably aren't experienced enough for high power electronics design from esc's to solid state switch's. Maybe post how you/others blew switches and pictures so the mistakes get around for people to avoid. :hugs: 
I have a eswitch I soldered myself with my own hand-picked components from Jameco and they worked fine, for now. Guess I am in luck. :sweat_smile:
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-03-06T03:35:09.457Z Reads: 327

```
you’re, uh, “special”
```

---
## \#15 Posted by: b264 Posted at: 2018-03-06T03:35:24.174Z Reads: 323

```
[quote="ZackoryCramer, post:13, topic:48272"]
10$ :joy:
[/quote]

This is why the shit fails and we don't want to help design a better one that costs more.
```

---
## \#16 Posted by: Lospalaz Posted at: 2018-03-06T03:38:27.743Z Reads: 335

```
[quote="ZackoryCramer, post:13, topic:48272"]
I have a eswitch I soldered myself with my own hand-picked components from Jameco and they worked fine, for now. Guess I am in luck.
[/quote]

Post BOM.  Post schematic. =P
```

---
## \#17 Posted by: pennyboard Posted at: 2018-03-06T03:57:37.742Z Reads: 328

```
I'm currently studying electrical engineering in university so not a full on engineer yet. But the easiest way to begin to design a reliable anti-spark switch is to figure out what's causing the existing ones to fail, and why. I've personally never used an anti-spark switch, (I have an alternative switch I use) so I'm not to familiar with them, but I am going to take a look at Vedder's design and BOM to familiarize myself with them. Do you have any idea which components on your switch failed and what caused them to fail?
```

---
## \#18 Posted by: Jebe Posted at: 2018-03-06T04:15:09.599Z Reads: 315

```
fets.......
even the supower BMS's with E Switches have trouble fully isolating the voltage ( voltage creeps up - drops when under load when off ) and doesn't switch back on without momentarily shorting across the fet
```

---
## \#19 Posted by: pennyboard Posted at: 2018-03-06T04:26:15.606Z Reads: 314

```


[quote="Jebe, post:18, topic:48272"]
voltage creeps up - drops when under load when off
[/quote]

I'm not sure what you mean. Do you mean that the voltage across the MOSfets slowly increases during operation, or that when the mosfets are switched off, the voltage slowly increases until they short?
```

---
## \#20 Posted by: Jebe Posted at: 2018-03-06T04:27:32.085Z Reads: 308

```
Voltage measured at the output increases to about 33volts under no load. Under load the voltage is dragged down to about 5 volts.
```

---
## \#21 Posted by: myreala Posted at: 2018-03-06T04:49:15.922Z Reads: 297

```
Has anyone tried this SSR?
https://www.mouser.com/ProductDetail/Crydom/D1D100?qs=ftmCDQnBrlNIkJ8oaSttng%3d%3d

Or this one?
https://smile.amazon.com/100A-Solid-State-Relay-SSR/dp/B00KO46YCU?sa-no-redirect=1#customerReviews

Both of those can handle 100A. The first one is tiny compared to any anti-spark you'll see and can handle 100v. It does require some circuitry to use them in a skateboard but form factor would still be comparable to a anti-spark switch.
```

---
## \#22 Posted by: pat.speed Posted at: 2018-03-06T05:01:09.537Z Reads: 289

```
I think a good place to get ideas from would be those ebay escs. The power buttons on those work flawlessly.

EDIT: Iv'e been thinking about this topic for a bit now and I have thought of a potential design for a new Anti-spark. DO NOT GET YOUT HOPES UP THIS IS 90% LIKELY NOT TO WORK and has probably already been tried or is how the current switches are made. I will update you on how this goes once I have tested my idea. Oh and I am still at high-school so I guess that gives everyone even more faith. lol
```

---
## \#23 Posted by: evoheyax Posted at: 2018-03-06T05:02:59.889Z Reads: 290

```
Any help in solving this problem would be be appreciated and I can see what can be done to help with funding :slight_smile:

All I know is in every case, the FETs get stuck in the open position and never close again. What causes this is a mystery to me.
```

---
## \#24 Posted by: pennyboard Posted at: 2018-03-06T05:22:24.830Z Reads: 289

```
I'm actually taking a class that focuses on the physics behind MosFets right now, I'll review the notes and come up with an explanation as to why this might happen. 

By FETs stuck open, do you mean they're stuck as an "open switch" and thus the anti-spark is always in the "off" position?
```

---
## \#25 Posted by: pat.speed Posted at: 2018-03-06T05:24:49.697Z Reads: 282

```
Pretty sure he means closed position, well thats the most common thing Iv'e seen happen
```

---
## \#26 Posted by: ZackoryCramer Posted at: 2018-03-06T05:35:55.283Z Reads: 290

```
Nothing special. Just took the Fechter's :sweat_smile: design with matched components:

![image|665x500](upload://sXVQQe9beWjxN8yzzRaw1adPLDt.jpg)

I used this N-channel [fet](https://www.jameco.com/z/IRFZ44N-Major-Brands-Mosfet-IRFZ44N-TO-220AB-N-Channel-55V_669951.html) and these [diodes](https://www.jameco.com/webapp/wcs/stores/servlet/ProductDisplay?catalogId=10001&freeText=36169&langId=-1&productId=36169&storeId=10001&krypto=gWnFu6qu3aeAY%2F7QFXrttQhYJoL42%2BzvdHCihpjO2VVvmrpLwvgCGHpuhbz4lvHv2TX2LB3U60w%2BpKBL%2B4Y%2FuIyJqOkhKpAmS9jZP8TSmfM%3D&ddkey=https%3AStoreCatalogDrillDownView). I used only two fets in paralle though. :space_invader:
```

---
## \#27 Posted by: PXSS Posted at: 2018-03-06T05:38:18.794Z Reads: 276

```
You mean Fetcher design...
```

---
## \#28 Posted by: evoheyax Posted at: 2018-03-06T05:48:01.247Z Reads: 272

```
I've been told to think of the fet as a gate. The more the gate is open, the more electricity comes through. And thus when you get your batteries full voltage through the power switch, the fet is open and electricity flows.

If I'm wrong, please correct me :)
```

---
## \#29 Posted by: chuttney1 Posted at: 2018-03-06T05:48:54.312Z Reads: 266

```
None of this is required if you get yourself a BMS with a precharge function.
```

---
## \#30 Posted by: evoheyax Posted at: 2018-03-06T05:50:00.479Z Reads: 266

```
Please explain to me what is a precharge function? My solution to balancing is simple: A balancing board. Let the switch turn the board off and on and the vesc's to limit current and protect from under voltage.
```

---
## \#31 Posted by: chuttney1 Posted at: 2018-03-06T06:04:53.368Z Reads: 320

```
Exactly what the VESC anti-spark switch is. The photo posted by ZackoryCramer 4 comments above this one is titled "inrush limiter". The gist is it controls current over time such as 1 millisecond to prevent destroying sensitive electrical components. Now here the funny thing, an appropriately sized capacitor fits this category of controlling current that people in the RC community just use more capacitors and problem solved for preventing ESC destruction. But we have the electric skateboard with caps near ESC. The MOSFETs on the BMS does the job of controlling current output in the beginning. 


Side note. On my setup, my BMS has this feature and I just use a 50 amp LP J Case Fuse. It sparks, but it's contained within the case.


I understand you want an option as simple as a flick of the switch, but to increase the reliability of the circuit someone has to run a SPICE simulation to isolate the problem with the mosfet. The Zener diode, capacitor, and resistors are the least of your worry. I remember some post saying there is a specific type of Mosfet that can handle this Other than it being known as an N-Channel Mosfet.
```

---
## \#32 Posted by: Deckoz Posted at: 2018-03-06T06:07:39.829Z Reads: 315

```


[quote="chuttney1, post:31, topic:48272"]
option as simple as a flick of the switch
[/quote]

Flick this switch...

![image|666x500](upload://vWZEFd2TzSzHOo6J3geNeHf96LL.jpg)

AS150 antispark bullet...in a switch... its effectively a loop key you can't loose..

PS it's the size of one 18650...
```

---
## \#33 Posted by: Jc06505n Posted at: 2018-03-06T06:26:03.708Z Reads: 301

```
Can we see how that fits into your board/build for design perspectives ?
```

---
## \#34 Posted by: Deckoz Posted at: 2018-03-06T06:36:40.442Z Reads: 301

```
Don't have it installed yet.

But you could just "add another cell" to your battery pack size and just attach it to the end of your battery, redesign the panel part of the switch so the hole is only as big as the switch opening. And basically have the antispark built into the battery with a mechanical slide underneath the bottom side of the enclosure.
```

---
## \#35 Posted by: ervinelin Posted at: 2018-03-06T06:51:33.158Z Reads: 296

```
From what I recall there is a voltage drop across the relay. Also you'll need to find an alternative power supply to turn on and off the relay.

I bought one, then gave up and went back to XT90 antispark loopkey.
```

---
## \#36 Posted by: Lospalaz Posted at: 2018-03-06T07:25:51.438Z Reads: 288

```
Post BOM!  Post STL!  Post schematic!  =P Where's the resistor that limits the current?
```

---
## \#37 Posted by: b264 Posted at: 2018-03-06T07:33:06.398Z Reads: 289

```
The saturation of the FETs is what limits the current as C1 charges up via R2

Oh, I thought you were talking about @ZackoryCramer's schematic, sorry
```

---
## \#38 Posted by: Lospalaz Posted at: 2018-03-06T07:49:06.528Z Reads: 279

```
Nope, talking about @Deckoz ^_^
```

---
## \#39 Posted by: Lospalaz Posted at: 2018-03-06T07:52:31.298Z Reads: 285

```
...With 5 Hours into the thread:

@Deckoz has a good design, but no details. @chuttney1 has stunned with his "just add more caps" observation and @ervinelin has disqualified solid state switches, and soooo... 

@ZackoryCramer has the lead.  Because he's special =P

Can @Deckoz make a comeback?
Will we ever solve the mystery of the faulty anti-spark switches?
The thread is just getting started, folks!
```

---
## \#40 Posted by: E1Allen Posted at: 2018-03-06T08:29:51.558Z Reads: 278

```
So my 6s lipo spark inside my charger.  So to stop that I just plug in 3s for a second then 6s.  

Any way to precharge the caps with a lower voltage.
```

---
## \#41 Posted by: b264 Posted at: 2018-03-06T08:44:46.041Z Reads: 266

```
Adding more capacitance to the VESC will make it worse.  Also, don't add less...

Adding more capacitance to the antispark switch or upping the resistor value would increase the turn-on time, decreasing the current spike, increasing the longevity of the parts
```

---
## \#42 Posted by: Jebe Posted at: 2018-03-06T09:33:46.106Z Reads: 261

```
Used both. No problems. 100 amps minimum though. Have had 40 amp units fail after a week.
```

---
## \#43 Posted by: Lospalaz Posted at: 2018-03-06T09:34:19.665Z Reads: 264

```
Was he was talking about more caps on the VESC...?

Can't update the rankings until this is hashed-out... T_T
```

---
## \#44 Posted by: Jebe Posted at: 2018-03-06T09:38:19.870Z Reads: 262

```
I use a bms and use the 6s voltage connection from the bms as the switching voltage for the SSR. Measuring with a DC ammeter measures less than 0.05 amps. Will measure again with a 4-20ma meter when I remember.
No voltage drift in the pack as yet.
```

---
## \#45 Posted by: ervinelin Posted at: 2018-03-06T09:41:24.472Z Reads: 258

```
Can I know what do you mean you use the 6S voltage connection from BMS?
```

---
## \#46 Posted by: Jebe Posted at: 2018-03-06T09:42:31.030Z Reads: 257

```
Use the 24 volts from the 6s wiring back to the BMS
```

---
## \#47 Posted by: ervinelin Posted at: 2018-03-06T09:43:27.610Z Reads: 250

```
Do you mean if your battery pack is 10 or 12S you tap off the first 6S?
```

---
## \#48 Posted by: ElskerShadow Posted at: 2018-03-06T11:00:37.167Z Reads: 256

```
I have a 3 MOSfets antispark with XT90, 80A fuse with 12S from eskating and it works great so far.
```

---
## \#49 Posted by: banjaxxed Posted at: 2018-03-06T11:34:05.232Z Reads: 266

```
![image|295x228](upload://bPKb3cQ63UeuQmrUf8GLlq142Jo.jpg)Why yes, ve have something



![image|391x285](upload://k5uBoQisRqoRQfIfTS3BgL2ixz1.jpg)
```

---
## \#50 Posted by: e.board_solutions Posted at: 2018-03-06T11:38:54.294Z Reads: 268

```
Made these with @fottaz antispartk PCB's :slight_smile:  

![image|375x500](upload://7WjluTyPojWJk9za1GpUIwHPgM9.jpg)
![image|375x500](upload://pLZCzwheQZM4yYWgWmpHznrMWx6.jpg)
```

---
## \#51 Posted by: Alex.Scheff Posted at: 2018-03-06T12:16:47.760Z Reads: 262

```
More informations please
```

---
## \#52 Posted by: Deckoz Posted at: 2018-03-06T13:59:09.588Z Reads: 261

```
I gave you all the details you need it's literally two items. Just as simple as a loop key... 

[quote="Deckoz, post:32, topic:48272"]
AS150 antispark bullet…in a switch
[/quote]


As150 antispark bullet
3d printed switch. 

The guy that started the thread asked for a bullet proof idea. There it is. Now if he wants it HE can make it for HIS product.

No details haha.. more like you didn't expect a simple solution with only two parts. 

https://www.amazon.com/dp/B00RVM93YO/ref=cm_sw_r_cp_apa_K9PNAbJC2WN5P
```

---
## \#53 Posted by: Blitz Posted at: 2018-03-06T14:05:16.467Z Reads: 258

```
I had the same Idea! thought I'd make it from wood. ditched the idea when I noticed it's tough to pull the xt90 anti spark key out! Like your design and the use of bullets.
```

---
## \#54 Posted by: GrecoMan Posted at: 2018-03-06T14:11:49.392Z Reads: 257

```
relax....
put the 3d file on thingiverse and make all us happy 😉
```

---
## \#55 Posted by: Deckoz Posted at: 2018-03-06T14:25:06.224Z Reads: 256

```
Maybe, after I have some miles on it. 

Either way the AS150 has threads to hold it in place.. It's a simple model. I'm sure you could whip one up in a few minutes Greco...
```

---
## \#56 Posted by: GrecoMan Posted at: 2018-03-06T14:27:55.157Z Reads: 254

```
or optimize it in a tiny package and sell it 🤔
```

---
## \#57 Posted by: Deckoz Posted at: 2018-03-06T14:37:39.814Z Reads: 256

```
It's the size of an 18650...

It's probably smaller then most antispark footprints for fitment with connectors attached...lol just change the panel mount so it drops inside- out. Instead of outside-in like it is currently.
```

---
## \#58 Posted by: GrecoMan Posted at: 2018-03-06T14:38:25.176Z Reads: 253

```
i have an idea
```

---
## \#59 Posted by: cosmicc89 Posted at: 2018-03-06T14:48:31.935Z Reads: 252

```
What is wrong with the solid state relay idea? Use the tiniest buck converter you can find to drop the voltage off your main battery to say 5 or 12v, then use any illuminated switch you want. The switch activates low voltage to the relay, the relay then switches main power to the ESC/VESC. Easy peasy.
```

---
## \#60 Posted by: Deckoz Posted at: 2018-03-06T14:50:51.158Z Reads: 246

```
@cosmicc89  Size.

Is always the problem.
```

---
## \#61 Posted by: mmaner Posted at: 2018-03-06T14:51:29.457Z Reads: 240

```
[quote="Deckoz, post:60, topic:48272"]
Size.  Is always the problem.
[/quote]

thats what she said :slight_smile:
```

---
## \#62 Posted by: Vanarian Posted at: 2018-03-06T14:54:40.113Z Reads: 243

```
@Deckoz my bro we use the same G502 mouse ! It's unkillable and super ergonomic right ?

On topic  @evoheyax did you put a **fat** airflow cooled heatsink on your 3 direct fet version or simply ran it with the small one mounted by @GoldenHusky ?

I don't know if the FETs go dirty because they can't cope with inrush speed or if they simply fry due to instant / prolonged heat or get damaged over time by ramping heat ?

Cause if the failure doesn't come from the FET limited speed, then how about thinking of cooling the anti-spark just like you'd cool your ESC guys. I mean **all** of your battery power runs through it **dry and hard** like we like it (don't say you don't like, else you wouldn't be pressing that throttle so much).

Just a suggestion, not a solution (I don't have enough tools to probe failure points on anti-sparks unfortunately).

Edit : Note that I submit this point because you may notice how hot connectors are just after a spark. I suppose a similar reaction can occur even upon connection and shoot the FET down.
```

---
## \#63 Posted by: JdogAwesome Posted at: 2018-03-06T15:26:47.861Z Reads: 235

```
Thanks for tagging me @evoheyax I've been wanting to find an answer to this for a while now. To start I know almost for a fast the FET's aren't dying to due to heat or prolonged over current because I ran my board on a single MOSFET switch I made for months and it never even got warm. Now I've been running my dual hub motor build on a dual IRFS7730 switch I also built and again, it doesn't even get warm. Now like I said I have always used Hub Motors so I can't speak for geared builds. I think the problem lies with the voltage spikes from the inductive load and the high peak voltages from regenerative braking. It could also potentially be high inrush current for the capacitors, but like I said I'm not sure. Oh and on both of my switches there is no added capacitance to the gate for a slower ramp up speed.
```

---
## \#64 Posted by: Deckoz Posted at: 2018-03-06T15:39:47.013Z Reads: 236

```
[quote="JdogAwesome, post:63, topic:48272"]
I think the problem lies with the voltage spikes from the inductive load and the high peak voltages from regenerative braking
[/quote]

I would agree with this. 

The FETs on both the vesc and the Antispark don't know the voltage of the system. They just act almost like a bidirectional buck converter. During regeneration the initial spike of voltage, reversing the flow of energy has a period before the electrons hit the pack after passing from vesc to antispark to battery. As the electrons reach the battery a reverse "load" is applied to the system. Load always causes voltage drops, so the battery is absorbing and pulling down the voltage spike.

In order to fix this. You need to size the capacitor rail on the vesc for the system. As currently the cap rail is for protection of the vesc only. More capacitance will absorb these spikes, or add a reverse current  one way TVS diode to shunt the transients from reaching the antispark.
```

---
## \#65 Posted by: evoheyax Posted at: 2018-03-06T15:42:48.244Z Reads: 227

```
[quote="b264, post:41, topic:48272"]
Adding more capacitance to the VESC will make it worse
[/quote]

Can you explain why this is? I was recently experiencing voltage sagging due to capacitors fully draining and then not having any juice left to deal with voltage fluctuation. So I've doubled up the number of caps on vesc's as a result, problem solved... What can happen with too much capacitance?
```

---
## \#66 Posted by: Deckoz Posted at: 2018-03-06T15:44:00.282Z Reads: 233

```
He just means the spark will be bigger without an antispark(ie worse). But it should help in regards to transients suppression.
```

---
## \#67 Posted by: evoheyax Posted at: 2018-03-06T15:45:16.360Z Reads: 228

```
What I'm looking for is an anti-spark circuit that involves an led power switch... I mentioned in the first post the xt90 loopkey is what I'm stuck with for now, but that I'm looking for a better solution. Still don't see a better solution so far ;)
```

---
## \#68 Posted by: Deckoz Posted at: 2018-03-06T15:52:09.268Z Reads: 244

```
Hey that's fine. You could make a model like mine with an led in the head of the switch and contacts on the backside with an inline SMD resistor to apply the right voltage for the LED

You said it yourself, loopkeys don't fail. Most people's issue is you can loose your loop key, it sticks out, and it's tacky. I simply offered an idea... A loopkey you can't loose that looks like a switch. Make a micro pcb to sit in the switch head for an LED. I know it's not a button, but you didn't say button in the OP, you said switch

[quote="evoheyax, post:1, topic:48272"]
an led power switch can drastically change a product like mine, where one of the main goals has been to stream line the board into looking more like a normal longboard.

Are there any engineers in the community who want to take on building a power switch?
[/quote]

.. you could modify it to be a button from the side, with springs.

Add a spring.. ![received_10155148479166105|666x500](upload://u79mnN8lFgJqg1uV1FY2QUqgZ8B.jpg)

Spring is not strong. Just strong enough to keep it open while open so it doesn't "bounce". But really you could easily turn this into a button type...
```

---
## \#69 Posted by: PXSS Posted at: 2018-03-06T23:55:12.198Z Reads: 230

```
IF the issue is the voltage spike when turning on due to inrush current to the vesc. Adding additional caps to the ESC would make it worse as it needs more energy to fill up those capacitors and the voltage spike would be larger. I'm almost certain that's what @b264 meant.
```

---
## \#70 Posted by: b264 Posted at: 2018-03-07T00:06:52.174Z Reads: 226

```
[quote="evoheyax, post:65, topic:48272"]
What can happen with too much capacitance?
[/quote]

On powerup, you stress your antispark electronic switch or your loopkey resistor more, but the ESC should perform better.  If you don't have failing e-switches or loopkey resistors, it's better as long as you don't overdraw your battery on powerup.  Having a longer ramp-up on an electronic antispark switch could remedy that.
```

---
## \#71 Posted by: Deckoz Posted at: 2018-03-07T00:07:50.694Z Reads: 220

```
But it's not a voltage spike outward from the battery that would be higher then the originating voltage. Voltage from the battery will always be voltage from the battery

Voltage spikes on bldc systems when you reverse torque, can quickly rise if the resistance of your pack is to high to accept the incoming current.
```

---
## \#72 Posted by: deucesdown Posted at: 2018-03-07T00:20:42.032Z Reads: 220

```
[quote="Deckoz, post:71, topic:48272"]
Voltage spikes on bldc systems when you reverse torque, can quickly rise if the resistance of your pack is to high to accept the incoming current.
[/quote]

This would show up on Ackmania's app, no? I'm looking at my graph for today, and a hard brake shows maybe a 2v rise. Unless it's transient. Very curious about this, mayb enough to put a tiny battery powered o-scope on it...
```

---
## \#73 Posted by: Deckoz Posted at: 2018-03-07T00:25:31.388Z Reads: 215

```
I'm not sure the STM32 reads fast enough to capture these. I would scope three different areas.

On a phase pair.
After the vesc  before the cap rail
After the cap rail.

You'll need load to do this. But it will tell you what is being absorbed by the vesc SMD caps, what is absorbed by the cap rail, and what is making it through the cap rail to the AS or battery.
```

---
## \#74 Posted by: Sapphirinia Posted at: 2018-03-07T00:36:20.166Z Reads: 208

```
Whatever @akhlut did seems to work. I've had it for at least 6 months or so and it's never had any issues. I think he uses a little board as part of it.
```

---
## \#75 Posted by: akhlut Posted at: 2018-03-07T00:44:40.158Z Reads: 208

```
Its just a vedder switch, nothing fancy.  Im using loop keys now - less to worry about.
```

---
## \#76 Posted by: evoheyax Posted at: 2018-03-07T00:50:40.384Z Reads: 208

```
It really depends on how hard you push them. I do high amps at high voltage, and this is the trend I’ve seen with these anti spark failures.
```

---
## \#77 Posted by: evoheyax Posted at: 2018-03-07T00:52:33.181Z Reads: 211

```
How can I add a longer run up?
Are there any simple solutions? The problem is not lid cause I’ve blown out 3 different anti spark switches on the bench, and I did not turn them off and on quickly, I always let them drain.
```

---
## \#78 Posted by: b264 Posted at: 2018-03-07T00:56:34.034Z Reads: 204

```
[quote="evoheyax, post:77, topic:48272"]
How can I add a longer run up?
[/quote]

In the [schematic](https://www.electric-skateboard.builders/t/calling-electrical-engineers-can-some-please-build-a-power-switch-that-actually-works/48272/26) @ZackoryCramer posted, I would double or triple the capacitance of C1

(if you have a different schematic, please post it)
```

---
## \#79 Posted by: ervinelin Posted at: 2018-03-07T01:06:49.486Z Reads: 203

```
This is interesting, have you used it for a while and proven it to be reliable over multiple uses? My worry is the alignment might be difficult or gets sloppy after the moving parts wear down over extended use
```

---
## \#80 Posted by: PXSS Posted at: 2018-03-07T01:39:18.783Z Reads: 214

```
[quote="Deckoz, post:71, topic:48272"]
But it’s not a voltage spike outward from the battery that would be higher then the originating voltage.
[/quote]
Not quite. The voltage spike can be up to twice as high as the battery voltage. I've killed fets rated upwards of 100V with a 60V battery because the system did not suppress the inrush spike. 

Here's an example:
![image|666x500](upload://u1ADtNPwM0syNSt4BQzpOYGMkQr.jpeg)

Yellow line, is scoping before the switch and red after the switch. This is after I already implemented a fix to reduce the voltage spike. As you can see red can go above the input voltage.

Electrical engineering ain't easy or intuitive...

@deucesdown, spikes like these are transient and can be as short as a few 100 nanoseconds, so your ESC would never be able to record them. An oscilloscope is sampling at upwards of 100khz, (I think in the mhz range, not really sure)

---
This is also why you really should not run 13S on VESC without extensive testing that it won’t burn your components. Most of the components in it are rated to 63V and there isn’t much overhead for voltage spikes like the ones above.
```

---
## \#81 Posted by: deucesdown Posted at: 2018-03-07T01:54:50.047Z Reads: 209

```
This video precipitated yet another impulse purchase a while back

https://www.youtube.com/watch?v=fGU9LoEpQFw

Seems I may get some use out of it. Though maybe after it warms up a bit.
```

---
## \#82 Posted by: darkkevind Posted at: 2018-03-07T01:56:05.474Z Reads: 211

```
My solution has been working flawlessly for about 2 years now... Used regularly...

![20180307_015033|666x500](upload://6C324xhGQXRID6vduwMZuyzeUJN.jpg)

![20180307_015051|666x500](upload://qviY8YjJLfSmovi3EUsQh6zuFBJ.jpg)

It's a double (momentary) latching coil, single throw 120A relay.
It takes it's power from the main battery with an inline voltage regulator to drop the voltage to the coil voltage which is 24v.
Hook it up to an on/off/on momentary rocker switch and you're golden.
Doesn't use any current whilst on or off as it's latching both ways.
Allows full current from battery to flow with no voltage drop.
```

---
## \#83 Posted by: deucesdown Posted at: 2018-03-07T02:00:50.067Z Reads: 205

```
Come on don't tease, part number or link please :)
```

---
## \#84 Posted by: darkkevind Posted at: 2018-03-07T02:02:42.379Z Reads: 208

```
I can't actually find this exact one anymore! :frowning:

But if you search digikey or rs components and I think Mouser just look for a DPST latching relay. Choose your desired max current rating...


Latching Relay 80A meter relays coil 12VDC
 http://s.aliexpress.com/iuqa2I7j

Latching Relay 100A meter relay with big shunt
 http://s.aliexpress.com/qMfyeMne
```

---
## \#86 Posted by: PXSS Posted at: 2018-03-07T02:09:59.461Z Reads: 212

```
Link from another thread...
Although wayyy expensive 

[quote="PXSS, post:116, topic:38869, full:true"]
https://www.digikey.com/product-detail/en/crydom-co/D06D60/CC1521-ND/353616

Here, solved
[/quote]
```

---
## \#87 Posted by: deucesdown Posted at: 2018-03-07T02:12:46.620Z Reads: 208

```
This was linked in post 21 above. A whole benjamin! He linked a $23 one on amazon. IIRC AvE taught us we best get brand name versions of stuff like this.

Oh, edit, the latching relay has no passive current draw. I didn't think they were affordable/small enough for us.
```

---
## \#88 Posted by: PXSS Posted at: 2018-03-07T02:16:15.649Z Reads: 203

```
[quote="deucesdown, post:87, topic:48272"]
IIRC AvE taught us we best get brand name versions of stuff like this.
[/quote]

AvE has taught us not to anger the pixies and to keep our dicks in a vise!
```

---
## \#89 Posted by: briman05 Posted at: 2018-03-07T02:20:57.806Z Reads: 207

```
I feel like a toggle switch is more reliable then the push button as a push button will fail a lot quick because it is basically a button that has like a small spring in it. Where the toggle switch is a literal switch of a on off position that should not fail. How does boosted do it because I don’t think I have ever seen a boosted switch fail. I’m not a electrical engineer but I feel like if someone took apart a boosted and then saught out the parts out that boosted uses it could really make a better switch it would be basically reverse engineering it. I think is someone steps up maybe everyone sends any dead switches to them so they can see what could be the causes them to fail.
```

---
## \#90 Posted by: darkkevind Posted at: 2018-03-07T02:24:50.154Z Reads: 206

```
It's not the mechanical switch that's failing, it's the high current throughput switch that keeps failing.

The little push button or rocker switch to activate the FETs isn't the issue here...
```

---
## \#91 Posted by: deucesdown Posted at: 2018-03-07T02:28:12.674Z Reads: 210

```
https://www.youtube.com/watch?v=ftJ17Cp6itw

OMG he sharpied a "F" in front of RIGOL... ROFL.

Anyway, not the same but along the same lines.
```

---
## \#92 Posted by: mmaner Posted at: 2018-03-07T02:37:59.775Z Reads: 209

```
[quote="briman05, post:89, topic:48272"]
I don’t think I have ever seen a boosted switch fail.’
[/quote]

That's because you are limited to 30a throughout. We are pushing up to 80.
```

---
## \#93 Posted by: chuttney1 Posted at: 2018-03-07T07:13:12.002Z Reads: 206

```
Transient voltages from powering up are easily seen with an oscilloscope on the millisecond range. It cannot be seen to be seen in the Ackmania's App because the VESC is power on. The transient voltages from running should be seen if you went from full speed to full stop as fast as you can.
```

---
## \#94 Posted by: Alex.Scheff Posted at: 2018-03-07T18:00:31.432Z Reads: 198

```
Could [this](http://s.aliexpress.com/QNRfmIFV?) work? :joy:
```

---
## \#95 Posted by: PXSS Posted at: 2018-03-07T19:45:33.008Z Reads: 196

```
Top mount it!
```

---
## \#96 Posted by: Alex.Scheff Posted at: 2018-03-07T19:55:46.727Z Reads: 195

```
Thats my plan :wink:
```

---
## \#97 Posted by: b264 Posted at: 2018-03-07T20:00:03.010Z Reads: 200

```
[quote="Alex.Scheff, post:94, topic:48272"]
Could [this](http://s.aliexpress.com/QNRfmIFV?) work? :joy:
[/quote]

Yes, probably!  That might be one of the very, very few mechanical switches that will.  As far as fashion and looks go, it gets an F
```

---
## \#98 Posted by: deucesdown Posted at: 2018-03-07T20:04:05.965Z Reads: 203

```
There are "boat"loads of mechanical switches that would work (search for marine dc switch). They're all huge. There are even some circuit-breaks that are designed to use as a switch, that would work very nicely, give you some fuse action to go with it. The mechanical switches are big because as you up the voltage and amperage especially for DC, you need bigger air gaps to prevent arcing.

Love this video.

https://www.youtube.com/watch?v=Zez2r1RPpWY
```

---
## \#99 Posted by: GrecoMan Posted at: 2018-03-08T17:35:44.255Z Reads: 192

```
hehehe i see what you did there 😉
```

---
## \#100 Posted by: Toohat Posted at: 2018-07-13T22:48:52.265Z Reads: 145

```
Will this work? 
https://www.amazon.ca/gp/product/B07DKY2WW3/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1
```

---
## \#101 Posted by: Acido Posted at: 2018-07-13T22:56:53.606Z Reads: 143

```
Just get a bestech bms with an e switch
This is huge and it will look ugly but it should work
```

---
## \#102 Posted by: Gamer43 Posted at: 2018-07-14T09:04:52.879Z Reads: 133

```
Low side switching without transient suppression.

A proper solid state switch should use high side switching with a TVS diode. 
A chip like the ltc7000 and a high power mosfet (NONE OF THAT INTERNATIONAL RECTIFIER SHIT) will do the job, be sure to include a TVS diode.

LTC7000 is a high side static mosfet driver with inrush current limiting functionality.
```

---
## \#103 Posted by: zhud Posted at: 2018-07-19T15:28:32.967Z Reads: 121

```
I’m using something similar and have zero problems
```

---
## \#104 Posted by: Toohat Posted at: 2018-07-27T19:32:39.514Z Reads: 101

```
![IMG_0074|375x500](upload://3IwBbxL6JCP8KeOvKpG1YZn9Pd2.JPG) it looks really good actually
```

---
## \#105 Posted by: Toohat Posted at: 2018-07-27T19:33:28.869Z Reads: 100

```
Yeah I installed it and it works really well
```

---
## \#106 Posted by: Toohat Posted at: 2018-07-27T19:33:39.992Z Reads: 97

```
thanks guys
```

---
