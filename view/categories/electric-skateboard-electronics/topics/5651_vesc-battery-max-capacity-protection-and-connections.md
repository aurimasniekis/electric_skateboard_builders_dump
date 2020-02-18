# Vesc battery max capacity (protection and connections)

### Replies: 32 Views: 3803

## \#1 Posted by: nick191 Posted at: 2016-07-06T13:06:49.499Z Reads: 358

```
I'm about to build my first eboard and was wondering about the max capacity of battery to fit the vesc from enertion. I'm not too sure how too hook them up series/parallel as well as protection for vesc. I'm looking at some from hobby king now and a bit confused with them all and not sure how much is too much for the board to handle. 
ps sorry about making a new post been looking around for the last couple of days and couldn't find an answer. even a reply telling me a useful thread would be helpful if you know of one or even a short response  sorry for the inconvenience.
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-06T16:15:34.574Z Reads: 345

```
If you're looking for max capacity you'll want cylinder cell li-ion batteries. They're more energy dense than LIFEPO4 cells and Li-poly packs. Depending on how you lay it all out you can get upwards of 700+wh. For reference the Space Cell Pro 4 from Enertion has a pretty nice size and is 360wh. There's no capacity thats "too much" for the board to handle, it'll just get heavier and potentially produce more heat. Lithium batteries die quickly from too much heat. I'd recommend making/buying/commissioning a 10/12s 4-6p pack.
```

---
## \#3 Posted by: sl33py Posted at: 2016-07-06T16:55:03.942Z Reads: 332

```
I'll offer an alternative.  Instead of building an uber $ battery - go inexpensive to start and upgrade later.  HK lipos are relatively cheap, and flexible.  Flexible in that you can take 4 x 3s lipos (nice slim ones around 4-5000mAh (25C or so)) and set them up as 6, or 9, or 12s.  So when you want to show a friend your board, and they haven't ridden - you don't hand them a 12s setup they crash on.  Much more manageable at 6s...  I do this with my GF i set her up with dual 3s, and when i ride "her" board (mine she's permanently borrowed), i use 2x4s.  

For a first board, i would start small w/ a single motor.  Then only dual motors depending on your weight and if you need to go up steep hills (20-30% grade).  If you are heavy (like me) or want to ride around San Francisco...  you likely would need to get dual motors.

Check out some of the thread and stickies on ES (endless-sphere).  Some great (if dated) tutorials on a basic setup.  

VESC is awesome, but configuration can be a bit intimidating (not actually difficult, but tons of options).  If you follow the step-by-step videos from Vedder (on Ubuntu) - it works great.  Alternatively, depending on your comfort w/ Linux, you can also use one of the Windows or Mac BLDC ported options.  Just make sure you use the right version for your firmware.  And for VESC - you *must* do the motor detection and configuration.  Don't even try to use it without.

So, tell us more about yourself and what your goal is?  How heavy are you, are you riding lots of hills or flats?  Even with moderate hills, a single setup if you are a lighter person should work fine.  And you can easily add a second motor later if needed.  So no need to spend $$$ to start until you get a feel for what you need.

my .02

Welcome and look forward to helping if i can!
```

---
## \#5 Posted by: nick191 Posted at: 2016-07-06T23:24:41.989Z Reads: 264

```
@sl33py 
Thanks heaps I am looking at an enertion mono drive kit. Not looking at going up massive hills just around town. One I get the enertion kit and a vesc Am i just needing batteries and controller? 
What would you recommend for batteries and connecting them preferably from hobby King and do I need spark protection for the vesc.
```

---
## \#6 Posted by: raxell Posted at: 2016-07-06T23:26:50.570Z Reads: 269

```
Taking adventage of this thread.
@sl33py  Can I swap batteries (example 6s-10s) when i want or may i have to setup VESC config before?
The first time I config VESC, can I power it with a 5s battery and when it will be configured swap to 10s battery?

