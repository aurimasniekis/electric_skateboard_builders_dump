# Brakes cutting out - Focbox Unity

### Replies: 10 Views: 307

## \#1 Posted by: ajplant96 Posted at: 2019-06-09T11:51:02.352Z Reads: 120

```
So I have one last issue before I consider my rebuild complete. Spent the last hour or so searching for answers but haven’t been able to find anything specific enough to help. When I’m moving at speed >20kmph, the brakes applied more suddenly than gradually are cutting out. I’m thinking it could be something to do with my max braking currents. Can anybody offer any advice? Current settings are as follows...

Max battery discharge: 50A
Max braking regen -15A
Max motor: 50A
Max brake: -25A
```

---
## \#2 Posted by: McErono Posted at: 2019-06-09T12:06:38.803Z Reads: 118

```
What battery setup (xSxP)? Regen is highspeed brakes, max brake is lowspeed brake.
```

---
## \#3 Posted by: ajplant96 Posted at: 2019-06-09T12:08:28.462Z Reads: 116

```
10s4p totalling 10.4A I believe it was
```

---
## \#4 Posted by: Friskies Posted at: 2019-06-09T12:27:36.447Z Reads: 110

```
What are the specs of the BMS? How is the BMS wired?
```

---
## \#5 Posted by: ajplant96 Posted at: 2019-06-09T12:30:37.953Z Reads: 105

```
All I know about it is 10s, rated for 60A, wiring should be done correctly (was done by my battery builder - I don't understand the whole thing)
```

---
## \#6 Posted by: dareno Posted at: 2019-06-09T12:41:13.813Z Reads: 99

```
regen looks ok and I wouldn't mess about with that till you know what cells you have and the specs of the bms.  Try upping the max brake.  Its a little low.  Try going up in small increments ie; 5A to start with.  Other than that it may be a remote calibration issue.  Got some testing to do my friend.  Welcome to diy
```

---
## \#7 Posted by: ajplant96 Posted at: 2019-06-09T12:48:09.156Z Reads: 98

```
Sweet, I’ll start tweaking more tomorrow, thank you. Haha, I knew it was gonna take some learning and tedious tasks, fortunately for a lot of it I’ve had a mate help since he’d done the same build expect old focboxes instead of the unity. I may actually try my other remote too now then (nano-x, I prefer the flipsky vx1 though)
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-06-09T13:01:49.019Z Reads: 101

```
that battery seems weird, you said it was 10s4p, 10.4ah total meaning the cells that would be used are 2600mah and 12.5A discharge?
```

---
## \#9 Posted by: ajplant96 Posted at: 2019-06-09T22:10:34.179Z Reads: 68

```
Cells are 2600MAH btw, they’re unbranded but have been reliable, and only temporary anyway as I’m switching to a 10s5p with Samsung 30q cells in a few weeks.
```

---
## \#10 Posted by: ajplant96 Posted at: 2019-06-10T02:27:11.618Z Reads: 53

```
Solved the issue, was drawing too many amps for what the battery currently is so I’ve just dropped down to 40/-20 and -10 for the regen. Thanks everybody for your input. ☺️
```

---
