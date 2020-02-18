# Balance charger vs BMS for 12S5P Lithium Ion pack

### Replies: 64 Views: 10598

## \#1 Posted by: radium Posted at: 2017-01-13T19:29:45.050Z Reads: 515

```
Hey guys, so I'm in the process of of soldering up my 12S5P pack made up of 18650 batteries.

I've read that BMSes don't actually work very well for balancing over time since the resistors they use to create drain are so small. I've also read that they frequently burn out and you have no way of knowing without periodically testing your pack to see if it is balanced.

Do any of you guys use a balance charger for a 12S battery pack? If so could you recommend one? Are my BMS concerns unfounded? What BMS do you guys recommend, I'm not worried about the price of the BMS, the battery is one of the most expensive parts of this board as well as the most dangerous and I'd rather protect it well.

Another question I have is, do you think it is necessary to monitor voltage on each of the 12 parallel packs or is it sufficient to just monitor the voltage of the pack as a whole if I'm not draining it close to the cut off voltage.

I will probably only drain it to around 39.2 volts which is 3.3V per pack.
```

---
## \#2 Posted by: OskarCastrone Posted at: 2017-01-13T19:53:11.465Z Reads: 483

```
Your battery seems awesome! That will be BIG battery! :-) 
I cannot advise you which BMS to choose. Neither can I tell you if BMS's is safe.
All I can tell is, that using a balance charger is not as nice/easy/cool as charging through the BMS with a laptop style charger. I think that the convenience of BMS's charging oppurtunities is enough reason to use them. Especially if you are charging a 12s battery. 
Balance chargers for 12s batteries are expensive! Of course you could charge the battery as 2 6s batteries, but that makes the whole charging process even more inconvenient... 
I hope that helps
```

---
## \#3 Posted by: radium Posted at: 2017-01-13T19:56:20.179Z Reads: 479

```
Yeah that is what I'm noticing looking around. The 12S balance chargers are really expensive. It is a big battery, I was contemplating doing 12S4P but it's too late now :smile:. My board is big, and I've yet to make the enclosure but it should all fit.
```

---
## \#4 Posted by: radium Posted at: 2017-01-14T01:17:53.520Z Reads: 458

```
Do you have any advice on a decent laptop style charger for a standard 12S BMS? I've found one that looks good. It's rated up to 80A continuous and my battery is going to be 75A continuous max.
```

---
## \#5 Posted by: Okami Posted at: 2017-01-14T02:14:17.471Z Reads: 456

```
I can only recommend ''meanwell'' chargers. Though You should get one with adjustabale voltage. Im not sure was it as easy to get it for 12s but you might still look in the forum..

Which rating of charger you took? 80A might be 80W.. which would be quite weak for your battery setup! I would advise to get about 150-200w charger.. You probably will want to charge at around 5A, so ~50V x 5A = 250W

How much capacity will your pack have? I would advise that you can get a charger that is able to charge at half amps of your battery's capacity.. this way you wont need to wait more than a couple of hours till it finishes charging.. More like 2h for 0.5c charge rate..

So if you got 12.5Ah pack (2.5ah x 5), you might want to get about 6A capable charger. This way, if pack is really depleted it should be able to fully charge it in about 2 hours.. If you get a charger which is capable of only 2A, then you might need even 6hours for fully depleted pack. 4A might be your best shot! (~3h charge time)

Though you can dismiss my advice as Im interested in being able to charge batteries fast.. It might also not be that good, since you probably will need a bms which is capable of such high charge rate and not always you might want to charge the batteries that fast..

--

There is this ''Raphael Chang'' bms.. if you are willing to shell out more than 100usd for sophisticated / user configurable bms, it might be the best on you can get.. though it is still experimental and the first beta units will be only sent out in the coming weeks.. 

You can check it but it might be a ''heavy read'' if you are new to battery stuff.
```

---
## \#6 Posted by: radium Posted at: 2017-01-18T01:17:27.825Z Reads: 390

```
The capacity will be 15AH, 3000mAh x 5. Capable of 75A continuous discharge. From what I can see there are BMS capable of 80A discharge 10A charge for around $80-$100USD. The main issue with fast charging that I can think of is the ability of the BMS to apply drain to the parallel packs decreases as the charging amperage increases due to the small resistors. They seem to decrease the available current by something like 5mA-50mA, so if you're charging at 2000mA that is a bigger difference than charging at 10000mA.

That is why I wanted a charger rather than a BMS. They have much greater capability to vary the charging current (and that's why they require fans to stay cool, they dissipate the energy off as heat).
```

