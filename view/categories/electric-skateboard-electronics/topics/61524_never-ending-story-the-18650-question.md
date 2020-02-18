# Never ending story… the 18650 question…

### Replies: 32 Views: 867

## \#1 Posted by: Andy87 Posted at: 2018-07-11T12:33:40.232Z Reads: 290

```
Hey together!
I plan an all terrain 4WD for the cold winter in Russia.
For now I think about 4x 170-190kV motors (6474 or 6480) with a 12s battery
and ESCape ESC.
If everything went how I plan, I will have space for a 6-8p battery.
I calculated the max. battery current with 50Ax4= 200A.
The question is, do I really reach that 200A current?
Or better to say 200A for a longer time (like hill climb)?

I don´t have any experience how much Amps this setup could draw off road.
Maybe somebody can share his values with me?

I also made some calculation based on nkon prices:
VTC5 2600mA  30A 7p max 210A 231€
VTC6 3120mA  30A 7p max 210A 298€
VTC5A 2600mA 35A 6p max 210A 241€ (special offer price for 3,35€ per cell)
Q30   3000mA 15A 8p max 120A 278€
25R 2500mA 20A 8p max 160A 200€

Based on the numbers the VTC5A would be the lightest and cheapest option.
But that´s only the numbers. If somebody can speak out of experience, which would be the best choice for it, I would be very interested to hear it!
```

---
## \#2 Posted by: Sebike Posted at: 2018-07-11T12:58:04.239Z Reads: 258

```
Not an expert here, but I've never heard of an esk8 drawing 200 amps. Maybe a racing-build would, but I guess lipos would be a better choice for short time, high amp draw.
And li-ions and cold Russian weather doesn't seem like a good match. As I understand it, cold weather and batteries means poor performance, risk of failure and shortened battery life.
```

---
## \#3 Posted by: E1Allen Posted at: 2018-07-11T13:00:51.630Z Reads: 241

```
30q batteries are good for 20a continuous.  That's why most use them because 3ah and 20a discharge.  But for you at 7-8p you have options.

50a x 4 is going to feel like a rocket.  Like a big one. However this is going to be a peak current.  Your high P count will be more for range.  It's possible on 4wd you might not even reach 200a on a 4wd board.  Someone else with a mountain board and 4wd needs to chime in.
```

---
## \#4 Posted by: koralle Posted at: 2018-07-11T13:17:26.241Z Reads: 224

```
If you are average weight, 12V60A will shoot you like a rocket during acceleration.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-07-11T13:21:04.157Z Reads: 208

```
that´s one more question, I´m not sure yet.
Just because it can be able to put out 200A, does not mean it´s also practical and controllable.
just if I look on my dual drive which I limited to 35A, I reach them for the time I speed up. just for that time, but I reach them. the question how it will be with four motors.
The amps just go up linear, or it slow down because of 4 motors which will have less work to do....
```

---
## \#6 Posted by: Andy87 Posted at: 2018-07-11T13:23:33.843Z Reads: 192

```
rocket yeh :joy:
that´s exactly why I ask. 
What will be the max current I can expect and is also possible to handle on the board.
```

---
## \#7 Posted by: E1Allen Posted at: 2018-07-11T13:33:27.897Z Reads: 183

```
It's roughly split between the number of motors.
```

---
## \#8 Posted by: koralle Posted at: 2018-07-11T13:36:49.335Z Reads: 179

```
I have not seen more than 40-60A continuous yet. You would have to be pretty skilled, courageous and athletic to stay on the board above that.
I think spikes of around 100-150A can be reached with big awd cans but that is less than a sec and uncommon.
If you have a slow blow fuse of 40-60A you should always be fine.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-07-11T13:56:14.540Z Reads: 169

```
That means I would be fine with a 12s5-6p 30q or even 4p vtc6🤔
```

---
## \#10 Posted by: koralle Posted at: 2018-07-11T14:02:40.969Z Reads: 162

```
um... hell yes. 12s5p is a LOT
```

---
## \#11 Posted by: Blix Posted at: 2018-07-11T14:43:52.544Z Reads: 151

```
https://www.youtube.com/watch?v=ufFDLvNCwR8 by @Ackmaniac 
Maybe not the best source because it is a dual drive but better than nothing. :slight_smile:
82 amp start is bloody fast (3:39)
```

---
## \#12 Posted by: Acido Posted at: 2018-07-11T14:48:10.182Z Reads: 144

