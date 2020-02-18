# 18650 cells, which ones?

### Replies: 21 Views: 1059

## \#1 Posted by: memesupreme Posted at: 2017-06-22T15:35:20.879Z Reads: 221

```
I'm looking at building a 12s4p battery using 18650 cells, I was thinking mainly of using Samsung 25r cells but can someone tell me if these will be good to use instead? https://ru.nkon.nl/rechargeable/18650-size/sony-us18650vtc6.html
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-22T15:46:58.925Z Reads: 220

```
Yes, those should be good. Samsung 30q, Lg HG2 batteries would also work.
```

---
## \#3 Posted by: memesupreme Posted at: 2017-06-22T15:49:06.975Z Reads: 222

```
Awesome thanks matey, now my battery should last longer per charge, I'll check out the Samsung 30q's too, might use them for a third build later on
```

---
## \#4 Posted by: rpn314 Posted at: 2017-06-23T00:26:44.804Z Reads: 207

```
I've been happy with the Samsung 25R's that I have, but I kind of wish I'd got with the 30Q (when I bought them a year ago, we hadn't really figured out how good a cell the 30Q was)
```

---
## \#5 Posted by: sl33py Posted at: 2017-06-23T02:52:37.535Z Reads: 193

```
I'd also toss in the VTC5a's for consideration.  Newer variant w/ 25A output capability - but slightly less capacity at 2600mAh.
```

---
## \#6 Posted by: Schulerbible Posted at: 2017-06-23T03:05:18.258Z Reads: 196

```
What about the Sony VTC6?

https://ru.nkon.nl/sony-us18650vtc6.html
```

---
## \#7 Posted by: sl33py Posted at: 2017-06-23T03:41:45.326Z Reads: 194

```
VTC6 is a great cell too - but 20A vs 25A for the newer little brother VTC5a.  25% more amp delivery and only 400mAh penalty (2600mAh VTC5a vs 3000mAh VTC6).

I'd google some "VTC6 / 30q / VTC5a - mooch" and look for some of his discharge graphs - i opted for VTC5a for my next pack because i wanted more amp delivery available, without crazy range needed (or more weight).

VTC6/HG2 12s4p = 12000mAh capacity (50.4v * 12Ah = 604Wh = 60km/37mi!)  Assuming 10Wh=1km.
VTC5a = 12s4p = 10400mAh (50.4v * 10.4Ah = 524Wh = 52km/32mi)

I am going for 12s3p VTC5a = 7800mAh (50.4v * 7.8Ah = 393Wh = 39km/24mi)

And associated weights of each pack (cells alone):
30q 4p = 2.2kg / 4.85lb
30q 3p = 1.65kg / 3.6lb

HG2 4p = 2.15kg / 4.7lb
HG2 3p = 1.6kg / 3.5lb

VTC6 4p = 2.25kg / 4.96lb
VTC6 3p = 1.68kg / 3.7lb

VTC5a 4p = 2.3kg / 5.0lb
VTC5a 3p = 1.7kg / 3.74lb

so about 1.2-1.3lb 3p lighter each vs 4p cells alone (not counting wire/nickel strip/etc.)  A lb is a pretty big difference on a board and i am fine with 18-20mi range real world.

my .02 and hope helps someone if thinking/comparing.
```

---
## \#8 Posted by: skatardude10 Posted at: 2019-03-21T04:15:36.311Z Reads: 102

```
_**Should 30Q cells be the standard, for high powered boards?**_

**TLDR:** Mooch says, anything above 17A per cell, the VTC5A will last longer (per charge) than a 30Q. 

Here are some of the less obvious stats I think matter in this case...

_NKON Prices:_
* VTC5A - €2.75  |  x50 - €137.5
* 30Q - €3.35   |   x50 - €167

_300 Cycles to 70% Capacity:_
* VTC5A - 10A discharge
* 30Q - 15A discharge

_Charge Currents_
* VTC5A - Standard 2.5A   |   Max 6A
* 30Q - Standard 1.5A   |   Max 4A


From Mooch: 
> Can the 2500mAh VTC5A run for longer than the 3000mAh 18650’s?

> The Sony VTC5A is more efficient, i.e., it has a lower internal resistance, than the 3000mAh Sony VTC6, Samsung 30Q, and LG HG2. This means it has less voltage sag when being used and takes longer to drop to a low voltage cutoff point. But does it hold its voltage up well enough to run for longer than batteries with 500mAh more capacity?

