# 2a Charger Is Taking Longer To Charge Battery Than Expected?

### Replies: 7 Views: 490

## \#1 Posted by: deverewb Posted at: 2017-08-07T15:35:53.401Z Reads: 74

```
I recently changed my 10s board from charging with an Imax B6 charger to charging with a BMS. I picked up a 42v 2a charger from ebay. And one major thing I've noticed is that it takes way longer to charge than it should. The battery pack on my board consist of 2 5s 5000mah batteries connected in series, both wired up to a BMS. Now, if the charger is sending 2a into the board, then shouldn't the board take 2.5 hours to charge (since 5ah/2a = 2.5)? Instead it takes 5 hours. Can someone explain what's going on? I'm so very confused.

Happy to provide any photos or links if anyone can help me figure this out :slight_smile:
```

---
## \#2 Posted by: SilentException Posted at: 2017-08-07T15:39:21.670Z Reads: 71

```
What BMS? It balance charges at the very end of charging process and some BMS have really low balance charge current.
```

---
## \#3 Posted by: Bloop Posted at: 2017-08-07T15:41:37.454Z Reads: 69

```
Or maybe your ebay charger is not actually 2A.
```

---
## \#4 Posted by: deverewb Posted at: 2017-08-07T16:04:05.618Z Reads: 65

```
http://www.ebay.com/itm/Balance-BMS-PCM-21A-w-Temp-Switch-for-10S-36V-37V-Li-ion-Li-Po-battery-10S21W001/321790774602?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2055119.m1438.l2649

I actually only wired up the battery to it, not the charger. Is that a problem? (B-,B1,...,B10,B+)
```

---
## \#5 Posted by: deverewb Posted at: 2017-08-07T16:04:52.839Z Reads: 60

```
http://www.ebay.com/itm/42V-2A-Adapter-Charger-Two-wheel-Self-Balanced-for-36V-Li-ion-Lithium-Battery/142353186501?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160908131621%26meid%3D540a25cfcb0d474eb7e4f81476246ca7%26pid%3D100678%26rk%3D2%26rkt%3D4%26sd%3D371996513753&_trksid=p2481888.c100678.m3607&_trkparms=pageci%253A54c8058b-7b89-11e7-85c8-74dbd180faa7%257Cparentrq%253Abd6bc1ae15d0abc02cfa2a54fffd1752%257Ciid%253A1

This is it, I really hope I didn't get ripped off :sweat_smile:
```

---
## \#6 Posted by: jmasta Posted at: 2017-08-07T16:08:29.187Z Reads: 55

```
Your charger only outputs 2A when there is high enough voltage differential. As your battery voltage gets closer to full voltage, the actual charge current decreases. At near full capacity it is going to be less than 1A. Cutoff is usually around 500mA for most chargers 

Install a power meter and see for yourself
```

---
## \#7 Posted by: deverewb Posted at: 2017-08-07T16:09:46.586Z Reads: 54

```
Oh OK, that makes sense, thanks for clearing that up for me.
```

---
