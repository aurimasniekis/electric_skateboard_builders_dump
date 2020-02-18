# Vesc goes full throttle when remote disconnects?

### Replies: 6 Views: 846

## \#1 Posted by: chewydinosaurs Posted at: 2017-08-16T00:09:09.926Z Reads: 115

```
I assume it's somewhere in my settings, but I set up a mini controller yesterday and to test what would happen I turned the board on with the remote on, then turned the remote off and the receiver started flashing since it obviously lost signal but then the board went full throttle forwards? Here's my v<img src="/uploads/db1493/original/3X/9/7/979067e8886261b7054f18b67ec8810bce12ad73.PNG" width="690" height="356">esc settings
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-08-16T00:25:57.987Z Reads: 108

```
You need to adjust the failsafe of your remote. 
At most remotes it can be adjusted by adding the bind plug to the receiver, switch the board and remote on and remove the bind plug while the remote is still on. By this the receiver knows what default signal it should use if it doesn't have a connection to the remote.
```

---
## \#3 Posted by: lrdesigns Posted at: 2017-08-16T01:31:40.312Z Reads: 96

```
Yeah the receivers fail safe needs to be setup to send a neutral command to the vesc when the signal is lost. Which remote do you have exactly? Did it come with any instructions, if so it should say how to set the fail safe?
```

---
## \#4 Posted by: chewydinosaurs Posted at: 2017-08-16T02:04:18.232Z Reads: 89

```
It's this one here: diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/

It said to center the trims (which were indeed centered) so I assumed it was set up correctly however I'll try again
```

---
## \#5 Posted by: saul Posted at: 2017-08-16T03:16:02.146Z Reads: 79

```
you need to adjust the trim so the remote neutral is the same as the off neutral.

so you can disable control. and then click the remote on/off a few times and the display pwm should be about the same. a small difference can be taken out with deadzone setting. 

adjust the min max so that the center is the center.  
the signal can go to 2200ms sometimes and as low as 900. you need to cover the full range, vesc ignores input out of range, this will cause more problems...
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-08-16T03:25:02.600Z Reads: 69

```
your deadband needs to be 0.15  
it happen to me before with that remote. it has some bug. I wrote  0.10 and rewrite 0.15 
see if this works
```

---
