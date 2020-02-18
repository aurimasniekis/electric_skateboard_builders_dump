# What you think of this charging method

### Replies: 36 Views: 746

## \#1 Posted by: Hummie Posted at: 2018-08-11T04:08:52.014Z Reads: 158

```
im thinking of buying 12 of these chargers and then connecting them to the balance leads on a 12s battery.  this would be the only charging method used.  can balance charge with a single plug using off-board electronics.
just would need to find an ideal 13 prong plug.
https://www.aliexpress.com/item/1s-4-2V-10A-Polymer-Lithium-Li-ion-LiPo-AC-DC-fast-Charger-power-supply-for/32887585458.html?spm=2114.search0104.3.211.6a2622c4Kxkt2A&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10344_10130_10068_10324_10342_10547_10325_10343_10546_10340_10548_10341_5012013_315_10545_10696_10084_531_10083_10618_10307_5011913_10059_100031_10103_10624_10623_10622_10621_10620,searchweb201603_51,ppcSwitch_7&algo_expid=845ca624-db17-4027-8271-71dee46f6945-33&algo_pvid=845ca624-db17-4027-8271-71dee46f6945&priceBeautifyAB=0

it's 300$ but seems reasonable for what it would do.  id probably take the cases apart and mount the innards all inside a heatsink/box.
```

---
## \#2 Posted by: Blasto Posted at: 2018-08-11T04:18:51.689Z Reads: 154

```
Pass the blunt
```

---
## \#3 Posted by: deucesdown Posted at: 2018-08-11T04:19:06.842Z Reads: 150

```
Probably a show stopper, the dc ground is probably tied to ac ground so you'd have a bunch of shorts. Must have floating grounds.
```

---
## \#4 Posted by: Hummie Posted at: 2018-08-11T04:20:41.799Z Reads: 141

```
haha.   

so no it wouldnt work, bummer.  I need to find a supply with a floating ground?  you think they're out there.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2018-08-11T04:22:41.173Z Reads: 135

```
Puff puff pass @longhairedboy
```

---
## \#6 Posted by: deucesdown Posted at: 2018-08-11T04:22:51.998Z Reads: 122

```
Also

https://www.electric-skateboard.builders/t/diy-10s-cell-balancer/20767
```

---
## \#7 Posted by: Blasto Posted at: 2018-08-11T04:23:26.818Z Reads: 108

```
Could work, a bit impractical. What @deucesdown mentioned is a good point, but i believe the earth ground is floating.

Small balance leads can’t handle the current, max 1A... that’s pushing it
```

---
## \#8 Posted by: Hummie Posted at: 2018-08-11T04:25:45.550Z Reads: 107

```
great to hear.  nice to have you guys here telling me whats what.   but i think its very practical.  simplified.  

Id add the balance leads.  what gauge you think would be ok?
```

---
## \#9 Posted by: TowerCrisis Posted at: 2018-08-11T04:35:45.381Z Reads: 107

```
What you're better off doing is using one larger charger in conjunction, like a 3A 12S charger, and connect that to the main leads.

Then use your tiny chargers once the pack overall reaches ~90% capacity. That'll just be a small current balance.

You could have some sort of zener diode hooked up to the main battery positive and use that to switch a relay or something to switch between the large and the small chargers once the pack reaches a certain point.

But honestly at this point I'm describing a dumbed down balance charger with way less safety features.

Just get a 12S charger and use an external BMS and plug the balance leads into it.

Better yet, just stick a balance board up to the balance leads and keep it inside your board. They're super tiny and thin, very cheap, and has zero of the failiure risks of using a BMS for discharge. Using this method you could just have one DC jack to charge with, IMO a much more aesthetically pleasing and useful method.
```

---
## \#10 Posted by: deucesdown Posted at: 2018-08-11T04:36:57.663Z Reads: 97

```
[quote="Blasto, post:7, topic:64516"]
Small balance leads can’t handle the current, max 1A… that’s pushing it
[/quote]

I think a lot of builds use 22awg and that should handle (but not happily 10a). 3a should be safe -- revolectrix powerlab will do balance lead only charging at max 3a, and they're very conservative.

