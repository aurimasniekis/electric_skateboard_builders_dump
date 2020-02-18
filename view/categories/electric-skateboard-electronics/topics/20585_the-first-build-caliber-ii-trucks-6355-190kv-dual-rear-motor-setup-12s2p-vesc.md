# The First Build &#124; Caliber II Trucks &#124; 6355 190KV &#124; Dual Rear Motor Setup &#124; 12S2p &#124; VESC

### Replies: 22 Views: 3553

## \#1 Posted by: fmb Posted at: 2017-04-08T03:28:46.340Z Reads: 341

```
So after some reading and feedback I have updated my plan for my first electric skateboard!

I don't have experience building with electronics I was hoping to get some feedback and clarification about my build before I buy all the parts. I've done some research but I want to make sure that my setup is correct and that I have everything I need. Thanks in advance!

I am planning on making at Dual Rear Motor Setup.

I have a diagram below outlining my setup. I was wondering if you could make sure that everything is correct? Thanks!

<img src="/uploads/db1493/original/3X/2/0/20e64666a8cbe66ac8e9f149f52de2ae0d98a504.JPG" width="375" height="500">

2 Motors - 6355 190KV diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/
2 VESC's - diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
1 CAN-BUS - diy-electric-skateboard-kits-parts/vesc-canbus-connector/
1 Male to Male Servo Connector - diy-electric-skateboard-kits-parts/male-male-servo-connector/
1 Dual XT90 Parallel Connector diy-electric-skateboard-kits-parts/dual-vesc-xt90-parallel-connector/
4 Batteries in Series and Parallel - 5000mAh 6S 30C https://hobbyking.com/en_us/zippy-flightmax-5000mah-6s1p-30c.html
1 Charger - https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html
1 Remote - https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html
1 Pair of Trucks - Caliber II 50 
I am planning on using a 36t/15t set up with a 12mm belt from Enertion


To make the parallel connector, I am going to use some 10 gauge wire and some 5.5mm bullet connectors from HobbyKing. 

If I want to extend a wire, can I just cut to connector off, solder in some 10 gauge wire, and solder the connector back on at the end of the extension?

Let me know what you think of this setup! Any feedback would be helpful! Thanks in advance!
```

---
## \#2 Posted by: sl33py Posted at: 2017-04-10T05:26:27.509Z Reads: 308

