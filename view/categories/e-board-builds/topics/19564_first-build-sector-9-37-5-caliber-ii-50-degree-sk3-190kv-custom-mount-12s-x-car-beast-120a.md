# First Build &#124; Sector 9 37.5&rdquo; &#124; Caliber II 50 degree&#124; SK3 190KV&#124; Custom Mount&#124; 12S &#124; X-Car Beast 120A

### Replies: 14 Views: 1138

## \#1 Posted by: jlo Posted at: 2017-03-23T18:07:21.744Z Reads: 199

```
Hi Folks,

I've been reading the forum for about a month now, and have finally started putting the pieces together for my own build. I mostly went with components from the commonly used list. I haven't ordered the electronics yet and want to double check what you all think. I'm planning on using a single Hobbyking SK3 motor, X-car esc, and pre-assembled lipos. I weigh about 200 lbs, so I want to make sure my board will have enough torque. I'm living in Boston right now, so pretty flat, but ideally I would like to be able to climb small hills as well. My pulleys have a 2.5 gear ratio and 15mm wide belt. I would love your thoughts on motor KV, battery configuration, and custom motor mounts.

Sector 9 37.5"
Caliber II 50 degree
Flywheel 90mm clones
SK3 190KV (unsure about what KV to go with)
Two lipos 12S ( still unsure about what voltage I would need)
Already own a charger for lipos
X-Car Beast 120A 
Remote TBD
rider: 200 lbs

Also, stupid question here, but can you ride your electric longboard like normal if your batteries run out? Or does forcing the motor to turn cause damage to the batteries and/or ESC?
```

---
## \#2 Posted by: delduked Posted at: 2017-03-23T18:55:15.882Z Reads: 184

```
You need two 6s batteries in series to reach 12s or in other words two 22.2v batteries in series. And the motor kv refers to how many rotations the motor can make in a given amount of time. I forget the formula but depending on your gearing ratio the KV number will result in how much torque you have. With the gear ratio your essentially trading how many motor rotations you have for more torque. In your case every 2.5 motor rotations the wheel will spin one time. So it depends on how much torque you want. That way you can get a good balance between gear ratio and KV rating.
```

---
## \#3 Posted by: trampalovesshekels Posted at: 2017-03-24T05:29:58.546Z Reads: 152

```
(kv)(Volts)(pi*dia)(60)*0.00001 = km/h
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-03-24T12:07:15.328Z Reads: 137

```
I dont think there is a xcar beast out there which supports 12s!
```

---
## \#5 Posted by: lowGuido Posted at: 2017-03-24T13:00:29.208Z Reads: 137

```
yeah if you want to use the x-car beast you will have to go 6S and probably about a 280kv motor if you want decent speed.

also you can still push the board like a regular one, but it will have a little more drag.
```

---
## \#6 Posted by: jlo Posted at: 2017-03-24T13:03:11.409Z Reads: 134

```
Thanks! Yeah, sorry forgot to mention that I did run through the calculations, with 190kv motor, 12s battery, and 2.5 gear ratio, I come out with a top speed of around 25mph. So now I need to figure out how much torque I need/want... 

@TarzanHBK Thanks for pointing that out. I guess I misread the specsheet on Hobbyking. It says "Battery: 2 ~ 6S" which I took to mean it could handle up to two 6S batteries. Did I misinterpret this? Heres the ESC I'm looking at:
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html
```

---
## \#7 Posted by: lowGuido Posted at: 2017-03-24T13:24:53.854Z Reads: 119

```
2S upto 6S so 6S max.
```

---
## \#8 Posted by: SyrusB Posted at: 2017-03-24T13:43:17.757Z Reads: 112

```
Chose the gtb2 for your remote
```

---
## \#9 Posted by: saul Posted at: 2017-03-24T15:18:43.864Z Reads: 121

```
I got an xcar 120 on sale and it sucks! Lol
It actually works ok but the breaking noise  is like nails on chalkboards. 

I still have it and a LCD programmer card if you want it. But you should get a vesc and go 10s 190kv. 12s pushing close to erpm limits but does have serious torque. 

Also lipo is not the best if you don't have experience. But it is the most bang for the buck in a few ways.

A 149kv on 12s also has crazy torque! So smooth!
```

---
## \#10 Posted by: edoardo Posted at: 2017-05-23T07:33:27.512Z Reads: 85

```
Hi, I connected an Xcar 120A with my Turnigy SK3 280kv but the motor doesn't work. What can I do?

battery = 4500mAh 6s 
remote controller = Winning radio receiver and trasmitter

<img src="/uploads/db1493/original/3X/1/d/1d87f2e2d721467e3a7128ccd365ff734feae480.JPG" width="666" height="500">
```

---
## \#11 Posted by: GhettoFab.rictation Posted at: 2017-11-13T06:04:38.545Z Reads: 53

```
Why is the 60 in the formula? And also is dia diameter of wheel?
```

---
## \#12 Posted by: FredrikHems Posted at: 2017-11-13T06:24:59.727Z Reads: 51

```
You need to know to diameter of the wheel to find the  circumference. If you have a 90mm wheel: 9cm * 3.14= 28.26cm, which means: per rotation of the wheel, you will travel 28.26 cm.
```

---
## \#13 Posted by: GhettoFab.rictation Posted at: 2017-11-13T06:33:32.545Z Reads: 51

```
Thank you and is 60 the max erpm?
```

---
## \#14 Posted by: FredrikHems Posted at: 2017-11-13T06:55:47.175Z Reads: 49

```
I have no idea Why 60 is in there, but i dont think it has something to do with the erpm limit
```

---
