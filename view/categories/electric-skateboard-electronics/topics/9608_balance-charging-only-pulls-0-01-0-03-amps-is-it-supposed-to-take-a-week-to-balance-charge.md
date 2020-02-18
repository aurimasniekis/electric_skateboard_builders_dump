# Balance Charging only pulls 0.01-0.03 amps, is it supposed to take a week to balance charge?

### Replies: 32 Views: 3057

## \#1 Posted by: itsmikeholland Posted at: 2016-09-14T19:10:22.734Z Reads: 180

```
Hi guys, some of my cells are appearing to stray from 4.2v after a full charge, so i figured it was time to balance things out. However, after 45 minutes my cells are still at the same reading. Is this to be expected with balance charging? I have a Turnigy Accucell 6; so far its been very reliable for fast charging.[Uploading...]()
```

---
## \#2 Posted by: DougM Posted at: 2016-09-14T19:16:12.037Z Reads: 180

```
I had the same problem, mine did that for a couple of days then I heard this popping noise and 2 of the cells were destroyed.

Be sure you've got the charger set for the right kind of battery.  This may or may not have been my problem.

DougM
```

---
## \#3 Posted by: itsmikeholland Posted at: 2016-09-14T19:17:54.957Z Reads: 174

```
<img src="/uploads/db1493/original/3X/d/f/df4025cb2dd1a34ffed2ff79fd27bc3749571379.jpg" width="281" height="500">
```

---
## \#4 Posted by: itsmikeholland Posted at: 2016-09-14T19:24:00.495Z Reads: 165

```
Oh crap! Thats not good. Maybe ill just stick to the fast charging, im definitely in LiPo mode though. Thanks for the input!
```

---
## \#5 Posted by: Pantologist Posted at: 2016-09-14T19:37:38.490Z Reads: 161

```
I believe it helps if your power supply has a sightly higher voltage output.

For example, I use a Boosted charger and my cells are charged at 43.2v yet the charger outputs 43.6. the BMS shots off when fully charged but my cells are still all balanced.
```

---
## \#6 Posted by: DougM Posted at: 2016-09-14T19:40:31.364Z Reads: 160

```
45 minutes I wouldn't worry about, many hours I would worry about.  The other thing you can do if you can reach the connectors is charge each cell individually, then go ride it, then balance charge it.

Do you only have 4 cells or are 2 of them registering zero volts?
```

---
## \#7 Posted by: itsmikeholland Posted at: 2016-09-14T20:15:39.738Z Reads: 153

```
You might be onto something, it looks like my power supply is only pushing 13ish volts. I can still fast charge at 5 amps, so maybe balance charging requires more volts or something. Ill look into a higher voltage power supply in the meantime. Thanks for the input! <img src="/uploads/db1493/original/3X/b/8/b8dbcaa6af8cea8827589faaa06daa047c266213.jpg" width="690" height="388">
```

---
## \#8 Posted by: itsmikeholland Posted at: 2016-09-14T20:46:51.131Z Reads: 141

```
Ah man, i think im a little too inexperienced to charge the individual cells, but thats a solid idea! I have 3 4s batteries, which explains the 0s. I think i might need a more powerful power supply or just deal with the imbalance. I never really discharge it past 80% or so so i dont think i should be TOO worried, right?
```

---
## \#9 Posted by: DougM Posted at: 2016-09-14T20:56:04.361Z Reads: 133

```
Balance charging usually happens in the hundreds of milliamps, so let it run for a couple of hours (monitored) and see how it does.  If you've selected the right battery chemistry you're pretty safe.
```

---
## \#10 Posted by: itsmikeholland Posted at: 2016-09-16T01:41:27.004Z Reads: 117

