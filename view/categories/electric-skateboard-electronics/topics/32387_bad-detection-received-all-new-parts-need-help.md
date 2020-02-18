# Bad detection received all new parts (Need Help)

### Replies: 23 Views: 1002

## \#1 Posted by: MustardTiger Posted at: 2017-09-06T04:01:08.567Z Reads: 115

```

I've got the board assembled and it looks awesome but I cant get past the motor detection. I believe my vesc values are ok and i checked the resistance between the phase wires everything looks good. When I start detection the the motor spins up but I get "bad motor detection received". I then go to terminal and type in faults and there are none. The motor responds to the nano remote but I don't want to ride it without configuring the vesc properly. Also when I'm plugged into the computer the left and right keys don't spin the motor there's just a clicking noise. Any help would be greatly appreciated I really want to get this thing going.

<img src="/uploads/db1493/original/3X/d/7/d79af22b864100998d441fffcd93a2093b85eba5.JPG" width="640" height="480">

<img src="/uploads/db1493/original/3X/d/5/d5fce12ba7db7c2c048bfd84b85d836e3682e3e6.JPG" width="640" height="480"><img 

<img src="/uploads/db1493/original/3X/8/0/8089a34d6b2b1110beff02d6669688d1a9662508.JPG" width="640" height="480">

<img src="/uploads/db1493/original/3X/e/2/e22074ad14ef1e6e9f88c2df1e870db5b0835cd9.JPG" width="640" height="480">
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-09-06T04:07:19.048Z Reads: 107

```
Are your battery fully charge ?
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-09-06T04:08:14.170Z Reads: 106

```
U forgot to unload the motor. Take the wheel out!
```

---
## \#4 Posted by: MustardTiger Posted at: 2017-09-06T04:38:45.237Z Reads: 107

```
I was told it doesn't matter if the belt is on during detection but I'll give it a try
```

---
## \#5 Posted by: MustardTiger Posted at: 2017-09-06T04:39:54.996Z Reads: 107

```
Yes the battery is charged on the Realtime data it show the battery is at 24.7 V
```

---
## \#6 Posted by: dg798 Posted at: 2017-09-06T13:10:46.741Z Reads: 95

```
Check your values for cutoff start and end and make sure that the cutoff start is not too high
```

---
## \#7 Posted by: MustardTiger Posted at: 2017-09-07T03:27:32.105Z Reads: 86

```
Same results with belt removed
```

---
## \#8 Posted by: onepunchboard Posted at: 2017-09-07T03:29:38.875Z Reads: 87

```
try this. set up the ppm first and run the motor with default values.
Un plug receiver a disable app config
and do detection.

also try 3s batt instead of full batt u have
```

---
## \#9 Posted by: onepunchboard Posted at: 2017-09-07T03:44:46.492Z Reads: 81

```
and just in case. when motor detaction set batt cut off to 3v per cell and write config then give a try.
```

---
## \#10 Posted by: MustardTiger Posted at: 2017-09-07T05:09:46.412Z Reads: 75

```
Figured it out. Looks like I got a bad motor :( brand new too! I swapped in a different motor and the detection worked just fine
```

---
## \#11 Posted by: Namasaki Posted at: 2017-09-07T05:35:22.233Z Reads: 73

```
[quote="MustardTiger, post:4, topic:32387, full:true"]
I was told it doesn't matter if the belt is on during detection but I'll give it a try
[/quote]


I can't imagine why anyone would say that.
just having the pulley on the motor changes the detection values. How much more when you have the belt on and it's pulling the wheel.

BTW, on your Mac computer, you can press Command Shift 3 to take a screen shot to post your settings. It gives a much better picture than using your phone camera.
Command shift 4 will let you crop a section of the screen for screen shot.
```

---
## \#12 Posted by: torqueboards Posted at: 2017-09-07T06:47:10.341Z Reads: 66

```
@MustardTiger  Looks like your using our motor. It's not typical for the motors to be DOA. Send us an email at help@ and let us know the details, etc. we'll help you get it replaced or tested.
```

---
## \#13 Posted by: MustardTiger Posted at: 2017-09-08T07:59:21.378Z Reads: 60

