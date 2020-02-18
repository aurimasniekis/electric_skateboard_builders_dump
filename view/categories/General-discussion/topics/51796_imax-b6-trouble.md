# Imax B6 trouble

### Replies: 68 Views: 1443

## \#1 Posted by: Orin635 Posted at: 2018-04-10T10:52:28.557Z Reads: 112

```
Hi guys.

Just got my imax b6 today and I'm having a bit of trouble with it

First of all it's the imax b6 (copy) from hobbyking and I have a 15v 5a AC charging brick.

When I charge my LiPos (6s 5200mah)  I set it to 5a but when it's charging it only charges at 2.1a is this normal? Can I charge it faster.

Second is a hardware issue and I'm wondering if anyone else has had this problem. The port where I plug In the charger does not work correctly I have to put it at a angle and a heavy object on top. I think there's a issue with the outside connection.![15233574826921869310806|666x500](upload://h4LUmyseG6vWl2vOpwvh8Ewnalu.jpg)
```

---
## \#2 Posted by: Tuomalar Posted at: 2018-04-10T11:06:49.566Z Reads: 106

```
IMAX lowers charging curret when cell voltage approach 4.2 due to balancing.
```

---
## \#3 Posted by: Jumpman Posted at: 2018-04-10T11:09:41.305Z Reads: 105

```
It’s a 50 watt charger.  So, its normal it can only charge to about 2A on 6s.  You can calculate max charging amps using watts divided by voltage, so 50 watts divided by 25.2 volts(6s).  

Sounds like you might have a broken solder joint on the power port, used to happen on laptops in the past when the cable was snagged.  You need to return the charger, or fix it.
```

---
## \#4 Posted by: Yecrtz Posted at: 2018-04-10T11:11:19.195Z Reads: 101

```
Your power cable could be broken just before the plug that goes into the balance charger. Try another one too see if the problem is the cable, or the b6.
```

---
## \#5 Posted by: BoostedBuilder Posted at: 2018-04-10T11:19:44.330Z Reads: 88

```
This is probably a stupid question - I just woke up. 

How do you want to charge a 25.2V battery at 5A with a 15V and 5A brick?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-04-10T11:28:39.495Z Reads: 84

```
Imax has a boost converter
```

---
## \#7 Posted by: Orin635 Posted at: 2018-04-10T11:31:23.591Z Reads: 82

```
No that makes a lot of sense😂
```

---
## \#8 Posted by: Orin635 Posted at: 2018-04-10T11:31:54.032Z Reads: 84

```
It's taking very long to charge
```

---
## \#9 Posted by: BoostedBuilder Posted at: 2018-04-10T11:40:23.371Z Reads: 81

```
To increase voltage, the boost converter has to decrease current to about 3A. No?
```

---
## \#10 Posted by: pat.speed Posted at: 2018-04-10T12:56:44.642Z Reads: 80

```
Well the Imax is a 50w charger so for it to get 50w it needs slightly more than 50w on the input. So at 15v you would need 3.3334 amps to get to that 50w input even though the charge will only output about 2 amps because of the higher voltage output.

Another example you feed 10v into a boost converter and you set it to out put 30v. Now you want your output to be 30v 2a so about 60W. 

Input Wattage = output wattage (not including losses)

60w / 10v = 60w / 30v

10v 6amps = 30v 2amps

I think that math is correct and remember to factor in that most boost converters are around 90-95% efficient, although that decreases as the voltage difference increases.

Someone correct me if I’m wrong plz
```

---
## \#11 Posted by: Orin635 Posted at: 2018-04-10T13:11:56.287Z Reads: 63

```
It charger the first LiPo fine charging the second now. takes 2.5 hours per :expressionless:
```

---
## \#12 Posted by: Blitz Posted at: 2018-04-10T15:18:34.587Z Reads: 54

```
Was your battery pack out of balance like 3.65V 3.65V 3.63V

The thing about some Cheap balance chargers Is instead of charging the " 3.63V" They would just charge the whole pack through the mains And then discharge the over charged ones and then charge them all up again,
and It would repeat it until all cells are 4.2 which takes a very long time.
```

---
## \#13 Posted by: Orin635 Posted at: 2018-04-10T19:09:10.011Z Reads: 49

```
Yes the last cell was out of balance
```

---
## \#14 Posted by: Blitz Posted at: 2018-04-10T19:21:31.468Z Reads: 48

```
A connector like that Can go into the balance port and directly charge the Low cell,    

