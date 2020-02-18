# My first project, some beginner questions

### Replies: 23 Views: 2184

## \#1 Posted by: seantjaeger Posted at: 2017-01-30T22:09:21.995Z Reads: 198

```
Hey everyone. This is my first post here (as stated), and i'd like to get some input from other on my current ideas.

My goal is approximately 25-30mph max and decent run time (a few miles maybe?) anything achievable with a beginner setup.

**The board itself:**
For my first build I'm on a relatively tight budget like most others, so i'll be using the pre existing step that I have on my current longboard.

Sector 9 42 inch deck, bamboo drop thru
Orangatang Kegel 80mm wheels
Bones Red Ceramic bearings
Gullwing Sidewinder trucks

I'm not sure how important that info is, but I figured i'd include it just in case
Now onto the build...

For my board I'm looking to use an [Alien 190kV motor](http://alienpowersystem.com/shop/brushless-motors/alien-6355-sensored-outrunner-brushless-motor-190kv-2200w/) or  an [Alien 170kV motor](http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-170kv-3200w/). This brings me to my first question: What would the difference be between a 2200w 190kV motor and the 3200w 170kV motor be? I understand the difference in wattage and kV, but do not understand how big the difference will be. Would the 170 be better due to the higher wattage? Or could the 190 be better due to the higher kV? Any info would help.

For the mount/clamp, I will be using [this one](http://alienpowersystem.com/product-category/brushless-motors/63mm/), the Alien Drive universal mount with the 9mm belt and the 63mm version. I will be using the Paris truck type option being that I believe this will be the closest to the sidewinder hangers. If anyone else thinks otherwise please say so.

Now for my batteries... This is where I'm slightly stumped. Im leaning towards a 9-10s lipo setup, but I would like to use multiple lipos in series. I currently have an 11.1v 3s lipo with 35c discharge and 5500mAh. Would I be able to use this in my setup at all, perhaps by getting more lipos of similar stats? Also would it truly be that much better running a 10s setup over a 9s? What I was thinking was getting 2 more 3s lipos and wiring all 3 in series to make it a 9s setup. Is there another way that would be easier regarding theses batteries and getting a 9/10s setup? This is mostly due to my budget restrictions by the way. Any help with that will be greatly appreciated.

For an esc, I would like some suggestions on a relatively cheap one, I will upgrade later though if necessary. This also goes for a BMS, being that I heard they help a lot in charging multiple lipo batteries at once while also helping your circuit in general. Some input on this would be helpful if possible.

I think that pretty much completes it. if you guys wouldn't mind saying if I missed something or perhaps a change (important or minuscule) that would be great.

I hope this is relatively easy to understand, being that i'm only 15 (young compared to most people who build it seems) and have only some knowledge on electrical wiring and other things relating to that. If you have any questions for me, i'll see if I can answer them. Thank you all so much for this forum, I have already learned a lot in just the 2 weeks I have explored it for.

Hope I didn't go overkill on this!
-Sean :slight_smile:
```

---
## \#2 Posted by: sl33py Posted at: 2017-01-31T00:35:37.613Z Reads: 174

```
Welcome Sean!

A couple of the basic questions - 
How heavy are you?  Being 15 i'd assume pretty light... but let us know so we can give you good advice.
Hills in your area you want to ride up, or on the flats?
Where are you located?

Have you looked at any of the gear calculators?  When you want to see the difference in voltages and gearing - invaluable to help determine your target top speed (give or take a bit).  I usually aim for 25mph and it's ridiculously fast on a esk8 IMO.  

Personally, if i were to do it from scratch again - i would stick to caliber II clamps exclusively.  I ran an old v1 ADS motor mount and fought with it from day 1 to not rotate and grind the mount along the ground... YMMV, but i'd stick to Calibers as the "keyed" profile prevents rotation.  Then get either the DIYes or Enertion mount.  Get your gears at the same time - be aware the Enertion Wheel gear require you to cut your hanger back to fit, or buy their trucks to match.  I personally prefer the DIYes wheel gears as they are aluminum.

Even light i would go 12-15mm wide belts on a single motor setup - less likely to skip under hard acceleration/braking, and more leeway to run belt looser without skipping too.  (over tight is bad).

Batteries - i would only select batteries when you know what ESC you are getting.  VESC or similar - 10s is a definite "sweet spot" IMO.  I would not mix packs if you can help it.  they will likely have a different discharge rate and you don't want to over-discharge a pack.

on a budget i'd skip BMS and get a decent starter charger like the iMax B6ACV2.  Slow, but good.  Avoid the clones.


One of my favorite setups:

83mm wheels (Flywheels or clones), 190kv (want to try the 170kv's), 14/36 or 14/40 (motor / wheel gear # teeth):
25mph and 22mph (14/36 and 14/40 respectively).  You could go 15/36 if you wanted faster, but you sacrifice acceleration and hill climbing.  That would get you ~27mph.

HTH - GL!
```

