# Board slowly loses power up hill?

### Replies: 52 Views: 5244

## \#1 Posted by: michaelcpg Posted at: 2016-07-21T11:58:21.100Z Reads: 303

```
My boards been out of action for the last couple weeks while I was waiting on some extra batteries to arrive and get my repaired VESC back from @chaka. I've had the board back together for a day now and for the most part it's been running perfectly. 

However when I went to ride up a fairly long and steep hill tonight I got about half way up and I slowly began to lose power until it got to the point where the board was barely moving. I got off for a couple seconds then got back on and started riding again and it seemed to have full power back but about another 10 - 20m up the hill and the same thing started happening. This basically happened another 3 or 4 times till I got to the top of the hill.

I've ridden up this hill many times in the past without any issues and the battery was still at 65% at the top of the hill so it shouldn't have anything to do with low voltage cutoff kicking in. Since the board was running last (when I didn't have any issues with this hill) I've upgraded the battery from a 10s3p to 10s4p pack, replaced my enertion remote with a GT2B and had my VESC repaired. While @chaka had my VESC he flashed it with 2.18 firmware (from the original 2.16) and it's now running in BLDC mode (was running in FOC before the repair). Other than that, I'm using the same firmware settings as before.

Board specs:
10s4p space cell
Single Enertion 6374 motor
Ollin VESC
GT2B Remote

Any ideas?
Cheers
```

---
## \#2 Posted by: chaka Posted at: 2016-07-21T12:52:25.045Z Reads: 283

```
Did you run through motor detection again and configure your setting? Sounds like you are overheating.
```

---
## \#3 Posted by: PB1 Posted at: 2016-07-21T13:00:36.613Z Reads: 282

```
Seems like your VESC is overheating. You're not the first to experience this. 

It's interesting that you mention you could do that hill before. So what exactly has changed? 
- Ambient temperature? 
- 10sp3 to 10sp4? So are you giving your motors more power (amps) now and your VESC has to deal with that?
- FOC to BLDC? Interesting! In theory FOC should be more efficient than BLDS

Try to specify what exactly has change and it's potential influence on the system.
```

---
## \#4 Posted by: chaka Posted at: 2016-07-21T13:26:44.880Z Reads: 279

```
Post a screen shot of your motor setting when you get a chance.
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-07-21T13:26:50.358Z Reads: 283

```
@whitepony has said that he noticed a difference in temperature in the two modes BLDC / FOC.

BLDC was much hotter for him. So it will be much likely a overheating problem
```

---
## \#6 Posted by: onloop Posted at: 2016-07-21T13:36:22.039Z Reads: 282

```
What is the motor max current set at?
What is the battery max current set at?
What is gearing reduction ratio?
Wheel size?
Rider weight?
```

---
## \#7 Posted by: quanze Posted at: 2016-07-21T14:11:19.270Z Reads: 267

```
More importantly, when did you order the scp4 and when did you receive it
```

---
## \#8 Posted by: whitepony Posted at: 2016-07-21T14:28:49.803Z Reads: 267

```
[quote="michaelcpg, post:1, topic:6425"]
However when I went to ride up a fairly long and steep hill tonight I got about half way up and I slowly began to lose power until it got to the point where the board was barely moving. I got off for a couple seconds then got back on and started riding again and it seemed to have full power back but about another 10 - 20m up the hill and the same thing started happening. This basically happened another 3 or 4 times till I got to the top of the hill.
[/quote]

thats 100% the thing that happened to me - longer 5-7% hill and Ill eventually become slower and slower until Im barely getting forward anymore. Im about 90% sure that its the vesc overheating soft off that starts at 80°C and switches off the vesc at 100°C (only 90% because Ive never actually did live monitoring to convince myself, but so many indicators speak for a heat issue, that I feel I didnt have to make sure).

and like cookies said: in a direct comparison of bldc and foc, foc came out on top. I can reliably ride up that hill in foc with full throttle without powering down at all while I reliably get power reduction in bldc. thats with the exactly same hardware - just changed bldc for foc.

did that run up the hill several times on different days, since its part of my commute. every time the same result!
```

---
## \#9 Posted by: onloop Posted at: 2016-07-21T15:03:50.202Z Reads: 241

```
2 posts were merged into an existing topic: [FOC vs BLDC Debate](/t/foc-vs-bldc-debate/6216)
```

---
## \#10 Posted by: michaelcpg Posted at: 2016-07-21T21:10:17.960Z Reads: 240

```
@chaka
I ran motor detection and ran settings, will post a few screenshots later today when I get some free time at work.