```
Hey FMB - welcome and a nice clearly laid out plan.

Couple suggestions and questions:

[quote="fmb, post:1, topic:20585"]
I don't have experience building with electronics
[/quote]

I see a lot of cables and adapters you want to buy.  Do you want to learn how to build electronics, and are you willing to take some of that $ for a nicer solder station instead of adapters?

https://www.amazon.com/Zeny-Soldering-Station-862D-Nozzles/dp/B00W1AG0FG
(i looked at .ca site and STUPID expensive equivalents - maybe look at ebay or banggood/aliexpress).  I would not spend more than 60-90'ish for a decent one like this.  

The advantage of learning how to solder is really part to learn a new skill - and save some $ (which you just spend elsewhere), plus ability to make custom cables for a nice tidy build - no "spaghetti" mess of cables.  I love making my small XT90 series and parallel connectors with just the 3 connectors and some copper wire - stupid easy and work well.  Finishing touches - w/ some heatshrink - they look as good as the purchased ones.

Motors - great motors.  I have a set.  Are you going to run it sensored?

VESC - DIYes, Enertion, Axle, Etc - all the 4.12 seem to be good quality and work well as long as you work within a few limitations.  Yes you can push the limits - but do you know how to replace a DRV chip if/when you kill it?  If not - i'd recommend sticking to BLDC (NOT FOC) - and no more than 10s.  Yes you can run 12s, but you are on the verge of the 60k ERPM limit, and even braking downhill you might exceed and kill the DRV chip.  Alternatively you might try the direct FET variants from Chaka/Ollin or the VESC X from enertion which *may* not have the 60k ERPM limit (not sure if this is truly fixed w/ these, but know the VESC 6 does seem to not have this limitation).  I'm going to get a VESC X i think and play with one on 12s.

Bouncing around a bit - Trucks - great trucks - best thing you can do is get the right bushing for your weight.  I really like the super high rebound or vhb variants from Venom, blood orange, rip tide, etc.  More "spring" back to center - but i'm a big guy.  Figuring what works best for you is really personal preference (barrel, cone, elims... etc.).  A local skate shop might be a good place to chat and see if they have any setups you could get onto to feel the differences to see what you like.  At least get the right duro for your weight and start there.

remote - good inexpensive choice.  If you have a 3d printer at school or know someone to help out - look at the badwolf or flatline customs files to move to a much smaller handheld formfactor.  I have tried a few and [did a basic step-by-step for the badwolf a few years back now.](https://www.electric-skateboard.builders/t/how-to-hack-build-compact-controller-using-gt-2b-badwolf-v2-enclosure/114)  I've definitely found it to be more reliable in areas with lots of bluetooth and wifi "noise" where other remotes still drop out occasionally, and my GT2b just keeps the connection solid!  

Charger - I'd suggest the iMax B6ACv2 instead - all-in-one so you don't need an external power supply.  At only 5A it's SLOW - but really inexpensive and pretty nice though slow.  If you are going to go to the effort of an external AC->DC power supply - look at an iCharger that can do 10/20/30A (denoted in the name: iCharger 306b i have is 30A and up to 6s).  The ACv2 version of yours is a bit more, but by the time you skip buying a power supply - it's probably about the same price.  You can cobble something together from a laptop power supply or similar - so it just depends on your creativity and willingness to solder up connectors and wiring to make sure it's also safe and not a fire hazard if you hack it together.  

Speed and gearing - 15/36 may be pretty common, but at 12s you will have a ROCKET that is geared to do 53kph (assuming 83mm wheels - 190kv - 12s - 15/36).  I would gear down and shoot for a top speed of 22-25mph/37-40kph.  

Since you already are getting gear from DIYes - look at his 40t gears (it will slow you about 2mph vs the 36t gear).  Additional bonus of those gears are they are aluminum vs injection plastic (which is pretty strong, but not aluminum strong), and you won't need to cut your Caliber II's hanger to fit them like the enertion gears need.

Saving the big one for last - batteries.  Why are you doing 12s, and 2p?  Are you riding it 30mi and need the range?  Those batteries are pretty huge, and heavy...  I am more of a thin and light w/ moderate range builder.  

Range and Wh - those 5000mAh/5Ah batteries * 25.2v = 126Wh (per 6s), so 2 in series gives you 5Ah * 50.4v = 252Wh.  Now in 2p like you plan that's 10Ah * 50.4v = 504Wh.  And since each weighs 730g - a simple 12s1p = 1.46kg/3.2lbs - so 12s2p you will be carrying 2.92kg/6.4lbs of batteries - that's a heavy and big battery to lug when you aren't riding.  A 20lb+ build...

And the usual range estimate is 10Wh = 1km.  So 12s1p/252Wh = 25.2km/15mi and 12s2p/504Wh = 50km/30mi!  

Wire - get good flexible silicone wire - easier to route and helpful that it's more flexible.  Superworm or wet noodle on amazon both work well.

You asked for feedback - sorry for the novella, but hope it's helpful.

GL!
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-04-10T14:12:38.587Z Reads: 268

```
@sl33py makes a lot of very good points. You probably do want to go with 10s max on your first build. Otherwise you're going to learn all about blown eswitches, blown ESCs, and other than just blown stuff, you'll find odd behaviors in braking, accelerating, and during top-end testing. 12S boards can be very high maintenance, which is why i offer the warranty i do. 

How are you planning to switch it on and off? Flier style eswitches will utterly fail at actual 12S usage, despite being rated at 12S.  Standard Vedder antispark eswitches will also fail, though not as quickly. I have some modified Vedder style eswitches that i've been using that use the 75volt mosfets instead of the typical 60v ones and they do not seem to be failing yet unless i blow one up by shorting shit out with the soldering iron, which can happen. PM me and maybe i can work out something with you to get you one. I can probably send you a raw one for $20 shipped. Decked out with xt60 connectors and heat shrink etc will probably be around $30 if you're interested. 

