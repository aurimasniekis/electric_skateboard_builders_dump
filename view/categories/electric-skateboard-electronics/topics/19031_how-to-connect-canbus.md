# How to connect canbus

### Replies: 12 Views: 3086

## \#1 Posted by: moe_lester Posted at: 2017-03-13T22:00:16.722Z Reads: 320

```
Guys Ive just received two Maytech Vesc, I ordered it from Alien power systems. How Do i connect the Canbus? the cable I was sent doesn't look like the right one?? 
 
One end goes into the Vesc but the other end doesn't seem to plug into anywhere on the second Vesc.

Am I missing something??

<img src="/uploads/db1493/original/3X/c/1/c14e887551707ae9d235818a7b08eb0b9d63a034.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/9/4/942d02819a187ccce707a4b467d0aa9e9b32ba76.JPG" width="375" height="500">
```

---
## \#2 Posted by: mmaner Posted at: 2017-03-13T22:07:23.818Z Reads: 307

```
It should go into the same plug on the opposing VESC, but it only needs 2 wires.  Not sure why your lead has 5.
```

---
## \#3 Posted by: rpn314 Posted at: 2017-03-13T22:07:24.831Z Reads: 308

```
That is definitely not a cable that will work. Both ends should be the same connector

Edit; That's not the Can-bus cable anyways. The can-bus connector is the 4-pin connector on the right next to the USB plug.
```

---
## \#4 Posted by: lowGuido Posted at: 2017-03-13T22:10:30.042Z Reads: 308

```
I think you have the cable for hall sensors in your hand there..
canbus only needs the 2 pins like this cable:

http://www.ollinboardcompany.com/product/canbus-connector-for-vedder-s-motor-controller
```

---
## \#5 Posted by: flatsp0t Posted at: 2017-03-13T22:11:07.913Z Reads: 302

```
Please use the search function next time first:

http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
```

---
## \#6 Posted by: moe_lester Posted at: 2017-03-13T22:18:00.554Z Reads: 273

```
Yh I just released thanks, I only asked because I emailed the supplier before hand and they told me they would put in a canbus with my order :/
```

---
## \#7 Posted by: IsTalo Posted at: 2017-03-13T23:03:32.612Z Reads: 239

```
Man, I have this Vesc and I think it is for a Uart port or a extension for a Sensored motor
```

---
## \#8 Posted by: Lambjr088 Posted at: 2017-05-11T04:34:29.721Z Reads: 196

```
Is that the only person who has the Canbus plug?
```

---
## \#9 Posted by: paul775 Posted at: 2017-05-11T05:35:22.650Z Reads: 189

```
Diyelectricskateboard has them
```

---
## \#10 Posted by: Mikenopolis Posted at: 2017-06-08T16:56:25.033Z Reads: 180

```
FYI: I was just looking for a Canbus cable. DIYelectric's shipping was like $10 and Ollin's shipping was $3 (cables were roughly the same price.
```

---
## \#11 Posted by: thisguyhere Posted at: 2017-06-08T16:59:48.233Z Reads: 177

```
or skip the CAN altogether and just split the remote signal to each of the VESCs: https://www.electric-skateboard.builders/t/how-should-i-go-about-programming-double-vesc/19731
```

---
## \#12 Posted by: lowGuido Posted at: 2017-06-08T17:16:43.243Z Reads: 168

```
you can just use 2 wires and solder them to the board.
```

---
