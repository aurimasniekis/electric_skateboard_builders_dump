# Sk3 sensorless stutters in bldc tool

### Replies: 6 Views: 399

## \#1 Posted by: telnoi Posted at: 2017-09-28T05:03:50.479Z Reads: 74

```
Lots of topics on stuttering, but could not find a description of a similar issue.

I replaced a maytech motor with a sk3 (149kv, big hills around here and I am 1.87m). Motor detection went fine and using the keyboard arrows the motor moves fine. However, if I command the motor too quickly after stopping, it will stutter. I then have to wait for a few seconds before giving another throttle command.

I have a second new motor to test with and it behaves identical. Is this just due to sensorless? 

Motor detection was done without anything connected to the motor/no load, no pulley.
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-28T05:09:15.932Z Reads: 74

```
Increase Current A in detection and/or min erpm
Oh wait your detection was fine,
Is ppm calibrated?
Can also try increasing startup boost
```

---
## \#3 Posted by: telnoi Posted at: 2017-09-28T05:14:54.163Z Reads: 73

```
Not using my remote yet. The stuttering happens when I use the arrow keys to for example change motor direction with the Vesc connected to the bldc tool, thus still no load.

Only happens when there is not enough time in between keyboard commands, though I am uncertain if this behaviour will cause issues in the field when riding.
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-28T05:36:23.254Z Reads: 62

```
I would certainly confirm it's an actual issue 😉
```

---
## \#5 Posted by: telnoi Posted at: 2017-09-28T05:41:41.625Z Reads: 59

```
Hoping to prevent blowing up two 200€ VESCs before testing it in the field
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-28T05:45:45.491Z Reads: 57

```
Did you try increasing startup boost?

Still..you could be trying to fix a problem that doesn't exist which could actually cause a problem.
```

---
