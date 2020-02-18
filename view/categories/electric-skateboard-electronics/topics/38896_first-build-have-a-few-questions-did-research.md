# First Build, Have A Few Questions (Did Research)

### Replies: 36 Views: 1604

## \#1 Posted by: A-lone-tenno Posted at: 2017-11-21T09:56:56.551Z Reads: 166

```
So I'm new to this, been learning for the past couple weeks, hope I have a basic understanding of everything, but I might be completely off, so I wanted too make sure. Sorry for making a new post I get that that's annoying sometimes, it's just Im a kid without too big a budget....
Anyway here's what I have so far:
Battery:2 x ZIPPY Flightmax 5800mAh 5S1P 30C
Motor: Carvon v3 would be ideal, but if I can't find them I'll go for https://m.ebay.com/itm/Electric-Longboard-Skateboard-90mm-Dual-6364-Hub-Motors-Drive-Parts-Brushless/142536343656?hash=item212fd40068:g:un8AAOSwPoJZ3sG5 
Now I understand that's a terrible idea, but I really don't have that big a budget, and while I would splurge for the carvons, I can't find where to buy them, or hummies for that matter.
Deck: custom- skate free ride ( I'm going for a boosted board look)
Vesc: I don't know, I've checked but if someone could link a good budget one I'd be really grateful
Battery hub:https://m.ebay.com/itm/Nylon-Battery-and-ESC-case-for-electric-skateboard-longboard/263109909597 
I don't think I'm missing much, shrinks off Amazon, and a remote I'll find last
I've been skateboarding a long time, but I don't need this ridiculous 35 mph a 20-23 mph max would be fine by me, and I would like a safe mode that caps your speed to less as well. If I have any rookie mistakes I apologise in advance, and thanks to whoever takes the time out of their day to help me out.
```

---
## \#2 Posted by: pat.speed Posted at: 2017-11-21T10:20:24.544Z Reads: 155

```
Hey mate, it's lovely to see that you can see the benefit to spending a bit more money to get good parts. The batteries are good although if you would like a slimmer style you could get 5x 2s batteries. You can't actually buy the carvon motors by themselves so you would need to get them second hand, some people on here sell them. If you can't get carvons Diy electrics hubs are decent and their Vesc is the best budget Vesc. Lastly if the diy hubs are too expensive you could use a belt and pulley setup which is much cheaper
```

---
## \#3 Posted by: lasplaner Posted at: 2017-11-21T10:22:33.727Z Reads: 148

```
Are your batteries in Parallel (5S) or Series (10S). For a starter build, I wouldn't go for 10S. Tbh 6S is enough for me, but if you weight more than 70kg (155 pounds), then 8S should suffice.

Cheap (and mostly reliable) VESC:

products/torque-esc-vesc-bldc-electronic-speed-controller

Now if i were honest, a dual hub motor system would definetly not be good for your first board. That means you will need two of everything. 2xVESC, 2xMotor (duh). Get a single belt driven motor setup. That is much better.

For a Belt Driven setup, you will need:

- Motor (63+mm) from DIY, or other company. collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-260kv (6S-8S)
- Mechanical Kit. collections/electric-skateboard-motor-
- Trucks and Wheels. You will need **caliber** trucks. the DIY ones are here: collections/longboard-trucks/products/torqueboards-218mm-trucks
Wheels: collections/longboard-wheels/products/83mm-epower-flywheels-clear-blue Choose any color.
- Deck + 1 VESC + Battery.

It's not going to be cheap. Electric Skateboards are expensive, and even in DIY. I understand, but it is MUCH better in the long run to get a better quality build, then a bad one to last 2 days.

Remotes are the MOST IMPORTANT part of your setup. If you get one that disconnects, and you're going even "only" at speeds like 20km/h (12mph), you could suffer serious injury. Trust me, I know. (The remote wasn't bad, it was just physical malfunctioning. Not manufacturing problem) 
http://www.electric-skateboard.builders/t/broken-collarbone-from-diy-esk8/38017

So I would recommend this ridiculously expensive remote, but ULTRA reliable remote which fits in your hand PERFECTLY. It's also small.
http://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/

For this "safe mode", just set it in the VESC settings. I'm not going to get into it now, since you haven't even purchased it. Also, the remote has a beginner mode, which halves the power. It is great for cruising on flat ground, with the expense of lower-power braking as well, fine for flat ground anyway. This will limit your power, and then when there is a steep hill or place you want to go fast on, flip the mode to FAST, and watch your board fly!

-lasplaner
```

