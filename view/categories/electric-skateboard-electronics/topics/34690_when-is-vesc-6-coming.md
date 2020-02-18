# When is VESC 6 coming?

### Replies: 40 Views: 2410

## \#1 Posted by: Acido Posted at: 2017-10-03T19:06:05.170Z Reads: 259

```
Is there a date or something, when will companies like enertion trampa torqueboards whoever else exist will start selling it, im interested in it because the older vescs prices will drop hard probably and a bunch of people will be selling them so if its soon id like to wait and save some money
```

---
## \#2 Posted by: DavidBanner Posted at: 2017-10-03T19:08:48.528Z Reads: 260

```
The VESC6 is already out and being sold on Trampa's website.

The "older VESCs" are not going to drop in price due to two factors, a) the cost of manufacturing (these are very small runs) b) the VESC6 is considerably more expensive
```

---
## \#3 Posted by: MrHappy Posted at: 2017-10-03T19:08:57.166Z Reads: 252

```
http://www.trampaboards.com/vesc-6-complete--vedder-electronic-speed-controller-trampa-exclusive-p-24166.html i love google, dont you?
```

---
## \#4 Posted by: RedEagle Posted at: 2017-10-03T19:09:26.453Z Reads: 246

```
Vesc 6 has been trademarked by benjamin and trampa. As a result only trampa will be seling it.
```

---
## \#5 Posted by: Acido Posted at: 2017-10-03T19:10:13.935Z Reads: 231

```
I know trampa has been selling them, but i didnt know that they will be the only ones selling them

Its so expensive!

I guess i will have to go with the old one :)
```

---
## \#6 Posted by: Jinra Posted at: 2017-10-03T19:10:23.981Z Reads: 224

```
Reference design should be out soon-ish where other manufacturers can build their own VESC6 boards, though not with the same branding.
```

---
## \#7 Posted by: DavidBanner Posted at: 2017-10-03T19:10:34.267Z Reads: 218

```
Good point @RedEagle, although I do believe Mr Vedder will be releasing the information needed for others to making them under different names.
```

---
## \#8 Posted by: RedEagle Posted at: 2017-10-03T19:13:03.439Z Reads: 213

```
Be ready for people eating dirt when that happens xD
```

---
## \#9 Posted by: Jinra Posted at: 2017-10-03T19:14:23.952Z Reads: 207

```
? why's that?
```

---
## \#10 Posted by: DavidBanner Posted at: 2017-10-03T19:15:02.968Z Reads: 199

```
lol! yeah it's gonna happen, but to be fair I think the same thing will happen as with the VESC 4 - some boxes will be cheap as possible and prone to failure, others will be made by people who want to build a good reputation and will perform well because they spent the time and money on getting it right rather than saving a couple of bucks.
```

---
## \#11 Posted by: RedEagle Posted at: 2017-10-03T19:15:47.265Z Reads: 199

```
Because there will be companies who will cheap out on parts resulting in an unreliable product.
```

---
## \#12 Posted by: Eboosted Posted at: 2017-10-03T19:26:27.971Z Reads: 198

```
If they use the same componentes suggested by Vedder the the only possible issue could be the quality of soldering jobs, the original components on the VESC 6 have proved to be good so far with no need to upgrade them as was needed to run reliable as vesc 4.

@DavidBanner in order to happen what you estimate manufacturers would have to change the part numbers of components for cheaper ones, I'm not sure if anyone would venture to do so as they would be asking for trouble altering original BOM. 

The vesc6 versions from other manufacturers won't drive the cost down by downgrading components (maybe 2% of the cost) but by cutting out the middleman.
```

---
## \#13 Posted by: DavidBanner Posted at: 2017-10-03T19:40:31.325Z Reads: 193

```
@Eboosted Seems like Maytech may have taken that path already....

Soldering is not really such an issue unless it's done in a proper DIY way - i.e. with a soldering iron, anyone serious is going to be use wave soldering.
```

---
## \#14 Posted by: DavidBanner Posted at: 2017-10-03T19:42:28.100Z Reads: 185

```
I know guys who work for seriously high end audio equipment manufacturers, one of them left because he couldn't deal with the compromises, he was literally being forced to save $1 and $2 on units that were retailing for $15k+
```

---
## \#15 Posted by: Acido Posted at: 2017-10-03T19:42:43.805Z Reads: 181

```
I guess it takes about 3 hours to solder it and if done by one person it is some serious time like 3 per day only
```

---
## \#16 Posted by: DavidBanner Posted at: 2017-10-03T19:47:40.666Z Reads: 176

```
it takes a couple of minutes to do a PC main board, so the time to do a VESC size PCB is going to be measured in seconds not hours

[Wave soldering](https://www.youtube.com/watch?v=inHzaJIE7-4)
```

---
## \#17 Posted by: Acido Posted at: 2017-10-03T20:00:29.703Z Reads: 175

```
oh man this is so frickin cool
```

---
## \#18 Posted by: DavidBanner Posted at: 2017-10-03T20:01:00.774Z Reads: 178

```
yeah it is!

If anyone is wondering what to get me for Christmas.....
```

---
## \#19 Posted by: Acido Posted at: 2017-10-03T20:02:16.109Z Reads: 177

```
having that mashine would be ao cool i would make a 100per day lol
```

---
## \#20 Posted by: fedestanco Posted at: 2017-10-03T20:29:43.616Z Reads: 181

