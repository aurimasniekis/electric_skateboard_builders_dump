# Connecting Samsung 25R 10S1P battery packs with different charge voltage in parallel (e.g. 41v max and 3.5v min): bacon pan/ smokey/ fire/ explosion in your face - what could happen? Use of diodes?

### Replies: 9 Views: 501

## \#1 Posted by: composites_r_awesome Posted at: 2018-06-24T16:59:45.048Z Reads: 136

```
Hi Hivemind!

I'm making 'universal' 10S1P/5S2P battery packs I dream on using on everything I could power with electricity.  
  
They would have 4-point charge indicators on them, but I'm still wondering what are the risk factors if I would parallel stack those batteries into eboard or hedge trimmer and one of them would be like 38 volts instead of 41 volts?  


Thank you in edvance
```

---
## \#2 Posted by: Okami Posted at: 2018-06-25T08:22:51.555Z Reads: 102

```
In theory current should start rushing to lower charged packs..

 not sure how fast but some balancing should happen non the less
```

---
## \#3 Posted by: karma Posted at: 2018-06-25T14:58:01.066Z Reads: 84

```
Connecting 2 batteries in parallell with different voltage can lead to high currents from the higher voltage pack into the lower one. Exemple, one pack is 42 and one 34V, just differently charged 10S1P batteries. Difference is 8V and the resistance is the completed circuit will be quite low since each cell has a small internal resistance. 20 mili Ohms in each cell (10-30 mili ohm is normal internal resistance of 18650 li ion) , 10 in series and 2 packs  => 0,02x10x2 = 0,4 ohms. This will create I = V/R = 8/0,4 = 20A flowing into the lower voltage pack which is around 5-8 times the rated max charing current which could permanently damage the pack or destroy it.
```

---
## \#4 Posted by: composites_r_awesome Posted at: 2018-06-25T19:34:18.018Z Reads: 64

```
THank you! for doing the math:)  
  
I was wondering before, jep - the 'charging' current would like 10x the safe rated of that, but even if the difference would be 8 volts, when I tried charging a 3.4v battery on smartcharger with 6a current it took the battery like 2-3max seconds to reach 4.1 volts (?)
  
I'm wondering if I would connect the batteries in parallel like that and the voltage would equalize in 3 seconds, does the current stop as well?  Will it really shorten the lifespan on battery?  
  
I [plan on using 4-point charge/voltage indicator](https://www.aliexpress.com/item/Non-Waterproof-3S-Lithium-Battery-Capacity-Indicator-12-6V-Battery-Power-Display-Board-Tester-Li-po/32786264984.html?spm=a2g0s.9042311.0.0.27424c4dkpbGd1) on all of the batteries and make sure all users would know not to connect battarais in parallel if indicators are off  
  
With max 4-volt differenace, a 3-second burst of 10A would still do enough damage?
```

---
## \#5 Posted by: karma Posted at: 2018-06-25T20:37:30.223Z Reads: 52

```
No problem, reading up on batteries with the
[Batteries in a portable world](http://batteryuniversity.com/buy/) book so getting to use the knowledge helps learning. It is free to read online and has good explanations and guidelines. 

If you would connect the packs in parallell they would balance out themselfs until they have the same voltage and no current would flow. However there is a max charing current rating for a reason. 1. Higher charing current than rated drastically shortens the life span, like alot. 2. If the current is too high the temperature would rise and in worst case senario this could lead to thermal runaway, gas buildup, venting and potentially fire.

What you could do to make it safer is to balance both packs before connecting them in parallell with the help of a balance charger. Example: balance the 10S1p pack so that all cells are 4.2V then disconnect and connect them to 5S2P.
```

---
## \#6 Posted by: karma Posted at: 2018-06-25T20:43:19.221Z Reads: 47

```
The voltage indicator you linked is only for 3S and shows LEDs at 3,2 3,4 3,6 and 3,8V. That seems a bit weird as li ion is fully charged at 4.2V each and not 3.8V. Having one that displays the acctual voltage would be better.

10A charge on a max charge rated current of 3-4A is still about 2.5-3.3 times more than allowed. It will definetly be bad for the cell and I would strongly recommend against it. 

Why not do 2 packs? One 10S1P and one 5S2P or do a 10S1P and use a voltage regulator (buck) to reduce the voltage when needed?
```

---
## \#7 Posted by: Ishayc Posted at: 2018-06-26T05:54:42.459Z Reads: 34

```
[quote="karma, post:3, topic:59922"]
0,02x10x2
[/quote]

the packs are in parallel so the resistance would be 0.1(0.02x10x0.5) which theoretically will cause 80A running between the packs.
```

---
## \#9 Posted by: karma Posted at: 2018-06-26T11:41:13.401Z Reads: 27

```
Yes they will be in parallell when they have the same voltage. However when they have different voltage they create a complete Circuit where the voltage diff. creates a current through every single cell in both packs. So you would have to take every single cell resistances and add them upp that’s why I wrote 0,02x10x2.

When they are balanced, connected in parallell and connected to a load then they would appear to have lower resistance because the current can take multiple ways through the 2 parallel groups of batteries.
```

---
## \#10 Posted by: composites_r_awesome Posted at: 2018-06-26T18:50:18.180Z Reads: 22

```
Jup I planned on connecting it to 3 of the cells there because it only uses current when it's ON, tho I only intended to use them for broader view of battery status like tool batteries have. The cool ones with displays wouldn't fit due the batteries would only ~20mm in thickness although I could still mount them differently or make the battery enclosures way more robust. Jep, I think I'll go with voltage display ones rather than the indicators

I would be making about 12 of those with both 10S1P and 5S2P wiring in them
I like the 10S1P because of the airline approval. I've heard people getting the airline's go-ahead for multiple <100Wh batteries if they're using proper labebs and 'battery' bags <:P

I would LOVE to use this ride around in foreing cities and metrpolises:)))
```

---
