# Curious about amperage draw of 500watt diyeboard hub motors

### Replies: 7 Views: 1113

## \#1 Posted by: schertza Posted at: 2018-08-06T19:41:19.848Z Reads: 138

```
I’m new to all this and I basically built up a board from diyeboard.com

I put together a diyeboard.com10s5p battery, their V2.1 ESC, and their dual hub motor 1000W75KV Power Truck (2 500W motors). The board works and I enjoy riding it around.

I found the board to be really heavy. (50 cells) And I only have a 1.5 mile commute to work, so I did not need a whole lot of capacity, so I decide to try and build up a board, with a new battery pack from 20 cells.

I thought at first I just wanted a 10s1p so I ordered up 10 2500ma LG cells.  But before I tried them out, I ordered another 10.

I knew that I needed a BMS and I wanted something relatively quick, (I live in the US) so I ordered this from amazon: DC42-45V Input Battery Protection BMS PCB Board for 10 Packs 36V Li-ion Cell Max 40A w/ Balance.

(In fact I order two of them)

I blindly ordered the 40a BMS’s (Output current up to 30A) without really understanding how much current my twin 500watt motors pull. Could it simply be 500watts divided by volts (~39) to equal 12.8 amps per motor?

So my game plan was to use 1 BMS with a 10s1p cell configuration. and the other BMS for other 10s1p cells, then place the two 10s1p packs in parallel for what might be considered a 10s2p pack with 2 40A BMS.

I guess my question is does anybody know how much current my diyeboard twin 500watt motors actually pull? Will my two BMS’s work in the configuration that I proposed?

Thank you in advance, and forgive me if I should be posting in a different catagory,

alan
```

---
## \#2 Posted by: rey8801 Posted at: 2018-08-06T20:00:15.084Z Reads: 127

```
Hi. Here my telemetry from dual vesc configured as showed and paired with diyeboard 76Kv 500w hub motors drive and a 10s3p battery Samsung 30Q capable of 60A max continuous current (is the battery that limit the current drawing and so decide which BMS to use). My BMS is configured as charging only. As you can see during the hardest acceleration I barely reach 1600w put of the 2200w capable and set. The max motor current is like about 50A from the sum of the two motor (25A each) even if they are rated up to 50A. The max battery A is around 40A (20A each), well below the 60A max capable. So in your case you have to calculate the continuous discharge current of your battery pack, but I bet it's above the 40A required and the limit of type BMS. So you can probably run the 10s2p battery pack with only one 40A BMS in configuration charging/discharging or wire it in charging only and forget about it since the current drawing is not limit anymore. ![vescmonitor|281x500](upload://zBcHDAhvkNU5NWll16jQsdu38NE.jpg)![vescmonitor|281x500](upload://yuEzJdPQR69R7V7JGQEQ0oFzazw.png)
```

---
## \#3 Posted by: accrobrandon Posted at: 2018-08-06T21:41:01.448Z Reads: 105

```
did you spot weld the batteries or use a vruzend/NESE style kit? based on all the components you mentioned you basically built a meepo/wowgo board with better hub motors as theirs are 250w x 2 ...500w total where as you have 1000w total.

now lets talk about output... a 1p battery based on those cells is gonna suck... im not spending time researching these cells but im gonna assume they can output 10amps continuous as that would be minimum standard for small packs.

the esc can probably max out at 50amps input. and the 10s5p could probably do 50amps output if the bms allowed but probably is set at 40amp.

lets get to numbers.... amps x volts = watts basically..  so that crappy 1p at 10a x 40v max = 500w total... spread over 2 hubs each could receive 250 max watts (someone correct me if im wrong.)

so your half way there...  i dont know if the esc has any max watt settings but assuming not..and if you could pump the 50a continuous that would be like 2000w total... i think... 

honestly you should be fine... i have the same hubs i used to upgrade my meepo... and no issue.. most main demand will be on acceleration then levels drop as you just maintain speed.

to answer the question if linking both 1p batteries in parallel with separate BMSs yes that will work but why?? kind of waste of good space for the parallel connector and extra bms.

just make a 2p and call it a day. a 1p will have shit range and even if your only going a mile who wants a battery "good enough" to get the job done. have the extra juice for extra errands, carving, fun, or even a long mile of aggressive riding with minimal sag.

if it were me id just keep the 5p battery installed and in a few weeks of carrying it around your muscles will grow and it wont feel so heavy any more...but nothing less than a 2p
```

---
## \#4 Posted by: rey8801 Posted at: 2018-08-06T22:44:47.907Z Reads: 77

```
Hi man! One question since you tried both the original meepo hubs and the diyeboard. Do you notice a difference or they are the same? I know they are listed at 500w each compare to 250w, but a lot i people think they are actually the same. I also have the diyeboard one but never tried the Meepo to know it.
```

---
## \#5 Posted by: accrobrandon Posted at: 2018-08-07T00:57:09.899Z Reads: 71

```
well at the time I would say that the diyeboard hubs were a bit more smooth during hill climbing in my area AND i got an early run of the meepos last sept.... i got my brother to order a meepo about 4 months later and when riding his it felt like a slightly better build although there shouldnt be any major differences.

with all that said in retro spect and from what ive learned here in the last year I do wonder if there is any difference between the 2 assuming they both have the same kv and stator size but one can handle more watts ... why can it handle more watts? but assuming all is the same the 500w hubs would have a higher head room thus keeping them cooler.

BUT... since i built a 10s4p dual drive 6355 i havent really ridden the meepo since =P must...have...more...power!!
```

---
## \#6 Posted by: rey8801 Posted at: 2018-08-07T02:25:39.089Z Reads: 61

```
Got it. Yeh they probably are the same. Nevertheless good hubs for the price
```

---
## \#7 Posted by: dareno Posted at: 2018-08-07T05:04:53.805Z Reads: 54

```
Damn son you learn a new thing everyday!  So meepo hubs that are 90mm are only 250w and the diyeboard version which are also 90mm are 500w?  Find that a bit strange as the stator size is identical
```

---
