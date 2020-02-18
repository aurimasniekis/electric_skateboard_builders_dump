# Help! programming new turnigy motors

### Replies: 23 Views: 422

## \#1 Posted by: Jcammarata4 Posted at: 2019-05-07T16:00:32.576Z Reads: 102

```
i have replaced my scramboards motors with turnigy 6374 149kv motors. i am first time vesc program user. i used the wizard...seems to have worked but i am not sure the motors are not responding consistantly.....can someone walk me through simply....i am great with computers but new to programming motors...i think somethings off sometimes one motor spins up and the other wont...then they both work ...then not.....i am sure i have missed something please help...need to ride been off the trails for 2 weeks now....
```

---
## \#2 Posted by: sk8l8r Posted at: 2019-05-07T16:05:48.492Z Reads: 99

```
The very first thing when you type 'vesc' in search 

https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#3 Posted by: Grozniy Posted at: 2019-05-07T16:11:34.360Z Reads: 90

```
https://www.electric-skateboard.builders/t/wiki-a-beginner-guide-to-diy-an-esk8/46844/16?u=grozniy
```

---
## \#4 Posted by: Jcammarata4 Posted at: 2019-05-07T17:47:08.175Z Reads: 76

```
thats for an older program and is on an apple computer. i have the newer program version which is not the same.
```

---
## \#5 Posted by: linsus Posted at: 2019-05-07T17:51:26.373Z Reads: 77

```
point is, use the freaking search function, two weeks off the road. didint even spend 2 seconds searching...
```

---
## \#6 Posted by: Jcammarata4 Posted at: 2019-05-07T19:18:53.907Z Reads: 71

```
of course i did a search and you werent replying to what the question actually was....did all the necessary work first, the issue is after the programming has been done i still seem to have an issue. but thanks
```

---
## \#7 Posted by: Jcammarata4 Posted at: 2019-05-07T19:20:56.623Z Reads: 68

```
why respond if you dont give a**** just ignore it and troll on.....
```

---
## \#8 Posted by: Arzamenable Posted at: 2019-05-07T19:23:25.186Z Reads: 63

```
If one motor will spin and the other won’t, unselect “traction control “

Then see if they spin the same way. If not change so they do.
```

---
## \#9 Posted by: Jcammarata4 Posted at: 2019-05-07T19:26:22.068Z Reads: 62

```
thats not checked i looked....its not constant like it kinda wants to spin then does....then wont...the physical connections are all good. i got some gut feeling its some setting though thanks for the suggestion
```

---
## \#10 Posted by: Jcammarata4 Posted at: 2019-05-07T19:27:09.259Z Reads: 60

```
any more suggestions are welcome thanks
```

---
## \#11 Posted by: mynamesmatt Posted at: 2019-05-07T19:32:16.961Z Reads: 57

```
are they sk8s? have you set up hall sensors correctly? is it on bldc? hybrid bldc? foc? has the remote been properly configured?
```

---
## \#12 Posted by: Jcammarata4 Posted at: 2019-05-07T19:49:27.023Z Reads: 54

```
Ok the remote is set up correctly and working the motors are aerodrive 6374 149kv ...sensorless.
```

---
## \#13 Posted by: Jcammarata4 Posted at: 2019-05-07T19:51:19.121Z Reads: 55

```
And set up via the wizard tool. So I feel there's other settings not set correctly...I'm just trying to figure out if the wizard will do just the bare minimum and there are more things I need to apply
```

---
## \#14 Posted by: Halbj613 Posted at: 2019-05-07T21:24:24.558Z Reads: 51

```
Can you send a video of the setting so and what the motors are doing
```

---
## \#15 Posted by: Jcammarata4 Posted at: 2019-05-07T22:44:18.289Z Reads: 47

```
I am going to set that up and try to record and post it ...good idea. Maybe it's been seen before.....will do that asap
```

---
## \#16 Posted by: Jcammarata4 Posted at: 2019-05-08T05:00:51.354Z Reads: 46

```
Here is a video of what's happening. 

https://www.instagram.com/p/BxMGBDVFwec/?utm_source=ig_share_sheet&igshid=hl4m1yfka47g
 
It's 1 minute long but the issue happens about 4 or 5 times.....
```

---
## \#17 Posted by: Andy87 Posted at: 2019-05-08T05:33:06.763Z Reads: 42

```
Did you set them up in FOC or bldc?

Also, did you try to redo the motor detection on the motor which sometimes not running?
```

---
## \#18 Posted by: Jcammarata4 Posted at: 2019-05-08T13:29:30.434Z Reads: 32

```
I used the wizard. It's setup in foc I didn't think there was an option either way in the wizard. So wizards ran and we're all finished and green lit. I did this more than once to be sure it was all done and saved.
```

---
## \#19 Posted by: Jcammarata4 Posted at: 2019-05-08T13:31:55.702Z Reads: 33

```
When it does the detection it seems to only use one motor for detection then after that both spin up ..is that right or should it spin one up...then the other.....seems to dial one in then send info to can bus and then both work??
```

---
## \#20 Posted by: Andy87 Posted at: 2019-05-08T13:42:03.624Z Reads: 30

```
There should be one motor detection run for each motor. If you made that only for the master, than we found your issue. Is the faulty motor controller by the master or the slave vesc?
```

---
## \#21 Posted by: Jcammarata4 Posted at: 2019-05-08T16:27:33.133Z Reads: 21

```
ok so i run motor detect and it picks up one motor goes thru its paces and its done. how do i get second motor to register...meaning do i actually move the usb to the second vesc and then run program again....or does it see motor via can bus and i need to see how to do that??
```

---
## \#22 Posted by: linsus Posted at: 2019-05-08T16:41:41.419Z Reads: 21

```
loosen the tension, the motorshafts looks like theyre at an unhealthy angle, taking burden, either the mounts are flexing(weak mounts) or they're not aligned properly. Truck axle and motor shaft should be as parallell with eachother.

Regarding the spinning, remove the belts entirely. Do they still behave the same? The drag koefficient from the belts to pulleys wont be exactly the same obv. between the two motors.
```

---
## \#23 Posted by: Andy87 Posted at: 2019-05-09T00:05:39.077Z Reads: 13

```
You can do it via CAN bus by clicking the can forward button on the right side, or just plug in the usb in the other esc. Just make sure you go in both esc through motor and input wizard. Yes also input wizard as you need to set the slave to slave. It’s just one click, but important to do.
```

---
