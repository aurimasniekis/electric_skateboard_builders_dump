# At what voltage your pack reaches 100%

### Replies: 146 Views: 6594

## \#1 Posted by: Eboosted Posted at: 2017-03-19T18:56:49.816Z Reads: 298

```
I have a 10S so full charge should be around 42V,  33.6V for 8S, what voltage do you usually get on your fully charged pack?
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2017-03-19T19:15:48.763Z Reads: 292

```
4.2 Volts per cell is pretty much full

Full charge voltages:
3S - 12.6 V
4S - 16.8 V
5S - 21.0 V
6S - 25.2 V
7S - 29.4 V
8S - 33.6 V
9S - 37.8 V
10S - 42.0 V
11S - 46.2 V
12S - 50.4 V
```

---
## \#3 Posted by: Eboosted Posted at: 2017-03-19T19:57:45.632Z Reads: 285

```
My charge stops at 95% every time, 95% means 41.3V
```

---
## \#4 Posted by: Maxid Posted at: 2017-03-19T19:59:34.380Z Reads: 280

```
depends on your charger.
I choose to charge my pack to only 41V instead of 42V - keeps them healthy for longer.
```

---
## \#5 Posted by: Eboosted Posted at: 2017-03-19T20:18:59.440Z Reads: 267

```
I use a regular brick charger, what voltage do you guys (with this charger) get when the led turns green?
```

---
## \#6 Posted by: smurf Posted at: 2017-03-19T21:38:10.140Z Reads: 261

```
Stopping at a 41.3 is very healthy for the battery.
```

---
## \#7 Posted by: Eboosted Posted at: 2017-03-19T22:24:35.152Z Reads: 252

```
I guess It stops at 41.3v because one pack has higher voltage than the rest, so BMS shots the charging down
```

---
## \#8 Posted by: Namasaki Posted at: 2017-03-19T22:38:40.403Z Reads: 247

```
I get 42v at full charge with this charger:
<img src="/uploads/db1493/original/3X/8/5/850ac7365a1491f0c0f2f23b935fe2fd0fc089a0.jpeg" width="375" height="500">
```

---
## \#9 Posted by: smurf Posted at: 2017-03-19T22:50:11.151Z Reads: 234

```
Where did you get that?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-03-19T22:50:47.278Z Reads: 233

```
Amazon.com
```

---
## \#11 Posted by: Maxid Posted at: 2017-03-19T22:54:27.077Z Reads: 232

```
It is a lab power supply - you can get them in almost every electronics shop.
```

---
## \#12 Posted by: smurf Posted at: 2017-03-19T22:56:00.032Z Reads: 235

```
This one?

https://www.amazon.com/KA6005D-Precision-Variable-Adjustable-Regulated/dp/B00G0HAY3U
```

---
## \#13 Posted by: Namasaki Posted at: 2017-03-19T22:56:22.302Z Reads: 230

```
The way it works, 
It starts in CC mode delivering 5a at a voltage just above the current battery voltage until the battery gets to around 41v
then it switches to CV mode and delivers 42v with the current dropping slowly until the battery is full. The bms starts trimming cells to balance at 42v meanwhile the power supply continues to deliver a small amount of current to fill the low cells.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-03-19T22:56:48.250Z Reads: 224

```
Yes, that is exactly the one I have.
```

---
## \#15 Posted by: smurf Posted at: 2017-03-19T22:58:17.362Z Reads: 224

```
Well ideally that's what is happening inside the bricks but the results don't show that.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-03-19T22:59:36.158Z Reads: 226

```
My brick chargers fail to charge my packs fully because they shut off prematurely.
The power supply gives results more like a hobby charger
```

---
## \#17 Posted by: Namasaki Posted at: 2017-03-19T23:05:06.525Z Reads: 225

```
I believe that charging a pack 100% does not harm or shorten it's life.
But that discharging a pack too low can be harmful and shorten its life.
http://techguylabs.com/episodes/1022/how-can-i-make-my-batteries-last-longer
In this link they are talking about device batteries but the basic principle is the same for all lithium batteries.
```

---
## \#18 Posted by: Maxid Posted at: 2017-03-19T23:12:14.681Z Reads: 226

```
You are wrong
http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries

Table 4: Every 0.10V drop below 4.20V/cell doubles the cycle but holds less capacity.
```

---
## \#19 Posted by: Namasaki Posted at: 2017-03-19T23:23:30.014Z Reads: 224

```
I don't have time at the moment to read the whole article but I will later.
One quick point , charging a sinlgle cell to 4.1v would be easy enough.
But if your charging a pack of many cells with a BMS that starts balancing at full charge, how is it going to balance the pack if you never charge the pack full?
```

---
## \#20 Posted by: Eboosted Posted at: 2017-03-19T23:26:32.286Z Reads: 232

```
How are you so sure that BMS does not balance while charging even though it didn't reach 42V?

The most logical method to balance each pack would be to send more amps to the pack with less charge as soon as the charging starts and keep doing it until it reaches 42V
```

---
## \#21 Posted by: Namasaki Posted at: 2017-03-19T23:31:34.466Z Reads: 223

```
1.Protection Circuit Board for 37V 10S Li-ion and Li-polymer battery pack;
2.PCB applies for 10 cells Li-ion/Li-polymer battery pack;
3.To prevent the battery packs from overcharge,overdischarge,over current, over temperature ,short circuit ;
4.Compatible with both Li-ion and Li-Polymer cells.
**5.How balancing function works? after battery pack is fully charged. PCM will detect each cell's voltage and trim higher voltage down until other cells reach the same voltage level. Therefore, it helps cells have longer service life.**
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#22 Posted by: jmasta Posted at: 2017-03-19T23:35:26.654Z Reads: 228

```
The specs of your BMS should tell you when it begins balancing

For example the specs for my BMS (from Battery Supports) state:

> **Technical Parameters:**

> Balanced current: 60mA (VCELL = 4.20V when)
> Balanced for: 4.20 ± 0.05 V


Recently I have only been charging to about 80% (4.00V/cell), which means the BMS is not balancing the cells.  The max delta voltage between all 12 cells has only grown from 0.02V to 0.04V after several partial cycles without balancing.  Perhaps a good practice would be to go to 4.20V every few cycles to force the BMS to balance

That said, I don't think charging to 100% each cycle will have any real negative effect on battery life.  Discharging too far would be much worse
```

---
## \#23 Posted by: Eboosted Posted at: 2017-03-19T23:45:47.750Z Reads: 219

```
That's the Bestech BMS logic, I wonder what would be the Battery Supports one.

Lets state an example:

1. Battery pack does not charge full with a brick charger only until 41V
2. You forcethe charge with a high powered charger as the one you posted from Amazon
3. Battery pack reaches 42V
4. At least one individual cell was unballanced, 9 packs have 4.15V and the unbalanced one 4.65V (cell has already being damaged)
5. Balancing from BMS starts lowering the unbalanced cell from 4.65V back to a normasl 4.2V and rasing the other 9 packs to 42V

If order to verify this you will need meassure the voltage of the highest pack before and while balancing occurs
```

---
## \#24 Posted by: jmasta Posted at: 2017-03-19T23:52:20.496Z Reads: 226

```
To me it seems **Depth of Discharge** is the biggest factor. As long as you don't let your battery sit at full voltage for long, charging to 4.20V should not adversely affect the overall battery life


<img src="/uploads/db1493/original/3X/1/4/14dc58e0874097ef165ef1cfd621dcbae4027a1d.png" width="690" height="455">
```

---
## \#25 Posted by: jmasta Posted at: 2017-03-20T00:07:43.291Z Reads: 217

```
[quote="Eboosted, post:23, topic:19302, full:true"]
That's the Bestech BMS logic, I wonder what would be the Battery Supports one.[/quote]

They either begin balancing at 3.90V/cell or 4.20V/cell

I have one from SuPower (aka Battery Supports) and I can't figure out how to tell which model I have. When I bought it from eBay last year, I could have sworn it said 3.9V, which is what their website claims. But their eBay listing now says 4.2V.  Emailing them was not helpful at all

Balancing starts at 3.9V: http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html

Balancing starts at 4.2V: http://www.ebay.com/itm/44V-48V-50-4V-12S-60A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System-/221644780045
```

---
## \#26 Posted by: Namasaki Posted at: 2017-03-20T01:25:47.786Z Reads: 197

```
[quote="Eboosted, post:23, topic:19302"]
At least one individual cell was unballanced, 9 packs have 4.15V and the unbalanced one 4.65V (cell has already being damaged)
[/quote]

If a pack was this far out of balance, charging to even 40v would be a problem.
```

---
## \#27 Posted by: Namasaki Posted at: 2017-03-20T01:31:30.132Z Reads: 187

```
[quote="jmasta, post:24, topic:19302"]
To me it seems Depth of Discharge is the biggest factor. As long as you don't let your battery sit at full voltage for long, charging to 4.20V should not adversely affect the overall battery life
[/quote]

I agree with this theory.
I think it is better to charge to 100% and discharge to %40 than to charge to 80% and discharge to 20%
```

---
## \#28 Posted by: Eboosted Posted at: 2017-03-20T01:33:54.703Z Reads: 173

```
Not if the brick charger stopped the charge (which was the correct thing to do), but with a high power charger as your it might have continued until it reached 42V damaging all unbalanced packs.

