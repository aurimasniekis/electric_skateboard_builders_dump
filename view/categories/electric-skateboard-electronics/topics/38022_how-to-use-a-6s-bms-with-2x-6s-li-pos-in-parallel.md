# How to use a 6s BMS with 2x 6s Li Po&rsquo;s in parallel

### Replies: 20 Views: 1761

## \#1 Posted by: Orin635 Posted at: 2017-11-11T15:20:13.652Z Reads: 87

```
I have ordered this BMS (going to bypass discharge)<img src="/uploads/db1493/original/3X/0/c/0c6f597d7d9d990cfc7d070c414b0d6a6883659a.PNG" width="476" height="330">
and originally was going to use 2x 3S LiPo's in series but in the end, bought 2x 6s LiPo's and will be using them in parallel. but now have I only realised that the batteries I bought have 7 balance leads each and the bms only has 5  in total.

Have I ordered the wrong BMS? or do I just need to solder the balance leads together somehow.
Sorry if this is an obvious answer I am just so confused :P
Thanks everyone for the help.<img src="/uploads/db1493/original/3X/7/e/7e8d8a5ac8957681a5d7a2bbfa90312a23a49d72.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/5/65840c82afdde7d78bd3235f0f7030ae6ed167af.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/4/1462f3e0b25eab9103fc8c52e50d4ab1eb94247d.PNG" width="629" height="500">


EDIT: I was also going to originally going to follow this<img src="/uploads/db1493/original/3X/2/d/2de4c9ceeef2862c85f4d371df747ca4f9e0b5fa.PNG" width="690" height="345">
```

---
## \#2 Posted by: telnoi Posted at: 2017-11-11T17:09:52.188Z Reads: 78

```
That bottom diagram is confusing...judging by the first picture, B0 and B6 is B- and B+ respectively, hence you have 5 left.
```

---
## \#3 Posted by: Orin635 Posted at: 2017-11-11T17:26:50.680Z Reads: 77

```
What do you mean [quote="telnoi, post:2, topic:38022"]
B0 and B6 is B- and B+ respectively, hence you have 5 left.
[/quote]
```

---
## \#4 Posted by: telnoi Posted at: 2017-11-11T17:37:49.917Z Reads: 73

```
Your black (b0) and red (b6)  balance wire is apparently obsolete and essentially replaced by bat - and +.

Though I would research that. Weird BMS.

B + number stands for the balance wire number that has to be connected. Balance wire 1-5 is marked on the PCB.
```

---
## \#5 Posted by: Orin635 Posted at: 2017-11-11T17:39:19.909Z Reads: 69

```
I have a total of 7 balance on my LiPos (each)
```

---
## \#6 Posted by: telnoi Posted at: 2017-11-11T17:41:09.995Z Reads: 66

```
Your confusion confuses me :stuck_out_tongue:
B0 = black bat negative
B1 - connected via balance plug
B2 - ,,
B3 - ,,
B4 - ,,
B5 - ,,
B6 = red bat positive
```

---
## \#7 Posted by: Orin635 Posted at: 2017-11-11T17:42:57.949Z Reads: 62

```
Sorry, I am still confused. what do I do?
```

---
## \#8 Posted by: Orin635 Posted at: 2017-11-11T17:46:15.216Z Reads: 60

```
Do i just ignore B0 and B6
```

---
## \#9 Posted by: telnoi Posted at: 2017-11-11T17:51:50.039Z Reads: 63

```
Basically, yes. Take a look at the diagram below for 6s and compare it to the first picture you posted. The first (b0= black wire) is ignored as well as the last (b6=red). 

From what I understand, b0 is replaced by the negative battery lead that is soldered to what is indicated as b - in the PCB. Same for bat positive to b+.

<img src="/uploads/db1493/original/3X/3/f/3f9cf9536304339890197cecd32c938791228b58.jpg" width="690" height="493">
```

---
## \#10 Posted by: Orin635 Posted at: 2017-11-11T17:55:47.803Z Reads: 64

```
Ok, thank you. so I will solder B1-B5 together then to there corresponding to the BMS?
```

---
## \#11 Posted by: Orin635 Posted at: 2017-11-11T17:55:59.932Z Reads: 58

```
If that makes sense
```

---
## \#12 Posted by: telnoi Posted at: 2017-11-11T18:02:39.418Z Reads: 57

```
Balance lead B1 from bat 1 & 2  to BMS B1.
Balance lead B2 from bat 1 & 2 to BMS B2.

Repeat till 5.

Then of course the two negative battery leads to BMS B- and the two positives to BMS B+.

I think that should be correct.
Someone correct me if I am wrong.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-11-11T18:55:17.125Z Reads: 51

```
This look like one of those very cheap bms's from eBay.
I would highly recommend that you do not use such a bms.
Either buy a good bms or just use a hobby charger.
This is serious stuff and if you try to use cheap junk hardware, you might wind up with a bon fire
```

---
## \#14 Posted by: Orin635 Posted at: 2017-11-11T19:07:14.478Z Reads: 46

```
I am only using it for charging not discharge. also I have a volt tester
```

---
## \#15 Posted by: Namasaki Posted at: 2017-11-11T19:21:55.513Z Reads: 47

```
I would not use them for charging or discharging.
They are cheap and unreliable.
If your trying to budget, 
You can save money on a cheap deck, wheels , trucks but not on batteries and electronics.
Honestly, since your only running 6s, a hobby charger is a much better choice than a bms and brick charger.
The hobby charger will do a much better job of balance charging than even the best bms.
```

---
## \#16 Posted by: Orin635 Posted at: 2017-11-11T19:33:47.749Z Reads: 47

```
what BMS would you recommend that isn't too pricey then?
```

---
## \#17 Posted by: Namasaki Posted at: 2017-11-11T19:52:16.053Z Reads: 45

```
Bestech is number one
Battery Supports or Supower (eBay name) is a close second.

Bestech has more options but must be ordered direct from manufacturer with a min order of 2.
Supower can be purchased from the manufacturer's eBay site.
Both of these are name brands and proven for reliability.

@chaka was selling Bestech 6s bms's a while ago. Don't know if he still has any.

Here is a link for Supower:

http://stores.ebay.com/SuPower-Battery/22V-6S-High-Drain-BMS-/_i.html?_fsub=1108655119
```

---
## \#18 Posted by: Orin635 Posted at: 2017-11-11T19:53:36.730Z Reads: 39

```
All I want a bms for is to charge is there anything cheaper?
```

---
## \#19 Posted by: Namasaki Posted at: 2017-11-11T19:56:52.323Z Reads: 38

```
[quote="Orin635, post:18, topic:38022, full:true"]
All I want a bms for is to charge is there anything cheaper?

It doesn't get cheaper than this unless your buying junk.
[/quote]https://www.ebay.com/itm/22-2V-24V-25-2V-30A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System-/321823419482?hash=item4aee2bac5a
```

---
## \#20 Posted by: Orin635 Posted at: 2017-11-11T19:59:14.813Z Reads: 38

```
Ok If the cheap eBay one does not work I will get one
```

---
