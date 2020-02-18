# Important BMS specs

### Replies: 36 Views: 1540

## \#1 Posted by: ikjahaa Posted at: 2018-01-27T16:11:16.018Z Reads: 176

```
I've bought a battery pack some while ago, but the included BMS is just tooo bluckey for my enclosure.
I'm using a 10S3P battery, on a single motor setup with a 50amp fuse.

Which BMS would you guys recommand ?
```

---
## \#2 Posted by: Achmed20 Posted at: 2018-01-27T16:29:22.773Z Reads: 174

```
how about some pics of your current one?

BMS are usualy all about the same size
```

---
## \#3 Posted by: mmaner Posted at: 2018-01-27T16:42:27.388Z Reads: 170

```
I had a BMS a while back it was as wide and about half as deep as the battery pack itself. It made it fairly difficult to use.  Take a look at Bestech and SuPower.
```

---
## \#4 Posted by: ikjahaa Posted at: 2018-01-27T16:44:43.883Z Reads: 164

```
its 18Cm x 11cm, pretty huge..
```

---
## \#5 Posted by: ikjahaa Posted at: 2018-01-27T16:56:58.477Z Reads: 150

```
Thanks,

I thikn these two look interessting :slight_smile:

* (Tiny) http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCB-D189.html
*  http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

I'd prefer the tiny one, but 35Amps max discharge might be too low, not ?
```

---
## \#6 Posted by: mmaner Posted at: 2018-01-27T17:01:19.888Z Reads: 143

```
The second one looks ok, but I would ask @Namasaki just to be sure.  He's the king of BMS's and Lipo's.
```

---
## \#7 Posted by: Acido Posted at: 2018-01-27T19:41:39.813Z Reads: 123

```
Get a bestech charge only bms they are like 8x8x1 cm for 25$
```

---
## \#8 Posted by: Acido Posted at: 2018-01-27T19:42:09.559Z Reads: 121

```
35a for discharge is low
```

---
## \#9 Posted by: ikjahaa Posted at: 2018-01-27T19:56:02.403Z Reads: 125

```
What's the difference with these ones ?
Also, could you please pass me an example? 😁
```

---
## \#10 Posted by: Acido Posted at: 2018-01-27T23:00:03.901Z Reads: 121

```
HCX-D150
Check out this one if you lack space in your enclosure

The second one is capable of discharging out 80a continous while this one is only for charging the cells
```

---
## \#11 Posted by: b264 Posted at: 2018-01-27T23:05:58.621Z Reads: 119

```
Get a [Bestech D190 10S BMS](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D190.html)
```

---
## \#12 Posted by: koralle Posted at: 2018-01-27T23:48:54.021Z Reads: 120

```
side note: Bestech is out of IC stock for BMSs with this configuration until May (fucking up my group buy):

G3P
Over charge detection voltage: 4.20V+/0.025V 
Over charge release voltage: 4.10V+/0.05V 
Over discharge detection voltage; 2.80V+/0.05V 
Over discharge release voltage: 2.90V+/0.1V

so if you ordered directly from bestech you will have to go with one of these for now:

G3M
Over charge detection voltage: 4.28V+/0.025V 
Over charge release voltage: 4.08V+/0.05V
Over discharge detection voltage: 2.80V+/0.05V 
Over discharge release voltage: 2.80V+/0.1V
 
G3J
 Over charge detection voltage: 4.28V+/0.025V
Over charge release voltage: 4.08V+/0.05V
Over discharge detection voltage: 3.00V+/0.05V 
Over discharge release voltage: 3.00V+/0.1V
 
101CD
 Over charge detection voltage: 4.25V+/0.025V
Over charge release voltage: 4.05V+/0.05V
Over discharge detection voltage: 2.50V+/0.0625V 
Over discharge release voltage: 3.00V+/0.1V
```

---
## \#13 Posted by: ikjahaa Posted at: 2018-01-28T00:27:11.038Z Reads: 115

```
Actually, another question... 
if i bypass my bms for discharge, then how do i connect my e-switch ? :thinking:
```