> If you just compare the mAh delivered by both down to 3.2V ([https://imgur.com/a/QvYU2](https://imgur.com/a/QvYU2?fbclid=IwAR0NP2IpSVqrdEeR0zSD6BsH7IJqmpWHvw6Rat9MD_RzI8ZyJ0oYfjIdjVA)) then it looks like the 30Q is equal to or better than the VTC5A. But for a regulated device the voltage the battery runs at is important too, not just the capacity. You want the battery to stay above the mod’s low voltage cutoff for as long as possible. The watt-hour (Wh) specification for the battery take both the voltage and capacity into account.

> I compared the watt-hours delivered by the VTC5A and 30Q at 10A/30W and 20A/60W down to 3.2V (about 3.5V-3.6V when put on a charger). At 10A/30W the 30Q was the winner, lasting about 10% longer.

> But at 20A/60W they both ran the same amount of time.

> Why? The larger voltage sag of the 30Q shortened its running time enough that the VTC5’s greater efficiency, and smaller voltage sag, let it run for just as long.

> Bottom Line: At up to about 17A/50W or so the 30Q, VTC6, and HG2 will run for longer in a regulated mod. At above 20A/60W the VTC5A is the better choice. It will run for the same amount of time or longer and will run cooler at any power level.

> For an unregulated/mech mod the VTC5A is the better choice since it hits harder, i.e. runs at a higher voltage, at the discharge current levels typical for those mods.

> The Sony VTC6 and LG HG2 perform about the same as the 30Q and these results will be about the same for them.

[Source](https://www.facebook.com/batterymooch/posts/can-the-2500mah-vtc5a-run-for-longer-than-the-3000mah-18650sthe-sony-vtc5a-is-mo/2063768540579388/)

https://scontent-dfw5-1.xx.fbcdn.net/v/t31.0-8/29662852_2063768487246060_7160812136560407156_o.jpg?_nc_cat=105&_nc_ht=scontent-dfw5-1.xx&oh=d04ccfc264be2498bc44302f89d791ff&oe=5D1132F4

Lygte:
![test|690x438](upload://s7JBOlfhf8C0g8O93YZmumu5MXD.png) 

I don't pretend to be a battery expert, but if you can get cells that drop voltage less, can charge with more amps for significantly better braking, discharge higher current, stay cooler under load, last longer (AH wise) under 17A+ loads per cell, for significantly cheaper, with a _slightly_ less overall life expectancy, why are VTC5As not the standard? Is it because nobody buys from NKON? Honestly, if I were buying cells from US distributors i'd have chosen 30Qs... but i'd like to hear if there is any consensus on this in the community?

For me right now, this is the best choice cell in terms of price/performance. VTC6 may be even better, but at almost double the price, it doesn't make much sense. Is it price consistency, that 30Qs tend to be priced reasonably across the board?
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-03-21T04:23:04.770Z Reads: 87

```
Erm the thread is kinda old lol 🤣
```

---
## \#10 Posted by: skatardude10 Posted at: 2019-03-21T04:26:20.526Z Reads: 91

```
Yeah I was looking at battery threads and didn't want to make another one, figured i'd put it in a related thread.
```

---
## \#11 Posted by: rich Posted at: 2019-03-21T14:19:46.348Z Reads: 83

```
Good reminder for this cells and for sure a good option for smaller packs which don't get too hot on higher discharge.

You made me thinking also because of the price but...

[quote="skatardude10, post:8, topic:25927"]
VTC5A - €2.75
[/quote]

Price of today is €3.34 VTC5A and €3.42 for 30Q (50pcs).
```

---
## \#12 Posted by: Virol Posted at: 2019-03-21T15:46:26.713Z Reads: 81

```
I've been using vtc5 for years in vaping and 25r, and I can tell that I really like 25r, but the vtc5 I feel like last longer and can reach a lower value delivering the same strength than when it's fully charge
```

---
## \#13 Posted by: thisguyhere Posted at: 2019-03-21T16:13:32.985Z Reads: 76

```
we're not really drawing anywhere near the max discharge rate of the cells.

below is a chart of battery current drawn on my last ride, max is less than 40a - this is on a 12s4p pack - so max current draw on this ride was less than 10a per cell.

![image|690x356](upload://jF27MGqwylc4z4yBSAc28xQ283I.png) 

on average, current draw is about 6a for the entire ride.

all that's to say, we're not maxing out the cell discharge, so accordingly to mooch:

[quote="skatardude10, post:8, topic:25927"]
At 10A/30W the 30Q was the winner, lasting about 10% longer.
[/quote]
```

---
## \#14 Posted by: Sn4pz Posted at: 2019-03-21T16:35:06.315Z Reads: 69

```
How are you manipulating your ride data? Would be a good graph for me in include in my build thread
```

---
## \#15 Posted by: thisguyhere Posted at: 2019-03-21T16:52:37.609Z Reads: 63

```
using @Ackmaniac's vesc monitor, android only.

app outputs telemetry data as csv:

 ![image|281x500](upload://bVqSN8m5h2q1ei4QGvXlmwkZa2J.png) 

then i just stuck it in excel to make the graph.

i think metr does this better but...you know, it costs money.
```

---
## \#16 Posted by: Sn4pz Posted at: 2019-03-21T16:57:52.298Z Reads: 62

```
I think the singular data set looks better, I dislike how metr makes me look at all of the data on one screen.

Maybe it doesnt work that way, I dont know. My only experience is with the web plugin.
```

---
## \#17 Posted by: thisguyhere Posted at: 2019-03-21T16:59:24.504Z Reads: 60

```
have no experience with metr.

it's an extra step, but once you put this data into excel, you can select whatever dataset you want displayed.
```

---
## \#18 Posted by: skatardude10 Posted at: 2019-03-21T17:19:36.854Z Reads: 61

```
Here is the ride data from my last ride, battery amps charted from highest to lowest over the course of the ride. Basically how many data points (how long) I was at some level of amp draw... It should make sense:

![Screenshot_20190321-111441_Sheets|689x172](upload://lYucaXnMv3R9edv0liX9vMxOilV.jpeg) 

I don't draw 80 battery amps a lot, but it's still a chunk small chunk of the ride at least. This is on a 10S4P battery. This small chunk of high amp output probably doesn't make the (continuous) high discharge on a VTC5A span out to being able to beat a 30Q, at least on my average ride. 

Either way, having an even higher amp draw capable cell will be more fun and drawing more than 20A per cell consistently probably applies the most to EMTBs or lower pressure pneumatic riders who ride hard, maybe even just urethane riders at constant stop and go under full acceleration and fat on the bones (or a backpack and hands full of groceries). This isn't me, minus the extra fat... I do just want batteries rated to give me double that 80A battery output for kraaazy torque.

Maybe I've just answered why 30Q is standard. Our amp draws are generally not consistently higher than what a 30Q is capable of, and prices on VTC5A fluctuate wildly depending on your source and when you buy.
```

---
## \#19 Posted by: thisguyhere Posted at: 2019-03-21T18:05:06.334Z Reads: 52

```
that's an interesting way to visualize it.

also, i think the first chart i had was for a single drive, i think i need to double it since it's dual.

even with doubling values, average current draw is 12a.

![image|690x334](upload://zH8OlWpv3l997BtGt4yp7G9Gc6z.png)
```

---
## \#20 Posted by: Darkie02 Posted at: 2019-04-03T13:48:12.030Z Reads: 38

```
Click on the name of the data and it toggles it on or off on the metr app.

Depending on why your looking at data but I don’t see the point in looking at one part of the data with out it’s related parts. 

It’s like comparing the mpg of 2 cars when ones a family car going slow down a hill and the others a race car floring it up a hill climb.
```

---
## \#21 Posted by: Darkie02 Posted at: 2019-04-03T14:35:13.169Z Reads: 32

```
Technology changes, how we use it changes, things need to be constantly braut back up and assesed and re evaluated. Take touch screen tablets 20 years a go thay were a complete flop couldent sell them. Now it’s a multi billion pound industry!

It’s part of the forum rules to look for posts and reply to them over creating new posts about the same things all the time. I found it disrespectful that you belittled some one for it.

Im looking at old posts as research in to battery’s and comparing the VTC5a vs Q30 (as that’s what I’ve narrowed it down to so fare) and witch would be better for my build.

A 4p/5p I would go q30 more range no penalty’s on lifespan or volt drop 
A 3p I think is the tipping point between q30 and VTC5a (still looking in to it but leaning towards the advantages the VTC5a over the advantages the q30 in this config. even tho most of the community’s seems to say q30 blindly for any battry config if you go back to older posts you had people insisting the r25 was better then q30).
A2p q30 just are not good enough lack of regen charging, lack of power running them so hard the volt sag would be crazy lower watt hours. I think the VTC5a would JUST cope
Above 5p and all sorts of options open up as most battery’s would cope

These are all opinions on what I have picked up from reading old posts that have useful information in them and help me and others make informed choices on what is going to work better for our builds.
```

---
