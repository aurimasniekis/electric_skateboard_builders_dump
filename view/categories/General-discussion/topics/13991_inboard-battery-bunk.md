# Inboard battery bunk

### Replies: 31 Views: 3387

## \#1 Posted by: Hummie Posted at: 2016-11-30T21:42:20.824Z Reads: 241

```
Someone below posted that inboard will be on shark tank on Friday and I went to their site to see what they're selling.   (I posted this in that thread but didn't get the response it deserve I think🤓). Their battery is 10 cells of li-ion. Ten total and 97 watt hours. 48 volts.  And they claim 1600 watts at the motor.  1600/48= roughly 32 amps.  Ten cells at a 32 amp draw each cell!!  What are the poor cells that will suffer extreme voltage sag before a quick death and possible fire!?!?  Is this a load of crap or am I right and this is a load of crap?!?
https://inboardtechnology.com/shop/powershift-battery
***edited.  They have different voltages stated.  36 and 48 and I did the math for the higher.  Thinking about it 10 cells isn't 48 and using the 36. ..1600/36 =roughly 43amps per cell being sucked.  Stunning.
```

---
## \#2 Posted by: Okami Posted at: 2016-11-30T23:30:07.586Z Reads: 222

```
well.. it just gets annoying.. I agree..

It is hard to understand whenever they are ignorant on purpose.. or just truly believe that most of the ppl know nothing about batteries and will buy their stuff in a hindsight.. believing all the power, range and speed stats are true and the board will truly perform as they advertise.. 

Yeah, quite disappointing.. unless they have invented a 50A capable battery.. I think the A123 systems battery (the 26' size) had even max rating of 70A or something.. but im pretty sure they are not using it.. just thought to throw the info I saw today about which I was amazed myself..

https://eu.nkon.nl/a123-systems-anr26650m1b-a-grade-3-3v-a-grade.html

high price and only about 2500mah..
```

---
## \#3 Posted by: NewbieBoardBuilder Posted at: 2016-12-01T04:11:26.277Z Reads: 197

```
https://inboardtechnology.com/blog/2016/11/21/inboard-on-shark-tank
```

---
## \#4 Posted by: Hummie Posted at: 2016-12-01T04:20:07.565Z Reads: 192

```
Nice cell. Low energy high power. If they used that then it would turn from crap to a really nice board
```

---
## \#5 Posted by: Pantologist Posted at: 2016-12-01T04:23:03.969Z Reads: 191

```
It's actually a 12S battery. That would be 43.2v nominal voltage.

http://m.imgur.com/a/nxxKZ?branch_used=true
```

---
## \#6 Posted by: Hummie Posted at: 2016-12-01T04:26:17.978Z Reads: 192

```
Aha they sneak two off the side.  That makes things a bit better but still it will be way over-discharging those cells or having to run very low power.  What are those cells?

Searching I find this has been done before:
http://www.electric-skateboard.builders/t/fake-12s1p-battery-on-the-inboard/9659/15

Still don't know the cells though
```

---
## \#7 Posted by: jmasta Posted at: 2016-12-01T04:39:20.731Z Reads: 186

```
The battery is 12S1P with LiMN battery chemistry.  The LG HE4 18650 cells are 20A continuous / 30A burst

What's interesting to me is their voltage cutoff is 2.5V.  But still the standard 3.7V nominal, 4.2V max


 > LG HE4 18650 2500mAh ( 4.1 W ) 3.7 V newest and most powerful battery for Mechanical Mods, RDA/RBA PVAs, and Sub-Ohm'er vapes. LG HE4 18650 2500mAh has excellent safety performance: overcharge, over-discharge, overload & over heat protection. High capacity, low inner resistance, long cycle life, low self-discharge. Strong current charge and discharge capability reached IEC standard
>  LG battery made with a safer chemistry LiMN and not require a protection circuit and also have a low risk of venting with flame or explosion.
```

---
## \#8 Posted by: saul Posted at: 2016-12-01T08:00:59.496Z Reads: 169

```
https://101vape.com/batteries/598-lg-he4-18650-35-amp-2500-mah-battery-pair.html

this one says 20A/35A so I guess they can get some power but I really don't think they will last for long.
```

---
## \#9 Posted by: Maxid Posted at: 2016-12-01T08:07:02.319Z Reads: 169

```
HE4 have been around for a looong time and are nothing special. Nobody in his right mind would use them in a 1P configuration. Also almost all Liion and Lipos have a low voltage cut off at 2.5V - that does not mean you should actually go that low. That is why everyone on this forum recommends to stay above like 3.2 or 3.3V to keep your cells happy, safe and healthy.
```

---
## \#10 Posted by: Okami Posted at: 2016-12-01T09:35:39.226Z Reads: 167

```
Anyways - is someone a vaper here? Does pulsed current mean peaking amps for 2-3 seconds or is it a longer time?

Anyways - if someone went uphill it probably wont be pulsed current anymore.. I assume 5-10 seconds or even more would be needed to reach the top of incline.. meanwhile these batteries will probably bake a bit and then sag hard and loose power.. at least that's the scenario I can imagine
```

