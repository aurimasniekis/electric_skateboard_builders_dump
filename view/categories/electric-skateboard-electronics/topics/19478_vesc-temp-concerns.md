# VESC Temp Concerns

### Replies: 30 Views: 2916

## \#1 Posted by: pyttroll Posted at: 2017-03-22T17:07:58.313Z Reads: 180

```
Hi guys,

I'm concerned about the temperature of my VESC, today I went for a short ride (4.4km) and the temp reached 55ºC (131ºF), it might not sound that bad but it's -11ºC (12.2ºF) outside, which is kinda of cold...
The peak occurred going up at the end of a slight hill (maybe 10m over 1km), just going downhill the VESC was already reaching 34ºC (93.2ºF).

I'm running a single 190kv 63mm motor from DIY with a 10S5P, I'm about 80kg / 175lbs.
Here is the ride: https://metr.at/r/2hg3H

So basically my question is, is it normal?

Pyt
```

---
## \#2 Posted by: torqueboards Posted at: 2017-03-22T17:45:54.107Z Reads: 169

```
@pyttroll - Did you get a VESC from DIY? If so, you might have gotten a bad VESC which has a damaged R1 component. You can ship it back and we can send you a new one and/or you can replace the R1 component. Let me know.
```

---
## \#3 Posted by: pyttroll Posted at: 2017-03-22T17:47:56.694Z Reads: 165

```
Yeah @torqueboards I got it from you, how expensive is that R1 component? And how easy is it to change?
```

---
## \#4 Posted by: Montiey Posted at: 2017-03-22T17:55:55.547Z Reads: 165

```
@pyttroll, how is your VESC enclosed? If the FETs were open to the air, then I would say 55° is extremely hot, but if it's in any kind of case, and with shrink-wrap over the FETs, then I suspect there is just too much insolation for the outdoor temperature to matter once it heats up inside.
If you let the board sit for 10 minutes, THEN you'd get a ton of power, but once the heat shrink and foam warm up, that effect wears off.

I haven't implemented any sort of cooling on my VESC, and so going up a steep enough hill to cause 100% current draw brings my FETs up to the 80-100°C limit in about ~10 seconds. I know 100° is hot, but the only problem I think I'd ever have is melting the foam tape I use to cushion the inside of the enclosure.
```

---
## \#5 Posted by: pyttroll Posted at: 2017-03-22T17:59:46.427Z Reads: 158

```
Hey @Montiey my VESC is in a tight 3mm ABS enclosure, sharing space with part of the battery, a buck converter and an anti-spark switch. I don't seem to have a loss of power when the temp goes up.
```

---
## \#6 Posted by: torqueboards Posted at: 2017-03-22T18:03:41.320Z Reads: 155

```
@pyttroll It's a fairly cheap component. I'd have to double check and it's easy to fix since it's on the outside.

If you didn't want to deal with changing it out though you can just send it back. We have a new batch that should arrive today. I'll send you a PM with more info.

@Montiey - It's specifically a bad R1 sensor so it's not actually hot. Awesome answer though :)
```

---
## \#7 Posted by: Montiey Posted at: 2017-03-22T18:05:03.077Z Reads: 152

```
EDIT: Torqueboards just confirmed R1. That's what I get for taking too long to reply! :P

Hmm.. I'm reading now about a bad batch of VESCs from DIYElectricSkateboard. I would investigate the accuracy of those temperatures… If you can, take it out of the enclosure, and see what it reads idle outside, and inside. For example, I would expect 20° inside and -11° outside.
```

---
## \#8 Posted by: torqueboards Posted at: 2017-03-22T18:06:45.058Z Reads: 149

```
@pytroll - Actually, I think yours might not be that issue. At least, I don't think yours was part of the bad batch since your order was before the fact.

After your VESC has been sitting for a while can you connect to it and check the real time data tab for what the mosfet temp is?

From actually reading your initial post the symptoms are actually different so @Montiey this might be a different issue.
```

---
## \#9 Posted by: pyttroll Posted at: 2017-03-22T18:09:34.807Z Reads: 143

```
Yeah @torqueboards, it reads 13.6ºC right now, which is my garage temp, so the sensor seems ok.
```

---
## \#10 Posted by: Montiey Posted at: 2017-03-22T18:13:09.066Z Reads: 139

```
Interesting. So that's not the problem, then, unless the sensor only becomes inaccurate at higher temperatures.

Perhaps you could post your BLDC tool settings pages? If this isn't in fact a hardware issue, then that's probably where we'll find the problem.
```

---
## \#11 Posted by: pyttroll Posted at: 2017-03-22T18:16:25.364Z Reads: 139

```
Here you go:

<img src="/uploads/db1493/original/3X/0/a/0af71bef0a1ba88cdbda6b7806a279811f8dddf7.png" width="690" height="417">

<img src="/uploads/db1493/original/3X/2/6/267a7ac8e434e5befb089de78e7b4473ba24b300.png" width="690" height="417">

<img src="/uploads/db1493/original/3X/3/9/3909ff2a710541b9a0cebbe016f8e3c732c1043a.png" width="690" height="417">
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-03-22T18:20:43.252Z Reads: 120

```
Put batt max at around 30amp. That should help. But also don't really take for granted the data from the app, specially if the outside temperature is bellow -10, we've got some weird data last time we try a board at low temperature 😉

Also your way over the temps cutoff, so if the data was right it should had slow you down.
```

---
## \#13 Posted by: torqueboards Posted at: 2017-03-22T18:22:17.156Z Reads: 122

```
Has it done this before? I'd try riding again and see if the issue comes up again.
```

---
## \#14 Posted by: Montiey Posted at: 2017-03-22T18:22:54.008Z Reads: 121

```
Where is the sensor located? I ask because if you can rub it with a finger or give it a little warm air from a blow dryer, etc. you might be able to see if it reacts accurately.

