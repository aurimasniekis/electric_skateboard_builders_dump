# How do i make a plug in and leave to charge setup?

### Replies: 41 Views: 2827

## \#1 Posted by: Jammeslu Posted at: 2017-02-15T21:41:08.222Z Reads: 276

```
im a beginner on my first build and want to make a easy charge function without needing to take out the batteries each time, running 3s 5200mah x2 on a sk3 249kv single drive setup with vesc. so how do i do and what do I need? a bms thing? what like a laptop charger tho I'm a student and need to carry charge with me. didn't know how to create a thread so just posts this here and would be very happy for answers
```

---
## \#2 Posted by: Okami Posted at: 2017-02-15T21:52:12.986Z Reads: 280

```
You can either get Bms (one plug charging).. or make ''VGA port'' / Miami boards all in one charger..

VGA port charging would happen through one port but you would have to solder the balance leads to the pins of the port.. This way you would still get the chance to use your smart charger (which I assume you have).. to charge your lipos..

BMS -> One plug -> No smart charger, just constant voltage source or so..

VGA port ''mod'' -> One plug for charging (but many smaller wires connected to the port) -> Smart charger
```

---
## \#3 Posted by: RogerD Posted at: 2017-02-15T22:56:24.619Z Reads: 261

```
There is a VERY easy way to do this, and it's how I charge my main board (2 packs of 6s 15000mah each).

1) buy a power jack (3.5mm - or whatever the below charger has on the end) and link it into your main power feed to your batteries - not to the balance leads (ignore them), but at the main power output of your joined battery packs.  + and -
2) buy a cheap lipo charging "brick" rated at your battery voltage, in your case 6s (like mine) . Here is what I use (£13 delivered)

Plug charger into power jack you installed. Walk away and forget it. When it's charged the LED on the charger will go from red to green.

You do not need a BMS. Everyone is fretting over BMSs. I've been using lipos for years and years, well before esc8ing. Unless you have a bad pack, or you regularly run your packs below 3.2 volts per cell they will stay mostly in balance. By mostly, I mean close enough it makes zero difference. If you have a bad pack then no amount of BMS balancing will make it good.

Set your ESC to cut off before your batteries get to 3.2v and you can't flatten your lipos. On most ESCS choose the middle to cautious cut off setting. If your pack doesn't seem to run for long before cut off, measure the voltage at rest, and if it's ok, reduce the cut off voltage, then retry.

That's it. All for under £14 and dead easy.

I've just gone to my shed and metered my two 6S Turnigy Multistar (cheap) 15000mah packs, disconnected. Used all last year, never balanced, always charged as above.

Pack 1: 
4.01
4.02
4.00
4.02
3.99
4.01
Pack 2:
3.95
3.95
3.98
4.05
4.04
4.05

Easy close enough to be fine, and I can guarantee they will all settle at 4.2 v when charged.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-02-15T23:54:21.102Z Reads: 214

```
You need to balance your Lipos every time you charge them. So either install a bms and use a brick charger or go the VGA port with a hobby balance charger.
Either way you should never walk away while charging Lipos. You should always keep an eye on them in case the unthinkable happens.
https://youtu.be/fF9fhlr9S5s
https://youtu.be/osfgkFyq7lA
```

---
## \#5 Posted by: Jammeslu Posted at: 2017-02-16T07:16:40.057Z Reads: 202

```
But both was, Will it still balance charge and dont over charge if i leave IT over night? And what do you mena with smart charter?
```

---
## \#6 Posted by: Jammeslu Posted at: 2017-02-16T07:20:25.254Z Reads: 198

```
Ok seems pretty easy then, but are you sure I dont need bms? And how long would A brick charge?
```

---
## \#7 Posted by: RogerD Posted at: 2017-02-16T08:45:23.355Z Reads: 190

```
You dont' need to balance charge them every night. I've been non balance charging lots of packs for years.

