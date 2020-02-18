# Flipsky fsvesc 50a sk8-esc

### Replies: 202 Views: 10524

## \#1 Posted by: thamer Posted at: 2018-04-08T17:19:43.089Z Reads: 634

```
Is this VESC good??

https://flipsky.net/collections/electronic-products/products/torque-esc-vesc-%C2%AE-bldc-electronic-speed-controller

I will buy one and want to know
```

---
## \#2 Posted by: E1Allen Posted at: 2018-04-08T17:28:04.096Z Reads: 588

```
We all want to know.  A quick forum search provided two results. One was your question the other was also a question.  

You might be the one to tell us if it's good or not.
```

---
## \#3 Posted by: evoheyax Posted at: 2018-04-08T17:29:57.184Z Reads: 577

```
No upgrades, so it's similar to most other vendors I would assume.

However, don't trust you can do 50 amp con without adding a heat sink. Vedder himself showed it can only do 27 amp con without the heat rising.
```

---
## \#4 Posted by: thamer Posted at: 2018-04-08T17:32:37.626Z Reads: 563

```
Ok!! I will use with one of this motor here: https://www.banggood.com/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html?rmmds=myorder&cur_warehouse=CN

Wich max output current is 34 A.

Will it work??
```

---
## \#5 Posted by: RedEagle Posted at: 2018-04-08T17:33:24.222Z Reads: 549

```
It'll work.
```

---
## \#6 Posted by: thamer Posted at: 2018-04-08T17:36:25.974Z Reads: 530

```
Using only one of this racestar motors won't be so powerfull right??

But will it go like 25 km/h?? at least??
```

---
## \#7 Posted by: RedEagle Posted at: 2018-04-08T17:38:21.986Z Reads: 521

```
It depends on your battery,  wheels and gearing.
I need more specs to give you a better answer. What are you going to use in your build?
```

---
## \#8 Posted by: thamer Posted at: 2018-04-08T17:41:25.436Z Reads: 517

```
I am building by parts, first I bought one of this Racestar motors, now I am looking for the best VESC to use with.

I am in doubt of buying this: https://flipsky.net/collections/electronic-products/products/torque-esc-vesc-%C2%AE-bldc-electronic-speed-controller

or this: https://wholesaler.alibaba.com/product-detail/Maytech-rc-system-remote-controller-electric_60533968246.html

If you could give me tips of batteries to buy as well would be great!!
```

---
## \#9 Posted by: thamer Posted at: 2018-04-08T17:42:25.588Z Reads: 492

```
I will use this remote control: https://www.banggood.com/2_4GHz-Radio-Remote-Controller-Receiver-Transmitter-For-Electric-Skateboard-p-1125575.html?rmmds=search&ID=514182&cur_warehouse=CN
```

---
## \#10 Posted by: E1Allen Posted at: 2018-04-08T17:44:33.098Z Reads: 478

```
http://calc.esk8.today 

Do your calculations here
```

---
## \#11 Posted by: e.board_solutions Posted at: 2018-04-08T17:44:37.842Z Reads: 466

```
I got a mail from them today, asked maytech about them, they say the components are not good quality, but if someone would try them I'm interested :slight_smile:
```

---
## \#12 Posted by: RedEagle Posted at: 2018-04-08T17:44:47.549Z Reads: 471

```
I don't have any info on the first one. I use maytechs and they're rock solid if used right. Why not buy the first one for science? 

As for the battery, go liion if you're good with spotwelding or just order a premade one. 
ru.nkon.nl

If you want to live dangerously and be a rebel go the lipo route. 
hobbyking.com
```

---
## \#13 Posted by: RedEagle Posted at: 2018-04-08T17:46:29.874Z Reads: 433

```
Maytech also uses subpar parts but they're rock solid if used right. The solder job is horrible, though!
```

---
## \#14 Posted by: e.board_solutions Posted at: 2018-04-08T17:47:31.896Z Reads: 430

```
[quote="RedEagle, post:13, topic:51591"]
subpar
[/quote]
what is subpar?

The maytech vesc's work fine for me :slight_smile:
```

---
## \#15 Posted by: E1Allen Posted at: 2018-04-08T17:48:06.403Z Reads: 408

```
Subpar.  He means the components and build quality could be better
```

---
## \#16 Posted by: e.board_solutions Posted at: 2018-04-08T17:49:25.027Z Reads: 403

```
uhu, if it does the job it's fine for me :slight_smile:
```

---
## \#17 Posted by: RedEagle Posted at: 2018-04-08T17:51:05.904Z Reads: 398

```
Go watch people on YouTube comparing cheap solder vs good solder. You'll see what I mean!
```

---
## \#18 Posted by: thamer Posted at: 2018-04-08T17:56:43.466Z Reads: 401

```
I am a little bit afraid of buying one that anyone had tested before. So I am going to buy the one of Maytech, just because other people used it before.
But what is the correct way to use Maytech VESCs??
```

---
## \#19 Posted by: FredrikHems Posted at: 2018-04-08T18:01:10.667Z Reads: 405

```
[quote="thamer, post:18, topic:51591"]
what is the correct way to use Maytech VESCs?
[/quote]

Set battery max low, like 35A (Your motor can only do 34A). Keep the ERPM under 60.000, and do not try FOC under any circumstances.
What battery will u be using?
```

---
## \#20 Posted by: thamer Posted at: 2018-04-08T18:02:28.772Z Reads: 396

```
I don't know the battery I will use,

do you have any suggestion??
```

---
## \#21 Posted by: RedEagle Posted at: 2018-04-08T18:09:11.567Z Reads: 382

```
[quote="FredrikHems, post:19, topic:51591"]
Set battery max low, like 35A (Your motor can only do 34A).
[/quote]
**30a!!!!!**
```

---
## \#22 Posted by: GrecoMan Posted at: 2018-04-08T18:09:41.816Z Reads: 372

```
why tho...
```

---
## \#23 Posted by: RedEagle Posted at: 2018-04-08T18:14:22.522Z Reads: 366

```
Two 5s 25c will work fine.
```

---
## \#24 Posted by: RedEagle Posted at: 2018-04-08T18:16:52.104Z Reads: 364

```
Uhmm.. Why what?
```

---
## \#25 Posted by: FredrikHems Posted at: 2018-04-08T18:17:21.328Z Reads: 362

```
[quote="RedEagle, post:12, topic:51591"]
If you want to live dangerously and be a rebel go the lipo route.
[/quote]

30 mins later...

[quote="RedEagle, post:23, topic:51591, full:true"]
Two 5s 25c will work fine
[/quote]

:man_facepalming::man_facepalming:
```

---
## \#26 Posted by: GrecoMan Posted at: 2018-04-08T18:17:23.657Z Reads: 347

```
why only 30a...?
```

---
## \#27 Posted by: RedEagle Posted at: 2018-04-08T18:20:00.413Z Reads: 350

```
Lipos are much less work than liions but you have to be careful when handling them. You would have to assemble a liion pack yourself. I gave this advice because I think he doesn't have time/experience to make a liion pack.
```

---
## \#28 Posted by: FredrikHems Posted at: 2018-04-08T18:20:10.166Z Reads: 354

```
Since your motor really doesn't have the most ideal Kv I would use a 10s + battery. Most people have 190kv motors
```

---
## \#29 Posted by: FredrikHems Posted at: 2018-04-08T18:21:31.290Z Reads: 351

```
You can buy Li-ion packs fully assembled too.. Just like LiPos..
```

---
## \#30 Posted by: RedEagle Posted at: 2018-04-08T18:22:04.351Z Reads: 356

```
You will have drv errors and reliability issues if you set batt max any higher than 30a on a maytech. Additionally, hw 4.12 vescs can only handle 27a continious.
Edit: excluding chaka vescs and focboxes.
```

---
## \#31 Posted by: RedEagle Posted at: 2018-04-08T18:23:55.583Z Reads: 355

