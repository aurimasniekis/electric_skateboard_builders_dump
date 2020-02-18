# Adding on a solar panel?

### Replies: 24 Views: 2697

## \#1 Posted by: Quinlanbrown Posted at: 2017-01-29T18:29:09.671Z Reads: 279

```
https://www.amazon.com/ALLPOWERS-Portable-Battery-Cigarette-Charging/dp/B00QRHDIPY/ref=sr_1_5?ie=UTF8&qid=1485711786&sr=8-5&keywords=solar+panels
Would this do any good if I wire it in with the charger on my bms?
```

---
## \#2 Posted by: treenutter Posted at: 2017-01-29T18:34:47.178Z Reads: 275

```
@Quinlanbrown check out @cmatson s build with solar charging for ideas.
```

---
## \#3 Posted by: Okami Posted at: 2017-01-29T18:42:45.315Z Reads: 270

```
5w does not sound much.. if you could cram in 10-20w, I think that would be somewhat worthy.. depending on do you get full exposure of your panel and how much hours do you spend in the sun..
```

---
## \#4 Posted by: Quinlanbrown Posted at: 2017-01-29T18:46:28.129Z Reads: 258

```
I thought it would be a cool thing to use when I'm at school and stuff I could just put in in the window or something
```

---
## \#5 Posted by: Okami Posted at: 2017-01-29T19:04:49.666Z Reads: 250

```
I think you would be fine charging your phone.. or your remote controller with this panel.. but other than that.. at like 18v and 5W (which seems to be about ~300ma, max) such power amount is not much usable anywhere..

Even, if you left the board/panel out in the sun.. let's say.. from 9pm till 4-5pm, which would be 7-8 hours... then the total amount of energy you could put into the batteries or elsewhere.. would be 7 x 5w = 35W-40W..

If you convert this into direct electrical energy, then if, your board was ''parked outside'' without any other power rather than the sun. then you would probably pump back something like 4kilometers of ride time (at 10wh/km).. and this is without taking into consideration the inefficiencies in the system..

--

You would be better off, building a seperate ''charge pack' for your main batteries.. if you want to charge the board while outside.. and not connected to any other power source nearby..
```

---
## \#6 Posted by: Fin420 Posted at: 2017-01-29T19:19:19.095Z Reads: 224

```
Honestly I doubt it would be worth it, I've used these things quite a lot and they just don't have a high enough current output to be any real use,  I've used small 5w ones like that, up to bigger 100+ watts and they are still like pissing in the wind. They might be some good for charging head and tail light batteries though!
```

---
## \#7 Posted by: RogerD Posted at: 2017-01-30T00:02:38.491Z Reads: 190

```
A 6S board with, say, 7000Mah of batteries will charge at 1s at 25.2volts at 7 amps (176 watts). 1s = 1 hour to full charge.

A 100w 12v (20v really) solar panel, in full sun will give 6 amps max. (96watts @ 16v) (solar panels voltage drops as they heat up - hence they start at around 20v for "12v" applications). So that's a little over half what you need for charging, with a panel that is 1m x 60cm.

5w = pointless.
```

---
## \#8 Posted by: Quinlanbrown Posted at: 2017-01-30T00:39:02.712Z Reads: 171

```
Ya I didn't look into it that much but it would be kinda cool to charge a car battery with a bigger panel and charge my board with that to get the feeling that it's all solor
```

---
## \#9 Posted by: Okami Posted at: 2017-01-30T01:21:21.373Z Reads: 169

```
I think with wind power you could get far more power... 

Boards dont eat up that much energy.. to move around with a car takes about 10times or more energy I think.. at least this is a somewhat approximate guess.. comparing the vague numbers I remember from Tesla's wh consumtion per mile/km. and tesla itself is quite heavy car..

If your battery is about 200wh.. you only need about 200w of power to charge it..

Your computer probably burns a similar amount of energy in a couple of hours :D
```

