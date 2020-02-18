# Help: Bestech 6-10s BMS shorted and caught fire while soldering

### Replies: 34 Views: 2238

## \#1 Posted by: solideogloria Posted at: 2018-02-16T06:31:10.530Z Reads: 234

```
Hi everyone,

My Bestech BMS seems to have shorted and caught fire while soldering. 

In shock right now... The fire extinguisher failed (fell out of charge...). Had to use a damp rag to put out the fire. Quite the disaster. Burnt BMS. Possibly burnt battery pack... Hundreds of dollars of damage... But all else is well, thank God. 

My 8s4p li-ion battery pack had been finished earlier, and I was on to soldering the very last wire to the BMS... A black negative lead (from the load / anti-spark switch / VESC) to the "P-"... Everything was connected except for P-. I'm really not sure how it all burst into flames?

The P- wasn't even hooked up to anything, apart from an unplugged XT90! There was fire before I even connected the negative wire to the P-.

The last thing I vaguely recall doing was putting a droplet of flux onto the P- connection. I think so anyway, as I did that to prep the C- and B- the same way. It's all hazy right now. Next thing I see is smoke and flames... Maybe the droplet was too big? Maybe it seeped through the PCB, connecting the C- (red positive lead) to the P- (black negative lead). -- Looking at the underside of the PCB, these two connections are really close, like 1-2mm. So, maybe the flux seeped through?

It's a sticky mess right now. Hot glue has melted everywhere. Even small melted solder puddles. A couple of nickel tabs came off the 1st series connection. Heatshrink has melted everywhere, both the original layer and the 2nd layer I added. But somehow the battery is still registering 25.7v (was ~26.2 earlier before the fire), so 3.21v per cell.

Is the battery ruined? What should I do? What went wrong? Should I try again and connect my 2nd BMS? I'm shocked and confused, uncertain how this happened. I thought I was doing everything right.

[DSC03070|690x388](upload://n6eoMPEuU4KI1CpjbsPgsuTkaJV.JPG)![DSC03066|690x388](upload://ceZDlKYrlWlNnCmFMJdxCjIQn2b.JPG)![DSC03068|690x388](upload://t8Hp2s0dHV56sCSj2e7KLEIPRFc.JPG)![DSC03067|690x388](upload://dE26Hobqv7Zjnizygwq8IzpeD94.JPG)[Uploading...]()

**Details:**
  - **BMS Model:** HCX-D223V1LI10S80A-06
  - **Battery:** 10s4p Li-ion, cardboard ring sealed, shrink wrapped each cell, soldered nickel strips
  - **Load:** NA. Nothing connected.

Please help if you can. Thank you.
```

---
## \#2 Posted by: ShutterShock Posted at: 2018-02-16T07:12:24.314Z Reads: 218

```
Ummmmm just for clarification.  You didn't happen to have the batteries plugged into the bms while soldering did you?
```

---
## \#3 Posted by: solideogloria Posted at: 2018-02-16T07:43:31.383Z Reads: 219

```
Hi ShutterShock,

Yes, battery was plugged into the BMS while soldering. 

There was, however, no load connected. So the battery was not completing a circuit (not intentionally anyway). As per photos, an XT90 was just about to be connected. No connection to anti-spark switch / VESC.

Did I make a rookie mistake? I assumed that's the only way, since BMS are often sold built into battery packs, and the wiring diagrams I trusted on ESK8 were the same.

E.g. @Namasaki's ![41 PM|664x500](upload://2qXy5gyFfE0zTjQHvgn5WM3mKNt.png)
```

---
## \#4 Posted by: solideogloria Posted at: 2018-02-16T08:00:19.665Z Reads: 215

```
To illustrate what I was attempting _before_ the fire: Burnt BMS vs New BMS with the wires I was originally trying to connect connected.

![DSC03072|690x388](upload://1KI6G8BL4TzVrXCWxEDnVFX7J6o.JPG)

Perhaps someone with experience can confirm what went wrong? On closer inspection, I can only suspect the culprit may have been from excess flux seeping through the PCB and shorting the positive and negative terminals (C- and P-). :face_with_monocle:

The underside of the BMS PCB between the two terminals. It's super close! Like 1-2mm close! You'd never notice on the topside.

![DSC03073|690x388](upload://4jTVB9lpc29bub5ak21noOmxaPf.JPG)
```