```
Hey doug, so just a positive update here. I let my charger balance charge for 3 hours and sure enough it did its job! All cells are up to 4.20 and 4.19, i think a weekly balance charge should be in order from now on. One of my batteries had cells all the way down at 4.14 when others were 4.20. Thanks for all your input!
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2016-09-16T01:50:51.689Z Reads: 110

```
You should balance charge evertime you charge lipos. Charge at 1c (5000mah @ 5amps). Long balance times is a sign of bad or poor quality lipos. Hobbyking lipos are a hit or miss
```

---
## \#12 Posted by: itsmikeholland Posted at: 2016-09-16T04:02:18.746Z Reads: 107

```
I would totally balance charge each time but with 3 batteries and one charger, and as long as it takes to gain .5 volts of charge, it would take nearly 27 hours just to recoup my daily morning commute :frowning: . Right now i charge at .75c, which takes about an hour and a half to recoup the 1.8 volts i spend getting to work quickly. I think i just need a more powerfil
```

---
## \#13 Posted by: Titoxd10001 Posted at: 2016-09-16T04:34:42.474Z Reads: 105

```
I think a parallel charging board would be better than not balance charging. I charge my lipos like this (not my photo) and I charged all my batteries one time in 15min because i was in a hurry. <img src="/uploads/db1493/original/3X/7/f/7fb7e4c1a87ad86d46c9627a417b1eb7f904603d.png" width="690" height="388">
```

---
## \#14 Posted by: itsmikeholland Posted at: 2016-09-16T05:45:08.090Z Reads: 97

```
15 minutes would be a dream, thankfully I have 8 hours during the day I can charge. Is it really a huge deal if one cell is lower than the others? I've yet to drain any single cell lower than 3.8 volts since I use the board almost exclusively for my 4 mile commute to work and charge it during the day.
```

---
## \#15 Posted by: Titoxd10001 Posted at: 2016-09-16T06:08:06.447Z Reads: 92

```
I guess it might not be the biggest deal if the voltage difference is not more than .4 volts. Ideally you want them at same voltage for longevity. I'm more worried about overcharging never go above 4.2v per cell
```

---
## \#16 Posted by: lowGuido Posted at: 2016-09-16T06:12:52.341Z Reads: 89

```
it takes so long to balance charge because your cells are so badly of of balance.
you can speed it up by setting your charger to 2S and then charging the 2 cells that are only reading 4.16V
```

---
## \#17 Posted by: itsmikeholland Posted at: 2016-09-16T06:28:08.434Z Reads: 87

```
oh shoot i didn't realize this was possible! I'll try it out real quick!
```

---
## \#18 Posted by: itsmikeholland Posted at: 2016-09-16T06:38:11.978Z Reads: 84

```
meh, no luck. my charger gave me an error saying I had the wrong number of cells selected. Good news is that even with the cells out of balance, "fast" .75C charging has never taken the cells over 4.2, and they've never been drained past 3.8 since my commute is so short. I'll just keep balance charging them every day after the fast charge cuts off until they're back in order, 2 of my 3 batteries are right where they should be with just a .01v variance. Thanks for all of the tips and pointers, lesson learned is to balance charge as much as possible.
```

---
## \#19 Posted by: itsmikeholland Posted at: 2016-09-16T06:41:09.541Z Reads: 86

```
I agree, and also I feel like I'm sacrificing a bit of range with 2 cells being .05 and .04 v off, thats almost an entire volt, which is pretty significant. Thankfully my chargers fast charge setting doesn't take any individual cells over 4.2 before it cuts off, leaving the others at 4.16 and 4.15. I plan to fast charge till it cuts off, then balance charge the other two up as close to 4.2 as I can before I need to ride again. Thanks for all of your pointers!
```

---
## \#20 Posted by: lowGuido Posted at: 2016-09-16T06:45:52.467Z Reads: 86

```
you need to obviously isolate the 2 cells. you cant use the same balance lead. you need to custom make a 2S lead to do it. other wise the charger just wont let you
```

---
## \#22 Posted by: itsmikeholland Posted at: 2016-09-16T07:12:55.862Z Reads: 78

```
that wasn't so obvious, and sounds like a bunch of work for what can be fixed while I work tomorrow with an 8 hour slow balance charge to get things evened out. lesson is learned though.
```

---
## \#23 Posted by: lowGuido Posted at: 2016-09-16T07:14:05.246Z Reads: 79

```
when you use the balance charge function on your charger it does a funny little dance with a series of resistors across each cell. when a cell reaches 4.20V it stop charging all cells puts a resistor across that cell and waits for it to drain down to 4.19V and then starts charging all cells again. 
the reason it takes forever to charge is because it is in fact NOT charging but rather discharging your 4.20V cells ever so slowly, before ever so slowly trying to charge all the other cells only to be stopped again by the high cell. this dance continues, charging and discharging 0.01V up and down for hours at a very low amperage.

