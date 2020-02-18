# I want to charge 12S from my van will this work?

### Replies: 24 Views: 605

## \#1 Posted by: amazingdave Posted at: 2018-09-11T13:40:31.986Z Reads: 152

```
I’m looking at this boost converter on eBay to charge my 12s with bms from my van (my van has 300Ah of battery so I’ve got plenty of juice)

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F252510173758

May well use the same converter as a range extender as per this thread...

https://www.electric-skateboard.builders/t/range-extender-plugged-into-loopkey/64327

Can anyone see a problem?
```

---
## \#2 Posted by: Octave Posted at: 2018-09-11T14:20:43.510Z Reads: 134

```
Yea sounds fine. Just triple check the voltage settings on the boost converter. Sound like a great idea, good luck :slight_smile:
```

---
## \#3 Posted by: TinnieSinker Posted at: 2018-09-11T14:49:59.888Z Reads: 121

```
is your van battery the regular single 12v lead acid? if so, you wont get enough amps out of it after the boost. the bigger the difference in voltage the less amps you get out.

for 12s you would want 24v minimum, from memory i think that gives you around 4-5amps. efficiency was not great but that shouldn't be a problem

I have two small 15ah 12v deep cycle batteries on the charge now. hoping to put them in the ute, charging off the main battery in parallel with another circuit in series to power the boost converter.... whether or not this'll work though, i dunno ..:grin:
```

---
## \#4 Posted by: amazingdave Posted at: 2018-09-11T15:32:28.974Z Reads: 107

```
My van has 220Ah of AGM deep cycle... I can charge 2 x 6s 10000mAh drone batteries simultaneously at 10A each using 2 hobby chargers so I think I’m good for amps!

So I’d have to parallel ✖️  (Series) ✔️my van batteries to get the volts?
```

---
## \#5 Posted by: TinnieSinker Posted at: 2018-09-12T02:57:04.631Z Reads: 86

```
yea that sounds right. 12v up to 24v is fine, only 12v step up. however, 12v up to 48v is 36v difference.

I think it depends on the boost converters maximum input amps. the one i have has 15a input max and i found a huge difference between boosting 24v to 36v and 15v to 36v. with 24v i could get up to 10a output but with 15v i could only get 1.5a output.

looking at boost converters this morning i found this one with 30a input, which might be enough to charge 12s off 12v ... emphasis on 'might' :grin:

https://www.banggood.com/DC10-60V-30A-1500W-To-12-90V-Boost-Converter-Step-Up-Power-Supply-Module-p-1076169.html?rmmds=search&cur_warehouse=CN

and yea that would be series connection to multiply the volts of your car battery. parallel multiplies the capacity.
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-09-12T04:36:05.758Z Reads: 68

```
[quote="amazingdave, post:1, topic:67711"]
May well use the same converter as a range extender as per this thread…
[/quote]

How exactly can that converter be used as a range extender? I'm missing something here. Do you plan on having an external loop key battery to bump up to 12S?
```

---
## \#7 Posted by: amazingdave Posted at: 2018-09-12T08:15:05.508Z Reads: 62

```
The loop key boost was the initial idea. If you look towards the end of the linked thread the discussion turned to using boost converters to act as range extenders with good results. Which seems much more straightforward.
```

---
## \#8 Posted by: amazingdave Posted at: 2018-09-12T08:16:14.833Z Reads: 61

```
@TinnieSinker  Sorry, brain fart on series/parallel! Typing faster than my brain speed!
```

---
## \#9 Posted by: TowerCrisis Posted at: 2018-09-12T12:21:13.041Z Reads: 48

```
Yeah this is a pretty bad idea. I wouldn't advise this AT ALL.

Charging the evolve was easy enough because it went through different charge circuitry to limit output current.

If you just slap on a DC-DC converted in parallel to your main pack here's what will happen.

The buck converter and the main battery will share the load. So if you pull 40 amps overall, you'll pull 20 from the main battery and 20 from the buck converted.

But the buck converter is stepping up the voltage 5X, so the tiny battery behind it will have to be supplying 100 amps! That's incredibly dangerous to pull that constantly or for an extended time.

His went through a BMS charger (i believe) which limits the charging current.

But even so, that's not good. You will be able to over discharge the small pack because it has no protection. It could run out without you knowing and the buck converter is gonna pull more and more juice out of it till it puffs.

It's just not a good idea.


