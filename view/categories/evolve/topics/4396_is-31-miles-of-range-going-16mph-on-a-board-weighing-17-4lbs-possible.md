# Is 31 miles of range going ~16mph on a board weighing ~17.4lbs possible?

### Replies: 63 Views: 5007

## \#1 Posted by: Mr_Mahal Posted at: 2016-06-07T16:24:12.051Z Reads: 387

```
It seems most people believe that the GT given it's size and weight will not be able to make it ~30 miles on a charge.  After this picture surfaced:

<img src="/uploads/db1493/original/2X/b/bc48293642315b428bf6afc635bb6fc6adaa2a88.jpeg" width="360" height="480">

One person (@evoheyax)  speculated that the battery might be similar to the Raptor's:
[quote="evoheyax, post:1028, topic:2510"]
It's seems no different internally from the raptor. Same logic, also a 10s lion battery. Still can't find the number of p, by the size, it looks like 3p or 4p, which would make it the same config as the space cell. I don't see how that battery pack gives 31 miles...
[/quote]

Let's assume the picture above is a 10s4p set up. To my understanding, if the Raptors (that get the 10s4p battery) can go ~24.8 miles on a charge (in ideal conditions, going top speed most of the time) why is it not possible for the Evolve GT to get more range if 1) the torque is less powerful 2) the top speed with 83mm wheels is 22mph (vs the Raptor at ~28mph) or 3) the test for max range with the GT was conducted in an eco mode (where the top speed is limited to around 16mph).

The board is less powerful than the raptor and has several different modes that can limit the power used. Maybe some of you can enlighten me on why getting that range would not work. Thanks guys.

**Edit:** **** No one knows what the Wh is for the battery, which is what is causing most of the doubt. *******
```

---
## \#2 Posted by: CSN Posted at: 2016-06-07T16:31:54.906Z Reads: 362

```
How many watt hours is it supposed to be?

I think the max range would hammer the battery pack.

Would be interesting to see a graph of the voltage levels as the pack is discharged.
```

---
## \#3 Posted by: Mr_Mahal Posted at: 2016-06-07T16:32:51.546Z Reads: 360

```
No one knows, it's a big mystery. For some reason they will not release that info.. All they said was it's Li-ion and 42v.
```

---
## \#4 Posted by: Maxid Posted at: 2016-06-07T16:40:55.056Z Reads: 352

```
well if it is in fact a 10S4P battery just like the raptor this could easily be possible with a different 18650 battery used.
You say the Raptor goes 25miles on 2500mAh Samsungs then the GT on LG HG2 3000mAh cells could go 3000/2500*25miles = 30miles. Add this to the more "economical" drivetrain with less top speed and you get your 31miles.
```

---
## \#5 Posted by: Mr_Mahal Posted at: 2016-06-07T16:46:08.868Z Reads: 334

```
I just got the range spec on the space cell pro4 (the battery the raptors will eventually have) from Jason's website. Seems like the GT range should be legit then. I'm sure more people care about how it would do with the 97mm wheels at the top speed of 26mph full throttle though. I will be sure to test and post a thread/video once I get mine in a few weeks...
```

---
## \#6 Posted by: Jinra Posted at: 2016-06-07T16:57:10.063Z Reads: 320

```
A 16A multistar lipo pack is 2P. Since each cell is 8A, if you were to run 10s2p on those cells, you'd end up with 592wh which is enough for the ~50km range they spec out.
```

---
## \#7 Posted by: Maxid Posted at: 2016-06-07T16:59:06.948Z Reads: 305

```
but the size would be totally different - apples and oranges.
I can put a Tesla pack on the board and ride for 100s of miles but the weight and size will not nearly be comparable to a 10S4P 18650 pack ;)
```

---
## \#8 Posted by: Jinra Posted at: 2016-06-07T17:00:31.852Z Reads: 291

```
Lipo's can be molded in various shapes. I'm not saying they're using actual multistar cells. Just providing background to how they can fit the wh inside the GT.
```

---
## \#9 Posted by: Maxid Posted at: 2016-06-07T17:17:32.763Z Reads: 285

