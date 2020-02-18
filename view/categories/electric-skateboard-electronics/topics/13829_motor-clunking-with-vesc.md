# Motor clunking with vesc?

### Replies: 17 Views: 633

## \#1 Posted by: Charster10 Posted at: 2016-11-28T17:50:49.570Z Reads: 43

```
So i recently got my vesc...went to install it and basically when i programmed it it all saved and was all perfect but when i gave it throttle the motor doesnt move and just clunks and occasionally gives LOADS of throttle and i cant find what it is....is it the motor wires ? If anyone knows PLEASE tell me !

Thanks guys.
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-11-28T18:00:45.575Z Reads: 43

```
What type of supply do you use, also are you in FOC or bldc ?
```

---
## \#3 Posted by: Charster10 Posted at: 2016-11-28T18:01:19.354Z Reads: 42

```
Im in bldc
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-11-28T18:02:33.387Z Reads: 40

```
Ok have you done a motor detection ? And what type of supply and motor are you using
```

---
## \#5 Posted by: Charster10 Posted at: 2016-11-28T18:04:17.167Z Reads: 36

```
Yeah done That I got a 6s lipo with a 320kv motor
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-11-28T18:05:45.719Z Reads: 36

```
I might sound stupid but are your battery fully charge ?
```

---
## \#7 Posted by: Charster10 Posted at: 2016-11-28T18:06:58.767Z Reads: 36

```
Charged = 25.2v ( MAX )
Mines on = 22.7v
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-11-28T18:08:56.078Z Reads: 35

```
Maybe you should charge them then retry(at that voltage they might not provide enought current to power your motor)...also what are your bldc tool parameter for the vesc cutoff start and cutoff (or just post a screenshoot)
```

---
## \#9 Posted by: Charster10 Posted at: 2016-11-28T18:10:12.189Z Reads: 35

```
Ok ill try , do you mean cut off for the battery??
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-11-28T18:10:35.539Z Reads: 35

```
No vesc cutoff, but battery cutoff should stay at 8v (or in that area)
```

---
## \#11 Posted by: Charster10 Posted at: 2016-11-28T18:11:09.123Z Reads: 35

```
Oh i dont think i set that...whats it under?
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-11-28T18:12:59.124Z Reads: 34

```
Never try it before 🤔
```

---
## \#13 Posted by: Charster10 Posted at: 2016-11-28T18:15:40.185Z Reads: 34

```
<img src="/uploads/db1493/original/3X/1/d/1df914564f7e0e1d3bc46a899c21c1a079cdf260.jpeg" width="566" height="185"> do you mean the min input and max input here?
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2016-11-28T18:16:24.602Z Reads: 33

```
No the cutoff start and end
```

---
## \#15 Posted by: saul Posted at: 2016-11-28T18:34:51.086Z Reads: 31

```
the cutoff start and end need to be lowed for detection.
delete the leading 2's.
write config.
motor detection.
test.
put the 2s back.
write.

go ride!
```

---
## \#16 Posted by: saul Posted at: 2016-11-28T18:36:45.427Z Reads: 30

```
also that is too high for 6s, you'll be on half power.

3.3*6 start
3.5*6 end
is the usual.
```

---
## \#17 Posted by: Charster10 Posted at: 2016-11-28T19:15:38.103Z Reads: 22

```
Yes i know there too high but i got that off google just to show you...also what do you mean leading 2's?
```

---
