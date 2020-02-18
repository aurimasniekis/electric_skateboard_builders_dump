# Sanyo 20700a vs 20700b.. questions

### Replies: 40 Views: 3450

## \#1 Posted by: Taliesin Posted at: 2018-04-27T01:58:59.470Z Reads: 295

```
So the 20700a is 3300 mAh and 30A, and the 20700b is 4250 mAh and 15A.

How do these numbers translate to use in an eskate when it comes to range, power, and top speed?

Motors will be 6374 190kv with dual escapes.
```

---
## \#2 Posted by: mmaner Posted at: 2018-04-27T02:03:50.212Z Reads: 294

```
You need 60 amps at minimum so you need to figure 2p or 3p or whatever so you get the amp delivery you want. 

I've never used those specific cells but here's some perspective...

The 30q is rated at 15 amps but performs very well at 20a constant so a 10s3p is usable, a 10s4p is way better.   The 25r is rated at 15 amps so you really need at least a 4p to be usable, a 6p is pretty nice.
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-04-27T02:09:49.723Z Reads: 282

```
@Taliesin Given the same number of cells, the 20700a would give less range but more power. Vice versa with the 20700b.

That's assuming the same number of cells. But to have enough current, you'd need more 20700b cells as well, so a 20700b pack with enough current would have a MUCH higher range than a 20700a pack, and also be larger.

The 20700 cells are still fairly expensive, so it's probably still cheaper to go with 18650s for now.
If you must go for 20700s, go with the A cells unless you're going for a HUGE pack.
```

---
## \#4 Posted by: Taliesin Posted at: 2018-04-27T02:28:54.915Z Reads: 256

```
Copy that. Would a 12s4p be considered a huge pack? Or should I be considering a 12s8p if I’m going to go with the 20700b’s? I’m leaning towards the b’s due to the range aspect.
```

---
## \#5 Posted by: MysticalDork Posted at: 2018-04-27T02:43:16.680Z Reads: 247

```
4p would probably be enough, maybe 5p. 8p would be absolutely huge, 1.5KWH.
```

---
## \#6 Posted by: MysticalDork Posted at: 2018-04-27T02:45:07.605Z Reads: 239

```
4p of 20700A would still give 586WH, which is still a very large range, and it would give you a lot more power to feed those big motors.

most boards with 'thane wheels get 10-15 wh/km, so 586wh would give you something close to 40-50km of range, depending on your board.
```

---
## \#7 Posted by: Taliesin Posted at: 2018-04-27T03:06:08.173Z Reads: 218

```
I think I would be satisfied with 40-50km of range. But let’s just say I went with the B’s, getting 1.5KWH, that’s three times as much, so would that basically be like 120-150km of range?
```

---
## \#8 Posted by: MysticalDork Posted at: 2018-04-27T03:10:09.229Z Reads: 212

```
Yep, and the pack would weigh 13.5 pounds. It'll be a beast.
```

---
## \#9 Posted by: Taliesin Posted at: 2018-04-27T03:24:11.923Z Reads: 212

```
And how much noticeable difference in power/top speed are we talking between the 2 if we were going 12s4p for both? 

I’m not expecting to ever need to go faster than 30mph, and I’m most comfortable between 20-25mph.  I also don’t need to climb any hills steeper than my backfire g2 already handles. 

I’m not power hungry but if I went with the B batteries and felt like I wished I had a little more power that would be a big chunk of money to reinvest.
```

---
## \#10 Posted by: MysticalDork Posted at: 2018-04-27T03:33:04.432Z Reads: 201

```
You won't notice any difference in top speed, only acceleration. (and maybe braking to some extent)

With either setup, you'll have way more power than the backfire had, even the B cells will be able to provide about 4x the power, and the A cells will do closer to 8x.

With the B cells, it might be worth considering going with 6355 motors instead of 6374, since you'd only be able to feed each motor 30 amps, whereas if you were using A cells, you could feed each one 60.

My last build had dual 6355s at 40 amps each, and the power and torque were awesome - I couldn't stay on the damn thing if I tried to go full throttle from a standstill.
```

---
## \#11 Posted by: Taliesin Posted at: 2018-04-27T03:45:45.458Z Reads: 191

```
Ok awesome really great info, thanks so much. I already have my motors but I’ll look into possibly getting some 6355’s as well.
```

---
## \#12 Posted by: MysticalDork Posted at: 2018-04-27T03:59:51.635Z Reads: 189

```
Don't get me wrong, it does no harm to run motors at less than 100%. 

