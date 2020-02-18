# Custom carbonfiber deck &#124; VESCX &#124; 10s 5000mah

### Replies: 38 Views: 3264

## \#1 Posted by: BexBle Posted at: 2016-11-04T19:13:27.064Z Reads: 315

```
Hi thanks for reading. I'm looking for a build that can go about 20KM range and I would be looking for about 35KM/H
min max speed.  My budget is around 500Euros but I can break it slightly. I was hoping you could mabey recommend some parts or tips. I was thinking : 

VESC-X or normal 150A car esc


x2 5000mah 5s 30-50c batteries.

SVK3 or Enertion motor

Custom fiberglass deck
```

---
## \#2 Posted by: ajaynagra Posted at: 2016-11-05T14:22:41.877Z Reads: 288

```
Batteries between 20c-30c

Get your vesc from @B4Me

Whats you plans for your deck?
```

---
## \#3 Posted by: evoheyax Posted at: 2016-11-05T16:40:10.405Z Reads: 260

```
deck (~$300) +  batteries (~$150) + vesc (~$100) + motor (~$100)  will already push you over $600 euros, and you still need the drive train sustem and a charger plus wires and plugs ect. If you want a budget board, your better off buying a complete from china IMO. But those things won't last long, and neither will a $500 diy board. You realistically need $800 euros at least for a quality board that will last more than a few weeks of riding.

For $500 euros, you need and fvt 120a, sk3 motor, cheapest lipos possible, and the cheapest charger for those lipos (imax clone charger, authentic ones are quite a bit more). Invest a bit more and your be way happier with a vesc and r-spec motor.
```

---
## \#4 Posted by: SirDiff Posted at: 2016-11-05T18:11:23.714Z Reads: 235

```
Not at all, I'm building a 6374 190kv, liion with bms, vesc and all the other stuff for 530 euros. Just look for group buys.
```

---
## \#5 Posted by: BexBle Posted at: 2016-11-05T21:06:41.577Z Reads: 222

```
Thanks for replying the deck is coming to below 80 Euro. i should've mentioned I'm making it. my plan is to buy military grade foam and carbon fiber. I will use the foam as a base source some layers of carbon fiber ontop. I will be using plywood supports where the trucks go. For more info please go to http://www.instructables.com/id/Carbon-Fiber-Electric-Skateboard-Deck/
```

---
## \#6 Posted by: BexBle Posted at: 2016-11-05T21:07:37.133Z Reads: 217

```
I will also be making my own motor mount out of aluminium and carbon fiber. Do you guys think two 5000mah 10s 30c batteries would wrk.

Thanks Reuben
```

---
## \#7 Posted by: ajaynagra Posted at: 2016-11-05T21:08:47.859Z Reads: 206

```
Using a CNC machine ?
```

---
## \#8 Posted by: BexBle Posted at: 2016-11-05T21:10:30.258Z Reads: 204

```
No is the answer any ways but out of interest for what part?.

Thanks Reuben
```

---
## \#9 Posted by: BexBle Posted at: 2016-11-05T21:18:40.659Z Reads: 199

```
@evoheyax I've one question what do you mean more than a few weeks ride time?.
```

---
## \#10 Posted by: ajaynagra Posted at: 2016-11-05T21:31:35.074Z Reads: 199

```
The motor mounts
```

---
## \#11 Posted by: BexBle Posted at: 2016-11-05T21:39:34.768Z Reads: 201

```
No I will be making a design on my PC. Then I will 3d print it to check if it works. then once I get it working i will send the design to a friends dads company to cut the clamp for me. I will make the motor plate by hand and a drill out of carbon fiber.
```

---
## \#12 Posted by: evoheyax Posted at: 2016-11-05T22:00:45.909Z Reads: 213

