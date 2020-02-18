# Advice on how to continue my build

### Replies: 17 Views: 892

## \#1 Posted by: Zimbombe Posted at: 2018-02-07T18:04:33.061Z Reads: 202

```
So last year around the same time i started my first build and it was a great experience overall
even if i had a lot to learn. 


https://www.electric-skateboard.builders/t/human-instrumentality-project-6s3p-single-racerstar-140kv-5065-custom-deck-battery-box-holder-fvt-120a-esc/32737/26

I have a 6s3p setup made with Samsung  18x Samsung 30Q a 60s Bms and these very beautiful battery holders

battery holders- https://www.banggood.com/5Pcs-E1A1-ABS-Battery-Box-Holder-For-4-x-18650-p-964192.html?rmmds=myorder&cur_warehouse=CN


BMS- https://www.aliexpress.com/item/13S-100A-bms-2016-new-Li-ion-48V-100A-large-high-current-BMS-PCM-with-different/32759040792.html?spm=a2g0s.9042311.0.0.2pWKnp 

motor- https://www.banggood.com/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html?rmmds=myorder&cur_warehouse=CN

It worked pretty good besides one minor problem, Voltage sag. It almoast dropped from 100% Load to ~65% Load under full throttle which was imo mainly caused by the esc i used (some members of the forum told me so)



    So a new year and a new try. 
I have build myself a Spot welder, bought a 10s BMS and a vesc (and anti spark switch, bluetooth module) thx to @rich .
My plan was to go for 12 more 18650´s and go for a 10s3p by using my old batteries too but now i´am not sure anymore if it would be a good idea to mix up my used battieres with some new ones.
From what i saw my batteries shouldnt be damaged that much and can hold still around 4.08 - 4.15 V.

    My question now is 

Would you suggest to either,

- use my 18 old batteries and build a proper 6s3p battery pack with my spot welder ?

- use my 18 old batteries, buy 12 new and build a proper 10s3p battery pack with my spot welder ? 

- buy 20 or 30 18650´s and build a proper 10s2p or 10s3p battery pack with my spot welder ?



I really prefer option 1 if i could get the same performance with now a proper Vesc and WITHOUT the Voltage sag problem i had before, but some ppl. here mentioned also that the low Voltage of my system could be a part of the problem.

Sorry for the long thread and thx in addition for any help.
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-02-07T18:31:41.996Z Reads: 158

```
I wouldn’t recommend mixing used 30q cells with new ones since they probably different capacity. Be safe and pour in the xtra $ for a new pack 😏

Also think about using the bms for charging only that way you can secure your breaking when the battery is full and spent less money on a low amp output bms
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-02-07T18:37:34.918Z Reads: 156

```
As long as your cells are the same type and you haven't put an excessive amount of wear on the old cells, option two will work. If the old cells are well-used, it's definitely a better idea to make a whole new pack. 

You will always get some voltage sag. 18650 cells sag more than lipo cells of the same capacity, which is why most 18650 builds have a minimum of 3p, and usually 4p or more, to compensate for the sag.

Make sure to practice a lot on some old crappy laptop cells before trying to weld your nice 30qs. look on the forum, find good pictures of welds and packs to guide you. Make SURE you know what you're doing and how not to end up with a fireball.
```

---
## \#4 Posted by: ZackoryCramer Posted at: 2018-02-07T18:42:01.743Z Reads: 137

```
Would you recommend using the old cells in parallel or mix them with the new in parallel? My prediction is that mixing cells in parallel would damage the new cells and separating them in series would put more stress on bms
```

---
## \#5 Posted by: MysticalDork Posted at: 2018-02-07T18:43:38.801Z Reads: 122

```
It would be best to have the P blocks have an even mix of old and new cells. Having some with all old and some with all new is just asking for an unbalanced pack.
```

---
## \#6 Posted by: Zimbombe Posted at: 2018-02-07T19:07:27.388Z Reads: 121