Also keep in mind that you can upgrade your battery pack later if you feel the need, by adding another parallel group or two.
```

---
## \#13 Posted by: Taliesin Posted at: 2018-04-27T04:05:15.016Z Reads: 179

```
Is combining cells a thing? Like could you wire A’s and B’s in the same pack or would that not work/stupid idea?
```

---
## \#14 Posted by: MysticalDork Posted at: 2018-04-27T04:30:56.577Z Reads: 177

```
That wouldn't be a good idea, but adding more of the same cell to a pack is acceptable - e.g.going from a 12s4p to 12s5p.Mixing different types of cells isn't recommended because they don't share current evenly.
```

---
## \#15 Posted by: Acido Posted at: 2018-04-27T04:47:37.249Z Reads: 173

```
These cells are good for small packs, but for larger ones they are just too expensive
```

---
## \#16 Posted by: Taliesin Posted at: 2018-04-27T04:55:23.087Z Reads: 173

```
Ok right on, thank you.
```

---
## \#17 Posted by: MysticalDork Posted at: 2018-04-27T04:56:35.931Z Reads: 180

```
Also true - The advantage of 20700  cells is that they have about 50-60% more energy than an 18650, so you can use fewer of them for the same performance. Doesn't make too much sense to build a huge pack with them though, when you could do it with more 18650s for cheaper. 30Qs are available for ~$3.50.
```

---
## \#18 Posted by: sebaszz Posted at: 2018-04-27T14:58:21.114Z Reads: 173

```
this my buikd in progress

20700b 12s5p