```
Essentially, A lot of people build boards, but the quality of materials and the engineering of the electrical system is very important. If you want your electronics to last, you need to keep heat down. Heat kills electronics. The by product of drawing amps is heat is generated. So this is why higher voltage (10s or 12s) is recommended. The problem with higher voltages is that there's not a lot of hobby grade escs that can do 10s or 12s. And the ones that can are usually around the same price as the vesc anyways.

Theres a lot of details that you must pay attention to if you want your board to last. If your an electrical engineer and really understand this stuff, you can build a board for under $500 USD (which is what, like $350 euros) if you already have the tools you'll need (i.e. soldering iron, heat gun, hot glue gun, jig saw, maybe 3d printer and/or cnc milling machine). But it's hard to do because hobby grade escs and motors will blow up if you put too many amps through them. Knowing how many amps you will draw determines the gauge of wire you should use, the esc, and the motor. It may also determine if you need at least 2 motors (or in my case, 4 motors). And there's no way to know becuase theres no formula that allows you to plug all of the variables that will determine this (even little things like the duro of your wheels will affect range and amp draw).

We call this the false economy. You think your saving money by buying the cheapest parts you can, but unless you buy exactly the right parts you need considering your riding style, weight, and the terrain you'll be riding in, things will blow up and cost you more money in the long run. I feel into this trap, as many others (including Jason from Enertion) have.

Higher amp (and voltage) escs and higher amp motors (i.e have thicker gauge phase wires) are more expensive. There's no sensible way to control amp flow of a hobby grade esc. You can change settings which in turn limit amps flowing to the esc or to the motor, but they give them names like acceleration, and have values like high, medium, or low. There's no mathematical/scientific way of knowing what the actually numbers are, and thus, your likely to blow up escs and/or motors.

This is why the VESC is highly recommended. You can control whats happening and protect your electrical system. You can prevent ESC overheating, pulling too many amps from your battery (which could destroy your battery and/or esc), pushing too many amps into your motors (which could destroy your motors), and many other limits.

If you don't have your electrical system engineered correctly with proper gearing, you will be able to ride at first with little to no issues, but something will blow with in a few weeks (or when you push its limits on hills). If your macanical system is not engineered correctly, belts constantly breaking will be the least of your issues.

A properly engineered system should never break, but the reality is, most are riding systems that could be improved with proper engineering.

The other thing is, many will try to convince you that you can go the keep route without issues. There's only a handful of builders that I know who have done this successfully that use their boards to commute like this. I know because I commute over 50 miles (or 80km) per week, and have built many boards cheaply that do this. Many with cheaper setups don't ride very often and/or live in flat environments. If you expect to go up hills, understand what effect that has only the max amps you need your esc to be capable of drawing (will likely double or triple it).

Even buying a vesc, not all vescs are the same. Chaka, for example, has upgraded his vescs so they are more robust. Many have had issues with enertion or diy's vescs. You want a warranty on something like this, because if you buy two (like I did) and one comes broken and the other breaks on day 2, your out a lot of money. again, the false economy of thinking you can save a few bucks for something that looks exactly the same, but are not.

My recommendation is, don't build your own board because you need to save money. Build your own board because you enjoy the building process or because you want to build something more robust and powerful than what's already on the market. Because the odds are, you'll spend at least twice your original budget before you have board that works for more than a few weeks.

Most people don't need what I'm riding right now, but being DIY, and having engineered this board correctly before building it (based on testing and data I've gathered in the past), It still came out to a little more than $1800 USD (or $1615 euro). A good DIY board should cost in the range of $1000 USD to $2000 USD. You can build a good board for less, but make sure you have the knowledge and know what your doing, or you will waste a lot of money. I don't know many builders that have successfully built their first board for under $500, that actually get the range your looking for.

Also, you need way bigger batteries than 5 Ah if you want the kind of range your looking for. A minimum of 10 Ah if your a light guy and riding on flats, higher if your more than 150 lb and want to ride hills. On my first board, After blowing up 3 ESCs and 3 motors (one being an expensive r-spec due to too high of the acceleration parameter setting in a hobby grade car esc), 8000 mAh could get me about half the range your looking for. Given, it was on 6s, not 10s, but even the space cell (which is 10s at 7500 mAh or 10000 mAh) won't get you that long of a range. For that kind of range, you need at least $250 eruo in batteries alone...
```

---
## \#13 Posted by: BexBle Posted at: 2016-11-05T22:21:25.477Z Reads: 182

```
Thanks soo much. last 2 thing could you recommend me a:

Battery to go 15-20KM range
ESC, motor and controller to go with.
Thank you also I'm a bit confused between mah ah s c I know I'm asking a lot but could you please explain these and which one I need to increase to get more range.

Thanks Reuben
```

---
## \#14 Posted by: evoheyax Posted at: 2016-11-05T22:50:23.641Z Reads: 185

