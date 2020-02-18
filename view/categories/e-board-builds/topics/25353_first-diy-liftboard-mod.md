# First DIY/ Liftboard Mod

### Replies: 104 Views: 10602

## \#1 Posted by: Lunasi Posted at: 2017-06-14T07:53:19.972Z Reads: 587

```
Hey guys, so I've been riding a while now and am a beta tester for leiftech, I've been wanting to start building my own DIY boards and learn more for a while. I won a liftboard as part of an amazon give-away and the thing is obviously a POS and I has given me problem after problem, but the good thing is I didn't pay a dollar for it and it offers up an great opportunity to start a DIY and learn something in the process. I'm looking at getting the dual motor mechanical kit from torque boards as well as two motors to start. I've already collected a bit of information on all this but I think I'm just having trouble connecting a few of the dots and am hoping to get the communities help. I am on a budget and am going paycheck by paycheck to build my own ultimate DIY, but am using the Liftboard as a base to start the whole build. Basically at this point I want to strip most the liftboard except for the battery and current vesc (with a friend from my riding groups help) and see if theres any way to modify the vesc for more speed or find out if I need to buy a different one in a future paycheck. For the time being I would be basically mounting this all on the current liftboard I have until I can afford a new deck and any other excess pieces. 

Big questions I'm coming to that I really need answered and I'll try to give info to extrapolate. The liftboard as I have read has a 21.9V8Ah (LG-HD2-18650-3.65V-2000mAh-6S4P) battery.... so for starters can I buy any motor and hook it to any battery basically? When it comes to the motor and battery connection can any motor be hooked to any battery, I am assuming that the battery being more powerful plays a stronger role in stronger wattage motors.

I realize without knowing a lot about batteries that a 6S4P battery is kind of weak, I have an old LT3X battery from my leiftech that kind of backfired from some wiring that came out but I think its generally salvageable, I'd like to get a new bigger enclosure from psychotiller or other and add those batteries to the 6S4P that is currently there, that should give me a lot more mileage, P.S. can I even do that? The LT3X from what I have info on is 24v, 144Wh and would probably be much better with the better motors anyways (I would think)? 

Ultimately this is a process I'm hoping to learn from and gain a much better board in the process, any help you can give would be amazingly appreciated!
```

---
## \#2 Posted by: lowGuido Posted at: 2017-06-14T08:17:43.766Z Reads: 541

```
so I just had to google (actually bing because my google broke.. long story) what the hell a liftboard was..
it looks like a rebranded benchwheel board.
probably first thing I would do is replace the ESC with a FOCBOX or DRV cooker of some sort to get you that programabillity that you are after. and chuck a few more cells on too.. 8S or even 7S if the wallet is tight. (its only a few more cells here and there.)

the motors and drive line will probably live up to 10S.. at a guess...
```

---
## \#3 Posted by: Lunasi Posted at: 2017-06-14T17:02:32.311Z Reads: 494

```
It's not a rebranded benchwheel but their company gets that a lot, that said it is incredibly cheap "like the benchwheel." Since I haven't paid a dime for it though it seems like the perfect base to learn some DIY on. If I don't change the vesc immediately will it run similarly to how it already does but just with added torque from the two better motors? I'm assuming it will probably run like a much better version of my current board until I can upgrade the Vesc or see if my friend can help me use the current one. How big of a deal is it to buy a VESC or ESC? Should I be looking at a site like torqueboards or is it all the same if I go to a local RC store to pick something up?
```

---
## \#4 Posted by: Hummie Posted at: 2017-06-14T17:15:16.094Z Reads: 450

```
do u have an actual Vesc or is it out of the leifbpard and a regular esc? If not I'd get that for starters. U only need one motor really to get enough power.
You do standup?
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-14T17:26:45.822Z Reads: 439

```
So one of my projects is to convert a bunch of the internals if my benchwheel like you. While liftboard may say it's not a rebrand the parts are almost completely identical, so I'm wary to believe them.

You may be able to reuse the enclosure and battery but if the liftboard is similar to the benchwheel, the bms is integrated with the ESC. You'll want to pick up one or two escs (should probably get a vesc) and a proper bms. Order a handful of xt60 connectors and 12awg silicone wire and you should be good to go on parts.
```

---
## \#6 Posted by: sl33py Posted at: 2017-06-14T17:27:10.546Z Reads: 441

```
it's definitely using the benchwheel remote (good remote i've heard), and looks like the benchwheel battery...  There are so many rebrandings it's ridiculous.  Regardless - 6s4p and single motor - how to make it "better" right?!

Is it a single motor or dual motor currently - i see single and dual Liftboards.

Are you using "VESC" generically and meaning ESC?  as in the motor controller (Electronic Speed Controller).  VESC is an open source ESC designed by Benjamin Vedder (Vedder ESC = VESC).  Great controller (best one so far IMO).

Depending on your weight - 6s should be fine.  I'm a big guy and ride regularly on 6 and 8s setups.  If they are legit HD2's they should be able to provide about 20-25A peak per cell in parallel.  So in 4p = 80-100A output capability.  So, until you have range or other power/performance issues - ride what you got!

Two motors will give you more torque for hills and accelerating to the same top speed as a single motor.

Upgrading motors and mounts - i'd only do this if an issue with the motor or mount.  I'd upgrade the ESC to VESC first and see if it sorts it out for you and works better.
```

---
## \#7 Posted by: Lunasi Posted at: 2017-06-14T18:07:45.877Z Reads: 410

```
@Hummie Yup I'm a comedian :slight_smile: 