---
## \#4 Posted by: pat.speed Posted at: 2017-11-21T10:41:46.046Z Reads: 114

```
A much cheaper and even more reliable remote is the mini remote. Found on eBay, banggood and buildkitboards
```

---
## \#5 Posted by: A-lone-tenno Posted at: 2017-11-21T11:12:40.067Z Reads: 110

```
Ok first of all thank u so much for all of this. I thought about a belt and pulley but I'm worried the belt can fall off, and the motor is very close to the ground, and can get hit and stuff although I suppose the manufacturers probably thought of that. I weigh around 55- 60 kilos, and I know that 20 mph is really dangerous, I only said only because of the people on this forum who go crazy XD. I will look through the all the things you mentioned because they look amazing, and I just wanted to ask if I should stick with zippy lipos or maybe build my own pack... I have a soldering iron, my dad knows how to use it, I'm just confused as to how you charge it ( the pack), and how it doesn't overcharge and everything, but overall wouldn't that be more expensive ?( between the bms and the batteries and everything). Oh and with a belt I should still stick to 1 motor, or should I go 2 and then connect them to the same vesc ( I think that's possible,i may be wrong) Again thanks!
```

---
## \#7 Posted by: A-lone-tenno Posted at: 2017-11-21T17:54:22.206Z Reads: 99

```
I did my research, but i still dont know how many batteries to get. If i have as mentioned before, 2 x zippy 5800 mah 5s batteries in parallel ( because i dont know how to connect them as a series) how much range would i most likely get? I know people answered this but i cant find the formula... also, would i be better off connecting 3 x 3s 5800 in series if possible? The whole battery config confuses the hell out of me. And one last thing, with my flexible deck and 83 mm wheels, isn’t the motor really close to the ground? Dangerously so?
If someone could give me an ideal battery config, i would be really happy... thanks anyway. And how do you charge the batteries? Oh and is vesc/battery/motor cooling something i should worry about?
```

---
## \#8 Posted by: aigenic Posted at: 2017-11-21T19:07:14.827Z Reads: 97

```
[Here](https://carvonskates.com/collections/parts/products/carvon-v4-speeddrive) you can preorder carvons

You dont want 5s board...go for 6s at least :) 10s is used in most of our builds :) you just connect the batteries in series...[Like this](https://qph.ec.quoracdn.net/main-qimg-d1dbfd0a210295e37f1a7df66be93439-c)

To estimate your range use [this calculator](http://calc.esk8.today/) (10Wh per mile if you are going half throttle, about 17Wh if you go full speed all the time and accelerate much...efficiency about 90%)

If I were you I would use single belt drive, 6354 will be enough for your 60 kgs, if you want to leave most of commercial esk8 behind, then 6374 is the way to go :) (or more expensive dual)

VESC might get hot, but it monitors itself, so it shouldnt be a problem :) 
Batteries wont get hot if you buy good ones of higher discharge rating than  your max motor amps :slight_smile:
 
CHraging...for 10s you want to use BMS...it can be cheaper than hobby style charger if you make few compomises...
```

---
## \#9 Posted by: aigenic Posted at: 2017-11-21T19:14:13.637Z Reads: 90

```
With vanguard style deck you can always use bigger wheels like 90 or 97mm :) with 83mm it is doable even without risers, if you want more space, you can buy risers and the motor will be quite safe :) 

Budget VESC...mhmmm if you are from USA, then DIY VESC for sure, certainly the best budget VESC as @pat.speed said...[this](https://goaxle.com/shop/) VESC has also very good reputation, SOLD OUT ATM, didnt heard about them for a long time...if you could spent more, you can go for FOCBOX :)
```

---
## \#10 Posted by: pat.speed Posted at: 2017-11-21T20:05:46.079Z Reads: 84

```
Yep what aigenic has said is spot on. Your motor will not hit the ground and the belt won't come off because of the flanges on the pulleys. If you do go for a belt drive get a 190kv 6364 motor from HobbyKing, the brand I used is keda because it's cheaper but the sk3 brand is good too
```

---
## \#11 Posted by: aigenic Posted at: 2017-11-21T20:36:59.755Z Reads: 77

```
Yeah I used Keda motor too, they are cheap and work well :) SK3 motors are a bit more expensive, but bullet proof and more used :)
```