---
## \#5 Posted by: rojitor Posted at: 2018-02-16T13:07:46.875Z Reads: 196

```
Did you solder correctly the balance wires? 
Every bms units are "similar" but not the exact same. Some have 10 balance wires... some 11, some have charge and discharge in two ports...Some share the same port, some balance...Some do not.
Did you get intructions with it? Some bms must be soldered in a very specific order. First -b then -c and -p and the last step solder and plug the balance. 
Just by looking at the pics I have no idea. It could be a faulty bms, incorrect wiring or incorrect order.

![20180216_141203|690x388](upload://m3mzd5m06unqDjqXZY6FOg1yJx0.png)

That part worries me. The main negative looks too close to the positive and I see no insulation. Was it protected?
```

---
## \#6 Posted by: solideogloria Posted at: 2018-02-16T14:32:35.810Z Reads: 187

```
Thanks rojitor. No instructions I'm afraid. Vague directions on a datasheet, yes.

Yes, good point, I believe 8 balance wires were connected as per instructions from Bestech. Pre-purchase I clarified how to the balance wires worked: They confiemd that the BMS has "10 wires (B1-B10), but for 6s I only need 6 wires (B1-B6). Likewise, 8s would need 8 wires (B1-B8)." 

Thus, for an 8s battery, I connected 8 balance wires (B1-B8).

Hopefully, they were connected correctly. I believe they were. I mimicked the position @Eboosted used in 'Upgraing an Evolve GT Battery':

![46 AM|690x241](upload://3Vq2GAGnc9WBpIEZHkuuyRfZIbo.jpg)

I thought the positions were odd at times, but I went with it:



Diagram as per Bestech's BMS Datasheet:
![44 AM|532x427](upload://8I0iAvielAu7EOQD8JiSiztaDtW.png)

> That part worries me. The main negative looks too close to the positive and I see no insulation. Was it protected?

**Good eye.** But, no short there, I don't think so anyway... Not at that point specifically. 

The main neg lead (and leads and balance wires) have ample hot glue insulation, and have 3 layers of nickel strip (stepping up to that lead). i.e. ebikeschool's diagram:

![15mm|690x431](upload://qMXmNu3sl2win4N9rbcmdJOVR6.jpg)

However, now that you mention it, _two nickel tabs had come off nearby_,  but on the far lefthand side, between B1 and B2. It's obvious in pic1 and pic2 (see op) where they're separated (amplified by me lifting the esk8 out onto my driveway).

**ALSO at B1**, the cell _right beside_ the main neg lead _slipped out of place_ (desoldered and shifted out of position). Very shifty... I assumed it came loose from heat (heat overall from the short - you know, hot batteries everywhere, glue melting everywhere, etc) but perhaps that main neg lead you've pointed out somehow contributed to this!? Because, while the 4p packs came apart, that cell is the _only cell_ to have slipped out of place...?:confused:

Also, I'm not sure if this is important, but the balance wire at B1 is on the pos corresponding end of the cell that the main neg lead is attached? Is that the correct positioning? Does it have any affect, perhaps on current flow?

> Some bms must be soldered in a very specific order. First -b then -c and -p and the last step solder and plug the balance.

**Good point! But I did B-, C-, then P-?**  And it was the final P- that seemed to cause the fire?? 

But in terms of order, I now wonder if my balance leads are backwards. But, then, it's wired as per the Bestech diagram... and Namasaki's and others have done it that way. Wrong _placement_ maybe, but surely not wrong order.

OK. After double checking Eboosted's it seems that the main neg lead is a culprit. It seems to have supposed to go on the _other end_ of the 4p pack... which makes sense, since the series connections are placed _diagonally_ across the pack. What was I thinking... So thank you rojitor, it seems that's absolutely an error. 

Yep, definitely an error. @Delta_19 had his main neg lead _**at the corner**_. His configuration is different though, but the leads are essentially the same.

![46 AM|690x370](upload://n6ICb2CF6zfKhgBcAOJ2A9kk6B6.png)

But in @oyta's diagram with my same configuration, his leads are _centred?_
 
![25 AM|690x296](upload://8JFdcmPYf2d05R6f6aLTXAU6JP5.png)

I'd be happy to try anything at this point, but will relocating the main neg lead fix things and prevent another short? 

And, if location of wires on the 4p pack is critically important, then, would improperly placed balance wires cause a short?

Thanks again.
```

---
## \#7 Posted by: PXSS Posted at: 2018-02-16T14:49:03.735Z Reads: 157

