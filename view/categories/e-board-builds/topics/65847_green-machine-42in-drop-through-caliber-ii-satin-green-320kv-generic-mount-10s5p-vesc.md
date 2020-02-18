# Green Machine &#124; 42in drop through &#124; Caliber II satin green &#124; 320KV &#124; Generic Mount &#124; 10s5p &#124; VESC

### Replies: 14 Views: 497

## \#1 Posted by: Bugist Posted at: 2018-08-23T17:01:36.179Z Reads: 187

```
Most of the parts are still on their way, but for now ive discovered that my wheel pulley needs a bit of modification to properly fit the truck. So here it goes.
```

---
## \#2 Posted by: Bugist Posted at: 2018-08-23T17:06:08.931Z Reads: 186

```
![20180823_110220|374x499](upload://lHDshGzyHuO7SfwltkS17ZqleDH.jpg)
Currently enlarging the ID of the pulley, battery updates later today.
```

---
## \#3 Posted by: mynamesmatt Posted at: 2018-08-23T21:37:16.025Z Reads: 164

```
320kv is very high, just saying
```

---
## \#4 Posted by: pat.speed Posted at: 2018-08-23T22:14:27.833Z Reads: 157

```
It will work as long as it is geared properly, something like 15:44 or so would probably be good
```

---
## \#5 Posted by: Bugist Posted at: 2018-08-24T05:06:38.077Z Reads: 139

```
Exactly, I'm actually using 20 60 and only weigh 130 lbs / 60 kilos so I should be well within its limits, plus the motor only cost 40 USD
```

---
## \#6 Posted by: delinlo Posted at: 2018-08-24T11:16:03.219Z Reads: 133

```
I've always wanted to do a build with really high kV motors but sadly I live in the mountains and I need the torque. If I were you, 60kg and living somewhere flat, I would actually use the speed of the motors to my advantage, not undergear them to shit. If you're an experienced rider, prepared to push start and ready to wear the proper safety gear, we can do some maths:

Admitting you use: 
- regular 100mm wheels
- 14:36 pulley ratio
- 10s 18650
- 320kV motors

That means full battery voltage is 10x4.2=42V
At no load full power 42Vx320kV= 13440 rpm 
14:36=0.388
13440rpmx0.388=5227rpm
100mm wheelx3.14=314mm travel per wheel revolution = 0.314meters
5227rpmx0.314=1641 meters per minute = **98.47 km/h max theoretical top speed**

That's the no load top speed, IRL it'll be more like 70-90% that value depending on conditions.

Now if you use your 20:60 ratio, the theoretical top speed is **84.4 km/h** which is still wayyy over the average 170kV motor top speed. 

So be aware that your board will be very speedy and dangerous but will greatly lack in torque and be extremely inefficient at lower speeds (10-20km/h). At those pretty normal speeds, most of your battery will go into heat because your motor is build to be efficient for wayy higher rpm. Electric motors like spin fast!
For reference, 14000 RPM is the speed at which, on average, f1 cars' engines hit the rev limiter. So imagine how your board will sound like at full speed!

Anyways, rant over, all the best for the build!
```

---
## \#7 Posted by: Bugist Posted at: 2018-08-25T00:11:57.747Z Reads: 106

```
Loving the math! Only problem is i live at the bottom of the steepest bridge in the city, im not sure what its grade is but i know its pretty bad
```

---
## \#8 Posted by: Bugist Posted at: 2018-08-25T00:14:51.874Z Reads: 105

```
![1535155924089727760130|374x499](upload://7gE25mT8nfb0SUto2zXc0fUvKuy.jpg)
Heres the battery that im beginning to wire up for 10s5p. These are 2200 MAH LG cells out of about 13 modems...
```

---
## \#9 Posted by: delinlo Posted at: 2018-08-25T12:11:13.151Z Reads: 82

```
Then gear down or else you’ll fry your motors. Do the maths upside down trying with 50km/h top speed to figure out your ideal ratio. So you’ll get a similar performance than 190kV motors through gearing.
```

---
## \#11 Posted by: Bugist Posted at: 2018-08-25T14:19:06.992Z Reads: 77

```
With 83mm wheels and a 3:1 ratio the esk8 calculator puts me right at about 30 mph/50 kph loaded top speed at the nominal battery voltage
```

---
## \#12 Posted by: delinlo Posted at: 2018-08-25T20:44:18.780Z Reads: 68

```
That is perfect then. I did the math with 100mm wheels.
```

---
## \#13 Posted by: Bugist Posted at: 2018-08-25T21:38:55.031Z Reads: 70

```
![15352330033041355151736|375x500](upload://5Sd5S5wn14LV2eUPzH3LqVRVbaP.jpg)
Anyways maybe you guys have been wondering why it's called the green machine.
```

---
## \#14 Posted by: Bugist Posted at: 2018-09-09T19:51:06.239Z Reads: 45

```
![20180905_234720|374x499](upload://2bSrKXuo5PmmR9t7tg8MIAKw4FK.jpg)
Battery is all done, its going in a case as i type this
```

---
## \#15 Posted by: Bugist Posted at: 2018-09-09T19:55:57.874Z Reads: 45

```
![Electric%20Longboard%20schematic%20(2)|690x345](upload://3qfh61ELfm2B2A9JNQfz2wrcSMR.png)
Also my BMS is charge only so heres how its wired, with all the yellow bits being XT-90s
```

---