@nick191 I am a newbie like you. I'm waiting 2x lipo batteries 5s 8000mah. I think that spark protection is a "must have", so i read
```

---
## \#7 Posted by: sl33py Posted at: 2016-07-07T00:16:46.929Z Reads: 250

```
@nick191 @raxell - hey gents.  Glad it's helpful.  It's just my .02, and what Jinra said is valid as well.  I prefer the simplicity and cost of the lipos from hobbyking, but do dream of getting a custom or DIY built 18650 pack one day soon.  

Nick - you never said your weight, but with a mono setup i'd suggest the following:
VESC - it's expensive but worth it.  You do need some technical "savvy", but if you can follow directions (copy/paste steps) it's doable.

Does your mono-drive kit from enertion include a motor?

You will likely still need some wire, connectors, shrink tube, etc.  Soldering ability is a plus, but you might be able to buy some pre-made cables and use those as well.

For a controller - i'd recommend the GT2b.  Get the mad monkey, baby buffalo, or badwolf enclosure for it.  Most reliable and good feel for the trigger.  If you don't have a 3d printer - you can d/l the .stl files and use 3dhubs or similar to print the enclosure.  Again soldering skills needed.  Or use it as-is for a bit.  Bulky but still works great.

Batteries - i'd recommend the slimmest 3 or 4s batteries you can find on Hobbyking.  Any of the 4-5000mAh 3/4s batteries around 20-25c should work.  I usually sort by their "C" size to get the thinnest batteries possible.  Then run them in series for 3/6/9/12s, or 4/8/12s (3s or 4s).  I like to keep mAh capacity around 5Ah/5000mAh and then swap packs when needed.  I do have some 8000mAh 4s i run on my GF's single 6355 200kv setup that work great as well.  It's really about how thin you want to keep them.

here's the 5Ah flightmax ones (25mm thick) -  also about $24 ea (wait a few minutes before adding as they often give you a lower "buy it now" option:
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=8579


Anti-spark - i'm a fan.  You can get something nice from DIYes or Enertion, or DIY.  Can't go wrong with either.  I did a how-to a bit back on how to DIY:
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

A loop key is the simplest and cheapest kill switch - adding the XT-90 anti-spark type makes it also a great anti-spark for connecting your batteries.  Not hard, but you do need some solder skills.  A good thing to learn if you want DIY e-boards.  And as far as projects go - it's a great learning process on these simple connectors vs swapping connectors on your VESC or other more sensitive electronics!
```

---
## \#8 Posted by: sl33py Posted at: 2016-07-07T00:25:35.912Z Reads: 206

```
It depends how you configure the VESC.  I have swapped batteries between 6s (dual 3s), 8s (4s x 2) often w/o issue.  I use a dedicated battery monitor to alarm when any cell in the pack gets down to 3.6/3/7v.  

For initial setup of VESC - Ben/Vedder recommends a low amp setup - 12v lab power supply or small 3s battery pack.
```

---
## \#9 Posted by: nick191 Posted at: 2016-07-07T03:35:05.210Z Reads: 199

```
@sl33py
im 85kg and yes the kit comes with a motor www.enertionboards.com/diy-electric-s… how many batteries would i need and how do they charge ( all at once or seperatly) i think ill get the 5Ah flymax ones.
```

---
## \#10 Posted by: nick191 Posted at: 2016-07-07T03:45:06.708Z Reads: 204

```
Not too sure about what deck is best for this would be much appreciated if you could have a look.

https://www.warehouseskateboards.com/globe-prowler-vintage-black-thistle-skateboard-deck-10x38 

https://www.warehouseskateboards.com/dusters-california-skateboards-kodiak-sunburst-orange-skateboard-deck-9.75x36 

https://www.warehouseskateboards.com/globe-pinner-marble-skateboard-deck-9.75x41.25

