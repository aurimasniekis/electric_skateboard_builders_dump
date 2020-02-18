# Pichted sound from battery when charging

### Replies: 10 Views: 214

## \#1 Posted by: rey8801 Posted at: 2018-09-05T19:55:49.232Z Reads: 87

```
Hi guys! Basically I was using my board daily to go to work when suddenly yesterday when I charge the board I heard a pitched sound (not loud) form the battery. I first thought was the charger so I try another one and it seemed to work but then after one minute the same. I open the enclosure and the sound came from battery/BMS. Do you have any idea what can be? Broken BMS? Is it possible to test it? Like my is charge only, if I disconnect the balanced leads from the BMS and try to charge the board than would be the same as not having a BMS? It's just to understand if actually a battery can make sound :sweat_smile: it sounds stupid to me but I don't know what to think about it. Thx!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-05T20:00:14.504Z Reads: 85

```
Did you check your cells with a multimeter?
Should be easy if you didn’t packed them totally in heatshrink.
I know just one sound which cells can make but this sound is scary and would already mess up all what’s around them 😬
```

---
## \#3 Posted by: rey8801 Posted at: 2018-09-05T20:59:41.034Z Reads: 64

```
:joy: Yeh I got which sound. Check the battery overall 39. The cells from 3.9 to 4. One group 3.6. I was going to change the BMS since only charging doesn't balance well. Do you think the sounds comes from the BMS?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-05T21:04:53.279Z Reads: 58

```
Don’t have experience with bms yet but I can’t imagine that it comes from the cells.
Cells can only release gas but that would sound different. So than there not so much oportunitys left right?
Which bms you have? Just interested as I plan to go charge only too for the next build and if you say it’s not working well I shouldn’t buy the same 😅
```

---
## \#5 Posted by: rey8801 Posted at: 2018-09-05T21:13:28.790Z Reads: 50

```
I know the sound of degassing cells since I punctured some test ones while I was building the spot welder. Not the case now. I hope it's only the shit bms. Anyhow I used one from Ali https://www.aliexpress.com/item/10S-60A-bms-Li-ion-large-high-current-BMS-PCM-with-SAME-discharge-port-for-electric/32829800932.html?spm=a2g0s.9042311.0.0.27424c4doLEYok 10 was working fine as discharge/charge, but charging only doesn't work well. Now I am getting another one from the same seller with a bluetooth module attach so that you can actual monitor the cells and it was advice from the forum. Otherwise bestech is a good one. Now I am actually thinking of add one group in series and go 11s, but I really have not that much space under the enclosure. Anyhow I am going to get the 75Kv version too of the hub I think. More balanced for my battery.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-09-05T21:31:09.875Z Reads: 34

```
I was in communication with Lucy from bestech and she told me that some of there bms don’t work for charge only. Maybe that’s the case with your ali bms too.
Thought about a Bluetooth bms too.
Don’t like the fact that I need to trust the bms without to know the real cell or pack voltage.
I had 11s4p hg2 before without bms but measured the packs after each cycle. A bit more work but with it I was as min sure that the packs don’t drift away from each other.
```

---
## \#7 Posted by: rey8801 Posted at: 2018-09-05T21:33:21.714Z Reads: 37

```
I want definetely avoid to measure cells like now every 3 weeks and charge them separately. Indeed can be that my BMS since made for discharge also doesn't work properly like that. Since with discharge the cells were always fine for over 4 months. About 11s how do you charge it? I don't find normal laptop format charger for 46V.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-09-05T22:31:17.025Z Reads: 25

```
Was charging with something like this 
http://s.aliexpress.com/7JriqM7F

I found one laptop brick too, but only 1,5a
http://s.aliexpress.com/Uje6juMJ
```

---
## \#9 Posted by: rey8801 Posted at: 2018-09-05T22:42:06.345Z Reads: 23

```
Perfect and as BMS I guess a 12s used as 11s.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-09-05T23:03:03.439Z Reads: 22

```
No, didn’t used bms but was planed and ordered 11s bms from bestech. Just got lostet in transit so I ended up without using a bms.
It’s not a problem to get a bms for 11s thou.
Most smart bms even possible to adjust from 6-12s or so
```

---
