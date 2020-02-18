# Dual motors, only one of them sensored?

### Replies: 6 Views: 481

## \#1 Posted by: Brando Posted at: 2017-09-08T21:09:33.411Z Reads: 110

```
I have a very odd specific problem. I have two 6355 motors from buildkitboards. They come with sensor wires, but get this, one decided to come lose (my fault, I know😂). It ended getting caught under the wheel and was yanked out.

My thought is this, I put the sensored motor in hybrid mode, so that it helps get the board going, then as soon as it passes the erpm limit, both motors will run unsensored together.
FYI I have 2 VESCs connected by canbus. Is this a terrible idea? I miss smooth startups.
```

---
## \#2 Posted by: mkeboard Posted at: 2017-09-08T22:17:21.357Z Reads: 104

```
Maybe not the answer you're looking for, but if you contact buildkitboards, he might be willing to send you new sensor wires or the pcb. It would be a good chance to learn how to fix motors. I've never done this before though so it might be a bit more complicated than that.
```

---
## \#3 Posted by: bigben Posted at: 2017-09-08T22:20:13.784Z Reads: 102

```
I've run motors like this but with split transmitter signal not canbus.
It didn't turn out to be a problem for me.
```

---
## \#4 Posted by: Brando Posted at: 2017-09-09T02:00:34.524Z Reads: 82

```
That's what I'm worried about. I think the canbus will get confused. What happened to your board? Why did it only have one sensor?
```

---
## \#5 Posted by: onloop Posted at: 2017-09-09T02:13:24.561Z Reads: 80

```

this will work fine, can setup each vesc independently. sensor-hybrid-master + non-sensor-slave can even play with start boost on non-sensor side.
```

---
## \#6 Posted by: bigben Posted at: 2017-09-09T07:16:41.088Z Reads: 53

```
For some reason in the new vesc tool the sensors wouldn't detect on one motor. Switched to FOC now however and it runs perfectly detecting both motors.
```

---
