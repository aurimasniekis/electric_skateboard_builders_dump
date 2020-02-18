# VESC Braking with a 10C battery

### Replies: 3 Views: 631

## \#1 Posted by: brun Posted at: 2016-07-24T18:29:32.224Z Reads: 107

```
Recently upgraded my 1st board from a hobbyking ESC to VESC ( 5200mAh  6s 10C battery, 147KV motor, 16T,36T,83mm wheels).  I LOVE the improvement.  Torque when you want it, breaking and in FOC it's practically silent. But I'm worried about over-charging my battery in breaking.  Seems it's not "recommend" to charge over the C rating (in Amps).  My VESC brake is set at -10A so I'm already over that by 2x.  -10A feels pretty good when ridin, but would like more braking...say 15-20A.  Is this going to blow out these batteries if I brake for say a full minute down a hill?  How long can a 10C lipo handle 20A in breaking?   (I plan on upgrading to 10S 25C for my second board).  Incidentally, I've never had any heat issues with my 6s setup...only the motor itself ever gets even slightly warm on a 6 mile ride..I am a bit top-end limited though.
```

---
## \#2 Posted by: XIII Posted at: 2016-07-24T22:56:46.761Z Reads: 81

```
10c with a 5200mah battery 

means the battery can deliver 10*5.2A continious = 52A so you are well in the safe zone. 

Just make sure you don't overcharge the vesc when you are braking with a full battery. Dunno if Vesc has protection for that
```

---
## \#3 Posted by: brun Posted at: 2016-07-25T00:21:33.135Z Reads: 63

```
Thanks X.   I see that these batteries have a C rating for charging that is independent of the C rating discharge.  Here are a few examples.
Turnigy 5000mAh 5S 25C Lipo Pack max charge rating is:  2C.
Multistar High Capacity 6S 5200mAh (my batteries)  also:   2C.

Of course this is recommended setting for continuous charge.  Makes me thing that doubling that for relatively short periods would be ok...ie a 25A charge rate (5C for a 5000mAH battery) would be ok for short periods...under a minute or so.  Just a guess.
```

---
