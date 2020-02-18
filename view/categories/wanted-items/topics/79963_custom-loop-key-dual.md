# CUSTOM LOOP KEY ( dual )

### Replies: 20 Views: 698

## \#1 Posted by: hyperIon1 Posted at: 2019-01-05T08:59:07.837Z Reads: 238

```
We are going to offer custom loop keys 
With a X,Y,Z custom lengths 
X- input from battery 
Y- loop( key ) 
Z- output (single or duel) 
Custom connectors T60 or T90 (in/out) 

$10 for single T60
$15 for duel T60
$15 for single T90
$18 for duel T90 
All loops are T90 ( off set ) anti spark connectors
T90 duel 
![image|690x381](upload://rF5RA2bCSI6EulXp7LKTFP2F5HE.jpeg) ![image|690x454](upload://vCgyTs7zSjxNta2XYa5acrOvwbr.jpeg) 
T60 duel
![image|665x430](upload://uhCeymkvl89gNyrSZUuyAKYTjNj.jpeg) ![image|690x421](upload://9xMn2P9n5djMs0f8YeQ3QdGYOxb.jpeg)
```

---
## \#2 Posted by: bigben Posted at: 2019-01-05T09:09:12.218Z Reads: 221

```
These look very nicely made. I would always use the male part as the key though. Then you don't have the two male live prongs exposed on the board when the board is off, if you see what I mean?
```

---
## \#3 Posted by: Arzamenable Posted at: 2019-01-05T09:10:37.990Z Reads: 220

```
I feel you, but how does that mount? Pics please.
```

---
## \#4 Posted by: bigben Posted at: 2019-01-05T09:16:30.144Z Reads: 212

```
It's ugly! But the other way is still only clean when you don't have it plugged in. When you plug it in, there's still the key sticking out at an angle wherever you put it. Unless you make it like the folding one that showed up on the no words thread.
```

---
## \#5 Posted by: totalgeek9224 Posted at: 2019-01-05T09:18:20.283Z Reads: 203

```
An advantage to this (female as key)  is that if the resistor were ever to blow, you could easily just get another without having to disassemble your board
```

---
## \#6 Posted by: hyperIon1 Posted at: 2019-01-05T09:18:43.728Z Reads: 187

```
True. I thought of that. It can work both ways or be done both ways. One will limit your mounting area 
The possibility of the two prongs touching or making contact is highly unlikely with out help It’s true with smaller prong type connectors. 
It would be preference and how it’s going to be mounted.
```

---
## \#7 Posted by: hyperIon1 Posted at: 2019-01-05T09:21:45.238Z Reads: 176

```
I am working on a close ( none wire loop ) 
I’m going to have some 3D thumb drive style handle printed and glue the connector into it versus a wire loop
```

---
## \#8 Posted by: bigben Posted at: 2019-01-05T09:39:42.863Z Reads: 166

```
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5852
This is the cleanest I've seen. (still not my preference way around..)
```

---
## \#9 Posted by: b264 Posted at: 2019-01-05T10:08:19.620Z Reads: 163

```
[quote="bigben, post:2, topic:79963, full:true"]
These look very nicely made. I would always use the male part as the key though. Then you don’t have the two male live prongs exposed on the board when the board is off, if you see what I mean?
[/quote]

I would use the female part as the key
```

---
## \#10 Posted by: hyperIon1 Posted at: 2019-01-05T10:13:13.848Z Reads: 159

```
![image|375x500](upload://sDDRBKrQjCC4Fnm5ubYupPw7Ev2.jpeg) ![image|375x500](upload://pH53zVgfFqCDUrKgmBmKQn4wXzD.jpeg)
```

---
## \#11 Posted by: hyperIon1 Posted at: 2019-01-05T10:15:36.192Z Reads: 157

```
Just looking for a better way, low profile
```

---
## \#12 Posted by: totalgeek9224 Posted at: 2019-01-05T10:28:06.001Z Reads: 155

```
For sure the cleanest
I wish we could see some other nice and easy implementations of something like this 
Or that maybe someone would spend time designing a hardware cutoff like the XT90S but purpose built for esk8 like we have been trying to do with antispark switches
```

---
## \#13 Posted by: hyperIon1 Posted at: 2019-01-05T10:40:02.069Z Reads: 157

```
It's just so hard to find a good switch.
I'm tempted to go back to the luna switches but they burn out just as fast. It seams flipsky switches have issues with 12s batteries.
the Vedder switch is just outdated.
So far the mini momentary switch the unity has works well.
seems that integrated soft switches in the esc are the way to go.
or loop key
```

---
## \#14 Posted by: b264 Posted at: 2019-01-05T10:42:38.034Z Reads: 152

```
[quote="hyperIon1, post:11, topic:79963, full:true"]
Just looking for a better way, low profile
[/quote]

https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204/104?u=b264
```

---
## \#15 Posted by: b264 Posted at: 2019-01-05T10:47:16.921Z Reads: 151

```
[quote="hyperIon1, post:13, topic:79963, full:true"]
It’s just so hard to find a good switch.
...
the Vedder switch is just outdated.
So far the mini momentary switch the unity has works well.
seems that integrated soft switches in the esc are the way to go.
or loop key
[/quote]

There is an actual reason for that ;-)

https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=b264

When the switch is integrated into the ESC it can be on the other side of the power filter capacitors, which has the effect of allowing it to NOT burn out, but also has the side effect of allowing the capacitor's leakage current to slowly chew away at your battery while the board is turned off.  It's like there is a tiny piece you can't turn off.  Unless they have a digital switch with separate precharge resistor & FET, which I doubt.
```

---
## \#16 Posted by: hyperIon1 Posted at: 2019-01-05T10:51:21.005Z Reads: 131

```
we have noticed this effect when testing on the bench with switches, its a bounce effect or backwash and the switch bleeds at low volts
```

---
## \#17 Posted by: briman05 Posted at: 2019-01-05T13:57:37.401Z Reads: 119

```
LHB uses a 300a switch that he has had success.
```

---
## \#18 Posted by: amazingdave Posted at: 2019-01-05T14:10:43.257Z Reads: 112

```
The fatboy switch has an inrush resistor so I’m hoping it keeps working for longer than its competitors....
```

---
## \#19 Posted by: hyperIon1 Posted at: 2019-01-05T20:23:40.720Z Reads: 107

```
the fat boy switch is impressively large, I haven't seen LHB switches yet. I would be interested in its size.
with all the upgrades and tight spaces its difficult to find a good fit
```

---
## \#20 Posted by: deucesdown Posted at: 2019-01-05T21:04:36.478Z Reads: 102

```
[quote="hyperIon1, post:13, topic:79963"]
It’s just so hard to find a good switch.
[/quote]

I've been thinking about this for a while. Something like this:

https://www.ebay.com/itm/Battery-Disconnect-Knife-Blade-Switch-Top-Post-Heavy-Duty-Terminal-Cut-Off-NEW/323569470729

With a precharge resistor on a momentary switch. Mount it topside near the rear truck. I'm gonna do it, one day soon.

Hm maybe SPDT knife switch, so it can lock in open position...
```

---
