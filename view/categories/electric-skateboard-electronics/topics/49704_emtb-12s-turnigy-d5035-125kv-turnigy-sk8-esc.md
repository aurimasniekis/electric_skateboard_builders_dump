# eMTB, 12s, Turnigy D5035-125KV, Turnigy SK8-ESC

### Replies: 47 Views: 3215

## \#1 Posted by: janpom Posted at: 2018-03-21T08:35:01.169Z Reads: 268

```
Could anyone please sanity check this setup? I'd like to convert my MBS Core 94 mountain board. These are the components I'm considering (single drive):

- Turnigy D5035-125KV (https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html)
- Turnigy SK8-ESC (https://hobbyking.com/en_us/turnigy-sk8-esc-for-electric-skateboard-conversion.html)
- 4x Multistar High Capacity 6600mAh 6S 10C (https://hobbyking.com/en_us/multistar-high-capacity-6s-6600mah-multi-rotor-lipo-pack.html)

The batteries would be wired both in series and parallel giving 12S2P, 13200mAh. I should get 132A constant discharge from that, which is more than enough for the motor and should be sufficient even if a second motor is added later (the Turnigy D5035-125KV takes 45A).

I should also get 586 Wh, which, as I understand, should provide ~25-30 km range on a MTB.

For the mount, I'm considering one for MBS from Idea that has 4.8:1 gear ratio. On MTB with 8 inch wheels that should give me 37 km/h of max speed (http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":125,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":72,"wheel-size":200}|).

Does this all sound correct?

This is my first build. I want to start with something on a low budget and upgrade later. Might add another drive and/or get a better ESC. Even though this is a MTB, I'm mostly going to take it on road. More about that here: http://www.electric-skateboard.builders/t/mtb-with-easy-to-add-remove-motor/49317/14

I'll greatly appreciate any suggestions. I realize this may be too much on a low budget.
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-03-21T09:11:39.155Z Reads: 244

```
The Tunigy VESC doesn't look too promising. It's just too cheap for a VESC and i think i never heard of someone using it for a long time without any errors. You should at least get a regular 4.12 ESC, or even better a Focbox or similar design. Think about it this way - if this VESC fails after a while you lost 70 Bucks and have to buy another, better vesc for above 100 bucks anyways. You should just go for the better VESC in the first place.

The motor should be fine if you don't have to climb any steep hills on you way, same goes for the batteries. 

Maybe consider waiting a bit and saving up to get components that are already approved in the esk8 community. Like FocBox, SK3 Motors and Zippy Lipos.
```

---
## \#3 Posted by: janpom Posted at: 2018-03-21T09:50:19.001Z Reads: 225

```
Thanks. This is helpful. I don't really need to save up. I just prefer not to spend too much on my first build. I want to make sure I will actually use and enjoy the eMTB before I pour a lot of money into it. On the other hand, I don't want to buy shit either (even if it's cheap).

I'll take your advice regarding the ESC/VESC and avoid the Turnigy SK8-ESC.

I chose the motor because it's sensored, which seems like a good feature. The Turnigy SK3 motors are about the same price, but with no sensors. They have more power, but 2 kW of the one I chose seems like plenty and it has very high KV so torque should be good. It may not be super fast, but I don't mind that. I prefer not to kill myself anyway. :)

Regarding the battery, what problems can I expect from buying these cheap ones? The Zippy are not that much more expensive and in fact, I could live with a little bit less of a range, so maybe I could get Zippys with less mAh for about the same price.
```

---
## \#4 Posted by: Tuomalar Posted at: 2018-03-21T09:59:15.981Z Reads: 191

```
I recommend you to read another eMTB build threads. A motor is very small and that vesc will probably die on the first hill in MTB use. I recommend using car esc and 6s system if you want a budget build. But first, read a lot. However eMTB and budget really don't belong in the same sentence.
```

---
## \#5 Posted by: janpom Posted at: 2018-03-21T10:03:38.259Z Reads: 188

```
I have actually read quite a lot already. The problem is my use case is quite a bit different from everybody else's. People usually don't build a MTB to take it on the road. I guess my config should actually be closer to what people use on skateboards.
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2018-03-21T10:19:17.497Z Reads: 189