---
## \#10 Posted by: Quinlanbrown Posted at: 2017-01-30T01:25:03.439Z Reads: 156

```
no 200wh is = to 20,000w it would take for ever
```

---
## \#11 Posted by: Okami Posted at: 2017-01-30T01:25:56.622Z Reads: 151

```
do you mean 20kw?

1 kw = 1000w?

200w = 0.2kw

--

I've seen a solar panal ''trailer'' attached to an ebike.. I think that guy was able to ride on solar energy alone! But he did manage to get something like 200-300w out of his panels.. but do count that he had a trailer with him.. not just tiny piece in size of a smartphone :D
```

---
## \#12 Posted by: Quinlanbrown Posted at: 2017-01-30T01:32:40.004Z Reads: 141

```
what kind of panal was that, i thought 1wh=1000w
```

---
## \#13 Posted by: PXSS Posted at: 2017-01-30T02:45:33.136Z Reads: 134

```
1Wh = 1 Watt of power for 1 hour...

Saying 1wh = 1kw is Kinda like saying:
1m/s = 1000meters
```

---
## \#14 Posted by: Quinlanbrown Posted at: 2017-01-30T05:08:08.957Z Reads: 120

```
it would just take a wile to charge if i got a 10w panel it would take 30 hours to charge my 300wh battery but thats only in direct sun light so itd probly take like a week
```

---
## \#15 Posted by: Okami Posted at: 2017-01-30T09:04:03.915Z Reads: 116

```
Now you got it correct I think ;)

Yes.. it would take unreasonably long time to charge anything that big.. as your eboard's battery..

And that is at maximum efficiency.. without taking into consideration that bms/charger might eat up some watts along the way.. 

--

If you want some sort of ''solar solution'' - buy big solar panel.. rig it up (with the right electronics) to charge up some other batteries.. (or connect yours directly, if panels are capable enough).. and then charge it that way from another battery.. though this still uses chemical energy.. but I know some ppl have been advertising such method as somewhat ''clean energy'' without using the energy from the grid..
```

---
## \#16 Posted by: RogerD Posted at: 2017-02-03T12:59:30.767Z Reads: 103

```
His panels would have been charging a battery - a battery which was powering his ebike. To give him extra range on already charged batteries.

He would not have been running his ebike of 300watts of panels directly.

300Watts of panels produces, at max, 18 Amps at 16 volts, or 12 Amps at 25 v (at theoretical max efficiency - which means a cold day with bright direct sun pointed directly at the panels).

As you will know having an eboard, you need, at 25 volts, around 70+ amps to get anywhere. My eboard (6s) pulls up to 120 Amps uphill. On the flats around 30-70 amps.  Even with higher voltage you have the same ratios - you'll gain voltage but drop in amp production from your panels.

If you built a very light bike, with low friction tyres, panels angled at the sun, in ideal weather, with a pedal start, on flat ground, you could slowly propel yourself with 300watts of solar. Until you were not aligned with the sun directly...  and that's with a solar panel area of 3metres by 1.5 metres.

I am a solar specialist - I make and install solar panel kits for camper vans, so I am aware of what they are capabale of.

One thing I do do in the summer, is charger a car battery with solar, which I then in turn use to partially charge by eboard sometimes. But a car battery doesn't have the beans to charge a 15Ah 6s battery pack before the voltage drops below the charger's minimum requirement.
```

---
## \#17 Posted by: Okami Posted at: 2017-02-04T22:41:25.235Z Reads: 85

```
Will post Link once I find it again..

The idea behind ''running on solar panels'' was behind that - he almost did not use battery power at all.. the battery was there, but his panels output a decent 300-400w of power, I think.. totally enough for ebike riding
```

---
## \#18 Posted by: RogerD Posted at: 2017-02-08T18:53:10.820Z Reads: 76

```
I'd very much like to see the link. He must have a very efficient bike with massive panels.
```

---
## \#19 Posted by: Okami Posted at: 2017-02-08T19:22:18.565Z Reads: 79