The ERPM limit is a real thing. Also, you may want to limit your actual RPM to something equivilent to 30mph or you're going to see some voltage sag that could potentially cause riding disruptions when you try to top it out and you're battery is below 20%. This MAY not be an issue with those zippy lipos, they're pretty solid packs and tons of people use them, but it is an issue with li-ion cells. I'm still working on a way around that one that doesn't involve custom volt meters and artificial limitations in the VESC settings or stupidly expensive cells. It's probably a wild goose chase but worth exploring. 

wear a fucking helmet. You're building a seriously powerful board. It may not have the watt hours and range that some others do, but its defintily going to have that ballsy 12S punch. You'll probably end up flying through a bush or something eventually so gear up. 

YES YES YES to the solder station. 30 watt Radio Shack/Walmart/generic soldering irons will work, but when you get a taste of that rework station you'll wish you had that $20 back from that cheap iron. 

Also, don't skimp on the solder. I have found that 50/50 tin/lead flux cored solder is the best for wiring. Its messy for SMD shit, but for wiring its great. It tins the leads very well and creates a very strong weld and is super easy to work with. That lead free shit at walmart/autozone/radioshack is bullshit. Get some 50/50 from Amazon, if you have prime you can usually get it the next day.  Use in a very well ventilated aera and try not to breath it in. Obviously. 

If you decide to paint your deck, go with a Valspar paint product. The Project Perfect spray paint comes in a variety of colors and is an absolute dream to work with.  Rustoleum, Krylon, and other known spray can brands don't seem to hold a candle to the Valspar spray stuff. The only other spray paint i've found that works well on everything from fiberglass boxes to alumium mounts is Duplicolor, which is hard to find.  If you prefer foam-brushing it, Lowes will sell you $4 samples of Valspar water based house paint in literally any color you can imagine. Its excellent for boards. They probably won't tell you this, but i swear i've seen so many Valspar cans in the backgrounds of Bustin's instagram that i went out and tried it. I think that's what they're using. It coats well, lightly sands smooth, and cleans up trivially easy. I have a few foam brushes i've been using for months because the paint just comes right out of them with water. For a clear poly coat, go with Minwax Spar Urethane, water based. They have a glass clear variety that works very well and also cleans up super easy with just water. 

Hot glue is a legitimate cable management solution. You can use it to tack down your receiver wires and stuff to keep things tidy in the box. And don't forget the tiny zip ties! They work well to keep things from turning into a pile of spaghetti. 

And yes, 15/36 on 83mm wheels at 190kv is a rocket on 12S. You'll be looking at top speeds of around 33 ish mph when actually on the board and riding. Of course if you're completely insane like me and my customers, you'll want to go with a 15/33 on 83mm at 190kv wheels and shit your pants with top ends approaching 37-38mph on flats. 

WATCH OUT FOR THE VTECH. If you're running unsensored motors you're going to have a noticable boost in "power" when approaching the top end. It will literally jerk forward a little as it kicks in and hits that efficiency sweet spot. We got used to it, we even laugh about it and look forward to it. HELMET. 

I would like to mention that the V-TECH effect is totally gone on my test board when using sensored motors on VESC-Xs at 12S. Not sure where it went, but topping my board out has become less interesting. By that i mean safer. Also, i don't know quite how it happened, but somewhere along the way we got bored with ONLY doing 35mph. Maybe I've been doing this too long. I was being followed by a cop yesterday in my neighborhood and i realized i was breaking the speed limit on one of the main roads that connects several hoods in my area. He looked puzled, but kept going after i turned onto my street. 

I used to be terrified of that board. Maybe i need a tolerance break.
```

---
## \#4 Posted by: rwxr Posted at: 2017-04-10T14:20:00.264Z Reads: 208

```
@longhairedboy: Your posts are as informative as entertaining. Love it!
@sl33py: I wish I had found a post like yours for my first build.
```

---
## \#5 Posted by: sl33py Posted at: 2017-04-10T18:34:04.288Z Reads: 219

```
Hehehe - i always love your posts LHB.  Great sense of humor.

I also agree on appropriate gear.  and at 25+ i think it's more than a helmet - pads or leathers like the downhill guys wear for a reason.  At those speeds you are going to slide or impact - wishing to slide...

