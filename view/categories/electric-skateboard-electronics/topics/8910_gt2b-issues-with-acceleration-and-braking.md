# GT2B Issues with acceleration and braking

### Replies: 11 Views: 1454

## \#1 Posted by: ecuadorche Posted at: 2016-09-04T19:06:49.106Z Reads: 109

```
Whenever pull the trigger hard on my gt2b either to accelerate or brake with or without load the board stops responding for a few seconds and then works, however when i brake or accelerate in a short smooth motion it brakes and accelerate correctly what could be causing this, the first time i experienced this the board had a fully charged battery i havent rode it since so idk if it has to do with fully charged batteries being a cause, im using a gt2b with vesc and 5s lipos wired to 10s the lipos are 18.5v 4000 mah 15c
```

---
## \#2 Posted by: sl33py Posted at: 2016-09-04T19:20:19.999Z Reads: 107

```
sounds like you need to look at the VESC errors.  Realtime logging and the faults command line.

my guess is you are getting an ABS error on braking and overvoltage error on hard acceleration.  I had similar issues when testing 12s and fixed by adjusting the settings.  IIRC i'd get a couple blinks of one of the LEDs (red i think) and it would be non responsive for 1-2 seconds then reconnect and respond.

Hook up your VESC to BLDC and give us some screenshots.
```

---
## \#3 Posted by: ecuadorche Posted at: 2016-09-04T19:32:08.022Z Reads: 103

```
yep its giving me a couple of blinking red light when i do it the way i explained, whenever i accelerate gently it shows yellow lights but then goes red when i do it hard.. I'll give screenshots in a bit im not near my pc atm
```

---
## \#6 Posted by: Titoxd10001 Posted at: 2016-09-04T19:43:11.089Z Reads: 88

```
It could be over voltage you can set your max voltage to 57v. It doesn't sound like a remote issue but vesc issue
```

---
## \#16 Posted by: sl33py Posted at: 2016-09-04T23:54:14.492Z Reads: 79

```
[quote="ecuadorche, post:3, topic:8910, full:true"]
yep its giving me a couple of blinking red light when i do it the way i explained, whenever i accelerate gently it shows yellow lights but then goes red when i do it hard.. I'll give screenshots in a bit im not near my pc atm
[/quote]


Yeah sounds exactly like my issue.  Adjusted both my ABS and voltage settings and fixed.  You'll probably see ABS overvoltage error when braking and another over voltage error accelerating.
```

---
## \#4 Posted by: treenutter Posted at: 2016-09-06T03:07:00.887Z Reads: 53

```
11 posts were split to a new topic: [Throttle issue with GT2B](/t/throttle-issue-with-gt2b/9027)
```

---
## \#17 Posted by: ecuadorche Posted at: 2016-09-14T15:13:40.040Z Reads: 55

```
so yeah its still doing the same and you are correct @sl33py it gives an overvolatage error what do you need screenshots of???
```

---
## \#18 Posted by: ecuadorche Posted at: 2016-09-14T15:20:06.364Z Reads: 52

```
<img src="/uploads/db1493/original/3X/e/b/eb0e71da08339dc3a30affa54e592da01c64620a.png" width="690" height="431"><img src="/uploads/db1493/original/3X/5/3/53b74e2c3af69439830ac7685b7a00e6211f4094.png" width="690" height="431"><img src="/uploads/db1493/original/3X/3/a/3a8dd6860edc12f54d567ddf84fbd9969df67001.png" width="690" height="431"><img src="/uploads/db1493/original/3X/2/3/23d12900e8196507e9f201daf096a2e39c953171.png" width="690" height="431"><img src="/uploads/db1493/original/3X/4/d/4d83bf5707b9a439d05e96f177f5ad695e8d2984.png" width="690" height="431"><img src="/uploads/db1493/original/3X/0/b/0b262686206154230c147c86c4e4a88ae44e8bcf.png" width="690" height="431">

im using an enertion vesc with a 200kv chaka motor and two 5s 18.5 v 4000mah 15c batteries
```

---
## \#19 Posted by: elkick Posted at: 2016-09-14T16:40:30.168Z Reads: 42

```
You are having the max current ramp step error, described here: http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262

Enertion seems to have sent out a ton of VESC with that error.

Also, better set the value of the "max input voltage" in the motor tab back to the default value of 57V (it's 42V currently, which might kick in if you are having voltage spikes).
```

---
## \#20 Posted by: ecuadorche Posted at: 2016-09-14T17:09:11.591Z Reads: 43

```
hmm ill be sure to update my vesc then any other tips???
```

---
## \#21 Posted by: chewydinosaurs Posted at: 2017-01-17T04:38:29.875Z Reads: 28

```
Ive got the same issue but with a vesc (I got last week) from ?
```

---