---
## \#3 Posted by: seantjaeger Posted at: 2017-01-31T00:54:00.940Z Reads: 148

```
Agh I knew I was forgetting something!!

I live on Long Island so not many hills at all if any, pretty much just flat streets with some slight uphill/downhill every now and then. I weigh around 115, so not much for the motor to push really.

As for the gears I was looking at a 32T Hub gear with a 15 or 16T motor gear. This was calculated around 27mph max which sounds like a very nice speed. What are your opinions on that?

With the trucks/wheels, I really do like the way my sidewinders ride right now. Also with my deck being a drop thru, they keep it more elevated. How are the calibers for carving/free riding? Also i think for now I may just stick with the kegels due to my budget and eventually upgrade to larger wheels.

I'll go with your decision on the belt and pick up a 15mm too.

Is there any cheaper/more available ESC's that you could recommend, even if just temporarily? And if so what battery setup would work whether its mine or a different one?

Thanks
-Sean
```

---
## \#4 Posted by: seantjaeger Posted at: 2017-01-31T01:05:09.982Z Reads: 141

```
Hmm... Just found this:
http://www.enertionboards.com/diy-electric-skateboard-kits/mono-drive-mechanical-kit

Could this be a good setup as opposed to buying everything separate?
```

---
## \#5 Posted by: sl33py Posted at: 2017-01-31T01:11:10.829Z Reads: 142

```
Yeah at 115lbs (52kg for everyone else) - you are going to be fine w/ a single motor - either.

Kegels are great wheels - but you will have to re-buy wheel gears if you want to go bigger.  Vs flywheel gears which will fit 76mm through 97mm without problems.  107mm electric flywheels need work/shims or a new gear.

Since you want more speed, and are so light - i'd go w/ 190kv motor, but i'd get from Enertion or DIYes (likely faster shipping than from APS).  DIYes for sure, but i think Enertion has his motors in the states now to to help speed them along faster (no customs delay).

Thanks for reminding me - drop through decks are a _**PITA**_ to electrify (doable but a lot more work).  Most folks try and then top mount the board after giving up.  Doesn't look to bad to do this, but just FYI if you are dead set on using the drop through deck.  Sidewinders are flexy so you are going to have trouble when flexing for the motor to not hit the bottom of the deck, or the mount on the truck hanger to hit the bottom of the deck.  Seriously - get caliber trucks - with good bushings for your weight they work _really_ well.  Won't be as carvy/surfy as the gullwings... but you may not want that much carve when going 20mph+ anyway!

Yes - that's a good setup.  Couple caveats.  The enertion mount is stupid simple and really well made - love them for simple setups, BUT your adjustable angle is limited - so you can't rotate (easily - yes you can modify the mount) to have the motor outboard (behind vs inside), and if you want to use a drop deck or drop through deck you may not be able to adjust the motor down enough to easily clear at full lean.

Also check out the batteries from Miami electric and DIYes if you want a SPACE cell like battery w/ BMS.  Pretty competitive vs building your own.  Especially when you factor in the cost of a spot welder to make your own!

I would also check the flex of your deck - not familiar with the drop through Sector 9.  If it's not stiff and flexes - you might have some more challenges with battery selection and placement.

HTH!
```

---
## \#6 Posted by: seantjaeger Posted at: 2017-01-31T01:31:28.695Z Reads: 130

```
Wow, you sure know a lot about this!

Basically what I'm getting out of this is:

New deck- The bamboo gets some pretty crazy flex which could be dangerous
-DIYe full set for the mechanics, wheels, gears etc.
-Prebuilt battery from one of those few you listed
-190kV motor (Probably enertion)

But that leaves me with another question-
If I were to get the DIYe kit with trucks and all, would it still be beneficial to get calibers? Or would that just about complete my mechanical setup?

-Sean
```

---
## \#7 Posted by: IsTalo Posted at: 2017-01-31T01:47:50.065Z Reads: 127

