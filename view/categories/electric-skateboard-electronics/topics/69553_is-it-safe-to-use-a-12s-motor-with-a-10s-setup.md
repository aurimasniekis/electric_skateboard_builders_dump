# Is it safe to use a 12S motor with a 10S setup?

### Replies: 6 Views: 250

## \#1 Posted by: Pafrican Posted at: 2018-09-29T17:32:06.192Z Reads: 113

```
Hello,

My board died on me last week; I'm guessing it's because I was running a TB VESC (in FOC) on 10S using a Turnigy 245kv motor. 
I'm thinking of upgrading to an Ollin VESC and replacing the motor with a Turnigy 168kv.

The voltage rating on the 168kv motor is 12S. I'm going to keep my 10S setup. I'm wondering if I'm putting my hardware, particularly my VESC, at risk by doing so.

I know it is safe to run a motor with lower voltage, it just won't reach its full potential and it may run a bit hotter. I'm concerned that the VESC will fry because the motor might draw max current too quickly. This should be limited by the VESC program, but I just want to run this by everyone before I spend another $300.

Thanks
```

---
## \#2 Posted by: b264 Posted at: 2018-09-29T17:33:57.207Z Reads: 113

```
Yes.

The lower kv motor will draw less current anyway.
```

---
## \#3 Posted by: Namasaki Posted at: 2018-09-29T17:35:33.323Z Reads: 107

```
The Vesc controls the motor. 
So the motor will only take what the Vesc gives it. 
The Vesc is the boss of the whole system.
That pertaining to current. 
As for voltage, it’s better for the motor to be over rated than under rated.
The motor’s voltage rating is simply the max voltage it can handle.
```

---
## \#4 Posted by: pixelsilva Posted at: 2018-09-29T17:54:03.492Z Reads: 94

```
> The voltage rating on the 168kv motor is 12S.

:point_up_2: ...I don't know much about it, but is this the voltaje rating, eh? ...12s?
```

---
## \#5 Posted by: Namasaki Posted at: 2018-09-29T18:50:40.879Z Reads: 72

```
That would be the voltage rating which means the motor can handle up to 50.4v but will also work with less voltage.
Since the battery in this example is only 10s or 42v, there is plenty of headroom for the motor and headroom is always a good thing.
```

---
## \#6 Posted by: Hummie Posted at: 2018-09-30T03:47:19.655Z Reads: 43

```
the voltage limit of the motor is just the insulation on the windings which can get to many more volts before electricity will break through.  I bet you could run it at 10,000 volts.  there's also the limit at which the bearings can spin but that's not really a voltage limit.
```

---