```
But evolve apparently also stated that they are using liion. But I get what you are saying - there are a number of ways they can fit more juice than the raptor in there.
```

---
## \#10 Posted by: Jinra Posted at: 2016-06-07T17:21:34.628Z Reads: 273

```
Pretty sure it's lipo. Lipo is Li-ion in a polymer casing.
```

---
## \#11 Posted by: chaka Posted at: 2016-06-07T17:32:32.841Z Reads: 265

```
Those are definitely 18650 cells, it is a 10s5p pack.
```

---
## \#12 Posted by: E-Boarding Posted at: 2016-06-07T17:34:18.210Z Reads: 260

```
how do you know?
```

---
## \#13 Posted by: chaka Posted at: 2016-06-07T17:40:09.694Z Reads: 261

```
When you are around these things long enough you can just tell... plus you can see the profile through the heat shrink.
The only real question is what capacity the cells have.
```

---
## \#14 Posted by: Jinra Posted at: 2016-06-07T17:42:43.877Z Reads: 256

```
Hope that's true, I love me some 18650's
```

---
## \#15 Posted by: evoheyax Posted at: 2016-06-07T17:50:25.782Z Reads: 251

```
How ca they fit 2 times the old space cell into that? The space cell is big as it is.

If it is 10s6p, then the 31 mile range number might actually be true. I wish they would just give more details so it wouldn't be a guessing game, but I also don't really care that much. They still don't have FOC, so :)
```

---
## \#16 Posted by: Jinra Posted at: 2016-06-07T17:51:27.370Z Reads: 256

```
I think I remember hearing 666wh floating around somewhere, which would make sense for a 10s6p setup @3A per cell. I really want to run FOC on my DIY as well, but too scared burning out my drv chip
```

---
## \#17 Posted by: Skitzor Posted at: 2016-06-07T19:02:34.189Z Reads: 248

```
Correct me if I'm wrong guys. But the spacecell 4 pro is indeed 10s4p. I've got a raptor delivered 1,2 months ago and if I'm not mistaking the most of the spacecells before are only 10s3p.
```

---
## \#18 Posted by: Mr_Mahal Posted at: 2016-06-07T19:04:25.784Z Reads: 252

```
Your Raptor came with a space cell pro 4?? I thought he wasn't doing that yet because they wouldn't fit with the current deck..
```

---
## \#19 Posted by: Jinra Posted at: 2016-06-07T19:08:30.402Z Reads: 249

```
yea it's only 3p, 4 is only for the standalone battery for now
```

---
## \#20 Posted by: chaka Posted at: 2016-06-07T20:00:48.556Z Reads: 240

```
Closer inspection tells me this is probably 10s5p. Have any better quality pics? @Mr_Mahal
```

---
## \#21 Posted by: Mr_Mahal Posted at: 2016-06-07T20:15:39.469Z Reads: 229

```
Unfortunately no, this was posted by @Sk8. He might have better pics..have not sen them anywhere else. I will ask one of the riders I know that's in the beta testing group to take another picture.
```

---
## \#22 Posted by: loose_nickers Posted at: 2016-06-08T09:11:33.971Z Reads: 212

```
So I have managed to get this photo. From gt battery
<img src="/uploads/db1493/original/2X/c/c517b6ad1ae7d57c726110d81db79aec7996bdc1.jpg" width="500" height="500">
```

---
## \#23 Posted by: lox897 Posted at: 2016-06-08T09:23:01.849Z Reads: 208

```
What? It is only 360wh nominal voltage?
```

---
## \#24 Posted by: Mr_Mahal Posted at: 2016-06-08T10:52:22.583Z Reads: 212

```
No way that is correct. That is the exact same Carbon Street battery spec. Look here:
<img src="/uploads/db1493/original/2X/f/fe92aa1cd5839ebcc7287358b38e6baa4275c83e.png" width="690" height="409">
Plus, they spec the GT as a 42v battery not 36v. You need a better shot @loose_nickers or that wasn't it at all, where did you get that from?
```

---
## \#25 Posted by: lox897 Posted at: 2016-06-08T10:54:12.605Z Reads: 207