Up to you if you go for the scare stories or not.
```

---
## \#8 Posted by: PXSS Posted at: 2017-02-16T09:02:02.247Z Reads: 184

```
I would not follow @RogerD advice unless you are experienced with RC stuff and how LiPos and your esc operate. You're just asking for trouble otherwise.
```

---
## \#9 Posted by: Okami Posted at: 2017-02-16T10:21:19.017Z Reads: 179

```
I think this is especially true if the lipos get to rattle inside the enclosure or they may get ''banged up'' in some way..

A buddy of mine ''lost'' his drone this way.. I believe he left it charging and he did not choose balance charge either.. (his charger allowed to charge in non-balance mode).. So when he returned his workshop was full of smoke and basically what was left out of his drone was a pile of coal and burnt material :D

Non the less.. this was a drone which had crashed a couple of times.. but yeah the risk is always there to overcharge a battery or something may go wrong if some sort of short happens in the battery itself
```

---
## \#10 Posted by: Jammeslu Posted at: 2017-02-16T15:14:08.063Z Reads: 163

```
Ok, I think I'll go with bms since I cant take the risk, how ever could someone link som Good reliable stuff that is not overprized, bms, charge brick, charge port and any wires, and if any one has A diagram on how to wire everything would be very helpful
```

---
## \#11 Posted by: Hummie Posted at: 2017-02-16T19:00:30.197Z Reads: 154

```
i also think a bms isnt necessary as long as you monitor the cells.  you should always be around when charging and charge somewhere you can deal with it if it does blow or somewhere it wont matter if it blows.  
get in touch with your inner lipo and feel the lipos after you ride and while charging for any heat.  this is on top of watching their voltage when charging.
```

---
## \#12 Posted by: mmaner Posted at: 2017-02-17T19:15:31.789Z Reads: 145

```
[quote="Hummie, post:11, topic:17755"]
get in touch with your inner lipo and feel the lipos
[/quote]

Lol, u r funny dude 😀
```

---
## \#13 Posted by: sl33py Posted at: 2017-02-17T19:48:40.141Z Reads: 148

```
[quote="RogerD, post:3, topic:17755"]
That's it. All for under £14 and dead easy.
[/quote]


Cannot agree here.  IMO you *must* balance every time you charge, or use BMS.  Don't skimp on something like this to save a few $ and potentially risk lives/property.  

I know my GF is *super* paranoid about fire, so i've started using the temp probe for my packs when charging as well to help her feel more comfortable.  In pyrex dishes (cheap from value village) as added insurance.  Only a few $ to add the temp probe and it will stop charging if the battery exceeds a set TEMP on my iCharger (others have it too like iMax B6ACV2 iirc).  Heat is the first warning before catastrophic issues.

I understand being on a budget, but "cheap" and "charger" are not something i'd try to mix...  

HTH - GL!
```

---
## \#14 Posted by: Hummie Posted at: 2017-02-17T20:37:07.032Z Reads: 139

```
Using the integrated temp sensor on the finger while charging works well.  Also I can press on the pack while doing temp sensing with the same finger and see if it's expanded, and at the same time look with the eyes at the voltmeter and see the voltage the pack is seeing.  When charging I think a bms performance can be beat, it's in an instance when a cell were to be damaged while riding, after its done with me on the charger, that a bms comes into its own and a cell could get damaged and I wouldn't know what's going on.   I think a simple temp sensor on cells while riding would be a solution as its not going to burst into flames before increasing substantially in temp.  
The benefits of not using a bms for me are: more room for batteries (which is a safety feature in a way), less things to break (bms often seem to break), cheaper, I get more aware of what's going on and ..a biggie I think..with this awareness I would know if I have bad cells or a bad cell ruining performance as apposed to riding blindly with a bms and just accepting what it does.

Makes me wonder is there a way to hook a temp sensor up to the vesc simply?
```

---
## \#15 Posted by: Okami Posted at: 2017-02-17T21:52:24.456Z Reads: 138

```
@Hummie The temp thing you mention seems like a good idea.. I've seen some of these ''heat pads'' which change color, if they get heated to or above 40C (104F) or maybe even other temps..

ask @Ackmaniac about temp sensor thing.. I thing there was this possibility to attach ''motor temp'' wire/connection.. it is just not used up a lot and can be used to measure other things (batteries)
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-02-17T21:59:39.011Z Reads: 140

