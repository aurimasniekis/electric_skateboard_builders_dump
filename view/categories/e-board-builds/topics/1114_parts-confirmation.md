# Parts confirmation

### Replies: 16 Views: 2204

## \#1 Posted by: ikjahaa Posted at: 2016-01-27T13:03:04.304Z Reads: 86

```
Hello I am still pretty new to the E-board world, so I would like to get a comfirmation regarding my parts list.

MOTOR
----
http://www.hobbyking.com/hobbyking/store/__18128__Turnigy_Aerodrive_SK3_6364_245kv_Brushless_Outrunner_Motor.html
or
http://www.hobbyking.com/hobbyking/store/__14408__Turnigy_G160_Brushless_Outrunner_245kv_160_Glow_.html

my preference was going to the first one cause it has a bigger diameter.

ESC
------
product/single-motor-120a-6s-esc/

This one only supports 6S, i would have prefered at least a 9S one.

BATTERY
-----
http://www.hobbyking.com/hobbyking/store/__8587__ZIPPY_Flightmax_5000mAh_3S1P_30C.html
or
http://www.hobbyking.com/hobbyking/store/__8579__ZIPPY_Flightmax_5000mAh_3S1P_20C.html
I'll be using 2 of these. (set them in serie)
30C vs 20C not sure what kind of impact that will have ?


NOTE
---
I would like to set my motor and esc at the front of my board and the batteries at the back, so i'll be using a wire to extend the current battery wires, would a 10 AWG suffice or should i go 11/12 AWG ?
```

---
## \#2 Posted by: laurnts Posted at: 2016-01-27T13:55:33.194Z Reads: 82

```
[quote="ikjahaa, post:1, topic:1114"]
http://www.hobbyking.com/hobbyking/store/__14408__Turnigy_G160_Brushless_Outrunner_245kv_160_Glow_.html
[/quote]

I recommend to stick with the SK3 motor as most thread / build are using it (known also to have CAN bearings).

Currently I have no experience with that ESC, but strongly recommend to get VESC (one of the best if you know what you're doing).

Personally for normal commuting I found 6s already overwhelming (depending on your gearing and needs).

For battery, just a personal opinion, 20c is adequate, but I am using 25c at the moment. Going to 30c also fine,
the difference would not be significant. If you think of getting dual motor build, maybe 30c is a better option. But as I see people are using lower c rating with li ion batteries, it should be fine what ever battery you choose :)
```

---
## \#3 Posted by: ikjahaa Posted at: 2016-01-27T14:11:06.776Z Reads: 75

```
Thank you, The main reason I went with that esc was because it had a fan and was water resistant.
I don't know wether the vesc has any problems regarding these two things.

Do you know what AWG wire comes with that battery ?
```

---
## \#4 Posted by: laurnts Posted at: 2016-01-27T14:19:49.175Z Reads: 76

```
I have similar ESC in size and shape of the one you linked here.
To be honest, the low speed performance is not so good as well as making high pitch noise when braking.
I got mine from Hobbyking, not sure about this version though.

And I don't like the fan as well. It's noisy as well as drains battery.
The waterproof might be handy, but I prefer going with water insulated ESC with a water resistant enclosure.
Nevertheless you will most likely install an enclosure for your electronics because of debris, stones and water spill.
Trust me you don't want to ride 20km/h, slip and slam your lipo batteries to an obstacle :smiley:
```

---
## \#5 Posted by: delta_19 Posted at: 2016-01-27T14:21:43.868Z Reads: 70

```
10 awg on the battery but 12awg can carry that amount of current just fine. Vesc can be shorted easy so I would recommend going with the 12s 120A esc on diy's website
```

---
## \#6 Posted by: ikjahaa Posted at: 2016-01-27T14:24:33.921Z Reads: 71

```
[quote="laurnts, post:4, topic:1114, full:true"]
I have similar ESC in size and shape of the one you linked here.
To be honest, the low speed performance is not so good as well as making high pitch noise when braking.
I got mine from Hobbyking, not sure about this version though.

And I don't like the fan as well. It's noisy as well as drains battery.
The waterproof might be handy, but I prefer going with water insulated ESC with a water resistant enclosure.
Nevertheless you will most likely install an enclosure for your electronics because of debris, stones and water spill.
Trust me you don't want to ride 20km/h, slip and slam your lipo batteries to an obstacle :smiley:
[/quote]

Yes, I am planning to 3D-print an enclosure.


[quote="delta_19, post:5, topic:1114, full:true"]
10 awg on the battery but 12awg can carry that amount of current just fine. Vesc can be shorted easy so I would recommend going with the 12s 120A esc on diy's website
[/quote]

But that one doesn't come with an internal BEC :/
I see that there is comming a newer version of the vesc in feb. perhaps that one has this issue fixxed ?
```

