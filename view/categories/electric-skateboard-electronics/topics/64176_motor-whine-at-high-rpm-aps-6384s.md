# Motor whine at high rpm? APS 6384S

### Replies: 12 Views: 330

## \#1 Posted by: michaelcpg Posted at: 2018-08-07T21:17:34.172Z Reads: 94

```
Hey all, recently upgraded my pair of sensorless 6374 APS motors to sensored 6384 APS motors and I've noticed that the new motors produce an audible whine at higher RPMs? 

I'm running sensored FOC on FOCboxes with an E-Toxx gear drive. 

I opened the motors before installing them to inspect them and give the sensors a waterproof coating and didn't see anything obvious that might produce such a noise.

Anyone have any idea what might be causing the whine?
```

---
## \#2 Posted by: Amonada Posted at: 2018-08-23T11:57:50.100Z Reads: 76

```
I have the same "problem" with my two 6384 sensored 170kv. 
They are relatively quiet until a certain RPM, then they get really loud and go silent afterwards again. I have to check at which RPM this whining occurs. I'm using ESCapes in FOC btw.
My Motors also get really hot during riding, i dont know if there is a connection between these two issues...
```

---
## \#3 Posted by: Schulerbible Posted at: 2018-08-23T12:17:50.739Z Reads: 70

```
Street or AT setup? How loud is loud? My RSPEC in bldc mode are loud af compared to other brands ....
```

---
## \#4 Posted by: Amonada Posted at: 2018-08-23T12:44:43.662Z Reads: 67

```
They are mounted on a Mountainboard with an E-Toxx Gear drive. 
I dont know how loud exactly, i do not have the equipment to measure it.
But they get around 4-5 times louder at the mentioned RPM, sounds like a angry turbine.
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-08-23T12:50:48.265Z Reads: 66

```
Does changing the f_sw / switching frequency value help at all? Just curious... Not saying it will help
```

---
## \#6 Posted by: Schulerbible Posted at: 2018-08-23T13:50:07.675Z Reads: 55

```
That sounds good 😀 ...... might be getting into resonance with the system?
```

---
## \#7 Posted by: chocol4te Posted at: 2018-08-23T14:35:12.821Z Reads: 49

```
The same thing happens to me and some others with the APS8082S. Really bad resonance at 65% rpm.

It was pretty bad with no load, and I assumed it would be dampened once I got the belt on and tightened it, but no luck.
```

---
## \#8 Posted by: PatRocks Posted at: 2018-08-23T15:18:42.758Z Reads: 45

```
If it sounds like a "guitar string" (use your imagination, like a twang-y ish sound) it's a loose motor winding. Pull the can off, grab a toothpick and find the loose wires, hit 'em with a dab of epoxy and get schwifty
```

---
## \#9 Posted by: chocol4te Posted at: 2018-08-23T16:32:17.912Z Reads: 44

```
It’s a strange issue, because that’s not really the sound it makes. It’s a much harsher grinding sound, but disassembly reveals no scratches (and I looked everywhere). The manufacturer tells me it is normal and will not damage the motor.
```

---
## \#10 Posted by: PatRocks Posted at: 2018-08-23T16:54:38.814Z Reads: 41

```
Got any pics? Magnets show any signs of wear?
```

---
## \#11 Posted by: chocol4te Posted at: 2018-08-23T22:54:45.657Z Reads: 36

```
I’m away so won’t be able to for at least a week, but I think the vibration is along the axis of the shaft, not side to side, based on the slow motion video I took (again, saved on my desktop, so can’t post for a week)
```

---
## \#12 Posted by: michaelcpg Posted at: 2018-08-23T23:13:09.290Z Reads: 35

```
Sounds similar to my issue, it only seems to happen in a certain RPM range, outside of that range the motor sounds perfectly fine. I haven't had any issues with the motors getting hot though so that may be a separate issue?

The videos in this post are fairly similar to the sound that I'm getting from one of my motors though

https://www.electric-skateboard.builders/t/trampa-emtb-8072-sensored-alien-motors-with-e-toxx-direct-drive/65188/36?u=michaelcpg
```

---
