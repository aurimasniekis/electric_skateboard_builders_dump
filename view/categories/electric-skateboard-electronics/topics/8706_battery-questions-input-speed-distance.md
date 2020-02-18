# Battery Questions / Input (speed, distance)

### Replies: 7 Views: 958

## \#1 Posted by: jak Posted at: 2016-08-31T15:59:11.378Z Reads: 85

```
Here are some calculations i made. Would someone more knowledgeable than i review? Did i do this correct? The size motor does not effect distance? is this because you will get same distance but at different speeds? seems like a different motor couldbe less or more efficient, but i guess that is what the weighted section is for.

i used this formula for distance and the superblog esk8 calc for speed.

<img src="/uploads/db1493/original/2X/f/fc4c72bd928d0290b79dc7f2468e855e07ef510a.png" width="393" height="500">

r spec @6s
<img src="/uploads/db1493/original/2X/3/3da0faa90285be9355b0c31e35d6acd3e792494b.png" width="314" height="460">

r spec @8s
<img src="/uploads/db1493/original/2X/e/e4a56755b420e4d19b0c59171377d91f385a6b3a.png" width="308" height="456">

Sk3 @ 6s
<img src="/uploads/db1493/original/2X/7/7e3773350b7e61894e8a40e5c48f56e6382fcbee.png" width="328" height="456">

Sk3 @8s
<img src="/uploads/db1493/original/2X/4/4d830327ea2154f506f8b66941308fd198553f29.png" width="349" height="458">

If these Calculations are correct i will be leaning to the 8s. Im just trying to narrow down some more parts so i can get things ordered. 

I also Found these batteries. Im looking to run 4 of them. 2 in parallel and then in series to give me 8s@10Ah they have a continuous 25C rating with a peak at 35C (10 secs)
<img src="/uploads/db1493/original/2X/3/33a939d3ede32d4c2cd4918ad5908d737ffa0fb3.png" width="516" height="445">

If someone could give this the old once over. If i go to 8s i will need to get a new charger since the imaxb6 will not work. I checked the commonly used parts thread and there are not chargers listed. Any standby 8s chargers? in the meantime i will be on hobbyking. Thanks for any input and info.
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-08-31T17:15:59.363Z Reads: 63

```
[quote="jak, post:1, topic:8706"]
If i go to 8s i will need to get a new charger
[/quote]

You Could still discharge in series and charge in parrallel.
```

---
## \#3 Posted by: sl33py Posted at: 2016-08-31T17:24:59.677Z Reads: 60

```
The grey quote above looks familiar...  hehehe.

Yep your calculations look correct.  A good example of the better efficiency you get with higher voltage.  8Ah vs 10Ah and realistically the 1km difference will be negligible.  

I too would discharge in series, but charge in parallel - so your charger should work fine.  But you'll need to at least disconnect to charge.  Or go with BMS if you wan in-board charging.  I don't mind the extra step as it also lets me inspect my lipos and keep an eye on them when charging (vs in board).  In pyrex container etc.
```

---
## \#4 Posted by: jak Posted at: 2016-08-31T17:31:16.189Z Reads: 70

```
alright good info! Keep it coming. i don't mind taking them out to charge as well. it is only one more step and i plan on putting them in an easily accessible container. also if something should happen while charging the whole board doesn't wind up in flames. ;] will this take forever to charge them this way? it isn't a huge deal as it will be for after work cruises, just trying to get my ducks in a row. not crap i have no battery let me charge at the office.
```

---
## \#5 Posted by: sl33py Posted at: 2016-08-31T18:20:07.585Z Reads: 65

```
charging - that's another whole can of worms.  Or down the rabbit hole or something...

Your charging is going to depend on a couple key things.  

1 - pack life vs quick charge.  Your battery will have a charging "c" rating.  Just like the discharge rating of the battery - it lets you know max charging amps.  

2 - more complex setup with AC-DC PSU and you'll need a Parallel balance board to utilize the need for more amps.