Just a thought, maybe I'm mistaken, but wouldn't be bad to check the voltage of each individual cell.
```

---
## \#29 Posted by: Namasaki Posted at: 2017-03-20T01:47:46.779Z Reads: 169

```
It's really hard to say since it is a hypothedical situation and a very unlikely one at that.
Normally if you have an extreme out of balance situation, it will be one cell much lower than the rest.
```

---
## \#30 Posted by: Eboosted Posted at: 2017-03-20T04:30:36.052Z Reads: 164

```
When my battery only charged at 90%, in my case at least, it was because one of the packs was higher than the rest, BMS shutted down the charging cycle to prevent damaging of the highest voltage cell.

When I checked the voltage of individual packs, only two of them had 4.20V and the other nines were 4.05-4.08V, if you sum them all up you got 40.8V only, brick charger refused to charge more. I'm not sure if it'll be a good idea to force charge the battery with a high powered charger as yours.

To fix my issue, I individually lowered the voltage of one of the unbalanced packs and after that I was able to charge until 95% again, I'm going to lower the other pack as soon as I have time and I'm pretty sure it'll go all the way up to 42V after that.

I'm not the owner of the truth, just pointing out my own experience.
```

---
## \#31 Posted by: Namasaki Posted at: 2017-03-20T04:57:03.268Z Reads: 154

```
[quote="Eboosted, post:30, topic:19302"]
BMS shutted down the charging cycle to prevent damaging of the highest voltage cell.
[/quote]

If the BMS shut down the charging cycle, it would have done that with either charger.
A Lab power supply isn't really a "high power charger" it's just a power supply that can be used as a charger while allowing the operator full control of voltage and current and lets you monitor the voltage and current going into the battery.
Because the power supply switches to CV mode when the battery is around 90% full, the current output decreases steadily to below 1 amp so the final stage of charge is done at very low current.
```

---
## \#32 Posted by: PXSS Posted at: 2017-03-20T05:03:51.704Z Reads: 153

```
You can't take partial information from a source to suit your needs. That same source states how many cycles more you get from not fully charging @jmasta @Namasaki. The proof is there. If you choose to ignore it then that's your choice...

<img src="/uploads/db1493/original/3X/7/f/7f07646ba82756c9fa4ad7a99ef6469ba4f9fb8f.PNG" width="281" height="499">

This is technical data based on lots of research papers. All of their citations are there. We discussed this recently (yesterday) in some other thread.
```

---
## \#33 Posted by: Namasaki Posted at: 2017-03-20T05:20:47.005Z Reads: 135

```
They have a chart for charging and a similar chart for discharging.
So you can increase cycles by under charging or by under discharging.
I'm just saying that I believe under discharging is the better option.
And it's good that we are getting opinions from both sides so that people who read this can make up their own minds.
Partial Charge or Partial Discharge
Or, you could do both if range isn't an issue.:wink:
```

---
## \#34 Posted by: PXSS Posted at: 2017-03-20T05:28:05.017Z Reads: 137

```
@Namasaki It just seemed from your initial post that you were dismissive of life cycle improvement through lower full charge. Yes, you can trim up at either end and ideally at both. 

80% DoD gets you roughly 33% more cycles
80% Charge gets you roughly 200% more cycles. 
Take it however you want.
```

---
## \#35 Posted by: Eboosted Posted at: 2017-03-20T05:28:58.401Z Reads: 139

```
Yeah, that's the beauty of this forum.

But whatever is the voltage of the whole pack we choose to charge, we need to have each pack well balanced.

Tomorrow I'll try to manually discharge/balance the highest voltage pack just to see if the charging capacity increases. 

<img src="/uploads/db1493/original/3X/5/d/5d34490b5a2c0136f2e4288708c1b2773e742ec0.jpg" width="374" height="500">
```

---
## \#36 Posted by: Namasaki Posted at: 2017-03-20T05:34:36.978Z Reads: 136

```
[quote="PXSS, post:34, topic:19302"]
80% DoD gets you roughly 33% more cycles80% Charge gets you roughly 200% more cycles.
[/quote]

In order for that to be an equal comparison, you would have to discharge your 80% battery to 0%
And I don't think your gonna want to do that.
I think that fully charging and partially discharging is the better option because discharging is harder on the batteries than charging.
At Least that has been my experience with Lipo batteries. I've seen them get hot and swell during discharge but never seen it while charging them.
```

---
## \#37 Posted by: Namasaki Posted at: 2017-03-20T05:41:15.839Z Reads: 131

```
[quote="PXSS, post:34, topic:19302"]
It just seemed from your initial post that you were dismissive of life cycle improvement through lower full charge.
[/quote]

I did not believe it at the onset of this discussion but now that I have seen the article, I accept that it is true. :bulb:
```

---
## \#38 Posted by: PXSS Posted at: 2017-03-20T05:43:18.140Z Reads: 129

```
li-ions hate being at high voltage. That is fact. I discharge my li-ions to 2.5V at work all the time. 

You measure the temperature delta while charging and discharging at the same current and tell me which one gets hotter. There's a reason why the charge current rating is way lower than the discharge rating
```

---
## \#39 Posted by: Namasaki Posted at: 2017-03-20T05:44:23.628Z Reads: 126

```
My point is that we charge at a much lower current than we discharge.
Thats partly why I would rather cut the discharge short than the charge.
Besides, as we discharge the voltage drops and more current is needed to produce the same wattage.
```

---
## \#40 Posted by: PXSS Posted at: 2017-03-20T05:51:07.821Z Reads: 132

```
As I said, I've discharged tens of packs down to 2.5V for hundreds of cycles. Look up the spec sheets, manufacturers do it all the time too. I don't see the point in cutting it short other than you might over discharge a cell if your cells are out of balance. 

I have data. Lots of it. I cannot share it since it's work related but trust me. You rather trim up top than bottom. The numbers don't lie. 

Good night!!! (It's 2am!!! :sweat:
```

---
## \#41 Posted by: Namasaki Posted at: 2017-03-20T05:54:03.288Z Reads: 132

```
This has been a good discussion but it's also getting late here and I have to get up early so good night.
```

---
## \#42 Posted by: Eboosted Posted at: 2017-03-20T06:22:24.301Z Reads: 134

```
In that case, I'm going to test a cutoff start voltage of 28v and cutoff end at 26v, let's see how range is improved
```

---
## \#43 Posted by: jmasta Posted at: 2017-03-20T07:23:37.552Z Reads: 143

```
This an interesting chart. You'll notice that 75-65% gives the best cycle length.  But this is somewhat misleading because you are only using 10% of the battery's capacity.  

So we don't necessary seek a long cycle life, but rather- a long cycle range [miles].  
We want to **maximize range** (i.e. Depth of Discharge) while **minimizing capacity loss**.  




There are multiple values at play here:

<img src="/uploads/db1493/original/3X/f/8/f887cc727658dd96f44b6077871527cb02e55f72.jpg" width="570" height="456">




I wanted to see if we could use this chart to find an optimal charging/discharging strategy.  I interpolated values at **4000 cycles** to find the percent capacity loss, and recorded them in the table below.  Assume that DOD is proportional to the amount of energy used, and therefore proportional to your cycle range.  

We want a high range (DOD%) with minimal Capacity Loss:

<img src="/uploads/db1493/original/3X/0/5/055a8ff1f76fa566ac9cbcee4f4f64e8ce0de408.png" width="690" height="273">

This would suggest that the best strategy is to **charge to 85%** and **discharge to 25%.**

* (85-25%) maximizes range with the least effect on battery life

* (75-25%) is much better than (100-50%) but has the same theoretical range (50% DOD)

* (100-25%) has the best range, and would still be a viable charging strategy. It is not nearly as bad as the first chart would suggest because you are getting much higher range for each discharge cycle
```

---
## \#44 Posted by: smurf Posted at: 2017-03-20T07:47:03.422Z Reads: 121

```
What was the charging strategy used? Did they charge at 4.2 volts and just stop at 85% or did they charge with reduced voltage?
```

---
## \#45 Posted by: Maxid Posted at: 2017-03-20T07:51:03.668Z Reads: 119

```
I feel like you guys are overcomplicating this. Charging to 4.1V per cell instead of 4.2 only decreases the usable energy by ~3%. This is barely noticeable and will already double the cycle life which is good. The level of discharge is much harder to control as that depends on your riding style and the distance you travelled. I am pretty sure you will not stop riding while in the woods far away from home just because you reached 25% of your capacity. You will ride until you get to the next convenient power outlet. 
The only value that makes sense to adjust is the end of charge voltage. After that just ride your battery and charge it as often as possible.
```

---
## \#46 Posted by: jmasta Posted at: 2017-03-20T08:01:16.396Z Reads: 116

```
You're missing the point.  You can't always charge to 4.10V if your BMS does not start balancing until 4.15V.  

Charging to 4.20V is fine but not ideal for battery longevity
```

---
## \#47 Posted by: Maxid Posted at: 2017-03-20T08:03:48.993Z Reads: 118

```
Which is why I don't use a BMS in the first place ;)
Also I am pretty sure those discharges were not at the same currents we use - which will decrease cylce life even more. Your numbers are already "cleaned" of those additional factors and gives the result for only the charge voltage deviations.
```

---
## \#48 Posted by: smurf Posted at: 2017-03-20T08:19:22.403Z Reads: 111

```
I'll bet the regenerative braking doesn't help either.
```

---
## \#49 Posted by: SimosMCmuffin Posted at: 2017-03-20T08:26:48.036Z Reads: 124

```
4.1 Volts seems like a good deal for longevity, because it has such a minimal impact on SoC (assuming that you can balance your pack). I do believe pretty much all manufacturers spec their cells at the 4.2 charge voltage and then give out the cycles for 70% capacity left with full DoD.

Samsung INR18650-25R
<img src="/uploads/db1493/original/3X/c/9/c9dfe09f95ab012872baac7b26dc98cd08c76375.jpg" width="690" height="490">

LG INR18650-HG2
<img src="/uploads/db1493/original/3X/8/b/8bd00c202cc733231a068abbb1835630ab4e2e99.jpg" width="414" height="500">

So we are already trying to outperform the spec'd cycle performance, but that doesn't mean we shouldn't do it.
```

---
## \#50 Posted by: jmasta Posted at: 2017-03-20T08:28:46.942Z Reads: 117

```
[quote="Maxid, post:47, topic:19302, full:true"]
...
Also I am pretty sure those discharges were not at the same currents we use - which will decrease cylce life even more. Your numbers are already "cleaned" of those additional factors and gives the result for only the charge voltage deviations.
[/quote]

Those are not "my numbers", and they are not "cleaned" of anything. I am simply interpreting and analyzing the data  in the article.  The article **you** presented


[quote="Maxid, post:18, topic:19302"]
You are wrong
http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries
[/quote]
```

---
## \#51 Posted by: Maxid Posted at: 2017-03-20T17:31:28.423Z Reads: 111

```
Salty much?

You used them to make your case - I just doubted that you can take them quantitatively like that.
```

---
## \#52 Posted by: jmasta Posted at: 2017-03-20T18:31:23.627Z Reads: 115

```
Actually I used the numbers to disprove my original theory...

I'm not saying that your battery will have exactly 86% capacity if your discharge it from 85-25% exactly 4000 times. Not at all.  Your actual cycle count will be much less because of our high discharge rates. It's not even something you can predict because of all the variables involved.  The point is hold one variable constant  (the discharge rate) to find general trends to help guide our charging/discharging.

The numbers suggest it is **better to do a partial charge + full discharge (i.e., 85-25%)**, than it is to do a full charge + partial discharge (i.e., 100-40%).  

Or as @PXSS put it more simply:  

[quote="PXSS, post:38, topic:19302"]
li-ions hate being at high voltage
[/quote]

But charging to 100% is often necessary, especially if you use a BMS for balancing.  If you were really concerned about battery longevity, maybe you'd only want to go to 4.20V every few cycles. Personally I don't think it really matters; I have way more range than I need, so even 70% capacity after hundreds of cycles is perfectly fine for my needs
```

---
## \#53 Posted by: Namasaki Posted at: 2017-03-20T20:53:21.705Z Reads: 110

```
[quote="Maxid, post:47, topic:19302"]
Which is why I don't use a BMS in the first place
[/quote]
So what method do you use to balance your pack?
```

---
## \#54 Posted by: Maxid Posted at: 2017-03-20T22:30:21.597Z Reads: 108

```
None - I just leave them at 41v until the current drops significantlly to like 100-200mA.
That is the @whitepony way :) and it worked perfectly so far.
```

---
## \#55 Posted by: Eboosted Posted at: 2017-03-20T22:31:54.458Z Reads: 112

```
@maxid what charger balancer do you use to perform that procedure?
```

---
## \#56 Posted by: Maxid Posted at: 2017-03-20T22:32:30.206Z Reads: 117

```
I use a DROK charger - that is basically a small lab power supply
Made myself a 3D printed case for it together with a laptop psu to get the necessary DC voltage for the DROK
```

---
## \#57 Posted by: PXSS Posted at: 2017-03-20T22:32:54.235Z Reads: 127

```
The issue with this data is that they do not explore charging to 65% and discharging to 15% or 55% to 5%. 

