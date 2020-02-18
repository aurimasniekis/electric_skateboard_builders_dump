# What battery am I going to need

### Replies: 25 Views: 3107

## \#1 Posted by: elbari Posted at: 2016-08-30T21:58:42.579Z Reads: 227

```
i dont no anything about battery but i found motor and control. duel motor

2 x 190KV Electric Skateboard Motor 6355 
http://www.enertionboards.com/electric-skateboard-parts/190kv-electric-skateboard-motor/

Enertion Nano-X 2.4Ghz Controller   
http://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/

2x vesc standard
http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/

83 weel ithink
```

---
## \#2 Posted by: sl33py Posted at: 2016-08-30T22:17:59.938Z Reads: 228

```
usually i'd let the ESC determine batteries, but since you have VESC you have a lot of flexibility. 

So depending on the size of your deck and how much room you have to work with will help determine space for batteries and their sizes needed.

I tend to like smaller thinner batteries.  So instead of one big 6s battery, 2 x 3s in series is almost always thinner and lower profile (more ground clearance and less visible).  And since you have VESC you have the ability to do 2-3-4 batteries in series for 6/9/12s - letting you customize the power depending on your mood.  Of if you want to let a friend try it, you can simply remove one or two from series to get it down to 6s for less power/punch which might cause them to crash if unwary.

I might also suggest the venerable GT2b vs the nano.  Then later you can re-enclose in badwolf / master cho / flatline enclosure for smaller size.

GL!
```

---
## \#3 Posted by: elbari Posted at: 2016-08-30T22:24:50.613Z Reads: 207

```
thank for info:D  what is diffrence between 6s 8s 10s 12s i want atleast 1 hr of battery time
```

---
## \#4 Posted by: chinzw Posted at: 2016-08-30T22:30:11.532Z Reads: 205

```
[quote="elbari, post:3, topic:8655, full:true"]
thank for info:D  what is diffrence between 6s 8s 10s 12s i want atleast 1 hr of battery time
[/quote]

More battery time = more Amps/Hour
6s vs 10s vs 12s = the higher the more power and speed
```

---
## \#5 Posted by: racidon Posted at: 2016-08-30T22:47:19.328Z Reads: 198

```
You'll see the term

0s0p

replace the zeros with other numbers, example 10s3p     6s4p

This is a shorthand version of 10 batteries in series with 3 of these in parallel

Batteries in series increase voltage, which in turn increases power.
Batteries in parallel increase amp/hours, which in turn increases your battery time/range of your board

How does series work?
It takes multiple smaller voltage based batteries to create one larger voltage battery. A common example of this is a Car battery which is actually 6 small lead acid batteries in series. Each of these cells are just over 2 Volts each connected in series creating one 12 volt battery.
This will read in terms of the above short hand as 6s1p

Another thing to note though that a 6s using LiIon or LiPo will actually be a higher voltage as each cell is approx 4volts each.
So a 6s battery will be about  24volts

Parallel, the best analogy I can use here in relation to cars is that each P is a tank of fuel
So a 1p battery has 1 tank of fuel, a 2p battery has 2 tanks of fuel so on
So obviously a 4p battery will go almost (because of weight increase) four times as far as 1p battery

Hope this answers it all in layman's terms for you :)
```

---
## \#6 Posted by: Namasaki Posted at: 2016-08-30T22:54:45.452Z Reads: 182

```
Too many choices right?
Let's narrow it down. 
With dual Vesc and 190kv motors, 
10s battery is gonna be the sweet spot with power and speed to spare but at the same time very smooth and controllable. 
Range is usually rated by distance rather than riding time. 
Example
A space cell pro3 is 7.5 ah and should give abt 15 mile range
A space cell pro4 is 10 ah and should give over 20 mile range.
```

---
## \#7 Posted by: elbari Posted at: 2016-08-30T22:58:54.716Z Reads: 173

```
thanks man lots of good info:D
```

---
## \#8 Posted by: sl33py Posted at: 2016-08-30T23:00:07.467Z Reads: 174

```
Great breakdown @Racidon.

I'd also suggest knowing how Amp Hours relates to range.  Almost all batteries will state their mAh or Ah (milli-amp hour or amp hour) capacity.  PLUS their "c" rating (20c constant to 35c burst).  I would target a battery that is capable of around 100 Amps constant.  To get this take your 20c (example) on a 5000mAh (also = 5Ah) and 20 x 5 = 100 amps continuous, with capacity to burst to 35c or 35 x 5 = 175 amps burst.

If you draw close to the max continuous amp discharge capacity (say the full 100amps continuously) = it will either damage the battery over time, or greatly reduce the battery life (# of recharges usually).  So since my measured amp draw (using an inline watt meter) showed a peak amp discharge of 65A, i'm probably rarely above 30-40amps giving ample overhead for better pack life.

Then to figure out range you want to take your batteries Ah x voltage = Watt Hours.  So the simple 5000mAh 10s (simpler math) (nominal voltage of lipo is 3.7v per cell so 37v for 10s) would equal 5Ah x 37v = 185Wh.

Watt Hours and range - you can expect about 10Wh = 1km.  so the above 10s 5000mah / 185Wh pack would get (185Wh/10= 18.5km or 11.5mi).  Ballpark - on the flats - and not racing.  Hills, being a heavy rider, etc. will all decrease range.  Pack life too will degrade and lower your range.

It's a lot to digest - hope this helps and is understandable.

GL!
```

---
## \#9 Posted by: elbari Posted at: 2016-08-30T23:01:59.846Z Reads: 156

```
how big difrence is it between 8 10 im thinking money:O 10s is exspensive
```