---
## \#11 Posted by: jmasta Posted at: 2016-12-01T16:08:17.469Z Reads: 151

```
Someone asked what the cells were, and I looked them up. Don't shoot the messenger
```

---
## \#12 Posted by: Pantologist Posted at: 2016-12-01T16:37:31.075Z Reads: 139

```
If they programmed their BMS, it shouldn't allow for pulse discharge current levels for more than rated. Sometimes the pulse discharge is less than a second.
```

---
## \#13 Posted by: Maxid Posted at: 2016-12-01T16:42:51.615Z Reads: 138

```
Sorry - to me it sounded like you were impressed by those numbers since you found the low voltage cut off interesting (while it is nothing special).
```

---
## \#14 Posted by: FredSaberhagen Posted at: 2016-12-01T17:32:27.947Z Reads: 138

```
They would have to set the cutoff that low , because otherwise it would cut off every time you accelerate.  Look at battery test graphs, voltage droops like crazy once you start pulling 10, 15A.  You're not really getting more life by setting the voltage that low (voltage drops so fast past 3.3V)
```

---
## \#16 Posted by: saul Posted at: 2016-12-01T21:36:18.300Z Reads: 125

```
[quote="jmasta, post:15, topic:13991"]
5 mile real world range,
[/quote]

this is like a warm up. I take 2/3 5 miles rides per charge! lol
```

---
## \#17 Posted by: Okami Posted at: 2016-12-03T09:30:23.563Z Reads: 114

```
Some cool info to throw in (if they are really having HE4)

The one who made the test, says he did not discharge till 2.5v. 
> because I stop at 2.8 volt I will not get the full capacity. <

> **Source:** http://lygte-info.dk/review/batteries2012/LG%2018650%20HE4%202500mAh%20(Yellow)%20UK.html 

<img src="/uploads/db1493/original/3X/c/3/c31e16d2f8abdf37b2f7771208044ead3f0b5291.png" width="690" height="345">

So I assume they are correct to show 2.3ah or so
---
----

<img src="/uploads/db1493/original/3X/6/9/698ca3ff3712bb14e89c534dec518bc1dd569bd8.png" width="690" height="345">

<img src="/uploads/db1493/original/3X/b/7/b78251a8293b9ac062634c347186c2aedd9fe37f.png" width="690" height="345">

Perhaps someone can calculate what distance at what amps one person might travel... (by taking numbers from the chart)
---
---

Though, If im correct, it looks like 12 cells would get 96 wh or so.. (airplane limit).. and if you travel at **10wh/km**, you would get around **9.6km** (probably less), which in theory would be around **6miles**. Real world usage - test would be great.. that's probably why everyone focuses on just promotion videos and not real footage on the actual distance driven :D

And this one does not include speed and acceleration.

---
Stats from their page:
> Technical Specs:

> Range: 7-10 miles
> Capacity: 97Wh  2.25Ah
> Charge time: 90 minutes
> Type: Lithium-Ion 
> Weight: 1.8 pounds (.84kg)
> Voltage: 43.2v nominal / 49.2v peak

Board stats:
> Top Speed: 24 mph 
> Power: 1000 watts continuous, 1600 watts max
> Board Weight: 14.5 lbs (6.57kg)
> Max Rider Capacity: Tested to 250lbs 
> Wheels: 79mm
> Deck Flex: Stiff - designed for speed and stability
```

---
## \#18 Posted by: Okami Posted at: 2016-12-03T09:45:43.887Z Reads: 104

```
Sorry for double reply but the post got too long.

So, my further theoretical calculation are:

At **1000w and 46.2v** = amp draw seems to be **21.65 (A)**
46.2v is the average i took between nominal and peak.

For nominal it would take around 23A to reach the same power output.

---

Looks like they have just taken the written numbers as it usually is. I wonder can you reach 24mph easy with just 20A of power for such system.. still looks like it would stress heavily everything.. not to mention keeping such load for a prolonged time :) probably 10-15mph is more realistic and the cells would stay in 10A range or so.
```

---
## \#19 Posted by: Hummie Posted at: 2016-12-03T18:47:45.924Z Reads: 96

```
When they have a peak AND a continuous rating what does that mean in practice?  Does the controller reel back the power to continuous after a couple of seconds at peak or something?  Or are they just following the typical motor stats statements, which since there's no standardization of either the testing doesn't mean anything anyway?
96 watthours is what that pack would give with a 1amp draw maybe.  Under load I didn't do the exact math but it looks to be maybe a 1/5 less energy if it's doing 20amps continuously and netting 1000 watts total roughly.  1000 watts is what I end up around when I break a canbus and end up running only a single motor. Very lame.
```

---
## \#20 Posted by: Okami Posted at: 2016-12-03T18:57:07.062Z Reads: 93

```
Im waiting till the ''shark tank's'' episode comes out.. will be interesting to find what these guys have to tell about electric skateboards in general.. as of few hours back only a promo was available.. im not sure at what time the episode comes out.. but they do come out on fridays and it said 2nd dec..
```

