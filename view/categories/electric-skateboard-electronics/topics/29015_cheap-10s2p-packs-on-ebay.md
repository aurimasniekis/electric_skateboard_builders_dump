# Cheap 10s2p packs on ebay

### Replies: 24 Views: 3403

## \#1 Posted by: curioussavage Posted at: 2017-07-29T04:13:27.554Z Reads: 335

```
I saw this on ebay http://www.ebay.com/itm/NEW-SAMSUNG-18650-36V-4-4AH-BATTERY-EBIKE-VAPE-POWERWALL-BATTERIES-20-CELLS-BMS-/201895735309?epid=1621923126&hash=item2f01ec700d:g:Mh8AAOSwSypY9Y7d  35$ seems way too good to be true. I'm assuming somebody here might be able to comment on them. Anybody bought one of these for testing? cheap enough that it doesn't really hurt much if they are fake.
```

---
## \#2 Posted by: Boardnamics Posted at: 2017-07-29T04:18:44.926Z Reads: 333

```
Woah...imagine a 10s4p pack for $70! Something does seem fishy here though, my guess is the cells are maybe the binned samsung ones or not genuine. Then again I am no expert so someone else here can give a better idea.
```

---
## \#3 Posted by: Jinra Posted at: 2017-07-29T04:20:12.444Z Reads: 326

```
There's a couple threads on this already. They're using 10A continuous cells. Unless you go 6p+ you're going to incur a large amount of voltage sag.
```

---
## \#4 Posted by: Boardnamics Posted at: 2017-07-29T04:26:30.530Z Reads: 321

```
Still not too shabby. 10s8p would be close to 600wh for $150
```

---
## \#5 Posted by: curioussavage Posted at: 2017-07-29T04:34:14.635Z Reads: 299

```
[quote="Jinra, post:3, topic:29015"]
There's a couple threads on this already
[/quote]



could you link to them?
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-29T04:38:58.608Z Reads: 283

```
http://www.electric-skateboard.builders/t/cheap-18650s-1-75-per-cell-lg/25245

http://www.electric-skateboard.builders/t/1-to-2-lg-18650-cells/25006
```

---
## \#7 Posted by: adseguy Posted at: 2017-07-29T06:02:40.324Z Reads: 272

```
I've got them, I use them.  No issues.  Great stuff and at 10S6P I indeed am around 500Whr and really do get about 25 miles.  It's legit.
```

---
## \#8 Posted by: pennyboard Posted at: 2017-07-29T07:04:23.383Z Reads: 262

```
Can anyone who has them tell me about the physical shape? I looked at getting them for my board, but it looks like with them stacked 3 high, they won't give me enough clearance underneath the board.
```

---
## \#9 Posted by: ElskerShadow Posted at: 2017-07-29T07:15:11.082Z Reads: 245

```
What about voltage sag since it's only 10A ?
```

---
## \#10 Posted by: adseguy Posted at: 2017-07-29T07:20:35.691Z Reads: 242

```
Definitely a few volts of SAG, but the 10Amp is continuous with a 20Amp max.  Even at high speed I'm still not pulling a full 60amps through the battery and even if it's OK to do 20Amps for a second here and there that would be 120Amps!!
```

---
## \#11 Posted by: Kedwards Posted at: 2017-08-04T02:09:44.930Z Reads: 205

```
Did you harvest the cells from the pre-built packs, or instead used them in their original configuration? If the latter, I'm interested to know of your experience using the included bms; does it limit the discharging capabilities in any way, or is its function merely for charging?
```

---
## \#12 Posted by: adseguy Posted at: 2017-08-04T05:05:51.230Z Reads: 200

```
No Harvesting here.  Just using them in their original configs.  That's a good question on the discharging from the BMS, but I don't believe so (don't quote me).  Either way each Cell is rated for 10A cont. and 20A max making each "pack" 20A continous and 40A max.  Throw two of them in there (40 batteries) and you have a nice 16mile range with  40A continous and 80A Max.  That's great for anybody.  I opted for 3 packs and It's great to have 25 mile range.  I charge it every 4th ride or so (unless it's a super long)
```

---
## \#13 Posted by: Kedwards Posted at: 2017-08-04T19:37:05.807Z Reads: 183

```
Awesome; just ordered a pack off eBay. Since this will be my first foray into the 18650 world (basic lipos before), can I ask how you're charging them? Looks like I'll have to desolder the xt60s and use a standard 42v hoverboard power supply...
```

---
## \#14 Posted by: adseguy Posted at: 2017-08-04T19:57:40.207Z Reads: 178

```
I wired them all in parallel keeping the XT60 connections.  Then I paralleled a connector from my charger I already have from an electric bike.  It's an XLR connector.  Charging at 2Amps takes about 5 hours.  No need to charge each independently.
```

---
## \#15 Posted by: Silverline Posted at: 2017-08-04T20:05:13.569Z Reads: 173

```
Looks interesting.
Maybe he could do some custom builds ?
```

---
## \#16 Posted by: Kedwards Posted at: 2017-08-07T00:39:00.596Z Reads: 165

```
Would you mind sketching/verbally describing a super basic wiring diagram of how you connected everything together to charge without needing to disconnect the xt60 connectors? This is my first time wiring everything up, and I'm a bit confused as to how to solder in my XLR charging port without connecting to the individual BMS's. Many thanks if this is possible!
```

---
## \#17 Posted by: adseguy Posted at: 2017-08-07T03:48:04.505Z Reads: 167

```
<img src="/uploads/db1493/original/3X/1/8/1805c5d2b437a195c90380e8adf8fa11b2ea34a3.jpg" width="375" height="500">

