# \[NEED HELP\] Picking battery for first built (36v)

### Replies: 20 Views: 1892

## \#1 Posted by: Proxy Posted at: 2017-11-29T23:45:40.978Z Reads: 165

```
Part list:
Vesc: TORQUE ESC VESC
Motor: TORQUE Motor 6355 190KV
Wheels: Orangatang Kegel 80 mm
Motor Pulley: 16t
Wheel Pulley: 36t

According to CalcRC and other sources, it says the ideal voltage for this built is 36v battery. I need some help picking batteries because i know nothing about electronics. What battery should i get? How many packs? Any sources to find out how to put them "in series"? Also, let me know what you guys think about my built and if there are any adjustments i can make. Thanks a lot.
```

---
## \#3 Posted by: rojitor Posted at: 2017-11-30T10:59:05.616Z Reads: 160

```
36v is the nominal voltage. The real fully charged voltage is 42v.
Search "10s battery" most builds have 10s 2-4p li ion or two lipo bricks 5s in series.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-12-01T03:06:41.506Z Reads: 148

```
[quote="Proxy, post:1, topic:39711"]
i know nothing about electronics.
[/quote]


You might want to consider buying a pre-made 10s battery pack.
From your list it looks like your getting your motor and Vesc from  
They also sell ready made battery packs.
Matter of fact, they sell everything you need to build a complete E-board.
Since this is your first build, a one stop shop might be the simplest solution.
```

---
## \#5 Posted by: Proxy Posted at: 2017-12-01T03:54:11.856Z Reads: 137

```
what does it mean by fully charge and nominal voltage ? Will my board use 36v or 42v? How do i know if a battery's fully charge limit?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-12-01T04:38:09.073Z Reads: 129

```
Lithium batteries both Lithium ion and Lithium polymer  register 4.2v per cell at full charge. As they deplete, their voltage drops.
3.6v is nominal for Lithium ion cell also known as Lion or Li-ion
3.7v is nominal for lithium polymer cell also known as Lipo

2.5v is minimum voltage for Lion batteries although I would not go below 2.8v with them
3.0 is minimum voltage for Lipo batteries although I would not go below 3.4v with them.

So for example, a 10s Lipo pack would be 42v full charge, 37-38v storage charge, and in need of recharging at 34v
```

---
## \#7 Posted by: DEEIF Posted at: 2017-12-01T04:48:27.468Z Reads: 119

```
Nominal is discharged which is 3.6 volts a cell so in your matter if your doing 10s*p your nominal voltage would be 3.6 x 10 = 36 volt nominal voltage and charged voltage would be 4.2 volts a cell so that would be 4.2x10= 42 volts 
I am about to finish my first build and I got all my parts from diy electric skateboard and every thing seems to be working on my tests I just need a deck and I’m perfect
I went over kill and went single 6355 190kv, Vesc, 12s4p battery from them, 90mm Flywheels and 16/36 gearing the stuff from there is in my opinion high quality I’m not sure about the Vesc but the rest seems pretty good
```

---
## \#8 Posted by: Proxy Posted at: 2017-12-01T04:52:09.489Z Reads: 105

```
thanks for the info. It seems like our build are very similar.
```

---
## \#9 Posted by: DEEIF Posted at: 2017-12-01T04:53:17.048Z Reads: 109

```
Yeah the problem I’m having with the deck is because I want to be able to upgrade to sixshooters later
```

---
## \#10 Posted by: Proxy Posted at: 2017-12-01T17:39:59.042Z Reads: 95

```
I plan on getting the "ZIPPY Compact 5000mAh 5S 25C Lipo Pack". What do you think? Should it be alright or will it be overpowered?
```

---
## \#11 Posted by: DEEIF Posted at: 2017-12-02T02:58:49.718Z Reads: 87

```
I say go for like 30c or more
```

---
## \#12 Posted by: ARetardedPillow Posted at: 2017-12-02T07:30:44.649Z Reads: 76

```
6355 isnt overkill haha :joy:
```

---
## \#13 Posted by: ARetardedPillow Posted at: 2017-12-02T07:32:00.835Z Reads: 72

```
25c is fine, but I would definitely go for higher, and if you're getting a 5s lipo, make sure to get 2 and connect them in series.

I would look into this post, its a goldmine of information http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#14 Posted by: DEEIF Posted at: 2017-12-02T14:02:20.538Z Reads: 70

```
@ARetardedPillow
I meant that I’m going 12s4p with a single drive
```

---
## \#15 Posted by: Namasaki Posted at: 2017-12-02T15:41:37.203Z Reads: 71

```
[quote="Proxy, post:10, topic:39711, full:true"]
I plan on getting the "ZIPPY Compact 5000mAh 5S 25C Lipo Pack". What do you think? Should it be alright or will it be overpowered?
[/quote]

I used those batteries on my 12s build. They worked ok but did sag a bit and got a little puffy after a few cycles. 

I’m currently using Turnigy 60C hard case Lipos in a 10s configuration. 
The have minimum sag and after a year, they’re holding up very well. 

So I recommend 60C or higher when using Lipos. 
The higher discharge Lipos usually have a higher charge rate as well which is an advantage when considering regen braking.
```

---
## \#16 Posted by: ARetardedPillow Posted at: 2017-12-02T16:25:24.986Z Reads: 63

```
Thats really really overkill.
```

---
## \#17 Posted by: DEEIF Posted at: 2017-12-02T16:26:34.266Z Reads: 64

```
Haha told u
```

---
## \#18 Posted by: GrecoMan Posted at: 2017-12-02T16:33:42.707Z Reads: 62

```
LOL 12s4p with single drive does NOT equal overkill 😂

i’m not even overkill and i’ve got 10s6p on a single drive...
```

---
## \#19 Posted by: DEEIF Posted at: 2017-12-02T16:35:35.870Z Reads: 61

```
Lol
10 char
```

---
## \#20 Posted by: Proxy Posted at: 2017-12-05T07:06:45.694Z Reads: 53

```
Does the " c rating" also double if you link 2 batteries in series? Ex 30c + 30c = 60c?
```

---
## \#21 Posted by: Namasaki Posted at: 2017-12-05T11:56:10.641Z Reads: 49

```
No the C rating does not change. Only the capacity changes.
How ever, doubling capacity does double discharge capability.
```

---
