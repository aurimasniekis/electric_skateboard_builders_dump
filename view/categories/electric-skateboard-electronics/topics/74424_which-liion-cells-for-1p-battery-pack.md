# Which Liion cells for 1P battery pack?

### Replies: 32 Views: 513

## \#1 Posted by: Maxid Posted at: 2018-11-12T12:34:17.116Z Reads: 161

```
I want to build an additional battery pack for my Lou board (which can only take a 1P battery).
The obvious choice is 30Q cells but I am wondering if a VTC6 might be the better solution (or other types - I am open to recommendations).
Use case will be uphill to work for say 5min - until now I used the original Panasonic cells but the sag is real and I want more oomph. Other than the short uphill section its mostly flat and fairly easy on the battery.

Let me know what you'd choose!
```

---
## \#2 Posted by: moon Posted at: 2018-11-12T12:35:02.381Z Reads: 160

```
Samsung 30T?
```

---
## \#3 Posted by: Pedrodemio Posted at: 2018-11-12T12:38:34.433Z Reads: 157

```
Or 40T, almost same discharge as 30T
```

---
## \#4 Posted by: Andy87 Posted at: 2018-11-12T12:47:54.784Z Reads: 151

```
if you want to go with 18650 than VTC5A
```

---
## \#5 Posted by: brenternet Posted at: 2018-11-12T12:53:44.746Z Reads: 144

```
Form factor significantly different on them though
```

---
## \#6 Posted by: Maxid Posted at: 2018-11-12T13:09:04.258Z Reads: 135

```
well I am not sure if the 21700 batteries will fit so I'd rather use the 18650 I know will work.
```

---
## \#7 Posted by: Acido Posted at: 2018-11-12T14:17:32.479Z Reads: 131

```
VTC5A or if you can find VTC6A both good options

Have you considered splitting lipos?
```

---
## \#8 Posted by: moon Posted at: 2018-11-12T14:21:28.702Z Reads: 132

```
https://www.nkon.nl/rechargeable/18650-size/red-sony-murata-us18650vtc6.html

nvm out of stock

Whats the difference between the one i linked and this?

https://www.nkon.nl/sony-us18650vtc6.html
```

---
## \#9 Posted by: Acido Posted at: 2018-11-12T14:25:54.971Z Reads: 128

```
to me it seems that its the same battery 
probably just an old listing
```

---
## \#10 Posted by: Maxid Posted at: 2018-11-12T18:33:03.118Z Reads: 107

```
I just remember an old post about 30q and VTC6 that concluded that the Samsung are actually preferable because of cycle life or whatever. I know about the constant discharge curves and somehow can't bring myself to get the Sony at double the price than 30Q. Is there any data out there for this burst like behavior that I am interested in for a short uphill climb?
```

---
## \#11 Posted by: skatardude10 Posted at: 2018-11-12T23:15:44.418Z Reads: 88

```
Out of a box full of discarded vape batteries, all the brand new looking VTC6s were dead but one. Out  of all the old worn out looking 30Q, maybe one or two were completely dead.

That's anecdotal but it's enough to convince me personally to never build a pack with VTC*x*s expecting it to last too long.
```

---
## \#12 Posted by: PXSS Posted at: 2018-11-13T00:39:28.976Z Reads: 83

```
I've run both cells to the ground and VTC6s are slightly better but does not justify the price difference. I prefer working with VTC6 because the button is slightly raised too.
```

---
## \#13 Posted by: Maxid Posted at: 2018-11-13T06:46:22.920Z Reads: 73

```
Well I guess I go with 30Q then.
```

---
## \#14 Posted by: bigben Posted at: 2018-11-13T07:30:41.175Z Reads: 67

```
Check out the sanyo 20700B. You might just squeeze those in no?
```

---
## \#15 Posted by: b264 Posted at: 2018-11-13T07:33:24.729Z Reads: 70

```
I doubt there's room in the Lou board for those, but I could be wrong.  I don't have one.  They look rather cramped inside.
```

---
## \#16 Posted by: Maxid Posted at: 2018-11-13T08:17:52.534Z Reads: 67

```
I think they might fit when not using a case around the battery. But I'd rather not try and find out they don't so I'll stick to 18650 for now.
```

---
## \#17 Posted by: thisguyhere Posted at: 2018-11-13T08:22:35.844Z Reads: 67

```
just got some 30q cells today:

http://esk8life.com/samsung-30q-18650-cell
```

---
## \#18 Posted by: Maxid Posted at: 2018-11-13T08:25:19.695Z Reads: 68

```
I am in Germany so probably better off with a direct nkon purchase (I have to order some Sanyo GAs as well for another ebike pack anyway). But your battery looks amazing with the p groups and copper braid :+1:
```

---
## \#19 Posted by: Maxid Posted at: 2018-11-20T18:17:55.296Z Reads: 61

