# VESC HW 4.12 temperature comparison

### Replies: 11 Views: 2035

## \#1 Posted by: hexakopter Posted at: 2017-05-16T19:56:04.084Z Reads: 228

```
I have done a comparison how airflow is affecting the temperature rise of the VESC 4.12 hardware. You can watch the video here:
[https://youtu.be/UwVQQ_LY5bc](https://youtu.be/UwVQQ_LY5bc)
I know that this forum is mainly for electric skateboard stuff, but because my electric skateboard wasn't powerful enough to stress the VESC 4.12 as much as needed I think using a eBike does't make it less interesting for you guys. :grin:

To give you an more detailed insight of my setup: 
The VESC itself is self soldered with a self build heatsink on top of the MOSFETs. I was aware, that the heat transfer between the D2Pak plastic housing and the aluminum heatsink wouldn't be great but I did it anyways and also put thermal paste between them. The settings were at 50A max battery current and 120A max motor current. The MOSFET temperature limit start was set to 80°C and the end to 100°C.

I was running the test on my eBike with a MXUS 3000 v3 motor and 10000mAh Multistar 11s battery. I compared the temperatures when the VESC was inside my bike bag (so no airflow at all) and with the VESC + heatsink was hanging out of the bag.

I was logging all the VESC data with the bluetooth module from [https://metr.at](https://metr.at) and the metr.at iOS app. The app is also available for Android and there is also the perimetr app available to change the VESC settings on the fly. You can find more infos in this [thread](https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483).

Here you can see my logs from the metr.at logging app:
[https://metr.at/r/jTArX](https://metr.at/r/jTArX) 
(short run on hill with a big incline without air-cooling)


[https://metr.at/r/9LggY](https://metr.at/r/9LggY) 
(short run on hill with a big incline with air-cooling)


[https://metr.at/r/QgKsx](https://metr.at/r/QgKsx) 
(longer run on hill with a smaller incline without air-cooling)


[https://metr.at/r/Pk4XU](https://metr.at/r/Pk4XU) 
(longer run on hill with a smaller incline with air-cooling)

This data was then overlaid to the video that I have done with my Xiaomi Yi and a StorM32 BGC brushless gimbal. The elevation data isn't that accurate because of a missing barometer in my phone. You can also see that I had to release the full throttle sometimes and brake with the bikes disc brakes. (no regen braking activated right now)

I have also created two graphs of the two runs where you can see the different temperature rise better.
<img src="/uploads/db1493/original/3X/d/9/d96626f4a85c55de64c15efe175d86cb7fef3998.png" width="690" height="361">
As you can see without air cooling I was hitting the temperature limit at the end.
<img src="/uploads/db1493/original/3X/e/3/e3e9fbd22eafa0084baee577b01f99b4d2005dcc.png" width="690" height="361">
You can see in that graph how the temperature of the uncooled VESC stays in the "temperature limit zone". Because of that limit I reached the same location a lot later, while the cooled one stays under 70°C the whole time.

So lets summarize what I have learned from the test. It is very important to use the airflow when it is possible for you to mount the VESC where the air is flowing. When mounted correctly the VESC 4.12 hardware is able to take a lot of current without getting to hot. I was aware that the airflow has a big influence to the temperature development, but not as big as seen in the graphs. Impressive. A lot of builds of electric skateboards I have seen dont use the airflow from driving at all. When not hitting the temperature limit thats ok, but if you need more power you know what to do.
```

---
## \#2 Posted by: monkey32 Posted at: 2017-05-16T20:26:16.867Z Reads: 190

```
Cough cough......title.....cough cough

https://www.electric-skateboard.builders/t/new-name-for-vesc-poll-copyright-issue-with-current-name/23047/59?u=monkey32
```

---
## \#3 Posted by: SirDiff Posted at: 2017-05-16T20:32:19.243Z Reads: 180

```
So basically the real problem of the FUKYEA (this is how we call the vesc now) is heat dissipation. I think every producer should sell the heatsink version, that doesn't add much in terms of costs and it helps a lot with performance!
```

---
## \#4 Posted by: hexakopter Posted at: 2017-05-16T20:47:39.900Z Reads: 172

```
I call it VESC, because it is build exactly with Benjamins BOM.
Just adding the heatsink will not help. I haven't compared how the performance of a VESC with heatsink compares to one without, the main thing is using the airstream from the eVehicle for air cooling. So I think also a VESC without a heatsink will perform much better outside the bag than inside.
```

---
## \#5 Posted by: treenutter Posted at: 2017-05-16T20:56:15.472Z Reads: 153

```
@hexakopter this is a great experiment thanks for sharing it! With esk8 the problem we have is finding a way to get airflow to the VESC without exposing it a way that makes it susceptible to water damage (not to mention debris). 

Beautiful countryside trail, by the way! Looks like a great location for riding!
```

---
## \#6 Posted by: hexakopter Posted at: 2017-05-16T21:20:04.340Z Reads: 138

```
I know. As you can see in a screenshot from the video that was just a comparison test, so not a everyday solution to hang the VESC just out of the bag. But when you see how much airflow affected the possible power output it would be a bummer to not find a solution that protects against water and dust, but also lets air cooling the FETs.
```

---
## \#7 Posted by: Okami Posted at: 2017-05-16T21:40:35.793Z Reads: 133

```
Very nice video, thanks for ''bringing'' it here :slight_smile:
The difference is quite big indeed.. also nice that you can easly hit 50kph of speed with your ebike :D im starting to lean in this direction too (building 50kph capable ebike)..
```

---
## \#8 Posted by: hexakopter Posted at: 2017-05-17T09:35:28.429Z Reads: 117

```
Thanks. Lean in this direction is definitely a good start. :grinning:
```

---
## \#9 Posted by: onloop Posted at: 2017-05-18T06:21:13.321Z Reads: 109

```
[quote="hexakopter, post:4, topic:23230"]
I call it VESC, because it is build exactly with Benjamins BOM.
[/quote]

i don't think it matters what parts you have, technically it doesn't permit you to use the name VESC to describe your ESC. the name can only be used to describe the trampa product. Or you can say my ESC based on VESC(R) .... blah blah blah...

this is going to get funny...
```

---
## \#10 Posted by: fedestanco Posted at: 2017-05-18T09:32:11.801Z Reads: 91

```
You CAN use vesc in conversation among private users and in forums. But I believe it is in your best interest to pick a new name for vesc-x and start spreading it before raptor 2 comes out. So that people will talk well about it using its new name.
```

---
## \#11 Posted by: hexakopter Posted at: 2017-05-18T21:55:45.913Z Reads: 75

```
I think I can call my ESC VESC, because it is not a product from any company nor is it intended to sell anywhere. It is just what I have build for myself. But this thread isn't intended to talk about the TM discussion. I think we have enough threads about it.
```

---
