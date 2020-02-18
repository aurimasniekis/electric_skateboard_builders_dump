# Help soldering battery to evolve BMS

### Replies: 20 Views: 590

## \#1 Posted by: Leo81486 Posted at: 2019-01-20T17:01:28.181Z Reads: 122

```
I bought a built battery from eboost.
He was a really busy guy, a nice pack of 10s5p made for me n just recently shipped .
But I have no idea of how to solder it onto my evolve BMS.
The balancer cable it's not in the picture .

Can someone share Info's or maybe a wiring diagram
Thank u
![20190118_213501|375x500](upload://bQ2ENFomBKlNBvr1cBVZDgSP34Y.jpeg)
```

---
## \#2 Posted by: Marsen Posted at: 2019-01-21T07:01:00.174Z Reads: 110

```
The Black lead from the battery has to be soldered to the B- on the BMS. That's the black lead sticking out of the BMS that you cut off from the old battery. Unsolder the one on the bms and then cut the black lead on the battery long enough to solder to the B- terminal. Use some of the Black wire to solder to the P- on the BMS and that goes to the T style plug used by Evolve. The red lead goes to the positive of the T style plug. Where's the power connector to the ESC gone?  You also need to solder the charging leads to the C- and the positive of the battery. You need to get some insulation on that battery, way to much exposed metal. That XT plug is very close to touching the weld strip and will make a wonderful flash and bang. Tape it up and if possible shrink wrap it.
![P-%20and%20C-|690x388](upload://bsEwhiqICEF3oPmYLbpxJAteUAl.jpeg) 
P- and C- connections. Power lead to ESC plug and charge lead to charging port.
![Power%20plug|281x500](upload://yB5ypHFIOZElgwpJ9LyUzw9VGnx.jpeg) 
T style power plug from ESC to BMS/battery. 
The red lead goes directly to the battery positive and the black to the BMS P-. The other half of the plug is wired to the ESC.
```

---
## \#3 Posted by: Leo81486 Posted at: 2019-01-21T19:18:26.281Z Reads: 94

```
What about the old 11pin plug .
We don't need those now ??
```

---
## \#4 Posted by: Marsen Posted at: 2019-01-22T00:46:55.390Z Reads: 88

```
You said the balancer cable was not in the picture. So you don't have a balancer cable for this battery then? That's a pretty basic battery you got there. Yes you need the balancer cable and plug otherwise the BMS/ESC  won't start up.
```

---
## \#5 Posted by: J0ker3366 Posted at: 2019-01-22T03:18:16.836Z Reads: 84

```
Why weren't balance leads put on it in the first place? Did the battery come assembled or did you have to join p groups?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-01-22T03:22:56.633Z Reads: 80

```
Seems someone made A huge mistake :wink:
```

---
## \#7 Posted by: PickSix24 Posted at: 2019-01-22T03:48:23.277Z Reads: 79

```
Ya you’re gonna need some balance leads buddy
```

---
## \#8 Posted by: b264 Posted at: 2019-01-22T11:04:27.760Z Reads: 74

```
Yes, you will need the balance leads for that to work
```

---
## \#11 Posted by: Leo81486 Posted at: 2019-01-22T13:57:48.839Z Reads: 64

```
Eboosted made this .
I sent a DM in the first place . But no reply so far
```

---
## \#12 Posted by: J0ker3366 Posted at: 2019-01-22T18:08:41.088Z Reads: 62

```
@Eboosted mind helping your customer out...
```

---
## \#13 Posted by: Eboosted Posted at: 2019-01-22T18:48:07.645Z Reads: 65

```
@J0ker3366 thanks for tagging me.

Hello Leo:
Sorry, I must have missed your DM, but here I'm replying you.

This is how you should connect the your BMS to the battery.

