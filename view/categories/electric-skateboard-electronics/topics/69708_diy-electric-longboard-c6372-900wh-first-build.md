# DIY electric longboard - C6372 - 900Wh - first build

### Replies: 35 Views: 581

## \#1 Posted by: TheRafter Posted at: 2018-10-01T05:49:27.014Z Reads: 162

```
I recently decided to take on the challenge of building an electric longboard. I've never owned one and have only ridden one a few times, though I use my non-electric one all day every day. There are a few bumps that I just cannot figure out though. My build includes 4 14.8v 16ah Lipo batteries, a C6374 2900w motor, VESC, BMS, etc (I will put links to my parts below). The main thing that I am stumped on is, the motor says it is 24-36 volts. I want to have two sets of batteries plugged in series, then plug those sets parallel, so I'll end up with 29.6 volts in the end. I would want to get as close to 36 volts though as possible to get maximum power, right?

Also, can I discharge these batteries fully then just charge them up, or do I have to get a voltage regulator to make sure they don't go below a certain voltage?

The VESC has a continuous output of 60 ampres , but a max output of 120. I don't know what that relatively means, is 60 amps enough? I would like to get one to match the motor with 100amps, but I fell like that would be overkill and pointless.

Also, I was planning on only using the BMS to charge the board, not for the output to the motors. With my four Lipo batteries, I would end up with 947.2 watt hours - that should be enough, right? I know it will suck a lot more battery because it has no BMS, but again I'll probably never use full power as someone who did a similar build made theirs go ~55mph. (although it all depends on the pully ratios and all).

Lastely, I'm not super familiar with how BMS' work. If I put my batteries in series as mentioned, I'll end up with 8s (4s per Lipo). Does that mean I have to get a 8s BMS, or will a 10s work? Also, the one. I have below is a 36 volt BMS, will that work or does it have to be the exact voltage (29.6)? 

Most of this is dependent on the very first question, if I need 36v to achieve maximum power. If not, them I'm good, but if I do, then I want to try to get as close to that as possible. I don't want to use 18650's because I'm not sure how to build them myself and can't find a good enough pre-built one. Also, these lipos that I have have a much greater discharge rate if needed (for the extra boost).

I hope at least some of the made sense. Thanks for the help in advance.

Battery:
https://hobbyking.com/en_us/multistar-high-capacity-16000mah-4s-12c-multi-rotor-lipo-pack-w-xt90.html

Motor (I don't think the stats on this is correct, they are 2900w not 3600.):
https://www.amazon.com/gp/product/B07FSVKYQB/ref=as_li_tl?ie=UTF8&amp;camp=1789&amp;creative=9325&amp;creativeASIN=B07DNWKS58&amp;linkCode=as2&amp;tag=skatemetric01-20&amp;linkId=c948d644ccd47683c0e5bfd113972766&amp;th=1&amp;psc=1

VESC:
https://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

BMS:
https://www.amazon.com/Lithium-LiFePO4-Battery-Protection-Balancing/dp/B073VMYFM5/ref=sr_1_1?ie=UTF8&qid=1538371882&sr=8-1&keywords=10s+bms&refinements=p_72%3A2661618011

UPDATE:

Now that I think of it, I do realize that I will never need 100 amores for the motor. 60 ampres should be more than enough. I will then need a BMS, but I could limit it to 60 amores, right?
```

---
## \#2 Posted by: b264 Posted at: 2018-10-01T06:03:50.667Z Reads: 132

```
900Ah is ridiculously big and will weigh more than you
```

---
## \#3 Posted by: TheRafter Posted at: 2018-10-01T06:09:31.776Z Reads: 131

```
I realize it will be large and weigh a lot. It will be roughly 10lbs, but weight isn't a very big matter for me. Because I am not going to have a BMS, I will need the large capacity, bout this is all still subject to change.

Thanks for you input though.
```

---
## \#4 Posted by: b264 Posted at: 2018-10-01T06:10:00.777Z Reads: 130

```
[quote="TheRafter, post:1, topic:69708"]
I know it will suck a lot more battery because it has no BMS
[/quote]

It will just cause it to not charge properly and damage the battery eventually.  It should not make the charge last less long.
```

---
## \#5 Posted by: TheRafter Posted at: 2018-10-01T06:11:14.488Z Reads: 123

```
I will have the BMS to charge it, just not to restrict the output to the motors.
```

---
## \#6 Posted by: b264 Posted at: 2018-10-01T06:11:57.415Z Reads: 118

