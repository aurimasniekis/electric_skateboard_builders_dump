# Float charging &amp; why you shouldn&rsquo;t bypass the BMS

### Replies: 49 Views: 3033

## \#1 Posted by: chaka Posted at: 2017-12-01T17:09:38.138Z Reads: 403

```
Many more builders are using huge packs today, two years ago stuffing 60+ cells in a board would likely get you blasted on the forums for not needing the range and having a heavy board but people are beginning to see the benefits and going big. 

Maintaining a large pack is a little different than 100 to 200 watt-hour pack. Most BMS circuits only output around .09 amps when balance charging which may work fine for a XXs1p battery but it takes many times longer to balance a larger battery with big P groups. Overtime insufficient balance charging will lead to a large enough drop in voltage to significantly reduce your range due to the low cell voltage cut-off found in a good BMS. 

 In this scenario, if the board has a bypassed BMS, you are running the risk of dropping the cell voltage below recommended levels and damaging the cells or worse. I have noticed many builders now using this method and relying on the VESC software to do all low voltage monitoring without any fail safe or accounting for individual cells. This may seem like a sparkling idea on a fresh board and battery but life is never perfect, cells will drift and if you are not monitoring your cells you need to be using a BMS and leaving it on the charger longer once it reaches its target voltage.

It can take weeks for a BMS to balance a large pack if it has drifted significantly. .09 amps is a snails pace when charging a 500+ watt-hour pack. Keep this in mind next time you hear the fan in your power supply turn off, that is usually the moment the charger has reached the target voltage and float charging commences.
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-12-01T17:25:32.796Z Reads: 388

```
This is great info. Thank you. So this is the case even though the light turns green? The bms is still balancing?
I’m using a torqueboards 12s3p it occurred to me that my range was lower than I thought it should be. It’s pretty cold here now though and i’m using six shooters.
```

---
## \#3 Posted by: chinzw Posted at: 2017-12-01T17:31:40.123Z Reads: 377

```
depends on your bms, but yes, most of the time it will still be balancing even when the charger goes green.
```

---
## \#4 Posted by: egzplicit Posted at: 2017-12-01T17:39:20.999Z Reads: 362

```
It's worth noting that (at least) a Bestech BMS will start balancing as soon as a group hits 4.2v and once a charger goes green, even if you unplug it right after that, the BMS will still balance the pack. I had a chat with the Bestech guys and they confirmed balancing happens even when the charger is unplugged.
```

---
## \#5 Posted by: chsknight Posted at: 2017-12-01T17:43:01.286Z Reads: 351

```
How much drift has anyone actually observed here?  As long as we bottom balance the cells, then they should stay relatively in sync right?  I can see this being a problem with LIPO's but not with 18650s.
```

---
## \#6 Posted by: Hummie Posted at: 2017-12-01T17:43:39.987Z Reads: 342

```
it seems very rare for people to have balancing done by any other method than just discharging balancing cells only when they hit 4.2 and when this happens its a very slow discharge balancing.  With this method if youre charging fast the whole pack voltage will rise to the whole pack cut-off voltage and some cells are too high and then come down slowly so you might have cells at as an example: 4.0,4.0,4.3,4.3....  and the discharger function keeps going even off the charger as just said.  so you now have 4.0,4.0,4.2,4.2.    A very slow charge must be done to truly balance.  But i havent used mine yet to see how it plays out or to see what kind of drift happens with li-ion
```

---
## \#7 Posted by: briman05 Posted at: 2017-12-01T18:29:16.862Z Reads: 321

```
I would think that you would want a charger that can do 3 to 4A when charging you never want something super fast at charging as you will burn out the cells but you also dont was 1A or maybe even 2A because it will take someone a very long time to charge totally.  Now I might be wrong but I believe if you have a 4p battery and a 2A charger it will do .5a per P.
```

---
## \#8 Posted by: E1Allen Posted at: 2017-12-01T18:40:39.764Z Reads: 314

```
When did people start straying away from balance chargers with balance leads on each pack
```

---
## \#9 Posted by: Achmed20 Posted at: 2017-12-01T18:49:06.404Z Reads: 307

```
i dont get that either. its usualy jsut bypassed while using the pack, not while charging it.
everything else would be "skipping" the BMS alltogether.

