# Did 47 km / 29 miles on one charge

### Replies: 18 Views: 1589

## \#1 Posted by: SimosMCmuffin Posted at: 2017-09-05T20:50:31.645Z Reads: 382

```
With the new battery pack and VESC installed. I've been finally able to start benchmarking the board's performance again and it's pretty nutty.

<img src="/uploads/db1493/original/3X/4/a/4a5065d35ac18513d4ec64e03cc2bc51bf9b652d.jpg" width="690" height="389">

10S5P Samsung-35E pack. Build log available here http://www.electric-skateboard.builders/t/10s5p-battery-pack-build-log-50-pieces-of-samsung-35e-cells/23547


<img src="/uploads/db1493/original/3X/3/2/325d2e32f3ca08eb76f6c76e3f1affc016270d48.png" width="281" height="500">

<img src="/uploads/db1493/original/3X/5/d/5d5e7bf04ea89738b4f8e5512409e78954199257.jpg" width="690" height="388">

The run contained a decent amount of city cruising, with plenty of braking for lights, slowing down for bad road surface and other non-ideal things with range in mind. The board would absolutely do 50 km / 31 miles, with little lower speeds or better route planning.

I also need to get used to the higher speeds the board would be capable. I have the VESC currently limited to a max duty cycle of 0.7, which I plan to slowly raise as I get more used to the speed. The board, being quite a high-rider with a higher center of gravity makes it less stable at high speeds. It should do almost 50 kmh / 30 mph with the 0.95 duty max. Of course that also reduces the max range.

https://imgur.com/a/ftAy7
```

---
## \#2 Posted by: Okami Posted at: 2017-09-05T20:52:22.029Z Reads: 357

```
Hah crazy distance / rider. You should start competing with @chaka who would do most miles kms in one run :)
```

---
## \#3 Posted by: Clonkex Posted at: 2017-09-05T22:43:21.484Z Reads: 333

```
Daaaang, that's one hell of a ride! And a freakin huge battery too. With a board like this I could easily ride to town and back again. I wonder how many lipos I could fit under my deck :P
```

---
## \#4 Posted by: Okami Posted at: 2017-09-08T12:08:59.049Z Reads: 280

```
Maybe we should create some sort of chart with longest distances made on eboard? :D
```

---
## \#5 Posted by: squishy654 Posted at: 2017-11-06T16:48:16.256Z Reads: 235

```
Have you pushed your range any further yet? https://www.youtube.com/watch?v=sDaCqbPwN7M
```

---
## \#6 Posted by: Battosaii Posted at: 2017-11-06T18:52:04.402Z Reads: 219

```
[quote="squishy654, post:5, topic:32359"]
https://www.youtube.com/watch?v=sDaCqbPwN7M
[/quote]

can i ask why is the battery box so big? looks like @SimosMCmuffin got 20 miles less than you but his battery looks to be an 8th of the size of your batter case. Did you use Lipos? Try Lithium ion and it may look like a skateboard again lol
```

---
## \#7 Posted by: squishy654 Posted at: 2017-11-06T19:41:40.317Z Reads: 199

```
It's all li-ion cells, the box is 3inches deep because the hoverboard batts I didn't want to rebuild them or rearrange them into smaller packs (too lazy)  they are 2.5inches high, they are not packed or packaged in a nice fitting arrangement but more for the hoverboards or balance boards they go in. I also used 6 of them , here's a picture of three of the batteries during mockup for an idea of their size. I am currently building the 100 mile battery and it's only slightly larger and will have twice the capacity..at near 50,000mah...but the cells will be stacked and staggered and arranged much better using the powerwall formfactor.. <img src="/uploads/db1493/original/3X/0/0/002874cecd96f56c31a4d804f6fd13a6a7bd4cce.jpg" width="666" height="500">
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2017-11-07T06:38:01.838Z Reads: 168

```
It's the enclosure vs. built-into-deck difference. I designed my deck to fit my particular self assembled battery pack and therefore could optimize the used space. @squishy654 is using hoverboard batteries, which are some "phat" stacks of lithium by the looks of them. And because using an external enclosure is a much more easy way to add a pack to a deck. I say to hell with the aesthetics, get er' going!

