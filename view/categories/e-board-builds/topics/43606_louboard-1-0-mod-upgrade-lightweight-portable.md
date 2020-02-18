# Louboard 1.0 Mod, Upgrade &#124; Lightweight &#124; Portable

### Replies: 274 Views: 13567

## \#1 Posted by: jdnicholson Posted at: 2018-01-13T10:47:06.098Z Reads: 723

```
So I was lucky enough to pick up a very cheap Louboard 1.0. I bought it for a gag and to keep in the office for a fun commute to the local coffee shop. 

See: [https://www.louboard.com/product/lou-1/](https://www.louboard.com/product/lou-1/)

But I actually love the size and weight. Its been a load of fun. But man it is slow!!!!! The single hub does **NOT** do hills, like not even a slight incline. The battery sag as well is real!! 

So I'm thinking I need to throw in a VESC (or two) and maybe change the battery pack. I have experience in belt setups but I have no idea about hub motors. According to the louboards website it has a 1.5kw motor. I assume based off the fact it hardly moves that it is terrible. 

So I want to upgrade to a new hub motor setup. The board is running 83mm wheels which I actually like on the nickel board setup. So Im looking for some help. 

Can any one suggest:
1. Single or dual setup?
2. Quality hub motors with some grunt? (prefer high torque over top speed) 
_(prefer 83mm rather then 90mm)_ The new Predator Banshee hubs look pretty powerful.

![s-l960|400x225](upload://qIRXFBnbditOXwCYDSqe2ORNyAc.jpg)

![1a|375x500](upload://2S7bkMeVWTHHkGGPXxQwQwFmapr.png)
The inners of the Louboard. The VESC's are tight but it should fit where the original ESC is.

![2a|375x500](upload://hltgMtacFcZQgvCoMd3hwDjyUiD.png)

![3a|375x500](upload://yGc7xfvbVAfwmp1O5LEGj6NrCtS.png)
Original Louboard 1.5kw motor
```

---
## \#2 Posted by: Vanarian Posted at: 2018-01-13T14:27:28.968Z Reads: 609

```
Well that's a single drive hub motor with no reduction and freaking tiny size + closed design with no cooling whatsoever, this was to be expected.

Generally single drive hubs in small sizes are very weak.
```

---
## \#3 Posted by: BoostedBuilder Posted at: 2018-01-13T15:36:57.993Z Reads: 598

```
You are not going to fit a big enough battery to acomodate a dual drive. I'd say make a single belt drive. 
6355 motor
15mm 15/36 or 16/36
1 Vesc
As big of a battery as you can fit (10s2p VTC6?)
```

---
## \#4 Posted by: aigenic Posted at: 2018-01-13T15:49:14.527Z Reads: 574

```
Or you can use different deck or different ESCs...sadly I dont know about any realible ESC with good brakes that would be small enough and comparable to VESC :/ 

The idea with single 6355 is probably the best :) but you would have to change so many parts that it would be better to build a new board instead :/
```

---
## \#5 Posted by: TranxFu Posted at: 2018-01-13T15:53:46.490Z Reads: 541

```
I also love the deck and size of the Louboard :) A perfect commuter board. 
 I'd say go for a single setup like @BoostedBuilder said. Slap some kegels or flywheels on there and go for 10s2p with high quality cells.
```

---
## \#6 Posted by: SilentException Posted at: 2018-01-13T16:27:34.021Z Reads: 516

```
No way 2p is going to fit in the existing battery slot.
```

---
## \#7 Posted by: Truebanana Posted at: 2018-01-13T16:34:56.227Z Reads: 510

```
Someone on Kickstarter said it's 10s1p

I have a 1.0 (for my gf) and a 3.0, with one dead hub and maybe dead ESC. 

I'm thinking about using a Meepo ESC, as it's written on their website that you can push to start the board, like the Lou board who doesn't have an on/off power switch.
Maybe also their 90mm hub, but it might be too big and get wheelbite.
```

---
## \#8 Posted by: SilentException Posted at: 2018-01-13T17:27:05.100Z Reads: 477

```
Existing battery is 1p yes. 2p won't fit in 1.0.
Lou already has the same ESC as Meepo, or at least similar, that cheap eBay one.
I was thinking of doing some upgrades but the space is limited and IMO it would be better to build a DIY board of this size, if you want a penny (nickel).
I will probably just upgrade the battery pack using better cells.
```

---
## \#9 Posted by: RickMcDuck Posted at: 2018-01-13T17:54:57.716Z Reads: 468

```
Will there be any other upgrades needed when you upgrade the battery pack on LOU 1.0? I mean can you keep all the other parts original? 

And what would be the best option for the battery when upgrading the LOU 1.0?

(I`m pretty inexperienced with electronics so I`m just trying to get some info :) )
```

---
## \#10 Posted by: SilentException Posted at: 2018-01-13T17:59:56.376Z Reads: 470

```
If using same type and number of cells in series (10s), it will be the same voltage as original one, that's it.

If you want to charge that pack using the board charger you need to add a 10s BMS for charging.

Since there really is no room for a 2p pack, the next best thing is to use decent cells in the 1p pack, like sony VTC6.
```

---
## \#11 Posted by: topcloud Posted at: 2018-01-13T18:10:34.331Z Reads: 464

```
https://www.reddit.com/r/ElectricSkateboarding/comments/7f2nbo/improving_the_lou_board_diy/

fwiw, you may wish to fasten the plastic deck to the chassis with nut-and-bolt technology before attempting even the _simplest_ driveway carve 

(naked lou cut me lol)

rooting for you.  I really want to heart that thing.
```

---
## \#12 Posted by: RickMcDuck Posted at: 2018-01-13T18:12:42.848Z Reads: 431

```
Okay. But when you build a pack using better cells, do you also need to get other new components? Better ESC?
```

---
## \#13 Posted by: RickMcDuck Posted at: 2018-01-13T18:16:23.042Z Reads: 403

```
I was looking at that Reddit post as well. There are some good ideas there but those are for the LOU 3.0 by the looks of it.
```

---
## \#14 Posted by: SilentException Posted at: 2018-01-13T18:18:02.570Z Reads: 391

```
Sure, if you want to. I think the ESC is _good enough_.. But if you have spare VESC..it is possible. Then you need to upgrade the remote as well.
Next thing, you'll be upgrading the hub.

But why? This board ain't worth it. As I said, at this point it is better to build your own small board. At least you'll have space for bigger battery.
```

---
## \#15 Posted by: RickMcDuck Posted at: 2018-01-13T18:36:49.443Z Reads: 369

```
So I quess I could build a better battery pack with better cells, have the same voltage and amps and it would work fine with original parts? Just have bigger battery capacity for longer work time.
```

---
## \#16 Posted by: SilentException Posted at: 2018-01-13T18:45:29.168Z Reads: 376

```
Yes, longer ride times but also less voltage sag which means better performance.
You need cells with higher Amps rating, not the same though :)
```

---
## \#17 Posted by: RickMcDuck Posted at: 2018-01-13T18:56:50.591Z Reads: 374

```
That sounds great! So best option for an upgrade would be to build a 10s1p battery pack with better cells and get a 10s BMS for that to use the original charger?
```

---
## \#18 Posted by: SilentException Posted at: 2018-01-13T19:05:55.074Z Reads: 383

```
Exactly. That's my plan anyhow. Anything beyond that is just too much and not worth for this toy IMO.

But there are other things that need attention.

The swappable deck for example needs some work. It is bad design, borderline dangerous. They said the upgrade kit will be available but I wouldn't hold my breath.

I also find that the charging port is not really safely mounted and the wires are exposed.

Also, bluetooth module and the wires from ESC should be more safely routed and mounted since they are just hanging in there and the vibrations might cause problems. Not to mention the rattling sounds they make..
```

---
## \#19 Posted by: BoostedBuilder Posted at: 2018-01-13T19:05:56.877Z Reads: 370

```
I think VTC5A cells would be better for this application
```

---
## \#20 Posted by: SilentException Posted at: 2018-01-13T19:09:09.940Z Reads: 374

```
May be. But VTC5A are currently 25% more expensive than VTC6 and I really don't think anyone would notice the difference. OK, maybe larger rider. But why would a larger rider get Lou 1.0 anyhow ??? :)
```

---
## \#21 Posted by: BoostedBuilder Posted at: 2018-01-13T19:13:28.884Z Reads: 332

```
You should be running the VTC6 at 15A while the VTC5A can be run at 20A and it would be at the same temperature. Thats a solid 33.3% amp increase and he said he is trying to climb hills! Lou 1.0 is definitely not for larger riders but since he has it already, why not try it?
```

---
## \#22 Posted by: SilentException Posted at: 2018-01-13T19:23:19.391Z Reads: 327

```
Sure, depending on how much you want to spend. And if you're going hills. VTC5A have less mAh. It is always tradeoff. For me, VTC6 are better choice.
```

---
## \#23 Posted by: RickMcDuck Posted at: 2018-01-13T19:30:42.980Z Reads: 322

```
The back and front velcros of my board seem pretty sturdy but the middle ones came off today when I removed the deck so Im going to glue those on with stronger stuff. Also it seems that the middle part of the board is not leveld with the sides so that`s interesting. 

Not sure what to do about the ESC and the wires. They do seem a bit too "out in the open" and loose, so if you have a solution for those Id be grateful to hear it :smiley:.
```

---
## \#24 Posted by: RickMcDuck Posted at: 2018-01-13T20:20:40.479Z Reads: 316

```
So, what I`m getting is that VTC5A is better for climbing hills and better for bigger riders but VTC6 does the job aswell. Bigger mAh?

Regarding the price it seems they are about the same. UK Amazon shows that VTC5A and VTC6 are the same price if bought per 1 cell and if per 4 cells then VTC5A is cheaper.
```

---
## \#25 Posted by: SilentException Posted at: 2018-01-13T20:24:57.737Z Reads: 303

```
[quote="RickMcDuck, post:23, topic:43606"]
Not sure what to do about the ESC and the wires.
[/quote]

ESC is fine, it is the Bluetooth module that should be secured. I mounted it on some foam and neutral silicone next to the ESC. Same thing with wires on the other side.

You don't really wanna buy batteries from Amazon. NKON.nl is the place to go.
```

---
## \#26 Posted by: RickMcDuck Posted at: 2018-01-13T20:35:00.174Z Reads: 292

```
Not that big of a difference in price but what is better to get? More mAh for longer rides and just Amps for speed?

And do you have a picture of your solution to the wires and the Bluetooth module? :)
```

---
## \#27 Posted by: SilentException Posted at: 2018-01-13T20:40:15.206Z Reads: 278

```
Yeah, I would have already posted the pic but don't have the board with me at least until next week. It is snowboarding season, not esk8 season around here so most of my boards are tucked away in hibernation :)
```

---
## \#28 Posted by: RickMcDuck Posted at: 2018-01-13T20:57:35.329Z Reads: 274

```
Haha I see :D. But what are the pros of having more mAh and pros of having more A?
```

---
## \#29 Posted by: aigenic Posted at: 2018-01-13T21:01:36.253Z Reads: 282

```
If you have more mAh you get more range...
If you have higher discharge rating (A), your battery wont "sag" that much, meaning it will loose its capacity during discharge slowlier and the battery shoud live longer :)
```

---
## \#30 Posted by: SilentException Posted at: 2018-01-13T21:05:47.408Z Reads: 287

```
^^^ what he said :slight_smile:
Also, the rated mAh / A are not directly comparable. It is best to look at some tests and graphs and decide for yourself.
```

---
## \#31 Posted by: RickMcDuck Posted at: 2018-01-13T21:13:36.831Z Reads: 278

```
So it seems that for the post writer the VTC5A would be a better choice. And going double hub motor on LOU 1.0 is pretty impossible.

I quess for my type of riding more mAh would be a better choice. (Like those long rides :D )

But building the pack is going to be a whole different story
```

---
## \#32 Posted by: aigenic Posted at: 2018-01-13T21:20:32.189Z Reads: 273

```
Look for some battery producers in your neighbourhood, they will certainly make such a small pack for you and it shouldnt be expensive :) Certainly better idea than doing it yourself ;) 

Also do not expect great rise in the range, there will be some for sure, but not much...If you want more range, you can modify the lou to have a swappable battery like inboard, which would be completly hilarious :D :D
```

