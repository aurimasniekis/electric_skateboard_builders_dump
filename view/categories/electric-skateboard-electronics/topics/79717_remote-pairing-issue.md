# Remote pairing issue

### Replies: 29 Views: 248

## \#1 Posted by: yanggatang Posted at: 2019-01-03T03:12:08.516Z Reads: 70

```
When I tried pairing the remote to the master vesc, the light signals that it has connected, but the motor won't turn. I had this same issue back when I was pairing my remote for a single motor, and I somehow fixed it(forgot how exactly maybe by adjusting motor settings?). I was wondering if yall could help me?

Here are the links to the videos for my vesc config and setup:
https://drive.google.com/open?id=1HzCoh9pN9zzI1l8hRwPSSNPrHrFXSyr3
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-01-03T03:15:22.661Z Reads: 62

```
Did you "write" your configs before disconnecting?
```

---
## \#3 Posted by: yanggatang Posted at: 2019-01-03T03:15:59.579Z Reads: 61

```
I saved it each time
```

---
## \#4 Posted by: J0ker3366 Posted at: 2019-01-03T03:19:39.454Z Reads: 58

```
So in your master input video you didn't set the parameters for the trigger.
```

---
## \#5 Posted by: J0ker3366 Posted at: 2019-01-03T03:21:47.353Z Reads: 59

```
When yoyou get here, you need to full throttle. Don't worry it won't turn the motors. So, full throttle then pull back to full brake. Then hit apply
![Screenshot_2019-01-02-20-20-25|281x500](upload://jtOd07XvhfsZdkxwu46BUInrljM.png)
```

---
## \#6 Posted by: tardyparty7 Posted at: 2019-01-03T03:39:13.281Z Reads: 51

```
i had the same thing!!!!!!! check the hall sensor, or whatever its called connecting remote to the vesc, and flip it. red should be to the left. i think.... did that make sense
```

---
## \#7 Posted by: J0ker3366 Posted at: 2019-01-03T03:57:13.621Z Reads: 49

```
lol PPM cable.
```

---
## \#8 Posted by: tardyparty7 Posted at: 2019-01-03T04:20:58.376Z Reads: 47

```
:upside_down_face:
```

---
## \#9 Posted by: yanggatang Posted at: 2019-01-03T05:12:39.329Z Reads: 44

```
Um, my ppm cable has the red line in the middle?
```

---
## \#10 Posted by: yanggatang Posted at: 2019-01-03T05:18:10.519Z Reads: 36

```
you my dude are a life saviour
```

---
## \#11 Posted by: yanggatang Posted at: 2019-01-03T05:18:42.476Z Reads: 36

```
thanks so much for helping me out!
```

---
## \#12 Posted by: J0ker3366 Posted at: 2019-01-03T05:27:40.603Z Reads: 35

```
Glad I could help. Stay safe
```

---
## \#13 Posted by: tardyparty7 Posted at: 2019-01-03T05:30:49.837Z Reads: 38

```
i haven't made a board since the summer and im tired...
```

---
## \#14 Posted by: yanggatang Posted at: 2019-01-03T05:32:43.792Z Reads: 37

```
sorry, one last question. I thought that after one motor runs with the controller that after connecting both vesc via canbus, both motors should work with the remote?
```

---
## \#15 Posted by: yanggatang Posted at: 2019-01-03T05:33:13.816Z Reads: 38

```
because right now, only one motor is turning when I flip the remote after connecting both vesc via canbus?
```

---
## \#16 Posted by: J0ker3366 Posted at: 2019-01-03T05:34:32.703Z Reads: 33

```
I'm not too familiar with canbus. @Andy87 @mmaner @Sender
```

---
## \#17 Posted by: yanggatang Posted at: 2019-01-03T05:41:15.890Z Reads: 32

```
do you reccommend using split ppm?
```

---
## \#18 Posted by: Andy87 Posted at: 2019-01-03T05:50:39.441Z Reads: 28

```
Did you set the second vesc as slave?
You need to configurate the second vesc too.
```

---
## \#19 Posted by: yanggatang Posted at: 2019-01-03T06:00:25.547Z Reads: 26

```
Yes, I set the second vesc as slave
```

---
## \#20 Posted by: Andy87 Posted at: 2019-01-03T06:02:04.312Z Reads: 25

```
You also made motor detection on the slave and still only one is responding when moving the trigger?
```

---
## \#21 Posted by: yanggatang Posted at: 2019-01-03T06:05:30.563Z Reads: 22

```
For the slave input setup, there wasn't the option to test the ppm brake and acceleration like on the master on the VESC tool.
```

---
## \#22 Posted by: yanggatang Posted at: 2019-01-03T06:12:53.570Z Reads: 22

```
heres the setup vid https://drive.google.com/drive/u/2/folders/1HzCoh9pN9zzI1l8hRwPSSNPrHrFXSyr3
```

---
## \#23 Posted by: Andy87 Posted at: 2019-01-03T06:37:10.696Z Reads: 22

```
Not the ppm. I speak about the motor wizard.
Did you go through it on the slave too?
Will have a look in the videos later. On the way to airport right now 😅
```

---
## \#24 Posted by: yanggatang Posted at: 2019-01-03T06:46:54.675Z Reads: 19

```
yeah, i went through the motor setup for the slave as well
```

---
## \#25 Posted by: Andy87 Posted at: 2019-01-03T07:41:39.687Z Reads: 18

```
Ok, two things that went wrong.
First is that the remote is not centered, but I think this you fixed already, right?
Second, I don’t see any CAN cable which connect the both vescs.
```

---
## \#26 Posted by: yanggatang Posted at: 2019-01-03T07:43:41.424Z Reads: 17

```
I have fixed the remote config and after that I connected the CAN cable when one motor worked
```

---
## \#27 Posted by: yanggatang Posted at: 2019-01-03T07:49:07.857Z Reads: 17

```
So currently the master motor works and the slave doesn't even when connected via canbus. Should i go split ppm?
```

---
## \#28 Posted by: Andy87 Posted at: 2019-01-03T08:28:17.797Z Reads: 18

```
The settings look right.
Did you try to do a new set up with CAN connected? Maybe some settings haven’t been saved out of a reason I don’t know 😅
If that’s not work, split ppm would be an option, but you need to setup both vescs as master than.
```

---
## \#29 Posted by: mmaner Posted at: 2019-01-03T12:59:00.743Z Reads: 19

```
You need to reboot both VESC's after the can bus cable is connected.
```

---