```
Its not the best to let the batteries cool below 0 degrees since theres some liquid that can be frozen and make the cell puff itself if i remember well, reccomend you to read a bit on batteries and low temperatures
But if they are in an enclosure they will heat up itself from the use and the heat will stay inside
```

---
## \#13 Posted by: Andy87 Posted at: 2018-07-11T15:42:02.265Z Reads: 135

```
I don’t worry so much about the temperature.
As i usually come from warm place and after I start driving they should heat up as you said.
Tried it last year with my drone and -20.
The only thing is that the range will be not as much as in summer.
For real hart times I have one way heating pads for hands. Just put it in the enclosure and should hold everything round about 20-25 degrees for 6-8h
```

---
## \#14 Posted by: Narnash Posted at: 2018-07-11T15:42:05.966Z Reads: 135

```
 I want to give you some genral advice regarding your batteries and low temperatures.

1. Don't not store the batteries for very long times below 5°C (so don't store the board in a freezing garage for example)

 2. When the cells they will produce heat which will help to keep the battery at reasonable temperatures (btwmake sure to not hammer on the throttle when you know they are cold, the  max. Amp draw ratings do not really apply when the battery is far off the testing conditions) they won't work as efficient on low temp and battery temperatures below -15°C are very dangurous over all you should make to not use it when the actual cells are < -5°C.
3. Therefor you should insulate the battery a (regular electrical insulation+ thermal insulation) working insulation material for example would be silicone, non flammable products like expanded glass granule/foam glass or mineral wool(might cause problems when it gets wet) . 

4. By the way after a ride in the snow when you store the board you should check for moisture build up caused by the temperature differences, allow them to dry of fully befor you ride or charge up again.


And to ask your question which cell you should choose .. you can basicly use any of these you listed they are all great candidates for a esk8 battery. As long you have a high parallel config (>6-8P) you should be perfectly safe with either of them. 

The 200A draw is a burst draw at best, I mean we speak of ~8.5KW power for a board with 20-55 kg. And since you want reasonable speeds (I guess < 65 km/h) this will be geared down by a  4.5 - 6.5 ratio that is probably a torque greater than you can use on basicly any ground anyway, even with 4WD.

So what I want to make clear, any of these cells should work in the appropriate parallel battery setup, the 200A will be a burst at best. You should choose between these cells by reliability, the capacity and cost.
```

---
## \#15 Posted by: Andy87 Posted at: 2018-07-11T15:47:50.808Z Reads: 114

```
Thx for the long explanation!
I will not store the batteries under 5 degrees and for sure don’t start from a cold battery. There I had already some not so good experience with my drone batteries 😅.
I usually always open my enclosure after a ride, so there shouldn’t be a problem with water inside too.
```

---
## \#16 Posted by: Andy87 Posted at: 2018-07-11T15:52:29.200Z Reads: 116

```
But just to understand, that 82a in the video is for one vesc only. So in this case 160a for a start up on flat ground.
```

---
## \#17 Posted by: Sebike Posted at: 2018-07-11T15:58:02.683Z Reads: 116

```
When running dual motors you can set the app to show values for two vescs to give realistic values for total power / amp draw etcetera. What makes you think this 82a is for one vesc only? Doesn't seem right.
Also, Max batt is set to 50 A, so the 82 is most probably the two vescs combined.
```

---
## \#18 Posted by: Duffman Posted at: 2018-07-11T16:03:05.154Z Reads: 115

```
Depends on the board you are building. If it's going to look like this: [4WD Monster](https://www.electric-skateboard.builders/t/4wd-heavy-duty-offroad-monster-board-vesc-c6364-sensored-12s30ah-10kw/20783) you can easy reach more than 200A when driving in snow or loose sand...
```

---
## \#19 Posted by: E1Allen Posted at: 2018-07-11T16:47:37.941Z Reads: 109

```
That's a monster board. Some big power sucking wheels as well.
```

---
## \#20 Posted by: karma Posted at: 2018-07-11T19:02:08.714Z Reads: 104

```
Where on earth did you get 30 and 35A from a 18650 cell as CDR? Testing by mooch and the datasheet shows nowhere near 30A. 
I don’t see why you would need 200A continues for off road, remeber that battery amps is not = motor amps.
```

---
## \#21 Posted by: Andy87 Posted at: 2018-07-11T19:50:54.445Z Reads: 96

```
As my app just calculate for one vesc I asked to be sure how to interpret the values.
Unfortunately I don’t have an Android phone and can’t use the ackmaniak app...
```

---
## \#22 Posted by: Andy87 Posted at: 2018-07-11T20:00:02.226Z Reads: 93

