# Re: DRV8302, help autopsy! Pictures

### Replies: 13 Views: 615

## \#1 Posted by: Nix Posted at: 2017-10-01T23:42:39.652Z Reads: 148

```
Hi... There was a similar post to this but I forgot to add photos... 
2days prior on my first real ride, I used the DIYes Vesc 4.12, new, on 12 mph , for about 1/4 miles. I turned it on yesterday and the motor had more resistance than usual as it moved in steps... I connected it, and pulled the trigger, and the motor moved, glitched, and stopped. Then it never worked after that. I check in the bldc tool the motor detection and it failed multiple times, and I checked the faults and it told me the DRV8302 basically failed. I run 6s with 200kv motor, and an DIYes 4.12 vesc. Can anyone help me figure out what happened? There are pictures if they help<img src="/uploads/db1493/original/3X/1/4/141548ce4f81ed17042a8838f7abd7f28382b60c.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/9/0/90fc8bbe08cbc521b9dbf6bc345643eb0958a9a3.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/9/e/9e16f937ed1b3397633cba0274c0cb07ef12082b.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/6/d/6d28dd9c517d4b58d509daa4d9d055132f43e0da.jpg" width="374" height="499">
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-02T03:44:18.855Z Reads: 121

```
Impossible to tell anything from the pictures , too blurry. The one thing I can say for the future if you manage to spot that the motor isn't spinning freely do NOT try to throttle it...disconnect the motor, if the problem is still there, then check that your phase leads aren't shorting nor are the screws holding your motor to the mount. If the motor is fine as soon as you unplug then it's something with the vesc.
```

---
## \#3 Posted by: jmasta Posted at: 2017-10-02T04:26:43.466Z Reads: 113

```
http://i.imgur.com/kSra8VV.jpg
```

---
## \#4 Posted by: Nix Posted at: 2017-10-02T11:30:17.044Z Reads: 94

```
@scepterr I unplugged the vesc and nothing happened and then I loosed the mounting screws and it turned fine. It failed multiple motor detections when I plugged it back in and then when I type in faults of the terminal tab it told me something was wrong w/ DRV8302... I can update the pictures to higher quality later on in the day. Thanks!
```

---
## \#5 Posted by: karma Posted at: 2017-10-02T15:40:19.040Z Reads: 75

```
Clean your lense and adjust the focus to focus on the thing you want us to see.
```

---
## \#6 Posted by: karma Posted at: 2017-10-02T15:41:55.394Z Reads: 74

```
Your DRV probably blew. Any chance the phase wires contacted?
```

---
## \#7 Posted by: Nix Posted at: 2017-10-02T18:43:26.902Z Reads: 61

```
I don't think they did? The heatshrink should prevent that
```

---
## \#8 Posted by: scepterr Posted at: 2017-10-02T19:10:22.135Z Reads: 56

```
Does the motor spin freely when unplugged?
```

---
## \#9 Posted by: Nix Posted at: 2017-10-03T02:17:04.998Z Reads: 48

```
I didn't until I had to release the motor mount screws
```

---
## \#10 Posted by: i2oadsweepei2 Posted at: 2017-10-03T11:13:05.531Z Reads: 36

```
If it's spins better with the mounting screws loosened then they are too long and we're touching the windings. That is and was the problem. It would be very similar if the phase wire shorted on the can. So many people make the mistake when the motor has trouble spinning they pull the trigger more to force it to and poof!! Sounds like you blew the drv chip and need a repair. Post where you are located and hopefully someone can recommend a place to get it repaired.

If you are/were using 12mm long m4 screws order some 10mm.
```

---
## \#11 Posted by: Nix Posted at: 2017-10-03T11:27:40.397Z Reads: 33

```
Wow thanks for the information! Could this ruin my motor? And im working on getting it fixed.
```

---
## \#12 Posted by: i2oadsweepei2 Posted at: 2017-10-03T13:27:21.639Z Reads: 30

```
It's unlikely but not impossible. Not connected to the vesc and with the phase wires not touching each other if it spins freely and smoothly with no odd noises then it's probably fine. Also if it's not a sealed motor you can and should look through the slots at the end under a light and see if any of the windings are noticeably l damaged.
```

---
## \#13 Posted by: Nix Posted at: 2017-10-03T13:39:24.204Z Reads: 32

```
Thanks!
10 char
```

---
