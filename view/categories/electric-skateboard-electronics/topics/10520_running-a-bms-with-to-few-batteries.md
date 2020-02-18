# Running a BMS with to few batteries?

### Replies: 11 Views: 1780

## \#1 Posted by: B4Me Posted at: 2016-10-02T18:36:52.999Z Reads: 145

```
Hi
As an electronic engineer this is properly a stupid question.. but I will try anyways, as some may have tried my problem on a real BMS..
I started using zippy 3s 8000mah lipo packs, and have two of them.. but soon I'll change to a VESC, therefor I would like to bumb up the cell count a little with an extra pack..
This will result in me having a 9S setup...
Most BMS circuits I have seen are for 6, 8, 10, 12S.. Never 9S
But is it possible to use a 10S BMS on 9S, I am ONLY interrested in balancing, NOT discharge protection, therefor I will bypass the BMS while driving, but I need the balancing function
```

---
## \#2 Posted by: IDVert3X Posted at: 2016-10-02T18:49:54.012Z Reads: 141

```
Sorry, it won't work. Basicaly because you would have to connect the last cell to the balance lead instead of the terminal that it is supposed to go and that is not going to work.
Go with 12S and change motor KV / gearing ratio.
There is no BMS for 9S because it's not a standard value. 10S is tho.
```

---
## \#3 Posted by: Pantologist Posted at: 2016-10-02T19:26:42.080Z Reads: 136

```
Just order a 9S battery pack from bestech.

http://bestechpower.com/333v9spcmbmspcbforli-ionli-polymerbatterypack/
```

---
## \#4 Posted by: 2-alex-2 Posted at: 2016-10-02T19:51:53.464Z Reads: 127

```
https://www.ebay.co.uk/itm/221809130907  That would be ok for charging but not for discharge only 21a so not enough. Only other option would be to get three 3s bms and link them all together some how.
```

---
## \#5 Posted by: B4Me Posted at: 2016-10-02T20:03:49.412Z Reads: 122

```
The thing is.. I would like to keep my two batteries, so 10S is not an option :-/
isnt 12S to high for VESC :frowning: ?
Was looking at this one :
[http://www.ebay.co.uk/itm/Battery-Protection-BMS-PCB-Board-for-10-Packs-36V-Li-ion-Cell-Max-40A-w-Balance/301605144140?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D39012%26meid%3D4045398bfd5747c7be4a1150592e4689%26pid%3D100005%26rk%3D5%26rkt%3D18%26mehot%3Dpp%26sd%3D401184874132](http://www.ebay.co.uk/itm/Battery-Protection-BMS-PCB-Board-for-10-Packs-36V-Li-ion-Cell-Max-40A-w-Balance/301605144140?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D39012%26meid%3D4045398bfd5747c7be4a1150592e4689%26pid%3D100005%26rk%3D5%26rkt%3D18%26mehot%3Dpp%26sd%3D401184874132)

It seems like its a "dumb" circuit, only measuring over each cell and regulating this cell (if over 4,2V)
so if it works, then I will loose over charging protection but still balance :)
```

---
## \#6 Posted by: IDVert3X Posted at: 2016-10-02T20:57:39.906Z Reads: 109

```
12S is fine for VESC. Just make sure you have right motor to go with that voltage.
```

---
## \#7 Posted by: B4Me Posted at: 2016-10-02T23:24:53.356Z Reads: 103

```
I have a 6355 200kv motor from Alien Power systems
```

---
## \#8 Posted by: IDVert3X Posted at: 2016-10-03T06:02:50.202Z Reads: 89

```
That might work, just use higher gearing ratio. You can find ideal values using calc.esk8.it
```

---
## \#9 Posted by: B4Me Posted at: 2016-10-03T07:02:23.174Z Reads: 85

```
Using it already :slight_smile:
But would you advice going with 6s or 9s on the vesc with my motor and like 16/36 gearing (76mm wheels)
```

---
## \#10 Posted by: IDVert3X Posted at: 2016-10-03T07:08:31.768Z Reads: 82

```
Really depends on the speed you want to achieve.
Just remember that on 6S your speeds are gonna be low with that motor, gearing ratio and wheels. You can either use higher-kv motor or use higher voltage like 9s you mentioned or just simply use bigger wheels which are better anyway.
```

---
## \#11 Posted by: B4Me Posted at: 2016-10-03T07:30:10.801Z Reads: 80

```
On the current setup, I go between 27-24kmt, but I would like to go like 35-30 ish
But without my motor burns out
```

---
