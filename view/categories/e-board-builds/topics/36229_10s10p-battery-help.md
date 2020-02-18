# 10S10P Battery help

### Replies: 59 Views: 2496

## \#1 Posted by: Gabriel_Robinson Posted at: 2017-10-22T23:49:16.880Z Reads: 309

```
My old build is here. 
http://www.electric-skateboard.builders/t/surf-6s-30c-diy-vesc-jlab-6374-190kv-mono-drive-robert-august-deck-97mm-wheels-mini-remote/18671 
It was good for about 6 months but now it is just too slow and doesn't have nearly enough range. To fix this I am going to get these batteries. 
https://www.ebay.com/itm/5-SAMSUNG-18650-36V-4-4AH-BATTERY-EBIKE-VAPE-POWERWALL-BATTERIES-100-CELLS-BMS-/172657519593?hash=item283330abe9:g:Mh8AAOSwSypY9Y7d
Right now I am planing on having a  10s10p battery. The only problem is I don't know how I would charge all of them at the same time. Can someone please help me with this? Thanks!
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-10-22T23:54:09.152Z Reads: 276

```
connect all of them in parallel. charge that way.  you just need to splice the discharge leads into a charging port and your all set
```

---
## \#3 Posted by: Gabriel_Robinson Posted at: 2017-10-22T23:59:57.604Z Reads: 276

```
Are the discharge leads the black wires on the bms jst connector?
```

---
## \#4 Posted by: scepterr Posted at: 2017-10-23T00:00:40.899Z Reads: 271

```
There's 1 connector to use, the xt60, that is all
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-10-23T00:01:00.649Z Reads: 259

```
the discharge leads are the ones with the connector on them
```

---
## \#6 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:01:42.569Z Reads: 239

```
would I just use a hobby charger with an xt-60 connector?
```

---
## \#7 Posted by: scepterr Posted at: 2017-10-23T00:02:10.589Z Reads: 228

```
You can use any 42/36 lithium charger
```

---
## \#8 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:04:24.426Z Reads: 230

```
I'm confused. So I would splice all of the Bms Leads?
```

---
## \#9 Posted by: scepterr Posted at: 2017-10-23T00:05:12.224Z Reads: 224

```
No, don't touch the BMS at all
You're dealing with **1** connector the xt60, forget the BMS exists

You just combine the xt60s that is IT
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-10-23T00:06:17.813Z Reads: 214

```
yea. what scepterr said.

I'm talking about the main thick wires that lead to the xt60.  the same ones you would plug into the vesc
```

---
## \#11 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:06:40.644Z Reads: 199

```
So just hook all of them in Parallel and charge through the xt-60 connectors by adding a charging port ?
```

---
## \#12 Posted by: scepterr Posted at: 2017-10-23T00:06:55.869Z Reads: 194

```
Yes, it's that simple
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-10-23T00:06:56.368Z Reads: 194

```
exactly
10chars
```

---
## \#14 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:07:16.881Z Reads: 185

```
Lmao thanks guys I feel stupid now.
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-10-23T00:08:02.286Z Reads: 182

```
just letting you know...

10s10p is gonna be heavy as FUCK.  10s6p is 7 pounds. my guess is that 10s10p will weigh around 13 pounds
```

---
## \#16 Posted by: scepterr Posted at: 2017-10-23T00:08:14.170Z Reads: 182

```
It's all good, you got it now 😉

I would deff suggest a 5A charger to charge 20Ah
..that'll take like 6hrs
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-10-23T00:08:28.833Z Reads: 178

```
he explained the exact same thing to me lol. took me a bit longer to comprehend though
```

---
## \#18 Posted by: scepterr Posted at: 2017-10-23T00:10:17.782Z Reads: 180

```
Hooking these up is so simple it is facepalm worthy
```

---
## \#19 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:10:22.471Z Reads: 178

```
Yah I know its going to be heavy but I'm planning on buying 5 of them becuase I would rather have to much range than not enough because I am tired of my board dieing.
```

---
## \#20 Posted by: GrecoMan Posted at: 2017-10-23T00:11:06.413Z Reads: 178

```
I set aside like 4 hours the day I got these to wire them. took about 30 minutes to get a completed pack lol
```

---
## \#21 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:11:34.010Z Reads: 158

```
Have you tried yours out yet?
```

---
## \#22 Posted by: GrecoMan Posted at: 2017-10-23T00:12:24.952Z Reads: 155

