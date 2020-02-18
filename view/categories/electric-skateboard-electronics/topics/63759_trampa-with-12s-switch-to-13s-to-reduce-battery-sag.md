# Trampa with 12s, switch to 13s to reduce battery sag?

### Replies: 29 Views: 445

## \#1 Posted by: brotori Posted at: 2018-08-03T23:03:08.547Z Reads: 141

```
I have a trampa, with a 12s lipo battery (2  x 6s in series), 6000mAh. So at full charge the battery is at 50.4 volts (4.2 per cell). Low cut off is set at 42 (3.5 per cell).


I have a bunch of 1s batteries. Does it make sense to put a 1s battery is series when the battery is at 46 volts (3.8v per cel)  ????   So it will be switching to a 13s battery and voltage back to 50 volts?



I plan on using a 1s2p battery (2 x 5000 mAh in parallel.),  10,000mAh total, not too much additional weight.


If I do this the total voltage will be back to 50 volts, and less battery sag???? Does this make sense???



The idea is that by just adding only a small 1s2p battery when the main battery is getting close to the low voltage cutoff, switching to a 13s will reduce battery sag. 


I have an alarm in the main 12s to detect when any cell is below 3.5 volts.
```

---
## \#2 Posted by: JonathanLau1983 Posted at: 2018-08-04T01:47:38.973Z Reads: 121

```
You should only really use matching cells, voltage and C rating wise
```

---
## \#3 Posted by: DeathCookies Posted at: 2018-08-04T06:23:57.294Z Reads: 97

```
Your Pack will likely get out of Balance. If you discharge 50% and then add one cell to compensate sag you have an unbalanced Pack. Next thing is that the Low voltage cut off is a problem. When 12 cells reaches the end or you did not enable the extra cell. 

It is possible but more of a hassle imo
```

---
## \#4 Posted by: Andy87 Posted at: 2018-08-04T06:59:52.801Z Reads: 88

```
Can just agree with @JonathanLau1983
The cells should match together if you work with lipos.
The only way to reduce sag is to use cells with high discharge values or add more cells (which should match) parallel.
If you put cells in parallel the load divided to every p cell. So less load for the single cell, which results in less sag
```

---
## \#5 Posted by: Acido Posted at: 2018-08-04T07:05:36.118Z Reads: 77

```
thats a serious no go
```

---
## \#6 Posted by: brotori Posted at: 2018-08-04T16:55:48.531Z Reads: 61

```
[quote="DeathCookies, post:3, topic:63759, full:true"]
Your Pack will likely get out of Balance. If you discharge 50% and then add one cell to compensate sag you have an unbalanced Pack. Next thing is that the Low voltage cut off is a problem. When 12 cells reaches the end or you did not enable the extra cell.

It is possible but more of a hassle imo
[/quote]

What is the problem with an unbalance pack during discharge? As I understand, the issue is that you should not discharge a lipo CELL below a certain voltage (damage is likely below 3.0 volts). If the vesc is the only protection,  and battery isn't balanced, it's possible for the total voltage to be above the cutoff threshold, yet still have a cell below the 3.0V danger zone.
In my case, I have a voltage meter for each of the battery cells. It does sound an alarm if ANY OF THE CELLS go below 3.5 volts, so that will never happen!
So, I am missing something here? What’s the problem?  What is the worst-case scenario?
```

---
## \#7 Posted by: brotori Posted at: 2018-08-04T16:59:39.560Z Reads: 51

```
[quote="Andy87, post:4, topic:63759"]
The cells should match together if you work with lipos.
[/quote]

I hear people saying that all the time, but I can't find what is the likely problem, as long as each cell are monitored individually to prevent over discharge using a low voltage alarm.
```

---
## \#8 Posted by: DeathCookies Posted at: 2018-08-04T17:04:57.421Z Reads: 47

```
[quote="brotori, post:6, topic:63759"]
In my case, I have a voltage meter for each of the battery cells. It does sound an alarm if ANY OF THE CELLS go below 3.5 volts, so that will never happen!
[/quote]

Well your Statement is totally true! You did not write this Information in the first place so i could only give an answer with the Information i had...

You should be good to go if you have a alarm for each cell but i think it will get quite annyoing. (the beeping)
```

---
## \#9 Posted by: Andy87 Posted at: 2018-08-04T17:54:51.937Z Reads: 43

```
You don’t give more information about your cells.
So let’s say your 12s pack is rated with 60c at 6000mah, your 1s 5000mah just with 25c.
What you think will happen under heavy load?
And just to make sure that I understood right.
You first want to drain your 12s pack to 3.6-3.7v and after that add a 1s pack with 4.2v on top to reduce the sag, right?
I‘m not a lipo expert and somebody can help me out if i‘m wrong, but
The sag depends on the internal resistance of the lipo and the load. Why should the sag become more with less voltage? 
For me in this context it don’t make a sense at all to add a 1s battery to the pack.
If at all it would make sense to add parallel cells to your 12s pack. This would reduce the load on the main pack and with it the sag would become less
```