@PB1
It's the middle of winter here so ambient temperature will be cooler than before if anything.
I don't think changing from 10s3p to 10s4p should have any effect in this regard as the VESC will still only pull as much current as it needs.

@onloop 
From memory, 
motor max current: 80A
battery max current: 40A
Unsure of the gear reduction ratio but I'm using the older version of this kit that had the metal wheel pulley:
http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-pulley-drive-hub-kit/
Wheel size: 83mm Enertion wheels
Rider weight: 90KG
```

---
## \#11 Posted by: Mrmoonlight Posted at: 2016-07-21T22:00:14.302Z Reads: 235

```
I've been having the same issues with my board although I just finished building it. Happens after I ride for awhile and try to go up a hill. Doesn't necessarily have to be that steep of a hill or that long, the board just has to be running for a bit. With the board cold, I can run up a 2-3% grade for half mile with no issues. Just added some heatsinks to my VESC last night. Haven't tested it yet, but will see how it works.
```

---
## \#12 Posted by: michaelcpg Posted at: 2016-07-21T22:11:50.792Z Reads: 242

```
Are you running in BLDC or FOC?
```

---
## \#13 Posted by: chaka Posted at: 2016-07-21T22:15:50.036Z Reads: 238

```
Drop the motor max down to 40-50 amps if you want to climb hills. It may still overheat the vesc because 63's motors will still pull a large amount of wattage but it should help. Best to go dual if you want a cooler running board. 80 amp max will work on flats and short hills in a single 63mm drive but you may need to bump your overheat protection up a few degrees and use a heat sink and fan.
```

---
## \#14 Posted by: Randyc1 Posted at: 2016-07-21T22:39:53.450Z Reads: 238

```
Will the (V6 Vesc)  fix this Overheating problem using 63mm motors chaka ?

And does  B. Vedder know why some have trouble using FOC, or know what the problem is ?
```

---
## \#15 Posted by: michaelcpg Posted at: 2016-07-21T23:00:56.393Z Reads: 235

```
What other noticeable effects might I expect from lowering the motor max? Lower top speed?

Definitely planning to upgrade to dual motors, just not sure whether to wait for VESC 6 or not as well as whether to go with dual 63mm vs dual 50mm motors...

@chaka if I'm having issues running a single 6374 motor up this hill, how do you expect a pair of your 5065 motors would handle it in comparison? 
The hill is 0.7miles long with around a 310 foot increase in altitude
```

---
## \#16 Posted by: onloop Posted at: 2016-07-21T23:24:04.980Z Reads: 230

```
are you the same guy who bypassed the BMS for discharging?

do you know what the BMS is rated to in your SPACE Cell?

it's either the 30A one or the 50A one.

You need to set the motor max lower, 80a is way too high. 60A MAX for that. Maybe lower.

Battery MAX of 40A is also too high if your BMS has a 30A BMS.

It might also be worth checking the voltage MIN - MAX, maybe you are hitting the voltage soft cut.

worst case scenario bypass the BMS and increase your Battery Max current to number closer to the Motor MAX. The VESC will appreciate that especially at lower RPM.
```

---
## \#17 Posted by: onloop Posted at: 2016-07-21T23:25:37.565Z Reads: 224

```
[quote="Randyc1, post:14, topic:6425"]
Will the (V6 Vesc)  fix this Overheating problem using 63mm motors chaka ?
[/quote]

63mm motors don't over heat the VESC, bad settings overheat the VESC
```

---
## \#18 Posted by: onloop Posted at: 2016-07-21T23:27:02.949Z Reads: 224

```
[quote="michaelcpg, post:15, topic:6425"]
What other noticeable effects might I expect from lowering the motor max?
[/quote]

it will prevent your vesc from shutting down, VESC is only rated to 50A cont

slightly less torque during rapid acceleration (probably not noticeable)
```

---
## \#19 Posted by: michaelcpg Posted at: 2016-07-21T23:36:37.556Z Reads: 222

```
In the end I didn't bypass the BMS for discharging, managed to get that issue resolved.

From one of my previous threads, you've told me that my BMS is rated for 50A continuous, because of this and the fact that my space cell came with a 40A fuse, I've set the battery max to 40A.

I based most of my VESC settings off the information you've provided here for the space cell which states that the motor max should be set at 80A:
http://www.electric-skateboard.builders/t/vesc-faq-optimized-s-p-a-c-e-cell-settings/414

