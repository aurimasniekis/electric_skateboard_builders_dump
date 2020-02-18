# VESC doesnt boot up when I connect hall sensors to it

### Replies: 4 Views: 324

## \#1 Posted by: orkunturkey Posted at: 2017-12-12T09:01:23.741Z Reads: 59

```
7+6So I salvaged these hub motors from an unbranded esk8 and hooked them up to a VESC. Things seem to be working almost okay, with one problem being the top speed compared to the unbranded skateboard the hubs originally belonged to, another being the startup clogging. I believe that the issue would be resolved if I could get the hall sensors to work (6pin) but when I hook the sensor on the VESC, VESC does not show up on the BLDC tool. Anyone faced similar issues and know any ways to troubleshoot?
```

---
## \#2 Posted by: Martinsp Posted at: 2017-12-12T11:14:12.158Z Reads: 51

```
What do you mean does not boot up? That you can not connect to the vesc using bldc tool or that the vesc does not turn on at all.
```

---
## \#3 Posted by: JTAG Posted at: 2017-12-12T13:20:26.843Z Reads: 43

```
Are you sure the hal sensors are connected with the correct power supply polarity? Sounds like you might be shorting the 3v3 power rail.
```

---
## \#4 Posted by: orkunturkey Posted at: 2017-12-12T13:56:48.920Z Reads: 37

```
is there a way to check the polarity without opening up the motor?
```

---