I have whatever the liftboard comes with (can you tell I'm a noob?). I honestly still need to take the board apart but I'm waiting to get help from my friend and get all the parts in first. I know I would be fine with a single motor but I really want a dual motor board and here in Colorado there are a lot of hills so dual would suffice much better than single, plus my board is currently a dual so I don't want to go back to a single.

@Jinra While they do use similar if not the same components Liftboard from what I understand from the owner is still a US based company and the boards are assembled here and were not based off of the benchwheel but use similar components. Apparently the reason the board is so cheap is because the company orders parts in massive amounts for instance their last order for motors was for 80,000 motors.  

@sl33py Excuse my noobishness, still learning about everything so didn't really know quite the differences between vesc and esc, have only just started to get into that part of building the boards. I'm only 140lbs so I'm not a generally heavy rider. As far as the mounts that was one of the most important things off the bat. One of the reasons I've had so much issues with the current product is because their motor mounts. The motor mounts that come with the liftboard are NOT adjustable, this means they pre-set all the screws and positioning so you aren't supposed to be able to mess with it. The company has now replaced 3 boards for me because I kill or destroy something within about 5 days of riding it each time xD. Their mounts tend to have an issue where a screw will come loose and then one of my belts will lose all its tension on the mount, this has happened twice to me out of the 3 boards sent to me. The second board died from what couldn't even be called a "puddle" in a rain drain. The reason I'm trying to do the mounts and motors first is because I fucked up a motor after 5 days on it and the mounts are a constant issue for my belt tension, I'd rather get the parts just to make it operational first then improve its speed with a VESC and design with a better deck at a later date. I can deal with it only going 18.5 until I get new parts as long as it runs smoothly and doesn't have the kind of bs issues the liftboard gives me on a weekly basis.

Oh and anyone have suggestions on the battery enclosures? I've heard good things on psychotiller, enertion had a nice looking enclosure too that he says is water tight, I've also looked at Unik boards and torqueboards for enclosures but would love to get some feedback from people who have used them. The enertion enclosure honestly looks the best to me but I have heard that enertion is awful for shipping things in a timely matter and this makes me seriously re-consider that as an option. Thoughts?
```

---
## \#8 Posted by: Hummie Posted at: 2017-06-14T19:14:21.315Z Reads: 373

```
I have my cleanest joke to try on you. Think I got it from readers digest!
An old Greek lady, young pretty Swiss girl, an Englishman, and an Irish guy are all in one of those cool trains where you sit across from each other in a little compartment with a big nice window on the side.  They go into a black tunnel and you hear a "smack!", and coming out the other side the English guy is clinching his cheek and he's obviously been smacked in the tunnel in the dark!  The old Greek lady figures he must have gropped the young pretty Swiss girl in the dark tunnel and she slapped him.  The young Swiss girl figures he must have tried to grop her but missed and got the old Greek lady and she smacked him.  The Englishman thinks the Irish guy must have gropped the young Swiss girl in the tunnel and she mistakenly thought it was him and that's why he got slapped! And the Irish guy is thinking he can't wait for another dark tunnel to smack that English guy again. 
I used to go watch the open mike for fun around here.  If they're good, then they're pretty good and that's wholesome fun, and when they're bad they die in flames for seven minutes and that's fun to watch too
```

---
## \#9 Posted by: lowGuido Posted at: 2017-06-14T21:56:30.781Z Reads: 401

```
[quote="Lunasi, post:3, topic:25353"]
It's not a rebranded benchwheel
[/quote]
well they sure fooled me....

https://aaboards.com/wp-content/uploads/2017/05/liftboard-single-motor-bottom-e1493692628724.jpg

https://www.electric-skateboard.builders/uploads/db1493/original/2X/b/bf0349105734499d57b4d0a5216297d879734188.jpg

oh wait.. they changed the deck shape and used black wheels. I see it now.

all seriousness though, the motors and drive parts seem like reasonable quality. if you are having trouble with them just fab your own and weld or clamp it on.
personally Id just ditch the ESC and get with a FOCBOX or similar. add more volts. job done.
```

---
## \#10 Posted by: sl33py Posted at: 2017-06-14T22:14:11.652Z Reads: 380

```
[quote="lowGuido, post:9, topic:25353"]
oh wait.. they changed the deck shape and used black wheels. I see it now.

all seriousness though, the motors and drive parts seem like reasonable quality. if you are having trouble with them just fab your own and weld or clamp it on.
personally Id just ditch the ESC and get with a FOCBOX or similar. add more volts. job done.
[/quote]

hehehe - play nice @lowGuido!

@Lunasi - seriously trust us when we say "rebranded" - yes they buy in bulk - from the same place benchweel does.  so tomato tomahto - it's basically the same.  Moving on (not worth the argument and regardless of what they are telling you - same components).  

No stress on VESC/ESC confusion.  Gotta start somewhere - search for some of my old posts...  I was as green as anyone!  Keep asking questions and the group here will help you learn quickly (and spend your $).

So dual motor on it currently, but the mount sucks.  I'd try the obvious blue loctite on every piece to see if you can get it to last at all - otherwise new mounts, and likely new trucks (the mounts are made specifically for a specific set of trucks).  Most common are setup for Caliber II's (44 or my recommended 50*).  

If you swap to dual motors - the biggest motors you can easily fit on Caliber 50's is usually 6355's.  For mounts - besides Enertion, DIYelectricskateboards.com, there are quite a few made by folks here and sold for a lot less $.  I recommend @korryh's mounts - i've used a few of them and one of the better regardless of price.  I'd get the stainless motor mount w/ aluminum clamp.  I think the SS mount is a few $ more, but thinner which can help you squeeze in dual motors.  

If you swap motors you may need new gears for the motors - look for ones with 8mm shafts (some are 10mm and a PITA to find gears or $$ for 10mm gears in comparison).  I'd also confirm the gears on your current wheels are HTD5's and not HTD3 or something else "funky" which could be an issue.

GL!
```

---
## \#11 Posted by: lowGuido Posted at: 2017-06-14T22:36:24.875Z Reads: 326

```
im just having a dig. 
seriously though we are here to help. 
number 1 LOCTITE
number 2 VESC
number 3 more voltage.
```

---
## \#12 Posted by: Lunasi Posted at: 2017-06-15T06:24:50.054Z Reads: 345

```
Trust me I know the loctite game from taking apart my leiftech constantly and learning from the owner Aaron while living near their old factory in NYC. The issue really is their mounts are bunk, I'm friends with Kali NYC (Ernesto) and showed him the board in person when I was living there and he couldn't even help me fix the mount issues and straight up suggested new motor mounts (So I'm not just being a drama queen on this xD).

Okay so everyone has suggested stuff, this is what I'm looking at based on speaking to some of the people at torque boards.

Dual Motor mechanical Kit
63mm motor mount
13T Pulley size (for more torque)
255mm belt
2× 6355 190kv motors
battery enclosure? (make suggestions on favorites please)

Minus the battery enclosure all together should cost me 480, seems like a fair price to me. 5K watts of power for those big hills, I'm kind of in love already before I've even got my paycheck for parts! <3 I know that much power sounds like way too much for some but I want to be able to go freebording and ride something up the
```

---
## \#13 Posted by: Jinra Posted at: 2017-06-15T06:28:50.249Z Reads: 327

```
Don't forget wheel pulley. I'm using the Space Cell Pro enclosure for both my builds and it works great. I'd recommend it if you want a slim easy to use enclosure. Parts look good, just keep in mind that you'll need new trucks as well unless you can find something to fit your benchwheel trucks, which may be kind of hard.
```

---
## \#14 Posted by: lowGuido Posted at: 2017-06-15T06:30:40.778Z Reads: 328

```
my favorite enclosures..
https://www.instagram.com/p/BVJbdutA-3m/
only $2.50
```

---
## \#15 Posted by: Jinra Posted at: 2017-06-15T06:32:13.108Z Reads: 312

```
Do you just use wood screws going straight into the deck? Or do you mount something in the deck for the screw?
```

---
## \#16 Posted by: Lunasi Posted at: 2017-06-15T06:32:29.339Z Reads: 303

```
@lowGuido smart and budget worthy, good thoughts appreciated!

@Jinra The mechanical kit from torque boards comes with the trucks, these should work I assume?
```

---
## \#17 Posted by: Jinra Posted at: 2017-06-15T06:33:52.812Z Reads: 306

```
Ah okay then yea those should work just fine.
```

---
## \#18 Posted by: lowGuido Posted at: 2017-06-15T06:34:20.820Z Reads: 308

```
@Lunasi I use these all the time.. they are sturdy and cheap, they dont look half bad either. 
https://www.instagram.com/p/BULwuFTA-av/
```

---
## \#19 Posted by: Lunasi Posted at: 2017-06-15T06:39:38.507Z Reads: 312

```
No that totally looks decent and leaves me money for marijuana :grin::yum: haha. But on a serious note that space cell pro looks awesome, that's the one I had been looking at. Might end up going the budget route this month on the liftboard to save a dime and then buy the enclosure along with a new deck at a later date, might even save me some money to get a VESC that way. Can anyone suggest a cheap place to find a good VESC? Seems they're all in that hundred dollar range.
```

---
## \#20 Posted by: lowGuido Posted at: 2017-06-15T06:40:59.650Z Reads: 308

```
[quote="Jinra, post:15, topic:25353, full:true"]
Do you just use wood screws going straight into the deck? Or do you mount something in the deck for the screw?
[/quote]

this was directed at me?? yeah I just go straight through the deck with countersunk bolts... I did do one where I put nutserts or "demon nuts" into the wood

@Lunasi unfortunately VESC are not cheap.
```

---
## \#21 Posted by: Jinra Posted at: 2017-06-15T06:43:14.386Z Reads: 274

```
@lowGuido Yea, I'm actually not familiar with how enclosures are commonly mounted to the deck. I drill a hole straight through for the SCP enclosure and use rivet head knurled inserts for the screws, doesn't look as nice though since you see the inserts from the top.

@Lunasi VESCs are going to run you at least $100 each. For American distributors I recommend Ollinboards (a bit pricey) or Axle (https://goaxle.com/shop/). Not sure if Axle is taking orders right now though.
```

---
## \#22 Posted by: Lunasi Posted at: 2017-06-15T06:43:21.123Z Reads: 262

```
So VESC is open source as I understand, what's the big difference with ESC though? Is it like a pre-set speed controller in a way where the settings are already set in and you can't adjust it? Do people ever use ESC's in e-skate besides the companies or is it all VESC?
```

---
## \#23 Posted by: Jinra Posted at: 2017-06-15T06:45:26.151Z Reads: 266

```
People use regular car ESCs all the time for esk8, but they were built with RC cars in mind, not heavy humans. I know lowguido uses the x-car beast ESC in some of his builds and others have used the FVT, but most hobby ESCs have a 6s voltage limit. It's hard to find regular ESCs that support over 6s voltage, though there are some. VESC supports from 4-12s and is customizable in almost any way you can imagine.
```

---
## \#24 Posted by: Lunasi Posted at: 2017-06-15T06:48:08.283Z Reads: 253

```
@jinra Thank you for putting that into lamens <--(who knows if I spelled that right) terms for me! Much easier to understand.
```

---
## \#25 Posted by: Lunasi Posted at: 2017-06-15T07:04:14.689Z Reads: 257

```
What do you guys think, should I sacrifice a single motor the first month and get the VESC and then get the second motor at a later date? Then I can save some $ and do the single motor mechanical kit for the time and afford other parts needed. If I have 5000watts of power but a liftboard esc that only goes 18mph its just going to be a powerfully slow board, eh? <--- I used to live in Canada xD   2500 watts of power and a vesc is still going to be more powerful than my current board (1800 watts, 900 per motor) and with the VESC I should be able to jack up the speed a bit which I'm kind of a speed demon TBH because I used to race go-peds as a teen (had one that went 48mph).

P.S. So glad I posted here, you guys have all been a million times helpful in helping me plot this whole thing out!
```

---
## \#26 Posted by: lowGuido Posted at: 2017-06-15T07:21:40.461Z Reads: 230

```
I think one powerful motor is good enough unless you need real hill climbing torque.
```

---
## \#27 Posted by: Lunasi Posted at: 2017-06-15T18:10:10.583Z Reads: 233

```
For now I think I'll be okay without the super torque of two motors if I get to jack up the speed on the vesc. If I'm only buying one motor to start is it worth while to do something even more powerful like the torque boards 6374 190kv 3150W motor? Or should I just stick with the 6355?
```

---
## \#28 Posted by: Hummie Posted at: 2017-06-15T18:29:31.629Z Reads: 243

```
With your old board claiming 900watts of power each motor that's just a claim as to what the power the motor is CAPABLE of but doesn't mean that when you pull the trigger you're getting it.  The esc and battery decide how much power is put to the motor and I bet it is less that that with what you had. If you really were to use 2000 watts you will be going from 0-30mph in ...maybe 5 seconds is a guess. I was programmed to do 2500 and regardless of what boosted's motor wattage claim is there is no comparison between us  
You need the battery that can put out the amps for it (not hard),  and also no battery discharge limit from the bms if you use one or bypass it, and you need the esc that can do it and is programmed to do it (not hard to do but rarely high numbers possible unless diy)
Tell me if its layman's terms
It's pretty hard to stay at 2000 watt output especially if you're 140lbs unless you're going up hill non-stop.   Me doing a two block hill vs boosted ...they'll be at maybe 2/3 when I'm at top
The Vesc will allow you to program and monitor it all from a pc or your phone. It's worlds better than rc stuff.  Foc program is the best. 
One 63mm motor and Vesc and I think you'll be good and have tons of power and torque

I like this gem and has a great rep and cheap
http://www.hobbypartz.com/96m608-bigfoot160-5335-245kv.html
```

---
## \#29 Posted by: Lunasi Posted at: 2017-06-15T20:31:43.707Z Reads: 239

```
@Hummie All that made sense to me, those motors are actually a great price! I might look at those because every little bit I save is piece I can buy. I might even be able to do the dual motor setup, vesc and afford it all with that. 

Okay as far as batteries I have two options, I can use the 6S4P inside the liftboard and/or I can take apart this LT3X leiftech battery that the wiring got messed up on but it's rated for 24v 144wh (not sure if it's 10s 8s...whatever the rating). I also have a smaller leiftech battery that's rated for about a third of the bigger batteries life. Can I put the two or all 3 together into one big pack? I have a few friends in my local Colorado riding crew I lead who are electrical and mechanical engineers to help me. If I were to do that would I need any parts to put it together? 

On top of that are there any parts or pieces for the board that I haven't thought of? Important pieces that ill need? 

Battery and Enclosure 
Vesc
motors
Dual Motor mechanical Kit 
......? (things missing?)
```

---
## \#30 Posted by: Hummie Posted at: 2017-06-15T21:01:13.037Z Reads: 225

```
Make sure the vescs can do the foc program.  
Mini trigger remote is reliable and cheap.

I don't know about those batteries but you should shoot for 10s or even 12s (if 12 then must limit erpm on Vesc but easy)


U still need a way charge the battery and it can be complicated or easy depending on what way you go.  I much prefer getting a bulk charger that can do huge fast power and a balance discharger on the side.  This is much cheaper and faster but requires being aware of what your cells are at while charging vs doing the whole bms thing or a true balance charger that will do it all. 

If you want to solder you could take apart those batteries you mentioned but otherwise 18650 cylindrical are an obstacle compared to lipo
I'd go with the single tacon160 to see first.  Save bucks

I have remote. Vescs.  A tacon 160 missing bearings, all of which in trying to get out and make bucks to get the parts I need.  And new deck with hole in it. And lots of trucks and kegel wheels
```

---
## \#31 Posted by: ScootThatTrick Posted at: 2017-06-19T11:06:18.861Z Reads: 202

```
So Lunasi, let me get this straight.  You won a free Liftboard and had some issues with it?  I purchased one, and had some issues with it.  I reached out to the Liftboard and found them to be a young company going through some growing pains, but good folks who took great care of me and more than rectified the the problem.  You might want to reach out to them and give them a shot to make things right before calling out their product online (which they gave to you) as a "POS".  Just a thought.  And btw, from everything I've read, they have tightened up the product and are getting a lot of good press.

As for your reverse engineering project of the Liftboard you have going, I am definitely going to stay tuned...  Who knows, you might end up inventing the "Back to the Future" hoverboard we've all been waiting for!  More than likely though, I see some humble pie in your future.
```

---
## \#36 Posted by: sl33py Posted at: 2017-06-21T20:44:24.852Z Reads: 192

```
[quote="ScootThatTrick, post:35, topic:25353"]
Apparently, 7 days ago you called yourself a "noob" when it came to knowing what kind of parts were even on your Liftboard, and now, all of the sudden you're an engineer?   Come on...
[/quote]

And you joined 2 days ago...  So what's your point?  quoting and dismissing statements as @Lunasi is learning and trying to make the liftboard work better - do you work for Liftboard perhaps?

fishy
```

---
## \#37 Posted by: sl33py Posted at: 2017-06-21T20:51:17.995Z Reads: 206

```
@Lunasi - my recommendation if you are on a tight budget - 

Go VESC.  Axle or Ollin are both good, Ollin are top notch but $, Axle great price with improvements over standard BOM 4.12.  DIYes also a good option and less expensive.

Motor - i'd stick to 190/200kv max if you want to move up in voltage later w/o frying DRV on VESC (exceeding 60k ERPM) = for the v4.xx versions.  New VESC Six will not have the 60k erpm limit, but still in beta so not really available yet.  v4 is solid if you keep those erpms down.  Recommend DIYes motors as really nice w/ keyway and well made w/ sensor option if you want.

To save $, i would go with @korryh's mounts, and @Titoxd10001 ' s 15mm gears.  The wider belt will help with a single motor, but may limit you on dual rear setup later - you can add another motor on the front truck.  If you know you are going to go dual rear - 12mm belts and gears from DIYes is another option.

If you are riding in the city with a lot of interference - i'd suggest the GT2b for the most reliable "rock solid" setup.  You can 3d print an enclosure later to make it smaller, but reliability is the critical consideration over looks or even form factor.  I get a lot of drops in Seattle w/ other controllers...

So yeah - i'd go a single motor setup to start, and add another later.

HTH - GL!
```

---
## \#39 Posted by: Lunasi Posted at: 2017-06-22T05:34:27.775Z Reads: 182

```
@sl33py I picked up the torque boards single motor mechanical kit that comes with trucks and everything I need to mount it. I also picked up a single motor and the torque boards vesc. I'm supposed to get the parts Friday and would love to mount it all but I'm not quite sure about the vesc. I'm assuming the liftboard currently has a ESC of some sort so when it comes to installation I have a couple things on my mind. As far as putting this together (motor mounts, motors, trucks) I'm not too worried. With the vesc however I know it's open source and I can adjust all the settings on it. Assumably I replace the current ESC with the vesc but do I have to adjust any settings first? If I just switched it out would it be on some pre-set setting and work well still? Secondly is there some program I need to download that I can easily adjust it from and then how would you connect it to said computer? Anything people can teach me about vesc's would be of the greatest help!
```

---
## \#40 Posted by: sl33py Posted at: 2017-06-22T05:42:34.267Z Reads: 211

```
[quote="Lunasi, post:39, topic:25353"]
If I just switched it out would it be on some pre-set setting and work well still? Secondly is there some program I need to download that I can easily adjust it from and then how would you connect it to said computer? Anything people can teach me about vesc's would be of the greatest help!
[/quote]

No.  If you swap a VESC in without configuring it - best case it won't work.  Worst case you'll damage the VESC.

VESC is open source and a lot of great articles and videos how to do it.  Direct from Benjamin Vedder's site (vedder.se) - he has some youtube videos using Ubuntu Linux w/ copy/paste steps.  You can also find several videos from folks here, and numerous threads.  I'd recommend you look through these and get an idea on how to do the motor detection and configuration to start:
https://www.electric-skateboard.builders/search?q=VESC%20configuration

I'd recommend you stick to BLDC to start - and when you want to try FOC later hopefully you'll understand enough to do it safely without damaging the VESC.

Tons to learn on VESC - when you have a better grasp to ask questions - ask and the experts will give you a hand.  I'm merely passable w/ it, and no expert.

GL!
```

---
## \#41 Posted by: Lunasi Posted at: 2017-06-26T07:33:20.188Z Reads: 228

```
@sl33py @Hummie @lowGuido   

Okay so I started pulling everything apart with my friend who also e-skates and is starting to DIY, boy was that an adventure. It started off simple enough, remove the trucks and take the battery/esc mount off of the board. We soon realized that the piece in the middle is a hollow aluminum tube where all the components have been stuffed inside. So we pulled the battery out and tried to salvage some pieces but honestly the whole setup is a mess. The only thing I might keep is the 6s4P battery from it and maybe put it on a cheap build later on with some a better motor mount and motor. The Bluetooth receiver they use for it was so small there is no way to easily attach it unless do they make pieces that might fit it onto my new VESC? 

So... I started looking at things and did some legwork today to get things started. I have been reading on the vesc and went to an RC car store nearby today to get some components. I'm going to use one of my LT3X batteries from my leiftech. So a couple questions I have while I also expand on some information. The LT3X battery as I understand it is rated at 144Wh 24 volts. From what I have gathered the battery is actually "two" batteries with separate battery management systems in it, one for each motor on the original leiftech board which is why the battery has two xt60 connectors on it. For starters I cant for the life of me get an answer from anyone and haven't been able to speak to the owner of leif lately about whether its 6s4P, 10s2p whatever the friggin number P it is xD. This would help me and my friend helping me build it understand a bit better some of the inputs for programming the vesc. Or maybe I'm just complicating things, is 24 volts 144wh all the info I need to program this thing? Moving on...

The guy at the store is helping me set up a connection I can put inside my board. The LT3X battery has the two xt60 connections mentioned and the vesc has the xt90 connection. I asked him to create a connection where both the xt60's could plug into an xt90 converter for the vesc, but then he's also helping me set up a separate charging port that I can connect from the outside of the enclosure. He's also adding a power switch button to the board. 

Okay so then my final piece to get this thing working this week is the remote. I went in today and surprise surprise all the remotes were gigantic, I should have probably ordered it before but I was hoping to use the Bluetooth remotes from the liftboard and adapt those on. Now I didn't bring the Bluetooth connection into the RC car store today, but the connection was reasonably smaller on the little chip they had and I could visibly see it would not fit the VESC. Does anyone have any idea if I can get a piece to adapt the smaller Bluetooth connection to the bigger connections on the vesc? If not my option two is either wait til the end of the week and order the DIY electric mini remote or buy one of the big honking massive ass remotes they sell in the store. My impatience tells me I want it now, but my riding sense tells me to wait. I have seen the sparkle remotes before and I am wondering as well is that something I can easily buy online or do I have to have a 3D printer? How hard is it really to take a bigger remote apart and mount it inside a smaller compartment? I am the kind of person that is still getting used to buying hardware so I don't like to have to cut things, solder things, or do some of those things if I don't have to xD.

Last thoughts I'm looking at different decks for the build later on. I'm looking at a few loaded decks vs never summers and would love to hear some peoples preferences on different decks and top vs bottom mounted trucks on their electric skateboards. I have ridden a few of my friends bamboos lately and even though I'm used to a stiff deck on my leiftech and the liftboard I think a flexible deck is calling to me. The loaded Bhanghra, Icarus and Dervish Sama are calling out to me. The Neversummer Heist, Deviant, El Jefe, and Superfreak also look good. I want something that's going to be stable but I love that carvy feel which is why I think I'm leaning towards the loaded decks. Thoughts?
```

---
## \#42 Posted by: lowGuido Posted at: 2017-06-26T19:18:04.393Z Reads: 171

```
you can buy a GT2B massive remote and then re house it in a baby buffalo case or similar later.
```

---
## \#43 Posted by: sl33py Posted at: 2017-06-26T20:04:32.034Z Reads: 209

```
[quote="Lunasi, post:41, topic:25353"]
This would help me and my friend helping me build it understand a bit better some of the inputs for programming the vesc. Or maybe I'm just complicating things, is 24 volts 144wh all the info I need to program this thing? Moving on...
[/quote]
You are making it too complicated.  All that matters from a "make it work" perspective is knowing your volts it supplies.  Where parallel and such come into play is their C rating.  How much amperage can they supply?  Also good to know, but if you conservatively test, you should be able to tell if it can supply ample amps or it will run poorly and get hot (bad - stop using).  If you push it even when they get hot - you'll damage the cells, puff them, or otherwise have a bad time.

Looking for the LT3X batteries - can't see specs.  If you have access to ask someone who knows what they are using - great.  It would be good to know before you damage something with over-drawing them.  You could also crack one open and send us the pic.  We should be able to tell you what's going on then.

Let us know or be very cautious so you don't damage expensive batteries!

[quote="Lunasi, post:41, topic:25353"]
Okay so then my final piece to get this thing working this week is the remote. I went in today and surprise surprise all the remotes were gigantic,
[/quote]
Second @lowGuido's suggestion of the GT2b - rock solid.  Get a 3d printed smaller enclosure and move the internals into it.  Save space, but still solid connection even with lots of interference in the city.  BT is usually inconsistent and gets drops.
 
[quote="Lunasi, post:41, topic:25353"]
I'm looking at a few loaded decks vs never summers and would love to hear some peoples preferences on different decks and top vs bottom mounted trucks on their electric skateboards. I have ridden a few of my friends bamboos lately and even though I'm used to a stiff deck on my leiftech and the liftboard I think a flexible deck is calling to me. The loaded Bhanghra, Icarus and Dervish Sama are calling out to me. The Neversummer Heist, Deviant, El Jefe, and Superfreak also look good. I want something that's going to be stable but I love that carvy feel which is why I think I'm leaning towards the loaded decks. Thoughts?
[/quote]

You need to figure out what you like.  I personally like drop decks and drop through drop decks - but they are a PITA to electrify (hub motors a good option).  If you want flex - be prepared to split your enclosure to run batteries on one end and electronics on the other - less room for both so the middle can flex, and a fair bit more work than a regular stiff board you can screw your lunchbox under.

Drop through and drop decks are difficult for motor placement.  You can run the motors outboard behind the deck, and just make sure your mounts clear and everything flexes/turns without hitting.

tip of the iceberg!  GL!
```

---
## \#44 Posted by: Hummie Posted at: 2017-06-26T20:52:30.778Z Reads: 208

```
What button switch is he going to add?<img src="/uploads/db1493/original/3X/8/7/87971618a68ecfe0add3973f9169ed240fe1faff.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/f/5fb4206f8a2163f7530b77dff469cb31321be565.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/f/afe51dd90fe03c3338885204339867928d9e201a.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/1/0/10dd20e4b1df538b790c4865376bb506a0220c1f.jpeg" width="375" height="500">

I like this deck a lot. Drop/drop-thru. W a mount off the back or front u could get really low still.
```

---
## \#45 Posted by: Lunasi Posted at: 2017-06-27T06:31:42.335Z Reads: 213

```
Okay so I decided to be patient and order the mini controller from DIYelectricskateboard and wait til the end of the week to do everything. @Hummie as per the button switch I was asking him to add a power button to power on the vesc and the board but when I went to pick up my stuff today he hadn't added it, I think he was honestly scared to touch my vesc because they're used to all those tiny little RC car esc's. He did however do what I asked him in creating a xt60 to xt90 connection, pairing the two connections to a single connection that goes to the vesc (because the leiftech battery has two batteries inside the single wrapped battery with two separate BMS' keep in mind), and then also off of that leaving me two XT60 connectors I can access from the side of the board to charge it. Here's a picture to show you a bit of what he did with the battery to vesc. Back to the power button switch, like I said he didn't add it, I think he thought his stuff in his shop wouldn't work with it. He suggested going to micro center for a switch as they deal in a ton of computer parts and components and there's one not too far away from me, than sound ideal to everyone else? I have been watching stuff on programming the vesc and quickly realized I needed both a power source and a physical power button to actually turn on the VESC to program it, I also am waiting on the remote so I'm able to do some motor tests before things are properly mounted, all sound good so far? Am I missing anything or am I on the right track here?

<img src="/uploads/db1493/original/3X/b/4/b4bd9108991fc9d8fe5f505ec1d7ce3e1469fc23.jpg" width="366" height="500">
```

---
## \#46 Posted by: Hummie Posted at: 2017-06-27T06:34:50.731Z Reads: 206

```
you can get away with just using your battery as a power source when programing the vesc.  maybe use the half to be safer.   
an on/off switch has to be high power or will break quickly.  I'd just use an xt90s plug and be done.  maybe make an xt90s loop key.
```

---
## \#47 Posted by: Lunasi Posted at: 2017-06-27T06:38:08.578Z Reads: 205

```
@Hummie What do you mean it has to be high power, is there something in particular I should look for in a power switch? You said maybe to just use the XT90's plug and be done but what do you mean by that, can you extrapolate a bit for me? Also what is a loop key? All the advice so far has been incredibly helpful!
```

---
## \#48 Posted by: sl33py Posted at: 2017-06-27T06:43:25.680Z Reads: 206

```
it will spark and you can definitely just plug it in to start.  I always jump when i do it...

A way to eliminate the spark is to use a loop key with a XT90 anti-spark.  Instead of a switch w/ inrush control and complexity/cost (though nice).

A super old how-to i did almost 2 years ago now (damn time flies):
https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

GL!
```

---
## \#49 Posted by: Hummie Posted at: 2017-06-27T06:46:27.902Z Reads: 184

```
switches seem to always break anyway.  

I'd make sure your vescs are totally good and have all the parts and can do foc and a warranty too.  I forget your plan but you could surely get away with one big motor and one vesc.  or i see you already have them
```

---
## \#50 Posted by: Lunasi Posted at: 2017-06-27T06:48:36.112Z Reads: 185

```
How do you set up your battery enclosures so you can access it to plug it in and turn it on easily but also keep the water out of your compartment?

Also the XT90 anti-spark plugs I'm reading about, should I have them switch out the connections to those? Are you guys basically suggesting that to start the board each time I just plug in the XT90 connector to the vesc to turn it on with an anti-spark XT90 plug? From what I read on the loop keys it looks like its just a simple connection with a button on it. I am definitely not the most technically minded, do they make XT90 loop keys with those little buttons on them? The button seems much more convenient to hide than that big wire connection.
```

---
## \#51 Posted by: Hummie Posted at: 2017-06-27T06:58:43.040Z Reads: 175

```
 you could use silicone in a tube and coat things but I've never done it and don't like riding in the rain.   my stuffs still just held together under the board with duct tape still and using an xt90s and it's ugly but performs.    I have a bunch of extra tape all over the deck for the future.  very ghetto but beats wasting time for me and I've yet to read of a switch or even a bms I'd want to use.
```

---
## \#52 Posted by: Lunasi Posted at: 2017-06-27T07:12:20.983Z Reads: 177

```
Okay watched some stuff and got a good idea of what a loop key connection looks like, my question now can I use a loop key anti-spark connection like that to power on the vesc to program it? I would assume yes but I feel kind of like a ditz here trying to figure this all out. If I set up a loop key connection like that all I have to do is plug in the little key and it will turn on? Does the connection on the looped part just send an on signal to the wires basically without having to have a physical power switch? How vital is it that I get the anti-spark stuff too? On my leiftech when I plug in the battery I plug in two xt60 connections to power on the PCB board, they don't look like they have anti-spark on them and they make a sparking sound when you plug them in which I always just assumed was normal. Is that sparking sound bad for the VESC somehow and that's why I want the anti-spark connectors instead?
```

---
## \#53 Posted by: Hummie Posted at: 2017-06-27T07:43:54.528Z Reads: 177

```
the spark isn't a big deal and will just mess up the connectors.  the loop key just makes a complete circuit as if you'd plugged in your battery it just has the little loop making the circle complete.  if the vesc gets connected to the battery it's on.  the bigger the voltage the bigger the spark.  id just use an xt90s plug and be done.  it sounds like you were doing the same anyway just without the antispark feature.   supposedly not bad for the vesc.  maybe a bit rough on the capacitors that lead to the vesc as they instantly take up the voltage and charge up but ...that's splitting hairs and caps last a very long time.   some people chose not to use an antispark as then, when they don't get a spark, they know the big capacitors aren't working and that will ruin the vesc quickly.
```

---
## \#54 Posted by: wafflejock Posted at: 2017-06-27T17:17:35.817Z Reads: 184

```
The spark just depends on the voltage you're running.  Like @sl33py mentioned there is a large inrush of current that happens when the connection from the battery goes into the capacitors attached to the VESC, the caps can take in a lot of current really fast and if the voltage is high enough it will be able to jump across the air a tiny bit and just as the connectors come near contact there can be a big spark. 

With regular XT-90s you're fine with lower voltages but when I started messing with 12S and now using 10S it became necessary to have some sort of antispark otherwise I was burning up the contacts on the XT-90s with the sparks.  Like others said here already though if it isn't causing you problems a little spark won't fry the VESC (even the big ones I was getting just fried the connectors).

Having a loop key (anti-spark plug with a loop) is still a nice thing to have though it's a simple way to completely open the circuit if anything ever goes haywire and cuts the batteries from the rest of the electronics so the whole thing is basically guaranteed to shutdown (as soon as the caps drain, basically immediately).

I'm working on redesigning my battery pack right now I'm going to see if I can design a shell to wrap the 5S LiPo batteries that can be locked in tightly but easily be removed.... with XT-90s on the hard shell surrounding the battery... basically like a network attached storage drive bay but for batteries.  Currently the battery box I have just has 3 XT-90 female jacks sticking out of it for charging the two batteries and the third for the loop key but it's a bit dangerous since if the loop key goes in the wrong jack it quickly becomes an expensive not very effective little bomb (redesign will take care of this issue too).
```

---
## \#55 Posted by: Lunasi Posted at: 2017-06-29T06:24:10.982Z Reads: 181

```
@wafflejock 

Okay so I have an anti-spark xt-90 plug coming in the mail now, my friend told me he would help me solder the loop key from it so that's one check down, just gotta wait a week for the part. Waiting on the remote at the end of the week and then I should have roughly all my components together. The only thing I'm missing is my battery enclosure still which I'm still looking for a cheap solution, just haven't found what I want at the local stores I've checked yet, gotta keep looking. Can I make some holes on my enclosure to make it easily accessible and run it without the loop key in the meantime? I might buy two of whatever I get for an enclosure and close it up more when I get the piece for the loop key if so, then I could be riding this weekend theoretically which I am very much YES to. 

Secondly if you look at my photo I posted I had them rig up a xt60 connector piece where the battery can be plugged in from the outside with separate xt-60 connectors that go outwards for charging. My question is could I get a big battery compartment and theoretically put "two" of my 7s3p leif batteries in it using those connectors? I'd have to put on double risers but I would get a ton of extra power from it, and my leiftech is waiting on some parts currently so using the batteries in-between paychecks until I can afford a 12s4p is no big deal. Thoughts?

Edit Note: People have been asking about the Leif battery, turns out it's 7S3P.
```

---
## \#56 Posted by: wafflejock Posted at: 2017-06-30T00:57:53.497Z Reads: 196

```
Yeah regarding the enclosure you can just put a hole in the side of it for running the two silicon cables from the battery(ies) to wherever you put the VESC (somewhere near the motor).  When I was starting my first build I just used some XT-90 connectors to make a Y cable that would hook the batteries up in series like you can see below (I just ordered a handful of XT-90 male and female connectors at some point).

http://rcmodelparts.co.uk/product/xt90-series-y-harness-lead-cable-2-batteries-series-splitter-lipo-uk

The male connector in the picture with the red and black goes to the VESC you could have this cable inside the box with your batteries and then just the cable that plugs into that red and black connection comes out of the enclosure and goes to the VESC.  I just replaced one of the connectors on my battery with the anti-spark one so I'd just hook up the regular battery first then the anti-spark one second (you want to have the antispark one be the last thing you connect to complete the circuit it can't just be in there).

