# 8s2p lipo BMS wiring?

### Replies: 4 Views: 160

## \#1 Posted by: Shaz Posted at: 2019-04-05T07:14:19.904Z Reads: 46

```
Does anyone know how to wire two 4s lipo packs into an 8s BMS? Both lipos have 5 balance leads but the BMS balancing port has 9 leads. 

Thanks
```

---
## \#3 Posted by: mynamesmatt Posted at: 2019-04-05T10:18:59.271Z Reads: 39

```
https://www.electric-skateboard.builders/search
this link worked for me
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-04-05T11:38:43.923Z Reads: 32

```
Woah it worked.

https://www.electric-skateboard.builders/search
```

---
## \#5 Posted by: olestra Posted at: 2019-04-05T15:15:31.941Z Reads: 29

```
in brief, those 5 wire leads overlap. there is always one more wire than the series count.

for an example let's show 2 2s with the leads connected for a 4s cell:

each | is a balance wire, + is positive side of battery, - is negative.

a 2s battery would have |+-|+-|  so to turn two of those into 4s |+-|+-|+-| you would combine the positive power lead of the first pack with the negative power lead of the second. you would do the same with the balance wires |+-|+-|<-this wire would combine with this wire->|+-|+-|.

If this isn't perfectly clear, then just charge each 4s by its self, with a lipo balance charger, and a parallel charge port.

Also 2 4s packs can be combined to form either a 8s1p, or a 4s2p. you would need 4 packs to achieve 8s2p
```

---
