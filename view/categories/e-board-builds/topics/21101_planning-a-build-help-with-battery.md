# Planning a build, help with battery?

### Replies: 11 Views: 916

## \#1 Posted by: Shiven Posted at: 2017-04-15T21:33:52.921Z Reads: 121

```
Over the past year or so I've been looking into building an esk8, and have done a decent of research and looking around, some successful and some not so much.
My build is composed of:

- Turnigy Aerodrive SK3 168Kv motor (single motor)

- 36 inch cruiser deck from Amazon, with Caliber Trucks and 83mm Flywheels

- VESC as the esc (ofc)

- Pulley and 12mm belt from Enertion

- Motor mount from ebay

My only real struggle is with the battery. I am planning on getting a 12s setup, but I'm not sure whether to get a lipo set up or  a Li-Ion setup. I'd like to have 10,000 mah capacity because distance is more of a priority than speed. I've been looking at the [Multistar High Capacity 10000mAh 6S 10C Multi-Rotor Lipo Pack](https://hobbyking.com/en_us/multistar-high-capacity-6s-10000mah-multi-rotor-lipo-pack.html) and putting them in series for 12s, but the C rating is rather low. I've seen a lot of people using lipos with 20-30c's, so I don't know if the high mAh will help with the low C rating, or if a higher C rating would be preferred.

I'm planning on using a lipo charger for the lipos/li-ions and may be eventually wiring up a BMS with a switch and charger just to make charger a lot easier.

 Another thing I've been looking into is using 18650 cells, but the capacity isn't as large without requiring a lot of cells and putting the cells in parrell (to add up the mAh) and in series (to add the cells). 

EDIT: 
[For the Li-Ion option, I was thinking of buying 48 2500mAh cells. I was thinking of wiring them into 3s packs. Then wiring them into parallel to double to mAh to 5000, then wiring them into series for a 6s pack, then putting those into parallel to make the mAh to 10,000, then wiring the two final 6s packs into a 12s setup.

3s 2500mAh + 3s 2500mAh (parallel)= 3s 5000mAh, doing that until I have 16 packs.
Then combine two into series to get from 3s to 6s for all of them. Finally, wire the 6s packs into parallel to get two 6s packs at 10,000 then wires those into series for 12s. Then wire that to a BMS with a charger port and switch.]

Here is what I think the 12s pack with the [BMS](http://www.batterysupports.com/44v-48v-504v-12s-80a-12x-36v-lithium-ion-lipolymer-battery-bms-p-392.html) and charger schematic should look like;
<img src="/uploads/db1493/original/3X/f/8/f8c57e6e2071d9f3d274957dab1816b1fbbc7e89.jpg" width="666" height="500"> I plan on having the people who sell the BMS wire a switch for me when they send it.

If anyone can help with a solution that wouldn't be much more than two of those Multistar lipos, it would be **greatly** appreciated! The only problem with the Li-Ion is finding that many cells, wiring them, and doing it succesfully, if anyone knows where I can get that made for me that is also be awesome! Thanks!
```

---
## \#2 Posted by: EmielHuyghe Posted at: 2017-04-15T22:17:41.189Z Reads: 98

```
Capacity does matter when looking at the C-rating. Since these are big capacity packs, with those LiPo's you should be able to get a continuous discharge rate of 100A (10 000mAh * 10C), so that is a viable option.

I am building a Li-Ion setup because I think it is a bit safer than LiPo, although LiPo's should be fine as long as you handle them properly I think (which actually applies to all kinds of batteries). To get an 18650 pack with your requirements, you could build a 12s4p pack to get the same capacity of 10 000mAh (for example with Samsung 25R cells). As you mentioned yourself, it does take a lot of cells (and more effort), but that eventually comes down to preference I guess.
```

---
## \#3 Posted by: Shiven Posted at: 2017-04-15T22:33:57.167Z Reads: 95

```
Thanks for the reply! I plan on using an IMAX B6 charger with a parallel board for the batteries. I may stick with the lipos for now.
```

---
## \#4 Posted by: anorak234 Posted at: 2017-04-16T01:31:35.805Z Reads: 88

```
I always recommend Li-ion over LiPos. For safety, money, and longevity Li-ion is better. It's easier to include a bms with Liion, they are of a more stable chemistry, and they get up to 4x the charge cycles as Lipos, so you'll end up saving money if you use the board regularly
```

---
## \#5 Posted by: Shiven Posted at: 2017-04-16T01:52:44.950Z Reads: 86

```
Hmm, very true. The only problem I have with it is the amount of cells I'd need to achieve a similar capacity as the lipos mentioned above.
```

---
## \#6 Posted by: Shiven Posted at: 2017-04-16T02:13:23.524Z Reads: 83

```
I added an edit to the post, any idea that could possibly help with what I have in mind
```

---
## \#7 Posted by: anorak234 Posted at: 2017-04-16T02:35:57.062Z Reads: 82

```
I don't know what your budget is at hand, but the best cells I've ever used were the BASEN 26650s. They're each 4500mah and have 60amps so a 12s3p would more than satisfy the requirements. They run ~8$ a cell, which means ~300$ for the cells, plus 150 for a bms and wires and metal strips. Looks to be around a 500$ battery once all is said and done. Trust me - a battery like that will last you ages and never disappoint. Just don't be expecting to carry your board around much.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-16T07:25:03.492Z Reads: 73

```
Others have tried using those multi rotor 10c packs and have reported that they are not good.
A better High capacity Lipo option is the 3s/8000mah 30c Zippy Flightmax.
Four of those in series for 12s/8000  would give you 240a constant discharge which is a lot of head room that will keep voltage sag to a minimum and might get you 20 miles on a charge depending on how you ride.

If you go with Li-ion, 12s4p, I would recommend 18650 30Q cells. Rumor has it that they are the best available at this time.
As for the Basen 26650 cells, there 60a rating is a pulse rating. They're continuous rating is 30a
I built a 10s2p (9ah)  pack with them and it worked well on flat ground, I got up to 28 mile range.
But when I went hill climbing with it, the voltage sag was excessive and cut my range down to 12 miles.
```

---
## \#10 Posted by: Shiven Posted at: 2017-04-16T07:37:49.722Z Reads: 71

```
Is there anywhere I can get a the battery set up I mentioned? It's a lot of wiring and I'm not sure of 100% of the things and rather not risk anything messing up.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-04-16T07:43:34.484Z Reads: 63

```
@barajabali is a battery builder who can build you a custom battery.
```

---
## \#12 Posted by: anorak234 Posted at: 2017-04-16T15:37:39.106Z Reads: 53

```
I second that ^ @barajabali is the man for any lithium-ion builds
```

---
