# Throttle Curve Not Affecting Nano X Breaking

### Replies: 10 Views: 245

## \#1 Posted by: ToucanSam Posted at: 2018-08-16T00:02:55.192Z Reads: 85

```
Okay so I have the TorqueBoards Nano X remote.

I have set the Throttle Expo and Throttle Break Expo to -100%, natural. The following is a picture of what it looks like in the VESC Tool.

[My PPM Throttle Curve](https://imgur.com/a/prnk7CB)

This gives me a nice smooth and easy accel on the low end but its still nice and powerful on the high end. Its a nice accel curve for me. My problem is that no matter what I do the breaking is instantly 100% break the second you hit 16% on the remote. No matter what I set the curve to the breaking is instantly locking the wheels.

Once I set the Throttle Break Expo to -100% natural to match the accel and on the bench I actually got a nice smooth break and it was perfect, but the second I saved the config and disconnected the VESC and restarted the board It went straight back to instant 100% break no smooth no curve no nothing.

Can anyone provide any insight on how to get a smooth break experience with the most recent VESC Tool and the Nano X remote?
```

---
## \#2 Posted by: PartyPoison Posted at: 2018-08-16T03:16:06.495Z Reads: 72

```
Have you tried to 
Turn on the remote 
Push all the way up
Push all the way down
Then turn in the board?
```

---
## \#3 Posted by: ToucanSam Posted at: 2018-08-16T03:45:57.204Z Reads: 64

```
I read about all the calibrating stuff and yes I tried it and it didn't change anything that I could tell
```

---
## \#4 Posted by: Blasto Posted at: 2018-08-16T04:10:23.278Z Reads: 61

```
Are you testing this out on the bench or actualy toad testing?
```

---
## \#5 Posted by: ToucanSam Posted at: 2018-08-16T04:45:59.163Z Reads: 54

```
Both, on the bench and off i cant seem to get a smooth brake. But Ill make changes and test both every iteration.
```

---
## \#6 Posted by: PartyPoison Posted at: 2018-08-16T04:48:51.940Z Reads: 54

```
That happened to me before,  i redo all my vesc settings and forget the throttle curve.
```

---
## \#7 Posted by: Blasto Posted at: 2018-08-16T04:50:39.638Z Reads: 53

```
Ok, then my next guess is you motor max settings are a bit high (which is fine) 

Another thing you can try is put a really exagerated curve
```

---
## \#8 Posted by: ToucanSam Posted at: 2018-08-16T05:10:40.969Z Reads: 45

```
i'm using as exaggerated of a curve as i can but the -100% expo does feel any different than the 0% expo, so somethin' ain't right. The graphs look entirely different but don't seem to make a difference.
```

---
## \#9 Posted by: Sender Posted at: 2018-08-16T12:49:04.484Z Reads: 37

```
What are your motor and battery mins?
```

---
## \#10 Posted by: ToucanSam Posted at: 2018-08-17T03:41:21.509Z Reads: 31

```
Both motors are set to -60 min 60 max. What is a battery min?
```

---
