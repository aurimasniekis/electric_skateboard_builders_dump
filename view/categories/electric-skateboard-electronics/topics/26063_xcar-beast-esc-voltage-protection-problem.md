# Xcar beast esc voltage protection problem

### Replies: 7 Views: 384

## \#1 Posted by: pat.speed Posted at: 2017-06-24T09:28:40.884Z Reads: 54

```
Hey guys, 

I was riding my board the other day and it just stopped dead in the middle of the road. I checked it and I think my escs low voltage kicked in. I don't think I programmed it properly because the lipos discharged down to about 3.0v per cell luckily it isn't too bad.

Anyway when I got home I charged them and tried to run the esc but when I try to pull in the throttle it runs the motor for a few seconds then the low voltage led on the esc blinks and the motor runs really slow. Anyone know what is happening? I have even tried it with my benchtop power supply and the same thing happened
```

---
## \#2 Posted by: Maxid Posted at: 2017-06-24T10:22:36.825Z Reads: 46

```
The esc also goes into the same "undervoltage" mode when you have a overvoltage - what exact voltage have you used?
```

---
## \#3 Posted by: pat.speed Posted at: 2017-06-24T12:10:38.847Z Reads: 39

```
Hi I got it working again.I was using 6s. I ended up having to connect it to the computer and reset all the settings. Sorry about that I should have tried this earlier but I only just found the software for my pc. 

Thanks anyway
```

---
## \#4 Posted by: Maxid Posted at: 2017-06-24T12:31:05.134Z Reads: 33

```
6s is not a voltage
```

---
## \#5 Posted by: pat.speed Posted at: 2017-06-24T12:31:58.633Z Reads: 31

```
I meant 22.2v which is the equivalent to 6s of 6 cells in series
```

---
## \#6 Posted by: Maxid Posted at: 2017-06-24T12:34:30.901Z Reads: 30

```
I am pretty you did not have it at exact the nominal voltage of 22.2.
Do you know how a lipo works?
A full lipo cell will have 4.2V while an empty one will have something like 3.2V.

A slight overcharge in a 6S setup to 25.5 instead of 25.2 (=6*4.2) might cause an overvoltage error.
Additionally there are HiV cells with a 4.3V voltage when full.
```

---
## \#7 Posted by: pat.speed Posted at: 2017-06-24T12:37:37.798Z Reads: 31

```
Oh you meant at the time. Sorry I thought you meant what kind of pack I was using silly me lol. I'm not sure the exact voltage although a few minutes earlier my battery checker said 23v. So I don't think it was that. My guess is I hit the cut of voltage or something. But that doesn't explain what happened when the batteries were charged
```

---
