# How much A for a two motor setup (10s8p)

### Replies: 44 Views: 1698

## \#1 Posted by: Alex.Scheff Posted at: 2018-02-28T18:41:12.676Z Reads: 235

```
Hello,
I'm alex from Germany and I'm a bit confused.
I will make a battery 10s8p (panasonic ncr18650b) with a max discharge current of 52 Amps (bms max discharge current of 60A) I will use two 6355 motors (2400W 230kv maxA 60A) from alienpowersystem.
Also I use two vesc from maytech with a max current of 50A. Now my question, do I need a battery with a max discharge of 50A or 100A to power the two vesc with the motors on it?
Thanks!
Akex
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-02-28T18:45:06.750Z Reads: 235

```
No, you dont need a battery with a Max discharge of over 50A discharge. Its recommended thouht.. The 50A is the max the vesc can take, it doesnt have a limit for how low it can take :slight_smile:
```

---
## \#3 Posted by: Acido Posted at: 2018-02-28T18:46:11.921Z Reads: 229

```
Do not trust max motor ratings, my motor is rated up to 3000W but maxes out at 1600W
```

---
## \#4 Posted by: Alex.Scheff Posted at: 2018-02-28T18:48:44.292Z Reads: 219

```
Yes I agree but thr motors from alienpowersystem are pretty good
```

---
## \#5 Posted by: Alex.Scheff Posted at: 2018-02-28T18:52:25.771Z Reads: 204

```
@FredrikHems Sure but I don't know If the motors get enought amps😅
```

---
## \#6 Posted by: Acidfie Posted at: 2018-02-28T19:11:24.739Z Reads: 193

```
100A, every VESC on max. discharge will draw about 50A for peak limits, also if you have an 10S8P packs will the max discharge current not much.

why did you choose those cells? 

the ncr18650b are rated at 2C which means like 6,2 Amps per Cell, this multiplied by 8 because of the paralel wiring will be summa about 50A continous discharge current! this ist not very much, i used the sony vtc5 and they have about 30A per Cell at 3P it is about 90A **cont!**

add: also, using a bms with that discharge current is a bad idea, becaus amp peak spikes could be much larger than the bms can handle! only use the bms for charging, not for discharging.
```

---
## \#7 Posted by: Alex.Scheff Posted at: 2018-02-28T19:14:26.068Z Reads: 179

```
@Acidfie I choosed the cells because of the 3400mAh but forget to check the max dicharge current, very dumb.
I will change to some other cells to reach the 100 Amps.
Thanks for your reply
Alex
```

---
## \#8 Posted by: Alex.Scheff Posted at: 2018-02-28T19:15:43.778Z Reads: 175

```
@Acidfie What should I do with the bms, no bms? A Li-Ion charger?
```

---
## \#9 Posted by: Acidfie Posted at: 2018-02-28T19:21:01.947Z Reads: 172

```
well, theoretically you'll need 100A. it is like @Acido said, never trust motor specifications. 

someone had a table a few days ago, which current is realistically drawn cont. it was about 30-40A but i am not sure if 1 motor or 2. you could be safe with 52 discharge.

better look for some cells with about 10A **if** you are using 8P, which is fucking much capaticity.

you'll need a bms for balancing the cells, you can get pretty cheap ones from china at ebay, just search for "BMS 10S 40A" -they cost around 10-20€ but they will do the trick! just be sure to connect them correctly. i have one bms lying around here, just dm me, bin auch aus D ;)

You'll need a CCCV charger, there you'll be at about 30-50€, its not that expensive!
```

---
## \#10 Posted by: e.board_solutions Posted at: 2018-02-28T21:03:38.758Z Reads: 147

```
You could also use LiPo cells than will 1P be fine ;)
```

---
## \#11 Posted by: Alex.Scheff Posted at: 2018-02-28T21:17:35.037Z Reads: 133

```
@e.board_solutions Hm I don't know, if I use LiPo I really don't have much mAh
```

---
## \#12 Posted by: b264 Posted at: 2018-02-28T21:24:30.793Z Reads: 133

```
For an 8P pack try to use Samsung 35E or Samsung 30Q or Panasonic PF cells
```

---
## \#13 Posted by: E1Allen Posted at: 2018-02-28T21:38:06.734Z Reads: 126

```
What size of board are you putting these cells in?
```

---
## \#14 Posted by: michaelcpg Posted at: 2018-02-28T21:41:29.685Z Reads: 123

```
https://ru.nkon.nl/sanyo-18650ga.html