[quote="longhairedboy, post:3, topic:20585"]
Maybe i need a tolerance break.
[/quote]
Maybe you need to borrow an E-Go or similar for a week.  After topping out around 10-12mph for a bit, suddenly 20 will seem too fast!

I've always geared for 25mph as my comfort zone - also relatively close to my skill level (not excellent, but decent and improving).  I usually ride in the 15-20mph range comfortably... until i ride with my buddy on his Dual+ who likes to top it out around 22-25, which i find myself pacing and keeping up.  It's nice to have the extra oomph and top speed infrequently, but cannot imagine 30+ on any sort of regular basis.  Just not big enough cojones i guess...  ;)

@rwxr - hehehe - i'm hot/cold on the forums, sorry i missed your first build and didn't help.  Sometimes it's nice outside and screw chatting - time to ride or fly (motorcycle/esk8 or paraglide).  Or usually work... work always screws with the fun!
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-04-10T19:36:35.797Z Reads: 202

```
[quote="sl33py, post:5, topic:20585"]
but cannot imagine 30+ on any sort of regular basis.  Just not big enough cojones i guess...  :wink:
[/quote]

i was that way until my son moved in.. then everything became a competition after he burned up two of my boards and started building his own. Now i'm a complete rush junkie. 

my favorite thing in the world right now is doing 30+ up a hill and watching the stares i get when the warbly whine of the motors start to sing the praises of Lord Skatan in unison.
```

---
## \#7 Posted by: fmb Posted at: 2017-04-10T23:40:25.992Z Reads: 190

```
Thanks so much @sl33py and @longhairedboy!! All of the information and feedback that you gave me was incredibly helpful!!

I will definitely be getting a solder station. It seems like a much better investment. Thanks for all the information about the solder station and the solder itself. I've been really worried about making any weak solders.

I am going to be changing the batteries as well. I think I'll be going with 5000mAh 5S 20C instead of the 6S. I want a powerful board but from what you've said I definitely think it's overkill and I don't want to blow the VESC. I'll also be changing the gear ratio to decrease my speed bit. I think for me first one I don't want to be crashing into anyone or anything.

That post on the remote is amazing btw @sl33py! I am 100% going to try that! I'm glad I have access to a 3D printer! 

I was planning to switch it on and off with an anti spark switch. I've seen the post @sl33py made about it and was hoping I could use that. That would work if I changed to the 10S batteries, right?

Thanks again for all the information! It is incredibly helpful! Without it I'm pretty sure I would have broken a bone or screwed up my setup. Thanks!
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-04-11T11:54:27.789Z Reads: 182

```
Something you could also do instead of changing your gear ratio is to limit your motor amps in the VESC to something lower than usual. That will give you a more friendly throttle response with a wider trigger range (provided your remote settings are good for your remote)  and won't be so brutal at launch, but the top end would always be there once you get more comfortable. Then later on you could increase them a little at a time as you grow into it.
```

---
## \#9 Posted by: fmb Posted at: 2017-04-11T14:43:57.640Z Reads: 188

```
@longhairedboy  I was wondering, I don't think the DIY VESC BLDC has programming? So are there any other VESC's with easy programming that you would recommend?

Also, @sl33py and @longhairedboy what do you think of this soldering station? 
http://www.ebay.ca/itm/BAKU-BK-601D-SMD-Brushless-Heat-Gun-Soldering-Iron-Station-with-Stand-700W-/172602609533?hash=item282feacf7d:g:rbEAAOSwB-1Y3XSj
Unfortunately I cannot buy the soldering stations on Amazon.com since I live in Canada and the majority of them do not ship to Canada.
```

---
## \#10 Posted by: mmaner Posted at: 2017-04-11T15:41:18.548Z Reads: 174

```
All VESC's are programmable (said configurable) via the BLDC tool.  THis includes the DIY VESC.
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-04-11T16:31:11.134Z Reads: 174

```
what @mmaner said. They're all configurable via USB and BLDC Tool. 


 That solder station looks pretty good but i have no experience with that brand. The stylus looks like it has those standard replacable tips though, which is very important. You definitely want those. And if you can, grab a few extra tips. You'd be suprised how easy it is to ruin them with shorts and bad solder chemistry.
```