---
## \#10 Posted by: elbari Posted at: 2016-08-30T23:04:35.707Z Reads: 151

```
6s3p how much will that give me
```

---
## \#11 Posted by: caustin Posted at: 2016-08-30T23:26:11.374Z Reads: 147

```
Here is an example
 Ping @barajabali though, he is custom battery master builder

 https://www.ebay.com/itm/191954555405
```

---
## \#12 Posted by: sl33py Posted at: 2016-08-30T23:27:17.848Z Reads: 152

```
it will depend on the pack.  a 6s 5000mAh = ?? Wh?  (6 x 3.7v = 22.2v)  So Ah x V = Wh.  5Ah x 22.2v = 111Wh.

the "P" for # in parallel doesn't factor in.  That's part of the capacity of the pack, and the "C" rating for continuous and peak amps able to provide.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-08-30T23:35:22.994Z Reads: 141

```
You can expect substantial increase in performance going from 8s to 10s and an increase of range.
```

---
## \#14 Posted by: elbari Posted at: 2016-08-31T00:10:26.101Z Reads: 139

```
how do i connect the vescs togehter and batery to drawings?
```

---
## \#15 Posted by: Namasaki Posted at: 2016-08-31T00:43:17.288Z Reads: 130

```
I have used 12s/5000mah Lipos 
And 10s/9000mah Li-ions
The12s gave me  12 mile range 
The 10s gave me over 20 mile range
```

---
## \#16 Posted by: elbari Posted at: 2016-08-31T00:56:28.753Z Reads: 128

```
Witch motor do u have?
```

---
## \#17 Posted by: elbari Posted at: 2016-08-31T00:57:08.461Z Reads: 124

```
What motors are the best?
```

---
## \#18 Posted by: Namasaki Posted at: 2016-08-31T04:53:06.040Z Reads: 123

```
When I was running 12s it was with Torquesboard 6355's 230kv and Torquesboard 12s Esc
With 10s I'm using Ollin Vesc's and Alien Power Precision 6355's 190kv
```

---
## \#19 Posted by: Namasaki Posted at: 2016-08-31T04:58:48.526Z Reads: 119

```
[quote="elbari, post:17, topic:8655, full:true"]
What motors are the best?
[/quote]

Imo, the best motors are the ones that are made specifically for E-boards
They Have Key ways cut in the shaft so they are designed for a pulley with shaft key and grub screws.
They are well made heavy duty motors that will perform and hold up well under the high torque demands of E-boarding.
```

---
## \#20 Posted by: sl33py Posted at: 2016-08-31T05:08:07.097Z Reads: 115

```
@elbari It really depends on your budget.

R-Spec and DIYes motors are nice but a bit more $ - keyway and longer shaft makes it easier, etc.

less expensive and work well - the hobbyking SK3's - you have to file a flat spot or keyway and some extra steps if you want the nicer wires swapped...

Also tried some aliexpress no-name motors - just watch out for the 10mm shaft (PITA).  You want 8mm for easiest compatibility w/ whats available.
```

---
## \#21 Posted by: Namasaki Posted at: 2016-08-31T05:20:06.325Z Reads: 114

```
The Alien Power motors also have 10mm shafts. Limited selection of 10mm pulleys but they are Heavy Duty!
I just ordered a set of 10mm pulleys from Alien Power when I ordered the motors. Ran them a bit and they have not loosened up. No bearing slop
```

---
## \#22 Posted by: jga Posted at: 2016-11-30T13:11:54.947Z Reads: 84

```
[quote="racidon, post:5, topic:8655"]
Batteries in series increase voltage, which in turn increases power.Batteries in parallel increase amp/hours, which in turn increases your battery time/range of your board
[/quote]
[quote="sl33py, post:12, topic:8655, full:true"]
it will depend on the pack.  a 6s 5000mAh = ?? Wh?  (6 x 3.7v = 22.2v)  So Ah x V = Wh.  5Ah x 22.2v = 111Wh.

the "P" for # in parallel doesn't factor in.  That's part of the capacity of the pack, and the "C" rating for continuous and peak amps able to provide.
[/quote]

I am a bit lost: if a 6s 5000mAh gives you 111Wh, if you put two in parallel this should give you maybe not the double but sensibly more?
Or am I just completely stupid? (which cannot be excluded...) :slight_smile:
```

---
## \#23 Posted by: DeathCookies Posted at: 2016-11-30T13:24:24.391Z Reads: 82

```
Lets clear things up:

S = cells in series --> determines voltage
mAh = capacity
C = max continous current the battery can deliver

Wh = V * Ah

6S = 6*3,7 = 22,2
5000mAh = 5Ah

6S1P 
**22,2V** (6s) * **5Ah** (1P) = **111Wh**
**22,2V** (6s) * **10Ah** (2P) = **222Wh**
```

---
## \#24 Posted by: jga Posted at: 2016-11-30T14:45:54.764Z Reads: 78

```
Perfect, that was my initial understanding.

That means if you have let's say 12 x 3,7V batteries to put together, whether you put them in S or in P will have an effect on the power you deliver (in P you will deliver less power to your motor) but not on the range.
As an example: 6S2P is equivalent to 3S4P (at 5000mAh, so 111 Wh) but in the first each pack gives 22,2V where in the second each pack gives only 11,1V.

I would then tend to prefer a high S. But I suspect there is an issue somewhere in my reasoning.
```

---
## \#25 Posted by: DeathCookies Posted at: 2016-11-30T15:39:38.921Z Reads: 70

```
No, you are completly right!

P is for range and S for power

More voltage is recommended but (nearly) everytime more expensive. So if you have the money for a high voltage ESC (like the VESC) then go for it. Your electronics will thank you for it.
```

---
