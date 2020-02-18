# Will 18650 30Q batteries work for me?

### Replies: 12 Views: 425

## \#1 Posted by: Strobi1 Posted at: 2019-02-19T15:31:41.393Z Reads: 160

```
I've read a bunch of debates about the differences in batteries, but I'm not sure if any of the conclusions relate to my build.  I'm 230 lb (104kg) building board with 8 inch inflatable tires and will be using it off-road as much as on-road.  I want to build a 12S4P using samsung 18650 30Q batts.  I only have a limited knowledge of how a VESC works and that is probably my problem with the math.  Considering the max draw of my 2 motors is 6400watts and the 30Q batteries max continuous output in a 12S4P setup is 2700ish watts makes them sound way under powered (will I realistically ever even hit that number?).  By the way all of the debates seem to go is that this setup is fine.  What could be reasonable expectation of actual current draw given my weight and the fact that I am on inflatable tires?  Do I need to put more cells in parallel to accommodate my requirements? 

Here are my specs.
MBS ATOM mountain board
203mm inflatable wheels with - 84 tooth pully
Dual 6374 BKB 190KV 3200watt max 70amp motors -15 tooth pulley
FOCBOX Unity (160A continous 300A max) on pre-order
15mm wide belts

Thank you very much for your help!!!
```

---
## \#2 Posted by: linsus Posted at: 2019-02-19T15:40:12.823Z Reads: 149

```
While the datasheets does not lie, relying only on continuous isn't realistic, You'll have peak amps well above the continuous and thats fine, aslong as its not for extended periods. Batteries are as much about temperature as it is about current draw. If you're in a warm climate then they're prob more prone to high temp than if you're in a cold climate etc. With all things considered from your description, I'd probably add atleast one cell parallell. Given your weight and setup. I have something very similiar but I'm rougly 30 kgs lighter and dont do offroad.
```

---
## \#3 Posted by: evoheyax Posted at: 2019-02-19T17:30:14.231Z Reads: 123

```
Well 30Q can do 20amp each, so your looking at 80a max with a 12s4p. You could in theory do 4000 watts, which is pretty good.

But you will not hit the 160a the unity can do. At 80a, the voltage sag will be heavy. You'll probably go from 50v straight down to 44v. And once your at 48v (which is pretty quick), you'll be sagging to 42v.
```

---
## \#4 Posted by: Strobi1 Posted at: 2019-02-19T21:57:07.010Z Reads: 102

```
Thanks for the advice @linsus ! @evoheyax do you have any battery type or configuration advice for me?  Should I build what @linsus suggested and just leave room to grow if that is not enough?  or is there a cell you guys would recommend that would suit my setup better?
```

---
## \#5 Posted by: evoheyax Posted at: 2019-02-19T22:24:06.622Z Reads: 101

```
It's not that the 30Q won't work for you, it will. I just think you should ask yourself what are you looking for?

Lipo gives best performance, highest risk and lowest battery life (400+ cycles).
Lithium Iron cells have decent performance, much safer than lipo or li-ion, super long life (2000+ cycles), but low energy density.
Li-ion cells have ok safety (much safer than lipo in theory).

What do I run? Lipos all day. But that's cause I want performance. So you have to ask what do you want.

The issue I have with li-ion is the voltage sag and drop off. Most of lipos power is at a higher voltage. At 12s, It drops from 50.4v to 49 pretty quickly, and then stays between 46v and 49v and then drops off quickly after 46v. Li-ion in comparison drops from 50.4v to 49v quickly, then drops at a steady rate until it hits around 35v and drops off quickly again.

Since watts = amps * voltage, when your voltage drops, watts drop. And gearing/motor kv/wheel size aside, this is what is going to determine the oomph of your acceleration.

So with li-ion, later in your ride, you'll feel way less acceleration than on a full charge. You'll notice a difference on lipo boards too, but not very much of a difference, since the voltage doesn't change very much.

Lipos need extra care though. Lipos will puff over time. How quickly, depends on how you treat them. Too much pressure, and boom! Li-ion and lithium iron cells don't have this risk or issue. For me, the solution is simple. Larger battery than I need so I don't discharge it low or charge it high. But it comes with a risk still.

One cell you can look at is the Samsung 30T. It's a slightly larger cell and more pricey, but... They have half the voltage sag of a 30q at double the discharge (40a instead of 20a per cell). These are great cells, but they are at least double the price. A 12s4p would allow you to get the full 160a out of the unity. This would give you 8000 watts at full charge, which is more power than most know what to do with.

With the 30T, you could also go smaller, i.e. 12s3p or even 12s2p, if range is not an issue for you.

Other wise, 12s6p is a really nice size for the 30q. Again, 4000w is a lot for most people. And even at 80a with the 30q 12s4p, you can still hit 4000w. Your in the right area, just need to ask yourself about your priorities (range, price, level of safety, power of your acceleration, long battery life).
```