---
## \#10 Posted by: E1Allen Posted at: 2018-08-04T18:20:02.259Z Reads: 38

```
This would be a serious mistake and ruin your cells.  You can't take your 12s pack and run it low, then add a 1s.  Yes it will increase voltage, that's what series cells do.  However increasing voltage won't help because your 12s pack is already near LVC.  So you're just tricking the vesc to think you still have battery.  When all you will do is decrease the voltage of the 12s pack below safe limits as you continue to ride.  You should really only combine the same capacity, type, and C rate.

You're better off running 13s with full batteries so they drain together and equal.
```

---
## \#11 Posted by: brotori Posted at: 2018-08-04T18:40:17.284Z Reads: 33

```
[quote="E1Allen, post:10, topic:63759"]
When all you will do is decrease the voltage of the 12s pack below safe limits
[/quote]

That is where I disagree. That will not happen because I have an alarm that monitor ALL cell. They will never go below 3.5 volts.

So, my question is, apart from over-discharge (which will not happen), there is any other problem?
```

---
## \#12 Posted by: Andy87 Posted at: 2018-08-04T18:42:05.045Z Reads: 31

```
That it will not reduce your sag problem.
And if you use a low rated 1s cells they will heat up under load and can start to  puff
That’s the main two issues
```

---
## \#13 Posted by: Hummie Posted at: 2018-08-04T18:47:54.413Z Reads: 28

```
sounds doable to me!  if there's an alarm so no cell goes too low then there's no real risk, and the risk of imbalancing the cells isnt there as it's still the same 12 cells with the same draw on them.  i think its a weird solution but would work without a problem
```

---
## \#14 Posted by: brotori Posted at: 2018-08-04T18:48:12.043Z Reads: 27

```
[quote="DeathCookies, post:8, topic:63759"]
it will get quite annyoing. (the beeping)
[/quote]

Yes, it annoying! the beeping is very loud! 

 ![20180804_154301|666x500](upload://ougyl4l1Aro01A4WYL9Tj2KAllt.jpg)
```

---
## \#15 Posted by: brotori Posted at: 2018-08-04T18:55:48.406Z Reads: 28

```
[quote="Andy87, post:9, topic:63759"]
The sag depends on the internal resistance of the lipo and the load.
[/quote]

Internal resistance is a characteristic of the cell. It will get worst over time, as the cell is deteriorated after many discharge cycles. 
As I understand sag, it is related to lower voltage,  less power delivery.  power (watts) = current x voltage.
But as long as the battery can deliver enough amps. It will be a problem if the main 12s battery is at very low voltage, so it will not deliver enough amps. But that is not the case here, I will cutoff before that (at 3.5v).
```

---
## \#16 Posted by: brotori Posted at: 2018-08-04T18:56:43.553Z Reads: 27

```
[quote="Hummie, post:13, topic:63759"]
i think its a weird solution but would work without a problem
[/quote]

thanks! If its weird, I love it...
```

---
## \#17 Posted by: brotori Posted at: 2018-08-04T19:05:13.213Z Reads: 27

```
[quote="Andy87, post:12, topic:63759"]
And if you use a low rated 1s cells they will heat up under load and can start to puff
[/quote]

Yes, that is a concert. That is why I actually use a 1s2p, 10,000 mAh, at 20C, so about 200 amp max, which is much higher than what I need. I have tested and I am using less than 2500 mAh from the 1s2p batteries, before the cutoff of the 12s, 6000 mAh batteries.
```

---
## \#18 Posted by: Hummie Posted at: 2018-08-04T19:09:48.931Z Reads: 26

```
all the cells in the 12s will still be getting a good sucking though, pretty evenly with your added 1s big cell.  based on internal resistance i guess and voltage of each cell. ..that's a guess.  but just saying, so you dont think otherwise, that 1s addition isnt going to be able to add more current than any of the other individual cells in the 12s pack im pretty sure.   this is sounding like the cheap guy solution, which works,  but just getting a bigger 12s battery would be the better way for sure.  who wants to carry around a battery, not me.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-08-04T19:18:30.937Z Reads: 28

```
That’s my thoughts too.
If to add at 3.7v one 4.2v cell the average voltage would rise up to 4v, but will the 4v be in every cell? Don’t know about voltage swap and how much it can be.
So if no than it would be still 12cells with a high sag and one with less.
Maybe @brotori you already have some real world experience?
```

---
## \#20 Posted by: brotori Posted at: 2018-08-04T19:18:33.327Z Reads: 30

```
It more about weight and convenience than price. I do have several large batteries, but they are really heavy (2 x 6s tattu 28000 mAh for example that I use for very long rides).  Sometimes I want a short, but intense ride, with a light pack. The 1s2p adds only about 200g. 