How do we know that 75%-25% is ideal or 85%-25%. 

I'm with @Maxid, charge lower and ride till it dies. Low voltage doesn't hurt cells as long as you're not storing them there long enough so that self discharge kills them. The only reason not to discharge to 0% is because if the cells are not balanced at the low end, you could end up with a cell below the 2.5V limit. So in my case I will be lowering my cutoff to 26V. What I need now is a proper watt controller instead of current controller. I may talk to @Ackmaniac to see if he's willing to take up the task, e.g. 0 throttle corresponds to 0W and 100 Throttle corresponds to a defined Wattage. 

@Namasaki 
I'm sure we could source a BMS from Bestech designed to balance charge at a lower voltage.
You can also balance your packs with an RC charger which is what I do

---

Also, we do not need to balance on every charge. I would say once every 10 cycles or once a week, given that we use good cells. 

---
BTW I think I figured out why people keep having issues charging to 100% with a BMS.
In short, the BMS only balances with very small currents and the brick charger shutoff current is higher than this, therefore it will turn off before it starts balancing. @Namasaki's lab supply works because it's current cutoff is lower than the max balance current.

---
@Maxid, if you do not balance at all how do you know if one of your cells is going bad?
Basically, you're just using a brick charger straight to the battery. If one cell does go bad and you don't catch it, you could easily kill the rest of your pack, even if you're only charging to 41V
```

---
## \#58 Posted by: whitepony Posted at: 2017-03-20T22:47:08.186Z Reads: 125

```
[quote="PXSS, post:57, topic:19302"]
if you do not balance at all how do you know if one of your cells is going bad?Basically, you're just using a brick charger straight to the battery. If one cell does go bad and you don't catch it, you could easily kill the rest of your pack, even if you're only charging to 41V
[/quote]

Im running batteries like that since 3 years now - some of them under quite a lot of use with several thousand kilometers of boarding per year. initially I was suspicious and kept measuring cell voltages quite often, but I got more sloppy by each month. my latest boards dont even have balance wires anymore, because the 2 batteries I kept monitoring never ever showed any drift at all. like at ALL!

several factors contribute to that i think:
* using only quality cells from long standing quality distributors such as nkon.nl
* 4.1V/cell cut off for better cell life and some robustness towards drifting (if it should ever occur)
* winter storing the battery in a cool place at 3.6V/cell
* I never discharge lower than 3.0V/cell, vesc soft cutoff 3.4V->3.0V
* i never draw a lot of current when the battery is cold - when I ride in winter, I start with a room temperature battery
* i generally dont really demand much current from my batteries, cause Im mostly single motor carving
* I avoid all heat, always keep the board in shadows during summer
```

---
## \#59 Posted by: Maxid Posted at: 2017-03-20T23:09:54.137Z Reads: 117

```
My 10S battery is divided into two 5S packs with balancing wires. This means I can check them on a standard RC charger. The few times I tried all cells were perfectly in sync.
```

---
## \#60 Posted by: PXSS Posted at: 2017-03-20T23:37:23.835Z Reads: 115

```
Not saying it's not doable, but you have to be very vigilant on how you treat your cells and all as @whitepony is.
Using quality cells is a big one, but every once in a while you just get unlucky and get a dud.

I personally rather not limit their performance that heavily and balance them whenever I see them go more than 50mV out of balance but I also own a $350 charger that has programmable charge and discharge features
```

---
## \#61 Posted by: Namasaki Posted at: 2017-03-21T01:46:20.391Z Reads: 112

```
[quote="PXSS, post:60, topic:19302"]
I also own a $350 charger that has programmable charge and discharge features
[/quote]

Wow, and I thought I went overboard on my $170 charger
```

---
## \#62 Posted by: Namasaki Posted at: 2017-03-21T01:50:57.656Z Reads: 113

```
[quote="PXSS, post:57, topic:19302"]
I'm sure we could source a BMS from Bestech designed to balance charge at a lower voltage.You can also balance your packs with an RC charger which is what I do
[/quote]

Here are the adjustable parameters:
<img src="/uploads/db1493/original/3X/4/f/4f14b907da214a7ed1b5d2b479b7bde0594d7cab.png" width="431" height="500">
```

---
## \#63 Posted by: PXSS Posted at: 2017-03-21T02:03:38.086Z Reads: 106

```
Yep. I know. But I also know that you can get customized ones from them too as we do for work
```

---
## \#64 Posted by: Eboosted Posted at: 2017-03-29T06:01:56.672Z Reads: 107

```
I found last week 2 of my cells were 0V, BMS didn't detect that because I'm using it only for charging.

I don't want to go over this again and at the moment I have a pack with 2V less than the rest, it's taking forever to balance on each charge cycle

@namasaki you were right regular brick chargers won't do the job.

Brick chargers are presetted at 42.3V howewer BMS will stop the charge as soon as the first pack reaches 42V (for protection) and will stop charging completely, leaving lower voltage packs unbalanced.

What we need is to charge the pack at 41V as suggested by @Maxid, sending small current amounts until all cells are filled equally, in this case we won't need a BMS at all.

So I decided to buy an adjustable balancer charger and forget about all BMS nonesense.

Is there a travel size charger or all of them are big as the DROC and 
KORAD? or all of them are huge boxes?
```

---
## \#65 Posted by: Namasaki Posted at: 2017-03-29T06:33:39.851Z Reads: 103

```
The one I got really isn't too big. It is kinda heavy though. It's a Linear power supply and they tend to be a bit heavy.
I use it at home and I still have my 5a brick charger for travel.
```

---
## \#66 Posted by: Namasaki Posted at: 2017-03-29T06:39:43.966Z Reads: 98

```
[quote="Eboosted, post:64, topic:19302"]
What we need is to charge the pack at 41V as suggested by @Maxid, sending small current amounts until all cells are filled equally, in this case we won't need a BMS at all.
[/quote]

I would keep the bms because as in your case, you have one cell group that's not taking a charge, you might wind up charging 9 cell groups to 41v or 4.5v per cell group which could be a real problem.
```

---
## \#67 Posted by: Eboosted Posted at: 2017-03-29T06:40:16.220Z Reads: 96

```
Were your cells perfectly balanced after the first charge on the Korad?

