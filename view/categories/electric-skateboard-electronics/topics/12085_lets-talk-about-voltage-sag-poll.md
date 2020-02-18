# Lets talk about &ldquo;Voltage Sag&rdquo;&hellip; \[POLL\]

### Replies: 65 Views: 6116

## \#1 Posted by: evoheyax Posted at: 2016-10-28T16:37:06.549Z Reads: 551

```
Voltage sag is one of the issues I've seen many complain about with the Evolve CGT. It's an issue I think is pretty prevalent in the DIY community. the easiest way to escape voltage sag shutting down your board is simply to using a bigger battery pack. But sometimes, that's just not an option.

So I wanted to start a discussion about things that some in our community have done to deal with voltage sag. I also want to see how much people can sag their battery.

So how low can you go % wise before you sag your way down to 0% (in the worst case scenario)?
[poll public=true]
* less than 10%
* 10%-19%
* 20%-29%
* 30%-35%
* higher than 35%
[/poll]

And to those with more knowledge about voltage sag and solutions, please post away your thoughts and advice for the community :P
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-28T16:42:19.474Z Reads: 496

```
To mitigate sag, you have to leave as much buffer room as you can between maximum actual current under load and maximum rated discharge current. Best way to do this is to use prismatic cell lipos. Otherwise building a huge parallel pack would work as well. I don't sag much on my route 5~% and I never go too low to prolong cycle life. I put 10-19% for now, but I'm sure it'd be a lot higher if I went up insane hills.

Hubs, I imagine, would sag worse since they need more current than belt drives.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-10-28T16:46:00.294Z Reads: 474

```
I have a lot of hills on my route. I sag very little on flat ground, but when I go to tackle some steep hills, it can easily sag 25% or more, depending on the hill.
```

---
## \#4 Posted by: Jinra Posted at: 2016-10-28T16:47:24.642Z Reads: 455

```
That's pretty crazy. My Evolve GT sagged pretty bad, but I'm pretty sure they designed the throttle to be too aggressive on their ESC. Also, pretty sure they're using bad cells for their battery.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-10-28T16:51:50.309Z Reads: 424

```
Well, I am using 4wd with hubs, and I pull 80 amps (which is the max for my 12s4p battery) on steeper hills. Mind you, this is on a hill that was 25% grade.... But still... I think 12s6p or maybe even 12s8p would be the perfect battery for my board, but that's a bit too much, haha/
```

---
## \#6 Posted by: johnny_261 Posted at: 2016-10-28T17:34:30.355Z Reads: 397

```
Will you get less sag from say A123 26650 cells like in the boosted?
```

---
## \#7 Posted by: Pantologist Posted at: 2016-10-28T18:01:02.882Z Reads: 384

```
I have A123 cells in 12S1P config and I still get decent sag up hills. From Nominal voltage per cell of 3.3v, I drop to around 3v per cell while going up decent hills.

A 12S2P pack of these cells would be great.
```

---
## \#8 Posted by: johnny_261 Posted at: 2016-10-28T18:24:40.311Z Reads: 361

```
Yeah I was thinking about a 12S2P for my next build with A123. 

Do you have any boards with different battery setups.  Just trying to get an idea of what a A123 26650 12S1P setup is like.  In terms of sag would it be like 10S3P with 18650's roughly?
```

---
## \#9 Posted by: Pantologist Posted at: 2016-10-28T18:26:09.219Z Reads: 344

```
I only have the A123 setup so far. I'm thinking of 12S2P 18650 cells for my next build too.
```

---
## \#10 Posted by: Jinra Posted at: 2016-10-28T18:34:48.774Z Reads: 344

```
Yea since 26650  A123's have 70A discharge, you'll have sag similar to something between 10s3p and 10sp4 18650's.
```

---
## \#11 Posted by: johnny_261 Posted at: 2016-10-28T18:45:46.093Z Reads: 328

```
Thanks for confirming. Just wondering if anyone in practice has some real world experience to see if it actually behaves like that.  All makes sense from a theoretical perspective.
```

---
## \#12 Posted by: Jinra Posted at: 2016-10-28T18:56:26.063Z Reads: 318

```
You could ask anyone with a boosted board. They'll have to look at their mobile app while riding.
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-10-28T19:15:53.694Z Reads: 314

