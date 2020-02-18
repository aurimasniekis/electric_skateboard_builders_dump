# 300a esc and 70a motor

### Replies: 27 Views: 1092

## \#1 Posted by: Ron189 Posted at: 2018-03-12T17:54:22.060Z Reads: 143

```
Hey!
I have a 300a esc and a 70a motor.
So I have two questions for you:
1) Can the esc and the motor work together? the amp of the esc is not too high for the motor?
2) If the esc works with the motor, so the esc would take 70a from the battery? or still 300a?

Thanks a lot!!!
```

---
## \#2 Posted by: MoeStooge Posted at: 2018-03-12T17:57:12.644Z Reads: 139

```
Yes! ESC is ok if motor kv is within kv limit of esc. Make sure your 70a motor is up to the mechanical task it's being asked to perform..
```

---
## \#3 Posted by: Ron189 Posted at: 2018-03-12T17:59:05.134Z Reads: 134

```
Thank you so much!
and what do you mean by " Make sure your 70a motor is up to the mechanical task it’s being asked to perform"
Sorry, my English is not too strong
```

---
## \#4 Posted by: FredrikHems Posted at: 2018-03-12T17:59:20.612Z Reads: 130

```
1. The esc and the motor will work together, the question is how well.. To answer that we need more specs.

2. Its the motor that decide how many amps are pulled (on regular esc, not vesc i think), so the esc will pull maximum 70A from the battery.

Edit: @MoeStooge was faster :expressionless:
```

---
## \#5 Posted by: MoeStooge Posted at: 2018-03-12T18:06:27.936Z Reads: 111

```
Use this tool. http://calc.esk8.it/ if your motor lacks the amount if watts it takes to push the weight your loading the motor at, it will burn up..
```

---
## \#6 Posted by: Ron189 Posted at: 2018-03-12T18:17:51.594Z Reads: 103

```
Thanks a lot!
```

---
## \#7 Posted by: Ron189 Posted at: 2018-03-12T18:18:41.887Z Reads: 101

```
but on this tool i can only measure speed
```

---
## \#8 Posted by: Tuomalar Posted at: 2018-03-12T18:30:59.184Z Reads: 96

```
Please tell us more about these parts or send some pics.
```

---
## \#9 Posted by: Ron189 Posted at: 2018-03-14T17:49:55.737Z Reads: 78

```
![15210497297691898397900|690x388](upload://vyaMMINGcAufIPpIY2lESrS6k90.jpg)
Is that helps you?
Flier 300a car esc
```

---
## \#10 Posted by: MoeStooge Posted at: 2018-03-14T18:21:30.842Z Reads: 75

```
More motor info needed. 70a motor at what voltage will determine your watts or horsepower.  For instance say a 500w motor(70a x 7.2v = 500w) will safely drive a 170lb vessle 12mph at wide open throttle. Gear it for 15mph and now it runs hot and has less applied torque at the wheel.   Watts(HP) needs to exceed the load to determine what top speed you need to calculate so you don't make magic smoke..
```

---
## \#11 Posted by: Ron189 Posted at: 2018-03-14T18:48:59.208Z Reads: 71

```
Voltage: 12S Lipoly
RPM/V: 149KV
Internal resistance: 0.021 Ohm
Max Loading: 70A
Max Power: 2250W
Gearing: 1:7.8

Thanks a lot!!
```

---
## \#12 Posted by: Cobber Posted at: 2018-03-14T18:51:17.782Z Reads: 69

```
wheel size is the lat bit for a roll out calc.
```

---
## \#13 Posted by: MoeStooge Posted at: 2018-03-14T19:25:13.995Z Reads: 64

```
2250w I'd say 20mph would be a safe Target to start with.  Monitor motor temps and shoot for 135 deg farenheit 160 tops..
```

---
## \#14 Posted by: pat.speed Posted at: 2018-03-14T19:47:55.871Z Reads: 61

```
He could surely go faster than that, right? You only start to pull around 2000w when nearing 50kmh, well that’s what I saw on a different post
```

---
## \#15 Posted by: Ron189 Posted at: 2018-03-15T11:52:42.394Z Reads: 51

```
the wheel size is 200mm 
So, can I build this? is that ok? the motor would not burn or something?
```

