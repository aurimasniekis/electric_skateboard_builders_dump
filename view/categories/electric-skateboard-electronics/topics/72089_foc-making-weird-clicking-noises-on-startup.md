# FOC making weird clicking noises on startup

### Replies: 28 Views: 288

## \#1 Posted by: Livid Posted at: 2018-10-23T17:17:46.479Z Reads: 80

```
I've got a dual motor setup, pair of 100kv hubs and vesc4.12's, BLDC works fine on both of them, i had to upgrade c18 to get FOC working without drv errors on one of the two sides, but that side now makes clicking noises and shakes pretty damn badly accelerating from low speed, like regular bldc jitter but much worse, doesnt happen unloaded at the same erpm, any ideas?
```

---
## \#2 Posted by: nuttyjeff Posted at: 2018-10-23T17:42:46.628Z Reads: 74

```
I have the exact problem on FOC with one of my VESCs now. Nfi idea why, woukd love it if someone could solve this issue.
```

---
## \#3 Posted by: dareno Posted at: 2018-10-23T21:53:13.438Z Reads: 69

```
I know you've upgraded but 4.12 does not like foc unless its a focbox so maybe tag one of the enertion boys to see if they can help.
```

---
## \#4 Posted by: Livid Posted at: 2018-10-23T22:27:29.654Z Reads: 64

```
Ok, i might just go back to bldc, shame as it's so quiet on FOC, but i can't afford to break anything
```

---
## \#5 Posted by: dareno Posted at: 2018-10-23T22:32:55.770Z Reads: 61

```
Yeah it seems to be the case.  Problems on foc with 4.12.  I'm not in any way able to help with the tech on that but I know its never worked well for me on anything other than a focbox.  I like the loud whine of my sk3's though and would not trade that esk8 signature scream for anything.  BLDC all the way.
```

---
## \#6 Posted by: Livid Posted at: 2018-10-23T22:38:20.805Z Reads: 57

```
maybe in the future i'll upgrade to a unity or something, but i guess bldc will work for now. FOC was weird, working better for climbing hills, but seems like it has a lot less speed for a set current
```

---
## \#7 Posted by: Deodand Posted at: 2018-10-23T22:39:36.048Z Reads: 60

```
sensored or unsensored?
```

---
## \#8 Posted by: Livid Posted at: 2018-10-23T22:40:30.517Z Reads: 55

```
hall sensors correctly setup on both
```

---
## \#9 Posted by: dareno Posted at: 2018-10-23T22:40:54.180Z Reads: 54

```
I'll just leave you in @Deodand capable hands.
```

---
## \#10 Posted by: Deodand Posted at: 2018-10-23T22:41:47.563Z Reads: 53

```
are you running 2.xx FW or 3.xx?
```

---
## \#11 Posted by: Livid Posted at: 2018-10-23T22:42:42.691Z Reads: 53

```
Latest one, 3.40 i think. it's a bit weird that one of the motors needs a tad more current to spin up, but that might be because i have invert motor direction set on that because i CBA to fiddle with the wiring
```

---
## \#12 Posted by: Deodand Posted at: 2018-10-23T22:44:17.542Z Reads: 50

```
Interesting, I've seen this problem on the 2.xx FW. There's a couple possibilities. Have you tried increasing the sensorless ERPM setting under MOTOR SETTINGS>FOC>HALL SENSORS in the vesc tool? Try 5k erpm instead of 2.5 k default
```

---
## \#13 Posted by: Deodand Posted at: 2018-10-23T22:44:44.797Z Reads: 50

```
Also can you tell me your motor inductance/resistance values?
```

---
## \#14 Posted by: Livid Posted at: 2018-10-23T22:45:43.024Z Reads: 49

```
Ok, possible it is that as it is a 36p motor, i'll try that for sure. I still think it's unusual only one motor is having issues, but oh well
```

---
## \#15 Posted by: Deodand Posted at: 2018-10-23T22:47:44.035Z Reads: 48

```
I've had some issue where the current controller time constant is mismatched with the motor and it has caused jitters on me. Problems with only 1 of the motors then? Strange. Screenshot of the hall sensor values would be helpful also, possible one of your halls is being weird.

Edit: suppose if the halls work in BLDC they should be ok... hm.
```

---
## \#16 Posted by: Livid Posted at: 2018-10-23T22:49:13.141Z Reads: 48

```
resistance was 88mohm, then i reran it after a run and it was 100mohm, Inductance is 24.65 uH, lambda is 7.005.
```

---
## \#17 Posted by: Livid Posted at: 2018-10-23T22:51:34.030Z Reads: 48

```
The differences are the motor that works perfectly is direct soldered to the vesc with cut down wires, the one that's behaving weird is using a vesc that i got about a month after the first one, but both from maytech, and the wires are untouched
```

---
## \#18 Posted by: Deodand Posted at: 2018-10-23T22:57:00.971Z Reads: 50

```
Try sensorless Erpm change first, if that doesn't work then try the following: 

25 uHenry / 100 mOhm = 250 uSeconds. Try changing T in the FOC detection to a lower value closer to 250 u Seconds instead of 1000 u Seconds.
```

---
## \#19 Posted by: Livid Posted at: 2018-10-23T22:59:04.064Z Reads: 48

```
Ok great thanks, i've got to go now as it's past midnight where i am, but i have hours tomorrow to check and test and fiddle, Thanks so much for all your help, I really appreciate it
```

---
## \#20 Posted by: Deodand Posted at: 2018-10-23T22:59:27.246Z Reads: 47

```
No worries, dump some screen grabs here if problem persists.
```

---
## \#21 Posted by: Livid Posted at: 2018-10-24T09:31:24.300Z Reads: 36

```
Running the motor config again i've noticed that the good motor spins straight upon lambda detection, the dodgy one stutters a bit before spinning up
```

---
## \#22 Posted by: Deodand Posted at: 2018-10-24T18:10:19.096Z Reads: 26

```
I've seen this behavior before with two good motors, could just be manufacturing variances.
```

---
## \#23 Posted by: Livid Posted at: 2018-10-24T18:41:59.434Z Reads: 24

```
Ok cool, my remote has been seriously playing up today so i haven't been able to test it much, but between the cutouts every 6 feet it certainly seems like it's helped a lot, i'll try and fix the remote tomorrow and let you know
```

---
## \#24 Posted by: Deodand Posted at: 2018-10-25T19:56:26.503Z Reads: 18

```
Any developments?
```

---
## \#25 Posted by: b264 Posted at: 2018-10-25T19:57:54.813Z Reads: 18

```
[quote="Livid, post:4, topic:72089"]
i can’t afford to break anything
[/quote]

If you can't afford to break anything, you should never be running FOC
```

---
## \#26 Posted by: Livid Posted at: 2018-10-25T20:22:24.485Z Reads: 16

```
seems much better, my remote still isn't helping me properly test it, but i think i've finally fixed the connection issues. it's certainly not as prevalent as it was. Thanks again for all your help
```

---
## \#27 Posted by: Deodand Posted at: 2018-10-25T21:06:23.743Z Reads: 14

```
Any insights on which change seemed to help?
```

---
## \#28 Posted by: Livid Posted at: 2018-10-25T22:40:17.108Z Reads: 12

```
No i changed both at the same time, didn't think to do them individually
```

---