---
## \#6 Posted by: Strobi1 Posted at: 2019-02-20T03:39:33.036Z Reads: 77

```
Thanks @evoheyax for that huge amount of info!  Going Lipo was actually my initial choice but I decided against it because of all of the potential issues (I have a bunch of them for RC stuff and charge all of them in a metal box).  The 30T does look pretty nice, but man is it pricey! just like you said, about double.  This brings me back to the 30Q...As I said before, I really should be more versed on how a VESC works by this point, but I guess this project has been broken down into less overwhelming bite sized chunks, so that will come after battery selection.  I guess at this point my real question is: can I program the VESC to limit the current draw so I don't over draw my batteries (of course at the expense of performance)?  I could I build this initial battery with the possibility of parallel expansion in mind and see what it gets me.  I would probably consider it a win if it moves me down the road and as I figure out what my true goals and desires are.  I can expand the battery accordingly.  Would that be a valid plan?
```

---
## \#7 Posted by: Battosaii Posted at: 2019-02-20T05:33:06.100Z Reads: 63

```
Are you used to riding esk8?

If not the power a 12s4p can deliver is a bit overwhelming. @evoheyax has great advice but trust me that motor set up and battery is very very fast and will take time to grow into even if you have some esk8 experience.

Btw I'm much much heavier than you and I've taken a similar set up 40+Mph
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-02-20T05:50:37.144Z Reads: 60

```
God dammit I've never hit 30mph and my rspec drive kit maxes out at  29.6mph FML.

Untill my TB DD comes :smiling_imp:
```

---
## \#9 Posted by: Battosaii Posted at: 2019-02-20T05:55:15.989Z Reads: 61

```
Passed my buddy today going full throttle top speed on a Raptor 2, I was on my board only a little over half throttle passing him lol

Rspec drive train should do 30+ with 12s no what's your battery set up and are you running 90 or 97mm wheels?
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-02-20T05:58:58.483Z Reads: 60

```
10s 90mm wheels waiting for my unity and out wheels 😭
```

---
## \#11 Posted by: MysticalDork Posted at: 2019-02-20T08:37:47.311Z Reads: 50

```
It should also be noted that motor ratings are more like guidelines, and if you feed them 3200W each for more than a couple minutes without serious airflow, they'll overheat. The only time you'd get near that rating is during heavy acceleration uphill. Cruising on level ground, even on dirt and rough terrain, I doubt you'd draw above 1KW total. 

I'm 210lbs and was running dual 6355s on 10s4p, 40 amps in and 60 amps out per motor with 6" tires 15:60 and I couldn't stay on the damn thing if I mashed the throttle.

Even with a severely limited battery, the ESC acts as a buck converter, which allows it to feed more amps (and less voltage, same watts minus losses) to the motor at low speed than the battery is supplying. 40 amps in and 80 amps out per motor isn't uncommon. This means that until the power going to the motor (volts times amps) equals the maximum power output of the pack, you won't notice a significant difference in low-speed torque and acceleration between a 40-amp battery and a 160-amp battery. It's just a matter of where on your acceleration curve it tapers off - a battery with more current capability will be able to keep you accelerating **hard** for longer and to a higher speed before tapering off. They'll both hit the same top speed, and both launch just as hard, but the 160 amp pack will keep accelerating harder, longer.
```

---
## \#12 Posted by: Strobi1 Posted at: 2019-02-22T03:02:48.440Z Reads: 33

```
This is my first ESK8 ever.  I have snowboarded for most of my life and skated some, so I hope it won't be too hard to pick up :grin: I want to thank all of you for such great advice.  I still have a ways to go with this project, but I definitely wouldn't have gotten this far without your help.  Well maybe that's not such a good thing.  This project started out with stripping 2 razor scooters and building a board out of that.  I quickly decided that just would not do, so here I am several hundreds of dollars later :rofl:  Time to build this battery pack!
```

---