```
i build my packs to handle 80 amps continuous and i use a BMS that handles 60 amps continuous. Because of that, i've not seen one of my boards shut down due to voltage sag yet. I'm not saying it couldn't happen, it just hasn't. 

So yeah, there's something to the "big pack" approach that works. I use 12S 4Ps made from sammy INR-18650s.
```

---
## \#14 Posted by: evoheyax Posted at: 2016-10-28T19:45:43.053Z Reads: 309

```
What are the max con amps you've drawn using your board @longhairedboy ?

I am using essentially the same pack but I sag a lot on hills, because I get close or hit my 80 amp limit on super steep hills. Most of the time, I sag less than 10%...
```

---
## \#15 Posted by: jmasta Posted at: 2016-10-28T19:46:46.536Z Reads: 303

```
What voltage are you running if you are pulling close to 80A?
```

---
## \#16 Posted by: evoheyax Posted at: 2016-10-28T19:47:41.933Z Reads: 301

```
50.4v 12s about as high as the vesc can do...
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-10-28T20:00:18.625Z Reads: 299

```
i've got my abs max set at 130 usually.
```

---
## \#18 Posted by: evoheyax Posted at: 2016-10-28T20:02:27.003Z Reads: 299

```
I mean like, what is the most amps you've recorded drawing from your vesc from your battery?
```

---
## \#19 Posted by: Rob.Endless Posted at: 2016-10-28T20:19:57.748Z Reads: 298

```
I've had the Carbon GT since a few days after the U.S. launch date and I haven't had the voltage sag causing the board to shut down issues ever. I never knew that was even an issue. The voltage sag does makes the battery life percentage unreliable to look at while on the throttle as it does drop. I just look at the trip meter a lot to see how much longer I can ride.

Good thing I live in a non hilly area, the voltage sag hasn't slowed me down on flat roads so far.
```

---
## \#20 Posted by: evoheyax Posted at: 2016-10-29T03:04:17.058Z Reads: 285

```
[quote="Rob.Endless, post:19, topic:12085"]
Good thing I live in a non hilly area, the voltage sag hasn't slowed me down on flat roads so far.
[/quote]


