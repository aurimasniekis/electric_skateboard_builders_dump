# Help needed dual bms vs 2 battery in parallel

### Replies: 9 Views: 1560

## \#1 Posted by: pedr0g0mes Posted at: 2017-11-02T17:32:19.182Z Reads: 141

```
Hi everyone, this is my current setup, my doubt is can i safelly charge this setup even tough the batteries are connected in parallel ? i know the batteries tend to balance betwen them, i really wanted to maintain the 2 bms so i can accurately charge each cell, by the way the discharge phase is bypassed so i just wanted to use them to charge.
<img src="/uploads/db1493/original/3X/f/0/f0c37ceb5e7c96ed84b32601d0dfe4760fd6bc01.jpg" width="690" height="252">
```

---
## \#2 Posted by: pat.speed Posted at: 2017-11-05T11:10:49.010Z Reads: 90

```
If you just connect the balance leads in parallel you can charge it with one bms. The cells will stay perfectly balanced as they did before
```

---
## \#3 Posted by: pedr0g0mes Posted at: 2017-11-05T11:29:18.079Z Reads: 88

```
Thanks for the reply, the thing is I have 2 chargers instead of buying an expensive one, I bought 2 2A 42v chargers (7£ each) thats why I wanted to use two bms to make the charging time faster,but if I charge one of them thru one BMS, eventually i will balance the cells from one pack at the same time that will increase the total voltage of the other battery without balancing it right? Or if I charge the two bms at the same time is any danger of burning anything? I didn't though this before unfortunately xd
```

---
## \#4 Posted by: pat.speed Posted at: 2017-11-06T02:55:14.997Z Reads: 84

```
I'm not sure I quite under stand, but there was a thread on this and it was found that you can use two bms to charge one pack
```

---
## \#5 Posted by: jmasta Posted at: 2017-11-06T04:12:58.581Z Reads: 77

```
Technically you could just wire your chargers' outputs in parallel. Then you'd have a "4A" charger with two AC plugs. Only one BMS needed.  If you felt so inclined you could even wire the AC inputs in parallel as well

Or put two charge ports on your board, wired in parallel internally. Then you could use one or two chargers
```

---
## \#6 Posted by: HumanMint Posted at: 2017-11-11T04:44:58.797Z Reads: 66

```
This may sound weird. (and probably obvious)

I currently have a 10s bms rated for "less than 8a" charging that I am planning to use for charging only.  I am running a 6Ah 10S2P setup (4 x 3Ah 5S1P). I ordered a 4a charger online, then fiddling arounf this website made me find your post.

If I get an extra 2a charger online and solder either the 2 chargers in parallel or the 2 charging ports in parallel does this mean I will get 6a charging? If it is correct is it worth it? (battery life and whatnot)
```

---
## \#7 Posted by: b264 Posted at: 2017-11-11T04:52:53.338Z Reads: 59

```
[quote="HumanMint, post:6, topic:37193"]
... I am running a 6Ah 10S2P setup (4 x 3Ah 5S1P) .... does this mean I will get 6a charging ...
[/quote]

I think a question that needs to come before that is, can you charge at 6A without damaging your cells?  2P is kind-of shallow to get that heavy on the charge rate.  But without more info and not being an expert myself, I can't say for sure
```

---
## \#8 Posted by: HumanMint Posted at: 2017-11-11T05:07:23.184Z Reads: 54

```
Cuz I know the max charge amps is 6a for my setup, so I wanted to have slightly faster charging as an option in case I'm in a bit of a hurry in like a cafe or something. I understand that higher amp charging shortens the life of my lipos therefore I dont want to max out the 6a and go for a decently low 4a
```

---
## \#9 Posted by: pedr0g0mes Posted at: 2017-11-14T15:52:41.615Z Reads: 46

```
Thank you all for the replys i'll probably wire them in parallel then ! i was afraid of burning something that's why i haven't done it before eheh.
thank you guys for all your help !
```

---