```
Hi Sean, I saw that you are going to buy a lot of expensive things and buy a cheap Esc, Tell Me, Why? Buy a Vesc from Alien, or Enertion, but Vesc is better for E-Boards, It is smoothier and you can change what you want in the software. About the Batteries in Series, Yes, you can make a 10s or even a 12s (Don't know, create a topic for it) but use an anti-spark... Alien Motors and Enertion motors are from the same factory so they are very similar. And always remember, Safety is very important, 20mph is too fast man
```

---
## \#8 Posted by: sl33py Posted at: 2017-01-31T01:48:16.367Z Reads: 126

```
I'm not skilled enough to tell the difference w/ real calibers vs the clones Enertion and DIYes sell.  I *can* tell the difference w/ cheap bushings and good bushings setup for your weight make a huge difference.

If you are tight on budget - i would skip the pre-build battery and get some simple lipos and an iMax charger (the one i suggested).  Especially if you are getting a new deck, wheels, trucks, etc...

Look at the longer motor for more torque on a single setup (at 115lbs you are pretty golden, but power is nice to have):
diy-electric-skateboard-kits-parts/motor-6374-190kv-3150w/

ESC - I'm a huge VESC fan.  I've not tried the new *almost* v6 options both DIYes and Enertion have.  A good 4.12 or so VESC might be ideal if you aren't afraid to follow steps in linux or one of the ported versions for Windows/OSX.  Tons of walk-through videos to help too.  

I'm super helpful blowing your budget out of the water... sorry Sean.  Just remember that replacing parts that fail or don't work well will cost you more.

GL!
```

---
## \#9 Posted by: seantjaeger Posted at: 2017-01-31T03:41:00.925Z Reads: 106

```
Alright I guess I'm gonna have to extend my budget some more :joy:  With the VESC, which would be a relatively cheap option but still hold the values of what it is acclaimed for? I know I'll have to dish out some money either way, but I'd rather keep it reasonable you know for obvious reasons. If you could tell me which is a good cheap-ish one that'd be great.

As for speed, I've been skating for a while now, probably 7-8 years and on my current board I've been able to hit around 23mph just pushing so hopefully that shouldn't be an issue. Thank you for considering that though, I'm gonna look into that some more now so that should help.

Thanks
-Sean
```

---
## \#10 Posted by: seantjaeger Posted at: 2017-01-31T03:47:04.273Z Reads: 108

```
Thank for that I've never been focused on my bushings enough to tell what difference they could make. I won't mind putting some money in for bushings too and I'll make sure that I can get some nice ones for my weight. 

You said that you've used the DIYe trucks, right? Or were you just saying you reccomend them because of reviews and such? If you've used them, would they be ok for the type of build I'm leaning towards? I'd rather stick with those if possible, but if I truly need to then I'll go for the calibers.

I've looked into the VESC more and I think you guys are right (I mean, you are the experts compared to me) so I'm just gonna get together some more money and get one of those. Would those work ok with a 10s battery? Or a 9s instead?

This build might take me a bit longer than I thought, but in the end it seems like it'll all be worth it. Thanks for the suggestions and all. 

-Sean
```

---
## \#11 Posted by: sl33py Posted at: 2017-01-31T18:20:39.745Z Reads: 100

```
Both Enertion and DIYes trucks are basically Caliber clones.  They work fine for me.  I don't have theirs, but on my Marbel i have a caliber clone they used.  Rolls fine!  ;)

Bushings are a noticeable improvement when setup right.  Being a shit-ton heavier than you - i go really hard duro and like the high rebound versions from Blood Orange, Venom, Riptide, etc.  Good quality sources.  Just look at one of their weight range suggestions and you'll have a good starting point.  Another great alternative is to go to your local skate shop and chat w/ those guys - they likely will have something and can help you dial in the right bushing for your weight.

So yeah, i'd stick to the supplied DIYes trucks and just upgrade bushings.  You can always swap later if you feel the need or bend one or ...  

VESC is sweet.  Hard to go wrong starting with one - as long as you follow directions and setup correctly.  If you go with 4.12 or similar VESC - stick to 10s and 200kv max (you want to avoid exceeding 60k ERPM or you'll fry the DRV chip).  Simplistically that limits you to 10s or less, and 200kv or less.  Some of the nicer gear calculators will give you the ERPM of that setup to help you plan better.  And yes - 9 or 10s on VESC will work great.  I've run 6 and 8s on my GF's board for a few years now (on old 4.6 or 4.7 VESC) - no issues.  Single 200kv motor and she loves it (but goes about 8mph max - no joke).

Can't speak to the "almost v6" variants that DIYes, and Enertion have.  Ollin/Chaka had some direct FETs too, but you get my drift.  I'm sure they work well too.  Personally my 4.7-4.12 work fine not running FOC and staying around 10s on lower kv motors <200kv.  So i'll wait for Ben's v6 for now.

It's a lot to learn - just keep asking questions and the folks here will help!

GL!
```