---
## \#33 Posted by: SilentException Posted at: 2018-01-13T22:12:55.660Z Reads: 289

```
As you were browsing UK Amazon, maybe you could ping @darkkevind about building the pack for you. He does packs for Evolve and is located in UK.

And yes, do not expect anything incredible. The pack will sag less then original which is not crap but it is not using highest rated cells. Some performance increase yes, maybe even a bit longer ride and much less of that annoying beeping sound from ESC :) For more range build 2 or 3 packs!

[quote="aigenic, post:32, topic:43606"]
can modify the lou to have a swappable battery like inboard
[/quote]

Since the deck plate can be taken off pretty easily, it is already highly swappable anyhow.
```

---
## \#34 Posted by: jdnicholson Posted at: 2018-01-13T22:42:49.771Z Reads: 301

```
So after some thought and looking through what I have in the workshop. I think I'm gonna stick to belt driven. It will ruin some of the stealthy design but I think it provides a much better power to weight option. 

I have a @psychotiller Ripba mount laying around and a 6355 motor. So I'll hook that up so a VESC an get a small battery pack made. That should give the board more torque but will unfortunately ruin the free roll of the hubs. I'll experiment with a 9mm and 12mm pulley option and see if I can get a balance of good coasting and good torque delivery with no belt skipping. 

Couldn't sleep last night so did a quick mockup last night whilst everyone else was asleep. 
![image|666x500](upload://rwyuigsuZWmu22gjgKUUXUYgczQ.jpeg)
Obviously nothing is aligned, spaced correctly or tight. Just wanted to get an idea of what it would look like.
```

---
## \#35 Posted by: Maxid Posted at: 2018-01-13T23:21:44.426Z Reads: 278

```
Does anyone know if there is a way to just get the deck?
```

---
## \#36 Posted by: darkkevind Posted at: 2018-01-13T23:24:26.684Z Reads: 275

```
You'd be better off making up a pack of Sanyo 20700 cells and using the Meepo ESC, truck & hubs....

Those hubs have quite a surprising amount of torque.
```

---
## \#37 Posted by: pat.speed Posted at: 2018-01-13T23:46:29.065Z Reads: 282

```
Why has everyone overlooked lifepo4 cells? They have a high enough discharge for a 10s/12s1p configuration. The down side is they are on the expensive side. Pair that up with a set of 83mm hubs from diyeboard and a dual EBay esc and your good to go


Edit: here's the cells rated for 70amps max


https://ru.nkon.nl/rechargeable/26650/a123-systems-anr26650m1b-a-grade-3-3v-a-grade.html
```

---
## \#38 Posted by: SilentException Posted at: 2018-01-13T23:51:34.767Z Reads: 299

```
Finally. Found the pics I took on the first week I received the board. Thought I had lost them.

![lou_inside_1|400x300](upload://f43nREYYNLIAHOO5QxJGwr8chQc.jpg)

![lou_inside_2|400x300](upload://JfVze2MEN1xq9CbbbL3dzzkB0R.jpg)

20700 10s pack would maybe be possible but the BMS would be problematic to fit.

Height of the pack should not go over 20-21mm. The 22mm is really tight fit as is and the middle straps are not holding the deck securely.
```

---
## \#39 Posted by: pat.speed Posted at: 2018-01-13T23:54:29.772Z Reads: 288

```
To fit the bms he could do @scepterr portable bms idea and just have a jst sticking out for the plug
```

---
## \#40 Posted by: jdnicholson Posted at: 2018-01-14T04:36:49.731Z Reads: 303

```
UPDATE---------------------------------
So I have filed down the trucks, attached the motor mount and motor. I have a spare vesc but no antispark switch at home. 

![0DA63515-2BF6-492E-B826-1C9F90A86CA5|666x500](upload://eVx1eCh3gwOyCad3bpWWkPmiN6K.png)

I was thinking can I simply wire the Enertion rspec 6055 motor up to the existing esc???? Will the 6055 simply overheat and fry the current esc or the current configuration won't work because I'm going from a low kv hub motor to a 190kv outboard motor? Any thoughts??
I don't really want to fry the ESC if I don't have to. I may put back all the original parts and sell it one day.

![7531F619-52CD-40C0-BB86-06BFED403B57|666x500](upload://rS3LfZyrH9t6NitRBnVbp5Rm4HF.png)

![BD5BE9FD-3BA5-46BB-A870-EB5760447C79|666x500](upload://cQaRI3gjj9NsWJVmOieTLi1RIz2.png)

I know a vesc is way way better and configurable and I will use one in the end but for now whilst I wait for the switch to arrive Id love to try it out, plus the smart start on the current ESC is pretty sweet.


![1A359256-9F04-4CB2-BA4C-0D433190CCC4|666x500](upload://xzN4CENaeh7aanp6jDVYpmKCPUk.png)

![aaaa|375x500](upload://ru56ir1KqMPd77EOlbbEhPB0Uj4.jpg)

I'm really liking it so far. I just hope its as powerful as I am hoping.
```

---
## \#41 Posted by: PredatorBoards Posted at: 2018-01-14T05:38:54.831Z Reads: 286

```
Some seriously bad looking shit right there! I'm doing a very similar build with my Banshee, which is a similar form factor and similar weight to the Lou.

https://www.instagram.com/p/Bbk-5bdFyW_/?taken-by=predator_eboards
```

---
## \#42 Posted by: jdnicholson Posted at: 2018-01-14T05:54:59.432Z Reads: 274

```
I know!!! I have put your board in my cart about 20 times. Just haven't clicked pay now yet! Im in Australia and saw a recent review by Jay Boston and thought this may be the way to go!!! Loving your work.
```

---
## \#43 Posted by: PredatorBoards Posted at: 2018-01-14T05:57:07.516Z Reads: 274

```
Hey! At least there's one person thinking I''m doing something right. Seems like all of Reddit wants to downvote my product to oblivion and upvote the 20th meepo clone coming to market. 

If it means anything, I'm going back and forth with my partner on a risk assessment for potentially selling just the deck alone for others to use.
```

---
## \#44 Posted by: jdnicholson Posted at: 2018-01-14T06:12:22.173Z Reads: 277

```
I mean meepo has its place. But I'm looking for a good backpack board that has some good power whilst importantly being very lightweight. I have electric longboards but I want a portable commuter. Hence this board. But I may end up going with the banshee. Just want to see more hands on reviews and opinions rather then just readit and deep analysis of the specs here. 

The enertion raptor 1 got hit hard online. But I love mine. It's such a personal thing. The only specs that matter is what matters directly to you. Aka I don't need a board that goes 30km or at 30 km/h I just want a lightweight stable backpack board that I can take a incline and I can strap it to my bag and take it to dinner with the misses if I need to.
```

---
## \#46 Posted by: PredatorBoards Posted at: 2018-01-14T06:59:53.362Z Reads: 274

```
Yep! Definitely sounds like a good  fit for you, that's for sure... A beta unit is with Ronnie Sarmiento, who can probably provide more insight into how the board rides and all(since he basically tried every 'cheap' board under the sun). I'm pretty confident the Banshee will stack up well versus all the meepo clones... that's for sure.
```

---
## \#47 Posted by: Grozniy Posted at: 2018-01-14T09:28:21.974Z Reads: 278

```
I had a similar idea of portable board and wanted only the deck. [This](http://www.ebay.co.uk/itm/192404650231) looks promising if only they sold the deck.
![FB_IMG_1515921776551|690x388](upload://q0B6SzuNaykN8iF0g3FMTnzDqtU.jpg)
```

---
## \#49 Posted by: jdnicholson Posted at: 2018-01-21T19:21:46.180Z Reads: 285

```
So I have finished up my mod from a hub motor to belt driven Lou board 1.0. So to back up and explain why. 

Essentially the original louboard 1.0 single hub motor was very very weak and was next to useless at taking any inclines. With parts I had handy and a cheap hobbyking motor mount. 

I was able to give the board significantly better brakes and torque with only a little more weight. The board is still lightweight and portable. Just not as sleek as it once was. 

The only thing I'm still waiting to change is the esc. For simplicity I have decided to simply swap over the hub programmed esc with a single belt programmed esc. I know going to a VESC would be far far better but without an antispark switch handy and not wanting to do a loop key. A cheap swap of the escs was the most simple option. This should give better throttle and braking as the esc will be programmed for a belt rather then hub motor. 
 
![image|666x500](upload://utlBP4PmtDfo0dn8EZUOVfuuvyS.jpeg)![image|666x500](upload://67pL02ioVESz5TC0plOEA3eaqcq.jpeg)![image|375x500](upload://aXy9SdYR0tvoMQ7QHohL3JQfDyd.jpeg)![image|375x500](upload://x4nyGDAzOsXXFDyPbrcQVjSwQMV.jpeg)
```

---
## \#50 Posted by: aigenic Posted at: 2018-01-21T20:35:30.508Z Reads: 265

```
Good job :) It looks fantastic :) Did you replace the battery?
```

---
## \#51 Posted by: jdnicholson Posted at: 2018-01-21T21:20:12.173Z Reads: 262

```
Kept the same battery, With a belt system and not a hub it seems to put a lot less stress on the battery. So far I have taken it up some decent inclines and it only starts beeping at the end rather than at the start with the hubs.
```

---
## \#52 Posted by: TranxFu Posted at: 2018-02-11T11:44:12.448Z Reads: 252

```
I just contacted SoFlow to ask if they are selling the board separately. Want to do a similar build to yours :) Just love the form factor and look of the Lou board. Have you tried 20700 and the focbox ? Since the focbox takes less room as the build-in esc I think
```

---
## \#53 Posted by: Grozniy Posted at: 2018-02-11T11:57:58.745Z Reads: 241

```
Tell me how it goes 😉
```

---
## \#54 Posted by: Lukas Posted at: 2018-02-11T12:53:48.075Z Reads: 244

```
Already asked them some time ago.
They said they wouldn't do it back then but they wanted to think about it.
```

---
## \#55 Posted by: jdnicholson Posted at: 2018-02-13T02:17:59.766Z Reads: 240

```
A focbox would be the way to go. I don't have one handy and didnt want to spend a fortune on this as it's just a fun kick around board. I will be changing it over to a vesc in the next couple of weeks as I have a couple old ones handy, just waiting on an antispark switch. 

This is my first single motor setup. I have 4 other boards with dual belt and dual hub. I can't say I'm in love with the feeling or performance of a single belt drive. I'm going to change over to dual belt. 

Because I want to keep things cheap and and simple i'm going to go with the diyeboard dual belt setup. 
http://www.diyeboard.com/dual-belt-drive-1400w2-n5055-motor-power-truck-p-658.html

The change over to a dual setup will require some reconfiguration of the boards internals. I'm going to need to get out the Dremel and remove some of the extra plastic and dividers that held the original electronics and battery. 

No going back after I start cutting. I had planned on just playing with this board and then just selling it on. But I'm actually quite enjoying the form factor of the deck.
```

---
## \#56 Posted by: TranxFu Posted at: 2018-02-13T09:37:13.795Z Reads: 233

```
Sounds good. But wouldn’t going for dual drive diminish the purpose of a commuter board (lightweight). What about going for a 6374 ? No need for the extra Vesc in there. 

I’m currently on the lookout for a used Lou board to diy it. Let me know if you want to sell yours :))
```

---
## \#57 Posted by: jdnicholson Posted at: 2018-02-13T09:55:54.869Z Reads: 239

```
I'm located in Australia so postage would be killer. The weight is important but not the most important. I have found I am able to attach this to my backpack which makes it so convenient. An extra 2kg max wouldn't make a huge difference on a backpack. 

I have tried a 6374 which is great. But again I'm not a fan of the single setup.
```

---
## \#58 Posted by: Chase Posted at: 2018-02-13T09:57:14.641Z Reads: 232

```
I bought someone’s used Lou 3.0 after it arrived to them with a broken speed controller. I ended up replacing it with the dual hub esc from diyeboard. It works great other than the range. As others have mentioned, the battery gets far less range than advertised. Also, I can’t brake if there is a full charge or it will shut off the board. I was thinking of replacing it with a 10s1p 18650 battery, but I’m wondering how which type of cells are in the stock battery. That aside, the deck is by far the best part of the board. Perfect commuter board. I’ll watch to see what you guys come up with.
```

