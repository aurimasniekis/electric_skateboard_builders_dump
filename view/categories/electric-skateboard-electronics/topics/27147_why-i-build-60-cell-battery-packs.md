# Why I build 60 cell battery packs

### Replies: 4 Views: 681

## \#1 Posted by: chaka Posted at: 2017-07-09T15:51:38.244Z Reads: 215

```
Back in 2015 I started posting picks of the insanely large battery packs I was installing in our beta builds. The largest we built was an 80 cell pack. Many told us it was not needed and we were adding unnecessary weight but I knew they just could not see the bigger picture. Voltage sag is directly related to a battery's ability to give up the amps. Adding more cells in parallel is what we do to overcome this sag and give a flat discharge curve. From experience I have found no cell that performs well when asked to give more than 10 amps constant, peaking at 5 is better. In a 10s6p pack this comes to a max of 30A and 60A. 30A for extended climbing and 60A during acceleration. 

When you consider the lack of voltage sag in a pack this large you will begin to make the connection and see you will actually produce more watts because you will be running at a higher average voltage during discharge. I will be happy to go into further detail but I hope this scratches the surface into my reasons for building such a large pack as my industry minimum. 

Here is a graph showing the discharge curves of my 2 favorite cells at 5 and 10 amps. Anyone want to do the math on what capacity we get on a 10s6p ncr20700b battery pack?!!

<img src="/uploads/db1493/original/3X/6/9/69b606419dc0b80efc01a56521b349addf1e85c2.png" width="690" height="389">
```

---
## \#2 Posted by: Okami Posted at: 2017-07-09T17:59:11.274Z Reads: 186

```
At what power levels do you usually use your board?

From the chart alone, yes it can be seen, that 5 / 10A difference can be quite huge.. a 0.2v drop per cell, at 10S, this might equal to 2v drop, and probably about 300 - 400 (~150kv - 200kv) drop in max rpm from motor directly.

@chaka have you thought about 'buffer battery' or some sort of capacitor bank for such situations?

I have heard of using lipo battery for high power demand situations but so far it looks like it is not used frequently by builders here but a while ago I saw a few ebike builders using such 'tactic' to get a bit of a boost, the only thing is you need seperate switch/circuit, to 'activate' the boost pack.

As about the capacitors - I imagine they probably cannot store enough charge for meaningful impact on delivering enough energy, so they are quite useless, unless used for sensitive equipment like vesc. 

But maybe there is a potential if someone went really far, and installed larger capacitors? Though as Im not really good with capacitor physics im not sure what quantity would be needed then to make it worthwhile and not just add more batteries in parallel.
```

---
## \#3 Posted by: mwkeefer Posted at: 2017-07-10T12:31:21.599Z Reads: 138

```
Coming from 10 years of building one off custom EBikes, custom li-ion/Lipoly packs and custom bmses... you would be better off just to ditch the lithium-ion, forget the booster packs and stiffening capacitors and just go high C Lipo from GO... or build out in parallel, just as @chaka does :slight_smile: to  produce a flat discharge curve which of course translates to more consistent and streetable performance with a nice side benefit of extending the cycle life of a given pack since the demand is so minimal! :smile:

 I know everybody says this doesn't really work to extend life cycle of lithium ion her lithium polymer packs, I have Hobby King 30 C 13S, 15S and 20S packs (10/15AH) with well over 1000 cycle count on them and they are still going strong with >= 95% of capacity

-Mike
```

---
## \#4 Posted by: chaka Posted at: 2017-07-10T14:27:07.200Z Reads: 121

```
Lipo is great for smaller battery packs but I would worry about having 60 individual prismatic cells with a bms. Simply put, lipos are too unstable at DOD to trust. They have a much more pronounce cliff compared to a li-ion. Lipos require much more care that the average consumer can give to avoid puffing their packs.  They are perfect for light weight craft with high current demands but still require a lot of care to avoid problems

.
@Okami  Not sure you will get any gains from adding caps but there are multiple reasons why I use 60 cells. I want my boards to last years without any significant loss in capacity, as @mwkeefer  mentioned, a pack this large will have many more useful charge cycles because the individual cells will have a much lower demand on them during discharge "and" charge cycles. 

Another reason to go big is the fact that more amps can be pushed back into the pack during regenerative braking without pulsing the voltage over the max or harming the cells from too much charge current.

Cost is another reason to go big. If you use cost and watt-hours as the metric cost goes down when you increase the size of your pack. For example, a boosted will cost you roughly $15.00 per watt-hour at full retail. Our FreeRide with HG2 cells is around $3.60 per watt-hour. Sure, you could say I am playing with numbers but capacity is a very important spec and plays a huge role in how enjoyable a board can be.
```

---
