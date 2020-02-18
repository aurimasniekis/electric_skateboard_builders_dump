# Mountainboard Build

### Replies: 63 Views: 2009

## \#1 Posted by: CoolRextreme Posted at: 2019-01-30T10:38:33.603Z Reads: 340

```
Hey there!
I usually go by "Rex"
Long time stalker of the E-board community since way back in 2015 lol.

I was 17 when I made my first longboard build, and made an instructables to go with it!
(https://www.instructables.com/id/DIY-Electric-Longboard/)

Good days!


Needless to say, times have changed and my budget has really increased.

I started by finishing a second board (Dual 230kv, 12S belt drive w/ dual VESCs, TB Samsung battery, and an LED underglow that is controllable via my phone, all on 97mm wheels). It has been a blast, and a HUGE HUGEEEEE upgrade from my original board in every single aspect (I have yet to be able to charge my phone off it :/)

With two longboard builds done, I am interested in dipping my feet into the world of Mountainboards. I can zip through grass well enough on my longboards, but curb jumps and other simply fun looking tricks one can only do when strapped to a board look like fun, and I want IN!!

My objective is a more versatile curb/terrain friendly board, that that can be used both on and off road. Something on the 'lighter weight' as far as mountain boards go. Hard dirt, dead grassy fields littered with cow poo and gopher holes, skate parks, irrigated almond fields, and pavement will be the types of terrain I will be tackling.
Not much mud expected, and no snow here!
25mph on flat ground is a must. Should be somewhat maneuverable/manageable. 

Having followed the longboard side of things for a while, I find myself severely lacking in the knowledge of mountain boards. If you knowledgeable builders could point me in the right direction I would be much obliged!

As of now, here is what I know so far:

Trampa 16ply Holypro (I am 5'10 and 190lbs)
8 inch Superstars.
Idea's v4.5 motor mounts,15/60 gearing.
x2 6380 170kv motors.
x2 TB VESC

I have multiple 16000mah 4s 12c batteries laying around that I feel ought to be used.
https://hobbyking.com/en_us/multistar-high-capacity-16000mah-4s-12c-multi-rotor-lipo-pack-w-xt90.html

For power, I would like to build my own under-deck battery using these cells. I would build it in a way so that each cell (Possibly two stacked on top of eachother) would run perpendicular to the deck to allow for flex.
Each group of two cells would be protected by a 1/16" thick aluminum sheet should anything strike or grate against them from below

Assuming I have about 24 inches of usable under-board length, I could have 7 perpendicular 3 inch wide 'spaces' to use. 6 of those would be for the groups of cells, and the last one would house a BMS.
@ 2 cells deep, it would add up to be a 12s 16000mAh battery, only an inch thick, and flexible.

The VESC's would be housed in a box above/behind the dual motors w/ an LCD screen and on/off switch.

Also needed is SOME SORT of LED underlighting. That is a must. I've done it twice before, and will do it a third time!! I can wire those in with a BEC easy.
Also a headlight for sure.

Anyway, I have very little detailed knowledge of electrical wiring in terms of building a battery with a BMS, as well as on/off switches and LCD screens lol (More forum hopping will likely help that)

Will it be a problem using 6380 170kv motors with the VESC?

Should I go continue with two 6380 170kv motors with the VESC? I don't seem to see a lot of mountainboard builds with the TB VESC used... Is this because of the amps wanted/needed?
```

---
## \#2 Posted by: taz Posted at: 2019-01-30T10:57:07.705Z Reads: 292

```
First of all welcome.
Now about your build, if you intend on using it as a proper mountain board there are a few things I would change.
1. Go for a top mounted battery. A bottom mounted battery looks really cool and tidy in exchange for reduced clearance and on the first jump or rock you risk destroying you enclosure and batteries.
2. Belts are not ideal for a mountain board if your terrain has rocks. Either go for an enclosed belt drive, a gear drive or chain drive. If you ride mostly on grass, disregard this remark. From your description it may be somewhat acceptable.
3. 15/60 gearing is a little too tall for my liking especially combined with 170kV motors. However this is also terrain dependent so you may be fine.

@dareno Too slow.
I beat you, you old geezer.
```

---
## \#3 Posted by: dareno Posted at: 2019-01-30T10:58:43.081Z Reads: 271

```
[quote="taz, post:2, topic:82563"]
@dareno Too slow.
I beat you, you old geezer
[/quote]

Bahahahahaha!
```

---
## \#4 Posted by: CoolRextreme Posted at: 2019-01-30T11:08:50.549Z Reads: 265

```
Thank you! It feels great to finally be IN the forum as opposed to watching :slight_smile:

 I am not opposed to a top mounted battery. It would simplify things and give added peace of mind

Mostly grass and duft. not a lot of pebbles or rocks, although I have done quite a bit of packed gravel roads with my E-board, and have yet to experience belt difficulties as a result of gravel.

As for gearing, I honestly have no clue for mountain boards. If not for 15/60 then a 14/70 or 15/75 (1/5)?

Edit: Idea offers 15/72. So a 1/4.8 ratio
```