```
Post detailed pictures of your battery pack. The location of the wire isn't super critical.
```

---
## \#8 Posted by: PXSS Posted at: 2018-02-16T14:56:06.323Z Reads: 163

```
[quote="solideogloria, post:3, topic:46554"]
Yes, battery was plugged into the BMS while soldering.
[/quote]

Dont do this. You would have not shorted anything if the battery was not plugged in. Not saying that it would not have happened as soon as you plugged it in but yeah. You would have only seen big spark and melted the connector but everything else would have been okay. 

E: I'm reading through your posts slowly, trying to figure out what went wrong :)

--- 
Error #2:
 Is the pack welded or soldered?
Looking at your second picture, if it was welded then your welds were weak. No weld should have come undone. If they were solder joints, then your battery is toast and consider yourself lucky that it didn't catch fire.
```

---
## \#9 Posted by: solideogloria Posted at: 2018-02-16T15:02:19.748Z Reads: 159

```
Thank you PXSS. 

To confirm, my balance lead wiring is practically the exact same as @Funktapus. 

Same:
 - BMS Model
 - Wiring

But different:
 - Neg lead location. Like everyone else, he's on the outside edge of the 4p pack. I'm at the inside (wrongly I suppose).
 - Charge port wiring. He's before XT90. Mine's not hooked up yet. It will be after the XT90, spliced with the anti-spark switch.

![41 AM|690x320](upload://lmopvMlmknRVkv7fH9v1oFycwNM.png)


[EDIT]

**Problem identified:** Ah ha! I think I've identified the root problem. **Wrong charge port wiring!** See pic 3 with one red wire. Although it's not connected to a load on the XT90, it _shouldn't have been connected at all_ to the C-. 

I hard wired the main pos lead to C-, _without_ a switch (i.e. charger). :blush: So effectively, I was charging the BMS / battery _with_ the battery, effectively flooding the C- port with far more than the 2amps typical of an average charger. 

Meanwhile, Funktapus' charge port wiring (with black AND red) _separates_ the main pos lead at B-10 (equivalent to my B-8) from C-, a critical separation from shorting the BMS and battery pack.

![54 AM|574x370](upload://zv7yWgGJ2d78fFKPrYci7uQ9ln3.png)

But it still doesn't fully explain how this short happened, because:
1) **The e-switch was _disconnected**_. -- According to the Bestech Datasheet: "During charging and discharging, The Switch should be on(connected)". Thus, a disconnected e-switch should have had _prevented_ the short, if it worked.

2) The BMS has an **over charge detection** voltage of "4.28V±0.025V" (4.255-4.305v). Thus, since my 8s4p pack was registering 26.2v earlier in the day, it would have sent ~3.275v (26.2/8=3.275) into the BMS / battery, which is much less than 4.255v. More precisely, 0.98v less.
```

---
## \#10 Posted by: PXSS Posted at: 2018-02-16T15:04:48.338Z Reads: 142

```
Please read and reply to the edits I make to my post above.
```

---
## \#11 Posted by: solideogloria Posted at: 2018-02-16T15:07:00.312Z Reads: 142

```
By "plugged in" I meant it's all hard wired in, all soldered together. Maybe I'm missing something. I don't understand how a battery is connected to a BMS without soldering it. 

E.g. If a 4mm banana plug is placed between the lead wires, the result would be the same, as you say.
```

---
## \#12 Posted by: PXSS Posted at: 2018-02-16T15:10:03.680Z Reads: 138

```
My BMSs have always come with balance connectors. JST XH connectors. Did yours not come with them?
```

---
## \#13 Posted by: solideogloria Posted at: 2018-02-16T15:10:29.151Z Reads: 139

```
Toast = damaged, or damaged beyond repair? 

Battery is soldered, not spot welded. But it still registers 25.7v on a voltmeter? That's 3.21v per cell, which is OK, right?
```

---
## \#14 Posted by: solideogloria Posted at: 2018-02-16T15:12:35.559Z Reads: 136

```
[quote="PXSS, post:12, topic:46554"]
JST XH connectors
[/quote]

Yes, they came together, and I had them plugged in while soldering. Is that an error?
```

---
## \#15 Posted by: DavidBanner Posted at: 2018-02-16T15:14:21.910Z Reads: 137