hat's exactly why you haven't had issues. They seem to be fine on flat ground. But steep hills apparently make it sag down to 0% from 30%.
```

---
## \#21 Posted by: Rob.Endless Posted at: 2016-10-29T04:08:51.840Z Reads: 267

```
Lol so true, I even swapped out the stock 15t pulleys for 20t pulleys and still problem free. Gear ratio of 1.6:1 versus stock 2.13:1 or 2.53:1 (optional 38t drive gears) I definitely can't pull this off in a hilly area, especially with 97mm flywheels. With the Kegels, it climbs hills quite okay considering the gear ratio.
```

---
## \#22 Posted by: BoardSportsRN Posted at: 2016-10-29T23:22:33.152Z Reads: 257

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#23 Posted by: evoheyax Posted at: 2016-10-29T23:43:19.630Z Reads: 256

```
I've been quite a bit of battery research the last few days. And It really seems to do with the amps getting too high for the battery pack. If you run an efficient drive train system (like enertion), you can do very low amps. I use hubs mostly, so that means amps are even more of a problem. I'm thinking of make a super thick board that has a hollow 2 hollow channels 36 x 330 x 76 mm each. You could fit a vesc-x and 60 cells for a 12s5p (without a bms, which is how I've ridden since July with no issues or balancing needed), or a 10s5p with a charging only bms. Total cruiser dimensions will be 34 inch x 8.5 inch x 42 mm chubby board. That would push the amp limit up to 100a con, which should help with the sag.
```

---
## \#24 Posted by: barajabali Posted at: 2016-10-30T05:32:41.787Z Reads: 246

```
10s8p/12s7p packs no sag to report here
```

---
## \#25 Posted by: guyguy Posted at: 2016-10-30T14:19:20.123Z Reads: 240

```
Haven't been able to get on a long ride since Bara helped me out with my battery issues. Prior to that, high headwinds on flats could cause the low voltage cutoff to trip.
```

---
## \#26 Posted by: Brad Posted at: 2016-10-31T01:38:05.390Z Reads: 232

```
My daily work commute is 11kms making it 5.5kms each way. 

On the way back home from work, the battery would read 89% before leaving the work depot, but at the last main hill at the 4 Km mark, I can actually sag the battery to cut off. After I stop at the top of the hill, the battery would read 60%.

When ever I approach that hill, I have to actually monitor the % and let go the trigger a bit when it hits 2% and it would go up to about 12% till I get to the top. It sure would be nice to just leave that to a program and enjoy the ride.

This issue have got me thinking about going DIY for an AT board if I can find something that would manage the sag by auto slowing down. Would try to keep the GT AT wheels and maybe use that with Enertion motors and a longer board.

Evolve info and weight - Bamboo GT with AT wheels in FAST mode and my weight with backpack is at 100kg/220lbs.
```

---
## \#27 Posted by: Jebe Posted at: 2016-10-31T04:38:58.315Z Reads: 221

```
you can see the battery voltage readout by pressing reverse button then scroll down 2 steps. Can even see individual cell voltages.
```

---
## \#28 Posted by: BoardSportsRN Posted at: 2016-10-31T18:03:31.641Z Reads: 214

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#29 Posted by: evoheyax Posted at: 2016-10-31T20:27:45.320Z Reads: 209

```
That sounds like a really bad technician they have working for evolve... How can they even make a such mistakes?
```

---
## \#30 Posted by: Rob.Endless Posted at: 2016-10-31T20:46:43.892Z Reads: 208

```
I never knew that, i will check it out once i get home later today. Thanks for the info.
```

---
## \#31 Posted by: TheRedPanda Posted at: 2016-11-03T05:48:31.071Z Reads: 206

```
I run 12S1P A123. It's absolutely excellent.charges super fast and I never have enough voltage sag that it's even noticeable.

edit: by voltage sag I mean a noticeable lack in power/top speed due to a lowering of charge from use or from strain.
```

---
## \#32 Posted by: johnny_261 Posted at: 2016-11-03T07:18:33.690Z Reads: 208

```
awesome. I'm going to do it.  what bms are you using? Just gotta find some cells now!
```

---
## \#33 Posted by: Jinra Posted at: 2016-11-03T14:58:42.832Z Reads: 210

```
keep in mind lifepos are a bit heftier and aren't as energy dense as liion
```

---
## \#34 Posted by: Mellow Posted at: 2016-11-04T00:15:22.344Z Reads: 209

```
Hi, we're wondering why the discussion is around bigger packs when the real problem is that voltage reading alone is an inaccurate fuel gauge? The DIY already has two open source BMS that monitor current and profile battery resistance (Impedance Track, sorry for the caps, but it's a Texas Instruments trademark. ;-)), DieBieMS and Battman (both are in threads elsewhere.)

Fun (if you're into it) educational video here: https://youtu.be/A6oeL2ltKL0

An update coming soon will talk about Mellow's own BMS. Yes, we use all three methods. The BMS is located in the (removable)  battery pack itself.
```

---
## \#35 Posted by: evoheyax Posted at: 2016-11-04T00:31:38.668Z Reads: 205

```
Many are likely getting readings from inaccurate fuel gauges. How, with the new iphone app I have been developing (Vesc Status), I can monitor sag in live time with the data that the vesc is seeing. This data seems to be accurate, and has shown me that even with a 12s4p 18650 LG HE2 in my config, I sill have a voltage sag of around 25-30% on hills of 20%+ grade. I will add a specific tool in my app to measure voltage sag specifically in the background while you ride so that this can be monitored more accurately in the future by the community. I do agree those fuel gauges are often surprisingly inaccurate. I also use volt monitors on my board which have been very accurate. I calibrated them, and have noticed every time I check, they are within .1 volt of accuracy.

Thanks for dropping in though and giving some perspective ;)
```

---
## \#36 Posted by: TheRedPanda Posted at: 2016-11-04T03:54:47.121Z Reads: 191

```
I'm working on a company, we use a custom BMS. I will be posting a thread on the forum introducing the brand when we have a date for our Kickstarter.
```

---
## \#37 Posted by: BoardSportsRN Posted at: 2016-11-04T03:59:15.559Z Reads: 188

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#38 Posted by: jmasta Posted at: 2016-11-04T05:03:31.016Z Reads: 192

```
When discussing voltage sag, it would be helpful to mention terrain.  Voltage sag on flats is minimal but can be significant when climbing hills (high current draw).  If you live in, say, Florida, you won't be pulling much current.  Hilly terrain is a whole different story, and you may draw in excess of 60A, depending on your setup and current limitations.

