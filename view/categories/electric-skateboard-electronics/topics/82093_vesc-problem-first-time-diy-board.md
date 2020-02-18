# VESC Problem - First time DIY board

### Replies: 7 Views: 175

## \#1 Posted by: badger4life Posted at: 2019-01-26T01:03:19.374Z Reads: 70

```
I'm setting up my first DIY board and I'm running into issues with one of the VESCs not turning the motor that it's attached to.  I know the motor is OK because I've hooked it up to the other VESC and it spins.  I've also hooked the problematic VESC to my second motor and it won't spin that motor either.

I'm running a split PPM set up I think...  I have a remote and two receivers, one receiver for each VESC.


Here is some info from my troubleshooting:

-When I press the throtle on the remote both VESCs have a green LED on the VESC board that lights up (telling me that the signal is being passed to the VESC).

-I've hooked the VESC up to the vesc_tool_0.95 software and when I press the "Start detection" button on the BLDC page the motor will spin up.

So basically it seems to me that the remote signal is being received by the VESC and the motor will spin when hooked up to the vesc_tool_0.95 software, but when I press the throttle on the remote the motor won't spin.

Any ideas or help would be greatly appreciated.
```

---
## \#2 Posted by: TowerCrisis Posted at: 2019-01-26T01:20:26.248Z Reads: 58

```
Have you tried cloning the settings from the vesc that works and uploading them to the vesc that isn't? That way you can rule out any accidental settings problem.
```

---
## \#3 Posted by: badger4life Posted at: 2019-01-26T01:26:11.252Z Reads: 54

```
I'll give that a try now, thanks.
```

---
## \#4 Posted by: badger4life Posted at: 2019-01-26T01:45:33.212Z Reads: 52

```
@TowerCrisis That did it, thank you!!!!

Also, I think the setting that was different was the Safe Start setting.  It was set to false on one VESC and true on the other.
```

---
## \#5 Posted by: linsus Posted at: 2019-01-26T01:52:49.025Z Reads: 49

```
For future refrence, if you see a red LED flashing, type "faults" into the Vesc tool terminal to see whats wrong
```

---
## \#6 Posted by: badger4life Posted at: 2019-01-26T01:53:34.946Z Reads: 47

```
Thanks, will do.
```

---
## \#7 Posted by: TowerCrisis Posted at: 2019-01-26T08:35:42.214Z Reads: 28

```
That's great! Congrats on getting it working, good luck on your build
```

---
