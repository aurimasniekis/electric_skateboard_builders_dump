# Need help with batteries!

### Replies: 44 Views: 380

## \#1 Posted by: Winkelmann Posted at: 2019-04-15T14:48:10.695Z Reads: 94

```
So Im currently planning my project and after some feedback, I've realised that im a bit unsure about the batteries...

I was initially looking at building a 10s2p back with 25r, then someone recommended to build it with 30Q instead so I started looking into it more!

I'm looking to build a board that has 10-15 km range.

I've also looked into building with [Samsung 30T](https://liionwholesale.com/products/samsung-30t?variant=38001589841) Instead since they can handle more current. I also looked at 40T but they seem a bit too expensive...

Im going to build a single 6355 190KV setup with orangatang wheels geared for 30-35 km/h

I've also heard that the batteries play a role in the regenerative breaking...

Can someone please help me to clarify this?

What battery pack are a good choice for a decent range and won't overheat when I pull a lot of current at acceleration and hills!

I'm going to use this as a general commuter for university.

Here is a link to my [project](https://www.electric-skateboard.builders/t/project-board-better-than-boosted/89825?u=winkelmann)
```

---
## \#2 Posted by: Mich21050 Posted at: 2019-04-15T14:51:57.358Z Reads: 88

```
All of your questions are common knowledge so let me give you a small advice:\
![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/6/0/60234b9d5bf554c1bd0e8298f2587e940689c288.gif)

Credit to @Sn4pz
```

---
## \#3 Posted by: Simnol Posted at: 2019-04-15T14:52:56.480Z Reads: 82

```
Your voltage will determine your speed.
Your nominal amp will determine your range.
Your maximum current ( amp output ) will determine your acceleration.
Thats a simplified explanations from my understanding.
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-04-15T14:54:13.491Z Reads: 80

```
Search for a calculator on the forum, it will tell you how your battery and motors will do...but 10s2p 25R will match your motor and take you 20km
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-04-15T14:55:52.050Z Reads: 74

```
https://calc.3dservisas.eu/?PdDNCsIwEATgd8lZJDU_Va-xeFICgr3bHiJYG-ix-O7uTKK3b5fNbJJVPUJSR_V6zm-1keIqhdl68RJu4kaTUbijAuR1aZ9QmWrM2GJmNsKMDAOUSZ7LEV1L_YJziXIkmp78Bw0p1KQhdaK9Ju84zqVTqJMTr92yF2fYkph0uoyyjbVjv_CRLXy-wI7ssQ3fMGLbQavPFw==
```

---
## \#6 Posted by: Winkelmann Posted at: 2019-04-15T14:57:34.954Z Reads: 70

```
Yeah, ive might have been a bit unclear in my text sorry,

Those things i undernstand, what are your thoughts about building a 10s2p with 30Q or the same pack with 30T?

Will i get alot better breaking with the 30T or will de 30Q be good enough?

so the peak pulse current would be 40 amps < 5 sec, that would mean i could pull 80 amps for a short time and lets say that my motor would be rated for max 80 amps... do you think im having to small of a margin and would i have problems with overheating?

Im turning to you guys since i dont have any experience with this

Cheeers!
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-04-15T14:58:24.696Z Reads: 65

```
No 6355 will be rated for 80A, the best (MayTech and their equivalents) are 65A max

Go look at the data sheets for all the cells but 30Q will do 20A continuous and 25R will to 30A continuous...you can burst at 1.5x continuous in general, 3p 30Q or 2p 25R will have similar performance
```

---
## \#8 Posted by: Winkelmann Posted at: 2019-04-15T15:01:16.884Z Reads: 62

```
Okay right, so that would mean that 25R would work.. what are your thoughts on which ones to go with?

but do you have any experience with the breaking side?

any battery config that would be better?

30T might be a little overkill?
```

---
## \#9 Posted by: skatardude10 Posted at: 2019-04-15T15:02:14.622Z Reads: 56

```
Add gearing into the mix. Voltage + gearing determine top speed and acceleration.
```

---
## \#10 Posted by: skatardude10 Posted at: 2019-04-15T15:03:25.949Z Reads: 56

```
As a 25r rider, go with 30Q. If you want less capacity but higher amp output (25r says 20A, but sag is INSANE) go with VTC5A, cheap on nkon.
```

---
## \#11 Posted by: ZachTetra Posted at: 2019-04-15T15:04:27.642Z Reads: 55

```
If it's a campus board then 10s2p 30Q will be enough...you don't need all that power.  I am running dual cheap 350W hubs on a 10s2p of fake 30Q cells and it's definitely enough to get around...I get about 8 miles in each day and charge it every night