Are you charging until 42V or less?

How do you charge your cells if the charger does not have a laptop plug, do you have an addapter?
```

---
## \#68 Posted by: Namasaki Posted at: 2017-03-29T06:44:06.654Z Reads: 97

```
I haven't pulled the enclosure and checked them after fully charging. I will do that in the next couple days and report back.
I am charging to 42v but I usually stop when the power supply output drops to around 50ma.
When I start charging, its in CC mode with 5a and voltage just a little higher than the battery.
As it charges the voltage output increases as the battery voltage increases.
Once the battery gets to around 90%-95% the power supply switches to CV mode and the voltage is at 42v and the current start to decrease as the battery fills.
I made a charge cable with banana plugs on one end to plug into the charger ports.
```

---
## \#69 Posted by: Eboosted Posted at: 2017-03-29T06:48:17.509Z Reads: 96

```
[quote="Namasaki, post:66, topic:19302"]
I would keep the bms because as in your case, you have one cell group that's not taking a charge, you might wind up charging 9 cell groups to 41v or 4.5v per cell group which could be a real problem.
[/quote]

If this happens how would the charger fill the half-charged cells?, BMS would detect a cell with 4.2V and stop all charging activity leaving low charged cells still unbalanced.

I guess in this case it'd be better to charge at lower voltage, once all packs are balanced, charger would continue the charge all the way to 4.2V for each pack.
```

---
## \#70 Posted by: Namasaki Posted at: 2017-03-29T07:02:05.970Z Reads: 94

```
If I understand correctly, the bms monitors each cell or cell group and when they reach the detection voltage, it starts trimming them down. On my bms the detection voltage is 4.28
Hobby chargers continue to fill low cells while trimming higher cells once they are full.
I think the bms will do this also IF the charger will continue to supply low amperage charge while the full cells are being trimmed. 
This is where the adjustable power supply rocks.  And the brick charger falls short.
I'm gonna do a test in next couple days.
I'll pull the cover off and record all cell voltages before charge and again after full charge and I'll get back to you with the results.
```

---
## \#71 Posted by: Eboosted Posted at: 2017-03-29T15:00:33.397Z Reads: 95

```
I'd like to buy an adjustable charger or hobby charger for this purpose but really don't want to buy one as big as yours, it's difficult to carry around, I wonder if that'll be the only alternative
```

---
## \#72 Posted by: Namasaki Posted at: 2017-03-29T15:29:45.829Z Reads: 97

```
If you can find a hobby charger for 10s, it will be expensive. 
If you use a power supply, it will need to be a CC/CV with adjustable voltage and current. 
Commonly they come in 30v and 60v versions. 
So for 10s you would need 60v. 
You could save money by getting a 3a version. 
As far as size and weight, it is what it is.
```

---
## \#73 Posted by: Eboosted Posted at: 2017-03-29T17:15:33.344Z Reads: 98

```
I wonder if this one would work:

https://www.amazon.com/Digital-Adjustable-Regulated-Stabilizer-Supply/dp/B01N6AHGTG/ref=pd_sbs_469_6?_encoding=UTF8&pd_rd_i=B01N6AHGTG&pd_rd_r=0H79F16T09Y6XBJ6746J&pd_rd_w=y8AHl&pd_rd_wg=VXgWB&psc=1&refRID=0H79F16T09Y6XBJ6746J
```

---
## \#74 Posted by: smurf Posted at: 2017-03-29T17:47:24.271Z Reads: 95

```
10 amps

https://www.circuitspecialists.com/bench-power-supply-csi6010x.html
```

---
## \#75 Posted by: Namasaki Posted at: 2017-03-29T22:02:04.406Z Reads: 94

```
[quote="Eboosted, post:73, topic:19302, full:true"]
I wonder if this one would work:
amazon.com
  Digital Adjustable Regulated Stabilizer DC Power Supply 60V 5A
Features: 1. Leading technology: new PWM switch for voltage stabilization, MOS linear secondary voltage stabilization 2. Energy-saving and high efficiency: over 80% high efficiency, 40% higher than 
$65.99
[/quote]
It has CC AND CV so it should work.
```

---
## \#76 Posted by: Namasaki Posted at: 2017-03-29T22:03:46.244Z Reads: 93

```
[quote="smurf, post:74, topic:19302, full:true"]
10 amps
https://www.circuitspecialists.com/bench-power-supply-csi6010x.html
[/quote]
I didn't see a price on the link but it looks expensive.
```

---
## \#77 Posted by: smurf Posted at: 2017-03-30T00:45:19.474Z Reads: 94

```
Ya I know I would like to get a powerful charger but there just so expensive.
```

---
## \#78 Posted by: Okami Posted at: 2017-03-30T01:21:16.776Z Reads: 98

```
Im sorry guys for cutting your power supply / charger talk short but I wanted to ask @PXSS one question directly
 
[quote="PXSS, post:40, topic:19302"]
As I said, I've discharged tens of packs down to 2.5V for hundreds of cycles. Look up the spec sheets, manufacturers do it all the time too.
[/quote]

With this - do you mean **rest voltage** or **under-load voltage**?

---
I tried to bring my cells to **2.8v rest voltage**.. but they were weak as fuck so to speak at already 3.1v rest voltage or so..
---
At using the cells with 3.0v rest voltage, the voltage started to ''dip into red zone'' - of 2.3v or so **under load** at 2.5 A of load per cell. These are 10A capable cells, so the load was about 0.25c when on their weak side..

---

So - @PXSS what do you consider ''red zone'' for cells under load? How much voltage sag have you experienced and how much sag is ''normal'' and can be sustained? 

I might as well go into this on the old voltage sag topic.. but since u mentioned 2.5v I got interested..
```

---
## \#79 Posted by: PXSS Posted at: 2017-03-30T01:25:36.592Z Reads: 96

```
@Okami. Stuck in traffic, so short answer is 2.5v under load. 2.5v is your absolute minimum. Can be more detailed later
```

---
## \#80 Posted by: Okami Posted at: 2017-03-30T01:29:13.336Z Reads: 94

```
@PXSS  Cool. Thanks for letting me know! yeh more detailed answer would be nice.. if it gets too lenghty u might as well write to me in private!

I think this is a bit misleading that 2.5v is not **''marked''** as no load voltage.. since it is not always possible to determine what is the rest voltage at this level or when battery has already depleted itself..
```

---
## \#81 Posted by: PXSS Posted at: 2017-03-30T01:49:38.523Z Reads: 99

```
2.5V under ***any*** load is empty. That's what I meant by absolute minimum. Under no circumstances should your battery ever be under 2.5V regardless of the no load or rest voltage. 

The battery cannot have an empty no load voltage as you voltage sag varies with current draw. How would manufacturers define empty voltage? 
2.5V at no load
2.3V at 5A
2.0V at 10A
1.5V at 15A
You see how fast that gets confusing plus the cell only cares about the actual voltage and not the no-load. 

Its easier to determine a voltage which you should stay above under any current draw.  This is why the higher your current draw the lower the capacity of the cell is.

E: @Okami 
25R at 1A to 2.5V= 2.4Ah
25R at 10A  to 2.5v= 2.3Ah

If you slow down the current draw from 10A to 1A keeping the voltage at 2.5 (like what happens when you charge), you would get almost the same capacity (difference would be losses due to heat at higher current draw)
```

---
## \#82 Posted by: Namasaki Posted at: 2017-03-30T01:58:33.495Z Reads: 99

```
@PXSS @Okami
Not sure if you realize it but you are making a very good argument for using a bms for discharge.
Seeing that a bms will monitor individual cell group voltage and shut you down if any cell group dips below a safe level while under load.  
I ran my Li-ion battery until the bms shut down and there was no damage to the battery. My low voltage trigger was set at 2.8v
```

---
## \#83 Posted by: Okami Posted at: 2017-03-30T01:58:53.892Z Reads: 101

```
Yeh, cutting down power once cell reaches certain ''treshold'' sounds reasonable..

Though.. it pinpoints the ''problem'' which you are talking about.. if load is not big, you can continue to ''sip'' the power from battery for longer period of time before it gets drained..


I've also seen charts where energy count graph is cut short, since load for cell was way higher.. and the process was stopped way earlier.. than when cell was discharged at very little load, for example..

---

@Namasaki

I suspect the ''danger'' might be way higher for these who dont use any other cell monitoring methods or 'tactics'.. 

Generally, I think it can be felt quite easly if battery / pack is quite empty or close to depletation.. setting some limits or 'warnings' of course is a good choice and just provokes / sustains longer battery life.. if we assume cells might get a bit more damaged if overdischarged regularly..

---

On a side note.. if talking about BMS'es, I think they can be ''poked around'' a lot... but the final fact, conclusion i have come to, is that they need to be functioning or of high quality not to cause more problems than they are meant to solve.. have heard of too many stories of faulty bms'es which cuts power way too early, stops working, does not balance cells properly or cause some other issues.

---

So far Raphael Chang's bms seems to be the most promising.. but I believe he is only in early production phase as the first bms'es are yet to be received by the first customers / testers..

--

Sorry for taking this reply so long, sometimes it just happens when I want to adress more than one issue / argument to which I want to respond..

Though I still find it interesting that I was able to draw enough power to propel the board forward.. but non the less, the last 5-10 mins i had of it riding slowly was not very 'enjoyable' in a sense that the lack of power could be felt drastically. 