@sl33py @raxell
```

---
## \#11 Posted by: sl33py Posted at: 2016-07-07T06:47:08.182Z Reads: 198

```
the least expensive option would be the Imax B6AC v2:
https://www.amazon.com/Genuine-SKYRC-Power-6Amps-50Watts/dp/B00ND7J38C
http://www.hobbyking.com/hobbyking/store/__58285__IMAX_B6AC_V2_Professional_Balance_Charger_Discharger.html

Also recommend you get a parallel charging board like this from HK or the better quality one from BuddyRC/Paraboard.
http://www.hobbyking.com/hobbyking/store/__31676__Hobbyking_Parallel_Charging_Board_for_6_Battery_Packs_2_6S_XT_90_.html
(it allows you to connect 6 batteries at once to charge and balance at the same time)

It will be slower than some of the dedicated DC chargers (where you need a AC/DC power supply).  But slow charging (while it will take you longer to re-charge your batteries) also extends their life.  Fast charging is great in a pinch, but you get fewer charge cycles on the lipo.  Not a big deal, but worth mentioning.

If you are just starting out i would get 4 batteries, and ride 2 at a time for 6s and double the range.  Then as you get more comfortable you can add them in series for 9s, and eventually 12s if you want.  I ride quite a bit on 8s and it works fine for me...

You will need to connect them in series - and pick a connector type (and stick with it).  I've had many over the years with RC and really like the XT-90's.  Bigger than you might need but they work really well and can handle more (overbuilt) than you need.  (the number on the XT plugs roughly = amp ability so xt-60's can handle 60A, XT-90's can handle 90A).  

Connectors if you go w/ XT90's:
https://www.amazon.com/ARRIS-Connecting-Batteries-Connectors-Wires/dp/B00ZOI9N4C
(i make these for myself w/ the combined connector using the XT-90 anti-spark.  Pretty slick if i do say so myself...)

Boards - tough one man...  it's like asking if redheads or blondes are better...  all personal preference.

AND... like redheads (crazy and a lot of work (and fun)) - the drop through deck "prowler" while doable is going to be a lot more work than the others since it reduces motor clearance and the lower ride height can be an issue w/ batteries on bottom.

And any of the top mount decks - you can be limited on the size of wheels you run.  I personally like to start w/ the 83mm flywheel clones (likely what's in your kit - your link doesn't work).  So instead of big ass risers to fit them, i'd get a symmetrical board like the prowler - just not drop through.

I really like the Loaded Vanguard shape.  @armandr posted a cool link to these guys:
http://www.customskateboards.com/Blank-Longboards/Blank-Freeride
@itsmikeholland[quote]These are made to order, so you could probably ask them to use just 100% rock hard maple and get a stiff deck.[/quote]

For the price - worth checking out!!
```

---
## \#12 Posted by: nick191 Posted at: 2016-07-07T10:57:50.337Z Reads: 160

```
@sl33py i love those decks but i don't think i can get them shipped to aus 
that battery connection would that be the spark connection as well and what setup do you have and what did you start off with.
```

---
## \#13 Posted by: sl33py Posted at: 2016-07-07T17:45:45.198Z Reads: 164

```
Gotcha - yeah AUS makes it a challenge.  My friends in Canberra and Sydney are always jealous of "Prime 2 day"...  Last time we went down we actually brought a few things they had delivered to our house.

So Decks - pick one you like.  A local skate shop also would be a good place to go check out - and talk w/ the staff to see what they recommend.  What i'd caution you is to make sure you have wheel clearance for at least 83mm wheels - without monster risers.  And though i like a bit of flex in a deck normally - this makes it more difficult w/ an e-board.  So you either want a stiff deck (easiest to make into e-board), or you need to keep the center free of enclosures and separate the batteries and ESC/VESC w/ room in the middle for it to flex (like on Boosted).  Not super difficult, but folks always seem to forget and then rip up their battery enclosure mounting when the board flexes under them.