```
Ok gonna go now and find it.. it is somewhere

[Edit]

Here, ya go @RogerD :

http://www.cbc.ca/news/canada/newfoundland-labrador/solar-energy-powers-7-000-km-bike-ride-across-canada-1.3101603

There was one similar - link - it should have another guy having a ''solar trailer'' and travelinger around etc..

--
---

> "It's a 48-volt system and I have 600 watts of solar ... and that's what I'm romping across the country with.

So I assume he is not getting all 600w all the time.. it is the maximum capacity of his panels.. non the less,, he probably receives a good 200-300w of power anyways,, if it is a sunny day.. (at least I hope the math is right for solar intensity n such)
```

---
## \#20 Posted by: Okami Posted at: 2017-02-08T19:33:42.936Z Reads: 78

```
Here''s the second article, for those who missed it in the first one:

http://www.cbc.ca/news/canada/thunder-bay/solar-bike-turning-heads-in-thunder-bay-1.1133385

> Small said on a sunny day the bike can run for 300 kilometres.

He does not say how much power he gets but 300 km does sound good..
```

---
## \#21 Posted by: RogerD Posted at: 2017-02-08T19:44:14.300Z Reads: 77

```
Now things are clearer :slight_smile:

He's got 600w, not 300w, but there is no way that powers that contraption alone. 

He's got car batteries in there, which the panels charge. He also has pedals which "  **help** to power him down the highway"

The details are all a bit muddy, if you follow the link from the article  (http://www.cbc.ca/news/canada/thunder-bay/solar-bike-turning-heads-in-thunder-bay-1.1133385) you see the non-trailered version which he claims is around 18 Kg! lol. On that one he has three rigid 100W panels, They weigh 8 Kilos each. Trust me, I know.
So that's 24 Kilos in panels before you've even allowed for the trike - whose wheels are probably 5 or 6Kg each.....

Then there are the batteries.... If he's using car batteries it's a huge weight, so I would hope he's using Lipos or similar, though he refers to a 48v system which is coincidentally the exact voltage of 4 car batteries in series.

On his trailered versiojn he's using 6 thin panels. They  weigh much less, like 2 Kg each. But his trailer is heavy duty.

He's aldo got the panels angled at one side so he's grand when cycling with the sun to his side, but he's snookered when he turns a corner and the sun is behind / in front of him.

The reality is that the solar panels charge his batteries, which helps him pedal. He stops to eat/rest etc - at which time he's getting good solar energy put into the batteries. When he goes down hill he's also charging the batteries.

600W is not enough however, to reliably power that thing. Take a look at my numbers again. it doesn't stack up.

The solar is , as he has stated, "helping him".

Also remember that 600watts is ideal conditions. I can tell you for a fact that a 100W panel maxes at around 85 watts after real world losses, and that is when it's pointed directly at unobstructed sun.
```

---
## \#22 Posted by: Okami Posted at: 2017-02-08T22:34:39.910Z Reads: 69

```
So, I assume at 85% max efficiency he might achieve 510w of power in direct sun.. now, if ''remove''  the panels on the ''shade side of the sun/trailer'' from total power received from sun.. Then we might divide this number by two or so? 

Perhaps by 1.7 would be better.. as there is still some light flowing in into the panels on the shade's side..

So now we get about: 510 / 1.7 = 300w of power..

I assume there could be some other.. minor losses and ''not ideal sunlight''.. so during somewhat cloudy not so sunny day.. he should still get about 100-200w of power, right?

I know.. this is not direct solar energy.. but I think we will get there some day.. when the panels get more efficient or some other new tech (like lenses for panels) become more available/popular..
```

---
## \#25 Posted by: amusingwake Posted at: 2018-07-01T07:48:47.500Z Reads: 50

```
Thanks ALL
```

---
## \#26 Posted by: amusingwake Posted at: 2018-08-09T05:35:31.932Z Reads: 27

```
Are solar panels affected by rain? How solar panel working changes in different seasons?
```

---
