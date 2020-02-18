# Different motor settings

### Replies: 6 Views: 215

## \#1 Posted by: yanggatang Posted at: 2019-01-12T22:30:28.638Z Reads: 94

```
I was wondering if I am running split ppm, can I have two different settings for the motors for the VESC?
```

---
## \#2 Posted by: e.board_solutions Posted at: 2019-01-12T22:31:20.856Z Reads: 92

```
yes you can :slight_smile:
```

---
## \#3 Posted by: mynamesmatt Posted at: 2019-01-13T02:40:29.771Z Reads: 64

```
you can yes, but why?
```

---
## \#4 Posted by: yanggatang Posted at: 2019-01-13T07:32:03.013Z Reads: 52

```
one motor seems to be slower when I ride it and i just wanna up the motor max settings to 60 from 50
```

---
## \#5 Posted by: Friskies Posted at: 2019-01-13T08:22:18.336Z Reads: 45

```
How do you know that it is actually running slower? Throwing more amps isn't going to fix your problem. You should try re-calibrating the ppm on that particular vesc(I assume you are using vesc).
```

---
## \#6 Posted by: mynamesmatt Posted at: 2019-01-13T12:33:53.000Z Reads: 30

```
upping motor current will only increase torque (acceleration) not top speed. redo your motor detection, and make sure both vescs are set to a maximum duty cycle of 95. if you up the current on one motor you will experience minor torque steer similar to a single motor would
```

---
