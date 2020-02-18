# Intermittent drv8302 fault code from initial dual motor setup

### Replies: 13 Views: 807

## \#1 Posted by: cwazy1 Posted at: 2017-09-01T18:45:02.664Z Reads: 70

```
I'm trying to learn from my mistake and understand why I had a drv failure when first setting up my dual motor configuration. 

The fault comes up once every 10 or so throttle pulls. It'll flash red three times on the master vesc and shows the fault on BLDC tool. The slave will continue to work and does not throw any faults. 

The master vesc has been run about 50 miles perfectly as a single motor setup before the second motor parts arrived (yesterday). As a single motor, I had battery settings at 40a, and -14a. I also had all can related settings unchecked.

I also made sure that my duty ramp settings were 0.02

Also- detection works fine for both. 

Here is what I'm using
12s4p battery from DIY
6355 190kv sensored
vesc 4.12 with 2.18 from DIY
CANBUS connection between master and slave
BLDC with sensored motors
nano remote from DIY

And here are my BLDC settings

Master:

[url=https://ibb.co/hy78UF][img]https://preview.ibb.co/bZ3hpF/master1.png[/img][/url]
[url=https://ibb.co/iEjBia][img]https://preview.ibb.co/dxOhpF/master2.png[/img][/url]
[url=https://ibb.co/gzhLbv][img]https://preview.ibb.co/kakHOa/master3.png[/img][/url]
[url=https://ibb.co/jVC8UF][img]https://preview.ibb.co/c3fHOa/master4.png[/img][/url]

Slave:

[url=https://ibb.co/bJv6Gv][img]https://preview.ibb.co/hhzYwv/slave1.png[/img][/url]
[url=https://ibb.co/cVgfbv][img]https://preview.ibb.co/nG6ria/slave2.png[/img][/url]
[url=https://ibb.co/egWJUF][img]https://preview.ibb.co/faX3wv/slave3.png[/img][/url]
[url=https://ibb.co/fecE3a][img]https://preview.ibb.co/gKwk9F/slave4.png[/img][/url]

Can someone help me identify what went wrong? 
I'm thinking of just doing split PPM when I get a replacement vesc. Will I be able to avoid blowing another DRV8302 chip?
```

---
## \#2 Posted by: Eboosted Posted at: 2017-09-01T19:29:14.875Z Reads: 58

```
Did you make motor detection with the wheel and belt on? You should do it with no pullies attached, just the motor
```

---
## \#3 Posted by: cwazy1 Posted at: 2017-09-01T19:38:30.223Z Reads: 58

```
detection was made with the belt and wheel on. I never had an issue doing it this way with the single motor?
```

---
## \#4 Posted by: L3chef Posted at: 2017-09-01T19:40:11.689Z Reads: 60

```
Your slave hall table doesn't match the detection value you got. Did you forget to click write perhaps?
```

---
## \#5 Posted by: L3chef Posted at: 2017-09-01T19:40:43.996Z Reads: 59

```
And do detection without any load. Wheel, belt pulley
```

---
## \#6 Posted by: cwazy1 Posted at: 2017-09-01T19:44:46.577Z Reads: 57

```
That was the detection for the master. I didn't run detection on slave before taking a screenshot.
```

---
## \#7 Posted by: cwazy1 Posted at: 2017-09-01T19:46:00.174Z Reads: 56

```
Ah, okay, I'll keep this in mind moving forward. 

Could this have caused the drv failure? I was running detection with wheel and pulley on for single and was having no drv issues on the same vesc.
```

---
## \#8 Posted by: Eboosted Posted at: 2017-09-01T21:04:45.101Z Reads: 53

```
I had issues before making detection with load on, DRV failures, sometimes it's OK sometimes the VESC just dies, so why risk it. 

Just do motor detection with no load
```

---
## \#9 Posted by: cwazy1 Posted at: 2017-09-01T21:10:23.701Z Reads: 53

```
So you're saying that it could be the motor detection is causing issues with the drv? 

Would that mean there is a chance that my drv is not actually dead?
```

---
## \#10 Posted by: Eboosted Posted at: 2017-09-01T21:23:06.631Z Reads: 53

```
If your motor dies not spin and your get a drc8302 error, then you need to replace your drv
```

---
## \#11 Posted by: cwazy1 Posted at: 2017-09-01T21:30:14.462Z Reads: 54

```
Just tried to re detect without any pullets or wheels. The changes were insignificant enough not to make any impact to the rounded numbers when applied. Still showing DRV fault.
```

---
## \#12 Posted by: cwazy1 Posted at: 2017-09-02T22:37:01.883Z Reads: 46

```
Anyone have any other feedback? 

I just picked up a servo y harness as well as an extra servo male to male and have removed the +5v pin from one of them. 

Definitely planning to go the split ppm route.
```

---
## \#13 Posted by: L3chef Posted at: 2017-09-04T13:05:56.321Z Reads: 41

```
If you go with split servo, the one vesc only need signal wire
```

---
