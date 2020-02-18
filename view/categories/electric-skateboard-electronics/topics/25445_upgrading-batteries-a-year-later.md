# Upgrading batteries a year later

### Replies: 17 Views: 1330

## \#1 Posted by: Sleepingalex24 Posted at: 2017-06-15T18:43:45.417Z Reads: 150

```
I have been riding on a 6s setup for about a year now and am looking to increase my range. Currently I have two of these: [Multistar Batteries](https://hobbyking.com/en_us/multistar-high-capacity-3s-5200mah-multi-rotor-lipo-pack.html). I want to add another pack in parallel but I'm not sure if I can since these are almost a year old and generally batteries in parallel should be the same type. Would I have to buy two new 6s batteries or could I just buy one and add it to my current setup? Also would I be able to just buy this [6S1P](https://hobbyking.com/en_us/multistar-high-capacity-6s-5200mah-multi-rotor-lipo-pack.html) instead of hooking up two 3S batteries in series.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-06-16T05:37:13.184Z Reads: 119

```
Get a meter that can read battery internal resistance and check the value of your old battery cells and if they are 5 miliohm or less and the new batteries are about the same and the new pack is the same mah and C rating, then it might be ok but I would monitor how the packs charge and discharge for the first few cycles just to be sure that they are staying even.
Of course, the best thing to do is to buy all new batteries.
https://youtu.be/xvMIId9uK4c
```

---
## \#3 Posted by: Sleepingalex24 Posted at: 2017-06-18T02:04:58.946Z Reads: 95

```
Hey sorry I forgot to check back up on this. Thanks for the idea! I've been doing some research and I'm thinking about just making my own 18650 pack. I saw your 26650 pack and really liked it but I don't know if I have enough money to buy a spot welder. I plan on using the [Vruzend Pack](http://vruzend.com/product/vruzend_basic_kit/) to make an 8s pack out of the Samsung INR18650-25R but don't know how many I need in parallel. Would 3 be high enough for my motor which draws 20A continuous?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-18T02:30:23.007Z Reads: 92

```
Don't use 25R batteries, they have a bit of a bad reputation for voltage sag.  Apparently they're overrated. 
Better use 30Q's instead.  Even though they have a lower rating, peeps are saying they outperform 25R's.
And I would recommend doing at least a 10s4p

BTW, the 10s2p pack I made with Basen 4500 cells was ok for riding on flat ground but acceleration was a bit weak and voltage sag was excessive when climbing hills.
That's why I went back to using Lipos.
```

---
## \#5 Posted by: Smorto Posted at: 2017-06-18T02:41:14.010Z Reads: 87

```
Hasn't there been talk that this type of system for connecting the batteries can't handle high continuous amerpage? I'll try to find it again

Found it. It says in the post just below this one.
https://www.electric-skateboard.builders/t/battery-packs-no-spot-welder-or-solder-required/25135/18
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-18T02:55:45.916Z Reads: 83

```
Kudos to @Smorto for the informative link. 
So based on that I would not even try to use the bolt together system. 
Another option if you don't want to invest $200 for a welder is to get a 300watt soldering gun and connect the cells with 10ga silicone wire. 
Note: I have tried the 260watt version and it does not work nearly as well as the 300watt version. 

https://www.amazon.com/dp/B000JEGEC0/ref=cm_sw_r_cp_api_BSErzb67B2ZD0
```

---
## \#7 Posted by: Smorto Posted at: 2017-06-18T18:54:23.296Z Reads: 66

```
Ive never used a soldering gun or even seen one in a action. Does it heat the cells up just as much as a soldering iron? What makes it better then an iron?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-06-18T20:44:30.826Z Reads: 61

```
It's better than an iron because it is only on and hot while you hold the trigger.  This prevents the tip from overheating and burning up. This also allows you to have a lot more wattage with a relatively small tip.
It's better to have a high wattage soldering tool because it will get the spot your soldering to hot enough and fast enough to avoid the heat spreading over a large area of the battery.

The faster you can make the joint, the less you heat up the whole battery.
This is why welding cells together is the best solution, it's the fastest and consequently it heats the battery up the least.
```

---
## \#9 Posted by: Sleepingalex24 Posted at: 2017-06-18T22:00:38.517Z Reads: 55

```
I wanted to try the 18650s because I didn't have a very good experience with the lipo cells and a fake B6AC Balance Charger. Not only did the charger unbalance the cells but it didn't even charge them up all the way. Granted it was a fake charger but I just don't know how much better a real charger would work. Also I want to make an easy way to charge my batteries without taking the board apart. So @Namasaki would you recommend I just do a lipo setup with a BMS? As it would be cheaper and also easier to assemble than the 18650s.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-06-18T22:27:10.993Z Reads: 58

```
I'm using a Lipo with bms setup on both of my builds and couldn't be happier.
Lots of power for fast acceleration and charging up hills.
Enough range for my purposes, 12-14 miles
A good balance charger or a good bms is very important.
I have had some swelling issues using cheaper low C rated Lipos but I have had no issues at all with the Turnigy 60c Lipos that I am currently using. 
You can check out my build thread here:
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#11 Posted by: Sleepingalex24 Posted at: 2017-06-18T23:12:27.836Z Reads: 54

```
I found this good deal on the same type of batteries [Turnigy Hard Case 4s 40C](https://hobbyking.com/en_us/turnigy-7200mah-4s-14-8v-40c-hardcase-pack.html) and I would hook them up in series. I saw this [post](https://www.electric-skateboard.builders/t/lipos-c-ratings-vs-mah-battery-choice/19908/2?u=sleepingalex24) where you said that the current the batteries should be able to output is 300A. I calculated it for these and it is 288A continuous. Would I be able to use this [BMS](http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html) even though it only has a 60A discharge rate? Also, would this C rating be high enough?
```

---
## \#12 Posted by: Smorto Posted at: 2017-06-19T00:06:46.979Z Reads: 53

```
Awesome, I was going to go with the the arduino spot welder for my pack but I might consider this...
```

---
## \#13 Posted by: Namasaki Posted at: 2017-06-19T02:19:19.122Z Reads: 48

```
Let me start here by saying that this has been a learning process. Therefore I am no longer boasting 300a continuous from my battery build because after more consideration, it really doesn't seem realistic.
For one thing the main supply wires from the batteries are only 12ga and rated for 75a.
So how could a battery handle 300a with 75a wires?
So now I'm saying don't think of the C rating as an actual measure of current capability but rather a relative value for comparing Lipos.
So a higher C Lipo will be better than a lower C Lipo in terms of less voltage sag and less heat.
Better to get the highest C rated Lipo you can.

And the battery does not determine the current flow through the system, neither does the bms.
it is determined by the Vesc and is adjustable in current control mode. So a 60a bms is fine.
```

---
## \#14 Posted by: Sleepingalex24 Posted at: 2017-06-19T11:39:03.909Z Reads: 37

```
Ok great. Thanks so much. I will get these batteries. :+1:
```

---
## \#15 Posted by: Sleepingalex24 Posted at: 2017-06-19T14:11:42.705Z Reads: 30

```
Just so you know @Smorto, if you were planning on buying those batteries I linked they are only sold in the UK.
```

---
## \#16 Posted by: Smorto Posted at: 2017-06-19T14:21:59.651Z Reads: 29

```
I was talking about the soldering gun but thanks for the info :wink:.
```

---
## \#17 Posted by: SpeedSloth Posted at: 2017-06-19T15:06:18.657Z Reads: 25

```
That's really interesting, thanks for sharing I'll look into getting one of these :smiley:
```

---
