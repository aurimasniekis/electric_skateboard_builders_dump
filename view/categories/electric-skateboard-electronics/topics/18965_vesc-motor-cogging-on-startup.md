# VESC Motor Cogging on Startup

### Replies: 11 Views: 1293

## \#1 Posted by: Esk8Builder Posted at: 2017-03-12T21:48:24.083Z Reads: 186

```
I am working on setting up my new electric longboard and have noticed that the motor (280kv 5055 SK3 motor) vibrates violently when I try to accelerate. The VESC is running in FOC mode but this phenominon also occurs when running BLDC. I have re-measured the inductance, resistance and flux linkage of the motor to no avail. Any help and adice would be greatly appreciated!
```

---
## \#2 Posted by: psychotiller Posted at: 2017-03-12T21:51:32.437Z Reads: 187

```
Is your motor sensored?
```

---
## \#3 Posted by: Esk8Builder Posted at: 2017-03-12T21:56:37.955Z Reads: 184

```
No, it's not. I'm considering buying a Hall Effect sensor for use with this motor. Would it fix the problem?
Here is a video of the cogging: [video](https://youtu.be/ymvaituupGA)
```

---
## \#4 Posted by: DougM Posted at: 2017-03-12T22:03:04.397Z Reads: 178

```
I usually just push to get the board started before I kick in the power.  I know this doesn't solve the problem, but it works.
```

---
## \#5 Posted by: Esk8Builder Posted at: 2017-03-12T22:04:47.095Z Reads: 174

```
Yeah that fixes it, but it would be nice to have a smooth startup. Maybe its a matter of motor torque?
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2017-03-12T22:09:18.177Z Reads: 168

```
try accelerating slowly, starting from the very bottom of the throttle
```

---
## \#7 Posted by: mmaner Posted at: 2017-03-12T23:41:17.601Z Reads: 157

```
That's a pretty small and high KV motor for a single motor build. I'd go with a 6355 245kv.
```

---
## \#8 Posted by: psychotiller Posted at: 2017-03-12T23:53:33.510Z Reads: 158

```
Yes it would fix the problem.
```

---
## \#9 Posted by: Eboosted Posted at: 2017-03-13T00:01:45.177Z Reads: 155

```
I don't like "uncensored" motors anymore only in porn
```

---
## \#10 Posted by: saul Posted at: 2017-03-13T00:37:22.582Z Reads: 148

```
The motor is just too small. 
50mm need a push.
63mm can go without.

I usually give a push anyways. It's very inefficient to start from stop. Lots of energy to get moving. Not much to keep moving.
```

---
## \#11 Posted by: michondr Posted at: 2017-05-04T14:32:33.651Z Reads: 121

```
according to video, it sounds like the belt its skipping teeth
```

---
