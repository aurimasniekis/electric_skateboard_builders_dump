# Fault code drv8302: Motor wont spin and red LED flashing

### Replies: 32 Views: 812

## \#1 Posted by: nordlicht Posted at: 2018-06-14T10:31:42.613Z Reads: 95

```
Hi,
I was about to finish my build and spun the motor at full throttle without load, than it suddenly stopped.
The BLDC tool gave me the fault code DRV8302. This is the controller chip.
Is the Controller dead now? 
![foctab|623x500](upload://kTSiPXn5J6OraCXsV83EFmXUtPP.jpg)![bldctab|625x500](upload://h0Wy5iU6BCrcxDXRJV3UDw85DNe.jpg)![motortab|625x500](upload://q7m2lHgqvbGWPu1iJNLDE9qbq5D.jpg)![foc_detection|625x500](upload://qn9Mo92lyOXiPSNiAnnREXmPOSV.jpg)

Those are the configurations. Did I screw up? Is this a known error? Would soldering a new chip help?

Cheers
```

---
## \#2 Posted by: bplatoff Posted at: 2018-06-14T11:05:47.051Z Reads: 78

```
Not sure about your settings but you will need to replace the chip talk to this guy @JohnnyMeduse
```

---
## \#3 Posted by: nordlicht Posted at: 2018-06-14T12:37:41.575Z Reads: 75

```
I'm at a uni and can infrared solder it myself. The question is if the DRV is REALLY the issue and how that issue started. I never even use the board on the ground.
```

---
## \#4 Posted by: bplatoff Posted at: 2018-06-14T12:54:48.154Z Reads: 73

```
If the red led flashes three times on the VESC when you use the throttle then it is a DRV error. I would still talk to @JohnnyMeduse and he can help you diagnose your problem even if you don’t want him to fix it.
```

---
## \#5 Posted by: Pimousse Posted at: 2018-06-14T12:55:38.563Z Reads: 74

```
FOC + no load + full throttle = DRV killer on HW4.12.
What kind of VESC is it ?
```

---
## \#6 Posted by: nordlicht Posted at: 2018-06-14T13:14:45.313Z Reads: 66

```
I think it IS 4.12, but how can I be sure? Just checked my order from diyelectricskateboard and it doesn't say it there :confused:

Edit: Its written on the board it self, it is 4.12. My nerfes are zero right now :frowning:
So the DRV is toast? Will it be repaired if I solder a new one in?
```

---
## \#7 Posted by: Ebisane9 Posted at: 2018-06-14T13:29:45.461Z Reads: 63

```
That MIGHT be the only thing toast but it is possible a lot of other components are toast as well on the board. Did you go directly from neutral to full throttle? The key to not killing the vesc(without load) is gradually easing into full throttle when on the bench. Going directly into full delivers too many amps at once and fries the drv and maybe other things. On bench, the motor is able to go to full speed in about 20-30% of throttle as opposed to the full range when under load. 

Bottom line: DRV is definitely toast, Inspect other components, Ease into throttle next time.
```

---
## \#8 Posted by: Sn4pz Posted at: 2018-06-14T13:32:30.237Z Reads: 59

```
did you even measure R and L and lambda?

doesnt look like that.... i ran dual foc with TB vescs and i had no problem with it.... maybe thats where u went wrong?

also if the vesc isnt tucked away send a picture of the long rectangular chip on its pcb
```

---
## \#9 Posted by: nordlicht Posted at: 2018-06-14T13:35:57.398Z Reads: 59

```
I did measure it all through, but thanks for the hint! I'm using Torque board HUBs, maybe thats why the values look different?

I'm running dual motor setup and the other controller is luckily fine. I just had my first test ride and had super low torque, I drove like 3km/h.
Back on the bench am I able to hold the wheel with my bare hands (and not too much effort). Battery amps stay low, motor amps go up high, but there is no real torque. Any clue why?
```

---
## \#10 Posted by: Pimousse Posted at: 2018-06-14T13:37:28.991Z Reads: 59

```
You shouldn't set your VESC up with FOC using a HW4.12
Resolder a new DRV, switch to BLDC and (hopefully) you'll be good.
```

---
## \#11 Posted by: nordlicht Posted at: 2018-06-14T13:39:06.505Z Reads: 59

```
I switched to FOC because with BLDC did the tool not find the hall sensors.
Can you give me some insight on why not to use FOC except this full throttle without load thing?
```

---
## \#12 Posted by: Ebisane9 Posted at: 2018-06-14T13:39:54.522Z Reads: 56

```
I mean you can, a lot of people run it. I know @mmaner has hundreds of miles on his. You just need ackmaniac firmware and a gentle curve to limit input of amps into vesc.
```

---
## \#13 Posted by: Pimousse Posted at: 2018-06-14T13:40:53.376Z Reads: 52

```
Yes, you can. But here is the exemple why you shouldn't.
Up to you.
```

---
## \#14 Posted by: Sn4pz Posted at: 2018-06-14T13:41:31.753Z Reads: 52

```
well as to why your motors lacked umph, 20a motor max is really low, I was running 50A motor max on a dual setup for each, and 20a for batt max




with a space cell pro 4, ymmv based on your battery
```

---
## \#15 Posted by: Ebisane9 Posted at: 2018-06-14T13:43:43.988Z Reads: 50