```
[quote="TheRafter, post:3, topic:69708"]
It will be roughly 10lbs,
[/quote]

No, a 900Ah battery will be about 350 lbs
```

---
## \#7 Posted by: TheRafter Posted at: 2018-10-01T06:12:58.070Z Reads: 115

```
Haha, my bad. I meant watt hours.
```

---
## \#8 Posted by: Grozniy Posted at: 2018-10-01T07:58:18.560Z Reads: 110

```
What is your budget?
Do you plan on not upgrading your board?
Those batteries are bad. If you go lipo, save money for the future and get turnigy graphene >60C discharge.
There are plenty of great battery builders here, depends on where you're based.
I think it's possible to make work 10s bms on 8s, but safer is just using 8s bms. Do not go cheap on bms, it will burn your house. Choose bestech or supower.
Last thing: this hobby is expensive
```

---
## \#9 Posted by: Superflim Posted at: 2018-10-01T07:59:03.260Z Reads: 107

```
Can confirm. Very expensive
```

---
## \#10 Posted by: TheRafter Posted at: 2018-10-01T08:13:09.983Z Reads: 105

```
Right now, I'm just messing around. For all the parts I have so far (including decks, trucks, other electrical components, etc), I'm at $1,300.

What make the batteries bad? I've seen videos with other people recommending them. Also, the pack a large capacity in a small area. I need the power to get 900wh.

I did actually just find a 8s bus, so that Is no longer a problem.
```

---
## \#11 Posted by: Grozniy Posted at: 2018-10-01T08:32:41.453Z Reads: 98

```
https://www.electric-skateboard.builders/t/multistar-battery/16628/19?u=grozniy
https://www.electric-skateboard.builders/t/multistar-6s-8000ah-10c-in-2p/44337/13?u=grozniy
```

---
## \#13 Posted by: b264 Posted at: 2018-10-01T10:39:05.869Z Reads: 81

```
[quote="Grozniy, post:8, topic:69708"]
this hobby is expensive
[/quote]

It's not a hobby for some folks, unless minivan-driving is a hobby for a soccer mom

You're doing yourself and all of us a disservice by spreading the myth that these can only be toys and not tools.
```

---
## \#14 Posted by: electric Posted at: 2018-10-01T10:45:17.801Z Reads: 79

```
Maybe soccer mom's hobby is being a mom.
```

---
## \#15 Posted by: Skunk Posted at: 2018-10-01T10:52:24.765Z Reads: 78

```
[quote="b264, post:13, topic:69708"]
spreading the myth that these can only be toys and not tools.
[/quote]
Why not Both? 
But they can be toys.
I've had cars that are tools
But I've also cars with only a driver seat, no interior and its sole purpose is to go sideways around corners
```

---
## \#16 Posted by: b264 Posted at: 2018-10-01T11:28:58.889Z Reads: 75

```
Cars are super-dangerous and kill more people than most other things.  If cars were viewed as "toys" by the general population, they'd CERTAINLY be illegal to drive on public roadways.

But, they're not.  The public views them as "tools" for transportation and, as such, tolerates the danger for the better public good.

I use esk8 as my own CLEAN transportation, in place of a car, and other people spreading a myth and referring to them as "a hobby" just means it's ever slightly more likely that *my way of life will be outlawed* and thier toy might get taken away.  If you call it a hobby, someone else might, and someone else might, and people who know nothing about esk8 will hear that and pick-up that these are toys, which means they are ***BANNABLE***.  Because laws are based only on what Joe-Blow-non-Esk8r thinks.  Whether what Joe Blow thinks is wrong or not, doesn't matter.  The laws will follow public opinion whether wrong or right.  So spread helpful information, not hurtful information.

So, enough with the "hobby" nonsense.  I use these fucking things to get to work and go grocery shopping, and I don't need my way of life outlawed because you use them as toys.

Admittedly, when I still drove a car, I didn't make my own car...but some folks do
```

---
## \#17 Posted by: Jc06505n Posted at: 2018-10-01T11:43:36.661Z Reads: 64

```
*staring into a mirror in a candle lit room”

Hobby Mary Hobby Mary Hobby Mary
```

---
## \#18 Posted by: Skunk Posted at: 2018-10-01T11:45:42.095Z Reads: 64

```
I love poking bears. Thier so cuddly.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-10-01T11:50:44.443Z Reads: 71

```
don´t take things said too close to you ;) 
you just hit in a difficult topic with the words you choose.