---
## \#5 Posted by: Andy87 Posted at: 2019-01-30T11:13:50.553Z Reads: 261

```
@taz already pointed out the most important things. Top mount battery is a must, chain over belt or even better gear drive if you can.
If you want something on the light side I also wouldn’t go with that big battery packs. 5-8Ah graphens should do a good job and save a lot of weight. If you need more range, take spare packs in your backpack and swap them out.
I don’t have personal experience with multistar packs but I read that they not really made for high drain applications. As you already have them you will know better than me if they good for your purpose or not.
I wouldn’t go with the tb vesc, or as min use a heat sink box for them. 
If you run them with 35a battery max than you can also use smaller motors as you will not gather more power over a 6355 or 6374.
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-30T11:18:10.579Z Reads: 249

```
It’s not only the rocks which can hit your enclosure. I‘m about 170 and bottom out my 16ply trampa when jumping. I know you don’t like to hear it 😅 but I would use a under deck mount really only on the carver or if you plan to cruise with the board. As soon as you want to have serious off-road or jumping plans it’s a big no go.
Yes it looks better, but if you short out your lipos because you hit them on the ground multiple times it’s not really good looking anymore 😬
```

---
## \#7 Posted by: CoolRextreme Posted at: 2019-01-30T11:39:39.536Z Reads: 241

```
I got 4 of those 16000 batteries off a friend who tinkered with RC stuff for cheap. Have been hoping to find a good use for them, but I guess they serve as good paperweights for now. No they are not meant for high drain. But their low C rating is somewhat offeset by their high capacity. You are right though, they ARE heavy!
I'll go the smaller zippy/Graphen route then. I always forget about the "Use a backpack" trick. Honestly I never board without a backpack. I ALWAYS have a small tool set/spare belts/light/charger. Just in case :]

Be cautious about overheating VESCs. Got it.


If I didn't want to hear negatives/other opinions, I would not have posted! :wink:
I'll shoot for 17ply with a top mounted battery and motor mounted VESCs (Or the like)
I do indeed dislike the idea of a big box looking thing between my legs. 
I don't know how long the space between the foot straps is. I'd guestimate a little over a foot. Perhaps I could fit 4 3S batteries side-by-side between my feet for a long/low(er) profile flexible battery housing on top. 

Could I bug you to take a quick peek at the length of that space? :pray:
```

---
## \#8 Posted by: Andy87 Posted at: 2019-01-30T11:43:40.465Z Reads: 210

```
I can’t tell you in foot 😅
But with 30x20cm you on the max you can get.
I think 28x19cm is ok
26x18cm is perfectly fine.
```

---
## \#9 Posted by: Andy87 Posted at: 2019-01-30T11:49:27.038Z Reads: 217

```
About the battery box.
You could go with a pelican case, but it’s big and you need to like how it looks 😅 
There is also the trampa mega box I think it’s called. @taz is using this one and can surely tell you if it’s a good one or not.
If you have access to a 3D Printer you could also print your own boxes like I did for example.
https://www.electric-skateboard.builders/t/ice-crusher-16ply-holypro-4w-chain-drive-mtb-4x-6374-170kv-aps-quad-escape-steering-damper/65823?u=andy87
They fit 2x 6s 5Ah lipos for each case
```

---
## \#10 Posted by: CoolRextreme Posted at: 2019-01-30T11:58:43.557Z Reads: 219

```
That is alright.
Imperial units are dumb anyway. I don't know who thought that something other then the Metric system would be a good idea.
I wish the US ran Metric as a standard of measuring. It makes so much more sense. Just like 24 hour time. :man_shrugging:

Perfect.
With each battery side by side, I would only need a space  28x17cm, which would leave it at a height of about 2.5cm. 

Honestly its not only the look, but alsot the idea of the board feeling more topheavy with a tall box. I like the weight spread out, and the slim look is great as well :) 
I have some aluminum I can cut out and use as for building a flexible housing.

Yes! I saw your build earlier today. It looks amazing, especially with the LEDs. I am always biased towards LEDs. :+1:

Unfortunately I do not have access to a 3D printer. I should really invest in one of those, and soon. I either need to hand craft or buy enclosures, which can be a bit of a pain as neither may easily yield the exact results I want. The closer the better though!

Thank you! I have gotten answers in the last hour, that I did not find in the past few days of looking at Mountainboard Builds!
```

---
## \#11 Posted by: taz Posted at: 2019-01-30T12:31:53.319Z Reads: 187

```
The trampa monster box is exactly what its name suggests. A monster.

http://www.trampaboards.com/monster-box-with-space-for-twin-internal-vesc-made-specifically-to-work-in-conjunction-with-trampas-electric-deck-p-25814.html

It has a lot of space, I fit a 12S7P battery in there and could fit a 12S9P if I wanted to.
I like the fact that it is mounted with 3 bushings on the middle of the deck. This allows the deck to flex as designed and in combination with the electric trampa deck makes for very clean cable routing.
```

---
## \#12 Posted by: CoolRextreme Posted at: 2019-01-30T12:40:02.062Z Reads: 183

```
Oh wow. That IS a MONSTER box! Though a little big for me.
I'll steal that LCD screen though haha.