And to those who might not be aware, I did that on purpose to see how low the cells can go and what rest voltage will they sit, since there are still discussions about when power should be cut and when some time ago I came to conclusion that 3.3-3.4v no load voltage is a somewhat good point, some ppl were suggesting to deplete them further since there was still energy left..
```

---
## \#84 Posted by: Namasaki Posted at: 2017-03-30T02:09:57.879Z Reads: 94

```
I agree totally and that is why I cringe whenever I see anyone saying that they just want to buy a cheap bms.
```

---
## \#85 Posted by: Eboosted Posted at: 2017-03-30T05:47:20.779Z Reads: 94

```
How is your power supply holding up?, I've read too many DOA stories on the US$ 65 power supply I found on Amazon, I wonder if I should just pull the trigger and buy a better power supply like your Korad
```

---
## \#86 Posted by: Namasaki Posted at: 2017-03-30T05:53:44.762Z Reads: 94

```
The one I got works perfectly. It's has a fan that runs the whole time its on and it never gets hot or even warm even when charging at 5a.
It has good reviews which is partly why I pulled the plug and bought the more expensive model.
I think it's a good idea especially if your gonna be charging on a daily basis.
This one also has a really good feature:  There is a main power switch that you turn on and set the power settings and then there is another switch that enables the output.
```

---
## \#87 Posted by: Eboosted Posted at: 2017-03-30T05:56:21.831Z Reads: 92

```
I'd like to know if you were able to complete balance you unbalanced cells with only one charge on this power supply
```

---
## \#88 Posted by: Namasaki Posted at: 2017-03-30T06:05:03.076Z Reads: 93

```
Surfing today and tomorrow.  We have a swell that peaked today and hopefully some leftovers tomorrow.
I'm gonna try to get the test done by Saturday and I'll post the results as soon as I have them.
Both batteries are over 39v now so I want to drain one down at least the nominal and record the voltages before and after charging.
```

---
## \#89 Posted by: Eboosted Posted at: 2017-03-30T06:12:38.916Z Reads: 93

```
I pulled the trigger and got this one, you really convinced me. It's the same as yours but only rated at 3A instead of 5A, I don't mind waiting a bit longer to charge a pack, just need to keep them balanced.

Hope it has the same features as yours.

http://www.ebay.com/itm/131286137884

I'll wait eagerly on your charging results
```

---
## \#90 Posted by: Namasaki Posted at: 2017-03-30T06:18:20.819Z Reads: 86

```
It's exactly the same as mine except for the amperage output.  3a should be fine.
```

---
## \#91 Posted by: PXSS Posted at: 2017-03-30T14:26:49.492Z Reads: 88

```
[quote="Okami, post:83, topic:19302"]
Though.. it pinpoints the ''problem'' which you are talking about.. if load is not big, you can continue to ''sip'' the power from battery for longer period of time before it gets drained..
[/quote]

This is not a problem. It's just how batteries work... Less wasted energy by drawing little current.

[quote="Okami, post:83, topic:19302"]
I've also seen charts where energy count graph is cut short, since load for cell was way higher.. and the process was stopped way earlier.. than when cell was discharged at very little load, for example..
[/quote]

The process was not stopped short. It was stopped when the cell reached 2.5V. You need to forget about the energy count, the rated capacity is just what the manufacturer guarantees the cell will output at a specified current. This would change if you ran it faster or slower, it's just how the chemistry works.

@Namasaki, ish... If you set your esc limits correctly it shouldn't be an issue but if you're trying to empty the cells constantly and are not properly balancing your cells then as @Eboosted found out, you will kill your cells. Having the battery discharge through the BMS would have saved his pack.

[quote="Okami, post:83, topic:19302"]
On a side note.. if talking about BMS'es, I think they can be ''poked around'' a lot... but the final fact, conclusion i have come to, is that they need to be functioning or of high quality not to cause more problems than they are meant to solve.. have heard of too many stories of faulty bms'es which cuts power way too early, stops working, does not balance cells properly or cause some other issues.
[/quote]

There is nothing wrong with the BMSs, its the combination of BMS and crappy charge. I think I mentioned it in another thread already. The reason @Eboosted BMS stops his brock charger from balancing is because the brick charger has a minimum current output, once the current gets too low in cv mode then the brick stops charging so it doesnt damage the cells. The BMS from batterysupports only consumes like 80mA when balancing, if this is lower than the cutoff current then the brick charger will cutoff current before he gets to the balancing stage. Since he didn't have a low voltage cutoff on the individual cells then the ESC only stopped working when the whole pack was under a specified voltage. So max voltage per cell is 4.2V and I'm assuming his ESC low voltage cutoff is 30V for a 10S pack. Then he can have 7 cells at 4.2V, 1 at 0.6V and 2 at 0V before his ESC and BMS limits converge. At this point 3 of the cells in the pack are dead.
```

---
## \#92 Posted by: Eboosted Posted at: 2017-03-30T14:51:52.891Z Reads: 81

```
Well, from my own tests I found out the brick charger stops as soon as the first pack reaches 42V, I guess in this stage BMS restricts current draw and brick charger stops, so the charging cycle stops because a combination of the two.
```

---
## \#93 Posted by: Okami Posted at: 2017-03-30T15:37:37.067Z Reads: 80

```
Doesnt this suggest that voltage should be higher when using brick charger + bms?

How much over-voltage can bms take?
```

---
## \#94 Posted by: PXSS Posted at: 2017-03-30T16:01:15.152Z Reads: 84

```
Yeah, the brick charger has a minimum current which is higher than the balancing current. That would be why it stops as soon as the BMS reaches the balancing stage.

The reason lab power supplies work is because they can go down to miliamps
```

---
## \#95 Posted by: Eboosted Posted at: 2017-03-30T16:04:59.966Z Reads: 87

```
If the assumptions from this thread are correct, the charge shouldn't exceed 42V, it should be lower at e.g. 41V (set with an adjustable CC/CV power supply) but the current shouldn't stop flowing, this would allow all empty cells to be charged at 41V at minimum current (CC mode on the power supply), after that you could normally charge the remaining 1V untill 42V normally (power supply or brick charger), until this stage BMS shouldn't have been working at all.

However if the cells are in fact 99% balanced, BMS will work blancing them as soon as the whole pack reaches the balancing voltage, 42.7V for the Bestech BMS, not sure about the Battery Supports one, but I guess somewhere below that.
```

---
## \#96 Posted by: PXSS Posted at: 2017-03-30T17:03:24.927Z Reads: 86

```
@Eboosted
The BMS will start working as soon as ony one cell reaches 4.2V. This could be at 26.7V if all of your other cells are at 2.5V. You don't need to be afraid of the BMS doing its job. The reason your stuff failed is because you were just using a bad combo.

Seriously, read the following slowly...

Brick Charger,
42V 4A output
cutoff at 400mA

BMS
Input 42V, 20A
Balance current: 120mA

If you use these two, your board will **NEVER** balance because the balance current is lower than the cutoff of your brick.

---
Here's a different example:

Brick Charger,
42V 4A output
cutoff at 50mA

BMS
Input 42V, 20A
Balance current: 120mA

In this case, your BMS will do its job and balance your pack just fine. This is because the cutoff for your brick charger is lower than the balancing current.

It has nothing to do with the voltage of your brick charger, you can have a 60V charger, if the cutoff is higher than the BMS balance current then the BMS will **NEVER** do its job.
```

---
## \#97 Posted by: Eboosted Posted at: 2017-03-30T17:23:32.381Z Reads: 90

```
Thanks for taking the time to explain, would you share where to find the Lab Power Supply charger that that you use?

From the Battery Supports web, their 42V 60A BMS has 60mA and starts balancing at 3.90V

Technical Parameters:
Balanced current: 60mA (VCELL = 3.90V when)
Balanced for: 4.20 ± 0.05 V

So the charger should go lower than 60mA
```

---
## \#98 Posted by: PXSS Posted at: 2017-03-30T17:35:30.460Z Reads: 91

```
I have a brick charger from alibaba through a groupbuy, but yes, you got it now, your brick should charge all the way down to 60mA
```

---
## \#99 Posted by: Eboosted Posted at: 2017-03-30T18:04:34.454Z Reads: 93

```
Damn, it's really hard to find a brick charger like yours. Sellers do not usually state this info on the spec sheets.
```

---
## \#100 Posted by: Namasaki Posted at: 2017-03-30T21:07:30.933Z Reads: 94

```
I have a 5a brick charger from battery supports and it shuts off befor the pack is full.
```

---
## \#101 Posted by: Okami Posted at: 2017-03-30T21:12:29.979Z Reads: 98

```
Hah.. so do you suggest that you found a brick charger which brings the current low enough for the bms to allow to balance the cells?

I assume this brings us to the thing that regular supplies some people use are not really intended to be used along with low-current bms'es and more suitable variant (like psu with low current capability) are desirable.

I was thinking about this.. but it kind of is logical maybe, that these led light / regular psu's were not meant to be powered in such low-power state.. :D otherwise, maybe someone can come up with a solution how to fix this.. and trick the charger to allow the current to flow..

A ''parasite'' load (resistor) maybe, which gets turned on only when voltage is high enough?
```

---
## \#102 Posted by: Eboosted Posted at: 2017-03-30T21:23:36.245Z Reads: 93

```
@Namasaki Can you confirm what's the cut off current of this charger?

http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html

If the cutoff is more than 80mA then it'll turn itself off before balancing cycle starts.