```
1 Ah = 1000 mAh.

I have crunched the numbers, as I'm working on build a cheap complete cruiser that would serve as a good introductory board for new riders. This build would include:

- Deck with hollow channels (or integrated enclosure like the one you posted above) (depends on your cost of materials and tools needed)
-  ESC: VESC-X with warranty (~200 euros) or Ollin board (chaka on this forum) VESC (~150 euros with 2 year no questions asked warranty)

- Battery: Personally, I like 18650 li-ion cells. But they are more expensive in the short term (but they last 4 time + longer, so they are really cheaper in the long run). For the range you want, no less than a 10s4p, which is 40 cells. 10s5p (50 cells) would be more likely what you want or even a 10s6p (60 cells). I use the LG HE2, due to the low internal resistance and they are cheaper than the other good cells like the Samsung 25R). at ~4.50 euros a piece, That's 225 euros for a 10s4p, 270 euros for a 10s5p. Plus bms (~35 euros) and a charger (~35 euros) and a matching charging port (~5 euros. You'll likely have to buy a pack of 10) so that's really 300 euros for 10s4p or 345 euros for a 10s5p. You also need heatshirnk and solder, which is probably another 30 euros (you need a lot of solder to build a battery pack and it's not cheap), or you can spot weld them if you have a spot welder. For lipos, I would recommend 4x zippy 8000 mAh 6s and running 12s. You'll draw less amps (which means less heat, better for electronics) and get the ranger your looking for and some. but they are ~80 euros a piece, plus you need a balancing charger with lipos, which can be 40 euros for a knock off, unknown quality imax or 100s for good ones.

- Motor: I like the R-spec (~100 euros). Many have had great success with the sk3, which can save you a few bucks. I have no experience with sk3 motors though, so I can't speak from experience.

Personally, I think the mono drive kits from enertion are a steal for new builders like you. You get everything you need minus the battery, esc, board, and a transmitter/receiver. They are around $350 euros, and add a 300 euros battery + 100 euros for a board + 150 euros for a chaka vesc + ~40 euros for a remote (I'm using the mini trigger sold by DIY and many others on this forum) and you would have what your looking for with quality parts for ~940 euros. That's as cheap as I think you can make a quality board with the kind of range you need.
```

---
## \#16 Posted by: evoheyax Posted at: 2016-11-05T23:01:26.806Z Reads: 157

```
yes, thank you *bangs head on desk for forgetting a 0*

My mind was there, but my fingers, were not, haha.
```

---
## \#17 Posted by: BexBle Posted at: 2016-11-05T23:35:34.233Z Reads: 152

```
Thanks soo much again could you please direct me to a tutorial for the cell battery packs.
```

---
## \#18 Posted by: evoheyax Posted at: 2016-11-05T23:45:55.401Z Reads: 164

```
This seems to have a lot of good info: http://www.powerstream.com/BPD.htm

I don't really have a one stop solution to building your own battery pack. What I can tell you is the way I solder them is by wetting the cell on both ends with a nice little pool of solder. Then cut a piece of wire howevery many cells wide one p is. I strip one end of the wire, solder that to one cell, and pull the heat shrink on the wire offso I can solder the next cell until I get 1p built. Then, I solder a balance wire to the positive side and heat shrink it. Do that how every many s you have and trim the wires and attach the correct balance plug.

The beauty of building your own pack from 18650's is you can add cells if you realize your not getting the range you need. You shouldn't mix super old cells together with new, but I've used cells with maybe 20 discharge and charge cycles (which is plenty to determine your range) with no issues. Just make sure they stay balanced.

With the bms, you can get away with using it for charging only if you use a vesc. You need to make sure you configure the right voltage cutoffs in the vesc's settings. But the vesc will do essentially what the bms does in discharging, so you don't need to spend 60 euros more for a high discharge bms. Just split the negative wire from your final battery pack into two dirrections. One goes to the bms p-, and the other goes to your vesc. This way, current during discharge is not drawn through the bms, but essentially around it.

Another fun fact: I haven't used a bms on my board for the last 400 or so miles, with no issues of balancing needed. Eventually, they will get worse, but you can survive without a bms. But I also use an LED panel to display all of my voltages of each p of cells. So I can confirm it. And building the panel was around $60, so it was more expensive actually going the no bms route.
```

---
## \#19 Posted by: BexBle Posted at: 2016-11-06T21:22:50.283Z Reads: 149

```
Thank you, I have decided to go ahead with the build. Have you seen jasons from enertions $400 build would that be alright.
```

---
## \#20 Posted by: BexBle Posted at: 2016-11-07T01:44:59.723Z Reads: 150

```
@evoheyax

Does increasing the voltage increase range or speed or does
increasing mah increase range.

Thanks Reuben.
```

---
## \#21 Posted by: evoheyax Posted at: 2016-11-07T02:55:23.565Z Reads: 147

```
More mah/ah means more range. Higher voltage mean higher speed. But there's several ways to gain more speed, like gearing or using larger wheels. These both also decrease torque, so it's a fine tuning game between torque and top speed.
```

---
## \#22 Posted by: Hummie Posted at: 2016-11-07T03:11:25.166Z Reads: 134

```
Voltage x ah equals watt hours.  Watt hours is energy.  Energy is range. U can get to greater range adding either
```

---
## \#23 Posted by: Made-in-China Posted at: 2016-11-07T07:18:09.894Z Reads: 124

```
you should to consider software too.
```