```
@Mr_Mahal It is 36v nominal and 42v fully charged.
```

---
## \#26 Posted by: Skitzor Posted at: 2016-06-08T11:00:26.784Z Reads: 206

```
no, just for the sake of argument. The raptors have 10s3p's in them. The standalone spacecell he sells now is 10s4p like @Jinra mentioned. I get 15 miles / 23-25 km at mostly full throttle in curvy landscape. I'm quite happy with that !
```

---
## \#27 Posted by: Mr_Mahal Posted at: 2016-06-08T11:15:39.765Z Reads: 207

```
Ok, same 10Ah as the previous though.. 

Edit: Can someone explain this lol
```

---
## \#28 Posted by: DeathCookies Posted at: 2016-06-08T12:43:23.264Z Reads: 200

```
Different motors? Reduced power output?
```

---
## \#29 Posted by: Mr_Mahal Posted at: 2016-06-08T12:56:36.288Z Reads: 201

```
I'm just wondering how if their using the same voltage and Ah how they can go from single to dual motors and have even more range and more power..
```

---
## \#30 Posted by: E-Boarding Posted at: 2016-06-08T13:05:56.316Z Reads: 203

```
agree, I don't think this is possible
```

---
## \#31 Posted by: chaka Posted at: 2016-06-08T13:06:00.250Z Reads: 196

```
Marketing...... tis a magical thing. You would need to deplete this pack to a dangerous level to even come close to reaching 31 miles.

I did a little digging and it is very doubtful that you can fit 18650 cells in that enclosure, not enough thickness. They really should have left the hatch on the bottom side so users could upgrade to 18650's later like you can with the older models. I just finished a 10s6p pack for an evolve carbon rider but the battery cover needs to be shimmed a little to make them fit.  Can't do that with the hatch topside.
```

---
## \#32 Posted by: Mr_Mahal Posted at: 2016-06-08T13:23:23.383Z Reads: 191

```
I'm still waiting to confirm that is the actual GT battery and spec. It doesn't make any sense if it is because that would mean every person that's ever tried it would have poor battery life and lied about it lasting.  It would be a shit ton of effort to continuously fake all these tests for no reason in the end. This would be found out very quickly when when first batch gets delivered and they would see returns within a day or 2 if it indeed won't last. @chaka doesn't matter how much marketing they do if it doesn't last when customers get it there will be outrage, returns, and no one (else) will buy it...that simple..hopefully this is not what will happen
```

---
## \#33 Posted by: chaka Posted at: 2016-06-08T13:41:37.841Z Reads: 185

```
You over estimate the percentage of people who take their outrage to the internet.  Crappy range hasn't hurt them in the past but seeing older boards with upgraded packs will certainly provide a little angst for the gt owners when they find out they can't do the same.

They really did a number on you guys with their marketing, I mean people were scrambling to pay over $2k for essentially an evolve carbon with outrunner motors and a new ESC. Marketing is like crack for consumers.
```

---
## \#34 Posted by: Mr_Mahal Posted at: 2016-06-08T14:00:42.261Z Reads: 180

```
Let me speak for myself, I will make it my mission to tell everyone how shitty it is if it gets worse range than I would expect. I don't expect to get 30 miles on a charge because I have hills and ride fast and do a lot of start and stop. But 23-25 miles should still be possible...I will be testing the range a variety of different ways, mainly on a track and then doing my reg commute. 

Considering the number people I know that are active on the forums, here, reddit, YouTube etc that are getting it and will be testing I doubt word/video/pic evidence will not spread fast. Sure, some people will not listen or care, that'll be on them though. There are quite a few that are waiting for me to test it that will listen and that's enough for me..after that I'll just return and move on, no big deal. People may have scrembled to pay 2k only to be disappointed in the end but at least they can get (most of) their money back.
```

---
## \#35 Posted by: Mr_Mahal Posted at: 2016-06-08T14:32:34.800Z Reads: 180

