# Will this VESC modification work?

### Replies: 18 Views: 910

## \#1 Posted by: NAF Posted at: 2017-03-25T16:18:27.453Z Reads: 112

```
Guys my soldering skills are pretty bad, and I had to change the layout of the cables with xt60 connector. I am concermed about capacitor board and the way Xt60 cable is soldered to it. Is it ok? Will this setup work? Or the xt60 cable has to be soldered dorectly to capacitor board?

<img src="/uploads/db1493/original/3X/1/2/123211a96e72b11e62a372a86df1b4173a09ac91.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/6/56bf9d4e9bb55c1ae95f25019e35f5b192daae96.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/5/558eb3533b5101894d56c876289437030c7bdca5.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/9/4977339e550ee2e402b95877af007682e5d8515c.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/a/ea392e8dbe28c9cc2335e1dbeeec123192bf02e5.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/d/cda4bd547dff88e965b72225ce1afd8ae7466e25.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/5/058f27084bf64bae25738ce81389634d9c5db374.jpeg" width="375" height="500">
```

---
## \#2 Posted by: Iceni Posted at: 2017-03-25T16:59:11.562Z Reads: 93

```
That'll work fine.
```

---
## \#3 Posted by: NAF Posted at: 2017-03-25T16:59:15.949Z Reads: 94

```
Ok i am looking at other vescs and i am guessing its all wrong?
```

---
## \#4 Posted by: goldenHusky Posted at: 2017-03-25T17:08:58.116Z Reads: 92

```
What do you think is wrong? It looks fine to me aswell.
```

---
## \#5 Posted by: 3sly Posted at: 2017-03-25T17:34:38.793Z Reads: 88

```
Shouldn't the connector go after the caps? Not before like in the pictures.The caps are just floating.
```

---
## \#6 Posted by: NAF Posted at: 2017-03-25T17:41:52.446Z Reads: 82

```
Thats exactly what worries me. Can anyone confirm if connector can go before the caps?
```

---
## \#7 Posted by: Namasaki Posted at: 2017-03-25T17:42:28.264Z Reads: 78

```
I can't tell for sure from the pics but I think you may have bypassed the Caps.
<img src="/uploads/db1493/original/3X/1/f/1f6abf2fef3b343412f58ffd5ec6e8d9dbee00a6.PNG" width="690" height="387"><img src="/uploads/db1493/original/3X/9/2/929b2078daeb7c432a029fa1e8a81fad1f1d3e90.PNG" width="690" height="387">
```

---
## \#8 Posted by: Blasto Posted at: 2017-03-25T17:44:38.639Z Reads: 73

```
Nothing wrong here, carry on.
```

---
## \#9 Posted by: goldenHusky Posted at: 2017-03-25T17:52:44.809Z Reads: 74

```
@NAF  Don't worry. The caps must be in parallel to the wires in a "short as possible" distance to the VESC, and that's the case here. You can't bypass the caps since they are soldered parallel.
```

---
## \#10 Posted by: NAF Posted at: 2017-03-25T17:57:06.418Z Reads: 72

```
There are four slots in capacitor board. Two of them were left empty. The xt60 is 
soldered before the caps.

One side of the capictor board with two empty slots.
 <img src="/uploads/db1493/original/3X/2/c/2c89402ae8b4a7c98507a97be83bebc73f90c741.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/c/d/cda4bd547dff88e965b72225ce1afd8ae7466e25.jpeg" width="666" height="500">

And the other side with xt60 soldered before the caps

<img src="/uploads/db1493/original/3X/0/b/0b0db7b3d89c864b29d2729444172b23b88c0fbc.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/1/a16d27415abe6fcab160abd3d1c18f072a85270a.jpeg" width="666" height="500">
```

---
## \#11 Posted by: Namasaki Posted at: 2017-03-25T18:02:15.499Z Reads: 70

```
But how is the + side of the caps connected?
<img src="/uploads/db1493/original/3X/4/f/4f201b0d6744f3b4f2c88c202d1bd6af308bda51.PNG" width="690" height="387">
```

---
## \#12 Posted by: goldenHusky Posted at: 2017-03-25T18:18:44.987Z Reads: 67

```
There is a connection between the holes, so it doesn't matter if the other 2 holes are left unsoldered.

<img src="/uploads/db1493/original/3X/0/f/0fe01200cb62b8f1bf652757d0fb163ae3425544.jpg" width="690" height="420"> 
https://raw.githubusercontent.com/vedderb/CapPCB/master/Plot/CapSch.png
```

---
## \#13 Posted by: NAF Posted at: 2017-03-25T18:20:43.375Z Reads: 64

```
@Namasaki  The VESC I got was soldered exactly like on your pictures. All I did is I removed the the xt60 cables from these two slots ...and they are now left empty. I did nothing else.

<img src="/uploads/db1493/original/3X/6/b/6b15f0b6c436a00e99c05c61ca2e11ea0e83a661.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/2/22fab26e5e40c395c6ceef99b088ccb5b6c7d01e.JPG" width="666" height="500">
```

---
## \#14 Posted by: Namasaki Posted at: 2017-03-25T18:47:42.689Z Reads: 55

```
Ok, based on this schematic, it should work.
But are you sure that is the right schematic?
Because it doesn't appear to match the layout of the board.
```

---
## \#15 Posted by: goldenHusky Posted at: 2017-03-25T19:12:51.006Z Reads: 50

```
I took the schematic directly from Vedders Github https://github.com/vedderb/CapPCB/
The renderings of the pcb match with the ones in the pictures in here (as far as I can see).
```

---
## \#16 Posted by: Paulf Posted at: 2017-03-25T19:13:55.027Z Reads: 52

```
Capacitors are wired in parallel 
So + are all the same and so are - 
This will definitely work
```

---
## \#17 Posted by: Namasaki Posted at: 2017-03-25T19:15:04.736Z Reads: 53

```
Ok, I'm convinced
```

---
## \#18 Posted by: NAF Posted at: 2017-03-25T21:35:04.408Z Reads: 45

```
Thank you guys !! It all works !
```

---