I'll lower the motor max for now and see how that affects things
```

---
## \#20 Posted by: Randyc1 Posted at: 2016-07-21T23:48:28.979Z Reads: 214

```
So what setting would you suggest for the vesc to not power down while riding a long hill?

10s4p (40A continous  power capable).
6364-245kv 15T, 36T, 80mm wheels. 74kg.

Starts Strong , then i guess when vesc becomes hot , powers down ?
```

---
## \#21 Posted by: Mrmoonlight Posted at: 2016-07-21T23:53:00.545Z Reads: 206

```
Running FOC. Had the same thing on happen on BLDC too. I'm running a single Carvon Hub. I have my motor max at 70A right now. Haven't tried bumping it up any higher. On flats it runs great. I'm going to try and get some temp data if it still has the issue with this new heatsink installed. <img src="/uploads/db1493/original/2X/e/e57f8b64fc19eb49cf577b80937a1391126ec416.jpg" width="600" height="400">
```

---
## \#22 Posted by: onloop Posted at: 2016-07-22T00:02:54.182Z Reads: 200

```
[quote="Randyc1, post:20, topic:6425"]
So what setting would you suggest for the vesc
[/quote]

you need to be careful not to have the Motor Max & Battery Max current settings too far apart. (or too high)

this is what contributes to VESC heating issues when motors are not running at their max rpm.

Keep turning it down until your problems go away.

If once you resolve the problem the torque output is not enough you need two motors. (or more reduction)
```

---
## \#23 Posted by: chaka Posted at: 2016-07-22T01:48:57.928Z Reads: 199

```
> Will the (V6 Vesc) fix this Overheating problem using 63mm motors chaka ?

> And does B. Vedder know why some have trouble using FOC, or know what the problem is ?

Yes, with V6 you will be able to run 63mm motors to their full potential. Untill then you will need to limit output as best you can with the motor max settings.

FOC should also work a little better due to the more robust design. V6 will be less susceptible to failures.
```

---
## \#24 Posted by: michaelcpg Posted at: 2016-07-23T03:09:10.966Z Reads: 190

```
Here's some screenshots of my current settings. I've dropped the motor max current down to 60A, will test it out once the weather clears up.

<img src="/uploads/db1493/original/2X/7/743b0c5e9c70a19205222bfa64411fd1dbef7a01.jpg" width="690" height="407">
<img src="/uploads/db1493/original/2X/5/54eceb858c93c09734f44797623f14e56b3d18d5.jpg" width="690" height="407">
<img src="/uploads/db1493/original/2X/7/7a75f5e8954ee5f3d708114f171d96e1fa14c704.jpg" width="690" height="407">
<img src="/uploads/db1493/original/2X/d/d6e0f938451a5a9a17d7a5d575a96c71c30dffb5.jpg" width="690" height="407">
<img src="/uploads/db1493/original/2X/4/4989897deefff4e7b41f8a02363ff272d6dcb12d.jpg" width="690" height="407">
```

---
## \#25 Posted by: chaka Posted at: 2016-07-23T03:21:56.128Z Reads: 175

```
If it still overheats drop it down to 40 amps and try again. You can also increase the mosfet start temp to 85 and give yourself a little more headroom.
```

---
## \#26 Posted by: michaelcpg Posted at: 2016-07-23T03:27:43.618Z Reads: 174

```
Ok cheers, will see how things go :)
```

---
## \#27 Posted by: philipp Posted at: 2016-08-01T14:11:18.507Z Reads: 173

```
How did your testing turn out? :)
```

---
## \#28 Posted by: michaelcpg Posted at: 2016-08-01T22:43:46.129Z Reads: 169

```
Got a chance to test the board up the hill again over the weekend (Board was out of action all last week after my belt started tearing). 

Unfortunately I'm still having to stop several times going up the hill to let the VESC cool down, I also found that I'm also having the same issue with another hill that I never used to have issues with when running in FOC which is rather unfortunate. If only FOC was more reliable :/

@chaka I might look at turning the motor max down to 40A and try again, do you expect that this will have much effect on my hill climbing ability though? Certain parts of these hills get quite steep.
```

---
## \#29 Posted by: chaka Posted at: 2016-08-01T22:56:13.217Z Reads: 160

```
You could but you may just have to bite the bullet and reduce your gear ratio. What is your theoretical top speed on you current drive train?
```

---
## \#30 Posted by: michaelcpg Posted at: 2016-08-01T23:04:08.793Z Reads: 158

```
45km I believe? Not that I've ever hit top speed on my board. 
It's essentially an Enertion Raptor mono with a 10s4p pack. These are the pulleys I'm using: http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-pulley-drive-hub-kit/