---
## \#7 Posted by: PXSS Posted at: 2017-01-18T02:37:17.851Z Reads: 371

```
I am against meanwell power supplies/chargers.
We have gone through 5 at work. Unless you have them on a UPS they will blow in a few months. 

We originally bought 2 and they both blew, we got them replaced through warranty and they both blew after a few months, got them replaced again and placed them on battery UPS and surge protectors, they survived for a year or so until one of our interns decided to plug one in straight to the wall and it blew after 15 minutes. 

So yeah. Don't go with meanwell if you can avoid it imo
```

---
## \#8 Posted by: Okami Posted at: 2017-01-18T06:46:39.000Z Reads: 361

```
I've heard of using ups units + voltage booster "modules"' How well does this combination work? @PXSS 

I heard this idea from electric bike builders as they.need chargers in 1kw+ range.and I believe some of these server.ups' units were rated at about 1.5kw

---

@radium in your case I might consider going with dual 20A version of Turnigy reaktors. Wont be as nice as "integrated" bulk charging with bms but charging speed might be really sufficient. Of course u will also need beefy psu for this charger..

https://hobbyking.com/en_us/turnigy-reaktor-2-x-300w-20a-balance-charger.html
350ma balancing current capable
Charging 2x6s 15 000mah, at 7.5A or so, should probably yield 2+ hours charge time. 

Actually from this it looks like you could go with 10A version but you have to check the specs then.. Also consider fan noise might be an issue when charging at higher amps.. I cannot actually be in the same room sometimes when my little 80w turnigy charger kick in its noisy fan.

----
 As for.bms - wont be able to recommend much else. I would perhaps.look at charge.only.bms to drive the.cost.down./ improve other.areas of it. But if u think.u.need.discharge.side.bms that"s fine
```

---
## \#9 Posted by: OskarCastrone Posted at: 2017-01-18T23:26:47.643Z Reads: 336

```
I suggest that you contact bestech.com. They sell a lot of different BMS units. To buy from them you have to contact them. You need to buy at least two units but if you ask politely for a sample you might be able to buy a single. 
And yes, you dont need the discharge capabilities if you are using the VESC since you can limit the amps there instead. 
I have not yet got a problem with a laptop style power supply though... You may also be able to buy your power supply through bestech.
```

---
## \#10 Posted by: radium Posted at: 2017-01-19T19:47:57.286Z Reads: 321

```
Has anyone ever thought of installing a small balance charger in their board to act as a BMS for charging? https://hobbyking.com/en_us/turnigy-b6-compact-50w-5a-automatic-balance-charger-2-6s-lipoly.html 

That charger is quite small and has drain capability of 200mA per cell which is quite a bit more than what I've seen from any of the other lithium BMS I've seen around. But if installed on the board it would provide the convenience of laptop style charging. I would need two for my setup and I think I'm just going to electrically split my cells with a loop key that keeps them in series for operation and parallel for charging so I can use 2x 6S chargers for my 12S cell. I will probably use external chargers though.
```

---
## \#11 Posted by: Okami Posted at: 2017-01-19T20:06:29.497Z Reads: 303

```
I actually considered doing the same awhile ago!

They are quite small and can be fitted onto the board!

Though, for faster charging I would actually consider mounting 2 of these, if the space allows it!

Otherwise you will probably need to leave your board for quite a while, till it finishes charging!

Great, if you are visiting someone and just have to keep it somewhere for more than a couple hours to fully charge!

----
**Some charging time speculation / calculations**

At ~2A and 6s, it looks like you would need something like 7+ hours to charge your battery, if it was really empty..

So, in an hour you would get approx 2 Ah, so the minimum would probably be to charge about 2-3 hours before the next ride.. 

Half that with two chargers :)
```

---
## \#12 Posted by: jmasta Posted at: 2017-01-20T00:42:39.980Z Reads: 284

```
If you're going to buy two of those at $15/ea plus shipping, just get a 12S BMS.  It won't be much more expensive.

Then you can skip the series/parallel loop key
```

---
## \#13 Posted by: radium Posted at: 2017-01-20T00:54:58.020Z Reads: 282

