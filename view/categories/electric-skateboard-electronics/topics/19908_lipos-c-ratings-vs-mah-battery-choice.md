# LiPos C ratings vs mAh battery choice

### Replies: 30 Views: 2967

## \#1 Posted by: Sictrampa Posted at: 2017-03-29T11:48:51.518Z Reads: 334

```
Question is.....?
I'm trying to work if c ratting has anything to do with punch the battery has got in comparison to the amps it puts out.
If there is more amps and less C ratting due to the pack having a larger capacity does that a effect on performance and battery durability.
Eg:
12s 12000mah - four 6s 6000mah (65c)packs, two in series, two in parallel = 12s 12000mah.
6000x65 = 390 continuous amps.

Vs

12s 22000mah - two 6s 22000mah (25c)packs, conectected in series =12s 22000mah.
22000x25 = 550 continuous amps

Even know the 22000mah pack only has 25c compared 65c of the 12000mah  pack  does that make it have more punch and power?

The 22000mah pack has 160 more amps than the 12000mah, does this make up for the C ratting?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-29T13:29:58.486Z Reads: 321

```
There will be different opinions on this topic. 
I have never tried multi-rotor packs which is one extreme 10ah or more x 10c. 
I have heard that they lack power. 
I have compared 5ah / 25C in 12s config and
5ah / 60C in a 10s config. 
Although the 12s should yield more range, it did not. 

One thing I found is that the 60C cells have about 1/2 or less the internal resistance that the 25C had. 

My 10s 5ah 60c  Lipo battery yields about the same range as my 10s 9ah 60a Li-ion battery when both where subjected to high power demand. 
The reason was much less voltage sag with the 300a battery. 
So to get 300a continuous capability you need
5ah x 60c 
Or
30ah x 10c
So with higher C and lower AH you get the power in a smaller lighter package.
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-03-29T13:45:41.016Z Reads: 269

```
i have tried the multirotor style 10C Turnigy LiPos. They provide mad range and not a lot of oomph. I used a 16ah 6S2P Turnigy Multistar for a while and loved it as a general derping board. IT was no drag racer but it was still fast and ran for almost 25 miles.
```

---
## \#4 Posted by: Northlake Posted at: 2017-03-29T16:01:56.574Z Reads: 257

```
I agree with Namasaki and longhairedboy, the higher the C rating the less heated and stress on your batteries. That comes at the tradeoff with cost. higher C batteries are slimmer in design and cost more. You'll find that 10wh = 1km of range.
```

---
## \#5 Posted by: sl33py Posted at: 2017-03-29T19:09:26.493Z Reads: 249

```
Another point of view - similar to LHB.  Cruising where you don't need "punch" those big 10c lipos work OK.  Lots and lots of range w/ moderate acceleration and no hills.

But when you need power, you'll find them anemic and if you really push them you'll likely damage or puff them.  THey can't provide the power needed, and their "10c" rating (like most lipos) is marketing and not accurate outside a lab in ideal conditions (if that and not just made up for sales).

I try to get the highest C packs i can afford - less voltage sag when pushing them hard, and more oomph when you want it (hills or acceleration).
```

---
## \#6 Posted by: Sictrampa Posted at: 2017-04-02T13:26:49.343Z Reads: 222

```
I originally wanted to use two large capacity, high discharge 6s packs in series to try and make things simple.
Since not being able to get my desired configuration I've had to go for plan B...
The following configuration is what I've come up with.
•4 Turnigy Graphene 6000mah 6s packs
•65C continuous 390 amps
•130C burst 780 amps
•133.2 WH
Connected in series and parallel to achieve 12s.
https://hobbyking.com/en_us/graphene-6000mah-6s-65c-w-xt90.html

Im aware that these figures are proberly not realistic, Turnigy proberly use Chinese cells but I've heard that these particular graphene pack are not to bad.
At least I'll end up somewhere in the ball park of where I want to be and they are also available in Australia.

This is a option that I really didn't want to use because it will require 2x icharger duo chargers and have more wiring/connectors, but will fit in my enclosure nicely.

Reguarding the chargers, would I be correct in saying that I will require 2 chargers and two power supplies to power them?

The charger or chargers that I have chosen are.
• Icharger 406
I can't see the point of having 8 or 10s capable chargers when all I'll be charging is 6s.

Do you know of any other quality charging/balancing options I have to charge all four battery's on the one charger?

What would the specifications or the power supplies have to be to power the charger/chargers?
```

