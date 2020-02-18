# Trouble shooting dead board

### Replies: 9 Views: 526

## \#1 Posted by: christopherindenver Posted at: 2017-02-12T18:59:51.638Z Reads: 64

```
Took board to Discovery Park, rode for 20 min from 41.7v to 36.6v and then it kinda died on me. One wheel turns very slowly, the other not at all. No water abuse, very little dust/dirt. What happened?
```

---
## \#2 Posted by: Alextech Posted at: 2017-02-12T19:02:42.631Z Reads: 62

```
Hey man we are going to need alot More details, what board? What conditions were you riding in? Was there any water damage? Ect
```

---
## \#3 Posted by: christopherindenver Posted at: 2017-02-12T19:55:30.558Z Reads: 57

```
Sorry, it's a standard Trampa deck with Scram build; 10s, dual vsec, dual motor. Seems Right motor runs at 1:10 speed, left not at all. Last run was in Dry conditions, but medium use on dirt, asphalt, and grass.

Cycled, no change. Charged, no change. Wished for miracle, no change.
```

---
## \#4 Posted by: Alextech Posted at: 2017-02-12T21:38:33.338Z Reads: 49

```
Are you using 18650s? Bms? If you are chances are one of your spot welds failed.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-02-12T21:40:44.000Z Reads: 47

```
Also post your vesc settings.
```

---
## \#6 Posted by: Eboosted Posted at: 2017-02-12T23:00:05.846Z Reads: 40

```
Here arethe stps you should follow:

1. Take the enclosure out
2. Check for disconnected/torn wires
3. Measure the input voltage at the VESC
4. Mesaure the input voltaje after the switch
5. Mesaure the out voltaje ditectly from the battery
6. Check if both of your VESC have a solid blue led
7. Run motor detection on both VESCs and check if the motors spin
8. Go to tereminal type "faults"
9. Check the voltage of each individual pack
10. Check if you have good PPM signal on BLDC tool
```

---
## \#7 Posted by: christopherindenver Posted at: 2017-02-20T22:47:42.248Z Reads: 23

```
 your analysis of the situation is astute, but in fact it was simply  a loose connector on one of the motors.
```

---
## \#8 Posted by: Alextech Posted at: 2017-02-20T22:49:44.832Z Reads: 23

```
Odd, If it was just a issue on one of the motors, suprised that it killed power to both.
```

---
## \#9 Posted by: christopherindenver Posted at: 2017-02-20T22:50:04.148Z Reads: 22

```
Ok, for the record, nothing went wrong with the Scram build. Totally my fault for not seeing a loose cable connection. Rookie move.
```

---
