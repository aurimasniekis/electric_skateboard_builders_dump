# Battery wont charge and weird noise coming from BMS

### Replies: 26 Views: 956

## \#1 Posted by: cryo Posted at: 2017-10-19T13:49:34.221Z Reads: 89

```
I've been riding my board for about 2 weeks. Yesterday I left my board on for a couple days by accident and now my board wont charge, plugging in the charger the light indicator on the charger doesnt even light up. I have 2 lipos through a supower bms and whenever i plug in my loop key I get a weird, very soft, siren/alarm like sound coming from the BMS. 

Any ideas whats going on?
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-10-19T13:53:27.828Z Reads: 88

```
you drained your cells to low...

check the voltage of the pack and report back
```

---
## \#3 Posted by: chaka Posted at: 2017-10-19T13:57:13.773Z Reads: 85

```
Voltage is probably too low to initiate charging. you will need to "jump the pack" by charging with low current at the battery terminals. Once you bring the voltage of the cells above 2.8v the bms should allow charging again. You will need a controllable power source to do this since you don't want to dump to much current into the pack when the cells are too low.

Of course, check voltages with a multimeter to be sure this is the problem.
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-10-19T14:00:53.965Z Reads: 83

```
... and try not to have to do that too often, cells don't like that too much, it seems to shorten the lifespan a bit. Obviously shit happens.. but you know.
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-10-19T14:02:12.918Z Reads: 78

```
maybe he could do some sort of regen braking charging...

get pulled by a car with light brakes on for a bit to revive the cells...  only if you have vesc though
```

---
## \#6 Posted by: chaka Posted at: 2017-10-19T14:02:23.106Z Reads: 75

```
Not very good for the BMS either. That whine is the BMS screaming for help. :joy:
```

---
## \#7 Posted by: chaka Posted at: 2017-10-19T14:10:23.997Z Reads: 65

```
I just saw that you are running li-po..... It isn't to a great idea to run lipo with a bms. Most BMS units, if not all, have a low voltage cut-off far to low for prismatics. Chances are you have puffed your packs and they are now toast.
```

---
## \#8 Posted by: cryo Posted at: 2017-10-19T14:15:19.502Z Reads: 67

```
I just checked the voltages of my batteries the voltages of the first lipo every cell is at 3.4v which is my cutoff in vesc.
My second lipo which is plugged into 6-10 on the BMS is at 
2.3v
1.9v
2.9
1.4
3
For a grand total of 11.5v
It originally is a 5s zippy compact 5000mAh 18.5v pack

Do i just buy a new one? Is it safe to try and rescue this pack?
```

---
## \#9 Posted by: cryo Posted at: 2017-10-19T14:16:01.326Z Reads: 63

```
also the lipos arent puffed at all no changes in appearance
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-10-19T14:16:47.248Z Reads: 62

```
what in the hell.

your cells are down to 1.4v?  your bms shouldn’t have let them drop below 3.2.  those are dead batteries.
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-10-19T14:17:20.225Z Reads: 59

```
not to mention crazily unbalanced
```

---
## \#12 Posted by: longhairedboy Posted at: 2017-10-19T14:18:06.896Z Reads: 58

```
hahahaha that's how jake puffed his evolve-leftovers pack he made.
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-10-19T14:18:57.748Z Reads: 58

```
unless you want to tap into and charge each cell individually i would toss that shit into a bag and call waste management.
```

---
## \#14 Posted by: cryo Posted at: 2017-10-19T14:19:53.108Z Reads: 57

```
I left my loop key in so my board was just on for like 4 days. Nothing the BMS could do at that point.
```

---
## \#15 Posted by: cryo Posted at: 2017-10-19T14:21:21.177Z Reads: 57

```
damn :frowning: 

Is there something wrong with my build? Seems kinda shitty that I destroy my batteries just by leaving my board turned on.
```

---
## \#16 Posted by: chaka Posted at: 2017-10-19T14:21:21.605Z Reads: 58

```
You have a balance board not a BMS. At least that is what it seems by your description.
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-10-19T14:21:51.110Z Reads: 57

```
true.

time to call waste management.  for the love of god, DO NOT throw those in the trash lol
```

---
## \#18 Posted by: cryo Posted at: 2017-10-19T14:22:36.491Z Reads: 57

```
I have this exact model

http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html
```

---
## \#19 Posted by: chaka Posted at: 2017-10-19T14:24:58.030Z Reads: 58

```
Did you bypass the bms for discharging? Even if you didnt, lipos can self discharge when they get too low, that's why you see most of us use cylindrical li-ion. They are more stable at low voltages.
```

---
## \#20 Posted by: cryo Posted at: 2017-10-19T14:27:18.145Z Reads: 55

```
No everything is going through the bms, both charge and discharge
```

---
## \#21 Posted by: chaka Posted at: 2017-10-19T14:35:39.931Z Reads: 49

```
What happened here is you let the cells go too low and they self discharged. Normally when we hit a low voltage cut-off it is under significant load and the cells bounce back to 3.6 volts when the load is cut. In this case the cells slowly discharged, effectively dropping the resting voltage to a level were they would start self discharging.

 I am still just speculating but you can be sure those cells will never be the same. Their internal resistance is probably much higher now.
```

---
## \#22 Posted by: cryo Posted at: 2017-10-19T14:44:46.110Z Reads: 45

```
all 5 cells of my other lipo pack are at 3.4v though. Why didn't that one get crazy unbalanced and low as well?

Also thinking back on it now shouldn't my BMS have somehow turned my board off by closing a circuit or something even if I'm using a loop key?

Theres no way everybodys boards are killing batteries just by leaving them on are they?
```

---
## \#23 Posted by: chaka Posted at: 2017-10-19T14:48:04.120Z Reads: 45

```
You probably damaged the cells prior to this happening, your pack is really small so it was under heavy use.
```

---
## \#24 Posted by: rich Posted at: 2017-10-19T20:15:34.522Z Reads: 37

```
[quote="chaka, post:21, topic:35961"]
dropping the resting voltage to a level were they would start self discharging
[/quote]

That's interesting, at which voltage this starts to happen?

I left my mtb switched on for about 28 hours and my 10s 10Ah Turnigy Graphene dropped from 35V to 8.87V total voltage and is puffed and dead now. So pffffff @cryo 1.4V is not bad but I win with 0.89V per cell :joy: 
But joking aside I'm planning to use a bms on my new battery, too to save it. But that your cell dropped to 1.4V with bms is strange.
```

---
## \#25 Posted by: cryo Posted at: 2017-10-19T20:51:05.124Z Reads: 31

```
Yea I thought thats what BMS were used for, I think it should have closed off the circuit when it detected cells below 2.9v like it says in the spec sheet but I guess not apparently. Either that or I have a faulty BMS for discharge because I think its highly unlikely Lipos self discharge that much over a couple of days, I remember reading somewhere that they only discharge ~5% a month with no load.
```

---
## \#26 Posted by: cryo Posted at: 2017-10-23T04:10:33.719Z Reads: 21

```
Managed to bring my lipos up back to an acceptable voltage to be charged normally again. Used a benchtop regulated power supply to charge each cell to 3.4v and from there I was able to use my regular charger. No puffed cells or overheating so far, runs just like it did before though I don't doubt its lifespan was shortened by my fuckup. 

Thanks for the insight guys :slight_smile:
```

---
