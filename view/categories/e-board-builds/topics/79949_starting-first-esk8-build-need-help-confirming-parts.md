# Starting first esk8 build. Need help confirming parts!

### Replies: 122 Views: 1209

## \#1 Posted by: ZachTetra Posted at: 2019-01-05T04:43:26.168Z Reads: 189

```
I am starting my first esk8 project, converting my current long board (Minority 40' downhill drop deck with 90mm wheels).  I think I have all the parts picked out but I want some help confirming they are good choices or that they are the cheapest available!

This is mostly going to be used on a college campus (5 miles per day and 10 degree slopes) but occasionally on back roads (10 mile cruises in the dark and 25 degree slopes).

The plan is to...
- separate series battery cells into 6 groups of 2, stick cells to underside of deck, cover with aluminum sheets (countersink bolted), impossible to puncture or compress and less than 0.5" in added thickness
- seal ESC and RC receiver in aluminum housing as heat sink (poke antennae through deck) with silicone seals, impossible to get wet/dusty
- bolt steel motor mount to trucks (I think they are Paris trucks?) by each wheel, impossible to slip
- chain motor (one motor to each wheel) to rear wheel with 1:3 gear ratio, 8 tooth to 24 tooth with bike chain, also impossible to slip
- remove electronics from transmitter and place in 3D printed housing, mount to forearm and use wrist motion to control speed, dead man switch
- wire a LED strip in parallel with the main power for under glow and headlights

I know all the parts fit and I think the specs are good.
The motors sit tail to tail off the back end of the board but the motor mounts will be bigger to act as a shield.
It should go up to 2.5kw if I max the throttle which is a lot for a board but the deck is drop down so there is more grip by the back of the board.  The max speed is about 30mph/48kmh.
I think the battery will be fine if I pull it apart, I will use low gauge silicone wires to connect everything 

Please tell me if there are better or cheaper alternatives to any of the parts listed, and if anything I am doing is stupid or wrong.  You have no idea how much I would appreciate some input, several of my friends have boards but nobody is taking the process seriously so I am basically on my own.

I draw up rough sketches for any parts if they are needed for someones understanding but I would rather not since they are time consuming

$357.47 for new parts, $430.45 for everything

Board: $42.99 (already purchased) (MINORITY Downhill Maple Longboard 40-inch Drop Deck) https://www.amazon.com/MINORITY-Downhill-Maple-Longboard-40-inch/dp/B06XJQQ2NJ?ref_=bl_dp_s_web_16950019011

Wheels: $29.99 (already purchased) (90mm Wheels Longboard Flywheels + Owlsome ABEC 7 Precision Bearings) https://www.amazon.com/Longboard-Flywheels-Owlsome-Precision-Bearings/dp/B01IBJ5Y1G/ref=sr_1_4?s=sporting-goods&ie=UTF8&qid=1546657978&sr=1-4&keywords=90mm%2Bskateboard%2Bwheels%2Bwhite&th=1

Motor: $46.72 2x (Turnigy Aerodrive SK3 - 5045-450KV Brushless Outrunner Motor) https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5045-450kv-brushless-outrunner-motor.html

Controller: $24.99 (XCSOURCE 2.4GHz Radio Transmitter Remote Controller + 4 Channel Splash Proof Receiver + Binding Plug Electric Skateboard OS917) https://www.amazon.com/XCSOURCE-Transmitter-Controller-Skateboard-OS917/dp/B073GX83NH

Battery: $119.02 (Multistar High Capacity 10000mAh 6S 12C Multi-Rotor Lipo Pack w/XT90) https://hobbyking.com/en_us/multistar-high-capacity-10000mah-6s-12c-multi-rotor-lipo-pack-w-xt90.html

ESC: $91.82 (Turnigy SK8-ESC V4.12 For Electric Skateboard Conversion w/BEC) https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html

Charger: $28.20 (IMAX B6 BALANCE CHARGER W/ POWER SUPPLY) http://www.valuehobby.com/b6-charger-set.html
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-01-05T04:56:49.878Z Reads: 149

```
Stick with the motors but lower the kv. 190kv is a nice spot. Low 200s is fine as well
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-01-05T05:19:01.147Z Reads: 148

```
The problem is that there is only 152mm between the inside edges of the wheels and I want 2 motors with chains to fit in that gap so I can only use XX45 or smaller, but anything smaller can't take the amps.  I can't find this motor with lower Kv, is there something you had in mind?

The only solution I can come up with is gearing the wheels down 1:3 which ends up around 30mph under load which I think is reasonable for open roads
```

---
## \#4 Posted by: J0ker3366 Posted at: 2019-01-05T07:25:41.680Z Reads: 137

```
Solid build. Caliber II trucks? If so, you can use 12mm pulleys and use dual xx55. Definitely 190kv motors in those
```

---
## \#5 Posted by: mynamesmatt Posted at: 2019-01-05T09:11:02.403Z Reads: 129

```
you'll soon realise 2.5kw isn't really that much power g
```

---
## \#6 Posted by: Noob-at-building Posted at: 2019-01-05T12:45:22.066Z Reads: 122