---
## \#14 Posted by: Namasaki Posted at: 2018-01-28T03:01:13.543Z Reads: 115

```
If you go with a smaller BMS and bypass during discharge, you will not have short circuit protection, or the ability of the bms to shut your system down when something goes wrong with your battery's cells that doesn't drop the total voltage enough to trigger the Vesc low voltage protection.

More importantly, is the issue of Regenerative brakes.
With a bypassed bms, the regen charge goes strait into the battery and can cause overcharging when braking on a full battery.
When discharging through the bms, the regen charge goes through the bms and is controlled by the bms so that it prevents overcharging of the battery when braking on a full battery.

And if you bypass for discharge, you will not have the full function of the E-switch and will have to use a loop key.
```

---
## \#15 Posted by: ikjahaa Posted at: 2018-01-28T21:30:42.669Z Reads: 104

```
What maximal continuous discharging current would you advise on ? for 10S3P setup.
Also, how do i know if a BMS supports an eswitch? :confused:
```

---
## \#16 Posted by: ikjahaa Posted at: 2018-01-28T21:34:54.565Z Reads: 107

```
I'm thinking of taking these ones : 
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D276.html

do you know if these ic's are still in stock ?
```

---
## \#17 Posted by: deucesdown Posted at: 2018-01-28T21:43:39.937Z Reads: 110

```
[quote="Namasaki, post:14, topic:44800"]
When discharging through the bms, the regen charge goes through the bms and is controlled by the bms so that it prevents overcharging of the battery when braking on a full battery.
[/quote]

The flip side of this is when BMS protection kicks in, it cuts power (and brakes), right? So a choice between saving the pack or saving your skin.
```

---
## \#18 Posted by: Namasaki Posted at: 2018-01-28T22:47:34.801Z Reads: 103

```
[quote="deucesdown, post:17, topic:44800"]
The flip side of this is when BMS protection kicks in, it cuts power (and brakes), right? So a choice between saving the pack or saving your skin.
[/quote]


I have tested my setup braking constantly downhill on a full battery and once the battery voltage reached the overcharge detection voltage, the bms did not shut down. It just stopped the battery voltage from climbing any higher and dissipated the charge current like it does while balancing.
The only thing that might be a problem is if while braking down a very long hill with a full battery the bms might overheat and shutdown.
Although I have not been able to make mine shut down because of heat yet.
This is one of the main reasons I like the Bestech D223V1. It comes with good heatsinks.
```

---
## \#19 Posted by: Namasaki Posted at: 2018-01-28T22:59:11.647Z Reads: 97

```
[quote="ikjahaa, post:15, topic:44800"]
What maximal continuous discharging current would you advise on ? for 10S3P setup.

Also, how do i know if a BMS supports an eswitch? :confused:
[/quote]

When it comes to the battery and bms, the more headroom you have the better.
If your pulling 40a from the battery and you have an 80a bms, it's going to handle the current much better than a 50a bms. And the chance of overheating will be much less.
Same thing but even more so with your battery because the more headroom your battery has the less voltage sag you will experience and the cooler your batteries will run.

Bottom line, put the beefiest battery and bms that you can fit. But try to leave ample room around your bms to allow heat dissipation. This also holds true for your Vescs or Focboxes. 

If the bms has a built in E-switch, it will be specified.
For example:

![44 PM|690x443](upload://qHzxizna1HQ0XGudRChOIlMreRF.png)
```

---
## \#20 Posted by: Ackmaniac Posted at: 2018-01-28T23:13:21.558Z Reads: 83

```
There is no way that the bms can take all that power when the battery is full. It will melt itself in seconds. If your lucky it desolders the components first so that you can assemble it again.
If over or undercharge protection kicks in it simply shuts down.
```

---
## \#21 Posted by: koralle Posted at: 2018-01-28T23:19:33.681Z Reads: 77

```
The ICs are the same for the Bestech BMS models that are useful for us. 
Which IC they need depends on which voltage settings you would like. At the moment the most popular settings around here are not possible (until May) because @thisguyhere bought all the ICs with his huge ass group buys  :japanese_goblin:
```

