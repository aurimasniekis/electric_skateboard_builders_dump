# VESC bat regen settings with a discharge BMS

### Replies: 13 Views: 244

## \#1 Posted by: taz Posted at: 2019-03-08T11:21:06.142Z Reads: 72

```
Here is my problem.
I changed the 6355 sealed Maytech motors with 6374 sealed Maytech on my Evo. Both motors are supposed to be 190kv but I am not so sure if this is the case.
Now the board has weak high speed brakes, low speed is fine.
VESC settings:
Motor Current Max Brake:-50A
Battery Current Max Regen:-10A

Normally I would increase the Battery Current Max Regen to something like -20A but since I use a discharge BMS in this board I am afraid it will trigger the BMS protection.
The BMS is the Besttech HCX-D223V1 and the Maximal continuous charging current is 20A so I am already at the limit.

Do any of you guys have any suggestions? (apart from bypassing the BMS of course).
```

---
## \#2 Posted by: Battosaii Posted at: 2019-03-08T12:38:23.062Z Reads: 67

```
Weird cause my 6374s had significantly stronger braking than my 6355s both 190kv

I would raise it to -12 battery amps and try it out. Usually when braking it's for a short amount of time so it would be an amp spike not a constant so even the BMS should be able to handle it. 

What battery are you using?
```

---
## \#3 Posted by: taz Posted at: 2019-03-08T12:40:42.260Z Reads: 62

```
Yeah, I can't figure out why.
I use a 12S5P 30Q so handling more current for a short time is not a problem, it is the BMS I am worried about.
On my other board with a charge only BMS I have the batt regen around -30A .
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-03-08T13:45:08.115Z Reads: 57

```
[quote="taz, post:3, topic:86541"]
-30A
[/quote]

Wtf..... How heavy are you 🤣and dual or single?
```

---
## \#5 Posted by: taz Posted at: 2019-03-08T13:46:36.182Z Reads: 52

```
78kg, maybe close to 90kg with gear and backpack.
Dual, however it is pretty steep where I live.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-03-08T13:47:12.791Z Reads: 52

```
-30a per vesc?
```

---
## \#7 Posted by: taz Posted at: 2019-03-08T14:01:20.591Z Reads: 53

```
Yes.
10 char.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-03-08T14:01:42.175Z Reads: 52

```
Hmmmm...... Alright than 😅
```

---
## \#9 Posted by: L3chef Posted at: 2019-03-08T14:07:22.312Z Reads: 51

```
Just curious. What vesc version and brand do you have? Also, what firmware?
```

---
## \#10 Posted by: taz Posted at: 2019-03-08T14:15:02.209Z Reads: 47

```
Focboxes, FW 3.51.

The other board (the one with the bypassed BMS) has VESC6.
```

---
## \#11 Posted by: mmaner Posted at: 2019-03-08T14:47:20.642Z Reads: 50

```
did you re-do motor detection?  you should be able to go to -12 on max regen without issue, i mean try it out to make sure, but you should be ok.  That's my minimum, and that is really soft brakes IMHO.
```

---
## \#12 Posted by: taz Posted at: 2019-03-08T14:51:16.123Z Reads: 50

```
I did motor detection after I changed motors. Everything is working great apart from the high speed braking which is kind of weird since I did not have any problem with the 6355s.
I am just afraid that if I go over the BMS's maximum charge current it may at some point shut down and I am left without brakes.

At this point I am thinking that bypassing the BMS may be the only solution.
```

---
## \#13 Posted by: mmaner Posted at: 2019-03-08T14:54:57.013Z Reads: 47

```
I would bypass the BMS, I've had too many issues with Charge/Discharge BMS's including e-switch failures, random cutouts on brakes (even at really low amps).  To be clear 90% of the BMS's Ive used in charge/discharge have been fine, but the bad 10% have me gun shy now.

Depending on you rBMS you may be able to direct swap the balance lead connector making the change out to a charge only BMS pretty fast and easy.  The BesTech D140 is pretty great, I've used 10 or 12 and have only had 1 bad BMS.

If you have a BT module you can pad up and test the brakes at different levels to see if it cuts out at -12a per vesc, my feeling is that it wont, assuming the BMS is not faulty.
```

---