---
## \#16 Posted by: MoeStooge Posted at: 2018-03-15T13:55:12.915Z Reads: 49

```
Use the calculator tool above to achieve the mph I stated above using the equipment you have and it will be a safe starting point base line..
```

---
## \#17 Posted by: DeathCookies Posted at: 2018-03-15T15:06:37.160Z Reads: 43

```
[quote="Ron189, post:11, topic:48880"]
Voltage: 12S Lipoly
RPM/V: 149KV
Internal resistance: 0.021 Ohm
Max Loading: 70A
Max Power: 2250W
Gearing: 1:7.8
[/quote]
@MoeStooge @pat.speed  
I do not think that hobbykings 2250W is correct. IMO they mislabeled that...
50,4V (12S) * 70A ~ 3500W
```

---
## \#18 Posted by: MoeStooge Posted at: 2018-03-15T15:08:25.685Z Reads: 38

```
3500w will get him to 30mph
```

---
## \#19 Posted by: professor_shartsis Posted at: 2018-03-15T15:41:45.486Z Reads: 38

```
[quote="Ron189, post:11, topic:48880"]
Voltage: 12S Lipoly

RPM/V: 149KV

Internal resistance: 0.021 Ohm

Max Loading: 70A

Max Power: 2250W

Gearing: 1:7.8
[/quote]

KT torque per amp = 60 / (2 * pi * KV) = 0.064 nm/a

70a max recommended amps * 0.064nm/a = 4.486 newton meter max recommended torque

2250w max recommended mechanical power / 4.486nm = 501.56 radian per second max recommended angular speed at max recommended torque

501.56 r/s * 9.5492 rpm per r/s = 4789.5rpm max recommended rpm at max recommended torque at 70a

70a * 70a * 0.021ohm= 102.9w motor heating @ 70a

300a * 300a * 0.021ohm= 1890w motor heating @ 300a
```

---
## \#20 Posted by: Tuomalar Posted at: 2018-03-15T15:59:41.273Z Reads: 33

```
[quote="Ron189, post:15, topic:48880"]
the wheel size is 200mm
[/quote]

Diameter? If so that's crazy big wheel.
```

---
## \#21 Posted by: FredrikHems Posted at: 2018-03-15T16:06:10.258Z Reads: 29

```
I guess they`re just standard 8" pneumatics?
```

---
## \#22 Posted by: Tuomalar Posted at: 2018-03-15T16:07:54.360Z Reads: 30

```
True dat. I didn't realize that pneumatics are so damn huge.
```

---
## \#23 Posted by: Ron189 Posted at: 2018-03-15T16:33:19.414Z Reads: 29

```
Its a mountain board. So the wheels are very big 
8inch
So nothing happend right? Im a little bit confused with all of that data.
```

---
## \#24 Posted by: professor_shartsis Posted at: 2018-03-15T17:15:00.064Z Reads: 24

```
at 0.021ohm, the esc limits the current, not the motor.... so at 12S you can get 300a.

simply shorting the motor with 48v (not advised) gives:

48v/0.021ohm=2285.71a

2285.71a * 48v=109714.28w

the job of the esc is to limit the current below 2285.71a (in this case to 300a).

for motor heating that works out to: 300a * 300a * 0.021ohm= 1890w motor heating @ 300a

since the kv is 149kv, torque at 300a motor current works out to: 300a * 0.064nm/a (kt-torque per amp)= 19.2 newton meters.
```

---
## \#25 Posted by: FredrikHems Posted at: 2018-03-15T17:36:32.886Z Reads: 22

```
I didnt quite understand that, but there is no way you`ll get 19.2 Nm of torque directly from a 6374 motor..
```

---
## \#26 Posted by: MoeStooge Posted at: 2018-03-15T18:55:33.679Z Reads: 19

```
Disregard the over educated... Your motor will not pull over it's designed amp if you don't overload it.. gear it properly so it operates in it's load window and you will be fine.  A 300a ESC on a 70a motor is a good combo and a great safety factor window for your power delivery system..
```

---
## \#27 Posted by: Ron189 Posted at: 2018-03-15T19:37:02.955Z Reads: 15

```
Thanks a lot!!
God bless you
```

---
