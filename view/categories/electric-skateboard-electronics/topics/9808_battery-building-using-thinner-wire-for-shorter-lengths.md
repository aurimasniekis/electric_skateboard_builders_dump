# Battery building: Using thinner wire for shorter lengths?

### Replies: 12 Views: 833

## \#1 Posted by: michaelcpg Posted at: 2016-09-18T23:12:05.682Z Reads: 102

```
I'm in the process of building a modular 10S4P pack that can easily be split up into 6 smaller packs so I can take my board on a plane. I've got a bunch of this wire already which I'm considering using to solder between the connectors I'm using and the ends of each smaller pack. 

http://www.jaycar.co.nz/25-amp-dc-auto-power-cable-black/p/WH3082

I understand that generally you'd want to use thicker wire than this in most areas but considering that the length of wire between the actual battery packs and the connectors are only at most a few cm long, should I be able to get away with thinner wire like this for such short lengths?
```

---
## \#2 Posted by: michaelcpg Posted at: 2016-09-18T23:28:34.356Z Reads: 95

```
<img src="/uploads/db1493/original/3X/8/8/888b183c39e842ccf7a9c664a0e62caaa2f64b4b.jpg" width="690" height="388">

These are the sections where I'd be looking to use this wire
```

---
## \#3 Posted by: Jinra Posted at: 2016-09-19T00:39:33.393Z Reads: 87

```
what awg you talking? You'll probably burn up the wire if you use anything thinner than 14-16awg. Keep in mind the faa allows you to bring 2 spare packs with one pack in the "device", so you probably can't bring all 6.
```

---
## \#4 Posted by: boards Posted at: 2016-09-19T00:42:49.729Z Reads: 83

```
I'd try to leave space for some 12 awg and bullets for quick connections and then use longer brass plates to get each pack under 100wh
```

---
## \#5 Posted by: boards Posted at: 2016-09-19T00:44:03.561Z Reads: 83

```
You can bring any amount of packs under 100wh.
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-09-19T00:59:57.795Z Reads: 77

```
I'm unsure of the AWG but the wire itself is about 2.5mm thick from memory.
```

---
## \#7 Posted by: Jinra Posted at: 2016-09-19T01:02:50.795Z Reads: 77

```
Ah you're right, I'm thinking of 101-160wh

@michaelcpg yea that sounds way too thin. You need wire capable of supporting 80a continuous load without melting.
```

---
## \#8 Posted by: Jinra Posted at: 2016-09-19T01:09:29.067Z Reads: 78

```
See here for rough current limits of various wire

http://www.powerstream.com/wire-fusing-currents.htm
```

---
## \#9 Posted by: michaelcpg Posted at: 2016-09-19T01:16:14.108Z Reads: 72

```
80A seems a bit much I would've thought? I've always had a 40A fuse on my board which has never blown. Thanks for the link, the main thing I'm thinking about when looking at those sort of tables though is that I expect the ratings would be based on wire that's significantly longer than a few cm's?
```

---
## \#10 Posted by: Jinra Posted at: 2016-09-19T01:42:33.987Z Reads: 66

```
Thickness plays more of a role than length. 80a is what your pack is rated for, so I'd follow that guideline. The 40A fuse made me street my face once from it blowing, so I'd replace that if i were you. However, you shouldn't blow it if you don't do anything extreme.
```

---
## \#11 Posted by: michaelcpg Posted at: 2016-09-19T01:48:44.962Z Reads: 65

```
Hmm yea I remember reading your post about that a while ago actually, what was your battery max set to on your VESC/s at the time?
```

---
## \#12 Posted by: Jinra Posted at: 2016-09-19T03:10:02.335Z Reads: 57

```
40 per VESC so 80 total.
```

---