---
## \#12 Posted by: seantjaeger Posted at: 2017-01-31T20:42:45.777Z Reads: 96

```
Perfect, hopefully I can start building soon. I just opened up an old hover board and got the battery out, I'm gonna make a seperate post on it if you wouldn't mind taking a look? Thanks for all your help so far it really means a lot. Now I think I've got everything sorted out except for the battery. 

-Sean
```

---
## \#13 Posted by: sl33py Posted at: 2017-02-01T01:31:30.098Z Reads: 92

```
Get some decent lipos if you want to get started, and know you're going to go VESC.  Personally i like 3s batteries in series - 2 for 6s (good for loaning to a friend so they don't hurt themselves), 9s for great power, and if you can avoid 60k ERPM - 4 for 12s and top speed/power (149kv maybe).

You want the best C rating you can afford - it equals less voltage sag under use.  So two "equivalent" 5000mAh Lipos - one will be 20C, and another 35C - get the 35C one.  I would not go lower than 20C on 5000mAh to make sure it can supply ample amps.  (C x Ah = constant amps capacity so 20C x 5Ah = 100Amps capability).  Marketing being what it is - a bit of extra leeway to make sure you don't over discharge or have excessive voltage sag when in use.  5000mAh = 5Ah to be clear.

I'd get batteries from hobbyking (US warehouse), fast and cheap.  No they won't last as long as 18650 batteries, but much less $ and a good starting point.

GL!
```

---
## \#14 Posted by: seantjaeger Posted at: 2017-02-01T02:46:05.021Z Reads: 89

```
Perfect, I'm 1/3 lipos there. 

Would I able to use perhaps a setup with two 35c 11.1s and a 20c 11.1 all with the same capacity? Or two 20c 11.1s and one 35c 11.1? If so that would help a lot.

Also I don't know if you saw my other post referencing the battery from the hover board, which is apparently a pack of 18650s (36v worth) so maybe I could use that instead?

Otherwise I'll look into the lipos some more right now.

Thanks
```

---
## \#15 Posted by: Youngin255 Posted at: 2017-04-13T05:37:30.788Z Reads: 74

```
I also am trying to build my first eboard. I will be using gullwing sidewinders and i was thinking of using this motor mount
http://www.ebay.com/itm/DIY-Parts-Pulleys-Kit-And-Motor-Mount-For-80MM-Wheels-Electric-Skateboard-New-/222353819287?hash=item33c5520697:g:aqEAAOSwJ7RYW59Q
I weigh 165 pounds will be riding on relatively flat terrain with a few hills here and there an want to go about 25-30mph I was wondering what motor and esc to get that would be around $150 
i will be using 2 venom 5000mah 35c 3s lipos and 1 venom 5000mah 50c 3s lipo
for the wheels i indend on using generic 90mm wheels from amazon. 
If anybody could let me know whether that motor mount would be good and what motor and esc to use i would really appreciate it as well as any other advise or feedback.
```

---
## \#16 Posted by: seantjaeger Posted at: 2017-04-13T18:55:06.995Z Reads: 66

```
As much as i wanted to use sidewinders, i just dropped that idea and i'd advise you to also. I know it seems great to be able to carve like that at those speeds, but it's just not very smart because the motor will grind against either the street or the board and you will also get lots of speed wobbles.

As for your other questions, the VESC is preferred by most people although it is out of your price range. It is one of the only ones actually meant for eBoards so it has many more settings that favor riders. If you're looking for both a motor AND esc for under 150, you're kinda out of luck being that the VESC alone is around 100. 

The mount looks okay, but just make sure it will fit your other parts/specs.

I'm not sure how much you've looked into motors and such but if i were you i'd go with maybe 190kv and 65mm motor being that this should get you good speeds for a relatively low price. If i were you id cap the speed at maybe 25 or a little bit higher because it starts to get very fast around there. If you'd like you can go here to calculate the speeds you'll get: calc.esk8.it/

Your batteries sound okay, but i wouldn't mix the batteries, it can lead to them getting destroyed if they charge at different rates and/or discharge at different rates. It's better to go with 3 of the same just for consistency and safety.

I know this will probabt blow up your whole plan and be frustrating, but I am dealing with the same problems really. I actually had to put off my build so i could get more money to build it.

I hope some of this helped, if you have any other questions you can ask and ill try to answer them as best as i can.
```

