# Cannot map pulse length on VESC 6.4 with Arduino as receiver

### Replies: 3 Views: 182

## \#1 Posted by: MaxMaker Posted at: 2018-06-20T18:38:34.522Z Reads: 48

```
Hi, so I hooked up my Arduino to the VESC 6.4 with Signal and GND going through 10k Ohm Resistors. The resistors were neccessary, because otherwise the VESC would power the Arduino. Somehow I cannot get the VESC app to show any kind of pulse length data. It always says "please activate realtime data and measure the pulse length first." I tried all kinds of things, but cannot get it to work. What am I doing wrong? I feel that is should at least display some random data. 

To check my connections, I let the Arduino control a small servo and that worked fine.
```

---
## \#2 Posted by: AchimWurm Posted at: 2018-06-21T10:19:34.501Z Reads: 35

```
If you don't want the vesc to power the Arduino, why do you plug anything else then signal into the vesc in the first place?
```

---
## \#3 Posted by: MaxMaker Posted at: 2018-06-21T19:59:10.917Z Reads: 24

```
Because... I personally don’t know. I followed advice from all kinds of people. And I belive they need a common ground to transmit the signal at all. I powerd a servo once on its own and only connected signal. That didn’t work.
```

---