```
[quote="MysticalDork, post:3, topic:45823"]
As long as your cells are the same type and you haven’t put an excessive amount of wear on the old cells, option two will work. If the old cells are well-used, it’s definitely a better idea to make a whole new pack.
[/quote]

Am i able to see how good they still work only by looking up how many V max. they still can hold ? If so i would just charge them one by one with a 18650 charger and see for which option i go.

[quote="MysticalDork, post:3, topic:45823"]
You will always get some voltage sag. 18650 cells sag more than lipo cells of the same capacity, which is why most 18650 builds have a minimum of 3p, and usually 4p or more, to compensate for the sag.
[/quote]

So your Advise would be to go for 6s4p instead of 10s3p ? and am i able to handle the Voltage sag better by using a Vesc then instead of my old China Esc ?

[quote="MysticalDork, post:3, topic:45823"]
Make sure to practice a lot on some old crappy laptop cells before trying to weld your nice 30qs. look on the forum, find good pictures of welds and packs to guide you. Make SURE you know what you’re doing and how not to end up with a fireball.
[/quote]

I don´t know if i have the chance to practice but i´ve been through all Videos of 

https://www.youtube.com/channel/UCRMrqzsrPIWvY3PINkLKs-Q

, looked up several threads of diy battery packs and offcourse will ask the forum again once i´ve set everything up and made a wiring scheem
```

---
## \#7 Posted by: Zimbombe Posted at: 2018-02-07T19:09:47.213Z Reads: 91

```
[quote="ZackoryCramer, post:2, topic:45823"]
Also think about using the bms for charging only that way you can secure your breaking when the battery is full and spent less money on a low amp output bms
[/quote]

I´ve heard about this multiple times now here and will have a closer look at it, thx mate.
```

---
## \#8 Posted by: ZackoryCramer Posted at: 2018-02-07T19:10:42.032Z Reads: 87

```
[quote="Zimbombe, post:6, topic:45823"]
So your Advise would be to go for 6s4p instead of 10s3p
[/quote]
No. The more POWER/current a cell outputs the more sag. Having a lot cells in a p block doesn’t necessarily mean less sag. Since 10s3p has 6 more cells than 6s4p you would have less sag from outputting the same power.

And all esc’s probably are probably similarly efficient, using a cheap esc doesn’t make you output more power, they could be power limited.
```

---
## \#9 Posted by: rich Posted at: 2018-02-07T19:59:31.238Z Reads: 79

```
Hey, looking forward to see the progress of your build!

Don't bypass your BMS, it has 120A over current and 4,25V over charge protection. If you don't break for kilometers after a full charge you don't have to worry about that but you have good safety for your cells. I have the same BMS in 10s, it's cheap.

I would recommend upgrading to 10s, the vesc will run cooler and you'll get more top speed with 140kv (depending on your gearing). New 10s BMS plus 2-3A charger is about 50€ :sunglasses:
```

---
## \#10 Posted by: ZackoryCramer Posted at: 2018-02-07T20:10:11.969Z Reads: 73

```
[quote="rich, post:9, topic:45823"]
120A over current and 4,25V over charge protection.
[/quote]
 The current protection is legit but since you put it in parallel for charging, you get the charging protection. And I don’t know about you but I can’t get away without breaking for a kilometer
```

---
## \#11 Posted by: MysticalDork Posted at: 2018-02-07T20:10:45.764Z Reads: 70

```
If you have a balance charger like an imax B6 or similar, you can test the capacity of your cells. The final charge voltage means nothing, all lithium ion batteries end at 4.2v.

You need to PRACTICE welding cells, not just watch videos. Get some old busted laptop batteries, they're common as dirt. Take them apart, and use them to practice.

6s is really low for esk8 applications, the low voltage means you need a LOT of current to get a decent amount of power. By going for a 10s setup, the voltage goes up, so the current goes down.

You should still go for at least a 10s3p, 2p is just awful for sag. 4p would be better.
```

---
## \#12 Posted by: rich Posted at: 2018-02-07T20:30:10.483Z Reads: 70

```
[quote="ZackoryCramer, post:10, topic:45823"]
And I don’t know about you but I can’t get away without breaking for a kilometer
[/quote]


True :joy: 
No I meant if someome lives on top of a hill and start his ride with continious braking for kilometers
```

---
## \#13 Posted by: MysticalDork Posted at: 2018-02-08T02:32:29.535Z Reads: 58

```
That's how my rides start. I live on a bigass hill.
```

---
## \#14 Posted by: TarzanHBK Posted at: 2018-02-08T11:34:23.242Z Reads: 51

```
Interesting find with old and new cells.
@PXSS Patrick what´s your point of view with mixing them parallel or series?
I thing parallel would work too
```

---
## \#15 Posted by: PXSS Posted at: 2018-02-08T12:33:31.605Z Reads: 55