```
It would be possible to hook up sensors. But you don't need it for the battery. I attached a external temperature sensor to my pack with laptop batterys and rode it hard for 5 km in my completely sealed enclosure. And the temperature only raised by 10 °C. So with propper Li-Ion cells you won't face any issues. Even my 10 °C were harmless.
If you start riding at 40 °C outside temperatur and climb up the steepest never ending hill and drive full speed until the battery is empty then you might reach it. But i think that's never going to happen.
So simply don't worry about the battery temperature.
```

---
## \#17 Posted by: Hummie Posted at: 2017-02-18T02:20:14.924Z Reads: 135

```
the reason for the temp sensor would be if you run without a bms you can still know if you have a dud cell before it were to get so abused as to possibly vent.  hook up the sensor to your phone and it could tell you if something were getting hot.  most fires with lithium happen while charging, and you could utilize the temp sensor then as well while bulk charging.  If only the cell voltages could be transferred to the phone too.
```

---
## \#18 Posted by: RogerD Posted at: 2017-02-18T11:31:16.198Z Reads: 126

```
Sorry to disagree here , but there is no "MUST" in balance charging. You may only be happy balance charging, but it is in no way a must.

You should also not equate cheap = bad/poor. That's an Apple mindset.
```

---
## \#19 Posted by: PXSS Posted at: 2017-02-18T13:52:54.566Z Reads: 119

```
I'll just sit here and watch for the fires to start happening :)

@RogerD, please tell me you ride without a helmet
```

---
## \#20 Posted by: RogerD Posted at: 2017-02-18T15:16:55.615Z Reads: 120

```
If I'm going to the pub 1mile down the road I keep it around 10mph and ride without a lid.

I never cycle with a lid.

If I go out for a proper skate bard ride (i,.e for the sake of a ride) I wear a lid.

I always wear a lid on a motorcycle.

I take resposibility for my actions, and balance risk with practicality and enjoyment.

I've not had a lipo fire, ever. Must be a miracle.
```

---
## \#21 Posted by: Hummie Posted at: 2017-02-18T19:16:14.106Z Reads: 115

```
I like to view it from the perspective of being a tour de france bike racer before 1990 when they didn't wear helmets.   If the total time of all the riders from any of the tours of more recent date, when better records are kept, is added and put in relationship with the amount of long lasting head injuries that occurred, there's a ratio revealing a likelihood that's unknown to me but I like to believe it tells of the greater importance of being good at falling.  

I wear a helmet if I go out of the city on a bike but on the board I almost always put it on.  too many weird things happen on a board. literally two days ago almost fell off someone else's crazy powerful board without a helmet just trying it going down the street.
In a weird unexplained bike accident I had I experienced a very scary fading out for a 20 minute period but I luckily started to recognize faces and shook it off and have been said to be as good as ever if not better now!   If I had been wearing a helmet I wouldve been just as injured as I hit my cheek bone only.   If there had happened to have been a car behind me and I'd been run over my helmet wouldve likely been no help of course.
```

---
## \#22 Posted by: sl33py Posted at: 2017-02-18T21:19:09.362Z Reads: 109

```
[quote="RogerD, post:18, topic:17755"]
but it is in no way a must.
[/quote]


Yeah absolutes are tough.  Not an apple guy either.

Let me rephrase - _your_ tolerance for risk is much higher than _mine_.  I _**always**_ balance charge my lipos.  If i had some 18650 packs i might not, but for Lipo - i *always* balance charge.  

Safety is more important to me, and _**i would not feel comfortable suggesting to anyone that they don't balance charge lipos.**_  That seems like suggesting negligence... Someone will do this, with damaged cells, or already mis-mashed and different charge levels...  it's a BAD IDEA AND RISKY.  So please, balance charge your lipos until you know what you are doing and can make an informed decision and accept that _risk_ for yourself.
```

---
## \#23 Posted by: mmaner Posted at: 2017-02-19T02:11:26.451Z Reads: 107

