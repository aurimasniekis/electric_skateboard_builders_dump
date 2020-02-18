# Busted 3 Vesc tonight - swear log

### Replies: 6 Views: 1547

## \#1 Posted by: Blasto Posted at: 2016-05-05T04:26:04.822Z Reads: 163

```
So i keep busting my slave vesc on my dual build

http://www.electric-skateboard.builders/t/the-troll-enertion-cf-deck-dual-tbs-6355-sensor-10s-build-completed/1491/16
Installed and busted the slave 3 times.
All three vesc were freshly repaired, thinking that they were not actually repaired made me simply swap them out then i would bust the next one... A little stupid of me but i had my dough's

I'm not asking for any help here, just logging the info.

All three had the same behavior, they work fine when working alone configured as master. When i set them up as a slave, both motors work fine for about 1minute then the slave drv will blow out of nowhere.

So here my actions i will take in hopes of isolating the problem:
-replace the old crusty 3300uf caps that i got in a sketchy electronic shop with new ones
-disable the traction control
-run the motors in sensorless mode (currently sensored)
-replace the new 3300uf caps ( if it doesnt work) with 6 680uf caps(like the capacitor boards)

I'm open to other actions to take, but like i said, i'm just logging what i'm doing.
```

---
## \#2 Posted by: willpark16 Posted at: 2016-05-05T04:59:41.875Z Reads: 153

```
enertion, chaka, or torqueboards vesc?
```

---
## \#3 Posted by: DougM Posted at: 2016-05-05T15:29:16.018Z Reads: 113

```
For my short failed stint with a dual motor board I ran them in chained serial.  Not sure it makes any difference, but it might be give you some debugging data points.

Tie the TX line to both VESC's, but of course the RX line only comes back from one.

I do think that bigger caps might help - that jolt on first start is likely what caused my failure.  Both motors started at exactly the same time.  Next time I'm going to run separate serial channels and add a slight delay to one of the motor starts.

DougM
```

---
## \#4 Posted by: chaka Posted at: 2016-05-05T15:50:31.365Z Reads: 106

```
Not mine, those look like they are from modified gerber files. Why did you move C29 @Blasto?
```

---
## \#5 Posted by: Blasto Posted at: 2016-05-05T15:54:42.497Z Reads: 104

```
OCD, i like having the components lined up. All the boards had that extra 2.2uf on gvdd.

The same thing happened with a production vesc. I'm almost tempted to put a tvs across the bulk caps.
```

---
## \#6 Posted by: Blasto Posted at: 2016-05-09T03:21:45.958Z Reads: 76

```
Out with the old caps

<img src="/uploads/db1493/original/2X/3/3ecf618774be1fefe69352ddefde18523a99558d.jpeg" width="666" height="500">

In with the new

<img src="/uploads/db1493/original/2X/9/95129b38d94d120fc308e3c14bc0a2ff681624b1.jpeg" width="375" height="500">

No blowage on the bench, good sign. the other 3 vesc blew 30sec into bench testing.

I'll try to get my hands on a multimeter that is able to measure capacitance. Then i'll be 100% sure my problem was the caps.
```

---
