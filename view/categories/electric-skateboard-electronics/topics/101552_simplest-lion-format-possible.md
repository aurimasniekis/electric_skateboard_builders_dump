# Simplest LiON format, possible?

### Replies: 7 Views: 160

## \#1 Posted by: beherit Posted at: 2019-09-09T20:42:09.371Z Reads: 77

```
Hi! Not particularly Esk8 based but this seems like the best place to ask. I'm working on a portable single board computer with the intention of being buildable at home by most hobbyists and I'm wondering what would be the best way to replicate the laptop battery format. I figured I'd ask here first to make sure I don't ruin a couple cells.

If you were to connect 4 cells in series, end to end, could it be charged evenly through a cheap battery charging board such as [this](https://www.aliexpress.com/item/32835132061.html) provided they're all the same cell and inserted with the same charge?
```

---
## \#2 Posted by: Hummie Posted at: 2019-09-09T21:04:43.576Z Reads: 71

```


 if youre trying to replicate how batteries are charged in computers you'd need a bms to control the voltages of all cells in series.  youd need four of those things assuming they charge to 4v about.  even then im not sure you could run 4 of them at once to a connected battery being fed from your one power source without a short. don't read Russian though.
```

---
## \#3 Posted by: beherit Posted at: 2019-09-09T21:11:30.757Z Reads: 64

```
Hmm, wouldn't 4S1P with a single group BMS like I linked be the same as how those generic portable batteries packs work though? I thought you only needed a BMS when it came to keeping multiple parallel groups at the same charge.
```

---
## \#4 Posted by: Afrovis Posted at: 2019-09-09T21:14:09.768Z Reads: 57

```
The biggest reason you need a BMS is because all cells in series will fluctuate in voltage, because the internal resistance differs and thus the charge/discharge rate differs ever-so-slightly. Even with cells from the same batch.
```

---
## \#5 Posted by: Afrovis Posted at: 2019-09-09T21:17:50.668Z Reads: 53

```
BMS is for batteries in series. Parallel batteries keep the same charge by themselves just because they are connected. Current will flow between the cells to equalize.
```

---
## \#6 Posted by: beherit Posted at: 2019-09-09T21:19:22.163Z Reads: 53

```
I see. So series is unrealistic without a 4S BMS, but could I do parallel with that board and get reasonable results?

EDIT: On second thought, I suppose 2S2P would be the best solution for voltage higher than 3.6V.
```

---
## \#7 Posted by: Tinp123 Posted at: 2019-09-10T05:23:41.361Z Reads: 36

```
you can install 1s bms on each cell and then connect them in series to get 4s1p. but I don't see why, you can get 4s bms for cheap
```

---
