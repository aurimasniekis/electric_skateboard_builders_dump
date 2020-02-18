# Viable cheap charger?

### Replies: 28 Views: 1174

## \#1 Posted by: DragonSwagin Posted at: 2018-03-11T19:23:50.534Z Reads: 163

```
I wanted an outside opinion of a charger I found on amazon. Assuming I don't mind the slow 1.5A charge time (since I charge my board overnight anyways), what do y'all think of this charger?

https://www.amazon.com/50-4V1-5A-charger-lithium-li-ion-battery/dp/B076KJD4J5/ref=sr_1_1?ie=UTF8&qid=1520796117&sr=8-1&keywords=50.4v+charger
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-03-11T20:16:11.061Z Reads: 151

```
Seems legit.
```

---
## \#3 Posted by: Okami Posted at: 2018-03-11T20:31:15.431Z Reads: 145

```
I would get higher powered one non the less.. it does pay off if you are outside and want to charge up quickly.. Also these metal ones do seem a lot nicer, and a bonus feature would be if they are adjustable.. Otherwise I think these somewhat cheapo 'chargers' / power supplies rely a lot on bms.. If bms fails in some way it might not be that good for batteries..

Though welcome to hear opinions from others as I dont really have first hand experience with these.. I have just collected info and im still using balance charger for my builds.. so cant tell much about 12s 'bulk' charging
```

---
## \#4 Posted by: Namasaki Posted at: 2018-03-11T20:51:42.717Z Reads: 126

```
1.5 amp will be very slow charging if your battery has high capacity as most Li-ion packs do.
Besides that, this type of charger usually doesn't have a cooling fan or any other adequate cooling and therefore get pretty warm while charging and in time, heat will break down electronics.

I used a similar 2a charger early on and noticed the charger getting hot during the charge cycle.
```

---
## \#5 Posted by: L3chef Posted at: 2018-03-11T20:56:24.393Z Reads: 121

```
[quote="Namasaki, post:4, topic:48801"]
I used a similar 2a charger early on and noticed the charger getting hot during the charge cycle.
[/quote]

yep, same here. My advice would be not to cheap out on the charger since you are charging when you sleep.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-03-11T20:59:09.315Z Reads: 110

```
These are much better and still very affordable 
http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#7 Posted by: mmaner Posted at: 2018-03-11T21:01:35.017Z Reads: 105

```
Since no one else is going to say anything, leaving your batteries unattended to charge overnight is not a very good idea. One shorted cell that heats up while charging could be a very very bad night.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-03-11T21:05:20.230Z Reads: 101

```
@mmaner 
You are so right.  Lithium batteries should never be left unattended while charging.
```

---
## \#9 Posted by: DragonSwagin Posted at: 2018-03-11T21:12:56.047Z Reads: 99

```
I suppose I should rephrase my statement of letting my board charge over night. I plug it in when I get home and it usually takes less than an hour to charge (I'm lucky if I use more than 50% of my board capacity). No way I'd be able to sleep with the little fan whining on my current charger. I don't unplug it until the morning though which I definitely shouldn't be doing.

As for the charger I posted, I was playing with the idea of a budget build and was wondering about the longevity of this charger. I don't think I'll ever be in a situation where I need to charge my board super quick, so I thought it'd be a nice idea. I understand these chargers normally heat up quite a bit, but probably not more than my laptop charger I've been using for years.

For $25 in my case, I'll probably give it a shot.
```

---
## \#10 Posted by: ZackoryCramer Posted at: 2018-03-11T21:44:31.628Z Reads: 92

```
Make sure you charge outside so your bed doesn't catch on fire. :fire: 
I don't really trust overnight charging.
```

---
## \#11 Posted by: Jcullinan09 Posted at: 2018-03-11T21:53:42.598Z Reads: 91

```
Ok guys, I agree, one should not charge their boards overnight or any li-ion for that matter. But let's be real here how many of you guys charge your phones overnight?
```