An A123 18650 battery has a continuous discharge rating of 30A.  Check out the voltage sag in this published diagram.  It just seems hard to believe that a 1P pack wouldn't have noticeable voltage sag, even at 12S

<img src="/uploads/db1493/original/3X/b/6/b699ad567497f79f37ec5d96f0aa467fcdb0d1bf.jpg" width="609" height="500">
```

---
## \#39 Posted by: Jinra Posted at: 2016-11-04T05:49:58.578Z Reads: 178

```
You're looking at the wrong A123 cell. 26650's is the lifepo cells people typically talk about which is rated for 70A discharge.
```

---
## \#40 Posted by: jmasta Posted at: 2016-11-04T06:23:28.790Z Reads: 189

```
Roger that. Thanks for the correction

**A123 26650**

<img src="/uploads/db1493/original/3X/5/1/5151a9d435fa1ff82ad52ba2456dffe880bc5108.png" width="690" height="396">
http://www.a123systems.com/Collateral/Documents/English-US/A123%20Systems%20ANR26650%20Data%20Sheet.pdf
**Samsing 25R 16650**


<img src="/uploads/db1493/original/3X/4/8/487a4a13a6aa82cd2ad608376170e056b0405590.png" width="642" height="499">

More charts for 25R here: https://www.powerstream.com/p/INR18650-25R-datasheet.pdf
```

---
## \#42 Posted by: E-Boarding Posted at: 2016-11-04T12:22:55.386Z Reads: 176

```
[quote="BoardSportsRN, post:22, topic:12085"]
The manufacturer of the battery used in the GT told me he thinks there is "something wrong" with the packs.
[/quote]

Do you have more details on that?
Whats cells are used in the GT and what is their discharge rating?
```

---
## \#43 Posted by: evoheyax Posted at: 2016-11-04T14:55:43.255Z Reads: 170

```
4wd hub motors. Hubs eat up more current, on steep hills, I can pull 80a across the 4 motors (which is the max continuous of my pack). The reality is, on flat, I sag very little. But on hills, it's another story.

Part of me is thinking I might be better going back to lipos so I can do higher amps again. 80a max is not always enough for me, even at 12s.
```

---
## \#44 Posted by: SORRENTINO Posted at: 2016-11-04T15:03:21.499Z Reads: 168

```
Higher C rating and better IR in cells will give you what you seek.
```

---
## \#45 Posted by: Mellow Posted at: 2016-11-06T15:51:14.913Z Reads: 167

```
** deleted because wrong **
```

---
## \#46 Posted by: DeathCookies Posted at: 2016-11-06T16:07:18.700Z Reads: 163

```
Could you provide and example?
```

---
## \#47 Posted by: evoheyax Posted at: 2016-11-06T16:11:40.015Z Reads: 168

```
[quote="Mellow, post:45, topic:12085"]
There will be more sag in longer serial configurations
[/quote]

I guessing this is due to the fact you have a wider voltage window, but how can you define Vs = Vw*N, for N is the number of cells (and number of cells in the entire pack, or the number in series?)? That doesn't make much sense. For example, I run 12s, so my usable windows is 38.4v to 50.4v, so 12v is my usable window for my entire pack. According to your formula, it's also my sag. But I sag at most 3v under high loads if I'm in the right part of my battery pack (fully charged for example, because that first 2 volts or so drop off quickly). I never sag 12v, so I don't get what you formula is telling me, other than the range of my batter's voltage.

Maybe we are talking about different sags... We are talking about the sag under load, not from using the energy out of the cells through normal discharge.

From another forum, I found this:
> For instance if the internal resistance is 50 milliohms (0.05 ohms), 
> then the voltage sag on a 6 A load would be 6 x 0.05 = 0.30 V.

Which seems more like the sag we are after. So...

sag = load * resistance

Can anyone confirm or deny this formula? My understanding prior to finding this was that resistance directly affects sag, which is true in this formula.
```

---
## \#48 Posted by: Mellow Posted at: 2016-11-06T17:18:05.126Z Reads: 162

```
Sorry.. Misquoted a conversation with our tech guy Kilian (again): Max SOC window was the formula described as voltage windows * number of cells. 

