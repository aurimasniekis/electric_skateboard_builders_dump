# My board goes full throttle when the remote is off!

### Replies: 11 Views: 252

## \#1 Posted by: Hummie Posted at: 2019-05-25T23:26:31.551Z Reads: 101

```
its the mini trigger and focboxs on a new board im putting together.   it seems fine when the remote is on and the throttle is fine but when i turn the remote off then luckily just on my table.
```

---
## \#2 Posted by: mutantbass Posted at: 2019-05-25T23:27:27.563Z Reads: 101

```
did you pair it with the failsafe? torqueboard has a video on youtube. there is a step by step way you have to do it .
```

---
## \#3 Posted by: wannagofast Posted at: 2019-05-26T00:21:28.428Z Reads: 93

```
This exact same thing happened to me with the same remote. Did the failsafe fix it for you?
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-05-26T00:25:37.237Z Reads: 84

```
You need to calibrate it with the vesc tool. Have a look at the live deadband pulswidth with the remote off, make that the deadband setting in the vesc, then turn the remote on and turn the "th trim" forward or back accordingly to match up the "off" pulsewidth with the deadband pulsewidth.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-05-26T00:38:53.351Z Reads: 77

```
His particular case is with the failsafe.

Had the same issue. It was cause the failsafe was set at 100% so whenever the remote disconnects or turns off it would pin my board at 100% forever... 🤣
```

---
## \#6 Posted by: wannagofast Posted at: 2019-05-26T00:40:53.052Z Reads: 74

```
My remote was already calibrated but I did the failsafe set up again and it stopped. Thanks guys!
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-05-26T00:42:30.046Z Reads: 67

```
Vesc tool calibration has nothing to do with the remote Fail-Safe it's two different things 😀
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-05-26T00:45:56.084Z Reads: 60

```
It's good information regardless
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-05-26T00:46:41.679Z Reads: 58

```
[quote="Sn4pz, post:8, topic:94975"]
chill lmao
[/quote]

Huh.... Wdym
```

---
## \#10 Posted by: Sn4pz Posted at: 2019-05-26T00:47:40.202Z Reads: 54

```
I thought you were commenting about Matt's post again 

Fixed 🤔
```

---
## \#11 Posted by: nuttyjeff Posted at: 2019-05-26T02:29:05.387Z Reads: 42

```
Literally happened to me 2 times in the past 2 weeks.

The first time: i rebinded the tx to rx and it worked fine after.

The second time: no matter how maby times i rebinded, it didn't work. It worked after i swapped the rx out.
```

---