```
Please use these :frowning:
https://www.genstattu.com/tattu-30000mah-22-2v-25c-6s1p-lipo-battery-pack.html
![image|350x350](upload://3A92Dspivn75mDsxnrHZNR0Kh3Q.jpeg)  
Please
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-01-05T17:43:17.173Z Reads: 109

```
How much power should I aim for?  I've used my friend's 350W hub motor board and it's not awful, with a backpack I'll only be 140lbs so it's not like the board is under a lot of load
```

---
## \#8 Posted by: ZachTetra Posted at: 2019-01-05T17:51:47.166Z Reads: 108

```
I think Caliber IIs are square shaped and these are round so I doubt it.  As far as I can tell 2 xx55 motors end to end is at least 16.8 cm with the axle and bearings (according to the HobbyKing technical diagram associated with a 5055 motor).  Is there a particular xx50 or xx55 motor you had in mind?
```

---
## \#9 Posted by: mynamesmatt Posted at: 2019-01-05T19:56:16.829Z Reads: 104

```
alot of guys here run dual setups anywhere between 5000 and 7000w. personally i run 8800w.
```

---
## \#10 Posted by: mynamesmatt Posted at: 2019-01-05T19:57:03.247Z Reads: 107

```
[quote="Noob-at-building, post:6, topic:79949"]
Please use these :frowning:
[https://www.genstattu.com/tattu-30000mah-22-2v-25c-6s1p-lipo-battery-pack.html ](https://www.genstattu.com/tattu-30000mah-22-2v-25c-6s1p-lipo-battery-pack.html)
![image|350x350](https://www.electric-skateboard.builders/uploads/db1493/original/3X/1/9/191c855a2b7f1f0aa8e05394220b63f249ebbce2.jpeg)
Please
[/quote]

Please DON'T use these. your boards wheels won't touch the ground with this under it
```

---
## \#11 Posted by: Skunk Posted at: 2019-01-05T20:06:40.858Z Reads: 99

```
[quote="ZachTetra, post:1, topic:79949"]
impossible to get wet/dusty
[/quote]

[quote="ZachTetra, post:1, topic:79949"]
impossible to slip
[/quote]

Definitely possible...

There are tons, tons of 5045 5055 6345 6355 motors that will fit dual in the 100-220 kv range.
Just randomly click on build threads and you'll find then in mins. Or use search.
```

---
## \#12 Posted by: J0ker3366 Posted at: 2019-01-05T20:10:52.584Z Reads: 88

```
Paris mounts. I forgot you said that. 180mm caliber II will hold xx54 for sure. Just make sure your trucks are at least 180mm
```

---
## \#13 Posted by: J0ker3366 Posted at: 2019-01-05T20:11:27.355Z Reads: 92

```
You could always run one forward mount and the other reverse mount.
```

---
## \#14 Posted by: Skunk Posted at: 2019-01-05T20:12:49.163Z Reads: 99

```
https://buildkitboards.com/collections/motors/products/6354-208kv-motor

https://longhairedboy.com/collections/all/products/totally-bitchin-190kvs-6355-electric-skateboard-motor

collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-01-05T21:52:33.411Z Reads: 88

```
Thanks for showing me these!  I'm not 100% if they fit, I don't immediately see the length with axles, but it's something I can look deeper into.  These seem awfully powerful since I'm using 2 of them, is there a certain scale factor that is condusive to motor longevity?  I can't afford top of the line motors unless there's a good reason for it.
```

---
## \#16 Posted by: Skunk Posted at: 2019-01-05T22:00:09.301Z Reads: 85

```
The nice thing about these is all of these sellers are members on the site.
Im personally a maytech fanboy atm. 
@hyperIon1 @hyperIon2 is about to get more stock in as well and would have a 6354/55 that would work. (They sell maytech)
I go for quality motors because my esk8 is my car. There are less expensive motors for sure, but buy cheap.... buy twice (hobby king isnt bad tho)
Notice all the motors i posted don't have those little nipples at the end. That makes a big difference when using standard skateboard trucks going dual.
```

---
## \#17 Posted by: ZachTetra Posted at: 2019-01-05T22:47:04.559Z Reads: 81

```
Do you just slide hub motors over the existing axle and the square pocket on the inner face indexes with the truck ends?
```

---
## \#18 Posted by: Skunk Posted at: 2019-01-05T22:48:22.011Z Reads: 81

```
Oh i don't use hubs. I like full urethane.  Belts, gear, direct drive.
```

---
## \#19 Posted by: ZachTetra Posted at: 2019-01-05T22:49:07.631Z Reads: 81

```
Do they not have enough power or not absorb impact or something?
```

---
## \#20 Posted by: Skunk Posted at: 2019-01-05T22:50:28.123Z Reads: 84

```
For one I like being able to swap out wheel types and sizes when I want to.
Plus there's just more urethane between you and the road. Streets suck where i live.
```

---
## \#21 Posted by: ZachTetra Posted at: 2019-01-05T22:57:34.830Z Reads: 76

```
All brushless outrunners will be waterproof but will suffer from dust and gravel right?
```

---
## \#22 Posted by: Skunk Posted at: 2019-01-05T23:00:29.005Z Reads: 76

```
By design yeah.
I read some members wash their Motors out with distilled water after grimy trips.
Some guys use polyurethanes or other types of coatings on the inside of the motors for Extra Protection.
There's also a number of sealed Motors but water with Brin will still get in and require some maintenance to keep from failure if you're riding in bad weather
```

---
## \#23 Posted by: ZachTetra Posted at: 2019-01-05T23:04:47.809Z Reads: 73

```
Is it worth looking for sensored or sealed motors?  Theres usually light rain in this part of the world so the ground has lots of small puddles
```

---
## \#24 Posted by: Sascha_stevenson Posted at: 2019-01-05T23:10:55.271Z Reads: 70

```
That Turnigy SK8 ESC is rubbish, it just can't handle anything. Try find something like a used focbox. Ask around on the forum! Create a wanted items post. It really helps to cut down the cost. I only use sealed motors. looks great tho :wink:
```

---
## \#25 Posted by: Skunk Posted at: 2019-01-05T23:11:23.014Z Reads: 69

```
I'm honestly unsure. im relatively new to all this.
There's a lot of good threads that discuss waterproofing (the best you can)  your motors and board.
```

---
## \#26 Posted by: ZachTetra Posted at: 2019-01-05T23:12:43.114Z Reads: 65

```
Is it something about this kind of ESC (are there certain characteristics I should look for) or this ESC in particular (its a rip off because its actually kinda trash)?
```

---
## \#27 Posted by: Sascha_stevenson Posted at: 2019-01-05T23:13:17.353Z Reads: 62

```
You can't go wrong with a focbox, Look for a VESC
```

---
## \#28 Posted by: Skunk Posted at: 2019-01-05T23:13:53.418Z Reads: 61

```
Most guys go for vesc.
```

---
## \#29 Posted by: Noob-at-building Posted at: 2019-01-06T05:35:18.251Z Reads: 59

```
Yea i am just messing around :slight_smile:
```

---
## \#30 Posted by: Noob-at-building Posted at: 2019-01-06T08:15:05.727Z Reads: 58

```
I have herd that the multistar batteries are not that reliable, so i would much rather you get a reliable brand like turnigy or smc
Also keep in mind the 6s batteries are quite big so if you don't mind having an enclosure that is bulky at one end, go ahead
```

---
## \#31 Posted by: ZachTetra Posted at: 2019-01-06T13:42:37.053Z Reads: 58

```
Is there anything you know about the types of batteries Turnigy or SMC make?  I've heard bad things about the compact series getting puffy and such.
```

---
## \#32 Posted by: Noob-at-building Posted at: 2019-01-06T23:16:37.822Z Reads: 55

```
It depends how much you are willing to pay for a set of batteries,
i would recommend getting the Turnigy Graphene Panther or just the Turnigy Graphene batteries becasue they have a batter build quality, higher discharge and charge rate and better cycle life averaging around 600+ that they have stated.
If your looking to go on the cheap side of things and not get an expensive battery, like a am doing.
If you where to go 12s i would recommend a 3s battery like this
https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack-xt-90.html?wrh_pdp=3

or if you want a 2s battery for a slimmer enclosure
https://hobbyking.com/en_us/turnigy-5000mah-2s-20c-lipo-pack-xt-90.html
The 3s Turnigy 5000mah batteries are very reliable as @AdamE3399 has multiple sets of these in his boards and has ran them well over what they should be rated for and has not had a single lipo puff or break.
if you plan to go higher than a 3s i would not recommend going any higher  because it just makes the lipos very big and bulky and you will end up hitting lots of things on your board if you do not use any riser pads.
```

---
## \#33 Posted by: Noob-at-building Posted at: 2019-01-06T23:30:06.990Z Reads: 56

```
[quote="ZachTetra, post:23, topic:79949, full:true"]
Is it worth looking for sensored or sealed motors? Theres usually light rain in this part of the world so the ground has lots of small puddles
[/quote]


Motors are already water proof although stay out of puddles for safety, and i would not recommend going with a sensored motor if possible only because you probably wont be using it if you get a vesc. the hole point of a vesc is for it to take a  sensorless motor and make if feel sensored on the other hand if you have a shit Chinese esc then definitely try to find a sensored motor
```

---
## \#34 Posted by: Noob-at-building Posted at: 2019-01-06T23:37:30.190Z Reads: 53

```
With the hobbyking vesc 4.12 i wouldn't recommend going with it as it is very over priced,
instead go with a flipsky vesc 4.12 or higher as they are based off the Benjamin Vedder 4.12 design as well
another benefit is that they are like half the price :)
```

---
## \#35 Posted by: Noob-at-building Posted at: 2019-01-06T23:42:01.380Z Reads: 59

```
[quote="ZachTetra, post:31, topic:79949, full:true"]
Is there anything you know about the types of batteries Turnigy or SMC make? I’ve heard bad things about the compact series getting puffy and such
[/quote]


Sorry forgot to mention but Zippy is the brand that make the compact series which frankly are very shit[DO NOT GET ZIPPIES] Turnigy and smc are to very well know brands that have little to no fails.
```

---
## \#36 Posted by: ZachTetra Posted at: 2019-01-07T00:43:36.038Z Reads: 62

```
@Noob-at-building I've done some more hunting around the old forum posts after looking at the replies (which I really appreciate from everyone!!), and I think this is the new plan...

2x 6355 260Kv from DIYES and a dual FSESC 4.20 with a 7:12 sprocket and chain ratio (30mph loaded)

Those motors are sealed which puts me at ease since the bottom of the board usually has a thin layer of gritty mud stuck to it.  They are sensored and can pull more amps than the ESC can push so I'll set it to disable sensors after startup and limit the cruising speed to 50 amps.  I don't think I'll pull more than 2 kilowatts after startup for long so I'm not too worried (I'm making an aluminum finned case so it should sync off most heat pretty fast).

The batteries are a bit tricky, I will go over a fair amount of hills so I need capacity but it's primarily a suburban college campus rider I need to carry to class (and I can't bench press a pillow) so it needs to be light, and I can't afford the cost of high end racing batteries or the space for enough 18650s or 26650s without some compromising the integrity and aesthetics of the deck.

If I split a 6s2p Lipo into 6 pairs of 2 in parallel then re-series them with the thermocouple in the pair closest to the charging lead (changing the length affects the resistance) then I can create flanged aluminum housings for each pair and bolt them down the deck to keep it thin.  I did the math and I can do 6 pairs of 2 with space for wire/bolts/ESC/transceiver but not as 12 individual packs.  What ever the battery is I need to charge off a 6s Lipo charger and have at least 150Wh, and I need it to flat pack otherwise I'll get beached on my own batteries.

I'm thinking the 12000mah 15c Turnigy Graphene as it looks like a very good deal, (please tell me if there's something better for long term that isn't awful upfront) but I can't tell if I can split it apart safely yet.  It should add 15mm to the bottom of the deck (10mm for 1/6 of the battery, 2mm for an aluminum housing, and 3mm of low density rubber against the deck to give the cells some room to expand and the housing to bend) and half the usable real estate of the under deck.



It'll tack on another $145 which I'm not particularly chuffed about but it looks like it will be less on fire for longer

products/electric-skateboard-motor-6355-260kv
https://flipsky.net/products/dual-fsesc4-12-100a 
https://hobbyking.com/en_us/turnigy-graphene-professional-12000mah-6s-15c-lipo-pack-w-xt90.html?wrh_pdp=3


PS: Do I need a programming card for the ESC or just stick it to my laptop and give it some number poking until I only die occasionally on stop and start?
```

---
## \#37 Posted by: venom121212 Posted at: 2019-01-07T00:46:11.603Z Reads: 57

```
No card needed. It's just a bldc software you can find from flipsky. Then set all numbers that make sense to you. Thennnnnnn poke numbers til you don't die
```

---
## \#38 Posted by: ZachTetra Posted at: 2019-01-07T00:48:28.451Z Reads: 58

```
Will the board run with something plugged into it?  If I can I'm gonna stick the laptop to the nose of the deck and change the numbers slowly up on the go  :P
```

---
## \#39 Posted by: venom121212 Posted at: 2019-01-07T00:51:46.595Z Reads: 58

```
Depends entirely on the controller. Most are smart enough to cut motor power while charging.
Another plug for the focbox unity.. It has an app for on the go quick tuning.
```

---
## \#40 Posted by: J0ker3366 Posted at: 2019-01-07T00:58:25.253Z Reads: 56

```
There is nothing wrong with Multistar lipos. @MoeStooge is running four 4s of those and he's no problems. Most cases of them being bad is people using them out of their specs range. Meaning over discharging and pulling more amps than the lipos allow. Treat any lipos like this and it will fail.
```

---
## \#41 Posted by: Noob-at-building Posted at: 2019-01-07T01:46:27.039Z Reads: 51

```
Okay sorry i just have herd some bad reviews on them, ill check up on that :slight_smile:
```

---
## \#42 Posted by: ZachTetra Posted at: 2019-01-07T01:49:51.263Z Reads: 50

```
Does anyone have recommendations for the cheapest way to charge an 8s?  I've got the space and the parts can handle the power but all the chargers are expensive and the BMS chargers have me spooked (and I don't understand buying from Bestech).  I don't need the speed but I'd like the extra capacity
```

---
## \#43 Posted by: Noob-at-building Posted at: 2019-01-07T01:55:33.344Z Reads: 52

```
Are you thinking about bypassing the bms discharge?
```

---
## \#44 Posted by: ZachTetra Posted at: 2019-01-07T02:02:54.221Z Reads: 54

```
If I get an 8s BMS, can I wire all the cells to it and have a port for a DC power source and let it do its thing or do I need to watch the voltage to charge and drain?
```

---
## \#45 Posted by: Noob-at-building Posted at: 2019-01-07T04:27:18.275Z Reads: 49

```
A bms is a battery management system, it will make sure the cells are the correct voltage by balancing the cells.
Yes you can plug it in and leave it to charge. 
the balance leads go to each individual cell on your battery so there will be 9 balance leads
B0: 0V
B1: 4.2V
B2: 8.4V
B3: 12.6V
B4: 16.8V
B5: 21V
B6: 25.2V
B7: 29.4V
B8: 33.6V
0 to 8 is 9 wires
also keep in mind you will need a 8s  or 33.6volt charger
```

---
## \#46 Posted by: Noob-at-building Posted at: 2019-01-07T04:29:23.908Z Reads: 48

```
For more information @b264 is an expert on bms knowledge just ask for some help
```

---
## \#47 Posted by: MoeStooge Posted at: 2019-01-07T04:43:08.714Z Reads: 48

```
Multistar cautions. I have received a new MS battery with a bad cell out of the box. I have had a cell fail to a zero volt without abuse or misuse while riding.  Had a MS 4s pack catch fire from over discharge. (My fault) They puff quicker than most packs and seem to run a lower amount if charge cycles than higher end packs. That being said, there is no substitute for quality. If your in a budget and do a good job taking care and storing of your Lipo's, MStar will get the job done. You definitely get what you pay for.  I moniter the crap out of all my Lipo's and usually catch irregular cells before a serious problem occurs.  There are pro's and con's here for sure. For racing application the lipo for me makes the most sense. Multistar is ok for upping amp hour by banking cells but not a good idea for delivering reliable high amps alone.
```

---
## \#48 Posted by: ZachTetra Posted at: 2019-01-07T04:49:07.876Z Reads: 45

```
I often get dragged off in the middle of the late afternoon (the joys of dorm life) so I probably can't babysit a pack charging, should I try to stay away from MS packs if possible? And if so is there something very stable you're aware of?
```

---
## \#49 Posted by: Noob-at-building Posted at: 2019-01-07T04:52:06.085Z Reads: 49

```
[quote="ZachTetra, post:48, topic:79949"]
I often get dragged off in the middle of the late afternoon (the joys of dorm life) so I probably can’t babysit a pack charging
[/quote]
You dont have to if you use a bms, just plug and play
```

---
## \#50 Posted by: ZachTetra Posted at: 2019-01-07T04:54:32.982Z Reads: 48

```
Do you use them?
```

---
## \#51 Posted by: Noob-at-building Posted at: 2019-01-07T04:55:40.410Z Reads: 48

```
My mate uses them, and so does everyone else that knows what they are doing.
i am in the middle of building my own board and i am using a 12s 100a continues bms
```

---
## \#52 Posted by: Noob-at-building Posted at: 2019-01-07T04:57:30.749Z Reads: 45

```
are going to bypassing or safely discharge you battery through your bms
```

---
## \#53 Posted by: ZachTetra Posted at: 2019-01-07T04:58:24.891Z Reads: 45

```
Is there anything different between a balance charger and BMS except for the case?  I know some chargers will tell you if a cell is bad but I'm not sure if a BMS has any way to be controlled or give feedback
```

---
## \#54 Posted by: ZachTetra Posted at: 2019-01-07T04:59:28.042Z Reads: 43

```
I really don't understand how a BMS works...I know is a PCB with fancy bits but it's totally black box to me
```

---
## \#55 Posted by: Noob-at-building Posted at: 2019-01-07T05:00:50.547Z Reads: 45

```
A balance charger is slightly different form a bms
A bms chargers all cells up to a certain point and then balances the cells where as a balance charger balances the cells and then starts to charger whilst still balancing the cells if one goes out of sync
```

---
## \#56 Posted by: ZachTetra Posted at: 2019-01-07T05:01:50.236Z Reads: 46

```
Is there any advantage to a BMS besides cost and convenience of charging?
```

---
## \#57 Posted by: Noob-at-building Posted at: 2019-01-07T05:06:05.033Z Reads: 49

```
It usually takes less time as they charge the cells first, this inst always good as some cells will naturally go out of sync
```

---
## \#58 Posted by: Noob-at-building Posted at: 2019-01-07T05:06:50.261Z Reads: 46

```
Oh and also you don't have to unscrew your enclosure every time you want to charge your boards
```

---
## \#59 Posted by: ZachTetra Posted at: 2019-01-07T05:07:59.865Z Reads: 42

```
Is there anything that will keep cells balanced and use a cheap charger to add power or would that be dumb?
```

---
## \#60 Posted by: Noob-at-building Posted at: 2019-01-07T05:09:32.221Z Reads: 41

```
The chance of a cell going out of balance is slim btw unless you have a really shit $1 bms
and you need a 8s or 33.6v charger to charge the board
```

---
## \#61 Posted by: ZachTetra Posted at: 2019-01-07T05:11:41.824Z Reads: 48

```
How do you discharge through a BMS? Is there a button or switch and it dissipates heat until the voltage drops then stops?
```

---
## \#62 Posted by: Noob-at-building Posted at: 2019-01-07T05:15:07.344Z Reads: 48

```
![image|500x500](upload://vSehibjplV5tPgTRqco6S6KNo8C.jpeg) 
through this, btw bypassing discharge is not recommend it is only used if you use a bms that cant handle you battery amps
```

---
## \#63 Posted by: b264 Posted at: 2019-01-07T05:17:27.484Z Reads: 46

```
Sometimes it's recommended.  There are pros and cons both ways.  And you can only do it if your ESC has low-voltage cutoffs, like any VESC derivative for example.  Most of the cheap china ESC do not have that, or if they do, it's not adjustable in any way and thus I would not use it.

I like to know if my battery is fully charged and I hit the brakes, I would prefer to overcharge the battery instead of have a brake failure
```

---
## \#64 Posted by: Noob-at-building Posted at: 2019-01-07T05:19:45.165Z Reads: 45

```
True.
 im looking at this 8s bms and it says in the description [supply voltage 7.4] how would that work?
```

---
## \#65 Posted by: ZachTetra Posted at: 2019-01-07T05:19:45.841Z Reads: 46

```
Where does the power go when you drain a lipo?  I imagine it turns to heat but I never see massive heat syncs on BMSs
```

---
## \#66 Posted by: Noob-at-building Posted at: 2019-01-07T05:22:33.254Z Reads: 40

```
what do you mean by that?
do you mean when a lipo is fully discharged?
or when it is currently been used, cause that goes to the vesc/esc which goes to the motors.
```

---
## \#67 Posted by: ZachTetra Posted at: 2019-01-07T05:24:48.529Z Reads: 41

```
If the esc is legit then it shuts off when the batter voltage is to low but if the battery is to be stored then it's supposed to be drained and I though you used a BMS or charger to drain what ever is left in the pack (until it's down to the storage voltage)
```

---
## \#68 Posted by: Noob-at-building Posted at: 2019-01-07T05:26:32.582Z Reads: 42

```
storage voltage is around 3.8 for lipos i think, a bms doesn't discharge like that btw it is talking about going to the motors to power them not discharging in the way of wasting energy or turning into heat
```

---
## \#69 Posted by: ZachTetra Posted at: 2019-01-07T05:28:04.831Z Reads: 40

```
So the batteries all go to the BMS and the esc pulls from the BMS?
```

---
## \#70 Posted by: Noob-at-building Posted at: 2019-01-07T05:29:22.187Z Reads: 41

```
in a way yes
```

---
## \#71 Posted by: ZachTetra Posted at: 2019-01-07T05:31:24.689Z Reads: 40

```
My brain aches and I fear I will set my house on fire soon, but thanks for bearing with my ignorance.  I sort of get it so I think I can research details on my own
```

---
## \#72 Posted by: Noob-at-building Posted at: 2019-01-07T05:32:51.393Z Reads: 40

```
if you connect the bms correctly you can plug in the charger let it sit for the time,  say it takes 2hours you could come back 5 hours later and it would be fine.
```

---
## \#73 Posted by: ZachTetra Posted at: 2019-01-07T05:35:37.826Z Reads: 42

```
If you have a BMS and a AC to DC adapter if the charged voltage if the pack, is there anything else you need or should have to get the best performance from you packs?
```

---
## \#74 Posted by: Noob-at-building Posted at: 2019-01-07T05:39:38.742Z Reads: 43

```
All you need is these
Charger
https://www.aliexpress.com/item/Yangtze-33-6V-4A-5A-6A-Lithium-Li-ion-Battery-Charger-For-29-6V-30V-Lipo/32838587192.html?spm=2114.search0104.3.22.21936e80rpRKP2&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_10130_10547_319_317_10548_10696_453_10084_454_10083_10618_10307_537_536_10131_10132_10133_10059_10884_10887_100031_321_322_10103,searchweb201603_52,ppcSwitch_0&algo_expid=39893841-5f4e-41a8-8016-3b11b0b2f12f-3&algo_pvid=39893841-5f4e-41a8-8016-3b11b0b2f12f
and the bms
https://www.aliexpress.com/item/8S-50A-29-6V-PEAK-200A-li-ion-BMS-PCM-battery-protection-board-with-balancing-bms/32815791835.html?spm=2114.search0104.3.204.1aa3722737oVqD&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_10130_10547_319_317_10548_10696_453_10084_454_10083_10618_10307_537_536_10131_10132_10133_10059_10884_10887_100031_321_322_10103,searchweb201603_52,ppcSwitch_0&algo_expid=12c45339-a414-41b4-8216-86f4ddfc83ae-30&algo_pvid=12c45339-a414-41b4-8216-86f4ddfc83ae
```

---
## \#75 Posted by: Noob-at-building Posted at: 2019-01-07T05:40:32.640Z Reads: 37

```
you don't need and ac to dc converter
```

---
## \#76 Posted by: b264 Posted at: 2019-01-07T05:46:18.400Z Reads: 41

```
[quote="ZachTetra, post:65, topic:79949, full:true"]
Where does the power go when you drain a lipo? I imagine it turns to heat but I never see massive heat syncs on BMSs
[/quote]

Bipolar transistors get really hot running power through them because of their voltage drop, but newer FET devices have no set voltage drop and act more like a 50mOhm resistor and hence don't burn off near the amount of power as-of it was, say, a 0.7V drop across the device.  At 50A that would be 35W burnt-off as heat right in the junction.  But with a MOSFET 50A running through it is more akin to 2W burnt-off as heat in the device or about 20 times more efficient.  Those numbers are all examples and each device is different.

Most of the power ends up converted to mechanical energy, but a lot of it gets burnt-off as waste heat inside your motor.
```

---
## \#77 Posted by: ZachTetra Posted at: 2019-01-07T13:01:42.599Z Reads: 42

```
So how do you drain a Lipo for storage? Do you sit the board on a chair and run the motors for 20 minutes?
```

---
## \#78 Posted by: b264 Posted at: 2019-01-07T23:10:13.247Z Reads: 40

```
Why not ride it :smirk:
```

---
## \#79 Posted by: Noob-at-building Posted at: 2019-01-07T23:49:35.691Z Reads: 40

```
if you storing lipos for a long time i think the voltage should be around 3.8
```

---
## \#80 Posted by: venom121212 Posted at: 2019-01-07T23:56:45.821Z Reads: 42

```
You could hook it up to a single led and drain it too
```

---
## \#81 Posted by: b264 Posted at: 2019-01-08T00:13:43.963Z Reads: 43

```
Or a 1500 ohm resistor but you can't leave it connected too long.  Only a week or two until it gets down to 3.8V
```

---
## \#82 Posted by: ZachTetra Posted at: 2019-01-08T02:06:52.181Z Reads: 52

```
Does anyone have recommendations for sealed and sensored xx45 to xx55 motors meant for 22.2V and less than 50A continuous/150A burst?  Anything from 150kv to 450kv is acceptable (I can get 8 to 24 tooth sprockets).  I'd like to be able to ride through the rain and there's a lot of grit that I don't want in the can, but I would rather have the oomph since brushless motors are waterproof and I can wash them now and then.

Whatever motor it is it needs to go with  the dual FSESC 4.20 but if the connectors don't match I'll just make an extender wire but I absolutely can't have anything get toasted, I can only afford parts once.

I did a test getting dragged by a car with a force gauge and I can safely do up to 10N-m of torque total after gearing (3m/s/s or 6.7MPH/s on 90mm wheels)

What would be perfect is torque (N-m) = 750 / kv so...
150kv and 5N-m
300kn and 2.5N-m
450kv and 1.67N-m
...and so forth

The BKB 6354 208kv looks good but the torque isn't listed and Jared can't give me numbers
https://buildkitboards.com/collections/motors/products/6354-208kv-motor

The FlipSky 6354 190kv looks good (78% extra kick) but its still has open vents and I've heard of people getting a different (but sealed) motor so I'm not sure
https://flipsky.net/collections/e-skateboard/products/6354-190kv-2450w-2

The TB 6355 260kv from DIY ESB looks okay but its a little under powered
collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-260kv

The KEDA 5663 196kv from HK, SK3 5045 540kv, and G60 300kv are wide open and have no torque ratings, looking at the high voltage SK3s from someones testing they seem a bit weak so I don't have high hopes
https://hobbyking.com/en_us/kd-53-20-brushless-outrunner-195kv.html
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5045-450kv-brushless-outrunner-motor.html
https://hobbyking.com/en_us/turnigy-g60-brushless-outrunner-300kv-60-glow.html

The MicHobby sealed motors are to long for my trucks and Maytech's are expensive 

I see a lot of motors but they are all higher voltage and I think getting a 40V motor and feeding it 22V is kinda inefficient and a waste of money.  Do you guys think I would be better off getting a bigger pack like a 10s and a BMS?  I already have access to iMax B6s from roommates and I don't want to spend money unless I have to.

PS: sorry if my posts are incoherent
```

---
## \#83 Posted by: Noob-at-building Posted at: 2019-01-08T04:41:32.788Z Reads: 44

```
Go with the TB 6355 260kv motors
they will be perfect for your build
```

---
## \#84 Posted by: Noob-at-building Posted at: 2019-01-08T04:44:47.062Z Reads: 45

```
If you do want to go with 10s or even 12s i would recommend going with the TB 6355 190kv motors as they can handle 10-12s unlike the 260kv which cant
```

---
## \#85 Posted by: b264 Posted at: 2019-01-08T04:51:26.362Z Reads: 45

```
The [3D Servisas calculator](https://calc.3dservisas.eu/) has N&middot;m
```

---
## \#86 Posted by: ZachTetra Posted at: 2019-01-08T14:33:00.642Z Reads: 44

```
Why do you think the TBs are the best?
```

---
## \#87 Posted by: Noob-at-building Posted at: 2019-01-09T01:21:12.919Z Reads: 38

```
Cause they have a higher kv which is better if you are going for a 1:3 gear ratio. they are mainly used if you are going with 6-8s builds as well.
```

---
## \#88 Posted by: ZachTetra Posted at: 2019-01-09T04:05:14.544Z Reads: 36

```
I was testing the 3DSerivas site and it's giving way higher torque for motors that specify what it should be, also is the listed torque at the max amps?
```

---
## \#89 Posted by: ZachTetra Posted at: 2019-01-09T04:07:32.828Z Reads: 36

```
The kv doesn't matter as long as the kv is enough I can gear it, I haven't gotten the sprockets yet, what matters is if it has the torque for high acceleration, any idea if it's what's listed on BKB?  (2.56N-m @ 65A)
```

---
## \#90 Posted by: b264 Posted at: 2019-01-09T04:11:38.892Z Reads: 37

```
Torque is in about 8 places, so it's difficult to say.  You'd have to be more specific.  Make sure you fill in the max motor wattage you want to run, maybe like 2kW per motor.  I'm still trying to wrap my head around the new calculator after the good one disappeared from the internets
```

---
## \#91 Posted by: ZachTetra Posted at: 2019-01-09T04:17:42.527Z Reads: 38

```
I made sure all the battery/motor/gear train boxes were properly filled out and accounting for less voltage so I'm not sure what's wrong...I just wish these companies would release their dynamo data, I know they have it because my dad works with some the companies that make BLDC motors for other uses and they always have the measurements for RPM and torque at every voltage, amperage, and load combination
```

---
## \#92 Posted by: Grozniy Posted at: 2019-01-09T07:28:42.039Z Reads: 36

```
It will be a hover board :rofl:
```

---
## \#93 Posted by: ZachTetra Posted at: 2019-01-09T20:47:05.017Z Reads: 34

```
Does it matter which transmitter and receiver I get? There's a $25 set on Amazon with both and I think it's enough but don't know if you can rebind the controls through the ESC.  And is it worth getting an antispark connector?
```

---
## \#94 Posted by: mynamesmatt Posted at: 2019-01-09T22:43:56.635Z Reads: 35

```
[quote="Sascha_stevenson, post:24, topic:79949"]
That Turnigy SK8 ESC is rubbish, it just can’t handle anything.
[/quote]

[quote="Sascha_stevenson, post:27, topic:79949"]
Look for a VESC
[/quote]
bruh the sk8 esc IS a vesc....
```

---
## \#95 Posted by: Sascha_stevenson Posted at: 2019-01-09T22:56:14.724Z Reads: 34

```
Yes, a very very shit VESC
```

---
## \#96 Posted by: ZachTetra Posted at: 2019-01-09T22:56:30.202Z Reads: 35

```
Is the Turnigy esk8 a good vesc and will it be on fire if I give it 2 motors to power?
```

---
## \#97 Posted by: ZachTetra Posted at: 2019-01-09T22:57:00.348Z Reads: 34

```
Hmm...gonna take that as a no
```

---
## \#98 Posted by: AdamE3399 Posted at: 2019-01-09T23:15:22.320Z Reads: 34

```
Ive been using the turnigy vesc for 6 months on 12s without a single problem, and for people who say their shit, they are based on the same design as other 4.12 vescs and are in my experience built better than flipsky 4.12's
```

---
## \#99 Posted by: mynamesmatt Posted at: 2019-01-10T02:44:52.456Z Reads: 33

```
dude where is your evidence regarding this? my dad and i run dual 6374's on these at 10s and they're perfect?
```

---
## \#100 Posted by: ZachTetra Posted at: 2019-01-10T02:50:49.673Z Reads: 35

```
Are you using one sk8-esc for each 6374?
```

---
## \#101 Posted by: mynamesmatt Posted at: 2019-01-10T02:56:05.865Z Reads: 37

```
yeahp, you have to. Cant really use one esc for 2 motors
```

---
## \#102 Posted by: ZachTetra Posted at: 2019-01-10T03:02:12.595Z Reads: 39

```
Would you recommend it over the FlipSky 4.20 50A FSESC or the Torque Boards 50A ESC?
```

---
## \#103 Posted by: mynamesmatt Posted at: 2019-01-10T04:27:09.163Z Reads: 33

```
not sure, i think quality wise they're very similar. I think someone said something about the fsesc having issues but idk
```

---
## \#104 Posted by: Sascha_stevenson Posted at: 2019-01-10T22:27:58.202Z Reads: 36

```
@mynamesmatt
 I’ve used that Turnigy SK8-ESC on my single set up and it worked better as a cooker than it did a vesc. If you want to be able to make an omelette on the go use that. Just trying to say, get quality parts like a Focbox, something that people are able to help you out with if you run into problems in the future. Not trying to cause an argument :wink:
```

---
## \#105 Posted by: mynamesmatt Posted at: 2019-01-11T04:01:36.860Z Reads: 34

```
nah not trying to cause an argument, but a 4.2 vesc with no cooling on a single setup is a one way street to getting hot.
```

---
## \#106 Posted by: Noob-at-building Posted at: 2019-01-11T08:03:22.126Z Reads: 30

```
[quote="ZachTetra, post:93, topic:79949, full:true"]
Does it matter which transmitter and receiver I get? There’s a $25 set on Amazon with both and I think it’s enough but don’t know if you can rebind the controls through the ESC. And is it worth getting an antispark connector?
[/quote]
It doesn't really matter what transmitter and receiver you get, but try to get a combo with both.
 Having an anti-spark will be very useful as your vesc will always use power in sleep mode ruffly around 100mA. So having an anti-spark loop key will save battery life over time because if you left it in over night your battery would be dead by morning
```

---
## \#107 Posted by: ZachTetra Posted at: 2019-01-11T09:04:15.280Z Reads: 24

```
But is it worth $20 for the ESC with the antispark built in, $15 for the inline version, or is there a type of connector that's good enough?
```

---
## \#108 Posted by: Noob-at-building Posted at: 2019-01-11T09:19:48.463Z Reads: 22

```
Just using an xt-90 anti spark for a loop key is fine for a vesc/esc that doesn't have one built in. 
And what esc/vesc are you looking at getting?
```

---
## \#109 Posted by: ZachTetra Posted at: 2019-01-11T09:22:00.385Z Reads: 24

```
FlipSky dual FSESC 4.20
```

---
## \#110 Posted by: ZachTetra Posted at: 2019-01-11T09:23:05.307Z Reads: 24

```
It's one of the cheaper high rated dual ESCs with all the other connections and wires factored in and that's pretty important
```

---
## \#111 Posted by: Noob-at-building Posted at: 2019-01-11T09:27:00.949Z Reads: 26

```
Okay thanks
```

---
## \#112 Posted by: Noob-at-building Posted at: 2019-01-11T09:27:31.357Z Reads: 28

```
So do you know what parts you are going with yet?
```

---
## \#113 Posted by: ZachTetra Posted at: 2019-01-11T09:35:04.559Z Reads: 29

```
Minority 40" drop deck
90mm glowing wheels
clamp on spikes for rain and snow (might sell these)
180mm Paris trucks
dual fsesc
2 fs 6354 190kv
         or
2 tb 6355 260kv
6s 12ah graphene lipo flat packed w/ xt60
aluminum box plate battery covers for each cell in series
cheap rc transmitter/receiver
custom wrist motion redesign for transmitter (might sell these too)
battery alarm
borrowed IMAX b6s
custom steel motor mounts
motorcycle sprocket and chain
neon purple led underglow
high intensity led headlights
mechanical friction pad brakes
spark scraper
carrying handle and strap

Probably $550 with the superfluous stuff and not counting stuff I already have ($80)
```

---
## \#114 Posted by: DerelictRobot Posted at: 2019-01-11T09:38:35.980Z Reads: 27

```
[quote="Noob-at-building, post:112, topic:79949, full:true"]
So do you know what parts you are going with yet?
[/quote]

ENERTION EVERYTHING.
```

---
## \#115 Posted by: ZachTetra Posted at: 2019-01-11T09:41:17.674Z Reads: 25

```
I can't afford high quality ESCs or full drive kits
```

---
## \#116 Posted by: DerelictRobot Posted at: 2019-01-11T09:42:07.208Z Reads: 25

```
[quote="ZachTetra, post:115, topic:79949, full:true"]
I can’t afford high quality ESCs or full drive kits
[/quote]

YOU CAN BUY THEM WITH ENERTION DOLLARS
```

---
## \#117 Posted by: ZachTetra Posted at: 2019-01-11T09:45:52.533Z Reads: 23

```
Of which I have E$00.00?
```

---
## \#118 Posted by: Noob-at-building Posted at: 2019-01-11T09:59:22.056Z Reads: 24

```
Are you going to weld the motors mounts to the trucks? or if not how are you mounting them
```

---
## \#119 Posted by: ZachTetra Posted at: 2019-01-11T10:12:14.485Z Reads: 25

```
Gonna machine the mounting plate and adapter then tap the holes and locktite the bolts in...it will damage the trucks but they'll be secure...I might just use aluminum if it's to much work
```

---
## \#120 Posted by: Noob-at-building Posted at: 2019-01-11T10:30:27.129Z Reads: 26

```
There are lots of different types of aluminum that you can use for making a motor mount. Here are the benefits of each type
They both are are really good for motors mounts cause of there high strength 
[ Aluminum 2024](https://www.metalsupermarkets.com/metals/aluminum/aluminum-2024/)
Tensile Strength (PSI) 68,000
Yield Point (PSI) 47,000
Elongation *** 20
Brinell Hardness 120
Typical applications: Aircraft structural components and parts for the transportation industry.
[ Aluminum 7075](https://www.metalsupermarkets.com/metals/aluminum/aluminum-7075/)
Tensile Strength (PSI) 83,000
Yield Point (PSI) 73,000
Elongation 11
Brinell Hardness 150
 Typical applications: Used mostly in aircraft and transportation industries where strength is critical.  Can be used as mold material for the plastics industry
@Boardnamics Uses [Aluminum 7075](https://www.metalsupermarkets.com/metals/aluminum/aluminum-7075/) as some main benefits over [Aluminum 2024](https://www.metalsupermarkets.com/metals/aluminum/aluminum-2024/) is it has a higher Average Corrosion Resistance than [Aluminum 2024](https://www.metalsupermarkets.com/metals/aluminum/aluminum-2024/)
Although [Aluminum 2024](https://www.metalsupermarkets.com/metals/aluminum/aluminum-2024/)has an easier Formability / Workability  
Both are really good options for making a motor mount, but [Aluminum 7075](https://www.metalsupermarkets.com/metals/aluminum/aluminum-7075/) is better for the longer run as it last longer in the environment
```

---
## \#121 Posted by: ZachTetra Posted at: 2019-01-11T10:41:22.936Z Reads: 25

```
Oooh thank you!
```

---
## \#122 Posted by: Noob-at-building Posted at: 2019-01-11T10:41:42.017Z Reads: 24

```
Np
10char
10char
```

---
