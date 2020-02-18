# How should i start?

### Replies: 47 Views: 873

## \#1 Posted by: mylow Posted at: 2019-04-15T04:18:24.311Z Reads: 189

```
im getting a deal through a friend to buy some lifepo4 at a $1 each so i figured dam ill grab 200. im currently on a project right now with another lined up after so this will be after that. not sure what to do with these cells other than use it on an e-board. super fresh to this thing. not sure how to go about it, been doing a bit of reading and should i go all out with 4 motor 12s12p. sounds lots of fun but how should i get to that? buy each part individually or is it possible to use an existing model hopefully without battery and build my own pack.

should i get more batteries, what else should i build?
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-04-15T04:20:01.853Z Reads: 179

```
Do a bit more reading, look for other people's builds and think about parts, come back to here when you've got more of an idea about what you're getting into

Also what lipos did you get?
```

---
## \#3 Posted by: mylow Posted at: 2019-04-15T04:21:59.830Z Reads: 172

```
havent got em yet but he says they are a12326650
```

---
## \#4 Posted by: RedBaron Posted at: 2019-04-15T04:23:12.673Z Reads: 157

```
Finding an enclosure and deck to fit 12s12p and two dual or 4 single vesc is going to be a challenge. What are the dimensions of the lipos?
```

---
## \#5 Posted by: KaramQ Posted at: 2019-04-15T04:24:18.156Z Reads: 153

```
I don’t think they are lipos, aren’t they lifepo4 batteries
```

---
## \#6 Posted by: mylow Posted at: 2019-04-15T04:25:27.990Z Reads: 149

```
26mm(1.0") x 65.15 mm(2.6") and yes they lifepo4. (corrected)
```

---
## \#7 Posted by: mylow Posted at: 2019-04-15T04:30:10.346Z Reads: 143

```
since im new to this, what would be more realistic to take advantage of in my situation, money is not much of a concern as long as i build something REALLY vicious
```

---
## \#8 Posted by: Andy87 Posted at: 2019-04-15T04:37:11.710Z Reads: 133

```
If you can get batteries super cheap I would always ask myself, where they coming from and are the legit or if used, what’s there conditions.

Nothing more annoying than having shitty cells in your board. Or let’s say worst case, nothing more shitty than lightening up your whole build because somebody sold you fake cells.
```

---
## \#9 Posted by: mylow Posted at: 2019-04-15T04:38:35.919Z Reads: 128

```
from what my friend tells me they were briefly used in a prototype truck, seller gots 2 trucks full of batts.  should i get more? $1 compared to something like $9 plus shipping is such a bargain
```

---
## \#10 Posted by: ZachTetra Posted at: 2019-04-15T04:40:33.597Z Reads: 126

```
Since it will weigh like 20lbs in batteries alone, no you don't need more
```

---
## \#11 Posted by: ZachTetra Posted at: 2019-04-15T04:42:26.422Z Reads: 120

```
33lbs actually
```

---
## \#12 Posted by: mylow Posted at: 2019-04-15T04:42:51.731Z Reads: 121

```
am i going to carry this around? btw im only 145 lbs
```

---
## \#13 Posted by: Andy87 Posted at: 2019-04-15T04:43:22.826Z Reads: 121

```
[quote="mylow, post:9, topic:90574"]
$1 compared to something like $9
[/quote]

If it sound too good to be true, than most time something is wrong. But nobody here can tell you if it is like this in your case.
```

---
## \#14 Posted by: ZachTetra Posted at: 2019-04-15T04:43:24.485Z Reads: 114

```
HOLY FUCK THATS 79Kw BURST DISCHARGE
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-04-15T04:44:19.394Z Reads: 116

```
It will also go 100 miles...that is insane
```

---
## \#16 Posted by: mylow Posted at: 2019-04-15T04:44:26.321Z Reads: 112

```
4 motors can handle that right? hope it doesnt sound to dangerously fast(sarcasm)
```

---
## \#17 Posted by: ZachTetra Posted at: 2019-04-15T04:45:05.167Z Reads: 115

```
It's about 10 times as much power as a 'normal' board
```

---
## \#18 Posted by: ZachTetra Posted at: 2019-04-15T04:46:14.908Z Reads: 117

```
If you want motors to handle that power this is a good start, a group buy for custom MayTech 6880 motors (top notch quality) is open

https://www.electric-skateboard.builders/t/group-buy-maytech-6880-8mm-x-34mm-shaft-160kv-sensor-wire-2-0-jst-and-logo-or-no-logo/90313/43
```

---
## \#19 Posted by: mylow Posted at: 2019-04-15T04:46:22.132Z Reads: 113