Regarding skipping on the loop key and anti-spark plug, I'd say the no anti-spark is fine, the no loop key is also okay, but really good to have the loop key on there in some way you can grab it and pull it in case things go haywire at least you can cut off the power.  So ya know, it's all up to you really on what you do, personally started without a loop key too, but I find it to give me quite a bit of peace of mind that if the board goes crazy at least I can cut it off.

My board has three connectors sticking out like you're describing and I cut the silicon wires that come off the batteries to give me leads that go to the VESC (regular leads go into the connectors for charging and stick out the side of my enclosure).

https://raw.githubusercontent.com/shusain/eskatecontroller/master/Images/IMG_20170420_203124.jpg

When I plug the loop key into the center connector that completes the circuit and for charging I just use the left and right connector separately.  The danger here is if i accidentally plugged the loop key into one of the batteries I'm just shorting it out (again expensive crappy bomb).  I'm reworking the 3D designs and prints right now on this so I can have trays that I can pop in and out just to make it easier to carry a couple extra batteries and swap on the go plus extra bit of safety if I can pull the batteries off the board quickly.  In the redesign I'm going to have the shells around the individual 5S 5Ah batteries with the male XT-90 sticking out and will plug into the female port that will connect everything.... basically what it is right now but flip the two outward facing ports inward and then I just slide the cells out to charge... it's overcomplicated and extra paranoid, but I like it that way :slight_smile:

