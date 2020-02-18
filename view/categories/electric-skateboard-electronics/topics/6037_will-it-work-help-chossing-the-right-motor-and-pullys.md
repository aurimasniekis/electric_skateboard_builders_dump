# Will it work ? help chossing the right motor and pullys

### Replies: 12 Views: 2029

## \#1 Posted by: RomR Posted at: 2016-07-13T16:53:37.763Z Reads: 166

```
Going for my first build and i decided to go with this battrys:

* 2x FLOUREON 14.8v 6200mAh 4s 35c  so in total it will be 8s 12400mA

* Enerition vesc

no my big concerin is chossing the right motor and pullys...
@Hillso sugested going with hobbykings Turnigy Aerodrive SK3 - 6354-260kv Brushless Outrunner Motor
and i got some sugestions to go with Alien 5070 HEV Outrunner brushless motor 270KV 2200W

now my qustion is what will be the best for me (as a first time builder with no exp) to buy,
and yea i will need to feat the pully system and evreything wihch will be littel bit diffucalt for me (not buying a premade kit) thats way i prefer to go with alian, but i understand the most kv i can use is 260 or it will damage the vesc....

what should i do guys ? 
thanks for the help!
```

---
## \#2 Posted by: AutoHax0r Posted at: 2016-07-13T17:24:31.299Z Reads: 155

```
Hi,

Welcome to the forum - I'm quite new to here as well.

Sadly, your two batteries won't give you 8s 12400mA. There are two ways to connect batteries:

**Series**: Doubles your voltage.
**Parallel**: Doubles your mA.

You're going to want no more than 8S, to not damage to VESC, so preferably connect them in series. This is certainly up to you, though. Speed/torque vs range?

Both motors are great. I'd choose the Turnigy SK3.
```

---
## \#3 Posted by: RomR Posted at: 2016-07-13T17:40:05.370Z Reads: 128

```
im aiming for range aginst speed... i will need a small climbing abillity (not much hills here but there are some)

what batterys would you sugest ?
```

---
## \#4 Posted by: sl33py Posted at: 2016-07-13T17:42:28.778Z Reads: 136

```
Hey RomR - welcome to the madness.  It's a slippery slope my friend, but so much fun!

First off - as AutoHax0r mentioned - in series to double your voltage it will remain 6200mAh capacity.  (and 183 Watt Hours!)  Wh is an important measurement - roughly for 10Wh you can go 1km.  Weight, hills, riding super aggressively will all affect/diminish range, but a good rule of thumb.  You get Wh by taking your pack voltage (29.6 for 8s) x Ah (6.2Ah).  Or 6200mAh/1000 (same thing as 6.2Ah).

So, that confusing bit of mathematics aside - it's time to start reading and educating yourself.  I would look at folks builds here and on Endless-sphere.  There are some great stickies on ES - how to build your own e-board or similar.

I will caution you on going DIY unless you want to become skilled building it yourself.  If you want a pre-made and ready to go board... DIY is probably going to be frustrating for you.  You will need to do some soldering for almost any DIY build.  So a good soldering iron, wire, flux, solder, shrink tube assortment, and misc tools - all really helpful to have.  And you can spend $$$ on those (especially a good solder "station" which can have hot-air rework ability).  Good tools are expensive.  

If you still want DIY and plug-and-play... I would recommend checking out one of Enertion's pre-made boards.  Best of both worlds.  Or one of their kits to electrify your own board.

Otherwise i'd check out the new boosted offering, or similar production boards.

It really depends on your willingness to learn, tools and skills to DIY, and budget (always a major factor).  It can be cheaper to DIY, but it also can be a lot more $ when you get all the tools, quality components can be expensive, and misc to fab/DIY your own.

all those caveats aside - you asked about motors and pulleys.  It will depend on your weight, and what kind of riding you will be doing.  Everyone wants to be able to ride up 30% hills...  But realistically if you are just cruising along on the flats - you don't need dual motors and geared down 12/44 (motor/wheel gears).

So first off - how much do you weigh?  If you are <150lbs it's really easy to get a single motor setup.  If over 150lbs you can still do a single, but it may not be as great accelerating or going up hills.

What kind of riding do you want to do?  Just cruising along?  Commuting?  Going like a bat out of hell all the time?  And what kind of hills where you will ride?

Maybe most importantly - whats your budget?  

We'll get you squared away - just give us some more detail.

GL!
```

