# 10s battery pack low profile(UK)

### Replies: 11 Views: 1276

## \#1 Posted by: geohan Posted at: 2016-10-18T09:28:28.214Z Reads: 168

```
hi there, i am looking to build a pretty low profile board, but i cant decide on how i want to do the battery pack. I was thinking of do 5 2s packs and wire in series to get a 10s pack. and as 2s packs are pretty small they wouldn't stick out much from the bottom of the board.

The problem with this is how I would charge all the batteries, as charging 5 batteries separately doesn't really appeal to me. I have looked at BMS's but I cant seem to find any 10s suitable products.

Does anyone have any ideas on how I could charge them all together or in two smaller packs?
```

---
## \#2 Posted by: lox897 Posted at: 2016-10-18T09:36:26.398Z Reads: 170

```
Maybe 2 packs of 5s3p and wire them in series when you are on the board, then when you aren't unplug them and charge. Or just do one 10s3p and get a bms from supower
```

---
## \#3 Posted by: TarzanHBK Posted at: 2016-10-18T09:38:39.346Z Reads: 166

```
sounds like you want to use lipo.

if you want to use a bms, just search for something like that:
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html
then you can charge them with a laptop style charger.

other option is like you suggest charging 2 packs seperatly (one 4s + one 6s) with a balance charger like an imax b6.
therefore connect the packs in series and wire the balance cables together to get a 4s and a 6s pack.
```

---
## \#4 Posted by: geohan Posted at: 2016-10-18T09:42:43.169Z Reads: 156

```
the two packs (6s+4s) does seem like a good idea, could you link a video or thread for a wiring tutorial for batteries in series?
```

---
## \#5 Posted by: lox897 Posted at: 2016-10-18T09:43:34.942Z Reads: 149

```
Go 5s and 5s not 6s and 4s. Not as good for batteries.
```

---
## \#6 Posted by: geohan Posted at: 2016-10-18T09:45:15.368Z Reads: 143

```
how can you wire 2s packs into 5s pack
```

---
## \#7 Posted by: TarzanHBK Posted at: 2016-10-18T09:51:56.058Z Reads: 138

```
thats the problem! i´m talking about charging wireing! If in use, put all 5 2s batteries in series.
So charging with an bms is much easier than that.

Also better than your 2s plan: two 5s like @lox897 mentioned and you could lay them out flat. (Should be a tutorial somewhere)
```

---
## \#8 Posted by: geohan Posted at: 2016-10-18T09:54:42.939Z Reads: 127

```
yea that makes sence
```

---
## \#9 Posted by: geohan Posted at: 2016-10-18T09:56:27.914Z Reads: 128

```
also, i known its not related to this topic but is it bad to run a motor at its max voltage, say 10s battery with 10s motor when battery is fully charged?
```

---
## \#10 Posted by: lox897 Posted at: 2016-10-18T10:00:32.921Z Reads: 128

```
No it's fine
```

---
## \#11 Posted by: rpasichnyk Posted at: 2016-10-18T12:26:31.031Z Reads: 111

```
I would strongly advice you to look at @whitepony builds. They are ultra slim. And he always has good photos of his builds so you can figure out the layout. He doesn't use BMS because good cells usually do not drift at all. Seriuously, read his build threads.
```

---