```
I'm gonna put my 2 cents in here...

I'm not particularly safety minded, I almost always forget my helmet unless my kid is with me...Then I remember because I make him wear his.

I do get particularly pissed off by burning up money and that is ABSOLUTELY what you will do if you continually do NOT balance charge.  You might not have a fire from a vented cell, bit you will eventually get a bad cell.  Then you have useless battery and have to buy another.  All of which could have been avoided with the use of a BMS, or in my case, a balance charger.

More importantly, saying you don't need a BMS to new builders makes you an asshole or an idiot.  Don't be that guy.  I guerentee some 15 year old will see this post and figure he can save 30 bucks, and $30 is a lot to a 15 year old, and burn up a battery, get pissed and quit.  

Is making an inane statement that cannot be justified or proven under any definitiin of normal conditions worth causing some kid to quit skating?

The more people on boards the lower the cost of components, the less often cops will screw with us, the more prolific shops will be that sell estate components.

I say again, don't be that guy.
```

---
## \#24 Posted by: Montiey Posted at: 2017-02-19T03:31:23.156Z Reads: 98

```
I've been using 4 5400mAh 4S Multistar packs in a 2S2P configuration… Some of the cells charge to 4.21, others only to 4.17. After riding, the difference is even more dramatic.. Even a 0.2V difference in some cases. If you buy 1000 cells off eBay and match them up based on internal resistance (don't quote me on that), then you may get away without balancing or balance charging, but you definitely shouldn't tell a newbie that they don't need safety features…No offense, but people don't seem to know much of anything about LiPos when they're just starting into an RC hobby or EVs..
My friend bought a HobbyZone Champ a couple of years ago, and was confused about why the small lipos wouldn't hold a charge after sitting full for a month or two- case and point. Yes, you can say that you know what your doing because you've blown up a few packs of your own, but everyone ought to use LiPo safe-bags and anything else that would seem even remotely necessary, regardless of experience.
Check out [this](http://www.bat-safe.com/web/) or [this.](https://hobbyking.com/en_us/lithium-battery-charging-safe-box.html)
```

---
## \#25 Posted by: RogerD Posted at: 2017-02-19T10:55:21.895Z Reads: 88

```
No need to call me an arsehole and an idiot. I haven't stooped so low, particularly on a forum that is, as you highlighted, full of kids.

I give advice based on my knowledge and experience.  If you don't like it you know where to stick it. 

It's experienced advice, take it for what you will or ignore it. But no need to be offensive.
```

---
## \#26 Posted by: Jammeslu Posted at: 2017-02-19T22:37:59.245Z Reads: 92

```
I started this and ask in the thread and Im 15 on my first build, just like you all say that you shouldnt try to save a couple bucks on bms but since Im on a limited budget and on my first build what other components can I save on?
```

---
## \#27 Posted by: Hummie Posted at: 2017-02-20T05:48:11.719Z Reads: 87

```
15?  doesn't matter.  you can figure it out if you want to at any age.  it takes responsibility either way and wiring up a bms is fraught with dangers as well.  I'm sure you'll figure it out and do the responsible thing either way, there are different paths to chose and a bms is not the land of instant safety even after you get it running.  expect failure!  electric skateboards are failing left and right, look around and you'll see.
```

---
## \#28 Posted by: Jammeslu Posted at: 2017-02-20T10:31:01.455Z Reads: 83

```
Thanks, my dad is a top enginerr so he can help me if I need it but i want to do everything myself so i can be proud of my very own board at the end
```

---
## \#29 Posted by: Jammeslu Posted at: 2017-02-20T20:13:04.941Z Reads: 81

```
Btw can anyone Tell me how much of A capacity A bms must have, Im on A singel motor with 6s batteries
```

---
## \#30 Posted by: Montiey Posted at: 2017-02-22T19:26:18.008Z Reads: 77

```
What motor? More specs on the batteries, too. I run 8s packs, but it's really a total of 16 cells- 4s packs in 2S2P, for example.

On the BMS side, you may need to match the configuration, but I don't really know. I haven't messed with BMS's too much, I just make sure my packs are at 3.8v before I leave them lying around. Maybe soon, though :)
```