```
[quote="solideogloria, post:14, topic:46554"]
Yes, they came together, and I had them plugged in while soldering. Is that an error?
[/quote]

yes, you are not meant to plug in the balance wires via the connector until the rest of the connections have been soldered onto the BMS.
```

---
## \#16 Posted by: solideogloria Posted at: 2018-02-16T15:18:13.709Z Reads: 134

```
Thank you DavidBanner.

> yes, you are not meant to plug in the balance wires via the connector until the rest of the connections have been soldered onto the BMS.

Oh dear. I didn't get that instruction.
```

---
## \#17 Posted by: PXSS Posted at: 2018-02-16T15:52:32.392Z Reads: 127

```
Never have power on electronics when soldering if you can avoid it.

[quote="solideogloria, post:13, topic:46554"]
Toast = damaged, or damaged beyond repair?
[/quote]
Definitely damaged, maybe beyond repair. It'll have to be an extensive repair to make it trustworthy but it can be done. 

I would suggest get them pulled and re heatshrunk
```

---
## \#18 Posted by: solideogloria Posted at: 2018-02-16T15:58:53.132Z Reads: 122

```
[quote="PXSS, post:17, topic:46554"]
Definitely damaged, maybe beyond repair.
[/quote]

Thank you PXSS. How can you be certain? Is there a way to measure your conclusion?
```

---
## \#19 Posted by: Sebike Posted at: 2018-02-16T16:09:44.548Z Reads: 119

```
Don't know how bestech bms'es are designed, but on a supower bms balance wires should never be connected before battery + and -  are connected or bms will fry.
```

---
## \#20 Posted by: PXSS Posted at: 2018-02-16T17:09:02.432Z Reads: 124

```
[quote="solideogloria, post:18, topic:46554"]
How can you be certain
[/quote]
It's my full time job. I design and build batteries for military UAVs. I've shorted plenty of batteries both on purpose and by accident and have honestly never seen batteries get hot enough to damage heatshrink in the manner yours is damaged without catching fire. Its either, they shorted out for a few seconds and are okay or they shorted out and burned. 

[quote="solideogloria, post:18, topic:46554"]
Is there a way to measure your conclusion?
[/quote]
Yes, there is a way but it's not cheap. You need an RC charger that can measure IR. I use an iCharger 4010 Duo but that is definitely overkill for what you need. You can measure IR, capacity and balance the pack with it. Then you can compare that data to the manufacturer specs and see if you're within the limits. 

There is a way to measure IR manually but you need a good multimeter. Again, I use a Fluke 87V but that is overkill for you.

---
E: All the heatshrink damage seems to be on the negative terminals. Not one cell from what i can see on those pictures is damaged on the positive end. Did you damage these before hand or cut the heatshrink for any specific reason? It almost looks deliberate, it's a little confusing.
```

---
## \#21 Posted by: darkkevind Posted at: 2018-02-16T17:20:52.031Z Reads: 110

```
I think the most glaring problem here is that the positive wire is NEVER (in my experience) connected directly to the BMS, which what you've done here...
```

---
## \#22 Posted by: ZackoryCramer Posted at: 2018-02-16T17:40:29.272Z Reads: 111

```
I would use a standard 80 amp fuse on the xt90 out and Tesla fuses between the balance leads 🔋🗯 for maximum protection 🧐

Next time, solder on the balance leads unplugged and double check each grove with a volt meter.
```

---
## \#23 Posted by: PXSS Posted at: 2018-02-16T18:04:41.612Z Reads: 105

```
Yep! I missed that edit. That would be a direct short across the battery. But the FET diodes should have protected the battery. Something is still wrong with the BMS, I'll look at the spec sheet.
```

---
## \#24 Posted by: solideogloria Posted at: 2018-02-17T01:18:41.680Z Reads: 106

```
> All the heatshrink damage seems to be on the negative terminals. Not one cell from what i can see on those pictures is damaged on the positive end.

Yes, I now suspect the damage came from the C- port. I assume the current flowing via the main neg lead damaged the subsequent neg terminals.


[quote="PXSS, post:20, topic:46554"]
Did you damage these before hand or cut the heatshrink for any specific reason? It almost looks deliberate, it’s a little confusing.
[/quote]

Negative. 

I thought I did everything correct, up until:
- Plugging the balance wires in
- Connecting the main leads in the wrong order
- Connecting the main pos lead (disastrous)

This is the battery pack pre-soldering the BMS:

- Cardboard rings on pos terminals
- Each cell shrinkwrapped (clear)
- Hot glued together
- Nickel strips soldered to every terminal

![DSC03063|690x388](upload://1A5tt6d4efSUSGmZJfP45KVIjVU.JPG)
```