---
## \#12 Posted by: A-lone-tenno Posted at: 2017-11-21T20:49:28.140Z Reads: 74

```
Is there a universal size for the motors or are they all different sizes
Is the keda compareable to the diy motor? If so should i maybe get 2? I know that means 2 of everything but I’m trying to get as close as possible to the boosted board like build. And 2 motors doesn’t affect the batteries right? I plan on going 3 x https://hobbyking.com/en_us/zippy-flightmax-5000mah-6s1p-30c-xt90.html
In parallel, and if i go for the motors off hobby king ( the keda 63-64) will i be able to connect the pulley and belt and trucks and everything off the Diy kit? Because I didn’t find that on hobby king. Last thing, since I’m going 6s3p( 10s speed is too much) how will i charge the packs? BMS? I want to make a charging port through the battery enclosure, if someone knows how that’s possible? And a power button I use get off eBay and connect to the vesc i assume, but I’ve seen people talk about spark something, and i was wondering if maybe that’s super important and i just didn’t research it enough.... sorry for the amount of questions, Thanks for everything btw.
```

---
## \#13 Posted by: pat.speed Posted at: 2017-11-21T21:00:14.620Z Reads: 63

```
Well if you want a 6s build and a dual motor, I would say possibly dual Keda 240kv 6354 motors with 15/36 gear ratio on 83/90mm wheels. That will give you about 20mph and it should have plenty of power for someone your size. About the charger you can use a standard hobby charger from hobbyking (IMAX B6 is good, just make sure to get the genuine one) and get a 15v power supply of eBay. If you don't want to mess around with the charger a bms is the other option though more expensive and you will need a 25.2v charger which are hard to find
```

---
## \#14 Posted by: A-lone-tenno Posted at: 2017-11-21T21:37:38.291Z Reads: 62

```
I cant seem to find 6354 kedas, or 240 kv ones. Want to know if 2 keda 6364 190 kv would do me justice? I prefer a charger over a BMS , although I’m still interested in how it connects, and how i can make a battery port on the board. And would the dual motor mechanical kit off diy work with these motors?
```

---
## \#15 Posted by: aigenic Posted at: 2017-11-21T23:52:24.172Z Reads: 62

```
Only with extended caliber trucks, the classic length calibers are too short to fit dual 6364 motors...
You can also consider [this kit](http://www.diyeboard.com/dual-belt-drive-1400w2-n5055-motor-power-truckfront-truck-kit-p-422.html) 2x1400W, 270 kv, I saw some ppl use it, should work ok, even though it is from china...

5055 motors are smaller, more space under the deck

On 6s it would run like a butter :) But I do not recommend to run these motors on higher voltage...

If you want more power, go for dual 63xx motors :)
```

---
## \#16 Posted by: A-lone-tenno Posted at: 2017-11-22T14:19:02.931Z Reads: 63

```
So a couple things before I buy, say I were to go with the Chinese ones @aigenic linked, would I be able to upgrade to 5 mm 15t 13 mm pulleys? And change wheels? Because 12t seems somewhat weak according to the calculator. If not then I'll most likely go double / single ( still undecided ) 6364 kedas, and the extended calibers, although I would still need the pulleys and all, and I prefer to buy the wheels separate ( say I were to go w the diy kit). Wanted to ask about the antispark, and whether or not I should get one, and also how to charge my board ( a battery port ) as I'm still unsure how that's possible ( the articles I've read do not specify how they do it) other than that, everything else is pretty much fine I hope,
-6s3p lipos 5000 mAh, 
-Vanguard loaded (eBay)/custom skate freeride
-3d printed enclosures ( plan to go to a 3d printing place 141 USD (apparently eboosteds price) is way over my budget, will also look into the vacuum solution)
-single 6364 235 kv/ double 5054 270 kv
-caliber 2 trucks either way (extended if need be)
-vesc/double vesc, the one mentioned before
-imax b6 (hobbyking)+ charger off eBay
-mini remote, either eBay or enertion
-antispark? Still unsure what that is, would love to know if I need it.
-battery indicator? Would like one but unsure as 2 how it works
-power button? Same as battery indicator.
-orangetan kegels/abec 11 flywheels 83 mm off eBay ( originals tho, not clones)
That's my build as of right now, anything missing by any chance?
And of course a helmet and kneepads be cause safety first.
And a huge thanks to anyone who's helped me until now
```

