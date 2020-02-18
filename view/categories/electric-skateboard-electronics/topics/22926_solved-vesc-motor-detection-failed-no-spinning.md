# \[solved\] VESC - Motor Detection Failed (No spinning)

### Replies: 26 Views: 2372

## \#1 Posted by: cricrithezar Posted at: 2017-05-13T02:12:40.882Z Reads: 145

```
EDIT: Looks like the temperature reading was was off (113C when idle) and that was causing the vesc to not want to spin the motor. Bumping up the mofset max temp made it spin but this isn't really a fix since i have no idea what the actual temperature of the chip is. It looks like a hardware defect with the VESC, shouldn't be too hard to fix and they offered to replace it so I'll probably go with one of those two options.

Hi!

Sorry if you see these all the time (I'm sure that's the case given how many of these threads I've read and still couldn't fix my issue).
I have my VESC set at pretty standard settings. Just changed the battery cutoff start to 33V (which is way lower than my current voltage of 38V on my 10s4p battery). I tried running it with both the stock and Ackmaniac firmwares and had the same results (it's the hw4.12 vesc from diyelectricskateboards). My motor is a 192kv 6374 turnigy sk3 if that makes any difference. Tried various minimum erpms. Not sure what's wrong, when I run motor detection, the motor doesn't even react, it just sits there and after a few seconds outputs a detection failed message.

I'm using this config and I can see the motor spinning in realtime data (when I spin it with my hand) so the connection is probably good enough for it to at least try to spin it up:
<img src="/uploads/db1493/original/3X/0/e/0eb21fdf1b6f5aca8207e98083cec861b3c59ba7.png" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/d/dda7d796672e88cf66dd5e7b6554868685ca5fbb.png" width="690" height="388">

Is there anything I'm doing wrong? First time using a VESC
```

---
## \#2 Posted by: mmaner Posted at: 2017-05-13T02:16:39.042Z Reads: 127

```
On your current limits i would start with 60, -60, 60, -30 ams adjust from there after your running  

Have you setup PPM yet?  Go to app > general and select PPM and click write.  The got to app > PPM and select watt/current no reverse with brake and click write.  

That should get you running.
```

---
## \#3 Posted by: cricrithezar Posted at: 2017-05-13T02:24:18.561Z Reads: 129

```
I just set it to 60,-60,30,-30 (my motor is 80 though, but I guess that won't hurt it in any case).
PWM was set up, and I could see it change (can't find a receiver, I'm still waiting for it to get here so I'm using an arduino instead, but the pwm reading was varying which means it should work).
Still not spinning though. I'm not quite sure what's wrong. Can't see changes in pulsewidth anymore with the new firmware/software, but even with the motor detection nothing happens.

<img src="/uploads/db1493/original/3X/0/a/0aa15eed44386816af946780d488c28e99fa9ea3.png" width="690" height="388">
```

---
## \#4 Posted by: mmaner Posted at: 2017-05-13T02:27:13.880Z Reads: 108

```
Just because the PPM signal moves doesn't mean that your Arduino is working.  With my remote off and the RX unplugged it still bounces a little.  Can you move the motor using the arrow keys?  Look at the @Ackmaniac firmware, gives a lot more options and a ton of explanations.  Double check the PPM is selected in app > general.  Do a read when on that tab.

Edit: I see you are running the @Ackmaniac firmware, carry on.
```

---
## \#6 Posted by: cricrithezar Posted at: 2017-05-13T02:30:41.706Z Reads: 104

```
actually you were right I didn't reboot but that's still not fixing the issue. PWM signal is now showing but still no motor spinning
```

---
## \#7 Posted by: cricrithezar Posted at: 2017-05-13T02:32:16.156Z Reads: 105

```
Yes I have PPM set in  general and I have now rebooted. The arduino changes the PWM signal from 0 to 0.98ms in the PPM tab. Still, no dice.

<img src="/uploads/db1493/original/3X/5/e/5e12841c6e911bfaafccf8020750c0b765b1131b.png" width="690" height="388">
```