```
Vesc has mostly surface mounted components and is double side populated so I doubt they use wave soldering; it is a cool video to watch though :slight_smile:

In the vesc manufacturing most of the time is spent inserting all of the components reels in the pick & place machine, and in the optical/x ray testing. Basically anything that has to be human-handled slows down the production. Reflowing 100 vescs may take up to 5 minutes with a decent industrial oven.
```

---
## \#21 Posted by: DavidBanner Posted at: 2017-10-03T20:34:31.823Z Reads: 176

```
AFAIK SMD can be done with both wave and reflow? I guess reflow is more efficient in this case?

[quote="fedestanco, post:20, topic:34690"]
In the vesc manufacturing most of the time is spent inserting all of the components reels in the pick & place machine
[/quote]
Yeah, that is the real cost right there, stopping the machine to load components for a short run...
```

---
## \#22 Posted by: fedestanco Posted at: 2017-10-03T20:42:16.480Z Reads: 174

```
Yes in theory. Wave soldering smd components requires to change the pcb design accordingly: rectangular chips must travel (during the assembly) with the short side perpendicular to the "tin wave", components hight must not exceed a certain height.....
```

---
## \#23 Posted by: DavidBanner Posted at: 2017-10-03T20:43:36.820Z Reads: 178

```
thanks for the info @fedestanco - that makes a lot of sense.
```

---
## \#24 Posted by: esk8 Posted at: 2017-10-04T09:07:41.565Z Reads: 165

```
I have ask my Vesc producer how much cost so one machine.
He say over 250.000€ :confounded:
Can this be true?
YAMAHA YS12F

https://youtu.be/ObPvU5fru7k
```

---
## \#25 Posted by: BigBoyToys Posted at: 2017-10-04T09:12:58.990Z Reads: 168

```
@Vanarian aren't you already working on a VESC6 alternative?
```

---
## \#26 Posted by: esk8 Posted at: 2017-10-04T09:22:35.953Z Reads: 170

```
There are alternatives:
FocBox Ollin ESC 1.1 and ESK8 1.1 controller
All have direct fets on it what is better for cooling
But the Vesc6 has much more than the 4.12 does not have.
But you need it for an electroboard?
```

---
## \#27 Posted by: Ken_Chen Posted at: 2018-01-22T06:57:49.494Z Reads: 126

```
We will start selling our own VESC.  so far all of the test of our VESC are run smooth, and we will sell start officially when all test are finished.
```

---
## \#28 Posted by: scepterr Posted at: 2018-01-22T07:00:30.741Z Reads: 124

```
Is it vesc6 based? Do you have details, pics you can share?
```

---
## \#29 Posted by: Ken_Chen Posted at: 2018-01-22T09:22:37.533Z Reads: 118

```
It's only vesc4 based now. 
The first version we start to sell is base on vesc4, but after it , we also will selling the vesc6 based, are you interest in it?
```

---
## \#30 Posted by: scepterr Posted at: 2018-01-22T09:24:23.385Z Reads: 120

```
Is it using the 4.12 bom? Any upgrades?
```

---
## \#31 Posted by: b264 Posted at: 2018-01-22T10:03:37.176Z Reads: 116

```
What are the changes to the vesc4.12 BOM on your board, or is it identical?
```

---
## \#32 Posted by: bimmer Posted at: 2018-01-22T10:42:54.635Z Reads: 120

```
![15165086316631502401422|690x388](upload://wG5u1YjwIiYRSLPkqPlYnAjkakv.jpg)![15165276106441122986251|281x500](upload://2AZ3hK44kD8JSyLj7pxVnltthJ2.jpg) took me about 2hrs for 2 I had bought 4 pcb destroyed 1 and have 1 left.
```

---
## \#33 Posted by: Acido Posted at: 2018-01-22T10:49:48.944Z Reads: 113

```
I would love to do this once i have the time to learn and money to waste because for sure I will blow one up :D
```

---
## \#34 Posted by: bimmer Posted at: 2018-01-22T10:52:14.503Z Reads: 116

```
I spent about 600$ with tools to make 4 and blew one so about 200$ per vesc 6 on my end but I can make a 4th with just a new pcb, drv and some small parts :D so lets say 630$ for 4.
```

---
## \#35 Posted by: Acido Posted at: 2018-01-22T10:55:00.721Z Reads: 114

```
Cheaper to buy it from @stewii , if you are looking to save money, but for fun its worth it
```

---
## \#36 Posted by: bimmer Posted at: 2018-01-22T11:04:53.238Z Reads: 118

```
I bought my boards from him. I was looking for a challenge and a reason to buy a smd rework station.
```

---
## \#37 Posted by: Slak Posted at: 2018-01-22T11:36:58.356Z Reads: 111

```
Hello Acido,

Don't know if you're still looking for VESC6 to buy, but here's a link in France : https://www.unikboards.com/en/boutique/vesc-6/
```

---
## \#38 Posted by: Charles_Chan Posted at: 2018-01-23T07:20:40.893Z Reads: 88

```
For the VESC 6, what is the greatest advantage of VESC 6 than other ESC. I want to buy one, but I still not very clear the advantage of it.
```

---
## \#39 Posted by: Acido Posted at: 2018-01-23T07:22:18.815Z Reads: 86

```
Can handle a lot more amps than regular one
And has a higher erpn limit
```

---
## \#40 Posted by: linsus Posted at: 2018-01-23T08:21:58.243Z Reads: 82

```
This is just untrue.. The VESC 4 is proof enough that there are both cheap and expensive ways of producing it. Component cost can be cut alot more then 2% if you choose the cheapest set of components. Quality of the product will follow.
```

---