---
## \#22 Posted by: deucesdown Posted at: 2018-01-28T23:54:09.621Z Reads: 77

```
[quote="Namasaki, post:18, topic:44800"]
I have tested my setup braking constantly downhill on a full battery and once the battery voltage reached the overcharge detection voltage, the bms did not shut down. It just stopped the battery voltage from climbing any higher and dissipated the charge current like it does while balancing.
[/quote]

[quote="Ackmaniac, post:20, topic:44800, full:true"]
There is no way that the bms can take all that power when the battery is full. It will melt itself in seconds. If your lucky it desolders the components first so that you can assemble it again.

If over or undercharge protection kicks in it simply shuts down.
[/quote]

I would tend to lean in ackmaniac's direction, but experience beats theory.

I'm watching this thread with much interest, hope something develops to make things more clear.
```

---
## \#23 Posted by: lock Posted at: 2018-01-29T00:38:47.840Z Reads: 76

```
I'm with @Ackmaniac on this, the bleed resistors on BMSes are tiny. The BMS either shuts down, or keeps feeding charge into the battery pack. In @Namasaki case I guess power just keeps getting fed into the pack where it's absorbed/burnt off as heat, and this may indeed be the preferred option.

Did some load testing on my battery pack and a low 1.6a (approx 60w) managed to get 4 100w resistors burning hot (in still air) in a matter of seconds. A little power makes a lot of heat.
```

---
## \#24 Posted by: Namasaki Posted at: 2018-01-29T02:10:08.806Z Reads: 77

```
@lock @Ackmaniac

As @deucesdown stated, experience beats theory.

I tested my Bestech HCX-D223V1 and it did not melt down in seconds nor did it shut off and niether did my battery continue to increase in voltage after the overcharge detection value was reached.
I monitored the battery voltage with an inline volt meter visible through the top of the deck while performing the test. My overcharge detection is set at 4.28. My battery voltage climbed while braking until it reached 42.8v
At that point if stopped climbing although I continued braking down the hill. After I reached the bottom of the hill and released the brake, the bms proceeded to trim the battery back down to 42v while I was coasting.

These are my current settings for dual drive

![51 PM|690x300](upload://45SzjodNoYWTeInUajHJxCUZD2j.png)
```

---
## \#25 Posted by: lock Posted at: 2018-01-29T04:31:48.064Z Reads: 72

```
[quote="Namasaki, post:24, topic:44800"]
experience beats theory.
[/quote]

Maybe so, but it does little to satisfy my curiosity :wink:.

I'm not convinced that your battery voltage observations give the full picture. Now if you had a watt meter inline between BMS and battery, and that showed 0w/0a in a regen/overcharged situation, then that I would believe.

I believe your BMS has a separate discharge/charge ports, and I think there's still some questions ([here](https://endless-sphere.com/forums/viewtopic.php?f=14&t=61625#p920535), [here](https://endless-sphere.com/forums/viewtopic.php?f=2&t=92178#p1347965), and [here](https://endless-sphere.com/forums/viewtopic.php?f=14&t=82336#p1209202)) around on whether you get high voltage cutoff when charging through the discharge port.

Indeed the Bestech BMSes may be better suited to our use as they allow overcharging of batteries through the discharge ports, whereas other brands shut down (killing the brake) due to exceeding high voltage cutoff.

It took my BMS (jtag's one), 24hrs to balance out my battery pack when I first put it together. Cells may have been 10% apart. It certainly doesn't have the capacity to burn off regen type levels of power, I'm fairly sure balancing in discharge mode is disabled anyway.
```

---
## \#26 Posted by: b264 Posted at: 2018-01-29T04:41:07.028Z Reads: 66

