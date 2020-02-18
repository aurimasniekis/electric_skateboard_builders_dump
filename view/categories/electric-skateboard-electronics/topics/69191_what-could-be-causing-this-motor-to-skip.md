# What could be causing this motor to skip?

### Replies: 9 Views: 156

## \#1 Posted by: Jcullinan09 Posted at: 2018-09-25T22:19:32.444Z Reads: 60

```
Not sure why, but upon doing a motor detection I can't get this one motor to detect. 

![08%20PM|690x201](upload://uV6beXkG1eJZtULqk3wloPkivbz.png) 

https://photos.app.goo.gl/AHhUJEj7gdZ4zLA39
```

---
## \#2 Posted by: mishrasubhransu Posted at: 2018-09-25T23:14:17.017Z Reads: 47

```
increase amps from 5 to 10 and try again.
```

---
## \#3 Posted by: notepad Posted at: 2018-09-26T00:04:22.888Z Reads: 46

```
Not going to lie.  If the motor is securely mounted, id detect with the full amperage your going to use to get the most exact detection.
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2018-09-26T00:12:12.998Z Reads: 41

```
Its not the amps, increase the duty cycle(D) from 0.05 to 0.15
```

---
## \#5 Posted by: Schulerbible Posted at: 2018-09-26T01:07:45.955Z Reads: 31

```
Are your settings in BLDC or FOC? My Vescs didn't detect the motors until I discovered that my setting was on FOC rather than BLDC!  

![image|683x345](upload://cCVdbU9JxebB4xhpSTVphAWg8kq.jpeg)
```

---
## \#6 Posted by: Jcullinan09 Posted at: 2018-09-26T01:20:11.318Z Reads: 27

```
I havent been using BLDC tool. Some guys yesterday suggested I try ACKMANIAC's ESC tool so I've been running bench tests using the ESC tool not BLDC tool.
There should be an option to switch to FOC on ESC tool. Let me check.
```

---
## \#7 Posted by: Jcullinan09 Posted at: 2018-09-26T01:22:12.069Z Reads: 25

```
@ARetardedPillow I think you're suggestion worked increasing the duty cycle to 0.15. BUT for whatever reason, now the damn thing sputters at roughly 15% duty in the negative x direction. Imma bout to throw the thing out the window :sweat_smile:

UPDATE: Never mind @Schulerbible got it. Just switching to FOC made it work like a charm. Not sure why but its functioning as it should now.
```

---
## \#8 Posted by: mmaner Posted at: 2018-09-26T01:24:12.491Z Reads: 26

```
Get a hammer, more fun 😀. 

Power everything down, reset to defaults and retry detection in bldc 1st, when that's successful then try FOC. If it doesn't work increase the sure cycle to . 1. Over that and your risking the VESC in the bench.
```

---
## \#9 Posted by: Jcullinan09 Posted at: 2018-09-26T01:26:24.386Z Reads: 26

```
@mmaner Thank you for the advice! Apparently FOC has it functioning at the moment.
```

---