the only way to stop this is to individually charge each low cell up to 4.20V (or at least whatever voltage the high cell is at) via the balance connector.
setting your charger to 1S or 2S accordingly.. you will likely need to custom make a cable for 2S but 1S cables are probably provided with your charger.
```

---
## \#24 Posted by: dinodave Posted at: 2016-09-16T07:17:58.027Z Reads: 77

```
My apologies for my previous post which is now withdrawn, it was not very friendly to @lowGuido, I meant no offense. I think I have been a bit spooked by this thread: http://www.electric-skateboard.builders/t/exploding-lipo-batteries-is-no-joke/9634?u=dinodave 

I don't believe most people should try to screw around with what @lowGuido is recommending here however. If you know exactly what you are doing and have full faith in your charger and wiring, by all means, it could sort out your problem. It's just that there are possibilities things could go wrong if you make a mistake, so please be careful.
```

---
## \#25 Posted by: lowGuido Posted at: 2016-09-16T07:22:06.974Z Reads: 77

```
by all means be careful with lipos.
they can be dangerous.
I'd even say more dangerous charging unattended..
```

---
## \#26 Posted by: lowGuido Posted at: 2016-09-16T07:26:28.547Z Reads: 77

```
here is a good video. watch it and it will explain everything.
https://www.youtube.com/watch?v=wIbHLacozFo
```

---
## \#27 Posted by: itsmikeholland Posted at: 2016-09-16T17:45:27.804Z Reads: 69

```
Hey guys, just wanna say how much I appreciated the input. I spent the morning balancing my cells and now it's balance charging at .75C, which is basically as fast as the fast charge was going. Balance charging from now on since its not any faster than fast charging
```

---
## \#28 Posted by: Namasaki Posted at: 2016-09-16T19:09:06.491Z Reads: 67

```
You should never fast charge Lipos. 
You should always balance charge Lipos. 
Balance charging doesn't take that long. 
I could fully balance charge a 6s 5000mah Lipo pack in 1 hour or less charging at 5amps. 
If your pack won't balance, it may already be damaged from unbalanced fast charging.
```

---
## \#29 Posted by: itsmikeholland Posted at: 2016-09-16T21:29:02.849Z Reads: 59

```
I think they arrived a little unbalanced, which is why it was taking hours to balance one battery. After all the advice last night I spent the past 8 hours balancing them, then took a short joy ride. Now they balance at .75C which is perfect! Will definitely be balance charging for now on
```

---
## \#30 Posted by: Namasaki Posted at: 2016-09-16T21:59:53.798Z Reads: 57

```
When ever I buy Lipos I check them first with a Turnigy IR meter. 
I've gotten 2 bad packs from HK right out of the box. 
Lipos should have no more than 5 miliohms per cell when new.
```

---
## \#31 Posted by: paul775 Posted at: 2016-09-17T01:32:44.302Z Reads: 57

```
Having this same problem with one of my 5000mAh 30C LiPo the past few days. 
Cell 1: 4.16 
Cell 2: 4.16
Cell 3: 4.20

I have tried to leave it at _Balance Charging_ for more than an hour yesterday but it stayed at those values.

Today as of this moment I am _Discharging_ it at 1A to about 3.7V per cell and will see if they come together. Then will _Balance Charge_ back up.
_(BTW I always Balance Charge my LiPos and this was the only LiPo out of my 3 that went off track._
```

---
## \#32 Posted by: lowGuido Posted at: 2016-09-17T02:25:39.947Z Reads: 57

```
there is 2 types of balancing; top balancing and bottom balancing.
you can either discharge all cells to the lowest voltage of charge all cells to the highest voltage.
i would suggest to try both in succession to bring them back.
```

---
## \#33 Posted by: Menjos Posted at: 2017-09-21T11:59:55.551Z Reads: 41

```
One of my 10s1p packs with integrated BMS is only charging to 40.9 volts, after about 100 cycles. So I'm assuming the cells are out of balance. I had made it a habit of trying to keep the voltage under 40-41 volts most of the time to increase cycle lifetime. But after reading about how balance charging works, it looks like I might have not allowed the BMS to do its work, because it only functions on fully charged cells. So does this mean it's actually better to always fully charge battery packs to keep them balanced? I hope I can get it balanced again, leaving it plugged in over night didn't help so far. Does it make a difference if you're charging with a higher or lower amp charger?
```

---
