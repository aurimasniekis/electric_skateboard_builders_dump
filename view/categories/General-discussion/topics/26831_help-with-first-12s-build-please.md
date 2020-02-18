# Help with first 12s build please!?

### Replies: 8 Views: 662

## \#1 Posted by: Bh59 Posted at: 2017-07-05T10:39:55.569Z Reads: 73

```
hi all, wanting to run 2 6s batteries have done a lot of research, wanting to know if this charging diagram will damage the vesc at all seeings it doesn't really disconnect? also any help on where to find a 12s voltmeter?
current build specs are:
2x 5500mah 6s 70c screamin batteries
192kv 6374 sk3
vesc
nano remote
calibre 44's
90mm flywheels
prism origin deck
torqueboards mount and pulley system 13t or 16t motor / 36t wheel<img src="/uploads/db1493/original/3X/f/e/fe1b56fe2ffe609d72424641819a35488ffcde25.png" width="479" height="500">
```

---
## \#2 Posted by: Bh59 Posted at: 2017-07-05T10:40:47.981Z Reads: 67

```
any vesc settings will also be greatly appreciated :beer:
```

---
## \#3 Posted by: pat.speed Posted at: 2017-07-05T11:19:58.360Z Reads: 62

```
Yes that should work. Do you have to 6s chargers? Also check with someone more experienced just to make sure
```

---
## \#4 Posted by: Bh59 Posted at: 2017-07-05T13:29:38.356Z Reads: 55

```
Sky Rc duo charger
```

---
## \#5 Posted by: Decdog Posted at: 2017-07-05T14:37:35.792Z Reads: 46

```
With 36-16 gearing, your top speed(unweighted) would almost be 40 mph according to this: http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":192,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":90}|
```

---
## \#6 Posted by: sl33py Posted at: 2017-07-05T16:01:09.641Z Reads: 42

```
with the 90mm wheels - i'd suggest the 13/40 gears to keep speeds more reasonable.  Will help with acceleration and hills too.

Looks like a solid plan!  GL!
```

---
## \#7 Posted by: Bh59 Posted at: 2017-07-10T22:36:37.329Z Reads: 22

```
Board is running good and is scary fast, can anyone help me as I want to wire in a voltmeter and headlights to my boards, my question would be can you wire in a 6s BEC to a 12s system?
Also if anyone has anything on me being able to charge both batteries at the same time using a duo charger without damaging vest if it's still connected to one positive and one negative between 2 batteries
```

---
## \#8 Posted by: sl33py Posted at: 2017-07-10T22:58:24.410Z Reads: 22

```
No.  **You need a BEC that can handle 12s/50.4v** - and i'd look for 12v out if you want LED lighting.  Or 5v and look for 5v LEDs.  The brighter and inexpensive LEDs are typically 12v.

Also No on the charger - unless you disconnect them from being in series and charge each on it's own channel as 6s.

You can look at the Thunderpower 1220:
http://www.hobbypartz.com/75p-1220-charger.html

I have one and it works fine, but nothing special except it'll charge to 12s.

GL!
```

---
