# Ninestep/Diyeboard/L-FASTER 8&rdquo; mountainboard/trucks/electronics review

### Replies: 29 Views: 5825

## \#1 Posted by: telnoi Posted at: 2018-02-20T14:51:16.056Z Reads: 386

```
_**Disclaimer**: Before continuing to read this review, I want to point out that the board has not been purchased from diyeboard. Upon asking for the difference between their A grade components and the identically looking equipment I bought, I received no conclusive evidence that leads me to believe that there is a difference in quality._ 
![mountainboard|690x460](upload://9m4cJLYSoVe69lNKEC75lcMKkUf.jpg)

**Background info**

Snowboarding is/or rather was one of my biggest passions. I started riding 20 years ago. However, due to the increasing prices of Wintersport vacations and the necessity to support my wife in a foreign country, I had to give most of it up about 7 years ago. The added frustration of deteriorating snow conditions most certainly did not help and I was rarely able to capture the same feeling I had when bombing down mountains off-piste all those years back.

I looked at regular mountain boarding, kiteboarding & kitesurfing, but these sports were too restrictive, especially in Germany. Hardly any decent slopes nor big lakes around.

Enter esk8. The prices were steadily dropping and several resellers were offering a Chinese made electric mountain board, sold under different brand names. They all appear to be identical, with the exception of a few specs (motors, deck/bamboo mix).

**The specs as indicated by the reseller:**
* 11AH LG Li-Ion
* 20-30 KM range
* 42 km/h top speed
* 2000W (total)
* climbs of 30º possible
* bamboo/maple deck
* 8'' wheels

It comes with a 2A charger (roughly took 5+ hours to charge after a ride). 

**The specs that you will find are more important**
If you are new to ESK8, the above mentioned specs sound impressive...and they are, if you stick to flat roads and a bit of offroading with some minor climbs. However, the manufacturer/distributor/reseller will often omit the specifications that have a big influence on performance. Cheecky. 

* The chinese 2.1 ESC delivers 25A per motor (50A total)
* The battery pack delivers just that, 50A

These are performance limiting factors that will turn the mountain board into something that is great for streets with potholes, but rather mediocre to terrible for serious offroading. If you expected anything more, you basically bought a lemon. And as it will turn out, it is somewhat complicated to turn that lemon into lemonade. 

**Malfunction**
I didn't get to enjoy the board for long. After 700 meters, the ESC malfunctioned. However, since I already established that the board was not going to perform according to my wishes, I decided to try and turn that lemon into lemonade.

https://www.youtube.com/watch?v=T-wt-2217xE
 
**First upgrade - motors & VESC**
After doing some research, I learned that the ideal motor size for my weight and intended purpose was 6374 or even bigger. The stock motors were 6355 (Maytech - sold under different brand names). Since I was going to upgrade to VESC, I also had to ensure that I was not working with a high KV motor (VESC RPM limit) and 190KV or lower was recommended for high torque offroad builds. I chucked the stock motors and bought some SK3 149KV motors. Along with the motors, the pulleys have to be exchanged due to the inner bore diameter difference (10 vs 8 mm motor shaft).

The stock motor mounts could be redrilled to fit the new motors, but they suffered from belt slipping, which would most certainly become worse with additional power. It has no belt tensioning options, thus I chucked those too and 3D printed some alternatives after which I had the final design CNC'd out of aluminum. 

_Original design - no belt tensioning_
![mountain-board|690x434](upload://vLCXtSzo0QULUIm0TKmgh81qcXA.jpg)

_Simple but effective clamped redesign_
_Belt tension can be adjusted by moving motor_
![custom-motor mount|666x500](upload://8eBxwuEjJosxXL1WnrMsAZyXiHo.jpg)
![custom-motor mount_2|690x388](upload://ycFdGCfn0sKbSsJMRwGewxTFTvb.jpg)

I then bought an ultrabox 206 and placed all my electronics inside of it (first ESK8.de VESC and then dual focbox). Yes, that's allot of dirt. It's being used as it should ;)

![current|666x500](upload://ggc3Y8OvA0ExixDus0WqLZLwsxr.jpg)

**Stock 10S5P Li-Ion pack - weak sauce**
I had some hope that I could still use the Li-Ion pack. I was very wrong. I had to walk the majority of the offroad track I drive to work, because the pack could not deal with the increased amp draw...at all. The VESC was set to pull 25A each, but even that was too much with a voltage sag of over 2V at times. In addition, the board would slow down significantly around 39 V due to the extreme voltage sag, so I could not get much range out of it in a hilly area. The last of the stock electronics had to go.

I bought 4x zippy 8000mah 30C lipos and a charger capable of delivering 14A at 24V, meaning I can usually get going again within 2 hours. That, plus no more walking. The VESC is currently set at 50A battery amps (100A total), providing enough power to conquer the hills around here. 

I read all about BMS integrated systems and how they tend to cause issues (braking, over-voltage), so I decided to go with a simple & cheap, but effective approach.
* A couple of parallel & series adapters
* ISDT Q6 plus charger
* Balance board
* 24V power supply
* Cheap voltage alarms - they do their job fine letting me know when I am at 36V under load

![lipo_wiring|666x500](upload://xHFwJlERwv83w8OgbRPeYLAbzZl.jpg)

The lipos are thrown in a padded backpack and fastened to my board. The charger is in my regular backpack. After around 900 KM (longest trip, 24 km) I can safely say that it works fine. 

**Recap**
At this point, I replaced the stock ESC, motor mounts, motors, electronics enclosure & Li-Ion pack.


**still not done - stock trucks/wheels**
Whilst working on the board and actually using it, it became obvious where manufacturing corners were cut on moving parts. The trucks are unstable due to a variety of reasons and you will easily encounter speed wobbles beyond 30 km/h offroad or with unpredictable wind. 

The reason for this is that:
**A.** These trucks are not precision engineered (no cnc)
**B.** These trucks do not have dampeners

The bushings and kingpin all have several mm of free play. The bushings are actually too small for the trucks (or the holes too large) and just by looking at the picture below you will see what the remaining issues are. Nothing fits. Aligning bolts and bushings is difficult if a truck is not precision engineered, so instead they decided to create oversized holes for pretty much everything. In addition to causing speed wobbles, it creates a hell of a noise.

The next step is to see if new bushings will resolve the issue. Last resort is drilling oversized holes and machining custom bushings to resolve the play. If that does not work, it will be time to invest in a more expensive board as my platform (MBS or Trampa).

![trucks-axis|375x500](upload://y5Gbm22gM1eiuq9WXtIr2jLjCk2.jpg)

In an additional attempt at trying to improve the riding characteristics, I tried to install dampers made for MBS trucks. Sadly, they are too compressed when installed, thus that is not a solution.

_compressed dampers - also notice the pressed in bearings for those hubs. Maintenance will be a b_&tch.
![trucks|666x500](upload://fmyE9NTcEBGID68QTrSjx8QAlce.jpg)

Lastly, the hubs (wheels) are out of balance. Even when removing the 8'' pneumatic tires, I noticed that the hubs wobble adding to the instability and vibration of this board. 

**What I ended up with**

So what I ended up with in the end was a board that did not fulfill my personal expectations, but hey...you get what you pay for. Upgrading the board did force me to learn allot about basic manufacturing (developing a motor mount) and the electronics involved. Since you won't find expertly designed parts for these boards, you have to do it all yourself.

It also became painfully obvious that I could have bought a Trampa or similar brand at roughly the same price. It would have been a better option in the end. Still, I am having a blast with my board and with the list of improvements I made, it has turned out to be reliable enough for day-to-day commuting.

https://www.youtube.com/watch?v=84nQwxUMiGI
```