```
[quote="RedEagle, post:12, topic:51591"]
As for the battery, go liion if you’re good with spotwelding or just order a premade one.
[/quote]

I said that too. Which path he chooses is up to him.
```

---
## \#32 Posted by: Blitz Posted at: 2018-04-08T18:24:14.041Z Reads: 351

```
[quote="FredrikHems, post:29, topic:51591"]
You can buy Li-ion packs fully assembled
[/quote]

Money money money...♫
If he had a bigger budget why not get focbox.
```

---
## \#33 Posted by: FredrikHems Posted at: 2018-04-08T18:26:43.189Z Reads: 337

```
We haven't heard anything about his budget..
```

---
## \#34 Posted by: RedEagle Posted at: 2018-04-08T18:26:52.936Z Reads: 335

```
Cuz cheap is good! Let's all buy twice!
```

---
## \#36 Posted by: RedEagle Posted at: 2018-04-08T18:31:38.935Z Reads: 336

```
We all go through that at least once in our life. Looks like I'm gonna have to stock up on drvs here though..
```

---
## \#37 Posted by: Acidfie Posted at: 2018-04-08T18:32:03.031Z Reads: 349

```
i want to recite myself here from another thread:

"It’s unwise to pay too much, but it’s worse to pay too little. When
you pay too much, you lose a little money - that’s all. When you pay
too little, you sometimes lose everything, because the thing you
bought was incapable of doing the thing it was bought to do. The
common law of business balance prohibits paying a little and getting a
lot - it can’t be done. If you deal with the lowest bidder, it is well
to add something for the risk you run, and if you do that you will
have enough to pay for something better.”

John Ruskin
```

---
## \#38 Posted by: RedEagle Posted at: 2018-04-08T18:34:18.324Z Reads: 333

```
More skatanistic words have never been spoken.
```

---
## \#39 Posted by: Acidfie Posted at: 2018-04-08T18:37:58.000Z Reads: 343

```
Back to Topic: They say you can run FOC. 

![53|690x122](upload://hScyvBsUGASeTcVEfGKQfglNyPB.png)
```

---
## \#40 Posted by: Acidfie Posted at: 2018-04-08T18:42:28.139Z Reads: 346

```
lol dude,

i was completely stumped about that "skatanistic" and just thought you meant satanistic and wrote it the wrong way..until i stumpled upon another thread where someone called "Skatan" and then the scales fell from my eyes

idiot me
```

---
## \#41 Posted by: RedEagle Posted at: 2018-04-08T19:10:53.857Z Reads: 346

```
Can't like your comment enough :joy:
```

---
## \#42 Posted by: e.board_solutions Posted at: 2018-04-08T19:14:50.055Z Reads: 325

```
I use maytech vesc also in foc, and also more amps than 30 (not continiious though)
```

---
## \#43 Posted by: Bjork3n Posted at: 2018-04-08T19:23:19.839Z Reads: 332

```
Of all my three maytech vesc none work very well when above battery max over 30A. 
If I push more than 30A battery I get random drv failures.
```

---
## \#44 Posted by: e.board_solutions Posted at: 2018-04-08T19:24:20.433Z Reads: 329

```
uhu interesting, when did you buy them?
```

---
## \#45 Posted by: RedEagle Posted at: 2018-04-08T19:26:19.990Z Reads: 340

```
Back on topic

@thamer If you use this general guideline you should be golden.

10s3p 30q battery pack OR 10s1p 5ah lipo
BMS (optional, some say it's necessary)
Maytech vesc
Motor Racerstar 140kv 
Mini remote
83mm wheels, gearing 15/16t motor, 36t wheel
15mm belt (chain is also an option)
Antispark switch
Enclosure
Motor mount

I might have missed something. Anyone is free to give pointers/advice on this.

https://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983
```

---
## \#46 Posted by: Bjork3n Posted at: 2018-04-08T19:37:37.476Z Reads: 313

```
3 weeks ago
```

---
## \#47 Posted by: e.board_solutions Posted at: 2018-04-08T19:39:04.046Z Reads: 314

```
hmm, did you contact your dealer? That shouldn't happen
```

---
## \#48 Posted by: Bjork3n Posted at: 2018-04-08T20:16:24.260Z Reads: 316

```
Well it is just a problem when doing rapid acceleration and fast standing starts. 
There are more than me that found maytechs limitations at 30A. 
If I push start or is easy on the throttle the first meters I can use 40A but I feel like it's safer just to stay at 30A.
```

---
## \#49 Posted by: e.board_solutions Posted at: 2018-04-08T20:21:37.736Z Reads: 301

```
uhu, less stress is always better, 30 amp gonna give you some nice acceleration no?
```

---
## \#50 Posted by: Bjork3n Posted at: 2018-04-08T20:57:56.449Z Reads: 297

```
In dual config yes :slight_smile:
```

---
## \#51 Posted by: e.board_solutions Posted at: 2018-04-08T21:05:58.008Z Reads: 303

```
Dual :heart_eyes::heart_eyes::heart_eyes:
```

---
## \#52 Posted by: thamer Posted at: 2018-04-08T21:48:18.489Z Reads: 309

```
Hey!! Thank you for the answers, I will follow the guideline that @RedEagle sent to me:

10s3p 30q battery pack OR 10s1p 5ah lipo
BMS (optional, some say it’s necessary)
Maytech vesc
Motor Racerstar 140kv
Mini remote
83mm wheels, gearing 15/16t motor, 36t wheel
15mm belt (chain is also an option)
Antispark switch
Enclosure
Motor mount 

I am just not so happy because I bought the Racestar 140kv Motor (I didn't realize that it is not so good), maybe in the future I can upgrade my board to a dual motor.

I will buy the Maytech VESC instead of the Flipsky.

If you have any more tips for me, about BMS, power switches and battery ports to charge, things like taht, will be great!!
```

---
## \#53 Posted by: RedEagle Posted at: 2018-04-08T22:23:41.285Z Reads: 293

```
You should get a 190kv motor.
```

---
## \#54 Posted by: FredrikHems Posted at: 2018-04-08T22:28:24.977Z Reads: 296

```
Yea, an 190kv motor would be better. Top speed with the components over would be ~28km/h
```

---
## \#55 Posted by: Bataleon Posted at: 2018-04-20T20:45:12.116Z Reads: 295

```
If you're running a 10s pack, definitely go for the 200kv Racestar instead of the 140kv.
```

---
## \#56 Posted by: BensonYong Posted at: 2018-05-25T13:45:00.417Z Reads: 292

```
New product ![01 (5)|690x499](upload://lPuJkJBNh66ALRpAAqUaKbXvWX7.jpg)
```

---
## \#57 Posted by: aigenic Posted at: 2018-05-25T13:57:42.150Z Reads: 289

```
Look nice, I expected a bit lower price, but it is not that bad :) I found on your website that it includes Anti-spark switch, but I don't see any on the pictures...

EDIT: Found it :D
```

---
## \#58 Posted by: dkac Posted at: 2018-05-25T14:01:18.717Z Reads: 292

```
It looks like anti-spark switch is included on mainboard. 

I've received more photos from them:
![71875fe30500aec0f8aa5e9ce49fdaa455bfc63c_1_375x500|375x500](upload://aiIaMlSSNyMwBa1atcfQbilbSJ4.jpg)![image|375x500](upload://qYncovLceTWhZRFHQz7oaBxFCO3.jpg)
```

---
## \#59 Posted by: aigenic Posted at: 2018-05-25T14:02:06.222Z Reads: 290

```
Yeah I just found some more photos in other thread and the antispark switch should be on the side of the case :)
```

---
## \#60 Posted by: uigiroux Posted at: 2018-05-25T14:31:50.514Z Reads: 291

```
I've spoken with them and if we can organize a GB for 20 units they'll sell them for $124 each.  I'd say that is an incredible price, if they perform as advertised that is..
```