```
Isn't the space cell pro 4 360 Wh? Remembering this response earlier in the thread:

"well if it is in fact a 10S4P battery just like the raptor this could easily be possible with a different 18650 battery used.
You say the Raptor goes 25miles on 2500mAh Samsungs then the GT on LG HG2 3000mAh cells could go 3000/2500*25miles = 30miles. Add this to the more "economical" drivetrain with less top speed and you get your 31miles."

But if you guys are saying the enclosure wouldn't be able to fit the specific type of batteries needed to get the range idk..
```

---
## \#36 Posted by: Tarzan Posted at: 2016-06-08T14:34:07.532Z Reads: 176

```
The Raptor is using LG's too.
At least the three space cells I have opened up!

Some day we will know.
```

---
## \#37 Posted by: Maxid Posted at: 2016-06-08T14:42:24.735Z Reads: 180

```
[quote="Tarzan, post:36, topic:4396, full:true"]
The Raptor is using LG's too.
[/quote]

Yeah but only HE2 or HE4 - which both are similar to the Samsung 25R and have 2500mAh.
The HG2 have 3000mAh - that is a 20% increase in capacity at the same size.
```

---
## \#38 Posted by: Tarzan Posted at: 2016-06-08T14:45:07.957Z Reads: 177

```
You are right sir!
```

---
## \#39 Posted by: chaka Posted at: 2016-06-08T14:48:28.586Z Reads: 180

```
The problem with that plan is the fact that under perfect conditions, average speed and rider weight you will be able to get 30 miles of range and your ranting will be discredited.

Take my boards for instance. I only get about 20-25 miles on a charge but I weigh around 185-200 lbs and I spend most of my time above 30mph or burning up watts getting there. Of the few beta testers out there all of them are reporting well over 30 miles on a charge, some as high as 45 miles. This is why manufactures should disclose capacity rather than range. Similar to fuel tank specs on an automobile.
```

---
## \#40 Posted by: longhairedboy Posted at: 2016-06-08T14:53:18.937Z Reads: 179

```
it doesn't matter what cells you're using if the total pack is 36 volts at 10Ah then you have a 360 watt hour battery. 

Is 30 miles possible on a 360 watt hour pack is the question here. Probably if you're riding at 8 mph the entire time on flats and slight declines. 

my 10S4P 36v 10Ah (360 watt hour) packs get about 20 miles out of a charge while averaging 18mph on slightly mixed elevation, read: normal bike path terrain.

Also, the weight of the board is practically, while not totally, irrelevant. ITs marketing bullet points and the only reason it matters is because you have to carry it. Rider weight varies much more than the difference between a 15 pound esk8 and a 20 pound esk8. I'm 150 pounds and i get the range i do on 17-20 pound boards. A guy weighing 180 isn't going to get that range even if he's on a kevlar/carbon fiber space base composite deck, so advertised ranges have little do do with board weight and are pretty much unreliable, which is why i tell people how much i weigh when i post stats most of the time.
```

---
## \#41 Posted by: longhairedboy Posted at: 2016-06-08T14:54:51.275Z Reads: 170

```
you run some seriously ridiculous watt hours in your boards too lol
```

---
## \#42 Posted by: HoboFarts Posted at: 2016-06-08T15:11:47.451Z Reads: 167

```
So... what I'm hearing is...

Lose weight = More E-Board Range.

All of our problems have been solved :D
```

---
## \#43 Posted by: E-Boarding Posted at: 2016-06-08T15:33:44.369Z Reads: 167

```
Carbon charging time 4-5h (fast charger 2,5h)
Carbon GT charging time 4-5h (fast charger 3h)

same battery size or not?
```

---
## \#44 Posted by: longhairedboy Posted at: 2016-06-08T19:10:18.349Z Reads: 167

```
pretty much lol

I've lost about 35 pounds since i started esk8ing a few years ago. getting more range and speed out of your boards is a good reward for losing that gut. I had some serious gut too, i don't have the frame for 185. My frame is thin and looks much better at 150. Basically i looked like a sack of flour on a fence post.
```

---
## \#45 Posted by: Mr_Mahal Posted at: 2016-06-08T21:50:32.958Z Reads: 170