How would a pair of your motors handle steeper hills? I'm looking to upgrade to a dual drive system at some point in the near future anyway so I'll probably be looking to sell my 6374 and either buy a pair of 6355's or a pair of your 5065's depending on how well they handle steep hills as I like the idea of sensored motors due to the fact that the city I live in is basically built over of a bunch of hills...
```

---
## \#31 Posted by: Jinra Posted at: 2016-08-01T23:06:00.411Z Reads: 154

```
What grade is the hill?
```

---
## \#32 Posted by: michaelcpg Posted at: 2016-08-01T23:07:46.411Z Reads: 158

```
It varies a bit. This is one of the hills (Brooklyn Rd). I believe its an average 8% grade but some parts are definitely a fair bit steeper

https://goo.gl/maps/xe1CNJdXHh32
```

---
## \#33 Posted by: onloop Posted at: 2016-08-01T23:13:32.483Z Reads: 158

```
check this out, 

https://www.youtube.com/watch?v=eakga9Bzj9E
```

---
## \#34 Posted by: Mrmoonlight Posted at: 2016-08-01T23:22:10.395Z Reads: 155

```
Do you get the heatsink package with your VESC? 

I'm working through a very similar issue and while I still haven't solved it, installing heatsinks has made a world of difference. I used to cut out on 3% grades after a few meters, now I can go a quarter mile if I don't push it. It's still not performing as it should, but the heatsinks made a huge improvement.
```

---
## \#35 Posted by: michaelcpg Posted at: 2016-08-01T23:25:06.556Z Reads: 155

```
Yea I've got the heatsink package, might have to eventually look at cutting a section out of the bottom of my enclosure where I can install a larger external heatsink which I can attach VESC's to similar to Evolve boards
```

---
## \#36 Posted by: chaka Posted at: 2016-08-01T23:25:21.871Z Reads: 154

```
A good top speed for an all around board on a single drive is about 35 km or less. This will take the edge off the torque needed to take on hills without overheating the VESC. 

You could drop down to a smaller motor and the VESC will not overheat as easily. The problem is that motor will pull way more amps than the VESC can give without heating up.
```

---
## \#37 Posted by: Randyc1 Posted at: 2016-08-01T23:40:59.021Z Reads: 150

```
So the vesc is not 50A continuous ? , my battery 4p can only provide 40A continuous and will have the same behavior up a long hill. ?
```

---
## \#38 Posted by: chaka Posted at: 2016-08-02T00:19:26.151Z Reads: 150

```
What type of cells are you using? You could be tripping the low voltage back off strategy on the vesc if your pack is only capable of 40 amps without voltage sag.
```

---
## \#39 Posted by: Randyc1 Posted at: 2016-08-02T01:24:07.387Z Reads: 144

```
Using the Tesla cells from okashira, they are supposed to be very similar to the Panasonic GA cells with slightly less capacity 3200mah.
```

---
## \#40 Posted by: evoheyax Posted at: 2016-08-02T04:30:37.031Z Reads: 139

```
[quote="onloop, post:16, topic:6425"]
are you the same guy who bypassed the BMS for discharging?
[/quote]

No that was me. But I've helped a couple others do the mod. It's been through 200 or so cycles like this no problems so far for me.
```

---
## \#41 Posted by: c4Lvin Posted at: 2016-08-02T06:30:13.293Z Reads: 126

```
I think there's your problem. Those cells are probably not high discharge like the 25Rs or HE/HG cells.
```

---
## \#42 Posted by: philipp Posted at: 2016-08-02T20:46:18.143Z Reads: 130

```
[quote="Mrmoonlight, post:34, topic:6425"]
installing heatsinks has made a world of difference.
[/quote]

