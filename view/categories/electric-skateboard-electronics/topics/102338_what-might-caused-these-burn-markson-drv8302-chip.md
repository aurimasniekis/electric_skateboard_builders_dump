# What might caused these Burn markson drv8302 chip

### Replies: 8 Views: 213

## \#1 Posted by: ciscotory Posted at: 2019-09-28T22:20:10.334Z Reads: 66

```
One of my Vesc's stopped working recently
Won't switch On it seems it's burnd out 🥺
Check it and found these Burns on drv8302 chip
want to know what might cus such burns? 
For future reference.. thanks

![sketch-1569705771743|690x476](upload://fEbiPySonms9ikWezMLtg257uSD.jpeg) ![sketch-1569705835628|326x500](upload://4jzhJzAkrjOCQpbVHje5rwbNRSI.jpeg)
```

---
## \#2 Posted by: Jansen Posted at: 2019-09-29T07:02:07.511Z Reads: 48

```
Interested cause I just got back from a ride and towards the end I got a DRV8302 fault and have noses what is. Also got an under voltage one as well when battery has been working just fine and taken good care of working great day/night before.  Not sure if it’s a VESC or a battery issue though. Will wait to see what you find out and others say. Going to open my enclosure when I get home to see if I have burn marks.
```

---
## \#3 Posted by: nickw1881 Posted at: 2019-09-29T19:01:32.833Z Reads: 41

```
What voltage you running?
```

---
## \#4 Posted by: louwii Posted at: 2019-09-30T02:43:06.698Z Reads: 31

```
DRV fault (DRV burning out) is actually quite common. There are a few people on this forum that can replace the DRV. I think @JohnnyMeduse?
```

---
## \#5 Posted by: KevinH Posted at: 2019-09-30T03:26:05.640Z Reads: 27

```
louwii do you work for enertion?  Will they replace this under warranty?
```

---
## \#6 Posted by: louwii Posted at: 2019-10-02T05:58:44.342Z Reads: 19

```
I don't work for them. I don't think they'll replace it under warranty, as most of the time it's due to ''user error" (wrong settings and whatnot).
```

---
## \#7 Posted by: nickw1881 Posted at: 2019-10-02T08:11:58.654Z Reads: 16

```
I've burned out a bunch of them. It's the gate drive linear regulator inside the DRV that fails most often (for me) and leaves exactly that mark. TI used a linear regulator for the gate drive power supply, which is very inefficient at 12s.

I wouldn't call this a user error or settings error. It's more of an issue with the VESC hw design. DRV830x is designed for running fans in server racks, not 2kW skateboard motors.

Maybe try and run the switches as slow as possible, that reduces the load on the gate drive power regulator. 20kHz seems to keep it from failing. 

Unfortunately unless you or a friend have a microscope and a heat gun, that VESC is fried.
```

---
## \#8 Posted by: ciscotory Posted at: 2019-10-20T17:44:22.758Z Reads: 13

```
the battarey im suing in 10s3p with 36V
```

---
