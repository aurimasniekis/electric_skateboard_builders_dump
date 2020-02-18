# How many LiFePo4-s do i need for my motor?

### Replies: 14 Views: 400

## \#1 Posted by: IvanNott3rrible Posted at: 2018-09-27T13:56:07.994Z Reads: 124

```
Hi.
I am building an esk8 for the first time, and I am planning to use LiFePo4, but the problem is that I really do not know how many I need for my motor.
 (https://www.mboards.co/collections/hub-belt-motors/products/mboards-6355-180kv-motor)
I want to use my board to get to school and back.
Be pretty good up-hill. Have a distance of around 10 miles and go like 15-25 mph, if it's not possible, how many 18650 do I need?
```

---
## \#2 Posted by: Jake2k17 Posted at: 2018-09-27T14:02:56.554Z Reads: 120

```
I would recommend using Samsung 30Q liions, they are the most commonly used cell on this forum. For 10 miles of range use a 10s2p or 10s3p
```

---
## \#3 Posted by: deucesdown Posted at: 2018-09-27T14:39:24.967Z Reads: 117

```
[quote="IvanNott3rrible, post:1, topic:69355"]
I am planning to use LiFePo4
[/quote]

[quote="IvanNott3rrible, post:1, topic:69355"]
18650
[/quote]

Don't do this. There are no LiFePo4 18650s that are appropriate for eskate. If you go LiFePo4 the most common cell is A123's 26650 (which are not generic LiFePo4 but a superior version).

Most likely you want to do 30q. The number of cells will determine range, but also the amount of power (and braking) your board will have. Unless you're really light or want to go really slow, typically it's 10s4p or greater.
```

---
## \#4 Posted by: IvanNott3rrible Posted at: 2018-09-27T14:43:23.220Z Reads: 107

```
Do you think 10s2p will work?
```

---
## \#5 Posted by: ElectricCoast Posted at: 2018-09-27T15:10:30.994Z Reads: 98

```
what type of wheels are you using?  urethane? Gummies? Pneumatic?
```

---
## \#6 Posted by: boogiewookie Posted at: 2018-09-27T15:25:25.332Z Reads: 89

```
10s2p would just about get 10 miles and top at 21.5 mph with some hills assuming you havee 80mm wheels
Here is a calculator that shows range and top speed depending on your setup
http://calc.esk8.today/
If you want to increase your top speed I recommend getting a 190kV ~ 200kV motor or do 12s on the 180kV or increase your wheel size
If you want more torque for those hills 10s2p with the same motors would work with 80mm wheels

TIP: Remember top speed increases with bigger wheel size, higher kV and more voltage at the expense of torque, except voltage doesn't get affected. Higher voltage is always better!
BUT you also need a VESC that could handle 12s which is $$

edit: forgot pulley ratio too gotta consider that 36T/15T is standard
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-09-27T15:29:44.768Z Reads: 85

```
don't buy anything from mboards.

the guy's sketchy af.

