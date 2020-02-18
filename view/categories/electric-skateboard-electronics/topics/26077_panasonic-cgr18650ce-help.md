# Panasonic CGR18650CE Help

### Replies: 18 Views: 1889

## \#1 Posted by: Chigzy Posted at: 2017-06-24T12:13:51.073Z Reads: 90

```
Ok, so I managed to win a bid of 10 Toshiba Laptop batteries for £50.
Ive cracked open a few and it appears they hold Panasonic CGR18650CE Cells. Does anyone know their Amp rating or if they will be suitable for an Electric Skateboard battery. Tried doing searches, but cant seem to find anything on the Amp rating. 

Can anyone chime in :slight_smile:
```

---
## \#2 Posted by: pat.speed Posted at: 2017-06-24T12:53:04.623Z Reads: 89

```
Sorry to say mate but I don't think they will work unless you have about 15 cells in parallel. It is certainly possible though and others have done it
```

---
## \#3 Posted by: Chigzy Posted at: 2017-06-24T13:11:39.233Z Reads: 85

```
That's unfortunate :(  out the 90 cells I've took out. 60 of them are above 3.4v. None of the others are below 2.4v. This is going to be my first battery build so it's a practice run. Before I buy brand new cells. Looking to test a 10s6p or 12s6p. What's the Mac rating you think I can set in the vesc for these. Don't really care if I fry them tbh. It's more for learning as its my first battery build
```

---
## \#4 Posted by: Alan_Smithee Posted at: 2017-06-24T14:22:51.197Z Reads: 74

```
I have these cells in [my spreadsheet](https://docs.google.com/spreadsheets/d/1fYjDxxCJXfm2wdpGWCaOUGq8V8TOEgsnplHQa4YQpRQ/edit#gid=0) but I never managed to find any stats for them other than that they are 2200mAh probably.

The 2.4V cells are probably still good to use, but you have to meassure the cell capacity of ALL cells. Charge them up (to 4.1V), let them sit for at least 2-4 weeks and sort out the cells that dropped to much voltage in that time (shouldn't be much more than 100mV). For capacity testing you cells, I recommend something like the [opus bt-c3100](http://www.gearbest.com/chargers/pp_173012.html) charger.

Since they come from Laptops, we have to assume they can do 5A tops.

To save on amperage draw of you board you would have to make it as high voltage as possible. What kind of motor or esc are you planning to use?
```

---
## \#5 Posted by: Tuomalar Posted at: 2017-06-24T14:51:43.017Z Reads: 63

```
I would say that you just wasted 50£. It's common mistake to try make a battery from laptop batteries. Those just can't deliver enough power.
```

---
## \#6 Posted by: Chigzy Posted at: 2017-06-24T16:19:54.013Z Reads: 53

```
Will be using the Vesc and enertion Rspec 192kv. Is that any good
```

---
## \#7 Posted by: Tuomalar Posted at: 2017-06-24T16:22:56.745Z Reads: 51

```
You have to put like 16 of those in parrallel to get enough discharge. And then 10 in series.
```

---
## \#8 Posted by: Chigzy Posted at: 2017-06-24T16:50:33.903Z Reads: 49

```
I've got 90 cells so max I can do is a 10s9p. I'll try it anyways. Not going to have high expectations tbh just more for learning how to build a pack.
```

---
## \#9 Posted by: smurf Posted at: 2017-06-24T18:20:47.871Z Reads: 47

```
Test the cells discard the ten worst performers. You should be fine with 10s8p taking a few precautions. I highly recommend a quality BMS with thermal temperature probe (it's reusable) definitely set the Vesc to draw no more than 40A
```

---
## \#10 Posted by: Alan_Smithee Posted at: 2017-06-24T19:48:56.500Z Reads: 46

```
that would leave you with 40A max. Thats usable current.. however.. fitting 90 cells to a board is kind of tricky

this is my 10s6p pack and its already pretty bulky:
<img src="/uploads/db1493/original/3X/2/4/2483b398f87324601054bcedfb62bc9dc423495f.jpg" width="690" height="388">

definitely make sure to capacity test every cell though, because you will have to design your battery with every parallel pack having the exact same capacity. if not you will wreck your battery in no time.
```

---
## \#11 Posted by: Chigzy Posted at: 2017-06-24T21:37:01.936Z Reads: 41

```
Any recommendations on the Bms. I'm new to this. Not sure what to look for. Been testing a few , charging and discharging. Omggg. This takes ages lol. What's the max I could charge and discharge these using the charger I have. Imax v6 , I'm currently charging a single cell which was at 3.4v and its taken 1500 mah so far. Been stuck on 4.2 for a while though.
```

---
## \#12 Posted by: Chigzy Posted at: 2017-06-24T21:40:43.026Z Reads: 39

```
It will be a challenge getting the 80/90 cells to the board. I might make a cube type battery and strap it to the top , rather than underneath and have it lay between my feet on the board.
```

---
## \#13 Posted by: Alan_Smithee Posted at: 2017-06-24T21:47:10.303Z Reads: 39

```
I won't charge them faster than 1A. I would always discharge test at 1A. This way you get the most capcity out of them. It won't be the real capacity you'll get in the field since you are going to run them at their limits all the time, but for comparing the individual cells I'd go with 1A.

I stopped using the imax for capacity testing since it can only do 1 cell at a time. one of those $30 opus chargers can discharge test 4 at a time. also I think the imax is limited to 1A discharge testing while the opus can either do 4 at 1A or 2 at 2A.

As for the BMS.. I don't use one since my setup will never draw more than the battery can provide. I only use one of those $15 ones off ebay for balance charging the pack.

For you setup I would highly recommend using a BMS though.. one that limits current drawn from the battery to no more than 40A (get a fuse, too). don't know wich one is good though.. I would just try one of those 10S 40A ebay ones.
```

---
## \#14 Posted by: chuttney1 Posted at: 2017-06-25T21:35:01.564Z Reads: 30

```
Putting 90 cells are starting to become more problematic. You're extra weight. At 45 grams per cell, the whole pack weighs 4.05 kg or 8.91 lbs. Not counting the nickel strips, solder, balance, wires, and the possibility of using the plastic cell holders.
```

---
## \#15 Posted by: Chigzy Posted at: 2017-06-25T21:50:15.225Z Reads: 30

```
Im not too fussed about the weight for now, this is more for learning and tinkering. Then when I get the hang of things, I will be building a better battery using BASEN 26650 4500mah, or maybe the Samsung 25R cells. Just seeing how it goes.
```

---
## \#16 Posted by: Chigzy Posted at: 2017-06-26T04:28:33.719Z Reads: 26

```
Quick update. After getting to grips with 18650 cells and the IMAX V6, ive started to properly test the cells. The 2 I have, I charged to 4.2v and discharged them at 1A each. Good news, First 1 measured 2084mah, and the second one is 2122mah

Considering I have to build a 9P pack, it may end up being big and bulky, but have a decent Ah. Only time will tell.
```

---
## \#17 Posted by: Okami Posted at: 2017-06-27T13:14:21.962Z Reads: 18

```
@Chigzy  ah tells us how it looks later on.. Otherwise, wish you a good start with harvesting enough good cells to make a pack out of them ;)
```

---
## \#18 Posted by: Challlsss Posted at: 2017-06-27T15:40:47.876Z Reads: 16

```
Just replace the deck with batteries.... Problem solved
```

---