---
## \#2 Posted by: Mattmccrary8 Posted at: 2018-02-20T15:16:35.712Z Reads: 300

```
Great review and I was going to get one since they were so cheap but you get what you pay for like anything in life. Kind of dissapointed but mine as well make a Trampa board now.
```

---
## \#3 Posted by: telnoi Posted at: 2018-02-20T15:24:14.980Z Reads: 290

```
Yup, I was naive in thinking that 700 euro was a big enough investment. Double that amount and you'll scratch the bottom of what could be considered acceptable by many :rofl:
```

---
## \#4 Posted by: Okami Posted at: 2018-02-22T07:41:25.126Z Reads: 264

```
Hi, did u cut deck shape also? 

Will probably have more questions but wanted to find whenever u cut it yourself
```

---
## \#5 Posted by: telnoi Posted at: 2018-02-22T07:45:08.373Z Reads: 251

```
No, the deck was not altered. It does not have a concave and is flexy for my weight (92 kg).
If I were to choose a different deck, I would opt for something a bit stiffer with a concave for better grip and control.

It does offer allot of room for motor mounts/drive train. All in all, the deck itself is ok. Would not go jumping with it. As mentioned in my review, there are a few variations of this deck, some with cheaper PLY variations.
```

---
## \#6 Posted by: Okami Posted at: 2018-02-22T08:05:25.431Z Reads: 223

