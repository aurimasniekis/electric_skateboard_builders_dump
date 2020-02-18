# Sony VTC 4 18650 for 10s3p pack

### Replies: 37 Views: 2192

## \#1 Posted by: marcus Posted at: 2017-06-14T18:21:24.006Z Reads: 178

```
Hey guys,

Thinking of building a 10s3p pack with these li ion batteries. What do you think? Anyone have any experience with them?

https://liionwholesale.com/collections/batteries/products/sony-18650-vtc4-battery-genuine-tested-30a-2100mah-flat-top-wholesale?variant=1038136780

Thanks!

Marcus
```

---
## \#2 Posted by: anorak234 Posted at: 2017-06-14T18:25:08.810Z Reads: 171

```
I don't have experience with these cells in particular however at 30A you will not have much voltage sag and in 10s3p these will probably get you a decent 9-10 miles. As for lithiumionwholesale they are not always bulletproof... I got a weak 26650 cell with them in an order of 12 so quality check can be hit and miss (from my experience, others have had good experiences with them)
```

---
## \#3 Posted by: marcus Posted at: 2017-06-14T18:29:33.047Z Reads: 164

```
Thanks for the info. This pack would have a theoretical 222amp hour size, so I'm thinking range will be be a bit farther than 10 for a 150-60 pound rider. The general consensus is it is about 10 amp hours per kilometer
```

---
## \#4 Posted by: bullrider12 Posted at: 2017-06-14T18:42:05.573Z Reads: 154

```
I have 2 packs of VTC5 cells, they are nearly the same except that the vtc5 has 2500 mAh. 
One is 8s3p and the other one is 10s3p. With a 200 kv motor I get nearly 18-20 miles with a rider weight of 170 pounds.

I can fully recommend those cells :slight_smile:
```

---
## \#5 Posted by: Smorto Posted at: 2017-06-14T18:58:56.833Z Reads: 141

```
I think you mean watt hours no amp hours :wink:.
```

---
## \#6 Posted by: rpn314 Posted at: 2017-06-14T19:00:51.187Z Reads: 138

```
I thought Sony had discontinued the VTC cells. If Li-ion Wholesale has them, I'd believe they're legit (I and many others have purchased cells from them before). Many in the electic bicycle community love those cells. I'd say look at the discharge curves of them vs the 30Q and then go for the best one vs. their respective price.
```

---
## \#7 Posted by: marcus Posted at: 2017-06-14T19:13:07.113Z Reads: 128

```
Oop, watt hours...aha
```

---
## \#8 Posted by: Smorto Posted at: 2017-06-14T19:30:36.762Z Reads: 128

```
Can I ask why you need the 90A other then to reduce voltage sag? Because if range in important to you you can go with the samsung 30q cells that have 3000 mah but only 15A? Or the LE2 cells that have 3000mah and 20A?
```

---
## \#9 Posted by: marcus Posted at: 2017-06-14T19:42:49.690Z Reads: 122

```
Cost and goal. I want to keep my setup to 3p and the Sony cells at 30 cells are only 4.10 a pop. Howeve, most other cells with higher capacities are only 20amps and three of those in parallel is only 60 amps, a bit too low of a max for the board (correct me if I'm wrong). Otherwise I would have to build a 4p cell to make it a max of 80 amp pull.
```

---
## \#10 Posted by: marcus Posted at: 2017-06-14T19:43:39.904Z Reads: 118

```
The Sony VTC cells are 30 amp max draw which only Three of those will nicely put me at 90amps
```

---
## \#11 Posted by: Maxid Posted at: 2017-06-14T19:52:20.735Z Reads: 117

```
ratings mean nothing.
Look at the actual discharge test
http://lygte-info.dk/review/batteries2012/Common18650comparator.php

I used the VTC5 to compare the 30Q to - VTC4 should be even worse than the VTC5 since they are older generation.
Less sag is better!

You are not going to be drawing 90A constantly - that would be a constant 90A*36V=3240W and your ESC and motor would die. A VESC can do like 50A continously - but even that is ridiculously high for a standard esk8.
If you want to climb the mount everest in one go at 50km/h on an esk8 you should probably look into a larger battery anyway ;)
```