```
i believe i read that lifepo4 can handle fairley harsh abuse compared to the other alternatives so i dont think their conditions will veer to far from what your saying
```

---
## \#20 Posted by: ZachTetra Posted at: 2019-04-15T04:50:23.207Z Reads: 111

```
Power: 3.3V (nominal voltage) * 12 (series count) * 50A (continuous amps) * 12 (parallel count) = 23,760W (5,960W per motor)

Range: 3.3V (nominal voltage) * 12 (series count) * 2.5 (capacity) * 12 (parallel count) /  18Wh/mi (generous efficiency) = 66mi on a single charge
```

---
## \#21 Posted by: mylow Posted at: 2019-04-15T04:52:19.030Z Reads: 99

```
yeah thats sounds like i could give up the car and take the board instead
```

---
## \#22 Posted by: Andy87 Posted at: 2019-04-15T04:55:45.088Z Reads: 98

```
[quote="mylow, post:16, topic:90574"]
4 motors can handle that right?
[/quote]

I see this is going through the last comments.
Just because your battery can output 1000000A it does not mean you need to use this. Your battery will just supply what you ask for. No need for special motors or what not ever.
```

---
## \#23 Posted by: ZachTetra Posted at: 2019-04-15T04:56:32.262Z Reads: 96

```
My recommendation if our want something insane without regard for cost is get 4 of the 6880 and the helical drives that are going to be out soon for the drive

Do a 13s battery to max out the voltage on the motors and ESC and 5p for the amp discharge

You'll get about 30mi on it but at least you could carry it, battery will be 11lbs and maybe another 20lbs for the rest of the board
```

---
## \#24 Posted by: Andy87 Posted at: 2019-04-15T04:57:32.959Z Reads: 89

```
The 6880 has same ratings than other 6374 motors. It’s not a better motor regarding this point.
```

---
## \#25 Posted by: ZachTetra Posted at: 2019-04-15T04:58:30.972Z Reads: 91

```
But it will last longer at max power if that's important to him, he said he wanted hella performance and I'd assume he's gonna want to go all out of he's putting this much into it
```

---
## \#26 Posted by: Andy87 Posted at: 2019-04-15T04:59:25.431Z Reads: 88

```
[quote="ZachTetra, post:23, topic:90574"]
13s battery to max out the voltage on the motors
[/quote]

Doesn’t lifepo4 have a different nominal voltage 🤔


I see a lot of FAKE news here 😂😂😂
```

---
## \#27 Posted by: Andy87 Posted at: 2019-04-15T05:00:42.701Z Reads: 87

```
No. Just no. Why should it? Yes it’s a good motor but a sk3 could rock the same power.
```

---
## \#28 Posted by: mylow Posted at: 2019-04-15T05:01:02.637Z Reads: 96

```
ur suggestions looks like an optimal setup which is awsome, tnx much, but also i believe i read that its best not to drain your batts at high c as it effects its life. wouldnt it be good idea to add some more for "p" for this case, not necessarily for performance but just battery longevity?
```

---
## \#29 Posted by: ZachTetra Posted at: 2019-04-15T05:02:40.663Z Reads: 93

```
12s with li-ion is 43.2v nominal
13s with LiFePO4 is 42.9v nominal
```

---
## \#30 Posted by: ZachTetra Posted at: 2019-04-15T05:03:54.617Z Reads: 92

```
Fair enough...all will be about 2800W from 6374 and larger
```

---
## \#31 Posted by: mylow Posted at: 2019-04-15T05:04:04.109Z Reads: 88

```
assuming your talking new condition figures, every1 is to remember these batteries are slightly used
```

---
## \#32 Posted by: ZachTetra Posted at: 2019-04-15T05:05:09.841Z Reads: 85

```
Then add another cell or two per parallel pack to account for a loss to discharge and capacity, so 6p or 7p to support 4 65A motors
```

---
## \#33 Posted by: Andy87 Posted at: 2019-04-15T05:07:35.596Z Reads: 85

```
Yes, but it’s not maxing something out. You can go 14s lifepo4 to have similar max voltage to 12s LiIon
```

---
## \#34 Posted by: ZachTetra Posted at: 2019-04-15T05:09:27.946Z Reads: 87

```
Actually 12s li-ion and 14s LiFePO4 are 50.4V at full charge, so yeah 14s would be the best 12s equivalent
```

---
## \#35 Posted by: chaka Posted at: 2019-04-15T16:15:11.360Z Reads: 80

```
> Finding an enclosure and deck to fit 12s12p and two dual or 4 single vesc is going to be a challenge. What are the dimensions of the lipos?

Not too hard to do. 12s12p dual here but I still have room for 2 more vesc's. Wheelbase is about 24 inches.

![20190321_073704|690x335](upload://lqLXBCrA5g8aqGcdJxjM1x59ZEY.jpeg)
```