Adding an additional 2S in series seems to be the best method for what you want. You just need to make sure that the add-on pack starts at the same voltage as your main battery, and that it's made of the same cells.
```

---
## \#10 Posted by: amazingdave Posted at: 2018-09-12T13:20:20.313Z Reads: 41

```
Ok I see your point... maybe this reply should be to the other thread though?!
```

---
## \#11 Posted by: mikenyc Posted at: 2018-09-12T13:30:01.018Z Reads: 40

```
does having the van running make any difference?
```

---
## \#12 Posted by: TowerCrisis Posted at: 2018-09-12T13:39:45.373Z Reads: 38

```
The method I'm describing in that post is for when the board is active. It's using a smaller battery ON the skateboard. This is not for recharging in a car.
```

---
## \#13 Posted by: amazingdave Posted at: 2018-09-12T13:50:00.193Z Reads: 34

```
@moderators could the comment on the range extender be moved to that discussion to avoid confusion?
```

---
## \#14 Posted by: mikenyc Posted at: 2018-09-12T13:51:39.157Z Reads: 30

```
lol. yes, that was quite confusing
```

---
## \#15 Posted by: TinnieSinker Posted at: 2018-09-12T13:55:35.708Z Reads: 25

```
@amazingdave haha oh good, i felt weird explaining that :flushed::grin:
```

---
## \#16 Posted by: TinnieSinker Posted at: 2018-09-12T14:00:57.297Z Reads: 26

```
so there's this dedicated thread started about boost converters and such now, not much in it yet but looks like where all the new info will go.

https://www.electric-skateboard.builders/t/step-up-booster-lipo-as-external-charger/67070
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-09-12T14:12:44.549Z Reads: 26

```
[quote="amazingdave, post:1, topic:67711"]
May well use the same converter as a range extender as per this thread…
[/quote]

[quote="amazingdave, post:1, topic:67711"]
Can anyone see a problem?
[/quote]

Look man you're the one who in this thread specifically asked about this and if it's a good idea, and I clearly explained how that works and why you shouldn't do it. I don't think anything's out of place.
```

---
## \#18 Posted by: amazingdave Posted at: 2018-09-12T14:36:15.515Z Reads: 23

```
Oh well I guess I’ll agree to disagree.
```

---
## \#19 Posted by: AlexBE Posted at: 2018-09-12T23:37:57.777Z Reads: 21

```
Yes using that boost converter will work just fine as it has an adjustable current limit and voltage. I would be careful with the voltage though, its probably worse than 1% accurate, so set it a little lower than you need and check with a multimeter.

Note that the converter has a maximum input current of 15A, so at 12V you are limited to 180W, ie 12s charging at ~3.5A. Still decent.
```

---
## \#20 Posted by: AlexBE Posted at: 2018-09-12T23:44:04.600Z Reads: 18

```
@TowerCrisis, the thing you are missing is that this kind of boost converter DOES contain a current limit. So you could set it to 2A output to use it as a range extender. Similarly, you can set an undervoltage limit on the input side to protect your secondary pack (or use a BMS on that pack). A guy i know does exactly this with a backpack full of batteries and a cable running down his leg and plugging into his onewheel.
```

---
## \#21 Posted by: TinnieSinker Posted at: 2018-09-18T00:47:13.744Z Reads: 15

```
Just remembered a thing, I read that you can run two boosters in parallel to increase the output. This might give you a decent charge off the one 12v car battery
```

---
## \#22 Posted by: b264 Posted at: 2018-09-18T01:04:23.213Z Reads: 13

```
If you want to charge from your van, get [an inverter that makes 120VAC from your van](https://www.ebay.com/itm/BESTEK-12V-DC-to-110V-AC-Car-300W-Power-Inverter-USB-Outlets-Auto-Truck-Adapter/201694686167) then use the same charger you use at your house, plugged into that.  Otherwise this sounds like a big fire hazard
```

---
## \#23 Posted by: TowerCrisis Posted at: 2018-09-18T01:06:45.485Z Reads: 13

```
You can also definitely get a cheapo one that's low wattage, you won't be needing to pump 300 watts into your battery hopefully 😅
```

---
## \#24 Posted by: b264 Posted at: 2018-09-18T01:19:03.209Z Reads: 13

```
I did a quick back-of-the-envelope calculation that 4A*50V ~ 200W and then suggested a 300W one that will almost certainly work.

If you did more work you could probably get by with a cheaper one, but the bigger one will be better anyway and probably last longer.  It's also not every expensive.

Besides, you may want to charge a cell phone and run something else while charging your board...
```

---
