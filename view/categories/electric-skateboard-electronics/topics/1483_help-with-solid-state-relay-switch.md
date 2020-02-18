# Help with solid state relay switch

### Replies: 5 Views: 1203

## \#1 Posted by: tommyb10 Posted at: 2016-02-21T06:04:15.325Z Reads: 92

```
Hey guys, so I purchased a 100A solid state relay to use with a spdt switch to turn my board on and off.

After connecting it, there is a voltage difference (4v) over the relay when off and my switch illuminates. When I turn it on, this voltage difference is subtracted from my actual voltage so I get a lower voltage (eg 24-4 = 20v)

This is not good as my low voltage alarm goes off and my esc will throttle down as it thinks the cells are low.

How can I fix this? or is my relay borked?

Cheers!!
```

---
## \#2 Posted by: Blasto Posted at: 2016-02-22T06:13:34.201Z Reads: 81

```
Link to your SSR and a quick schematic of how you are using it?
```

---
## \#3 Posted by: tommyb10 Posted at: 2016-02-22T06:44:58.625Z Reads: 81

```
Here is some more info in an endless-sphere thread: https://endless-sphere.com/forums/viewtopic.php?f=35&t=76479

Hope someone somewhere is able to help :stuck_out_tongue:

What I think is happening is that for some reason the ssr is acting as a resistor or something instead of a relay?
```

---
## \#4 Posted by: Blasto Posted at: 2016-02-22T14:05:44.788Z Reads: 73

```
tldr

but based on what your a saying, sounds like your are seeing the Vgs of the fets inside the ssr (sign of lack of isolation).

<img src="/uploads/db1493/original/2X/f/f3103a1a2ab15c7f5644ca625c6b3807a5f10950.png" width="690" height="261"> You can try putting the SSR on the low of the circuit
```

---
## \#5 Posted by: tommyb10 Posted at: 2016-02-22T22:53:33.170Z Reads: 62

```
Tried putting it on the negative but still no go. When the ssr is off I can measure 7v across it, which means that 5 are going to the load. I'm going to get a new relay, I reckon this ones borked. 

Cheers!
```

---