```
Anybody know how the Samsung 50E performs?
https://eu.nkon.nl/rechargeable/21700-20700-size/samsung-inr21700-50e.html
Can't seem to find any discharge curves on the web.
```

---
## \#20 Posted by: Maxid Posted at: 2019-07-05T10:07:05.546Z Reads: 42

```
Looks like the 50E is actually quite capable. 
https://lygte-info.dk/review/batteries2012/Samsung%20INR21700-50E%205000mAh%20(Cyan)%20UK.html

I am thinking of building an ebike pack out of it in a 3P configuration - should outperform a 4P Sanyo GA pack

@PXSS you seemed to like the GA quite a lot - have you considered the 50E for your projects? 

![image|634x288](upload://ixTIbadqniKnRNLAW5wovivjo2u.png)
```

---
## \#21 Posted by: Darkie02 Posted at: 2019-07-05T10:48:53.009Z Reads: 35

```
![image|690x388](upload://uWkFF0TSnfmAZoMeBaW4y565fGh.png) ![image|690x388](upload://ybwito7iV1Jj0wukyiQQNH7GOMU.png) [quote="Maxid, post:1, topic:74424"]
The obvious choice is 30Q cells but I am wondering if a VTC6 might be the better solution (or other types - I am open to recommendations).
[/quote]

Q 30 are not capable of 30A discharge VTC6 and VTC5A are

Personaly Id only use Q30 in a 4P or more config below there’s better options IMO.
```

---
## \#23 Posted by: PXSS Posted at: 2019-07-05T12:33:22.722Z Reads: 31

```
You're looking at and comparing incomplete data. Henrik stopped the test for 30Q cells at 75C but lets the VTC6 reach a higher temperature (into the 80s) before he stopped the test. 

As I've stated before, with appropriate cooling, 30A per cell can be achieved on both 30Q and VTC6. 

Besides, continuous rates at that current is irrelevant to esk8. Running continuously at 30A per cell means that you would discharge your entire battery in under 6 minutes. We normally don't do bursts longer than 10 seconds, very few do bursts longer than 30 seconds. I haven't been around here in a while so I may be wrong there but unless something drastically changed in the past 6 months, we are nowhere reaching the limits of 30Q yet.
```

---
## \#24 Posted by: Maxid Posted at: 2019-07-05T12:45:49.116Z Reads: 28

```
You're still my go to guy when it comes to batteries - so far your advice has been invaluable.

I calculated the volume and capacity in the spreadsheet above and to me it looks like the energy density is actually higher for the 50E (even though only slightly) with a usable capacity at 111% that of a GA pack and only a 108% in size. I used the data from lygte to get the actual dimensions and usable capacities.

Also the voltage sag seems to be lower on the 50E (I compared the lygte data for 7A for the 3P 50E pack and 5A for the 4P GA pack to get comparable currents for the individual cells) which should make for a very energy dense but still powerful ebike pack.
```

---
## \#25 Posted by: Pedrodemio Posted at: 2019-07-05T12:54:03.971Z Reads: 26

```
@Maxid I've looking a lot at 50E, Padja at endless sphere has some good insights, not only for the 50E, really recommend reading all his posts

They should perform really good, better than the 30Q if you consider the cycle life, even if it doest matter for most people 

The GA still my cell of preference with larger packs

https://endless-sphere.com/forums/viewtopic.php?f=14&t=100209&start=50&fbclid=IwAR2Op66V33uiT4SNvNlL8Zgxqoh1nrBxJbyIj9EzBU1WFxFxOA8R6-noYGQ 

https://endless-sphere.com/forums/viewtopic.php?f=14&t=100907&fbclid=IwAR1qqhXufAA08MrFmJNIbLa6_pPcoWb0fuunZ7E_SQ4wnAS8_zpEekh-x5o
```

---
## \#26 Posted by: PXSS Posted at: 2019-07-05T13:14:57.336Z Reads: 24

```
[quote="Maxid, post:24, topic:74424"]
I calculated the volume and capacity in the spreadsheet above and to me it looks like the energy density is actually higher for the 50E (even though only slightly) with a usable capacity at 111% that of a GA pack and only a 108% in size. I used the data from lygte to get the actual dimensions and usable capacities.
[/quote]
That is correct,  but when assembling a pack, you lose space between cells. If you take this into account, the 50E is no longer more energy dense. 

Assume they are rectangular or hexagonal in cross section. Rectangular is worst case, hexagonal is best case. 

[quote="Maxid, post:24, topic:74424"]
Also the voltage sag seems to be lower on the 50E (I compared the lygte data for 7A for the 3P 50E pack and 5A for the 4P GA pack to get comparable currents for the individual cells) which should make for a very energy dense but still powerful ebike pack.
[/quote]
Did you also compensate for different discharge capacity? If you compare vertically in the graphs, you are catching both cells at different stages of the discharge cycle which will make the difference more pronounced than it actually is. For an appropriate comparison you have to shift to the right 40% as well. For example, the voltage sag at 5A when the GA cell has discharged 1Ah should be compared to the voltage sag at 7A when the 50E cell has discharged 1.4Ah.

When looking at those two in Henrik's charts, they match.
```