---
## \#61 Posted by: squishy654 Posted at: 2018-05-25T17:27:55.714Z Reads: 296

```
These guys just cold messaged me on Facebook to try and sell me this thing, it was sort of annoying. And then they offered the huge discounted price of $126 to buy them in bulk like I'm some sort of huge buyer or a store...hell I can barely afford the crap I do get my hands on, lol..and no thanks, not about to spend 126 bucks for a unproven new product with iffy ratings..lemme know when they cost about 40 bucks and don't break when you breath on them..
```

---
## \#62 Posted by: moon Posted at: 2018-05-25T17:39:34.560Z Reads: 287

```
How did they message you on Facebook?
```

---
## \#63 Posted by: squishy654 Posted at: 2018-05-25T17:41:29.624Z Reads: 289

```
Barbie Zhang
https://www.facebook.com/profile.php?id=100024974145966
```

---
## \#64 Posted by: e.board_solutions Posted at: 2018-05-25T17:41:49.224Z Reads: 286

```
Yes be carefull, they contact me also everywhere with different sales persons.

Not sure about the quality

I think they are here for quick money, not sure ...
```

---
## \#65 Posted by: uigiroux Posted at: 2018-05-25T17:45:36.367Z Reads: 289

```
I believe LHB has purchased 2 of their VESC 6 to test out so hopefully we'll find out soon enough.
```

---
## \#66 Posted by: squishy654 Posted at: 2018-05-25T17:47:53.797Z Reads: 292

```
[quote="uigiroux, post:65, topic:51591, full:true"]
I believe LHB has purchased 2 of their VESC 6 to test out so hopefully we’ll find out soon enough.
[/quote]

![maxresdefault|690x388](upload://5h1sO7AdZ0jM8bJpKiInusc8JUQ.jpg)
```

---
## \#67 Posted by: pootis_owner Posted at: 2018-05-25T18:09:36.911Z Reads: 286

```
Guys please this vesc is a good vesc in my eyes i got one to they contacted me and i thought why not works good a video is in the making off the vesc!!
```

---
## \#68 Posted by: uigiroux Posted at: 2018-05-25T18:55:55.371Z Reads: 287

```
You got one already?  Are you running single or dual?  Pics??
```

---
## \#69 Posted by: pootis_owner Posted at: 2018-05-25T19:20:31.085Z Reads: 290

```
Currently running a single vesc i have direct contact with the designer and factory so if you guys have any questions im here :D im currently building a 10s6p battery pack if that is finished i will make the video off the vesc. ![vesc flipsky|666x500](upload://4NTUcq8NDIz2bAccjRqW3HQZpRv.jpg)

here a little video https://www.youtube.com/watch?v=5NNv6Hrfptc&feature=youtu.be motor running on foc mode atm
```

---
## \#70 Posted by: moon Posted at: 2018-05-25T19:22:55.062Z Reads: 283

```
All I want is a non biased review of this VESC...
```

---
## \#71 Posted by: pootis_owner Posted at: 2018-05-25T19:28:18.196Z Reads: 279

```
I can say whatever i want about the vesc i bought it myself....  i only help making this vesc better....
```

---
## \#72 Posted by: Hummie Posted at: 2018-05-25T19:30:52.849Z Reads: 279

```
is it all the original BOM?  it looks like a double stacked cap at least.
```

---
## \#73 Posted by: uigiroux Posted at: 2018-05-25T19:31:25.669Z Reads: 278

```
Damn I was hoping it was the VESC 6 you had.  I wish they made the one got a 100A like the Maytech one LHB is testing.
```

---
## \#74 Posted by: Hummie Posted at: 2018-05-25T19:32:26.386Z Reads: 278

```
but 100 amps is overkill and doubt youd need so much power.  i never get overcurrent/heat shutdowns, but i have blown up bits that weren't part of the upgraded bom
```

---
## \#75 Posted by: pootis_owner Posted at: 2018-05-25T19:33:26.005Z Reads: 278

```
they are in the making off a 200a vesc based module to for electric gokarts and small cars they said :stuck_out_tongue:
```

---
## \#76 Posted by: uigiroux Posted at: 2018-05-25T19:33:30.758Z Reads: 276

```
Well not that you'd use it but from what I've read they are far less prone to breaking down than the 50A versions.

Or is it 60A ones that are super reliable?
```

---
## \#77 Posted by: trampa Posted at: 2018-05-26T15:21:05.397Z Reads: 276

```
The brake down reliability has nothing to with rating!
It has only something to with design.
It's funny people refer to the Flipsky ESC as the VESC 6. It's obviously a totally different design. 
You wouldn't call a Subaru a Toyota or a VW a Mercedes. Different designs and brands.

Only because Flipsky copies our words from our website and use a branding they shouldn't use doesn't make the thing a VESC 6. 
I get email from them, made up from our website text, LOL... 

I hope Flipsky will realize that it doesn't work in their favor to use other peoples wording and branding to advertise their products.
```

---
## \#78 Posted by: uigiroux Posted at: 2018-05-26T16:26:31.186Z Reads: 268

```
I have to agree with you entirely on this one.  Though I'm guilty of calling it that all the time... I guess that's for convenience sake though.
```

---
## \#79 Posted by: thamer Posted at: 2018-05-26T17:25:38.856Z Reads: 279

```
Guys,

I've been talking with them for at least one month.

They are working pretty hard to build a good product for us with a honest price.

I know that some companies maybe are awe about the appearence of new concurrents in the market, however I am believing that FlipSky is going to deliver us a good product with high performance as well other companies are already doing.

I am pretty anxious about testing it and give you a detailed review. I already bought one, and when it arrives I will do it for you guys.

As @uigiroux mentioned before, if we organize a GB for some units they can give us a huge discount. If you want I can organize this group in another forum post.

In concluison I am hoping that they are going to build a good product and provide us more options of VESC 6 for buiyng.
```

---
## \#80 Posted by: Hummie Posted at: 2018-05-26T17:30:50.085Z Reads: 271

```
do group buy please!  what kind of price?  if a place does a vesc version that shows solid on foc and we can all get a bunch to test that sounds great.
@trampa your stuff is too expensive and especially for us in the usa.   and in my mind it probably is overkill in the current handling ability.  ive never had a temp shutdown running two!  especially with people who are running two we just need it to not breakdown.  I don't even want bells and whistles and would be happy with a non-adjustable version if it was preset well.
124? when's the groupbuy start?  what more you know about it?  any warranty?  any endorsement by people who use it on foc or know about the bits?
```

---
## \#81 Posted by: uigiroux Posted at: 2018-05-26T17:31:36.800Z Reads: 269

```
I'd really like to see a dual case, since the two power buttons is a bit odd.  They'd solve many problems if they were to make this a dual unit.
```

---
## \#82 Posted by: uigiroux Posted at: 2018-05-26T17:32:12.210Z Reads: 254

```
I posted a bit further up, they'll do $124 if we buy 20.
```

---
## \#83 Posted by: thamer Posted at: 2018-05-26T17:33:18.590Z Reads: 256

```
@uigiroux would you organize this group buy or prefer that I do it??
With whom you have been talking in the company??
```

---
## \#84 Posted by: uigiroux Posted at: 2018-05-26T17:35:25.673Z Reads: 256

```
A couple people, mostly Zhang Barbie.  I could, or if you want to that's fine too.
```

---
## \#85 Posted by: moon Posted at: 2018-05-26T17:38:53.106Z Reads: 254

```
A regular user needs to organize the group buy
```

---
## \#86 Posted by: thamer Posted at: 2018-05-26T17:41:26.361Z Reads: 256

```
Nice!!

Can you do it for us?? Please mark me on the post and I will help you talking with them and some other stuff.

Let's do it and give them the opportunity to show us the quality of their product.
```

