# Fault_code_abs_over_current

### Replies: 8 Views: 287

## \#1 Posted by: DavidBanner Posted at: 2018-06-16T14:16:31.013Z Reads: 112

```
I am working on a dual 6374 build and have a gremlin problem.

I am getting FAULT_CODE_ABS_OVER_CURRENT on both FOCBOXes but only when both motors are running via CANBUS. I can run the individual motors/FOCBOX without issue.

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 86.1
Current filtered : 135.7
Voltage          : 37.79
Duty             : 0.52
RPM              : 37191.9
Tacho            : 16403
Cycles running   : 28
TIM duty         : 3932
TIM val samp     : 1903
TIM current samp : 5652
TIM top          : 7498
Comm step        : 2
Temperature      : 30.70

So far I have replaced:
FOCBOX x 2 
Bullet Connectors
BMS
Remote and RX module

but the issue persists....

Anyone got any suggestions ? @barajabali @Blasto
```

---
## \#2 Posted by: Blasto Posted at: 2018-06-16T16:04:33.546Z Reads: 97

```
For fun, reverse the focbox roles. Make master the slave, slave the master. Without changing any hardware
```

---
## \#3 Posted by: zpoole27 Posted at: 2018-06-16T16:31:00.618Z Reads: 92

```
Do you have any mechanical symptoms? Stuttering? Weird noises from motors?

I had this issue on rspecs because they were shorting out, totally unnoticeable for the first while, so I ignored it, kept riding for a few weeks until it started randomly throwing full brakes (shorting) on me.

Maybe its your motors? In my professional noob opinion.
```

---
## \#4 Posted by: DavidBanner Posted at: 2018-06-16T20:14:02.255Z Reads: 85

```
it seems to be something sensor related.

I am running sensorless BLDC without an issue. I will check the sensor cable wiring tomorrow, but it's weird that the both the motors detected the sensors okay and run independently in sensored mode without an issue.
```

---
## \#5 Posted by: ducktaperules Posted at: 2018-06-16T21:23:33.026Z Reads: 79

```
I also get this when im running on dual focbox with your dual 6374, but it never caused me any problems whilst riding.
```

---
## \#6 Posted by: DavidBanner Posted at: 2018-06-17T08:36:53.523Z Reads: 63

```
[quote="ducktaperules, post:5, topic:59095, full:true"]
I also get this when im running on dual focbox with your dual 6374, but it never caused me any problems whilst riding.
[/quote]
this is odd! I have built more than a few dual boards using my 6374s and dual FOCBOX without this issue. I did extend the phase leads so I suspect that must be the cause.
```

---
## \#7 Posted by: PatRocks Posted at: 2018-06-17T08:50:20.771Z Reads: 59

```
Go split!!!...?
```

---
## \#8 Posted by: Andy87 Posted at: 2018-06-28T13:14:39.462Z Reads: 41

```
did you found the problem?
I have a similar problem.
Motor detection running without problems.
but I get the fault when sensor is connected.
if disconnect sensor wires no fault at all.
```

---
