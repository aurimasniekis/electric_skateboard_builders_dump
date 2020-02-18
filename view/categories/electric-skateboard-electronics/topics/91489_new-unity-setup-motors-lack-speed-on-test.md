# New unity setup, motors lack speed on test

### Replies: 18 Views: 285

## \#1 Posted by: evangreen Posted at: 2019-04-23T12:45:49.825Z Reads: 93

```
Excited to get my board running and just setup the unity and got the wheels spinning for the first time.

My motors spin up really fast then sag down to 5 km/hr at full throttle. First time setup and not sure of I have the configuration correct, appreciate help!

I have 2 torque boards 190kv 6355 motors, unity, and an 11s3p Samsung 30q pack. 
Here are my settings after the initial setup:

I checked w a multimeter and my battery is putting out 34.1v which doesn't change when hitting the throttle 

![Screenshot_20190423-134020|236x500](upload://7mQLBGx99ZfR6SpiUKUMDiPZ38D.jpeg)
```

---
## \#2 Posted by: venom121212 Posted at: 2019-04-23T12:49:31.679Z Reads: 84

```
Have you done the remote calibration?

Is everything charged up (remote and board)?

Does the HUD tab show your motors getting signal and reflecting the speed you would be going?

Try this then head to the [unity support thread](https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/)
```

---
## \#3 Posted by: J0ker3366 Posted at: 2019-04-23T12:51:37.139Z Reads: 84

```
Uh 11s and it reads 34v... Your cells are @ 3.0-3.1v so im willing to bet your hitting cutoffs. Charge your battery and try again
```

---
## \#4 Posted by: evangreen Posted at: 2019-04-23T12:53:45.835Z Reads: 81

```
I just figured out. My voltage was just below the cutoff level automatically specified by having an 11 cell battery.

OK, so given my setup, what should those cutoff values be?

Also, what should I charge this pack to!  3.6v x 11 = 39.6?
```

---
## \#5 Posted by: J0ker3366 Posted at: 2019-04-23T12:56:38.698Z Reads: 77

```
46.2v is max charge for 11s. Id put cut offs @ 38/36v. Thats me though. I tend not to run cells below 3.5v. Peraonal reasons.
```

---
## \#6 Posted by: J0ker3366 Posted at: 2019-04-23T12:57:54.233Z Reads: 77

```
[quote="evangreen, post:4, topic:91489"]
3.6v x 11 = 39.6?
[/quote]

A fully charge cell holds 4.2v. So 11s x 4.2v = 46.2v
```

---
## \#7 Posted by: laurnts Posted at: 2019-04-23T13:20:00.933Z Reads: 72

```
it seems like your battery is finished... you hit cut off voltage
```

---
## \#8 Posted by: evangreen Posted at: 2019-04-23T13:39:01.856Z Reads: 66

```
Thanks guys.

Batteries are brand new and have been sitting around for months while I build. I'll charge them up and go from there.


What about the max discharge and regen?
```

---
## \#9 Posted by: J0ker3366 Posted at: 2019-04-23T13:41:02.754Z Reads: 64

```
Mostly flat riding or hilly?
```

---
## \#10 Posted by: evangreen Posted at: 2019-04-23T13:47:05.191Z Reads: 59

```
Mostly flat here in London but a few light hills. Nothing super steep
```

---
## \#11 Posted by: J0ker3366 Posted at: 2019-04-23T13:52:28.650Z Reads: 58

```
40a. If you find yourself struggling with those little hills, up it to 50a. Keep uping till you dont struggle with those hills.
```

---
## \#12 Posted by: evangreen Posted at: 2019-04-23T14:25:00.501Z Reads: 48

```
Ok so 40 on each?
```

---
## \#13 Posted by: J0ker3366 Posted at: 2019-04-23T14:26:40.755Z Reads: 46

```
20a on each. Combinded 40a.
```

---
## \#14 Posted by: banjaxxed Posted at: 2019-04-23T15:20:15.741Z Reads: 41

```
It’s a 3p, 60A continuous/2 = 30A
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-04-23T15:31:13.089Z Reads: 37

```
for the unity he puts in 40a, cause it combines the current of 2 esc's
```

---
## \#16 Posted by: evangreen Posted at: 2019-04-23T16:08:32.805Z Reads: 33

```
I was asking 40a on each i.e. Discharge and regen
```

---
## \#17 Posted by: J0ker3366 Posted at: 2019-04-23T16:10:20.087Z Reads: 32

```
[quote="evangreen, post:16, topic:91489"]
Discharge and rege
[/quote]

Discharge 40a 

Regen -11a or some shit. Might want to ask around for that. I may be wrong.
```

---
## \#18 Posted by: evangreen Posted at: 2019-04-23T16:28:37.286Z Reads: 31

```
Ok thanks...
```

---