---
## \#87 Posted by: uigiroux Posted at: 2018-05-26T17:41:34.354Z Reads: 253

```
Ugh, It seems I've been demoted from lvl 3 for some reason... Ok well no worries, that disqualifies me though so someone else will have to handle the GB.
```

---
## \#88 Posted by: thamer Posted at: 2018-05-26T17:42:43.866Z Reads: 246

```
That is ok. I am Basic user as well. :frowning: :frowning:
```

---
## \#89 Posted by: uigiroux Posted at: 2018-05-26T17:43:01.465Z Reads: 250

```
I'll certainly help with anything needed and talk with them,, but I can't run it since my member level has gone down from lvl 3, lol.
```

---
## \#90 Posted by: uigiroux Posted at: 2018-05-26T17:43:58.484Z Reads: 246

```
Give me a little time and I'll try and get someone to help on this. :wink:
```

---
## \#91 Posted by: uigiroux Posted at: 2018-05-26T17:45:50.140Z Reads: 245

```
Perhaps since I've been level 3 and this isn't something that I'm making myself I might be allowed to run it?  I don't know...  I'll ask though.
```

---
## \#92 Posted by: thamer Posted at: 2018-05-26T17:45:51.308Z Reads: 237

```
That is perfect.
```

---
## \#93 Posted by: Jc06505n Posted at: 2018-05-26T17:47:57.202Z Reads: 240

```
You would need to be a current lvl 3 in order to do so.
```

---
## \#94 Posted by: Hummie Posted at: 2018-05-26T17:47:58.102Z Reads: 246

```
someone do it or I would for no profit.  but @trampa if they are using your language and claims I'm sure that's aggravating and that bothers me as a customer.  

I wish one of these Chinese suppliers would step up with something solid, or maybe they already have and we don't know.  the lack of reliable vescs especially now with axle and chaka gone, and we have a forum to do testing.
```

---
## \#95 Posted by: Jc06505n Posted at: 2018-05-26T17:51:54.569Z Reads: 250

```
Also guys let’s not get ahead of ourselves, why do a Group Buy on something untested, especially when none of us have none of the details on how it works exactly. 

Has anyone here worked out how ones suppose to run dual with Anti Spark switches on both? Or how well it’s Heatsinks work  or if it’s design (which has been critiqued by respected members of the forum) would mean $124+ down the drain ? Didn’t think so. 

Hold off on Group Buy talks until this Piece of hardware has been tested by someone like @longhairedboy or a respected third party.  

Don’t feel like reading a whole month worth of complaints in the future.
```

---
## \#96 Posted by: uigiroux Posted at: 2018-05-26T17:54:13.622Z Reads: 244

```
I think LHB actually ordered one of these for testing.  Or it might be the version 4 they have...  On the plus side, I believe they have a 1 year warranty...
```

---
## \#97 Posted by: Hummie Posted at: 2018-05-26T17:55:01.350Z Reads: 248

```
we could be that testing.  how many testers have there been of their esc in foc so far?  I'm not jumping into anything but the lack of reliable vescs makes me want to get some organized testing done

and with a hub motor vs a much faster spinning motor with a pulley it might be apples and oranges and work on the hub but not the pulley maybe.
```

---
## \#98 Posted by: Jc06505n Posted at: 2018-05-26T17:57:17.922Z Reads: 249

```
Yay 1 year warranty from a non US/Euro company that isn’t bind by our laws and can easily use warranty to make you pay out $300 for a piece of hardware over the course of a year due to possibke intentional hardware negligence. Woopdedo
```

---
## \#99 Posted by: bigben Posted at: 2018-05-26T17:57:36.852Z Reads: 246

```
But these things are huuuuge. 
Far wider than would fit in a regular enclosure in dual settup.
```

---
## \#100 Posted by: Jc06505n Posted at: 2018-05-26T17:59:07.266Z Reads: 254

```
That can be done , but don’t call it and condone I.T under a group buy, we should call It something else, because i guarantee people are going to jump on it as group buys on the forum are usually for reliable products or from reliable individuals.
```

---
## \#101 Posted by: uigiroux Posted at: 2018-05-26T17:59:18.369Z Reads: 271

```
Ok, or not..?  I'm just stating stats about the product, no need to take out any of your reservations on me.
```

---
## \#102 Posted by: Hummie Posted at: 2018-05-26T18:00:25.943Z Reads: 274

```
doesn't seem that big.  20mm for the caps maybe.  big caps maybe? 


BUT ITS 90$!!!!!
https://flipsky.net/collections/electronic-products/products/torque-esc-vesc-®-bldc-electronic-speed-controller
```

---
## \#103 Posted by: Jc06505n Posted at: 2018-05-26T18:01:03.300Z Reads: 275

```
I’m being realistic here. If you’re falling back on “at least there’s warranty” on a product for your justification to buy something, then maybe rounding up a group buy on it isn’t the best idea.


Edit: but I do apologize for my aggressive tone. Really sorry man.
```

---
## \#104 Posted by: uigiroux Posted at: 2018-05-26T18:01:07.617Z Reads: 271

```
I think we're all taking about the vesc 6, not the 4.
```

---
## \#105 Posted by: Hummie Posted at: 2018-05-26T18:02:15.437Z Reads: 266

```
why get the 6 if the 4 does foc and doesn't break? (I don't think the amp limits a prob with two of them) and 90$!?  things are seeming too good to be true but until reviews are in its all claims.

or maybe this is all old bom stuff
```

---
## \#106 Posted by: uigiroux Posted at: 2018-05-26T18:02:43.091Z Reads: 261

```
All good, no worries :wink:  I do think it's a bit early for a GB too personally, I've been wanting to hear from LHB what he thinks of it.  Again though, I'm not sure which version he got though...
```

---
## \#108 Posted by: bigben Posted at: 2018-05-26T18:04:47.490Z Reads: 258

```
Sorry I was looking at the pictures of the thing in a case with the xt90 and the on off. 
That’s a big unit.
```

---
## \#109 Posted by: moon Posted at: 2018-05-26T18:06:16.245Z Reads: 259

```
Seriously?

Only $60 on taobao, I wouldn't mind buying one for testing. 

But I am not a very good tester :(

@bigben

Want to test out their VESC 4.12?
```

---
## \#110 Posted by: Hummie Posted at: 2018-05-26T18:13:42.277Z Reads: 252

```
I wrote them seeing what I can get them to sell me in bulk on the 4.    why is taobao cheaper than their site?  the prices are getting scary low.  but with a hub motor maybe you can get away with a lesser esc anyway. who's actually tried this and the other Chinese versions and can say anything?
```

---
## \#111 Posted by: moon Posted at: 2018-05-26T18:15:53.773Z Reads: 257

```
I don't know but it makes sense. Theres hardly a  market in China but they can still sell units for that price point.

Also theres other vescs around the $60-$70

The maytech vesc is(was idk) $72

[quote="Hummie, post:110, topic:51591"]
who’s actually tried this and the other Chinese versions and can say anything?
[/quote]

Thats the problem, theres a couple here that have tried flipsky but their review seems a bit dodgy and inexperienced.
```

---
## \#112 Posted by: Hummie Posted at: 2018-05-26T18:18:51.983Z Reads: 256

```
at least when these things break it doesn't seem catastrophic throwing you off.   

if they do foc with a hub motor, if you see that please tell me.
```

---
## \#113 Posted by: Sebike Posted at: 2018-05-26T18:23:56.911Z Reads: 255

```
here are the taobao flipsky listings.. FS 4.12 63 usd, 84 with case

https://shop304874456.taobao.com/
```

---
## \#114 Posted by: moon Posted at: 2018-05-26T18:26:34.968Z Reads: 256

```
You could also say the same thing about Maytechs v2 remote

EU market 50 euros
Taobao $20
$16 if you order more than 10 sets
Alibaba probably more $22-50 - probably north of the range if small order
```