```
Thanks for quick answer. Yeh i had seen the circular decks which i think look ugly, the same one as in first picture u posted.

I know someone is selling similar boards under voltair name (or similar), these also have similar shape as yours.

Nice that u have the good looking shape.

On a side note - how did u find out escs are rated for 25A and battery also rated for that (2x 25A)? They usually dont mention esc / battery specs power wise, only motor power i think
```

---
## \#7 Posted by: telnoi Posted at: 2018-02-22T08:07:49.722Z Reads: 191

```
Diyeboard (aka Jason here) disclosed that in their dedicated thread.
The battery is a 5P consisting of LG cells that deliver 10A max, thus 50A total. 

The type of cell used was also disclosed by diyeboard and verified after I pulled out the Li-Ion pack. A 10S5P with better cells (individual cells are rated at 20A-30A) is around 500/600 EUR alone.
```

---
## \#8 Posted by: Okami Posted at: 2018-02-22T08:19:07.250Z Reads: 188

```
Thanks for info. I might reconsider getting original battery then. Ive got a similar board now but i got it without battery, might as well rebuild vtc 4 pack i have. Will have more power at least.

Well hard to tell what else to add. I suppose i can say all is good that ends well (your journey upgrading it), just too bad that wheels and trucks are still not perfect in your case.  As u said, might as well build decent board from groundup

Anyways thanks for extra info. Do u have any info on what type of bms was inside of original battery? That is the only question i have now - how will i charge the  battery, if i make it on my own
```

---
## \#9 Posted by: telnoi Posted at: 2018-02-22T08:29:15.354Z Reads: 186

```
I sold the pack, thus I did not pull it apart to see what kind of BMS was in there. Diyeboard was asked in their thread, but an answer has never been given.

If there is one thing I learned, it is that these kits are constructed in such a way as to´precisely deliver the performance of the weakest part, thus saving on the total cost.
* The Li-Ion delivers 50A (limiting factor/weakest part)
* The ESC is programmed to use 50A max (can't be changed by user)
* The BMS is wired to charge & discharge. It will most certainly not have discharge specs surpassing 50A

The type of BMS you need depends on if you want to discharge via BMS or only charge, plus how fast you want to charge your packs. The integrated BMS must have had a charge rate of around 2A. I would most certainly not attempt to charge it at a higher rate.
```

---
## \#10 Posted by: Okami Posted at: 2018-02-22T08:59:42.204Z Reads: 180

```
Mh yes looks like all system is designed that way.

Well i will either split 10s pack in 2 parts, one 6s, one 4s (charging with hobby charger). 

Or go for all in one solution with bms.

Just curious will i find suitable aftermarket bms.

How do u like the thin tires? They look tiny when i compare them to my primo strikers, 9inch, which ones i have on previous board
```

