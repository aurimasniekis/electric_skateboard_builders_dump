# The REAL capacity of your battery pack

### Replies: 3 Views: 269

## \#1 Posted by: bartroosen12 Posted at: 2018-10-14T11:10:20.621Z Reads: 120

```
Hi everyone!
I'm riding my new build for like 1000km and it still runs great! I just want to share some of my thoughts about my battery pack.
I'm just thinking about getting more range out of my pack because I think it can be better. I'm very happy with the max range I get now (25km agressive riding + 5km normal riding)

This is my board:
![IMG_20180920_172058|666x500](upload://nlJxOqIRWUltbUBhLaCt23AVfQv.jpeg) ![IMG_20180920_171349|666x500](upload://4apvaoXIH5bxwb9mzfythBGiKhw.jpeg) ![IMG_20180923_231849|666x500](upload://vaZJ7Q8353GUX4PZVmosr60djy9.jpeg) 
10S4P 30Q pack
60A bluetooth bms
Ownboard hubs
Ownboard esc
2A 41.5V charger

I discovered that if the battery hits around 3.5V / cell the board slows down and will completely stop at 3.2V / cell.
This is normal and programmed in the esc which is actually pretty healty for the batteries.
![IMG_20181014_123729|690x388](upload://wABak2r9H81Ii905PeECIoJzCZn.jpeg) 

I can do around 25km of agressive riding and after that it gets 'boring' but it will still ride for like 5km.
I did a 25km ride yesterday and the board started so no boring ride and charged it (only took 4h)
I use a slow 2A charger and it charges at real 1.8A (I can see this in the bluetooth app from my bms) so that means 1.8A x 4h = ~7Ah

Now I was just inspecting the graphs of the samsung 30Q and chose the curve that shows these average values, so 7 / 4 = 1.75Ah / cell.
![IMG_20181014_131724|690x388](upload://4zyh24kRRGTIDbe3ElIwJl9GYVQ.jpeg) 

I was just thinking to use the new flipsky dual vesc so I could adjust the cut off voltage to get more range out of these beautiful cells.
I know the cells need to put out much more current when going to a lower voltage but I'm not planning to pump up the amps of the motors, just set them on 10A per motor (now I pull 9A per motor and its fine for me)
So I can ride 'agressive' for a longer time.

Has anybode ever switched from the standard hub esc to a vesc and got a much better range/performance of their battery?
```

---
## \#2 Posted by: pat.speed Posted at: 2018-10-14T11:32:12.451Z Reads: 98

```
I have switched to a vesc from a dual esc and noticed better performance but not really range as I never discharge my lipos below 3.6v so I don’t hit the cut off.

However I do know that 18650 cells can safely discharge down to 2.8v and judging by that graph you would get an extra 4ah total or another 10-15km of range. That could be pushed further by dropping the cut off to 2.5v but that will lessen cycle life and potentially harm the cells
```

---
## \#3 Posted by: Acido Posted at: 2018-10-14T11:35:58.386Z Reads: 95

```
You can choose battery life (more charges, more miles out of it)

Or you can choose less range but longer life
```

---