How's the ground clearance though? Looks pretty dang low.

**Personal update:**
At the moment, I have packed my board away for winter storage, so I doubt there will be any riding for a couple of months. I have also gotten a permanent job with a local engineering firm where I have so far done both SW & HW designs. I also recently moved from my parents house to my own apartment and I am making it into a good hobby workshop for myself.

Before packing my board away, I did travel from my parents' home to my job place couple of times with my board (33 km back-n-forth) and managed to do some unscheduled wet environment testing in some heavy downpour. Board held up okay, no cut-outs or anything, but I did find some light water seepage into the innards. But considering that I was completely soaked to the bone, I think it was pretty decent performance.

For winter time I plan to focus on developing my own BMS module and once that is in a working condition start working on my own FOC capable motor controller.
```

---
## \#9 Posted by: squishy654 Posted at: 2017-11-07T17:27:09.576Z Reads: 139

```
I would be interested in your BMS designs once completed..
```

---
## \#10 Posted by: ramon Posted at: 2018-01-07T17:03:08.278Z Reads: 122

```
I'm buying 2 broken hoverboards for salvaging parts and I'm probably gonna use 2 of those batterys for my skate so I had a few questions:
did you wired all those batterys in paralel? how much discharge capacity are you getting for each of them? did you skipped the batterys stock bms for the output power? 
Thanks in advance
```

---
## \#11 Posted by: squishy654 Posted at: 2018-01-07T17:32:36.119Z Reads: 106

```
I use the batteries as-is, with the BMS, it does work well in protecting the batteries. I simply wire them in parallel, yup, I charge and discharge through all the BMS's at the same time, they manage themselves..I thought this would cause a balance issue between the packs, obviously there is variation in the internal resistance of each, but with the BMS involved it simply cuts-off when anything is out of range to protect the batts. We find they are only 1c, maybe 2, this is why I currently run 6 of them to get the amp draw I require..make sure you do the math and ensure your system will not draw more than they can handle, they sag like mad when abused..I wouldn't put less than three packs on a board if you want some torque and power.
```

---
## \#12 Posted by: Blitz Posted at: 2018-01-07T17:52:48.790Z Reads: 99

```
I love the battery big capacity Low Amp's but Parallel makes up for low amp's
```

---
## \#13 Posted by: Paolosk8 Posted at: 2019-11-07T03:47:42.847Z Reads: 48

```
Hi mate, how did you wire them up such as it is possible to charge them in parallel? 
I'm thinking to do a similar design with 2 battery (not a powerful board)

Can I just put these battery in parallel via a 2to1 connector and then add an in line charger port before I connect the ESC?

Thanks
```

---
## \#14 Posted by: squishy654 Posted at: 2019-11-07T04:08:02.128Z Reads: 48

```
That's what i did yes..
```

---
## \#16 Posted by: murdomeek Posted at: 2019-11-07T20:02:52.703Z Reads: 43

```
[quote="SimosMCmuffin, post:1, topic:32359"]

![Screenshot_20170905-232342.png](https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/2/325d2e32f3ca08eb76f6c76e3f1affc016270d48.png)
[/quote]

what app is this?
```

---
## \#17 Posted by: SimosMCmuffin Posted at: 2019-11-07T20:21:22.050Z Reads: 41

```
Geo Tracker

I like to use it for just general GPS tracking
```

---
## \#18 Posted by: Paolosk8 Posted at: 2019-11-07T22:26:47.347Z Reads: 39

```
Basically something like these two connector should do the job?
![Screenshot_20191107-160943_AliExpress|365x500](upload://j5Yzu73R0trh80dE7TaIRK5v95T.jpeg) 

![Screenshot_20191107-160914_AliExpress|392x500](upload://1i1oLJ1rrleroa6roga842wWBTt.jpeg)
```

---
## \#19 Posted by: squishy654 Posted at: 2019-11-21T00:42:00.065Z Reads: 26

```
I made my own but yeah...
```

---