---
## \#59 Posted by: jdnicholson Posted at: 2018-02-13T10:28:38.645Z Reads: 245

```
I had the esc cut off on me going downhill last week. Very very sketchy. How does the 3.0 handle hills? All the videos I have seen still show it struggles. Hence why I'm going with belts. The deck is great! Everyone is saying just scrap it and get something else. But that's not the point. I love the deck and it's super clean and short. I have other electric skateboards that are great and comfy because they are long. But I just want a sweet small commuter and just something to keep playing with and upgrading.
```

---
## \#60 Posted by: TranxFu Posted at: 2018-02-13T21:18:10.715Z Reads: 233

```
how much room to work can you get out of it if using a Dremel ? Possibly fitting a 10s1 A123 or 20700 pack in there ? Would you know if there is a difference in room between the 1.0 PU deck and the carbon fiber decks ? 

I've thought about putting 90mm flywheels on it. Should I worry about wheelbite ?
```

---
## \#61 Posted by: jdnicholson Posted at: 2018-02-13T21:41:38.990Z Reads: 231

```
I will get an extra 2cm in length I think. The carbon decks internals are much larger. The 3.0 needs to fit a dual belt esc which is wider and longer. Wish I had a carbon deck instead!

With wheelbite it really depends what width trucks you put on. I think you would get some wheelbite. Maybe a spacer or two would help.
```

---
## \#62 Posted by: Chase Posted at: 2018-02-14T00:43:43.459Z Reads: 213

```
Yeah the carbon fiber deck is designed to basically fit the battery, the dual hub esc and the wires. No room to spare at all. The dual belt struggles going up even minor hills. It will start to beep almost immediately even with a full charge. I agree that it is a great commuter board when the ground is flat. The deck is by far the best part of the lou board.
```

---
## \#63 Posted by: jdnicholson Posted at: 2018-02-14T01:42:03.396Z Reads: 217

```
Thats why I decided to go over to a belt drive. The battery just can't handle the draw from hubs. With the single belt ( at close to full charge) I climb quite steep hills with no beeping. The belt has made the board so much more usable for me. Just wish I had the carbon fibre deck!!!
```

---
## \#64 Posted by: Chase Posted at: 2018-02-14T03:58:32.243Z Reads: 213

```
In the Hi5ber thread, Brian says he may be releasing an ion 30 with built in enclosure at some point. That sounds promising for a nice commuter deck.
```

---
## \#65 Posted by: TranxFu Posted at: 2018-02-16T14:52:39.506Z Reads: 222

```
I am getting my hands on a 1.0 soon. I can’t justify the couple hundreds more for the carbon though. But it would be perfect 😅 it’s also lighter than the PU 1.0 Deck... what are the dimensions of the battery pack ? Can you confirm that it’s a 10s1p 18650? I’ll be ordering some VTC5/6 beforehand. Or do you think I can fit some A123/20700 in there ?
```

---
## \#66 Posted by: Chase Posted at: 2018-02-16T18:39:34.815Z Reads: 214

```
My battery is about 8 by 4 inches. I HIGHLY doubt its 18650 cells. If it is it is certainly no more than 1p. Its truly a shit battery.
```

---
## \#67 Posted by: GrecoMan Posted at: 2018-02-16T18:54:19.137Z Reads: 214

```
did you say 8x4... 😳

does it weigh like 85lbs? if so it’s probably lead acid
```

---
## \#68 Posted by: TranxFu Posted at: 2018-02-16T19:18:07.802Z Reads: 209

```
I think its 18650 though. 10s1p with some 2ah cells. It'd actually be a pretty nice upgrade to go from low-end 18650 to high-end 18650 like the VTC5/6 for just 50 bucks ? Better discharge rate for a little less sag and more capacity.
```

---
## \#69 Posted by: Hummie Posted at: 2018-02-16T19:23:17.854Z Reads: 212

```
sounds like the battery must be tiny.  id go lipo if you need to keep it so small and want power.  

1500 watt hub motors, continuous, don't look that small.  I could sell you a single hub motor that will eat both of those for snacks the near future.
```

---
## \#70 Posted by: TranxFu Posted at: 2018-02-16T19:33:59.860Z Reads: 210

```
@Chase I'm not too keen on the Hi5ber one... People here will demand freaking chunky 10s4p packs and stuff :expressionless::confounded: ....  With this kind of segment its not about prioritizing power and speed. But people don't get that...
```

---
## \#71 Posted by: Hummie Posted at: 2018-02-16T19:55:15.283Z Reads: 216

```
with lipo could have small and powerful. 
https://hobbyking.com/en_us/turnigy-battery-heavy-duty-4000mah-3s-60c-lipo-pack-xt-90.html
```

---
## \#72 Posted by: Chase Posted at: 2018-02-17T00:22:03.796Z Reads: 216

```
I agree. I only want thin sleek decks that are as light as possible. If he Brian wants to sell them, he will have to cater to the 2wd community and not the 4wd few. I’ve said my piece on that forum. Seems like the 4wd people would rather flood out other comments to make it seem like they are the majority. I’ll definitly look into hummies as an option to upgrade the lou. I’ve also been considering changing these cells. Voltage sag is a bitch on this battery.
```

---
## \#73 Posted by: jdnicholson Posted at: 2018-02-17T00:37:09.759Z Reads: 232

```
A lot of the posts and opinions are for long range ultra smooth longboard setups. Which are great. But not what I want for commuting. It’s really the difference between a weekend long range rider and a convenient light weight portable board. Yeah you will sacrifice comfort, speed and range but I don’t need all that for my 2km commute in the city to work. 

I want to be able to go to dinner in the city with my girlfriend after and not have to carry this really long board and find a place to store it. I have had to do that for the last 2 years. Since having a small board my partner loves it as it doesn’t affect where we go for dinner or if I need to walk with her around the city I just throw my board on my backpack and I forget it is there.
```

---
## \#74 Posted by: esk8jpn Posted at: 2018-02-19T05:34:44.844Z Reads: 233

```
Hey guys
This is a picture of 18650 cells put in my Lou 2.0.
![jeBfrDe_d|409x500](upload://nPO6sLS0cq3luX7dbpSTuXU6fvi.jpg)
The original battery pack is probably 10s1p of 18650.

I plan to make a 7s2p battery pack using LG HG2. Arrange them like the third picture from the top.
```

---
## \#75 Posted by: aigenic Posted at: 2018-02-19T05:46:16.083Z Reads: 227

```
You will get less top speed, hope you get it :) Maybe rewinding motors woud help a little :) Also if you plan on using the same type of ESC, the power output will be lower :(
```

---
## \#76 Posted by: esk8jpn Posted at: 2018-02-19T06:31:31.414Z Reads: 220

```
yep, I understand.

Since top speed is directly proportional to voltage, top speed is slower. but I think the range will increase.
Lou's original battery pack range is too short!!!:tired_face:
```

---
## \#77 Posted by: jdnicholson Posted at: 2018-02-19T06:45:29.887Z Reads: 215

```
Loving the battery mod. With the new battery setup you would have plenty of room for two vescs. That would solve your speed problems.
```

---
## \#78 Posted by: TranxFu Posted at: 2018-02-19T12:05:09.386Z Reads: 214

```
I honestly think there is no need to top off the speed with a dual drive there. Rather keep the single vesc and add a belt drive or go for the dual vesc/dual hub which is used in the 3.0 or meepo ?

Or try a 20700/A123 10s1p setup. Will give you a boost on the range and the discharge rate on those should be higher than the original pack
```

---
## \#79 Posted by: esk8jpn Posted at: 2018-02-19T12:50:01.563Z Reads: 214

```
A123 Systems 26650?
It will not enter Lou's battery space.

I think that Sanyo NCR20700B will get in. maybe.
```

---
## \#80 Posted by: BoostedBuilder Posted at: 2018-02-19T13:34:10.008Z Reads: 220

```
If you can get your hands on 10 or 14 of [these cells](https://www.imrbatteries.com/lg-hg6-20650-3000mah-30a-battery/) to make a 10s1p or 7s2p depending on your needs (speed vs torque respectively) , you'll get a nice board out of them.
```

---
## \#81 Posted by: jdnicholson Posted at: 2018-02-19T19:03:24.480Z Reads: 230

```
Totally ridiculous for this board. But I had two 6355 in my workshop and thought I’d have a look at how it would fit. Looks pretty awesome. But way way way too much power for this tiny board. 

![image|401x500](upload://nThZ4JiPJ0xqPhMXx2q1kO3Ct7.jpeg)![image|400x500](upload://5i0nNAQPSiaM5XqxXR7PONYH3R7.jpeg)
```

---
## \#82 Posted by: ZackoryCramer Posted at: 2018-02-19T19:10:02.263Z Reads: 221

```
:star_struck: Absolutely gorgeous. But the only thing I don't like about longboard trucks on penny size deck is the wheel potentially protruding to where your feet might be. But then again, who's pedaling? :joy:
```

---
## \#83 Posted by: Mikenopolis Posted at: 2018-02-19T19:24:26.713Z Reads: 222

```
[quote="ZackoryCramer, post:82, topic:43606"]
protruding to where your feet might be
[/quote]

I've done that before, turning becomes a problem because your feet causes wheel bite...or in your case butt cheeks :wink:
```

---
## \#84 Posted by: ZackoryCramer Posted at: 2018-02-19T19:26:24.084Z Reads: 222

```
Butt bite. Ouch. :peach:
```

---
## \#85 Posted by: esk8jpn Posted at: 2018-02-20T00:48:26.855Z Reads: 219

```
It's a small monster!
```

---
## \#86 Posted by: SilentException Posted at: 2018-02-21T19:44:43.379Z Reads: 219

```
Insides of a Lou 1.0 battery pack. Nothing to see here, move along people :) But really, nothing unexpected there.

![IMG_20180221_195520 - Copy|400x300](upload://jpnIbiSQqLFupjBB5hFt7GqbSfd.jpg)

![IMG_20180221_201458 - Copy|300x400](upload://uVQrubLqF25PDunMP9EeelM4ky0.jpg)

![IMG_20180221_203543 - Copy|300x400](upload://uXw3zzVv3nOrTR6nGSgYJXlw57y.jpg)
```

---
## \#87 Posted by: TranxFu Posted at: 2018-02-21T19:53:00.379Z Reads: 204

```
Really nice :)! Thanks for the insight ! 

So 22p... they are rated at 10amps continuous. 
This will be a straight 1:1 swap then ?
```

---
## \#88 Posted by: esk8jpn Posted at: 2018-02-22T00:50:29.446Z Reads: 205

```
Thanks a lot. I could not open the battery pack.
It seems to be glued, not screw.
```

---
## \#89 Posted by: SilentException Posted at: 2018-02-22T13:55:47.386Z Reads: 209

```
[quote="TranxFu, post:87, topic:43606"]
So 22p… they are rated at 10amps continuous.

This will be a straight 1:1 swap then ?
[/quote]

Yeah 22P, was expecting those. I asked on KS but of course they wouldn't say.
I think swapping those with some VTC5A or VTC6 should be doable without problems.

With 20650 you wouldn't be able to use the enclosure, obviously. And the plastic lips holding the enclosure in place (on the board) would get in the way but you can trim those. And I don't think the lips are even there on 2.0 and 3.0 (carbon fiber boards).

Not sure about BMS. I haven't found suitable replacement or alternative yet. If using 18650 there is obviously decent amount of space on top of the cells but with 20650 you are getting much closer to deck (original pack is 22mm and that is the maximum height).
```

---
## \#90 Posted by: TranxFu Posted at: 2018-02-22T14:23:39.118Z Reads: 201

```
Well, there are quite a few slim 10s bms out there. Bypass discharge is also a possible solution. 20700 with an slightly bigger 3D printed enclosure should not be a problem. Although I think settling for VTC6 seems the most effective and efficient way.
Can’t wait to get my hands on the board soon ! :blush:
```

---
## \#91 Posted by: TranxFu Posted at: 2018-02-22T14:24:42.679Z Reads: 200

```
They stated at the Kickstarter that the 2.0 and 3.0 „extended“ packs are not compatible with the 1.0. would you know why ?
```

