# Wheel slipping (Single drive)

### Replies: 8 Views: 170

## \#1 Posted by: Superflim Posted at: 2019-05-07T15:31:11.311Z Reads: 67

```
Hi fellow esk8 builders,

Lately my wheels have been slipping a lot. During hard acceleration and braking at low speeds.
I remember a time when I adjusted my acceleration curve and motor amps so it wouldn't slip, and it never did. I changed these settings with the mobile app. After finding out my ideal settings I went and changed these in the vesc standard settings, and this was when my wheels started slipping again. I've tried changing to my ideal settings using the app again, it did not work. Maybe because my wheels have slipped a lot, it lost grip? Or is this a silly thought? 

My settings are:
70A motor
-32A motor

30A bat
-12A bat
```

---
## \#2 Posted by: rusins Posted at: 2019-05-07T15:34:14.975Z Reads: 68

```
That certainly is a lot of amps to the motor. Got any pictures of the wheel? You could just swap left and right or front and rear.
```

---
## \#3 Posted by: mmaner Posted at: 2019-05-07T15:34:41.652Z Reads: 68

```
Is the belt slipping in the pulley or the wheel slipping in the road?  What's the throttle curve values currently?
```

---
## \#4 Posted by: Superflim Posted at: 2019-05-07T15:40:57.389Z Reads: 61

```
I'm pretty sure it's wheel slipping on the road. Otherwise my belt would have been obliterated by now :sweat_smile:

Curve is at 
-28% Acc
-35% Brake
Expo-natural
```

---
## \#5 Posted by: Superflim Posted at: 2019-05-07T15:42:09.058Z Reads: 58

```
![15572436997682737189545521424666|375x500](upload://eOjzOGmq7MUCtOxRYD8VUmq6KtP.jpeg)
```

---
## \#6 Posted by: mmaner Posted at: 2019-05-07T15:44:36.075Z Reads: 56

```
That's a liberal curve, you should be good. I'd lower the motor amps to 60 and the curve to -22/-26, test and see how it performs.
```

---
## \#7 Posted by: Superflim Posted at: 2019-05-07T15:45:49.064Z Reads: 54

```
And also lower brake amps?

Because at braking I find it the most annoying. I don't mind slightly less acceleration
```

---
## \#8 Posted by: mmaner Posted at: 2019-05-07T15:59:08.514Z Reads: 44

```
Yeah, you'll just have to experiment. Maybe some lower during wheels.
```

---
