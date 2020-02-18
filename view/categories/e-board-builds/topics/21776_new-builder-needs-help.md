# New Builder Needs Help

### Replies: 40 Views: 3046

## \#1 Posted by: Youssless Posted at: 2017-04-25T21:07:38.911Z Reads: 155

```
Hey guys,

So I've been lurking for the last few days and I'm looking to graduate from building my first gaming PC to something that's a little less like Lego for adults. I've done some reading and looked (read admired) some builds by @makevoid (I'm from London too!) and @longhairedboy (loving your builds but I won't be able to afford your luxury I'm afraid).

Whilst I don't want to be fed a build I am looking for some clarification as the parts are a tad more varied than PC parts and there's certainly a a steeper learning curve I think. 

I tend to go on so will try and list some points/questions that I've tried searching for but either I really suck at understanding or my Googling skills are underwhelming:

My mass = 95kg, though I get as low as 75kg when cutting for a fight.

Desired use = cruising and commuting (especially since the weather is getting nicer :smile:)

Desired top speed = 25-30mph
Desired range = 10-15 miles (16-24km)

Budget = £300 - £400

I've gathered that I should go for a 190kv motor with a 10S battery (though I don't know what the 'p' means in 10s4p), get a VESC (though I still need to learn about tweaking with it on the software side of things) and I think I'd like 83mm wheels with a stiff board for the stability at higher speeds.

There are loads of guides for how to piece things together and once I have the parts I'm sure I'll be fine but I'm scratching my head about what exact parts to get.

I have loads more questions but will leave it there and try not to overstay my welcome. Apologies for not listing a build and asking for tweaks as I genuinely can't make sufficient judgements ATM.

Thank you in advance for any pointers.

Youssless
```

---
## \#2 Posted by: darkkevind Posted at: 2017-04-25T21:19:29.191Z Reads: 139

```
I'd go for the SK3 motor, you can't really go wrong with those...
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html
```

---
## \#3 Posted by: darkkevind Posted at: 2017-04-25T21:22:45.387Z Reads: 137

```
Either these: http://www.evolveskateboards.de/index.php/en/shop-buy-online/compatible-longboard-wheels/evolve-gt-wheel-83mm-76a-detail

or these wheels: http://www.evolveskateboards.de/index.php/en/shop-buy-online/compatible-longboard-wheels/abec11-flywheels-longboard-wheels-83mm-78a-green-detail
```

---
## \#4 Posted by: Youssless Posted at: 2017-04-25T21:27:39.054Z Reads: 130

```
Thanks, saw these exact ones earlier today, its good to know I'm sticking my nose in the right direction.

The wheels are more expensive than I anticipated, is this standard?
```

---
## \#5 Posted by: darkkevind Posted at: 2017-04-25T21:29:37.387Z Reads: 126

```
You could probably find cheaper elsewhere to be honest...
```

---
## \#6 Posted by: Youssless Posted at: 2017-04-25T21:31:06.993Z Reads: 124

```
like eBay? I'm not familiar with vendors.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-04-25T21:45:33.168Z Reads: 124

```
Yeah, should be fine. You can get some Abec clones I'd imagine.
```

---
## \#8 Posted by: sl33py Posted at: 2017-04-25T22:23:07.174Z Reads: 116

```
it might be a challenge on your budget.  I'd suggest Lipo vs Li-Ion for cost savings - will also have less voltage sag if you get a decent lipo (5000mAh 20c or higher would be my recommended).

Abec clones work well.  I have a set on GF's board and they aren't as soft duro as legit flywheels, but for a fraction of the price - seems plenty good enough.  I got mine on ebay and Amazon.

Look at a speed calculator.  I usually gear for a top speed of 25mph.  If you plan to ride up fairly steep hills, or want to accelerate really hard/fast - you might eventually go dual motors.  But on your budget i'd start with one and add a second motor later.  I like to gear down w/ 15/40 or 14/40 motor/wheel usually - trying to keep to reasonable speeds w/ higher voltages.

