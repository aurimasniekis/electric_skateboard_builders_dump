# Four Vesc canbus wiring diagram

### Replies: 13 Views: 468

## \#1 Posted by: toma Posted at: 2018-11-07T03:33:28.420Z Reads: 101

```
Could someone please providing me with a wiring diagram on how I can connect four vescs? @chaka  Is this something u can help me with?

**Is this correct?**
![F_Modules-11%20(2)|690x471](upload://rXz6Nge9EMDxE07dwflSbQ9SiRy.png) 

**TEMPLATE:**
![F_Modules-11%20(1)|690x471](upload://42QRiRPulkFGVIpoDhqW3je7YNq.png)
```

---
## \#2 Posted by: chaka Posted at: 2018-11-07T03:47:37.348Z Reads: 88

```
No don't do that. You want all the CANH pins to be connected together in parrallel same goes for the CANL. Also make sure you make your canbus connections after you finish you main power connections. If you have the canbus harness connected and only power one VESC you will pop the can transceiver and possibly the stm chip.
```

---
## \#3 Posted by: Blacksheep Posted at: 2018-11-07T03:52:27.748Z Reads: 86

```
Could you make a diagram ?
```

---
## \#4 Posted by: BensonYong Posted at: 2018-11-07T04:05:51.487Z Reads: 83

```
![F_Modules-11%20(1)|690x471](upload://mEz2qJtHcils4P2oVBsDRQo0DZ2.jpeg) 
Hope can help you.
```

---
## \#5 Posted by: chaka Posted at: 2018-11-07T04:07:06.599Z Reads: 78

```
@BensonYong beat me to it but here it is anyway ;) 

![canbusquad1|690x471](upload://xkMx1PJp8rGNoxaheUo0hwFLVkB.png)
```

---
## \#6 Posted by: Arzamenable Posted at: 2018-11-07T04:07:13.835Z Reads: 74

```
But also like the dating scene, length matters! The lengths and twists matter. Drv wizard and my smoked motor controllers agree.
```

---
## \#7 Posted by: Arzamenable Posted at: 2018-11-07T04:07:37.075Z Reads: 70

```
I split ppm to dual can x2.
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-11-07T05:09:10.263Z Reads: 63

```
![20181107_160724|690x470](upload://uQwJRc9r8Iv6x6vQ846KIqbAV41.png)
you want each vesc in parallel. so vesc 1 can L to vesc 2 can L to vesc 3 can L to vesc 4 can L
Then
vesc 1 can R vesc 2 can R vesc 3 can R vesc 4 can R
daisy chain em essentially
```

---
## \#9 Posted by: ARetardedPillow Posted at: 2018-11-07T05:14:58.742Z Reads: 55

```
The more the merrier ![image|690x484](upload://7OuX4P4ci84n0ayq4tN0CTgN95i.png)
```

---
## \#10 Posted by: lrdesigns Posted at: 2018-11-07T05:40:29.320Z Reads: 47

```
![image|690x489](upload://b7s9M1reFU3k5boyrPnaDcv5LP.png)
```

---
## \#11 Posted by: ARetardedPillow Posted at: 2018-11-07T05:55:58.410Z Reads: 48

```
![image|690x454](upload://dk8RV08txeJgn300R9zPBvzz8mh.jpeg)
```

---
## \#12 Posted by: xilw3r Posted at: 2018-11-07T06:48:41.270Z Reads: 46

```
U TRIGGER ME WITH THAT
lol
```

---
## \#13 Posted by: mmaner Posted at: 2018-11-07T19:29:59.349Z Reads: 36

```
![image|690x387](upload://nOsrviz4MSYICbLPVZeuX9tmRy8.jpeg)
```

---