```
I know the difference between motor amp and battery amp.
The intention behind this post is to find the right size of battery to run cool and safe and use only max batteries as needed. That’s why I asked if a 200amp battery in real life is needed...
If I calculate the potential of my vescs I come to 200a...that’s why I ask.
I don’t understand your statement about the battery datasheet.
If I look into the official datasheets of a Sony vtc 5 or 6 or vtc 5a, they claim a constant current of 30,35a. 
That’s the official datasheet. I don’t know anything about any other test who proofed or has shown something else.
Would be nice if you just could link it. Than i directly could have a look into it.
```

---
## \#23 Posted by: Sebike Posted at: 2018-07-11T21:00:30.714Z Reads: 89

```
https://www.e-cigarette-forum.com/threads/bench-retest-results-samsung-30q-3000mah-18650…a-great-15a-20-battery.846955/

Lots of tests to be found there.
```

---
## \#24 Posted by: karma Posted at: 2018-07-11T21:56:53.591Z Reads: 82

```
Ah okey I see. I would not think you need 200A continues from the battery. Hard to estimate though, will you be riding on alot of snow with big wheels? 

Where did you find 30A CDR on VTC6? 20A shows almost 90deg on the battery from the [datasheet](https://voltaplex.com/media/whitepapers/specification-sheet/Sony_VTC6_Specification_Sheet2.pdf). 
I know of no 18650 that does 30A or more continues. 

[Here](https://www.e-cigarette-forum.com/threads/bench-test-results-sony-vtc6a-18650-samples-beats-vtc5a-estimated-2900-3000mah-20-25a.849291/) are some tests done by mooch, he does alot of battery tests. 
[Here](https://www.e-cigarette-forum.com/blog-entry/18650-battery-ratings-table.7447/) is a nice conpact table for tests.
```

---
## \#25 Posted by: Andy87 Posted at: 2018-07-12T05:41:37.682Z Reads: 73

```
@karma and @Sebike thx for the links, that´s what I needed.
Will have a look through it.
```

---
## \#26 Posted by: Okami Posted at: 2018-07-12T07:05:50.799Z Reads: 69

```
Check @Nowind videos . I think some should have video overlay.. (can be found on youtube or in forum)

U should probably calculate what power u might use / need..

I think 4-5kw of power should be a good estimate.. I expect at least 1-2kw when on not so good, hard roads..

Maybe @telnoi or @rich have some data figures to share
```

---
## \#27 Posted by: rich Posted at: 2018-07-12T08:47:22.233Z Reads: 65

```
On my MTB (2x 6374 150kv, 65A motor max and 50A batt max each vesc) I usually reach 130A motor max every ride but the battery max is between 60-90A. The highest value was 97A.

VTC6 are rated for 15A cont. each cell without temperature monitoring, above 15A continious they get hot. I think 12s6p is the minimum due to voltage sag and for keeping it cool.
```

---
## \#28 Posted by: telnoi Posted at: 2018-07-12T08:47:46.515Z Reads: 72

```
I throw as much at it as possible within my budget to combat voltage sag and battery strain during hill climbs. Especially during winter, Lipo performance will be worse.

I have a theoretical max amp rating of 480 (Lipo setup). My VESCs are set at 60A each. Worst voltage sag I noticed during a hill climb in winter is 1V. Due to that alone, I would get even higher C rated lipos for hill climbs when my current packs are done for, despite that my setup will never get close to those numbers.

PS. I go by real life performance instead of looking at logged statistics. If I see voltage sag, there is a reason to upgrade.
```

---
## \#29 Posted by: solideogloria Posted at: 2018-07-12T10:34:07.425Z Reads: 69

