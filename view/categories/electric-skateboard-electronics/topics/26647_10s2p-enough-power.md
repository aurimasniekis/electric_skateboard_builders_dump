# 10s2p enough power?

### Replies: 10 Views: 3547

## \#1 Posted by: ATMorris Posted at: 2017-07-03T01:27:14.229Z Reads: 303

```
Hello everyone, I've got a bit of a dilemma here. For my current (unbuilt) setup, I've got:
Batteries: Samsung 18650 25r  ---> 2 packs of 10 in series   --->  5ah at 36V with 40A continuous output
Motor: 200kv 2300 (max) watt brushless (to be used in mono drive)
BMS: 40A continuous
Belt Drive: 16 tooth to 48 tooth
Wheels: 83mm

I'm debating whether I should build a second battery pack, putting me up to 10s4p. As is, do you think 10s2p is enough power to move me around? I'm relatively light at 65kg, but I'm concerned as to whether this setup is sufficient to get me up hills. I'd love some input on the issue. I can also thrown in more info if necessary. Thanks!
```

---
## \#2 Posted by: Decdog Posted at: 2017-07-03T02:15:33.763Z Reads: 296

```
10s2p and 10s4p will have the same power, but 10s4p will have double the range
```

---
## \#3 Posted by: Jinra Posted at: 2017-07-03T02:52:12.395Z Reads: 290

```
10s2p would not have the same power as 10s4p. 4p effectively gives double power to 80A continuous. His BMS is limited to 40A continuous, but it will still give double the power for bursts.

You should not put 2 packs of 10 for 10s2p, you should do 10 packs of 2. Otherwise, you'll need a BMS for each pack. You should go for 4p to minimize voltage sag.
```

---
## \#4 Posted by: ATMorris Posted at: 2017-07-03T05:21:04.593Z Reads: 261

```
I appreciate the input and quick reply. From what I've seen, 10s BMS boards rated for 80A tend to be about six times the price of a generic 40A version. Do you reckon I could connect the two 40A BMS boards in parallel, having a common charging input and discharging output? It would essentially be two identical 10s2p packs with individual BMS boards wired in parallel.
```

---
## \#5 Posted by: Jinra Posted at: 2017-07-03T05:33:44.775Z Reads: 246

```
I don't think that would work, but I'm not sure. You could always bypass discharge on your bms. That's what i do for my builds.
```

---
## \#6 Posted by: ATMorris Posted at: 2017-07-03T06:58:31.648Z Reads: 236

```
I'll certainly have to look into that further, thanks for the knowledge :)
```

---
## \#7 Posted by: IsTalo Posted at: 2017-07-04T23:51:39.536Z Reads: 193

```
Parallel do not increase the Mah, increases the C-Rating, but if you do the calculations C-Rating*(Mah*2) is the same as (2*C-Rating)*Mah, so thats is why we say that is doubles the range (Experts, correct me if I'm wrong, plz)
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-05T01:06:23.238Z Reads: 186

```
Parallel directly increases mah **and** discharge potential. More discharge doesn't mean more range, more voltage and mah do.
```

---
## \#9 Posted by: IsTalo Posted at: 2017-07-05T01:22:21.198Z Reads: 179

```
Oh, fine, now I understood it
```

---
## \#10 Posted by: ATMorris Posted at: 2018-06-18T06:09:25.842Z Reads: 108

```
It's lit!!
```

---