---
## \#24 Posted by: TarzanHBK Posted at: 2016-11-07T08:19:43.488Z Reads: 121

```
?
#10characters
```

---
## \#25 Posted by: Maxid Posted at: 2016-11-07T09:43:38.765Z Reads: 120

```
That is not correct. More mah means more range if the voltage stays the same: a 6S battery with 5Ah will have half the range than a 6S battery with 10Ah. If you also increase voltage however it becomes just like @Hummie said: the total watt hours are what is important for range. Meaning with 12S 5Ah you will not only double the range compared to a 6S 5ah but also the speed. This is all neglecting any real world losses however.
```

---
## \#26 Posted by: BexBle Posted at: 2016-11-07T09:49:24.339Z Reads: 117

```
I know its hard to estimate but do you think x4 5000mah batteries wired in parallel and then in series(or in other way around idk which better) would get me 15-20KM range and 35-45KM/H speed @evoheyax. @SirDiff. @TarzanHBK. @ajaynagra.

Thanks.
```

---
## \#27 Posted by: Maxid Posted at: 2016-11-07T10:00:02.860Z Reads: 117

```
You can't wire the same batteries in parallel AND series. Just stick to the roufh estimation of 10Wh gives 1km.
```

---
## \#28 Posted by: BexBle Posted at: 2016-11-07T10:17:44.114Z Reads: 114

```
I mean wire 2in serises and two in parrellel
```

---
## \#29 Posted by: TarzanHBK Posted at: 2016-11-07T10:26:39.408Z Reads: 113

```
so if you choose these 5s 5000mah x 4 - 2 in parallel to get 10000mah and then 2 parallel packs in series to get 10s 10Ah.
= 370Wh = estimated 37km (depends on your motors, gearing, weight) but you should get 30km if you´re not crazy fat ;)
```

---
## \#30 Posted by: BexBle Posted at: 2016-11-07T10:44:37.976Z Reads: 115

```
Thanks. No im not im 54kg😂😂
```

---
## \#31 Posted by: BexBle Posted at: 2016-11-07T23:01:55.658Z Reads: 109

```
Do you think two of these will get the range of 20KM

<img src="/uploads/db1493/original/3X/8/b/8bffd8b8dfb62be418507defc1eb7271b7994b5c.PNG" width="666" height="500"> and wich one should is hook them up in series or parrellel. Thanks. @Maxid @Hummie @Blasto @SirDiff @evoheyax @ajaynagra @onloop.
```

---
## \#32 Posted by: BexBle Posted at: 2016-11-07T23:02:48.463Z Reads: 107

```
<img src="/uploads/db1493/original/3X/a/2/a2381a3a7133c92e6a7acd3766bf5fa81f009f0b.PNG" width="666" height="500">
```

---
## \#33 Posted by: Maxid Posted at: 2016-11-07T23:02:56.337Z Reads: 97

```
you can calculate this yourself. we told you the formula. I will not spoon feed you.
```

---
## \#34 Posted by: Hummie Posted at: 2016-11-07T23:13:14.188Z Reads: 96

```
Probably.  Figure the watt hours.  8x (let's say 50 because it's simpler)= 400watthours.  I've done 8ah at 12s and done 20miles easily.
```

---
## \#35 Posted by: BexBle Posted at: 2016-11-07T23:19:54.371Z Reads: 94

```
Series or parellel
```

---
## \#36 Posted by: BexBle Posted at: 2016-11-07T23:26:26.978Z Reads: 94

```
Thanks so much guys u helped allot. Acording to my calcuations ill get 17.7KM which is alright. Stay tuned for a build😂😂😅😇😉.
```

---
## \#37 Posted by: Mobutusan Posted at: 2016-11-08T07:13:45.772Z Reads: 91

```
I have two of these exact batteries in series and get between 21-25km around town, on flat ground, riding moderately aggressive. I'm 80-85kg fully loaded, and this is on a dual 6355, 230kv, 14/36 belt drive, on 83mm wheels.
Hth.
```

---
## \#38 Posted by: BexBle Posted at: 2016-11-08T12:10:41.731Z Reads: 91

```
So ill probaly get a bit more weighing less and on 1 motor. Thanks what vesc do you use and what do u mean mideratly aggresive.
```

---
## \#39 Posted by: Mobutusan Posted at: 2016-11-08T18:58:53.123Z Reads: 85

```
I'm actually running dual Torqueboards 12s esc's. VESC might be more efficient and get better range, but I haven't used one yet. 

And by moderately aggressive riding, I mean generally cruising around town, but accelerating hard and doing 25-30+ mph speed bursts whenever I can. Half cruising, half racing, I guess. I definitely got a couple extra miles out of riding slower and more conservatively.
```

---
