# Problems with Braking Focbox

### Replies: 8 Views: 517

## \#1 Posted by: Benjamin899 Posted at: 2018-05-15T21:05:20.307Z Reads: 114

```
Hi guys,

i have problem, that is my braking isn't as strong as i want them to be. So my Question is what i can do to change that or if that is just it. FYI i have a Focbox and before that an APS 120a RC ESC which had strong brakes.
I am currently using Ackmaniacs Tool.
Motor: sk3 6364 245kv
Battery: 6s1p 5AH Zippy Lipo 
Reduction: 15:40 and 97mm wheels
These are my motor settings.
![motor3|690x152](upload://wdV1aN0tjJ4kKpX1tEaVrHN2zTn.JPG)![motor4|690x427](upload://2aZpPKio16dLZNBZDE5DTL82091.JPG)![motor2|690x423](upload://t976IKf4jvlJP5O6ZV3Cqq4viCn.JPG)![Motor|690x422](upload://kietCGrX2ytMp1PGCfRsoqThoCe.JPG)
Here my App Settings.
![app2|690x269](upload://abI6rpecyL7uP2CFbKF6qpDD1sn.JPG)![app3|690x429](upload://bvjRUIuwRQZy32GvhXDYEAKGBqX.JPG)![app1|690x261](upload://uD02IjtDdtqUOKYn3g5j1U8sg6J.JPG)
```

---
## \#2 Posted by: Scoo_B_SK8 Posted at: 2018-05-15T21:10:24.715Z Reads: 89

```
“Motor current Max Brake”
```

---
## \#3 Posted by: Benjamin899 Posted at: 2018-05-15T21:12:56.034Z Reads: 90

```
what about it? Do i have to lower it? Do i have to keep it under 50A since that is what the focbox can handle continiously? I dont want to fry it
```

---
## \#4 Posted by: FredrikHems Posted at: 2018-05-15T21:15:46.095Z Reads: 92

```
Your lipos can most likely handle 2C charge rate. If thats the case, then you can lower your batt max regen to -10.
```

---
## \#5 Posted by: Benjamin899 Posted at: 2018-05-15T21:20:23.300Z Reads: 87

```
damn you are right, i always thought they were only 1c. So the Motor Current Max Brake is playing second fiddle?
```

---
## \#6 Posted by: Battosaii Posted at: 2018-05-15T21:39:03.116Z Reads: 75

```
Raise the -max motor amps I run mine at -65a and i like the brakes you will not damage the focbox it can handle up to 50a battery amps continuously the motor amps are different.
```

---
## \#7 Posted by: Ackmaniac Posted at: 2018-05-15T22:10:03.420Z Reads: 64

```
It's as simple as that
"Motor Current Max Brake" is for total brake strength and especially for mid and slow speed
"Battery Current Max Regen" is for brake power at high speed.

But in your case -5A for "Battery Current Max Regen" will limit the brake power at nearly all speeds because it is too low.
If you Battetry can officially handle 2C charge current (5Ah * 2 time capacity = 10A) you can set it to 10A. But even that is a bit low. I recommend to go even 50% higher than that because to my experience these max charge current ratings are only for continuous charge and not for short bursts which take mostly not longer than 5 seconds.
So even 15A shouldn't harm your battery.

And when you think about it, your APS 120a RC ESC didn't give a fuck about any max charge currents specs.
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-05-15T22:47:23.894Z Reads: 55

```
ok thanks for elaborating
```

---
