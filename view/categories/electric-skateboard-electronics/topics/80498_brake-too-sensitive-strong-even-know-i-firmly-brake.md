# Brake too sensitive/strong even know I firmly brake

### Replies: 12 Views: 500

## \#1 Posted by: huzaini Posted at: 2019-01-10T18:28:17.784Z Reads: 98

```
Hi guys I have problem with my 1st build trampa holipro with flipsky dual fsesc 6.6 and flipsky 6370 190kv. 12s4p Samsung. Where the setting on vesc tool to adjust brake smoothness. Right now it's too sudden and hard. Not smooth as my koowheel.
```

---
## \#2 Posted by: Balta_6 Posted at: 2019-01-10T18:36:42.631Z Reads: 96

```
Motor regen that is : it's a negative value, try to put it up a little bit (from -12 to -10 for example, yours could be way off ;-) )
```

---
## \#3 Posted by: tardyparty7 Posted at: 2019-01-10T18:44:08.335Z Reads: 93

```
yeah, if you have a high negative value it can send you flying.
```

---
## \#4 Posted by: huzaini Posted at: 2019-01-10T18:55:57.180Z Reads: 87

```
Is this setting what you mean? ![Screenshot_20190111-025419|281x500](upload://szwcHa8Tax4JSfOmKdaBplkAGXG.png)
```

---
## \#5 Posted by: huzaini Posted at: 2019-01-10T19:03:45.717Z Reads: 80

```
Or is it this one? ![Screenshot_20190111-030237|281x500](upload://e4ebN8HIIJnmP6HYZC8CZgqOfb3.png)
```

---
## \#6 Posted by: Saturn_Corp Posted at: 2019-01-10T19:07:24.073Z Reads: 79

```
Do you mean motor amps and not regen? The value you're talking about has to do with battery regen when braking and not the motor amps when braking I believe. I could just be misunderstanding you though lol.

@huzaini how many amps do you have set for the motors? Should be a positive number for acceleration and a negative number for deceleration.

EDIT: that second photo. Try turning down the negative amps a bit and see from there.
```

---
## \#7 Posted by: MatrixWriter Posted at: 2019-01-10T19:09:49.670Z Reads: 76

```
For motor currents I use:
60A and -30A (braking).

If you want stronger brakes, lower the brake value to -35A.

For battery set the current to what the pack or BMS is capable of delivering. So if 60A, then put 60A.
For current max regen, I would start out with -10A and work your way up to a lesser value. It is somewhat depend of your BMS charge rate. -40A is too much by default.

After these are configured, adjust your throttle curves.

Sample setting of what I use on one of my boards:
![2018-12-28%2021_56_11-Greenshot|690x388](upload://7TGfvJ3YiHgjU8mDJVTKsu9baz0.png)
```

---
## \#8 Posted by: Andy87 Posted at: 2019-01-10T19:11:01.243Z Reads: 72

```
Your battery current with -40 is way off.
Set it to -12 or -15a that should already help a lot.
Motor min i world set to -50a and you should have way much more gentle breaks
```

---
## \#9 Posted by: Narnash Posted at: 2019-01-10T19:18:14.770Z Reads: 72

```
You can also play a bit with the brake "Throttle Curve" in the VESC Tool to make sensitive low braking easier.
https://imgur.com/a/S7t1KtL
```

---
## \#10 Posted by: trampa Posted at: 2019-01-10T19:35:12.019Z Reads: 71

```
**Motor max Regen** is dominant at low speed, **Battery max Regen** is the dominant value at  high speed. 
At full speed, -10A will hardly slow you down. 
For linear braking, symmetric settings are best. E.g. -30A motor, -30A batt. Battery charge currents drop very fast with decreasing speed, so in real life your Battery will never see 30A charge currents for more than some seconds. 

No need for throttle curves. If batt regent is set to low, throttle curves will not improve the high speed braking behaviour! 

If you want softer brakes, you should use a higher **negative ramping** value. 0.5 to 0.8s would do the trick.
```

---
## \#11 Posted by: huzaini Posted at: 2019-01-10T20:04:07.796Z Reads: 59

```
i cannot find these setting, can you specified more for **negative ramping** . 
and 1 more thing, i decrease the motor regen and battery regen now its softer , but at near end of brake i got strong stop.
```

---
## \#12 Posted by: trampa Posted at: 2019-01-10T20:07:21.669Z Reads: 61

```
App settings >> PPM >>Pos and Neg ramping time. 
Defines how much time the VESCs spends to ramp from input level A to input level B.
This is the best way to get a smoother response to the finger trigger.
```

---
