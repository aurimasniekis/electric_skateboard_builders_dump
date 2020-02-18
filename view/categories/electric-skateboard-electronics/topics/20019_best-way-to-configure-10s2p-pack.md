# Best way to configure 10S2P Pack?

### Replies: 8 Views: 1992

## \#1 Posted by: gr8sk8m8 Posted at: 2017-03-30T18:23:45.184Z Reads: 196

```
Hi eSk8 community!

I've been doing a lot of research lately and I've decided to start deciding on parts I want to get to put together for my board. So far it looks like an [Ollin Board Company 200kv motor](http://www.ollinboardcompany.com/product/om5065-200kv), a [VESC](http://www.ollinboardcompany.com/product/vedder-s-speed-controller), and 20 [LG HG2 18650 batteries](https://www.alibaba.com/product-detail/2016-new-chocolate-lg-hg2-20_60308411399.htm). Right now, Iv'e got a thunder AC lipo and lithium ion battery charger to charge batteries for my race quad. I'd prefer not to buy a new charger so I'm looking to configure my eboard pack in a way that would allow me to charge the battery in sections. The way I see it, I've got a couple of options. I could put 5 cells in series as a single pack (with balance connector of course) and put that in series with another identical pack. Then, I'd put this 10s pack in parallel with another one identical to it. The upside to this is that in order to charge I could just take apart the 4 separate 5s1p packs and balance charge them one at a time. The downside, is that the wiring would be messier. I don't like the idea of having to splice two 10 gauge wires together for both positive and negative to get them to an XT90 connector (that's what's already soldered onto the VESC I bought). The other way I could do this, is solder together quantity 10 1s2p packs and put all of them in series. This would be a lot cleaner for wiring, but charging 10 separate batteries would be a hassle. Also, I'm not sure what the safety concerns with batteries configured like this are. Can I just solder two 18650's in parallel with nickel solder tab and just charge them like I would a 1s lipo pack? Do I need a balance connector (leaning towards no, but I'll put the question out there)? If I keep all my batteries the same voltage and make sure everything is equal in a pack do I need a BMS (really don't want to incorporate one I'd rather go through all the work of charging individual packs). Any help is greatly appreciated.

-gr8sk8m8
```

---
## \#2 Posted by: PXSS Posted at: 2017-03-30T20:21:02.051Z Reads: 179

```
Why not just do 2 5S2P packs and then wire them in series?
```

---
## \#3 Posted by: gr8sk8m8 Posted at: 2017-03-30T20:31:33.165Z Reads: 179

```
Wow. I feel pretty stupid not thinking of that. Thank you! Being that I've got a drop through board, I'm trying to keep the battery as flat as possible. Is it feasible to tab and solder two 18650's with anodes facing one direction, and then solder it to one of the same parallel parts in the opposite direction? I guess I'm trying to picture how I'd make this battery as flat as possible.
```

---
## \#4 Posted by: willpark16 Posted at: 2017-03-30T20:39:31.951Z Reads: 175

```
That will be flat
```

---
## \#5 Posted by: PXSS Posted at: 2017-03-30T20:44:58.036Z Reads: 170

```
2 cells looking one way and 2 cells looking the other, back and forth. 

This is a 10S3P pack split in two 5S3P
<img src="/uploads/db1493/original/3X/d/4/d4c027baab22a6dc083f1186d1c5b7306c1c93f0.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/4/1/41648f4db018b3be8837e53ba4ecef194d065f47.JPG" width="666" height="500">
```

---
## \#6 Posted by: gr8sk8m8 Posted at: 2017-03-31T16:25:09.459Z Reads: 144

```
Thank's for all the help! @PXSS I'm guessing that the small tabs with holes coming off between the parallel cells are the balance charging lead points? Also, I'm confused as to how to add up constant draw amounts. I know that typically with lipo batteries you're supposed to charge them at 1c. Being that I'm using LG HG2 batteries, 1c would be 3 amps I believe? In the configuration that I would have my pack in (5s2p), what charging current should i be pushing?
```

---
## \#7 Posted by: PXSS Posted at: 2017-03-31T16:30:49.366Z Reads: 144

```
Refer to the spec sheet of the specific cell you use as to what current you should use to charge.
You can double that current since you have a 2p pack.
Most people around here just settle for somewhere between 2-5A though.

[quote="gr8sk8m8, post:6, topic:20019"]
I'm guessing that the small tabs with holes coming off between the parallel cells are the balance charging lead points?
[/quote]

You are correct, that is where I will be wiring the balance leads
```

---
## \#8 Posted by: gr8sk8m8 Posted at: 2017-03-31T19:26:41.433Z Reads: 133

```
I know that range is a touchy subject as every small variable of the rider, board, and route ridden matters, but what gear reduction would you all suggest for maximum range from this setup?
```

---
