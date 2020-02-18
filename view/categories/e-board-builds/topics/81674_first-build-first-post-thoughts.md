# First build, First post. Thoughts?

### Replies: 15 Views: 335

## \#1 Posted by: MercKo Posted at: 2019-01-22T02:10:34.133Z Reads: 131

```
Hey all, I've been lurking this forum for a long time and have wanted to build a board for a long time and I've finally got the ability to start on a project but this is still new to me and I have some questions and would love to know if I'm going down the right or wrong path. 

I'll be using a Trampa HolyPro with the cable channel as the base, I'm about to order that first. 

I plan on using Trampa's Monster battery box, as well as their hangers, wheels, etc.

My intent on building this board is for alternative transportation on various trips I may take. The board would be mailed partially assembled and batteries bought on location unless you can help me find batteries that can be checked on flights or mailed easily, still looking into this, but the idea is it could drastically offset the cost of my transportation on those trips, even if I had to buy batteries wherever I took it from a hobby shop, I'd still save a lot, these trips can be 2-3 weeks on average so it's not like a weekend of ubering. I often want to head to another town for a day from wherever I am but using a train or long distance uber sucks, I'd literally rather stand for 2 hours and save the money and find cool stuff along the way. 

That said, many places I go tend to be hilly and can be hot. As I want this as a form of transportation, speed will gladly be sacrificed for reliability, climbing power, and low end torque. With that thought, I'm planning on using the Etoxx 80mm direct drive with helical gears. I plan to pair it with a 50-80kv 80mm motor. 

I want 80mm for the heat control, and better torque, low KV as I don't want or need to go over 20mph and anything around 10-15mph is sufficient. Direct Drive was chosen because it's a sealed system that can be oiled and offers helical gears which I need as suppressing noise is important as well.

If I'm using the 8" Trampa wheel, and 12s for each motor at 50-80kv geared 1:5, am I correct that would put me around 10-15mph? Or is that just too low of a KV to be viable at all? I can't find much info on low kv builds. I want to do twin 12s in the monster box to keep volts up, as that also helps keep the battery cool, is that right?

What would be good VESCs for a setup like this? This is an area I don't know much regarding. I want them to be able to be sealed in a water resistant case as well

oh and, despite using a 80mm motor and 80mm direct drive, do you think i could pick it up from the front and roll it on it's back drive wheels? or will the drive/motors hit the ground? 

Is this even the right direction for what I want, am I crazy, or would something like that be viable? Thanks for any input! I'm scared to mess anything up when so much of what I want will be international lol. I've not seen or heard much info on what it's like to ride a board with under 100kv, and very little info on 80mm either. if it seems viable, I'll be giving it a go and reporting my progress and updates here! This will be a slow build but once the Trampa deck arrives, I'll be seeing it through to the end.
```

---
## \#2 Posted by: tardyparty7 Posted at: 2019-01-22T02:13:09.442Z Reads: 117

```
ho damn. someone did their research...
```

---
## \#3 Posted by: MercKo Posted at: 2019-01-22T02:19:21.671Z Reads: 113

```
I try, but I'm still unsure, I learn hands on so a lot of this is still foreign and I'm not comfortable saying I'm correct with any of my thoughts until I've actually built a board lol. Just taking notes and learning and hoping I don't fudge everything up after I press "confirm" xD
```

---
## \#4 Posted by: J_Dizzle Posted at: 2019-01-22T05:29:32.022Z Reads: 96

```
You could go much higher kv, go for 190 if you can. Dual 6374 motors would be good. Pneumatic tires will effectively cut your range in half, so keep that in mind. If you go for something like a 12s8p liion battery pack you could go pretty far on one charge. By the way it does look like you have been lurking for quite a while, with your total of 5 hours of read time lol
```

---
## \#5 Posted by: Andy87 Posted at: 2019-01-22T05:41:47.378Z Reads: 90