---
## \#12 Posted by: marcus Posted at: 2017-06-14T20:05:42.920Z Reads: 111

```
Ok, what do you think about the Samsung 25R? 2500mah and 20 amp continuous
```

---
## \#13 Posted by: Maxid Posted at: 2017-06-14T20:19:05.742Z Reads: 108

```
Again: the rating means nothing.
Look at the discharge curves. The 25R is clearly worse than a 30Q.
They are not bad - but there are better alternatives out there.
You could also look into HE2 and HE4 but best bang for buck IMO is the 30Q right now.
It is basically the same cell as a HG2 just with a more conservative rating.
```

---
## \#14 Posted by: Jinra Posted at: 2017-06-14T22:17:16.235Z Reads: 103

```
That's interesting. When i took a look at official datasheets for each cell (30q 25r) the 25r's had better sag performance
```

---
## \#15 Posted by: rpn314 Posted at: 2017-06-14T23:27:29.019Z Reads: 108

```
Yeah, that's why I would look at the real performance tests and not datasheets as @Maxid linked to.

That site makes it a bit difficult because I think the test equipment they used on the 30Q was different (not sure if it's better. see the notes on their site). The tests on that site show that the 30Q is a little better than the 25R in voltage sag, even though they are rated ratings are the opposite. It's possible that the 30Q gets hotter, as they note that the 30Q hits a cutoff temperature while the 25R didn't (or maybe the test equipment didn't account for that, not sure).
```

---
## \#16 Posted by: Maxid Posted at: 2017-06-14T23:30:19.205Z Reads: 115

```
yeah they used an older test station for the 25R (and other older cells like HE2 and so on) - However I doubt that this has such a large impact.
30Q are not just a little better IMO in terms of voltage sag.
You are right with the temperature increase in 30Qs but then we have to keep in mind that this was for constant discharge - we are not draining our batteries that way so they always have time to cool down to moderate levels when used in eks8s. Anybody that would be draining a battery so hard constantly should not build a 3P battery pack but look into either A123 cells or Lipo pouches

Here is a good comparison of VTC5, 25R and 30Q in one graph at 20A discharge (on hopefully equal test equipment performed by Mountainprophet)

http://www.mountainprophet.de/wp-content/uploads/2015/06/Samsung30q.png

You can see the 25R having the largest voltage sag while the 30Q (even though discharged at an overspecced 20A) performs better than a VTC5. Temperature increase is not considered though.
```

---
## \#17 Posted by: fedestanco Posted at: 2017-06-15T00:07:50.000Z Reads: 103

```
I saw the comparison graphs for the 30q. Considering amp vs sag there is no game: 30q outperforms any li ion cell except vtc6.

I believe though that if a company advertises 30% less power ,thus damaging sales by a significant percentage, there are VERY good reasons to do it.

We are in fact just considering amp vs sag. There are many more graphs that could prove that more than 15amp continuous is TOXIC for the cell. 
Could be : amp vs cell life ; amp vs temperature; temperature vs insulation failure ; temperature vs adhesives failure .....

Samsung is telling you :"we guarantee 15amp continuous because in some of our graphs (non available to the public) this cell performs shit at 20amps and could fail miserably"
```

---
## \#18 Posted by: Maxid Posted at: 2017-06-15T00:13:17.658Z Reads: 96

```
But I just showed you a graph for 20A :confused:

And again: we are not draining the cells constantly at 20A. The typical usage is 10Wh per Km. That is 300mAh at 10S per Km. With say 30km/h you get 9A that you are discharging - in total - not per cell.
Per cell in a 3P config this is just 3A.

But what you want to be prepared for is spikes in current when you go uphill or accelerate. So voltage sag is the most important thing to consider because it indicates how well your cell can cope with this

I also think that the reason for the underspecced 30Q is just liability issues. It is not hurting sales because every informed guy will know whats going on but you can't blame them if something happens while you used them at 20A instead.
```

---
## \#19 Posted by: fedestanco Posted at: 2017-06-15T00:34:12.310Z Reads: 97