@hummie if you push a bunch of amps through skinny wires there will be big voltage drop. Might not matter since the current decreases in the cv stage so voltage drop should lessen.
```

---
## \#11 Posted by: Eboosted Posted at: 2018-08-11T04:39:10.498Z Reads: 87

```
Even better than that, I'd suggest you get a voltmeter for each pack and balance charging/discharging only the one that drifts through the balance leads. Cheaper and more efficient
```

---
## \#12 Posted by: skatardude10 Posted at: 2018-08-11T04:43:28.493Z Reads: 84

```
Sorry to sound dumb. Not an electrician. But when people say they beleive the Earth's ground is floating and talking about passing blunts... I get the inkling that something is funny.

But I know it's just you guys talking electricity.
```

---
## \#13 Posted by: deucesdown Posted at: 2018-08-11T04:44:46.252Z Reads: 82

```
[quote="Hummie, post:8, topic:64516"]
gauge you think would be ok?
[/quote]

Technically I think you'd be okay if you match the dc wire on the charger -- not much point going heavier. Unless it's a crap danger charger lol.

Hummie I love your wacky threads lol
```

---
## \#14 Posted by: mynamesmatt Posted at: 2018-08-11T04:48:36.332Z Reads: 76

```
wouldn't you need a 24 prong connector as you need the positive and negative of each cell?
```

---
## \#15 Posted by: Hummie Posted at: 2018-08-11T04:49:00.786Z Reads: 76

```
thanks for all the alternative suggestions but im still stuck on my original plan if it will work.  it seems easiest to me compared to the others, with one plug and done, and the big perk is charging at 10amps which other methods with other added electronics wont allow.   

so throw me a stong "no!" if it's not going to work because otherwise im still into it.

think could use 13 prong and pair up the cells on one wire but maybe not.
```

---
## \#16 Posted by: mynamesmatt Posted at: 2018-08-11T04:51:09.620Z Reads: 74

```
what capacity are your cells?
```

---
## \#17 Posted by: Hummie Posted at: 2018-08-11T04:51:39.993Z Reads: 75

```
12s4p   30Q.   at 4 amps a cell max charge rate this should be fine.
```

---
## \#18 Posted by: mynamesmatt Posted at: 2018-08-11T04:52:52.862Z Reads: 73

```
sooo how are you planning on charging at 10a?
```

---
## \#19 Posted by: Hummie Posted at: 2018-08-11T04:53:14.789Z Reads: 73

```
the chargers do 10a.  look above.   i charge at 10a now but with just a bulk charger, so moving up in the electronics and safety world possibly.   throw me your "no!" now so i dont think too much about it as im about to go to bed!   east coast
```

---
## \#20 Posted by: mynamesmatt Posted at: 2018-08-11T04:54:56.558Z Reads: 79

```
yes but if your cells only take 4a charge max it'll cook your cells real quick
```

---
## \#21 Posted by: TowerCrisis Posted at: 2018-08-11T04:55:16.688Z Reads: 68

```
I'm going to give you a solid "no!" on this one. You're wasting money and adding tons of complexity.

Use a charger like this: https://www.aliexpress.com/item/Global-Certification-50-4V10A-Charger-44-4V-Li-ion-Battery-Smart-Charger-Used-for-12S-44/32822262578.html

And a tiny resistor board like this: https://www.ebay.com/itm/263384603242

The resistor board I linked isnt for 12S but they do make them for 12S. I'll try and fine one. Dirt cheap

And there you have it, 10A charging with passive balancing for a FRACTION of the price and far simpler. It's so small you could even leave that tiny board inside your battery pack. But it will also work just as well outside as an external device. I highly recommend just sticking it inside your board, it will ensure the cells are always balanced.
```

---
## \#22 Posted by: Hummie Posted at: 2018-08-11T04:55:26.038Z Reads: 65

```
with 4 in parallel can do 16a and be within manu specs
```

---
## \#23 Posted by: deucesdown Posted at: 2018-08-11T04:55:37.235Z Reads: 66

```
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F371912572891

It comes in 2 sizes. There are plastic versions too.