---
## \#92 Posted by: esk8jpn Posted at: 2018-02-22T14:37:37.119Z Reads: 206

```
Both my 2.2 Ah pack and 2.9 Ah pack are the same size.
I don't know why they said were not compatible.
![15193097614361|528x500](upload://qesE2WZQR6RGOcrkhksN7uVvnTg.jpg)
```

---
## \#93 Posted by: Grozniy Posted at: 2018-02-22T15:36:11.357Z Reads: 205

```
I think i found [Lou 2.0 Clone](https://www.alibaba.com/product-detail/New-Hub-motor-electric-skateboard-booster_60616718446.html?spm=a2700.7724838.2017115.240.40d73253tNdHb9)
Who wants to ask if they sell the deck only? eheheh
```

---
## \#94 Posted by: aigenic Posted at: 2018-02-22T15:58:13.119Z Reads: 199

```
Dont know if they will, but the bamboo cover is much sexier thah this "swiss cross" bullshit
```

---
## \#95 Posted by: GrecoMan Posted at: 2018-02-22T16:03:21.654Z Reads: 198

```
holy shit a 700 meter long board 🤭
```

---
## \#96 Posted by: SilentException Posted at: 2018-02-22T16:03:50.483Z Reads: 203

```
No idea, probably marketing and hope they will sell more 2.0.

2.9mAh pack just has Panasonic PF cells, 2.9Ah and same 10A rating.

If you find any suitable thin BMS, let me know. Of course for charging only.

@aigenic Lou also has wooden deck, I got one being one of the earliest backers :)

![image|400x300](upload://a7jnImQJspgYCCxAhGdvVt2emKE.jpg)
```

---
## \#97 Posted by: esk8jpn Posted at: 2018-02-22T16:05:18.176Z Reads: 199

```
No, It is the base product of Lou.
SoFlow started crowdfunding with the exclusive sales rights of that products.
```

---
## \#98 Posted by: Chase Posted at: 2018-02-23T17:55:35.134Z Reads: 202

```
So like I said above, the board came to me with a broken esc. Changed it to one of those dual hub esc from diyeboard. If I brake on full battery, I loose connection. I have been trying to start my ride with an upward incline to drain the battery from the start to avoid this. This has become too much of a hassle/danger. What is responsible for this? Do I need to change the esc or the bms?

Thanks
```

---
## \#99 Posted by: mmaner Posted at: 2018-02-23T17:57:39.788Z Reads: 204

```
Its the battery cutoff, regen breaking.  What you replace depends on whether its the battery packs BMS or the ESC that's cutting off.  You would be better served with a VESC so you can program your own cutoffs at the controller level.  If you can figure out what BMS you have, looking up the cutoffs should be easy.
```

---
## \#100 Posted by: FredrikHems Posted at: 2018-02-23T18:57:06.180Z Reads: 196

```
Why dont you do a 10s1p with some 5Ah lipos? I am pretty sure it will fit nicely, and you will Get more Wh/range, and alot more discharge capability!
Edit: Even more top speed too!
```

---
## \#101 Posted by: Chase Posted at: 2018-02-23T20:01:08.450Z Reads: 196

```
Are you able to tell us which bms that is in there?
```

---
## \#102 Posted by: SilentException Posted at: 2018-02-23T20:47:16.902Z Reads: 192

```
No, it is something proprietary or custom. Couldn't find anything like it yet.

Not sure what you expect though. If the pack is full you don't wanna be overcharging the cells with regen. Charge the pack to 41V instead. I need to open the original charger to see what's in there, maybe it could be modified :)

[quote="FredrikHems, post:100, topic:43606"]
Why dont you do a 10s1p with some 5Ah lipos? I am pretty sure it will fit nicely, and you will Get more Wh/range, and alot more discharge capability!
[/quote]

You are pretty sure LOL. Fine, then. You have all the facts about the space in there (I have posted couple of images with exact dimension of original pack, there are couple of other images and posts about internal size /placement. 
So go ahead and find cells that will make 5Ah 10s LiPo pack that will fit. I challenge you :)
```

---
## \#103 Posted by: Exiledd_Top Posted at: 2018-02-23T21:35:14.131Z Reads: 189

```
Hey guys I saw this thread and it got me thinking I think what would be best is to mount all the batteries 7 18650's series probably 7s5p would fit just In the deck inside and the screws to hold the ESC from the bottom of the deck use them opposite so hold the ESC outside make a adapter case to mount from the outside like a small enclosure just to hold the esc .
This is probably going to be my 4th project as soon as my carvon 4wd is finished
```

---
## \#104 Posted by: TranxFu Posted at: 2018-02-23T21:39:56.636Z Reads: 183

```
but.. 7s5p are 35 cells... 

and this would make it hella ugly + heavy. Just get a longboard then :roll_eyes:
Would defeat the purpose of the board.

EDIT: and yeah, did I mention 35 CELLS ? This would NEVER fit in there
```

---
## \#105 Posted by: pat.speed Posted at: 2018-02-23T21:40:54.926Z Reads: 178

```
For the bms why not just use the stock one and bypass it for charge only?
```

---
## \#106 Posted by: FredrikHems Posted at: 2018-02-23T21:43:29.116Z Reads: 180

```
Bro, chill out.. No need to get mad. I was only coming with a suggestion. And I was writing to @esk8jpn , not you :wink:
```

---
## \#107 Posted by: Exiledd_Top Posted at: 2018-02-23T21:54:50.846Z Reads: 179

```
"Heavy" you call that heavy 20lb is normal for me  that thing should be light. 7s3p with bms and vesc at the bottom of the board single motor 200ish kv should be fine
```

---
## \#108 Posted by: Chase Posted at: 2018-02-23T21:57:26.561Z Reads: 180

```
I have to agree with fu. For me the lou is all about weight and portability. I would never want it any heavier than 13 lbs and hate externally mounted electronics.
```

---
## \#109 Posted by: SilentException Posted at: 2018-02-23T23:14:04.733Z Reads: 198

```
http://www.electric-skateboard.builders/t/louboard-1-0-mod-upgrade-lightweight-portable/43606/74?u=silentexception

This post is perfect. Really good example what will fit in there. In 1.0 space is even more limited because of the plastic "lips" holding the battery in place but those are easy to trim.

If you want anything more than that, you will need to destroy the deck in some way which most aren't going to do because the deck is quite okay, nice looking and decent in weight and size as is.

@pat.speed I will tear down the battery pack further next week but I'm quite sure BMS is already bypassed (charging only)

@FredrikHems not mad at all bro. You read me wrong.
```

---
## \#110 Posted by: pat.speed Posted at: 2018-02-24T00:53:38.500Z Reads: 197

```
I think if you really squeezed it in the you could potentially fit 20cells, a Vesc 4 and a micro bms. That means you could run a 6s3p which would eliminate some voltage sag. You could also try fitting the bms in the space left by the missing two cells


![IMG_1179|640x353](upload://oSoozYqW6z8RkpMjM5aNLTkDi3J.PNG)
```

---
## \#111 Posted by: SilentException Posted at: 2018-02-24T01:26:08.604Z Reads: 195

```
The cells in the image aren't welded and that takes some of the space as well. Height wise, there is 21mm total - 3mm left therefore anything over the cells is a no go.

But just maybe it could fit in. This would probably be the best way to solve the sag provided motor is running well on 6s, Not for 3.0 because of dual hubs / dual VESC.

I also think the @esk8jpn idea of 7s2p is also a good one. With good cells and not too heavy rider it could also be perfect.
```

---
## \#112 Posted by: esk8jpn Posted at: 2018-02-24T09:58:18.179Z Reads: 191

```
@pat.speed

It is difficult to put three more cells there.
I will put a BMS in that space.
```

---
## \#113 Posted by: pat.speed Posted at: 2018-02-24T11:50:27.366Z Reads: 185

```
It couldn't be that hard if you were to use a smaller esc, ie Vesc or hobby esc
```

---
## \#114 Posted by: TranxFu Posted at: 2018-02-28T17:10:06.341Z Reads: 186

```
Is there an aftermarket ESC like the Lou for cheap online ? I've got a focbox here but I'd have to wire in a push button and Dremel an opening somewhere. And I quite like the push-start feature.
```

---
## \#115 Posted by: Grozniy Posted at: 2018-02-28T17:45:11.114Z Reads: 183

```
https://m.ebay.com/itm/Dual-motors-longboard-skateboard-control-modula-ESC-Substitute-with-remote/323106658704?hash=item4b3aa85990:m:mnTgHbWA95Vts7jzZsG0QnA
```

---
## \#116 Posted by: esk8jpn Posted at: 2018-02-28T17:46:34.352Z Reads: 185

```
DIYeboard's ESC is very similar to Lou genuine ESC.
http://www.diyeboard.com/v11-single-hub-motor-sine-wave-foc-esc-speed-controller-p-609.html

I actually bought it.
PCB size, Sensor wire connector is the same thing. Only the XT60 connector is different.

That means Lou's ESC can also change 6S, 7S, 10S voltage settings with simple soldering. and I confirmed that it actually works with 7S.
```

---
## \#117 Posted by: Truebanana Posted at: 2018-02-28T19:40:32.595Z Reads: 176

```
I think the Meepo ESC also have the push to turn on thing, so no power button if you buy the ESC alone. But at least few months ago when I was looking for another ESC as Soflow support is Soslow
```

---
## \#118 Posted by: Chase Posted at: 2018-02-28T21:06:30.951Z Reads: 195

```
DIY eboard esc on 3.0

![image|374x500](upload://A8mg89ijK5zXuQ0MwODMaF3GyYv.jpeg)

Not even a mm taller will work. The wires would barely squeeze in. I changed the battery Velcro to a stronger/thicker brand and just the slightest difference in Velcro’s thickness causes the lid to not latch.
```

---
## \#119 Posted by: TranxFu Posted at: 2018-02-28T21:10:35.380Z Reads: 190

```
Whats the reason you went with a new esc ? Is the DIYBoard ESC also push-start ? Did you try fitting a focbox in there ? 

For now I've got 10 VTC6s on my way. I'll reprint the battery enclosure to keep the 2,2ah one as a carry-on battery.
```

---
## \#120 Posted by: Chase Posted at: 2018-02-28T21:17:33.466Z Reads: 198

```
I got the new one because the one it came with breaks way to easily. It came to the person I bought it from with all the capacitors broken off. The same thing happened to a lot of the Kickstarter backers. Yes the diyeboard starts by moving the board forward or an optional power button add on.

Here is the original esc. Originally I tried just replacing the capacitors but the height of the new capacitors were slightly too tall. The esc they provide basically rubs against the lid to the board. I may switch to vescs soon to fix the cutout when braking on full charge. 

![image|374x500](upload://4wcPmVS4gAiEIYtMVekNM91AJo3.jpeg)
```

---
## \#121 Posted by: jdnicholson Posted at: 2018-02-28T23:06:32.645Z Reads: 195

```
I went over to a diyeboard esc. It is simply a remove and replace job. Exactly the same size and bolt holes. It is a push start but you can also use the power switch they supply. It also comes with a battery indicator if you want it. 

The remote for me is also way better than the louboard joystick.
```

---
## \#122 Posted by: mrquin Posted at: 2018-02-28T23:27:36.626Z Reads: 180

```
has the braking and/or acceleration feel changed?
```

---
## \#123 Posted by: Chase Posted at: 2018-02-28T23:54:10.698Z Reads: 181

```
Not at all the case with the 3.0. None of the holes line up. The metal plate isn’t even the right size for the new esc. The diyeboard esc will sometimes continue to throttle a few seconds after you release on the remote. Someone made a good YouTube video showing this so you know what to expect.
```

---
## \#124 Posted by: jdnicholson Posted at: 2018-03-01T00:04:50.932Z Reads: 181

```
true, I should have said that. My experience is only with the Louboard 1.0 with a single hub motor. The throttle staying on after you release is odd when it's on the bench. But when your riding it it's not heaps noticeable. It just feels like your coasting a little further. 

I did, however, change from a hub motor esc to a belt esc for my conversion, so I can't comment on the braking strength. The original louboard hub esc for braking was terrible.
```

---
## \#125 Posted by: esk8jpn Posted at: 2018-03-01T00:56:43.832Z Reads: 180

