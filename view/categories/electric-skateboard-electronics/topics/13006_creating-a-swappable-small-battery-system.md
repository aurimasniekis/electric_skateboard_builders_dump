# Creating a swappable small battery system

### Replies: 4 Views: 1452

## \#1 Posted by: faust Posted at: 2016-11-13T19:36:15.163Z Reads: 220

```
Hi everyone!
 
I feel I need to develop a swappable small batter system so that I'm able to create a tiny e-board with sufficient range for any situation. I was hoping you all might be able to help. Just for some background on the battery requirements, here's the board I'm planning to build so far: 
* 22" board with 125mm trucks and wheels to fit. Details here: http://www.electric-skateboard.builders/t/mini-rover-121c-22-rover-randal-125mm-trucks-hub-motor/12851
* To deal with the 125mm trucks, I need hub motors with low kv (thinking Jacob's). I'm fine with low speed, but I need the motors to actually be able to push me around. 
* To deal with the small board size, I need a small battery pack. To enable decent range, that small battery pack needs to be swappable.  

As for the battery, I'm thinking of the following: 
* 10s2p (Within 2"x4"x8")
* Built in switch, spark protection
* BMS
* Under 99Wh (for air travel)
* Easy, slide-in connector (e.g., like the Mellow Drive). 
* 3D printing and whatever to get a nice enclosure (both board-side and battery-side)

I'm looking to build something elegant, so I'm willing to learn spot welding and all that if it's necessary. But it'd also be great if there were pre-built options you'd recommend (e.g., modding an existing product or starting with pre-built packs, etc...). Any example might be to modify a space cell or to get battery packs from Alibaba or something ([https://www.alibaba.com/product-detail/High-recommmend-18650-36v-10s2p-battery_60535325860.html](https://www.alibaba.com/product-detail/High-recommmend-18650-36v-10s2p-battery_60535325860.html)). Though I worry about reliability in the latter case. 

Any thoughts?
```

---
## \#2 Posted by: Luke Posted at: 2016-11-13T20:30:21.458Z Reads: 195

```
You'll need to watch out for voltage sag with 10s 2p battery packs. I'd have a look at what people are doing with 12s1p A123 cells.
```

---
## \#3 Posted by: faust Posted at: 2016-11-13T21:14:46.762Z Reads: 184

```
It looks like there are less options available with the available space that I have. I do see that there is a preorder available at , and the dimensions listed (secondhand) in this [thread](http://www.electric-skateboard.builders/t/diyelectricscateboards-coms-epower-battery-12s1p-a123-26650/6387/6) indicates a size of 30mmx150mmx308mm (1.2in x 6in x 12.2in).

I looked at a few other options, and the size requirements seemed to be roughly the same. I might be able to extend my wheelbase an inch to accommodate, but in general, I'm thinking the 12s1p A123 route might demand more space than I have. Especially considering the extra space required to make the battery replaceable. Perhaps there's a way to address or mitigate the voltage sag present in a 10s2p (or maybe 10s3p) configuration.
```

---
## \#4 Posted by: Okami Posted at: 2016-12-13T18:56:26.569Z Reads: 117

```
To mitigate voltage sag some ppl sugest to try to add a lipo pack in parallel (if you cannot afford to go with higher discharge cells or make more cells in parallel).. though, I have not tested this myself but I've seen some ppl mentioning (on ebike / escooter forum) that they have mixed the chemistries and just monitor voltage for each pack..).

I think it is hard to find such examples on this forum.. but this is just an idea to consider but the risk and real life reliability is up to the ones who decide to go this route.. as I have not seen a very detailed explanation of how everything works but it just seems to work and that's all.



---
A new idea I've found is that some ppl (electric car makers) even ponder the idea about using ultra capacitor (large capacity capacitors).. to get ''boost'' and to be more gentle on the batteries by not draining them too hard. Though, this solution probably goes out of hand without questions, as the size of these ultra caps are quite large, they usually cost quite a bit (unless you make some on your own) and they are just not very practical - suitable for eboard use because of their size and possible other electronic modifications needed.
```

---