Back to your plan.
why you think you need 900wh battery?
nothing bad with it, but if you don´t need a crazy range there is no need for it.
it will just make your board more heavy and more expensive.

a bms will not influence the voltage sag.
It depents on the quality of your lipos.

if you run an average board you can easily use a bestech bms with 80A
charge and discharge. 
If you plan to build a MTB and expackt to draw more amps than better no.
```

---
## \#20 Posted by: mixedcreation Posted at: 2018-10-01T11:52:20.288Z Reads: 68

```
.....and driving back on course.  Can you break down what exactly you are buying.  Also instead of amazon, you might want to look into actual E-board sites that sell quality products., @JLabs, @psychotiller, @hyperIon1.... hell there more than those as well.  Those are just a few.

So put up a list of what you have planned, then let some people scrub that list.  It seems like you know where you want to go, so let some of the experts get you there in one piece.
```

---
## \#21 Posted by: Skunk Posted at: 2018-10-01T11:55:00.292Z Reads: 55

```
Have parts from both psychotiller and jlabs.  Highly recommend
```

---
## \#22 Posted by: Andy87 Posted at: 2018-10-01T11:58:21.537Z Reads: 58

```
[quote="TheRafter, post:1, topic:69708"]
The VESC has a continuous output of 60 ampres , but a max output of 120. I don’t know what that relatively means, is 60 amps enough? I would like to get one to match the motor with 100amps, but I fell like that would be overkill and pointless
[/quote]

Motor amps not battery amps.
Your focbox can for example take 40a from the battery and make 80a for the motor out of it by lowering the voltage for the motor.
so you don´t need to worry, if you have a motor rated to 80a and run your focbox with battery max 40a it´s everthing fine.
```

---
## \#23 Posted by: L3chef Posted at: 2018-10-01T12:22:02.846Z Reads: 55

```
[quote="b264, post:13, topic:69708"]
It’s not a hobby for some folks, unless minivan-driving is a hobby for a soccer mom

You’re doing yourself and all of us a disservice by spreading the myth that these can only be toys and not tools.
[/quote]

Maybe he ment that building them is an hobby. Riding them are another thing
```

---
## \#24 Posted by: Grozniy Posted at: 2018-10-01T12:28:24.055Z Reads: 57

```
I meant that this is fairly expensive, hobby or daily driver transportation device. Reliable boards are expensive, cheap components will need to be replaced eventually.
```

---
## \#25 Posted by: Andy87 Posted at: 2018-10-01T12:30:15.598Z Reads: 57

```
expensive parts unfortunately also from time to time :sweat_smile:
but yeah, with e-boards better to go with quality parts
```

---
## \#26 Posted by: TheRafter Posted at: 2018-10-01T17:10:19.357Z Reads: 49

```
I would like extra range as this is going to be my main mode of transport. I am a collage student and my classes are 5 days a week and 2.5 miles from my dorm. I would also use it a lot more than just that, so extra range would be helpful. How long do you think 900wh would last with these motors without a BMS (though I would never give it full power because that would be ridiculous).
```

---
## \#27 Posted by: TheRafter Posted at: 2018-10-01T17:11:55.952Z Reads: 49

```
Some of the parts on the original list have changed and thus do not match with these. These are the most up-to-date parts.

***Battery:***

https://www.ebay.com/itm/173497574736

358.87

***Motor:***

products/electric-skateboard-motor-6374-190kv

120 x 2 = 240

***Board:***

https://www.skateshred.com/wholesale-blank-longboard-decks/36-x-9-5-bamboo-drop-through-deck.html

39.99

***Trucks:***

https://www.amazon.com/gp/product/B00NY3Q5Q8/ref=as_li_tl?ie=UTF8&amp;camp=1789&amp;creative=9325&amp;creativeASIN=B00NY3Q5P4&amp;linkCode=as2&amp;tag=skatemetric01-20&amp;linkId=bcc393c538aa16ebbd34e0f61a751c1c&amp;th=1&amp;psc=1

39.95

***Motor Mount:***

collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-w-drive-wheel-kit

collections/electric-skateboard-motor-mounts/products/single-bolt-on-motor-mount-set-only-black

106.99 + 60.00 = 166.99

***Wheels***

https://www.amazon.com/Orangatang-Downhill-Longboard-Skateboard-Cruising/dp/B07CLMPP98/ref=sr_1_sc_1?s=sporting-goods&amp;ie=UTF8&amp;qid=1538374348&amp;sr=1-1-spell&amp;keywords=orangoutang+wheels