```
[quote="Chase, post:123, topic:43606"]
sometimes continue to throttle a few seconds after you release on the remote.
[/quote]

This also happens with my Lou 2.0 genuine ESC. I dislike this behavior very much.
Also, I wanted to improve Lou's weak braking force. However, it was not improved in DIYeboard's ESC.
I will go to the dual hub motor setup.
```

---
## \#126 Posted by: TranxFu Posted at: 2018-03-01T13:44:49.636Z Reads: 176

```
Are you guys using the diyboard esc have a delay or lag when Pushing the throttle ? Or is it immediate like a VESC
```

---
## \#127 Posted by: Chase Posted at: 2018-03-01T21:03:50.361Z Reads: 173

```
No lag for the throttle
```

---
## \#128 Posted by: TranxFu Posted at: 2018-03-06T20:21:24.032Z Reads: 184

```
>**Hummie 18d**
sounds like the battery must be tiny. id go lipo if you need to keep it so small and want power.
1500 watt hub motors, continuous, don’t look that small. I could sell you a single hub motor that will eat both of those for snacks the near future.

overlooked this one :D are you still up for it ?
```

---
## \#129 Posted by: TranxFu Posted at: 2018-03-08T11:41:47.194Z Reads: 190

```
Finally received my 1.0. I’ll do a build log on updating to VTC6 soon. How is your experience with the belt setup ? I don’t like how the Original esc feels. I have a spare focbox lying around and will replace that. I’ll get out the dremel and see where I can place the power button. 

I just don’t know if I should keep the hub or change it to a belt drive. 

It is a bit heavier than i thought too. Trucks look kind of massive, did you swap em out too ?
```

---
## \#130 Posted by: mrquin Posted at: 2018-03-09T17:41:56.322Z Reads: 184

```
Let us know how it goes!  Any reason you're going with vtc6 vs 30q or others?  Kind of a battery noob here..

I have a lou 3.0 here with a dead battery so i'd love to fix up the battery if possible.
```

---
## \#131 Posted by: Lyr3x Posted at: 2018-03-14T13:50:35.554Z Reads: 203

```
Hey guys,

got my Lou 1.0 for a while now and im quiete happy with this stealthy commuter board. What i dont like is the short distance (about 8-10 km for me).... So i'll build my own spare battery pack :man_mechanic:

I'll share my first iteration of the case (yeah.. its a clone) i designed today. I think i'll go for some VTC6 in 10s2p.![batterypack|690x467](upload://7Qx9iLpwxcAm3cEMen2MrEUU9uP.jpg)
```

---
## \#132 Posted by: Truebanana Posted at: 2018-03-14T14:27:14.395Z Reads: 187

```
Isn't it a 10s1p ? How will you fit a 10s2p ?
```

---
## \#133 Posted by: esk8jpn Posted at: 2018-03-14T14:41:47.348Z Reads: 186

```
My Lou is 2.0, I think that it is impossible unless ESC is remove.
```

---
## \#134 Posted by: TranxFu Posted at: 2018-03-14T17:16:28.291Z Reads: 187

```
I've used the Lou 1.0 with its standard specs for 2 weeks now. Other than its awesome design and portability it is meh. I've got some 30Q cells on my way which I'll arrange in either 10s1p or 12s1p. 

I'd go for 30Q rather than VTC6. The VTC6 has a lower lifecycle count and is way more expensive. I don't think 10s2p will fit in there. 
I barely have enough space for 2 more cells (hence 12s1p) with my focbox + anti spark + receiver in there. 

I hope that I can draw out more power from the hub with the focbox. The onboard ESC is so bad...
```

---
## \#135 Posted by: Chase Posted at: 2018-03-14T17:23:47.628Z Reads: 182

```
You won’t get a 10s2p in there. There’s no way. I’m swapping out my 3.0s 29e cells with 30Q batteries. I would make my old cells into a sore pack, so if you end up finding a reasonably fitting bms let me know.
```

---
## \#136 Posted by: Lyr3x Posted at: 2018-03-14T17:50:06.657Z Reads: 177

```
Ah damn it sorry. I meant 10s1p, it was just a typo
```

---
## \#137 Posted by: lu4 Posted at: 2018-03-16T13:10:12.014Z Reads: 187

```
Do you have a printable model of this? That would be great. My self made batteries don't have a housing right now.
```

---
## \#138 Posted by: Chase Posted at: 2018-03-16T16:04:04.583Z Reads: 191

```
Let us know if you find a reasonable BMS that will fit
```

---
## \#139 Posted by: Lyr3x Posted at: 2018-03-19T14:29:21.948Z Reads: 196

```
I will publish the printable files here when i tested them by myself. This will take a while. 
I'll order the batteries next month and this week i want to start printing the Case (may need some iterations).

When i build everything i'll post all used parts etc.
```

---
## \#140 Posted by: Maxid Posted at: 2018-04-03T08:21:18.857Z Reads: 200

```
I want just the deeeeeeeck

https://media.giphy.com/media/13AXYJh2jDt2IE/giphy.gif
```

---
## \#141 Posted by: lu4 Posted at: 2018-04-04T06:55:48.103Z Reads: 199

```
I did build some spare Batteries with VTC5 18650s and like them very much. Only 2500mAh, but the board isnt beeping for about 7-8km.
Just ordered 21700 cells... 4000mAh at continuous 30A discharge current. ( : That should give about 13km without beeping...
```

---
## \#142 Posted by: esk8jpn Posted at: 2018-04-04T07:53:11.204Z Reads: 185

```
Hi @lu4 

I think that cell is Samsung SDI 21700 40T.
Where did you order the cells?

I wanna buy it., too.
I'm looking for a seller of that cell.
```

---
## \#143 Posted by: TranxFu Posted at: 2018-04-04T07:59:44.024Z Reads: 179

```
I don't 21700 cells will fit there. At least not with the case on.
```

---
## \#144 Posted by: Lyr3x Posted at: 2018-04-10T16:11:14.712Z Reads: 182

```
Did anyone found a reasonable small bms for 10s?

Everything i found is just too big...
```

---
## \#145 Posted by: Chase Posted at: 2018-04-10T19:45:48.848Z Reads: 180

```
Nope. Good luck. I’m about to just switch out the cells. @SilentException how did open up the battery case? Careful dremel work?
```

---
## \#146 Posted by: aigenic Posted at: 2018-04-10T21:48:20.645Z Reads: 185

```
The smallest i know: 
https://www.electric-skateboard.builders/t/small-bestech-bmss/25819

Also you could buy something like 12 pin connector and use external BMS? It is not good solution, but it might work :) I have one if you would be interested :) 
But I would personally rather use BMS inside the deck and jsut for charging :)
```

---
## \#147 Posted by: Lyr3x Posted at: 2018-04-11T05:42:55.389Z Reads: 175

```
So, do we know that the esc can handle discharge (prevent overdischarge)? If so, i'll order one of this :slight_smile:

Edit: The bottom of my case is fitting perfectly (very tight). Its a bit larger than the original case, so we got a little more space. Printing the lid tomorrow or at the weekend.

I published the files on thingiverse :slight_smile: : https://www.thingiverse.com/thing:2857831

Keep in mind that i just test printed the bottom yet!
```

---
## \#148 Posted by: lu4 Posted at: 2018-04-16T12:15:25.215Z Reads: 165

```
I ordered 18650 BASEN 3500mAh cells from Banggood. Use the BASEN cells for long time in RC-Flight. 21700 will fit, but not with a case...
```

---
## \#149 Posted by: aigenic Posted at: 2018-04-16T12:20:47.508Z Reads: 164

```
BASEN cells are bit overrated from what I know :(
```

---
## \#150 Posted by: lu4 Posted at: 2018-04-16T12:45:22.717Z Reads: 165

```
Not, from what i know. ( : They are about 5,50€ each on Banggood (rabatt actions from time to time) and 100% of my cells had more capacity then labled.
```

---
## \#151 Posted by: esk8jpn Posted at: 2018-04-16T13:08:09.356Z Reads: 159

```
Thanks @lu4 !
Have you actually extended the cruising range with your purchased cell?
```

---
## \#152 Posted by: mikenyc Posted at: 2018-04-16T13:14:27.912Z Reads: 162

```
what have you heard about the basen cells? I'm curious.

were the the 18650? their prices are intriguing.
```

---
## \#153 Posted by: lu4 Posted at: 2018-04-16T13:19:45.528Z Reads: 161

```
Sure. With the original Samsung 22P (2200mAh) I get about 6km and with the basen it is about 9km
```

---
## \#154 Posted by: lu4 Posted at: 2018-04-16T13:22:18.273Z Reads: 157

```
I just ordered 21700 BASEN cells with 4000mah and real constant 30A! ( : Sounds lovely!
```

---
## \#155 Posted by: esk8jpn Posted at: 2018-04-16T13:22:41.658Z Reads: 166

```
That's great!

This is a Basen 30A 4000mAh 21700 Cell test result.
https://www.e-cigarette-forum.com/threads/bench-test-results-basen-30a-4000mah-21700%E2%80%A6ridiculously-overrated-just-an-average-20a-battery.836909/

The battery space of the Lou board is so narrow that I think 21700 cells are a good choice.
```

---
## \#156 Posted by: lu4 Posted at: 2018-04-16T13:30:47.188Z Reads: 166

```
Okay Thanks. We will see. I Love my 18650 ans the all have more them the 3500mAh / 3200mAh rated, ans i have 30 pcs of them.. I will let you know when they arrive.
21700 is the perfect size for this board if you go without the battery housing.
```

---
## \#157 Posted by: Lyr3x Posted at: 2018-04-16T20:58:40.687Z Reads: 170

```
I ordered VTC6 and a bestech bms (for charging) and some xt30 connectors. Hopefully everything fits into my case. Any feedback is very welcome
```

---
## \#158 Posted by: Lyr3x Posted at: 2018-04-23T19:41:21.754Z Reads: 181

```
I updated my thingiverse files. Everyhting fits very tight and it should be rigid enough :slight_smile: The holes for the the connectors were a little to small. Also the logo did not printed well in petg, caused by the bad bridging performance. Its a lot better now.

If somebody in germany without a printer want a case, you can pm me :slight_smile:

here are some pictures:

![18650_inside|690x480](upload://kjBR3XuGQmPZcqkZMRcj6bdf7sU.jpg)![IMG_20180424_201512|666x500](upload://idnX8rW3wBrcvhVJehTTK65m3QY.jpg)![IMG_20180424_201447|666x500](upload://gHzdGrDkHadAkxb6JiUMy5EIA9d.jpg)![IMG_20180424_201830|666x500](upload://mg3DSmv6qF0ESMOkBrp6z0t1f0w.jpg)![IMG_20180424_201842|666x500](upload://p2tuN0QDJpCRPe6q8UntaAnRlde.jpg)
```

---
## \#160 Posted by: Chase Posted at: 2018-04-25T16:19:59.610Z Reads: 174

```
Which bms did you end up getting?
```

---
## \#161 Posted by: Lyr3x Posted at: 2018-04-25T16:32:09.233Z Reads: 171

```
the HCX-D239 from bestech. Just for charging obviously
```

---
## \#162 Posted by: Chase Posted at: 2018-04-25T19:36:07.244Z Reads: 173

```
Looks really nice. Good job.
```

---
## \#163 Posted by: esk8jpn Posted at: 2018-04-25T21:25:23.413Z Reads: 168

```
nice work!
```

---
## \#164 Posted by: Lyr3x Posted at: 2018-04-26T09:32:11.572Z Reads: 167

```
Thank you :slight_smile:
 
I have two HCX-D239, so if somebody want to buy the spare one just pm me.. Otherwise i need to build a second pack :smiley:
```

---
## \#165 Posted by: BasWoods Posted at: 2018-05-03T12:41:06.989Z Reads: 162

```
Which weld do you change tho?
```

---
## \#166 Posted by: esk8jpn Posted at: 2018-05-04T01:51:01.816Z Reads: 165

```
Hope this helps.
http://www.electric-skateboard.builders/t/diyeboard-com-china-factory-direct-retail-electric-skateboard-diy-kits-and-parts/32666/1516?u=esk8jpn
```

---
## \#167 Posted by: Maxid Posted at: 2018-05-16T08:01:26.113Z Reads: 162