edit: dont paralel packs balance each other anyway??
```

---
## \#10 Posted by: onepunchboard Posted at: 2017-12-01T19:10:46.339Z Reads: 296

```
Parallel pack self balance itself for lion tho. not sure on lipo but then they dont voltage sag much and cheep
```

---
## \#11 Posted by: STREETSURFER Posted at: 2017-12-01T19:15:14.586Z Reads: 294

```
That is what I do on my build. I have two 6s4p lg hg2 packs that I charge up individually, and discharge together as 12s4p.
```

---
## \#12 Posted by: chaka Posted at: 2017-12-01T19:56:58.368Z Reads: 291

```
You are not hearing me correctly, I am talking about the charge rate while on a float charge. It is related to how much your BMS can burn off with the balancing resistors.

@Achmed20 you are correct parallel cells will discharge as one. The point I am trying to get across is the fact that a large parallel group will take forever to bring back into balance with the .09 amps a BMS will provide and if you do not pay attention you could end up with a dangerously low cell if you do not have any other fail safe than the VESC low voltage settings.
```

---
## \#13 Posted by: jmasta Posted at: 2017-12-01T20:45:26.059Z Reads: 285

```
I charge and discharge through a 12S BMS.  But I also build my packs so they can be disconnected from the BMS and broken down into 6S sub-packs. Basically it's 2x 6S4P connected in series. So then you can also service the pack with a balance charger if needed. Best of both worlds
```

---
## \#14 Posted by: treenutter Posted at: 2017-12-01T21:13:02.230Z Reads: 279

```
Thanks @chaka this is great info. I think we need to clear up some nomenclature:

**Standard use of BMS**: BMS is connected to pack for charging and discharging. Discharge rate is limited to BMS discharge capacity.

**"Bypassing" BMS**: Describes using a BMS for charging but bypassing for discharge. Allows for a cheaper and smaller BMS

**Skipping BMS**: No BMS is used at all. Cells are charged and discharged directly 

I've never quite understood how discharge through the BMS works to protect the cells. Does a typical BMS have the ability to monitor and control P group output? (I still discharge through BMS, because I've understood it to provide additional safety, but I admit that "I don't get it.")
```

---
## \#15 Posted by: darkkevind Posted at: 2017-12-01T21:21:07.897Z Reads: 268

```
Unless cells degrade, it's impossible for individual cells in a parallel pack to not be balanced...