---
## \#8 Posted by: Blasto Posted at: 2017-05-13T02:34:06.008Z Reads: 97

```
Ah so you're using an arduino, make sure your signal passes through the safe start (dead zone)
```

---
## \#9 Posted by: mmaner Posted at: 2017-05-13T02:35:19.774Z Reads: 94

```
Can you move the motor using the arrow keys? Make sure KB Ctrl is ticked on the motor > bldc tab.
```

---
## \#10 Posted by: cricrithezar Posted at: 2017-05-13T02:39:13.396Z Reads: 100

```
Just found a controller-receiver combo. I can make it vary from 1ms to 2ms which does display on the PPM tab. Can't see keyboard controls anywhere on the BLDC tab.
<img src="/uploads/db1493/original/3X/b/c/bc483de40fac9ba1b752f41ebe45dd07e2e69c3d.png" width="690" height="388">

Thanks for the help in any case. I'm slightly confused and getting limited feedback from both the software and the hardware doesn't help.

EDIT: just found it, but it's enabled already.
```

---
## \#11 Posted by: mmaner Posted at: 2017-05-13T02:40:42.130Z Reads: 95

```
KB Ctrl is on the bottom right, it's ticked in your screen shot. Just use the arrow keys 1 at a time and see if the motor moves.
```

---
## \#12 Posted by: cricrithezar Posted at: 2017-05-13T02:41:27.431Z Reads: 95

```
No motor movement unfortunately.

EDIT: Oh this is wierd. Mofset temp is being read as 113C

<img src="/uploads/db1493/original/3X/d/8/d80b665a15a08fc6514435a1391ef49c473d81ae.png" width="690" height="388">

EDIT2: Changed that and it worked. Really wierd my read mofset temps are so high. They're not even hot to touch. Is this something I can fix in software? Maybe recalibrate it?
```

---
## \#13 Posted by: mmaner Posted at: 2017-05-13T02:46:17.685Z Reads: 88

```
What are you peering the VESC with?
```

---
## \#14 Posted by: cricrithezar Posted at: 2017-05-13T02:52:39.622Z Reads: 94

```
So it seems that the relative temps are being somewhat read (not sure how accurate they are). But the base temp is 113C. 

<img src="/uploads/db1493/original/3X/0/b/0b80f69e6fcf50c4ee02244952dfb58cff5b779e.png" width="690" height="388">

I'm just using my finger to feel if it's hot and there's a thick layer of heat shrink on there but it's definitely not 113C. Is this something that has to be calibrated?
```

---
## \#15 Posted by: mmaner Posted at: 2017-05-13T02:55:14.636Z Reads: 91

```
I really don't know, never had that problem across a dozen VESCs. If your using a 3s or 4s battery to power the VESC that might cause weird shit, at least is has for some people in the past. I would see if you can contact diy support via the chat bubble on the website, or ask @torqueboards here.
```

---
## \#16 Posted by: cricrithezar Posted at: 2017-05-13T02:56:27.031Z Reads: 91

```
After a bit of research, it looks like it might  hardware https://www.electric-skateboard.builders/t/solved-mosfets-over-temp/19461/6
Bought it around that time too.

@torqueboards is this something I have to return my VESC for or is there some conversion factor I can use to set my max temps (since I assume it was just the wrong kind of thermistor giving the software the wrong value?)

EDIT: Also @mmaner thank you for the help. Took a long time to notice that value especially since it's half cut off on that page.
```

---
## \#17 Posted by: mmaner Posted at: 2017-05-13T03:13:34.571Z Reads: 88

```
No worries brother, wish we could've gotten you on the asphalt today.
```

---
## \#18 Posted by: torqueboards Posted at: 2017-05-13T03:19:49.463Z Reads: 87

```
@cricrithezar send us an email help@. We'll replace your VESC if it's related to the R1 temp issue.
```

---
## \#19 Posted by: cricrithezar Posted at: 2017-05-14T19:32:40.004Z Reads: 79