```
Hey guys I just got a second hand Lou 1.0. My first impression: size is awesome but man this thing sucks. The XT30 battery connector broke and also has the flimsiest wires I have ever seen. I normally wouldn't even charge my battery with such thin cables. The ESC cuts out at times and seemingly loses connection with the remote. Brake force is super low and on a slight incline the board will not stop you. Motor gets HOT. The lid does not stay on the deck due to the use of just velcro, I like the push to start function though without a button.

So what can we do? My plan is to try a Focbox instead of the ESC. Has anybody tried to find a new way to fix the lid to the deck? I thought about gluing nuts to the inside and have screws through the lid hold it - but that would diminish the stealthy look a bit :thinking:
So I am open for ideas.
```

---
## \#168 Posted by: Lyr3x Posted at: 2018-05-16T09:33:17.718Z Reads: 160

```
> I normally wouldn’t even charge my battery with such thin cables. 

Well for the 2 Amps charger these cables are thick enough. Should absolutely not be a problem, but i understand why you are complaining. 

> The ESC cuts out at times and seemingly loses connection with the remote. 

I rode this thing about 150km now and i dont had even a single connection issue. Maybe your ESC or the BT module is faulty

Do you have the "full velcro" ? If not send a mail to so flow and they will send it to you for free. Since i "upgraded" from the alpha to the beta product i dont had any issues with the deck
```

---
## \#169 Posted by: Maxid Posted at: 2018-05-16T09:57:29.648Z Reads: 155

```
[quote="Lyr3x, post:168, topic:43606, full:true"]
Well for the 2 Amps charger these cables are thick enough. Should absolutely not be a problem, but i understand why you are complaining. 
[/quote]
I said that to make a point rather than be 100% true :smile:. But for power wires that are supposed to see almost 40A (they advertise the board as 1500W which at 10S is ~40A) they are unacceptable - same with using XT30. No idea how they can sleep at night when using XT30 as battery connector even on the dual drive boards. An XT60 would have already been a significant upgrade.

[quote="Lyr3x, post:168, topic:43606, full:true"]
I rode this thing about 150km now and i dont had even a single connection issue. Maybe your ESC or the BT module is faulty
[/quote]
Not sure if it's connection or something else. Just noticed it this morning on my first real ride. 5min in the board did not respond. I carried it the rest of the way and when I tried it again it worked as if nothing ever happened. But I want to try a Focbox anyway simply because of the braking power.

[quote="Lyr3x, post:168, topic:43606, full:true"]
Do you have the "full velcro" ? If not send a mail to so flow and they will send it to you for free. Since i "upgraded" from the alpha to the beta product i dont had any issues with the deck
[/quote]
Already sent one this morning after reading about it on the facebook group. But since the board was second hand and they now sell the velcro for 40$ on their website I doubt they will send me one for free. Would be nice though. I am just a little suspicious that on the 1.0 there is only very little material for the velcro to hold on to.
```

---
## \#170 Posted by: Lyr3x Posted at: 2018-05-16T10:14:41.379Z Reads: 145

```
You are totally right :slight_smile:. i think there are some limitations with the Stock ESC. This Board never uses the advertised  Power :smile:. Otherwise these cables and the connector will burn like hell if you ride uphill 

I bought a used 1.0 ans they sent me a velcro Kit for free and it sticks very well
```

---
## \#171 Posted by: Lyr3x Posted at: 2018-05-16T11:25:30.207Z Reads: 145

```
Additional Info: I updated my thingiverse project today https://www.thingiverse.com/thing:2857831

Made some major changes in the design. I also changed the cell arrangement which shows how i did it in my case.
```

---
## \#172 Posted by: Maxid Posted at: 2018-05-17T21:44:38.195Z Reads: 147

```
They wrote me an email saying I could order the one from the website for 40$ :(
```

---
## \#173 Posted by: Chase Posted at: 2018-05-17T21:53:51.058Z Reads: 144

```
Order what?
```

---
## \#174 Posted by: Maxid Posted at: 2018-05-17T21:59:10.589Z Reads: 145

```
Velcro set to replace the thin strips I have on mine.
```

---
## \#175 Posted by: Chase Posted at: 2018-05-17T21:59:55.181Z Reads: 144

```
Yeah 40 bux is crazy and then I’m sure shipping to USA is outrageous especially when it should come standard
```

---
## \#176 Posted by: Maxid Posted at: 2018-05-17T22:00:50.550Z Reads: 150

```
I am from Germany :slight_smile:
Yeah it's weird - they even have this video  https://m.youtube.com/watch?v=e0sNg17hFZ8 where they say that you can get it for free. Not sure what's going on.
```

---
## \#177 Posted by: Chase Posted at: 2018-05-17T22:03:47.269Z Reads: 148

```
Maybe we could email them and see what’s the deal. We could cite that video.
```

---
## \#178 Posted by: Maxid Posted at: 2018-05-17T22:04:49.326Z Reads: 146

```
I did that already in my initial email to them. Let's see what they say after my second email from today.
```

---
## \#179 Posted by: Lyr3x Posted at: 2018-05-18T07:33:26.958Z Reads: 145

```
Pfff 40$ is hularious.. If they wont send it for free you May search for the Same Type of velcro and Cut it by yourself...
```

---
## \#180 Posted by: Maxid Posted at: 2018-05-18T08:19:58.325Z Reads: 150

```
any idea where i could find it or what type i have to look for? standard velcro is too thick unfortunately.
```

---
## \#181 Posted by: Lyr3x Posted at: 2018-05-18T08:42:03.007Z Reads: 146

```
absolutely no idea :-1:
```

---
## \#182 Posted by: Truebanana Posted at: 2018-05-18T16:21:04.141Z Reads: 154

```
I'm a Kickstarter backer and asked for the upgrade kit for 1.0. Everything was fine and they were replying to me, but no news since one month ago
```

---
## \#183 Posted by: Maxid Posted at: 2018-05-19T16:47:58.315Z Reads: 156

```
Now we're talking: [img]upload://nS7oVuH8fEmgGJwdJKgDP1WkRmi.jpg[/img]

Had to make me an adapter for the Focbox XT60 to XT30 and the sensor wires need a 6pin jst connector (waiting for @bevilacqua to help me out - thanks bro)
So much more power and responsiveness - and the breaking is a lot safer now. Feels like a 1000$ difference. Now we just need to figure out how to put the VESC to sleep without a bulky switch...
BTW: anyone in need of a spare ESC? ;)
```

---
## \#185 Posted by: Maxid Posted at: 2018-05-19T17:25:20.110Z Reads: 169

```
Impossible. 12 cells could fit and a single VESC. This deck is not made for dual drives. A cheap Chinese dual ESC fits but who really wants that? ;)

This might be interesting to some:
![IMG_20180519_191327|375x500](upload://hv1kHQhn27iqNrMYQCeQfajHvng.jpg)
Even though my board is the 1.0 I got a 2.9Ah battery and it is made out of Panasonic PF cells. Lygyte does not have a discharge curve unfortunately. Anyone got a comparison to 30Q cells?
```

---
## \#186 Posted by: Maxid Posted at: 2018-05-21T07:57:51.657Z Reads: 165

```
Any news regarding the 21700s?
```

---
## \#187 Posted by: TranxFu Posted at: 2018-05-27T21:44:39.681Z Reads: 159

```
How's the Lou with a focbox and the original Single drive hub ? I've got a belt driven 6374 and it got quite the oomph.. Too much for my taste and for the use of the board tbh. I consider switching back to the hub.
```

---
## \#188 Posted by: Maxid Posted at: 2018-05-28T09:47:00.302Z Reads: 160

```
Well the Focbox is way better than the standard ESC but it still feels a little weak. Uphill is basically not doable and the board cuts out. I am not sure if the problem is due to my Nyko Kama or whether the battery has an overcurrent protection. What battery are you using? I am thinking of making one from 30Q but they are not available at nkon right now :(
```

---
## \#189 Posted by: mistahhmoll Posted at: 2018-06-21T12:35:14.626Z Reads: 158

```
this might me a stupid question, but would this (http://www.diyeboard.com/dual-belt-drive-1400w2-n5055-motor-power-truck-p-658.html) be too powerful? thanks in advance!
```

---
## \#190 Posted by: jdnicholson Posted at: 2018-06-22T01:28:31.206Z Reads: 158

```
I have run that setup on a different board. You will be drawing a bunch of power from a very small battery. I'd recommend sticking with a single drive just from a power draw perspective. But in saying that I hate single drive. 

Have you or anyone else considered one of the new ownboard/wowgo esc and hub combo??
I got a set recently during a group buy and they are fantastic!!! So damn smooth and fast. Plus the ESC is tiny so it shouldn't be an issue in the enclosure. Im sure the battery wont like it though.
```

---
## \#191 Posted by: sunnyD Posted at: 2018-06-22T17:09:10.208Z Reads: 155

```
does anyone have the truck size for the Lou board? I cant find it anywhere, thanks in advance!
```

---
## \#192 Posted by: bartroosen12 Posted at: 2018-06-22T17:42:34.716Z Reads: 158

```
Same as standard trucks I think (180mm)
![IMG_20180622_194151|666x500](upload://9smA0MpDjWzjts0zNndPrWq9X39.jpg)
```

---
## \#193 Posted by: sunnyD Posted at: 2018-06-22T17:43:10.977Z Reads: 150

```
oh ok, thats nice. thanks bud
```

---
## \#194 Posted by: ymzkala04 Posted at: 2018-06-28T04:16:18.219Z Reads: 150

```
For those of you who are familiar with the Lou 3.0 ESC, is there a way to pair it with another 2.4Ghz remote? I hate this joystick. I emailed SoFlow and they said it would only pair with a Lou remote. My understanding is that pairing requires a (unique?) receiver, which seems to be built into this ESC (and has a button). I bought the newest Meepo remote (I will use it either way) and will test it out when it arrives.
```

---
## \#195 Posted by: bartroosen12 Posted at: 2018-06-28T08:05:24.238Z Reads: 146

```
You should be able to connect another remote like the ownboard/meepo/wowgo remotes or the remotes that dickho and diyeboards sell.
```

---
## \#196 Posted by: Maxid Posted at: 2018-07-12T07:41:34.985Z Reads: 151

```
Went with a belt drive - so much better and finally some uphill and braking power even with the stock battery.
Had to design and print a pulley to get a proper ratio 
https://www.electric-skateboard.builders/t/3d-files-for-kegel-pulley/61625
![29|375x500](upload://mQpafsmqgOzaLZnlFTawgTEeAas.jpg)
```

---
## \#197 Posted by: TranxFu Posted at: 2018-07-12T13:09:55.933Z Reads: 143

```
Be careful maxid :D my printed pulleys melted after one ride. What material did you use ?
```

---
## \#198 Posted by: Maxid Posted at: 2018-07-12T14:15:59.637Z Reads: 146

```
it's TPU 95A - feels amazing. I had printed pulleys before (namely ABS+ and PETG) and all of them held up pretty well. Reason why I had to switch them out was me doing something stupid (for example motor mount screws came loose one time because i did not use loctite and they jammed the wheel) not the material being bad.
```

---
## \#199 Posted by: Maxid Posted at: 2018-07-15T09:14:01.644Z Reads: 143

```
![IMG_20180715_110357|666x500](upload://6dWF4ic26QamKJZ6KK6IsFDyYVm.jpg)
Thanks @Martinsp :+1:
```

---
## \#200 Posted by: bartroosen12 Posted at: 2018-07-20T14:32:45.071Z Reads: 143

```
I have recently upgraded the batteries for someone to sony vct6 cells. The board runs great right now. It's only a 10S1P but you do 10km riding with almost always full throttle (before with the shitty Samsung cells I could only get around 5km and hills were almost impossible).
The board doesn't beep anymore when going uphill because these cells can handle like 30A with no problem.
![IMG_20180623_231814|666x500](upload://8f3dIAIIjWVH80YVSg2HGNy67Yt.jpg)![IMG_20180623_210020|666x500](upload://lZl99thJuNzviH8mdMcyL50oXoR.jpg)
![IMG_20180623_205931|277x500](upload://vBtkzPQ6qObh2mte4sQQcc1qLBQ.jpg)
The battery looks just like before so taking it on a plane is no problem while the Wh amount is actually a bit to much but you won't notice from the outside :smile:
```