---
## \#17 Posted by: aigenic Posted at: 2017-11-22T14:53:36.975Z Reads: 55

```
AntiSPARK...mmmmhm...if you connect your battery to ESC directly, it can spark a little and cause a little dmg to ESC, after soem time your ESC might stop working...there are tow ways to prevent them:
ANsti spark switch with power button...costs about 60$, works well, cleaner solution...
Anti spark loop key...lasts forever, much cheaper, made of XT90s connectors, not as clean solution...

Both of these work as on/off switch

About the gear ratio...it is certainly changeable, but IDK if the motor can be moved on the motor mount..it would complicate things a little...

IMAX is the best, just make sure that you are not buying a clone :) 

3D printed enclosures are good, but the are not bullet proof, I have broken one after a week of using...now using glass fiber :) 

You plan on connecting 3 6S 5000Ah batteries in parralel to get 6S3P?

If you buy the kit I mentioned, the wheel pulleys will fit ABEC flywheels :) for oragnatang you would need different pulleys...
```

---
## \#18 Posted by: A-lone-tenno Posted at: 2017-11-22T15:12:34.226Z Reads: 58

```
Yes, in parallel, and thank u for the antispark knowledge, I would prefer to change the gear ratio, but only if it wouldn't damage the motor... 
If u don't mind me asking, how did u get the fiberglass enclosures? Wondering how much that solution would cost, maybe less then going to the nearest 3d shop? Anywho, now the only thing I'm missing is charging, I'm confused as to what cables Connect to where and how, and if it's possible to mod it to a charging port... Anyway, none of my friends believe me that I'm going to build it so I can't wait to prove em wrong XD
 Thanks @aigenic !!
```

---
## \#19 Posted by: aigenic Posted at: 2017-11-22T16:22:03.912Z Reads: 55

```
Np :slight_smile:
I made them myself :) It quite easy, if you use glassfiber with polyester resin it is cheap, in my case it was cheaper than 3D printing...if know somone with 3D printer who could print for you easily, go for it, other way I would go for fibrglass :) if you want better results, you can buy cheap clothes vacuum bag with pump and use vacuum bagging, but normal hand layup is good enough :)  Just do not expect nice results with your first enclosure...

A lot of ppl here use lunch boxes (or something similar) as enclosure on their first build, its the cheapest option.

Now abourt charging...if you want to use IMAX, then you can make it in these two ways:
1. Remove the enclosure and charge each battery separatly
2. Use a [9 pin connector like this one](https://www.ebay.com/itm/Pair-Waterproof-Aviation-Cable-Connector-w-Socket-SD16-9-9-Pin-IP68/311272378332?epid=1238406513&hash=item4879478fdc:g:k7IAAOSwZqZZ8K64) to charge it, when you have all the batteries inside the enclosure you owuld also need balance lead paralel harness, which would be connected on the balance leads and the 9pin connector inside the enclosure...This is more complicated...

Note: When you are balance charging, you have to connect 9 wires to the charger...7 balance wires, plus and minus wire...

If I remeber correctly you gave up on the BMS...


Canging the gear ratio wont dmg your motor :)
```

---
## \#20 Posted by: A-lone-tenno Posted at: 2017-11-22T16:54:43.949Z Reads: 50

```
The new motors saved me a couple hundred bucks, so I don't mind at all going bms if that's what I need to charge, because taking the batteries out every time seems like kind of a hassle you know? Thanks for all the amazing advice man!
```

---
## \#21 Posted by: Hummie Posted at: 2017-11-22T17:31:30.394Z Reads: 54

```
does diyelectricskateboards' vesc do foc?  seems a lot of people have broken them.  6s is too low a voltage and I bet you have temp shutdown  unless you are a mellow rider.  any  motor will be fine on 12s or 10s but maybe you'd need to limit the rpm with the vesc

there are other ways to charge and balance than a bms.  look up "discharge balancer"  and a full voltage power supply

sparks from connecting batteries to esc don't damage the esc just the connectors.  xt90s don't last forever.
batteries get hot from battery amps not motor amps.  this thread is a bunch of disinformation.  if youre being cheap that is not a cheap remote and theres others that are reliable and much cheaper.  mini trigger for one
```

---
## \#22 Posted by: A-lone-tenno Posted at: 2017-11-22T18:04:36.716Z Reads: 51