```
I'm a little iffy about this topic. I hate seeing old batteries go to waste but I don't want to recommend mixing old and new cells unless you do it properly. 

Is it possible?
Heck yeah. 
Is it simple?
Not very. 

The main reason why you are not to mix old and new cells is that as cells get cycled, their IR (internal resistance) rises and the capacity they hold diminishes. These two are related. To charge a battery, you apply a voltage (4.2v) to it with a current limit of course (usually 1.5A per cell) while the battery sits at a lower voltage. A low IR means that for the same voltage difference, you will have less energy lost to heat.

For example, new cell A has IR of 20mO, while old cell b has IR of 100mO. Both of them are sitting at 4.1V and you apply 1A to them. Cell A Voltage will rise to 4.12V while cell B will rise to 4.2V, therefore cell B is closer to fully charged than A. A could take 5 times the energy before it reaches the same voltage as B. 

Why is this an issue?
Higher IR means your cells charge and discharge faster at the same current (have less capacity) than new cells.
If you have them in series and you don't have any individual cell protection (like a discharge bms), by the time you hit your low voltage cutoff on the whole pack (lets call it 28V on a 10S) your new cells could be sitting at 3.2V while your old cells are at 2.4V. (I did not choose these numbers at random, between 3.2V and 2.5V, you usually have 10-15 percent left, and if there is a 10-15% capacity difference between your old and new cells then it would be easy to get caught in this situation.) This would mean that you over discharged your old cells and further damaged them. Eventually, you will either overcharge the bad cells, or over discharge them to the point that thermal failure is possible. 

If you have the cells in parallel, you have a little more protection in that the old cells will always be at the same voltage as your new cells so you cannot over discharge or charge them that easily. The issue here is, that the new cells get loaded harder than the old ones, because their ir is lower. Not only this but the old cells also run hotter dissipating heat into the new cells. What this means is that the new cells are getting worn down at a much faster pace than normal. The capacity you get from a pack like this will lie somewhere between the capacity of the new cells and the old ones as opposed to being truncated by the old cells capacity in a series pack. 

Series vs parallel mix new and old
Series pros:
New cells dont get accelerated wear
Easy to see and monitor difference in voltage and capacity of new and old cells
Easy to separate if necessary 

Series cons:
Reduced capacity of whole pack to old cells capacity 
Easy to over discharge and over charge
Needs monitoring 
Higher chances of fire failure if unprotected and not constantly monitored

Parallel pros:
Capacity is as high as can be
Less likely to over discharge and over charge
Requires less monitoring

Parallel cons:
Reduced life of new cells
Cannot easily separate old cells from bew. 
If failure does occur, new cells have to be replaced as well. 
Cannot monitor the health status difference between new cells and old cells. 

---
What I would do if I had to mix cells:
Use a charge/discharge BMS for protection
Use conservative ESC settings
Wire new and old cells in series and monitor health status constantly. 
Charge with balance charger and keep an eye on capacity differences.
```

---
## \#16 Posted by: Zimbombe Posted at: 2018-02-08T13:45:01.759Z Reads: 47

```
Thank you so very much these are a lot of very helpfull comments, i really like the in depth thoughts of @PXSS .

So i will get a friends 6s balance charger, see how worn the 18650's are and then post some results here.
But with the concerns of @PSXX I'll probably try to sell my old batteries and get 30x new batteries.

Luckely i have already bought that 10s bms you have @rich.
```

---
## \#17 Posted by: Zimbombe Posted at: 2018-02-28T12:05:18.650Z Reads: 39

```
I finaly have the 6s Charger from a friend which is also capable of showing the capacity....kind of... and a Capacity tester. The problem is that i´m not sure what to do to see how much capacity can hold. 
I really would like to know how worn my batteries can hold so i can sell them.

Can somebody help me ?

![20180228_115925|281x500](upload://5PUWOcU6PMwim9sox3YyZH6ICnS.jpg)

6s Charger :

http://www.carson-modelsport.com/CommonFiles/Dickie-Tamiya/PDM_Products/Carson/500606035/500606035_ExpertChargerDuo_en.pdf


Capacity Tester:

https://www.d-edition.de/RC-Modellbau-Zubehoer/Elektronik/Sonstiges/CN-Yuki-Model-Digitaler-Akku---Batterie-Tester.html?utm_source=google&utm_medium=shopping&utm_campaign=gs&gclid=EAIaIQobChMI8e6MwsfI2QIVDeAbCh3Zzw34EAQYAiABEgIlafD_BwE
```

---