4.2v x 10a = 42w, times 12 is 500w. You're better off with the big bulk chargers, and balance charging once a month.
```

---
## \#24 Posted by: Hummie Posted at: 2018-08-11T04:57:03.812Z Reads: 65

```
i have a bunch of those resistor boards already.  the last plan.  maybe will revisit it and read your post a couple more times later.   
thanks guys ...night!
```

---
## \#25 Posted by: ksfacinelli Posted at: 2018-08-11T04:57:41.121Z Reads: 65

```
I have a built in resistor board on my 10s4p pack just as @TowerCrisis is suggesting
```

---
## \#26 Posted by: mynamesmatt Posted at: 2018-08-11T04:57:47.282Z Reads: 64

```
aha i gotcha, why not just a cheap  ebay bms for charge only? 😂
```

---
## \#27 Posted by: TowerCrisis Posted at: 2018-08-11T05:01:11.338Z Reads: 63

```
@mynamesmatt 

He wants 10A charging, and most cheap bms's won't allow for that. You'd probably need a programmable BMS or one you can special order with specific settings.
```

---
## \#28 Posted by: Blasto Posted at: 2018-08-11T05:11:39.928Z Reads: 59

```
[quote="Hummie, post:15, topic:64516"]
so throw me a stong “no!” if it’s not going to work because otherwise im still into it.
[/quote]

Lol, you’ve been told no in the past

https://www.electric-skateboard.builders/t/anyone-got-xt60-plugs-in-the-bay-area/48316/10?u=blasto

So pass the blunt and lets see what gives
```

---
## \#29 Posted by: Wraith Posted at: 2018-08-11T05:53:08.817Z Reads: 53

```
Why don’t alot of people do it this way instead of picking up a pricey bms?