@PXSS can you send us a picture of your brick charger label?
```

---
## \#103 Posted by: PXSS Posted at: 2017-03-30T21:26:30.500Z Reads: 90

```
I dont have it with me but it literally says 
"Power Charger
42V 5A"
And on top there was a sticker that said "36-42V 5A"
```

---
## \#104 Posted by: Eboosted Posted at: 2017-03-30T21:36:36.888Z Reads: 85

```
How do you know if the cutoff current is 50mA on your charger?
```

---
## \#105 Posted by: PXSS Posted at: 2017-03-30T21:41:33.750Z Reads: 83

```
I didn't. It just works. But based on what you've said I'm certain that that is your issue. You have a cc charger and not a cc/cv. I specifically looked for a cc/cv charger. That might help
```

---
## \#106 Posted by: Namasaki Posted at: 2017-03-31T03:20:28.455Z Reads: 84

```
[quote="Eboosted, post:102, topic:19302"]
Can you confirm what's the cut off current of this charger?

http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html

If the cutoff is more than 80mA then it'll turn itself off before balancing cycle starts
[/quote]

There is nothing in the product description about cutoff current.  In fact in the product description, it says 
 5amp constant current process and it does not mention a constant voltage process.
I looked at the charger I got from Battery Supports and there is nothing on the label concerning cutoff current
```

---
## \#107 Posted by: Namasaki Posted at: 2017-03-31T03:26:53.826Z Reads: 93

```
So, I got the board that I'm test charging down from 39v to 37.1 after a 3 1/2 mile ride.
I popped the lid and checked each cell for balance and this is what I found.
1.  3.712
2.  3.713
3.  3.711
4.  3.719
5.  3.716
6.  3.711
7.  3.713
8.  3.718
9.  3.713
10. 3.709
This is with discharging through the bms and includes some  Regenitive braking.

I am recharging now with the Korad power supply
currently, my battery is at 38.6v and the power supply is in CC mode outputting 39.24v at 5a.
the voltage will increase as the battery's voltage increases until it reaches 42v at which time it will automatically switch to CV mode holding at 42v with the current steadily decreasing until the battery is fully charged.
Charging with this power supply is like using a "Smart Charger"
```

---
## \#108 Posted by: jmasta Posted at: 2017-03-31T04:19:42.964Z Reads: 93

```
My setup uses 12S lipos with a 60A BMS.  I have never had a problem with them coming out of balance; throughout charging/discharging they are always within 0.01-0.02V of each other.  I typically only charge to 48V (4.0V/cell) and discharge to around 45V (3.75V/cell), because this gets me around 12-13 miles.  _Note that when I charge to only 48V, the BMS balancing never actually occurs, but my cells always seem to end up balanced anyway_

However today I wanted to test the lower voltage performance. I started at storage voltage of **3.85V/cell ± 0.1V** and rode it to an (unexpected) cutoff.  I thought I had plenty of life left, but suddenly everything cut out as I went to pass a cyclist uphill.  Everything was dead, including the LEDs and voltage meters, which indicated it was BMS low voltage cutoff, not a VESC cutoff

I measured all the cells and found a huge voltage difference of 0.60V between the highest and lowest cell. Keep in mind they were within 0.01V at the start

1) 3.60
2) 3.45
3) 3.20 !!
4) **3.03** !!!
5) 3.40
6) 3.46
7) 3.63
8) 3.56
9) 3.48
10) 3.28 !!
11) 3.34 !
12) 3.45

So the BMS cut the power because cell #4 dropped below its 2.9V threshold during the high current load.  My VESC cutoff was set to 37.2V  (3.1V/cell) when the pack cut out at 41V

I charged at 45.8V with a 5A CC/CV charger.  The voltage jumped up quickly from 41V to 44V and then slowly increased until the set voltage. Once it reached 45.8V, it continued charging for some time until cutting off.

**But here's the interesting thing....** the pack rebalanced itself.. seemingly without help from the BMS.  I intentionally chose an end-of-charge voltage that was lower than the BMS balancing threshold. Yet the cells ended up nearly perfectly balanced, even though they were very uneven  beforehand

1) 3.82
2) 3.81
3) 3.80
4) 3.80
5) 3.80
6) 3.80
7) 3.80
8) 3.81
9) 3.81
10) 3.80
11) 3.80
12) 3.80

I don't know why the cells became so unbalanced after discharging past 3.7V/cell?
 Nor do I know why they rebalanced themselves..?
```

---
## \#109 Posted by: PXSS Posted at: 2017-03-31T04:56:37.693Z Reads: 87

```
Cool experiment,
Do you have means to measure the internal resistance of your cells?
It could be that the internal resistance is higher on some cells than others.
In this case that would be cell 4, that is why it charges and discharges faster.
This means that cell 4 has less capacity than your other cells. by keeping them in the 75-40% region you probably don't see much of the effect, but once you go underneath this then it all goes crazy.
Take this with a grain of salt as this is mostly me making an educated guess
```

---
## \#110 Posted by: Eboosted Posted at: 2017-03-31T05:14:18.223Z Reads: 89

```
Check your nickel strips, one cell of pack 4 could have been detached.

That's another example of bms not balancing at discharging, or maybe balancing only at low current,  good for low discharge rate as in cruising. 

@jmasta I'm extremely interested in runing a test that would change the idea of BMSs forever. If you won't be able to do it I'll do it anyways as soon as I receive my Korad power supply in two weeks. 

The test would consist in charging a set of unbalanced packs with and without BMS intervention, wiring alteration would be necessary for the test, the used charger would be a cc/cv one. 

If the pack is balanced wether you use BMS or not then, I'll be irrelevant to use bms for charging.
```

---
## \#111 Posted by: Namasaki Posted at: 2017-03-31T05:51:52.900Z Reads: 90

```
<img src="/uploads/db1493/original/3X/e/d/eda6a2652106e48adc37ad8a56710592f9939de6.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/f/6f6bc57741f18757d5fa6965b4bd9b8e6d29a5df.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/3X/2/2/22f14513d2a71023b79a0542f76243ab6688603f.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/0/10c662436c839a1294f0444892c0d90c8c9bede8.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/3X/4/3/438fac8299e734ba3636a313dc857a5fff2d4a98.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/e/0e89c4950f6d5c42e14682816fd2ee8dcc607f6a.jpeg" width="375" height="500">
```

---
## \#112 Posted by: jmasta Posted at: 2017-03-31T06:00:07.995Z Reads: 86

```
Yeah  @PXSS I think you're right about the internal resistance.  My 6S balance charger can measure the per-cell IR, but I would need to get to the original 3S balance leads to get an accurate measurement. They are pretty hidden away, so I'll measure them the next time I take everything apart.

In the meantime I want to repeat this test, but pay more attention to the individual cell voltages throughout discharge. I need to find out when it starts getting crazy, and also to see if cell 4 will do this consistently

(BTW, that adjustable charger you found from China is awesome!)[quote="Eboosted, post:110, topic:19302"]


@jmasta I'm extremely interested in runing a test that would change the idea of BMSs forever. If you won't be able to do it I'll do it anyways as soon as I receive my Korad power supply in two weeks. 

The test would consist in charging a set of unbalanced packs with and without BMS intervention, wiring alteration would be necessary for the test, the used charger would be a cc/cv one. 

If the pack is balanced wether you use BMS or not then, I'll be irrelevant to use bms for charging.
[/quote]

I wouldn't be able to do that test without rewiring my system. I intentionally wired it so the BMS must be installed for the DC charge port to be active.  (The negative charge terminal is on the P- output from the BMS)

However if anything, I think this further validates the need for a BMS.  Without one, I might have never known that one cell was dropping so fast.  If I had ridden to my VESC programmed cutoff, that cell could have been damaged.  Now imagine if you (unknowingly) did this every cycle
```

---
## \#113 Posted by: Eboosted Posted at: 2017-03-31T06:33:41.304Z Reads: 80

```
That's a good point. 

I wonder what went wrong during discharge
```

---
## \#114 Posted by: jmasta Posted at: 2017-03-31T07:17:29.184Z Reads: 81

```
I think it's largely due to the nature of LiPos.  I've never actually taken these batteries below nominal voltage (44.4V or 3.7V/cell) before today, so I can't say for sure without more testing

LiPos initially drop fast, then have very flat discharge line, and drop exponentially at the end (the dreaded lipo cliff).  So small differences in resistance could have a large effect on the end voltage/capacity of each cell.  Plus I am only running 12S1P, so each cell is on its own

Li-ion in general have a much more linear discharge curve, which I would suspect is more stable.  In addition, you guys often have 3 or more cells in parallel. The parallel groups help balance out small differences among the cells.  This is probably why li-ion packs can discharge to ~2.9V, whereas I need to cutoff my lipos at 3.4V

I hit the BMS voltage limit before the current throttling ever kicked in.  That would have helped reduce voltage sag going up the hill, and I might have gotten more range before cutoff
```

---
## \#115 Posted by: PXSS Posted at: 2017-03-31T12:04:21.117Z Reads: 85

```
Yeah for LiPos that makes total sense! I missed that part when I read your post last night. I thought you were using liions. 

Lipos have about 10% remaining after 3.5V and yes, the internal resistance has a big effect on how fast they drop off after. Whenever we buy LiPos we request the manufacturer to send us matched cells so we never fly packs with unmatched cells. We buy Lipos from thunderpower though and they are a bit pricey. 

