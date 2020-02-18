# VESC FOC Manual

### Replies: 3 Views: 999

## \#1 Posted by: notger Posted at: 2017-09-24T19:42:13.932Z Reads: 149

```
Hi,

until now i just accepted the Values that the Autodetect of the BLDC-Tool measures.

But I'm interested what are those values about actually ?, or how caould we tweak those values eventually ?

So here is a screenshot of some BLDC-Tool Pages, I'm not even Sure where changes have effect on the Foc Mode.
<img src="/uploads/db1493/original/3X/b/b/bb7bb1815d5409498211652972a6be2e455d046c.png" width="690" height="367">
What does General (cont):
F-SW and DTc
Speed Tracker
Duty Downramp
Openloop RPM

Gerneral:
Sensorless ERPM ??

Sensorless Startup and Low Speed
Open Loop
D Current Injection

<img src="/uploads/db1493/original/3X/f/b/fb7d47e9c40e814146353f4ff2b20fdf5cde54c9.png" width="690" height="229">
are values on this pas effectin FOC in any way ?


Thanks in advance

Notger
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-09-24T22:07:56.726Z Reads: 117

```
[quote="notger, post:1, topic:33873"]
F-SW
[/quote]

For This u can in crease a bit. I believe default is 20khz, can increase somewhere up to 40khz. this give u quieter motor spin as it passes human hearing range. but this can heat up the motor a little and less efficient. Depends on the motor u use u can actually gain more stability(less coggy) not too sure if true.
{source:Benjamin, Endless sphere}

start up boost is for initial current feed for stand still moving. it's like initial foot push for motor to start spinning, but electrical. Thats all I know
```

---
## \#3 Posted by: notger Posted at: 2017-10-03T21:50:51.757Z Reads: 81

```
how could i actually increas the top speed abit in FOC ?

with BLDC you could just rais the ERPM, but what value is it in FOC ?
```

---