Don't get 25R...but VTC5 is a good option if you want hella startup torque
```

---
## \#12 Posted by: ZachTetra Posted at: 2019-04-15T15:05:17.266Z Reads: 52

```
Shit I was thinking about the VTC5 specs then
```

---
## \#13 Posted by: Winkelmann Posted at: 2019-04-15T15:05:43.633Z Reads: 52

```
Right that is also one thing why @brenternet  recommended the 30T, so the sag would be less..

why VTC5A?
```

---
## \#14 Posted by: ZachTetra Posted at: 2019-04-15T15:06:15.775Z Reads: 45

```
Vtc is 2.6Ah 30A continuous
```

---
## \#15 Posted by: skatardude10 Posted at: 2019-04-15T15:07:43.499Z Reads: 47

```
VTC5A are rated at 35A, or 25A conservatively and sag is considerably less than 30Q even, with capacity and cycle life better than 25R. 25Rs sag a TON more than even 30Q let alone VTC5A with less capacity than any of them. I got my VTC5As from nkon for [$3.60](https://ru.nkon.nl/sony-us18650vtc5a-flat-top.html) a cell after taking shipping into account.
```

---
## \#16 Posted by: Winkelmann Posted at: 2019-04-15T15:08:22.684Z Reads: 46

```
Im not an extremly experienced longboard rider, i just want to have a nice smooth board that have the power! If you look at my project topic you can see what my plans are, i wanted to build a dual drive but since i dont have that money now i might just add another motor later
```

---
## \#17 Posted by: Winkelmann Posted at: 2019-04-15T15:09:35.712Z Reads: 49

```
If I remember correctly nkon cannot ship to sweden where i live! :confused:
```

---
## \#18 Posted by: skatardude10 Posted at: 2019-04-15T15:09:48.908Z Reads: 47

```
Nooooooo!!!! Damn. Such good prices.
```

---
## \#19 Posted by: ZachTetra Posted at: 2019-04-15T15:10:46.464Z Reads: 47

```
IMR batteries?
```

---
## \#20 Posted by: skatardude10 Posted at: 2019-04-15T15:11:13.276Z Reads: 47

```
Look at prices then. 25R cells aren't horrible. If you find they are significantly cheaper for you, they aren't a bad option, especially if your going to pay over double for 30Q for example.
```

---
## \#21 Posted by: Winkelmann Posted at: 2019-04-15T15:12:12.902Z Reads: 42

```
Yeah, i remeber that one of those could so thats not a problem!

The biggest one i have atm is that i cant decide if i should go with 30T or 30Q or now the VTC5, haha
```

---
## \#22 Posted by: ZachTetra Posted at: 2019-04-15T15:13:03.330Z Reads: 40

```
Boosted uses cells in the same size as the 30T if that helps :joy:
```

---
## \#23 Posted by: Winkelmann Posted at: 2019-04-15T15:13:14.911Z Reads: 35

```
Nope i was wrong NKON can ship to sweden
```

---
## \#24 Posted by: Winkelmann Posted at: 2019-04-15T15:14:26.431Z Reads: 37

```
HAHA then its settled!

No but do you think there is huge advantages with 30T_
```

---
## \#25 Posted by: Komamtb Posted at: 2019-04-15T15:14:42.442Z Reads: 36

```
As a owner of 12s5p made from 25r I will second the sag issue.
```

---
## \#26 Posted by: Winkelmann Posted at: 2019-04-15T15:15:49.688Z Reads: 38

```
Okay thanks!

So then 25R is off the table :confused:
```

---
## \#27 Posted by: ZachTetra Posted at: 2019-04-15T15:16:52.825Z Reads: 38

```
What is most important to you? (pick 2 or 3)
- cost
- range
- power
- lifetime
- weight

And which sites can ship to you..this is very important
```

---
## \#28 Posted by: Winkelmann Posted at: 2019-04-15T15:21:34.214Z Reads: 36

```
Okay so i want to build a battery for a bit over 100 dollars (BMS included) but excluding cables

Range im happy with 10-15 km

power i want it to be able to handle my motor to its best performace, might add another motor after summer when ive earned some money if im not happy with single motor setup.

is there huge differences in lifetime?

for the speed im happy with a 10s setup

i want to build quite light board which is why im aming for 2p max 3p

IMR cannot i think, everything else shouldnt be a problem
```

---
## \#29 Posted by: ZachTetra Posted at: 2019-04-15T15:25:14.785Z Reads: 33

```
A BMS will set you back about $20 so $80 for 20 cells, go to any reputable site and sort by around $2 a cell and 20A continuous and more than 2000mAh
```

---
## \#30 Posted by: Winkelmann Posted at: 2019-04-15T15:26:13.804Z Reads: 34

```
okay so im ready to spend 150 dollars, did some calculations haha


What are your thoughts on 30T compared to VTC5 and 30Q?
```

---
## \#31 Posted by: ZachTetra Posted at: 2019-04-15T15:26:53.078Z Reads: 35

```
lol, it be like that sometimes...best bet for light use but often is 30Q

https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html
https://eu.nkon.nl/rechargeable/18650-size/sony-us18650vtc5-flat-top.html
```

---
## \#32 Posted by: Winkelmann Posted at: 2019-04-15T15:29:08.546Z Reads: 31

```
but since im only doing a 2p setup ill prop experience more sag?
```

---
## \#33 Posted by: ZachTetra Posted at: 2019-04-15T15:29:55.734Z Reads: 32

```
Yeah...the 30Q has more sag, the VTC5 has less capacity and lifetime
```

---
## \#34 Posted by: Winkelmann Posted at: 2019-04-15T15:30:41.684Z Reads: 31

```
So maybe the 30T wont be such a bad idea?

https://eu.nkon.nl/rechargeable/21700-20700-size/samsung-inr21700-30t-3000mah-35a.html

and im also confused about the regenerative breaking, the numbers doesnt tell me anything haha... breaking on 2p 30Q vs 2p 30T? any idea?
```

---
## \#35 Posted by: ZachTetra Posted at: 2019-04-15T15:35:26.042Z Reads: 32

```
30T will have less lifetime...only 200 cycles when 30Q and VTC5 have 300...but it would be 1p

Regen brakes are kinda dependent on how many charging amps each cell can take but you can go way over since its a short time so all will work
```

---
## \#36 Posted by: Winkelmann Posted at: 2019-04-15T15:37:08.766Z Reads: 33

```
Oh... okay that is a big difference... maybe the 30T is off the table too then, dont know where you found that but is it the same with 40T?
```

---
## \#37 Posted by: ZachTetra Posted at: 2019-04-15T15:38:19.347Z Reads: 32

```
you could probably get 300 cycles from a 2p of 30t but its heavy/big/expensive
```

---
## \#38 Posted by: AlanZhou Posted at: 2019-04-15T15:38:19.499Z Reads: 31

```
Nah 30t is 21700, A123 Cells are 26650

A123 cells has a constant discharge of 70A (NEW Version
```

---
## \#39 Posted by: Netoa Posted at: 2019-04-15T15:38:30.520Z Reads: 32

```
Or you can ask Michal here https://endless-sphere.com/forums/viewtopic.php?f=31&t=61608 I'm buying 50 VTC5A for just under 150 euros shipped to France.
```

---
## \#40 Posted by: ZachTetra Posted at: 2019-04-15T15:38:46.621Z Reads: 30

```
my bad...thats massive
they hurt for capacity though
```

---
## \#41 Posted by: AlanZhou Posted at: 2019-04-15T15:39:26.144Z Reads: 28

```
People say who you can do 1p your wrong...

Just throwing it out there

Cause 12s1p a123 puts out 39.6v and 70a
```

---
## \#42 Posted by: Winkelmann Posted at: 2019-04-15T16:05:15.150Z Reads: 27

```
What are your thoughts on a battery setup? what are you using? are you happy?
```

---
## \#43 Posted by: AlanZhou Posted at: 2019-04-15T18:17:52.433Z Reads: 27

```
I'm using lots of battery.

10s5p, 12s3p, 10s2p, 2 5000mah 5s lipos.

And a 13s10p comming up
```

---
## \#44 Posted by: Dirt_Bag Posted at: 2019-04-16T07:16:59.672Z Reads: 20

```
Get a 10s3p or 4p and thank me later. Your best cell choice is

30q
Sony vtc5 or vtc5a
Lg hg2

These are all great cells at a good price point. Your batteries lifespan will be half of what it should if you are straining a 10s2p. Its cheaper now, but it won't be in half a year when you need a new one.

I can build you a 10s battery with sony vtc5 cells if you want. They are 25-30a 2600mah.
```

---
