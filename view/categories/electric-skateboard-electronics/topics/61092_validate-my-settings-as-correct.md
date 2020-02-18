# Validate my settings as correct

### Replies: 4 Views: 146

## \#1 Posted by: Hannes Posted at: 2018-07-06T18:45:51.016Z Reads: 45

```
Hi, so i just setup my vesc and I think i got it right but i just wanna make sure with you guys before i do anything more, I have a tourqeboards VESC, (single) 6374 and 10s4p 30q. Running sensorless.

the "cells" in voltage tab says 10, removed 0 by accident.

https://i.imgur.com/BRj2OiD.png
https://i.imgur.com/7aFaKXA.png
https://i.imgur.com/qVmHiae.png
https://i.imgur.com/Ngq9dQp.png
```

---
## \#2 Posted by: E1Allen Posted at: 2018-07-06T18:53:49.472Z Reads: 38

```
You probably won't hit erpm limit but 60k/-60k is your vesc limit.  If there is a check mark for limit erpm with negative torque make sure that is not checked.  Your battery min can go up to -16 for single motor which will be good.  You can probably up your motor Max and min to 70 each.   Your vesc will be the limiting factor I think.  I personally if I went single would set a temp cutoff start at 70c and 90c end.  But that's just what I would do. I've never ran single.
```

---
## \#3 Posted by: Hannes Posted at: 2018-07-06T18:57:00.780Z Reads: 38

```
Ok, will try your recommendation, yes i've read on other topics about the negative torque but cannot find it in vesc tool, so i suppose they don't have it anymore?

Thanks for the reply :)
```

---
## \#4 Posted by: E1Allen Posted at: 2018-07-06T19:30:21.432Z Reads: 31

```
I don't use that version so I'm not sure.
```

---