```
Hi and welcome first!
According the 80mm motors, if you buy them because you think they can handle heat better than you unfortunatelly wrong. They heat up the same as 63xx motors as they also take more current.
You should be more than fine with dual 6374/6384 and 130-150kV.
If you want to travel with the board it will save you a lot of weight too.
I wouldn´t go below 100kV and for sure not over 190kV if speed is not your goal. 

According the esc, I would go with a VESC6 or any of the derivatives.
The VESC6 from Trampa is pretty expensive, but as you plan to buy most of your things from them anyhow, think about getting a pre build board from them and sell the parts you don't want or need.

If you get your gear drive from @nowind aka etoxx, get a bull bar too.
https://www.e-toxx-shop.com/trampa/bull-bars-bumper/#cc-m-product-10002752270
It will protect your gear drive from scrateches and makes it easy to take the board and move it around.
If you anyhow on the side, order some elsastomer dampers too and you have the perfect board for all conditions.
https://www.e-toxx-shop.com/trampa/elastomere-damper/#cc-m-product-10002752170
```

---
## \#6 Posted by: MercKo Posted at: 2019-01-22T06:07:09.480Z Reads: 76

```
Thx for the info, I only recently made the account so I could post :p
```

---
## \#7 Posted by: MercKo Posted at: 2019-01-22T06:37:08.781Z Reads: 77

```
heat was only one of the considerations for 80mm, I only considered heat benefits from extra metal, and more metal mass in the direct drive more so than how fast the motor heats up, I figured it could be a pro having extra metal mass to draw heat away from the motor mount area. Also, extra mass in the gears could lead to longer life was another thought. 

My other reason I considered 80mm was for being able to use very low KV which I, maybe mistakenly, assumed it would give me gobs of low end torque. Basically geared like a [crawler](https://www.youtube.com/watch?v=muVla81nML4), even though it's going very slow, there's still plenty torque to crawl it's way over things and *hopefully* granting a smooth, very low speed acceleration through most of the acceleration band. though I'm not sure how accurate my thinking on that is. 

I've thought about the VESC6 from trampa, but I've also seen a lot of other companies for considerable savings. Don't really know what's realistically better than others or what has good support or longevity. From what I've seen on Trampa I'm mixed on them anyways and would rather my money get spread around the community. I'm getting them because their board is very nice and I like their battery box. I'm going with their hangers and wheels because they look nice and the direct drive support from Jens. (I pref his product over Trampa's version for a few design reasons). Trampa also doesn't take my credit card, International and all, so no completes will be had. I'd rather build one bit by bit anyways, more satisfying in the end. 

Thanks for the links, though, I've been eyeing everything on Jens's site for a few years after I found his vids on Youtube, and then found this forum because of it. xD

I'm not dead set on 80mm, or anything, But also don't want to disband my train of thought if it's not totally wrong or just because it isn't the norm. I'm more interested in if it would function as intended or be a waste of effort vs a alternative that can offer basically what I've stated.

Appreciate your thoughts man.
```

---
## \#8 Posted by: Andy87 Posted at: 2019-01-22T06:49:47.462Z Reads: 62

```
don´t get me wrong, i´m totally with you if you don´t want to purchase more than needed from trampa. just don´t know your budget and a complete would save some overall money. 
There are some new maytech VESC6 200A coming. I´ll get a set to test them out unfortunately there no reviews to it so far.
If they would be available I would recommend you to get some ESCapes, but there is little changes that you can get some used.
Keep in mind, if you want big motors you also want big controller and big batteries to have an advantage from it.
I just got 2 8085s and they huge and heavy.
I would recommend you to get in touch with jens if you anyhow want to buy stuff from etoxx.
I think he can give you the right recommendations, he has more experience with big motors than most other people ;)

one thought more on the 80mm motors:
if you get a gear drive for 80mm motors you fixed to them,
as far as I know you even fixed to APS 80mm motors.
As min the Leopard 8072 has other hole pattern than the APS 80xx motors.
Maybe it´s more clever to buy a gear drive for 63xx motors and get an adapter (which jens also sell) for 80mm motors.
with it you free to use any kind of motor size you want.

do you have any experience in e-mtb riding so far?
```

---
## \#9 Posted by: MercKo Posted at: 2019-01-22T07:05:10.721Z Reads: 57