```
jmasta the problem with BMS is that they're shit and you have no way to know when they're working or not without checking your cells are in balance. The tiny resistors they use on them only apply like 5mA-50mA of drain tops. That's almost nothing when you're charging at say 5,000mA a pack.

With 5P in each pack that's only 1A per battery. So let's say the BMS is capable of applying drain at 50mA(which I doubt it is), that's 1% relative to the charging amperage. If your batteries are unbalanced by more than 1%, the BMS is going to require more than 1 cycle to re balance them. Heaven forbid they're more like 10% out of balance that's 10 charging cycles to re balance your pack.

In the meantime, assuming your BMS is working it will prevent the depleted pack from being excessively drained by shutting your battery down when that pack reaches 0%, but you'll still have capacity sitting in the rest of the pack.

A lot of people one this forum seem to be wiring their BMS so that it is active only during charging and not discharging though. In that case the BMS wouldn't even prevent that one pack from being discharged excessively.

That's why I'm going to use a cell logger as well as balance chargers instead of a BMS.
```

---
## \#14 Posted by: jmasta Posted at: 2017-01-20T01:00:26.454Z Reads: 261

```
Cool. Just trying to help out

I have cell voltage monitors built into my deck, so that is not a problem for me.  One flip of a DPST switch and I can quickly check to see if they are balanced
```

---
## \#15 Posted by: Eboosted Posted at: 2017-03-29T05:30:53.075Z Reads: 241

```
@jmasta Wher did you get that cell voltage monitor?, I'm looking for one.
```

---
## \#16 Posted by: Eboosted Posted at: 2017-03-29T05:31:19.481Z Reads: 244

```
What balancer charger are you using?
```

---
## \#17 Posted by: radium Posted at: 2017-03-29T06:25:00.539Z Reads: 251

```
I'm using a Turnigy reaktor 2x 300w charger. It's 2 6S capable chargers off 1 power supply. I wound up breaking the pack into 2x 6S packs wired in series when the board is running. They can charge simultaneously with this charger which is nice.

I don't mind taking my enclosure off to charge, especially since the battery pack was the most expensive single component of the board. This way I know the pack is healthy and being charged correctly.

If you don't want to do 2x 6S packs or similar for anything above 6S, the only other reasonable option is to use a 12S BMS and laptop charger. 12S chargers do exist but they're insanely expensive.

I went with the reaktor 2x 300w solution because although it's slightly more expensive up front, I can use it to charge all my boards(building a second right now) and batteries. And since I had to buy at least 2 12S BMS from the source I found and they were almost $100 each after shipping it wasn't really that much more expensive.

The power supply I'm using to power the reaktor is just an old 1200W desktop power supply that I tuned to be appropriate for the reaktor. I just happened to have it laying around.

If anyone happens to be reading this, I seriously over specced my battery. I built a 12S 15Amp Hour pack. I don't really regret it, but I use maybe 50% charge on my longer rides. Unless you're commuting and need 25+ mile range I'd recommend a smaller battery :). I'd rather have a 12S 8Ah battery that weighed half as much for most rides and that's actually what I wind up using a lot, is 3x 4S Zippys. My riding style is still pretty conservative and I find myself coasting a lot.
```

---
## \#18 Posted by: Eboosted Posted at: 2017-03-29T06:30:39.087Z Reads: 238

```
I have a 10S4P 18650 Li-Ion battery, several packs are unbalanced even though I use BMS only for charging.

I'm looking for an adjustable charger to set the voltage to 41V and balance the whole pack but I have only found enormous/expensive chargers, I found no ajustable portable chargers at all.
```

---
## \#19 Posted by: radium Posted at: 2017-03-29T06:32:42.750Z Reads: 245

```
Your BMS might have fried. Do you have a multimeter? If it's working it should re-balance the pack over time. The resistors on the BMS are pretty small and can only apply a relatively small amount of drain to each pack. Your best bet might be to get another BMS and replace the one that's on there.

Or alternatively do what I did and break the pack into 2x 5S.
```

---
## \#20 Posted by: Eboosted Posted at: 2017-03-29T07:30:32.006Z Reads: 244

```
I used a second bms since I thought the one o had before was bad, but it was exactly the same. You need to use a variable charger with adjustable current to be able ti balance the pack.
```

---
## \#21 Posted by: willpark16 Posted at: 2017-03-30T01:34:25.929Z Reads: 240