```
nope. still no vesc.  I think scepty said hes shipping me one tomorrow though. hopefully itll be here Wednesday.  Did I mention hes a super nice guy?
```

---
## \#23 Posted by: scepterr Posted at: 2017-10-23T00:12:25.800Z Reads: 154

```
I know one of my clients with a 10s8p with the LG packs is getting about 20miles between charges
Vesc is set at 40A motor max, 30A batt max
```

---
## \#24 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:13:56.371Z Reads: 151

```
Do these packs have alot of sag?
```

---
## \#25 Posted by: scepterr Posted at: 2017-10-23T00:14:44.872Z Reads: 152

```
I have no idea about the Sona cells I have never in my life seen them or used or heard of them

The LG or Samsung cells do sag at full load
Running an 8P at 30A means 0 sag
```

---
## \#26 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:16:17.388Z Reads: 141

```
I accidently put the wrong link. I am planning on getting the packs with Samsung cells.
```

---
## \#27 Posted by: scepterr Posted at: 2017-10-23T00:17:44.035Z Reads: 134

```
Well then yah don't run them above 5-7A cont per cell, you really can't cause the BMS are 10-12A limited, with 10P you could do 50A batt
```

---
## \#28 Posted by: GrecoMan Posted at: 2017-10-23T00:18:21.217Z Reads: 132

```
wait so running my 6p at 20a means no sag also?

cause my plan was to put the batt. max at 30a
```

---
## \#29 Posted by: scepterr Posted at: 2017-10-23T00:19:00.176Z Reads: 130

```
Yeah, that should not have visible sag from just heavy load
You can do 25
```

---
## \#30 Posted by: GrecoMan Posted at: 2017-10-23T00:19:53.768Z Reads: 131

```
but 30a will correct?
```

---
## \#31 Posted by: scepterr Posted at: 2017-10-23T00:20:34.438Z Reads: 127

```
I wouldn't run at max BMS current either, they'll heat up, might pop, they are not great BMS...
```

---
## \#32 Posted by: GrecoMan Posted at: 2017-10-23T00:20:43.214Z Reads: 126

```
alright 25a max it is lol. guess I'm stepping down from 50a of my last pack...

its worth it for 20 mile range though
```

---
## \#33 Posted by: scepterr Posted at: 2017-10-23T00:21:13.278Z Reads: 127

```
I run my 9S at 25A max...
```

---
## \#34 Posted by: GrecoMan Posted at: 2017-10-23T00:21:51.580Z Reads: 117

```
yea not sure ive ever pulled anything over 25a so I should be ok either way.

its just that state of mind
```

---
## \#35 Posted by: scepterr Posted at: 2017-10-23T00:23:02.491Z Reads: 119

```
 I always start with lowest working settings and tweak up to where I want it. 
You will always have more conservative settings that way and get what you want. 
If you start high and tweak down you'll stop much higher
```

---
## \#36 Posted by: Gabriel_Robinson Posted at: 2017-10-23T00:23:42.954Z Reads: 122

```
Im gonna get this charger.
 https://www.ebay.com/itm/42V-5A-FAST-Charger-For-36V-Li-Ion-Electric-Bike-Bicycle-Ebike-Batteries-/263274070242?hash=item3d4c5b80e2:g:gcEAAOSwa~BYSrny

Where do you guys get a charging port.
```

---
## \#37 Posted by: GrecoMan Posted at: 2017-10-23T00:24:35.190Z Reads: 117

```
maybe ill pick up one of those mini usb extensions so I don't have to open my enclosure a bunch lol.

good idea though.

totally off topic but...
is the bt module I'm getting for metr? if not then which app is it good for
```

---
## \#38 Posted by: scepterr Posted at: 2017-10-23T00:26:07.834Z Reads: 122

```
It's not for metr, it works with EVERY other app, though I think it works read only on metr...not aure
```

---
## \#39 Posted by: b264 Posted at: 2017-10-23T00:26:33.627Z Reads: 131

```
[quote="GrecoMan, post:15, topic:36229, full:true"]
just letting you know...

10s10p is gonna be heavy as FUCK.  10s6p is 7 pounds. my guess is that 10s10p will weigh around 13 pounds
[/quote]

Won't anyone think of the range LoLz

Some of us know how heavy it will be and want it anyway.  I'm in the process of getting a 10S16P build underway.  I want a 100 mile board.  So if I want to ride it all day long, I can do that.
```