---
## \#5 Posted by: RomR Posted at: 2016-07-13T18:05:38.291Z Reads: 140

```
First of all thank you for the informetive comment!

im 75kg and my raiding goal is crusing around and going to work.
im not going to climb alot of hills so up hill abillty isnt my main issue but i will have a hill from time to time.

regarding tools im going to build it at my frinds dads garage (he modifys Razor RZR (kind of a off road veiacale))
so there ill have all the tools.

my budget is 700$ inc shipping, i aimed for a premade one but seens it will be much more expnsive and ill lose the exprince of bulding my own :)
```

---
## \#6 Posted by: sl33py Posted at: 2016-07-13T19:50:08.118Z Reads: 140

```
shipping is going to fluctuate a bit depending on location - let alone import fees/taxes.  So i'll outline my recommendations with just basic pricing to get you going.

I had a great chat with @exnor the other day and here's part of our discussion:

costs wise - the DIY can be cheaper for sure.  but if you want a 
premium deck like Loaded... it's easy to spend 150-250 on a nice deck.  
single vs dual motors and the type of motor really makes a difference.  
Between the extra motor mounts (again one of the most expensive 
components), and the gears (motor/wheel).

I'd break it down like so:

deck - $30-$250
trucks - $20-60
bearings - free to $80
Wheels - clones $30 - $80
motor mount(s) - $70-150 (each)
Gearing (motor/wheel) included in kit to $50ish
Motor(s) - realistically $50-100 for <6s or 12s 100-180
ESC(s) - >6s = hobby/RC $60-80.  >6s (8/10/12) = $100-200.  x2 if dual motor.  VESC are my preferred at 150'ish.
Misc (wire, solder, connectors, etc.) - $50 or more

So realistically - picking a cheapish board (not ebay blank for $30),
 good trucks, bones reds bearings (minimum IMO), clone wheels and single
 SK3 motor setup (gears/motor mount, etc) - i'd guess $600-700

Dual setup, trying to have a less expensive setup - no crazy $300 deck - likely about 900-1k.

You can super budget together a board for probably around $400.  If 
you can work aluminum w/ a router and file you can make your own motor 
mounts and save even more $.  I think onloop did a video on <$400 
setup.  I don't have the time/skill/tools to make my own quite yet, so i
 buy the kits to get the gears/mount/belts/etc.

I would usually get my components from one or two places to minimize shipping costs.  I've had great/fast service from both Enertion and  (Torqueboard's site).

For a single setup, here's what i'd get

Deck - personal preference.  I have some cheap blanks to custom carbon $250+ decks (i think i have 8 or 9 decks now - only a few are electric).

Motor mount - either [Enertion](http://www.enertionboards.com/electric-skateboard-parts/carbon-fiber-motor-mount-enertion/) or [DIYes](category/electric-skateboard-parts/electric-skateboard-motor-mount/). ($60-70 for mount only)

Alternatively - and likely save a few $ - the [kit from DIYes including gears/belt](diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-with-drive-wheel-kit/). (117ish)

Of the two mounts - depending on your deck (enertion is semi-adjustable, DIYes is almost fully adjustable and better for odd boards like drop decks or running motor in back more easily), i like the Enertion's simplicity and ease of belt adjustment better.  Unless you have an odd board or use where you need full adjustment or reverse orientation of the DIYes mount. You might be able reverse enertions as well - not positive.

But i prefer the wheel gear from DIYes vs Enertion's new injected molded gear which requires his trucks or to modify your caliber trucks to fit.  both are 12mm wide belt which is better for single motor setup (more contact area on belt = less skipping when braking hard).

Motor - DIYes 63mm motors, or Enertion R-Spec.  Either the [6355](http://www.enertionboards.com/electric-skateboard-parts/190kv-electric-skateboard-motor/) ($120ish) or [6372](http://www.enertionboards.com/electric-skateboard-parts/6374-190kv-electric-skateboard-motor/) ($160'ish).
[DIYes 6355 230kv](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355/) sensored ($90) or [DIYes 6374 230kv](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6374/) also sensored (120)

Trucks - Caliber II 50's are easiest and i like them.  pick a color/raw you like ($60)

Belts and gears - if not in a kit already - i would go for 14/36 as most easily available and geared down for slower speed.  Belt will be difficult to guess - there are some online calculators to help order the right length.  You can expect to pay 10-35 or so for gears (motor side 10-15, wheel side pulley 35ish).  

If you want the low profile (not visible on the outside of wheel, and are willing to modify your caliber truck hanger to fit (dremel/cut off material) - the [Enertion kit](http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-pulley-drive-hub-kit/) is a good option 15/36. ( $42ish)

ESC vs VESC.  you need to do some reading on pro's vs con's.  This is a Coke vs Pepsi type debate.  I love my VESC's and think they are worth the effort to use.  

VESC - from [Ollin/Chaka](http://www.ollinboardcompany.com/products) or [Enertion](http://www.enertionboards.com/electric-skateboard-parts/speed-motor-controller-esc-vesc.html).  150-180'ish
[DIYes 12s ESC](diy-electric-skateboard-kits-parts/torqueboards-12s-120a-car-esc-opto-hv/) - ($145) but remember you'll need the $15 programming card too.  he has [several other ESCs](category/electric-skateboard-parts/electric-skateboard-electronic-speed-controller/) including VESC (batch order for $99).

I'm working in my head backwards from the back of board forward...  So next is Rx.
Controller - Tx/Rx - [GT2b](http://www.hobbyking.com/hobbyking/store/__31671__HobbyKing_174_8482_HK_GT2B_3CH_2_4GHz_Transmitter_and_Receiver_w_Rechargable_Li_ion_Battery.html).  Then if you have access to a 3d printer or want to pay for a new enclosure you can pick one of the versions (badwolf, Flatline customs, or baby buffalo).  ($25 + $ for new enclosure)

here's my how-to for GT2b into badwolf:
http://www.electric-skateboard.builders/t/how-to-hack-build-compact-controller-using-gt-2b-badwolf-v2-enclosure/114

there are other controllers - Wiiceiver/Kama is a good option if you don't have much 2.4ghz interference where you ride.  Enertion has a nice controller, Winning little mini controller, etc.  I like the GT2b the best for rechargeability, and rock-solid connection.

Batteries - I'd recommend starting w/ two batteries in series.  Something like 2 x 3s, or 2 x 4s.  You can then add a 3rd or 4th if you want to go to 9s and 12s later.  More powerful, and faster if your ESC supports 9/12s.  It's also nice to give your board to a friend on 6s vs 12s so it's easier to learn on (less powerful).

Hobbyking has a ton - i would select the thinner 3/4s batteries like these:
[3s Turnigy 5000mAh](http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=9184) (23mm thick!) - ($25ish)
[4s Zippy Compact 5000mAh](http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=21371) - 29mm thick (40ish)

You can also look at 18650 packs from Enertion (SPACE cell) or custom from @barajabali - just more expensive usually.

That's it for electronics...
Wheels - 83mm flywheel clones from ebay or amazon - $40ish
bearings - i like good bearings, but you can get no-name or bones reds to start for free(included w/ wheels) or bones reds 20ish.  Tekton or Biltins are my favorite.  Good bearings, and maintenance to extend bearing life are really part of skating IMO. 

digest digest digest - i know i just dumped a ton of info on you.  You're lucky you have your Dad's friend's garage to work w/ his tools.  With some help from your friend this can be a fun project and GL!
```