```
I repeat: sag-wise 30Q is the winner on any amp vs sag graph.
Lets just not talk esk8 for a second and focus on the battery as a product. 
My point is: there is one or more variable (temperature, cell life....) that samsung found out to be consistently damaged after 15amp continuous. There is no graph on the internet containg that precise weak variable.

A good analogy would be : 25r is a car that goes 10 kmph; 30q is an e-bike that can go 20kmph. The seller obviuosly tells you not to go more than 5kmph with the ebike.
Problem with the cells is that they seem similar and hide weaknesses
```

---
## \#20 Posted by: sl33py Posted at: 2017-06-15T01:04:31.410Z Reads: 98

```
VTC6 looks great on sag, but i like the VTC5A for high discharge - hopefully not really stressing the cell to max.  A  few more cells in parallel to help with sag and a solid performing option!

Yes capacity is less but in a 3/4p being realistically able to do 20-30A per cell and not exceed his threshold of 78c = a true 90-120A capable 3/4p pack!  the VTC6 is great for range, but i don't need 9/12Ah 3/4p pack.  a 3p VTC5a pack at 10s (2.6Ah * 3 * 42v) = 327Wh.  12s (7.8Ah * 50.4v) = 393Wh.  10Wh = 1km... 32km/19mi and 39km/24mi.  

I'm less concerned with range/mAh of cells and more ability to provide amps when needed while minimizing heat which = less pack life.

nkon order in for some VTC5A's around $4 per cell!

Mooch:
<img src="/uploads/db1493/original/3X/b/7/b7b958d624606317706f70ecb29484624c9472dc.JPG" width="690" height="316">
```

---
## \#21 Posted by: jga Posted at: 2017-06-15T08:23:09.073Z Reads: 92

```
[quote="fedestanco, post:19, topic:25384"]
A good analogy would be : 25r is a car that goes 10 kmph; 30q is an e-bike that can go 20kmph. The seller obviuosly tells you not to go more than 5kmph with the ebike.
[/quote]

I am a bit puzzled with this comparison...What is it supposed to demonstrate?
```

---
## \#22 Posted by: fedestanco Posted at: 2017-06-15T12:21:49.352Z Reads: 84

```
Only that I trust sumsung and their tests when they say max 15amp.
I made packs of 25r and my next pack will be made of 30q; so there is no bias when I talk about these 2 cells.
```

---
## \#23 Posted by: mmaner Posted at: 2017-06-15T14:12:23.963Z Reads: 84

```
I have a 25r pack and a 30q pack, both 10s3p.  The 25r pack is ok, not bad at all...but the 30q pack kills it.  In terms of AMP delivery, I would put my 10s3p 30q pack against a 25r 10s4/5p pack any day.
```

---
## \#24 Posted by: sl33py Posted at: 2017-06-15T14:33:58.669Z Reads: 87

```
30q looks like an amazing cell.

I love comparing these on graphs (if you haven't read up on some of mooch's testing, or watched his youtube discussions - tons of good info!).  

Pictures and graphs and side-by-side goodness!  Satisfies my OCD geek tendencies...  BUT realistically i think when you are talking such tight differences like the 30q and HG2 in the below graph - it seems like you wouldn't actually notice a difference in real world?  

I also like seeing a "worst case" scenario like 20A *continuous* discharge - not something we'll see on esk8 unless you are going uphill the entire time accelerating...  Or am i missing something?  I want the ability to provide the "punch" of a high output pack, but if i'm pulling 100% it's amp capacity 100% of the time - it's going to not last and get really hot.  Mooch set his threshold at 78C/172F for an acceptable temp for max output - where he then over-draws some 15A cells and rates them for 19/20A since they aren't stressed and exceeding 78C.  

more picture goodness:
[img]http://www.dampfakkus.de/highamps/592-20A.png[/img]
(heavy 20A discharge across multiple cells w/ little real-world difference - except 25R and VTC5's more noticeable 2500/2600mAh capacities)

Hope others like the graphs - great thread!
```

---
## \#25 Posted by: Smorto Posted at: 2017-06-15T15:20:56.382Z Reads: 77

```
Is the 45A enough for you? Is there much voltage sag?
```

---
## \#26 Posted by: mmaner Posted at: 2017-06-15T15:29:16.050Z Reads: 78

