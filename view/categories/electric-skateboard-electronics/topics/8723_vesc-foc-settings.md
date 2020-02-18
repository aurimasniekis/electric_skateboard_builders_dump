# VESC FOC Settings

### Replies: 6 Views: 1061

## \#1 Posted by: Cisphyx Posted at: 2016-08-31T19:36:35.151Z Reads: 174

```
This is my first build so I apologize in advance if I've overlooked something dumb. I like the idea of a quiet board, so I decided I wanted to try running the VESC in FOC mode. From reading about problems with FOC, it seems like switching back and forth between BLDC/FOC was thought to be causing issues, so I figured if I was going to try it I would just start off with FOC. After receiving my VESC, I updated the firmware as suggested and configured it in FOC mode. I took it out for a ride, and it was working great for a little over a mile. I was slowing down coming up to an intersection and after that it stopped responding. I plugged it back in when I got home and I'm getting a DRV8302 fault. There's no obvious damage so I'm assuming just replacing the DRV should get it back in working order. I'd like to not be going through them on a regular basis trying to find good settings, so I'm wondering if anyone has suggestions for my setup:

Sensored 230kv 6374 from Psychotiller
Enertion VESC
Space Cell Pro 3
97mm ABEC 11 Wheels
13T/36T

VESC Settings:
<img src="/uploads/db1493/original/2X/8/82648f816c2f3a8f70babb2f94c53096e8fb8ee9.JPG" width="690" height="412">
<img src="/uploads/db1493/original/2X/1/11a8e00133e8958985da9ccdb7d2b6004edcb4a9.JPG" width="690" height="200">

VESC Pictures:
<img src="/uploads/db1493/original/2X/2/265a2c4d2a7f75b39b8c3b57f511b898b8f06aa0.jpg" width="689" height="390"><img src="/uploads/db1493/original/2X/a/a65a68b899fcd6039cab0193acb73979f1b8d19d.jpg" width="690" height="390">

Any ideas for what I can do to avoid blowing up more DRV8302s? Should I use different settings? Should I abandon FOC and try BLDC instead?
```

---
## \#2 Posted by: Atxraider Posted at: 2019-09-16T14:45:44.614Z Reads: 28

```
It sucks no one has responded to your post, bc I’d like to know the answer to the exact same question since it happened to me, as well. 
Did you ever get it figured out?
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-09-16T15:05:04.462Z Reads: 28

```
Its likely the ERPM killing his DRV chip, as theyre only good till 60,000 ERPM on old single 4.xx VESCs

10s x 230kv motor = over 60000

Additionally, FOC is more stressful on the system than BLDC. If your preference leans more towards reliability, than BLDC might be better for you.
```

---
## \#4 Posted by: Atxraider Posted at: 2019-09-16T15:12:32.539Z Reads: 29

```
I’m currently running it in FOC, and have the ERPM limit set to 60000/-60000, as well as under the app tab I have it set to 53000 and 55000.
```

---
## \#5 Posted by: Sn4pz Posted at: 2019-09-16T15:17:56.027Z Reads: 28

```
They can still fail well below the 60000 magic number. I sort of think about it like the 'silicon lottery' with CPUs and how some are just better at overclocking out of the box compared to other CPUs of the same model. However in this case its slightly more dangerous :sweat_smile:.  Basically some DRVs / VESCs are built like tanks, yet some are incredibly fragile. 

Besides treating your VESC right, and not treating it like crap, its all up to luck. 

What brand do you have?
```

---
## \#6 Posted by: Atxraider Posted at: 2019-09-24T09:43:25.659Z Reads: 13

```
I have an old Vesc-x (pre focbox) from Enertion and a flipsky. Both are in aluminum enclosure/heat sink from Flipsky. I upgraded the firmware on both of the VESCs using the VESC tool.
```

---