![image|690x388](upload://yvTicWInN9rhUDpkrBmFH7zcdZK.jpeg) 

You don't need balance leads on the battery as the nickel strips are exposed and easy to access for solder the balance cable wiring.

Unfortunately I'm not familiar with the Evolve V3 BMS, you will have to see which one corresponds to B0 and which to B10 and solder in the same order as it was on the original battery.

@lee
According to the picture you posted I see Evolve uses a red wire in one side of the jst connector, so I'm "guessing" that's the B10 not the B0, can you confirm this?

@Leo81486 
What I'd suggest is to follow the red wire on the old Evolve battery pack and see where it was connected, if it was soldered on B10 or B0.
```

---
## \#14 Posted by: Sebike Posted at: 2019-01-22T19:17:24.493Z Reads: 59

```
Please edit or remove this picture as it's not correct and misleading. b1 is supposed to be connected where you put b10, and b10 should be where you put b1 and so on. (if evolve uses the same bms wiring as almost all other bms's) There is no b11, but maybe a b0.
```

---
## \#15 Posted by: Leo81486 Posted at: 2019-01-22T19:53:25.778Z Reads: 55

```
To be honest, I have no clue at all 
Or els I would of so everything myself .
The most knowledge part were the wiring n soldering skills for it to be functional properly.

May I send u back for wiring the balancer 
I thought that's what I was looking for in the beginning.
```

---
## \#16 Posted by: Eboosted Posted at: 2019-01-22T20:17:31.485Z Reads: 54

```
@Leo81486

Don't worry I'll guide you through all steps so you have you battery up and runing in no time, I'll contact you by DM and I'll help you out until the end :sunglasses:
```

---
## \#17 Posted by: Leo81486 Posted at: 2019-01-22T20:33:56.332Z Reads: 54

```
Hell ya .
Knew u were great .
Thx
```

---
## \#18 Posted by: LEE Posted at: 2019-01-22T22:17:26.674Z Reads: 53

```
![IMG_9945|666x500](upload://ppw1TxxuqePG5mxUBblqe3vRyOz.JPG) 

I misrecognized figures and + -.
As you pointed out, it is B10 → B0.
I searched for this image on Google. Probably the same type EVOLVE BMS.
```

---
## \#19 Posted by: Eboosted Posted at: 2019-01-22T22:27:22.250Z Reads: 51

```
That's great @lee, @Leo81486 please upload a picture of your bms and bms connector, so I can tell you what should be the wiring instructions
```

---
## \#20 Posted by: Marsen Posted at: 2019-01-23T06:09:25.017Z Reads: 48

```
The red positive wire is on the left of the BMS plug, as you can see in the picture from LEE. Wire up working your way around the battery using eboosted's picture till you get to the black negative. This is B10 down to B0 going on the picture. The plug only fits one way. That is the correct bms for evolve in this picture. I always check the voltages after wiring up and before plugging in, if you flip the plug over you will see the terminals through the locking lugs. With a multi-meter measure the voltage between the terminals. B0 - B1 3.6V,  B0- B2 7.2V, B0-B2 10.8V Etc. The voltage will vary from these reading slightly depending on the state of charge of the cells but you are looking for a consistent increase in voltage with each time you move to the next cell group on the plug. This will ensure the cell groups are in the correct order. Most cells arrive in a storage charge state which is about 3.6V. Full charge will be 4.1V - 4.2V.
Be careful when measuring the first two pins (B0 and B1) these are very close together so don't touch the multi-meter probes together when touching the terminals. BANG if you do.
I have just ordered plugs and wiring looms made up for evolve BMS's (500) which will make this sort of thing a lot easier but they will be a few weeks from delivery.
```

---
## \#21 Posted by: Eboosted Posted at: 2019-01-26T16:30:43.616Z Reads: 41

```
Here is more easy-to-follow procedure, I also sent it to you via PM

1. Unplug the bms connector:
2. Wire the balancing wires in this order:

[img]https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/f/1/f1e4cf60b2b5043530ba39861f4a7b2648af4958_1_690x388.jpeg[/img]

![image|603x500](upload://3lTqRUqSW2DMOE36lxh9A0DIiw.jpeg) 

3. Charging wire should already be installed if you are using an Evolve BMS

4. Reconnect everything back again
```

---
## \#22 Posted by: Leo81486 Posted at: 2019-01-26T17:53:12.494Z Reads: 34

```
![20190126_125236|374x500](upload://htXqZ3ryW9RxjNsufF5dpda64b7.jpeg)
```

---