---
## \#7 Posted by: Namasaki Posted at: 2016-07-13T20:11:21.255Z Reads: 103

```
[quote="RomR, post:1, topic:6037"]
my big concerin is chossing the right motor and pullys..
[/quote]

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125?source_topic_id=5899
```

---
## \#8 Posted by: RomR Posted at: 2016-07-14T12:46:47.546Z Reads: 102

```
So ive done some caculating and i thought about going with this spec:

Battrys:
2x Floureon 14.8v 5200mAh 4s 40c
Motor:
Turnigy Aerodrive SK3 - 6354-260kv Brushless Outrunner Motor
Vesc:
Enetrion vesc
Controller:
Winning 2.4ghz remote

and Enrtion Mono drive kite for all the rest (hubs, wheels, pullys, motor mount, etc...)

is it good ?

evrey thing will cost around 600$ which is grate for my budget :)
```

---
## \#9 Posted by: sl33py Posted at: 2016-07-14T18:29:26.592Z Reads: 112

```
A solid setup.

I would personally get some thinner batteries.  I've not heard anything either way on the "Floureon" brand batteries - but the specs don't look great compared to the nicer hobbyking offerings.

I would look at the Zippy Compact which is 29mm thick x 2:
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=21371 (~$38)

If you are already getting SK3's from hobbyking i'd get batteries at the same time.  I would also shoot for a lower kv motor - somewhere between 190kv-245kv.  260 will also work, but it's a bit higher than i prefer.

The Enertion mono kit looks good and has everything to get you going.  

A note on connectors - it's common to get multiple different connectors on your batteries, vs the ones on your VESC, and even between your SK3 and VESC (usually SK3 has 4mm - VESC 5 or 5.5mm).

So while you are getting motors and/or batteries from HK i would pick a standard plug you want to use, and then convert any on your board to this standard.  Avoids a ton of random adapters from one plug to another.

I like the XT-90's and XT60's.  but i've ran Deans in the past as a standard as well.  Almost any sized appropriately will work, it's just easier to pick one and stick with it.  Charging via parallel board w/ the right connector/plug etc...

Some extra wire (12g or so) shrink tube, solder/flux/iron, etc.

Look forward to seeing your build!  Best of luck.
```