```
That bms u used has had some bad reviews I was going to ask u how it was a while ago but forgot
```

---
## \#22 Posted by: Eboosted Posted at: 2017-03-30T05:18:06.173Z Reads: 236

```
I got the Battery Supports from Supower, everybody use but I had issues with it.

I didn't know you needed a professional power supply to be able to use the BMS to it's fullest capabilities, but if you buy a good power supply then why do you need a BMS in the first place?

If your cells are balanced on charging and you keep an eye on individual packs every once in a while then there's really no need for a BMS, I'm starting to understand @whitepony
```

---
## \#23 Posted by: willpark16 Posted at: 2017-03-30T05:36:55.393Z Reads: 228

```
My mistake thought it was a different one
```

---
## \#24 Posted by: radium Posted at: 2017-03-30T11:27:20.855Z Reads: 234

```
The BMS if it's working will balance the pack. It just takes many charge cycles because of how small the resistors on the BMS are.

The way I understand balance charging to work is:

You pump voltage through pack, if one of the series cells is charged higher than the others, you apply drain to that pack, via sensor wire or balance lead until the other packs catch up. BMS can only apply something like 50mA of drain because of how small its resistors are.

You can do the math. If you are charging at 1A current 50mA of drain is not a lot. You could try charging your pack using very very low current over a very long time to allow the rather poor balancing capabilities of the BMS a better chance.

Either way though, it will attempt to rebalance every charge cycle if BMS is working. It just may take 10+ cycles because of how slowly it applies drain.
```

---
## \#25 Posted by: Eboosted Posted at: 2017-03-30T14:56:21.032Z Reads: 222

```
After some testing and research I found out the BMS does not balance at all, because it never reaches the balancing stage with a regular brick charger. You need a 0-60V power supply to balance your cell or your BMS won't work at all for charging, it'll only balance through discharging
```

---
## \#26 Posted by: Eboostin Posted at: 2017-03-30T15:15:55.711Z Reads: 215

```
Why would you need 60V for 36V(42V) bms? 

I'm using a Supower(Battery Supports) BMS for charging and discharging without issue
```

---
## \#27 Posted by: Eboostin Posted at: 2017-03-30T15:17:13.547Z Reads: 212

```
It's also important to make sure the cells are all the same voltage before building a pack. I build mine into a 1S40P with nickel strip and magnets to make sure all the cells are exactly the same voltage then build out to 10S4P
```

---
## \#28 Posted by: Eboosted Posted at: 2017-03-30T16:19:49.612Z Reads: 214

```
The 0-60V power supply is mandatory to be able to balance any unbalanced individual packs, BMS if you use a brick charger it will not reach the balancing voltage which is higher that 42V. You will know your individual packs are unbalanced when the pack does not reach 100% or it has less than 42V and the led from the charger is green.
```

---
## \#29 Posted by: PXSS Posted at: 2017-03-30T16:35:16.569Z Reads: 216

```
Mandatory based on what?
You can't do blank statements like that without any proof. 

I am also using a batterysupports BMS with a brick charger and it balances just fine
```

---
## \#30 Posted by: Eboostin Posted at: 2017-03-30T17:04:21.299Z Reads: 217

```
How is that possible when the "Over-charged Protection: 4.2 ± 0.05 V."

It says that balancing starts at 3.9V per cell or 39V on a 10S pack. 

http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

Charging shuts off at 42.5V. If anything, with a 60V charger, you are trying to throw more voltage at an object that can't accept it. Isn't that why Boosted had issues with their BMS/batteries? They were using a higher voltage charger than pack voltage?
```

---
## \#31 Posted by: Eboosted Posted at: 2017-03-30T17:06:21.857Z Reads: 205

```
[quote="PXSS, post:29, topic:16050"]
what?You can't do blank statements like that without any proof. 

I am also using a batterysupport
[/quote]

The proof (maybe it's not good enough yet) comes from my own experience and from @Namasaki experience with brick chargers, I also tested several brick chargers and was never able to balance the packs, however when some packs got unbalanced he was able to balance them with a power supply.
```

---
## \#32 Posted by: radium Posted at: 2017-03-30T17:27:52.618Z Reads: 201

