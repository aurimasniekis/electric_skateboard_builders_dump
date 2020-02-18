# Motor stiff and grinding noise board not working PLEASE HELP

### Replies: 18 Views: 244

## \#1 Posted by: Halbj613 Posted at: 2019-04-14T19:21:15.791Z Reads: 62

```
Hi

I have 2 ollin gen 1 motors (5065)

I connected them up to a flipsky dual vesc and after connecting them up they make a weird sort of grinding noise and are extremely stiff around once every rotation (only for a small portion of the rotation)

I couldn’t see under a light any blockage

I tried using the board however it couldn’t anywhere near produce enough torque to even move me a couple of meters 

Please help

Here are some pictures![image|669x499](upload://enJuUxFum2FdS8q6LwoYdu1AdpY.jpeg) ![image|669x499](upload://1cjATMz3JK2reoEDaMNiUpkFTy6.jpeg) ![image|669x499](upload://vOeAC4wHY41hdKNqP693b2yvfhK.jpeg) ![image|669x499](upload://vQBOWCUyuzFN8mNMjH5zLjKfYR5.jpeg) ![image|669x499](upload://72OijIwhBAEjuKrrwl0299zoIqX.jpeg) ![image|669x499](upload://ge1qhfgpFyiDq2U8ZIIOT1Tj9fk.jpeg) ![image|669x499](upload://yhGs10pNgp9bQeLJPvKHrx5jqp.jpeg) ![image|669x499](upload://kT6NnKL8Zp2nCJbBiSk7zhSAQz2.jpeg) 

Why is this happening?

Thank you
```

---
## \#2 Posted by: SeanHacker Posted at: 2019-04-14T19:24:28.234Z Reads: 52

```
A video of the problem would really help out here. Also. Did you run motor detection? What settings? Ect...
```

---
## \#3 Posted by: Halbj613 Posted at: 2019-04-14T19:25:02.891Z Reads: 51

```
Will try and send
```

---
## \#4 Posted by: Halbj613 Posted at: 2019-04-14T19:31:40.315Z Reads: 50

```
Now one of he motors won’t turn and the other here is a picture of![image|669x499](upload://kT6NnKL8Zp2nCJbBiSk7zhSAQz2.jpeg)
```

---
## \#5 Posted by: Fraserrazor Posted at: 2019-04-14T19:51:48.695Z Reads: 45

```
Was the setup previously working with other motors aka have you done a successful motor detection and spin-up. It could be a broken magnet but you would have to open up the motor and send some pics.
```

---
## \#6 Posted by: Halbj613 Posted at: 2019-04-14T19:53:09.305Z Reads: 44

```
Dunno haven’t tried with any others I am getting some torqueboard 260kv ones on Tuesday though so will see then
```

---
## \#8 Posted by: Fraserrazor Posted at: 2019-04-14T20:00:09.329Z Reads: 44

```
gt2b is ppm and can be used with current and brakes with no reverse.
```

---
## \#9 Posted by: Fraserrazor Posted at: 2019-04-14T20:07:17.177Z Reads: 43

```
You can run ppm and uart
```

---
## \#10 Posted by: Fraserrazor Posted at: 2019-04-14T20:12:07.469Z Reads: 39

```
Just be careful that you acknowledge the current reverse switch on the gt2b remote before you mess with reverse setttings in the VESC  tool. If you don't mind swinging your board round on pivot to go backwardfs its easier to just run current with brakes no reverse. If you want the reverse function then you need to make sure the switch on the remote is forward and then code with current and model your pulsewidth to that, otherwise you can get problems where you switch direction and the throttle curve doesn't adjust and the board sends you onto your back. :+1:
```

---
## \#12 Posted by: b264 Posted at: 2019-04-14T21:03:00.844Z Reads: 35

```
Do the motors spin without being connected to anything?  (no wires or belts)

Did you hand-test the motors?

https://forum./t/how-to-hand-test-a-bldc-motor/568
```

---
## \#13 Posted by: Halbj613 Posted at: 2019-04-14T21:03:51.594Z Reads: 34

```
Without the belt on they are much better than with it on
```

---
## \#14 Posted by: Halbj613 Posted at: 2019-04-14T21:05:27.053Z Reads: 33

```
I am guessing it is a problem with the bldc settings or the belt taughtness
```

---
## \#15 Posted by: Halbj613 Posted at: 2019-04-14T21:06:11.070Z Reads: 32

```
[quote="b264, post:12, topic:90523"]
motors spin without being connected to anything? (no wires or belts)
[/quote]
Yes they do
```

---
## \#16 Posted by: b264 Posted at: 2019-04-14T21:10:17.804Z Reads: 28

```
What are the hand-test results?
```

---
## \#17 Posted by: b264 Posted at: 2019-04-14T21:10:27.538Z Reads: 29

```
Did you do motor detection?
```

---
## \#18 Posted by: Halbj613 Posted at: 2019-04-14T21:10:53.152Z Reads: 28

```
They are fine only very slight stiffness just due to age of the motors
```

---
## \#19 Posted by: b264 Posted at: 2019-04-14T21:18:58.290Z Reads: 26

```
How tight are the belts?  Do you have a photo of pushing on the belt with your finger?  It should deflect almost a full centimeter when you push on it.
```

---
## \#20 Posted by: Halbj613 Posted at: 2019-04-14T21:30:01.907Z Reads: 21

```
Hi think I found the problem the wheel pulley was rubbing on the motor mount tying to lubricate them both
```

---