```
This for instance?
http://www.myrcmart.com/rcx-3in1-battery-balancer-discharger-voltage-indicator-150w-discharging-p-4767.html
Not trying to be too cheap with important stuff, i just don’t have too big a budget...
When you say full voltage, what voltage are you referencing? 
Ill take your advice with the mini trigger and the anti spark switch, but i dont understand what you said about 6s not being enough, the motors say they max out at 6 cells, so I’m kind of confused. I’m willing to go over 6s and just configure the max speed in the vesc, if that’s what will solve the problem, although honestly I’m unsure as to what that problem is (still a newbie, sorry if I’m being ignorant)
```

---
## \#23 Posted by: Hummie Posted at: 2017-11-22T18:28:07.067Z Reads: 56

```
why motors put a max voltage ...makes no sense.  amps make a motor hot so they are the real limit.  the only other limit would be the speed the bearings can go and its true that with smaller motors they generally have a higher kv so will go faster per volt...or you could get higher spinning bearings even.  I wouldn't worry about it.  the enamel on the wire is good for surely way more voltage.
I mean full voltage of your complete battery.  you can bulk charge it and use the balance dischargers on the cells to monitor and discharge balance.  theyre slow and its safer just to charge each cell to 4.1 to give headroom just incase.  the discharger you linked has additional bulbs that can be added to increase the discharge rate to 150watts.  I have those but they're a pain and require a certain plug but they might be good for you.  Some people think bulk charging and side balancing is too complicated and dangerous for new people.  its easy and just don't let any cells go over 4.2 to be safe or even 4.1 to have them last a lot longer and be much safer. the vesc has low voltage cutoffs so it will shut down when the whole battery hits a certain low voltage you set it to.  give it some headroom there too and with lipo you can get down to 3.5 and they will live a long time.  3.0 is possible but they last less cycles and since you'd have no bms to cut off any specific cell that went too low and only the whole pack voltage is monitored its' better to stay at 3.5.  theres not much under there anyway and there's a cliff at mayb 2.8 and if the cell falls off that you might not get it back and it can be dangerous trying unless youre very cautious.

the vesc cant do many amps before it gets too hot.  a hobby store 150amp esc on 6s would be fine probably but 6s on the vesc or even 8 ...with amps and volts equaling power you have less voltage to add to the mix and are relying on just hot amps in the esc.  maybe 6s would be ok if you add a heatsink to the fets.  but get a decent vesc and they're often a problem if you get them some places.  

Id go 10s at least if doing one motor.  you can limit the erpm easily in the settings and figure that when you get it if need be.  
12s even better.  a good vesc.  some lipo.  minitrigger.  bulk charger and 2 balance dischargers is what I recommend if you want to be cheap.  but this isn't just cheap it's reliable.   the one thing that's weird I recommend is adding a wattmeter in line with the bulk charger so you can see what voltage it will put out.  a wattmeter there, soldered between the power source and its plug that will go to the battery (xt90s is awesome) and will tell you a lot and give you a lot more control and safety.

always be around when charging.  its much better to be able to see and feel your lipos when charging to make sure they aren't getting hot or puffing.  a little bit of a permanent puff in a cell from discharging is ok but you have to be careful of heat and puff as they're the signs of too much going in or out..or a cell being damaged.  lipo are more easy to physically damage.
```

---
## \#24 Posted by: A-lone-tenno Posted at: 2017-11-22T18:50:48.593Z Reads: 46

```
I’m prefer dual motor if possible (OCD) but i think i understand the part about the vesc/esc, what you are saying is for an vesc i should go 10s/12s to not heat up the vesc witch would heat up because less voltage = more amps= more heat. 
As for the battery config, the lipos are connected to the vesc, and the balancer in parallel , or is the balancer between the 2, or do i have it completely wrong? And you mentioned 2 balancers for charging, I’m confused as to how they would connect to the lipos and how the lipos would stay in sync, and also, 
Do i have it completely wrong? The discharges are in the enclosures at all time, only the charging cable is used to charge correct? And the cable connect the the balancers, witch in turn connect to the batteries? And for instance if i were to somehow make a port, the connection would be between the charger and the balancer? I hope i understood this correctly, and that I’m not hopelessly off... 
anyway i just wanted to say that I’m a fan of what you do and that I’m really happy that you took the time to help me out
Oh and the charger, just any old charging cable off eBay with the correct voltage or is it one with a special connector?
Thanks @Hummie
```