---
## \#21 Posted by: Hummie Posted at: 2016-12-03T19:12:16.309Z Reads: 85

```
The shark guys will eat up the numbers not knowing the realities of the battery's limits I bet.  They'll ask seriously about the risk of fires and I bet inboard will have some satisfactory answer for the unknowing and that fear will be washed away...but really maybe it shouldn't be.  I wonder what the battey cell manufacturer would say.
  Wonder why they switched from lipo.
When's the show I don't understand your post?
```

---
## \#22 Posted by: jmasta Posted at: 2016-12-03T19:14:56.611Z Reads: 83

```
It's out now. You can watch it online if you login with a TV provider.  Looks like you have to wait a week if not

http://abc.go.com/shows/shark-tank/episode-guide/season-08/10-episode-10
```

---
## \#23 Posted by: Okami Posted at: 2016-12-03T19:28:44.862Z Reads: 88

```
Thanks. Will have to wait a week then. Not from usa myself unfortunately :D unless I find somewhere online

[quote="Hummie, post:21, topic:13991"]
I wonder what the battey cell manufacturer would say.
[/quote]

I watched one of their earlier videos.. where some kind of tech channel was reviewing their board and they said they are in (at that time) in the process with the manufacturers who make the 'quality samsung batteries'.. So it seems they probably switched to something else or samsung also makes LG or they just called that name to sound better.. I bet the manufacturer does not care what they order and as everything is made by request..

----
```

---
## \#24 Posted by: Pantologist Posted at: 2016-12-03T19:33:01.852Z Reads: 88

```
*cough* @Hummie @jmasta @Okami *cough*

https://youtu.be/VXp_JpA33OY
```

---
## \#25 Posted by: Okami Posted at: 2016-12-03T19:41:16.211Z Reads: 90

```
Thanks, was willing to post a video from one of these stream sites but it was crapy.. loads of ads.. 

Thanks for finding one on youtube!

--

https://youtu.be/VXp_JpA33OY?t=3m18s

Im sure many will find this part.. Intriguing
>**Shark:** Im pretty sure there are many other eskateboards out there.. why is yours unique?
> **They:** ''Well, because we created the **first ever** inwheel motor..'' :D

I assume they only compare visible side of what's available in usa.. evolve and boosted :D perhaps including yuneec e-go
```

---
## \#26 Posted by: Hummie Posted at: 2016-12-03T20:23:42.703Z Reads: 84

```
Why are they even looking for money since they made so much from Kickstarter?  
The extent of any questioning related to power was "can it go up hills?"  
"Yes"
```

---
## \#27 Posted by: Pantologist Posted at: 2016-12-03T21:00:19.799Z Reads: 82

```
Yea seriously. How much money do they need before they'll really touched base with the industry? They haven't even fulfilled their current orders yet. Why not wait till they have more to show for?

Hopefully the few boards they've shipped out have little to no issues. Just scares me on how stressed the battery will be even in normal situations. They will be sending out replacement batteries within their warranty period as far as I can tell. They won't even be able to change the battery technology much without redesigning the board housing.
```

---
## \#28 Posted by: SirDiff Posted at: 2016-12-03T21:01:59.181Z Reads: 82

```
I think that's not about money, that's visibility. And I don't think any of those businessmen know how many amperes would a double hub setup drain, so there was no point asking that
```

---
## \#29 Posted by: Okami Posted at: 2016-12-03T21:11:29.489Z Reads: 84

```
yeah, some already said it was just for exposure.. though i kind of hate it that they still got the offer / money.. with that kind of f.. money they can probably launch 2-3 other boards by now.. 

Argh.. marketing and convincing at play here.. 

yeh, the deal with asking more money while the seemingly first batch has not shipped yet.. is kind of sketchy

---
[quote="Hummie, post:26, topic:13991"]
The extent of any questioning related to power was "can it go up hills?""Yes"
[/quote]

@Hummie well.. they answered what was asked.. no questions about the % of incline.. though, very fast paced conversion.. and that numbers game also seemed stressed at the end..
```

---
## \#31 Posted by: Hummie Posted at: 2016-12-03T21:25:59.162Z Reads: 83

```
As evohyax was mentioning in the raptor thread the limitation on all these board's power, the real bottleneck, is the li-ion cells.  All the esc must be set tragically low power.  I still don't understand what power they are really putting out and if it does possibly change from the peak 1500 to 1000 continuous, as in this stated specs with inboard @mellowboard.  Especially with hub motors
```

---
## \#32 Posted by: Pantologist Posted at: 2016-12-03T21:31:16.868Z Reads: 84

```
Their failure to realize their battery bottleneck might have something to do with their electrical engineers going to UCSC and SJSU. Not the greatest engineering schools. Meanwhile, Boosted hires people from Tesla and Stanford.
```

---
## \#33 Posted by: Hummie Posted at: 2016-12-03T21:34:17.949Z Reads: 80

```
But even hobbyists such as us can figure this out. They know what they're doing for sure.  They're sales people taking advantage of the large majority of buyers not having a clue
```

---
