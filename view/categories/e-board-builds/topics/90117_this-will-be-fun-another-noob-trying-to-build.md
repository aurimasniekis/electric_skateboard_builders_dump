# This Will Be Fun! Another noob trying to build

### Replies: 27 Views: 319

## \#1 Posted by: HixStix6 Posted at: 2019-04-11T05:22:59.117Z Reads: 102

```
First off, I'm a boarder. I never played with rc. I was at a skatepark, mountain, lake, or ocean. I love boarding, all of them. So i've finally made it here. I need an esk8. I dont know my way around a circuit board but i can build giant buildings so how hard could it be? What you guys do here is extremely challenging. This is my first build. Any advise will be greatly apprieciated.

Trampa Carver
Vertigo Trucks
Hypa hubs
@idea motor mounts
@idea pulleys
2 x Hobbysky 6384 170 kv sensored
Dual FSESC6.6 Plus based on VESC6
2.4Ghz Remote VX1 flipsky remote and reciever
Anti spark Switch Smart 280A flipsky
Bluetooth Module 2.4G Wireless Based upon the nrf51_vesc project
2 x Gens ace 6200mAh 22.2V 60C 6S1P Lipo Battery

i think i still need a bms and a charger. Any suggestions? Thanks in advance!
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-04-11T05:31:04.835Z Reads: 97

```
I personally don't like electronic antispark switches, they have a tendency to fail at inopportune times - A regular XT90-S loopkey is the gold standard in my book for simplicity, cost and reliability.

6.2Ah of batteries won't give you much range, especially with pneumatic tires - I'd guess less than ten miles if you're riding conservatively, and probably more like five or seven if you're going hard. For a mountainboard (I assume you are going that way beased off your trucks and hubs), I'd recommend at least 15Ah, and li-ion instead of LiPo.
```

---
## \#3 Posted by: Dirt_Bag Posted at: 2019-04-11T05:33:07.622Z Reads: 90

```
The parts list is alright. For a learner, dual 6384 is massively powerful. The hobbysky ones seem to have a lower amp rating than advertised. For a mtb, you want a bare minimum of 10ah worth of batteries. I would recommend going with a 12s6p or 8p 18650 pack, or build a 12s3p pack using turnigy 5000mah batteries. 

Dont rush into this and make mistakes. Most people have already made several boards before they build a mtb
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-04-11T05:34:20.500Z Reads: 83

```
I get 5 miles off an old 10s 10ah lipo on dual 6374. The batteries dont sag and have the rated capacity. Riding style chews through 10ah in very little time.
```

---
## \#5 Posted by: Andy87 Posted at: 2019-04-11T05:35:13.845Z Reads: 83

```
[quote="MysticalDork, post:2, topic:90117"]
XT90 loopkey
[/quote]

I agree with that but please use a xt90s (anti spark version) of the xt90 as loopkey. 

I get like 7-10km out of my 5Ah packs if I go hard, so I would assume like 9-12km on those.

The rest looks good so far. If you ever want to change to gears, I have some new sprockets for hypa hubs laying at home 😉
```

---
## \#6 Posted by: HixStix6 Posted at: 2019-04-11T05:35:43.802Z Reads: 73

```
Great info. i was trying to save money. I would like to ride it hard up and down hills. Ten to fifteen miles seems like a lot of riding.
```

---
## \#7 Posted by: HixStix6 Posted at: 2019-04-11T05:37:39.461Z Reads: 67

```
Great. Now i'm nervous. I've bought everything but the battery pack:fearful:
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-04-11T05:38:02.140Z Reads: 67

```
True, but you'd be surprised how quickly that goes by. Especially when going up hills - That drains the tank faster than anything else. With a big battery, you also don't have to charge it each time. Just top it off when it gets low, and you've got several rides' worth in there.

One of the most often mentioned complaints I see on budget builds is something along the lines of "Dang, I wish I'd bought bigger batteries", or "How can I add more batteries to my existing pack? My range sucks."
```

---
## \#9 Posted by: Andy87 Posted at: 2019-04-11T05:40:07.275Z Reads: 66

```
[quote="HixStix6, post:1, topic:90117"]
i think i still need a bms and a charger.
[/quote]

I like to use a hobby charger to put my lipos into Storage charge when I didn’t used a pack of them. That’s always handy and an easy imax b6 does the job pretty slowly but good.
To charge up my packs I use a 8A charger with a smart bms which allows my to monitor the individual cell voltage
```

---
## \#10 Posted by: Dirt_Bag Posted at: 2019-04-11T05:41:10.750Z Reads: 62

```
Dont be afraid! Its a great hobby! Just be careful. You are building something capable of popping a wheelie and planting you on the ground. Honestly, i would try dual 6374. It works for me VERY well. I weight 215lbs or so. Take it slow and if you need help, ask. Building it right the first time with good parts saves you alot of money 

If you have parts already, just limit the current while you learn.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-04-11T05:42:38.718Z Reads: 56

```
Thats not an issue with a top mount lipo pack. Easy to swap. If you need more range just buy two more packs and good. More weight on the board makes the ride more uncomfortable for me. So i‘m pretty happy with a 5Ah pack and a fast swap system
```

