# Raptor 1 brake locked after upgrading to Nano-X

### Replies: 8 Views: 644

## \#1 Posted by: bucksd Posted at: 2017-11-03T20:05:01.199Z Reads: 97

```
I updated to the Nano-X on my Raptor 1 and now the brakes are always on when the throttle is in the neutral position. 

I need to apply a little 'acceleration' on the throttle in order to find 'neutral' to allow the board to coast. 

I read something about going full-acceleration and then full-brake to 'reset' it or something, but that hasn't worked. How do I fix it? I think I need to tell the thing where neutral is on the remote, cause it seems to think I want to brake all the time...
```

---
## \#2 Posted by: cwazy1 Posted at: 2017-11-03T20:20:35.406Z Reads: 90

```
Did you go into your BLDC tool and change the ppm settings? You can't just change remotes without changing the min pulse width and max pulse width
```

---
## \#3 Posted by: bucksd Posted at: 2017-11-03T20:26:52.673Z Reads: 90

```
I did not. Never used BLDC before. I connected my Macbook Air to the Raptor 1 via a mini USB cable but the BLDC tool isn't showing the board as an available serial connection, it just shows some bluetooth devices. I think it might be a charge-only mini USB cable I'm using...
```

---
## \#4 Posted by: Skitzor Posted at: 2017-11-03T20:40:10.073Z Reads: 74

```
And I'm not sure if it's a setting on the R2 cause I'm still patiently waiting, but the nano X on the R2 needs to be calibrated every time you boot your board. A simple full front and back movement after connection should establish this. (Someone correct me if that's a firmware setting from the R2 and not needed otherwise)

Second part:
[quote="cwazy1, post:2, topic:37271"]
You can't just change remotes without changing the min pulse width and max pulse width
[/quote]
So try and find a good mini usb cable and connect to the BLDC tool, adjustment of the PPM settings there should solve this too
```

---
## \#5 Posted by: cwazy1 Posted at: 2017-11-03T20:59:32.944Z Reads: 61

```
Yes, you'll need to find a mini USB with all 4 connections in the USB plug, versus the 2 connections for charge only USB. 

Also to @Skitzor's point, it is best to always flick full throttle and full brake on controller (while its on, duh) before turning on the board to pair the remote to board. This enables the full throw of the controller. If you don't do this, you'll still have a functioning controller, but you'll only be able to use approx 50% of the full pulsewidth of the remote. THIS APPLIES TO ALL NANO/WINNING CONTROLLERS. 

But also to skitzor's point, 'trimming' a nano controller before use will NOT result in a misaligned center pulsewidth and is irrelevant to OP's problem. Trimming a nano controller before each use is just something that will increase the pleasure of use of your controller.
```

---
## \#6 Posted by: Skitzor Posted at: 2017-11-03T21:09:18.532Z Reads: 55

```
Thank you sir for pointing out
```

---
## \#7 Posted by: scepterr Posted at: 2017-11-03T21:44:11.529Z Reads: 52

```
I never have to calibrate my nano-x, either of the 2 I have.
Just on and go.
```

---
## \#8 Posted by: cwazy1 Posted at: 2017-11-03T21:46:34.955Z Reads: 50

```
yeah, you don't have to. I also usually just on and go.
```

---
