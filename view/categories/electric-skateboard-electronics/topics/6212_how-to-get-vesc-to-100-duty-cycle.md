# How to get vesc to 100% duty cycle?

### Replies: 4 Views: 1304

## \#1 Posted by: Hummie Posted at: 2016-07-16T17:51:37.589Z Reads: 179

```
im stuck at 95% 
something on the bldc tool its not adjusting on the remote
```

---
## \#2 Posted by: treenutter Posted at: 2016-07-16T22:39:39.703Z Reads: 165

```
@Hummie how are you measuring this? Is it a problem with the max/min PPM settings for your remote? If you're not able to hit 100%, try adjusting the trim of the throttle on your remote first, and then tweaking the max and min PPM inputs.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2016-07-17T06:45:05.636Z Reads: 139

```
You can't, vedder explain this somewhere, something to do with the VESC 4.x only having current measurement on 2 phases (2 shunts) so it need at least some time with the transistors off so it can measure que current flow
```

---
## \#4 Posted by: Hummie Posted at: 2016-07-17T16:05:33.455Z Reads: 120

```
Ooo.  Yea I tried the transmitter trims
```

---