```
Looking at his values I don't think he studied enough about the bldc tool to use it TBH.
@nordlicht try @Ackmaniac VESC tool. It has wizards that can guide you through all you have to set up to get it working. Also study study  study. 9h read time is actually quite low.
```

---
## \#16 Posted by: nordlicht Posted at: 2018-06-14T13:44:25.640Z Reads: 48

```
WHat do you mean by motor detection? detection of the parameters for FOC and hall sensor detection? yes I did, or do you talk about something different?
```

---
## \#17 Posted by: nordlicht Posted at: 2018-06-14T13:45:38.489Z Reads: 47

```
Alright, just downloaded the VESC tool from Ackmaniac. You got recommendations where to start reading?
```

---
## \#18 Posted by: Sn4pz Posted at: 2018-06-14T13:45:44.686Z Reads: 48

```
i remember that between the help on here and myself, I wouldnt allow myself to change anything on the vesc until I had watched that long vesc setup tutorial and read  :laughing:
```

---
## \#19 Posted by: Ebisane9 Posted at: 2018-06-14T13:46:16.794Z Reads: 46

```
oh hell yeah. I watched a dozen vesc setups
```

---
## \#20 Posted by: Sn4pz Posted at: 2018-06-14T13:46:22.607Z Reads: 48

```
ignore that comment im a boob.

edit ill find the video for you to watch, its full of the kind of basic knowledge you may( or may not) need :)
```

---
## \#21 Posted by: Ebisane9 Posted at: 2018-06-14T13:49:05.812Z Reads: 45

```
just search vesc beginner guide on the search bar. 
Literally search whatever comes to mind
Things I've typed:
"Motor amps for peak performance"
"battery max"
"will I blow my vesc"

whatever is on your mind, then read read read and ask questions. Lots of knowledgeable guys you can run to on here. the higher their reading time the more helpful they likely are. People with multiple build ++++. Trusted Vendors +++
```

---
## \#22 Posted by: Sn4pz Posted at: 2018-06-14T13:49:08.856Z Reads: 43

```
Nice informative thread right here: http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

and heres the video everyone will show you, its a staple :)  https://www.youtube.com/watch?v=5HLZaMcYRuY
```

---
## \#23 Posted by: nordlicht Posted at: 2018-06-14T13:53:34.514Z Reads: 43

```
Thanks a lot, both of you!
```

---
## \#24 Posted by: Sn4pz Posted at: 2018-06-14T13:55:13.942Z Reads: 40

```
additionally, if it helps, I ran my hubs with FOC but it was sensorless.... could be a reason your chip ate it....

also 53 for maximum input voltage isnt proper, its supposed to be 57.... I cant explain why but Ive seen multiple people who say its not a good setting to touch.... 

maybe next time you setup the vesc go small and work your way up ( first dial bldc settings in, make sure it works, then move on to FOC ) 

make sure you change not only the stuff in the FOC tab but also under the app configuration make sure you take care of all the stuff like control mode and what not

I try my best :)  good luck man
feel free to pm with any questions :)
```

---
## \#25 Posted by: Ebisane9 Posted at: 2018-06-14T14:07:29.269Z Reads: 37

```
yup @nordlicht feel free to pm!
```

---
## \#26 Posted by: willumpie82 Posted at: 2018-06-14T14:15:36.404Z Reads: 37

```
Did you check the 5v rail? is there anything getting hot on the board (e.g. the TVS diode near the ppm input), that rail should be close to 5v +/- 0,1v. above or below that the drv will give errors, but USB still works (uC works of 3v3)
```

---
## \#27 Posted by: Static Posted at: 2018-06-14T14:41:42.150Z Reads: 35

```
I'm running FOC on HW4.12, is there a way to set limits to avoid this? What about sensored BLDC?
```

---
## \#28 Posted by: Pimousse Posted at: 2018-06-14T14:45:35.759Z Reads: 35

```
There not so much solution apart avoid using more than 8S voltage I would say (for a reliable VESC I mean, there is always someone who succeeded running a couple of seconds a 80100 with 13S in FOC with Maytech VESC...).
I would advice you to switch to BLDC mode with those VESC.
```

---
## \#29 Posted by: Static Posted at: 2018-06-14T15:19:29.602Z Reads: 35

```
Gonna give the sensored BLDC a shot. Is there a good vesc6 out that can run FOC reliably on 12s?
```

---
## \#30 Posted by: Sn4pz Posted at: 2018-06-14T15:26:34.608Z Reads: 39

```
http://www.trampaboards.com/vesc-6-library-c-895.html

probably your only option....
```

---
## \#31 Posted by: Static Posted at: 2018-06-14T15:53:54.052Z Reads: 35

```
The price to replace my two TB ESC's, the price has got to come down on these. 

![image|481x135](upload://yuIe4uEmjocPKmBvlVNGOM6LP08.png)

hopefully FOCBOX unity gets released soon
```

---
## \#32 Posted by: Sn4pz Posted at: 2018-06-14T16:06:49.904Z Reads: 32

```
yeah... something something frank... lol. 

maybe stick with dual focboxes and put them in @Kug3lis s case? It seems to do a good job.... I havnt recieved mine yet though. Im just relaying what ive been told :)
```

---