---
## \#31 Posted by: sl33py Posted at: 2017-02-22T20:59:44.396Z Reads: 81

```
[quote="RogerD, post:25, topic:17755"]
It's experienced advice, take it for what you will or ignore it. But no need to be offensive.
[/quote]


Fair enough.  I think the issue is your experience and willingness to chance damaging known-good cells is higher than most.  And more concerning - suggesting to folks that *definitely* do not have your experience and common sense when emulating your setup - who might use a mix of cells - good and bad, because "i don't need to balance" - could lead to catastrophic issues.  That is where i think we get our feathers ruffled and over-react.  I'd hate for someone to lose their board, let alone more, because they took something i said as gospel and didn't question or take precautions.
```

---
## \#32 Posted by: sl33py Posted at: 2017-02-22T21:05:22.884Z Reads: 93

```
[quote="Jammeslu, post:29, topic:17755, full:true"]
Btw can anyone Tell me how much of A capacity A bms must have, Im on A singel motor with 6s batteries
[/quote]


BMS adds a fair bit of complexity.  I'd get your dad's help to get it setup correctly.  You need to do a ton more research - keyword search BMS and start reading.

Having not setup a single board with BMS (my marbel has it, but i've not built one w/ it) - there is another wrinkle - pay attention to both *Charging* Amps, and *Discharge* Amps.  Folks have wired less expensive BMS'ssss as charging only and bypassed for discharging direct from the batteries to avoid the small/cheap BMS limited discharge.

A space cell 10s3p has 60A discharge capability.  I've measured on dual motors 8s a peak of 45A using VESC's.  It will depend on your batteries' discharge ability (look at the C rating of lipos, or discharge in amps of an 18650 cell (25r's claim 20A iirc) - then you get into increased Amp delivery/capacity in parallel...

Higher voltage is more efficient - so less amps.  A 6s setup will pull more amps for the same load/speed vs 8s i got 45A peak.

It's a lot of info - takes a while to get the hang of it all.  I don't claim to be an expert by any stretch, but love learning new stuff every day!

HTH - GL!
```

---
## \#33 Posted by: PXSS Posted at: 2017-02-22T21:31:53.364Z Reads: 92

```
I'll just leave this here. I have a dozen or so more ammo cans full of swollen or exploded LiPos, but by all means @RogerD, keep advicing strangers to not use a BMS. 

<img src="/uploads/db1493/original/3X/3/6/36885013684dbbb9fb17fedf8de6889cecb117bc.jpg" width="375" height="500">
```

---
## \#34 Posted by: RogerD Posted at: 2017-02-22T21:46:05.107Z Reads: 87

```
Then you must be exceptionally careless. I dont' have one single "dangerous" cell. And putting slightly puffed batteries in an ammo case kind of explains to me where exactly you are coming from, so to speak. Some people are over obsessed with safety :-)
```

---
## \#35 Posted by: sl33py Posted at: 2017-02-22T22:28:57.790Z Reads: 86

```
[quote="RogerD, post:34, topic:17755"]
Then you must be exceptionally careless. I dont' have one single "dangerous" cell. And putting slightly puffed batteries in an ammo case kind of explains to me where exactly you are coming from, so to speak. Some people are over obsessed with safety :slight_smile:
[/quote]


Roger - losing respect for you quickly.  (i know i know - i'm sure it hurts... ;) )

You are saying someone is careless vs poor quality/inexpensive cells that just fail...  that's ignorant.  It's called MTBF.  happens.

"over obsessed with safety" - by not using "slightly" puffed cells?  Dude - really?!?

**Newbies - please use common sense.**  Don't listen to Roger here.  WIll you burn your house down - likely not, but you definitely might fry your board.  And all we all need is another news article about some board catching fire/smoking on public transport... so we have further restrictions using these for transportation/last-mile/fun!

Balance to start - if you get comfortable and feel confident later to not balance - at least learn enough to make this an informed choice vs following some _random guy on a forum who isn't seeming very credible..._

Don't take my word - do research.  Inform yourself.  Check other forums and look for someone who has a reputation for being knowledgeable/helpful and ask them!
```

