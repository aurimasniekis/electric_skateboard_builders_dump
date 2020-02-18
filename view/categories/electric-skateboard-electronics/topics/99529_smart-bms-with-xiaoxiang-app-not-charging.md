# Smart BMS with xiaoxiang app not charging

### Replies: 10 Views: 423

## \#1 Posted by: Flouw Posted at: 2019-08-01T12:18:40.842Z Reads: 83

```
Hello guys, 
Due to a video on youtube i got my hands on an 10S 60A Li ion Smart BMS from Bmsbattery.com. Here is the link https://bmsbattery.com/bmspcm/833-16914-smart-bms-10s13s-60a-with-blue-tooth-android-or-ios-app.html#/17-battery_type-lithium_ion/107-cells_in_series-10 . In the beginning everthing seemed so work great. I connected the wires as shown in the diagram on the website und pluged in a 600W CC CV Buck converter with the voltage set to 42 V. The charging began and no problems occured only when i set the current to 2,3 amps the converter startet to smoke a tiny bit. After the charging was done i made a little tour with my board and after that i tried to charge the board again but with no success. I honestly have no idea what could be the problem. Has someone an idea ? :frowning: I am afraid the bms is broken but it still balance discharges and shows no error in the bluetooth app  
Greets Flo
```

---
## \#2 Posted by: Andy87 Posted at: 2019-08-01T12:27:10.556Z Reads: 81

```
i would have a look on the component which started to smoke.
```

---
## \#3 Posted by: Flouw Posted at: 2019-08-01T15:19:53.501Z Reads: 73

```
I'll post some pics
```

---
## \#4 Posted by: Flouw Posted at: 2019-08-01T15:22:09.985Z Reads: 74

```
![20190801_171609|281x500](upload://4kgMzRgqlCmBdVrMKuThD661iCF.jpeg) ![20190801_171641|281x500](upload://bmXVdLtulOCdzKYnK00VixdjM51.jpeg) 
The Capacitor i think smoked a bit but the Voltage output is correct.
```

---
## \#5 Posted by: Flouw Posted at: 2019-08-01T15:23:28.029Z Reads: 68

```
![Screenshot_20190801-171657_xiaoxiang|243x500](upload://poBNy3VmThh5m1T9aoTufszu47O.jpeg) 
This is a screenshot from the app. So i think it cant be the wireing because every cell is detected.
```

---
## \#6 Posted by: bartroosen12 Posted at: 2019-08-01T18:42:51.635Z Reads: 58

```
The cap smoked? Weird stuff

Are you sure the charger plug which goes to the bms is okey? I should measure the charge port of the bms if the voltage is correct (around 38V).

If that's the case I don't think your bms is broke but I guess your charger has failed.
```

---
## \#7 Posted by: Flouw Posted at: 2019-08-02T13:04:05.192Z Reads: 52

```
Thx for the reply :) 
the BMS shows 38V on the output. Maybe it's really the charger. I'll order a new one and post results.
```

---
## \#8 Posted by: bartroosen12 Posted at: 2019-08-05T12:20:36.930Z Reads: 43

```
A couple builds back I had the same issue with a power supply and a step u converter which didn't work, no idea why but the problem was also the charger.

I got my 42V 4A charger from alliexpress (25€) and it works good for me.
```

---
## \#9 Posted by: Flouw Posted at: 2019-08-06T08:54:50.065Z Reads: 35

```
nice 
a new charger is on the way :slight_smile:
```

---
## \#10 Posted by: Flouw Posted at: 2019-08-09T14:06:05.761Z Reads: 30

```
So everything works fine now :slight_smile:  it was indeed the faulty charger :frowning: thx all
```

---