---
## \#115 Posted by: trampa Posted at: 2018-05-27T09:11:20.965Z Reads: 266

```
[quote="Hummie, post:94, topic:51591"]
but @trampa if they are using your language and claims I’m sure that’s aggravating and that bothers me as a customer.
[/quote]

On top of that they send us their promo mail, with our words, asking us to buy vesc6. 3x LOL
That is off any scale...

If a company can't write it's own email, how can they design a proper esc or handle customer support?
If you design a product and you really believe in it, why use false and infringing branding? The only reason I can see is trying to fool customers, making them believe it's the same beast, just cheaper.
But it's not the same... 

If you believe in your product you usually would be proud of your achievements and your marketing wouldn't need to make use of other peoples achievements. Using the marketing and branding from other companies doesn't shine a good light on your product. Only fake products are marketed this way and we know what quality and service to expect when buying them. Alarm bells ringing....

The correct way of marketing would be:
We have a new ESC design for sale, it's called e.g. the Flipper and is fully compatible with VESC-Firmware and VESC-Tool.
```

---
## \#116 Posted by: pootis_owner Posted at: 2018-05-27T13:29:05.868Z Reads: 256

```
I got the vesc from this guys for 30 euro's for testing so i can get 20 more for 30 euro'sá piece i think for a groupbuy... but that is without shipping cost shipping is 15 euro's....
```

---
## \#117 Posted by: moon Posted at: 2018-05-27T13:30:40.742Z Reads: 250

```
Mate you can't organise a group buy
```

---
## \#118 Posted by: uigiroux Posted at: 2018-05-27T13:30:47.609Z Reads: 249

```
Who's, this flipsky version 4 one?  Christ, at that price I'd try a few and I'm in the states.
```

---
## \#119 Posted by: pootis_owner Posted at: 2018-05-27T13:45:27.696Z Reads: 247

```
yes it is the version 4
```

---
## \#120 Posted by: jourm Posted at: 2018-05-27T14:04:30.838Z Reads: 248

```
damn, at 30 euros that is insane! I would definitely want some
```

---
## \#121 Posted by: uigiroux Posted at: 2018-05-27T14:07:18.173Z Reads: 250

```
I just messaged them asking about a group buy price.  Will report with their response.  I know I can't organize it before anyone points that out :wink:
```

---
## \#122 Posted by: Hummie Posted at: 2018-05-27T15:58:47.714Z Reads: 253

```
why does anyone want the 6 if the 4 does foc and doesn't break?  I keep asking.   I guess the 6 could do more amps but if I never have a temp shutdown with the 4 when running two ...seems good enough.
```

---
## \#123 Posted by: eLDoska Posted at: 2018-05-27T16:01:18.698Z Reads: 258

```
![image|690x387](upload://x11BfVNeCtqhdjjovGBl04Fm5i0.jpg)
61.53 € shipped (57.8€ with cashback). without groupbuy and other time consuming things.
```

---
## \#124 Posted by: AndyL Posted at: 2018-05-27T17:54:30.252Z Reads: 257

```
Where did u find it for 20 on taobao? Link?
```

---
## \#125 Posted by: telnoi Posted at: 2018-05-27T17:58:05.303Z Reads: 261

```
You run huge ass motors.
You like to do burnouts.
You've got an MTB.
You want added reliability (disconnected phase wires/canbus/higher RPM not an issue).

Sometimes I wish I could get more out of the focbox and dual motors I have. It already improved with the @Kug3lis dual case. Previously had constant thermal slowdowns without even realising it (just suspecting).
```

---
## \#126 Posted by: Kug3lis Posted at: 2018-05-27T18:04:36.163Z Reads: 251

```
30 eur if you look at the BOM list and go for e.g. octopart to compare pricing even at 1000 units it wouldn't be 30€... Sounds so fishy...
```

---
## \#127 Posted by: moon Posted at: 2018-05-27T18:05:23.096Z Reads: 248

```
I am glad someone said it
```

---
## \#128 Posted by: pootis_owner Posted at: 2018-05-27T18:58:21.445Z Reads: 241

```
i payed 30 euro's but i was a early buyer but i can ask what i need to pay for 10 pieces.....
```

---
## \#129 Posted by: Kug3lis Posted at: 2018-05-27T21:45:39.259Z Reads: 244

```
Regarding thermals I am amazed myself I am running 90A/motor 90A/bat and even at 80A according logger its only 45ºC and even after hard non stop driving (big long street no red lights for like 5-7km at 50km/h avg) the case was barely warm...
```

---
## \#130 Posted by: Hummie Posted at: 2018-05-27T21:55:59.173Z Reads: 253

```
what is the amp output limit of the 6 as determined by the software and hardware?  maybe I'm wrong but I thought it was pretty much if not exactly the same as the 4.  It may keep cooler and not hit a temp cutoff, largely because it has a huge heatsink, but I think you can get close to the same output.  Maybe I'm very wrong, how many amps can be programed for battery and motor amps on the 6?
```

---
## \#131 Posted by: Kug3lis Posted at: 2018-05-27T21:58:57.190Z Reads: 263

```
https://github.com/vedderb/bldc/blob/master/hwconf/hw_60.h#L231
```

---
## \#132 Posted by: Hummie Posted at: 2018-05-27T22:06:59.692Z Reads: 257

```
thanks.   so if the software limits to 120 for both on the 4 and the 6, and I don't blow up using foc, and I can put a fat heatsink on the fets if I need to, why not just get the super cheap 4?

I'm also super suspicious of the super low price of this flipsky but I also hit them up for a bulk price.   

but all I really want to know is where can I find a cheap reliable 4 that does foc?  
how much safer would foc be when using a hub motor with therefore a low erpm?

also ive had different amounts of noise out of different versions of vescs with the same motor. and running foc  why?
```

---
## \#133 Posted by: uigiroux Posted at: 2018-05-28T06:53:15.112Z Reads: 261

```
Got some pics of the VESC 6 in the case opened up.  It explains why the case is so big relative to the size of the unit.

![Screenshot_20180528-014814|690x493](upload://4hqJYilFpz5zt8qz1UAM6nSGlFa.jpg)
![Screenshot_20180528-014747|669x500](upload://mRfdW7JIHTO1ULnUqMkseOCHJqk.jpg)
```

---
## \#134 Posted by: Kug3lis Posted at: 2018-05-28T07:00:06.399Z Reads: 253

```
Those capacitors look so "big" and so trust worthy... For this amount of money you can get decent branded ones...
```

---
## \#135 Posted by: trampa Posted at: 2018-05-28T07:05:18.140Z Reads: 256

```
Obviously not a VESC 6. It's a Flipper I would say.
If they are not branding it, feel free to give it a name Uriah (-;
```

---
## \#136 Posted by: Kug3lis Posted at: 2018-05-28T07:10:11.179Z Reads: 256

```
Sketchy6 :D
```

---
## \#137 Posted by: myreala Posted at: 2018-05-28T07:14:52.636Z Reads: 256

```
I don't know why people are badmouthing this VESC before it has even been tested. I don't care what it looks like don't care if caps are small. I am gonna wait until someone does extensive testing before passing judgement. The company has obviously taken some pain to design a good product even removing the need of an anti-spark. I don't know why everyone is so against it. 
@trampa I can understand. He just hates anyone who even mentions VESC6. Everyone else not so much.
```

---
## \#138 Posted by: uigiroux Posted at: 2018-05-28T07:16:02.986Z Reads: 253

```
Haha, ok your right Frank, the Flipper Sixer! :wink:
```

---
## \#139 Posted by: Fiori Posted at: 2018-05-28T07:16:32.057Z Reads: 249

```
I might have to test a couple of these out for my Carvons when they get here :)
```

---
## \#140 Posted by: willpark16 Posted at: 2018-05-28T08:23:39.845Z Reads: 255

