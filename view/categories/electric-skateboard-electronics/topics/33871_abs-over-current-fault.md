# Abs over current fault

### Replies: 8 Views: 775

## \#1 Posted by: ARetardedPillow Posted at: 2017-09-24T19:25:09.954Z Reads: 90

```
The vesc shuts off mid ride after around 5 minutes all the time and I got it to shut off when I was near home so I plugged it in bldc tool and i get this
<img src="/uploads/db1493/original/3X/0/0/008fcadcad5079b544bd11d0cc30e19ae9192f4e.png" width="293" height="500">.
My settings are this this
<img src="/uploads/db1493/original/3X/8/4/8401f34a3ce35f8b863116861a73f3243443b32a.png" width="690" height="400">
I have no Idea whats wrong help would be appreciated
```

---
## \#2 Posted by: Jinra Posted at: 2017-09-24T19:28:29.091Z Reads: 84

```
Battery max is too high, the vesc only handles 50 continuous, but you should try out 40 first to be safe
```

---
## \#3 Posted by: Martinsp Posted at: 2017-09-24T19:29:04.052Z Reads: 84

```
Often times this is caused by loose connections from the VESC to the motor, check that in case lowering the current from battery does not work.
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2017-09-24T19:32:27.060Z Reads: 87

```
It was at 40A before and it still cut off like how it does now, and all the connections are good and dandy, @scepterr did all the gucci soldering.
The vesc runs good for about 500 feet and then just dies, and I have a 10s setup
```

---
## \#5 Posted by: scepterr Posted at: 2017-09-24T19:52:00.775Z Reads: 84

```
I set your settings to 40A, tweak down not up ;) 40A was already high. And I set your battery max to 25A I believe....
Run detection a couple times and reapply.
Let me know if there are drastically different results between detections
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2017-09-25T03:51:17.468Z Reads: 75

```
Tweaked down most of my settings, vesc stops after a quarter of a hill and get really hot
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2017-09-25T03:54:28.336Z Reads: 72

```
dropped bat max to 25 and bemf to 850
```

---
## \#8 Posted by: Silverline Posted at: 2017-09-25T07:30:24.927Z Reads: 65

```
Maybe you have a short in the motor ??

Du you have a LC meter, so you could measure on the motor wires ?
```

---