---
## \#17 Posted by: faithfulpuppy Posted at: 2017-04-13T19:12:02.851Z Reads: 61

```
yep i was using sidewinders too.  It can be done with that mount, but make sure it actually mounts 63mm motors (the one i got took 50mm exclusively).  i ended up sinking a lot of money into it and it didn't work out so now i'm basically starting over with calibers.  You can get calibers for like $30 or $40 on ebay and there's a guy on here doing a GB for motor mounts for $22 ($28 shipped) so it's not much more expensive.  Get a kit like that without the mount for your pulleys and stuff because that's worked well for me so far.  

In short: Can it be done? absolutely.  Do i recommend it? no way in hell.

@Youngin255 just to make sure you see this

that being said: i'm probably going to try to revisit the sidewinders in a later build, maybe over the summer because i do like double-turning trucks (i ran carver c7s on the board that is now going to be my e-board for over 2 years)
```

---
## \#18 Posted by: seantjaeger Posted at: 2017-04-16T16:22:00.367Z Reads: 58

```
My god do I wish I could use my sidewinders and not have to worry, but like you said it's not recommended at all haha. Although I do believe it could be done with hub motors. That's a project for another day, though. Need LOTS of balance.

Those trucks look really cool, I'd love to try those out someday. If you've ever ridden sidewinders, how different are the two? Now you've got me interested, even though I'm about to begin a downhill board.
```

---
## \#19 Posted by: faithfulpuppy Posted at: 2017-04-16T19:46:51.465Z Reads: 57

```
Which two? the enertions and sidewinders? I own carver c7s, gullwing standard RKP trucks, gullwing sidewinders, and now caliber IIs: AMA!
```

---
## \#20 Posted by: seantjaeger Posted at: 2017-04-17T21:51:38.105Z Reads: 61

```
The sidewinders and the C7s. They seem similar so you got me interested
```

---
## \#21 Posted by: faithfulpuppy Posted at: 2017-04-17T22:54:01.411Z Reads: 58

```
the sidewinders feel a lot like normal trucks, just more so (if that makes sense?).  They lean and turn in much the same way, except you're just going to be leaning and turning a hell of a lot more

the C7s, on the other hand, are completely unlike anything else. They also turn really easily (the reason i originally got them was because at the time i was too light to actually turn normal trucks, being a shrimpy pre-teen), but they don't feel similar to other trucks.  Most of your turning is coming from the front, so the board really dives into turns.  Additionally, something about the way the hanger pivots makes the trucks bounce like nothing else.  They're really fun and lively trucks that you can just throw your weight into and thrash around.  Most people can't stand them but i absolutely adore them. If you get the chance to try them out you should

That being said, i don't know how much of that is due to the fact that the front truck turns more than the back (something that can be easily achieved on other trucks by angling them or swapping your bushings) and how much is due to them actually being differently designed.  However, the way they bounce around when you throw your weight into them is absolutely a carver thing

**DISCLAIMER**
*The Carver C7s were my first trucks and i rode them exclusively for like two or three years.  I got everything else in the last year or so, so i naturally have a lot of fond memories with the carvers*
```

---
## \#22 Posted by: seantjaeger Posted at: 2017-04-19T11:11:39.637Z Reads: 49

```
Hmm maybe I should look into the carvers then. I currently have sidewinders on my board and I made them extremely loose because you know, who doesn't love 90 degree turns! But the way you described the carvers makes me wanna try those out. I also have been missing my old Paris trucks though, so I'll probably end up breaking down and getting those again (had them like 5 years ago but the board got stolen :cry: ) they turned great for being a single set of bushings unlike the sidewinders.
```

---
## \#23 Posted by: faithfulpuppy Posted at: 2017-04-19T15:17:11.520Z Reads: 44

```
i'd say dont put carvers on your first esk8, they're not as stable at the speeds you're gonna be hitting.  They're fun, but impractical and expensive
```

---
