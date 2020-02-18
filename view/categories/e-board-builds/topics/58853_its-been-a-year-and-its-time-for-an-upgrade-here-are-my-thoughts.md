# It&rsquo;s been a year and it&rsquo;s time for an upgrade. Here are my thoughts!

### Replies: 9 Views: 439

## \#1 Posted by: Geddi Posted at: 2018-06-14T10:54:27.889Z Reads: 210

```
Thanks to the helpful people on this forum I was able to build my own e-skate last year and it was a perfect success. I love it and I ride it whenever I can. Still I am not completely satisfied and I would like to make an upgrade.

My build:

*     5 LiPo 2S 5000mah 40C batteries from Turnigy
*     10S BMS from Bestech
*     Maytech VESC from APS
*     APS 200kv 6374 Motor
*     motor mount from [APS](https://alienpowersystem.com/shop/cnc-kit/alien-drive-complete-kits/alien-drive-systems-electric-longboard-diy-kit-50mm-motor/) 
*     Orangtang 80mm wheels
![IMG-20180203-WA0009%5B377%5D|690x500](upload://iLG8baxIpJ8CNqjvNFyqM95z7pU.jpeg)

My Issues:

1. One of my main problems is that whenever I accelerate the percentage on my battery indicator drops to arround 50-60% and stays there when I keep going fullspeed. Once I stop the battery indicator goes back to 99% immediatly after a short ride. The problem with this that whenever I drive a longer distance my board will stop because it reaches the cutoff point, whlie riding even though there is more than 50% of my battery left. So effectivly I am only getting 50% of my boards capacity and I don't fully understand why. Of course I could set my cutoff voltage even lower, but thats not a good solution either I think. Why does the Battery level drop so quickly when accelerating and riding fast, but then goes back to where it was on stand still? Can Improve this with higher quality batteries? Does it have to do with the C Rating?
PS: I am not sure if this issue has always been there. I rememer that I used to get arround 14-18km out of my board. That seems impossible now. After 8km riding fast an continously the battery level (**while riding** ist too low. If I stop for a min and check it again there is still more than 40% left.

2. I have one motor. I am about 90kg heavy and my motor has enough power to get me almost everywhere I want to go.
My main issue is that when I go into a right curve (especially with tight ones) all the weight will be distributed on the other side of board, instead of where the motor is, which means I can't accelerate in curve. The wheel will just spin through because there is no traction. Most of the time thats not a big deal, but if its an upwards going curve you loose all your momentum and that can be really annoying OR you can't brake when going downhill.
So I will upgrade to a second motor. The motor I have right now has suffered a lot already and I will exchange it for 2 smaller 200Kv ones I think.  Also does it matter if the two vescs are not from the same brand?

3. Batterycapacity in general is not good enough for me anymore. I don't want to buy a new BMS and I love the slim formfactor of my build. 2S Batteries are perfect for that. I was thinking in buying a new deck and mounting the motors backwards. I think with that I will be able to fit another 5 2s 5000mAh Batteries under my deck without compromising my slim fromfactor. At one point it would be a little thicker, because I would have to stack the vesc and bms ontop of the batteries, but thats worth it. That would give me 10S2P and would be a significant improvement. Does anyone else have other Ideas for improving my battery capacity? 
PS: For now I would like to stick to Lipos.

4. The wheels are simply too small. 80mm in a city with tram rails and cracks is critical. Most of the time I have no trouble going over them, but its a hassle and really uncomfortable to drive with. Now I don't want huge offroad wheels, because I would have to change my entire mounting for that. I want to do an upgrade, not bulid a new board. I found these [wheels](https://www.amazon.com/MBS-13401-All-Terrain-Longboard-Wheels/dp/B015GJN0BA/ref=sr_1_5?ie=UTF8&qid=1528972722&sr=8-5&keywords=longboard+all+terrain+wheels). That would be a size improvement of 20mm. Do guys think that will make a big difference? It might, but I'm not sure about it. Do you guys know any other bigger longboard wheels and am I right that I could mount those wheels with my current mount from APS?
I also just found out about [these](https://shredlights.com/collections/electric/products/rough-stuff-wheels-pre-order).

It's time to get back to buisness. I see I missed a lot of new stuff while trying out my first board. I'm excited to get building again. Thanks for the advice in advance guys.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-06-14T12:20:51.822Z Reads: 135

```
I would not recommend adding new batteries in parallel with the 1 yr old ones, the reason the range is so bad is because there is probably a lot of life cycles on those batteries and lipos typically only get about 250/300 cycles
```

---
## \#3 Posted by: Geddi Posted at: 2018-06-14T12:43:57.998Z Reads: 134

```
not even close to that. I would say not even 100 cycles
```

---
## \#4 Posted by: pat.speed Posted at: 2018-06-14T13:33:04.015Z Reads: 120

```
Oh well maybe the cells are just giving up, some do before others, but I still would not add new cells to old ones
```

---
## \#5 Posted by: Geddi Posted at: 2018-06-14T17:00:23.971Z Reads: 91

```
Is there a way I can check that?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-06-14T22:16:39.216Z Reads: 69

```
You would need to measure the ir of the cells, which I can’t quite remember how to do, try googling it
```

---
## \#7 Posted by: wafflejock Posted at: 2018-06-14T22:42:35.230Z Reads: 62

```
There are little battery checker devices that will do it for you.  New charger I just got also shows internal resistance on the cells while it's charging which is nice.

What you describe in 1 is typical in terms of batteries dropping in voltage when under load (when supplying amps) and 'recovering' after they are left to sit and aren't under load.  This happens because of high internal resistance (could also say the C rating on the batteries is too low for what is needed, low C rating = high internal resistance).  If you spread the discharge across more cells in parallel then you will have less voltage dip on an individual cell but the better solution is to use cells with low enough IR or high enough C rating that the high amp draw on it doesn't cause it to dip so much.  40C with 5Ah or 200A max discharge should be able to handle it but perhaps the cells were somehow damaged best way I know to see what's going on with this kind of thing is to use a bluetooth module for telemetry (see metr.at or ackmaniac firmware https://metr.at/r/hmtOO can see my old data there shows about 2V dip or .2V per cell when just getting moving and the battery 'recovers' when it's not under heavy load.  Options are like you said either lower the cut off (don't go below 3.3V per cell, 3.0 is absolute minimum but I wouldn't push it that close to the edge) or get cells with lower internal resistance.

Out of curiosity do you charge at more than 1C charge rate?
```

---
## \#8 Posted by: Geddi Posted at: 2018-06-16T16:18:24.828Z Reads: 42

```
so in theory better qualitiy batteries. Meaning a higher C rating could reduce my issue. And if I add another set of batteries in parallel that should also improve the overall situation right?
No I don't charge them at 1C. That would be 5amps right? I have a 2amp charger.
I will also lower the cutoff voltage just a bit. Thanks a lot
```

---
## \#9 Posted by: wafflejock Posted at: 2018-06-16T23:46:57.783Z Reads: 32

```
Yup and reason you typically want to replace instead of adding is the old cells will have higher ir than the new cells typically since resistance will increase over time and. With lower capacity over time your old cells may end up with lower voltage than the new cells in which case the average voltage the vesc uses for cut offs might allow the low cells to get over the voltage cliff since average is high due to new cells.
```

---