I'm not following on your connectors question.  I like the XT90 connectors.  But i also make my own cables, and replace the connectors on my batteries to use XT90's.  

here's the bottom of my GF's setup - Vanguard 42 flex 1 (setup for me), Enertion mount w/ single 6355 200kv motor, VESC, and 3s/4s x 2 for 6s/8s.  on 6s it's about 13-14lbs!  
[img]https://lh3.googleusercontent.com/-rcLj8nCeszg/Vb_d6yPqIDI/AAAAAAAAlIQ/NmJZxBnrEawAC478HQzjGOE7EuDoHvrLACCo/s1152/20150802_210115.jpg[/img]

I tried to find a picture of the anti-spark series connector i made - it's basically identical to the one i linked from Amazon, just replacing the Male XT90 w/ the anti-spark XT90.  I had a couple different adapters made - an extension with the anti-spark plug on it, the series connector, and a loop key (how to linked above).

That help?  Or clarify what your question is on connectors?
```

---
## \#14 Posted by: raxell Posted at: 2016-07-07T23:29:11.048Z Reads: 142

```
@sl33py Thanks. I appreciate your help and your "how-to".

@nick191 I love vanguard board too but i'm in Europe, so expensive for me now. I have this [board](http://www.euroskateshop.es/shop/madrid-weezer-collage-3918p.html) 

I have ordered the same kit than you at enertion. I am waiting for it. And I'm 85Kg too xD
```

---
## \#15 Posted by: nick191 Posted at: 2016-07-07T23:49:41.129Z Reads: 145

```
@sl33py sorry my bad are the connection from amazon anti spark connections as well or will I need that after the connection So I'm trying to get a bit of a list together of what I need so far I think it is:
Batteries ZIPPY FLIGHTMAX 5000MAH 3S1P 20C
Enertion kit 
Vesc 
Controller Gt2b
Xt90 series battery connector 
Deck 
Parallel charging board  
What type of wire would you use
```

---
## \#16 Posted by: sl33py Posted at: 2016-07-08T07:17:44.734Z Reads: 145

```
Gotcha - no the one linked does not have the anti-spark XT90 on it.  Just regular series adapter for 2 batteries.  They are easy to make yourself - using two female XT90's and the anti-spark XT90 male.  
[img]https://lh3.googleusercontent.com/-120RWOs5I9A/V39RqsGEW3I/AAAAAAAAsns/vvjtyYTtukIVxywgmfYJMLitQH9DxyjygCCo/s1440/20160708_000054.jpg[/img]
[img]https://lh3.googleusercontent.com/-EbgBURjl5jo/V39RvoO-lmI/AAAAAAAAsns/1jI4Y63pRg806jR1Hh19kH4n77OZ3EO6wCCo/s912/20160707_235641.jpg[/img]
(one i use all shrink wrapped - and one set together so you can see how it connects - i use a 12g copper wire to bridge that gap like in my loop key instructions)
And here's a simple extension w/ anti-spark - handy to have!
[img]https://lh3.googleusercontent.com/-17MRRxz9tM8/V39RzZUz-pI/AAAAAAAAsnk/LwXwX6-mbm8x8AoW6vV7RnzO22jzr_FqQCCo/s912/20160707_235416.jpg[/img]

Do you have a decent soldering iron?  Soldering big gauge wire is a PITA without a good iron.  I would recommend some of the wet noodle 12g wire:
https://www.amazon.com/Deans-Noodle-Gauge-Black-WSD1410/dp/B0006NAOA2
(any of the nicer flexy silicone sheath wire should work - i like the wet noodle ones as they are true to claimed gauge wire)
I think the last ones i've been getting for wire are cheaper and just as good (someone here/ES recommended them): [Superworm](https://www.amazon.com/Superworm-Gauge-Silicone-Flexible-Racing/dp/B014AW4EEG)
[img]https://lh3.googleusercontent.com/--MtQXxMBiK4/V39R4L14GNI/AAAAAAAAsno/q8qrjGVDlAsOBLwy1AG2g4YDeB2zp1abgCCo/s912/20160707_235319.jpg[/img]


