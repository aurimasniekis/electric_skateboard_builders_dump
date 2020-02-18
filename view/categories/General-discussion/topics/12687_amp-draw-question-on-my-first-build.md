# Amp draw question on my first build

### Replies: 8 Views: 638

## \#1 Posted by: brawlincollin Posted at: 2016-11-08T02:11:12.452Z Reads: 121

```
I'm going to be running a 230kv diy electrics motor. I would ideally like to run 16/36 gears on 90mm wheels. I weight 150lbs give or take a good poop. My question is that I'm trying to decide running a 8s or 6s li ion battery but curious on what the amp draw would be. Also thinking about running a 8s but making 2 4s packs and running in series but, charge them in parallel using a vgs style connector. Do you guys think I can charge each 4s pack using 16 to 18 gauge wires using a balance charger? But still discharge the batteries with 10 to 13 gauge wire
```

---
## \#2 Posted by: TarzanHBK Posted at: 2016-11-08T08:39:07.071Z Reads: 105

```
Get 2 4s batteries for that motor.
Amp draw is as much as you feed the motor with till it reaches it´s Watt limit.
8s = 3,7V x 8 = 29,6V
Watt = Voltage x Amps

Charge each pack separately with a balance charger and yes you can use thinner cables. Use cables rated for the amount of amps you´re charger is capable of.

For discharging use 10G wires to avoid any resistance.
```

---
## \#3 Posted by: Okami Posted at: 2016-11-08T10:12:50.647Z Reads: 100

```
Im still no expert in terms of amp draw, especially for longboards.. you can try to look up some of the '' whitepony '' posts, he has pushed his board to the extreme I think.. :D

Would say go for the watts rating.. try to figure out how much power / watts you would need in everyday use.. not peak watts, but the continous ones..

Then based on that you should get a rough estimate on what continous amp draw should be and at what batteries to look at.

---

BTW - what's gonna be your motor controller / esc? Does not seem that you gonna be using vesc for this ''low voltage'' setup. Definately harder and more expensive to go with 8s I think, as 6s esc's are cheaper and more common, in my opinion.

--

I've got a mountainboard.. so far I have reached 60A max.. that was going full speed and against quite strong wind, watts were about 1200w..

They say - if your battery wont be able to sustain the juice - you wont be able to get as good acceleration and it will start to sag and be ''weak'' a lot quicker.. also it puts strain on the batteries, if you have to overdischarge (too many amps) all the time..

---

For ''normal'' ride, with 15mph / 20kph max or so.. I usually dont get more than 30A peak or so.. at least this is what my watt meter says for my 6s li ion setup (192kv motor, 4,33 ratio, 9inch wheels)
```

---
## \#4 Posted by: brawlincollin Posted at: 2016-11-08T15:02:12.951Z Reads: 78

```
Ok so would you say 30amp peak on a normal ride is about right for my set up? 1 maybe 2 hills that aren't steep. I'm just worried because I accidently bought low discharge cells but I bought quite a few. I think I can run a battery pack capable of 60 amps continuous.
```

---
## \#5 Posted by: Okami Posted at: 2016-11-08T18:12:07.037Z Reads: 67

```
yeah, 60 amp continious sounds like a good number.. you can also try to calculate how much current each cell in parallel pack will output.. let's say, if I have 30A draw and I have 4 cells in parallel, then Each cell would get roughly 7.5A pulled out. Of course, this is for a short momemt, so, for let's say 10A draw (10x 24v = 240w) would give 2.5A draw for each cell.

If you go the 'regular route'' and choose Samsung 25R, and ''abuse'' them with 5A draw, I think they should be okay (you can check the capacity decrease and temp factor in the charts about the cell.

Though - take everything as one guy's experience, I have not done tests on many boards so far.. though, I even ran 25c rated zippy compact 1500mah battery's.. and I did not feel performance decrease in the low - mid spectrum of the ride... did not try to push them to the max.. (their theoretical output was something like 37A, which would yield around 25-30A, If I derate them a little bit.)

--

Hills are a whole different story - have not tried to measure anything yet.. but if you have them, then yeah, take some extra margin / safe zone for the batteries.. depends on the size / incline, of course. I just know that mine sagged quite a lot but I was riding a really tough hill.. too bad did not have wattmeter installed then.
```

---
## \#6 Posted by: Okami Posted at: 2016-11-08T18:17:28.148Z Reads: 60

```
Try to look at some of the '' chaka '' videos.. they have started documenting amp draw and other data straight from the vesc - with video overlay.

I think you should be able to see what amp draw they reach.. though, check their setups.. I think they usually run 10-12s or so.. plus it could be dual drive setup
```

---
## \#7 Posted by: brawlincollin Posted at: 2016-11-08T18:46:52.163Z Reads: 57

```
Ya only problem with his videos is they are usually 12s packs. More voltage means less amp draw
```

---
## \#8 Posted by: Okami Posted at: 2016-11-08T20:16:39.942Z Reads: 53

```
yeah, I faced the same problem as you.. not enough info.. you can just adjust it to your motor ''needs''.. I see it says (for 6355) that the max amps are even 80A.. 

Personally, in the end I stuck with ~22A capable cells.. I had a choise to go with 10A per cell but that would be way too low..

So yeah, try to at least 3-4 cells in parallel at least, the more the better ;) (for the 20A capable ones.. )
```

---
