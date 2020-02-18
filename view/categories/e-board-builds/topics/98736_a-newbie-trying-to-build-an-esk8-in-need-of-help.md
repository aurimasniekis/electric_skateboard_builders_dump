# A Newbie trying to build an esk8 in need of help

### Replies: 46 Views: 401

## \#1 Posted by: Matamoros_2002 Posted at: 2019-07-19T04:05:54.416Z Reads: 106

```
Its been quite some time (like 8-10 months) since I've started inquiring about esk8, and now I want to build mine I don't have a huge budget but still need help deciding what to choose for the board. I am around 170 - 180 lbs.

Weight: I really don't care much about the weight but I care more about the range 

Speed: I don't really care about it being extremely fast (30 mph) but some good 18 to 20 mph will do

Range: I actually want it to have a long range of about 18 miles will do

Batteries: I don't know that much about them all I know is that a lot of people recommend the 18650 the ones in the Teslas I believe

Motor: I am trying to decide between the in hub and belt one since I've heard that when you run out o charge the belt ones are really hard to push. They have recommended me that for the in hub motors to be around 75 kv and 90mm with swappable urethane and for the belt to be 64something and around 200 kv

VESC or ESC and Controller: this I know nothing of sorts so all help would be appreciated

Board itself: I want the board to be a longboard and the style like the boosted board (downhill style I believe) 

I don't know if I need anything else, if im missing something please tell me.
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-07-19T04:19:46.416Z Reads: 95

```
It would help us to know the specific number of your budget before we go and reccomend parts

Remember a board is made from 
* Deck 
* Trucks
* Motors / motor mounts
* Wheels 
* Enclosure
* Battery
* VESCs
* Reciever/ Remote 
* Charger
* Optional other parts such as a Metr module / led lights / etc
```

---
## \#3 Posted by: Matamoros_2002 Posted at: 2019-07-19T04:34:42.421Z Reads: 84

```
I actually don't have a specific number since I can go on buying as I get more money, but around some 500-700$
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-07-19T04:59:27.483Z Reads: 77

```
Hubs aren't resistance-free when off and pushing, even when disconnected entirely. With belt drive, you can always remove the belt and it then behaves just like a regular unpowered board. One deciding factor between belts and hubs is hills - if you live somewhere hilly, you probably want extra torque to get up them, and belt drive is perfect for this.

One thing you need to figure out is physical size - nothing worse than picking a battery etc, then not being able to fit it all into an enclosure, or worse, not being able to find an enclosure that fits your board. I'd recommend picking your enclosure first, then your board, or at least checking that whatever board you have in mind has enclosures that will fit it. Then you can choose your electronics to suit the enclosure/board combo.
```

---
## \#5 Posted by: Sn4pz Posted at: 2019-07-19T12:30:20.196Z Reads: 58

```
Your budget seems perfect for a single drive with a 12s3p battery, adding the second motor and vesc would likely push your budget over the limit

12s3p Battery (including charger) - $350

Motor - $100 

Vesc -$80

Deck (Vanguard clone and Meepo style enclosure to mimic a boosted **Just make sure the battery fits the enclosure**, I remember seeing one that fits a 10s3p, so 6 extra cells might not be too much...) - $120

Chinese clone wheels - $20 
Pulleys -$50

Remote -$50 

I estimated on some of the pricing, and you could probably get some of the items for cheaper if you bought used, but this in my mind is the minimum for an 18 mi range board. 

My 10s2p only squeeks out 11 miles before sag becomes too much of an issue to ride. Past mile 6 it's slower than a full charge, and I only draw 12a from each Pgroup

Just remember that safety is the number 1 priority, and you shouldn't skimp on the vesc, controller or safety gear (which isn't written here). 

Send us links to products you think would work in your build and we can tell you what's good or bad
```

---
## \#6 Posted by: Matamoros_2002 Posted at: 2019-07-19T13:22:08.674Z Reads: 48

```
Perfect, thanks. I will be looking around some products this days and ill send you some as soon as I have.
```

---
## \#7 Posted by: Matamoros_2002 Posted at: 2019-07-19T13:55:23.676Z Reads: 44

