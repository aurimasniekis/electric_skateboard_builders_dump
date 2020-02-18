# Balancing individual packs with VESC and motors

### Replies: 16 Views: 1571

## \#1 Posted by: Eboosted Posted at: 2017-03-11T00:27:31.798Z Reads: 132

```
I'd like to manually balance the voltage of each individual pack for my 10S4P.

For each of the 10 packs I have meassured these voltages:

4.05v
4.05v
4.06v
4.04v
4.05v
4.06v
4.05v
4.19v
4.07v
4.04v

The pack number 8 has 4.19v, 0.14v above the average, what would be the best/safest way to lower the voltage of this specific pack?

Unfortunately I don't have a balancer charger.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-11T00:51:13.199Z Reads: 129

```
it is fairly easy to isolate parallel cell groups and use a simple load like an automotive running light to drain a particular group while monitoring its voltage.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-03-11T01:16:23.263Z Reads: 125

```
As you can see by the diagram, the positive balance wire from cell group 7 is the negative side of cell group 8.
Here is a diagram to isolate cell group 8 through the balance harness. It would be handy if you could find a female plug to fit your balance connector and make an adapter that would allow you to access any cell group individually in your pack.

<img src="/uploads/db1493/original/3X/0/4/04d289ffa5e3ed82c38f12dc5b1c2901701f7b68.png" width="547" height="500">
```

---
## \#4 Posted by: Eboosted Posted at: 2017-03-11T05:53:45.586Z Reads: 97

```
Fortunately for me is really easy to isolate the incorrect balanced pack. 

[img]http://i.imgur.com/Xf98GwO.jpg[/img]

Thanks for the input, I'll try the automotive bulb tomorrow
```

---
## \#5 Posted by: Namasaki Posted at: 2017-03-11T07:14:44.596Z Reads: 90

```
Oh, I see. I thought you were dealing with a more conventional, welded  Li-ion pack.
This is the Light I use. I got it at a local auto parts store and just added the connectors.
<img src="/uploads/db1493/original/3X/5/0/50badaceaac28c4aca10eac1d3eae723ef6321d2.jpeg" width="666" height="500">
```

---
## \#6 Posted by: Namasaki Posted at: 2017-03-11T07:24:49.898Z Reads: 81

```
I suspected that you may have already had an understanding of how this works, still I thought that it might be helpful to others reading this thread who are new to this stuff. 
Besides that I kind of enjoy making diagrams.
```

---
## \#7 Posted by: Eboosted Posted at: 2017-03-12T04:40:50.773Z Reads: 64

```
I'm going to use your method and just buy a regular 5v bulb
```

---
## \#8 Posted by: Hummie Posted at: 2017-03-12T15:52:00.824Z Reads: 60

```
https://commonsenserc.com/product_info.php?products_id=6705
```

---
## \#9 Posted by: Eboosted Posted at: 2017-03-12T17:02:02.261Z Reads: 58

```
This pack is only for 8S, are there any 10S options? 

BTW how does these balancers are able to tell what is the individual voltage of each pack, if it is only connected to the main charging plug?
```

---
## \#10 Posted by: Hummie Posted at: 2017-03-12T17:09:49.735Z Reads: 58

```
no 10s options I've found.  theres a balance discharger in the endless sphere for sale section that can do many more but it's not plug and play.
the one I posted connects to the balance wires
```

---
## \#11 Posted by: KTMinni Posted at: 2017-03-12T21:02:54.323Z Reads: 54

```
I love that enclosure where did you get it?
```

---
## \#12 Posted by: Eboosted Posted at: 2017-03-12T21:30:22.405Z Reads: 50

```
Thanks @KTMinni, I made the enclosure myself, check it here 

http://www.electric-skateboard.builders/t/loaded-vanguard-and-never-summer-reaper-enclosures-for-sale/17137
```

---
## \#13 Posted by: treenutter Posted at: 2017-03-13T00:27:57.637Z Reads: 41

```
@Namasaki that's a great diagram. Do you have suggestions for how to **charge** a single parallel pack that is already wired in series? Would it be the same diagram?
```

---
## \#14 Posted by: KTMinni Posted at: 2017-03-13T00:36:57.006Z Reads: 43

```
Wow! I'm actually really interested in getting one of these! Keep in touch Im still saving money.  That is if you're still selling.
```

---
## \#15 Posted by: cricrithezar Posted at: 2017-03-13T00:44:41.711Z Reads: 41

```
Why not get a cheap BMS off of ebay?
I'm getting this one and I haven't tested it yet so I can't talk about how good it is, but it's 10S and probably not enough for discharge but you can just keep it connected and run your power supply through it so it cuts off power once the pack is charged:
http://www.ebay.com/itm/391264318846
Not having any balance charging is kinda sketchy (then again trusting a cheap no-brand board for balancing is kinda sketchy too). Just something to consider.
EDIT: there are better BMSs that you could use for discharge as well if you want, can't remember the link though but if you want I can try and find it, they're about $35 which is still pretty reasonable.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-03-13T01:21:20.977Z Reads: 40

```
You could isolate a single parallel pack for charge through the balance wires as long as you do it at low amperage.
Another option is to connect your charge leads to the single pack with alligator clips connected to the weld tabs on the positive and negative sides of the pack to be charged.
```

---
