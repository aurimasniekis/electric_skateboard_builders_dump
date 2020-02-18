# VESC6 and bluetooth adapters compatibility

### Replies: 5 Views: 937

## \#1 Posted by: brotori Posted at: 2018-03-13T21:43:31.714Z Reads: 148

```
Newbie here. I am building a mountainboard. Trampa with Dual VESC6, 12S, and I want to install a Bluetooth adapter.

However, there is a warning in the vesc-project forum. [WARNINGs!! What you should not do!](https://www.vesc-project.com/node/45) stating that "... equipment that was designed for VESC 4 should not be used with VESC Six, until the vendor has stated that it is compatible."

I already have [this Bluetooth Adapter](https://miamielectricboards.com/shop-1/vesc-bluetooth-adapter)

I check with @trampa, and Frank said that the adapter probably would not work and the software would get messed up...  And that TRAMPA is working on a better solution. Or I could check with Roman, at Metr.at. (thanks for the info Frank!)

I also did check with the seller, @oriol360, and in his opinion, the adapter should work, but has no direct experience.

I would not like to risk messing up these expensive VESCs. Has anyone tried this module on a VESC 6?

The connector seems to be ok, There is a match between the BT module and the VESC6 connector

1 blue tdx
2 green rdx
3 
4 black gnd
5 red vcc
6

This is a picture of the connector installed, but I am not brave enough to connect the battery and test...

![20180313_181309|374x500](upload://assgxzgiRoCtUoi8DwlPk0EJ0YV.jpg)
```

---
## \#2 Posted by: trampa Posted at: 2018-03-14T13:20:37.194Z Reads: 119

```
If this thing is made for HW 4.xx, you will probably have issues.

Frank
```

---
## \#3 Posted by: Surfer Posted at: 2018-03-14T13:24:28.771Z Reads: 116

```
I really think is totally compatible
```

---
## \#4 Posted by: SeanHacker Posted at: 2018-03-14T13:31:29.711Z Reads: 112

```
I don't think you'll have any issues. Make sure to connect tx to rx and rx to tx.
```

---
## \#5 Posted by: Namasaki Posted at: 2018-03-16T22:23:52.419Z Reads: 94

```
there was post just yesterday where someone connected a bluetooth module to their Vesc 4 and the module shorted out the Vesc buck converter so be careful.
Metr sells a module wired specifically for Vesc 6 with an 8 pin connector.

https://metr.at/shop

![05 PM|500x500](upload://3XIuxsQWCJ0CZEewHGQOhwbgg9L.png)
```

---