Perhaps I should use the v6.41 VESCs...
```

---
## \#13 Posted by: venom121212 Posted at: 2019-01-30T12:42:48.431Z Reads: 204

```
Welcome bud! A few things I'll say, I suggest top mount enclosure. I was riding my hybrid mtb on gravel, grass, dirt, etc but am now going full emtb because I got stuck in the woods on some jumps and such. You're on the right path.

If you're considering a 3d printer, get the ender 3. 8.5 x 8.5 x 9" tall print bed can prototype enclosures and its phenomenal quality for the price. Lots of easy upgrades to eventually do too. Only $180 if you can find it at a good deal. Good luck to you man.

Check out diy junction boxes online as well. Decent platform to trick out for a top enclosure.
```

---
## \#14 Posted by: taz Posted at: 2019-01-30T12:48:45.196Z Reads: 207

```
As I said, lots of space.

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/b/5/b5d2c15b1aeb40f9d3fdeca10ce687e6208452b0.jpeg)

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/4/e/4eccc1f49f86ab32f0106ce6862e91151f2c33d7.jpeg)
```

---
## \#15 Posted by: CoolRextreme Posted at: 2019-01-30T13:23:19.861Z Reads: 201

```
Its definitely settled. A (slim light) top mounted battery box! I'll skip out on the bms for now and charge the individual batteries as needed.

Wow, 3D printer advice too! Ill deff poke around in that regard. It would be so helpful, especially for mounts, enclosures, and wheel pullies. 
And countless other things in general life and other builds.

Now to decide vesc 4.something...21? Vs 6.41 vs what others have been using.

Then I should be set for now!
```

---
## \#16 Posted by: Andy87 Posted at: 2019-01-30T14:08:15.825Z Reads: 184

```
Definitely with a vesc4 based I would only consider a focbox 
Better to go with a vesc 6 or vesc 6 based esc or focbox unity.
```

---
## \#17 Posted by: CoolRextreme Posted at: 2019-01-30T22:58:43.404Z Reads: 186

```
Looks like I'll be be pre-ordering the Enertion FOXBOX
https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc

Nervous about doing something other then a VESC, but I will take the 1 year warranty gladly :smile:
Seems to offer some neat tricks. Bluetooth connection, charging ports, 80A continuous.

This'll be fun!

And that is bad business for my card lol :money_with_wings: :moneybag: :money_with_wings:
```

---
## \#18 Posted by: FredrikHems Posted at: 2019-01-30T23:07:57.631Z Reads: 179

```
[quote="CoolRextreme, post:17, topic:82563"]
other then a VESC
[/quote]
The unity is a vesc based controlled. They just cant write VESC in the name because its trademarked by trampa. You’ll have all the futures that any other vesc have, + even more.
```

---
## \#19 Posted by: CoolRextreme Posted at: 2019-01-30T23:37:04.800Z Reads: 181

```
Ohh that makes sense!

Just downloaded the tool for programming the Focbox off Enertion, and its the BLDC tool I used to use for the older VESC lol. 

I have just ordered the Trampa board and FOCBOX. Now I just need to settle details with Idea, and figure out batteries!


And thanks to @venom121212 I now have 3D printer fever :frowning:
```

---
## \#20 Posted by: taz Posted at: 2019-02-01T13:20:56.330Z Reads: 172

```
You need to download the tool for the Unity

https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_TOOL_1.0.exe
```

---
## \#21 Posted by: CoolRextreme Posted at: 2019-02-01T13:28:14.897Z Reads: 160

```
Yes, the focbox bldc tool? I downloaded what was given to me in the confirmation e-mail.

I'm On mobile right now so I cant confirm your link matches what I downloaded.
```

---
## \#22 Posted by: taz Posted at: 2019-02-01T13:29:37.118Z Reads: 155

```
If it looks like the BLDC tool, it most likely is the one for the single Focbox.
The tool for the Unity looks like the VESC tool.
```

---
## \#23 Posted by: CoolRextreme Posted at: 2019-02-01T13:38:31.092Z Reads: 156

```
Intresting. Well I definitely did not buy the singular Focbox lol. In which case they sent me the wrong link. I'll double check when I can, and will try your link.

Thanks! That would have caused me a good deal of confusion later on!
```

---
## \#24 Posted by: CoolRextreme Posted at: 2019-02-05T02:12:49.993Z Reads: 157

```
I have two new members to my little crew!

Today my Trampa board came. (That shipping was fast!) Put it together (which took longer then needed thanks to my failure to realize that four of the washers were smaller then all the others :laughing: )  

It feels so nice to strap the board on. Super secure. I can tell it will be a whole diffrent experience compared to my longboard. 17ply was definitely the way to go.

Picture of it beside my longboard. 

