# Vesc 4.12 repair

### Replies: 8 Views: 181

## \#1 Posted by: g1tana Posted at: 2019-02-28T10:24:29.345Z Reads: 59

```
Hello everyone.

So im attempting to fix a vesc, i had sent my 6.6 to martin for repair and he done a great job and its back in the scooter pushing14s.

I had a couple of fs4.12 laying around but as they were only £45 it would made more sense to buy new 1's, so i decided to try and learn something by trying to fix myself.  With some advise from martin i picked the easiest 1 to do, change the fets.

Whilst i was waiting for the fets to arrive i decided to take some fets off of another to see if it would work. To my suprise it did work, kind of lol. When i would do a motor detection to spin motor, it would make a spark noise then nothing the it spun normally. That confirmed it was the fets to me, as it would do motor detection before.

Fets came yesterday and i swapped them out. Now when it tries to spin the motor on foc it makes a noise but nothing happens. I tried bldc and the motor spins real slowly and making a funny noise. When i throttle the motor turns very slowly. 

Its running a 4130 motor and 6s ion battery. Regen and braking are off as it for a free wheeling scooter.
```

---
## \#2 Posted by: L3chef Posted at: 2019-02-28T10:27:02.416Z Reads: 52

```
Try spinning the motor for hand when you do the ditection. Could be your motor is sensorless
```

---
## \#3 Posted by: g1tana Posted at: 2019-02-28T10:52:01.437Z Reads: 49

```
My motor is sensorless but i have not had to do this before
```

---
## \#4 Posted by: L3chef Posted at: 2019-02-28T11:19:44.067Z Reads: 46

```
Spinn them and see what happens
```

---
## \#5 Posted by: g1tana Posted at: 2019-02-28T11:32:25.951Z Reads: 45

```
As soon a i hit the measure flux button it jerks and the red light flashes but if i twist the throttle no red lights and the motor turns but slowly and there is no faults
```

---
## \#6 Posted by: g1tana Posted at: 2019-02-28T11:32:39.015Z Reads: 42

```
Turning motor didnt help
```

---
## \#7 Posted by: L3chef Posted at: 2019-02-28T11:34:06.531Z Reads: 43

```
Could be a blown drv or a bad mosfet.
```

---
## \#8 Posted by: g1tana Posted at: 2019-02-28T12:05:03.478Z Reads: 40

```
When i do continuity check on the front fets, they show a resistance of 624 from pin 1 to 6 but on the back the resistance is 0. Im sure it is resistance it measures
```

---
