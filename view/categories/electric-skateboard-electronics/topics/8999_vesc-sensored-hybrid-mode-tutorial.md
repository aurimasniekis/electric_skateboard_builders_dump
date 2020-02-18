# VESC: Sensored/Hybrid mode tutorial?

### Replies: 17 Views: 3655

## \#1 Posted by: michaelcpg Posted at: 2016-09-05T21:35:15.093Z Reads: 410

```
Hey all,

I've ordered a pair of @chaka's 5065 motors to replace my 6372 motor and was wondering if someone would mind pointing me in the direction of a tutorial on how to setup sensored/hybrid mode? 

Would be excellent if someone wouldn't mind explaining the difference between sensored and hybrid mode as well.

Cheers :)
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-05T23:32:01.862Z Reads: 400

```
You can check out my build log on how to setup the physical connection here

http://www.electric-skateboard.builders/t/honey-driver-honey-velocity-v3-deck-caliber-iis-83mm-evolve-gt-wheels-dual-om5065-200kv-space-cell-pro4-diy-pulleys-enertion-pulley-bones-super-reds-enertion-mounts-winning-remote-chaka-vescs-build-complete/5760/36?u=jinra

as for sensored vs hybrid. Sensored is pure sensored mode, which means it'll use sensors all the time. You probably don't want this as sensors are not efficient at high speeds and may cause issues such as high heat in my experience. Hybrid mode will cut off the sensored operation at a predetermined erpm from the "sensorless erpm" field in bldc tool. 

Make sure to set the hall table correctly when using sensored mode
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-09-06T00:35:54.471Z Reads: 375

```
Thanks for the info, sounds like hybrid is the way to go then.
Just have a couple questions:

What sort of ERPM would you recommend setting the cutoff at?

Would you mind giving a quick explanation of how to setup the hall table? I'm assuming that the numbers you set in the hall table somehow correspond to some of the pins on the VESC?

Any other settings I need to change in BLDC Tool in other than the hall table and changing the sensor mode to Hybrid?
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-06T00:39:13.795Z Reads: 356

```
id just leave the sensorless erpm at the default 2000. you set the hall table after motor detection, it will list the hall order, you just put the values in the sensor field.
```

---
## \#5 Posted by: FlashNova Posted at: 2016-09-13T08:53:47.663Z Reads: 328

```
Did you have any luck setting up hybrid mode? I have sensor wires coming in the mail and I can't really find any solid information on setting up hybrid/sensored mode in BLDC. I'm scared im gonna fry my vesc. I thought I saw a video on how to do it, but now I can't find it.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-09-13T10:26:49.467Z Reads: 316

```
Can you tell my how accurate the rpm detection is in sensor mode? Because in sensorless mine has waves of +- 400 rpm at a constant speed. Would be great to know if sensored mode is absolutely accurate.
And when it is accurate does it also stay that way above the sensorless erpm rpm (when it should run sensorless in hybrid)
```

---
## \#7 Posted by: Jinra Posted at: 2016-09-13T10:43:48.622Z Reads: 303

```
do you mean erpm? fluctuations in that range are normal. Normal sensorless erpm is about 2000 which is only a couple (1~) mph, so you run sensorless most of the time.

@FlashNova Just run it how i explained above, not much risk unless you setup the hall table or physical connection wrong
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-09-13T11:06:15.136Z Reads: 292

```
What i mean is how stable is the rpm signal for sensored motors when they run sensored or hybrid mode. Is it absolutely accurate or does it jump up and down a bit the whole time. Because in my sensorless mode it jumps up and down by 400 rpm. So the messured values are never 100% accurate.
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-13T11:10:44.087Z Reads: 282

```
That's why I'm asking if you're talking about the erpm reading in bldc tool. Reading is the same in both modes. +/-400erpm is very insignificant.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-09-13T11:16:07.778Z Reads: 277

```
For what i want to do with it it would be helpful to get very accurate erpm readings. Does it get more accurate when you set the "sensorless erpm" higher. So that it will run in sensored mode at the speed you are messuring.
```

---
## \#11 Posted by: Jinra Posted at: 2016-09-13T11:17:10.014Z Reads: 264

```
You can set it to pure sensored and the readings on bldc will be the same. It doesn't really change the readings.
```

---
## \#12 Posted by: Ackmaniac Posted at: 2016-09-13T11:19:25.981Z Reads: 259

```
So i need to check how the Firmware code detects the erpm. Seems that it doesn't read the sensored data for that value. Thanks alot.
```

---
## \#13 Posted by: michaelcpg Posted at: 2016-09-13T21:14:17.840Z Reads: 254

```
My motors arrived yesterday so I'm going to have a go at setting them up tonight. Tbh I'm still not 100% sure on the process of setting the sensors up either. 

@Jinra would you mind explaining how you setup the the hall sensor table? Do the values load into the table automatically on motor detection or is there some manual process to it?
```

---
## \#14 Posted by: Jinra Posted at: 2016-09-13T23:31:18.543Z Reads: 243

```
yep that's exactly how you do it. The values load during detection, then you just apply it. Make sure you plug the sensor wires in correctly.
```

---
## \#15 Posted by: korryh Posted at: 2016-10-10T02:42:01.797Z Reads: 221

```
This thread is kind of old but I am setting up Ollins motors also and want to use hybrid mode. I get how to detect the sensors but what do I change to make the sensors cut off at a certain point. Is there a box I check or is it something I have to set. Thanks.
```

---
## \#16 Posted by: Jinra Posted at: 2016-10-10T02:43:08.971Z Reads: 219

```
"sensorless erpm" = erpm at which sensors cutoff. 2000 is a good value for this. Make sure you're on hybrid mode and not sensored.
```

---
## \#17 Posted by: korryh Posted at: 2016-10-10T03:15:33.457Z Reads: 216

```
Gotcha. Thanks!!!
```

---