```
I’ll be testing these out for you guys, I think it only makes sense to try this before bashing, I mean look at axle or even the earlier enertion Vesc. As for @trampa, people might actually by your vesc 6 if it didn’t cost almost as much as someone’s rent😉
```

---
## \#141 Posted by: Benjamin899 Posted at: 2018-05-28T09:40:39.182Z Reads: 251

```
Mmmmh Well lets See whats IRL Testing says. For lighter Rider Like myself amps are Not that big of an issue.
```

---
## \#142 Posted by: trampa Posted at: 2018-05-28T09:43:14.073Z Reads: 264

```
[quote="myreala, post:137, topic:51591"]
Everyone else not so much.
[/quote]

Well, everyone else has spent a lot of money in the past for devices that failed very soon. 
People are careful about new esc-designs, because of what other users experienced in the past.
Must have been 100K or more that were spent on faulty HW 4 ESCs without warranty.
If a thing has a name, and it's known for causing trouble, people will avoid buying it. 
If a device works flawless people want to buy that exact device and they are happy if they can identify it in the market with ease.

@uigiroux,  Flipper Sixer is fine for me. 

Ps.: I hope their product is better than their advertising. To me that kind of stuff shows a poor business ethos.
```

---
## \#143 Posted by: Pabloh Posted at: 2018-05-28T10:29:25.885Z Reads: 261

```
To me, poor business etos is also to threaten competitors and speak bad about them trying to maintain a monopoly with highly overprices.
```

---
## \#144 Posted by: telnoi Posted at: 2018-05-28T10:43:18.154Z Reads: 261

```
80A detected during a ride and bat set to 90A on a focbox? Holy crap..

Can already tell from the pictures that the flipsky case does not have enough mass to dissipate heat quickly enough. It's very similar in design compared to the standard focbox case.
```

---
## \#145 Posted by: Kug3lis Posted at: 2018-05-28T10:44:59.524Z Reads: 258

```
I started on really steep hill and went almost full speed possible to climb it but that was only time I saw something beyond 70A
```

---
## \#146 Posted by: telnoi Posted at: 2018-05-28T10:47:12.720Z Reads: 259

```
well, that's good to hear. My runs are typically full throttle up an offroad hill. 80% of what I do.
```

---
## \#147 Posted by: trampa Posted at: 2018-05-28T11:38:02.263Z Reads: 268

```
As you can clearly see, there is no monopoly. We see more different hardware as ever before. This trend will only grow. Variety now starts to replaces a clone product armada. But different products should be easy to identify.
Some guys understand that they need to give their device a sound name and market it using that name.
This way the community can identify a certain device with ease. If it's reliable it will have a good reputation and sell. If it's carp people will not buy it and it will eventually disappear from the market. Same with software. People will use what they trust and they need to be able to identify a certain source.

I didn't say anything about the Flippers quality BTW. 
The community will find out if it's good, strong, reliable, practical etc. or not. 
I just dislike their way of market introduction. 
People here were referring to it as the VESC 6, which it obviously isn't.  
They did that because it was advertised as a VESC 6. 

If they can't give it a name, I will call it the Flipper from now on.
```

---
## \#148 Posted by: BensonYong Posted at: 2018-05-28T11:58:06.006Z Reads: 268

```
Dear Mr. Frank
Thank you so much for your worth suggestions and marketing ploy on our products, That’s really important to us.
First, I revere Benjamin and his team greatly. 
Benjamin’s team has made great achievements in the development of the VESC series that has leading the development of the industry and made users around the world crazy. Here we must highly praise the Benjamin team!
The products developed by our company are based on Benjamin product series. Since the technology of the VESC series products is open source, our company's research and development also stands on the shoulders of the giants and makes some adjustments to the functions of the original products. Of course, it is improper for us to use VESC to promote our products. Your comments are very useful to us. Then we will make promotional adjustments and use FSESC6.6  to promote our products.
Flip Sky always think intellectual property importance, respected previous research and development achievements. We are also working hard to improve our products and pursue even more cool technological innovations. In the future, we will promote text more rigorously. Your opinions and suggestions are the cornerstone of our development. Thanks again for your suggestions. 
Have a nice day 
Regards
Benson
```

---
## \#149 Posted by: Pabloh Posted at: 2018-05-28T12:11:37.074Z Reads: 263

```
Maybe my poor english skills lead me to a mistake but in my opinion puting a jocose name to a competitor's product it's bad business etos.
This behaviour added to some behaviours shown before makes me think you are not the correct guy to speak of business etos.
I'm quite new on this forum, just a consumer that is ashamed of the things that I read from you.
```

---
## \#150 Posted by: trampa Posted at: 2018-05-28T12:47:38.973Z Reads: 276

```
See it this way: They advertise it as a VESC 6. People here start calling it the VESC 6 and customers/users get confused big time - especially the newbies. The entire marketing is aiming at max confusion.

If a company fails to give their product a name, but uses another persons branding to market it, and people start to associate that brand to the infringing product, something is obviously funny. 

https://www.vesc-project.com/trademark_policies

This thing needs a name and that is not VESC 6 and not FS**VESC**6. 

Flipsky ESC is fine, nothing wrong with that - and Flipper is just a nickname because someone here realized that you need to flip one ESC over, so that you can reach the other ON/Off button in a twin setup. 
Sorry for that! 
.
```

---
## \#151 Posted by: BensonYong Posted at: 2018-05-28T13:00:33.622Z Reads: 274

```
![6|666x499](upload://vCjpdYpG6w24J9G6iAs1dixDIhL.jpg)
FSESC6.6  
Things inside the box.
```

---
## \#153 Posted by: BensonYong Posted at: 2018-05-28T13:06:21.094Z Reads: 270

```
![6-2|666x499](upload://oW71zBDqoFsOHN63tLcfIrkwpj2.jpg)
The appearance of the box
```

---
## \#154 Posted by: BensonYong Posted at: 2018-05-28T13:24:42.110Z Reads: 279

```
![IMG_20180528_211343|666x499](upload://x5A2JWKXL4u630DOCr3i3EnAv3e.jpg)
```

---
## \#155 Posted by: BensonYong Posted at: 2018-05-28T13:32:14.119Z Reads: 281

```
https://youtu.be/kiguWLLUEHo
Video of Install the aluminium case.
```

---
## \#156 Posted by: bigben Posted at: 2018-05-28T14:08:25.964Z Reads: 281

```
Hi @BensonYong,
Is the aim of the flippedyflipesc to be used only on single motor drives?
The width of the box and the on/off switch on each esc would suggest this? Or am I missing something?
Cheers
Ben
```

---
## \#157 Posted by: BensonYong Posted at: 2018-05-29T02:11:10.286Z Reads: 279

```
Hi,@bigben ,
It is single drive esc.CAN wire will be need if use two FSESC6.6 to Dual drive E-skateboard. 
Heat sink width is smaller than aluminum box and saves space.
If use two FSESC6.6 to Dual drive E-skateboard,we recommend shorting one of the on/off switches.
```

---
## \#158 Posted by: Jc06505n Posted at: 2018-05-29T02:26:01.585Z Reads: 279

```
Shorting ? I don’t get the design Decision here really. Why not just make a single Dual VESC with one on/off switch, and sell the other one as a single VESC
```

---
## \#159 Posted by: uigiroux Posted at: 2018-05-29T05:51:47.799Z Reads: 277

```
This doesn't make sense, cause regardless of if you use a second on switch, it's still going to take the same huge amount of space, that being the issue.  Also as many have pointed out, myself included, having the switch located on the side of the case means you have to open up the enclosure to turn it on.  Why wasn't the enclosure just made to fit the HW6 and the on switch could just be included to be installed on the outside of the boards enclosure.  By including space in the ESC case for this switch its added like what, 30ish mm extra in one direction, and 10-20 in the other?  It's nice that's there's a switch, don't get me wrong... but it's placement has compromised the entire design in my opinion...
```