---
## \#36 Posted by: PXSS Posted at: 2017-02-23T03:53:41.420Z Reads: 82

```
When you own hundreds of Lipos and thousands of Liions that go on half a million dollar aircraft, yeah you tend to be a little ocd about which cells you fly. 
You also tend to see a lot more duds when you buy this many. 

The ones in the picture are also not "slightly puffed", they also have shrapnel embedded in them. We keep them in ammo boxes because again, we have tens of half a million dollar aircraft sitting in our workshop and losing even a single aircraft because of carelessness is not an option. If a cell combusts a few years down the line, it won't matter because we took the appropriate steps to be safe.

I value my life more than these airplanes. If you dont then thats up to you but dont go telling kids its ok as that is idiotic. (I'm not calling you an idiot, I am calling your actions idiotic)

PX
```

---
## \#37 Posted by: Hummie Posted at: 2017-02-23T04:19:20.862Z Reads: 74

```
so you fly drones for the military?  guess.  they use lipos?  and then again maybe while a lipo gets a bad rep it's really the li-ion that are the more dangerous as they shoot off like rockets sometimes when they go up.  All this talk makes me want to blow some up honestly. for science.  want to know what would happen if it were hooked to the the ac outlet in my house. not "a plug and leave to charge setup"
```

---
## \#38 Posted by: mmaner Posted at: 2017-02-23T14:02:20.665Z Reads: 71

```
[quote="PXSS, post:36, topic:17755"]
(I'm not calling you an idiot, I am calling your actions idiotic)
[/quote]

I'm calling him an idiot.  Not because he said something stupid, but because he keeps saying it regardless of proof to to contrary.  

My father law has this saying that makes me want to punch him in his old ass fake teeth...  "It's ok to be a dumbass, but there's no requirement that you open your mouth and prove it".  It rings particularly true in this case.
```

---
## \#39 Posted by: PXSS Posted at: 2017-02-23T14:46:30.970Z Reads: 71

```
Yep. Thats our job. They use all kinds of different chemistry cells including Liions, Lipos and other lithium based primary cells.

I've blown a few of them up for science! Really fun stuff but you have to be careful
```

---
## \#40 Posted by: Hummie Posted at: 2017-02-23T15:10:21.474Z Reads: 73

```
i think people are giving Roger unwarranted hostility.  If you look in the ebike world, which has been spinning long before esk8, it's pretty common practice to no balance all the time when charging and they dont use a bms.  Many people bulk charge lipo if you look on endless-sphere.  It's fair to say it's more dangerous, maybe, but maybe not and it depends on the person.  It depends on even your charger as I've heard of cheap balancing chargers setting peoples stuff on fire.  In my mind the most important thing when charging lipo or li-ion is that you're there to deal with anything if it goes wrong.  Even if you burn up your house or your neighbors house at least youre there to get them out of it.  Of course putting out the fire is even better but a house is replace able and it's the lives that are all that matter.

here's the harbor freight new lithium saw teardown.  no bms!  no way to even balance if you wanted to!  danger direct from the store and you'd have no idea
http://www.etotheipiplusone.net/?p=4187
```

---
## \#41 Posted by: mmaner Posted at: 2017-02-23T20:02:08.300Z Reads: 64

```
[quote="Hummie, post:40, topic:17755"]
the most important thing when charging lipo or li-ion is that you're there to deal with anything if it goes wrong
[/quote]

Absolutely.

To be fair, my issue with Roger, and the "unwarranted hostility" was that he recomended EVERYONE not use a BMS or Balance charger.  He made no exceptions to that statement, like "New builders should ignore this" or "only do this if you are experienced".  And then he had the sack to defend the same position.  

I'm sure he's a great guy, probably rescues kittens and gives hugs to the elderly...he may even be MOther Teresa's long lost nephew and bound for a Cardinalship.  That doesn't change the fact that stupid fell out of his mouth, the aforementioned stupid could potentially damage the community, builders and property.

I am not trying to be a dick, there's just a few topics that need to be thought about before people say things...and at the very least modify the position so that other people do NOT take inane crap (formerly labeled as stupid) as gospel.
```

---