```
[quote="deucesdown, post:22, topic:44800"]
I would tend to lean in ackmaniac’s direction, but experience beats theory.
[/quote]

Laws of physics trump all, which is what @Ackmaniac's statement is based upon.  If you have thousands of watts coming from the motors, you just can't burn it off, even with a heatsink that big, for any non-negligible length of time, without the heatsinks being hot enough to melt solder or worse

@Namasaki could you make a video of this?  Also, did you check the heatsink with your hand afterward?  Was it hot?
```

---
## \#27 Posted by: Namasaki Posted at: 2018-01-29T05:19:18.280Z Reads: 66

```
[quote="lock, post:25, topic:44800"]
I’m not convinced that your battery voltage observations give the full picture. Now if you had a watt meter inline between BMS and battery, and that showed 0w/0a in a regen/overcharged situation, then that I would believe.
[/quote]


the battery voltage Increases as it takes charge, when the voltage stops increasing its a pretty good sign that no more charge is going into the battery.
I can't speak for other bms's, I have only tested the one I mentioned.
I do know that it has higher balance current than other bms's. Twice as much as Battery Supports.
And I did witness the bms trim the battery down from 42.8 to 42v after I released the brakes. 
So I am fairly sure that balancing is not disabled in discharge mode. But then with this bms, there really is not a charge or discharge mode. The bms is on when discharging and it's on when charging. So whether your charging or discharging, it's the same.
```

---
## \#28 Posted by: Namasaki Posted at: 2018-01-29T05:32:47.352Z Reads: 63

```
[quote="b264, post:26, topic:44800"]
Laws of physics trump all, which is what @Ackmaniac’s statement is based upon.  If you have thousands of watts coming from the motors, you just can’t burn it off, even with a heatsink that big, for any non-negligible length of time, without the heatsinks being hot enough to melt solder or worse

@Namasaki could you make a video of this?  Also, did you check the heatsink with your hand afterward?  Was it hot?
[/quote]

I'm not sure that there are thousands of watts coming for the motor during braking but either way the Vesc controls the amount of current going to the battery during regen braking.
the Batt Min Current setting.
The Bestech that I mentioned has a temp sensor on the heatsinks so if the heatsinks did get too hot it would trigger the over temp protection certainly long before they got hot enough to melt solder.
I did mention that there could be the possibility of the heatsinks overheating on a really long downhill but I have not had any over temp shut down with the tests I did.
```

---
## \#29 Posted by: b264 Posted at: 2018-01-29T05:45:08.972Z Reads: 60

```
"-10A battery min" is like a 420W soldering iron (that never shuts off due to temp) if you're not charging the battery with it
```

---
## \#30 Posted by: lock Posted at: 2018-01-29T08:18:53.969Z Reads: 63

```
[quote="Namasaki, post:27, topic:44800"]
the battery voltage Increases as it takes charge, when the voltage stops increasing its a pretty good sign that no more charge is going into the battery.
[/quote]

Actually, with what I think you are saying current would still be flowing into the batteries, but also flowing out of the batteries through the BMS bleed resistors. So even my approach of sticking a watt meter between the BMS and battery wouldn't confirm what was happening.

Or, maybe you're suggesting the BMS switches into a special mode where current no longer flows to the pack, and gets redirected to the bleed resistors. This sounds overly complicated to implement for little benefit given how small the resistors are.

Have you ever had the BMS shut down during regen? Why do you think it would? It seems fairly likely that high voltage cutoff only applies to the charge port. Battery voltages at their charged thresholds are a bit weird (non-linear), mine drop from 3.6v to 3.5v almost immediately at the sign of any load. Maybe voltage stops increasing because there's another undesirable process occurring in your pack.

It's a bit messed up, but the way I see it is on a long descent one or two things will happen. One, brakes stop working. Two, battery pack overcharges and explodes. Please don't take this as a specific to your board kind of thing... I just saw this on the [Boosted support page](https://support.boostedboards.com/hc/en-us/articles/115000912488-Regenerative-Braking-and-Conserving-Battery-Charge).

> Braking downhill on a full battery charge will cause the board to lose braking capabilities since the regenerative braking will cause the battery to overcharge. When this happens, the remote will warn you by beeping, and _you’ll lose your braking power_.

Helpful 😂
```