---
## \#160 Posted by: uigiroux Posted at: 2018-05-29T05:56:03.800Z Reads: 276

```
I don't see how anyone would even use this without just removing the switch from its original location and mounting it to the side of the board enclosure.  There really should only be one design which just fits the dimensions of the HW6, and if you want to use 1 switch and not the other, you just remove the switch from one...  This placement baffles me. :confused:

I did speak to a rep and they are in the making of a dual case unit for this.  Though I imagine it'll still be oversized with the placement of one of these switches in the case, rather than simply including it for us to choose where to mount it to the outside enclosure.
```

---
## \#161 Posted by: Hummie Posted at: 2018-05-29T16:50:24.007Z Reads: 269

```
if youre interested in giving the 4 a shot i can get them in bulk if we get 20.  im going to order just two today to see how they do.  60$
```

---
## \#162 Posted by: moon Posted at: 2018-05-29T16:57:00.791Z Reads: 272

```
Yeah! have you ordered them? :)
```

---
## \#163 Posted by: Hummie Posted at: 2018-05-29T17:08:18.929Z Reads: 286

```
im just going to get two today i think, unless 9 people want a set also and pm me and send me the bucks for 20 by tomorrow.  plus like 15$ for shipping!  im finding figuring shipping costs after sending is trouble
```

---
## \#164 Posted by: Parkman Posted at: 2018-06-05T03:29:42.738Z Reads: 283

```
I used Flipsky vesc 4 with aluminum enclosure for two month in BLDC mode. 
Today, I am bored, so I tried FOC mode. There are no problems to set up.
( 6s battery, motor +- 50a/ battery +30 -10a /arkmania 3.101 firmware in BLDC and FOC)

I ride about 20km for one hour and I am still safe.  
Foc is more soft, brake very smooth but torque is weak. It is hard to uphill. 
I changed motor amp +-60A, still a little weak. +-70A? seems dangerous 
Where is startup boost or ramp step in Foc? 

anyway, I am safe. If there is some accident, I will post again.
```

---
## \#165 Posted by: TarzanHBK Posted at: 2018-06-05T05:36:08.646Z Reads: 284

```
[quote="Parkman, post:164, topic:51591"]
arkmania
[/quote]
@Ackmaniac is that your sister or something? :rofl: 
Love how people mess up names.
(I'm pretty sure i changed some in a funny way too)
```

---
## \#166 Posted by: Parkman Posted at: 2018-06-05T06:09:08.670Z Reads: 287

```
Ha ha ha :sweat_smile:
```

---
## \#167 Posted by: Benjamin899 Posted at: 2018-06-07T20:03:56.095Z Reads: 281

```
i thought the FS esc 4 is without enclosure....this is getting confusing
```

---
## \#168 Posted by: banjaxxed Posted at: 2018-06-07T21:29:39.312Z Reads: 276

```
Very interesting a huge esc with many component changes, loosely based on the vesc6, untested & seemingly marketed in a way certain to cause offence.

Caveat emperor
```

---
## \#169 Posted by: moon Posted at: 2018-06-07T21:31:40.372Z Reads: 276

```
I know all they had to do is copy the schematic and change nothing :) and everyone will  be satisfied
```

---
## \#170 Posted by: banjaxxed Posted at: 2018-06-07T21:33:49.368Z Reads: 272

```
FriSky business this ESC game
```

---
## \#171 Posted by: squishy654 Posted at: 2018-06-07T21:48:58.769Z Reads: 274

```
[quote="trampa, post:147, topic:51591"]
As you can clearly see, there is no monopoly.
[/quote]


they why do you go around threatening the competition with cease and desist letters saying it's a copyrighted product? If you wish to portray this lack of monopoly? you seem like the type who wants his cake and eat it too, am I right?   ...I like that...just be honest about it..
```

---
## \#172 Posted by: trampa Posted at: 2018-06-08T06:46:12.576Z Reads: 288

```
[quote="squishy654, post:171, topic:51591"]
it’s a copyrighted product
[/quote]
What is "it"? 
All VESC-Stuff, a specific hardware design, the software code, the firmware, the hardware schematics, a specific products appearance? 

What do you mean by copyrighting? You can't copyright a product. Copyrights are assigned automatically to the author of certain forms of creative work (e.g. software code). You can't even get rid of your copyright. You have it automatically, whether you want it or not. This is why the GPL exists. It's a copyright license!

Google: what is:
a) a copyright 
b) the GPL-copyright license
c) the purpose of trademarks
d) Open Source projects with Trademarks

https://en.wikipedia.org/wiki/Copyright
https://en.wikipedia.org/wiki/List_of_trademarked_open-source_software
https://www.gnu.org/licenses/gpl-3.0.en.htm
```

---
## \#173 Posted by: thamer Posted at: 2018-06-24T01:36:23.407Z Reads: 282

```
Hi Guys!!

Today I received the FESC 4.12 from FlipSky and as soon as possible I will test it and give you more details. The alluminium case is nice and the product seems to be good!!

See you!!

![IMG_2707|375x500](upload://yVeomBurNJM2nf2IumHneDvr95z.JPG)
![IMG_2702|375x500](upload://zWjCjlowpGdjnIeoKjIlTn08CE.JPG)![IMG_2705|375x500](upload://smY1ZoATQd45oL15XMd7JherRaL.JPG)![IMG_2711|375x500](upload://iOswK6jg7kWVQQpLViOnATaD153.JPG)[Uploading...]()
![com-rotate|169x300](upload://jjV47lF8M1MRB8ir7EUTahFsWfp.gif)
```

---
## \#174 Posted by: Benjamin899 Posted at: 2018-06-24T02:12:33.655Z Reads: 276

```
looks cool.is it purely for protection or is it made to cool the fets a bit
```

---
## \#175 Posted by: strattos Posted at: 2018-06-24T03:14:10.388Z Reads: 279

```
There's thermal tape on the case so you'll get some cooling. Better than nothing I guess
```

---
## \#176 Posted by: thamer Posted at: 2018-06-24T19:21:40.689Z Reads: 273

```
Yeah!! It works for both, as @strattos said there is like a thermal tape for colling the MOSFETs (look at second picture). So it will get some colling. In addition, the case protects well all the electronics and connections and have some screw spots for fasten under the board.

I liked it, very well made.
```

---
## \#177 Posted by: Benjamin899 Posted at: 2018-06-24T19:23:11.031Z Reads: 272

```
cool thanks, now i see it.
```

---
## \#178 Posted by: boardman Posted at: 2018-07-03T18:50:27.062Z Reads: 266

```
Any Updates? They're having a sale right now so I would be interested in hearing how good these are. Also would you recommend the heat sink? I'm probably going with a 12s2p configuration for reference
```

---
## \#179 Posted by: Benjamin899 Posted at: 2018-07-03T19:15:06.930Z Reads: 272

```
Got mine today, now i am waiting for the vesc itself.
![IMG_20180703_210903|281x499](upload://1Rt6D8KygTchcfuWpDvjslbyCT8.jpg)![IMG_20180703_210914|281x499](upload://jiGShYARb1gxqsdqb9FJWgdrAfv.jpg)
```

---
## \#180 Posted by: PartyPoison Posted at: 2018-07-03T22:26:57.978Z Reads: 273

```
![DSC_1228|281x500](upload://28PPNRm3IkKvy0qQn2wi66Gehwa.JPG)i won this from the raffle :-)
```

---
## \#182 Posted by: jason182 Posted at: 2018-07-10T03:49:44.224Z Reads: 281