Liions hit the cliff at ~3.1V but that by itself is more tame than the lipo cliff, also using quality cells from the same batch usually means a lower spread in internal resistance and lastly we use several cells in parallel which helps out average the internal resistance in case there is a weak cell.
```

---
## \#116 Posted by: Namasaki Posted at: 2017-03-31T22:34:34.151Z Reads: 89

```
Ok, so I charged my battery last night until the power supply output was down to around 50ma and the voltage meter on my board showed 42v, then immediately shut off and disconnected he bms to check cell voltages.
1.  4.198
2.  4.202
3.  4.204
4.  4.205
5.  4.204
6.  4.205
7.  4.204
8.  4.205
9.  4.204
0.  4.205
So then I plugged the bms back in and went to bed.
Today when I got home from work, I turned the bms on for a few minutes and the total pack voltage was at 41.9v
I turned the bms off and disconnected it to check cell voltages again and:
1. 4.195
2. 4.195
3. 4.200
4. 4.200
5. 4.200
6. 4.200
7. 4.200
8. 4.200
9. 4.200
0. 4.200
So it appears that the bms with its low balancing current needs ample time to balance the pack once its fully charged.
I would have liked to leave it on the charger longer to see if it would balance while charging the low cells but it got too late and I work the early shift.
It also appears that one of my packs may be a little slow though 5ma difference isn't bad Imo.
I have it back on the charger now receiving 42v at currently 50ma to see if the low cells will balance up and wondering if the 4.2v cells will hold. I will update on that later.
**Update:**
So I left the pack on trickle charge (50ma) for about 2 hours and now the low cells (1and2) are at a full 4.2v
And now it's time to go ride...
P.S. I think the extra 2 hours of trickle charge is totally unnecessary. 
Simply charging down to 50ma the first time would have been plenty good enough.
```

---
## \#117 Posted by: jmasta Posted at: 2017-03-31T22:58:18.756Z Reads: 82

```
How are you measuring those?  0.005V is likely within the acceptable error of your meter

Those are perfectly balanced as far as I'm concerned. 4.200 ± 0.005V all around
```

---
## \#118 Posted by: Namasaki Posted at: 2017-03-31T23:00:54.368Z Reads: 86

```
Checked cells with this:
<img src="/uploads/db1493/original/3X/4/6/46fcca1336d262c7513685d67b7f8d6e5543bf34.jpeg" width="375" height="500">
```

---
## \#119 Posted by: Eboosted Posted at: 2017-04-01T03:04:24.497Z Reads: 90

```
Wow that's a great finding! 

I don't understand what you mean by "then I plugged the BMS back and went to bed" 

Were you charging with no BMS at the begining? Did you change the wiring and connected the BMS back in? I'm not following... Unplugging a BMS is not easy at all as you need to solder wiring

Did you measure the cell voltages before begining the charge cycle?
```

---
## \#120 Posted by: Namasaki Posted at: 2017-04-01T04:52:29.044Z Reads: 92

```
Check out my Lipo battery build, you will see that I have quick disconects on my balance wires for each 2s pack.
The bms was connected while charging then I disconnected the balance wires so I could easily check individual cell voltages.
Then I reconnected the balance wires and went to bed, it was late and I work the early shift.
The next day the cells where all balanced. I guess the bms was balancing them even though it was turned off.
I did measure the cell voltages before the charge cycle. those results where in an earlier post.
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#121 Posted by: Eboosted Posted at: 2017-04-05T07:07:37.408Z Reads: 98

```
I went for a long ridde tonight anfd I ran my board with my unbalanced pack until it reached cutoff start voltage which is 30V

Before the ride, this were the voltages of each pack:

1) 4.16
2) 4.10 
3) 4.09 
4) 4.16 
5) 3.75 
6) 4.08 
7) 4.12 
8) 4.16 
9) 4.10 
10) 4.18 

As you can see the pack #5 was unbalanced way below the others, unfortunately I don't have any way to balance that pack until I receive my Korad power supply in 20 days. Nevetheless, I went and made the test even though I knew pack #5 had high risk of getting below 2.8v

After going all the way down to 17% SoC, I felt a big drop in power, I knew I had reached cutoff start 30V (VESC Setting), so I stopped and went home. After checking the log I saw I had gone from 33.8V until 28.5V of battery because of battery sag, I knew I had gone too far and the pack #5 could have suffered a low voltage hit.

[img]http://i.imgur.com/OTLTmrX.jpg[/img]

So, I opened up the enclosure to meassure voltage for each pack and found out the pack #5 had 1.74v (sh!t) the other nines were 3.5v.

1) 3.56 
2) 3.53 
3) 3.53 
4) 3.56 
5) 1.74 (probable cell damage)
6) 3.53 
7) 3.55 
8) 3.57 
9) 3.54 
10) 3.57 

Pack five was signifcally hotter than the rest.

I connected my brick charger (that's the only one I currently have) and waited to see what happened. To my surprise, pack #5 started to charge pretty quick, faster than the rest, and recovered in less than 10 minutes from 1.74 to 3.3v, the temperature of the pack lowered and evened at the same temperature of the other packs, at this point I don't know if the cells from pack #5 are damaged or not.

[img]http://i.imgur.com/kmLkWUO.jpg[/img]

I'm still charging at the moment, currently at 90% SoC but cell #5 still has a lower charge than the rest, the initial fast charging of pack 5 stopped at 30% and continued at the same level as the rest.

[img]http://i.imgur.com/sIM3bNt.png[/img]

As you can see pack #5 won't reach 4.2v, it never did from day one.

My mistake was to not balance all packs before mounting the battery with nickel strips from the beggining, I though the BMS could take care of it but I was mistaken. I'm hopping I could fix it with my Korad charger otherwise if you have a better solution to balance the pack I'm open to ideas.

[img]https://images-na.ssl-images-amazon.com/images/I/61yW93AMmsL._SL1000_.jpg[/img]

If I had the pack disassembled I could use the parallelling method described [here](http://liionbms.com/php/wp_parallel_balance.php), unfortunately the pack has already being soldered, so I'm looking for an alternate method.
```

---
## \#122 Posted by: chuttney1 Posted at: 2017-04-05T07:41:51.268Z Reads: 86

```
Keep close watch on pack #5.
```

---
## \#123 Posted by: PXSS Posted at: 2017-04-06T09:51:31.412Z Reads: 80

```
Keep messing with it like that and sooner rather than later you'll find yourself with a board on fire...
```

---
## \#124 Posted by: Eboostin Posted at: 2017-04-06T14:06:20.312Z Reads: 79

```
Has anyone tried charging or discharging on the individual balance leads to bring out of balance cells back in?

I haven't had any issues with my packs but perhaps an option
```

---
## \#125 Posted by: Eboosted Posted at: 2017-04-06T16:51:24.047Z Reads: 84

```
[quote="Eboostin, post:124, topic:19302"]
Has anyone tried charging or discharging on the individual balance leads to bring out of balance cells back in?
[/quote]

That would be a good idea, but I guess you will need a 4.2v charger to balance the out of balance pack which I don't have ATM.

I have these options:

1. Disassemble the pack and use the parallelling method to get all them balanced, assemble them back again.
2. Disassemble the pack and discharge the cells untill I get them atthe same SoC
3. Wait until I get the Korad power supply

@PXSS I'm trying to fix this problem, I'm not sure how a cell with low capacity could potencialy lit my board on fire.
```

---
## \#126 Posted by: jmasta Posted at: 2017-04-06T19:42:39.732Z Reads: 79

```
You could just make a simple discharge device to manually bring down the voltage of each cell.  Basically you'd just attach a resistive load to the (+) and (-) terminals of one cell.

For a voltage range of 4.2V to 3.7V, a **2 Ohm resistor** would give you about **2A discharge**

The maximum power dissipated would be about **8.8W**.  Therefore you'd need to buy high wattage resistor, sometimes called a power resistor.  10W would do. 20W resistor would be better.  

Something like this 20W resistor would work:  
https://www.amazon.com/20W-Cement-Resistor-TOOGOO-Resistors/dp/B01GKWDTW2/ref=sr_1_2?ie=UTF8&qid=1491507211&sr=8-2&keywords=2+ohm+20w+resistor


Or on Amazon Prime for USA guys:  https://www.amazon.com/uxcell-Wire-Wound-Cement-Resistors/dp/B0087ZDDOU




<img src="/uploads/db1493/original/3X/0/f/0f9465748bb7029686671bb92edd39f23e6b2d29.jpg" width="332" height="500">

The pins could just be breadboard jumpers. You would unplug your balance plug from the BMS, and then stick your two discharger terminals into two adjacent pins on the JST plug (corresponding to the cell you're trying to discharge).  Check the cell voltage with the DVM.  Then activate the switch to apply a ~2A load to the 20W (2 Ohm) resistor.  Continue draining the cell until it matches the voltage of your lowest cell (cell 5 for you @Eboosted). Turn off the switch to see resting voltage. Keep toggling back and forth until the resting voltages match.

Then do this for every cell, bringing down the voltage of each cell individually until they match your lagging cell.  If done correctly, you've just manually balanced your pack without disassembling it. Your BMS should now be able to balance them since they are all roughly the same voltage

Note:  Would be a good idea to include a **fuse** as well!!
```

---
## \#127 Posted by: PXSS Posted at: 2017-04-06T19:52:19.533Z Reads: 74

```
Charging a cell that has been over-discharged has higher chances of exploding or as manufacturers call it "venting flaming gases". Manufacturers recommend any cell that has been discharged under 1.5V is disposed of. Who knows how many cycles you've over discharged your cells by now. You are playing with fire. Be careful
```

---
## \#128 Posted by: Namasaki Posted at: 2017-04-13T22:45:01.757Z Reads: 75