---
## \#25 Posted by: solideogloria Posted at: 2018-02-17T01:22:58.002Z Reads: 101

```
Thank you Sebike.

Yes, it seems they're the same in that regard. I don't know how I missed that instruction. My BMS definitely fried, and would have burnt down the table, if not the house.
```

---
## \#26 Posted by: solideogloria Posted at: 2018-02-17T01:58:14.364Z Reads: 106

```
[quote="darkkevind, post:21, topic:46554, full:true"]
I think the most glaring problem here is that the positive wire is NEVER (in my experience) connected directly to the BMS, which what you’ve done here…
[/quote]

Thank you darkkevind.

It seems I connected the pos lead to the BMS by mistake. I'm devastated at the outcome. :disappointed_relieved: 

Still uncertain how it all happened exactly though, because:
1. Not everything was plugged in (e-switch disconnected)
2. P- disconnected
3. Most importantly, while the main neg lead was connected to B- and the main pos lead was then mistakenly connected to C- it _did not_ short immediately. Had it done so, it would have been obvious there was a direct short taking place. That is, I soldered it a couple of times, _maybe even a few times_, adjusting the angle of the wire slightly and adding more solder for a shinier solder joint.

[EDIT] I quote @Namasaki back referring to the same BMS model.

[quote="Namasaki, post:6, topic:39082"]
Seems like **the D223V1 could detect a short at very low current.**

**Once I shorted my charge port and the bms shut down instantly so that there was no damage to batteries, electronics or wiring.**

Only the pins in the charge port suffered arc damage.

Well, maybe that was high current but only for a fraction of a second.
[/quote]

My case is similar to his, but without load connected, and without the charger connected. Even though I directly connected the main pos lead to the C- port of the BMS, the e-switch was off, and even if it switched on (somehow), the BMS really should have done the same thing it did for Namasaki (shut down immediately and protect batteries).



@PXSS  I think you've identified a core problem, within the problem. Clearly, I've made errors, but it doesn't make complete sense. In comparison to Namsaki's case, my outcome seems far too drastic and inexplicable.

[quote="PXSS, post:23, topic:46554"]
But the FET diodes should have protected the battery. Something is still wrong with the BMS
[/quote]

Yes, even if the main pos lead was connected to the C-, the BMS should have protected the battery. Right?

Are the FET diodes the black mosfet panels along the top of the BMS? If so, I recall them slowly erupting in smoke and igniting in flames _sequentially, from left to right. 

I recall putting out the first lot of flames before dragging the board outside onto the driveway (that's how the battery drooped out of shape, while hot glue had melted) and minutes later the mosfet panels / FET diodes smoked again and ignited into flames again.

See pic 3, on the balance lead side. The mosfet panels / FET diodes are more burnt than the other side. 

Also, notice the B- port. The B- port / the main neg lead melted & popped off the BMS tearing some PCB. Something definitely went wrong on there, while the C- port / red main pos lead remain unscathed (apart from melted hot glue). 

Perhaps this follows the logic that current flowed through the main pos lead > the C- port > the mosfet panels / FET diodes (and burning them) > throughout the battery (and burning some neg terminals) > ultimately burning the B- port to the point of disconnection. :face_with_monocle:
```

---
## \#27 Posted by: solideogloria Posted at: 2018-02-17T02:20:28.689Z Reads: 99

```
[quote="ZackoryCramer, post:22, topic:46554"]
I would use a standard 80 amp fuse on the xt90 out and Tesla fuses between the balance leads :battery::right_anger_bubble: for maximum protection :face_with_monocle:
[/quote]

Thank you ZackoryCramer.

Yes, some have focused on the balance lead issue (being plugged in whilst soldering - clearly an error it seems), but I don't understand how that caused malfunction. There was no heat, no spark, etc, coming from them whilst connected, and post-short they were unscathed. No melted glue. Nothing.

> I would use a standard 80 amp fuse on the xt90 out

Interesting suggestion. Please elaborate.

That sounds fine, but I wonder is that not excessive to the BMS's job, and the XT90's job? And the 80a fuse would be to protect the anti-spark switch / VESC more than the battery, right? Which would also be a bit redundant on the anti-spark switch, right?

I quote Bestech's BMS datasheet. See 80a max discharge current:

![57 PM|690x70](upload://l5LvmbH9sUCYPzJlVQe8Kl9SkjW.png)

> and Tesla fuses between the balance leads

What rating are the fuses? So,your suggestion would mean running fuses _inline_ per balance wire, right? i.e. 8 fuses, per 8 balance wires. Again, that would seem excessive and redundant since the BMS itself should be regulating. I'd have thought that's what the BMS is for.

Again, I quote Bestech's BMS datasheet. See overcharge protection, over discharge protection, and over current protection:

![01 PM|690x220](upload://j2kfumah2Dua7coTSH7CTjopNx1.png)
```

