# Quad VESC with gt2b dual receiver

### Replies: 6 Views: 226

## \#1 Posted by: Andy87 Posted at: 2018-07-21T10:00:57.069Z Reads: 66

```
if i want to control 4 VESC with one remote,
what's the best way to connect them.
I thought about CAN-bus between dual VESC sitting on each site 
plus one receiver on each site.
I read that it should be possible to bind two receiver to one GT2B remote.
I wanted to connect each site (two VESCs) with an own own XT90S.
As I'll need to switch on each site after each other, also the receiver will switch on after each other. 
Can somebody tell me if that could be an issue?

I could also go by 2xCAN + Y-split, but I'm don't like the idea to route the receiver cables from one site to the other site of the deck...
```

---
## \#2 Posted by: E1Allen Posted at: 2018-07-21T10:43:26.726Z Reads: 58

```
Are you running two separate batteries?  You should be able to power the receivers separately.
```

---
## \#3 Posted by: Kubbur Posted at: 2018-07-21T10:57:10.483Z Reads: 56

```
thats a long way to route a signal cable, if you wanna go that way id use a shielded coax cable or similar

from an rc standpoint it should be possible, ive done it with taranis and two drones at the same time, you just need to bind both of the receivers to the remote
```

---
## \#4 Posted by: Andy87 Posted at: 2018-07-21T11:31:13.999Z Reads: 49

```
The receivers powered by the vescs.
There is only one battery, but two parallel outputs to each side of the board, which powers always two vescs
```

---
## \#5 Posted by: Andy87 Posted at: 2018-07-21T11:32:15.236Z Reads: 49

```
The problem with the shield where my thoughts two. That’s why I don’t like this idea and wanna go with two receiver for one remote
```

---
## \#6 Posted by: Silverline Posted at: 2018-07-21T12:44:13.489Z Reads: 43

```
You can bind 4 Gt2b receivers to one remote without problems
```

---