---
**Additionally**
Since you've got 7S you'd probably want a parallel cable I imagine to just get more Ah out of the whole thing not more Voltage so you'd want to do a parallel style connector between the cables not the series one I linked above.

---

Other pics of my board here, not sure if they'll help though since there's some voodoo going on under the enclosure I didn't really document here yet:

https://github.com/shusain/eskatecontroller

Ignore the white loop around the cables coming from the battery to the ESC but might help give you a better idea, I've actually got the guts all open right now so I'll get some pictures of that too and put them on the github later.
```

---
## \#57 Posted by: Lunasi Posted at: 2017-06-30T03:46:44.475Z Reads: 173

```
@wafflejock 
So that's awesome and probably close to what my zombie will look like, at least it will perform better! Not sure my friends can help tomorrow and I can't bare my excitement to get this thing moving. I get the remote probably early afternoon and then I can set up the vesc finally. I'm sticking to bldc until I'm more experienced. Knowing what I know about the battery being 7s3p, 24v, 144wh are there any values ill need to plug into to bldc tool for those values? I have the 190kw motor but I can auto detect the motor settings in the program correct? I wanna make sure I don't do anything too serious without having an idea what I'm setting up.
```

---
## \#58 Posted by: Lunasi Posted at: 2017-07-01T01:34:34.900Z Reads: 160

```
@Jinra @Hummie @sl33py @wafflejock @lowGuido     