---
## \#27 Posted by: Darkie02 Posted at: 2019-07-05T13:18:32.923Z Reads: 25

```
[quote="PXSS, post:23, topic:74424"]
You’re looking at and comparing incomplete data. Henrik stopped the test for 30Q cells at 75C but lets the VTC6 reach a higher temperature (into the 80s) before he stopped the test.
[/quote]

Even befor the test stoped both of them VTC maintain less volt drop for longer.

[quote="PXSS, post:23, topic:74424"]
As I’ve stated before, with appropriate cooling, 30A per cell can be achieved on both 30Q and VTC6.
[/quote]

[quote="Maxid, post:1, topic:74424"]
(which can only take a 1P battery).
[/quote]

[quote="Maxid, post:1, topic:74424"]
Use case will be uphill to work for say 5min -
[/quote]

well I don’t know about you but I easily pull over 30amp up a hill sustained so for a 1p group that was originally asked about max discharge is hugely relevant IMO as that be the limiting factor 6 min discharge fine for a 5 minute journey.

As for cooling I’m sure if you cooled any battery enough you could get the desired output but doesn’t mean there’s not other better suited options out there.

Q30 are a very good middle ground but depending on you priority cost, discharge, charge, kWh density life span. Thay can always be beaten because thay are a compromise.
```

---
## \#28 Posted by: PXSS Posted at: 2019-07-05T13:31:25.749Z Reads: 23

```
@Darkie02 
You are correct in that VTC6s are slightly better as far as voltage sag goes, but not by much.

[quote="PXSS, post:12, topic:74424, full:true"]
I’ve run both cells to the ground and VTC6s are slightly better but does not justify the price difference. I prefer working with VTC6 because the button is slightly raised too.
[/quote]

[quote="Darkie02, post:27, topic:74424"]
As for cooling I’m sure if you cooled any battery enough you could get the desired output but doesn’t mean there’s not other better suited options out there.
[/quote]
My point with the cooling statement was that they ***both require cooling*** and about the same amount
```

---
## \#29 Posted by: Darkie02 Posted at: 2019-07-05T13:40:10.719Z Reads: 25

```
![image|281x500](upload://aKUkB9oDAY2FpWvCHRMzYLmMw3W.png) ![image|281x500](upload://aCYUyyv6X2LeIQbSOC03G1ezHby.png) 

The same argument can be applied the other way the 30Q are not that much cheaper. 24 cent let’s say it’s a standard 10s4p you save €9.60 on a €1000+ euro build. 

[quote="Darkie02, post:27, topic:74424"]
depending on you priority cost, discharge, charge, kWh density life span.
[/quote]
```

---
## \#30 Posted by: PXSS Posted at: 2019-07-05T13:41:13.033Z Reads: 25

```
8 months ago, that was not the case =)
VTC6s were about twice as expensive.
```

---
## \#31 Posted by: Maxid Posted at: 2019-07-05T13:49:35.571Z Reads: 23

```
[quote="PXSS, post:26, topic:74424, full:true"]
Did you also compensate for different discharge capacity? If you compare vertically in the graphs, you are catching both cells at different stages of the discharge cycle which will make the difference more pronounced than it actually is. For an appropriate comparison you have to shift to the right 40% as well. For example, the voltage sag at 5A when the GA cell has discharged 1Ah should be compared to the voltage sag at 7A when the 50E cell has discharged 1.4Ah.

When looking at those two in Henrik's charts, they match.
[/quote]

this I did not - thank you!
hm so looks like I will go for the GA pack - even though I thought I am super clever and the 50E is the way to go :see_no_evil:
```

---
## \#32 Posted by: Darkie02 Posted at: 2019-07-05T13:49:35.737Z Reads: 23

```
True but things move on and need re assessing. 

My first build I kept reading old posts and built a 25r pack because I believed things that were said with out evidence and opinions that were not updated. Combine that with manufactures stats and later realised the hard way I was wrong.

I think the 30Q is soon to be replaced by some thing same way the 25R was just unsure what will be the next standard we compare every thing against but o think it be very soon.
```

---
## \#33 Posted by: PXSS Posted at: 2019-07-05T13:56:43.238Z Reads: 22

```
With VTC6s being that cheap, I think they are already a replacement. I'd personally use the Sony cell over the 30Q always. But that's mainly because they're a lot easier to work with lol
```

---
