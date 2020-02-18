# DRV8302 and Under Voltage error - works after reboot. What is wrong?

### Replies: 6 Views: 696

## \#1 Posted by: oyta Posted at: 2017-09-01T22:11:45.204Z Reads: 70

```
I am struggling with an DRV8302 Under Voltage error. It happens whenever I am pushing the throttle quite hard. When the error occurs the VESC normally shuts down and I need to restart my board - then it works fine again. On some occations I react fast and break as soon as I notice the voltage drop and then the VESC stays on I can continue riding. You see a lot of these small voltage drops in the log. 

Some background info:

* See my build thread: http://www.electric-skateboard.builders/t/portable-custom-birch-fiber-glass-enertion-trucks-6355-190-kv-enertion-motor-mount-10s3p-lg-hg2-vesc-6-beta/26397
  * 10s3p LiIon with LG HG2 batteries
  * 190 KV enertion r-spec pro motor
 * 15-36 pulleys
 * VESC 6 beta 
* VESC-Tool Motor settings: https://www.dropbox.com/s/1usvf12bqc9b8io/Skjermbilde%202017-09-01%2020.41.47.png?dl=0
* VESC-Tool FOC settings: https://www.dropbox.com/s/mdyz3ooikcqv150/Skjermbilde%202017-09-01%2020.42.27.png?dl=0
* VESC-Tool PPM settings: https://www.dropbox.com/s/10rbahky2alqrrl/Skjermbilde%202017-09-01%2020.43.24.png?dl=0
* BMS configuration: https://www.dropbox.com/s/9kvxxaluf6n2t94/Skjermbilde%202017-09-01%2020.45.27.png?dl=0
 * You can see the errors clearly in the log. At least at about these timestamps: 19:23:58, 19:39:47, 19:43:17, 20:04:31.

Obs! When the problem first occured I had different VESC-Tool motor controller settings: https://www.dropbox.com/s/sykoecdbjsii98q/Skjermbilde%202017-09-01%2021.01.39.png?dl=0 The motor controller settings in the last post were used for the recorded drive (metr.at log).

What could be wrong? Is it a short? Or is it the setup? Is the BMS funky? Why does it work immidiatly afterwards/after a reboot?

My drive log: https://metr.at/r/KX1ng
https://metr.at/r/KX1ng
```

---
## \#2 Posted by: Lionpuncher Posted at: 2017-09-26T00:56:27.018Z Reads: 51

```
Nobody replied? Having the same issue. Did you ever get this sorted?
```

---
## \#3 Posted by: oyta Posted at: 2017-09-26T06:20:45.889Z Reads: 46

```
Hi! I have concluded that the BMS turns itself off. It is rated for the amps and it did function correctly earlier. However it looks like the  voltage goes down to a level where it is off. Unfortunately I have not has the time to look at it. It may be a short. I need to check the wiring and take the heatshrink off to see if there are any contaminat(?) that makes the short. It may also be the softswitch. I will post the solution here but it will take some weeks before I can analyse it 😕.
```

---
## \#4 Posted by: Martinsp Posted at: 2017-09-26T08:53:50.034Z Reads: 42

```
This has happened to me where the bms would turn of but in my case it was the balance lead that became unplugged. Check that and an easy way to check if it is the bms is simply bypass it, if the problem remains it is something else.

Check the details of your bms because it might be hitting some kind of limit. Maybe current or low voltage of one cell or something else.
```

---
## \#5 Posted by: oyta Posted at: 2017-09-26T16:03:16.994Z Reads: 37

```
Thanks. I will check the balance wires.
```

---
## \#6 Posted by: Deckoz Posted at: 2017-09-27T00:59:59.567Z Reads: 31

```
So this was my buddies issue similar things...

https://www.electric-skateboard.builders/t/over-voltage-fault-stuttering/33973/11
```

---
