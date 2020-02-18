# Motor spins the opposite direction randomly

### Replies: 6 Views: 226

## \#1 Posted by: achatham Posted at: 2019-09-24T01:03:32.823Z Reads: 74

```
On my recent dual motor build one of the two 6355 motors will every now and then spin the opposite direction on start. After a little throttle it then will then spin back the right direction (forward). Im running on a focbox unity. Does this sound like a phase wire issue?
```

---
## \#2 Posted by: kchxaz Posted at: 2019-09-25T18:07:49.607Z Reads: 44

```
Sounds like an issue I am having currently. Not likely your motors.

What brand/model VESC are you using?
```

---
## \#3 Posted by: Deodand Posted at: 2019-09-25T18:28:03.801Z Reads: 42

```
This can happen if you are running an uncensored motor sometimes. If it has hall sensors make sure they are detected properly.
```

---
## \#4 Posted by: RyEnd Posted at: 2019-09-25T18:58:28.069Z Reads: 37

```
Yeah, try switching up your phase wires as well. Has worked for me to smooth things out in sensorless setups.
```

---
## \#5 Posted by: kephart Posted at: 2019-10-13T19:53:47.016Z Reads: 24

```
This happens to me as well. Not a big problem though. It gets the idea with a little more throttle, or if you start with a moving board.
```

---
## \#6 Posted by: xsynatic Posted at: 2019-10-13T20:32:06.520Z Reads: 22

```
This problem happened to me when i had the phase wires wrong and just changed it via the VESC tool.
That way it turned still the wrong direction at first but jumps back to the now correct direction.
So Motor phase wires are plugged in that the Motor spins backwards. Changed it via software so the Motor turns forwards. Problem was gone after i used a different phase wire combination.
```

---