```
The Motor isnt as small as you think, it's just the stator size in the measurement instead of the rotor size you usually see. In the link it says 6376 i think.

Alienpowersystem sells the cheapest sensored 6374 motors that i know of, you might want to check those out. For on road use and not so many steep hills FOC would be enough, no sensors necessary. But it still feels nice on start up of course.

[quote="janpom, post:3, topic:49704"]
very high KV so torque should be good
[/quote]
Low kv is related to more torque at the same amps compared to high kv. High kv motors can handle more amps but also need more amps for the same torque. Just to clarify. 


The Problem with multistar batteries is that they are more of a 3C in the real world. Read that somewhere on endless sphere a while ago. They are only good for really low current applications so i would advise against them generally. Zippys are the mainstream Lipos from hobbyking and sufficient for most esk8 applications with regular motors, graphene would be high end for either really big low c packs or small high c packs.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-03-21T10:27:16.902Z Reads: 157

```
Is the turnigy esc not sold out in the US?
```

---
## \#8 Posted by: Tuomalar Posted at: 2018-03-21T10:58:51.624Z Reads: 164

```
[quote="Der6FingerJo, post:6, topic:49704"]
In the link it says 6376 i think.
[/quote]

From Hobbyking motor specs:
Can Diameter C (mm) 62.50
Can Length D(mm) 54.80

It's fine for a flat environment, but like Der6Finger said you should check out APS motors. Those are very popular and affordable. I would use 170kv 12s or 260kv 6s system. The last one is cheaper option.
```

---
## \#9 Posted by: janpom Posted at: 2018-03-21T11:32:54.844Z Reads: 153

```
Yes, it's currently sold out. It might still be available later, no? Anyway, looks like people here don't recommend it.
```

---
## \#10 Posted by: pat.speed Posted at: 2018-03-21T11:37:05.670Z Reads: 148

```
I’ve been waiting for it to come back for a little while, I contacted them and they didn’t know anything about new stock so it seems it may not
```

---
## \#11 Posted by: Grozniy Posted at: 2018-03-21T13:32:47.130Z Reads: 141

```
Multistar batteries are not known for good performance. So expect some voltage sag. Consider buying 30c+ batteries ;)
```

---
## \#12 Posted by: rich Posted at: 2018-03-21T14:08:44.841Z Reads: 144

```
[quote="janpom, post:1, topic:49704"]
I want to start with something on a low budget and upgrade later.
[/quote]

This is exactly me 2 years ago :laughing:
I think we have a similar story, i also started with landkiting and then wanted to convert my board to an e-mtb on a low budget. I've paid a lot for parts for selfmade motor mounts and chain drive but in the end it didn't work and I lost a lot of time and money. I bought different vescs until I realized I need a proper one and run in FOC. I bought different motors and drivetrains, I spent so much money that I'm afraid to tell how much it was :rofl:, all started with a budget build......

Long story, what I mean is don't try to cheap out because you WILL upgrade and loose all the money from the "cheap" parts which is very expensive. If you don't cruise in wet dirt or very high grass a belt drive is fine, the mounts from @idea are nice. Also like @Der6FingerJo and @Grozniy mentioned, don't buy these Multistar Batteries, go for Zippy's or Graphene, they are much better.

My advice: buy 2x 6374 motors (Alien are fine or the sealed maytech which I use now but they are double in price) and when you are based in US get 2x B-boxes, you will never ever have to upgrade and start with a proper reliable running system, I would call this the REAL low budget build because that's it, no upgrade needed.