---
## \#10 Posted by: RomR Posted at: 2016-07-15T07:11:51.280Z Reads: 107

```
im trying to avoid tax, as well caustomes check.

im thinking on 3 battrys right now, so i dont really know what to do yet.
i made an EXECLL chart with all the parts, ide love it if you can give it a look and tell me what you think and if i got evrey thing :slight_smile:

https://docs.google.com/spreadsheets/d/10FPlsoEd44ZtcRAARpaonp-WESeh7hf9R0mxYcWkAJY/edit?usp=sharing

cheers!
Rom.
```

---
## \#11 Posted by: dvoynin Posted at: 2016-07-16T17:19:18.992Z Reads: 78

```
I don't think you need batteries with such a high C rating.

Your motors max draw is 70A (which you will never draw continuously) and your batteries can supply 220A (5.5Ah x 40C) even with 20C you should be ok.

At least thats what I believe I may be wrong, have a read here (if you haven't):
http://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/
```

---
## \#12 Posted by: Conman Posted at: 2017-10-17T18:27:06.565Z Reads: 28

```
I agree with you. Might add that it can depend on your terrain, rider weight and gearing mainly tho.  If your setup properly to achieve an optimal performance (I’ll leave this alone).  I’ve seen examples of guys topping out at 100 amps or so but you can (should) limit your speed controller to max out according to the specs of your motor. About 60 to 80 amps.  That being said if a battery is designed to perform at a higher C rating it will go under less stress and you can prolong the life of it and keep the heat down in those tight inclosures.  I’m planning my build to be over spec’d for a good robust safety margin.  Such as a battery that can discharge 2x 5s 4000mah Lipo at 25-50c (I like lipoly cause of there power density and voltage that comes nice and close to the specs of the motor) and I’m gonna take the balance leads and integrate a 100amp bms (rates for 100amp continuous as it shouldn’t see above that for more than a few seconds).  My thinking is the battery can handle 200amps tops and I’ll never ask more than 80 for my motor and will be able to discharge 100 anyways from my bms ($73 is worth it to me) my battery will never so much stress and stay much cooler staying under the %50 capacity at its max.  I don’t need distance on my board (keep in mind an efficient C rating reduces voltage sag resulting in more efficient battery use anyways).  Keep in mind I haven’t done anything myself. I’m in my research mode atm. Buying coming soon! Not claiming I’m right either. May have some misleading facts in there but as far as I’m concerned your 20C rating is good at 5ah
```

---