---
## \#25 Posted by: Hummie Posted at: 2017-11-22T19:10:43.988Z Reads: 44

```
dual is nicer and the vesc has traction control that makes it really shine.  

yes with the less amps with more voltage 

you don't put the balancer in the board it just goes on any other time.   so take the xt90s plug out of the vesc, if you were just riding, and plug it into the power supply to charge, after the power supply is already plugged into the wall, and you checked the wattmeter wired onto it to make sure what voltage will come out is what you want, ...actually step back a bit and plug the discharge balancer into the cells first and leave it plugged in.  it will balance them all down to the lowest whenever it's plugged in.   you can leave the balancer plugged in anytime so if you want to completely balance the cells you'll have to leave it on a while.  the balancers without the bulbs, as I use it, takes a long time.  I do it anyway.  sometimes the balancer will shut off from maybe being too hot.  take it off put it back on screen comes back.  they're really weak things and been all over trying to get a small 12s more powerful one 
you cant use any old of ebay.  I'm not sure how close to "any old" you can do but remember it being important for it to be "regulated"  it could be a switching or linear supply and those differences are interesting but unimportant.  so some laptop supplies are good some not.  but if you want to be cheap and safer and with more control get an adjustable one.   someone here linked me to this beauty with golden knob and lucky led screen.  but sold out and I got it! https://www.amazon.com/LM-High-precision-High-stability-Certification-Communications/dp/B06ZYDZCG9/ref=sr_1_4?ie=UTF8&qid=1511377469&sr=8-4&keywords=switching+power+supply+60v
this is to 60v and I'll only charge to 50 and it says adjustable but not sure if it can get down there.  got it like that assuming the components will be more robust.   As soon as I get my hands on a three prong tail cut off a microwave and another found couple wires.  these things are weird and I advise mounting it on the wall.  I've dropped mine many times and it has broken.  long long plugs and mounted on the ceiling next time.  and wattmeter potted into the plug rock solid biggest plug the better. charge in an aluminum trash can or better a metal filing cabinet you can roll outside if things went wrong and maybe you should do this regardless of what you charge with maybe even a bms.
 I like to talk about charging no problem.
but maybe you don't want to do any of this and get a bms instead.  maybe its safer.  its not cheaper,  reliability is debatable, its way more powerful and fast, leaves you with more space in the board.
```

---
## \#26 Posted by: aigenic Posted at: 2017-11-22T19:35:54.942Z Reads: 40

```
About the ESCs...there are a lot of ppl using VESC on 6s and you would be using just 1400W motor on each, so the load would not be that big, about 63A,which would probably get theVESC hot, but remember all those guys running single 6374 with 80A :O 

Otherway you can buy twin 6S ESC, [this one](http://alienpowersystem.com/shop/esc/alien-120a-2-7s-ev-esc-bec-twin/) could work, I am using similar and it is good, even the brakes work well, if you set them up correctly :) There are also some on ebay, but they usually have bad brakes, can not be set up...

Or you can buy 2 6S ESCs and use signal amplifier (maybe differnet name) for the reciever...

P.S. I love you @Hummie, it is nice that a "big fish" like you comes to help begginers
```

---
## \#27 Posted by: Hummie Posted at: 2017-11-22T19:38:54.106Z Reads: 46

```
Ive never read of people using the vesc and one motor or two and just 6s.  I have read of people having trouble on 8s.  but all depends what youre doing I guess.    

and I love you too @aigenic.  and newbies.
```

---
## \#28 Posted by: A-lone-tenno Posted at: 2017-11-27T18:58:10.784Z Reads: 44

```
Ok so I'm looking at the deals, ready to buy, as of right now this is what I'm looking at as of right now

Remote: DIY / tb 2.4 remote, on sale
Kit: also diy single motor kit (with trucks and wheels)
Motor: sk3 6374
Batteries: 10s3p zippy lipos 2700 mAh 35c(say I have 4 in series, can I connect 2 more I'm parallel?)
Vesc: diy ( can't afford focbox)
Power switch: will buy, don't know which, noticed that on their site there where different types, wanted to know if there is a difference
Bms: unknown
Charging: working on it
Deck: vanguard second hand/ freeride

Only problem now is enclosures, and how do I connect the cables over the deck? What type of flat wire do I use to do so? If someone could link something it would be great, if searched but people who did it didn't really explain how and with what....
Anyway, if I have any mistakes, things missing ( I just want to make sure I don't buy everything and then I won't be able to connect them because they're incompatible/ different connectors and whatnot) 
If that's all I buy will I have a fully functional board?
Btw thanks in advance!!!!
```