---
## \#28 Posted by: solideogloria Posted at: 2018-02-17T02:44:40.570Z Reads: 91

```
[quote="PXSS, post:20, topic:46554"]
It’s my full time job. I design and build batteries for military UAVs. I’ve shorted plenty of batteries both on purpose and by accident and have honestly never seen batteries get hot enough to damage heatshrink in the manner yours is damaged without catching fire. Its either, they shorted out for a few seconds and are okay or they shorted out and burned.
[/quote]

@PSXX How devastating to read... :sweat: 

But, yes, while I'm grateful for your input and I don't doubt your qualification, but what you've written is not a reason for your conclusion. Can you perhaps elaborate and explain _how_ heatshrink damage equals battery damage, and give examples of cases you've experienced? 

Because as you've correctly noticed, _the battery did not catch fire_, and it's still registering 25.7v (3.21v per cell), which looks fine to me? Very optimistic. 

At 3.21v per cell (and no less), the BMS seems to have actually done it's job. As mentioned earlier, it went from 26.2v (3.28v per cell) to 25.7v (3.21v per cell) during the short.

I quote the Bestech BMS Datasheet. See over discharge protection / over discharge detection voltage at "3.00V±0.05V".

![14 PM|690x72](upload://aS9dr2oe6poPHA5BXyCS5IuCzVh.png)

I hope you have some more optimistic news. Because in the condition that it is right now, I'd honestly like to repair it, plug it in and run it again as per normal. But I wonder what would happen? What are the pros and cons of doing so?
```

---
## \#29 Posted by: ZackoryCramer Posted at: 2018-02-17T03:28:35.843Z Reads: 93

```
Giving trust to the battery pack(cells with strips and wires holding it together), the only way for a battery to malfunction is physical damage or unwanted load through the cells. The best way to do this is to use protected cells but they are a quater or more expensive and only available prebuilt in Panasonic NCR18650B. Or we can fuse all outputs which would be the BMS balance leads and outputs. Using a fuse like this one:

https://www.amazon.com/Absolute-ANL80-2-Pack-Fuses-Plated/dp/B005EUTU5W

in series before either + or - terminals, we can prevent current over draw physically(the current bridge is burnt). We can further improve unwanted output in the BMS balance leads through 26 awg wires which starts to melt down after 3~4 amps(compared to the max balancing 200ma current draw). Yes they aren't really Tesla fuses, I mean to say Tesla Style. I learned it here:

https://www.youtube.com/watch?v=raBWFsPlx7w
```

---
## \#30 Posted by: solideogloria Posted at: 2018-02-17T06:57:26.542Z Reads: 84

```
[UPDATE]

Balance wires via a voltmeter read:
- B1: ? -- How do I measure this cell?
- B2: 3.28v
- B3: 6.38v
- B4: 9.61v
- B5: 12.8v
- B6: 16.0v
- B7: 19.3v
- B8: 22.5v -- Why is not 25.7v (as read between main pos and neg leads)?

**Amended the battery pack & BMS wiring:**
- Repaired desoldered nickel strips
- Clamped the whole pack back into shape while re-heating hot glue obstructions (because bulges of glue were everywhere)
- Hot glued over the exposed unheashrunk cells (no cells remain exposed for risk of short)
- _Unplugged_ the BMS balance leads
- _Desoldered the problematic main pos lead at the C-_ and _spliced out new wires to the charge port_. Then heatshrunk the fat solder joint before finishing the XT90 plug.
- Cleaned the C- port and re-tinned it ready for connection to the charge port _negative_ wire (not pos which contributed to the short).
- Added new nickel strip layers to the neg terminal at B1, and relocated the main neg lead to the outside edge of the pack (not the inside).

The original nickel strips are too hard to remove (super securely soldered, and reinforced) so instead I made this guy with layers of nickel strip in the opposite direction for the correct reinforcement. 

@PXSS had me concerned about the main neg lead being too close to the pos terminals at B3, so I redirected it own the pack with ample hot glue insulation.

![DSC03074|690x388](upload://5dJuXdwsnrr4tdwWYyqs6rnpQVC.JPG)
![DSC03076|690x388](upload://n1Ep5ZytuJ3FBLew03TgL2qKZmS.JPG)

Ideally, I'd have rebuilt the entire pack as @PXSS suggested but it's way too much work when everything is mostly OK. I'm also low on heatshrink for the 198650 cells. And, desoldering and resoldering the nickel strips will apply what I think is unnecessary heat to pack. In my mind 25.7v looks fine.

Oh.. I'm so regretful, everything was tidy and quite pristine before the short. None of it was meant to be this sloppy. Had to learn the hard way, as usual. :blush:

![DSC03062|690x388](upload://9GInrNVCaGBgRHzppS9myR7noHt.JPG)
```

