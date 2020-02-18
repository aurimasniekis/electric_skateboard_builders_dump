# VESC for self balancing scooter motor wheel?

### Replies: 10 Views: 6119

## \#1 Posted by: Nicolas Posted at: 2016-04-03T21:31:30.421Z Reads: 133

```
Dear eSk8 community, 

I am looking for a solution to control a motor wheel (from self balancing scooter) with classical RC system. 
So my question is : does the VESC could do this ? Did some people already do a sk8 with this kind of wheels ? 

My main concern, is that the motor wheel is a brushless, 36V, 250W motor with 3 hall effect sensors, but the sensors are not in a 120° position. Could it be a problem ? 

<img src="/uploads/db1493/original/2X/a/af99d8de8fdcae0643da42b25c1f70e75287ab1d.JPG" width="666" height="500">

Thanks 
Best regards
Nicolas
```

---
## \#2 Posted by: laurnts Posted at: 2016-04-03T21:38:37.196Z Reads: 133

```
If the motor from the balancing scooter is a 3 phase brushless motor (3 wires motor), in which I assume it is. Yes it will run with VESC although the limit would be 40v - 60v tops in which those hub motor is usually operate. if it comes with some small wires for the hall sensor, VESC also support sensored mode.

If you plan to use this for your eboard longboard / mountainboard surely it will work.
```

---
## \#3 Posted by: Nicolas Posted at: 2016-04-03T22:17:38.418Z Reads: 132

```
Thanks a lot laurnts for your quick answer. 

Yes, it is a 3 phases brushless motor. It comes with the wires from hall sensors (the 3 sensors are visible on the picture, as well as the wires from the sensors : yellow, blue and green, and I assume black and red for + and -)). 

What do you mean by the limit would be 40v - 60v tops ? 
The motor is using a 10S2P Li-ion battery today (36 V - 4.5 Ah). 

I plan to use this motor to a kind of mountainboard. 

Thanks again
Nicolas
```

---
## \#4 Posted by: laurnts Posted at: 2016-04-03T22:43:46.690Z Reads: 119

```
VESC doesnt run higher than 12s, 10s is the setup that is very common in the esk8 community and 10s is the configuration of the well known space cell from enertionboard (10s4p).

The battery configuration you have will work for sure with self balancing as well as VESC.
We have @onloop from enertionboard provide a short video how he integrate the build together.
https://www.youtube.com/watch?v=N4xgtJMyl0o
```

---
## \#5 Posted by: barajabali Posted at: 2016-04-04T03:01:37.325Z Reads: 108

```
Why dont you just run them without sensors? surely they have enough torque without them if you run enough volts thru them...

Also how are you going to mount them?  i have a pair of them that id like to turn into a MT board but im not sure how to start
```

---
## \#6 Posted by: Nicolas Posted at: 2016-04-04T11:12:38.583Z Reads: 94

```
The sensors are already there, and I still want to keep a self balancing possibility in my prototype, that needs good control and torque at no speed... 

So I order a VESC, I come back as soon as I begin the tests with the motor.
Thanks !
```

---
## \#7 Posted by: barajabali Posted at: 2016-04-04T19:54:22.733Z Reads: 83

```
How are you going to attach these to a truck?
```

---
## \#8 Posted by: Nicolas Posted at: 2016-04-07T20:26:05.878Z Reads: 78

```
For now, I do not plan to use a truck, but self balancing possibilities... But this can change after the first try !
```

---
## \#9 Posted by: FloRider Posted at: 2016-08-08T05:49:08.881Z Reads: 68

```
Hi Nicolas. I am also trying to use the same kind of motor with the VESC (dual setup). Have you had any luck with your motors? How did you manage to have both motors spin in the correct direction and what connector do you use for your hall sensor connection?
```

---
## \#10 Posted by: Okami Posted at: 2016-10-06T01:49:43.691Z Reads: 53

```
Partly related - has anyone seen someone using these motors for a mountainboard?
```

---