I have tested already the solution, for science! and it is working. Will reports if I see any problem along the road.![20180804_161317|666x500](upload://7ieE7R5XZCI444vUbUphhvUgPYr.jpg)
```

---
## \#21 Posted by: Hummie Posted at: 2018-08-04T19:21:58.118Z Reads: 29

```
since you bought it up Im still wondering what the current draw is on the one cell at 4.2 and the other 12 at 3.5.    Math formula id like to know.
```

---
## \#22 Posted by: Hummie Posted at: 2018-08-04T19:23:46.468Z Reads: 29

```
[quote="Andy87, post:19, topic:63759"]
but will the 4v be in every cell? Don’t know about voltage swap and how much it can be.
[/quote]

if they were parallel voltage would balance but being series they stay the same voltage.
```

---
## \#23 Posted by: brotori Posted at: 2018-08-04T19:25:54.051Z Reads: 30

```
[quote="Andy87, post:19, topic:63759"]
but will the 4v be in every cell
[/quote]

The cells are in series. So yes, you add 4 volts to the overall voltage. So you have 12 cells at 3.8 volts, and 1 cell at 4.2 volts, for a total of 50 volts. That is about the same of having 12 cells at full charge, or 4.2 volts,
```

---
## \#24 Posted by: brotori Posted at: 2018-08-04T19:37:00.920Z Reads: 29

```
[quote="Hummie, post:21, topic:63759"]
Math formula id like to know.
[/quote]

Look at a figure showing the discharge rate for a 4s lipo at 25C constant discharge (Battery holds ok till 3.5 volts, then the voltage goes down a clift. 

![lipo%20discharge|690x457](upload://rMiaqGEQHgmWNRRwtNRwiFsM13u.PNG)
```

---
## \#25 Posted by: Andy87 Posted at: 2018-08-04T19:42:48.389Z Reads: 26

```
I calculate with 3.7, than it’s 4.05v😜
```

---
## \#26 Posted by: Hummie Posted at: 2018-08-04T19:46:20.000Z Reads: 25

```
i mean i wonder what the math is on the current that would come from each of those 13 cells with all being the same maybe at 3.5 and one at 4.2
```

---
## \#27 Posted by: brotori Posted at: 2018-08-04T19:49:26.242Z Reads: 26

```
[quote="Hummie, post:21, topic:63759, full:true"]
since you bought it up Im still wondering what the current draw is on the one cell at 4.2 and the other 12 at 3.5. Math formula id like to know.
[/quote]

Actually, I have the answer for that (i guess....). I use a similar setup in my onewheel, but for a 14s setup.
I use 2 x 6s 6000 mAh and 1 2s2p 10,000 mAh in series for a 14s at 58 volts, that is whats the onewheel needs.


After one ride, the 2s 10,000 mAh was fully charged with 3.86 Ah, almost the same as the two 6s in parallel (7.73/2 = 3.86).
I have done this one many many time, always the same. Amps hrs used for the 12s and 2s are almost always exactly the same. Keep in mind that at the end of the ride, the cells in the 6s are at about 3.7 volts, and the 2s cells are at about 3.9 volts, because the 2s have a higher capacity.

![20180717_121930|666x500](upload://rRyCtdTHVIHzVeRJpzMCtMuHYHc.jpg)
```

---
## \#28 Posted by: Hummie Posted at: 2018-08-04T19:54:13.281Z Reads: 26

```
starting at the same voltage that makes sense but what about when you mix the voltage as i understood you were doing with your other vehicle where you added a 4.2 volt cell onto a bunch of 3.5 volt cells.  what's the current draw from the different cells then with the different voltage?  will the higher voltage be able to put out more of the current than others? in ratio to the voltages maybe and the high voltage will put out more is my guess.  but it wouldnt be much more.
```

---
## \#29 Posted by: brotori Posted at: 2018-08-04T20:00:21.463Z Reads: 26

```
[quote="Hummie, post:28, topic:63759"]
maybe and the high voltage will put out more is my guess. but it wouldnt be much more.
[/quote]

Good question. My guess is that it is the same. In the onewheel setup, after some time riding we are in that situation. The 6s and the 2s cells are at different voltages, and still the amp usage seems to be the same, because at the end of the ride the total amps hrs is exactly the same for both packs.

I actually came up with the idea of reducing the battery sag in the trampa using this trick because of these results in the oneWheel. I have been using this setup in the onewheel for a long time already. Now I might try the same trick with the onewheel.... adding a 1s2p, and going to 15s at the end of the ride. Crazy indeed....  In the onewheel battery sag is really an issue because of risk of nosedives when the battery is very low.
```

---