```
I'm running a 10s3p 30Q pack on a 40in deck with 6in AT wheels (@psychotiller 6 Shooters) and it never sags more than 1V.  I don't actually feel the sag, that's just what I see on my volt meter.
```

---
## \#27 Posted by: Smorto Posted at: 2017-06-15T15:31:02.511Z Reads: 77

```
Sweet, what kind of range you getting out of that thing?
```

---
## \#28 Posted by: mmaner Posted at: 2017-06-15T15:31:54.001Z Reads: 76

```
I haven't really measured it, my kid rides it a lot as well and he's much lighter, so hard to tell.  I think about 15-18 miles.
```

---
## \#29 Posted by: Smorto Posted at: 2017-06-15T15:32:31.299Z Reads: 76

```
Awesome, I think I might go with a 10s3p 30q pack, do you have a diagram, of your pack?
```

---
## \#30 Posted by: mmaner Posted at: 2017-06-15T15:33:14.995Z Reads: 77

```
I dont, but @PXSS built it, he should be able to tell you.

Also, I am not running a BMS at the moment, so I charge to 41v and discharge to 34v.
```

---
## \#31 Posted by: Smorto Posted at: 2017-06-15T15:35:05.499Z Reads: 76

```
Cool, how should I go about contacting him?
```

---
## \#32 Posted by: mmaner Posted at: 2017-06-15T15:46:06.179Z Reads: 74

```
I would just message him here using his 'handle', @PXSS.
```

---
## \#33 Posted by: rpn314 Posted at: 2017-06-15T23:28:12.056Z Reads: 73

```
[quote="mmaner, post:23, topic:25384, full:true"]
I have a 25r pack and a 30q pack, both 10s3p.  The 25r pack is ok, not bad at all...but the 30q pack kills it.  In terms of AMP delivery, I would put my 10s3p 30q pack against a 25r 10s4/5p pack any day.
[/quote]

I also have a 25R pack. Frankly, I'm not sure why I thought the 25R was the best cell when I bought them a year ago (and I don't think I was the only one). I'd be curious what kind of longevity difference there is between your packs with similar use. It's harder to test and document and I wonder if that may be where the 25R is a bit better, though only by a little bit.
```

---
## \#34 Posted by: fedestanco Posted at: 2017-06-15T23:43:53.155Z Reads: 72

```
30q capacity drops to 72% after 250 cycles, discharged at 22A each cycle.
<img src="/uploads/db1493/original/3X/6/0/6085c860031d2fa8a2967eb0d7175faeee007a35.png" width="690" height="388">
25r capacity drops to 62% after 250 cycles, discharged at 20A each cycle
<img src="/uploads/db1493/original/3X/8/3/830777f3e2d469e44472e5d9ef37dfad61f7db49.jpg" width="690" height="388">

Thus 30q are better even regarding life cycle at crazy discharge.
```

---
## \#35 Posted by: mmaner Posted at: 2017-06-16T03:19:48.488Z Reads: 66

```
I've only charged my 30q pack about 10 times, I've charged the 25r pack prolly 50 times.  I rebuilt my dual ly too speed for my kid, he rides alot. 

I'll.pist if I see a major difference in capacity and/or performance over time.
```

---
## \#36 Posted by: Okami Posted at: 2017-07-10T22:46:27.251Z Reads: 66

```
Woah very good discussion! I think the thread should be renamed a bit to focus on the benefits of 30Q cells even more!

// If someone researched more then they would find that some claim VTC4's are actually good for about 23A anyways.. and they do tend to heat up after this 'treshold'·

Concerning 30Q's, nice graphs @fedestanco ! Hadnt seen those before.

--

I think I also had seen their temp graph somewhere and it also showed 30Q's tend to heat up even a bit less than some 20A 'officially rated' cells, for example.
```

---
## \#37 Posted by: sl33py Posted at: 2017-07-11T00:40:17.494Z Reads: 61

```
Agreed - would love to see more 250 cycle comparisons and temp graphs.

I just got some VTC5a's and can't wait to build them!  Realistic 25A with plenty of capacity.  Not sure on the 250 cycle comparison though!

Agree on the thread title - should be "current 18650 comparison" or similar.
```

---