```
@torqueboards I sent an email and a replacement would probably be the safest solution. Is there any way I could know what the issue with the R1 thermistor was and if it would be possible to simply change the max temp in software to take into account the different resistance of the thermistor? Or do you simply recommend not using this VESC at all? Everything else seemed to be working fine and I would be fine keeping this VESC if this is something I can fix on my end.
```

---
## \#20 Posted by: torqueboards Posted at: 2017-05-14T21:35:15.904Z Reads: 77

```
You can replace the R1 located here and/or we'll send you an RMA and we can send you a new one without the R1 issue.

I wouldn't recommend using it with the R1 issue.

<img src="/uploads/db1493/original/3X/2/4/24e8997b3a71fba1729e8013aa42691e9eb27fc9.png" width="351" height="500">
```

---
## \#21 Posted by: cricrithezar Posted at: 2017-05-14T21:44:16.792Z Reads: 72

```
Thanks for the reply, I'll probably RMA it but would you happen to know what NTC thermistor was used on that batch?

EDIT:
After looking at the datasheet on mouser it looks like you used the 1kohm thermistors (assuming that was the only error, if you have the part number I'd love to know to make sure, as I said everything else seems ok and this can likely be fixed in software), which means I should be able to find the temperatures that the software will see for the temperatures I actually want. This also makes sense since the temperature seen by the software is higher than the actual temp and my values fall right about where they should.
I'm working on a spreadsheet and will report back (not testing it, but I'm fairly confident this should work without replacing the resistor).

Ok calculator is done but the resistance value seems funny. If you can give me the exact part name I can find the temperature characteristics value B and that should give me the correct values. I'll stay on the conservative side since it won't be as accurate but it should work:

<img src="/uploads/db1493/original/3X/5/e/5e2769c0ccb99337d9767e9616ea53d164ad6a37.png" width="690" height="150">

I can post this once I test it out but I don't want to be the reason other people fry their vescs haha.

In any case I'll set it to something low (maybe an actual limit of 70C), but also current limited since it'll probably be fine temperature wise as long as I'm below 50A (my limit is set to 40A right now).
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2017-05-14T22:42:33.567Z Reads: 71

```
the right parts is suppose to be a 10K Thermistor 81-NCP18XH103F03RB
```

---
## \#23 Posted by: cricrithezar Posted at: 2017-05-14T22:45:54.548Z Reads: 70

```
yeah that's what I have (what the software thinks it is). Maybe it's not clear on my spreadsheet. I'll make sure to polish it a bit more if this actually works and I end up posting it.
The R1 value I get though should be about 1k since they only go in 10x increments. My B_real value is probably wrong.

EDIT: edited my comment with better values and clearer instructions, they're not quite exact without the part numbers but it should be on the more conservative side. I'll link the spreadsheet if this works.

EDIT2: I'll also probably get more error in the temperature measurements (more jitter in the data) since the resistance values will be lower (higher temps mean lower resistance for these thermistors) so I'll have to make sure that's not an issue.
```

---
## \#24 Posted by: torqueboards Posted at: 2017-05-15T00:59:45.104Z Reads: 64

```
It was the same but supposedly the batch was damaged somehow. NCP18XH103F03RB
```

---
## \#25 Posted by: cricrithezar Posted at: 2017-05-15T01:02:27.214Z Reads: 61

```
Wierd, well I'll probably just return it then, but it's funny that all the boards display the same temperature of ~113C.
Thanks for the feedback in any case, was just trying to find a way not to have to return it.
```

---
## \#26 Posted by: torqueboards Posted at: 2017-05-15T01:03:38.080Z Reads: 60

```
@cricrithezar You can just replace the R1 component and it would be perfectly fine. If you didn't want to go through the trouble. You can send it back and we'll send you a new one.
```

---
## \#27 Posted by: cricrithezar Posted at: 2017-05-15T01:05:44.366Z Reads: 60

```
I might do that then, might tinker around with it to see if temperatures are measured in a predictable manner since the max temp is adjustable. Thanks for all the feedback, sorry for the many questions.
```

---