Should have written "There will be more sag in longer serial configurations (comparatively). Max SOC window is the usable voltage window of a cell times the number of cells. Draw from a 2p setup with have much less sag than from a 1p, since the draw is distributed over 2 cells and thus resistance will be significantly lower."
```

---
## \#49 Posted by: evoheyax Posted at: 2016-11-06T18:13:19.392Z Reads: 161

```
So your saying a 6s1p will have less sag than a 12s1p, since the 6s has a smaller serial configuration?

And that the resistance is less in say a 12s2p than a 12s1p, which is why we experience less sag?

So say a cell has say a 20 milliohms of resistance. If I run it in a 1p, I would have 20 milliohms of resistance, while in a 2p, I would have only 10 milliohms of resistance?
```

---
## \#50 Posted by: Mellow Posted at: 2016-11-06T20:51:52.796Z Reads: 162

```
[quote="evoheyax, post:49, topic:12085"]
that the resistance is less in say a 12s2p than a 12s1p, which is why we experience less sag?

So say a cell has say a 20 milliohms of resistance. If I run it in a 1p, I would have 20 milliohms of resistance, while in a 2p, I would have only 10 milliohms of resistance?
[/quote]

Sorry, forget the serial length statement. There's a monkey at the keyboard. 

As Sorrentino put succinctly and you earlier correctly surmised, it's all about internal resistance. Your formula is correct. 

As in your example, more cells in parallel will distribute the current and experience less IR.
```

---
## \#51 Posted by: BoardSportsRN Posted at: 2016-11-07T00:23:56.305Z Reads: 155

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#52 Posted by: rodriguejoe1 Posted at: 2016-11-07T00:58:12.932Z Reads: 165

```
[quote="BoardSportsRN, post:51, topic:12085"]
I do not own a GT anymore so I quit caring.
[/quote]
OUCH!
10 CHARACTERS
```

---
## \#53 Posted by: cliofreak Posted at: 2018-02-22T22:47:01.075Z Reads: 116

```
Hey,

I have serious voltage sag when going up medium hill and pretty much just stops on steeper inclines.
Im running 10s4p 30Qs with Vesc and 6374 200KV motor.

I think it might be because Ive got conservative settings in my Vesc but I could be wrong. Here is a bit of a screen grab from the Metr app. Any ideas whats going on!?

When I pushed it up the same hill for 20 secs then jumped on and gave it power, it starting pulling really well... for about 15secs then starting bogging again. 

These readings are from a 15min ride with some flat areas and down hill in parts too. The last 5 mins was a significant hill but I felt the bogging even on a slight incline. 