If you're looking at using Panasonic cells I'd recommend these ones, they should work really well in a battery that size
```

---
## \#15 Posted by: Alex.Scheff Posted at: 2018-02-28T21:54:24.807Z Reads: 117

```
Thanks! I will check them out
```

---
## \#16 Posted by: Alex.Scheff Posted at: 2018-02-28T21:55:21.321Z Reads: 113

```
I will make a pintail with a lenght of 110cm x 23cm
```

---
## \#17 Posted by: Alex.Scheff Posted at: 2018-02-28T21:55:59.668Z Reads: 111

```
Thank you, I will check them out!
```

---
## \#18 Posted by: E1Allen Posted at: 2018-02-28T23:32:25.227Z Reads: 97

```
80 batteries is quite a few for a110cm pintail.  I'd go with the higher output cell recommendations so you can lower the price count.  Check out some other build logs to see other users setups
```

---
## \#19 Posted by: Alex.Scheff Posted at: 2018-03-01T06:04:30.230Z Reads: 87

```
I would make the battery very flat, so it has a lenght of 40cm, is this to long?
```

---
## \#20 Posted by: FredrikHems Posted at: 2018-03-01T06:32:49.016Z Reads: 83

```
Depends if your board flexes or not
```

---
## \#21 Posted by: E1Allen Posted at: 2018-03-01T06:35:39.510Z Reads: 80

```
Very flat means one layer 40 batteries 2 wide is almost 73cm in batteries alone.  Single stacked
```

---
## \#22 Posted by: Alex.Scheff Posted at: 2018-03-01T06:35:40.187Z Reads: 77

```
No I make it totalelly flat, maybe a 18mm or 21mm thinkness
```

---
## \#23 Posted by: Alex.Scheff Posted at: 2018-03-01T06:36:35.748Z Reads: 78

```
No sorry I mean two lines of cells next to each other
```

---
## \#24 Posted by: E1Allen Posted at: 2018-03-01T06:50:17.566Z Reads: 71

```
If you are still doing 10s8p that's 80 batteries.  If you do two cell across and 40 cells down that's a single layer 73cm long
```

---
## \#25 Posted by: Alex.Scheff Posted at: 2018-03-01T06:54:52.524Z Reads: 68

```
No, sorry I cant explain it good, on the 40cm (22 cells) cell layer will be another cell layer with a lenght of 33cm  (18cells) and all this will be two times next to each other. So I will have a flat but big battery pack.
```

---
## \#26 Posted by: michaelcpg Posted at: 2018-03-01T07:02:48.867Z Reads: 66

```
2 layers of cells is closer to 36mm rather than 18 - 21mm
```

---
## \#27 Posted by: Alex.Scheff Posted at: 2018-03-01T07:22:30.347Z Reads: 66

```
The 18 or 21 mm are the board wood thickness
```

---
## \#28 Posted by: E1Allen Posted at: 2018-03-01T08:38:21.186Z Reads: 62

```
Just measure it out on paper and put it on your board to help with layout.
```

---
## \#29 Posted by: Alex.Scheff Posted at: 2018-03-01T08:45:44.869Z Reads: 61

```
Yes I will make an exact plan, as soon as I'm done I will show it
```

---
## \#30 Posted by: laurnts Posted at: 2018-03-01T09:09:59.936Z Reads: 62

```
Motor max amp doesn't mean motor continuous amp. Your motor max or vesc max draw is 50 amp, but if you check vesc log, normally you will only draw 2 - 3 amp with 1 sec of 30A++ during startup or sudden jolt of speed. If you draw continuous 50A, you have something wrong.
```

---
## \#31 Posted by: rene Posted at: 2018-03-01T10:00:17.845Z Reads: 59

```
[quote="Alex.Scheff, post:1, topic:47773"]
6355 motors (2400W 230kv maxA 60A
[/quote]

I would use much less KV, because more KV less Torque!
130 or 170KV ist besser und mehr Drehmoment.
```

---
## \#32 Posted by: Alex.Scheff Posted at: 2018-03-01T10:05:05.765Z Reads: 59

```
Okay I will use the 190kv model
Danke!
```

---
## \#33 Posted by: Alex.Scheff Posted at: 2018-03-01T10:05:36.165Z Reads: 60

```
Okay and how much amps would be perfect?
```

---
## \#34 Posted by: pat.speed Posted at: 2018-03-01T10:16:18.616Z Reads: 60

```
If you can get a battery that will discharge 80a or more that is perfect. That way you can setup each Vesc to 35-40a each and still be under your total pack current.

Good Luck👍
```

---
## \#35 Posted by: pixelsilva Posted at: 2018-03-01T10:32:37.182Z Reads: 60

```
Why the resistance in adopting the 35E ? Everybody jumps inmmediately when we mention the 35E. Your stats showed they were the thing to follow...but noooo..... the still believe 30Q are much better. Then?
```

---
## \#36 Posted by: michaelcpg Posted at: 2018-03-01T10:44:38.900Z Reads: 59

```
It depends on the battery size. For most people using something like 3p or 4p, 30q potentially makes more sense due the the higher current output and lower sag at >10A per cell. For larger packs like this there a better cells
```

---
## \#37 Posted by: Alex.Scheff Posted at: 2018-03-01T10:52:47.160Z Reads: 60

```
I found some cells with a discharge of 10A. With a 10s8p I will have 80A, I think this is enought
```

---
## \#38 Posted by: michaelcpg Posted at: 2018-03-01T10:53:19.598Z Reads: 58

```
Should be plenty. What cells you looking at?
```

---
## \#39 Posted by: Alex.Scheff Posted at: 2018-03-01T10:54:30.913Z Reads: 60

```
The Sanyo NCR18650GA 3500mAh 10A, do you think they are good enought?
```

---
## \#40 Posted by: michaelcpg Posted at: 2018-03-01T10:57:06.342Z Reads: 60

```
That's the same model cell that I linked before. They should be really solid cells from the reviews I've seen. I'm using around 100 of them in my MTB I'm working on atm
```

---
## \#41 Posted by: Alex.Scheff Posted at: 2018-03-01T10:58:11.187Z Reads: 60

```
Okay perfect, thank you
```

---
## \#42 Posted by: Acidfie Posted at: 2018-03-01T11:55:39.118Z Reads: 58

```
Found it!

thanks to @DeathCookies 

interestingly with **_50% throttle_** / 40V

5km/h - 65 watts “available” - 1.6 battery amps
10km/h - 370 watts “available” - 9.25 battery amps
15km/h - 545 watts “available” - 13.62 battery amps
20km/h - 687 watts “available” - 17.17 battery amps
25km/h - 835 watts “available” - 20.87 battery amps
30km/h - 985 watts “available” - 24.62 battery amps
35km/h - 1155 watts “available” - 28.87 battery amps
40km/h - 1208 watts “available” - 30.2 battery amps
45km/h - 1154 watts “available” - 28.85 battery amps
49km/h - 909 watts “available” - 22.72 battery amps
```

---
## \#43 Posted by: Alex.Scheff Posted at: 2018-03-01T12:03:00.811Z Reads: 54

```
@Acidfie Theoretical I just need 60A from the battery to power two motors?
```

---
## \#44 Posted by: Acidfie Posted at: 2018-03-01T14:11:06.161Z Reads: 49

```
with exact this setup, on the paper!

1. I dont know which motors and ESC he used.
2. I don't know his gear ratio/wheel size
3. I don't know his weight
4. Did he testet it uphill/downhill/straight?
5. He used 50% throttle, are these properties linear if going to 100%? or do they correlate exponential?

You can't say that for everyone, but you can try calculate it here [CLICK ME HARD](http://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii)

Although you will need a maximum of peak discharge 120A, because your two motors can draw that at max.

The VESC can boost up to 240A at peak.

So i think a continous discharge of about 60-80 would be enough for your setup. Better more than less.
```

---
