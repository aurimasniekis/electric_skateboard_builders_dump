# Airplanes and BMS

### Replies: 9 Views: 1045

## \#1 Posted by: ZachNYC Posted at: 2016-11-26T21:15:06.459Z Reads: 108

```
Hi all,
I'm making planning on making a battery like this so that I can take it apart and take it on planes, but also using a bms for charging and possibly discharging (in 6S though) <img src="/uploads/db1493/original/3X/1/d/1de2efd18502153ae93aa4d2737a4e97e6c141b9.jpg" width="320" height="500">
I would like to charge without having to take the battery out and also charge all of them together, and to the extent of my knowledge, a bms is the only way to do that. Does anyone have any suggestions or ideas on how to make this work?
```

---
## \#2 Posted by: Eboostin Posted at: 2016-11-26T21:29:08.477Z Reads: 102

```
99Wh is the largest a pack can be. 

My plan when I start flying more is to break my pack into 99Wh or less packs. 

Use bullet connectors to connect the packs main leads and then create a harness for the BMS pins
```

---
## \#3 Posted by: ZachNYC Posted at: 2016-11-26T22:33:59.147Z Reads: 88

```
What do you mean by a harness?
```

---
## \#4 Posted by: Eboostin Posted at: 2016-11-27T00:00:42.059Z Reads: 73

```
If you want to use a BMS, the balance leads will have to be separated when you take the pack apart. 

If it is a 7s pack, you would ideally have a 3 pin and a 4 pin that connect to the 7 pin connector for the bms.
```

---
## \#5 Posted by: ZachNYC Posted at: 2016-11-27T03:56:06.292Z Reads: 62

```
It will be 6s, and I would ideally like it to split into 6 6p packs, so splitting them all up, how would I get it back together without resoldering
```

---
## \#6 Posted by: Eboostin Posted at: 2016-11-27T04:09:41.210Z Reads: 58

```
If the original photo in your post is of the cells your're using (25Rs) then 36 cells would be 324Wh. If you want to use 36 cells then you'll need to break up the pack into 6 packs of 6 cells or 4 packs of 9 cells to stay under the 99Wh limit.  

Take a look at some of the cell layouts/wiring diagrams and then where ever you split the packs, you'll need to keep the balance leads together. 

Definitely read up on here as the pack you're proposing takes more planning and know how then a non-modular pack.
```

---
## \#7 Posted by: composites_r_awesome Posted at: 2016-11-27T12:08:12.112Z Reads: 48

```
Hi,
I'm also building a board with similar setup (12s6p 25R, swappable). Mostly because of increased distance by having backpack of spare battarias. Also if you discharge 12s down to 3.3 or that, you get it right to 99Wh. If a bad cell would happen, the infected battaria could be easily taken out from the board. I thought I somehow could do it without having balance leads and main leads hanging from every pack, just like dangling in the breeze there, but I find [these pin headers](http://www.ebay.ca/itm/10Pcs-40Pin-2-54mm-Single-Row-Round-Female-Pin-Header-Socket-gold-plated-/252011129134?hash=item3aad08a92e%3Ag%3AOzsAAOSwBLlVAVYC) to be suitable,mostly rated some 4Amp, you can parallel those enough until you reach your desired need
```

---
## \#8 Posted by: Eboostin Posted at: 2016-11-27T17:12:55.884Z Reads: 34

```
The Wh rating is based of nominal voltage not what the batteries actual voltage is at (3.6v nominal for Li-ion, 3.7 for Lipo)
```

---
## \#9 Posted by: Eboostin Posted at: 2016-11-27T17:16:53.167Z Reads: 32

```
Something like this is what I meant by a harness.

<img src="/uploads/db1493/original/3X/0/4/0464624f0d5b5d61928e1231c7acb2fe6a3fe4e2.GIF" width="365" height="500"><img src="/uploads/db1493/original/3X/c/0/c0adeeadd14f9007eb5d8019a95bbee6597bd3d9.JPG" width="350" height="263">
```

---