```
Will do thank you
```

---
## \#14 Posted by: MustardTiger Posted at: 2017-09-12T10:01:00.922Z Reads: 56

```
@onepunchboard  @dg798  @JohnnyMeduse  @Namasaki  @torqueboards So I got the board up and running and it's a monster!! I am having some problems with the vesc overheating and also some issues with the brakes. When I first start out the board takes off like a rocket, hard to even stay on it(that's how I want it) it's really fast too I think I did 32mph. But shortly after it will reset the vesc and power will be greatly reduced. It also can't climb hills even small ones. I have a 6s board with an easy run car esc and 6374 194kv sk3 that can climb just about any hill. The fault I get is over temp fet. After doing some reading it seems that a single 6374 motor and the vesc isn't the best combo for heat. Can I increase the temp threashold or should I get a smaller motor or maybe the 12s car esc from TB? What I want is a torque machine with decent top speed that eats hills for breakfast. Oh yeah the vesc also resets when I come to a full stop(full brake throttle at low speeds)

TB 6374 190kv
12s2p 9AH 45c lipo
TB vesc
18:36 gear ratio
100 mm wheels
12 mm belt

Motor max-80
Motor min-60
Bat max-70
Bat min-12
I also boosted the start up and the throttle ramp speed a little
```

---
## \#15 Posted by: Namasaki Posted at: 2017-09-12T12:31:01.080Z Reads: 49

```
Heatsinks on the Vesc helps for heat. 
Also your gearing is really tall for hills. 
100mm wheels and 18:36 gears. 
I run 90mm wheels with 15:40 gears and have no problem climbing steep hills
```

---
## \#16 Posted by: onepunchboard Posted at: 2017-09-12T14:04:33.558Z Reads: 47

```
looks like something is wrong with vesc setting. try config ppm again. and do not touch temp limit. it will burn the esc. i ise much less torq motor as songle. and dont have any problem like this
```

---
## \#17 Posted by: MustardTiger Posted at: 2017-09-12T21:18:11.357Z Reads: 46

```
Yeah I wasn't even thinking about heat issues when I chose the gear ratio I just wanted the fastest setup and thought 12s could handle it. Did you print your own 40T pulley? I can't seem to find anything that big. TB has a 12mm motor pulley that would give me a 3:1 do you think that would fix it or should I just get the car esc? Before I built this new board I had the 100 mm MTB wheels on 16:36 with the 6s easy run esc and never had any overheating issues.
```

---
## \#18 Posted by: MustardTiger Posted at: 2017-09-12T21:30:47.079Z Reads: 45

```
@torqueboards do you think your 120amp car esc could handle this set up on its fastest setting without overheating?
```

---
## \#19 Posted by: MustardTiger Posted at: 2017-09-13T05:23:39.292Z Reads: 38

```
@Namasaki I installed my old 83mm abec clones and a 16T motor pulley and that did the trick!! Ripped around for 20 min and no resets. Thanks for the advice! I'll have to get some softer wheels though they're really rough compared to those soft mtb wheels
```

---
## \#20 Posted by: cwazy1 Posted at: 2017-09-13T05:46:05.273Z Reads: 35

```
TB VESC is only rated to handle 50a. Your battery max of 70a could cause some issues.
```

---
## \#21 Posted by: MustardTiger Posted at: 2017-09-13T05:53:19.974Z Reads: 34

```
Even though it's set that high you don't actually pull that many amps. I guess it's good to be careful but I felt the performance was lacking at the lower settings
```

---
## \#22 Posted by: Namasaki Posted at: 2017-09-13T12:30:37.051Z Reads: 31

```
[quote="cwazy1, post:20, topic:32387"]
TB VESC is only rated to handle 50a.
[/quote]

That's 50a continuous. 
It can handle higher current for short durations.
```

---
## \#23 Posted by: Namasaki Posted at: 2017-09-13T13:31:12.328Z Reads: 30

```
https://www.muirskate.com/longboard/wheels/1314/83mm-abec-11-flywheels-downhill-longboard-wheels
```

---