So you can see in this the XLR connector (or any connector really) will charge all the batteries at the same time.  I can even remove my loop key to keep everything off as well and still charge.

Edit: I noticed the right most pack looks like it's connected in series.  It's a mistake, but I know it's parallel.  Most might not assume the mistake so I want to make sure no one catches things on fire.
```

---
## \#18 Posted by: Kedwards Posted at: 2017-08-07T04:24:08.453Z Reads: 153

```
Awesome- that is so helpful. Many thanks!
```

---
## \#19 Posted by: oct0f1sh Posted at: 2017-08-16T02:14:55.228Z Reads: 144

```
Did you disassemble the packs to make them flatter? Also, are you using all 3 BMS boards, if so how do you charge it? Is there any way you can post a picture of your setup? I'm thinking about getting some of these packs for my build, but I live in SF and it needs to be able to handle some pretty serious hills.
```

---
## \#20 Posted by: adseguy Posted at: 2017-08-16T02:28:41.972Z Reads: 146

```
My Buddy did disassemble the pack just a bit and he re-routed the 3 BMS boards.  I kept as is.  No issues, I just can't hop curbs, but who does...
I think you should re-read the posts.  I put up a sketch, and I mentioned the current draw will never hit the limits, not even the continous limits in the 6P config.  They are never hot either.  Warm, yes, but not hot.
```

---
## \#21 Posted by: Izzet Posted at: 2017-08-16T03:51:17.708Z Reads: 129

```
any pictures of what it looks under a board?
```

---
## \#22 Posted by: Gabriel7845 Posted at: 2017-09-18T00:04:08.623Z Reads: 116

```
I want to make a really light board because I'm going to be using it to get to class and a small range isn't really a problem. could I just use one pack and set the 40A max on the vesc? if so how much would that affect performance?
```

---
## \#23 Posted by: Menjos Posted at: 2017-09-18T00:55:20.562Z Reads: 113

```
Stay away from these if you can. Yes they don't get hot, that's because the voltage sag is so massive. If you use these in 10s4p configuration you should be OK, but for 10s2p you'll be way better off investing a in 25R's.
```

---
## \#24 Posted by: yulaw2k Posted at: 2017-10-13T04:10:35.338Z Reads: 87

```
From everything I have read about these packs, these do not have BMS boards but just PCB boards, meaning it wont balance when you charge. I am using one as is on my board with a meepo esc board to two hub motors. I think i'll buy another one and make it a 10s4p and buy a real BMS.
```

---