![image|666x500](upload://stamXZRdYQiooyZhZknvaOq3ekA.jpeg)
```

---
## \#19 Posted by: FredrikHems Posted at: 2018-04-27T15:27:35.565Z Reads: 169

```
Build thread! Now! :heart_eyes:
@sebaszz
```

---
## \#20 Posted by: uigiroux Posted at: 2018-04-27T19:29:19.185Z Reads: 176

```
Yes that looks great!  Where did you get the battery holders I really like those!
```

---
## \#21 Posted by: uigiroux Posted at: 2018-04-27T19:46:34.914Z Reads: 175

```
I was looking at these cells, and it looks like they now have an even better looking 'C' option.  3500mAh, 30A, 12.6Wh.

https://voltaplex.com/panasonic-c-20700-battery-ncr20700c

One thing I consider for using these more expensive cells, regardless of the extra cost of needing a BMS, charger, cables, etc... is that if you were to buy a battery pack from nearly every builder, that the total cost of the pack makes the average cost of a cell usually around $10/cell.  Obviously there are cheaper/pricier exceptions, but it seems like they're usual that expensive.  So the way I justify paying that much for a larger pack is I could either pay ~ $600 for a battery pack from a pro builder for a 12s5p with 30Q's, or I could pay the same amount, build it myself, and use these new high capacity cells.  Of course I could just use 30Q's to make the cost like half or so, but I am not overly concerned with the cost for such an important part of the project.
```

---
## \#22 Posted by: sebaszz Posted at: 2018-04-27T19:55:42.242Z Reads: 170

```
I will start build threat soon, thanx
```

---
## \#23 Posted by: sebaszz Posted at: 2018-04-27T19:58:21.436Z Reads: 170

```
It's my own design 3d printed,

removing torsional flex, waterproof, stress relief on the batteries, cell level fusing, isolated routing for balance wires.

But still working on finishing the build.
```

---
## \#24 Posted by: Taliesin Posted at: 2018-04-27T21:38:49.339Z Reads: 165

```
How does Panasonic’s reputation hold up to Sanyo in regards to the 20700s?
```

---
## \#25 Posted by: uigiroux Posted at: 2018-04-27T21:49:20.765Z Reads: 165

```
Well I'm not 100% sure of this but I think Panasonic and Sanyo are essentially the same thing regarding the manufacturing of those cells.  Like they partnered up, say like Toyota and Scion for ex.  If you Google Sanyo NCR20700A/B/C, it'll show those cells with the Panasonic name.
```

---
## \#26 Posted by: Taliesin Posted at: 2018-04-27T22:23:25.282Z Reads: 165

```
I think you’re right. Welp time to start looking at places to buy those C’s at.
```

---
## \#27 Posted by: Namasaki Posted at: 2018-04-28T18:15:58.836Z Reads: 162

```
[quote="MysticalDork, post:3, topic:53618"]
Given the same number of cells, the 20700a would give less range but more power. Vice versa with the 20700b.
[/quote]

The 20700a's with twice the amp rating should reduce voltage sag substantially over the 20700b's
Range is increased when voltage sag is reduced. I don't know if it would be enough to make up the difference in capacity but as for myself, I would go with the 30a rated cell.
```

---
## \#28 Posted by: MysticalDork Posted at: 2018-04-29T00:31:02.312Z Reads: 155

```
So would I. If I wanted the extra range, I'd go with 30Qs instead.
```

---
## \#29 Posted by: mmaner Posted at: 2018-04-29T00:33:28.808Z Reads: 156

```
Have you checked the xyxlea for those cells?  I'm just curious.
```

---
## \#30 Posted by: sebaszz Posted at: 2018-04-30T10:24:20.628Z Reads: 155

```
Maybe i'm missing something but even the 20700B will outperform most 18650 batteries.

With the bench testing of "mooch", 30Q/ HG2/ 20700B are all rated for 20a continous (30Q on it's limits)

The 20700B will have the same voltage sag as most 18650 batteries. Of course 20700A will be even better but looking at voltage sag in our application, the 20700B will definitely have the best of both worlds,  increased capacity in limited space.


![9E73FF5F-7E3D-40D0-B6E1-0DA7A8A60B45|690x340](upload://bQofkbj3QLeBlkuzpk6ILVRjfZ.png)![E643149E-5767-4C82-846C-16F705C11AD0|690x340](upload://n4eC2dEPPHcnN0meTlNqGZPTEp.jpeg)![image (1)|690x340](upload://lj70L0o4IfLwGckl8gCh38oOzFy.png)

![image|690x340](upload://qridLKWPdUrrmI8nSvDolbtQC7x.jpeg)

[30Q](https://www.e-cigarette-forum.com/threads/bench-retest-results-samsung-30q-3000mah-18650%E2%80%A6a-great-15a-20-battery.846955/)

[20700B](https://www.e-cigarette-forum.com/threads/bench-retest-results-samsung-30q-3000mah-18650%E2%80%A6a-great-15a-20-battery.846955/)

[HG2](https://www.e-cigarette-forum.com/threads/bench-retest-results-lg-hg2-20a-3000mah-18650%E2%80%A6a-fantastic-20a-battery.846005/)
```

---
## \#31 Posted by: Pedrodemio Posted at: 2018-05-01T13:53:45.919Z Reads: 138

```
Not true, just because the battery is limited to 30A doesn’t mean that the motors will be, at anything less than 100% duty cycle the motor current can be higher than the battery. Max motor current = battery current / dutycycle
So at lower speeds you can easily feed huge current to the motors with a low battery current
```

---
## \#32 Posted by: MysticalDork Posted at: 2018-05-02T01:38:08.439Z Reads: 133

```
@Pedrodemio Let me revise my statement: You'd be able to feed each motor **controller** 30 amps.
```

---
## \#33 Posted by: gmurad Posted at: 2018-07-18T21:44:22.677Z Reads: 120

```
I think it's a common misconception that 30Q have better discharge rate than 20700b. The benchmarks that I saw also show 20700b being superior in discharge, voltage sag and capacity departments.
```

---
## \#34 Posted by: sayekim Posted at: 2018-07-18T21:59:24.475Z Reads: 122

```
I guess since you saw it it must be true. 

samsung 30q vs sanyo 20700b discharge results

![image%20(1)|690x340](upload://lj70L0o4IfLwGckl8gCh38oOzFy.png)![image|690x340](upload://n4eC2dEPPHcnN0meTlNqGZPTEp.jpeg)
```

---
## \#35 Posted by: gmurad Posted at: 2018-07-18T23:12:32.611Z Reads: 115

```
Did you realize you just copied the same charts from a few posts above, which was the message I was replying to in agreement?
```

---
## \#36 Posted by: sayekim Posted at: 2018-07-18T23:37:39.544Z Reads: 116

```
I did not copy those. I went to mooch’s page.

Not my point though.
```

---
## \#37 Posted by: gmurad Posted at: 2018-07-18T23:54:56.731Z Reads: 118

```
Might be easier to see when everything is plotted on the same chart:

![image|673x500](upload://wMTaE05VOu9I6kU8rkPTdNbKMX3.png)

What am I missing here? Why isn't 20700B better?
```

---
## \#38 Posted by: mmaner Posted at: 2018-07-19T00:23:26.514Z Reads: 115

```
Samsung 30q's are great for 20a, nit 15. Regardless of what Samsung says. It's been proven here a 100 times.
```

---
## \#39 Posted by: epss4 Posted at: 2019-03-04T20:12:30.329Z Reads: 69

```
Hey man you look like a real pro on this , i am building 12s5p pack , for raptor hub motor , i am better with samsung or sanyo ?i want crazy power and range !
Probably already respond to this but i don’t understand sh*t on those graphic ...
Thanks man
```

---
## \#40 Posted by: mmaner Posted at: 2019-03-04T20:15:10.597Z Reads: 67

```
I would go with 30Q's, they are proven robust and perfect for the application.
```

---