I thought they were integrated into the FETs but I can't be sure.
```

---
## \#15 Posted by: pyttroll Posted at: 2017-03-22T18:23:40.980Z Reads: 116

```
Thanks for the advice @JohnnyMeduse, the biggest draw logged by the app was 24.6A so I'm not sure reducing the batt max to 30A would help, unless the reading for the amps is also wildly innacurate...
```

---
## \#16 Posted by: Blasto Posted at: 2017-03-22T18:25:41.352Z Reads: 115

```
could it just be the units that are wrong? your starting temp is 23deg, if in F that would be -5C, which sounds right
```

---
## \#17 Posted by: pyttroll Posted at: 2017-03-22T18:26:49.474Z Reads: 114

```
I thought about that but the temp is good when the board has been idle for a while...
```

---
## \#18 Posted by: Montiey Posted at: 2017-03-22T18:27:23.078Z Reads: 114

```
Does the app read anything related to the motor temps? If you don't have a motor sensor, then obviously you should disable it if possible. Try setting the motor start and end values to 0 and see what happens.
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2017-03-22T18:27:30.929Z Reads: 114

```
You just want to be sure that everything is under control, I'm still not sure is the app might have some delay, or don't show you fast peak current. Don't forget that these are app and give you a average data, they are not precise as a thousand dollar meter can be.
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-03-22T18:28:26.987Z Reads: 117

```
For a normal VESC 4.12 in a enclosure without heatsinks this is absolutely normal. For a single drive the normal VESC get's temperature problems. So once you reach 80 degrees it will start to reduce the power. Add some passive heatsinks and it will get better. When go up a long hill my single easily overheats.
```

---
## \#21 Posted by: pyttroll Posted at: 2017-03-22T18:28:54.442Z Reads: 113

```
Right, I'll give it a shot and see what happens...
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2017-03-22T18:28:58.917Z Reads: 117

```
[quote="Montiey, post:18, topic:19478"]
related to the motor temps
[/quote]

If you don't have temps sensor in your motor it won't be related to the motor. 😉
```

---
## \#23 Posted by: pyttroll Posted at: 2017-03-22T18:29:40.347Z Reads: 111

```
Thanks for the info @Ackmaniac, I'll try to squeeze in some heatsinks.
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2017-03-22T18:30:15.879Z Reads: 108

```
But did you feel a lost in the power? Or it was to dam cold outside to feel anything 😜
```

---
## \#25 Posted by: pyttroll Posted at: 2017-03-22T18:30:45.622Z Reads: 109

```
I'm using the motor sensor but I have no idea if it carries motor temp...
```

---
## \#26 Posted by: pyttroll Posted at: 2017-03-22T18:31:26.494Z Reads: 105

```
Lol, no loss of power at all. Just fucking freezing my ass...
```

---
## \#27 Posted by: Ackmaniac Posted at: 2017-03-22T18:34:38.592Z Reads: 105

```
The motor temp sensor isn't used in the firmware. It only stores your settings and that's it. Doesn't read it at all even if you attach it. Would be relatively easy to add the functionality but then you have the stress with different sensors.
```

---
## \#28 Posted by: Jammeslu Posted at: 2017-03-22T19:57:13.256Z Reads: 100

```
Sorry for dusturbance or non relevant question but did'nt want to start new thread, bit is this Vesc legit?

http://m.ebay.com/itm/VESC-BLDC-Open-Source-Electric-Skateboard-ESC-/162366404102?hash=item25cdcab606%3Ag%3ARyoAAOSwNRdX2smF&_trkparms=pageci%253A875c9b82-0f21-11e7-956f-74dbd1805d85%257Cparentrq%253Af6f98b8015a0a62283653160fffa72b2%257Ciid%253A2

It seems pretty Good and are located in EU which is Good for me and not to expensive either bit is it legit?
```

---
## \#29 Posted by: torqueboards Posted at: 2017-03-22T21:32:29.920Z Reads: 97

```
Here's the Temp Sensor. Although, this issue might not be the issue for the OP. Just as reference for those who haven't seen it.

<img src="/uploads/db1493/original/3X/d/e/de3a249d25544fb498df00ca236c5a72ed08c31f.png" width="352" height="500">
```

---
## \#30 Posted by: makevoid Posted at: 2017-03-22T22:13:50.345Z Reads: 89

```
vesc starts cutting power off at higher temps as @Ackmaniac said, at 55 you're still fine.

As @chaka said some times in the past, vesc v4 tend to overheat especially with 637x motors around the same kvs, with 1 (and especially with dual) 5065 the vescs should overheat much less. 

This should be not an issue on vesc v6 (and vesc-x, and probably ollin-esc), they should be able to drive more powerful motors without overheating (w/ a motor with an higher max watt rating). 

So my advice for that is go dual (that should be enough), add heatsinks and improve aifrlow (there's a drawback if you don't seal everything well) or get a post-v4 vesc (x, 6, ollin). 

For others that live at lower latitudes and/or that are riding a lot in the summer and thus have higher temps and vesc power cutoffs due to overheating maybe switch to smaller motors if you can like 5065 or hubs (for example carvons). Another thing that should help prevent overheat on v4 it's to increase the voltage (10s -> 12s).


Bare in mind that the shrinkwrap prevents the vesc from  water / particles / moisture / electrical contact  damage. Ideally you should aim for a good airflow for the enclosure so the vesc is cooled down but no water ever touches it. At least a good amount of space/air around the vesc would be nice.

I think a cool idea for an enclosure is to have one with a heatsink  part exposed outside and you mount the vesc onto it so it cools down but that's maybee a bit extreme lol
```

---