```
I'm not really sure what is going on exactly. But your experience with a BMS is similar with a lot of peoples. They don't work very well for balancing. I explained above why that is, but I'll do it in more detail here.

Imagine you charge your 12 Amp hour pack(12000mAh) at 12 amps. It takes 1 hour to charge.(just for example)

Now your BMS is capable of applying 50mAh of drain to each of your 10 packs simultaneously.

Lets say one series pack reaches 4.1v but another pack is at 4.0v if you consider full charge 4.2v and full discharge to be 3.0v then each .1v is 1/12th of the charge state right?

At this point the BMS is pumping 42v into your 10S pack trying to bring each cell up to 4.2v. The cell that is at 4.1 will start to be drained at a rate of 50mA as per capabilities of the BMS. So the 4.1v cell is now getting 11950mA current in, while every other pack is getting 12000mA. Obviously this won't do much, and the 4.1v cell will still reach 4.2v charge state before the 4.0v cell leaving your pack out of balance. Over many charge cycles this may eventually be rectified.

This is also why charging at a lower current could help. If your BMS is capable of applying 50mA of drain and you charge at 12A that isn't very much. But if you charge at 1A that 50mA drain is going to make a bigger impact.

I hope my rather poor explanation makes sense. This is why BMS are a rather poor solution. Balance chargers need fans to dissipate the heat they generate from draining overcharged cells, thats why BMS is limited to something like 50mA of drain.
```

---
## \#33 Posted by: PXSS Posted at: 2017-03-30T17:38:26.378Z Reads: 185

```
The issue is that his charger was turning off because it was triggering the low current cutoff in his power supply. Nothing to do with the speed of balancing. It was simply not balancing at all. If a single cell reaches 4.2V it will not just turn the BMS off, it will try to balance the cells. BMS usually have their safety cutoff 50mV higher than 4.2 just for that reason. Now if you're running a 60V charger then yes, the BMS will cut off any and all current
```

---
## \#34 Posted by: Eboostin Posted at: 2017-03-30T18:03:16.128Z Reads: 190

```
How is your pack getting so out of whack though? The BMS is only an issue as you described if you are using low quality cells.
```

---
## \#35 Posted by: jaykup Posted at: 2017-03-30T18:21:15.444Z Reads: 194

```
This has peaked my interest.

Are you using the [Meanwell LED drivers (HLG series)](http://www.meanwell.com/product/led/LED.html) or their power supplies with fans?

What's the reason the wall power is killing them?
```

---
## \#36 Posted by: PXSS Posted at: 2017-03-30T18:52:26.369Z Reads: 191

```
@Eboostin ask @Eboosted, he had two dead cells in his pack.

@jaykup, I have a brick charger from a group buy that works just fine. @Eboosted is the one having all the issues with the BMS. The wall power is not killing anything, his cells are going out of balance. The BMS is not balancing as it requires lower current than the shutoff value for the brick charger and he wasn't discharging through a BMS so there was no low voltage cutoff for the individual cells. I think he said he had 2 cells completely dead at 0V. 
Check out this thread for more info: http://www.electric-skateboard.builders/t/at-what-voltage-your-pack-reaches-100/19302/98
```

---
## \#37 Posted by: longhairedboy Posted at: 2017-03-30T19:02:09.120Z Reads: 185

```
you know what's funny.. is people are always telling me to stop using the ones I use because they're allegedly terrible and that i should use meanwells, but other than being a little loud and warm, i have zero complaints with the 4amp ebike chargers from Battery Supports. They're super reliable in my experience and the only time i've seen one blow was when they shipped me one with a bad auto-switching circuit to adjust to 220 or 110. That problem was evident immediatly upon plugging in the unit and never got beyond that. 

I also have had zero issues with thier 60 and 80 amp BMSs. None. At all.
```

---
## \#38 Posted by: jaykup Posted at: 2017-03-30T19:14:05.853Z Reads: 178

```
Sorry - was replying to your comment a few months ago in this thread - 

[quote="PXSS, post:7, topic:16050"]
I am against meanwell power supplies/chargers.We have gone through 5 at work. Unless you have them on a UPS they will blow in a few months.
[/quote]

Just wondering which meanwell chargers you had issues with and why running them through the UPS seemed to make them last longer.  I was under the impression the LED drivers (aluminum fanless potted ones with adjustable voltage and current) were decent chargers for $40, but I haven't used mine long enough to see if it's going to last.  Since you've run yours for a few years I wanted to know more.
```

---
## \#39 Posted by: PXSS Posted at: 2017-03-30T19:21:05.399Z Reads: 179