---
## \#12 Posted by: sl33py Posted at: 2017-04-11T18:26:05.695Z Reads: 178

```
[quote="fmb, post:9, topic:20585"]
Also, @sl33py and @longhairedboy what do you think of this soldering station? 
  
    ebay.ca
  
  
    

BAKU BK-601D SMD Brushless Heat Gun Soldering Iron Station with Stand 700W |...

BAKU BK-601D SMD Brushless Heat Gun Soldering Iron Station with Stand 700W | Business & Industrial, Manufacturing & Metalworking, Welding & Soldering | eBay!

  
  
    
    
  
  

Unfortunately I cannot buy the soldering stations on Amazon.com since I live in Canada and the majority of them do not ship to Canada.
[/quote]


Yeah - that looks pretty decent.  Analog dial for the Iron temp - not a biggie and just make sure you get a good assortment of tips.  Working with big gauge wire like 12/10/8awg - the bigger tip is really important to get it to heat quick enough to solder.

Like mmaner and LHB already said - any VESC is configurable via USB and BLDC tool.  If you can throw together a linux system easily - it's copy/paste to update the VESC to latest firmware.  I usually do this to update and configure mine.  But i'm in IT and have an old laptop that is perfect for this.  Otherwise there are ported versions for both Windows and Mac.  But you need to pay attention to which hw version (likely 4.12 which is latest), and which version of firmware - some are "picky".

Another thing on the solder station - i think LHB mentioned it too, but *GOOD SOLDER* is really helpful.  Personally I like Kester 60/40 (but might try 50/50 like LHB suggests just for bigger wire - i currently dip my wire in flux before tinning - so basically same thing, just an extra step) - the .03 or .05 sizes.  (and also agree w/ @longhairedboy - lead free SUCKS so use the lead versions - remember to wash your hands w/ cold water after use, and don't breath in the fumes). 

HTH - GL!
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-04-11T19:09:52.816Z Reads: 164

```
[quote="sl33py, post:12, topic:20585"]
Personally I like Kester 60/40 (but might try 50/50 like LHB suggests just for bigger wire - i currently dip my wire in flux before tinning - so basically same thing, just an extra step) - the .03 or .05 sizes.
[/quote]

I've got that Kester solder too. 60/40 and 50/50. I think the Kester might be the best brand I've tried yet.  I like the .03-.06 for things like ppm leads and tiny stuff and the larger guages for petty much everything else such as butt joints, xt60s, bullets, and soldering leads onto eswitches and BMSs. 

I just bought a solder pot and am about to get some flux and start tinning my larger guage wires that way. Tinning 10awg and 12awg with an iron takes too long compared to the tiny wires which take a half second to tin with an iron.
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-04-11T19:22:05.671Z Reads: 174

```
[quote="sl33py, post:12, topic:20585"]
and also agree w/ @longhairedboy - lead free SUCKS so use the lead versions
[/quote]

also some of those brands of lead free crap will seriously corrode your tips. And i don't mean make them a little rusty. I mean it will pit them and literally dissolve them into misshapen and useless clumps of terrible. 

there have been several occasions where the only place i could get solder at the moment was walmart. You know, its three in the morning and you're finishing up some shit and damn you're out of solder. Walmart is all that's open. So i would settle for that lead free crap for the moment and then go ahead and try to use it up while waiting for the good stuff to arrive in the mail. By the time it got here my tip was a useless lump of pits and divots. 

This is why I have about 20 spare tips in a little plastic drawer. 

@fmb also these are the stations we're current;y using. They're inexpensive and very very reliable. We have two of them now and im kind of loving them:
http://www.mpja.com/Solder-Station-with-LED-Display-ZD-929C/productinfo/15845+TL/

and of course they have plenty of point tips for next to nothing:
http://www.mpja.com/Solder-Station-15845-TL-Replacement-Short-Shank-Pointed-02in-Tip/productinfo/15850+TL/

as well as blunt tips:
http://www.mpja.com/Solder-Station-15845-TL-General-Purpose-Thin-Shank-Blunt-Tip/productinfo/15854+TL

i don't see any flat tips on there for these though. I know they're really handy in some situations but i've managed to make due without them.
```