---
## \#11 Posted by: telnoi Posted at: 2018-02-22T09:14:00.509Z Reads: 185

```
Finding a BMS should not be an issue, but from memory there is a difference between Li-Ion and LiPo BMS due to the min voltage until cell degradation (over discharge protection). Just make sure that it can be configured or is suitable for your type of cell. Bestech is recommended. Some use SuPower too.

The tires are fine for my purposes. I could imagine that traction could be better without the thin stripe in the middle, but the size is fine (most here run 8'', including those using Trampa boards). I ride very rough terrain and am currently plowing through mud and sometimes a bit of snow without too many issues.

Older version of motor mount, but that's typical of the riding conditions over here. Usually more holes and mixed with some larger stones.
![dirt|666x500](upload://2V9mdLfIBX86C3e2D4f4jpXWu6S.jpg)
```

---
## \#12 Posted by: Okami Posted at: 2018-02-22T11:32:37.806Z Reads: 167

```
Nice picture. Looks like rough terrain is not an obstacle for you. 

Concerning road type / terrain, i hate to ride on rocky roads. Looks like no problem for you or maybe they are different texture than what i have witnessed
```

---
## \#13 Posted by: telnoi Posted at: 2018-02-25T12:34:55.601Z Reads: 168

```
Small update. 
A video highlighting the play of the trucks. Notice the sound it makes just moving it around with my hand. It clunks along nicely off-road. 

Only advantage. People hear me coming from miles away. 
https://youtu.be/A4Kj_wzvlKk

The tires and bearings are now done after 1300km in total (one tire is even warped slightly) . I guess not bad? Not sure how that compares to trampa.
![IMG_20180225_123113|375x500](upload://69E7RqFqHeGc68YZUQgpbjFAbPa.jpg)
```

---
## \#14 Posted by: Okami Posted at: 2018-02-25T13:17:12.496Z Reads: 157

```
Thanks for feedback. 'Interesting results. The 'wobble' on tire does look bad. Looks like cords / threads inside have weakened / broken
```

---
## \#15 Posted by: telnoi Posted at: 2018-02-26T14:31:19.604Z Reads: 156

```
Parting with the board in favor of 
![574-black_600x600|600x315](upload://bwh65VBwOTZNbUroshjwbS2vSTk.jpg)
Putting more money/time into the old board makes little sense at this point.

New pair of wheels is around 60 euro. New & better bearings around 20. New hubs around 70 euro. That's money better spent on a new board.

If I replace the hubs, I have to shorten the axis and create new threads + I would have to buy new pulleys.

Will be interesting to see the difference in riding experience.
```

---
## \#16 Posted by: Okami Posted at: 2018-02-27T19:54:51.154Z Reads: 145

```
Sounds wise. It did cost you a lot more in the end to rebuild the board..
```

---
## \#17 Posted by: J95hicks Posted at: 2018-05-28T13:11:26.684Z Reads: 128

```
Hi, relatively new member here. Bought same thing from diyeboard, minus the deck. I tried finding in the DIYEboard thread where they said 25A per motor.. their is alot of junk in that thread. Just wanted to confirm thats what you were told bc i received an email claiming "It is 50A continuous per motor" a few days ago. ![Screenshot_20180528-073615|281x500](upload://yg54fGLNSjhrU8VvXdO9ItL3t3E.jpg)Thx, sorry if im not posting correctly or whatever correctly lol
```

---
## \#18 Posted by: telnoi Posted at: 2018-05-28T14:08:17.428Z Reads: 120

```
Their ESC doesn't do more than 25A per motor, because they pair it with a Li-Ion that is capable of delivering a total max of 50A. They don't use a BMS for discharging, thus the ESC has been programmed to be within the safe levels so that the amp draw never exceeds 50A.


In other words, the ESC might be able to do more than 25A per motor, but it has been programmed to work with the kits they sell. That said, even at 25A the ESC heats up significantly to the point of failure (few reports of burned wiring). The performance of a focbox which truly delivers 50A per motor is on a whole different level, so I most certainly know the difference between 25 and 50A per motor.
```