Let's look at the specs for the Turnigy battery:
[img]http://goo.gl/BZuTF4[/img]
So 2 C max charge rate.  2x5Ah (5000mAh) = 10 Amps max charge rate!  That's quite a bit and will give you a fast charge.  Like if you get home from work, want to charge and get out the door to ride before sunset!  

BUT - nothing's free.  Higher amp charging and discharging decreases pack life.  Usually decreasing the # or re-charges it will do before IR (internal resistance) or a cell will go (discharge before the rest) - which leads to puffing and all sorts of bad things (why i look at my packs before charging).

So to extend battery life, you usually want to do a lower C charge - like .25 C or .5 C - so on this turnigy 1.25A or 2.5A respectively.  You can also charge just below "full" 4.2v per cell which extends life further - but decreases range.

Back onto chargers - if you have a b6acv2 charger (a budget charger i usually recommend) - it maxes at 5A charge rate - across all batteries you are charging.  So 2 batteries would be getting 2.5A ea.  That's good for pack life, but going to be slow sometimes when you want to ride NOW!

A better charger like an iCharger (206/306 etc) can charge at 20-30A respectively (the first two numbers of the model is amps, the last number is # in series it supports).  So the 206 could charge two of the Turnigy's at 10A each for 20A total - FAST!  or a slow .25 C charge for better battery life.  A great option.  

The downside of most chargers like this (iCharger or similar) is that they require DC voltage.  So a separate AC-DC power supply is needed.  You can get several really nice variable ones online, or do what i did and get a Dell Server (or other brand HP/Lenovo/etc.) power supply and modify (or buy already modified) to switch on and supply a huge 12v power source.  I have two 750w in series for 1500w 24v to supply my iCharger 306b and Hobbypartz Thunder 1220.

A setup like this as an example of AC-DC PSU -> 8s Lipo charger:
[img]http://www.hobbyking.com/hobbyking/store/catalog/81837-3.jpg[/img]

And in order to need 20A+ you'll need to connect enough batteries in parallel to utilize (also convenient and decreases swap and charge time) the full potential of a setup like this.  The best ones i've found (will depend on which connector you utilize on your packs) is [BuddyRC's paraboard](http://www.buddyrc.com/power-system/paraboard-parallel-charge-board.html):
[img]http://www.buddyrc.com/media/catalog/product/cache/1/image/700x/9df78eab33525d08d6e5fb8d27136e95/p/a/paraboard_v2_xh_xt60.jpg[/img]

Nicer chargers typically also have a temp probe you can utilize.  with an elastic band they sit against the pack while charging and will auto-shut down the charge if the temp of the pack spikes while charging.  Heat almost always happens before a catastrophic failure on Lipo.  So an inexpensive failsafe (usually a few bucks for the temp probe if not included).

Told you it's a rabbit hole discussion and a ton of info to digest.  Hope it's not too long winded and makes sense.  let me know any questions i can explain or help further.

GL!
```

---
## \#6 Posted by: jak Posted at: 2016-08-31T19:29:46.756Z Reads: 43

```
that is quite alright, never too much info. Besides i am already in the rabbit hole just have to find my way out. i might research the modded psu solution as i build computers from time to time and have a few spares laying around. I appreciate all the info and will attempt to digest it all. :joy:
```

---
## \#7 Posted by: sl33py Posted at: 2016-08-31T19:39:53.061Z Reads: 43

```
Alrighty then - more info for you to research:

Great forum thread w/ TONS of info:
http://www.rcgroups.com/forums/showthread.php?t=1292514

Also can check out this guy's tutorial/steps:
http://www.tjinguytech.com/my-projects/server-ps

I was going to do this with some server power supplies from work... then found these on ebay for cheap already modified for 24v series.  Did a quick search and don't see that seller right now, but here's a cheap dell PSU - i'd check on rcgroups if the modification steps are listed!  If so, <$20 you have a 750w 62A 12v PSU!!!

http://www.ebay.com/itm/Dell-PowerEdge-2950-2970-Server-750W-Redundant-Power-Supply-PSU-Z750P-00-JX399-/111767582257

be very cautious of series for 24v:
http://www.rcgroups.com/forums/showthread.php?t=1799197
Some steps to help understand if you go this route.
```

---
