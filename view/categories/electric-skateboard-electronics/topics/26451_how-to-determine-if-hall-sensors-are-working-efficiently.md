# How to determine if Hall sensors are working efficiently?

### Replies: 14 Views: 962

## \#1 Posted by: evoheyax Posted at: 2017-06-30T17:53:42.241Z Reads: 190

```
Hey community. Does anyone know of an easy way to test if the hall sensor is positioned in such a way that the motor runs efficiently?

I did notice that I can start from a standstill way better than before and I can't get that motor to stall on start, unlike the other 3 unsensored motors. So it seems to work. But I'm not sure how well and how to determine "how well".

Any help is much appreciated!!!
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-30T18:20:56.330Z Reads: 186

```
While I don't know the answer to this, you can use the VESC's hybrid mode to disable the sensors after you get started, then they don't have any affect at all.
```

---
## \#3 Posted by: evoheyax Posted at: 2017-06-30T18:21:35.911Z Reads: 181

```
Theres no hybrid mode as far as I can tell in FOC though...

Theres Encoder, Hall or Sensorless mode. The Hybrid mode is in BLDC :(
```

---
## \#4 Posted by: Blasto Posted at: 2017-06-30T18:43:53.513Z Reads: 174

```
In foc the sensors disable after a certain erpm (sensorless erpm in the foc tab) so the halls are only used for startup
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-30T19:01:05.598Z Reads: 167

```
Yep as blasto said, FOC has hybrid as well. For testing I'd say do every possible phase wire orientation then run detection, see if hall detection fails in any order.
```

---
## \#6 Posted by: evoheyax Posted at: 2017-06-30T19:39:36.203Z Reads: 164

```
Ok, thanks guys. So far, all looks good. So I epoxied the first motors, and will check again after they are set.
```

---
## \#7 Posted by: evoheyax Posted at: 2017-06-30T23:34:32.759Z Reads: 149

```
First motor seems ok, no issues. Just wired up the second motor and now it's giving me a bad detection result. The test seems good watching the motor though. It spins very slowly in one direction, followed by the same in the opposite direction. It just says bad detection with the red background after the test. Any ideas? 

I checked the wiring and it's all correct as far as I can tell...
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-30T23:58:33.492Z Reads: 139

```
How about bldc detection, same hall detection results?
```

---
## \#9 Posted by: evoheyax Posted at: 2017-07-01T00:15:25.985Z Reads: 136

```
I actually fixed it some how. I re positioned them again in the same spot and now detection is good. I checked carefully for any damaged pins or wires, but everything seemed good. So I epoxied them and ran it again to make sure they were positioned correctly. Everything seems good so I'll wait an hour for it to set, and then put the motor back together. So 2 motors down, 2 more to go :)
```

---
## \#10 Posted by: evoheyax Posted at: 2017-07-01T04:04:41.338Z Reads: 122

```
My first motor seems really good. The second one though is stuttering a bit. It gets good results and fails 50/50. Any ideas on the jitteriness? I can't move the sensors anymore since they are potted in epoxy.
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-01T04:43:47.366Z Reads: 119

```
So you're saying detection succeeds but the hall part fails? I've seen that happen as well, though not sure what causes it. Fortunately for me, it hasn't affected my rides negatively.
```

---
## \#12 Posted by: evoheyax Posted at: 2017-07-01T06:45:44.802Z Reads: 111

```
It always passes detection, but 50/50 pass/fail on the hall sensor detection.
```

---
## \#13 Posted by: Tinp123 Posted at: 2018-09-04T07:41:54.124Z Reads: 66

```
@evoheyax what did you do with your sensor with 50/50 bad detection? did you somehow solve it so it doesn't stutter anymore?
```

---
## \#14 Posted by: evoheyax Posted at: 2018-10-04T20:25:32.560Z Reads: 54

```
I gave up on these motors after testing them for about a year. They were simply too small and I needed larger motors. So now we have the hummie v4's!
```

---