```
@Acido @Andy87 @Narnash 

Karlo is right.

**Insulation inside the enclosure** is a very good point: Fibreglass is a very good insulator.

For example, my gum boots (also snow boots) that people wear in the frozen parts of the US (e.g. Denver, Colorado, etc - The same climate as Alaska, Siberia, and parts of Russia!), have a _fibreglass inner boot lining_, and man, they're so warm! They're the warmest boots I've ever owned. It's my go to in Winter! At first I was skeptical since I could only think of fibreglass insulation batts used for housing... But compared to my sheepskin UGG boots (an Australian thing), they don't even come close! I've got other boots that are more comfortable, but I will grab my fibreglass boots to wear, even around the house. It's unbelievable to _never feel cold in your toes_ in Winter.

Boats are made of fibreglass (without insulation batts), and sailors suffer freezing cold ocean temperatures at sea, and the fibreglass seems to work just fine.

**Check it out:** https://www.kamik.com/b2c_int_en/icebreaker-23013.html The website says they're "**Rated: -40°C**". 

That temp rating will remedy what Narnash warned:

[quote="Narnash, post:14, topic:61524"]
battery temperatures below -15°C are very dangurous over all you should make to not use it when the actual cells are &lt; -5°C.
[/quote]

![08%20PM|690x391](upload://ucd2DMD57iH65BxuNuy75BFYYBv.jpg)

![44%20PM|690x316](upload://gXgd0Q3ZgdPMmfrdBqxD2XGgBVZ.png)

--------------------------

I can make you an enclosure, and make it thick for you. It should keep your battery insulated, without having to use heat pads, etc.

Check out my enclosures here: https://www.electric-skateboard.builders/t/solideogloria-modular-flex-enclosure-au-sending-free-samples/57121/

![Demo___ Modular Battery Enclosure 1|690x388](upload://5HSdEtIvfxXS82XAtfSFgg0roWO.jpg)

![Modular Battery Enclosure - Blue Kevlar Carbon|690x388](upload://ju5tfvb04s01rz71ucJj7lUMC3D.jpg)

![Modular Battery Enclosure - Gloss Black Carbon|690x388](upload://sJQAhgAdLxgILcKeXZ4z152NYEt.jpg)
```

---
## \#30 Posted by: Minim Posted at: 2018-07-13T06:47:11.951Z Reads: 47

```
Why is it so dangerous with -15 or lower on the batteries? I drove my Tesla all winter in Norway and we had periods with -20 to -25 over weeks. No problem at all. I’ve even heard that the tesla batteries in colder climates get a much longer lifetime then in the hotter parts of the world. The battery is heated while driving but when parked I don’t have battery heating on other than for charging.
```

---
## \#31 Posted by: Andy87 Posted at: 2018-07-13T07:38:08.134Z Reads: 44

```
I don´t know about Tesla, but you can´t compare it with a DIY battery pack.
I think the battery will likely have a way much better isolation than a small
plastic or carbon battery tray, which means the battery can stand longer cold temperatures before cooling out.
I could also imagine that Tesla has a safety mechanism which slightly start do discharge the cells to heat them up by there own if they become to cold.
But honestly, I don´t know anything about Tesla batteries.
I work with highspeed trains and can say that our unprotected battery packs, which are LiIon packs, loose capacity if the temperature falls down.
But we never had any problems like blown up cell etc.
```

---
## \#32 Posted by: Narnash Posted at: 2018-07-13T09:02:41.424Z Reads: 44

```
It is dangurous with arround sub -15°C **battery temperature** (-15°C is a figure I set for our usecase, it's an estimate and simplification tbh) ambient isn't the problem as long you didn't store the board outside or expose the bare batteries to the air (hence insulation).

The problem is cold temperatures are increasing the internal resistance of the batteries, drasticly. For most batteries you can expect 50% or lower avaiable capacity at -10 to -20°C, with the high Ampareges we draw from our batteries this will result in a very fast temperature overshoot. Even though the low ambient temp. would help cooling the batteries down again, the heat is created inside the batteries and can't travel fast enough to cool down which would cause problems.

The consequence is either a very rapid aging of the batteries, or even failing(venting) cells maybe even more furious kinds of failing. Because we use relatively small batteries such a strong increase of IR is toping out the limits of our battery cells (we don't or can't calculate with a max. continous current margin that can compensate a loss of 50% or more power).
Big vehicles like trains, buses or high end cars even though they take a few hundred or thousand Amps usually come with way bigger batteries, they feel the loss of power (high IR = big voltage drop = slower speed) but the battery runs in spec. even with 50% les efficiency (And tbh it is to be expected that they have a some kind of thermal management for low and high temperatures to keep efficiency as high as possible) 

There are tailored batteries for low ambient temperatures btw but we already need high discharge cells and want as much range as possible (at best at a low weight) these specific low temperature cells can't deliver the performance we want.

 A123 for exampe gives figures some figures about low temperature, but mind you LiFePO4 is a expensive battery technology that comes (over all) with lower capacity than Li-Ion.

Here is a diagram for a A123 18650 2.5Ah LiFePO4 cell, the more  "normal" Li-Ions we use would perform even worse.
https://www.batteryspace.com/prod-specs/6610.pdf


[Also some more basic infos on batteries at low Temperature ](http://batteryuniversity.com/index.php/learn/article/discharging_at_high_and_low_temperatures)
```

---
