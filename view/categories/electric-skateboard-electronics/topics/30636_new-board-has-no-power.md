# New Board has no Power

### Replies: 7 Views: 668

## \#1 Posted by: mitchell898 Posted at: 2017-08-14T21:35:39.583Z Reads: 80

```
I just finished putting together my board and I can't figure out why it has no power. 
Parts I used:

Sk3 190kv 63mm motor
VESC
Two Zippy 5000mah 25c batteries
Torque boards remote

The batteries are charged and the motor will spin but has almost no power. (not enough to push the board by itself) 
The Vesc has not been programmed aside from the factory settings.

Any ideas??
```

---
## \#2 Posted by: tueboard Posted at: 2017-08-14T21:37:23.287Z Reads: 79

```
maybe this can help..
http://www.electric-skateboard.builders/t/help-the-motor-cant-handle-the-board-weight/8053
```

---
## \#3 Posted by: jammin Posted at: 2017-08-14T21:37:30.317Z Reads: 75

```
program your vesc, my build is very similar and it works no prob after calibration
```

---
## \#4 Posted by: mitchell898 Posted at: 2017-08-14T21:39:03.782Z Reads: 74

```
Okay sweet thanks! I'll post an update soon.
```

---
## \#5 Posted by: darkkevind Posted at: 2017-08-14T22:10:30.717Z Reads: 59

```
It's almost definitely your voltage cut off levels...

How many cells in series do you have?
```

---
## \#6 Posted by: mitchell898 Posted at: 2017-08-15T01:23:11.302Z Reads: 37

```
Changed the cut off values and it runs beautifully.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-08-15T01:30:23.419Z Reads: 33

```
Thought so.... :thumbsup:
```

---
