# First BMS bypass help needed please and thank you!

### Replies: 17 Views: 511

## \#1 Posted by: Danny414 Posted at: 2018-07-22T17:42:50.784Z Reads: 132

```
![battery%20layout|375x500](upload://xjDyXPzQRsEvr07OPAH6wqjD1oN.JPG)

Trying to do a bms bypass soooo I’m assuming I don’t use P- if I want to bypass I should use N- terminal instead?

B- terminal wire to negative side to group 1

N- terminal wire to negative xt90 
N- terminal wire to negative charging port

Positive xt90 wire to positive side on group 10 and connect the positive charging port wire to this wire 

10 little wires coming out of the bms should connect and match to the positive side of each group in order 10, 9, 8, 7, etc..

Is this correct??

Thanks!
```

---
## \#2 Posted by: Sebike Posted at: 2018-07-22T18:04:55.464Z Reads: 116

```
Look what I found using search :smiley:
https://www.electric-skateboard.builders/t/small-bestech-bmss/25819/47?u=sebike
```

---
## \#3 Posted by: Danny414 Posted at: 2018-07-22T18:35:42.305Z Reads: 112

```
I did research before asking Sebike and found all different answers.. thats why I asked on here.. thanks for the reply... so from what your saying 

B- wire to negative side to group 1

P- wire to negative charging port 

Positive xt90 wire to positive side on group 10 and connect the positive charging port wire to this wire

Negative xt90 wire to negative side on group 1

10 little wires coming out of the bms should connect and match to the positive side of each group in order 10, 9, 8, 7, etc..

???
```

---
## \#4 Posted by: Sebike Posted at: 2018-07-22T20:35:49.181Z Reads: 104

```
The "little wires" are for balancing and yes, they are connected between each p-pack (as in the SuPower wiring diagram). The 10th one on the battery positive. 

If you by xt90 mean an xt90s anti spark plug, that's connected on either the positive or the negative battery wire going to the vesc as seen in the diagram.

![DSC_0236-01|690x388](upload://rML4Sah6AVrdTSC7XZqe0OGuOgI.jpeg)
```

---
## \#5 Posted by: Danny414 Posted at: 2018-07-22T20:48:41.181Z Reads: 87

```
Awesome! You are the man with the game plan! lol Thanks bro
```

---
## \#6 Posted by: mynamesmatt Posted at: 2018-07-22T22:49:30.095Z Reads: 77

```
isn't that a 60a bms?
```

---
## \#7 Posted by: Danny414 Posted at: 2018-07-22T22:53:20.136Z Reads: 76

```
No it is a 30a.. http://www.batterysupports.com/36v-37v-42v-10s-30a-10x-36v-lithium-ion-lipolymer-battery-bms-p-265.html

I purchased the smaller one to save money and going to bypass discharge
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-07-22T22:56:01.986Z Reads: 75

```
aha okay, was gonna say why you wouldn't just use it normally hahhaha
this is mine:
![20180715_224716|666x500](upload://6o28dmrozAjNWtt2ag31qLsQxFf.jpg)
```

---
## \#9 Posted by: Danny414 Posted at: 2018-07-22T23:05:58.822Z Reads: 79

```
pssst I wouldn't even know how to set it up normally either.. this is literally my first battery build.. and im new to building.. but I've learned a lot in a short time.. i can make enclosures now and I’m learning batteries.. I've already built a board and working on a another![image|666x500](upload://yUP4wvFNzHgpRMDuwTUC1hPLgHI.jpeg)
![image|666x500](upload://R1doWrZyclNuEVrxQTaeVrcAC2.jpeg)![image|666x500](upload://mMwh86LeG0FW5KIEphM7s5uMMJF.jpeg)
```

---
## \#10 Posted by: Danny414 Posted at: 2018-07-22T23:24:54.880Z Reads: 71

```
Hey one more quick questions if thats cool.. since im doing the bypass the gauge of the wire that is coming out of the B- terminal doesnt need to be 10awg correct? I can use smaller gauge wire to connect it to the negative wire?

Thanks again bro!
```

---
## \#11 Posted by: mynamesmatt Posted at: 2018-07-22T23:30:33.805Z Reads: 68

```
that little board looks awesome!! congrats g
```

---
## \#12 Posted by: Danny414 Posted at: 2018-07-22T23:32:26.068Z Reads: 66

```
Thanks! This is what the battery im making is for.. im fitting a 10s4p on the jet spud deck.. thats why the battery looks like that in group 9 and 10
```

---
## \#13 Posted by: Sebike Posted at: 2018-07-22T23:40:04.264Z Reads: 64

```
Correct. Make sure it'll be able to handle whatever charging current you are going to go with.
```

---
## \#14 Posted by: mynamesmatt Posted at: 2018-07-22T23:45:20.682Z Reads: 65

```
how much did the jet spud set you back and whereabouts are you located?
```

---
## \#15 Posted by: Danny414 Posted at: 2018-07-23T02:14:21.002Z Reads: 64

```
The deck itself was $85 I think. I’m in Milwaukee, WI. Hey another quick question.. the little positive wire that comes out of the bms that I have to solder to each positive group.. so let’s say group 2 positive that is connected to group 3 that is negative... do I have to cover it up with kapton tape to prevent the solder end from positive group 2 from touching the negative end of group 3?
![image|375x500](upload://y4dvctT4m9VSjCRu4wgUrM2l9T5.jpg)
```

---
## \#16 Posted by: mynamesmatt Posted at: 2018-07-23T02:37:45.829Z Reads: 65

```
Probably not a bad idea, cover anything you have doubts about in kapton tape. I'm in Sydney Australia. How much has the entire build set you back?
```

---
## \#17 Posted by: Danny414 Posted at: 2018-07-23T23:31:51.810Z Reads: 51

```
Not sure.. $85 deck, $320 motor controllers, $250 motors, $40 on/off button, $60 remote, $250 battery, $200 motor mounts, $50 pulleys/belts, $10 enclosure, $175 wheels.. $160 trucks.. maybe $1650ish.. I might not use the evolve trucks and motor mounts on this build and use them for another landyachtz evo build im going to make to sell.. so might be able to knock off a few hundred.. crazy how it all adds up so quick
```

---
