# Speed and Range Deficiency?

### Replies: 8 Views: 364

## \#1 Posted by: carwyn987 Posted at: 2018-06-27T22:02:43.012Z Reads: 96

```
**_Two questions_**

I built an electric longboard two years ago using the following parts:

[1 - 5055 280kv electric brushless motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html)

[1 - Hobbyking 150A EZRUN](https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html)

[2 - 5000mah 11.1v 3 cell lipo](https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html)
in series to make 6s 5000mah battery

90mm wheels
16 tooth motor gear
40 tooth wheel gear

rider weight + board weight - 165

the cruising speed was only about 12 mph, with the top speed being only 13mph.
The range was about 5 miles and crapped out then because of the voltage cutoff on the esc, and the bluetooth phone app I was running with an rfduino and a regular arduino running off of a 9 volt battery drained it.

Did i do something wrong? why was the speed so low? was it the high kv rating and a low torque(and large wheels)/low number of cells?



**Now I know more and am building a V2.**
The parts I bought are listed below, they are shipping right now:

[1 - TORQUE ESC BLDC ELECTRONIC SPEED CONTROLLER](products/torque-esc-bldc-electronic-speed-controller)

[1 - ELECTRIC SKATEBOARD MOTOR 6374 190KV](products/electric-skateboard-motor-6374-190kv)

[4 - 5000mah 3 cell 11.1v lipo high discharge batteries](https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html) in series to make a 44.4v 5000mah battery. 

Same trucks and wheels and gears/belt:
90mm wheels
16 tooth motor gear
40 tooth wheel gear

rider weight + board weight - 175

Assuming i set the vesc up correctly, what should be the **top speed** and **range**(assuming I run it around 15-20 mph for its full battery life(assuming the 80% rule as to not damage the lipo's)).

Thanks in advance!
```

---
## \#2 Posted by: ROFEN13 Posted at: 2018-06-27T22:11:39.707Z Reads: 79

```
Top speed will be around upper 20s low 30s. And range will probably be around 10... but honestly it depends on how you ride. In theory my battery should be able to bring me almost 20 miles, but i ride hard so i get closer to 12. 
Search esk8 calculator or esk8 range calculator.
```

---
## \#3 Posted by: carwyn987 Posted at: 2018-06-27T22:13:53.925Z Reads: 75

```
@ROFEN13  Thanks that answers my second question. what do you think about my first?
Also, the range calculator only says it should go 4.2 miles and 30.24 mph max
```

---
## \#4 Posted by: ROFEN13 Posted at: 2018-06-27T22:28:49.459Z Reads: 66

```
![Screenshot_20180627-182744_Chrome|243x500](upload://ykQtWGDc2Uznm2ZFhwbtWaO5K5A.jpg)
![Screenshot_20180627-182732_Chrome|243x500](upload://5PoXiP1jshI5A52xG5GwxX1xlir.jpg)
```

---
## \#5 Posted by: carwyn987 Posted at: 2018-06-27T22:36:33.681Z Reads: 51

```
 huh i must have written something wrong.
sorry for the wasted time and energy
thanks @ROFEN13!
```

---
## \#6 Posted by: ROFEN13 Posted at: 2018-06-27T22:53:34.414Z Reads: 41

```
You didnt! Also, i have no idea why you only got 13 max speed on your last build. Maybe a setting with the esc, or the remote?
```

---
## \#7 Posted by: carwyn987 Posted at: 2018-06-28T20:09:00.705Z Reads: 31

```
@ROFEN13 why does that page show lipo to be 4.2 volt when it is actually more like 3.7(3.86) fully charged
```

---
## \#8 Posted by: ROFEN13 Posted at: 2018-06-28T21:45:16.087Z Reads: 19

```
Because lipos are supposed to be charged to 4.2 per cell. I think we found your performance issue!
```

---