---
## \#19 Posted by: J95hicks Posted at: 2018-05-28T14:33:44.665Z Reads: 121

```
Wow, okay. Thanks a ton man. Im a big guy(260lb, 6'5") and i was unimpressed with the power/torque/etc of the  Mountainboard type setup FOR my size. Would prob be okay for smaller folk or reg skateboard. But not mountainboard setups... thx for your input.
```

---
## \#20 Posted by: telnoi Posted at: 2018-05-28T14:43:56.343Z Reads: 127

```
I'm around the same weight actually at 1.90m tall.
The trucks were highly unstable for me around the 30 km/h mark off-road , though I got it up to 50 a few times on pavement (with focboxes, lipos and SK3 motors). Switching to trampa stuff has opened my eyes to how good and stable an off-road build can be... But yah, it's expensive.
```

---
## \#21 Posted by: J95hicks Posted at: 2018-05-28T15:20:36.496Z Reads: 123

```
Thats sad to hear lol. Especially after what all ive bought. My terrain is mostly crappy pavement and light grass in Texas so i might be okay for awhile with those trucks. I just bought the 6374 sk3 149kv motor, now i have to budget whats next.. focbox and a decent battery prob. But that alone is like what i paid for everything else lol. I really do like the 3 speed of the remote though, being able to ride casually or aggresive. I know their are 2 speed remotes but im also nervous of Canbus after peoples reports of frying..so i was thinking of just going the mini route and using 2 recievers and sacrifice the speed "levels".. apologies for over commenting just not to many people can compare this product to other things im interested in. And i couldnt justify getting top end stuff before but now im hooked lol
```

---
## \#22 Posted by: epss4 Posted at: 2018-12-19T19:32:18.437Z Reads: 77

```
when you receive the board , when its was all stock part, does the spec of the seller were right ?like 20 km range and 40km/h speed?? 
Thanks :) !
```

---
## \#23 Posted by: epss4 Posted at: 2018-12-19T19:33:57.061Z Reads: 79

```
what speed and range did you get from dthis board ?
```

---
## \#24 Posted by: topcloud Posted at: 2018-12-19T20:41:19.008Z Reads: 79

```
great review, bud.  5/5
```

---
## \#25 Posted by: telnoi Posted at: 2018-12-19T22:57:23.654Z Reads: 74

```
The original speed controller broke down after a few 100 Meters, so I never got to test the range with original specs. The battery lasted maybe 16 km after the initial vesc and motor upgrades, mainly due to the voltage sag.

There are far better choices available now, including completes.
```

---
## \#26 Posted by: Nomorechasingwind Posted at: 2019-04-27T08:44:37.630Z Reads: 48