![20190204_175918|666x500](upload://AvjuZtB9mhGP6tMUjEWH4QbmF5m.jpeg) 
Excuse the mess, the package caught me while i was in the middle of rearranging the workshop (aka my bedroom)

Super excited!!


Also managed to pick up the ender 3 off bangood for 170 bucks. Also got a glass plate. Still waiting on the abs and pla filliment.

I was double sure to make sure nothing was bent or leaning one way or another, and that all the wheels were adjusted just so.

Not only will I be able to create the perfect enclousures for my focbox and batteries, but I know I can find some other things to print
Custom phone case would be one of them!

![20190204_180015|375x500](upload://m0LXYJD9tMtcaLNx679NpvU3hBD.jpeg) 

(More mess 😅:roll_eyes:)
```

---
## \#25 Posted by: venom121212 Posted at: 2019-02-05T02:32:20.046Z Reads: 149

```
I'm about to PM you with every upgrade for that printer you should start printing! You won't be disappointed. I love mine and it's already payed for itself. Good call on the glass bed it's phenomenal
```

---
## \#26 Posted by: CoolRextreme Posted at: 2019-02-05T02:35:05.207Z Reads: 152

```
Please do! I already have a list of upgrades (printable and not) i wish to do before printing anything else. Including the fan cover.

Throw me a list. Maybe I have missed something. You would deff know what I need, more then I do. :+1:
```

---
## \#27 Posted by: jippijuk Posted at: 2019-02-05T03:17:36.146Z Reads: 162

```
Hi, maybe there is something from my Mountain board built experience that is "helpfool "

I started in october, reading and getting parts.
And didn't read enough , lol 
Wanted to use my MBS Comp 95 I was riding for some years, just walking up the hills....
Here is what Ive got. 
*  2 Motor Turingy 5035 125kv ( it was a recommendation here from esk8 forum builder)
* 2 zippy lipo 5000 40c in serie = 10C
* mountain board mbs comp95, 8’’ wheels,
* 72 teeth wheel side, 16 motor side, chain driven ( all from electric scooter parts.com, good stuff)
  But 72 Teeth are little to big in diameter for 8" wheels , one reason I would upgrade to 9"  rear wheels ( as you can see in the last picture )
* unity ( needed to buy a cheap laptop because the IOS experimental version is not working here )

Base line is, Im 150 lbs, board is 13kg, Range on paved road is 25 km, with max speed 34km/h

*on trail and gravel with elevation and carving Im down to 16-18 km Range
These motors are definitely to weak and torque is not enough .
I ordered last weekend the sk8 6374 - 149kv, those will boost my set up until my old knees shaking and my already 360 smile changes to 720 degree smile,lol 

Also the old matrix pro Truck is not ideal , Ive tried different egg shocks . But probably ending up buying better Trucks including better more durable top truck hangers.
But this will include new motor mount  and my budget is zero now lol
I definitely like chain driven, a bit noisy , but it just works and doesn't care about dirt .
Second, I would definitely think about where and what I wanna ride - regarding the gearing and the motor rpm. Using a good range calculator is smart .
Also I wasn't really paying attention to the weight whit my built until I did some 17 degree roads uphill-  so for me upgrades and changes will include some thoughts about saving weight . This includes batteries. Also Im tempted to upgrade to 9 inch wheels, because even with the battery pack on the to - clearance is not as much as I thought.
But this upgrade brings lots of extra weight with more rubber in the tires
And BTW - I would NOT use anything else as the unity. Ok , its hilarious and very committing to by a Laptop extra for my board - no regrets "Meister Nadelöhr"
if you have detail questions about my built ... I would love to share 
![IMG_1698|411x485](upload://bRfS09DP7imfFn9Bgq3lqFtNxGd.png) ![IMG_1567|375x500](upload://oOJlxGNTfqB5zRwEiDavbdmfBvJ.jpeg) ![IMG_1678|375x500](upload://a7pZ2i3ARU4d8FUzRQwrWeq5hpl.jpeg)![IMG_1672|374x500](upload://bKPurp0tZGFloUXNz2UxNwPfoCx.jpeg)![IMG_1753|690x459]
```

---
## \#28 Posted by: CoolRextreme Posted at: 2019-02-05T03:42:26.525Z Reads: 153

```
Thank you so much for taking the time to write all that! I have done a ton of reading (Heck, 17 hours of reading just in the past 7 days since I joined the forum. Imagine all the reading that has gone on before joining, as well as on other forums and threads :joy: No doubt days worth of reading time. Maybe even a week.) But that is time I will get back in great rides and sharing pics.
Everyone is SUPER nice here. Joining the eSk8 forum was one of the best decisions :+1:   


[quote="jippijuk, post:27, topic:82563"]
These motors are definitely to weak and torque is not enough .
I ordered last weekend the sk8 6374 - 149kv, those will boost my set up until my old knees shaking and my already 360 smile changes to 720 degree smile,lol
[/quote]
Upgrading from 5035 motors to 6374 motors will be a HUGE jump in power and speed. You are going to have TONS of fun on those! Just do not hurt yourself. You need to stay in once piece so you can keep your 720 degree smile!! :smile: Saving weight will be the least of your worries. No hill will be too steep!

[quote="jippijuk, post:27, topic:82563"]
72 teeth wheel side, 16 motor side, chain driven ( all from electric scooter [parts.com](http://parts.com), good stuff)
But 72 Teeth are little to big in diameter for 8" wheels , one reason I would upgrade to 9" rear wheels ( as you can see in the last picture )
[/quote]
I saw in the picture! The 72 teeth pulley is almost as big as the wheel :grimacing:
Maybe you can just take the tire off and use the chain as a tank wheel!! :rofl: 
I joke, do not do that lol.

Indeed. I have read the pros and cons to chains and belts. I like the quietness of belts, as well as there is no need to oil them! Belt pullies are also much smaller because the teeth are smaller unlike chain pullies. I am conscious of not wanting my belt to be to low and knock against rocks and things.

I definitely like the 8" wheels. They are not to big and not to small for what I will be using them for! I just hope they will not get popped easily by all the dry thorny weeds that grow around in the fields here :grimacing: 



[quote="jippijuk, post:27, topic:82563"]
I would NOT use anything else as the unity. Ok , its hilarious and very committing to by a Laptop extra for my board - no regrets “Meister Nadelöhr”
[/quote]
Haha! At least you got a new laptop out of it! I need a new laptop myself :wink: The one I have right now is 5 years old and very very slow! Right now I use my PC.  

[quote="jippijuk, post:27, topic:82563"]
if you have detail questions about my built … I would love to share
[/quote]
Keep me updated! Let me know of your thoughts when you get those new motors!! I am excited for you :smile: :call_me_hand:
```

---
## \#29 Posted by: Andy87 Posted at: 2019-02-05T03:46:34.158Z Reads: 137

```
[quote="jippijuk, post:27, topic:82563"]
board is 13kg
[/quote]

That’s already a very very good weight.
My quad is 25kg and the dual is 13kg too but with minimal battery I can add and belt drive.
```

---
## \#30 Posted by: jippijuk Posted at: 2019-02-05T07:53:21.030Z Reads: 151

```
A couple more things I would like to share from my first built 
( survived and got some insane fun with some other sport activities, from the darwin law perspective until now ,with 56 of age - I know recovery time is not fun and sucks)
So, the motor mount with both motors creates a rotating force around the truck while excellerating or braking .
 Also with chain drive train , wear of the chain and playing with different sprockets - the motor mount need to be adjustable . 
The motor mount I bought turned out a little bit flimsy and " mickey mouse" , the screws are not meant to use for adjustments, they are "mickey mouse " too.
So I customized the motor mount , drilled new holes, replaced screws and added a reinforcement .
I wanted to tension the chain while the wheels are on - makes sense to me . Using screws with allen key doesn't allow this , because the wheel is in the way. 

Next thing is the safety switch pull plug , in case Im flying of the board , me attached with a line to this plug would cut off the power. I made this out of a XT90 spark connector. In mind that I have also a MAX Blade Fuse 50A.All connections are precise soldered!
After three test rides( anytime I changed batteries I closed the circuit last with this xT90 antispark plug) this XT 90 just blew off with majestic smoke.
some detail pics here. If any input - please .
![IMG_1676|375x500](upload://5SfJ09U2dLmjZ3BEgCoG1jnOtgj.jpeg) 
thats the first reinforcement test 

![DSCN4021|666x500](upload://mjB698C3gBjzDg5stLU2PZkhHZt.jpeg) 
The screw head is on the wheel side for an allan key :/)
I drilled new holes and changed the screws.
![IMG_1675|666x500](upload://ja0mN38Bm5DXu0IJPDqCIKlSiWg.jpeg)
So I can adjust the chain tension with mounted wheel.
```

---
## \#31 Posted by: CoolRextreme Posted at: 2019-02-06T00:59:11.084Z Reads: 136

```
[quote="jippijuk, post:30, topic:82563"]
So, the motor mount with both motors creates a rotating force around the truck while accelerating or braking .
[/quote]
Hmm. I never thought much of this before. You are right. With bigger ties, a bigger load, and a longer distance between the motor and the tire, there will no doubt be much bigger forces then I am used to dealing with in terms of motor mounts. I like your reinforcement! Looks super sturdy :)

Smart move with drilling new holes for the chain adjustment. Seem's a bit funny the motor mount had the screws facing outward on a MTB. There ought to be plenty of space between the tires to get an allen key or ratchet down in there :smile: Well done! :+1:
```

---
## \#32 Posted by: jippijuk Posted at: 2019-02-06T03:15:22.393Z Reads: 134

```
thanks for your :+1: 
BTW - excellent idea taking the wheels of and riding on the sprockets and chain, its like a tank than so much traction :rofl: , way better than any wheel in this freezing weather lol 

one thing I remember that I never thought about when I picked and ordered the motor mount ...
 The width between both motor mount plates at the motor mount frame.
I wanted the wheel sprockets as close to the Tire as much as possible ( nothing gets stuck in there, and keeping the rotational force as close to the hub as possible . ( running the twistar hubs, they were on my board , light weight and seam durable - they seam to work) thats why I put on the outside a counter plate (all aluminum) for reinforcement. 
Also I wanted the motor sprocket as close to the motor mounting plate - less as possible force to the motor bearings. ( as curious as me the fool is - before I mounted the motor , I took the motor apart and was surprised - its a relatively heavy motor 745g the 6374 149kv is 937g, but the seating for the big bearing is kind of plastic .... so I decided to extent the width of the motor mount a bit .
```

---
## \#33 Posted by: CoolRextreme Posted at: 2019-02-09T01:24:14.974Z Reads: 124

```
[quote="jippijuk, post:32, topic:82563"]
excellent idea taking the wheels of and riding on the sprockets and chain, its like a tank than so much traction
[/quote]

I would be lying if I said I had not considered moving a board in other ways, tank treads being one of them :stuck_out_tongue:

Surely there is a way to make a board for the snow :joy:

And oo, nice! How are the 6374s treating you? Too fast and powerful? I hope you are not in a hospital! haha
```

---
## \#34 Posted by: CoolRextreme Posted at: 2019-02-09T01:30:58.727Z Reads: 127

```
Small little build update.


Ender 3 is up and ready to work!

After a bit of bed leveling
Just finished it's first print; the little XYZ test cube! (pencil for size reference)
![20190208_171806|375x500](upload://z44SVEq6qQjXQMTWsexRcx4rhS4.jpeg) 

Came out perfect! (To me at least. Being a newbie I wouldn't know what good and perfect was) Everything is sharp and smooth though! :)

Many thanks to @venom121212 for his helpful Ender 3 advice!
Also Filament Friday and various other youtubers
 

Now to test and dial in any stringing...
```

---
## \#35 Posted by: venom121212 Posted at: 2019-02-09T01:33:37.513Z Reads: 115

```
Necessary pass through thank you to @landonkun for originally hooking me up. And the torch passes on!
```

---
## \#36 Posted by: CoolRextreme Posted at: 2019-02-09T02:22:20.620Z Reads: 122

```
First try with the stringing test

![20190208_181713|375x500](upload://bPahlNWkvndt33qWYOJeDfJgZqc.jpeg) 

Passed with flying colors! :slightly_smiling_face:
Just a 3 or four tiny tiny little blobs on the inside face of the right post. No stringing at all.

No z-hop enabled. Combing enable within infill.
```

---
## \#37 Posted by: telnoi Posted at: 2019-02-09T05:42:04.802Z Reads: 115

```
Quick note, you'll do your vescs a disservice if the heatsink is not in contact with moving air. Depends on how hard or steep you ride, but my dual suffered from thermal throttling in an enclosure. The performance difference was big.
```

---
## \#38 Posted by: CoolRextreme Posted at: 2019-02-09T06:07:00.457Z Reads: 115

```
Thanks for the heads up! VESC cooling is definitely something I will be conscious about. Especially with this build which may have the ability to demand more amperage draw through the VESC. (And considering the enclosure will be made of a meltable material)
I will be designing an enclosure that will allow for as much airflow as I can manage while keeping it semi-water resistant :) Likely a single, or dual PC fans that that pull air through the enclosure over the heatsinks. 
Perhaps I can add some heatsinks to the bottom of the FOcBox as well.
```

---
## \#39 Posted by: jippijuk Posted at: 2019-02-09T17:59:00.159Z Reads: 122

```
Im not in the hospital( knock on wood), in my workshop ( old barn- Im ready for summer)
Regarding the cooling for the motor controller, I put a tube full of "Metal oxideThermal CPU compound heatsink" underneath my Focbox unity to transfer any heat to the metal plate where the unity is sitting on. . 10 bucks at the computer store , I think worth it.
![32%20AM|293x500](upload://xKxNTIFUmzCtB53UMRHqxEeu06c.png) 

Your printer is very cool. did you picked it up new or used?
What do you think about durability of those printed parts?

Ive got my new motors , they are longer in the tube and the higer rpm's - my mounted wheel sprocket is not balanced enough . it wobbles too much. I took everything apart and let my monkey brain smoke how to solve this. Its snowing outside anyway, lol 
I would appreciate your posts about the printer projects and how they turn out .
```

---
## \#40 Posted by: jippijuk Posted at: 2019-02-09T18:15:11.331Z Reads: 119

```
Ok, additional note to my heatsink paste . My unity is in a plastic box.And thinking how to transport the heat outside. So I put a aluminum plate inside the plastic box and screwed this on a aluminum ( exposed to moving air) with two bigger countersunk screws . And put the CPU paste between my unity and the aluminum  plate inside of my box . So I feel prety confident that there is a direct contact to moving air ![56896350553__CACE78B9-52D3-4507-A79C-53665962BBF7|375x500](upload://8q4pgrIghxg0UILJZ3KW9Kkj9T6.jpeg) /Users/surfstefan/Pictures/iPhoto Library.photolibrary/Previews/2019/01/12/20190112-200023/kIfsZQ4QRSyTnJNAIOqAIA/56896350553__CACE78B9-52D3-4507-A79C-53665962BBF7.jpg
```

---
## \#41 Posted by: jippijuk Posted at: 2019-02-26T08:35:58.845Z Reads: 114

```
![image|666x500](upload://rG2EPIOCcizfg9jMXe56X1trrMx.jpeg) cid:D1150618-3703-49B0-87A9-EC5D92CCA9A0@telus
the new Turnigy SK8 6374-149KV Sensored Brushless Motor (14P) is awesome . Love it , better torque, more rpm's and !!!! better range .
```

---
## \#42 Posted by: CoolRextreme Posted at: 2019-03-02T09:54:28.461Z Reads: 110

```
Glad you like em!

Thanks so much for all your commentary. This is definitely helpful.
Have not been logging on much. Currently doing a few 3D printer projects as I wait for all the pieces to slowly trickle in lol. 

I will certainly be figuring out the best way for me to get the heat out from my FOCBOX. I have a few ideas in mind. 
Using CPU paste is a great idea!
```

---
## \#43 Posted by: venom121212 Posted at: 2019-03-02T14:10:49.049Z Reads: 105

```
Unity right?
I bought one of these and it's on the way. Fits the unity very nicely

https://m.banggood.com/22-Tooth-120x69x27mm-Oxide-Aluminum-Heat-Sink-Module-Black-Heat-Radiation-p-1264301.html?rmmds=orderdetail
```

---
## \#44 Posted by: Sn4pz Posted at: 2019-03-02T14:40:58.147Z Reads: 101

```
Are you planning on shortening the fins? They seem quite long
```

---
## \#45 Posted by: venom121212 Posted at: 2019-03-02T14:46:26.216Z Reads: 103

```
Definitely depends on space I have haha
```

---
## \#46 Posted by: totalgeek9224 Posted at: 2019-03-02T15:23:13.735Z Reads: 106

```
Would love to see a list aswell!
```

---
## \#47 Posted by: CoolRextreme Posted at: 2019-03-11T11:03:04.501Z Reads: 104

```
Aye, the Unity. Can't wait till it comes :slight_smile:
I will certainly look into this heatsink. Looks like it'd bleed a ton of heat!
```

---
## \#48 Posted by: CoolRextreme Posted at: 2019-03-26T00:49:30.895Z Reads: 101

```
Its been a while, but the FOCBOX Unity JUST came in the mail! (Literally an hour ago)
**Initial notes;**
XT-60 (Not 90)
Wires and connectors all seem a bit small.
The whole thing is super small actually. Almost concerning so haha.
![20190325_165108|666x500](upload://5MTkefzjeYqGC1oCbJMzVOmDZwk.jpeg) 

Luckily I happened to already have an XT60-XT90 adapter lying around!

I also still had the 5.5mm female bullet connectors that came with the TB Motors/
The FOCBOX came with bullet connectors for whatever size it is (4mm I think? Does not list it on the site)
The nice thing was, the solder end of the 4mm slipped right into the solder end of the 5.5mm! I just slipped them together like so

![20190325_170303|666x500](upload://fkqS149lW3bkQ7RBBcTh4VcPmNl.jpeg)

And soldered them (it could not have been any easier)

Then added some shrink wrap

![20190325_173635|375x500](upload://wdkfDZNvnjcSbWHwbQO3nu9OKCe.jpeg) 

All ready!

![20190325_173707|666x500](upload://vLg0AvtXl4cdrScoFfUwO6Oa0yp.jpeg) 

So far the build is looking amazing!
![20190325_174026|666x500](upload://2iFilaHJvkkmtlp5q0iX4kY3ZWR.jpeg) ![20190325_174039|375x500](upload://3n4BUzS7n2O8ksQjOaizxALxwkT.jpeg) 

Re-using the 3S Lipos I had for my first build for a slim 12S 5000MaH pack.

The motor mounts from @Idea  are amazing!! Super sturdy, went together very easily.
Also shiny aluminum :wink:


However, one thing still remains.
The TB motor shaft is too long, and would end up digging into the wheel. So, I need to cut a bit off the end. (You can see that I am unable to push the wheel all the way in to align the pulleys)

![20190325_174058|375x500](upload://3shapD7tvLiWe7Cwj164SaR7SRX.jpeg) 

I'll need to go get an angle grinder :smile:


 Getting excited!!
```

---
## \#49 Posted by: rich Posted at: 2019-03-26T10:51:46.285Z Reads: 96

```
You can use a dremel or like me a cheap copy of it for cutting.

![173436h|690x388](upload://c8ZKulp2kfL5hoYHIDVVQQNpJjZ.jpeg) 

It is very important that the motor is fully covered because of metal chips.

![195843h|690x388](upload://cA1Y1wnUBccUrat030AU8r6mWiv.jpeg) 

Or you take a fine metal saw, hold it on the shaft and give throttle :sunglasses:  but it could be more tricky to cover the motor.
```

---
## \#50 Posted by: CoolRextreme Posted at: 2019-03-27T01:42:39.780Z Reads: 90

```
Ahahaha, thank you for the suggestions!
I stuck a plastic ziplog bag over the motor and very gently cut away the end of the shaft with an angle grinder.


Question for you Unitu FOCBOX users out there.
Or generally anyone who knows anything about versions and updating the Unity

![2019-03-26_183928|690x435](upload://mpK5tuAK0TI3kXZSUraGnuBNMpU.png) 


I am unsure if updating the Unity is the same as updating the (Singular? lol) FOCBOX

What the heck do I do lol
```

---
## \#51 Posted by: venom121212 Posted at: 2019-03-27T01:52:07.900Z Reads: 87

```
Do you have the focbox ui app on an android phone?
```

---
## \#52 Posted by: CoolRextreme Posted at: 2019-03-28T06:14:49.312Z Reads: 86

```
Ahaha, I forgot to actually send the post a day ago.

Yep Venom, I found The solution. I had the FOCBOX tool, not the FOCBOX UI downloaded.
Also I found the 'update' button and clicked it, hoping I wouldn't mess anything up.

It worked though so thats :ok_hand:

Promptly took it out for a spin, and Oh My Lawd is it smooth!

The terrible roading that would usually cause leg-numbing vibrations on my longboard is now smooth as a baby's bottom.

Its been raining quite a bit lately though, and I still need to design and print enclosures, so for now, that is all I can say.

As it stands now;

![20190326_195323|666x500](upload://fM7nYVh8qNN9bHEa0nImgGubMWi.jpeg)
```

---
## \#53 Posted by: venom121212 Posted at: 2019-03-28T11:32:09.067Z Reads: 81

```
Exactly how a maiden voyage should look! Keep up the good work man, looking good
```

---
## \#54 Posted by: taz Posted at: 2019-03-28T11:37:16.933Z Reads: 77

```
This is ideal for jumping as it is.
Can't get any lighter than that :sunglasses:
```

---
## \#55 Posted by: CoolRextreme Posted at: 2019-03-29T11:49:49.552Z Reads: 75

```
Thank you thank you!

I am running the bare minimum to see how it fares in terms of lightness and a small battery profile.
They are, however, 20C 5Ah packs, which put out 100Amps max.
Great for a single-motor longboard.
Not so great for a dual-motor mountainboard.
Batteries are expensive though, so I am more then happy to use these for now, despite the fact that they only give little more then half of what the rest of the system can take.

Tiny tiny update.

Organized the wires and focbox a little with some zipties and heatshrink for abrasion protection.

Also added an extension wire between the focbox and the battery so my right foot actually has room, and I dont keep unplugging the battery with my toes.

Designing my focbox box

Contemplating a 'flexible' battery housing design that will flex with the board, but still allow the batteries to lay side by side as shown. (Wow that is SUPER slim. I am very happy to not have a GIANT box between my feet) (No offense to those who do have giant boxes. Personal preference)

![20190328_125425|666x500](upload://xZFget7WXmKTD30aLarn7HqnNfX.jpeg) 

![20190328_125335|375x500](upload://fd0gplMZQaoheGrjjRX003zMMcB.jpeg)

Need to figure out wiring the sensors in. Starting from a stop is near impossible at the moment.

Took it out in the field behind my house. Its really weird transitioning from a longboard to this; I keep bracing for bumps that this board makes negligable.
Also the soles of my feet get sore super fast from all that bracing.

Right motor seems to be acting a little funky.:face_with_raised_eyebrow::unamused:
```

---
## \#56 Posted by: Andy87 Posted at: 2019-03-29T12:05:55.891Z Reads: 76

```
small thing to add

 the longer the wires the higher the inductive voltage spikes can be. that shouln´t be a big issue for everything that is around 50-70cm, but non the less, if you run 12s better hold them short and don´t run the wires in circles like you did on the wires from the battery to the esc.
```

---
## \#57 Posted by: CoolRextreme Posted at: 2019-03-29T15:06:45.538Z Reads: 74

```
Right!
This was simply a short term solution using two 2' wires I had on hand (Hence the little loop of slack wire). Once I have the battery casing finished I'll cut the wire down to the exact length needed so as not to waste anything for future projects :ok_hand:
```

---
## \#58 Posted by: venom121212 Posted at: 2019-03-29T15:16:09.106Z Reads: 76

```
I feel you on the sore heels. Especially the back one. Such a different game!
```

---
## \#59 Posted by: HEFF Posted at: 2019-03-30T19:16:21.674Z Reads: 74

```
Interested in your final mounting solution of the FOCBOX Unity. Mine just arrived today. Our setups are quite similar. *Following*
```

---
## \#60 Posted by: GustavoLacerda Posted at: 2019-12-06T20:36:49.677Z Reads: 47

```
Hi there.. Can you share your measurements to apply on the twistar hubs? Got the same here :( thanks
```

---
## \#61 Posted by: Munger Posted at: 2019-12-09T19:39:36.731Z Reads: 43

```
![Message_1575919887109|690x388](upload://vIVhHjk1Jllcj4qAOKQF7pbbw06.jpeg)
```

---
## \#62 Posted by: Munger Posted at: 2020-01-22T17:53:30.409Z Reads: 27

```
Im not sure I understand. Sorry for late response. I don't come here much
```

---
## \#63 Posted by: GustavoLacerda Posted at: 2020-01-23T20:19:12.716Z Reads: 23

```
No worries. Got it some while ago. 40mm from each hole to the center and 47mm between holes. Twistar hubs are not diy friendly. Got the measure right for the pulleys ;) thanks anyway man.
```

---
