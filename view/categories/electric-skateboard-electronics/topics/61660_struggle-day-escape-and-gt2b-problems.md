# STRUGGLE Day - Escape and GT2B problems

### Replies: 10 Views: 224

## \#1 Posted by: ElskerShadow Posted at: 2018-07-12T15:51:23.267Z Reads: 107

```
Noob thread.
I've spent my whole day trying to update one of my build. It was long and boring I had a tons of minor problems. Anyway it's been literally 2 hours that I am struggling to calibrate a remote on the VESC Tool. 
So far I have tried :
3 x GT2B 
2 x nano X 
1 x winning 

All the remote binds, I have the solid lights etc etc... But never a single pulswidth on the VESC tool. It's so infuriating. I tried all the combinaisons I could imagine. Nothing works.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-07-12T15:58:46.165Z Reads: 101

```
You sure you plugged in to the right channel on the receiver and the pins on the escape in the right order?
```

---
## \#3 Posted by: BigBrit Posted at: 2018-07-12T16:00:26.692Z Reads: 100

```
You have this if you have the receiver plugged in the wrong way round.  Turn the plug 180 degrees
```

---
## \#4 Posted by: ElskerShadow Posted at: 2018-07-12T16:20:06.219Z Reads: 94

```
![1531412338197|375x500](upload://xov9JgEhdNnz9IlapHW1Qc1brtj.jpg)
![1531412388229|375x500](upload://tq0oeG4zj1xfaIFU8tnoIA1vq8c.jpg)
```

---
## \#5 Posted by: ElskerShadow Posted at: 2018-07-12T16:20:49.810Z Reads: 84

```
I have done this 50 time already unfortunately
```

---
## \#6 Posted by: Andy87 Posted at: 2018-07-12T16:36:00.661Z Reads: 81

```
Stupid question, but you set your escape to ppm mode?
```

---
## \#7 Posted by: Silverline Posted at: 2018-07-12T16:36:44.535Z Reads: 80

```
Throttle is on channel 2 and not 1
```

---
## \#8 Posted by: i2oadsweepei2 Posted at: 2018-07-12T17:33:37.596Z Reads: 63

```
Like @Silverline said. Rc remotes channel one is for steering and 2 for throttle. Esk8 specific remotes like nano-x use channel 1 for throttle. It’s an easy mistake. Hope it all goes well for you.
```

---
## \#9 Posted by: ElskerShadow Posted at: 2018-07-12T18:31:34.160Z Reads: 57

```
It's an impression on the picture but the cable was plugged into ch 2
Anyway the issue was solved but don't know how, it just suddenly worked when I tried the same procedure on the other Escape, I have tried again on the other one and it's not working so I guess the ppm port of my second escape has a cold joint or something!
```

---
## \#10 Posted by: Kuchi Posted at: 2018-07-12T21:56:45.939Z Reads: 45

```
Have you adjusted your min and max on the vesc tool and turned on the readers
```

---