Nice to hear that. Just ordered me some raspberry PI heatsinks, will equip the mostfests with them and hope to get same results :slight_smile:
```

---
## \#43 Posted by: Mrmoonlight Posted at: 2016-08-02T20:55:19.190Z Reads: 128

```
If you have the space, go with a bigger one. I currently have four 20mmX20mmX6mm, but I think a bigger one like Chaka uses would work better.
```

---
## \#44 Posted by: philipp Posted at: 2016-08-02T20:59:26.120Z Reads: 126

```
I'm on ebay right now looking for a big one wich I will cut a rectangle in the Space Cell 3 enclosure.
I'm thinking about mounting the VESC directly on the inside of the heatsink while the outside will have direct contact to the wind. The mosfets facing inwards will get the small raspberry pi sinks.
```

---
## \#45 Posted by: c4Lvin Posted at: 2016-08-02T21:06:11.612Z Reads: 128

```
just wondering how the heatsinks are mounted onto the MOSFETS?
```

---
## \#46 Posted by: Mrmoonlight Posted at: 2016-08-02T21:27:55.309Z Reads: 137

```
Thermal paste then shrink tubing with a hole cut out for circulation.
```

---
## \#47 Posted by: Dunmer Posted at: 2016-09-21T13:31:26.346Z Reads: 107

```
Any updates about this problem? I have the same thing but on the flats :slight_smile:
With a fresh start i can go to my 40-42km/h top speed, no problem, but then the speed starts to decay and i can only go 35km/h and then 25-28km/h. If i then get some headwind i only go like 18 or so. Sucks alot! I like the 40km/h speed :slight_smile:

Same thing if i carve and coast at 25km/h and then i want to go fast and pump full throttle, then it stays put at 25km/h and i can't go faster. Stop the board, wait for 20sec and then i off again to 40km/h for a small period of time.

SK3 192kv single drive
12mm belt
10s3p space cell
VESC
83mm wheels
84kg rider
<img src="/uploads/db1493/original/3X/b/b/bbaf8cc28a0192a596b7611a5f1a2766a9135725.png" width="690" height="389">
```

---
## \#48 Posted by: makevoid Posted at: 2016-09-21T14:16:04.392Z Reads: 100

```
It seems pretty stupid but I didn't notice until recently, I am not a skater/longboarder so I really didn't know this one obvious thing. Believe it or not I overtightened my wheels / axle nuts and that squashed the bearings a bit, the wheels had a bit of resistance, now I loosened them enough that they don't move laterally and if I spin them by hand they spin for more than a minute. Before they were too tight (they used to spin like 20s max that way), enough to make the VESC overheat more on small hills. Now the VESC with my single 6374 still limits my speed on medium hills (6% grade, I'm ~220lbs) but at least I can do them. 

Also, increasing motor max from 40A  to 50A or even 60A (I'm using 50A batt max setting, using 40 li-ion cells) actually helped me increasing the initial speed so that the board starts to slow down / overheat later (this doesn't work if the hill is very long unfortunately).
Another stupid thing that can help you is carving (zig zag motion) instead of going straight :D ^^ To add on top of that, in winter  (colder weather) it will overheat less because of external temperature, I noticed that a 10deg C drop in temperature is enough to affect my rides. 

But yes, I agree that a smaller motor should overheat less, heatsinks help, some airflow in the enclosure and a fan will be my next steps and if that will not be enough I will go dual  :D
```

---
## \#49 Posted by: guyguy Posted at: 2016-09-21T17:55:57.682Z Reads: 98

```
[quote="makevoid, post:48, topic:6425"]
I am not a skater/longboarder so I really didn't know this one obvious thing. Believe it or not I overtightened my wheels / axle nuts and that squashed the bearings a bit, the wheels had a bit of resistance,
[/quote]
If it's any consolation I'm guilty of doing this too - even with washers you can over tighten the nylock nuts.
```

---
## \#50 Posted by: Mrmoonlight Posted at: 2016-09-21T18:54:06.873Z Reads: 93

```
Sounds like my issue with my VESC overheating. Have you installed a heatsink? What VESC are you using? Some VESC's are more prone to overheating with certain setups than others.
```

---
## \#51 Posted by: Dunmer Posted at: 2016-09-21T21:32:23.103Z Reads: 89

```
I don't have a heatsink. The vesc I am using is the 4.12 with 2.18 firmware. 
First ting I Will try is cut my vesc loose because now it is glued to my enclosure and the 3 mosfets are drowning in it :slight_smile: Should glue it on some other components. If this doesn't work then the heatsink is next to try out. Don't feel like cutting in my enclosure, it's so clean and slick now :slight_smile:
```

---
## \#52 Posted by: Mrmoonlight Posted at: 2016-09-22T01:03:53.823Z Reads: 84

```
For your VESC, I suggest adding a heatsink. They are only a couple bucks on Ebay. Make sure you attach them with some thermal paste so the heat transfers well. I used shrink tube to secure mine, but there are a number of ways. 

http://www.ebay.com/itm/381103432358?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
