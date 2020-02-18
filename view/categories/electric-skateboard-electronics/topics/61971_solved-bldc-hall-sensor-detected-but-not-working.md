# \[Solved\] BLDC Hall Sensor Detected but not working?

### Replies: 9 Views: 234

## \#1 Posted by: onepunchboard Posted at: 2018-07-16T01:47:10.496Z Reads: 64

```
I'm scratching my head now.
in BLDC, I tried to use Hall sensor. It detects but only jitter when tried to use the motor in at any amp/voltag/ throttle. Just Jitter.
Anyone knows why?
If I turn off Sensor Mode it works tho

right now values are 255, 6, 4, 5, 2, 1, 3, 255 there are only 6 wire so it is doing right. in the tap it show 225 as 6.

Only possibility I can think of is the extention I made. But even the sensor made in factory jitters could it be the wire prob?

Thanks for the help

NvM: I got it. it was Vesc tool error, it was set to -1 6 4 5 2 1 3 -1
I manually changed -1 to 6 now it works
```

---
## \#2 Posted by: MannyM0E Posted at: 2018-07-16T03:13:13.312Z Reads: 50

```
Maybe this the problem I'm having with my Hall Sensor. I run motor dectection with the hall sensors and the motor spins fine dectects and everything. Once everything done, I pull my throttle and the motors don't spin at all. Wonder what the issue could be could be
```

---
## \#3 Posted by: onepunchboard Posted at: 2018-07-16T03:29:45.725Z Reads: 48

```
Yeap try that
```

---
## \#4 Posted by: MannyM0E Posted at: 2018-07-16T03:51:13.596Z Reads: 40

```
I don't know how to calculate the settings manual for hall sensors
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-07-16T03:52:53.188Z Reads: 37

```
when u do the detection, the tool will show the  values. take that and put into sensor tap and write the setting. and make sure u running the hybrid.
```

---
## \#6 Posted by: MannyM0E Posted at: 2018-07-16T03:54:48.207Z Reads: 36

```
You would first select hybrid mode on the bldc setting manual before motor detecting ?
```

---
## \#7 Posted by: onepunchboard Posted at: 2018-07-16T03:55:50.864Z Reads: 35

```
well it doen't matter but thats what i did
```

---
## \#8 Posted by: MannyM0E Posted at: 2018-07-16T03:57:04.255Z Reads: 34

```
Awesome. Whenever get the chance I'll do that. Thanks for the topic
```

---
## \#9 Posted by: RafaelinMissouri Posted at: 2019-03-13T20:35:03.474Z Reads: 22

```
Hey dude. How did you change these values?
```

---