BTW since I have my e-mtb I enjoy it so much that I didn't kite for almost 2 years, the wind is in my thumb and controls if it's gusty or just a little breeze :rofl:, it's amazing.
```

---
## \#13 Posted by: janpom Posted at: 2018-03-21T21:01:44.637Z Reads: 121

```
@pat.speed HobbyKing just responded to my question and said "It could be out 4-6 weeks". Just FYI. I'm no longer considering it as an option.
```

---
## \#14 Posted by: janpom Posted at: 2018-03-21T21:41:21.255Z Reads: 125

```
Thanks everyone for responses. You guys are super helpful.

@rich Love your wind control analogy. :smile: Does that also work for sending the kite and jumping? :)

What you say makes sense to me. I'm rethinking this upgrade idea. I guess I'll go with good quality parts, but I'll stick with a single drive to keep the costs reasonable. Adding a second motor is then a straightforward upgrade and it's adding rather than replacing.

Plus, 2x 6374 really seems like an overkill for on-road use. These motors are around 3 kW each so that's 6 kW for a dual drive. In my student times (long long ago), I used to have an electric scooter with 1 kW motor. It ran on 32V lead acid batteries and it was heavy as hell -- like 40 kg. I could still make over 30 km/h on flat road and it even climbed steep hills (not particularly fast, but it would get there, eventually). 3 kW ought to be enough for anybody. ;)

Plus, my wife will kill me if I spend 1000 EUR+ on a mountain board. I'm still under suspended sentence after "investing" into my kiting gear.

BTW, I'm in Europe, so I guess it's ESCape for me if @stewii can get enough so that there's one for me.
```

---
## \#15 Posted by: rich Posted at: 2018-03-22T09:46:11.981Z Reads: 114

```
[quote="janpom, post:14, topic:49704"]
@rich Love your wind control analogy. :smile: Does that also work for sending the kite and jumping? :slight_smile:
[/quote]


Well.... this knob is missing on the remote, have to talk to the manufacture :laughing:

If you buy 1x ESCape and 1x 6374 that would be perfect, you can always upgrade with the same parts without loosing money. Just one thing to consider. I would buy a motor mount where you don't need a crossbar otherwise you would have to mount both motor mounts including crossbar even when you only use 1 Motor. The new aluminium mounts from Idea can be mounted as single mount, too :grin:. 

And next year if you want more power you can invest another 250€ (ESCape & 6374) and have a full powered MTB (and probably less struggle with your wife :wink:)
```

---
## \#16 Posted by: janpom Posted at: 2018-03-22T14:10:29.622Z Reads: 106

```
Use high wind (aka full throttle) and a ramp? You may be missing a soft landing feature then though. :slight_smile:

So, I'm taking everyone's advice on the battery and considering 4x 8000mAh 3S1P 30C (https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack-xt90.html) to connect in series. Now, I would greatly appreciate some advice on wiring and charging. I'd rather avoid using BMS for the battery pack. It seems complicated. I'm thinking of putting XT150 connectors on all batteries. That makes connecting in series very easy and I would be able to take it all apart for charging. Then use this guy (https://hobbyking.com/en_us/imax-b6-dc-charger-5a-50w-copy.html) together with 2x 3S to 6S BMS adapter (https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html) for charing. I would only be able to charge two batteries at the time, but I don't mind. Making charging less of a hassle is a part of my upgrade plan.

For connecting the battery pack to the ESC, I would use anti-spark XT150 connectors (https://hobbyking.com/en_us/7mm-as150-anti-spark-self-insulating-gold-bullet-connector-2-pairs.html). Each of the two terminal batteries would get one so that I don't need any adapter.

Does this sound like a good plan?
```

---
## \#17 Posted by: Der6FingerJo Posted at: 2018-03-22T14:36:03.317Z Reads: 104

```
Looks good, but the charger only does 50W. Your pack is 355 Wh, so more than 7 Hours to charge it from zero to 100 with balancing. If you can life with 6 hours of a small fan going berserk in the corner of the room it's fine, but i would recommend a ISDT Charger and a used server power supply for charging.

It's kind of the same thing in terms of being "cheap" but not as severe as with the ESC. Your charging setup would be 20€ for the charger and somewhere between 10-20€ for the power supply.
An ISDT Q6 would be around 50 bucks with a <20€ power supply. Or just get 2 Imax Chargers for the beginning and a 100W PSU.
```

---
## \#18 Posted by: rich Posted at: 2018-03-22T14:43:40.299Z Reads: 105

```
[quote="janpom, post:16, topic:49704"]
Use high wind (aka full throttle) and a ramp? You may be missing a soft landing feature then though. :slight_smile:
[/quote]

@DanSkates is the expert for ramps, maybe he is thinking about a small kite for a softer landing when he builds a mega ramp :laughing:

[quote="janpom, post:16, topic:49704"]
So, I’m taking everyone’s advice on the battery and considering 4x 8000mAh 3S1P 30C
[/quote]

Or 3x 4s Zippy's or 2x 6s Turnigy Graphenes 8Ah :grin:
About charging, this will be slow and annoying. I'm a fan of BMS and could help you with the wiring, it's not really complicated
You could get a 12s BMS for 25€ plus a charger between 12-25€ (2-4A) on aliexpress and you can charge the whole battery at once without taking it apart plus it is much faster. Can provide the links if needed.

XT150 is kind of overkill but why not.
You could use XT90, 4mm bullets or 5.5mm bullets.

I also have a 6s HK 6A balance charger which needs about 10 hours for 12s8Ah (5 hours for each 6s). With BMS and 12s charger it takes 2 hours :sunglasses:
```

---
## \#19 Posted by: rich Posted at: 2018-03-22T14:45:01.108Z Reads: 98

```
Don't listen to @Der6FingerJo, he doesn't like BMS :joy::rofl::laughing:
```

---
## \#20 Posted by: Der6FingerJo Posted at: 2018-03-22T15:06:57.771Z Reads: 98

```
Don't listen to @rich, he hates clean and simple charging solutions :joy:

But truth be told, a BMS is still a valid way to go. Didn't think of it because i don't really trust them with Lipos. I have no bad experiences or anything, just nut my way of doing it. Especially since i already had a nice 500W ISDT Charger before building my first board.

If you want to dig into this i'm sure you could find a cheaper solution than an ISDT charger.
```

---
## \#21 Posted by: janpom Posted at: 2018-03-22T15:56:20.627Z Reads: 93

```
[quote="rich, post:18, topic:49704"]
You could get a 12s BMS for 25€ plus a charger between 12-25€ (2-4A) on aliexpress and you can charge the whole battery at once without taking it apart plus it is much faster. Can provide the links if needed.
[/quote]

I'd really like the links. Thanks! This is all very new to me. I barely understood the difference between volts and amps before starting my research. :smile: 

One thing I'm a little concerned about wrt charging a battery pack with BMS is that (as I understand) this typically involves using a cheap and dumb charger that doesn't have any display indicating current state of charging and doesn't switch itself off once the batteries are fully charged. I imagine clever ones are available as well but probably nowhere near the price range of the IMAX.
```

---
## \#22 Posted by: Der6FingerJo Posted at: 2018-03-22T16:11:36.559Z Reads: 95

```
[quote="janpom, post:21, topic:49704"]
One thing I’m a little concerned about wrt charging a battery pack with BMS is that (as I understand) this typically involves using a cheap and dumb charger that doesn’t have any display indicating current state of charging and doesn’t switch itself off once the batteries are fully charged. I imagine clever ones are available as well but probably nowhere near the price range of the IMAX.
[/quote]

Oh hey you get what i mean! :smile:
Imagine charging with a BMS like charging your phone or laptop, it's just plugging in and letting the BMS handle the rest. With a dedicated charger you can at least see the voltages of the individual cells once every cycle. If a cell goes bad and you are using a BMS there's no way to tell except physical changes to the cell, like it puffing up or so.
```

---
## \#23 Posted by: rich Posted at: 2018-03-22T17:03:10.988Z Reads: 98

```
[quote="janpom, post:21, topic:49704"]
I’d really like the links. Thanks! This is all very new to me. I barely understood the difference between volts and amps before starting my research. :smile:
[/quote]

2 years ago I didn't know anything but after 3 builds and a lot of research I would call it "advanced knowledge" :grin: 

[quote="janpom, post:21, topic:49704"]
One thing I’m a little concerned about wrt charging a battery pack with BMS is that (as I understand) this typically involves using a cheap and dumb charger that doesn’t have any display indicating current state of charging and doesn’t switch itself off once the batteries are fully charged.
[/quote]

What you describe is a power supply.
I'm talking about an Li-ion charger, it has all safety features including overcharge protection for the whole pack. The overcharge protection for each single cell is managed by the BMS. There is double safety.

You could use [this 12s BMS](https://www.aliexpress.com/item/12S-60A-50-4V-li-ion-BMS-PCM-battery-protection-board-bms-pcm-for-electric-bike/32847948009.html?spm=2114.search0104.3.42.74146af36iq0Nt&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10344_10068_10547_10342_10343_10340_10548_10341_10696_10084_10083_10618_10304_10307_10302_5711215_10313_10059_10534_100031_10103_10624_10623_443_10622_10621_10620,searchweb201603_37,ppcSwitch_5&algo_expid=a7bcf286-4cdc-460b-924f-4faeb0c99a8d-6&algo_pvid=a7bcf286-4cdc-460b-924f-4faeb0c99a8d&transAbTest=ae803_4&priceBeautifyAB=0) for discharge, too so all cells are protected during usage as well (except over discharge).

As charger you could use any 50.4V Li-ion charger. There are the cheap "bricks" which get got during charging (like [this 1.5A](https://www.aliexpress.com/item/100-240V-DC50-4V-1-6A-polymer-lithium-battery-charger-DC-5-5MM-2-1MM-Portable/32777216768.html?spm=2114.search0104.3.1.3d852d9aNLEHUT&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10344_10068_10547_10342_10343_10340_10548_10341_10696_10084_10083_10618_10304_10307_10302_5711220_10313_10059_10534_100031_10103_10624_10623_443_10622_10621_10620,searchweb201603_37,ppcSwitch_5&algo_expid=9cbc60ea-a1dd-470f-92fa-4ffe1c997678-0&algo_pvid=9cbc60ea-a1dd-470f-92fa-4ffe1c997678&transAbTest=ae803_4&priceBeautifyAB=0), couldn't find a 2-3A brick now). What I use right now is this [4A charger](https://www.aliexpress.com/item/Yangtze-50-4V-4A-3A-Lithium-Li-ion-Battery-Charger-For-44-4V-Lipo-Bike-Power/32836644573.html?spm=2114.search0104.3.62.3d852d9aNLEHUT&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10344_10068_10547_10342_10343_10340_10548_10341_10696_10084_10083_10618_10304_10307_10302_5711220_10313_10059_10534_100031_10103_10624_10623_443_10622_10621_10620,searchweb201603_37,ppcSwitch_5&algo_expid=9cbc60ea-a1dd-470f-92fa-4ffe1c997678-9&algo_pvid=9cbc60ea-a1dd-470f-92fa-4ffe1c997678&transAbTest=ae803_4&priceBeautifyAB=0) which takes 2 hours to charge a 12s 8Ah lipo. It is plastic but small and has a fan so nothing gets hot. I personally don't like these huge aluminium chargers.

The big sale on aliexpress starts in 6 days and you could get this 4A charger for 19€ with free shipping. I think I'll buy this one in 6A again. But I have to mention that my charger came broke and I had to change the main power wire.

The last thing would be a waterproof charging port then you are ready to charge, no struggling....

I have a voltmeter attached to the BMS so I can see the voltage of the battery also during charging :sunglasses:

[quote="Der6FingerJo, post:22, topic:49704"]
Imagine charging with a BMS like charging your phone or laptop, it’s just plugging in and letting the BMS handle the rest.
[/quote]


Exactly, imagine you would have to open your phone or laptop everytime and take the batteries out for charging :joy: For me this is not an option......
```

---
## \#24 Posted by: DanSkates Posted at: 2018-03-22T17:19:46.560Z Reads: 79

```
[quote="rich, post:18, topic:49704"]
@DanSkates is the expert for ramps, maybe he is thinking about a small kite for a softer landing when he builds a mega ramp :laughing:
[/quote]

LOL, no, no kite - actually just sold all my kite surfing gear a few months back as I’m only riding this now. Plus I have a big soft ass to land on if needed!! 😂
```

---
## \#25 Posted by: janpom Posted at: 2018-03-22T19:09:15.556Z Reads: 79

```
Thanks again guys for all the info and the links. So I guess I can either go with the BMS and the 4A charger for about $55 in total (if everything is actually delivered and functional; I don't have particularly good experience with these Chinese online stores). Or I could get two IMAXes and a power supply (maybe [this one](https://hobbyking.com/en_us/hobbyking-350w-25a-power-supply-100v-120v.html)) for about 60 EUR. Not a big difference in price. I'm slightly inclined towards the without BMS solution for the reasons @Der6FingerJo mentioned -- you have more control: display on the charger that tells you if something is wrong. With BMS, the BMS will try its best to make sure there won't be a problem but if it is you'll get no feedback. Plus, taking apart 4 batteries for charging isn't that hard. Having 12x 1s would be a different story.

With BMS, on the other hand, the charging would be more convenient (no need to take the battery pack apart) and also about 2 times faster (hm, that's actually significant). I also wouldn't need that many connectors. I could just solder it all together (if I learn how to do it and get myself something to do it with :slight_smile:  ... which seems inevitable anyway).

That's like Sophie's choice, guys!
```

---
## \#26 Posted by: Der6FingerJo Posted at: 2018-03-22T19:33:03.137Z Reads: 71

```
For 60€ you can get an ISDT 300W Charger and some additional 15 bucks will get you a 500W PSU from eBay. Charging in a little above one hour is nice :D
```

---
## \#27 Posted by: Acido Posted at: 2018-03-22T20:13:38.317Z Reads: 75

```
vesc 4.12 costs about 60$ in materials, if you order a lot like hk does its even cheaper and sell large quantities of them its profitable for them
```

---
## \#28 Posted by: Acido Posted at: 2018-03-22T20:15:04.926Z Reads: 78

```
This afternoon I went kite skating on my trampa on a beach, wind was blowing like 60kmh, it was so fun :D
It pulled me like 10 times in the air,  10m2 kite is overkill!
```

---
## \#29 Posted by: Grozniy Posted at: 2018-03-22T22:16:19.486Z Reads: 78

```
How many amps did it pull? Ahahah
```

---
## \#30 Posted by: DanSkates Posted at: 2018-03-22T22:31:49.443Z Reads: 82

```
Goddamm that sounds fun! I have to say though based on some of the ‘lift and dumps’ I had in the water riding a board on land is terrifying 😂
```

---
## \#31 Posted by: janpom Posted at: 2018-03-22T23:52:36.675Z Reads: 84

```
At last I decided to go without the BMS solution. Seems cleaner and more modular. With the XT150 connectors I can easily wire up the batteries any way I want (not that I have a particular use case for that, but I like the flexibility :slight_smile:).

Going with two cheap IMAX B6 chargers (yeah, not even the genuine ones :slight_smile:). There's a youtube video from a guy who has both the genuine and the copy and says he doesn't see any difference. With two, I can charge the battery pack in about 3.5 hours, which is not too bad. Plus, slow charging is good for the batteries anyway, isn't it?

Here's my HobbyKing shopping list. I believe I have everything except for ESC (waiting for ESCape) and power supplies (will probably buy some used ones locally). Is there something else you would recommend throwing in? Thanks!

![image|590x500](upload://p2PLt7CkDqH2pe7A814MvKpsTCG.png)
```

---
## \#32 Posted by: telnoi Posted at: 2018-03-23T05:04:23.379Z Reads: 77

```
Must say that one is just awesome with a 24v power supply.

4x 8000 mah balance charged under 2 hours.
May already be too late, but would get 4x 6s due to te range. 8000 mah is around 8 km off-road with hills. If that's enough, go for it. If you lack the cash, I'd still go for 2x 6s 8000mah...otherwise you'll end up with a shitload of lipos on your deck when you do decide to increase range.
```

---
## \#33 Posted by: Acido Posted at: 2018-03-23T05:50:33.106Z Reads: 76

```
First time it is but when you fall on sand it doesnt hurt that muc, adrenaline overrides pain haha
It took me maybe 80cm max in the air nothing special
This was the first time I driven my trampa :D
```

---
## \#34 Posted by: Der6FingerJo Posted at: 2018-03-23T06:56:39.612Z Reads: 78

```
Have to agree with that, fewer LiPos are better imo. Just look if you can get 2x 6S instead of 4x 3S for a similar price.
```

---
## \#35 Posted by: janpom Posted at: 2018-03-23T07:08:07.111Z Reads: 79

```
[quote="telnoi, post:32, topic:49704"]
8000 mah is around 8 km off-road with hills.
[/quote]

@telnoi You mean 8000 mah 6s, right? Not 12s? From what [I have read](http://www.electric-skateboard.builders/t/whats-your-range-list-the-following-battery-size-wh-xsyp-lipo-li-ion-brand-drivetrain-hubs-belt-single-duo-quad-kv-ratio-vesc-y-n-regen-braking-y-n-average-payload-user-gear-bags-etc-range-miles-or-km-wh-km-or-wh-mile/14832), people are getting about 10 Wh/km on road with a skateboard and 20 Wh/km off road with a MTB. I'll mostly do MTB on road so I suppose to end up somewhere inbetween (15 Wh/km?).

8000 mah 12s LIPO is 352 Wh, so that should be good for about 17 km off-road. 17 km is exactly the range I need, but since I'm going to mostly do on road I hope to get more than that and have some padding.

I'm ordering everything from HobbyKing and the only reasonable option for 8000 mah 6s there is [Turnigy Graphene Professional 8000mAh 6S 15C LiPo Pack w/XT90](https://hobbyking.com/en_us/turnigy-graphene-professional-8000mah-6s-15c-lipo-pack-w-xt90.html) for 93.5 EUR. The [Zippy 8000 mah 3s I'm about to get](https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack-xt90.html) are 31 EUR, so that's 187 EUR for 2x 6s vs 124 EUR for 4x 3s. That's quite a bit of a difference. Also, the 6s is only 15c whereas the 3s is 30c.
```

---
## \#36 Posted by: telnoi Posted at: 2018-03-23T07:13:48.282Z Reads: 73

```
Depends on where and how you ride I guess. In my case, 8000 mah 10S is discharged to 3.7V in around 8 km. For you, that number might be different. Half of my journey is uphill, with partial mud plowing, etc.

Once you get used to MTB, you'll most likely want to go further and faster relatively soon. The prospect of having 8 lipos + all the wires is rather unpleasant. 

My current range with 16000 MAH 10S is good for around 17 km. You might get a bit more out of it using 12S.
```

---
## \#37 Posted by: janpom Posted at: 2018-03-23T07:30:09.842Z Reads: 72

```
I see. Thanks for the warning. I'll go with the 4x 3s anyway. The extra cost for 2x 6s just seems too much. I believe it will currently be OK for my use case. If I need more range, there's a number of options. I could either double up the battery and deal with 8 LIPOs (probably convert to BMS then) or change the battery pack completely (I'm hoping 3s might be easier to sell off than 6s) or maybe just get 2 extra batteries and convert to 9s (2x 3x3s).
```

---
## \#38 Posted by: telnoi Posted at: 2018-03-23T07:41:14.488Z Reads: 68

```
Price is why I went with 10S.
You get 8000 mah 10S for 106 EUR (zippy 5S 8000 mah 30C x2).
```

---
## \#39 Posted by: rich Posted at: 2018-03-23T19:33:14.151Z Reads: 70

```
[quote="telnoi, post:36, topic:49704"]
8000 mah 10S is discharged to 3.7V in around 8 km. For you, that number might be different. Half of my journey is uphill, with partial mud plowing, etc.
[/quote]

Do you already need a oxygen mask on your rides?
Jesus, this must be serious uphill action with this consumption :laughing:, no heat problems?
With the old setup I only tried once to climb a hill but the motors got sizzling hot and the vescs reached temp limits, my MTB felt like a old lame horse the whole ride.
```

---
## \#40 Posted by: telnoi Posted at: 2018-03-23T20:48:54.159Z Reads: 71

```
My voltage drops and stays down for 1v after I am done with one climb. That's with 16000. I go up there almost full throttle/about 28 km/h. In fact, some off-road sections I need to be full throttle to make it walking speed. That's with 149kv. With all that, my motors are Luke warm. My focboxes do overheat sometimes, crawling to a halt completely. 

The roads here are used by heavy machinery. Those foresters often repair the sand roads with big stones, so the board never rolls smoothly. There is always a massive loss of energy and momentum.

My hope is direct drive and the trampa will improve efficiency a bit. Different gear ratio. Also need to work on a waterproof enclosure with proper cooling.
```

---
## \#41 Posted by: janpom Posted at: 2018-03-24T17:06:49.234Z Reads: 68

```
[quote="rich, post:15, topic:49704"]
I would buy a motor mount where you don’t need a crossbar otherwise you would have to mount both motor mounts including crossbar even when you only use 1 Motor. The new aluminium mounts from Idea can be mounted as single mount, too
[/quote]

I specifically asked @idea about this and he said that single motor mount is not an option (at least for MBS; maybe it's different for Trampa). I wanted to only get the side part of the dual mount with crossbar that @idea makes, but he said that wouldn't work -- the part would bend. So I'm getting the dual motor mount and will only use it with a single motor for now.
```

---
## \#42 Posted by: Der6FingerJo Posted at: 2018-03-24T17:10:02.362Z Reads: 66

```
[quote="telnoi, post:40, topic:49704"]
That’s with 149kv. With all that, my motors are Luke warm. My focboxes do overheat sometimes, crawling to a halt completely.
[/quote]

Did that happen in the last few weeks with the current temperatures or is this also true for summer?
```

---
## \#43 Posted by: telnoi Posted at: 2018-03-24T17:18:08.575Z Reads: 59

```
Used the build since autumn.
```

---
## \#44 Posted by: rich Posted at: 2018-03-24T17:56:02.591Z Reads: 60

```
[quote="janpom, post:41, topic:49704"]
I wanted to only get the side part of the dual mount with crossbar
[/quote]

I think he sells dual mounts only, I don't know how it is with MBS but he has different mounts. The ones made of stainless steel and aluminium rings need a crossbar. The aluminium mounts can be used without crossbar except the truck has a bad angle. But he has a CNC machine so it shouldn't be a problem. BTW [this is an MBS truck with idea aluminium mounts](https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/2901?u=rich), they won't bend :wink:
```

---
## \#45 Posted by: hornet90 Posted at: 2018-04-14T09:59:32.581Z Reads: 54

```
I just got that 125kv motor to try out,I put it on a trampa 12s 6600 Vesc 6 14/66 8" super hit 43km
```

---
## \#46 Posted by: ToyoT Posted at: 2018-04-14T17:44:09.216Z Reads: 50

```
With only one motor ?
The torque is ok ?
```

---
## \#47 Posted by: hornet90 Posted at: 2018-04-15T08:39:55.113Z Reads: 47

```
It's super ![Screenshot_20180413-135301|281x500](upload://nG5MVlt9sgYCXz4w8vyA0iulzln.png)
```

---