Interested to see the 12s model too
```

---
## \#30 Posted by: mynamesmatt Posted at: 2018-08-11T05:59:38.320Z Reads: 60

```
![Screenshot_20180811-155808_eBay|243x500](upload://k2OFhaDmLUPpwmg8Oy2ROXlmSJ9.jpg)
this is 45a charge and discharge?
```

---
## \#31 Posted by: Wraith Posted at: 2018-08-11T06:06:33.510Z Reads: 75

```
Do you plan on putting this on the board or use as an external balancer?
```

---
## \#32 Posted by: TowerCrisis Posted at: 2018-08-11T08:02:59.491Z Reads: 68

```
**BMS vs Balance Board**

There's a few inherent disadvantages of using a bare board instead of a BMS or charging BMS.

Whatever charging port you add will be connected directly to the battery pack with no buffer in-between. Most BMS's have protection on their charging ports and don't allow significant current to flow in reverse, incase something has shorted out the charging port. So you'll likely need to put a small fuse on your charging port for protection.

You don't have any over voltage protection So if your charger goes haywire and for whatever reason gives too much voltage, or god forbid, you use the wrong charger :grimacing: then you have no protection and you could damage or end up venting your battery.

You also don't have cell level protection, although I guess this only applies to BMS's used for discharge. If I accidentally leave my board on and it bleeds power for a week, the BMS will cut power once any of the cells reaches 3V. That's useful if you want to save some cells and labor incase of accidental mistakes.

Over current protection is also a benefit from a BMS. If  for whatever reason your motor or main battery leads short out, and it pulls significantly more than 60A in my case, then the BMS will cut power. I think that's a safety feature that all builders should consider, it's good fire protection.

But with BMS you also risk not being able to brake on a full battery, because it will prevent cells from getting overcharged. This also only applies to a BMS that also discharges.

Overall there are many pros and cons to both scenarios that one should consider.

**Setups I recommend**
 
In my opinion these are some necessary precautions to take.
Here's one setup:
-RC tweeter that will alert you upoun lowor high voltage (left on too long or overcharging batteries on braking)
-Large fuse immediately after the base of the battery positive terminal, isolate all bare unprotected positive contacts
-Small fuse inline with charging port
-Balance board to keep cells in sync

Another option:
-Use a BMS for charging only
-large fuse on positive lead
-small fuse on charger port
-RC tweeter to alert high and low voltage.

One more:
-Use a BMS for charge and discharge
-Dont charge to full capacity but reach balance voltage of the BMS.

**What I DONT recommend is this:**

-Using a bare battery with no fusing or BMS.
Or
-Having balance leads exposed outside of the case for easy balance charging. (Unless you have every wire fused.) You really don't want your balance wires to become the fuse when the port gets shorted somehow.
Or
-Having no way to balance your cells :skull_and_crossbones:
Or
-Using a BMS for discharge, unless you have a separate way to bleed voltage spikes over your max battery voltage from braking hard.
Or
-Not properly recognizing the inherent and minimizeable risks we take by using high capacity, voltage, and density batteries.

**In response to this threads initial proposal**

There are some methods that are safe and some that aren't. Using a balance charger intended to charge a pack is safe. Using a balance board is safe. Using a BMS is safe.

What is not safe is strapping 12 chargers together and expecting them to function properly while their outputs are all connected in series. There's too many risks in my opinion. One of the chargers could stop working and that would likely end very badly. You could of course really engineer these things and ensure they all work right.

But then again, if this thing's really redesigned from the ground up you've effectively created a very expensive unproven balance charger for significantly more time and money.

The much better method is to have an external BMS connected to a 12S 10A charger, or to buy an actual 10A balance charger. I haven't even gotten into the risks of charging at 10A, I wouldn't use that on anything under 10Ah less you risk degraded battery lifetime.

This whole debacle is only to squeeze out a little less charge time. Sure, you can now charge your pack in an hour. But to me that isn't any more useful than charging it in 2 or 3, because at that point after waiting an hour there's no need or immediate urgency to use your board that could have waited that long.

TL;DR

Use stuff the way it's intended and add adequate protection the way actual companies do to protect their users. Spend more (or in this case actually less) to be as safe as you can be.
```

---
## \#33 Posted by: Wraith Posted at: 2018-08-11T08:39:55.426Z Reads: 52

```
Thanks! I appreciate the detailed response. Book
Marking this for reference :smile:

I do like the benefits of a BMS but having it on board adds another possible point of failure like losing brakes like you mentioned, something shorting inside and not being able to see if the BMS is balancing the cells as intended so relying on it on that point.

Which is why I would preferr a simpler method of not having a BMS on the board and have the charging done separately I think those points are why @Hummie is into the non BMS route. 

[quote="TowerCrisis, post:32, topic:64516"]
Over current protection is also a benefit from a BMS. If for whatever reason your motor or main battery leads short out, and it pulls significantly more than 60A in my case, then the BMS will cut power. I think that’s a safety feature that all builders should consider, it’s good fire protection.
[/quote]

This is for discharge BMS? Would there by any way to do this besides a BMS?
```

---
## \#34 Posted by: TowerCrisis Posted at: 2018-08-11T08:45:01.461Z Reads: 52

```
Yes, it's for a discharge BMS. The only other way I really know of is to add a fuse.

Some builders have integrated a fuse into their antispark loop key, but that doesn't have the same amount of protection against internal shorts like a fuse that's close to the battery terminal.

A fuse isn't easily replaceable or necessarily available whereas a BMS will automatically reset, which is why I have a preference towards it.
```

---
## \#35 Posted by: Wraith Posted at: 2018-08-11T09:12:20.109Z Reads: 50

```
I’ve read that discharge BMS have to be able to also take the amount of draw which usually causes them to be large and expensive otherwise they cut off early under heavy riding

Do you have any BMS that you recommend for 12s? Also how do you get to the balance voltage with a charge/discharge bms? Do you just get the average total voltage by reading it straight from the pack as the BMS doesn’t usually display the volts per cell
```

---
## \#36 Posted by: TowerCrisis Posted at: 2018-08-11T15:47:57.938Z Reads: 42

```
Supower battery has some good ones. Rated at 60A continuous for $40. The balance voltage is a spec of the BMS. In the case of supower battery, most of theirs are 3.9V. So as you charge it will only begin balancing a cell with the others once it's voltage reaches 3.9V. It will fully charge to 4.2V.
```

---
