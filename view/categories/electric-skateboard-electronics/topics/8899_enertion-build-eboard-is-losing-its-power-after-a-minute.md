# Enertion build &#124; Eboard is losing its Power after a minute

### Replies: 21 Views: 1715

## \#1 Posted by: Monte Posted at: 2016-09-04T16:21:13.567Z Reads: 119

```
Hi, i know there is a similar post like this, but i could not find it..
A few days ago i received finally my space cell pro 4 and today i had time to install it.
I did all the Adjustments in my Vesc for it. [here](http://www.electric-skateboard.builders/t/vesc-faq-optimized-s-p-a-c-e-cell-settings/414/7)
My problem now is that when i go out for a ride, my board have for the first 10 sec. full power but after 300m its loosing slowly its power and can only go 25kmh..
I have the Enertion Vesc v4.12, and the enertion big mono motor (Forgot the name)
Usually does @Onloop what to do?
<img src="/uploads/db1493/original/2X/5/50b8bf0ccdfe57b0b994831cdcb4fedd419c86da.png" width="452" height="500">
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-09-04T16:24:24.341Z Reads: 113

```
Doesn't the VESC come pre-loaded with the info for the SCP3 and R-Spec motor? This is a really interesting issue. Does the space cell still read the correct percentage or does it read that it's out/running out of power?
```

---
## \#3 Posted by: Monte Posted at: 2016-09-04T16:26:28.463Z Reads: 116

```
Do you mean the Battery lcd? Thats working normal.
In the Firmaware folder are only these:
<img src="/uploads/db1493/original/2X/1/130ac9a80e1f0cb27e3dacba8a119f383c710196.png" width="202" height="172">
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-09-04T16:28:37.296Z Reads: 112

```
Yes. I was wondering if the battery could be outputting weird but I guess not. Sounds like a VESC issue. Have you looked at the VESC after it has slowed down? Is it really hot?
```

---
## \#5 Posted by: Monte Posted at: 2016-09-04T16:30:14.197Z Reads: 103

```
No it have normal slight warm temp.
I got another 10s2p from a friend but that one gives power untill its empty.
```

---
## \#6 Posted by: Monte Posted at: 2016-09-04T16:31:49.274Z Reads: 97

```
I would go outside with a laptop and look for an error code but its raining here at the moment :confused:
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-09-04T16:56:40.260Z Reads: 91

```
Sounds like the battery then...
```

---
## \#8 Posted by: ra.rend Posted at: 2016-09-04T16:58:26.614Z Reads: 90

```
On flat ground? While climbing a mountain? How heavy are you?

Seems like your vesc is getting too hot. Mine (space cell 3, mono 6355 motor) slows down after being on full throttle for about a minute on roads with slight incline.
```

---
## \#9 Posted by: Monte Posted at: 2016-09-04T17:00:23.018Z Reads: 83

```
Flat ground, my weight is 85kg
```

---
## \#10 Posted by: ra.rend Posted at: 2016-09-04T17:17:01.616Z Reads: 79

```
I'd suggest going dual drive. Based on others experiences on this forum, a smaller 200 kv motor can climb a certain hill, while the bigger 190kv motor (what you have) will cause the VESC to shut down (due to heat) before it reaches the top of said hill because the bigger motor pulls more power than your battery can provide. I might be wrong though, I'm a noob :)
```

---
## \#11 Posted by: Monte Posted at: 2016-09-04T17:19:48.314Z Reads: 82

```
I dont think its the Overheat. The other battery can go up to 40+kmh for 15km without loosing power. Even with hills.
While driving with the space cell, it feels like the battery try to protect itself... Motor and vesc isnt that much hot. easy to touch.
```

---
## \#12 Posted by: Monte Posted at: 2016-09-04T18:47:48.028Z Reads: 75

```
So i did another test ride for about 4-5km with some other settings. The problem is still there :/
But i noticed that when i accelerate very slowly, it needs longer to lose power. and i get full speed for a longer time. I also noticed the 'slow down' disappear when i reboot the board and my remote.
```

---
## \#13 Posted by: boards Posted at: 2016-09-04T18:56:42.071Z Reads: 74

```
I had something similar happen when a connector had broken apart from a wire causing a poor connection. Connect your laptop and see how big the vdrop is when you accelerate.
```

---
## \#14 Posted by: Monte Posted at: 2016-09-04T19:00:53.851Z Reads: 72

```
I tried it but my laptop cant connect to the vesc. Manager say it sees the 'unknown com connection' but the bldc programm just dont want to connect.
I still try to connect it but if i cant do it i will resolder everything.
```

---
## \#15 Posted by: Monte Posted at: 2016-09-05T08:57:00.761Z Reads: 58

```
Resoldered everything, problem still there... 
I resettetet(etet?) the vesc complete and adjust just the gt2b and motor amps.
Does usually @EnertionSupport know how to fix?
```

---
## \#16 Posted by: Monte Posted at: 2016-09-15T10:03:31.843Z Reads: 47

```
FInally i found the Terminal and the Faults command :smiley:
This is what i get:
The following faults were registered since start:

Fault            : FAULT_CODE_OVER_TEMP_FET
Current          : -55.2
Current filtered : -41.1
Voltage          : 40.91
Duty             : 0.03
RPM              : 6882.4
Tacho            : 442256
Cycles running   : 22989
TIM duty         : 1163
TIM val samp     : 635
TIM current samp : 21468
TIM top          : 41666
Comm step        : 3
Temperature      : 101.24 

I really dont get why the mosfets are overheating that much... This fault code comes from a 10 min ride on flat ground with mid wind.
```

---
## \#17 Posted by: Pimplaren Posted at: 2016-09-15T10:25:52.018Z Reads: 45

```
I can ride hard with 15/32, 80mm wheels, 190 6374 r-spec, 10s 8ah and vesc without overheating, i am around 104kg =)

Has to be something with the battery? really strange tho
```

---
## \#18 Posted by: Monte Posted at: 2016-09-15T10:38:22.647Z Reads: 45

```
It has to be with the battery... I have a s 10s2p from a friend and with that one i can go full speed untill its empty... (15km)
But i dont want to send it back... I think i dont have the warrinty anymore because i changed the lcd and switch out.
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-09-15T11:11:26.440Z Reads: 45

```
Can you make a picture of the battery and exspecially the modofications you made on it. Because in the fault log the current seems quite high to me. Can it be that you breaked very hard when the vesc switched off.
```

---
## \#20 Posted by: Monte Posted at: 2016-09-15T11:13:52.629Z Reads: 46

```
Yes i did a brake. I do some pics later i have to go the work :)
```

---
## \#21 Posted by: Nordle Posted at: 2016-09-15T13:49:08.412Z Reads: 40

```
Sounds like a bad cell to me, when you draw many amps the voltage in your battery drops. When there is a bad cell the voltage drops even more and then VESC low voltage cutoff shuts it down.
```

---
