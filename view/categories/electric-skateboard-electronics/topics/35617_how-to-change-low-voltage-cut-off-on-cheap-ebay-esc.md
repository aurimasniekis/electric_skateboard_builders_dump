# How to change low voltage cut off on cheap eBay ESC

### Replies: 23 Views: 1967

## \#1 Posted by: Orin635 Posted at: 2017-10-16T00:41:11.568Z Reads: 159

```
Hi guys,

In this cheap eBay ESC It says the low voltage cut-off is 3.0V and I know that is way to low. So people who have used them before what have you done about this? <img src="/uploads/db1493/original/3X/e/e/eed009848bdc3229e94cd544fdaa4c165e9b49ff.png" width="281" height="500">



Ebay esc link:
  https://m.ebay.com/itm/322688412411?varId=511729893110&_mwBanner=1
```

---
## \#2 Posted by: pat.speed Posted at: 2017-10-16T08:47:33.542Z Reads: 133

```
I don't think it is possible to change without changing the software
```

---
## \#3 Posted by: Grozniy Posted at: 2017-10-16T09:04:14.707Z Reads: 132

```
And it is not possible to change the software or customize it. That's what seller said
```

---
## \#4 Posted by: Orin635 Posted at: 2017-10-16T09:52:14.711Z Reads: 125

```
What did people do to work around that?
```

---
## \#5 Posted by: pat.speed Posted at: 2017-10-16T09:55:19.988Z Reads: 121

```
Use lithium Ion cells or use a BMS or just monitor the cell voltages with a cell checker
```

---
## \#6 Posted by: Orin635 Posted at: 2017-10-16T10:07:44.001Z Reads: 119

```
I'd prefer not to get into lion cells , also I was going to buy a cheap eBay bms so would that do the job?
```

---
## \#7 Posted by: pat.speed Posted at: 2017-10-16T20:26:12.690Z Reads: 102

```
Well as long as it has the correct specs. Will you be discharging through the bms?
```

---
## \#8 Posted by: Orin635 Posted at: 2017-10-16T20:33:26.439Z Reads: 97

```
no only using it for charging
```

---
## \#9 Posted by: pat.speed Posted at: 2017-10-16T20:41:55.810Z Reads: 95

```
Well then you will need a way of monitoring your battery cells. Search for battery medic on hobbyking it is cheap and will also balance your cells
```

---
## \#10 Posted by: Orin635 Posted at: 2017-10-16T20:42:51.481Z Reads: 92

```
would that replace the BMS
```

---
## \#11 Posted by: bartroosen12 Posted at: 2017-10-16T20:58:15.953Z Reads: 93

```
I'm using that esc too,
I have done some test and I drained my battery until the esc stops and starts beeping when the battery is empty.
After the run I measured and every cell was around 3,4V so they won't be 3V.
It's because of the voltage sag I think but it's a healthy voltage for the batteries.
But you can always use a good 50A bms.
I use lipo batteries and they have a bms but only for charging.
```

---
## \#12 Posted by: pat.speed Posted at: 2017-10-16T21:00:36.344Z Reads: 88

```
No that monitor won't replace the bms
```

---
## \#13 Posted by: stellaren Posted at: 2017-10-16T21:05:45.948Z Reads: 87

```
how does the switch work? does it shut everything off or do you need antispark or separate switch?
```

---
## \#14 Posted by: Orin635 Posted at: 2017-10-16T21:07:24.117Z Reads: 80

```
Hi,
Could you tell me your thought on the ESC. is the breaking good?anything I need to know before I buy?
```

---
## \#15 Posted by: Orin635 Posted at: 2017-10-16T21:07:47.195Z Reads: 81

```
Your build sounds very similar to what I am planning on doing
```

---
## \#16 Posted by: bartroosen12 Posted at: 2017-10-16T21:49:36.957Z Reads: 82

```
The switch shuts everything off yep,
But I have also a xt60 but it's always plugged in.
<img src="/uploads/db1493/original/3X/6/3/63e44c402161a749a936e63694ac7ea88b6c477e.jpg" width="666" height="500">
```

---
## \#17 Posted by: bartroosen12 Posted at: 2017-10-16T21:55:47.566Z Reads: 81

```
I really love this esc.
It just feels so much better than the FVT120A.
Breaks are very good and can be very strong but you can choose how hard you brake with the trigger.

Yeah you really need to keep in mind that if you go for the 10S version of this you need to stay around a 150Kv motor. I discovered that the esc ermp is limited or how is it called. So you will get the same speed with a 150kV motor than with a 200kV motor.
So go for one of these:
If you want a cheap but still a good a built, the racestar is really very good and you can directly plug in the sensor wires into the esc.
https://m.banggood.com/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html?rmmds=mywishlist
https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html?___store=en_us
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html?___store=en_us
```

---
## \#18 Posted by: Orin635 Posted at: 2017-10-16T21:56:30.686Z Reads: 80

```
I will be using 6s,

Is the remote good? any disconnects? do all the buttons and functions work?
```

---
## \#19 Posted by: bartroosen12 Posted at: 2017-10-16T21:59:20.888Z Reads: 79

```
Yeah remote feels very good.
Everything works like it should, no disconnect.
Switch for low/fast mode,
Switch to switch motor direction,
Leds on controller indicating battery of the board.
6S so stay below a 250kV motor ;)
```

---
## \#20 Posted by: Orin635 Posted at: 2017-10-16T22:00:20.641Z Reads: 75

```
would a dual 270kv drive (3:1 gear ratio) be ok? 

what does the [quote="bartroosen12, post:19, topic:35617"]
Switch to switch motor direction,
[/quote]

do?
```

---
## \#21 Posted by: Brycehoosiers Posted at: 2017-10-16T23:29:34.853Z Reads: 70

```
Makes the board go forward or reverse
```

---
## \#22 Posted by: Orin635 Posted at: 2017-10-16T23:41:36.502Z Reads: 70

```
Lol that makes sense haha
```

---
## \#23 Posted by: bartroosen12 Posted at: 2017-10-17T05:32:03.017Z Reads: 69

```
Yeah 270kV will be fine
```

---