---
## \#12 Posted by: ZackoryCramer Posted at: 2018-03-11T21:56:09.086Z Reads: 91

```
[quote="Jcullinan09, post:11, topic:48801"]
charge your phones overnight?
[/quote]

With only 18wh~ of energy and a long legacy of reliability, it's logical to do so. 
But a 12 stacked 500wh/3kw pack? :-1:t2:
```

---
## \#13 Posted by: Jcullinan09 Posted at: 2018-03-11T22:00:07.676Z Reads: 89

```
Hey I do not charge my board overnight either. I don't think its a wise choice, but hear me out don't you see the hypocrisy in seeing its ok to charge one thing over another overnight. Even if one is Lipo and one is Li-ion.
```

---
## \#14 Posted by: ZackoryCramer Posted at: 2018-03-11T22:03:24.440Z Reads: 83

```
It is hypocritical in a narrow sense yes. How did you know he using lipo?
```

---
## \#15 Posted by: DragonSwagin Posted at: 2018-03-11T22:32:57.423Z Reads: 83

```
I’m using Lithium Ion
```

---
## \#16 Posted by: Jcullinan09 Posted at: 2018-03-11T22:57:20.213Z Reads: 82

```
@ZackoryCramer I never said he was using Lipo, I meant to say that cell phones use lipo's, cause I have yet to see a phone using a li-ion battery. I don't really get how its hypocritical only in a narrow sense, but I guess thats just me.
```

---
## \#17 Posted by: Hummie Posted at: 2018-03-11T23:06:47.330Z Reads: 80

```
[quote="Jcullinan09, post:11, topic:48801, full:true"]
Ok guys, I agree, one should not charge their boards overnight or any li-ion for that matter. But let’s be real here how many of you guys charge your phones overnight?
[/quote]
A phone charger is the same but the phone itself has safety features such as cutting the charge when it hits full.  What you’d be doing, since the current wouldn't cut off such as when you use your phose is I think termed “float” charging, where in your case of 12s at 50.4v it will be floating at full charge and incur a lot of deterioration of the cells: it will always be on and not shut off at full like the phone. This is ok to do but not at such a high voltage.  If I charge to 50.4 as soon as I hit that voltage and pull the cells from the charge they will sink down by maybe .1v. So that’s the difference really and having cells sit at 4.2 continually, either cause they were overcharged and drop down to that or they are floating on a power supply it’s the same results and the cells don’t last nearly as many cycles and also the dreaded “dendrite” growth with plating happens up there and that can cause spontaneous shorting of the cell. Rare but happens. 
U should get another power supply. A decent adjustable voltage up to 60v with an 8 amp current and lcd screen can be had for 60$. Then you can set it to a lower voltage if it will be floating and let it sit floating without damage to cells or risk, and you won’t wait all day, and u can see what voltage ur at so not blind.
Unless ur really in need of that extra bit of energy just getting one of those cheap low current supplies that will charge to 48v and no worries and cells last way longer ...n maybe 20% less energy stored

but then again that thing I just assume doesn't have a charge cut off but maybe it does since it says lithium charger...
after taking the two seconds to look at that one it says cc/cv so it reduces current when the battery is first put to it!  a safety feature which seems never appropriate with our use.  it doesn't say anything about a cutoff at full charge though.  so in my mind this charger is ridiculous especially because it charges to full charge at 50.4 and doesn't have the cutoff feature, which is considered pretty standard on a lithium charger, but it does reduce the current when it's already putting out just a trickle.  so you get a consistent 1.5 or whatever trickle as apposed to the pcu power supply which gives most current when an empty battery on it, so without the cc (constant current) junk.  don't waste your money or time.
```

---
## \#18 Posted by: ZackoryCramer Posted at: 2018-03-12T04:22:15.613Z Reads: 62

