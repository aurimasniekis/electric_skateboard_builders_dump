# Hypothetical question about motor, wattts, and voltage

### Replies: 21 Views: 1331

## \#1 Posted by: Jinra Posted at: 2016-05-15T04:07:00.024Z Reads: 142

```
So if i'm trying to calculate peak current draw for my board with dual 1800w motors running in a 6s (22v) configuration. Would it be save to say that my peak amp draw is 1800/22=82amps x 2 motors = 164 amps?

This calculation seems sort of high, so I feel like I'm doing something wrong.
```

---
## \#2 Posted by: Namasaki Posted at: 2016-05-15T04:18:38.694Z Reads: 140

```
ohms law is P=ie or power(watts)= i(current) X e(voltage)
So yes 1800/22v = 82 amps per motor however, if your using lipos, you'll have 25.1 volts at full charge and its a good practice to stop and recharge your packs when they get down to nominal or 22v because some packs like zippys go real fast after you cross the nominal threshold. I ruined 2 almost brand new 6s packs that way.
So, 1800/25v =72 amps per motor. This is the problem with running 6s, high amp draw.
But thats if your actually producing 1800 watts per motor.
The best way to find out your real amp draw is with an inline watt meter that saves peak amp reading while your riding because the load of your weight and wind resistance and any additional load like climbing hills will substantially affect amp draw.
http://www.all-battery.com/TenergyWattMeterandPowerAnalyzer.aspx?utm_source=GoogleShopping&utm_medium=GDF&gdftrk=gdfV26767_a_7c354_a_7c922_a_7c01446&gclid=CLK80uef28wCFUdrfgodZ_4BVw
```

---
## \#3 Posted by: Hummie Posted at: 2016-05-15T04:28:23.903Z Reads: 129

```
The motor's max wattage is probably assuming more voltage than you're using.
```

---
## \#4 Posted by: Jinra Posted at: 2016-05-15T04:30:36.712Z Reads: 124

```
I'm not sure I understand what you're saying. Or rather, I'm not sure why the motor power has anything to do with assumed voltage of the setup.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-05-15T04:36:46.484Z Reads: 117

```
In a real life comparison your motors will produce tons more power on 50v than they will at 25v.
And I think what hummie means is that the motors power rating is based on its maximum voltage rating.
```

---
## \#6 Posted by: seanpain4 Posted at: 2016-05-15T04:39:06.219Z Reads: 113

```
Your calculation is correct. What they are saying is that, if you run your motor at a lower rated voltage then it might not draw all the power the motor would at the higher voltage.

Example:

A motor is rated at 6-10S and at 1500W.

At 10S it is able to pull a max of around 1500W. But when at a lower voltage it isn't able to get enough power so it peaks at around 1200W of power.
```

---
## \#7 Posted by: Jinra Posted at: 2016-05-15T04:39:26.171Z Reads: 107

```
yea maybe I'll try changing up from 6s4p to 12s2p, just have to check with the mfg if the esc can handle a 12s setup. Thanks for your input!
```

---
## \#8 Posted by: Namasaki Posted at: 2016-05-15T04:42:10.542Z Reads: 108

```
There are a couple of very good 12s capable Esc's available by several suppliers who frequent this forum.
The Vesc is a favorite and also the torquesboard is a good simple version.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-05-15T04:43:37.746Z Reads: 99

```
10 or 12s is the way to go if your looking for maximum power and speed.
```

---
## \#10 Posted by: Jinra Posted at: 2016-05-15T04:43:39.649Z Reads: 97

```
I'm basically trying to fix up my benchwheel bored because I think it's a great learning experience, but it'd be hard to fit a new BMS + 2 VESCs in there, so I may be limited with using the MFG's ESC/BMS which are integrated into sandwich style circuit boards.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-05-15T04:45:01.200Z Reads: 93

```
Are you having problems with the protection circuit on that board cutting out repeatedly?
Iv'e heard that its a common issue with the electronics on that board.
```

---
## \#12 Posted by: Jinra Posted at: 2016-05-15T04:51:21.432Z Reads: 93

```
Yea, I have another thread I've been updating with my findings, but no luck so far resolving it. The engineer at Benchwheel said the battery needs replacement (and maybe  the esc/bms) so the first step I wanted to take was to make a new battery myself for it. Just have to decide which configuration to go with..
```

---
## \#13 Posted by: Namasaki Posted at: 2016-05-15T04:56:55.350Z Reads: 88

```
I doubt the problem is the battery, I'll bet its a design flaw in the Esc/bms.
I think theres lots of peps having same problem.
```

---
## \#14 Posted by: Jinra Posted at: 2016-05-15T05:01:10.031Z Reads: 83

```
Yea, the only reason I could imagine why it might be the battery is if the discharge rate isn't high enough to supply the ESC. In my email with their engineer he said that the software on the ESC needs to be updated, not necessarily replace. However, I have no way to update the software.
```

---
## \#15 Posted by: Namasaki Posted at: 2016-05-15T05:01:43.021Z Reads: 83

```
I have a couple Venom 6s 2500mah packs that I could donate to your project if your in the USA
<img src="/uploads/db1493/original/2X/8/8733c002c449d3f1a8787be38a8686627469384f.jpeg" width="375" height="500">
```

---
## \#16 Posted by: Hummie Posted at: 2016-05-15T05:03:06.058Z Reads: 74

```
Maybe their esc and bms are limiting the amps very low for what u want.  If you're on a budget I'd get vesc first and then ur enabled to have high voltsge then go cheap with everything else. Single motor is enough or maybe use the bench wheel motor and everything else. smooth silent Foc program.
```

---
## \#17 Posted by: Namasaki Posted at: 2016-05-15T05:05:36.697Z Reads: 72

```
I think the guys at Benchwheel miss designed there esc/bms so that is can't handle the motors.
This is a common issue with there dual motor boards.
```

---
## \#18 Posted by: Jinra Posted at: 2016-05-15T05:05:48.496Z Reads: 76

```
Thanks for the offer! I am in the US, but I'm not 100% sure I'm keeping the board yet. I'll let you know if I do.
```

---
## \#19 Posted by: Namasaki Posted at: 2016-05-15T05:07:52.140Z Reads: 77

```
Sure, just pm me if you want them. You can have them, just pay for the shipping.
There good batteries, I just don't need them anymore.
```

---
## \#20 Posted by: Boostedkiller Posted at: 2017-07-29T13:59:31.525Z Reads: 24

```
Hey do you still have those batteries ? I know a friend who forgot to switch off his board while he was on vacation so his batteries drained!
```

---
## \#21 Posted by: Namasaki Posted at: 2017-07-29T14:47:32.825Z Reads: 23

```
Unfortunately no. 
We suffered a burglary earlier this year and the thieves stole my safe. The batteries where inside the safe.
```

---