---
## \#40 Posted by: GrecoMan Posted at: 2017-10-23T00:27:20.964Z Reads: 129

```
lol. not sure what other apps there are for us IOS scrubs...
```

---
## \#41 Posted by: b264 Posted at: 2017-10-23T00:27:59.005Z Reads: 119

```
Pretty sure it's expected that if you use iOS, you also prefer a Boosted brand esk8.  Just something I've noticed
```

---
## \#42 Posted by: GrecoMan Posted at: 2017-10-23T00:28:28.562Z Reads: 119

```
:cry:

I didn't get a choice
```

---
## \#43 Posted by: scepterr Posted at: 2017-10-23T00:29:28.827Z Reads: 121

```
https://www.electric-skateboard.builders/t/new-version-2-0-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340
```

---
## \#44 Posted by: GrecoMan Posted at: 2017-10-23T00:29:58.448Z Reads: 116

```
shite.

Knew I saw a post about one somewhere lol
```

---
## \#45 Posted by: GrecoMan Posted at: 2017-10-23T00:31:07.074Z Reads: 118

```
awww wtf 3.99
```

---
## \#46 Posted by: scepterr Posted at: 2017-10-23T00:34:30.918Z Reads: 115

```
Blame Apple for not having simple app side loading
```

---
## \#47 Posted by: GrecoMan Posted at: 2017-10-23T00:34:57.686Z Reads: 114

```
ill write them a letter
```

---
## \#48 Posted by: b264 Posted at: 2017-10-23T00:50:05.519Z Reads: 113

```
[quote="GrecoMan, post:47, topic:36229, full:true"]
ill write them a letter
[/quote]

Don't write them a letter; vote with your dollars.  Never buy anything Apple.
```

---
## \#49 Posted by: GrecoMan Posted at: 2017-10-23T00:50:57.300Z Reads: 111

```
i told you.

I DONT CHOOSE

lol take it up with my mom. I cant really complain since I didn't have to pay a penny for it
```

---
## \#50 Posted by: Jedi Posted at: 2017-10-23T01:26:10.036Z Reads: 112

```
Why do you need 100 cells on a skateboard?
```

---
## \#51 Posted by: Chewie Posted at: 2017-10-23T01:41:31.632Z Reads: 111

```
I get 30 miles outta 60 of them, he must want 50!
```

---
## \#52 Posted by: Gabriel_Robinson Posted at: 2017-10-23T01:44:49.635Z Reads: 114

```
I don't I just want to never have to worry about it dieing.  I might end up only using 80 cells or 60 if it weights to much.
```

---
## \#53 Posted by: macncheese Posted at: 2018-06-13T19:35:37.173Z Reads: 90

```
Did you make a 10s8p? I need a diagram for one.
```

---
## \#54 Posted by: Jedi Posted at: 2018-06-13T19:43:55.244Z Reads: 92

```
Nope, I think @Gabriel_Robinson wants to.
```

---
## \#55 Posted by: Blitz Posted at: 2019-04-19T22:44:36.545Z Reads: 57

```
[quote="b264, post:39, topic:36229"]
Some of us know how heavy it will be and want it anyway. I’m in the process of getting a 10S16P build underway. I want a 100 mile board. So if I want to ride it all day long, I can do that.
[/quote]

Any updates?
```

---
## \#56 Posted by: b264 Posted at: 2019-04-19T23:59:32.888Z Reads: 49

```
Got delayed and then canceled and then restarted again as a 10S10P

![20190415_204127|690x388](upload://tmkkP5n2VpHcSKCDiQ6ur0gnDeS.jpeg)
```

---
## \#57 Posted by: jonez Posted at: 2019-07-28T15:59:43.224Z Reads: 27

```
Hey, I'm building 10s10p could you help with any diagram, I saw you connected 2 x 5s10p, could you share dimensions also?
```

---
## \#58 Posted by: Skyart15 Posted at: 2019-07-28T16:20:54.382Z Reads: 27

```
I built a battery out of the same 10s2p packs but none had LG cells my battery was a 10s14p and I ran it at 100 motor amps and 60 battery amps, had no problems, ran great! Was a beast! Range was about 25mph at mostly full throttle doing about 32-35 mph.
```

---
## \#59 Posted by: b264 Posted at: 2019-07-28T19:58:42.393Z Reads: 24

```
Are you on the new builder forum?
```

---