```
[quote="Hummie, post:17, topic:48801"]
A decent adjustable voltage up to 60v with an 8 amp current
[/quote]

Spot on. :ok_hand:t2: I am using a 400watt PC power supply with a 600watt boost converter. Got a fuel display and charging at 6 amps like a boss. :sunglasses:

Still don't trust unmonitored current flow. :smile:
```

---
## \#19 Posted by: b264 Posted at: 2018-03-12T04:24:44.590Z Reads: 63

```
If a battery can't be left on the charger overnight, it's defective.
```

---
## \#20 Posted by: Hummie Posted at: 2018-03-12T04:31:14.475Z Reads: 63

```
[quote="ZackoryCramer, post:18, topic:48801"]
Still don’t trust unmonitored current flow. :smile:
[/quote]

yea I really like to see that number and have a wattmeter wired up to the pcu also to see.
the pcu I have with an lcd screen showing the voltage, you set it to show the voltage you want the pack to get to and then when the pack is connected it shows the pack voltage and then you watch it climb back to where the voltage was set to.
```

---
## \#21 Posted by: ZackoryCramer Posted at: 2018-03-12T04:34:50.541Z Reads: 58

```
You can't really trust the charger or the battery being not defective either. :man_shrugging:t2:
```

---
## \#22 Posted by: DrJeff Posted at: 2018-03-12T04:49:03.435Z Reads: 64

```
[quote="ZackoryCramer, post:18, topic:48801"]
600watt boost converter. Got a fuel display
[/quote]

Can you explain what 600watt boost you use, and what are you using for the display? 
Something like this?
[Display?](https://www.amazon.com/bayite-6-5-100V-Display-Multimeter-Voltmeter/dp/B013PKYILS/ref=sr_1_6?ie=UTF8&qid=1520829867&sr=8-6&keywords=current+meter&dpID=41I6QB6-RxL&preST=_SY300_QL70_&dpSrc=srch)

Or just something like this?

[600 Watt Boost? and Display](https://www.amazon.com/Yeeco-Numerical-Converter-Transformer-Dissipation/dp/B06ZXYL8PK/ref=sr_1_1?s=automotive&ie=UTF8&qid=1520829981&sr=1-1&keywords=600+watt+boost&dpID=51Zjyr5qkRL&preST=_SX300_QL70_&dpSrc=srch)
```

---
## \#23 Posted by: ZackoryCramer Posted at: 2018-03-12T04:51:54.561Z Reads: 65

```
Yes I used something like that. :grinning:
```

---
## \#24 Posted by: b264 Posted at: 2018-03-12T05:11:27.939Z Reads: 63

```
[quote="ZackoryCramer, post:21, topic:48801, full:true"]
You can’t really trust the charger or the battery being not defective either.
[/quote]

Well it has to be able to do that, or it's a "toy" and not a "tool".  *If it can't do that, it's defective.*  Just like a cellphone that must be attended while charging or can't charge while you sleep.

It's not complicated.
```

---
## \#25 Posted by: Grolletje Posted at: 2018-03-13T13:49:48.546Z Reads: 49

```
hey, could you maybe post a picture of your charge setup?
thx
```

---
## \#26 Posted by: ihatetopush Posted at: 2018-03-23T06:43:05.339Z Reads: 44

```
love this 

    900W-Digital-Control-LED-DC-DC-Boost-Module-Power-Supply-Step-up-Converter

https://www.amazon.ca/Converter-10-120V-Step-up-Regulator-Digital-controlled/dp/B0725CKZHV

https://www.youtube.com/watch?v=4HAQhN6_cnM
```

---
## \#27 Posted by: ZackoryCramer Posted at: 2018-03-23T06:48:59.747Z Reads: 44

```
While I am at it,

![image|375x500](upload://zvvryhcUaa7Qwcjc6E1oNzPcdoJ.jpg)
```

---
## \#28 Posted by: banjaxxed Posted at: 2018-03-23T16:32:15.478Z Reads: 40

```
![IMG_8668|320x240](upload://hugurfxFCiRn6oBU8q69efQcV2f.GIF)
```

---
