# BLDC tool is says &lsquo;bad detection result recieved&rsquo; when I try to detect the motor

### Replies: 18 Views: 1634

## \#1 Posted by: Horiz0n Posted at: 2017-11-16T00:07:49.167Z Reads: 180

```
So I am new to all of this, this is my first time and I don't really know what I am doing. I have set the voltage limits and then I got to detect the motor and it doesn't spin or anything. I have 2*5s lipos and a 6374-192 motoe?
```

---
## \#2 Posted by: dg798 Posted at: 2017-11-16T01:33:02.767Z Reads: 176

```
Make sure all phase wires are fully connected.
Can u post a pic of ur vesc settings?
```

---
## \#3 Posted by: E1Allen Posted at: 2017-11-16T07:12:22.644Z Reads: 166

```
Also if your wheel and motor pulley are attached. Remove the belt and just let the motor spin.  I had mine set to hybrid and forgot to plug in sensor wires. It failed until I plugged those in. Also failed a few with the belt attached
```

---
## \#4 Posted by: Horiz0n Posted at: 2017-11-16T07:44:32.000Z Reads: 160

```
I will post a pic when I get home from work :slight_smile:
```

---
## \#5 Posted by: Horiz0n Posted at: 2017-11-16T07:45:13.578Z Reads: 151

```
No pulley is attached at the moment, and I don't thing my is a hybrid, how would I know?
```

---
## \#6 Posted by: Horiz0n Posted at: 2017-11-16T14:42:42.586Z Reads: 143

```
<img src="/uploads/db1493/original/3X/6/4/643baf7d31f9f89c579916628dced84213fa3553.PNG" width="690" height="367">
```

---
## \#7 Posted by: Horiz0n Posted at: 2017-11-16T14:49:23.285Z Reads: 139

```
I'm thinking it has something to do with the battery cutoff voltages but I thought I had set them right?
```

---
## \#8 Posted by: E1Allen Posted at: 2017-11-16T16:46:29.979Z Reads: 140

```
What S is your setup? 10s 6s 12s?
```

---
## \#9 Posted by: E1Allen Posted at: 2017-11-16T16:49:31.802Z Reads: 141

```
Your battery cutoff may be above your input volts. That might be your problem as well
```

---
## \#10 Posted by: Horiz0n Posted at: 2017-11-16T17:11:02.578Z Reads: 139

```
I have 2*5s so 10s. I think I have identified the problem though. I believe I have a faulty DRV... I have no clue how though
```

---
## \#11 Posted by: dAeM0N1K3 Posted at: 2017-11-16T17:28:09.944Z Reads: 132

```
I had the same problem. Remove the CANBUS wire before running motor detection from each VESC.
```

---
## \#12 Posted by: Horiz0n Posted at: 2017-11-16T17:41:56.119Z Reads: 129

```
Which one is the CANBUS wire? Sorry, I'm new to all of this
```

---
## \#13 Posted by: dAeM0N1K3 Posted at: 2017-11-16T18:04:08.313Z Reads: 126

```
The wires you see here between the VESCs are canbus. They're usually black or white in most cases though. However I didn't notice previously that you only have a single motor, therefore only one VESC. So this is probably not the issue you have. Sorry

<img src="/uploads/db1493/original/3X/8/4/84865c54ce5c15b17e5d45cc966cc1e241b04353.png" width="640" height="480">
```

---
## \#14 Posted by: EastLosMike Posted at: 2017-11-16T18:20:35.666Z Reads: 123

```
I had the same issue with my single drive. There is no need to remove the belts  (at least in my experience during motor detection) change the battery cutoff start to 8v. Run the motor detection once everything is set change the battery cutoff start to the suggested V for your 10S setup.

Shout out to @yummyblobs for this tip.
```

---
## \#15 Posted by: Horiz0n Posted at: 2017-11-16T20:57:27.815Z Reads: 118

```
Ah okay, I only have 1 VESC though, I forgot to mention that!
```

---
## \#16 Posted by: Horiz0n Posted at: 2017-11-16T21:01:21.286Z Reads: 115

```
Mine is single drive too, tried the 8v, exactly the same
```

---
## \#17 Posted by: Horiz0n Posted at: 2017-11-16T21:07:08.606Z Reads: 116

```
I get this fault in the terminal, looks like my brand new VESC's DRV is damaged somehow 


Fault            : FAULT_CODE_DRV8302
Current          : 0.2
Current filtered : 0.2
Voltage          : 41.56
Duty             : 0.02
RPM              : 1.9
Tacho            : 7
Cycles running   : 4
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 1
Temperature      : 23.30
```

---
## \#18 Posted by: dg798 Posted at: 2017-11-16T21:32:49.311Z Reads: 109

```
U can ask @jonnymeduse for a repair otherwise u have to buy a new one.
Sorry
```

---