I'm trying to hook up my vesc and do a bench test, I hooked everything up like in the videos but when I power it on the vesc light stays flashing pink to blue instead of going solid blue, when I try to connect in BLDC tool it won't connect there either. Can't figure out what I'm doing wrong here, xD help please!
```

---
## \#59 Posted by: wafflejock Posted at: 2017-07-01T01:36:42.938Z Reads: 157

```
After plugging in the VESC and trying to hit connect give it a few seconds and hit connect again a few times, occasionally I have issues with the serial connection not being immediately available.  Not sure about the constant flashing though haven't seen that one.

---

Did some quick googling looks like it might be the DRV chip got blown somehow or was defective but if you can get a connection to the VESC in the BLDC-tool it should give an error code that would help to narrow it down.
```

---
## \#60 Posted by: Lunasi Posted at: 2017-07-01T01:43:37.280Z Reads: 150

```
Can't get a connection, when I click connect it says "no firmware read response" and then says disconnected, but when I plug in the USB my computer recognizes something has been plugged in. Knew this was gonna be the pain in the butt part xD
```

---
## \#61 Posted by: wafflejock Posted at: 2017-07-01T02:42:18.236Z Reads: 162

```
Some clues here maybe http://www.electric-skateboard.builders/t/vesc-does-not-connect-or-stay-connected-on-ubuntu-or-windows/803/4 (maybe com port conflicts or something) and yeah the software is a mixed bag, can be a pain to get things to connect if they aren't working 100% or just have weird config things different computer to computer so can always take some finagling to get it connected on the plus side once you get it working the software gives you a ton of info about what's going on with your hardware (once you figure out how to understand it).  Hopefully nothing major with the flashing LED issue.
```

---
## \#62 Posted by: wafflejock Posted at: 2017-07-01T04:10:59.914Z Reads: 165

```
Any luck yet?  You may also want to try a different USB cable or port some cables and vescs have been finicky on me with regard to the cable too.
```

---
## \#63 Posted by: Lunasi Posted at: 2017-07-01T04:30:18.098Z Reads: 161

```
I'm out chilling with some friends at the moment but I'm gonna try putting fresh eyes and try Apple vs my PC with it in the morning, see if any better results.
```

---
## \#64 Posted by: Lunasi Posted at: 2017-07-01T20:46:49.112Z Reads: 160

```
Tried the apple computer today, same results. VESC continues to blink blue to pink, remote shows pairing, computer shows there is a USB device inserted but can't connect it and can't control it, it honestly is very much the same as in this video https://www.youtube.com/watch?v=2L82ARqBDAk waiting for Dexter to get back in today for some support with it.
```

---
## \#65 Posted by: Jinra Posted at: 2017-07-01T20:50:50.316Z Reads: 154

```
Have you tried a different cable?
```

---
## \#66 Posted by: Lunasi Posted at: 2017-07-01T20:52:05.064Z Reads: 140

```
Like a different USB cord? I only have the brand new one I bought with the motor and the kit, its not like a micro USB its one of those strange off brand mini USB to USB connections.
```

---
## \#67 Posted by: Jinra Posted at: 2017-07-01T20:53:01.198Z Reads: 139

```
Yea some cables only have pins for power, but not data. If it came with your VESC though, it should work.
```

---
## \#68 Posted by: Lunasi Posted at: 2017-07-01T20:58:55.798Z Reads: 149

```
I'm hoping its either that I'm a complete numb skull or its just some defect and it has to be replaced. I'm good with computers so this shouldn't be that hard to figure out, I'm so eager to ride my board, its just sitting here 80% of the way done and I can't ride it.... scrooge mc duck!
```

---
## \#69 Posted by: Lunasi Posted at: 2017-07-03T03:21:43.059Z Reads: 148

```
Sending it back in for them to take a look at the VESC and make sure there's not an issue. Guess we'll see what happens. Hoping I'm not being a clutz and missing something important. I followed literally everything Dexter told me to do though so I'm hoping this isn't just user error.
```

---
## \#70 Posted by: Schulerbible Posted at: 2017-07-03T06:04:35.908Z Reads: 143

```
Other question, how do you change the belt tension with these Boosted cloned motor mounts? Can't see any slotted holes in the pictures lowGuido posted a while ago ...
```

---
## \#71 Posted by: Lunasi Posted at: 2017-07-05T05:34:43.782Z Reads: 164

```
@Schulerbible good question! I actually posted about it earlier but this is a big post so its easy to lose it in all of this. So as I pointed out earlier there really is no way to adjust the motor mounts, and if you go to their website it even states that. I've gone through a single motor and two duals that were all sent to me for free and the first board worked great for like 2 weeks and then the belt wore and snapped, I messaged the owner and he sent me a free pack of belts and overnighted it. Sounds great right? So I put the new belt on the next day and the belt tension is totally out of whack and has no tension at all. I message them and they send me more belts saying that maybe the belts are wrong, I get the belts and they're the same size belts again xD. So I'm living in NYC at the time and figure, I'll go over to Kaly NYC and ask him what to do, he knows electric boards inside out. I head over to his place and show him the board and ask him what I can do and he looks over it and messes around and says "well you can't adjust the motor mounts at all on this, you need new motor mounts." So I send the thing into them and their final reply on it is that it was missing a screw in the mount... So finally they send me a dual motor board to replace it for the issues, that one gets to me, runs great for a week or so and then I hit a tiny little puddle and it kills something in the board, I'm assuming the water got into their badly placed charge port, none the less that it was a 90 degree sunny and hot day out and this was a tiny skid of water. So they send me another board and within I'd say 4 days one of the belts started to lose tension, I went to replace the belt and once again once replaced it had no tension at all. I inquired to liftboard and they had the gaul to say that a screw must be missing from the motor mount once again. I have one working motor on one side "with" tension and one on the other "without" tension and both have all the same screws in them, down to the set screws. So I tell them they're wrong and there are no screws missing, finally a guy acknowledges the fact that their mounts can become lose over a period of time and you have to move them back into place. Okay so that would be easy peasy if you had a motor mount that one could adjust but they don't, and secondly they even glue the motor mounts to the trucks so you CANNOT physically move them if you wanted to. All in all the liftboard has been a painful process for me but its taught me a lot about the quality that one puts in and gets out of a product and has inspired me to take the broken pieces and put them back together into something better. That said I have even spoken to the owner once at least in an email and told him that his motor mounts are a major issue that needs to be addressed. The Liftboard actually performs amazingly well out of the box but it has real issues that appear with hard riding and commuting like I do. Personally I think if they upped the quality of their deck, got a real enclosure instead of that aluminum monster, upped the speed to at least 22mph, had adjustable motor mounts, waterproof if not water resistance, a little bit better battery, higher quality remote and made the wheels interchangeable and could keep it at $700 and below they'd be able to compete with a company like boosted or some of the other top names. For now though in my honest opinion from riding a leiftech regularly which is already a kind of touchy board, my leiftech doesn't even compare in the problems it has in comparison, its mostly things that can be avoided with regular maintenance. The liftboard on the other hand to me has major flaws which appear fast to the avid rider but maybe a bit slower to the casual rider, which lets be honest if you're in the $500 e-skate market you generally are a casual rider just getting into the sport and maybe not riding the board as hard as others. If I was rating it on only my first 3 days of riding and was only judging price vs performance I'd give it at least an 8 out of 10. If I was judging the board on its overall flaws that appear vs price, performance and other specs I'd probably put it at a 4, which is where it is as a low/mid market board.
```

---
## \#73 Posted by: Bensaida Posted at: 2017-07-08T20:57:25.182Z Reads: 132

```
Motor mounts arent glued to the trucks
```

---
## \#74 Posted by: Lunasi Posted at: 2017-07-08T21:47:16.618Z Reads: 135

```
They most definitely are glued down they even told me they were, none the less that I've actually taken the board apart and seen that they are and you've really only ridden it.
```

---
## \#76 Posted by: Bensaida Posted at: 2017-07-08T21:59:49.745Z Reads: 139

```
I disassembled my board as well, since the motor mount was becoming loose, and i used an allen wrench to tighten the motor mounts. I am pretty sure the mounts arent glued. However, the motors are glued to the mount.
```

---
## \#77 Posted by: Lunasi Posted at: 2017-08-19T04:45:09.008Z Reads: 136

```
@Jinra @Hummie @sl33py @wafflejock @lowGuido 

