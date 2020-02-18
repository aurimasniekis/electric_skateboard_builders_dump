# ABS overcurrent after VESC repair

### Replies: 6 Views: 630

## \#1 Posted by: vicciu Posted at: 2017-07-18T15:21:12.616Z Reads: 94

```
I bought 2 VESCs form diyelectricskateboard in march and about 4 weeks ago the DRV8302 on one of them decided to die. So i bought some replacement drv's and replaced the broken one. From that moment I couldn't really get the VESC to work again.

First the FOC mode wouldn't really work. Detection went fine, however after applying all the detected values, the motor would just vibrate without really moving(even with no load). One thing to note is that before all of this, the FOC detection would return 0.014 ohms and 7.41mH, however after the repair, the values were around 0.030 ohms and 10mH. Putting the old values in didn't work, the motor wouldn't spin.

So I switched to BLDC mode and it seemed to work fine except for the fact that when going uphill, the motor would sometimes cut out and recover only after a few seconds. Thinking that it's just a low absolute current setting I kept going, however just before arriving home, the VESC simply refused to work. It would stop as soon as power was applied. Now any attempt to accelerate throws the "abs overcurrent" error.

Now I don't really know what could be the reason for the overcurrent error(it shows 150A overcurrent with the smallest amount of throttle and at low RPM). Adding a bit of solder to the shunts also didn't change anything. Any ideas on what could possibly be wrong with my VESC?
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-18T16:11:08.839Z Reads: 87

```
Sounds like the DRV repair wasn't properly done, check all connections (including the one under the chip).
```

---
## \#3 Posted by: Martinsp Posted at: 2017-07-18T17:13:53.806Z Reads: 80

```
ABS overcurrent is very common if you dont have your shunts connected properly... might have happened while desoldering DRV. Happened to me a couple of times :)
```

---
## \#4 Posted by: vicciu Posted at: 2017-07-18T21:01:15.012Z Reads: 73

```
I'll check the connections on the DRV tomorrow, maybe indeed some pins didn't get soldered well.


I added some solder to the shunts to make sure that they have proper contact. Is there anything else that should be checked on the shunts?
```

---
## \#5 Posted by: Martinsp Posted at: 2017-07-18T21:09:49.831Z Reads: 70

```
Well yeah it might not be the shunts themselves but the pins on the DRV that the shunts connect to... Have a look at that, it is in the schematic. Shunts also connect to some 100R resistors and so on... its all there I would start there and see if it is all ok :)
```

---
## \#6 Posted by: vicciu Posted at: 2017-07-19T07:18:10.739Z Reads: 57

```
After some probing it seems that all the connections on the DRV are fine. I was wondering, what happens if I solder SH1_A to SH1_B and SH2_A to SH2_B? Then the current should always be 0 and at least the overcurrent protection won't be triggered. Would this affect the way the VESC works in duty cycle control mode?
```

---