```
Thanks for the info man. You do raise a good point about brand dependence when using the 80mm, some of the places I'm going would not have APS for sure, let alone in 80mm. But I'm also not afraid of just carrying a spare. Good point though.

I'll look into some of those recommendations. 

and yea, I've ridden longboards since I was a kid, used to do normal mountain boarding, ridden a few electric boards from crappy Chinese companies that my friends bought but never liked any of them and always saw personal flaws in hub and belt motors so kept waiting and waiting until I felt like these products are ready enough for me to jump in. Trampa's small changes to the HolyPro and Jens offering the 80mm DD in Orange (even if it's sold out rn :( ) are what pushed me to actually start doing this rather than just eyeing things. 
Build budget is around 2-4 depending on what all I end up doing.
```

---
## \#10 Posted by: Andy87 Posted at: 2019-01-22T07:16:06.875Z Reads: 50

```
A lot of things you will just need to find out by your own.
I have a quad and now working on a super light board.
Some things are just so much more easy to handle if you have a light board.
I like to jump and make tricks and that´s just not possible with a 25kg board.
With 63xx motors I come everywhere and never had issues with overheating as min that´s my experience, but i also live a bit more in a colder region ;)
If you create your board, have the weight in mind.
2x 80100 are already like 4kg + the gear drive another 2kg or so.
the deck close to 3kg, the battery min 4-5kg... adds up fast.

one thing i want to let you know, I broke 2 APS motors in one day on different boards...and i´m not the only one in here which has problems with them. that´s said I can speak for now only for th 63xx motor size. the 8085s i couldn´t try yet i first need to send one of them back for replacement. the bearing was already broken from the factory....
so if you stay with APS motors, be ready to modify the motors to make them run reliable.
```

---
## \#11 Posted by: Trdolan03 Posted at: 2019-01-22T07:34:01.823Z Reads: 44

```
You could also look into @MBS products. @Nowind has begun to support them.
```

---
## \#12 Posted by: MercKo Posted at: 2019-01-22T07:44:06.723Z Reads: 43

```
Fair nuff. Weight actually isn't really a concern for this build, I've totaled the weight already for the entire build and don't find it concerning for how I'm intending on using it, but there are reasons regardless that have me on the fence for 80mm. Plenty of Pros if my pros are correct, but also plenty of cons. Reliability and ease of service are important considerations. 

long distance endurance, low speed across most of the slower acceleration curve, lower top speed (10-15), and gobs of torque, in a package that has a sealed drive unit that can be greased, is my goal. However is most reasonable to obtain my goal, I'll end up going with. 63 saves a lot of money, but I'm not convinced it will work entirely for my use case. That's why I'm ordering the board first and started this thread though. Input helps me come to conclusions, so thankyou.
```

---
## \#13 Posted by: Andy87 Posted at: 2019-01-22T07:54:33.368Z Reads: 43

```
i would try to get a hold of Jens. Write him about your plans to order his gear drive (and elastomer damper :stuck_out_tongue_winking_eye:) and I´m sure he will help you to find the right direction with motors.
Maybe consider also to include a AS5047 Encoder insteat of hall sensors.
As far as I know the etoxx gear drives have the option to add the pcb inside the gear drive. Better and smoother start up control you will not get than with the encoder.

Idk how much important range will be for you, but that is one thing you should keep in mind. Bigger motors, less range.
```

---
## \#14 Posted by: MercKo Posted at: 2019-01-22T08:20:37.931Z Reads: 43

```
I didn't know about the AS5047, thanks, That's along what I'm needing as well. 

and yea, I was planning on using the 6200Mah 6s Zippy batteries, 4 of them. 12s per motor. Was thinkin that would still get decent range yea?
```

---
## \#15 Posted by: Andy87 Posted at: 2019-01-22T08:30:00.645Z Reads: 44

```
Yap that should give you some good range.
If you have the money, investigated better in the graphen lipos. They hold up more charge cycles than the zippys. Also not sure about the c-rating of the zippys. Wouldn’t go under 45c in a 2p configurations if you want to use 80xx motors.
Again just my personal opinion 😜
```

---
