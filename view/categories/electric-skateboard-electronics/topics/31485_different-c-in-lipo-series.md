# Different &ldquo;C&rdquo; in lipo series

### Replies: 18 Views: 1455

## \#1 Posted by: Samuele00 Posted at: 2017-08-25T19:29:09.416Z Reads: 140

```
I have to put in series 3 lipo from 3s 5000mah turnigy. I already have one and have a 30/40 A discharge and I have to take two from hobbyking but are available and discounted those 25c is a problem?
```

---
## \#3 Posted by: SilentException Posted at: 2017-08-25T20:04:51.753Z Reads: 135

```
Yes it can be a problem because of internal resistances you will probably end up with very unbalanced pack after every discharge. Combine only same cells in series.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-08-25T20:05:15.250Z Reads: 134

```
You really need to match C rating or else your packs will not sag evenly neither will they drain evenly.
```

---
## \#5 Posted by: Hardwiring Posted at: 2017-08-25T20:39:41.747Z Reads: 126

```
@Namasaki  on a similar note, is it correct with large mah battery you can have a lower c? I.E.  5000mah 20c approx equal to 10000mah 10c in its ability to supply amps?
```

---
## \#6 Posted by: Samuele00 Posted at: 2017-08-25T20:57:50.176Z Reads: 114

```
Thanks you so much
```

---
## \#7 Posted by: Namasaki Posted at: 2017-08-25T20:58:45.594Z Reads: 111

```
Forget the math. 
They are not really the same
bottom line, don't mix different batteries if you want to do it right. 
I would not even mix different brands with same C rating and capacity. 
You can't count on a Zippy 25C 5ah being the same as a Turnigy 25C 5ah
Don't mix brands, C ratings or capacity
```

---
## \#8 Posted by: Samuele00 Posted at: 2017-08-25T21:02:19.445Z Reads: 101

```
I thought that for little difference would not change
```

---
## \#9 Posted by: Hardwiring Posted at: 2017-08-25T21:28:16.001Z Reads: 95

```
Yup agree on not mixing and matching, really nothing good comes from it, it's not money saving it's the kind of cheap that means you end up paying twice. 
I was actually just engaging in a bit of casual thread hijacking as the original question had been succinctly answered. I come from a quadcopter building background, I know that bigger mah battery require lower C to give the same kick. I'm rolling around on 10s 13000mah (18650's) and I keep thinking at this kind of level, the real C requirement is much less than the guys rolling 5000mah, C being proportionate in nature. 
 I only ask cus you seem to be one of those folks who actually has a clue🤣 I think I remember a YouTube video by a guy called Bruce (from the RC community) saying stuff about incorrect battery choice and people paying to much and carrying unnecessary weight because we don't understand C. I could just have dreamed it TBH.
PS and back on original topic... I also wouldn't mix old and new batteries, bad Juju
```

---
## \#10 Posted by: deucesdown Posted at: 2017-08-26T02:22:42.509Z Reads: 77

```
Dissenter here! I've been researching this because I'm in the same situation. If you understand what's happening it's fine.

* stay under C rating of lowest rated pack
* stop discharging before lowest pack is empty
* don't bulk charge, use a balance charger

If you can't do all these annoying things every time, it' no bueno.

And as namasaki said, the packs will probably diverge more over time. But these lipos live short and dangerous lives, no? like 100 charge cycles?

As in all dangerous things, before proceeding, don't listen to some guy on the internet, check for yourself.



Supporting internet evidence (some old timers saying it's fine if...):

https://www.rcgroups.com/forums/showthread.php?2279260-using-Lipos-with-Different-C-rating-in-series

https://www.rcgroups.com/forums/showthread.php?1629926-Mixing-lipo-packs-of-different-capacities-in-series

https://www.rcgroups.com/forums/showthread.php?1347277-Mixing-C-rating-batteries
```

---
## \#11 Posted by: deucesdown Posted at: 2017-08-26T03:45:09.722Z Reads: 62

```
I reread the original post. If I were you, I would go up in quality, not down. So 40/50c packs or better.
```

---
## \#12 Posted by: lowGuido Posted at: 2017-08-26T04:23:55.859Z Reads: 61

```
yes that is true.
```

---
## \#13 Posted by: Samuele00 Posted at: 2017-08-26T09:20:08.536Z Reads: 59

```
Ah okay okay, then I'll wait for the right ones, but do they really have so few recharge cycles?
```

---
## \#14 Posted by: Samuele00 Posted at: 2017-08-26T09:21:55.528Z Reads: 57

```
Ah do you have a solution to figure out the charge of a 9s? At home i have car testers with buzzer but they arrive up to 8s
```

---
## \#15 Posted by: deucesdown Posted at: 2017-08-26T14:34:34.277Z Reads: 54

```
Nothig good. BMS would be easiest but I have trust issues. 

Scared to bulk charge lipos.

probably gonna do a quick release hatch and complicated wrIng harnesses, and a parallel charging board.
```

---
## \#16 Posted by: Deckoz Posted at: 2017-08-26T14:52:06.236Z Reads: 53

```
I would not run packs that 

-aren't the same manufacturer
-aren't the same rated capacity
-aren't the same C or discharge rating,
-aren't new together(ie no old pack new pack combos)

See cells have internal resistance that changes depending on all of the above, even the same pack charged vs not charged will have different IRs. Mismatched paralleled cells with different IRs will cause strain on the lowest IR pack, as the higher IR pack will resist giving its magical juices. This will in the long run kill good cells.

Always match packs, always match packs by health/age. Good luck
```

---
## \#17 Posted by: Blitz Posted at: 2018-01-13T15:26:44.278Z Reads: 39

```
Turnigy owns zippy i think, Lol

Could you use same style Zippy batteries But different S count in series?
and charge in seires like 2+3s in balance charger, mod the balance cable into 5s.
I guess the Question is Can you run same batteries with different voltage's?
```

---
## \#18 Posted by: GrecoMan Posted at: 2018-01-13T15:35:20.963Z Reads: 40

```
different voltages =/= same batteries
```

---
## \#19 Posted by: Namasaki Posted at: 2018-01-13T16:17:36.692Z Reads: 37

```
As @Deckoz stated before.  
When you put 2 battery pack in series, your simply turning 2 packs into 1 pack with higher voltage. 
What is important is that the 2 packs are same brand, same capacity, same C rating and same age. 
And the internal resistance of each pack’s cells should be close as possible for balancing.

Over a year ago I bought 15 Turnigy hard packs 2s 5ah and 60/120C. They all had internal resistance of around 2 milliohms per cell which is very low. 
5 milliohms or less is good for Lipos. 
As they age, the internal resistance increases. 
That’s why you shouldn’t pair old packs with new packs.
```

---
