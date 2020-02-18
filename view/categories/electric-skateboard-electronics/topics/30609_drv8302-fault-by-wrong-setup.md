# DRV8302 fault by wrong setup?

### Replies: 7 Views: 511

## \#1 Posted by: Maxx Posted at: 2017-08-14T17:49:42.098Z Reads: 68

```
Hey
so I finished [my build](https://www.electric-skateboard.builders/t/my-first-build-orangatang-80mm-turnigy-6363-245kv-esk8-mount-diy-10s2p-diy-vesc/13376) with some modifications to the original post. For the battery I used two Turnigy 5S1P 1300mAh Graphene Lipos in series and and bought a complete VESC 4.12.

I did the motor measurements with a 15V power supply some time ago before I got the battery so I plugged in a rc remote for testing and spun the motors after setting up the remote. After spinning them for 10s without any load I tried it again and it didn´t work. DRV8302 fault :confused:

Any important settings to make the VESC work with my new DRV chip and 10S 245kv setup?

Max
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-08-14T17:59:32.214Z Reads: 66

```
Here is what i found out, for first turning up u need 12v not 15v or 3s batt.
motor detection, u need to connect the battery u will use. different amp and voltage result different values on motor. which can drv fault happens.

and I dont know which 4.12  u use but if it's firmware 2.18 it may has current ramping bug under advance section.  default is 0.04 if goes over like 0.4 it can fry  it too.

hope it helps
```

---
## \#3 Posted by: Namasaki Posted at: 2017-08-16T19:01:22.537Z Reads: 47

```
Vesc 4.12 ERPM safe limit is 60k
With 245kv motor and 42v (10s) your no load ERPM would be 72k
Exceeding the ERPM limit can cause DRV fault
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-16T19:05:33.004Z Reads: 44

```
Yea.. I think that's what caused it too
```

---
## \#5 Posted by: Maxx Posted at: 2017-08-19T19:54:27.002Z Reads: 35

```
So setting a limit on the erpm should solve this?
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-08-19T20:11:40.144Z Reads: 34

```
well, drvfault is permanent damage, so you have to replace. try flashing firmware it might work again.
```

---
## \#7 Posted by: Maxx Posted at: 2017-08-22T13:48:45.072Z Reads: 26

```
Yea so I replaced the chip.
Setting a erpm limit and then doing the motor measurements should work right?
```

---