As soon as you place cells in parallel they will automatically start to balance themselves, so inherently blasting some current in to one of those cells (in parallel) (which you can't actually do because they're all connected, but let's pretend you can), will be shared evenly amongst the parallel cells...
```

---
## \#16 Posted by: darkkevind Posted at: 2017-12-01T21:24:26.637Z Reads: 265

```
[quote="treenutter, post:14, topic:39879"]
Does a typical BMS have the ability to monitor and control P group output?
[/quote]

Yes, the BMS monitors all the parallel cells (s) and if one of those cells drops below the cutoff voltage the power will be regulated or cut. If your pack isn't well made, one or more cells in series could discharge at a faster rate than the others, therefore their voltage could drop to the cutoff level quicker than the others...
```

---
## \#17 Posted by: chaka Posted at: 2017-12-01T21:29:55.068Z Reads: 256

```
For the sake of not derailing the thread please think of a parallel group as 1 cell. When we talk about cell voltage monitoring we are talking about one parallel group not the individual cells. 

@treenutter The BMS will cut power if 1 cell/"p group" drops below a specific voltage. If you bypass the BMS you lose this fail-safe.
```

---
## \#18 Posted by: thisguyhere Posted at: 2017-12-01T21:30:00.673Z Reads: 262

```
[quote="chaka, post:1, topic:39879"]
you need to be using a BMS and leaving it on the charger longer once it reaches its target voltage
[/quote]

i just leave the board charging over night, at least 10 hours, to ensure the float brings all P group into balance.  at least that's what i picture is happening.
```

---
## \#19 Posted by: thisguyhere Posted at: 2017-12-01T21:30:54.871Z Reads: 260

```
[quote="chaka, post:17, topic:39879"]
The BMS will cut power if 1 cell/"p group" drops below a specific voltage
[/quote]

oh yea, learned this the hard way

https://www.electric-skateboard.builders/t/ate-shit-today-and-loop-keys/33613/30
```

---
## \#20 Posted by: chaka Posted at: 2017-12-01T21:34:56.235Z Reads: 259

```
That's why a set my soft at 3.3v and hard at 3v and leave the BMS as a secondary governor. Same with the over current.
```

---
## \#21 Posted by: egzplicit Posted at: 2017-12-01T21:36:03.644Z Reads: 259

```
[quote="treenutter, post:14, topic:39879"]
I've never quite understood how discharge through the BMS works to protect the cells. Does a typical BMS have the ability to monitor and control P group output?
[/quote]

It can't control individual amps on P groups, however, it can monitor their voltage. So discharging using a BMS has the following extra layers of protection:

* Offers protection against short circuits: a short circuit will cause high Amps to be drawn from the BMS and that will cause it to shut down immediately. A fuse might do the same, but a fuse is sometimes much slower to react
* Offers protection against low voltage on individual groups: if for some reason one of your parallel group discharges at a faster rate than others, it will shut down all the power once that particular group reaches the BMS over discharge protection voltage. This could happen if one of your cells goes bad for example.
* It will protect the pack from overcharge: if you start at full charge and go down hill for a long time, the bms will cut out the power due to the overcharge voltage limit.

That's basically it. It's also why a lot of people (including myself) prefer to bypass it for discharge: you can use a small one and you don't need the extra room in the enclosure. The over discharge protection is done by the VESC (**not on a per group level but on a pack level**). Same goes for protecting the pack from pulling too many amps, the VESC limits that (with the battery max setting). Over charge during regen is still a risk, same when a parallel group goes bad: unless the overall voltage drops dramatically, the VESC will have no clue it happened and will carry on.

Also, a BMS balances when a cell/group reaches 4.2v. I've seen people suggesting you will save some charge cycles on the cells by only charging to 4.1v. While that is true, if you do it too many times and your cells/groups start to drift, the BMS will never have the opportunity to balance them, since you never allow the voltage to reach 4.2v.
```

---
## \#22 Posted by: darkkevind Posted at: 2017-12-01T21:58:00.473Z Reads: 247

```
I think a few people might benefit from watching this and seeing how balance chargers actually do their job. BMS' work in a similar way also...

Slight over-charge, then individual or group discharge to bring lower cells up to voltage should other cells have reached voltage already...

Being as this is how they work, when a pack reaches voltage and the brick goes green for example, all cells should be equal.

This said, BMS' don't over-charge then drain, they cut charge to cells once they've reached voltage.

https://youtu.be/wIbHLacozFo
```

---
## \#23 Posted by: gogomrrobot Posted at: 2017-12-01T22:19:26.399Z Reads: 243

```
There has to be be a way to solve the BMS issue altogether. I want it... but outside the board or not at all.

No BMS type solutions (and no embedded in your build type BMS)

**Option #1** - use a 12S charger like the EVPeak A9 -- yes it was about $200 but it is rapid and well worth the investment.  The only issue I have is that I have my (2)6S cables that tie into the 12s charger's balance board hanging out of the case (in picture below I don't have the enclosure on but they would go into the 3d printed holes for the xt90 and the other rectangular hole/bracket to the right of it).

<img src="/uploads/db1493/original/3X/7/3/7384f3bbc1cf6243faf8f33b4dd80d8f108cf8c6.JPG" width="333" height="250">

**Option #2** -- Why not use something liike @Nowind cell pack monitor to charge and keep the voltages the same. Balance charge when they differ greatly.

<img src="/uploads/db1493/original/3X/7/8/78d2482d17ad2455445c6cc7a298d7105bfe7c06.JPG" width="333" height="250">

<img src="/uploads/db1493/original/3X/a/9/a9ff7a25ed320425b5e72e422c0e0e3c9da6b0fa.JPG" width="333" height="250">


**Option #3** -- put BMS leads outside the board like I have but have the BMS on the outside of the build then hook balance cables only when charging. This saves you from buying a 12S balance charger.


None of my ideas are gr8 because well how do you deal with portable charging? Maybe #3. There has to be a way to get rid of the BMS inside the build... it's a space waster and if you do like 4-5 boards... it just gets annoying... each build has to have an AS switch, each a BMS, each an x and a y and a z.  We need to find solutions to delete it from our builds. Maybe an engineering solution like a circular balance wire power plug that leads the balance cables outside to the BMS, Inside the circular plug are the (12) balance cables. The input and output of the power plug re-extracts the 12 wires. And the BMS is next to the power brick charger. I think that would be a cool invention. Then it's just two quick plugs to plug in -- both shaped like circular power charger ports. You only need buy one BMS + charger could solve all your builds!  This shit would literally cost like $2 to manufacture.
```

---
## \#24 Posted by: Quezacotl Posted at: 2017-12-01T22:31:09.279Z Reads: 226

```
Option #3 is what i'm using. a circular plug that has all the wires, and i'll just plug it in my external charger.
But that brings problems, like OP said. Risk of individual cell over-discharge despite ESC safe limits.

I had that happen when i don't have any BMS on board. I ran out to about 33V(10S pack), which in reality was one cell zero volt.
```

---
## \#25 Posted by: longhairedboy Posted at: 2017-12-01T22:48:38.392Z Reads: 223

```
Thank you @chaka. I'm glad it was finally stated so clearly.
```

---
## \#26 Posted by: Sebike Posted at: 2017-12-01T22:48:56.849Z Reads: 222

```
Looks like these would work fine for option #3, no?

[https://www.aliexpress.com/item/SP20TA-ZM-90-degree-elbow-waterproof-connector-IP67-Industrial-power-cable-connector-Male-plug-and-Femal/32763647137.html?spm=2114.search0104.6.3.FCaivo&s=p](https://www.aliexpress.com/item/SP20TA-ZM-90-degree-elbow-waterproof-connector-IP67-Industrial-power-cable-connector-Male-plug-and-Femal/32763647137.html?spm=2114.search0104.6.3.FCaivo&s=p)
```

---
## \#27 Posted by: longhairedboy Posted at: 2017-12-01T22:54:44.466Z Reads: 218

```
[quote="gogomrrobot, post:23, topic:39879"]
Option #3 -- put BMS leads outside the board like I have but have the BMS on the outside of the build then hook balance cables only when charging. This saves you from buying a 12S balance charger.
[/quote]

all that does is shift money around, and not in a good way. A good BMS and charger costs less than  a multipin milspec connector ( to send all your balance leads to an outboard balance charger) and an outboard balance charger. Especially at 12S. 

You're still doing the same shit just on a different day.
```

---
## \#28 Posted by: gogomrrobot Posted at: 2017-12-01T23:05:36.053Z Reads: 208

```
Ok but we can change the world... the BMS doesn't have to be in every one of your 10,000 boards right?

The component that @Sebike has linked + combined with Jenso's cell monitor lets you from having 10,000 bms's right for your 10,000 boards?  Now it will look ghetto with the BMS and charger on the outside... I get that part.

<img src="/uploads/db1493/original/3X/f/7/f7ccd419b8da02fd49fa55393664cf1c231814b4.jpg" width="539" height="500">
```

---
## \#29 Posted by: chaka Posted at: 2017-12-01T23:41:19.040Z Reads: 205

```
I suppose we could also switch a single drivetrain to different boards but that is not the scope of this thread. We need to be implement "best practices" now and avoid being over regulated in the future.
```

---
## \#30 Posted by: scepterr Posted at: 2017-12-01T23:46:39.882Z Reads: 204

```
For science i just charged up my 30Q 10S3P to 41.50V, the BMS is set to 4.125 end/balance voltage.   I will time how long it'll take to bring down to 41.25V. Considering it has to bring the whole pack down it'll give a good estimate in terms of max time to balance.
```

---
## \#31 Posted by: chaka Posted at: 2017-12-02T00:00:55.647Z Reads: 203

```
Be sure to let us know your BMS balance current specs, sounds like you have a larger programmable model.
```

---
## \#32 Posted by: scepterr Posted at: 2017-12-02T00:02:48.132Z Reads: 200

```
It's the D190 from bestech, 84ma balance current
```

---
## \#33 Posted by: longhairedboy Posted at: 2017-12-02T00:53:33.030Z Reads: 199

```
I think the DieBieMSs are what's going to change the eskate world, not regressing back to the days of the enertion 6S kit. Just sayin'
```

---
## \#34 Posted by: jmasta Posted at: 2017-12-02T01:14:57.669Z Reads: 194

```
We are severely lacking a quality programmable high-amp BMS. JTAG's looks so promising. Hopefully they become more readily available. Especially since BattMan is effectively dead
```

---
## \#35 Posted by: fedestanco Posted at: 2017-12-02T01:50:53.669Z Reads: 199

```
[quote="chaka, post:1, topic:39879"]
It can take weeks for a BMS to balance a large pack if it has drifted significantly.
[/quote]

I totally agree on this point of view. For this reason I believe IC bmss are in a whole different league.
For example there was an old firmware for @JTAG's bms where a "bug" allowed to balance the cells WITH THE CHARGER DISCONNECTED.
Just imagine how cool would be to have your cells start balancing whenever you like with or without charger. This is Tesla kind of stuff...
```

---
## \#36 Posted by: Titoxd10001 Posted at: 2017-12-02T02:59:55.133Z Reads: 196

```
If it's between one of p groups going below voltage and power cutting out while on the throttle. I'd rather let the p group go low voltage and let the pack potentially get damaged. Cells are rated for 2.5 volts aren't they. Rather save some skin
```

---
## \#37 Posted by: chaka Posted at: 2017-12-02T15:02:05.721Z Reads: 189

```
I would rather manage my cells properly and save my skin and my cash. Of course most/some of us know there is a cliff at 3v, once a cell gets there it plummets unpredictably and they turn into an expensive radiant heater. Good for warming all that skin you save on these cold nights.
```

---
## \#38 Posted by: deucesdown Posted at: 2017-12-02T23:47:43.593Z Reads: 181

```
Why is it BMS mfgs don't describe exactly what their devices do. So frustrating having mystery black boxes interfacing with the most dangerous and expensive part of our boards. (If I'm wrong and there are docs, plz post a link, I've yet to see docs beyond some basic basic specs)

Float charging is bad for lithium ion. Our phones and laptops don't float charge. If BMSes need hours with power to the cells to balance the cell groups, I'd argue that's another strike against BMS. If BMS can keep balancing after charger is removed, that's better for the cells, but makes me worry about malfunctions.

In theory cell groups should not be far out of balance so time spent balancing should be minimal. But we need some indication if things are not going well. Things break, cells wear out unevenly due to imperfect pack builds and heat distribution.

If BMS had a display or at least some flashing LEDs to indicate exactly what was going on that I could bring to the outside of the board, I'd feel a lot better.

Need JTAG's BMS.
```

---
## \#39 Posted by: Maxid Posted at: 2017-12-03T00:34:55.675Z Reads: 178

```
To this day I don't understand why people insist on having a BMS at all - it seems so unnecessarily complex and expensive plus is an additional part that might fail. Especially with larger p-groups the chances for drift should be even lower than on smaller batteries - why should a BMS be more important on a large pack then?

No BMS is the way to go for me - check your cells/groups after a ride and you'll be fine and even save some money in the process. Seems like a good hourly rate if you save 100$ on a BMS for a 10 second check with a lipo buzzer or whatever.
```

---
## \#40 Posted by: koralle Posted at: 2017-12-03T03:46:23.891Z Reads: 181

```
[quote="longhairedboy, post:25, topic:39879, full:true"]
Thank you @chaka. I'm glad it was finally stated so clearly.
[/quote]

curse you though for only starting this thread after I bought 2 charge only bms :-/
now I went from feeling pretty secure about doing a good build to having bad dreams and not being able to sleep!
```

---
## \#41 Posted by: longhairedboy Posted at: 2017-12-03T03:49:08.228Z Reads: 178

```
don't forget the heavy drinking. And the inevitable opiate addiction.
```

---
## \#42 Posted by: chaka Posted at: 2017-12-03T15:41:31.111Z Reads: 175

```
Just be sure you can monitor your cells manually and you will be fine. If they get far out of balance you can use a connector like this and manually balance the pack through the balance connector.  This is what I use to quickly balance a pack.

<img src="/uploads/db1493/original/3X/d/6/d6fb1f44cdc288b620a86b2826a817ddf8aa9507.jpg" width="638" height="450">
```

---
## \#43 Posted by: koralle Posted at: 2017-12-03T17:19:40.376Z Reads: 169

```
what do you use as a charger for single cells?
```

---
## \#44 Posted by: Kug3lis Posted at: 2017-12-03T17:31:07.608Z Reads: 168

```
I guess same LiPo charger, but instead of charging whole pack you charge a single cell
```

---
## \#45 Posted by: chaka Posted at: 2017-12-03T17:49:12.478Z Reads: 164

```
I use a lab power supply when I am at the bench.
```

---
## \#46 Posted by: SilentException Posted at: 2017-12-03T19:23:43.861Z Reads: 166

```
You can also use TP4056 module to charge single cell up to 1A. It has a proper LiPo charging curves as opposed to using regular bench CC/CV PSU just by itself.
```

---
## \#47 Posted by: Eboosted Posted at: 2017-12-04T05:13:20.771Z Reads: 161

```
I'm having the same idea but I'm planning to install an exposed connector on the enclosure itself, this way I wouldn't have to disassemble the enclosure and BMS to connect the lab power supply.

The lipo checker should give me the readings whenever I need to performance any balance.
```

---
## \#48 Posted by: nmagz3 Posted at: 2017-12-07T20:14:47.432Z Reads: 144

```
Wow, this is a great thread!  Thanks for the info everyone and thanks for starting this conversation @chaka.  I've recently purchased a 10S Bestech BMS with the knowledge that it will add additional protection to the cells due to low voltage monitoring.  However, I never really thought of the down side of bypassing the BMS for discharging.
```

---
## \#49 Posted by: Ashley_Beaum1994 Posted at: 2018-07-30T13:52:28.167Z Reads: 83

```
Awesome thread! have been searching through this forum trying to fully understand what i need and potentially don't need for my build! If this forum didn't exist I'd be screwed haha!
```

---