```
Ohhh! We have some of these at work:
http://www.progressiverc.com/mean-well-rsp-2000-24-power-supply.html

Some of our wall outlets are notorious for having sh!tty power. The voltage may vary from 110V to under 100V when loaded moderately. We had not had any issues with it until we started using and killing these power supplies and they're not cheap...

Using a UPS helps keep the power clean and if we ever get a drop below 105V then the battery kicks in to help. That's why they last longer now although they are still dying overtime. 

We have moved to modifying server power supplies to power our 1500W charger which have no issues with the dirty wall power. We still keep them on UPS though
```

---
## \#40 Posted by: Hummie Posted at: 2017-03-30T19:23:07.467Z Reads: 175

```
how many drone hits happen a day?  from my estimation a while back it was 3 a day in Iraq @PXSS
```

---
## \#41 Posted by: Namasaki Posted at: 2017-03-30T20:47:54.211Z Reads: 168

```
[quote="Eboostin, post:30, topic:16050"]
Charging shuts off at 42.5V. If anything, with a 60V charger, you are trying to throw more voltage at an object that can't accept it.
[/quote]
We are not charging at 60v 
We are using an adjustable 60v charger to charge at 42v
```

---
## \#42 Posted by: Eboosted Posted at: 2017-03-30T21:09:29.770Z Reads: 172

```
[quote="PXSS, post:36, topic:16050"]
lue for the brick charger and he wasn't discharging through a BMS so there was no low voltage cutoff for the
[/quote]

Yes, 2 cells were completely dead 0V.

I'm following @PXSS and @Namasaki recomendations, however I'm still having a hardtime trying to get a suitable brick charger with low cutoff voltage (less than 50mA), as a more expensive, cumbersome charging alternative I'm buying an adjustable power supply that's should also fix the balancing issue.

http://www.ebay.com/itm/131286137884?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#43 Posted by: Eboostin Posted at: 2017-03-30T21:43:37.154Z Reads: 160

```
If I understand @Eboosted thread correctly, it has to do with being below 60ma. 

It sounds like the fact that a 60v adjustable charger is being used is irrelevant if it is set at 42v.
```

---
## \#44 Posted by: PXSS Posted at: 2017-03-30T21:51:31.206Z Reads: 159

```
Yes. They are using a lab power supply which goes all the way down to 0A with 1mA resolution/3mA accuracy. That is the key, not the 60V part
```

---
## \#45 Posted by: radium Posted at: 2017-03-30T23:54:21.860Z Reads: 162

```
My pack is fine, but in general, sometimes there may be temperature variations or other things that cause cells to degrade faster than others. I'm just stating that this is why I chose to go with a balance charger and 2 6S packs run in series for 12S rather than one big 12S pack.
```

---
## \#46 Posted by: radium Posted at: 2017-03-30T23:58:53.219Z Reads: 166

```
Could you spell out the problem he is having for me? I don't think I fully understand it. Why does he need a lab power supply? What is the laptop charger doing incorrectly that's causing the cells to unbalance? Is the issue being able to adjust the current so it is very low while the balancing is happening?
```

---
## \#47 Posted by: Namasaki Posted at: 2017-03-31T00:43:16.322Z Reads: 163

```
Your right, its not about the charger being capable of 60v max.
It's about that it will not shut off before the battery is full because it will continue to charge until it's output reaches zero amps.
These power supplies come in a 30v version and a 60v version.
So in order to charge at 42v, you need the 60v version.
```

---
## \#48 Posted by: PXSS Posted at: 2017-03-31T01:32:01.540Z Reads: 163

```
The charger is simply stopping when the cells reach 4.2V instead of balancing. I suspect this is because his charger has a low current cutoff to prevent trickle charging. This cutoff is higher than the balancing current. Which means his BMS doesn't balance the cells when charging at all. 

Why his cells are going out of balance is beyond me. Not having any protection while discharging is what killed the two groups though
```

---
## \#49 Posted by: Mathias Posted at: 2017-03-31T06:08:35.526Z Reads: 160

```
I've also decided to go with a balance charger instead of a BMS and the only one for 12s and a decent price that I could find is this one:
http://www.ebay.com/itm/Graupner-Ultramat-18-6470-/331869185998?hash=item4d44f1e7ce:g:OywAAOSwB-1Yuaql
But it is still way more expensive even than two 6s chargers. But be careful if you want to connect both packs at the same time and charge in parallel: I think when you connect the balance cables you basically short them and if they are out of balance you will probably damage the packs or even set them on fire.
```

---
## \#50 Posted by: smurf Posted at: 2017-03-31T07:09:42.127Z Reads: 149

```
I don't know how good this one is but it costs less.

