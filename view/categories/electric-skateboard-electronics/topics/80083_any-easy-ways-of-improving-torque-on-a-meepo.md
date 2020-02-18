# Any easy ways of improving torque on a Meepo?

### Replies: 30 Views: 912

## \#1 Posted by: iKst Posted at: 2019-01-06T11:12:53.210Z Reads: 202

```
Hi guys, 

I will be building a belt driven esk8 in the summer with duač 6374 motors, but in the meantime, I am using my Meepo. I like it a lot, it rides very well and it's plenty fast. The only problem is, I live in a town with a lot of hills. I have to climb a quite steep, 300m long hill to get home. Right now the board can pull me up, but it's very slow on the uphill.

So, my question is. Is there an easy and not too expensive way of improving uphill performance of these hub motors? 

I've seen that some people are running 12S battery on meepo, but I am not sure if this would have an impact on performance since ESC is probably a limiting factor?
```

---
## \#2 Posted by: pat.speed Posted at: 2019-01-06T12:13:39.170Z Reads: 189

```
Running 12s _may_ help torque but it can’t be guaranteed, the best option would be to increase battery amps or motors amps. However neither of these can be done with the stock meepo esc.

The last option would be to add 4wd to it by putting an extra esc,battery and motors on the front, but this will be expensive and not entirely worth the money to do this
```

---
## \#3 Posted by: sayekim Posted at: 2019-01-06T12:15:48.581Z Reads: 187

```
I got rid of the esc and replaced them with focboxes. Torque was greatly improved. Like shit in pants torque if your battery can handle it. 

It can handle those hills easily afterwards. 
It is also what got me started to diy in the first place. 
Check my topic on this.

https://www.electric-skateboard.builders/t/meepo-esc-to-focbox-blank-double-kick-drop-down-90-mm-hubs-sanyo-20700b-10s2p-now-12s2p-sanyo-with-torque-drives-used-to-be-speed-drives/44021?u=sayekim
```

---
## \#4 Posted by: sayekim Posted at: 2019-01-06T12:21:17.433Z Reads: 170

```
My groupride on youtube from last year where I am rocking the meepo on focboxes. 

https://youtu.be/eoWumJU1MH4
```

---
## \#5 Posted by: rey8801 Posted at: 2019-01-06T12:21:41.303Z Reads: 166

```
I used the Meepo hubs. Best thing you can do is replace ESC with VESC capable to handle 12s. Then I made a 12s3p 30Q battery and now the Meepo hubs run for 25-30km at 45kmh and the torque is really really good. I am using two single FESC 6.6. Dual FeSC 6.6 will work too. If you want to stay dirty cheap I have seen people using the two single 4.12 from Flipsky (the one at 60$ shipped on ebay, Ali) at 12s with FOC.
```

---
## \#6 Posted by: Friskies Posted at: 2019-01-06T12:22:16.554Z Reads: 157

```
Meepo setting are something around 18A per motor. Should get a Flipsky dual and run at 30 or so and it will keep you happy until they break :slight_smile:
```

---
## \#7 Posted by: Matt_54 Posted at: 2019-01-06T13:04:47.516Z Reads: 154

```
What settings did you use?
```

---
## \#8 Posted by: Psmrman90 Posted at: 2019-01-06T18:24:31.358Z Reads: 135

```
Are 30amps/motor a good amount? I'm nearing the end of my build (11s3p, dual 6374, 16/40, 97mm) and have settings at 30 amps per motor and am curious what kind of kick it'll have
```

---
## \#9 Posted by: Hummie Posted at: 2019-01-06T18:32:13.748Z Reads: 133

```
90 motor amps per motor gives great low speed kick n reduced cogging.
```

---
## \#10 Posted by: Toughook Posted at: 2019-01-06T18:33:52.292Z Reads: 133

```
I'll have a couple of spare focboxs after I fit my UNITY to my main board. Wasn't aware the Meepo style hubs could be run off focboxs. Might be worth swapping out the ESC in my son's budget board for them by the sounds of it ? (Which is essentially a Meepo clone anyway).
```

---
## \#11 Posted by: Psmrman90 Posted at: 2019-01-06T18:40:34.227Z Reads: 131

```
You messin with me?  My battery has a max 60amps of total continuous, how the hell does someone do 90 per motor ??  180 continuous combined rhen?
```

---
## \#12 Posted by: Frenchy Posted at: 2019-01-06T18:45:37.140Z Reads: 128

```
Lipo power
```

---
## \#13 Posted by: Hummie Posted at: 2019-01-06T18:54:11.812Z Reads: 124

```
Motor amps aren’t battery amps.  Motor amps are real amps but it’s like the voltage has been bucked down n the battery current would be way less.  Look at the live data on Vesc tool

You could have maybe 5 amps sucked from the battery and have 90 motor amps
```

---
## \#14 Posted by: dareno Posted at: 2019-01-06T20:05:14.027Z Reads: 115

```
While its possible to use vesc's on a meepo and you can then control the amps you must be very careful of not overloading the bms in the standard battery.  Anything over 20 amps per vesc and you run the risk of the bms going poof.  Best way is to change out the esc and the battery and while this is expensive you will then have a board that is truly a lot of fun.  My "focpo"  runs a crappy old diye 10s5p and focboxes and its not bad at all although it does sag like a witches tit at about 30%.  Best way to really get some juice from it is as the guys have said get a 30q pack in there or a couple of lipos.  The motors are actually capable of a lot more than the meepo ever asks of them.  Great way to get amongst the diy scene is to upgrade a pre-built and leave it looking standard just to confound the other meepo riders on a group ride.  Sleepers rule!
```

---
## \#15 Posted by: Winfly Posted at: 2019-01-06T20:12:42.659Z Reads: 115

