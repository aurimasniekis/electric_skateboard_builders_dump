# VESC won&rsquo;t work - dim blue blinking light SOLVED

### Replies: 9 Views: 738

## \#1 Posted by: rittohassi Posted at: 2017-10-13T12:14:28.313Z Reads: 122

```
Hi guys! 

I recently made an electric skateboard using the VESC from esk8.de. Everything worked fine, until I had to disassemble the whole thing, so I could put some new 18650 cells, as the old ones were not that great. I got my new 10s4p pack, and I put everything back together - but now the VESC won't boot correctly. When I turn it on, it takes around 6-9 seconds before I even get a feedback from the VESC, and the only thing I'm getting is the BLUE LED blinking dimly. It won't connect to the BLDC Tool, and neither the green or red led ever turns on. I would say I'm pretty confident with the BLDC tool and VESC, but this problem I can't  figure out. Do you have any ideas on what to do? 

(The motor won't turn ofc, because the VESC can't boot)
```

---
## \#2 Posted by: rittohassi Posted at: 2017-10-13T12:32:29.768Z Reads: 118

```
UPDATE: Fixed it. Turns out my BMS wasn't working properly. Gonna leave the topic here though.
```

---
## \#3 Posted by: sodniwe Posted at: 2018-06-09T01:58:20.191Z Reads: 70

```
@rittohassi  I'm currently having the same issue and think it's an issue with my BMS as well.  What was the issue you resolved with your BMS?
```

---
## \#4 Posted by: Falcon87407 Posted at: 2018-06-09T02:47:42.805Z Reads: 65

```
I have this same issue after my friend hit the brakes hard.  I'm just going to replace the bms, any suggestions for a good bms for a 10s 4p. 18650s
```

---
## \#5 Posted by: rittohassi Posted at: 2018-06-09T10:00:58.642Z Reads: 59

```
My problem was that one of the resistors on the BMS was fried, so I just bought a new one. It turns out that the resistor was enough to resist the power to the VESC, but not completely tho. imo just buy a new BMS.
```

---
## \#6 Posted by: Falcon87407 Posted at: 2018-06-11T15:20:48.757Z Reads: 51

```
I've been using these $20 BMS from amazon.  The first time I fried it because the charger port I bought had the reversed polarity on the cables and I mistakenly did not check it before installing... Learned from my mistake, got a second and it seemed to have fried when a friend hit the brakes too hard and I'm guessing my settings for Regen were incorrectly set.

https://www.amazon.com/gp/product/B074WZL5NF/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1

Any suggestions, is this a good BMS or is there better ones out there for a 10s 4p?
```

---
## \#7 Posted by: telnoi Posted at: 2018-06-11T15:24:57.488Z Reads: 42

```
Use such a bms only for charging, not discharging.
```

---
## \#8 Posted by: Falcon87407 Posted at: 2018-06-11T15:28:10.412Z Reads: 39

```
That's a good tip actually.  I have read some posts on this, but I really didn't see the difference in the wiring on this.  I will double check those posts and try to wire it up for charge only for the next one.
```

---
## \#9 Posted by: sodniwe Posted at: 2018-06-11T17:22:02.466Z Reads: 32

```
@rittohassi How were you able to tell that a resistor was bad on the BMS?
```

---
