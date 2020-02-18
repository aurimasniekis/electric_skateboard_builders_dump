# BMS/antispark switch recommendations?

### Replies: 17 Views: 1213

## \#1 Posted by: michaelcpg Posted at: 2016-10-09T06:22:47.440Z Reads: 216

```
I'm currently using the 50A BMS that came with my original Enertion space cell but it's likely going to be too big for my new Vanguard deck so I'm looking to replace it with a small BMS just for charging my 10S4P 18650 pack and letting my VESCs and a fuse handle voltage/current regulation. I'm also after an anti spark switch so that I can charge my board with my laptop style charger and not have to worry about removing an XT90S connector to turn my board off.

I've had a look at various websites for small BMS's but would appreciate if someone would be able to make a recommendation for one that they've found to be reliable :) 

I've seen that @torqueboards and @chaka have options available as far as switches go but I'm wondering if there's differences between their functionality that I may not know about? @chaka's Vedder switch looks to include an integrated battery fuse which is handy as it makes for one less extra component I need to think about fitting somewhere else. Other than that, are there any other differences between the two that're worth noting?

Cheers :)
```

---
## \#2 Posted by: VladPomogaev Posted at: 2016-10-09T06:29:54.597Z Reads: 209

```
Hi! Just a shameless plug I guess; I'm designing a switch right now! It's pretty much the same as Torque Boards', but I'm going to sell it for much cheaper. Comes with a sexy blue LED button ;) 

If you wanna go with theirs but save a few bucks... 

http://currentcontrolsystems.com/2016/10/01/designing-a-4-4kw-power-switch-for-vesc/
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-10-09T06:36:54.725Z Reads: 204

```
Cheers man I'll have a look :) When do you expect them to be available by?
```

---
## \#4 Posted by: whitepony Posted at: 2016-10-09T08:03:14.900Z Reads: 194

```
im very interested too! the alienpowerswitch failed twice now for me, torqueboards runs stable, but too expensive with shipping and customs!
```

---
## \#5 Posted by: Blacksheep Posted at: 2016-10-09T08:35:10.494Z Reads: 181

```
When are you going too sell it?
```

---
## \#6 Posted by: Bender Posted at: 2016-10-09T08:35:20.616Z Reads: 176

```
I'm too am hoping @VladPomogaev new one works too 

Well I just had a torqueboard anti spark fail
After very little use, I'm hoping it was bad Mosfets and that the replacement will hold up

Also Chaka's doesn't have a fuse
He skips the fuse to get around the 40amp limit till his new design is in production
```

---
## \#7 Posted by: michaelcpg Posted at: 2016-10-09T09:10:49.790Z Reads: 166

```
Would you mind explaining what you're referring to in regards to the 40A limit?
```

---
## \#8 Posted by: Bender Posted at: 2016-10-09T11:35:44.221Z Reads: 167

```
40 amp is the highest amp rating of the style of fuse that was designed to fit on the PCB.
```

---
## \#9 Posted by: michaelcpg Posted at: 2016-10-09T11:56:25.113Z Reads: 167

```
Do you know what current the switch itself is able to handle?
```

---
## \#10 Posted by: Bender Posted at: 2016-10-09T13:44:01.692Z Reads: 160

```
I don't have that info
But I'm curious too
```

---
## \#11 Posted by: VladPomogaev Posted at: 2016-10-09T22:03:57.310Z Reads: 149

```
Well the thing is, I technically have them now. I already have the PCBs and the buttons and the rest of the components. The problem is, I wanted to increase the current limit and lower the amount of heat produced, so I decided to buy some more expensive MOSFETs, which will be here in a couple of weeks at least :( 

It basically means the difference between being able to barely run two motors, and being able to run two motors at full power without any cooling or heatsinking.

As always, each switch will be hand-made and each component will be hand-tested (especially the MOSFETS which I am buying in bulk). I'll also make a video tutorial/timelapse like I did for my smartphone remote.

Also, is a fuse a critical part of a switch? I don't think that there are many benefits to having a fuse to be honest.
```

---
## \#12 Posted by: michaelcpg Posted at: 2016-10-09T22:09:56.002Z Reads: 141

```
Would definitely prefer to wait for better quality MOSFETs personally :)
I don't really see having an integrated fuse as a big deal, can always have a separate one in the battery circuit. Just more of a nice to have to save a bit of space I think
```

---
## \#13 Posted by: VladPomogaev Posted at: 2016-10-09T22:16:07.325Z Reads: 140

```
Oh yeah I bet! I have never used a fuse in any of my builds, on the switch or otherwise, but I think it's generally a good idea.
```

---
## \#14 Posted by: michaelcpg Posted at: 2016-10-09T22:19:48.111Z Reads: 143

```
After seeing videos of batteries shorting/ending up in a thermal runaway, I don't think I would ever even think about building a battery without a fuse :p
```

---
## \#15 Posted by: TarzanHBK Posted at: 2016-11-04T14:54:06.154Z Reads: 124

```
this sounds really good.
-i´m going to build a 80a dual beast
-i want this blue button switch and don´t like these SDPT switches which you have to use in a vedder antispark.

some updates?
```

---
## \#16 Posted by: VladPomogaev Posted at: 2016-11-23T07:06:27.100Z Reads: 114

```
<img src="/uploads/db1493/original/3X/2/2/22a609ac50c5b1c933a4afe4c9396e44fe76352c.jpg" width="690" height="460">

Yup! Better late than never, the new MOSFETs arrived. I just gotta test my design out and hopefully put them up on my store. (Woops used wrong MOSFETs for picture)

Cheers, Vlad
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-11-23T20:03:21.202Z Reads: 102

```
I've got some coming too, as soon as the PCBs arrive i'm going to make 10 of them and post them here. Should be within a week or so. They're basically fuseless Vedder switches, v1.3 with 75v mosfets. 

https://www.instagram.com/p/BLl6ZZtAihf/?taken-by=longhairedboy

I've been testing them in my own board and i've used them in a couple of customer boards now so i'm going to start selling them on my site. They seem to hold up very well and don't seem to interfere with braking. 

List price will be around $35 and they'll be equipped with XT60s and a detachable SPDT rocker switch. I'm planning to donate some money back to Vedder on every sale.
```

---