```
+1 on upgrade to VESC

Cheapest way and the only way I see worth is with 2 x 4.12 VESC or the flipsky dual 4.20, which is only good to about 30A each motor, more than enough for the old meepo hubs. 

12s Battery upgrade is expensive and overkill for a cheap meepo.

P.s. not sure what spec is meepo battery.
```

---
## \#16 Posted by: sayekim Posted at: 2019-01-06T20:24:29.775Z Reads: 114

```
Considering that the op is going to diy they might as well purchase the unity if that proves to be good and reliable when it’s done and build a 12s battery. 

If just sticking with meepo hubs then yes purchase them cheap flipsky esc, but honestly if you’re upgrading a china production board with diy you’ll want to get the best of the best anyway since you’re hooked already and then you’ll already have some great main hardware to start with for your real first diy build.
```

---
## \#17 Posted by: Hummie Posted at: 2019-01-06T20:50:32.102Z Reads: 108

```
A lot of presenting of the unity as great stuff but according to vedder and others who know what the hell is what @linsus it’s not a good design with two shunts and not three. We will see
```

---
## \#18 Posted by: Roan_Psyko Posted at: 2019-01-07T01:05:15.696Z Reads: 99

```
![1546674160586|375x500](upload://xIMPeLAErFsQ3DC2UqCzEzmbCBM.jpeg) 

We're currently running some tests, but the unity may be the easiest option to swap out the original esc of most budget boards to increase hill climbing performance among other benefits. Like mentioned above, the motors can handle more than what those esc's allow. 
Once we're done testing it we'll make a video about our findings. getting a new battery pack may not be necessary depending on how much extra kick you need ;)
```

---
## \#19 Posted by: Winfly Posted at: 2019-01-07T03:56:19.282Z Reads: 96

```
[quote="Hummie, post:17, topic:80083"]
according to vedder and others who know what the hell is what @linsus it’s not a good design with two shunts and not three. We will see
[/quote]

Interested in what @Deodand would comment on that.
```

---
## \#20 Posted by: mmaner Posted at: 2019-01-07T04:03:18.764Z Reads: 99

```
I think it's safe to say Ben's interests are profit related these days, so I'm not sure how valid his opinion is about the competition.
```

---
## \#21 Posted by: Meeep Posted at: 2019-01-07T08:06:52.763Z Reads: 93

```
Since the ESC has a limited, non-programable amp output limit and hub motors have no gearing you have very limited options for improving torque.

1. The 90mm "beast" motors are more powerful than the original v2 motors and the swappable motors

2. VESC

3. Better cells. A Sanyo 2070C/20700A or a Sony VTC6A/5A pack will sag less than samsung 20/25r/30q. Power = Volts*amps

4. Parallel battery setup. Similar to the better cells approach. Spread the load over more cells = less voltage sag. I did this with my original meepo packs because the power output was abysmal. Required me fabricating a 10s4p custom enclosure.

5. Higher voltage since the current limit is fixed. This will more directly affect top speed than torque. I built my own 11s3p 30q pack for my meepo and the power output is much improved from my original samsung 22p packs.
```

---
## \#22 Posted by: pat.speed Posted at: 2019-01-07T08:50:58.387Z Reads: 89

```
Option 3 and 4 won’t make a difference as the esc limits the current going to the motors anyway
```

---
## \#23 Posted by: iKst Posted at: 2019-01-07T10:11:24.806Z Reads: 86

```
Thanks for all the answers. It looks like using a different ESC is the way to go.

For now, I ordered an upgraded battery pack for extended range (sanyo 20700b) and I will start researching my options about what ESC to get.

I will start reading about this, I have no clue what are the differences between VESC 4 and 6 etc, but can someone please explain what other options than flipsky and focbox unity I have and what to expect from them.
```

---
## \#24 Posted by: Meeep Posted at: 2019-01-08T02:04:28.246Z Reads: 76

```
I know but the cell will not have as much voltage drop under that load. I did a parallel conversion back in October 2017 and my hill climbing improved. This is all to my current (pun intended) understanding.
```

---
## \#25 Posted by: pat.speed Posted at: 2019-01-08T03:42:00.803Z Reads: 71

```
Yeah I suppose you will have less voltage sag, however the limit of the esc is still the main issue with hill climbing capability
```

---
## \#26 Posted by: b264 Posted at: 2019-01-08T08:50:43.712Z Reads: 72

```
Option 3 and 4 would make the battery last a lot longer though.  Especially if you upgraded the ESC or trucks/motors/transmission
```

---
## \#27 Posted by: Matt_54 Posted at: 2019-01-08T15:11:13.162Z Reads: 62

```
I plan on switching my meepo to vesc but for the battery upgrade should I switch to a 12s3p 30q or 10s4p 30q? Also does anyone have recommended settings for the meepo hubs?
```

---
## \#28 Posted by: sayekim Posted at: 2019-01-08T15:38:20.002Z Reads: 60

```
12s if you want 42kph. 10s if you’re fine with 35kph. 

60
-25
25
-15

If your batt can handle it.
```

---
## \#29 Posted by: sk8l8r Posted at: 2019-01-08T16:16:49.212Z Reads: 58

```
[quote="Winfly, post:15, topic:80083"]
+1 on upgrade to VESC

Cheapest way and the only way I see worth is with 2 x 4.12 VESC or the flipsky dual 4.20
[/quote]

totally agree.. dual 4.20 fits the meepo enc. its almost perfect
```

---
## \#30 Posted by: Meeep Posted at: 2019-01-09T17:41:43.567Z Reads: 40

```
I tested my v2 meepo esc at 12s and the HVC kicked in so it was useless. I run 11s.
```

---