i really like the [hobbyking motors](https://hobbyking.com/en_us/turnigy-sk8-6354-140kv-sensored-brushless-motor-14p.html), buildkitboards got some, diy, psycho, etc.

a 2p lifepo will sag like crazy and you'll get shit range like a boosted.
```

---
## \#8 Posted by: IvanNott3rrible Posted at: 2018-09-27T15:36:07.856Z Reads: 78

```
I live in norway so I can't really lagally go super high speed, but do you think my current motor will be ok in 10-25° hill with a 10s2p battery?
```

---
## \#9 Posted by: boogiewookie Posted at: 2018-09-27T15:45:50.955Z Reads: 76

```
In short, yes, but as @thisguyhere said mboards motors is not reliable
I recommend you do some more reading and research to build a list of things to buy first then ask us to help you cause we have no clue what your other components are
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-09-27T15:49:12.983Z Reads: 73

```
there's much better esk8 sources in europe, why would you order something from the US.  i know that guy's youtube videos are enticing but he doesn't really know what he's talking about.  he was a new builder like yourself a year ago and now thinks he can run a business.

https://www.electric-skateboard.builders/t/trusted-sellers-and-builders-these-people-will-not-rip-you-off/48508
```

---
## \#11 Posted by: evoheyax Posted at: 2018-09-27T16:20:33.511Z Reads: 61

```
I agree with thisguyhere, 10s2p will sag like crazy and range has a lot of factors.

- First off is weight. A 200 lb guy will use twice as much energy as a 100 lb guy.
- Second off is wind resistance and motor efficiency. For a 20-30 mph build, you are most efficient between 12-17 mph. Less then that and your motor will run inefficiently, and more than that and wind resistance becomes a huge factor. Remember, wind resistance is an exponential, starting to increase at around 17 mph. Even at 22 mph, you'll use twice as much energy as 17 mph from wind resistance, and 30 mph instead of 17 mph will be 4 to 5 times as much energy.
- Third off is your riding style. Are you gunning it from stop sign to stop sign, or are you coasting at a constant speed. This will change a lot.
- Fourth off is hills. Hills will make you draw exponentially more power. Even a slight 3% grade hill will double your power output. 10% grade will be 6-8 times the power output, assuming your board is setup be able to do this that is. I'm assuming you want to maintain the same speed and the board can use more power to do so. Other wise, you'll slow down, and possible completely stop if your board is not strong enough.
- Fifth off is tires. Air filled rubber tires get far less range than urethane wheels. But they are far more comfortable on less than perfect roads.

If your on the wrong side of the spectrum like me, a 10s2p could yield as little as 1.5 miles. Even a 10s4p only yields me about 3 miles. Again, I am on the more extreme side of things. But you have to ask yourself these questions and understand best case scenario, you get 10 miles from a 10s2p. Your range you tank quickly if you have any of the factors posted above.

I personally would need a 10s7p to get 10 miles of range comfortably. That is a massive battery pack for an eskate though. Why? Cause I'm 190 lb, I go stop sign to stop sign, gunning it in between to 30 mph and back down to 5 mph for the stop sign. I then have a long straight where I do a constant 30 mph (huge wind resistance) and all of the stop sign area of my rides are super hilly. All of these together destroy my range.

Just take the ranges anyone gives you with a huge grain of salt. It's a best case scenario, and what a 120 lb guy riding nothing but flat ground at 15 mph constant on urethane will get. Not to mention the sag... You'll go from 42v straight down to 36v right off the bat. Then you'll hit your low voltage cutoff shorty after that, which will drastically decrease range. This is where lipos are great (but they are more dangerous than li-ion, which is also still very dangerous. The lithium iron phosphate you mention is the best of both worlds. Higher discharge rates than li-ion, better discharge curve like lipo, and they are safest by far. I and many other have still lost boards to li-ion fires.

I run headway 15ah cells in my ebike and I am trying to figure out how to fit them on an eboard because of their safety.
```

---
## \#12 Posted by: Hummie Posted at: 2018-09-27T17:08:08.588Z Reads: 57

```
But @evoheyax uses the blue headway cells and they sell a high discharge red cell which will put out more amps with less sagging. At 2p I think those or some other iron cells could be good. All depends on the cell size as well.  A123 has done good high discharge cells too.  It need not be a problem with iron and few cell count
```

---
## \#13 Posted by: evoheyax Posted at: 2018-09-27T17:12:16.359Z Reads: 56

```
Iron cells don't have a discharge issue. Even the blue ones I use are rated to 200a. They are heavy, that's it. the cells I use are 1.1lb each, and with 14 of them to reach ~48v full charge, that's over 15lb on battery for about 1kw of energy.
```

---
## \#14 Posted by: Socrates Posted at: 2019-03-15T12:51:23.996Z Reads: 36

```
Hi there.
I have been studying a lot about EV and this forum around 1 year ago.
Im building my first board.

( 8S )
 Dual Motor SK3 - 6374 - 190kv - 70-80A - ESC 8S Ezrun Max6 - Mountainboard 
             -  Tires 200mm 
             -  Pulley 15T   Big 65T - Belt

My question its about Batteries, in order to have a good speed, how much Discharge Current Const will be good to support, like 40 - 45 km/h Const. cruise ?

I dont know how much time the motor sk3 6374 works fine running around 40-45 km/h Cruise Speed loading total 90 kg without blow up the ESC or motor.

Dual Motor (8S):
            - Discharge Current Const.:  For   Single Motor ->  xAmps
                                                                  Dual Motor   ->  xAmps
       
            - LiFePO4 Headway 15Ah 5C ( 75A ) -  8SxP
            - LiFePO4 Herewin 30Ah 3C ( 90A )   -  8SxP
     
Please, Could someone help me guys to solve the ''x'' ? 
1P its enough ?

Thanks all you guys to share the experiencies and knowledge :nerd_face:
```

---