```
@chaka 
[quote="chaka, post:39, topic:4396"]
The problem with that plan is the fact that under perfect conditions, average speed and rider weight you will be able to get 30 miles of range and your ranting will be discredited.
[/quote]

I weigh 155lbs, so l should be getting the good end of the range for most eboards.. Do you know the exact mph average I'd need to travel at to achieve 30 miles with this pack weighing that much on flats/low wind/warm day? What I'd hope is to be able to reach 30 at least in those conditons averaging around 15mph or so. If I were to get only 20 miles going that speed (Eco) THAT would trigger a rant. Weighing well around the lowest most riders are, I think my testing will show the better end of the range -- so if it's shit for me, it'll be shit for everyone lol. I have a variety of "ideal" conditions to test it in..

@longhairedboy 
[quote="longhairedboy, post:40, topic:4396"]
Is 30 miles possible on a 360 watt hour pack is the question here. Probably if you're riding at 8 mph the entire time on flats and slight declines.
[/quote]

I'm curious as to why a guy got ~40 miles averaging 12mph then: http://prntscr.com/be1pn0    http://prntscr.com/be1q1s Unless it's not legit...

[quote="longhairedboy, post:40, topic:4396"]
my 10S4P 36v 10Ah (360 watt hour) packs get about 20 miles out of a charge while averaging 18mph on slightly mixed elevation, read: normal bike path terrain.
[/quote]

I think because evolve limits the power through preset modes maybe it's just more efficient than having everything available at once (even if you don't use it, the GT's ESC is limiting the board vs. your thumb)? Have you tried testing the same motors evolve uses before? Idk, after seeing that screen shot above a long time ago I figured the range is pretty legit if that test was indeed real. I just wish someone would post a long clip of these tests...

[quote="longhairedboy, post:40, topic:4396"]
Also, the weight of the board is practically, while not totally, irrelevant. ITs marketing bullet points and the only reason it matters is because you have to carry it.
[/quote]
I put that in the title mainly because I didn't know the Wh or anything so I figured if you knew the weight you could kinda guess what size pack it is or w.e..


Guys; Idk what they have done with this board really, not sure how it all works out but I have so far not seen a single beta tester or person that a beta tester has let ride the board report getting range that is out of line with the advertised specs. Maybe this just a grand scheme and they just got a bunch of beta testers and fake people to test their board and paid them to lie about it. Or they're all just light as fuck :grin: Time will tell and I'll be sure to update you guys with my results once it arrives within the next 3 weeks. Thanks for all the info you two I do appreciate it.
```

---
## \#46 Posted by: longhairedboy Posted at: 2016-06-09T13:27:32.878Z Reads: 146

```
you're probably right about some kind of electronic magic. They could be throttling the acceleration curve to a more efficient shape. They could be dynamically limiting current in such a way as to keep fidgety thumbs from affecting draw while cruising. They only have one motor and once ESC to deal with, so the tuning possibilities are endless with those kinds of resources. 

There's really no end to what's possible when you're well funded and engineers on staff.
```

---
## \#47 Posted by: chaka Posted at: 2016-06-09T13:36:49.042Z Reads: 147

```
Part of me thinks they used the VESC to develop the ESC in this board. I'll have to peek inside and check the pcb for "trace" evidence. I know a lot of other companies are using it as a dev board.
```

---
## \#48 Posted by: longhairedboy Posted at: 2016-06-09T13:42:30.342Z Reads: 151

```
i just know you're right about this. It wouldn't make any business sense to NOT do it. Its open source and well documented, its basically low hanging fruit. 

so you create a board with traces for VESC and BMS and maybe a couple of feature adds for lights and other dumb shit and you're done with the hardest part.
```

---
## \#49 Posted by: chaka Posted at: 2016-06-09T13:46:16.413Z Reads: 148

```
That is actually the easiest part. When you get Ubuntu running on a decent computer try your hand at KiCad. Very intuitive to use and there are some very informative videos to help get you started on youtube.
```

---
## \#50 Posted by: longhairedboy Posted at: 2016-06-09T14:17:40.367Z Reads: 149