---
## \#7 Posted by: Namasaki Posted at: 2017-04-02T15:31:04.451Z Reads: 201

```
Glen, have you seen my thread on building a high power Lipo system with onboard BMS and simple charging?
I have been using this setup for a while and it has exceeded my expectations.
It is a 10s system but could easily be done in 12s as well.
Also about the quality of Turnigy Lipos, I feel that the Turnigy's high C rated packs are good quality.
I checked the internal resistance of the packs I'm using and they are substantially lower than the Zippy packs I have used.
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#8 Posted by: Ghettobird117 Posted at: 2018-01-26T15:01:51.000Z Reads: 143

```
What did you end up doing for a battery box?
As thoes 6000s are a bit too big for the gamed pelican 1150s and b&w 500 cases
```

---
## \#9 Posted by: Sictrampa Posted at: 2018-02-01T03:59:54.570Z Reads: 135

```
Decided against a battery box, mounted battery’s on top of board with Valcro. Had to move the front binding foward to get the batteries to fit on there sides tho...
![image|690x388](upload://73IwmzcnPEMWVWBJbxt7vHVZKzS.jpeg)
```

---
## \#10 Posted by: Volts Posted at: 2018-03-14T05:15:33.271Z Reads: 124

```
has anyone tryed compressing the lipos between two plates, I'v heard that this increases the capacity?
```

---
## \#11 Posted by: Deckoz Posted at: 2018-03-14T06:35:52.957Z Reads: 121

```
It doesn't increase capacity. It merely presses the anode and cathode layers.closer together lowering the IR of the battery. Lower IR = less heat when giving up energy. Closer the pack is held.to 90F degrees the more capacity you can pull from it. 

I squeezed my packs on my spot welder as it keeps them from heating..and also ya know the aluminum helps with that but it pulls the IR down about 30-40% from unsqueezed.

![IMG_20180302_212800|666x500](upload://8T1ORflV4GKgmZdEHl6aAnegrGI.jpg)

So no it doesn't increase capacity..just allows more efficient use of capacity. @Volts
```

---
## \#12 Posted by: Volts Posted at: 2018-03-16T16:43:40.159Z Reads: 113

```
Your the man thanks for the info was what i need to read
```

---
## \#13 Posted by: Cobber Posted at: 2018-03-24T12:07:21.136Z Reads: 109

```
Hey DeckyBro,
how much pressure are you putting the lipos under? :thinking:
```

---
## \#14 Posted by: Deckoz Posted at: 2018-03-24T14:27:00.775Z Reads: 103

```
@Cobber  Light pressure maybe 2-5lbs on the bolts, you dont need much to lower the IR, which in turn reduces voltage sag underload.

If you have an old lipo laying around, a tiny one(ex: 1300 4s, something you can fit in your hand and squeeze). You can experiment with this, put a lipo on a voltage checker/IR checker, with a 12v or dc lamp/load attached, and squeeze the pack by hand, you'll see the lamp get brighter as you squeeze, and the voltage increase (due to the lower IR between anode and cathode, the voltage sag of load decreases).
```

---
## \#15 Posted by: Cobber Posted at: 2018-03-24T14:35:22.878Z Reads: 97

```
was going to add heat sinks to my lipos, seems next level...

will test the IR on my icharger

thanks Bro, owe you a :beer:
```

---
## \#16 Posted by: E1Allen Posted at: 2018-03-24T17:59:08.541Z Reads: 94

```
Are your lipos getting hot?
```

---
## \#17 Posted by: Cobber Posted at: 2018-03-24T19:30:24.978Z Reads: 92

```
Not that I know of, telemetry data shows some sag though.

For science we like to ride fast...

2 x 1kg inrunners seem to suck as much juice as we can throw at them :thinking:
```

---
## \#18 Posted by: E1Allen Posted at: 2018-03-24T19:49:08.437Z Reads: 90

```
Voltage sag is normal under heavy loads though
```

---
## \#19 Posted by: Cobber Posted at: 2018-03-24T21:21:58.108Z Reads: 92

```
[quote="E1Allen, post:18, topic:19908, full:true"]
Voltage sag is normal under heavy loads though
[/quote]

Are you calling me fat?

:rofl:
```

---
## \#20 Posted by: E1Allen Posted at: 2018-03-24T21:35:38.734Z Reads: 88

```
![IMG_4674|646x499](upload://3z6rv5Zi1A8BtGbaghycJ9SZOdU.PNG)

One must first consult the BMI scale.  😁
```

---
## \#21 Posted by: Cobber Posted at: 2018-03-24T21:57:12.280Z Reads: 84

```
Just trying to mitigate what I can & keep as much of my top end as I possible.

Hopping to only use 330Wh/10Ah 8s 65C/130C Batteries with 296A of cont. rated motors. That's about 9,827W theoretical at 4.15V a cell (reality will prob. be peaks around >8,000W I think...).
```

---
## \#22 Posted by: E1Allen Posted at: 2018-03-24T23:05:20.634Z Reads: 79

```
Yeah but the huge amount draw, voltage is going to drop significantly.  When I pull over 100a on my 30q pack I see 7v drop.  What kind of amps are you pulling combined with those motors and what are they rated at??
```

---
## \#23 Posted by: Cobber Posted at: 2018-03-24T23:13:31.702Z Reads: 78

```
Manufacturer rates them (2x) at 5,180W/148A cont. at 35V 

I slightly under charge my lipos to 4.15V (33.2V) so even theoretical i'll bu under that to start.
```

---
## \#24 Posted by: Deckoz Posted at: 2018-03-24T23:16:11.343Z Reads: 80

```
7v drop??? Something doesn't sound right unless you'vr got s tiny pack...
```

---
## \#25 Posted by: Cobber Posted at: 2018-03-24T23:25:25.151Z Reads: 79

```
Deckoz is right, what is your voltage? mAh?
```

---
## \#26 Posted by: E1Allen Posted at: 2018-03-25T00:14:16.311Z Reads: 75

```
12s6p of 30q.  If you look at the discharge data sheet you can see about 5v of drop at 15+ amps.  So when drawing over 110A you get 5v plus losses in wires ~2v leading up to the vesc ish.
```

---
## \#27 Posted by: Volts Posted at: 2018-04-30T09:33:40.284Z Reads: 63

```
30qs are 18650 cells not lipos we are sharing info on the workings of compressed lipos cells, your playing English chess on a Chinese chess board
```

---
## \#28 Posted by: PatRocks Posted at: 2018-05-16T00:23:25.726Z Reads: 59

```
Holy shit, how have I overlooked this thread ??

LOL, I didn't realize squeezing lipolys had such an effect!! I thought I was imagining that my carbon fiber battery brackets made the board perform better. Now I KNOW they do 😂😂😎😎

I guess that endeavor was an even better idea than  I originally thought. Hell f*cking yea!!! Carbon fiber for the win
```

---
## \#29 Posted by: Kug3lis Posted at: 2018-05-16T00:37:29.841Z Reads: 59

```
Be careful... All problems with fire is then anode touched through insulator cathode then funs starts to happen :)

P.S. Also dendrite problem exist... 

https://youtu.be/E-OvK_sgoOE
```

---
## \#30 Posted by: lrdesigns Posted at: 2018-05-16T01:10:01.093Z Reads: 57

```
Dude that video was awesome! Most battery videos are like we have a new thing, it will be on the market in 10 years. 

But this showed some real information and some innovative research techniques. :sunglasses:

Edit. Found a related video. I has a lot of filler but it does show some shots of them making the button cells by hand 1pc at a time in the Argon chamber. 

Who wants to build an Argon chamber and DIY some batteries? hehe.

https://www.youtube.com/watch?v=79tg8sf63z4
```

---