---
## \#31 Posted by: solideogloria Posted at: 2018-02-17T08:16:25.953Z Reads: 79

```
Thank you ZackoryCramer.

80a fuse: Brilliant. Yes, quite right, I'll hook up fuses asap. I prefer the blade fuse design though, for easy replaceability while out and about.

Tesla-style wire fuse: 26awg melts at3-4 amps does it? Fascinating. I wonder if a similar inline resistor will work the same. But, replaceability while out and about will be difficult and inconvenient.
```

---
## \#32 Posted by: GrecoMan Posted at: 2018-02-17T14:00:37.884Z Reads: 75

```
go for a maxi fuse. 
Blue Sea Systems 80A MAXI Fuse https://www.amazon.com/dp/B000K2ILMC/ref=cm_sw_r_cp_api_zwdIAbQ66BNZK
```

---
## \#33 Posted by: PXSS Posted at: 2018-02-17T14:15:32.525Z Reads: 77

```
Another tip. Do not use hot glue. Everything inside your enclosure is at the very least going to get to 50-60c, hot glue melting point is at like 80-100c? Not exactly sure. Either way, at 60, hot glue is ductile which isn't good for keeping things in place. 

I use amazing goop if I want something that isn't permanent as it doesn't go ductile with high temps and can still be removed. If I want something permanent then I use Thick CA.

---
E:
[quote="solideogloria, post:30, topic:46554"]
Balance wires via a voltmeter read:

B1: ? – How do I measure this cell?
B2: 3.28v
B3: 6.38v
B4: 9.61v
B5: 12.8v
B6: 16.0v
B7: 19.3v
B8: 22.5v – Why is not 25.7v (as read between main pos and neg leads)?
[/quote]
You're supposed to measure between main neg and the balance pins. I assume you were measuring relative to pin 1 in the connector. Also, you should measure in the following manner:

Main neg - pin 1
Pin1-pin2
Pin2-pin3
Pin3-pin4
Pin4-pin5
Pin5-pin6
Pin6-pin7
Pin7-pin8

All of them should measure 3.XX volts and ***should have a max spread of 0.1v*** to be balanced properly.

---
From what you posted above:
Cell 1:?
Cell 2: 3.28
Cell 3: 3.10
Cell 4: 3.23
Cell 5: 3.19
Cell 6: 3.20
Cell 7: 3.30
Cell 8: 3.20
So you have an imbalance of 0.2v which is up to 15% imbalance.
```

---
## \#34 Posted by: oyta Posted at: 2018-04-08T07:56:53.593Z Reads: 60

```
Sorry, I missed that you mentioned me quite a while back! How did everything go?

I have tried to read through the thread and it seems you've got good answers. It would be beneficial to you gaining some basic electronic knowledge. Then you would be certain how to measure voltages, connect battery packs etc.

> The BMS has an over charge detection voltage of “4.28V±0.025V” (4.255-4.305v). Thus, since my 8s4p pack was registering 26.2v earlier in the day, it would have sent ~3.275v (26.2/8=3.275) into the BMS / battery, which is much less than 4.255v. More precisely, 0.98v less.

You wrote this. How I understand this over charge detection voltage is that it must reach those 4.28V (+-0.025V) before it stops charging. Which it didn't. The over current threshold is 200A which I do not think your battery is able to provide, and then that threshold was never reached either.
```

---