---
## \#36 Posted by: RedBaron Posted at: 2019-04-15T16:24:16.852Z Reads: 76

```
That's pretty awesome! Clearance looks pretty low though. What do you use to cover the enclosure?
```

---
## \#37 Posted by: murloc992 Posted at: 2019-04-15T16:29:25.091Z Reads: 91

```
Casual ride of @chaka : 

https://media1.tenor.com/images/4dd8f7bf0e75307c130984c1ae2ea96c/tenor.gif?itemid=5627585   

I'd say he uses his balls to cover the batteries. :joy:

This looks insane.
```

---
## \#38 Posted by: Sender Posted at: 2019-04-15T16:34:55.088Z Reads: 92

```
@mylow

There might be some good stuff in here for you to read.  Happy Building!

https://www.electric-skateboard.builders/t/is-diy-esk8-right-for-you/84563?u=sender
```

---
## \#39 Posted by: J95hicks Posted at: 2019-04-15T17:30:11.240Z Reads: 85

```
I dont have the link, but depending on your stance and board. You could do a top and bottom mount battery. I saw a EMTB doing that for the same reason. So like two seperate 14s6-7p lifopo4,one top box and one bottom enclosure each going to dual can focboxs(or 2 unity's)... buuut it would be heavy AF lol. Youll get killer range and maintained power bc of the split load btw 4 motors/vesc/batteries and probably like NO sag bc ur weight... I have 12s8p 30q dual Trampa Mtb and the sag bc my weight is sad😭 I weigh 270lbs. What everybody else is saying and im pretty sure you want. Maintaned power, performance, range... if monies no issue I wouldve too.... but tbh what everyone is saying about legit batteries is true. I wasted a couple hundred on fake 30q cells. Had to re order and wait for legit cells and pay more againXD.
```

---
## \#40 Posted by: Battosaii Posted at: 2019-04-15T19:07:53.159Z Reads: 77

```
As a long time rider and an owner of a 4wd build also one of the heaviest riders here i would suggest that 4wd 12s anything is not ok for a bigginer even if you can build it properly. Its hard to handle the power, id suggest build 2 2wd boards that way you always have a back up board when one need maintenence or one breaks, its also nice to have another board so friends can ride with you.
```

---
## \#41 Posted by: chaka Posted at: 2019-04-15T21:25:47.872Z Reads: 57

```
Clearance is not too bad, the belly pan is about 1/2 inch higher than the truck hangers so anything the trucks clear will be clear of the enclosure. The belly pan is an aluminum panel bent to fit. 
![IMG_20190328_194140_390|500x500](upload://aHY3sHDYO3iAtvQwwLZDNtW0SAi.jpeg)
```

---
## \#42 Posted by: Skunk Posted at: 2019-04-15T21:39:16.694Z Reads: 52

```
God i love this build.  Just want it with two more motors lol
```

---
## \#43 Posted by: chaka Posted at: 2019-04-15T23:54:23.247Z Reads: 48

```
I will be adding a 3rd motor to the front truck for added stability. :sweat_smile:  

@Battosaii I think a first time builder can build a fairly user friendly 4wd build if they keep the top speed in check. My main concern is the high voltage power mains since they can give you a good burn if you are not careful.
```

---
## \#44 Posted by: Battosaii Posted at: 2019-04-15T23:58:25.518Z Reads: 49

```
I dunno i dont see the point of 4wd if you are going to be using conservative settings. Its alot of added complexity and weight and points of failure to not really use it to its potential seems pointless

Building 2 dual drive boards would be alot more practical for a begginer.
```

---
## \#45 Posted by: chaka Posted at: 2019-04-16T00:32:37.778Z Reads: 49

```
Efficiency is what stands out for me. A 4wd with a gear drive or direct has proven to be more efficient than a single drive or dual.  Why not stage the build and start testing with a dual but leave room for an extra set of motors?

I was also lucky enough to ride a @psychotiller 4wd at bako and it was very user friendly! way more predictable than I remember from my first single drive. Going with quad also has the upside of running motor controllers at half the norm and this greatly reduces the likelihood of malfunctions due to high currents ect...
```

---
## \#46 Posted by: b264 Posted at: 2019-04-16T00:33:58.212Z Reads: 47

```
Are they used or new?  Are you sure?
```

---
## \#47 Posted by: b264 Posted at: 2019-04-16T00:34:34.898Z Reads: 46

```
[quote="ZachTetra, post:15, topic:90574, full:true"]
It will also go 100 miles…that is insane
[/quote]

And if it's LiFePO4 it will be a cubic kilometer large and weigh sixteen tons, but last forever even in arctic conditions
```

---