---
## \#201 Posted by: Grozniy Posted at: 2018-07-20T14:39:07.818Z Reads: 138

```
Beautiful. I so want a lou deck
```

---
## \#202 Posted by: Chase Posted at: 2018-07-20T15:38:06.271Z Reads: 143

```
Gotta love these tiny bms. Thanks to @Lyr3x for the hookup and for making the 3D printed case.

![image|374x500](upload://1WcQlKSxAl1VsqjhidPSw8Bu3fc.jpeg)
```

---
## \#203 Posted by: Chase Posted at: 2018-07-20T18:52:19.035Z Reads: 140

```
Anyone know what kind of Velcro that lou ended up using after switching from the orroginal stuff? Everything I buy is too thick or weak for holding the battery in place
```

---
## \#204 Posted by: esk8jpn Posted at: 2018-07-21T01:57:17.201Z Reads: 138

```
Hey guys

I recently found this new Chinese esk8 company.
https://eflowboards.com/

Noteworthy is that you can buy only the deck.
It is like the Lou, a compact integrated deck.
![x2|600x328](upload://1Sr3mGBKJCZA5yah72qP2KeEd7J.jpg)
https://eflowboards.com/collections/parts-accessories/products/deck-s

https://www.youtube.com/watch?v=SAsCR4cTEuA
```

---
## \#205 Posted by: Maxid Posted at: 2018-07-21T07:18:41.897Z Reads: 136

```
It's unfortunately just not as nice looking as the Lou.
```

---
## \#206 Posted by: Chase Posted at: 2018-07-26T00:06:00.571Z Reads: 135

```
Out of my 4 and 1/2 boards I use this by far the most. Such a convenient size and weight. These 30Q with bestech bms was a significant upgrade.
```

---
## \#207 Posted by: ymzkala04 Posted at: 2018-07-30T01:57:29.076Z Reads: 135

```
Turns out I wasn't able to pair out of the box. The Lou original ESC has a 'pair' button and I tried that with no luck. Has anybody made another remote work with this ESC?
```

---
## \#208 Posted by: boardman Posted at: 2018-08-02T06:45:40.333Z Reads: 133

```
Found another deck that might suit a similar build:
https://milespower.com/collections/miles-accessories/products/deck?variant=12212416512123
```

---
## \#209 Posted by: Maxid Posted at: 2018-08-02T07:01:16.768Z Reads: 124

```
that actually looks really nice - would love to get a picture from the inside though to see if it fits 18650 and how much electronics we could fit.
```

---
## \#210 Posted by: Chase Posted at: 2018-08-02T07:01:49.164Z Reads: 122

```
Wish that page gave weight, enclosure dimensions, and pictures from different angles
```

---
## \#211 Posted by: Maxid Posted at: 2018-08-02T07:03:16.962Z Reads: 123

```
they also don't ship to Germany apparently:
![image|624x264](upload://x3AZPH05yqLk7PH5FtLEmercIcR.png)
```

---
## \#212 Posted by: boardman Posted at: 2018-08-02T07:30:21.481Z Reads: 114

```
[quote="Chase, post:210, topic:43606, full:true"]
Wish that page gave weight, enclosure dimensions, and pictures from different angles
[/quote]

I sent them a message to ask for specifics but from what I can guess from the pictures, it looks like it can just a fit a 10s1p battery and an ESC
```

---
## \#213 Posted by: esk8jpn Posted at: 2018-08-02T11:15:25.944Z Reads: 123

```
It looks like a 10S2P pack. 
https://milespower.com/products/single-battery
![3_battery_1080x__01|304x500](upload://btbgHkb3VjD7aSKkJjMoCyX6rGX.jpg)
```

---
## \#214 Posted by: bartroosen12 Posted at: 2018-08-02T11:31:37.819Z Reads: 115

```
3Ah is possible with 10S1P.
But maybe for the 4Ah they used the Sanyo NCR20700B with a 10S1P setup?
```

---
## \#215 Posted by: pat.speed Posted at: 2018-08-02T11:57:25.691Z Reads: 114

```
These decks look perfect for my upcoming build. We should invite them to the forum and maybe get a group buy going for all the people outside the US. 

I also really like there description, the humour made me giggle a few times 🙂
```

---
## \#216 Posted by: Maxid Posted at: 2018-08-02T12:09:16.757Z Reads: 113

```
agree - if they play this right SoFlow got basically killed in an instant.
I'd love to see this deck next to a Lou - small commuter boards are the future for esk8s!
```

---
## \#217 Posted by: pat.speed Posted at: 2018-08-02T12:13:37.171Z Reads: 115

```
I think they use the same hubs too
```

---
## \#218 Posted by: esk8jpn Posted at: 2018-08-02T13:11:08.706Z Reads: 117

```
@bartroosen12
Oops, I completely thought they were using cheap cells like 1500 mAh and 2000 mAh.
```

---
## \#219 Posted by: boardman Posted at: 2018-08-02T16:42:47.157Z Reads: 124

```
Received from customer service:
"The current battery is 20.7mm tall, 122mm wide and 205mm long."

![38200043_688988638122930_4515734791177371648_n|242x500](upload://gWfm91gZ5hdKc1CUlmVz57u2mz6.jpg)![38297859_688988584789602_7587291390330011648_n|690x335](upload://AsJfLpBfWxXpeYyOvAwJwKizse5.jpg)
```

---
## \#220 Posted by: Grozniy Posted at: 2018-08-02T16:45:37.557Z Reads: 121

```
So it would only fit 10S1P 20700 cells. But was is the size of whole compartment including esc space?
```

---
## \#221 Posted by: bartroosen12 Posted at: 2018-08-02T17:11:33.940Z Reads: 129

```
Just mailed them too :smile: 
The space you got is 350mm x 127mm and 21 max height.
![inbox|281x500](upload://sgAOqQXW5kb01zfBwWYiAOIlCbp.png)
10S2P sanyo with small bms and the ownboard/wowgo dual hub bms would be awesome!
![IMG_20180802_192732|285x500](upload://tRsLYelCfW4G2CTsVaU8LhD4edR.jpg)
```

---
## \#223 Posted by: Maxid Posted at: 2018-08-02T19:10:34.276Z Reads: 116

```
Holy shit - I love that you guys came out and actually support the builders. We had companies before that wouldn't sell to people that did not buy a complete. How can Europeans get hands on a deck?
```

---
## \#224 Posted by: uigiroux Posted at: 2018-08-02T19:15:50.830Z Reads: 123

```
Dude is that the Nextboard??  I freaking love that design.  How'd you get one of those??  Would you consider selling?
```

---
## \#225 Posted by: Rob.Rast Posted at: 2018-08-02T19:17:32.448Z Reads: 125

```
Hey guys, this is Rob from Miles Board. 
Huge shout for mirin' our decks! 

We'd be thrilled to see what kind of builds you come up with!
To answer a few questions:

Outside Dimensions: 26.5" x 7.5" x .98" thick (670mm x 190mm x 25mm) Note: kicktail sits at 1.63" high (41.3mm)

Cavity Dimensions: 13.75" x 5" x .83" ( 350mm x 127mm x 21mm)

Weight 700g, 1.5lbs

Currently the deck on the site is offered as a replacement if anyone breaks theirs. It does not come with the lid/bolts.  If you guys are interested we could set up a group buy package with the deck, lid, bolts and whatever else you want. Let me know!

About the battery- it's actually not 18650s but a LiPo pack. They're 36V in both 3AH and 4AH capacities. You could just fit an 18650 pack in with no or minimal shell around it. 

Thanks and give us a shout with any questions.
```

---
## \#226 Posted by: uigiroux Posted at: 2018-08-02T19:20:05.536Z Reads: 126

```
Is this the board you are making?

![Screenshot_20180802-141828_Chrome|281x500](upload://wxTMWPEvhjBeViBlIZygxCkFCv7.jpg)

How much for the board with lid and bolts, etc, no battery or motors, just the complete board?
```

---
## \#227 Posted by: Rob.Rast Posted at: 2018-08-02T19:33:53.793Z Reads: 122

```
Yes it is. For a group buy of 10 or so we can do the kit for the same price as the bare deck ($119). Lead time about 2-3 weeks.
```

---
## \#228 Posted by: uigiroux Posted at: 2018-08-02T19:36:14.863Z Reads: 119

```
I definitely will want one if a GB is organized.  Is the kit basically the complete deck with lid and bolts, etc.  The bare deck just the deck without the lid or anything else?

What would one complete deck cost if I was the only one buying one?
```

---
## \#229 Posted by: Rob.Rast Posted at: 2018-08-02T19:39:37.422Z Reads: 111

```
That's correct. Bare deck is just the piece pictured. Kit would include the deck, carbon fiber lid and 10 m3x8 lid bolts.
```

---
## \#230 Posted by: sunnyD Posted at: 2018-08-02T19:41:17.100Z Reads: 117

```
Ohh this is really intriguing. I’d really like to test it before I hopped on. Do you have a place in NorCal some of us can try it at?
```

---
## \#231 Posted by: Rob.Rast Posted at: 2018-08-02T19:44:27.727Z Reads: 117

```
Where in Norcal are you? We could hook you up with a rider in Folsom if you're nearby, I'll be in El Dorado Hills/Sac with a board this weekend if you want to shred!

R
```

---
## \#232 Posted by: uigiroux Posted at: 2018-08-02T19:46:06.960Z Reads: 126

```
I'm a bit confused about something though.  I messaged Nextboard directly a few months back and was told the cost for the board would be $595 + p&p.  How are you able to sell it for such a dramatically lower price?  Did you take over production of this board?

![Screenshot_20180802-144447_Outlook|281x500](upload://iMdbepkDm7rf3PzyihcMsGoPdv2.jpg)

![Screenshot_20180802-144525_Outlook|281x500](upload://4MOv4qzYXHo3osbDBxgThOKM6Mc.jpg)

The dimensions they listed are very different from the dimensions you have listed also...

[quote="Rob.Rast, post:225, topic:43606"]
Outside Dimensions: 26.5" x 7.5" x .98" thick (670mm x 190mm x 25mm) Note: kicktail sits at 1.63" high (41.3mm)

Cavity Dimensions: 13.75" x 5" x .83" ( 350mm x 127mm x 21mm)
[/quote]
```

---
## \#233 Posted by: Grozniy Posted at: 2018-08-02T19:51:58.216Z Reads: 116

```
Hi Rob. Very nice deck. Do you have a black only lid without pink?
Would be interested in GB
And would you ship to EU (Iceland) ?
```

---
## \#236 Posted by: uigiroux Posted at: 2018-08-02T20:54:24.881Z Reads: 120

```
Ok cool, that answers my concerns :smile: So how many decks with an integrated enclosure do you currently offer?
```

---
## \#237 Posted by: Maxid Posted at: 2018-08-02T20:59:16.490Z Reads: 120

```
I want one to Germany!
```

---
## \#238 Posted by: uigiroux Posted at: 2018-08-02T21:02:56.406Z Reads: 124

```
Ok I see what I did, lol.  The angle of the pic of your board had me thinking your board was a different one, they do look very similar from the pic I saw.  I thought it was this one.

![Screenshot_20180404-201129|690x388](upload://h4vw0x4Go6GR3JUt9eInFx1cu3l.jpg)

Really like your design though.  What's the max battery pack this can for with dual VESC's?
```

---
## \#239 Posted by: boardman Posted at: 2018-08-02T21:06:04.624Z Reads: 119

```
It doesn't use 18650s so you have to be creative. They have an existing battery they're selling that is 36v at 4AH if you don't want to make your own battery pack. It leave enough room for dual Vesc's
```

---
## \#240 Posted by: uigiroux Posted at: 2018-08-02T21:26:47.110Z Reads: 116

```
I'd make my own pack from some 20650's :wink:
```

---
## \#241 Posted by: pat.speed Posted at: 2018-08-02T21:27:26.367Z Reads: 114

```
C’mon bro stop bombarding them with questions, how would they know the answer to that when they’ve already stated they use lipo batteries. Work it out, like @bartroosen12
```

---
## \#242 Posted by: uigiroux Posted at: 2018-08-02T21:29:23.586Z Reads: 110