```
Did you get your power supply yet?
I just tried to charge one of my boards with my Battery Supports 5a charger and when the battery got to 41.5v the charger switched to green light.
So I disconnected that charger and plugged my power supply into the board and it resumed charging with 42v 3a output in CV mode.
After about 10 min the power supply output is down to around 500ma and the battery is at 41.9 and still charging.
About 1/2 hour later
Now the output is at 53ma and battery is showing 42v
I usually stop when the output drops to around 50ma
```

---
## \#129 Posted by: jmasta Posted at: 2017-04-13T23:21:58.475Z Reads: 77

```
I found that my 12S adjustable charger "cuts off" at around 0.48A (480mA).  The light turns green, and the fan stops.  However **it is not done charging**.  It will continue supplying <0.5A current until reaching the set voltage.  The current slowly drops off from ~450mA to 6mA over about 20 minutes, resulting in an additional ~5Wh.   The battery pack then reaches within 0.01V of the no-load supply voltage
```

---
## \#130 Posted by: Eboosted Posted at: 2017-04-14T00:36:55.046Z Reads: 74

```
No. I'm still waiting for it, it might be here next weekend, so testing will have to wait a little bit.

I balanced the cells manually, lowering the higher packs until I reached the voltage of the lowest voltage pack, I used 4 parallel 12V car light bulbs connected from needles on the leads of the balancing plug.

[img]http://i.imgur.com/Y5WvCnS.jpg?1[/img]
[img]http://i.imgur.com/C9ydGz5.jpg[/img]

You can lower three consecutive packs at 12V, so the balancing process gets way faster.

[img]http://i.imgur.com/RYbfGCt.jpg[/img]
```

---
## \#131 Posted by: Eboosted Posted at: 2017-04-14T00:39:22.065Z Reads: 70

```
[quote="jmasta, post:129, topic:19302"]
I found that my 12S adjustable charger "cuts off" at around 0.48A (480mA).  The light turns green, and the fan stops.
[/quote]

Would you mind posting  picture of your charger?
```

---
## \#132 Posted by: Eboosted Posted at: 2017-04-14T00:42:39.391Z Reads: 73

```
@Namasaki if your charger stops at 41.5v I'm very convinced you have an unbalanced pack, one of them has 41.9v or 42.00v and BMS cuts the charging process leaving unbalanced cells semi empty, even though the full pack has not reached 42.00v.

You might be correcting the balancing with your lab power supply as you used it later that time.
```

---
## \#133 Posted by: jmasta Posted at: 2017-04-14T00:51:41.018Z Reads: 73

```
<img src="/uploads/db1493/original/3X/0/7/0727d943f5c82ff38c005b034c20aecc5c3dcb33.JPG" width="666" height="500">

Power meter was not included, but I'd highly recommend one (especially if you use an adjustable charger)

Notice the green light, while it is outputting 400mA
```

---
## \#134 Posted by: Eboosted Posted at: 2017-04-14T01:13:04.691Z Reads: 70

```
Would you share where did you get it?
```

---
## \#135 Posted by: jmasta Posted at: 2017-04-14T01:44:22.889Z Reads: 66

```
Somewhere in China from @PXSS 's group buy. There were 10S and 12S versions. It has a knob on the side to adjust the voltage; so for example, I can easily set it to storage voltage, max voltage, or anywhere in between. I usually only need to charge to 4.00V/cell
```

---
## \#136 Posted by: PXSS Posted at: 2017-04-14T01:45:04.917Z Reads: 67

```
Somewhere in China is accurate lol :joy:
```

---
## \#137 Posted by: Eboosted Posted at: 2017-04-14T02:19:19.770Z Reads: 67

```
You should do a new GB @PXSS
```

---
## \#138 Posted by: Namasaki Posted at: 2017-04-14T04:59:06.216Z Reads: 71

```
[quote="Eboosted, post:132, topic:19302"]
if your charger stops at 41.5v I'm very convinced you have an unbalanced pack, one of them has 41.9v or 42.00v and BMS cuts the charging process leaving unbalanced cells semi empty, even though the full pack has not reached 42.00v.
[/quote]

I don't think that it's the bms stopping the charger. I think the detection circuit in the charger is stopping the charger.
I Think if the bms was stopping the charge process, it would stop the power supply as well.
But, to be honest, I am just speculating at this point. I am sure of one thing. The power supply gave me a full charge and a friend and I went on a very long skate and my battery still had around 38v when we where done.
I know, very long skate means nothing. Sorry I couldn't get a good Satellite signal to track the ride.
```

---
## \#139 Posted by: PXSS Posted at: 2017-04-14T05:44:43.483Z Reads: 71

```
@Eboosted
You really need to fix your welding before we can help determine what if anything is wrong with your BMS/charger combo. I think all of your problems come from bad welds within your pack.

@Namasaki is correct. Your charger is stopping itself, not the BMS
```

---
## \#140 Posted by: Eboosted Posted at: 2017-04-14T17:56:21.935Z Reads: 73

```
After I manually balanced the pack of my Reaper it has been running perfect, battery goes all the way up to 42.1v consistently, yesterday I rode it and these were voltages:

1) 4.00
2) 4.00
3) 4.00
4) 4.00
5) 3.99
6) 4.00
7) 4.00
8) 3.99
9) 4.00
10) 4.00

I have a second build on a Loaded Vanguard with 10S4P, on that one I was getting ABS over current fault when I pulled the throttle from a dead stop, however during the last two days, I've not gotten that fault anymore.

Following @PXSS advice I pulled out the battery enclosure to check bad solder joints but all those were perfect, no bad welds at all, however unlike the Reaper this one has some sag even testing on the bench, just for a split second, it goes from 42v to 40.5v on full bench throttle, maybe it's because I have a faster (higher sample rate) battery tester, but I don't remember this sag when I first build it, hopefully this sag it's perfectly normal or maybe the bullet connectors connecting each pack are not a very good idea, I'm not sure though, what do you guys think?

[img]http://i.imgur.com/P0fSVWy.jpg[/img]

Another test I did was to check at what voltage the brick charger stopped charging. As soon as it got 41.4v charger stopped, I check the voltage of each pack and got these:

1	41.4
2	41.3
3	41.3
4	41.3
5	41.3
6	41.3
7	41.3
8	41.3
9	41.3
10	41.3

So, my assumptions from unbalanced pack on @Namasaki battery were wrong, the logic of the charger just works that way.

As soon as I receive my lab power supply I'll do all kind of tests and will start charging my batteries at 40v and 42v only for ocassional long trips.

If you guys find a brick charger with adjustable cutoff end please post the link.
```

---
## \#141 Posted by: PXSS Posted at: 2017-04-14T17:59:48.692Z Reads: 67

```
[quote="Eboosted, post:140, topic:19302"]
unlike the Reaper this one has some sag even testing on the bench, just for a split second, it goes from 42v to 40.5v on full bench throttle, maybe it's because I have a faster (higher sample rate) battery tester, but I don't remember this sag when I first build it, hopefully this sag it's perfectly normal or maybe the bullet connectors connecting each pack are not a very good idea, I'm not sure though, what do you guys think?
[/quote]

You were running 35A through it, so yeah, that is normal.

[quote="Eboosted, post:140, topic:19302"]
Another test I did was to check at what voltage the brick charger stopped charging. As soon as it got 41.4v charger stopped
[/quote]
Are you 100% it stopped? do you have a wattmeter to measure the power/current flow?
```

---
## \#142 Posted by: Eboosted Posted at: 2017-04-14T18:07:11.116Z Reads: 69

```
Thanks man, if you see the bench braking it seem I'm pushing too much current back to the battery, I'm affraid this could be causing cell damage.

Even on the bench under no-load braking I'm getting an high increase of input voltage until 43.3v

[img]http://i.imgur.com/KmkP8Al.jpg[/img]

Should I lower battery min?, I still need more braking force at high speeds and less at low speeds (belt slippage before dead stop)
```

---
## \#143 Posted by: PXSS Posted at: 2017-04-14T18:28:53.148Z Reads: 66

```
You're still bypassing the BMS? If so then yeah. You are damaging the cells
```

---
## \#144 Posted by: Eboosted Posted at: 2017-04-14T18:30:47.579Z Reads: 67

```
I'm begining to charge at 40V from now on, cant wait for my power supply.
```

---
## \#145 Posted by: PXSS Posted at: 2017-04-14T18:52:31.450Z Reads: 71

```
That's not going to help if your cells go out of balance...
Why don't you just dicharge through the BMS and avoid all of this???
```

---
## \#146 Posted by: Eboosted Posted at: 2017-04-14T19:45:05.835Z Reads: 68

```
On that builld I don't have BMS, just a small 10A BMS I'm currently using for charging.

I'm going to buy a couple of Bestech BMS next month though

I'm keeping close monitor on the cells to check if they go out of balance, so I could rely on VESC battery cut off sart and cutoff end.

On the other hand, as you might know, I had very bad experience with Battery Supports BMS when it cutted out regenerative current back to a full charged battery causing a sudden increase in current flowing through the VESC causing a reboot, hence loosing brakes on unexpected situations, I rather have less charge cycles than loosing brakes on a crossing after a downhill.

I have three options to fix thi:

1. A lab power supply adjusted to charge only until 40v, should increase battery life cycles, should avoid the BMS issue and will help me balance empty cells on every charge cycle.

2. A brick charger with adjustable cut off end voltage and continuous cell balance monitoring

3. A Bestech BMS which hopefuly won't have the Battery Supports issue in conjuction with the current brick chargers I'm using at the moment. On this matter I'm relying on forum members experience only
```

---