---
## \#12 Posted by: Dirt_Bag Posted at: 2019-04-11T05:43:31.331Z Reads: 55

```
Exactly this. Your range is halved at a minimum if you are offroading. A 25mi pack on a mtb would be great. It would give you plenty of offroading time
```

---
## \#13 Posted by: Dirt_Bag Posted at: 2019-04-11T05:44:56.151Z Reads: 55

```
Just be careful on the brand of lipos. With how short some lifespans are you really cant mix them if they have been used more than a few times. (Zippy, older gen graphene, multistar, nanotech)
```

---
## \#14 Posted by: MysticalDork Posted at: 2019-04-11T05:47:41.441Z Reads: 56

```
@Andy87 is of the fast-swap school of thought. I am of the big-battery school. Plus, with a really large pack, you don't need 60C batteries, because the drain is distributed across more cells in parallel. 

I don't like taking my stuff apart once it's done - I like having it all buttoned up and self contained - no balancing and storage charging outside the board.

Not saying there's anything actually wrong with doing it that way, I just don't personally like it.
```

---
## \#15 Posted by: HixStix6 Posted at: 2019-04-11T05:53:10.118Z Reads: 53

```


MysticalDork Where can i buy a big battery like this. What would be the best compromise on big battery vs weight?
```

---
## \#16 Posted by: Dirt_Bag Posted at: 2019-04-11T05:58:38.321Z Reads: 49

```
Weight is hardly and issue with a mtb. A performance build like yours will weight about 35lbs. If you have a few weeks to wait, i can build you a 10s8p pack. The lipo option is to use turnigy  3s or 4s packs to make 12s. You would need 12 3s packs or 9 4s packs
```

---
## \#17 Posted by: Andy87 Posted at: 2019-04-11T06:04:31.063Z Reads: 44

```
Or he can get those in 1p configuration 
https://www.gensace.de/tattu-14000mah-22-2v-25c-6s1p-lipo-battery-pack.html

There is the 16 and 22Ah version as well but they more expensive compared the price to the Ah you get for.
```

---
## \#18 Posted by: Dirt_Bag Posted at: 2019-04-11T06:05:43.459Z Reads: 42

```
I assume isnt comfortable soldering single cells with aluminum solder. Or spot welding...
```

---
## \#19 Posted by: Andy87 Posted at: 2019-04-11T06:07:10.279Z Reads: 44

```
Yap that’s totally right. There are pluses and minuses in big and small packs. Personally if I wouldn’t mind about weight I would go with a LiIon pack all the time. No need to worry about storage charge etc. 

Lipos i would only use if you want to go light weight and don’t mind to take them out after every ride.
```

---
## \#20 Posted by: Andy87 Posted at: 2019-04-11T06:08:07.596Z Reads: 45

```
Why he would need to do that? Can’t follow your thoughts 😅
```

---
## \#21 Posted by: Dirt_Bag Posted at: 2019-04-11T06:10:21.997Z Reads: 38

```
Oh crap. I misread the question and link. I thought you were linking single cell 1s1p cells. MY BAD.  Thats a good idea, but it seems cost prohibitive. I need to go to bed... im way to exhausted
```

---
## \#22 Posted by: HixStix6 Posted at: 2019-04-11T06:13:40.642Z Reads: 42

```
Thanks for your time. You've been very helpful
```

---
## \#23 Posted by: Dirt_Bag Posted at: 2019-04-11T06:18:36.017Z Reads: 44

```
Incase you didnt know, most experienced users charge $8 per question answered. I expect payment soon :smiley:
```

---
## \#24 Posted by: HixStix6 Posted at: 2019-04-11T06:20:56.592Z Reads: 44

```
Andy87. Do i need to run these in series? [https://www.gensace.de/tattu-14000mah-22-2v-25c-6s1p-lipo-battery-pack.html ](https://www.gensace.de/tattu-14000mah-22-2v-25c-6s1p-lipo-battery-pack.html)
```

---
## \#25 Posted by: Andy87 Posted at: 2019-04-11T06:23:27.693Z Reads: 41

```
Yes. You need two of them and a xt90 serial plug and you good to go.

PS: if you want to tag somebody you need to first use @ and than the user name @HixStix6
```

---
## \#26 Posted by: HixStix6 Posted at: 2019-04-11T06:25:21.190Z Reads: 44

```
@Andy87, Thanks. You think i could ride hard for 10miles with these?
```

---
## \#27 Posted by: Andy87 Posted at: 2019-04-11T06:38:07.559Z Reads: 43

```
Sure it depends how hard you go, but I would say 10miles is doable with it. If you shred on fields and small hills for sure it last.
As i said i get 7-10km out of a 5Ah pack. So 14Ah should be about 20km (12.4mi) range. 

In case that is something for you, check the dimensions of the lipo packs. They longer than the other packs which means you would need to mount them along the deck and not vertical.
That’s not a problem, but if you have a flexy deck you need to mount the lipos in a box which doesn’t flex and the box fixed only in the middle so that the box doesn’t restrict the flex of the deck.
```

---
