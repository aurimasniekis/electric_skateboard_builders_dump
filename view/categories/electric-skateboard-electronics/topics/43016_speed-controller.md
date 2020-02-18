# Speed controller

### Replies: 13 Views: 691

## \#1 Posted by: madlemgw Posted at: 2018-01-07T00:42:12.047Z Reads: 145

```
I’m new to the electric board community and I’m looking to build a electric board to use on my golf course. The commercial boards that are out there use dual 1000w motors. I’m thinking for an application like this I would need a speed controller but not sure exactly what they do?  The commercial ones have preset speeds 1-4 and not sure if that is what it used for?  I’m open to any advice anyone has.
```

---
## \#2 Posted by: Jammeslu Posted at: 2018-01-07T00:48:37.751Z Reads: 143

```
You need to read up alot more. The thing you are looking for is a esc/vesc/focbox they all do the same thing in the end
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2018-01-07T00:49:19.289Z Reads: 141

```
a speed controller essentially takes a PWM signal from a receiver and voltage from your battery and uses it to essentially fire certain electromagnets in your motor at certain times based on the desired speed and the relative positions and angular velocities of the rotor and stator. This is necessary to make a BLDC (BrushLess DC) motor turn. We use BLDC motors because of their high speed/torque to weight/size ratios.

For electric Skateboards, we use the VESC, which was purpose-built for eboards and has a lot of useful software features, as well as being very customizable and having really really high power throughput
```

---
## \#4 Posted by: PredatorBoards Posted at: 2018-01-07T00:49:31.097Z Reads: 132

```
Lol 1000W motors are tiny. Get 2 sensored 5060 motors. Read up about VESCs and what they do. The one I suggest you buy is the FOCBOX.
```

---
## \#5 Posted by: Dariks Posted at: 2018-01-07T00:51:19.480Z Reads: 122

```
For golf coarse applications you are looking for a mountain board.
```

---
## \#6 Posted by: madlemgw Posted at: 2018-01-07T00:54:56.268Z Reads: 117

```
Thank you for the information. This is what I’m looking to build. <img src="/uploads/db1493/original/3X/5/6/563ef9ed3fad2ae84fbe6baad9890939e2797b80.jpeg" width="391" height="499">
```

---
## \#7 Posted by: madlemgw Posted at: 2018-01-07T01:58:20.942Z Reads: 105

```
I just need to figure out how!
```

---
## \#8 Posted by: DavidBanner Posted at: 2018-01-07T02:00:17.656Z Reads: 104

```
oh man I could have so much fun winding up golfers with an MTB :slight_smile:
```

---
## \#9 Posted by: JdogAwesome Posted at: 2018-01-07T07:44:00.702Z Reads: 88

```
I think the best your gonna be able to build without some advanced engineering is gonna be an electric mountain board like [THIS](https://www.google.com/search?q=electric+mountainboard&rlz=1C1GCEA_enUS773US773&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjLvZvjrMXYAhUs7YMKHWKfD6UQ_AUIDCgD&biw=1536&bih=734#imgrc=_). And its still gonna cost you around ~$2K, if thats still cheaper and you dont want to build one yourself you could get one from [Kaly.nyc](https://www.kaly.nyc/) he makes some awesome boards. 
<img src="/uploads/db1493/original/3X/7/6/76373860de29fb00c7d01ebaba063031149209eb.jpg" width="666" height="500">
```

---
## \#10 Posted by: madlemgw Posted at: 2018-01-07T13:38:06.748Z Reads: 57

```
Thank you for the link. I’m hoping to stay in the $1000 range. The board in the pictures runs $5k retail. I’m not looking for something with speed 10-12 mph tops. Will need to have some power to get me (215 lbs) and 25 lbs golf bag up and down the hills. I would say miles wise it would be 10 or less. A golf round lasts about 3.5 hours and it would be a lot of stop and go riding.
```

---
## \#11 Posted by: Bor.inc Posted at: 2018-01-07T13:53:37.164Z Reads: 54

```
If you want to build something like that you can also look into brushed DC motors, they are cheaper but bigger, but for that vehicle I think its small enough! and the controll unit is cheaper
```

---
## \#12 Posted by: madlemgw Posted at: 2018-01-07T14:05:43.173Z Reads: 51

```
Specs of the board:

Underside:

• 30 Ah Quick release Lithium NMC (LiNiMnCoO2) battery (completes 18+ holes) + (9 holes) *
• 30 Ah spare battery option – don’t miss out on another rental again
• Fast Charger: 1.5 – 3 hours
• Low impact 10inch turf tire ( low ground force pressure impact of < 8psi )
• Dual 1000w whisper quiet high torque brushless motor with soft-start
• Custom computerized mapped software
• Automatically engaging parking break for slopes and inclines
• Tuned front bush and dual suspension springs
• Water resistant computer management system
• Rear suspension limiters
```

---
## \#13 Posted by: GrecoMan Posted at: 2018-01-07T14:13:19.891Z Reads: 45

```
Nobody uses lithium NMC in boards.  use lipos.

a lot of that sounds custom and unacheivable without equipment and cad knowledge
```

---