10s4p -  the "p" equals parallel.  So 10 batteries in series (10x4.2v = 42v pack), and 4 parallel = 40 cells total.  If each cell is 2500mAh (25r's for example) - 10s1p = 42v 2500mAh pack, 2p = 42v 5000mAh, etc.  4p = 42v 10000mAh.  For li-ion batteries the more important part is reducing the "workload" of the amp draw across more cells.  25r can supply 20A per cell (max - a lot of sag and reduced capacity and heat.  Heat = shorter cell life too), but if you do 4p you can supply 80A, but likely will draw more like 30-40A so less stress and sag for those batteries.  Better performance when riding hard (can supply more amps constant), and spreading the workload across 4 in parallel will help with battery life as additional benefit.  Downside of monster parallel packs - besides cost, is size and weight!  Lipo still have more energy density, weigh less, and can supply higher constant amps (less sag).

to calculate your distance - determine your Wh of your pack (V x Ah = Wh), and 10Wh = 1km (typical).  Good ballpark to see what size pack (mAh and voltage) you need for your goal of 10-15miles (you want 160-240Wh pack - easy math helps).

HTH - GL!
```

---
## \#9 Posted by: Namasaki Posted at: 2017-04-25T23:09:55.364Z Reads: 102

```
I agree with @sl33py if your on a tight budget better go with Lipo packs.
I'm not on a budget and I still go with Lipo packs because they provide the most power in the smallest and lightest package.

Since your in the U.K., you should check out Allien Power Systems.
They have everything thing you need to build an E-board and you will save money on shipping since they are in the U.K.
http://alienpowersystem.com/shop/
I really like their HEV motors. Very high quality and very reasonably priced
```

---
## \#10 Posted by: sl33py Posted at: 2017-04-25T23:21:16.763Z Reads: 95

```
A good way to compare lipo and li-ion is their C rating in amps.  So those 25r's 20A delivery capacity vs a 5000mAh 20c lipo - 20A 25r vs (5Ah x 20c) = 100A!  Admitedly this is "claimed" amp capacity of those lipos and actual will be less, but even at half the claimed amps it's still 50A vs 20A.  Then start looking at 30c and 45c packs and you can see why they provide so much punch vs li-ion!

Just to illustrate @Namasaki's point.  I too am still using lipo vs li-ion, but might build a small 3p pack for a flats and low-profile build.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-04-25T23:26:32.339Z Reads: 89

```
I should add one thing about parts sources.
Hobby King does have a warehouse in the U.K. so you can get low cost shipping from them as long as that warehouse has the parts you need.
```

---
## \#12 Posted by: Youssless Posted at: 2017-04-26T07:31:33.382Z Reads: 82

```
Thank you so much for the informative response. Both @Namasaki  and @sl33py gave some very valuable lessons and insight for me, thank you. 

I'll do some math and see if I can squeeze decent quality parts into my £400 budget (you said it was a challenge, not impossible) or I may have to up it to £500. 

I'll grab 5Ah 20c lipos, considering the HEV motor @sl33py recommended is 10S, I assume I should find 2x 5Ah, 10S batteries and connect both in parallel? that should give me 42V x 10Ah = 420Wh = ~ 42km? This sounds expensive/unrealistic as I've not seen anyone with that kind of range :sweat:. Edit: Scratch that, a bit of Googling let me know real fast why I don't see builds with 2x 5Ah 10S batteries in parallel. 

Does anyone have recommendation for budget, stiff boards?

Thanks again,

Youssless
```

---
## \#13 Posted by: Namasaki Posted at: 2017-04-26T15:43:53.643Z Reads: 74

```
A couple 5s lipos and a hobby balance charger is the cheapest and simplest way to get started. 
Try to get higher C batteries though. 
At least 25C but preferably higher. 
I use 60C lipos. 
You need lots of headroom when it comes to current to avoid excessive voltage sag.
```

---
## \#14 Posted by: sl33py Posted at: 2017-04-26T17:27:20.094Z Reads: 68

```
Agreed.  20c 5Ah/5000mAh is the *minimum* i'd suggest.  the 30c and higher will be even better.  Depending on your budget, get what you can afford - they can get significantly more expensive going higher C.

5s batteries are a bit of an oddity, so you might not see a ton of them, or they might be more $.  Option B - I regularly run 8s and it moves me along really well - two 4s.  Option C - 9s (3 x 3s).

Running a speed calc spreadsheet i found (don't recall exactly where - have a couple):

83mm - 190kv - 10s - 15/40 = ~24mph
same w/ 9s = ~22mph
same w/ 8s = ~20mph

Going any of those to 36t wheel gear = ~2mph more.  So 9s on 15/36 = ~24mph.

And wanting to go 25-30mph is *ridiculously* fast!  If you haven't done it, and don't have the skills (like you downhill and do this regularly) i strongly caution you to go slower to start and work up to faster speeds.  And wear gear appropriate for the speeds you intend to ride.  

As for inexpensive decks - since you are in the UK, i'm not sure if you'll get hit with taxes/fees/customs $, but funbox has a few decks that look nice and seem very reasonable price wise.  [Here's a link to their topmount decks only.](http://funboxskate.com/product-category/decks/longboards-decks/top-mount-longboards-decks/?products_per_page=all)
Drop through's look great but are much more difficult to setup - so for a first build i suggest a simple top mount (with micro or no drop).  I'd also caution away from flexy decks - possible, but a lot more work to setup.  Especially for a first board.

Deck shape and style is super personal - i typically prefer symmetrical boards w/ cutouts like the Loaded Vanguard - since it lets me run bigger wheels w/o risers or wheelbite.  If you do a more typical deck you likely will need risers even for 83mm wheels.

Caliber II 50's would be my suggested - the "standard" in most respects and the largest selection of motor mounts.  Being "keyed" the mount shouldn't rotate (depending on motor mount design).  I tried Paris 195's w/ ADS v1 mounts and they rotated when braking (dragging motor mount on ground) - so i'd suggest the more reliable Caliber II's or clones for this reason.  Most importantly i think is to get good bushings for your weight - regardless of which trucks you use.

as you figure out what you want - post up here so folks can help steer you before you buy.

HTH - GL!
```

---
## \#15 Posted by: Youssless Posted at: 2017-04-26T18:10:40.486Z Reads: 69

```
@sl33py and @Namasaki thank you both again for the info. I'm looking at components and I think I'll have to up my budget to £500 (though even that looks to be a bit of a challenge to work with). 

At the moment, I'm looking to go with @Namasaki's recommendation of the HEV 190kV brushless motor from alienpowersystem.com and though they have pretty much everything, they do seem to have higher asking prices for certain components. 

I'll look into getting a 5Ah, at least 30C 9s or 10s battery. Double checking; batteries in series add their voltages but batteries in parallel add their Ah, yes?. Just so I'm aware, will the extra wires for parallel prove somewhat cumbersome? there's not a whole lot of space under the board.

Think I'll invest in a VESC and batteries to maximise longevity, though how long can I expect my batteries/components to last if I use a full charge say three times a week over the summer months (say 4 to be optimistic about British weather) assuming I'll be mostly on tarmac? and if its not being used, do the components 'age' well?

Caliber II 50's caught my attention quickly though the enterion mount sitting at ~£50 has me hoping I can grab a cheaper, similar quality mount (been checking the commonly used components thread).

I'll post later with a build that will probably need some tweaking but gives an idea of what I can get to fit in my budget to help any suggestions.

Thanks again guys!
```

---
## \#16 Posted by: bigben Posted at: 2017-04-26T18:32:11.177Z Reads: 63

```
Not sure how long these are going to take to be available but they look like the biz.
https://www.electric-skateboard.builders/t/eu-us-22-carbon-motor-mounts-anodized-aluminum-clamp/20795/167
About speed, my build does perhaps 23mph and that does seem pretty fast. I'm 6'6" so perhaps that makes me feel more vulnerable.
For a controller I have a mini remote, found it great and good form factor. I just sold some for £30 quid. I have  a few more but may need them. If I don't I'll advertise them.
I started with a 6s system. Cheap and cheerful with an fvt 120 esc. Vesc with a higher voltage system is better though. Currently I use 3 x 3s 5000mah hobby king batteries that were about 30 quid each.
One thing to watch is the motors from Alien have shafts of 10mm. No problem if you go with their pulleys but a lot of other kits have 8mm holes.
```

---
## \#17 Posted by: sl33py Posted at: 2017-04-26T18:36:17.610Z Reads: 60

```
[quote="Youssless, post:15, topic:21776"]
batteries in series add their voltages but batteries in parallel add their Ah, yes?
[/quote]
Correct - Higher Voltage will give you more "Punch" and power (within your own skill limitation - and ability to "feather" or moderate the throttle).
At 10Wh = 1km.  A 10s 5000mAh setup = (42v x 5Ah =) 210Wh = 21km/13 miles.

Going parallel for more Ah would only be if you needed to double your range.  Heavy and $$ to do this.

[quote="Youssless, post:15, topic:21776"]
Caliber II 50's caught my attention quickly though the enterion mount sitting at ~£50 has me hoping I can grab a cheaper, similar quality mount (been checking the commonly used components thread).
[/quote]

A less expensive motor mount option you might look at:
https://www.electric-skateboard.builders/t/eu-us-22-carbon-motor-mounts-anodized-aluminum-clamp/20795

Remote - i'd suggest the GT2b and get a smaller enclosure later.  If you have access to a 3d printer look for Badwolf / Flatline customs / baby buffalo files on thingiverse.  OR buy MasterCho enclosure.

GL!
```

---
## \#18 Posted by: Youssless Posted at: 2017-04-26T18:41:56.169Z Reads: 52

```
Thanks @bigben, I noticed and was wondering if it would make finding pulleys difficult.

I'm listing my build on notepad with URL links and found 5Ah 3s 30c batteries for  £25 each on hobbyking. I saw that post earlier today though note that its estimated to arrive in 5 weeks which is quite a long time. Happy to wait if y'all think its worth the wait at that price.
```

---
## \#19 Posted by: sl33py Posted at: 2017-04-26T18:48:44.930Z Reads: 51

```
[quote="bigben, post:16, topic:21776"]
One thing to watch is the motors from Alien have shafts of 10mm. No problem if you go with their pulleys but a lot of other kits have 8mm holes.
[/quote]


This would be a deal breaker for me.  10mm gears are a PITA to find.  I would try to stick to motors with 8mm shafts.  I'd look at esk8.de or other EU providers and double check the axle size is 8mm.

Real world impact - the 10mm motor shaft gears are harder to find, won't go as low gearing if you are trying to keep speeds reasonable or keep torque/accell.  If you can find them, i'd not go lower than 13 or 14t for the motor gear - 12t doesn't have enough teeth in mesh and will likely skip!
```

---
## \#20 Posted by: bigben Posted at: 2017-04-26T18:49:24.169Z Reads: 50

```
Belting online can make any pulley but get expensive when you add shipping etc.
```

---
## \#21 Posted by: Youssless Posted at: 2017-04-26T18:53:04.955Z Reads: 50

```
[quote="sl33py, post:19, topic:21776"]
l.  If you can find them, i'd not go lower than 13 or 14t
[/quote]

I've found an SK3 6364 190kV motor for £10 cheaper on Hobbyking and it says it has an 8mm shaft. With the pulleys, can I stick to the beginner guide's recommendation of 15/36 or do I need a different ratio because of my weight?
```

---
## \#22 Posted by: bigben Posted at: 2017-04-26T18:53:24.143Z Reads: 52

```
Good old hobby king motors will require a flat spot making on the shaft but cheaper than  some of the other eu distributors.
I am going to try and do a group buy at some point but probably a while off yet.


What about these. You could see what he has left?
https://www.electric-skateboard.builders/t/sale-uk-vesc-motors-mounts-wheels-enclosure-gt2b-wheel-pulley-kits/21191/25
```

---
## \#23 Posted by: Youssless Posted at: 2017-04-26T19:00:49.765Z Reads: 52

```
Ah nice! a VESC for £90, do you know if it needs to be setup with lab-grade power supply (I think a guide on here called it)?
```

---
## \#24 Posted by: bigben Posted at: 2017-04-26T19:05:36.556Z Reads: 55

```
I'm no Vescpert. (see what I did there?)
But I set up my vesc on 1 of my 3s batteries. My vesc was the old enertion vesc which I'm led to believe isn't too far in quality from the diy ones. There is a chat function on the diy site, could be worth a look?
```

---
## \#25 Posted by: rwxr Posted at: 2017-04-26T19:42:12.111Z Reads: 54

```
Pulleys are available here. 15/40t 15mm for 8mm shaft

https://www.electric-skateboard.builders/t/europe-15mm-steel-motor-pulley-40t-abec-flywheel-mbs-all-terrain-pulley/21733
```

---
## \#26 Posted by: bigben Posted at: 2017-04-26T19:49:29.252Z Reads: 50

```
I've bought some of these and they're excellent. Aren't they 40 tooth wheel pulleys though?
Need large wheels for these. I'm looking for a source of 90mm+ so if anyone sees a some let me know!
```

---
## \#27 Posted by: rwxr Posted at: 2017-04-26T19:58:59.936Z Reads: 48

```
You are correct. Edited the post now. 
Been awake for 20h so I need some sleep before posting any more
```

---
## \#28 Posted by: Youssless Posted at: 2017-04-26T20:02:31.823Z Reads: 51

```
OK, so after some searching I think I have most of the pieces down and I hope I can fit it all in my £500 budget!

Please take a look and let me know if anything is incompatible/can be found cheaper elsewhere. With the board, I'll still need to look but I wanted to make sure I got the electronics secured since @rwxr will be making an order on the mounts tomorrow and I can use the 6 weeks to find a decent 2nd hand deck and some decent flywheel clones.


Motor = £55 (Sk3 6364 190kv) (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html)
Mount = $31 (~£24) from rwxr (https://www.electric-skateboard.builders/t/eu-us-22-carbon-motor-mounts-anodized-aluminum-clamp/20795)
Pulley System = £23 (12mm Enertion) (http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-drive-pulley-kit/)
Battery = £75 (3x 30C 5Ah 3s in series) (https://hobbyking.com/en_us/turnigy-5000mah-3s-30c-lipo-pack.html)
VESC = £90 (DIY electric skateboards.com)(https://www.electric-skateboard.builders/t/sale-uk-vesc-motors-mounts-wheels-enclosure-gt2b-wheel-pulley-kits/21191)
Remote and receiver = £20 (GT2b) (https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html?gclid=Cj0KEQjwioHIBRCes6nP56Ti1IsBEiQAxxb5G4L_b3V03gWQc_uZHtMubk-BJ3HS_ELkExHkcimnqqQaAuD08P8HAQ&gclsrc=aw.ds)

Switch = 
Charger = https://www.amazon.co.uk/HOBBYTIGER-Digital-Battery-Balance-Charger/dp/B01BBJKB8Y/ref=pd_lpo_vtph_21_bs_t_2/260-9328836-7975037?_encoding=UTF8&psc=1&refRID=SCKANQFJ22PHBHHNDYDM#Ask 
Enclosure = 

Deck = £40 budget
Trucks = ~£45 Caliber II 50's
Wheels = ~£40 83mm 76a or 78a
Bearings = £26 Bones super reds (https://www.amazon.co.uk/d/Skateboard-Bearings/Bones-Super-Precision-Skate-Bearings/B002NES3MS/ref=sr_1_3?ie=UTF8&qid=1493235576&sr=8-3&keywords=bones+reds) 


Electronics = £290

Board = £150

With a £500 budget I'm left with £59 for a switch, enclosure (I've seen these done real cheap) and a charger.

Thank you all  for your help so far, I'm psyched
```

---
## \#29 Posted by: bigben Posted at: 2017-04-26T21:29:08.247Z Reads: 44

```
Instead of a switch you could go for a loop key using an XT90 plug. Plenty of info on the forum. You could also go for a 6374 motor?
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
After using them both I'd use a mini remote as opposed to the very good gt2b. (quite big though)
https://www.aliexpress.com/item/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32735708994.html?spm=2114.01010208.3.41.pWwY55&ws_ab_test=searchweb0_0,searchweb201602_1_10152_10065_10151_10068_10130_10136_10137_10060_10138_10155_10062_10156_10154_10056_10055_10054_10059_10099_10103_10102_10096_10148_10147_10052_10053_10142_10107_10050_10051_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10179_10181_10182_10078_10079_10073_10070_10123_10124,searchweb201603_4,ppcSwitch_5&btsid=48383dcf-aca6-43fc-9e8d-04418c118f80&algo_expid=1a1d7cc6-5a06-45d3-b60e-e96c6273a117-5&algo_pvid=1a1d7cc6-5a06-45d3-b60e-e96c6273a117
```

---
## \#30 Posted by: Youssless Posted at: 2017-04-26T21:38:31.600Z Reads: 45

```
[quote="bigben, post:29, topic:21776"]
sing them both I'd use a mini remote as opposed to the very good gt2b.
[/quote]

Thanks Ben, though my focus is my budget at the moment, is the 6364 not powerful enough to lug my 95kg weight around?

I'll look into the remote you've recommended to see if its worth the extra price. If its just size then I think I'll stick with the cheaper GT2b and then transfer it to a smaller case down the line at some point.
```

---
## \#31 Posted by: bigben Posted at: 2017-04-26T21:53:50.513Z Reads: 53

```
If you've not got too many hills you might be ok.
I hear what you're saying about getting a smaller case down the line. I couldn't face the faf though! You should be able to save a few quid by going with the loop key too.
```

---
## \#32 Posted by: sl33py Posted at: 2017-04-26T21:57:36.653Z Reads: 54

```
[quote="Youssless, post:28, topic:21776"]
Switch = 
Charger = 
Enclosure = 



With a £500 budget I'm left with £59 for a switch, enclosure (I've seen these done real cheap) and a charger.
[/quote]

Switch - i'd just do a simple anti-spark loop key like this:
https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

Charger - look for a decent iMax B6ACv2 - integrated power vs needing an AC->DC power supply.  Not super fast at only 5A...  but good compromise charger.

Enclosure - Look at Kydex or ABS you can form yourself w/ a heatgun and patience, or look for a pre-made one you can buy from some of the guys here.  Psychotiller comes to the top of my mind if you want to buy:
https://www.electric-skateboard.builders/t/vacuum-formed-enclosures-for-diy-electric-skateboard-components/145

His how-to:
https://www.electric-skateboard.builders/t/making-your-own-vacuum-forming-set-up-cheap/126

Or you can try GF/CF enclosure you make yourself.  Here's a good thread on how-to on the cheap:
https://www.electric-skateboard.builders/t/how-to-make-glass-fibre-enclosure-without-vacuum/17197

Lots to learn and takes practice - depends on your ability and desire to learn new things!

GL!
```

---
## \#33 Posted by: Youssless Posted at: 2017-04-27T08:21:53.932Z Reads: 45

```
Thanks @bigben, there aren't many hills around where I live, the ones that are present/that I would ride are gradual but long (gradual incline over 100m to the longest at about 2.5km).

The other concern I have is that a wider motor might prevent me from installing a second motor down the line if I want the extra torque. I imagine I could also remedy torque provisions with different gear ratios,yes?
```

---
## \#34 Posted by: bigben Posted at: 2017-04-27T08:29:37.129Z Reads: 40

```
You can change the gearing yes. 
To fit two motors in the trucks you'd need to go with 6355 motors I believe. 
I did run a high kv 6355  originally on 6s and it was ok. (Alien) 
ANothing like the big motor I have now. 
I am moving toward a dual drive if nothing else but for better braking!
```

---
## \#35 Posted by: Youssless Posted at: 2017-04-27T08:32:45.547Z Reads: 38

```
In which case I think I'll stretch to fit the wider motor. Thanks!
```

---
## \#36 Posted by: MannyM0E Posted at: 2018-01-23T04:46:39.279Z Reads: 20

```
[quote="sl33py, post:8, topic:21776"]
to calculate your distance - determine your Wh of your pack (V x Ah = Wh), and 10Wh = 1km (typical).  Good ballpark to see what size pack (mAh and voltage) you need for your goal of 10-15miles (you want 160-240Wh pack - easy math helps).
[/quote]

So for (3) 5000mAh 3s 25c Lipo it'll be 
(4.2V x 9s) =  37.8V
(37.8V x 5mAh) = 189Wh
(189Wh / 10) = 18.9km/11.744miles
```

---
## \#37 Posted by: scepterr Posted at: 2018-01-23T04:51:31.325Z Reads: 19

```
You should calculate at nominal voltage, 3.7v
```

---
## \#38 Posted by: MannyM0E Posted at: 2018-01-23T04:54:35.101Z Reads: 20

```
16.65km/10.346miles 😁 Thanks
```

---
## \#39 Posted by: scepterr Posted at: 2018-01-23T04:56:43.118Z Reads: 19

```
It's also gonna take some tuning and tweaking to get to 10wh/km, keep that in mind too when evaluating real world range
```

---
## \#40 Posted by: Youssless Posted at: 2018-01-23T07:40:38.165Z Reads: 14

```
Yeah I can say that with my setup and riding style I consume just under 15Wh per mile since I like to punch the trigger a lot lol
```

---
