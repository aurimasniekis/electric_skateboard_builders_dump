# What&rsquo;s the formula to calculate top speed of a E board?

### Replies: 7 Views: 1847

## \#1 Posted by: BillySoul Posted at: 2016-12-08T01:50:29.038Z Reads: 212

```
How do I calculate what the top speed of a build will be? Cheers guys
```

---
## \#2 Posted by: ZachNYC Posted at: 2016-12-08T02:00:50.704Z Reads: 215

```
There are a couple calculators, there is a google sheets one that I think is pretty good. For a quick calculation though, just look up esk8 calculator.
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-12-08T02:03:06.820Z Reads: 211

```
Multiply voltage by kV to get the motors maximum RPM. Then multiply that by your reduction ratio to get the RPM of your wheels. Multiply that number by the circumference of your wheel. Then you would have something like speed in mm/min, convert that to mph or kph and you're good. Alternatively, you can use this online calculator: http://calc.esk8.it/
```

---
## \#4 Posted by: ZachNYC Posted at: 2016-12-08T02:55:19.979Z Reads: 193

```
For some reason it's not letting me copy the link from the original one, so here is a copy of it. Credit to @jacobbloy who made the original
```

---
## \#5 Posted by: BillySoul Posted at: 2016-12-08T02:58:35.444Z Reads: 157

```
You're the dude alright! How do I calculate 500wattw to KV as the manufacturer is a bit short champ?
```

---
## \#6 Posted by: 91Seconds Posted at: 2016-12-08T12:59:29.163Z Reads: 108

```
the kv of a motor (RPM/V) is independant of it's power (W).  Even without any load on an electric motor it will still have a maximum speed and not just due to the frictional losses of the motor acting as it's own load.  The top speed of a motor is changes depending on the voltage applied to it so motors are given kv numbers which tell you how many rpm the top speed is per volt applied.  

Two motors of the same wattage can have completely different kv with the lower the kv the higher the torque.  The top speeds calculated in these calculators are theoretical based on electrical properties and with no regard for physical limitations.  If you were to use a drone motor, which are tiny and have very high kv, your theoretical top speed would be up around 800km/h  but in reality the motor will likely not even be able to move the board even from rest with nobody on it.
```

---
## \#7 Posted by: 91Seconds Posted at: 2016-12-08T13:02:23.092Z Reads: 90

```
so having said that, you can use this [toddy616.blogspot.co.nz/2013/07/electric-skateboard-calculator.html?m=1](http://toddy616.blogspot.co.nz/2013/07/electric-skateboard-calculator.html?m=1) and assuming the drivetrain is well designed you can put an efficiency parameter of 75%
```

---
