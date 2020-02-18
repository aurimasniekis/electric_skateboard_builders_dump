# Motor sk3 not spin

### Replies: 22 Views: 386

## \#1 Posted by: Starymis Posted at: 2018-11-22T10:04:59.491Z Reads: 98

```
Hi everybody

Yesterday i was using my board and meanwhile motor stoped spin. Batterys are charged, conections and vesc looks good. When i conect it to vesc tool, the motor detection is failed. 
Can you help me how can i found the problem?
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-11-22T10:07:09.896Z Reads: 98

```
type fault into the vesc tool terminal. post results and your vesc settings
```

---
## \#3 Posted by: dareno Posted at: 2018-11-22T10:12:55.836Z Reads: 88

```
Yeah bit more info needed tbh.  What vesc and do you have an antispark?  Bms?  Charge or discharge?  How are you switching?  Oh the info needed should be much more involved in your build.  

DO NOT DETECT THAT MOTOR AGAIN.  until we get some more info.
```

---
## \#4 Posted by: Starymis Posted at: 2018-11-22T15:33:55.610Z Reads: 76

```
I have 2 x 5s lipo in serie, conectors Xt90, maytech vesc, sk3 192. Antispark key xt90, without bsm. Charging imax. 

![15429006428811143326864|375x500](upload://sujjEStStaOJApdyx7dt2EMDR.jpeg) ![15429006921461064421509|375x500](upload://l3lhw3bp2BJmt5FrnBTaLBdzssD.jpeg) ![15429007273292134492520|375x500](upload://lGPrUqKsaEyF8Ar40gIIdJnKkz5.jpeg) ![15429007464991501899519|374x499](upload://u53zVQCHQxPbEKMuWWOee34WNbH.jpeg) ![15429008137031664999396|375x500](upload://9df9961bZ6hcSBbIkOXBWxYnxsK.jpeg)
```

---
## \#5 Posted by: MannyM0E Posted at: 2018-11-22T18:13:31.075Z Reads: 59

```
This my input so don’t bash if I’m wrong, I’m sure others will correct. But you batt max shouldn’t haven been set higher than 50a because it can only handle 50a continuesly and you’re ermp should be set to 50,000ermp and -50,000ermp. Also I notice you put commas instead of dots on your setting. Idk if that matters but I never seen someone use commas before
```

---
## \#6 Posted by: dareno Posted at: 2018-11-22T19:48:14.573Z Reads: 54

```
I've never noticed the comma thing either.  While I agree with some of the points that shouldn't be the reason for a motor stop.  The vesc yes is rated to 50a but 55a won't kill it.  Max erpm is 60000 on most 4.12 vescs so again that shouldn't have killed anything.  
@Starymis did you notice anything on the motor before it stopped.  Smoke smell etc,  does it spin in the hand ok?

what was the nature of the fail?  Did it run down slowly losing power or did it just cut out?
```

---
## \#7 Posted by: Starymis Posted at: 2018-11-22T19:58:41.966Z Reads: 51

```
I use this settings around half year going to work aroin 6km one way.  I went straight around 25km/h and it stoped reciev power like cut out. I look immediate buty no notice nothing strange. Any smoke and smell. Loop key is ok,  vesc looking ok. Motor spin normal
```

---
## \#8 Posted by: MannyM0E Posted at: 2018-11-22T20:06:46.901Z Reads: 44

```
Maybe check the remote ?
```

---
## \#9 Posted by: ShutterShock Posted at: 2018-11-22T20:12:37.645Z Reads: 43

```
I think the commas thing is a european thing.  I have seen that before with other country's numbering.  It is very odd.  As for the batt max, if his battery can output 55A no problem with that, like for me, I have to vescs with each set to 30A batt cuz my BMS can output 60A continuous, and my lipos can do that easily
```

---
## \#10 Posted by: Starymis Posted at: 2018-11-22T20:23:17.606Z Reads: 40

```
Changed battery and nothing. Also should be working in vesc tool
```

---
## \#11 Posted by: Lionpuncher Posted at: 2018-11-22T21:02:36.362Z Reads: 37

```
Check the motor wires. Maybe shorting/broken. Look closely.
```

---
## \#12 Posted by: Starymis Posted at: 2018-11-26T11:38:24.891Z Reads: 33

```
I note that from the vesc is not going out current to the motor? Will be vesc KO?
```

---
## \#13 Posted by: dareno Posted at: 2018-11-26T19:18:15.407Z Reads: 31

```
Any light show on the vesc?
```

---
## \#14 Posted by: Starymis Posted at: 2018-11-26T19:31:33.593Z Reads: 31

```
The lights are working - blue,  white,  green.
```

---
## \#15 Posted by: wafflejock Posted at: 2018-11-26T19:42:26.855Z Reads: 32

```
Just to verify you did remove everything from the motor before attempting detection?  Not sure what caused the original failure but would be good to know what happens exactly when doing detection, does the motor move at all?  Can check for shorts in the motor wires too if you disconnect it from the VESC then spin it by hand it should spin easily, shorting any two of the three phase wires should drastically increase the turning resistance (just to narrow down the issue a bit).
```

---
## \#16 Posted by: dareno Posted at: 2018-11-26T19:51:01.043Z Reads: 32

```

This system is a good way to test the phase wiring on the motor.

Disconnect the motor from everything and disregard the sensor cable, if present.

Connect phase A to phase B and verify by hand spinning that there is choppy braking
Connect phase A to phase C and verify by hand spinning that there is choppy braking
Connect phase B to phase C and verify by hand spinning that there is choppy braking
Connect phase A to phase B to phase C and verify by hand spinning that there is strong, smooth braking

If any of the first 3 brakes feel different, the motor has an issue. They should feel  *identical* . The last brake should feel smooth and not be cogging.

Do this and it will tell you if the motor has an issue. If it checks out then you should be ok to do a detection again.   
Credit for this bit of diy gold goes to @b264  Its a useful check.

Bookmark it.
```

---
## \#17 Posted by: Starymis Posted at: 2018-11-27T10:52:38.117Z Reads: 29

```
One of the combination is going little bit harder but the rest is as you wrote. 
I did motor detection and is failed. 
Vesc terminal not see any fault.
```

---
## \#19 Posted by: dareno Posted at: 2018-11-27T20:49:14.281Z Reads: 27

```
Theres a problem with the motor then.  The first three should be identical in the revolution resistance.  Which combination is wrong?
Also my friend if you want me to reply then reply on my post or tag me.  It will notify me then and not leave you hanging
```

---
## \#20 Posted by: Tallguy64 Posted at: 2018-11-27T21:49:20.294Z Reads: 27

```
The best way to check would be to use a ohm meter and measure the resistance of the different combination to make sure that the coils are not shorted. While you have the meter out use the voltage and check that you are getting voltage at different points in your system.
```

---
## \#21 Posted by: Starymis Posted at: 2018-11-28T08:42:18.451Z Reads: 21

```
The resistance on all motor wires is the same -  1.4
```

---
## \#22 Posted by: Starymis Posted at: 2018-12-13T06:13:14.176Z Reads: 19

```
@dareno I try the motor with new vesc -  is good. 
Maytech vesc is not giving out put current when i throttle
```

---
## \#23 Posted by: dareno Posted at: 2018-12-13T06:15:15.724Z Reads: 17

```
Good stuff my friend.  Always nice when its fixed.
```

---
