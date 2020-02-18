# VESC controller configuration

### Replies: 5 Views: 431

## \#1 Posted by: MrCheatak Posted at: 2018-06-10T12:03:28.635Z Reads: 94

```
So, I'm a newbie eSk8 builder, though it's my second build, but my first acquaintance with VESC. 
Everything seem to be working as intended (and I absolutely love that soft startup) except these two things:
1) There is a Timeout option that is supposed to stop Motor when there's no signal from controller, but when I switch remote off, motor still tries to kill me. I looked all VESC tool through, but haven't found any similar setting
2) I can't figure out how to disable brakes when motor is still. They are not applied when I choose current control, but always work when its duty cycle control. Also green LED is always on when it's duty cycle and on current it goes bright only when I pull the trigger.

Second one is not critical, though I'd like to save battery life and not struggle so much if I had to pull esk8.
```

---
## \#2 Posted by: willumpie82 Posted at: 2018-06-10T20:21:30.146Z Reads: 80

```
What kind of remote controller are you using? My guess is that your receiver keeps pushing the same setpoint when connection is lost. If it is an rc-style controller you might have to setup some kind of failsafe on the receiver
```

---
## \#3 Posted by: MrCheatak Posted at: 2018-06-10T20:54:05.814Z Reads: 72

```
It's torqueboards mini remote. I haven't found anything but binding instructions. 
You mean VESC just doesn't see that connection is lost?
```

---
## \#4 Posted by: willumpie82 Posted at: 2018-06-11T04:56:31.953Z Reads: 50

```
Correct, check with vesc connected to your computer what the signal does (enable RT APP) when you switch off the controller.
Check this thread on the exact binding procedure
http://www.electric-skateboard.builders/t/fail-safe-on-mini-remote-not-working/31104/3
```

---
## \#5 Posted by: MrCheatak Posted at: 2018-06-11T08:25:07.315Z Reads: 41

```
I did that and it showed, that VESC recieves a specific ms value. 
Adjusted throttle so that center value is same with "no signal" one. Seems to be working like this.
```

---