```
I asked like 2 questions then made a few comments saying how I liked their product. I hardly feel that constitutes 'bombardment'.
```

---
## \#243 Posted by: Maxid Posted at: 2018-08-02T21:34:02.256Z Reads: 109

```
What are 20650s?
```

---
## \#244 Posted by: pat.speed Posted at: 2018-08-02T21:35:08.200Z Reads: 112

```
I don’t want to argue so let’s just get this group buy going!

I’m down for 1 full deck without grip, I am in Aus so I’ll cover extra shipping cost. Who’s next?
```

---
## \#245 Posted by: uigiroux Posted at: 2018-08-02T21:37:32.086Z Reads: 112

```
Agreed.  I'm down for a full board as well and am in the US.
```

---
## \#246 Posted by: uigiroux Posted at: 2018-08-02T21:41:52.329Z Reads: 112

```
20650's is a new size for Li-on cells.  It's not widely used as 18650's are the standard, and then 20700, and 21700 cells are the newest cells that are becoming more popular, and will likely replace the 18650 as the standard for cell size. 20650's are also new, but very few are made in compassion to the other ones I just listed.  Though, I know of one or two cells in that size by Samsung and Sanyo that are very good.
```

---
## \#247 Posted by: Chase Posted at: 2018-08-02T21:45:15.624Z Reads: 110

```
Same. I would like one
```

---
## \#248 Posted by: Grozniy Posted at: 2018-08-02T21:50:56.022Z Reads: 111

```
So how much is shipping to Iceland @Rob.Rast?
```

---
## \#249 Posted by: uigiroux Posted at: 2018-08-02T21:52:15.875Z Reads: 109

```
One thing I think needs to be addressed, is to organize a group buy you need to be a level 3 member.  Not my rule, but the mods are very strict about that.  They do allow you to sell a product, providing that you already have it in stock and ready to ship.  I don't know the exact rules, but I'd recommend checking them out before a mod shuts down the thread.
```

---
## \#250 Posted by: pat.speed Posted at: 2018-08-02T21:52:21.004Z Reads: 109

```
Yes, this could be a killer
```

---
## \#251 Posted by: uigiroux Posted at: 2018-08-02T21:53:41.099Z Reads: 116

```
Do you offer just the board for sale on your website?  I didn't see that, but perhaps that could be an option.
```

---
## \#252 Posted by: pat.speed Posted at: 2018-08-02T21:54:27.292Z Reads: 115

```
They do just without a lid
```

---
## \#253 Posted by: Maxid Posted at: 2018-08-02T21:55:25.229Z Reads: 121

```
I think the level 3 thing is regarding forum members that try to buy from a company and then pass it on. Not when you are talking to the company itself. 
@moderators could we move this groupbuy/new deck topic into its own thread?
```

---
## \#260 Posted by: Grozniy Posted at: 2018-08-03T08:17:43.985Z Reads: 116

```
If people don't want to drill holes for e-switch, they could use @Martinsp [Push to start switch](https://www.electric-skateboard.builders/t/push-to-start-switch-out-now/60879/64?u=grozniy)
```

---
## \#261 Posted by: tex Posted at: 2018-08-03T09:29:32.410Z Reads: 119

```
Pretty cool ;-)
```

---
## \#254 Posted by: treenutter Posted at: 2018-08-05T19:06:13.071Z Reads: 70

```
18 posts were split to a new topic: [Group Buy - Miles Board Deck](/t/group-buy-miles-board-deck/63935)
```

---
## \#262 Posted by: Chase Posted at: 2018-08-07T05:27:25.999Z Reads: 75

```
Just blew my first esc :face_with_symbols_over_mouth:
I feel like someone shit in my cereal. Somehow the positive wire on the esc broke or burned through. When I tried to solder it back onto the chip I must have made the solder joint just slightly too big or something because it immediately blew the xt30s on the battery and the esc. Not sure how the short happened because the negative wire was still far away from my solder for the positive but I clearly screwed it somehow.

It was weird because it locked up my hubs after until I unplugged the fried esc from the motors.
```

---
## \#266 Posted by: Maxid Posted at: 2018-09-06T10:41:19.092Z Reads: 72

```
sure - but ugly is still ugly even with better suited dimensions for DIY.
Spend some more time on the design - check out the miles board (a rebranded Winboard GT3 Mini AFAIK) for example to see how a good looking deck is supposed to look like.

Edit: I also flagged your posts - its been three times the same image
```

---
## \#267 Posted by: Maxid Posted at: 2018-10-24T10:11:38.047Z Reads: 71

```
@pat.speed what happened to that group buy of the miles deck? The page doesn't even exist anymore.
```

---
## \#268 Posted by: pat.speed Posted at: 2018-10-24T11:29:09.500Z Reads: 70

```
It was a flop, we didn’t get enough people on board... pun not intended. I think the page must have been closed by mods just to stop everything piling up, I’m pretty sure they delete old things. I would have liked that deck but I think I’m going to like the deck I’m making even more 😃 Mine is much slimmer, a bit longer and wider and has much more room for electronics, it’s not cool carbon fibre but oh well
```

---
## \#269 Posted by: anciltech Posted at: 2018-11-25T17:36:16.823Z Reads: 72

```
Did you notice an improvement with how steep of a hill you could climb or top speed? 
It looks like you desoldered the old battery, correct?
```

---
## \#270 Posted by: bartroosen12 Posted at: 2018-11-26T12:05:20.695Z Reads: 77

```
The battery was spotwelded so we only desoldered the balance wires and + and - to remove the battery.

I'm sure it can do better hills because before the board started beeping because the cells reached their cutoff voltage with small hills.
Now the weakest part isn't anymore the battery, I have no idea how steep the hill is which I did (it was a bridge) so no insane hill but it went up pretty easy.

Topspeed was increased just a tiny bit 2km/h extra
```

---
## \#271 Posted by: Chase Posted at: 2018-11-26T19:15:38.380Z Reads: 74

```
The battery was a huge huge upgrade for mine. I used to not be able to even get up mold hills without beeping. The other day I took it 11 miles before beeping at all. Blasted up hills with my 30q cells. Night and day difference
```

---
## \#272 Posted by: G-Motionboard Posted at: 2018-12-19T04:32:13.800Z Reads: 76

```
for this small board, what you can do is really limited, maybe just change to dual motor and big capacity battery to get faster speed and bigger range as you can. but no matter how you improve it, there is no doubt this board is not good for up hills(because of the deck size is too samll ) and also the range can't be longer than 10miles.
It's better just keep it as a board for short distance communicating and DIY another new longboard as you need.
```

---
## \#273 Posted by: Chase Posted at: 2019-04-04T20:01:46.036Z Reads: 66

```
My 30q mod takes me up pretty damn steep hills without an issue. I really want to upgrade to 30T cells but I doubt it’ll fit the extra few mm.
```

---
## \#274 Posted by: esk8jpn Posted at: 2019-04-05T00:46:22.546Z Reads: 68

```
You should do it. cheers!
https://www.electric-skateboard.builders/t/soflow-lou-1-0-issues/72065/18
```

---
## \#275 Posted by: Chase Posted at: 2019-04-05T00:59:33.783Z Reads: 71

```
![image|375x500](upload://cXnVS5qxyozPVKhkFYzmgVl331d.jpeg) 

I may try but I doubt it’ll fit. Just that few extra mm for each cell adds up and I don’t think it will end up fitting.
```

---
## \#276 Posted by: esk8jpn Posted at: 2019-04-05T02:20:14.508Z Reads: 70

```
Sorry!
For VESC based builds, I forgot that the enclosure space was very small.
```

---
## \#277 Posted by: Chase Posted at: 2019-04-05T21:38:14.922Z Reads: 70

```
Well mines a dual sine esc. It may fit if I printed a longer battery box or heat shrink wrap it instead, but even then I don’t know because the bms is too fat to lie below the cells. 

![image|375x500](upload://wtLc7OYpxMPjx5BujhinQGKQOK9.jpeg)
```

---
## \#278 Posted by: mistahhmoll Posted at: 2019-08-23T19:40:48.795Z Reads: 47

```
how did you attach the on/off button?
```

---
## \#279 Posted by: Maxid Posted at: 2019-08-24T14:43:51.067Z Reads: 44

```
3d printed holder
```

---
## \#280 Posted by: loguy Posted at: 2020-01-06T11:59:02.874Z Reads: 22

```
Hello all :slight_smile:  <br />
After 1 week of going through this amazing forum and understanding technical subjets about batteries, ESC/VESC... I come here to get some help.

2 years ago, I aquired a Louboard 1.0 through KS. I loved the form factor at that time but I understood later that components inside were poor quality... I never changed any component.
And this poor quality causes me issues to ride the board now. 

<strong>Here's the issue : Every time I take the board for a ride, after a full charge of it, I can ride (on flat roads) for 5 mins, sometimes 10 mins, sometimes 1 min, and the board stops instantly and can't restart until I charge it again. The stop appears sometimes when I'm breaking, sometimes when I fully accelerate...</strong>

Before this issue, I was fully happy with the top speed of the board and the ride duration; thus to fix that issue, should I change the ESC?
As information, I wanted to test the battery; so I made the board rides upside down, with no friction, it lasted 50 min.

Thank you in advance !  :slight_smile:
```

---
## \#281 Posted by: esk8jpn Posted at: 2020-01-07T00:53:54.946Z Reads: 18

```
> The stop appears sometimes when I’m breaking, sometimes when I fully accelerate…

That seems like a BMS problem. :face_with_raised_eyebrow:
```

---
## \#282 Posted by: loguy Posted at: 2020-01-07T10:55:14.909Z Reads: 21

```
Thanks for your answer; how to be sure? Also, the BMS doesn't seem easy to find in shops and replace it? :frowning: 
![image|375x500,75%](upload://u5tK4w9g3tWRK74lcuqZVuxlT1E.jpeg)
```

---
## \#283 Posted by: loguy Posted at: 2020-01-10T16:30:00.020Z Reads: 20

```
Does anyone can confirm that the BMS is the issue? :slight_smile:
```

---
## \#284 Posted by: esk8jpn Posted at: 2020-01-11T15:07:22.190Z Reads: 20

```
Hi @loguy sorry late.

You have the following options:

(Plan A) Get a new battery pack and replace it. This will tell you if the battery pack is broken or if the ESC is broken.

(Plan B) Find someone who can build an ESK8 battery pack in your country and ask them to create one, or request for a check of that battery pack.

Have you contacted the SoFlow?
The Lou Board Facebook group may be cheaper to get.

I have two battery packs for Lou boards that I do not use now. I want to offer you cheap, but unfortunately I live in Japan.
Shipping fee and aviation dangerous goods export procedures will not be worthwhile.

Lastly, This forum often stops because of financial problems with the owner. There are not many people here. If you need technical support for ESK8, go here.

forum dot esk8 dot news

Hope this helps.
```

---
## \#285 Posted by: loguy Posted at: 2020-01-21T14:47:47.709Z Reads: 18

```
Hey, thanks for your answer; I'm gonna try Plan A :)
```

---
## \#286 Posted by: Chase Posted at: 2020-01-21T22:09:02.974Z Reads: 16

```
As much as I dislike posting on this forum I felt I can give you some sound advice. Build a new battery with good cells. It was such a huge upgrade for my Lou 3.0. I have a bunch of boards and it’s still my main go to. 

You can see a battery I built somewhere back in this thread. I could always build you one if your not used to making them.
```

---
## \#287 Posted by: loguy Posted at: 2020-01-22T08:58:59.385Z Reads: 15

```
Thanks Chase for your answer :slight_smile:
 I've found the photo of your battery; is it a 10s ? You used several types of cells right? How much did it cost you with the BMS?
In fact, I'm sure that your battery is way better than the original one. But, the original one was suffisent for me as I was just riding for fun, for like 20-30min :slight_smile:
```

---
## \#288 Posted by: Chase Posted at: 2020-01-23T06:11:17.240Z Reads: 13

```
Their all 30q cells I was just being fancy by re-wrapping them in alternating colors. Yes it is a 10S
```

---
## \#289 Posted by: Sn4pz Posted at: 2020-01-23T12:20:36.080Z Reads: 12

```
@thisguyhere makes nice quality battery packs! You should hit him up
```

---