HTH and GL!
```

---
## \#17 Posted by: nick191 Posted at: 2016-07-08T12:49:36.255Z Reads: 138

```
@sl33py
would something like this work to go from the battery to an xt90 connector <img src="/uploads/db1493/original/2X/e/e810c6d8b045d71bc778f1d24813dcca0e7bbf3d.png" width="594" height="500"> 

or something like this 
<img src="/uploads/db1493/original/2X/e/e118fcbad15a04a0f8f1674cb1616b6ad4c5cf6a.png" width="600" height="500">
```

---
## \#18 Posted by: sl33py Posted at: 2016-07-08T16:33:31.384Z Reads: 136

```
the second one definitely will work.  the first and longer extension is usually something you'd use to charge, but being simple 4mm bullet connectors i think you'd need to swap the positive to a female (like in second adapter).

Even better would be to physically swap your batteries connectors to XT90.  Do one wire at a time (then you can't short them!)  Trust me - a short on one of these will make really big sparks (welding metal kind of spark).  Some shrink tube, a good iron (those flightmax batteries look to have 8/10 awg wire - beefy), solder, flux, and new connectors - pretty easy.  

Heavy gauge wires can be a PITA to solder - they are basically huge heat sinks and absorb the heat from the iron too quickly if you don't have a really hot iron and bigger tip (more contact area to heat the wire).  Flux definitely help and i would practice on some 8/10g wire before doing one of the batteries unless you already are reasonably skilled soldering.

The nice thing about getting your solder skills to a point you can do this easily - is the ability to make exactly the length and type of wires you need.  You can buy adapters like those linked, but you almost always end up with added complexity (failure points too) between the adapter and your current plug, and usually excess wire that just looks crummy.  stuff to get caught on while riding, or drag, or vibrate loose...  An enclosure and good cable/wire management will help with that, but if you're not careful it can be a problem.  

GL!
```

---
## \#19 Posted by: nick191 Posted at: 2016-07-09T12:45:33.118Z Reads: 129

```
@sl33py
thanks rob I'm waiting for orders to come now I have learnt so muchI really appreciate all the help you ave given me so far and once the packages start rolling in I may have a few more questions (I'm sure I'll have a heap) 
cheers Nick
```

---
## \#20 Posted by: sl33py Posted at: 2016-07-09T21:38:02.398Z Reads: 133

```
happy to help.  Ask away.

Some folks get grumpy about noob questions ("why didn't you search").  Gotta start somewhere and the only dumb question is the one you don't ask!

Best of luck!
```

---
## \#21 Posted by: nick191 Posted at: 2016-09-21T11:36:44.452Z Reads: 107

```
@sl33py  i've got my stuff on the way now im just wondering if i could have a look at your setup to see how you have yours on the board
```

---
## \#22 Posted by: sl33py Posted at: 2016-09-21T17:03:02.260Z Reads: 103

```
@nick191 - you want to see the wiring of my board?  you can setup yours any way that works w/ your deck and battery placement, and length of cables...  

OK, here's my GF's board as an example:
[img]https://goo.gl/CcyIFG[/img]

This isn't anything fancy or particularly well thought out.  my first DIY and test bed.  I'm going to re-do it soon w/ a new wheel gear and enclosures for everything.
```

---
## \#23 Posted by: nick191 Posted at: 2016-09-22T05:03:26.471Z Reads: 95

```
Thanks @sl33py so you need a voltage alarm on lipo batteries? Will it damage the batteries if I drain them to low?
```

---
## \#24 Posted by: sl33py Posted at: 2016-09-22T06:03:01.859Z Reads: 90

```
[quote="nick191, post:23, topic:5651"]
Will it damage the batteries if I drain them to low?
[/quote]


Yes you need a lipo alarm.  And Yes, this is the best way to damage your cells - over discharge them and they will puff or otherwise have issues.  Usually one weak cell will sag waaay early or puff or have problems.  Best investment is a decent little lipo alarm.  I usually set them to alarm at 3.6 or 3.7v (with heavy use and sag it will go a bit lower sometimes - so some insurance against that so don't damage the lipo).

GL!
```

---
## \#25 Posted by: nick191 Posted at: 2016-09-22T07:32:41.832Z Reads: 88

```
@sl33py Do you need one per battery or one for the two of them
```

---
## \#26 Posted by: sl33py Posted at: 2016-09-22T07:34:09.347Z Reads: 85

```
on per battery... or if you're like me in that pic, i measured both and the battery with the lowest cell got the checker.  Just get two - i was lazy.  They are like $2 ea on ebay/aliexpress.  not $.
```

---
## \#27 Posted by: Hummie Posted at: 2016-09-22T16:46:09.794Z Reads: 77

```
you may plan to put a case on your stuff but maybe you will get lazy...and then your batteries will be hit with ricocheting rocks and likely ruined.  I've ruined many and lucky I didn't ruin my escs too.  .  maybe even just cover them with a quick layer of fiberglass and resin or even easier and quicker with something else like just a thin hard plastic sheet.
```

---
## \#28 Posted by: sl33py Posted at: 2016-09-22T18:40:49.216Z Reads: 73

```
i hear you.  I inspect before charging, and GF rides it, so top speed is no joke about 8mph.  It's on the to-do list.
```

---
## \#29 Posted by: nick191 Posted at: 2016-09-23T07:17:36.623Z Reads: 72

```
 Are they caliber II trucks and an enertion motor mount? @sl33py
```

---
## \#30 Posted by: sl33py Posted at: 2016-09-23T07:23:09.280Z Reads: 76

```
Yep the Caliber II 50's w/ Enertion mount.  This has a printed wheel gear 36t, not sure #t motor gear.  15'ish i'd guess.

Enertion, DIYes, and a few others out there now all work well.  Realize that the aluminum mounts will act as heatsink and help cool your motor, where the CF (BLING!) Enertion doesn't do this as well (CF insulates).  Not a big deal and love the look and really well made mount (rock solid).  I've had ADS v1, Enertion, Psychotiller, DIYes v2 (soon v3 and v4 arrive).

Fiddly but my preferred is the V2 DIYes.  Enertion next for super simplicity and ease of setup.  The newer v4 DIYes should be cool as still 360* rotate ability.  Will do some small comparison when i get them and can see what i like/dislike.
```

---
## \#31 Posted by: nick191 Posted at: 2016-10-16T05:34:59.211Z Reads: 67

```
have i got the wrong motor i think i have its a sk3 5055 280 kv will it still work?@sl33py
```

---
## \#32 Posted by: sl33py Posted at: 2016-10-17T14:53:10.700Z Reads: 65

```
280kv is a bit high.  But should work.  You will want to make sure not to give it too much voltage (likely more than 8s - but i would need to run a calculator to confirm), so you avoid 60k ERPM.  If you are still using VESC as ESC (don't recall - please confirm)?

It likely will have less "off the line" or starting torque, and less hill climbing torque vs a lower kv motor.  but if it's a PITA to return or otherwise easier to keep - give it a shot.  A kick or two to start and you should be ok.  260kv used to be the recommended kv motor - so not too far off from that and it worked well (but cogged quite a bit at start w/o a kick or two).

GL!
```

---
## \#33 Posted by: nick191 Posted at: 2016-10-17T22:38:40.733Z Reads: 58

```
I'm using an enertion vesc @sl33py  have everything but the enertion wheel, drive train and the nano controller which will hopefully come once they sort out the controller.
```

---
