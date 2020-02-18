# Failed motor detection VESC

### Replies: 3 Views: 481

## \#1 Posted by: aotr Posted at: 2016-11-04T08:54:30.809Z Reads: 65

```
Hi!

I am trying to set up my VESC to my motor. i can connect to my VESC to BLDC tool just fine, but when i do motor detection it fails. It does not even spin up. I have tried adjusting the "current" and the "ERPM" settings, but nothing. Can i have wired the motor wrong?
```

---
## \#2 Posted by: ra.rend Posted at: 2016-11-04T12:45:35.709Z Reads: 55

```
what's your setup?
```

---
## \#3 Posted by: chaka Posted at: 2016-11-04T14:04:20.068Z Reads: 43

```
Check your low voltage cutoff. Some vendors send them with presets for 10s li-ion instead of the default 8v setting. If your battery is lower voltage than you will need to reset the cutoff before running detection.
```

---