Okay so I have been sitting on this for a while because I wanted to do this right. I bought a 12s4p battery from torque boards that comes with the enclosure and I'm at the very end point basically where all I need to do is program the vesc. I had this issue before when I first received it earlier where it wasn't connecting to the computer. I sent it in for them to look at it and they never said anything about it and sent it back like 2 weeks later. I got the 12s4p earlier this week and went to program it all. The VESC still wont connect and the torque boards guys said try a different computer or cord. So I have tried 3 different cords, 3 computers and my android phone and none can connect to the VESC. I'm starting to think they didn't look at my VESC at all and just sent it back. When I plug it in the motor responds to my remote and flashes blue the right way but I never get a connection in the program on my computer. 

So I'm at the point now where I want this thing to work and I have a couple options and wanted to know peoples thoughts. First things first is that I feel I need to send this VESC in again because I have put multiple variables in now and I know it is not my computers or the cords. Either way I'm buying another vesc in the future for an eventual dual motor so I could have him overnight a new controller while the other gets fixed.

Option two, send in the current controller and order a VESC from another company such as Ollin board or Trampa with built in heat sink. These seem like much higher quality VESC's but I want to know what peoples opinions are on this. I just don't want to waste my time again on a VESC that can't even do the most important thing, connect to a computer so so its even of use.