![08|690x116](upload://sAEnFxE8Xyb6DQEIlBUhoBdwi1l.png)![59|690x86](upload://jYAwql3bKLHKcOayzHh2IJpQnD6.png)
```

---
## \#54 Posted by: jmasta Posted at: 2018-02-23T19:37:16.278Z Reads: 109

```
Post the full Metr log. If you paste in the URL, it will load automatically
```

---
## \#55 Posted by: E1Allen Posted at: 2018-03-13T19:40:12.259Z Reads: 109

```
[quote="cliofreak, post:53, topic:12085"]
I have serious voltage sag when going up medium hill and pretty much just stops on steeper inclines.

Im running 10s4p 30Qs with Vesc and 6374 200KV motor.
[/quote]

Even conservative battery settings should yield 60a continuous.  What are your settings in the VESC.    What's your battery cutoff start and end? Also I see you're close to 80C on temp and somehow only pulled up to 27a Max.  Also what are your Max and min settings? Seems like you could post some more data to get a better idea.  

I also have some voltage sag.  12s6p 30q dual setup.  If I have 30% left and I accelerate hard I can see it drop to 0 %.  But I don't have any conservative settings either

https://metr.at/r/yeQ5W

Data is from one FocBox.  I have two but it only have data from one so double the amp and wh
```

---
## \#56 Posted by: Jebe Posted at: 2018-03-13T21:50:53.625Z Reads: 103

```
Check the welds. May only be running on a10s2p
```

---
## \#57 Posted by: cliofreak Posted at: 2018-03-14T10:04:06.107Z Reads: 100

```
Interesting... I have actually wondered about the % drop after my last ride (maybe 7km). It did seem to use more battery than I was expecting. Im wondering how it could be 10s2p instead of 4p. Im trying to think, where in the welds could break to give less p while also still functioning?
```

---
## \#58 Posted by: evoheyax Posted at: 2018-03-14T19:14:06.454Z Reads: 97

```
You will not experience 100% p failure. One p might lose a cell, which would decrease your range. But it would be easy to spot because one p would keep getting lower than the rest of the pack. You balance it, and ride till empty again, you would notice 1 of the p lower than the rest always. So something like that is not too hard to pick up on. I would start by checking the voltages of each p when the battery is below 25% full. The reason being in a 4p, 1 cell is 25% of the battery, so if your at 25% left on most p's, and on 1, you have 0% or around that, then you'll know one cell has broken lose.
```

---
## \#59 Posted by: longhairedboy Posted at: 2018-03-14T19:17:40.931Z Reads: 99

```
everything @evoheyax said. 

also, if you have not done so already, pick up a set of dental picks from the local flea market or online somewhere. You can use those to tug upwards on the nickel to see if any of the welds are loose.
```

---
## \#60 Posted by: Jebe Posted at: 2018-03-14T20:23:31.566Z Reads: 96

```
second hand dental picks? Think I need to buy a board from you to help support you !

@cliofreak look for something like this 
![29196494_1111858972289922_3466731192823316480_o|375x500](upload://6JsOZB34r9rrG99JaYe8tyW7hbt.jpg)![29214568_1111858988956587_5052781835491213312_o|375x500](upload://k9JCL259CxNF16JfCHPODUT2dB5.jpg)
```

---
## \#61 Posted by: E1Allen Posted at: 2018-03-15T05:52:44.876Z Reads: 88

```


So Mostly full batteries pulling 111A still sags 7v...

![IMG_4606|281x500](upload://sO6tc93HD7CxkoJbvkaVWPPNoMJ.PNG)![IMG_4605|281x500](upload://qa00Kz37vk6ObjG6ClyKDC4151o.PNG)
```

---
## \#62 Posted by: E1Allen Posted at: 2018-03-15T06:01:27.448Z Reads: 86

```
![IMG_4607|690x388](upload://8Fx7qONI6RrDhKGBrkhXJvWZXW3.jpg)

So apparently if you look at discharge curves you see 7 volts of sag on 12s is normal for these cells.
```

---
## \#63 Posted by: PXSS Posted at: 2018-03-15T08:37:16.120Z Reads: 80

```
111A / 6 = 18.5A/cell. 
Sag should be .4V/cell
0.4* 12 = 4.8V sag

The rest of your sag is most likely coming from the losses in nickel strips/wires/ESC. All that is required to lose 2V is 18mOhm of in line resistance which is more than acceptable. If you were to measure voltage directly across your battery, you would see that it doesn't sag that much but since you are measuring at ESC, you have to take those losses into account
```

---
## \#64 Posted by: E1Allen Posted at: 2018-03-15T09:32:05.510Z Reads: 76

```
[quote="PXSS, post:63, topic:12085"]
since you are measuring at ESC, you have to take those losses into account
[/quote]

Maybe I'll just throw another 1s6p in the line for fun.  Then I'll get my losses back! 🤔🤔🤔
```

---
## \#65 Posted by: longhairedboy Posted at: 2018-03-15T12:10:01.102Z Reads: 71

```
[quote="Jebe, post:60, topic:12085"]
second hand dental picks?
[/quote]

nobody said anything about second hand. You can get new ones cheap. I got a whole set for $5. I would also recommend getting a spudger set.
```

---
## \#66 Posted by: MoeStooge Posted at: 2018-03-15T14:22:05.320Z Reads: 67

```
SPD1 I found volt sag past 3.0v esc shut down running 100a constant current 10ah lipo at 8s.. https://youtu.be/jQcbA5fYCws.   By piggy backing 1.5ah 100c 8s paralleld to the high Mah pack solved the sag in heavy accel without adding much weight or used space..with  250a available delivery.   This was ok for short runs or heavy accel to speed as the voltage will eventually sag on the smaller mah. While cruising the voltage will equalize between the two paralleld packs like water finding it's own level..  it is better to have even mah packs paralleled to deliver amps necessary, but the capacitance pack works for short over amp situations..
```

---