68.00

***Bearings:***

https://www.amazon.com/Bones-Reds-Precision-Skate-Bearings/dp/B0798WGCB1/ref=sr_1_3?ie=UTF8&amp;qid=1538287755&amp;sr=8-3&amp;keywords=longboard%2Bbearing&amp;th=1

16.98

***Controller and Receiver:***

products/torqueboards-2-4ghz-nano-remote-controller

60.00

***VESC (Speed controller):***

https://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

138.55 x 2. = 277.10

***BMS:***

https://www.ebay.com/p/One-Protection-Circuit-Module-25a-BMS-PCM-for-8s-29-6v-Li-ion-Lipo-Battery-A72/2218162222

22.95

***Battery indicator:***

https://www.amazon.com/Searon-Battery-Indicator-Yamaha-Trolling/dp/B01LVUYS7S/ref=sr_1_6?s=sporting-goods&amp;ie=UTF8&amp;qid=1538280020&amp;sr=1-6&amp;keywords=battery+indicator

20.99

***Bushings:***

https://www.amazon.com/gp/product/B07F32W1JG/ref=as_li_tl?ie=UTF8&amp;camp=1789&amp;creative=9325&amp;creativeASIN=B07FH83HKS&amp;linkCode=as2&amp;tag=skatemetric01-20&amp;linkId=f246b436843e5da22d2c2544c5a08d26&amp;th=1&amp;psc=1

9.95 x 2 = 19.90
```

---
## \#28 Posted by: TheRafter Posted at: 2018-10-01T17:14:03.356Z Reads: 40

```
This is definitely going to be fun to ride, but mainly it is going to be my transportation around campus. It Is a 2.5 miles trip between my dorm and classes.
```

---
## \#29 Posted by: Pedrodemio Posted at: 2018-10-01T17:19:26.431Z Reads: 40

```
900 Wh you can get approximately 90km depending on riding speed

I think is throw money away using these batteries, size them for the tame you need and get a quality 18650 based battery, they will comfortably last way more than these
```

---
## \#30 Posted by: Andy87 Posted at: 2018-10-01T17:38:06.910Z Reads: 40

```
the bms doesn’t have an influence on your range.
The thing which has an influence is your riding style, the surface you ride on and if you use pneumatic wheels or urethan.
Out of a 10-12s4p which is between 400-500wh people get 25-35km, so with your battery you can easily hit the 60km if you don’t go uphill all the time.
If I remember right, there are even people here which need only 9-10wh per km, in this case you get your 90km like @Pedrodemio said.
Are you sure you need this extra range? 😜
```

---
## \#31 Posted by: mixedcreation Posted at: 2018-10-01T18:36:59.593Z Reads: 34

```
Ok I'll bite, why the do you need 900wh's?  If you are riding around campus, why in the world are you trying to build a 900wh setup for a first build.  That's like @PatRocks type of numbers...although I am sure less.  He had 950+wh's I am pretty sure.  His board is an absolute torque eating monster of a board. Although you are going to build a monster board for your first go?!?!?!  Man, I hope you gear up.  If anything, him as well as @Namasaki are some experts in the lipo category.  

There are so many builds for campus cruisers that make more sense for your scenario.  But good luck.
```

---
## \#32 Posted by: PatRocks Posted at: 2018-10-01T18:57:32.771Z Reads: 34

```
Lol, yeah I built big. 976Wh means I don't have to charge more than once or twice a month
```

---
## \#33 Posted by: mixedcreation Posted at: 2018-10-01T19:50:44.508Z Reads: 34

```
That is insane. I need new video on your build by the way. How sick is the ride now with the front SR trucks? I have been contemplating on SRs for a while now.
```

---
## \#34 Posted by: Skunk Posted at: 2018-10-01T20:02:22.217Z Reads: 33

```
Love my SR trucks. So much that i bought both the rkp and tkp after riding them.
They have a good fall sale atm too.
```

---
## \#35 Posted by: mixedcreation Posted at: 2018-10-01T20:09:59.740Z Reads: 33

```
Shit, off I got to the site.  Dammit Skunk.
```

---
## \#36 Posted by: Skunk Posted at: 2018-10-01T20:23:29.575Z Reads: 33

```
[quote="mixedcreation, post:35, topic:69708, full:true"]
Shit, off I got to the site. Dammit Skunk.
[/quote]

Think I've talked 6 people into buying them the past two months lol.
```

---
