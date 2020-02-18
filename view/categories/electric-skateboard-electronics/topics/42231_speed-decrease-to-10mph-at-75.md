# Speed decrease to 10mph at 75%

### Replies: 6 Views: 346

## \#1 Posted by: mgertner Posted at: 2017-12-29T20:25:18.010Z Reads: 119

```
I noticed that there is a very large decrease in speed as i ride my board. My top speed is around 21-23 mph and like a 15-16 mile range, however after I ride maybe 2 miles (87%), it slows down to 16-17 mph. And after 4 miles (80%) down to 13 mph. And after 5 mies (78%)  it's down to <11 mph. AndI'm not sure whats causing this. Could be a setting in the VESC? Or maybe the batteries are shot? And it can't be the BMS because its only wired for charging.
Well thanks in advance for reading!
```

---
## \#2 Posted by: dg798 Posted at: 2017-12-29T20:26:14.116Z Reads: 114

```
Check you cutoffs in the bldc tool
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-12-29T20:28:23.700Z Reads: 112

```
sounds like batt cutoffs are set too high in BLDC Tool
```

---
## \#4 Posted by: mgertner Posted at: 2017-12-29T20:45:48.668Z Reads: 97

```
yup that was it! Thanks!
```

---
## \#5 Posted by: Kug3lis Posted at: 2017-12-29T23:43:22.237Z Reads: 61

```
But set accordingly not like 1V... Because I smell voltage sag problem
```

---
## \#6 Posted by: Deckoz Posted at: 2017-12-30T00:25:02.466Z Reads: 48

```
Yea I was either gonna say

-temps
-sag
-cutoffs set high
```

---