```
I've been using two FS4.12 for about 6 weeks and haven't had any issues with them. I've been experimenting with different setups and just moved over to dual drive with two FS4s about two weeks ago.  I did have one small problem where I blew two of the Flier 120A power switches but I have a feeling those should only be used with 6S builds even though they say otherwis. I changed to the Flier 300A power switch and haven't had any issues yet but it's quite a bit beefier so I hope it seems to be holding up well on a 10S build. I've recently been using the FS6 and had several issues where the power switch kept going out on me but it wasn't killing the ESC just the push button switch. So I changed that to a suggested replacement from a friend  and haven't had any issues on the FS6 build since.  I didn't like the case in the F6 due to the bulky size so I had it removed and just installed with a heat sink. Now I'm in the process of trying to put usb ports in the enclosure so I have easy access to connecting to the vesc tool. It's a pita trying to open the electronics enclosure every time you want to make a small adjustment in software. Oh well, live and learn...hopefully gain some experience in the process. Here's a few pics of trial and error. :) Well, I guess I can only load one pic since I'm new here. Here's a pic of the FS6 removed from enclosure with an added heatsink. ![%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20180710104802|375x500](upload://6Ke7JZdTRtwGvlRqEWsckXwN5dm.jpg)
After removing from the case and adding heatsink it turned out to be quite a bit smaller and was small enough to fit in my esc enclosure.
```

---
## \#183 Posted by: rey8801 Posted at: 2018-07-10T07:46:54.147Z Reads: 280

```
Great thank you for the review. Anyhow for the software adjustment you can just connect a Bluetooth module and make the changes over the VESC tool or the app.
```

---
## \#184 Posted by: Benjamin899 Posted at: 2018-07-10T09:15:50.334Z Reads: 284

```
I also have the fsesc 4.12 and i am Happy with It. Especially for that price...56€ is a Killer deal
```

---
## \#185 Posted by: ricoghardforth Posted at: 2018-07-10T14:47:37.169Z Reads: 276

```
Is this case designed to be used directly on the deck or in another enclosure.  If it is are there any  caps or plugs available for the case to cover all the connectors over to make them muck and dust proof and maybe even splash proof.
```

---
## \#186 Posted by: PartyPoison Posted at: 2018-07-10T16:26:51.921Z Reads: 274

```
4.12HW Designed "In" the enclosure, 
the 6.6HW have case and "plugs" can be used outside the enclosure.
```

---
## \#187 Posted by: jason182 Posted at: 2018-07-11T03:03:36.525Z Reads: 273

```
@rey8801 Thanks for the advice about the bluetooth. I might need to look into a larger enclosure. I've got two vescs and a 300A Flier Power Switch in it. Right now it looks like a big bowl of spaghetti inside and I'm not sure I've got enough room inside at the moment for a bluetooth unit. I probably could cut some wire length off the ESCs and power switch to free some room though.
```

---
## \#188 Posted by: webst Posted at: 2018-07-12T14:52:23.712Z Reads: 261

```
Bluetooth units are small. METR 1.0 is like a stamp, albeit 3mm thick, so you should fit it somewhere.
```

---
## \#189 Posted by: Grozniy Posted at: 2018-07-26T16:27:47.905Z Reads: 253

```
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.de%2Fulk%2Fitm%2F362365819684

60€ with shipping
```

---
## \#190 Posted by: BilldisaBird Posted at: 2018-08-02T08:39:13.816Z Reads: 236

```
do you run these FS4.12 on BLDC or FOC ? cause i heard that other HW4.12 have buring issues with 8302 drv chip.
```

---
## \#191 Posted by: jason182 Posted at: 2018-08-03T11:30:43.256Z Reads: 229

```
I’ve been using FOC. I’ve not been having any issues with them as of yet. Only had issues with the flier 120v power switch but honestly those problems may have been my own doing because I just let them rattle around in the enclosure for the first few days before using double sided 3m tape to lock them in place. I moved over to a 300v flier switch from amazon and have yet to have issues with the switch failing.
```

---
## \#192 Posted by: Cloverr Posted at: 2018-08-08T06:21:04.390Z Reads: 218

```
can i see your 4.12 (with metal case) setup??
```

---
## \#194 Posted by: jason182 Posted at: 2018-08-14T11:33:24.439Z Reads: 214

```
We're the issue with FOC or BLDC? I just realized that I never really answered your question last time by just going on about the power switch. :) I did try BLDC but only briefly on the bench, once I tried FOC and realized it was almost silent while running the motor I decided to stick with that.
```

---
## \#195 Posted by: LEE Posted at: 2018-08-15T14:39:06.420Z Reads: 208

```
https://flipsky.net/collections/electronic-products/products/dual-fsesc4-12-100a
```

---
## \#196 Posted by: brenternet Posted at: 2018-08-15T14:46:29.274Z Reads: 211

```
This is magical
```

---
## \#197 Posted by: Riako Posted at: 2018-08-21T15:31:54.351Z Reads: 207

```
https://cdn.shopify.com/s/files/1/0011/4039/1996/files/V4_6_b932e4b0-5bb8-4a2a-a114-9255b219340a_2048x2048.jpg?v=1534836509
https://flipsky.net/collections/new-accessories/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike
Looks cool too !..?
```

---
## \#198 Posted by: Grozniy Posted at: 2018-08-21T15:45:38.208Z Reads: 202

```
Awesome one
```

---
## \#199 Posted by: Benjamin899 Posted at: 2018-08-21T16:55:15.392Z Reads: 201

```
thats rly nice. smaller than a focbox.
```

---
## \#200 Posted by: Newby Posted at: 2018-08-28T14:07:23.358Z Reads: 191

```
I made an offer on one of these on eBay of £40 and they accepted it. Can we play a game to see how low they go?
```

---
## \#201 Posted by: Octave Posted at: 2018-08-28T14:46:48.131Z Reads: 203

```
@Newby Can you give a link to the eBay seller
```

---
## \#202 Posted by: Hummie Posted at: 2018-08-28T16:22:03.670Z Reads: 205

```
doing a group buy on this one
https://flipsky.net/collections/electronic-products/products/dual-fsesc4-12-100a

https://www.electric-skateboard.builders/t/the-flipsky-dual-esc-group-buy-its-on-130-including-usa-shipping/65517

and the 6.6
https://www.electric-skateboard.builders/t/flipsky-groupbuy-again-120-including-usa-shipping-with-tracking/65563

they ship wednesday
```

---
## \#203 Posted by: BruSkater Posted at: 2018-08-28T16:25:03.215Z Reads: 201

```
Are you doing a grouo buyon thee dual 6.6 @Hummie?

https://flipsky.net/collections/new-accessories/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink
```

---
## \#204 Posted by: Hummie Posted at: 2018-08-28T16:36:47.652Z Reads: 193

```
i dont think we would hit the minimum needed and have my hands full already.  
they are also coming out with a 6.6 without the antispark which will make it smaller
```

---
## \#205 Posted by: Newby Posted at: 2018-08-28T19:28:49.914Z Reads: 185

```
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F283024783468
This is the UK item. If they do 2 for £70 you're definitely in for a deal considering last year it was that price for a single
```

---
## \#206 Posted by: SpeedyGonzales Posted at: 2018-09-19T21:38:41.880Z Reads: 150

```
I'm up for the next group buy for FSESC 6.6.
```

---
## \#207 Posted by: IcKOo Posted at: 2018-10-27T18:03:19.029Z Reads: 116

```
![44848403_1909333819104462_5821789910159327232_n|375x500](upload://vbWLlh56IOkBINa95PjntU14Vgx.jpeg) ![44878556_501650770312499_1239369824656687104_n|666x500](upload://TIO2hMqyamCtCwkaXedk4ssRQP.jpeg) ![Untitledd|690x458](upload://8QpvUqsFUFpy7wHhQQ1tF2vH4Cx.png) ![Untitlettd|531x500](upload://9mC2X0xNOaj9JMDKtXXDWQSguNa.png) ![Untitled|690x458](upload://sV4qBPug0c80VEQcc8gND2oO0PE.png) 

FSESC 6.6 mount on CCB (can bus bridge :)  and everything will remain waterproof + all add-on modules is inside
```

---
