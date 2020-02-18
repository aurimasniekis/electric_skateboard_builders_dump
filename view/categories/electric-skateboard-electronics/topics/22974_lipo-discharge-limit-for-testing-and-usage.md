# Lipo Discharge Limit for testing and usage

### Replies: 5 Views: 463

## \#1 Posted by: wmj259 Posted at: 2017-05-13T18:23:42.315Z Reads: 51

```
I wasn't able to find my answer on the search function.
How low should lipo voltages go in terms of discharging? I know that it should never go below 3.4Volts, but the Instruction Manual that came with my lipo says to never discharge below 3.0Volts. The issue is that my charger instruction manual also says that when doing the discharge test on the charger, it will go down to 3volts.
<img src="/uploads/db1493/original/3X/4/0/40b2919a24cb009b95f9036741fb77cba08b1258.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/0/40d8c1e33cc9cebb1a156ee96ea3fda040efb1f6.jpg" width="666" height="500">
Should I just go with the discharge program on the charger and manually stop it once the voltage reaches 3.4Volts?
```

---
## \#2 Posted by: Philippe1 Posted at: 2017-05-13T18:27:10.160Z Reads: 49

```
Lipo's should never go below 3.2V I think.
```

---
## \#3 Posted by: adrian009 Posted at: 2017-05-13T18:59:24.728Z Reads: 47

```
For discharge test 3.0v is fine but I wouldn't go that low in regural usage,  3.4v is ok
```

---
## \#4 Posted by: wmj259 Posted at: 2017-05-13T19:01:23.126Z Reads: 47

```
@Philippe1
@adrian009
Thanks for the replies. So as long as this is a one-time low, it should be good. Personally, I will just stop it at 3.2-3.4V and then interpolate, to find what my true capacity is. I know that regular usage should never go below 3.2-3.4V which is what alarms beep at, but these manuals made it really confusing.
```

---
## \#5 Posted by: adrian009 Posted at: 2017-05-13T19:04:06.052Z Reads: 45

```
If your charger display live data You can watch how many mah it drain till ie 3.2 and stop it. Won't be super acurate but shoud give some info about battery health
```

---