```
So hello I am new here! I live in BC Canada. I am a kiteboarder and RC Guy. Well I used to be it seems anyways......

I signed up just to post on this old thread, as this thread is all that really shows up on a search to reveiw these kits or boards. After much consideration (rye and ginger and one night on this forum) I bought the L faster kit on amazon.ca. (look it up if you care.) Why did I buy it? Because kite sessions are few these days with work and all. Also because I live in Canada and getting parts here is crazy expensive. Dropping 3 grand on a skateboard seemed a bit much (and cuts into my alcohol fund). 

Now I do ok with work. I could afford a trampa or even pay a machinist to make parts for me. I could even purchase a 3d printer and make parts for myself! But explaining why I spent that much or why this 3D printer was in the living room making a stink for months to my wife would be extremely painful. More painful than this guys gripe with his board TBH. Super Painful..... So I rolled the dice on a Chinese kit.  .....After all most everything is made in china anyways..... right? You just need to be handy and realize that you are the customer service and RandD. Not much support buds!  I expect nothing but a deal and a platform to build off of when I buy RC. I guess my background in fabricating and the RC hobby helped. But in all honesty I did not really need to fall back on it much....(but I guess there was that getting this thing together part come to think of it)......

More to the point of my post. I decided to post here to let others know that the Lfaster kit (referred to in this thread but not actually the OP's product in question ) is actually working out great!  It seems to have enough power to move my fat 200pound ass around at 42k on pavement (confirmed by tracking App). It even does trails and offroading very well too. I will add not perfectly. But that said I remember having to jump a bit on my mbs alex brown pro6 board with my kite to get moving in a bog. If I didn't I would get supermaned as my board stayed put.... But I could go on for hours about how and why. So to the meat .........and no potatoes........ Its Keto mania after all these days!

The $600 Cnd L faster kit comes as advertised not perfect.(Coughs) like most build threads on here..😉
  
So what I did to fix that......

1. Take it all apart and loctite, grease and tighten everything!

2. Add O rings to the spring seats and yellow mbs eggshocks to the trucks. (Orange is too stiff IMHO I like to carve)

3.Beef up all the hardware with bigger and better marine grade stuff where I could. 

4. Add a heat sink to the PCB board. Seems to help 

5. Glue the riser pad to the trucks with super 77. stops it from relying on just compression to hold it there. Less potential unwanted movement.

6. remove them dumbass motor covers and add a custom made brace that all these builds seem to have....

7. Drilled holes in deck to allow for longer dog point grubscrews from better truck spring adjustment. 

Some of these mods I had to do on my MBS boards in the past already. Like that slop found in the kingpin as described by the OP...... yep MBS Too.....

Now I built my own batteries from some recycled bus lipos from ebay. At first I thought it was a mistake (drunk Ebaying). So I bought some HRB 5000mah to try out (more drunk ebaying). They seem to heat up more than my homemade job 8000mah bus batteries. So them bus batteries are better. Even though they are huge.....

I stuck the works on my MBS jeep renegade board from 2005? (Bought so many dead brain cells ago).. I put a 120 Amp fuse inline to the electronics. The electronics are in a water sealed case. And batteries ride inbetween my feet in a bag. Standard esk8 stuff. 

The "all in one" electronics inclued in my kit... (reciever and 2 speed controllers in one) is something my RC hobby experience told me to stay clear from. But the price was right. So I went with it. I am happy to report the unit has functioned as it should. I believe the specs of this L faster speed controller are better than stated in the OP's reveiw. Closer to the advertised specs he stated. I have had no issues with the remote or connection to the board. But I mostly ride on closed golfcoarses and trails (no real interference out there)

Now all said and done I like to think I am into this for $1300 CND. (Why did I do that.....I bought my first steet bike for that!) I waited a month for parts in the mail. It took 2 weekends to put the thing together. So for that cake and time I got a 42kph board with 21000mah of 10s batteries and a dual bank AC/DC  hobby charger. Not bad. Really. Best part is I am out riding and smiling... and still married! 

I just want to add in closing that the original reveiw was a big help in working out the gremlins of these chinese kits. And the forum was also a big help in this endeavor.

 Thanks to all for the help and sorry about them potatoes!
```

---
## \#27 Posted by: telnoi Posted at: 2019-04-27T10:59:45.637Z Reads: 46

```
Enjoy the board. After all the mods, it was OKish. Still, nothing compared to my Trampa mainly due to deck stiffness, overal lack of stability and the awful motor controller (these have been abandoned by most if not all Chinese boards by now). 

One tip, don't ride in the rain or lube the hell out of those bearings, otherwise they will cease up in no time and it's no fun replacing them.
```

---
## \#28 Posted by: OBone Posted at: 2019-11-22T02:57:44.448Z Reads: 25

```
Hi all.
Flipsky now also have an AT truck kit with 11in AT trucks, 8in wheels. Comes with 6354 motors. I suppose these fall in the same category as the others in this thread? 
Anyone have experience with these?
```

---
## \#29 Posted by: jeorghe Posted at: 2019-11-23T19:15:40.923Z Reads: 20

```
Yes , It Is the same, but the motor mount has been improved.
```

---
