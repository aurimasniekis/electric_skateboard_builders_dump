# BMS for dual motor

### Replies: 12 Views: 902

## \#1 Posted by: moe_lester Posted at: 2017-04-02T14:09:03.177Z Reads: 95

```
Hey guys I just finished my first build, its fucking incredible never had an electric longboard let alone one I've built. It broke just known but its an easy fix the motor mount broke. 

I have a question about BMS. So the setup I had for my first build is a 60amp max motor and vesc 4.12, and the bms I attached to my 8s4p (Li-ion) is a 60A BMS. 

So my question is If I wanted to make this a dual setup with another motor would I have to find a 120A BMS because I will have two motors + another vesc aswell?? 

What would happen If I kept the 60A bms on my battery with dual motors?? 

Would it burn/damage the bms?? 

If you have any questions please feel free to ask
```

---
## \#2 Posted by: JLabs Posted at: 2017-04-02T14:10:55.708Z Reads: 96

```
Nope! You can still use the same BMS, but just limit each VESC to 30a which should be plenty for most applications. If you go with 120a each VESC would be at 60a
```

---
## \#3 Posted by: moe_lester Posted at: 2017-04-02T14:15:09.539Z Reads: 92

```
Ok but wouldn't that mean the motors will be a lot slower and producing less torque??

Or is that not how it works, sorry Im still relatively new to this??
```

---
## \#4 Posted by: Stefan Posted at: 2017-04-02T14:32:40.322Z Reads: 85

```
Keep in mind that motor amps is not the same as battery amps. As long as you just stay with 60amps pulling from your battery ( -> 30a battery max for each vesc) you should have no problem with your bms.
Regarding the torque, you should have more torque since you are using two motors instead of one while pulling the same power from your battery (battery amps * battery voltage).
```

---
## \#5 Posted by: moe_lester Posted at: 2017-04-02T14:45:47.745Z Reads: 79

```
So on the BLDC tool I just got on to motor - current limits but do I put 30amps for the battery max or the motor max??

thanks
```

---
## \#6 Posted by: Stefan Posted at: 2017-04-02T14:48:47.270Z Reads: 71

```
30 amps battery max, for both vescs.
```

---
## \#7 Posted by: moe_lester Posted at: 2017-04-02T14:53:52.015Z Reads: 68

```
Ok great thanks stefan, later on down the line I will make another build that can tackle hills, If i wanted more torque for these hills would you recommend using a bms that could handle 120amps so I can do max currents for both motors??
```

---
## \#8 Posted by: mmaner Posted at: 2017-04-02T14:58:32.856Z Reads: 65

```
What kind of hill are you riding, Everest?  I have what is arguable a not very good 10s3p on dual 190kv motors and can climb 25deg hills without loosing much speed, 15deg hills while accelerating.  I think you might focusing a bit too much in power deliver and not enough in motors and gearing.
```

---
## \#9 Posted by: moe_lester Posted at: 2017-04-02T15:41:39.572Z Reads: 62

```
Everest lool, I get what your saying. Im running 190kv 50mm motors so there quite small. 

At the moment my gearing is 16t motor pulley - 36t wheel pulley. You think I should try 15t motor pulley?
```

---
## \#10 Posted by: Hummie Posted at: 2017-04-02T16:00:03.427Z Reads: 54

```
U may have the vescs to pull 60 amps from the battery, as determined by the "battery amps", but if u put a watt meter inline you'll see that unless you're running at full speed you're not going to be able to get to that 60 amps. If u want more power at lower speeds u need to up the motor amp limit. Much more torque is possible and u could actually get (maybe depending on other things) the 60 amps u want but it won't happen unless the motor amp limit is much higher. 200 is the limit and supposedly 150 is the max that the sensors can read so maybe try 150 motor amp on each vesc and you'll blast off like you'd want
```

---
## \#11 Posted by: Namasaki Posted at: 2017-04-02T16:19:57.206Z Reads: 49

```
I would like to confirm what Hummie is saying.
I have put a watt meter in line and even with 6s voltage and dual motors going uphill, my peak amp draw from the battery was only about 36a total.
I have also tried increasing motor max current and even just raising mine from 60 to 80 per motor gave a noticeable increase in power especially at lower speeds.
```

---
## \#12 Posted by: mmaner Posted at: 2017-04-02T16:21:38.016Z Reads: 47

```
It would help.  I usually run 15 38, but I'm a little weird about my gearing.
```

---