http://www.nitroplanes.com/75p-1220-charger.html
```

---
## \#51 Posted by: Mathias Posted at: 2017-03-31T07:12:05.020Z Reads: 144

```
@smurf  Yes, I found this one too, but it was out of stock everywhere I looked. Also this one needs an external power supply, which would cost another 30-40 bucks.
```

---
## \#52 Posted by: smurf Posted at: 2017-03-31T07:14:37.333Z Reads: 147

```
Do most people hook them up to their car battery. Is that why they don't come with a ac power supply?
```

---
## \#53 Posted by: Mathias Posted at: 2017-03-31T07:20:53.024Z Reads: 150

```
@smurf I think so. Most buyers of these are probably charging large RC helicopters/drones I guess.
```

---
## \#54 Posted by: radium Posted at: 2017-04-05T02:09:10.723Z Reads: 153

```
I don't charge in parallel, I just use 2 6S chargers. The turnigy reaktor 2x works well for my purposes and does individual balancing of both 6S packs. It's also had the side effect of allowing me to split the pack for two boards when I don't have two charged batteries. I can still ride with a friend just at lower speeds, which is usually preferable to them anyway.
```

---
## \#55 Posted by: Builder_Of_Bots Posted at: 2017-04-05T14:11:51.558Z Reads: 150

```
What about this? http://www.icstation.com/lithium-battery-balanced-function-board-68ma-18650-polymer-battery-p-11653.html   It looks like it just moves electricity from battery to battery until every one of them is charged equally.
```

---
## \#56 Posted by: mmaner Posted at: 2017-04-05T14:14:40.261Z Reads: 141

```
    Operating Current:68mA
???
```

---
## \#57 Posted by: Builder_Of_Bots Posted at: 2017-04-05T14:20:16.402Z Reads: 145

```
Looks like it only moves electricity from one battery to another. So when one gets fuller than the rest it goes and gives some of its power to the other batteries that don't have as much. So it doesn't charge or discharge the battery it just moves slight amounts of current between batteries.
```

---
## \#58 Posted by: mmaner Posted at: 2017-04-05T14:25:46.989Z Reads: 149

```
could potentially be pretty cool, assuming you are correct.  I only say that because I've never heard of that before.  It would be cool to build a bunch of 2s packs with a 2s version of this, so you could plug them together to make 6s or 10s, or 12 s or whatever.  I wonder if you still charge over the NEG/PSO leg and if this non-BMS :slight_smile: would be affected?
```

---
## \#59 Posted by: PXSS Posted at: 2017-04-05T20:29:11.107Z Reads: 147

```
@Builder_Of_Bots
It doesnt work that way. Read the description 
"When the battery is in the end of full charged,it will discharge by resistor to first fully charged battery,namely shunt and balance function"

What you are describing does exist but is expensive. Research active balancing bms
```

---
## \#60 Posted by: smurf Posted at: 2017-04-05T21:54:58.183Z Reads: 146

```
Ya I checked in to the price is $1500
```

---
## \#61 Posted by: beckw Posted at: 2019-01-21T06:56:42.123Z Reads: 54

```
On this is it possible to have a Bms installed in your battery pack and have the cell cables rooted out to a pin header so you could balance the battery via balance charger from time to time or would this burn the Bms?
```

---
## \#62 Posted by: beckw Posted at: 2019-01-21T06:59:42.025Z Reads: 55

```
The point is you can charge your battery still with a normal power supply over Bms which is very convenient. To increase the battery lifetime and keep it balanced charge it sometimes with a balance charger.
```

---
## \#63 Posted by: taz Posted at: 2019-01-21T07:40:56.321Z Reads: 54

```
![thread-resurrection-memes-300x200|300x200](upload://ghoirNIFatmfJymINaUjkHpX2mU.jpeg)
```

---
## \#64 Posted by: AlexBE Posted at: 2019-01-21T08:19:42.274Z Reads: 48

```
It is definitely possible to root your cables. I encourage it.
```

---
