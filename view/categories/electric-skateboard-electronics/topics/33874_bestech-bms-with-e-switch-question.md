# Bestech BMS with e-switch question

### Replies: 6 Views: 505

## \#1 Posted by: karma Posted at: 2017-09-24T19:51:13.081Z Reads: 131

```
I have just made a spotwelded 10S4P with Samsung 30Q pack witha Bestech BMS with an e-switch.
I am using a normal SPST Switch for the BMS  and when the e-switch cables makes a closed circuit the pack shows 34,4V. When it is off it shows around 29 or 32V. Is this normal? I would assume the voltage to be 0 on the battery output. How is it an on/off switch if it is still able to power stuff?
```

---
## \#2 Posted by: willpark16 Posted at: 2017-09-24T19:58:05.442Z Reads: 129

```
Same thing happened to mine I was thinking it was a bad batch
```

---
## \#3 Posted by: mmaner Posted at: 2017-09-24T20:08:57.220Z Reads: 126

```
I've seen that before onto besttech bms's and a BMS I use from eBay for discharge only. The problem usually goes away after you put a load on the battery pack.
```

---
## \#4 Posted by: Silverline Posted at: 2017-09-24T20:09:48.116Z Reads: 124

```
Its normal, if you have no load on your P- You need some loade, to pull the fet. down..
```

---
## \#5 Posted by: karma Posted at: 2017-09-24T20:23:04.445Z Reads: 118

```
Ah okey! Thanks for the info I'll test it out tomorrow and set the problem to solved.
```

---
## \#6 Posted by: karma Posted at: 2017-09-26T19:52:22.186Z Reads: 89

```
The problem was solved by adding the load, it is pulled down to 0V after around 2-3S.
```

---