---
## \#31 Posted by: deucesdown Posted at: 2018-01-29T08:24:28.473Z Reads: 63

```
https://www.electric-skateboard.club/t/enertion-raptor-riders-club/256/314

[quote]
 Our custom designed BMS system allows a safe trickle of regen current into the battery so the brakes always work, we also have an array of TVS diodes in place to dissipate excessive energy & prevent any major battery damage.
[/quote]

Maybe D223V1 has something similar? I find it hard to believe cell balancing resistors can come into play for dissipating excess braking energy.

I don't speak enough electronics to understand what/how TVS diode arrays come into play.

But either way, I mean, watts is watts, right? 1st law of thermodynamics? Gotta go somewhere.

@b264 we don't have complete facts or total understanding, so we're making up _**theories**_ that hopefully don't violate any _**laws**_, to explain what's going on. :slight_smile:

EDIT The D223V1 has:

Balance current for single cell 108mA±15mA

so for 10s, we can dissipate at max 1.08a at 42v, 42w. That's not nothing, but doesn't seem like much? Especially with respect to VESC battery min current?
```

---
## \#32 Posted by: b264 Posted at: 2018-01-29T08:31:56.372Z Reads: 60

```
I think it's time for real experiments to happen with wattmeters and voltmeters and thermometers ;-)

I'm super-curious now, too

The only certainties here I'm aware of are the laws of physics and the laws of thermodynamics
```

---
## \#33 Posted by: deucesdown Posted at: 2018-01-29T08:40:01.665Z Reads: 63

```
If we only had specs on how these BMS work, things would be so much simpler. All I see is a table of numbers on bestech's website. The actual operating modes I have to try to guess from posts here. For example namasaki's bms seems to allow charging to 42.8v pack overall (slight overcharge), then cuts off charge power, and kicks in the balancers, bleeding energy from each cell until all cells reach the voltage of the lowest cell? Or maybe bleed them all down to 4.2v/cell? Or perhaps the final 42v pack voltage is just coincidence? And this doesn't apply to charging from the discharge terminals, which should be a very different thing?

Do these all use the same Texas Instruments chip or something? Maybe I've been trying to chase this from the wrong direction.
```

---
## \#34 Posted by: deucesdown Posted at: 2018-01-29T08:54:15.386Z Reads: 63

```
I looked at some ackmaniac app csv logs. On my dual 6355, for negative numbers in the "Power" column which I believe are in watts, I rarely see numbers greater than -100. Looks like when I'm feathering it's around -100, and when I'm braking for real, I'm exceeding -400.
```

---
## \#35 Posted by: SilentException Posted at: 2018-01-29T09:08:53.506Z Reads: 64

```
The only way to have the braking thing sorted out is so that ESC and BMS communicate with each other and a decent braking resistor. Mellow has a good setup there that is safe for every component of the system.

I was going to set things up for a bench test of our "normal" setups to see what is going on internally between both ESC and BMS and BMS and the battery pack but I just couldn't be bothered to risk destroying any of those pretty pricey components just for science. I will rather ride them to death :)

I also wanted to ask BesTech about it but I'm sure Donna or Jessie wouldn't be able to help and I don't think any of the engineers would be up for a chat.

If someone does decide to do the bench-test of this, I'm really interested as well.
```

---
## \#36 Posted by: Namasaki Posted at: 2018-01-29T18:13:51.982Z Reads: 55

```
[quote="lock, post:30, topic:44800"]
Or, maybe you’re suggesting the BMS switches into a special mode where current no longer flows to the pack,
[/quote]

I don’t know how it works, I just know that my battery’s  voltage did not increase beyond the over discharge detection value set on the bms, even though I continued braking downhill. 
And the bms did not overheat or shut down. 
The 4.28v over discharge detection was the default setting from Bestech. 
I assumed that thier engineers know what they’re doing and that 4.28v is a tolerable amount so I went with it. 
There hasn’t appeared to be any adverse effects on my battery from that test.
```

---
