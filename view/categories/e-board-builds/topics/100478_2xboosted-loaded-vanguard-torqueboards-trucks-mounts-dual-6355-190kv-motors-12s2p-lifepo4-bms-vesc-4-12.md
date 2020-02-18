# 2xBoosted &#124; Loaded Vanguard &#124; TorqueBoards Trucks &amp; Mounts &#124; Dual 6355 190KV motors &#124; 12S2P LiFePO4 BMS &#124; VESC 4.12

### Replies: 3 Views: 293

## \#1 Posted by: YoungDoughboy Posted at: 2019-08-18T00:23:11.241Z Reads: 106

```
[See bottom for my vesc question - it's not pulling enough amps!]
  
  
My first build, inspired by this forum (thanks everybody). I chose [LiFePO4](https://www.batteryspace.com/a123-lifepo4-26650-rechargeable-cell-3-3v-2500-mah-50a-rate-8-25wh-anr26650m1b---un38-3-passed-and-iec-listed.aspx) for the increased cycle life, safety, and the high amperage (which meant [more BMS](https://www.aliexpress.com/item/32953217422.html?spm=2114.12010612.8148356.15.1d7a7b7181isNc) and more difficulty wiring the pack with wire with higher gauge down the line)

Built my own spot welder with some huge capacitors from amazon and a bunch of mosfets:
![IMG_1666%20copy|666x500](upload://6kAtdXAtooLPFEHJc6PdKgxE5zo.jpeg) 

Used solid copper wire soldered to short nickel strips to build the pack (don't have any good pictures of this up close) so that it could put out its 100A cont. comfortably without melting anything. Here's the finished 12s2p pack with the BMS - which is as thick as one of the batteries itself:
![IMG_2700%20copy|375x500](upload://dLP6TPBWjPrTIOMHiAU7TSR1HQ8.jpeg)

For my enclosures I softened ABS sheeting in the oven, laid it over the green wooden molds below, and then pressed the frame around it to flatten the edging - this worked surprisingly well. I cut the bottoms of those frames at an angle to contour with the frame, so they ended up fitting really nicely. To address bending of the deck, I put lids on the enclosures and only attached them to the board in the middle, so when the board flexes, the enclosures stay flat to the ground, but gap on the front/back edges. This also keeps dust out of the enclosures and doesn't impact the flex of the deck too much.
![IMG_0630%20copy|666x500](upload://etjnO3NtWr327ln4OiHWug0nC2o.jpeg) ![IMG_5875%20copy|666x500](upload://tXPMOnwneB7YaqnR8zLylRJlulJ.jpeg) 

I bolted the battery through the deck, and used recessed bolts for the vesc enclosure - which I made too big by the way, it was the first one I made. Here's the final product:
![IMG_2359%20copy|374x499](upload://90MYuFppgQJwygrJjY6oZL3j2nM.jpeg) ![IMG_5370%20copy|666x500](upload://nhCcsLL7fDB0lnW9BRAw9cM638x.jpeg) ![IMG_1378%20copy|374x500](upload://xbrQbu3mLxPQPAZGW96oxTJlvWg.jpeg) ![IMG_3593|690x369](upload://exu1M6O2PXrkq9ZLF2lJs55RGHm.jpeg) 


So this thing is scary fast and accelerates well, but it's only pulling maybe 20-25a at full throttle from the battery according to by BMS app. The vesc has master/slave setup, and the master is set to the default 24.9a (give or take an amp I could be wrong). How can I turn this thing up to pull all 50a it's capable of (25a for each vesc4.12 x 2 = 50a from the battery, right?). I've changed it to current mode for the throttle control, but no difference. Tips on this would be greatly appreciated.
```

---
## \#2 Posted by: pingustar Posted at: 2019-08-25T13:05:05.188Z Reads: 45

```
looking great!

I have a question for you. How does your enclosure affect the flex? Most Vanguard builds I have seen use two enclosures and leave the middle part open.
```

---
## \#3 Posted by: YoungDoughboy Posted at: 2019-08-31T17:09:33.460Z Reads: 31

```
I used two enclosures, and only bolted them in the middle of the enclosures, with bolts about 2-3in apart. This is enough to keep them from twisting, but not enough to add noticeable stiffness to the deck. because this means the ends of the enclosures will hang down when flexing, I put lids on the enclosures to keep dust out.
```

---