```
Perfect, thanks. About that you said of removing the belt can I do it on the go or do I have to disassemble the whole thing? and where I live it is weird since I live up a hill and I believe that it is actually like 80 degrees as soon as I can ill upload a picture, but the rest of the city has minimal hills. Still I believe I'll go with the belt since I am scare of running out of battery and having to carry it.
```

---
## \#8 Posted by: Matamoros_2002 Posted at: 2019-07-19T13:56:04.620Z Reads: 41

```
Also, what does 12s3p and 10s3p mean and could you explain the difference please
```

---
## \#9 Posted by: Blitz Posted at: 2019-07-19T14:14:08.539Z Reads: 42

```
My dude my advice if you have a job put in some overtime it will cost less in all aspects for you mentally and physically

Buy a nice deck with an enclosure to go with it (seems like a rip off but eh) Go for direct drive get some nice wheels and happy days.
```

---
## \#10 Posted by: Matamoros_2002 Posted at: 2019-07-19T14:47:32.203Z Reads: 41

```
yeah that sounds good, just one problem im 17 hahahaha still undergraduate
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-07-19T14:54:45.043Z Reads: 42

```
So for esk8 batteries we talk in terms of cells in **S**eries and **P**arallel, S and P groups. 

More cells in Series results in a higher voltage, which correlates to higher speed and increased torque

More cells in Parallel would result in larger pack WH, aka more range. 

However I reccomended the 12s3p simply based on my observation that: With a battery made from Samsung 30q cells, each Ppack in a 10s pack seems to offer around 6 miles of range. 

The 30 cells of a 10s3p pack would give you around 18 miles, but the 36 cells of a 12s3p pack would likely give you 20 miles (10-14 quick-ish miles, and 5-6 miles of sag speed). 