---
## \#15 Posted by: fmb Posted at: 2017-04-12T17:32:36.938Z Reads: 155

```
Thanks again @sl33py and @longhairedboy for all the information!!

Thanks @mmaner too!!

I was told that the VESC came configured so I didn't know I could change the settings. I will be doing lots of research on that. 

Are there any posts that you can link that have recommended setups for the VESC? Or since my setup is different with dual motors and different batteries that I will need to have a different setup? Are there any particular settings that you recommend?

Thanks for all the recommendations with the soldering station! I will either be going with the one @sl33py or @longhairedboy recommended. Both of them look really good! I found out that I will be going to the US for 1 day in April so I should be able to get one them and hopefully the hotel I am staying at will accept the package (I don't see why they won't)

And thanks for the solder recommendations! I am worried I'll screw something up so all of this information is really helpful!!
```

---
## \#16 Posted by: mmaner Posted at: 2017-04-12T17:36:58.008Z Reads: 154

```
This link will show you all of the VESC FAQ's.
https://www.electric-skateboard.builders/search?q=esc%20faq

Here are some more specialized VESC FAQ's.
https://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500
https://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244/2
https://www.electric-skateboard.builders/t/vesc-faq-windows-version-of-bldc-tool/141/27
https://www.electric-skateboard.builders/t/vesc-faq-limit-output-voltage-according-to-motor-maximum-specs/683
https://www.electric-skateboard.builders/t/vesc-faq-duty-cycle-vs-current-control-ppm-settings/1218
```

---
## \#17 Posted by: fmb Posted at: 2017-04-12T22:54:31.718Z Reads: 134

```
Thanks so much @mmaner I'll be going lots of reading
```

---
## \#18 Posted by: fmb Posted at: 2017-04-12T22:56:42.812Z Reads: 132

```
@sl33py and @longhairedboy I was wondering, should I be looking for a solder with a core (rosin?) or no core? 

Also @longhairedboy where do you buy your Kester 50/50 I was looking on amazon and I could only find one but it only ships to the US and it doesn't have Amazon Prime so I can't buy it for the day I go to the US.

Thanks again!!
```

---
## \#19 Posted by: sl33py Posted at: 2017-04-12T23:10:24.051Z Reads: 137

```
I'd get the 60/40 Kester and call it done.  I've not tried the 50/50 to be fair, but the 60/40 works well for me for everything else...  You can always get the other later online and slow-boat it to yourself in canada.

As for core or no the Kester i get (Kester 24-6040-0053 Solder Roll, 66 Core Size, 0.050" Diameter and .03 version too):
[quote]Rosin inch 44 inch is a high activity RA core flux designed for excellent instant wetting action, even on nickel surfaces. Although" 44 inch is a ra-based material, the residues are non-corrosive If not cleaned. Per j-std-004b," 44 inch is classified as Rom1 flux. [/quote]
```

---
## \#20 Posted by: mmaner Posted at: 2017-04-13T00:37:25.682Z Reads: 136

```
No worries, holler if you need anything else.
```

---
## \#21 Posted by: fmb Posted at: 2017-04-13T04:34:21.805Z Reads: 129

```
Thanks @sl33py!!! I'll be getting the 60/40 with the 44" core that you have!

You said earlier that you used flux? What flux do you use and how do you use it? (sorry if that's a dumb question)

Also, if I got the 50/50 eventually, would you recommend a core for that too?

Thanks again!!
```

---
## \#22 Posted by: sl33py Posted at: 2017-04-13T20:22:24.571Z Reads: 127

```
I can't find my flux on Amazon (from memory - might've changed packaging)...

THis looks like a good rosin flux (sticky and messy - be aware).
https://www.amazon.com/Rosin-Paste-Flux-135-Jar/dp/B008ZIV85A

There are probably better ones, but this would be a good start - the one i have is a bigger jar, and more of a "gel".  I might switch to one of the water soluble flux when this runs out - it gets sticky and is a pain to clean off.

GL!
```

---
