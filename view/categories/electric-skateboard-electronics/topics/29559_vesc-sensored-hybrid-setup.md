# VESC sensored/Hybrid setup

### Replies: 7 Views: 715

## \#1 Posted by: florensvb Posted at: 2017-08-03T07:20:13.614Z Reads: 133

```
Hey guys,

Two questions regarding the vescs setup:

1. When i run Start Detection for BLDC mode, it works for the "three" values, but it always says that the Hall sensor detection failed .. what can i do?

2. i have purchases a sensor wire to connect my torqueboarda 5065 260kv with my vesc, but i dont seem to find any tutorials on how to set up a hybrid mode properly .. any ideas?

Cheers guys!
```

---
## \#2 Posted by: Martinsp Posted at: 2017-08-03T07:32:54.417Z Reads: 132

```
So you say that you have a sensored motor but you can not get the detection to detect them properly?

EDIT: 
Try it in FOC mode because I found that some sensors work in FOC perfectly but I could not get them to detect in BLDC.
```

---
## \#3 Posted by: florensvb Posted at: 2017-08-03T09:52:22.353Z Reads: 113

```
I hooked up the sensor wire, then put it in Hybrid mode in the BLDC tool and hit start detection. These are the results:

Detection results:
Integrator limit: 84.74
BEMF Coupling: 832.24

Hall sensor detection failed:
-1, -1, -1, -1, -1, -1, -1, 6
```

---
## \#4 Posted by: florensvb Posted at: 2017-08-03T10:08:23.692Z Reads: 103

```
[This is the motor that i have](diy-electric-skateboard-kits-parts/electric-skateboard-motor-5065-260kv/)
```

---
## \#5 Posted by: florensvb Posted at: 2017-08-03T10:19:08.870Z Reads: 101

```
Also when I click on Hybrid mode and then write configuration, I can not spin the motor using my remote, even though the vescs light turns green when i hit the throttle.
```

---
## \#6 Posted by: pshaw Posted at: 2017-08-03T11:39:08.160Z Reads: 98

```
[quote="florensvb, post:3, topic:29559, full:true"]
I hooked up the sensor wire, then put it in Hybrid mode in the BLDC tool and hit start detection. These are the results:

Detection results:
Integrator limit: 84.74
BEMF Coupling: 832.24

Hall sensor detection failed:
-1, -1, -1, -1, -1, -1, -1, 6
[/quote]

same exact thing happened to me last night. when I went into the FOC tab it would detect sensors though and fill out the table. I just wonder if i use BLDC that the sensors would be calibrated.
```

---
## \#7 Posted by: florensvb Posted at: 2017-08-03T11:56:21.779Z Reads: 90

```
do the hall sensors require the sensor wires?
```

---