![Untitled|690x452](upload://ngZ05rQtxQa92SWBdfhqoMR6TFV.jpg)
```

---
## \#15 Posted by: Orin635 Posted at: 2018-04-10T19:23:17.735Z Reads: 44

```
I dont understand. do you mean solder xt-60 connectors to the first and last balance leads
```

---
## \#16 Posted by: Blitz Posted at: 2018-04-10T19:24:03.735Z Reads: 44

```
xt-60 what you on about?!
```

---
## \#17 Posted by: Orin635 Posted at: 2018-04-10T19:24:23.336Z Reads: 42

```
idk :joy::joy:
```

---
## \#18 Posted by: Blitz Posted at: 2018-04-10T19:24:41.082Z Reads: 42

```
you see your balance port that white thing allows u to reach each cell individually.
right>?
```

---
## \#19 Posted by: Orin635 Posted at: 2018-04-10T19:25:06.976Z Reads: 41

```
ya?

10char
```

---
## \#20 Posted by: Blitz Posted at: 2018-04-10T19:25:37.598Z Reads: 43

```
Now what if you had this, 4.2V 4.2V 4.0V You would want to charge the 4.0V separately right?
Not charge the 4.2V 4.2V up and down until the 4.0V catches up.
```

---
## \#21 Posted by: Orin635 Posted at: 2018-04-10T19:25:59.629Z Reads: 43

```
yes i think haha
```

---
## \#22 Posted by: Blitz Posted at: 2018-04-10T19:27:32.169Z Reads: 42

```
![sds|690x420](upload://hUE65DBfpYoElURccyBcBLu8PvS.jpg)

Notice how that Fork Is inside the balance port. It is charging cell 1 by itself.
(at a low amperage the wires cant handle a lot.)
```

---
## \#23 Posted by: Orin635 Posted at: 2018-04-10T19:28:12.687Z Reads: 41

```
is that not good? what if they're not even
```

---
## \#24 Posted by: Blitz Posted at: 2018-04-10T19:29:30.210Z Reads: 38

```
Its safe because if you chose the wrong cell, the Imax b6 clone will read the voltage 4.2 wrong one switch 4.1 that's the one then Imax b6 charge that one alone.
```

---
## \#25 Posted by: Orin635 Posted at: 2018-04-10T19:31:31.325Z Reads: 39

```
Well if its takes to long and i get frustrated with the length I will do that thanks
```

---
## \#26 Posted by: taz Posted at: 2018-04-11T00:42:50.593Z Reads: 37

```
Actually even the very best of chargers work that way also.
I have a 1344W Powerlab 8 and a 350W icharger 208b that work that way.
The pl8 can charge through the balance leads but only for small packs. 
One of the differences between cheap small chargers and the big boys is in how much current they can discharge through  the balance leads.
```

---
## \#27 Posted by: MannyM0E Posted at: 2018-04-11T06:02:55.784Z Reads: 32

```
Will this method work if I have a 5s battery with 1 cell dead. Reason I know it's dead because my charger detects it as a 4s now and won't charge anymore. Trying to find a way to fix that one dead cell
```

---
## \#28 Posted by: taz Posted at: 2018-04-11T07:01:17.243Z Reads: 31

```
It might work. Set your charger to nimh or nicd and use a very low charging current until the dead cell goes over 3.3v. Then switch back to Lipo mode to continue charging. Do not exceed 1A charging through the balance wires otherwise you risk overheating and damaging them.
```

---
## \#29 Posted by: Orin635 Posted at: 2018-04-11T09:37:19.120Z Reads: 27

```
I used the imax b6 till they said it was fully charged then when I used my voltage tester there was a range of 4.17-4.21v
```

---
## \#30 Posted by: Blitz Posted at: 2018-04-11T09:41:21.781Z Reads: 24

```
Fake charger can have bad readings I think you can try calibrate it tho lemme check.
```

---
## \#31 Posted by: taz Posted at: 2018-04-11T09:41:23.972Z Reads: 24

```
Generally with a decent quality pack in good condition once the cells are balanced they should stay that way when discharging thus requiring minimal balancing when charging. If you have a pack though that is not so good (e.g. big variances in IR between cells ) then you will find out that it takes a lot more time to balance charge it.
```

---
## \#32 Posted by: Orin635 Posted at: 2018-04-11T09:42:27.561Z Reads: 22

```
My pack came and discharged with small difernces
```

---
## \#33 Posted by: Blitz Posted at: 2018-04-11T09:43:22.465Z Reads: 21

```
OK so Imaxb6 clone says its 4.2 but voltage checker says otherwise right?
```

---
## \#34 Posted by: Orin635 Posted at: 2018-04-11T09:43:46.897Z Reads: 19

```
yes
10char
```

---
## \#35 Posted by: taz Posted at: 2018-04-11T09:45:45.002Z Reads: 18

```
0.04V difference is not that much especially for a cheap charger.
```

---
## \#36 Posted by: Orin635 Posted at: 2018-04-11T09:46:38.182Z Reads: 21

```
Will it effect the life span and range i get?
```

---
## \#38 Posted by: Orin635 Posted at: 2018-04-11T09:47:35.360Z Reads: 20

```
I need to keep these LiPos for a year. next year I will be making a big Li-On pack
```

---
## \#39 Posted by: taz Posted at: 2018-04-11T09:49:15.249Z Reads: 21

```
No not really as long as it stays that way. If you want to increase the life of you packs avoid charging them above 4.1V and discharging them below 30% .
However may I suggest the purchase of a good powerful charger in the future as it is an equipment that will make your life easier, charge faster and last you for decades.
```

---
## \#40 Posted by: Orin635 Posted at: 2018-04-11T09:52:17.038Z Reads: 21

```
30% is what 3.6v?
```

---
## \#41 Posted by: Blitz Posted at: 2018-04-11T09:52:18.362Z Reads: 18

```
1+ I've read studies that said going from 4.2 to 4.1 can almost double your Lithium cell life 
(It was probably done with Li-ons but It still should help Lipos. 
But be careful with the cutoff voltage because cells can drift off quickly near the end.
```

---
## \#42 Posted by: Orin635 Posted at: 2018-04-11T09:53:33.594Z Reads: 14

```
its only a 10400mah pack how much range will I get? when i did a test run it seemed to run out very quickly
```

---
## \#43 Posted by: Orin635 Posted at: 2018-04-11T09:54:29.426Z Reads: 15

```
ive used calculators and they say 20km ish
```

---
## \#44 Posted by: Blitz Posted at: 2018-04-11T09:55:09.129Z Reads: 16

```
well, Do you drive efficiently? Give it and kick-start don't punch the gas too hard.
Or you have hills Hit the gas brake gas brake etc? 

drive easy and you can add like 20% range.
```

---
## \#45 Posted by: Orin635 Posted at: 2018-04-11T09:57:10.667Z Reads: 15

```
i do kick start. dont accelerate quickly. what you mean about the hills
```

---
## \#46 Posted by: taz Posted at: 2018-04-11T09:57:25.538Z Reads: 15

```
It depends on the battery. Personally I never go below 3.75V with my RC model batteries. Destroying 2 x 6S 5000mAh packs to fly my heli 30sec more is not worth it.
```

---
## \#47 Posted by: Orin635 Posted at: 2018-04-11T09:58:38.789Z Reads: 18

```
Thats very high is it not? I was thinking more 3.5v
```

---
## \#48 Posted by: Blitz Posted at: 2018-04-11T09:58:42.591Z Reads: 18

```
"Do you have hills near you?" climbing hills can take a lot of energy.
```

---
## \#49 Posted by: Orin635 Posted at: 2018-04-11T09:59:27.282Z Reads: 17

```
I have a lot of hills
```

---
## \#50 Posted by: Blitz Posted at: 2018-04-11T09:59:28.871Z Reads: 16

```
It sounds higher than it really is Lipos voltage Drips fast past like 3.7V. 
(I've been told)
 
Hills could make your range smaller Try driving up a hill with a bike and on flat.
you will know hills take more energy.
```

---
## \#51 Posted by: Orin635 Posted at: 2018-04-11T10:01:14.366Z Reads: 13

```
Yeah. it must use alot
```

---
## \#52 Posted by: taz Posted at: 2018-04-11T10:02:52.289Z Reads: 14

```
3.5V is definitely too low. Do a web search and you will find various tables with different correlation between %-V.
The only proper way to do it is to make these graphs for each pack you have individually. Some charges can do it for you (my Powerlab 8 has that function) but you can also do it yourself.
However this is too much work, just don't go below 3.75V if you want your packs to last.
```

---
## \#53 Posted by: Orin635 Posted at: 2018-04-11T11:11:29.725Z Reads: 15

```
I will set my alarm for 3.8v then
```

---
## \#54 Posted by: Blitz Posted at: 2018-04-11T11:19:46.257Z Reads: 15

```
Just don't go under 3.7 set alarm to 3.75.
Some people say 3.4 is fine so keeping that in mind. set alarm to 3.75
```

---
## \#55 Posted by: Orin635 Posted at: 2018-04-11T11:23:02.990Z Reads: 15

```
i only need the LiPo's to last a year
```

---
## \#56 Posted by: Blitz Posted at: 2018-04-11T11:24:13.233Z Reads: 16

```
do you have multi-star batteries.,?
```

---
## \#57 Posted by: Orin635 Posted at: 2018-04-11T11:26:39.787Z Reads: 16

```
ya

10character
```

---
## \#58 Posted by: Blitz Posted at: 2018-04-11T11:27:29.373Z Reads: 17

```
Well If you treat them wrong you'll have them for less than half a years.
They puff easier than others.

some people say lipos last fro 100-200 cycles others say 150-250 others say it lasted them 400+
I'd say the guys who claim 400+ go a little under 4.2 and stop at 3.75
```

---
## \#59 Posted by: Orin635 Posted at: 2018-04-11T11:29:48.106Z Reads: 17

```
That would not be very good
```

---
## \#60 Posted by: Blitz Posted at: 2018-04-11T11:31:19.576Z Reads: 17

```
Yeah,. so set alarm to 3.75V try to stay a bit under 4.2V (If possible.)
Don't charge a warm battery, never store a fully charged lipo for more than 2-3 days. storage Charge is 3.8v 
that's all I know to keep them safe.
```

---
## \#61 Posted by: Orin635 Posted at: 2018-04-11T11:31:49.045Z Reads: 18

```
I will try that.
```

---
## \#62 Posted by: Blitz Posted at: 2018-05-03T19:33:39.391Z Reads: 14

```
Hey guys, I will only charge at 3s voltage (12.6v)
can the Imax b6 boost the 4a to like 4.5a?

https://www.rcmoment.com/p-rm3767eu.html?currency=EUR&Warehouse=CN&aid=rmuscietjc&gclid=EAIaIQobChMIyIrTjaHq2gIVB7TtCh2gawKqEAQYAyABEgJ2gfD_BwE
```

---
## \#63 Posted by: Orin635 Posted at: 2018-05-03T21:33:59.126Z Reads: 11

```
what?
10char
```

---
## \#64 Posted by: Blitz Posted at: 2018-05-03T21:35:49.982Z Reads: 11

```
The psu Is 15v 4A

My 3s lipos at full charge are 12.6V
Can the Imax b6 convert the Extra voltage to higher amperage?

The Psu is 60W the Imax b6  max power output is 50W
```

---
## \#65 Posted by: Orin635 Posted at: 2018-05-03T21:36:28.697Z Reads: 11

```
no I dont think so unfortunately
```

---
## \#66 Posted by: Orin635 Posted at: 2018-05-03T21:37:02.112Z Reads: 12

```
but i could be complety wrong i have no experience
```

---
## \#67 Posted by: Orin635 Posted at: 2018-05-03T21:37:15.190Z Reads: 12

```
actually if its 60w then probably
```

---
## \#68 Posted by: Blitz Posted at: 2018-05-03T21:37:28.734Z Reads: 11

```
Yeah I'll look into it a bit more.
```

---
## \#69 Posted by: Orin635 Posted at: 2018-05-03T21:37:48.459Z Reads: 11

```
hows your build btw?
```

---