That being said, your range is entirely dependant on how you program your VESC( Don't worry about doing this yourself, unless you read into it extensively. We can help you with that as well 👍)

Feeding your motors a higher amperage will drain the battery pack faster, and shorten your range.
```

---
## \#12 Posted by: Blitz Posted at: 2019-07-19T14:55:05.769Z Reads: 34

```
soo whoops,

I'm in the same shoes as you, well then learn to make your own 18650 pack (biggest bucks can be saved right there)
```

---
## \#13 Posted by: Blitz Posted at: 2019-07-19T15:00:29.582Z Reads: 35

```
[quote="Sn4pz, post:11, topic:98736"]
More cells in Series results in a higher voltage, which correlates to higher speed and increased torque

More cells in Parallel would result in larger pack mAh, aka more range.
[/quote]

---___---

WATTAGE, WH pls 

Parallel = more current 
More current = more wattage and on the same rpm that wattage should  = more torque (if the esc motor conbo can handle it.)
```

---
## \#14 Posted by: Sn4pz Posted at: 2019-07-19T15:07:55.910Z Reads: 27

```
Lol fixed it 

(づ￣ _￣)づ
```

---
## \#15 Posted by: Blitz Posted at: 2019-07-19T15:10:31.488Z Reads: 32

```
mAh was technically correct, 

IT's just I don't want this guy thinking on if i go 1s 30p I'll get more range.

or think that if he goes 10s1p he'll have speed and lots of hill climbing torque.

(please take caution when liking blitz's comments when they have just been created
they can change in a split second) I will not be held liable for any embarrassment caused.
```

---
## \#16 Posted by: Blitz Posted at: 2019-07-19T15:34:33.968Z Reads: 33

```
[quote="Matamoros_2002, post:1, topic:98736"]
Board itself: I want the board to be a longboard and the style like the boosted board (downhill style I believe)
[/quote]

Downhill oh boy lol,
boosted deck is perfectly fine for 20mph but it's not what I'd consider to be a downhill deck because downhill decks tend to be stiff and have little to no flex but can handle 30mph easy.

[quote="Matamoros_2002, post:1, topic:98736"]
Range: I actually want it to have a long range of about 18 miles will do
[/quote]

Range let's focus on how much energy you could eat
The main  non complex factors are

* how much the load is (your weight) 

* Your speed (the faster you go the more wind resistance)

* the incline or decent of your route (this is where weight really factors in)

* How fast you accelerate aka ride (take a bike ride and pay attention to these factors so you would have a good understanding the above)

Now if you drive efficiently you might get 1km of range per 10wh but there are many variables.

[quote="Matamoros_2002, post:1, topic:98736"]
Batteries: I don’t know that much about them all I know is that a lot of people recommend the 18650 the ones in the Teslas I believe
[/quote]

Samsung Q30's are a great choice for esk8 Because they are

* High in capacity

*  high drain

There are some higher capacity cells but they either cost more or don't provide a lot of output unless you put a lot together.

@Matamoros_2002 Do you follow?
```

---
## \#17 Posted by: s5300 Posted at: 2019-07-19T16:10:30.083Z Reads: 30

```
I might try to reply with something more informative later, however, this is what I want to say now.

For your first build, I highly recommend not trying to do every single cool thing the community has came up with in the past 4 or more years, and even experimental shit on top of that. Also, make a build list with PARTS THAT ARE IN STOCK AND KNOWN TO SHIP WHEN PURCHASED FROM RELIABLE VENDORS. 

After your first build, do whatever the fuck you want. But for your first... heed my advice. Also, I'd definitely build the board to be able to go at least 25mph.... once you get comfortable topping out you're gonna want more.
```

---
## \#18 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:35:22.999Z Reads: 29

```
thanks for that on the topping out part
```

---
## \#19 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:35:39.616Z Reads: 29

```
perfect I'll be taking that into account
```

---
## \#20 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:35:59.481Z Reads: 29

```
understood everything perfectly thanks for the output
```

---
## \#21 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:39:05.851Z Reads: 28

```
also I was thinking of buying this one: https://www.amazon.com/gp/product/B07PCHM6KW/ref=ox_sc_act_title_2?smid=A1NYT505ZNPIKK&psc=1
or this one: 
https://www.paeanboard.com/PAEAN-37-ELECTRIC-SKATEBOARD-H2B-Max-p1155284.html
or this one:
https://www.paeanboard.com/PAEAN-37-ELECTRIC-SKATEBOARD-H2B-Max-p1155284.html

which one would you recommend me? or should I build a cheap one and then go upgrading from there?

for my first so then I can save up and star buying little by little meanwhile having a good way of transportation so I don't have to pay everything by the bunch.
```

---
## \#22 Posted by: Blitz Posted at: 2019-07-19T17:39:47.981Z Reads: 25

```
Meepo

IS the better pick they've been at it for a long time and I hear they provide decent customer service
```

---
## \#23 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:40:36.833Z Reads: 24

```
about how much is a meepo? does I have good range? as the advertised on the strailboard
```

---
## \#24 Posted by: Blitz Posted at: 2019-07-19T17:41:01.106Z Reads: 26

```
IF, they have a sanyo 21700 10s2p battrey in there than maybe otherwise it's a lie.
```

---
## \#25 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:42:27.704Z Reads: 27

```
oh ok perfect
```

---
## \#26 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:43:19.566Z Reads: 27

```
didn't quite understand that tho hahahaha
```

---
## \#27 Posted by: Blitz Posted at: 2019-07-19T17:43:52.435Z Reads: 26

```
With these chinise boards, there are only so many battrey options all these companies copy eachother

and I only saw a 10s2p sanyo variant provide anything near the 30km mark
```

---
## \#28 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:44:49.257Z Reads: 26

```
perfect ill check on that
```

---
## \#29 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:47:30.467Z Reads: 24

```
**Battery:**  Strailboard V2 Pro come with double discharge rate of 30A improved battery,you can mailtain high speed with low running battery.

this is what their page says about the battery
```

---
## \#30 Posted by: Blitz Posted at: 2019-07-19T17:49:57.395Z Reads: 27

```
check the amazon questions section the seller said the range is 19km

https://www.amazon.com/gp/product/B07PCHM6KW/ref=ox_sc_act_title_2?smid=A1NYT505ZNPIKK&psc=1

but it is cheap and from amazon. But I don't know IF i'd recommend it.
```

---
## \#31 Posted by: Matamoros_2002 Posted at: 2019-07-19T17:55:35.326Z Reads: 27

```
oh ok thanks
![39%20AM|473x500](upload://hzjSUsRs7OJN7pH8iEreQGjLRpz.jpeg) 
this is what it says about the battery I believe the one it comes with is the Sanyo
```

---
## \#32 Posted by: Blitz Posted at: 2019-07-19T17:58:53.608Z Reads: 25

```
Sanyo battrey is nice.

how much for the board with the sanyo pack got a link for me to inspect?
```

---
## \#33 Posted by: Sn4pz Posted at: 2019-07-19T18:00:57.296Z Reads: 26

```
I would go for a meepo as well, their ER (extended range) battery is made from quality cells, and can serve as a starting point for a build after you move past your meepo.

All of these other "powerful packs" from Chinese manufacturers are bs, they can't hold a candle to quality cells

Imo the only cells worth building a battery from are: Samsung 30q, 30T, 40T, and 50e , LG VTC5, VTC5a, VTC6, Sanyo cells ( there are many, I can't remember the numbers. ) 

Generally speaking 20700/21700 cells are better than 18650, but it all depends on your use case
```

---
## \#34 Posted by: Matamoros_2002 Posted at: 2019-07-19T18:12:19.337Z Reads: 26

```
this link is where I found it
https://strailboard.com/products/strail-electric-skateboard-battery?_pos=3&_sid=653028a26&_ss=r
```

---
## \#35 Posted by: Matamoros_2002 Posted at: 2019-07-19T18:13:13.784Z Reads: 25

```
perfect, the thing is that the meepo with ER is like 650$
```

---
## \#36 Posted by: Matamoros_2002 Posted at: 2019-07-19T18:13:26.235Z Reads: 25

```
I don't have that money all at once
```

---
## \#37 Posted by: Blitz Posted at: 2019-07-19T18:14:32.531Z Reads: 25

```
I feel ya man but that other board is risky.

with the meepo adleast you'll be broke but with a decent board.

not to mention better deck and trucks GTG ttyl guys
```

---
## \#38 Posted by: Matamoros_2002 Posted at: 2019-07-19T18:19:56.567Z Reads: 22

```
yeah, think ill  just save more hahaha

it is either the meepo ER or the Skatebolt Tornado
```

---
## \#39 Posted by: MysticalDork Posted at: 2019-07-19T19:00:43.574Z Reads: 27

```
[quote="Matamoros_2002, post:7, topic:98736"]
About that you said of removing the belt can I do it on the go or do I have to disassemble the whole thing?
[/quote]

It really depends on your exact setup and parts. My last build, you could slip the belt off the pulley and extract it over the wheel, with a little effort. Worst comes to worst, you can always carry a skate tool and/or a couple allen wrenches in a backpack and use them. Absolute worst emergency solution (busted board, no tools, gotta push to get home) you can just cut the belt off and replace it. A $3-5 replacement belt, and you're good to go again!
```

---
## \#40 Posted by: Matamoros_2002 Posted at: 2019-07-19T20:19:09.335Z Reads: 27

```
yeah that's good, but I don't live in the US so that might be sort of a problem, but I believe that with some research I can find some belts in my country
```

---
## \#41 Posted by: MysticalDork Posted at: 2019-07-19T20:42:25.484Z Reads: 24

```
Where do you live?
```

---
## \#42 Posted by: Sn4pz Posted at: 2019-07-19T21:27:37.264Z Reads: 24

```
[quote="Matamoros_2002, post:38, topic:98736"]
it is either the meepo ER or the Skatebolt Tornado
[/quote]

No competition in my mind, meepo all the way. 


...unless you want to save several hundred more and build a banger of a DIY board :P
```

---
## \#43 Posted by: Blitz Posted at: 2019-07-19T23:52:56.768Z Reads: 21

```
@Matamoros_2002 Where are you from and what dollars are you quoting?
```

---
## \#44 Posted by: Matamoros_2002 Posted at: 2019-07-20T09:46:11.475Z Reads: 18

```
Im from Costa Rica, but I'm traveling to the US and was hoping to buy my board there
```

---
## \#45 Posted by: Blitz Posted at: 2019-07-20T18:42:37.973Z Reads: 19

```
[quote="Matamoros_2002, post:44, topic:98736"]
traveling to the US
[/quote]
That's tricky,

parts can come later damaged or you could of bought the wrong thing,
esk8's are almost never done right the first time. and even if all is well don't forget to make a plan on how to bring an esk8 back home because airports might want to confiscate it because it has a (bigish) battery.
```

---
## \#46 Posted by: Matamoros_2002 Posted at: 2019-07-21T06:44:25.713Z Reads: 13

```
also the yeah, but I believe I won't be doing it this time since I have bigger priorities but still thanks for all the help given from all of you
```

---