I really want this done soon, but I want this done right, I also don't want to dick around with different cords and computers anymore either when it should just plug and play. What would you guys do here?
```

---
## \#78 Posted by: lowGuido Posted at: 2017-08-19T04:47:34.153Z Reads: 128

```
have you made sure you are connecting to the correct com port in device manager?
```

---
## \#79 Posted by: Lunasi Posted at: 2017-08-19T04:48:18.831Z Reads: 123

```
The only thing I see is COM 1 for a port option on it
```

---
## \#80 Posted by: lowGuido Posted at: 2017-08-19T04:50:02.701Z Reads: 126

```
you using windows?
```

---
## \#81 Posted by: Lunasi Posted at: 2017-08-19T04:51:19.191Z Reads: 125

```
At least on my main computer, the other computers I used had all these Bluetooth ports and stuff but I honestly am a little bit lost with what to do. I've watched a bunch of the videos and it seems so simple, I've been trouble shooting this for a while now and I feel like I should be on track. :-/ I swear everything makes such perfect sense to me so I feel like the VESC shouldn't be that hard
```

---
## \#82 Posted by: Lunasi Posted at: 2017-08-19T04:51:49.535Z Reads: 124

```
I've tried on windows (main computer) and two apples plus my android phone
```

---
## \#83 Posted by: Lunasi Posted at: 2017-08-19T04:52:54.901Z Reads: 127

```
Android phone notes that theres a connection but it says "weak connection" my windows computer also has trouble programming the USB. It also recognizes that there is a USB plugged in but it for some reason runs on issues reading it
```

---
## \#84 Posted by: lowGuido Posted at: 2017-08-19T04:52:58.811Z Reads: 126

```
connect VESC to USB and then press windows key and break. thenclick device manager and look at ports.
it should tell you what com port it is. mine is usualy 3 or 4. then got to the BLDC tool and change com to that number.. just type it in if it wont let you select it.
```

---
## \#85 Posted by: Lunasi Posted at: 2017-08-19T04:59:39.833Z Reads: 119

```
Comes up as unknown device
```

---
## \#86 Posted by: Lunasi Posted at: 2017-08-19T05:00:07.069Z Reads: 113

```
Drivers say up to date
```

---
## \#87 Posted by: Lunasi Posted at: 2017-08-19T05:00:42.593Z Reads: 116

```
"Device Status" Windows has stopped this device because it has reported problems. (Code 43)
```

---
## \#88 Posted by: lowGuido Posted at: 2017-08-19T05:04:05.738Z Reads: 115

```
well I dont know what is causing that, but it's fair to say that is why your VESC isnt talking to compy.
do both say that error??
```

---
## \#89 Posted by: Lunasi Posted at: 2017-08-19T05:05:35.209Z Reads: 123

```
Yeah it seems like I'm getting an error no matter the device or cord used for it, that's why I wondered if you guys thought it was better to go with a different company besides torque boards for VESC? I know they're all based off the same open source stuff but I assume there are differences depending on who's made them. What do you think as far as that?
```

---
## \#90 Posted by: lowGuido Posted at: 2017-08-19T05:08:42.563Z Reads: 121

```
I have used enertion and ollin VESC's and have never had issues with either.. having said that I have also never shorted the outputs. i feel that no matter who made the VESC, an output short would kill it.
```

---
## \#91 Posted by: Jinra Posted at: 2017-08-19T05:09:00.392Z Reads: 122

```
Ollin and Axle are my go to's. They've proven to be pretty high quality. Sure sounds like a VESC issue.
```

---
## \#92 Posted by: Lunasi Posted at: 2017-08-19T05:10:07.502Z Reads: 117

```
Would you go with the basic VESC or the heat sink from Ollin? I want to make sure it will fit in the 12s4p compartment, is the heat sink piece that big on it?
```

---
## \#93 Posted by: Jinra Posted at: 2017-08-19T05:11:04.646Z Reads: 125

```
Any of chaka's VESC would be fine, even one without the heat sink.
```

---
## \#94 Posted by: Blasto Posted at: 2017-08-19T05:19:08.460Z Reads: 132

```
Stm32 driver link