```
LOL funny how for me that's the hard part. I guess i'm the type who would rather be covered in dust than on a cad station. 

This is something i need to do though. I suck ad CAD of all flavors and i need all kinds of designs to come out of my head and into a computer, so i guess i need to learn.
```

---
## \#51 Posted by: jack_pate Posted at: 2016-06-10T00:03:44.002Z Reads: 139

```
How far could I go with a 12s2p, 44v, 5AH and I weigh 120 pounds. mono drive.
```

---
## \#52 Posted by: CSN Posted at: 2016-06-10T00:34:20.748Z Reads: 140

```
With 220 wh I would guess  12 miles but  not be a great idea to run it that low very often.

Maybe 8-10 miles to be nice to the pack.
```

---
## \#53 Posted by: longhairedboy Posted at: 2016-06-10T11:35:18.137Z Reads: 134

```
@csn is right. That's basically the watt hour equivalent of a 10amp hour 6S and i know from experience you'll only get about 10 miles out of those while approaching any sort of fun speed on occasion.
```

---
## \#54 Posted by: Mr_Mahal Posted at: 2016-06-10T23:07:59.165Z Reads: 133

```
@longhairedboy @chaka

FYI, Jeff confirmed on a live stream yesterday that the GT battery is indeed 10 Ah, and is lithium-ion -- no longer LiPo. He stressed that they have made it "extremely efficient" with the new "custom" bms, also mentioning the fact that their previous motors were bigger and the smaller size with the new ones help. Aussies are getting their boards now, my board should hopefully be here in about 2 weeks, I will post another thread once I've done some testing.
```

---
## \#55 Posted by: Jinra Posted at: 2016-06-10T23:59:24.870Z Reads: 131

```
i thought he was hush hush about the AH
```

---
## \#56 Posted by: Mr_Mahal Posted at: 2016-06-11T00:28:10.854Z Reads: 128

```
He was but I guess he just decided to say it. It's no secret though because it was kind of figured out by the fact that the GT uses the same charger and has pretty similar charge times to previous model speced on their site
```

---
## \#57 Posted by: Jinra Posted at: 2016-06-11T00:40:11.150Z Reads: 128

```
Hm so if 360wh can make it 40 miles with these new motors, I wonder how far I'll get with @chaka's motors
```

---
## \#58 Posted by: Mr_Mahal Posted at: 2016-06-11T00:57:28.306Z Reads: 135

```
Well, would need a bms/esc with some preprogrammed modes to limit the amount of current draw going by what Jeff said.. Seems like the diy world is still lacking remotes that have modes on them unless I'm mistaken
```

---
## \#59 Posted by: Jinra Posted at: 2016-06-11T00:59:04.111Z Reads: 136

```
The VESC can limit amp draw, but doesnt support multi-mode operation to my knowledge. My remote does have a two mode option which basically limits throttle to 50%
```

---
## \#60 Posted by: Mr_Mahal Posted at: 2016-06-11T01:21:15.382Z Reads: 144

```
Seems to be what makes the evolve special. Similar to boosted too, it's a combo of throttle limits and top speed limits that makes them go so long depending on the mode. Though I think maintaining speed on any board will take you farther than you can go on an average city commute
```

---
## \#61 Posted by: E-Boarding Posted at: 2016-06-11T06:46:40.268Z Reads: 149

```
Which live stream the first or second day?

What about the sensored motors, do the sensors make them more efficient and provide longer range?
```

---
## \#62 Posted by: damonic56 Posted at: 2016-11-04T16:53:01.952Z Reads: 91

```
<img src="/uploads/db1493/original/3X/0/e/0e088268f2d9f81095b3011f4c5a75fa3b28ec69.JPG" width="690" height="388">

Hi,  does anyone know if it's possible to order this from evolve? Please help.
```

---
## \#63 Posted by: Fiori Posted at: 2016-11-25T20:37:09.365Z Reads: 76

```
Not to dig up an old thread or anything, but I couldn't find this info listed anywhere else around here. 

Incase anyone was wondering: It's a 36v 10AH 360wh battery.

http://evolveskateboards.de/index.php/shop-buy-online/evolve-elektro-skateboards/evolve-gt-carbon-street-detail
```

---
