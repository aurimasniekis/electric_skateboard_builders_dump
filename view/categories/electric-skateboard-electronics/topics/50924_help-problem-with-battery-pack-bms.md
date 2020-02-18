# Help..problem with battery pack/BMS

### Replies: 12 Views: 560

## \#1 Posted by: theviith Posted at: 2018-04-02T04:09:23.818Z Reads: 111

```
hey guys, so my board is having some battery issues, can someone help me identify what the problem is? I've tested the VESC and determined it is not a DRV fault. Right now it seems more of either BMS or internal li-ion cell issue. Here's some of the symptoms:
1. when battery level is at 40-70 percent, I am able to brake without issues.
2. when battery level is either above 75% or below 35%, I am unable to brake at all but still able to accelerate without any problems. When I attempt to brake, the VESC gets cut off and resets itself. This happened on both VESC I swapped tested.
3. when battery level is at or below 33%, the board stutters on acceleration and randomly shuts down. But when I push on it manually, it powers on again and can go for another 10-20 feet before powering off again.

battery pack is 10S5P, custom made.
BMS is Supower 10S60A.
Had this pack for over a year now so it could be that the pack is slowly reaching it's end of life...but should it be cutting off the brake like that?

thanks for the help in advance
```

---
## \#2 Posted by: Lionpuncher Posted at: 2018-04-02T04:13:55.556Z Reads: 105

```
I'm no expert, but im guessing you have a bad cell in one or more p groups causing an unbalanced battery. Have you measured your voltages of each individual p group? My guess is bms us doing it's job and battery is sagging hard due to bad cell(s).
```

---
## \#3 Posted by: theviith Posted at: 2018-04-02T04:20:14.739Z Reads: 102

```
no not yet, I can try doing that.
if it is because of a bad cell causing unbalanced battery, would charging it to 100% help re-balance the cells? would it also be safe to charge the pack if one or more of the cells are damaged?
```

---
## \#4 Posted by: Acido Posted at: 2018-04-02T07:42:23.620Z Reads: 79

```
Keep it plugged for an hour or two aftet it charges, that should balance the cells if some packs are super drifted
```

---
## \#5 Posted by: Acido Posted at: 2018-04-02T07:42:49.254Z Reads: 75

```
If you have a bad cell, you must replace it
```

---
## \#6 Posted by: pat.speed Posted at: 2018-04-02T08:49:19.102Z Reads: 60

```
Can we see your VESC settings. It might be incorrectly set voltage limits
```

---
## \#7 Posted by: theviith Posted at: 2018-04-02T14:54:01.453Z Reads: 50

```
@pat.speed I will screenshot the settings once I get home today. 

@Acido thanks for the advise. So if there is a bad cell in the pack, would it be safe to keep the pack plugged in 1-2 hours after it charges like you've mentioned?

Also, how can I determine the bad cell from the pack if there is one?
```

---
## \#8 Posted by: theviith Posted at: 2018-04-02T19:25:38.746Z Reads: 44

```
here's my VESC setting for Master. 
Slave is basically the same except for controller ID and motor detection values.

![41|690x388](upload://mnyncIV6u3xvbhlN3pkrt352R0r.png)![50|690x388](upload://iYhPYyvoPb6jNOiuwpixwmtpTSC.png)![08|690x388](upload://p2IfEhz6bI6XOmFjJiBnnBjGr48.png)![01|690x388](upload://sRx6KEOVQwjXOSHN2AA5gElRuXr.png)
```

---
## \#9 Posted by: RedEagle Posted at: 2018-04-02T19:33:45.758Z Reads: 37

```
You might wanna uncheck limit erpm with negative torque.
```

---
## \#10 Posted by: pat.speed Posted at: 2018-04-02T21:47:32.189Z Reads: 31

```
Those values are also a little bit conservative for a 10s battery. You could change them down to 30v start, 28v end. Apart from that there doesn’t seem to be much wrong with anything else. I would also just check the cell voltages to see how balanced they are before setting the cut off lower
```

---
## \#11 Posted by: theviith Posted at: 2018-04-03T03:04:46.990Z Reads: 27

```
@RedEagle What does unchecking the limit erpm with neg torque do?

@pat.speed Thanks, yea I didn't think it was the VESC problem from the beginning. Sigh, guess I have to open the pack up and find the bad apple...
```

---
## \#12 Posted by: RedEagle Posted at: 2018-04-03T14:17:03.668Z Reads: 23

```
If you keep this checked the vesc will brake when you go over the erpm limit. This will result in you facebraking instantly when that happens. Since you're using a 170kv motor this'll never happen, but it's better to be safe than sorry.
```

---