---
## \#7 Posted by: delta_19 Posted at: 2016-01-27T14:29:28.210Z Reads: 69

```
Bec only cost 10-15 on hobbyking
```

---
## \#8 Posted by: trbt555 Posted at: 2016-01-27T14:35:52.313Z Reads: 70

```
10AWG should be fine.
So will 20C rating.

Bear in mind that if you want to balance-charge those lipo's in series, you'll need to be VERY careful how you wire and connect the balancing leads. I've had smoke & sparks before. Refer to my [schematic][1] here.

Also, if you run with those ZIppy lipo's, remember to get the right connectors to put them in series and connect to the ESC

You might also want to consider putting in a [loop key][2] which allows you to arm/disarm the power circuit easily.

If you're not afraid of some configuration, get a VESC. It really is superior to any ESC out there.
If you're in the US, [Ollin Board Co][3] can help you out.
It will come shrink-wrapped so you don't need to worry about possibly shorting it.


  [1]: http://www.electric-skateboard.builders/t/charging-2-x-3s-lipos-in-series-please-look-over-my-schematic/734/9?u=trbt555
  [2]: http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
  [3]: http://www.ollinboardcompany.com/product/vedder-s-speed-controller
```

---
## \#9 Posted by: ikjahaa Posted at: 2016-01-30T19:14:25.208Z Reads: 58

```
If i was to use the current VESC, would my build be future-proof? I mean if i want to add a second motor later on, would i be able to do this by only having to purchase the extra motor ?
```

---
## \#10 Posted by: psychotiller Posted at: 2016-01-30T19:29:58.523Z Reads: 54

```
You will always need 1 esc per motor. 
2 motors = 2 escs
```

---
## \#11 Posted by: ikjahaa Posted at: 2016-02-05T12:35:29.544Z Reads: 43

```
Does the VESC have any battery voltage safety ?
does it cut the power if any of the battery cells drop below a certain value ?

if not, could i possibly use http://www.hobbyking.com/hobbyking/store/__29652__HobbyKing_8482_Lipoly_Low_Voltage_Alarm_2s_6s_.html
permenatly? even when I want to plug my battery into the charger ? (so in parralel to the charger)
```

---
## \#12 Posted by: trbt555 Posted at: 2016-02-05T13:08:58.443Z Reads: 40

```
Yes, you can set the battery voltage cutoff limits in the VESC, using the [BLDC tool][1].
  [1]: http://vesc.net.au/
```

---
## \#13 Posted by: ikjahaa Posted at: 2016-02-06T17:47:35.648Z Reads: 39

```
Do I then need to connect the battery ballance wires to the vesc? or just the thick black and red power wires ?

Also, my batteries are 5000mah, since i'm using 2 in series will I therefor need a 10A charger if i want to charge at 1C ?

ps. I was thinking of using 2x 4S batteries instead of the listed 3s. This so I'll have longer drive times. (or doesn't the cell count have any effect on this?)



http://www.hobbyking.com/hobbyking/store/__9179__Turnigy_5000mAh_4S_25C_Lipo_Pack.html
```

---
## \#14 Posted by: trbt555 Posted at: 2016-02-06T19:13:00.024Z Reads: 39

```
You don't connect the balance leads to the VESC, just the power leads.
A general rule of thumb is 1km for 10Wh.
Multiply the voltage of your batteries with the capacity in Ah to get Wh.
2 3S 5000mAh batteries = 2 x 11.1V x 5 Ah = 111Wh => approx 10km
2 4S 5000mAh batteries = 2 x 14.8V x 5 Ah = 148Wh => approx 14km

You do not need to charge at 1c.
You can charge the lipos separately, you can charge in series, you can charge in parallel.

When you charge in series, your charger needs to be able to charge that many cells at once.
```

---
## \#15 Posted by: ikjahaa Posted at: 2016-02-06T19:25:02.807Z Reads: 36

```
But how does the vesc know when a cell has dropped bellow 3.6/3.7V ?
```

---
## \#16 Posted by: trbt555 Posted at: 2016-02-06T20:55:37.709Z Reads: 36

```
It doesn't.
You just set the cutoff at a safe level. If you keep your cells balanced, no need to measure them indivudually.
```

---