---
## \#29 Posted by: aigenic Posted at: 2017-11-27T21:09:52.069Z Reads: 39

```
Remote: OK, [This one](https://www.ebay.com/itm/Radio-2-4GHz-Remote-Controller-Receiver-Binding-Plug-For-Electric-Skateboard/253250151161?hash=item3af6e2a2f9:g:kWQAAOSwZtlaBBPK) is cheaper, doesnt loose signal...
Motor: I guess you plan on using 192kv?
Betteries: If i understand your question right, then no, it is not possible...
VESC: FOCBOX is on sale! Buy if you can afford it :) http://www.enertionboards.com/
Power switch: I see just [this](collections/electrical-connectors/products/on-off-power-switch-electric-skateboard) one there

Wires: [here](https://www.ebay.com/itm/1m-3-3ft-6-8-11-12-15-22mm-Flat-Pure-Braid-Cable-Copper-Braid-Wire-Ground-Lead/263047137847?var=562049951716&hash=item3d3ed4ca37:m:m5k4VYQSx8m5WwikUDbnjJQ), you just have to find how much amps which one transmits...you will need 80a at least if I count correctly
```

---
## \#30 Posted by: A-lone-tenno Posted at: 2017-11-27T21:25:46.108Z Reads: 39

```
Yea it's on sale for really cheap, but it doesn't ship to where I live and I only go to the us in Feb, and I have no where to keep it...... The focbox and the remote both would buy but it won't work out, and the switch is sold out but I guess I'll just wait, and do I also need an xt90s loop key, or is the switch enough?
And those wires look great btw thanks, and when u said how many amps, what changes it? Now all I need is patience and I hope the airport won have a problem with the motor or anything...
Thanks!
```

---
## \#31 Posted by: aigenic Posted at: 2017-11-27T21:52:23.118Z Reads: 34

```
If you have XT90s loop key, you dont need a switch :)
```

---
## \#32 Posted by: aigenic Posted at: 2017-11-27T21:55:56.435Z Reads: 32

```
I meant with it that you have to make sure that the wire choosen by you can transmit enough amps, otherwise it would burn out...If i remember correctly 12mm wide wire can transfer enough amps, but I am not sure, you will make better if you ask the seller or look for it on their webside, if they have any...
```

---
## \#33 Posted by: A-lone-tenno Posted at: 2017-11-27T22:05:36.399Z Reads: 33

```
Thanks but if I have a switch would I need a key? Or also no?
```

---
## \#34 Posted by: aigenic Posted at: 2017-11-28T05:41:19.386Z Reads: 31

```
No
10 char
```

---
## \#35 Posted by: A-lone-tenno Posted at: 2017-12-31T17:03:47.110Z Reads: 28

```
say i have this diagram right:

<img src="/uploads/db1493/original/3X/b/4/b48d190645fdff6e037c8d9665b0e53eca3c472e.png" width="270" height="500">

in places like the battery meter how do I make split the cable like that? is it with this?
<img src="/uploads/db1493/original/3X/1/8/18d558888f889ff085c0731968e0c9d28cd42f99.png" width="145" height="105">

and the red cable thats splits for the charging port. what do i use? basically how do I make 1 cable 2.

and say its dual motor, do i feed both cables into the master vesc, or do i split each with the image before?

and as for the charging port,
<img src="/uploads/db1493/original/3X/8/d/8dfe14d277d80bf8911eba06a625762c0ff519c6.png" width="225" height="181">
how does this connect to the bms? do i cut the white part and solder it? cause i didnt see a balance port on the bms for charging. did i just miss it?
 i've been searching for a long while, but it seems like most people just kinda know these things, and i feel like im just out of the loop, ik that i need to research, but im just reading the same posts over and over, so yea....
did i get it right?
```

---
## \#36 Posted by: aigenic Posted at: 2017-12-31T17:30:26.599Z Reads: 24

```
You cant use 12S on VESC with 230kv motor, you are exceeding eRPM limit! :) You can limit that, but you will never reach the motor's full potential...
```

---
## \#37 Posted by: A-lone-tenno Posted at: 2017-12-31T17:31:29.050Z Reads: 25

```
yea thats a mistake, its 2 170 kv motors (hopefully)
```

---