https://www.dropbox.com/s/9x6j2eb8thg6t30/en.stsw-stm32102.zip?dl=0

Update driver manually, point towards the stm32 folder
```

---
## \#95 Posted by: Lunasi Posted at: 2017-08-19T05:28:30.097Z Reads: 134

```
Didn't fix it, same error
```

---
## \#96 Posted by: Blasto Posted at: 2017-08-19T05:37:55.844Z Reads: 139

```
Are you able to snap a hirez pic like this, to see if there's anything funky with these two resistors

<img src="/uploads/db1493/original/3X/c/1/c17932601fa68a5525aa532105affdc06d531895.PNG" width="281" height="500">
```

---
## \#97 Posted by: Hummie Posted at: 2017-08-19T05:41:11.450Z Reads: 127

```
on the top right of the bldc tool does it give you options of different numbers you can chose to connect.  don't know the lingo but I have to chose the right number.  plug in the vesc then refresh the list then chose it.  think it's 3 or 4
```

---
## \#98 Posted by: torqueboards Posted at: 2017-08-19T06:01:54.532Z Reads: 125

```
@Lunasi - You can send me an email dexter@ I can see if I can help.
```

---
## \#99 Posted by: Lunasi Posted at: 2017-08-19T12:58:11.080Z Reads: 120

```
@torqueboards thanks for the reply Dex. I'll message you on your chat support when I'm off work today.
```

---
## \#100 Posted by: wafflejock Posted at: 2017-08-19T18:00:47.295Z Reads: 133

```
Regarding various VESCs there are some small variations on component choices between different manufacturers and different runs will have different problems I'm sure depending on the machines putting the boards together and available components at the time and all (think some capacitors or resistors or whatever can be changed as long as they have roughly the same values or are within the same tolerance they might be sourced from one manufacturer or another).  Basically long way to say it's a bit of a crap shoot but in general haven't seen this particular issue come up really at all.  I've heard maytech VESCs have some issues I think particularly with doing FOC at all but if you plan to use hall sensors for the motors and FOC mode for smoother acceleration then there is the FOCbox or VESC6 that both seem to be solid for that.

Regarding the connection to the computer it sounds like you're checking the right places in windows but I've just abandoned windows and moved over to Linux about 4 or 5 years ago so doing advanced debugging in there is a bit beyond me at this point.  You can try checking the event viewer to see if there's anything in the application (or other) logs related to the bldc process or that happens when you try to connect the VESC to the computer but hard to say without being there or having hands on it.

If you want to give it a go from linux you can just run ubuntu off a flash drive without installing it completely and could try from there:

https://www.ubuntu.com/download/desktop
https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-windows#0

From in linux you can use the `dmesg` command in a terminal to see information about any devices plugged in and unplugged, can also use `lsusb` to list usb devices.  If those seemed to show everything okay and no errors coming from dmesg after you plug in the board then you should be good to install and use the BLDC tool (dmesg should show that it saw a new device and the system gave it some id or should tell you if something went wrong trying to talk to the new device and that error should lead to more info).

If you decide not to do that would just do as you're doing work with support and get it exchanged or try another vendor.
```

---
## \#101 Posted by: Lunasi Posted at: 2017-08-20T14:01:47.253Z Reads: 116

```
So I talked to Dexter yesterday and still can't fix the driver issue but found out the motor and his battery I bought are already pre-loaded on that VESC as it's base setting. That means for the time I can ride and I've got ample time in the future to work out my computer issues. :slight_smile:
```

---
## \#102 Posted by: hornet90 Posted at: 2017-08-21T18:16:20.836Z Reads: 118

```
Im irish i love the uk and the people but thats funny
```

---
## \#103 Posted by: sl33py Posted at: 2017-08-22T18:14:14.764Z Reads: 120

```
If you have it working - great, but i bet there is something up with the versions you are running in windows vs the firmware on the VESC.  They are really picky.  I've found the easiest way to do it is via Linux following Ben's instructions step by step.

OR EVEN BETTER - The new VESC Tool is F'ing awesome.  Wizard driven and simple, plus on Windows (I'm a linux noob, so much easier for me).  I've programmed 7 or 8 VESC's now w/ the new VESC Tool.  It's supposed to be out "any minute" to everyone and works fantastic with 4.xx hardware.  I'm one of the Beta folks with VESC Six, so that's how i got it early.  

Not sure if it's out yet, but i'd check here frequently - i'll also look on the forums there to see any ETA if known:
http://vesc-project.com/vesc_tool

HTH - GL!
```

---
## \#104 Posted by: hornet90 Posted at: 2017-08-23T05:09:12.089Z Reads: 122

```
Post pics of what your doing
```

---
## \#105 Posted by: Lunasi Posted at: 2017-08-23T18:42:33.453Z Reads: 119

```
I'll be posting more soon, I have it all together now but I hated the deck and went to swap it. I got a loaded Poke deck instead of the awful liftboard particle board thing I started with but the torque boards enclosure really hates the shape of that deck. I also need to sandwich the components together a bit more to fit the deck. Waiting on my next paycheck and I think I'm going to go to a 3D printer place and have them make me a custom enclosure. For the bit I've rode it though this thing is a friggin rocket. I went for the extra torque gearing and if I'm moving already boy does this thing climb even the steepest hills! I'll post more pics when finished, hate showing a picture of an unfinished product. With the deck change this thing is now 100% not a liftboard and I couldn't be happier!
```

---
## \#106 Posted by: Hummie Posted at: 2017-08-23T18:45:13.794Z Reads: 119

```
custom enclosure from a 3d print?  expensive for a one-time thing.  if anything use the print for a mold and then you have  huge variability of materials to make it with and it can be done many times.
```

---
## \#107 Posted by: hornet90 Posted at: 2017-08-23T21:10:20.344Z Reads: 122

```
Dont waste your money doing that heres a link
https://psychotiller.com

Ill be sure theres one there for you if not email him 
He will get you sorted im sure
```

---
## \#108 Posted by: Tampaesk8er Posted at: 2017-08-25T18:44:15.729Z Reads: 112

```
They so cheap, they are selling them here at Walmart & Sams Club in Tampa, the Liftboard brand is trying really hard to sell them so they trying to sell them in dept. stores, I know someone who bought one and returned it back to Sams Club, to many glitches.
```

---
## \#110 Posted by: Lunasi Posted at: 2017-10-03T04:47:48.015Z Reads: 92

```
<img src="/uploads/db1493/original/3X/7/3/73b4184e39034db2e227a19e527a1012b09a1d4b.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/7/b76840e6afd34a4fc65b3129717e87e8be3a72ad.jpg" width="374" height="500">
Finally finished board on the Bustin' Maestro 39" deck, waiting for the 97mm abecs this week for the final touch, 90mm torque board wheels for now. ^.^
```

---
## \#111 Posted by: Lunasi Posted at: 2017-10-04T07:02:44.879Z Reads: 81

```
Whew just took it for the first ride today, what a massive improvement from that loaded Poke deck I first tried. The ride quality was just so smooth, the bamboo deck definitely absorbs the cracks much better, while not being overly flexible like a vanguard deck. By far one of the most comfy boards I've ridden, very happy with the completed vision! Thanks to @torqueboards for their awesome site and parts to make this beast!!
```

---
## \#112 Posted by: LOSI Posted at: 2019-03-04T14:03:04.823Z Reads: 26

```
Do you still have a good liftboard battery?  I need one for my dual setup and got screwed buying board second hand with lies. Only get about a mile out of it then dead.  Please contact me at strongislandguy@yahoo.com

Thank you
Joey
```

---
