# Bestech BMS, Switch not working

### Replies: 51 Views: 1933

## \#1 Posted by: Muke Posted at: 2018-04-25T22:03:31.992Z Reads: 180

```
Hey guys,

I finally found the time to put together my first esk8 and I currently have a few issues I could not find an answer to on this forum.

BMS: I'm using @Namasaki's [10s Lipo battery setup](https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014) with the exact same Turnigy 5000mah batteries and the Bestech HCX-D223V1 10s BMS. The issue is: for some reason my switch function doesn't work. It is always on, so the only way to turn on and off my board is to plug in and out one battery connection. I checked the resistance of the switch and of the solder points of the white wire and there are no shorts and the switch is working as it's supposed to be.
Has anyone had a similar problem?

Vesc: I'm using the hobbyking vesc and with the settings from this [thread](https://www.electric-skateboard.builders/t/vesc-configuration-10s-6374-sk3-15-36-gearing/15943) because I have the same 6374 sk3 as well. The issue now is that if I use 36 as the cutoff start voltage and 35 as the cutoff end voltage I can't do a motor-detection. I measured the voltage of my battery pack and it is a bit over 37V. So I lowered the cutoff start and end to 33 and both the motor detection and the power delivery worked fine. Then I put the cutoff start and end back to the previous settings (36 and 35) and the power delivery got really poor and the motor only pulled 4A.
So I think my Vesc is somehow getting a wrong voltage measurement.
I found a thread witch a similar problem on the forum and charging could help here so I will test that out tomorrow. But maybe someone has an other solution to this problem too?
```

---
## \#2 Posted by: Juiced Posted at: 2018-04-25T22:49:07.139Z Reads: 158

```
Same for me, my voltage when on is about 3-4v lower
```

---
## \#3 Posted by: Namasaki Posted at: 2018-04-25T23:06:37.638Z Reads: 151

```
If you test the bms without the vesc connected, it will seem to stay on after your turn it off because there is no load to drain the voltage down.
Even with the Vesc connected, it takes a few seconds for the voltage to drain down.
```

---
## \#4 Posted by: Muke Posted at: 2018-04-25T23:06:50.119Z Reads: 151

```
I actually never measured the voltage when my battery is connected. Thanks, I will check that tomorrow too
```

---
## \#5 Posted by: Muke Posted at: 2018-04-25T23:11:25.302Z Reads: 146

```
Thank you for answering so quickly! Unfortunately I don't really understand how this could affect the switch not being able to turn on and off the vesc when it is connected or affecting the voltage measured by the Vesc.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-04-25T23:14:36.783Z Reads: 137

```
Ok, I wasn't sure if you had the Vesc connected or not.
Some people in the past had thought something was wrong with the e-switch when they tested it without the Vesc connected.
```

---
## \#7 Posted by: Muke Posted at: 2018-04-25T23:15:45.706Z Reads: 132

```
I will elaborate my problem further: When I close whole the circuit of my battery, Vesc and BMS the Vesc turns on, no matter if my switch was in the on or off position. Then I test the switch and again: no matter the position of the switch the vesc stays turned on until I open the whole circuit manually (unplugging a battery wire) again.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-04-25T23:21:57.208Z Reads: 124

```
Are you using a simple button switch with 2 solder posts or the one with led and 4 solder posts?
```

---
## \#9 Posted by: Muke Posted at: 2018-04-25T23:24:14.345Z Reads: 123

```
One with Led and 5 solder points, 2 for the LED and the other 3 pins are for NO (normally open), NC (normally closed) and ground where I soldered to the NO and ground pin.
I'm not powering the LED though, but that's the way I measured it too and the resitance was really big when open and really small when closed
```

---
## \#10 Posted by: Namasaki Posted at: 2018-04-25T23:26:55.893Z Reads: 120

```
Did you wire it like this:

![25 AM|610x500](upload://n2NzG7HdEK1u4JSxnRgvKHUtAuM.png)
```

---
## \#11 Posted by: Muke Posted at: 2018-04-25T23:27:41.673Z Reads: 116

```
Exactly, only the green wires are connected at this stage
```

---
## \#12 Posted by: Namasaki Posted at: 2018-04-25T23:31:54.478Z Reads: 115

```
It is very uncommon for the e-switch to fail on that bms but it is possible.
I would double check the e-switch wires where they connect to the bms and make sure there isn't any solder bridge.
also double check the wires that they aren't touching where they solder to the bms.

Then email bestech about it.
```

---
## \#13 Posted by: SpartanFrench Posted at: 2018-04-25T23:37:40.407Z Reads: 119

```
I will link my post here because I have similar issue

https://www.electric-skateboard.builders/t/help-bms-always-on-e-switch-not-working/53090
```

---
## \#14 Posted by: Muke Posted at: 2018-04-25T23:45:38.488Z Reads: 117

```
I rechecked the resistances and the Led switch is working but there seems to be a short between the upper right and the 2 bottom pins on the BMS.

![Switch issue|375x500](upload://xF8RrM9wfMbQGF0oAOzFVCxbUfy.jpg)
```

---
## \#15 Posted by: Muke Posted at: 2018-04-25T23:48:55.587Z Reads: 111

```
I guess that's not how it is supposed to be?
```

---
## \#16 Posted by: Namasaki Posted at: 2018-04-26T00:45:49.562Z Reads: 109

```
Maybe the wires are touching together under the white goop they put on it.
```

---
## \#17 Posted by: Muke Posted at: 2018-04-26T12:16:06.197Z Reads: 102

```
Somehow I measure a negative resistance when the switch is on the off-position. Any idea what this could mean?
```

---
## \#18 Posted by: mmaner Posted at: 2018-04-26T12:21:22.539Z Reads: 102

```
I assume you have tried removing the switch and isolating the leads to see if it switches off?
```

---
## \#19 Posted by: Muke Posted at: 2018-04-26T12:25:33.977Z Reads: 99

```
Yes, but I will remove the switch again now to check if the negative resistance is also measured only between the 2 white cables
```

---
## \#20 Posted by: Namasaki Posted at: 2018-04-26T12:32:02.548Z Reads: 97

```
I’m not an electronics engineer but I think that the 2 white wires when connected, close a circuit. 
And when you test them with an ohm meter you are closing the circuit. Therefore you are reading the resistance of the circuit.
```

---
## \#21 Posted by: Muke Posted at: 2018-04-26T12:33:49.279Z Reads: 93

```
That makes sense. But I measure -2,45 Mega ohm. Isn't it weird that I measure a negative resistance?
```

---
## \#22 Posted by: Namasaki Posted at: 2018-04-26T12:39:16.580Z Reads: 90

```
Try reversing the test leads.
```

---
## \#23 Posted by: Muke Posted at: 2018-04-26T12:47:45.763Z Reads: 90

```
If I reverse them it won't show the resistance, which makes it even weirder
```

---
## \#24 Posted by: Muke Posted at: 2018-04-26T12:56:43.932Z Reads: 93

```
I must have done that 20 times now and repeatedly gives me the same result. I get a measurement of -2.45 Mohm with the test lead the one way constantly and I get no measurement when I switch the test leads
```

---
## \#25 Posted by: Muke Posted at: 2018-04-26T13:01:55.922Z Reads: 91

```
The negative resistance is measured between the 2 white leads of the BMS. The switch is working fine regarding that I get 0 ohm when the button is pressed in and no measurement (probably too high to measure) when it is in it's off position.
```

---
## \#26 Posted by: mmaner Posted at: 2018-04-26T13:17:59.901Z Reads: 92

```
OK, what I'm trying to figure out is if you have removed the switch and isolated the leads.  If so is the BMS off?  when you touch the leads together is it on?  All the switch leads do is complete the circuit, they are not positive and negative.
```

---
## \#27 Posted by: Muke Posted at: 2018-04-26T13:28:07.149Z Reads: 91

```
The board turns on when I plug in the battery, no matter if the leads are touching or not. Then touching the leads or not doesn't have any effect
```

---
## \#28 Posted by: mmaner Posted at: 2018-04-26T13:34:31.619Z Reads: 88

```
then the BMS is bad.  You easiest solution is to contact BesTech and get a replacement.
```

---
## \#29 Posted by: Muke Posted at: 2018-04-26T13:45:13.683Z Reads: 84

```
I think so too, thanks. The problem is that I didn't buy from Bestech directly but from a seller. I will contact him now
```

---
## \#30 Posted by: Muke Posted at: 2018-05-08T13:08:16.804Z Reads: 79

```
He will send me a knew one, but I want to try to fix this one first
```

---
## \#31 Posted by: Muke Posted at: 2018-05-08T13:13:02.468Z Reads: 83

```
Can anyone tell me if these pins are supposed to be shorted?

Respectively, what this part is used for?
![Forum 2|281x500](upload://mYfj1bMcbdbnfwew6YGpRktWaVK.jpg)
```

---
## \#32 Posted by: mmaner Posted at: 2018-05-08T14:57:50.212Z Reads: 82

```
thats the temp sensor
```

---
## \#33 Posted by: Muke Posted at: 2018-05-08T15:31:37.702Z Reads: 81

```
Thanks! Do you know how it works?

Is it supposed to create a short when the temperature-cutoff of the BMS is NOT reached? (and open when it is reached?)
```

---
## \#34 Posted by: mmaner Posted at: 2018-05-08T15:44:04.012Z Reads: 80

```
I honestly have no idea how it operates.  I would ask lucy@bestechpower.com.
```

---
## \#35 Posted by: Muke Posted at: 2018-05-08T15:44:51.068Z Reads: 79

```
Ok thanks!
```

---
## \#36 Posted by: t0m_r1dd1e Posted at: 2018-05-08T16:26:21.915Z Reads: 80

```
It's probably just a thermistor, always a closed circuit that varies resistance depending on temperature.
```

---
## \#37 Posted by: Muke Posted at: 2018-05-15T22:31:51.670Z Reads: 81

```
Somehow my problems solved themselves...
What happened: Since the button was not changing anything and the BMS and VESC where powered on anyway as soon as I plugged in my battery I didn't have my switch soldered to my setup anymore when I started testing my board for the first time after having loctited and secured everything properly. The board itself performed great for about 1km and then suddenly powered off. I already thought I smoked something because there was no more spark after unplugging and plugging back in my battery connection. Then I shorted the 2 white wires of the BMS manually again (had tried it before that test already) and the VESC turned on. So I soldered back on my switch and ever since everything is working just fine.

Thanks a lot for your help guys!

Edit:
VESC issue solution: Fully charging my battery solved my issue that the power delivery was poor. Disconnected my battery had a Voltage of 37,5V and as soon as I powered my motor with it it probably dropped below 3,6V or 3,5V which triggered the cutoff start/end
```

---
## \#38 Posted by: Chase Posted at: 2018-05-16T02:20:02.259Z Reads: 75

```
I’m having his exact same problem. I tried what you said I and it didn’t fix anything
```

---
## \#39 Posted by: Muke Posted at: 2018-05-16T14:14:19.254Z Reads: 69

```
I edited my solution reply.
```

---
## \#40 Posted by: Muke Posted at: 2018-05-16T14:19:13.080Z Reads: 72

```
I guess you are talking about my BMS related problem that the switch is not working? Do you also have the Bestech HCX-D223V1 10s BMS and this problem: 

[quote="Muke, post:1, topic:53504"]
for some reason my switch function doesn’t work. It is always on, so the only way to turn on and off my board is to plug in and out one battery connection. I checked the resistance of the switch and of the solder points of the white wire and there are no shorts and the switch is working as it’s supposed to be.
[/quote]

Maybe some pictures of your BMS could help :)
```

---
## \#41 Posted by: Chase Posted at: 2018-05-16T21:39:33.302Z Reads: 65

```
I actually have a very similar model, the 12s HCX-D596. I’ve about given up on it. I tried the things you described and it still just won’t turn off. In fact the only way to get the pack switched off was to remove the B- solder and unplug the balance pin set. I’m just going to buy a new d223 model for a 12s. I know that it’s just a short somewhere but at this point I’m going to just take the easy way out. 

Thank you so much for trying to help
```

---
## \#42 Posted by: Muke Posted at: 2018-05-16T22:11:58.526Z Reads: 65

```
Do you have a multimeter to measure if the switch is working correctly?
I had testet the e-skate before too and it was only after about 1km of total testing that it suddenly started to work
```

---
## \#43 Posted by: Muke Posted at: 2018-05-16T22:17:19.320Z Reads: 63

```
I could check voltages and resistances again to see what has changed since mine is working now, that could help.

I did other things that I did not mention here too, for example I took off the temperature sensor a few times (just screwed it off the heatsink) and put it back on. Maybe something has changed there too.
```

---
## \#44 Posted by: Chase Posted at: 2018-05-16T22:22:12.113Z Reads: 62

```
I did test the switch with the multimeter. It was stranger that there was voltage between the wires but snipping then apart did nothing to turn it off.
```

---
## \#45 Posted by: Muke Posted at: 2018-05-16T22:28:20.583Z Reads: 64

```
That's weird, so you measured voltage between the wires in eather position of the switch? Did you try taking off the switch and shorting the wires by hand? That seems like the switch itself is defect
```

---
## \#46 Posted by: Chase Posted at: 2018-05-16T22:34:08.651Z Reads: 65

```
Yep did both. I also believe it’s just a defect in the eswitch. Lucy from bestech couldn’t figure it out either. I’m just going to try to stick to the more common d223v1 model for 12s. Thanks for your time
```

---
## \#47 Posted by: Muke Posted at: 2018-05-16T22:50:09.023Z Reads: 65

```
OK, I hope everything will work out then :) you're welcome
```

---
## \#48 Posted by: wabbawabbe Posted at: 2018-09-04T09:17:26.552Z Reads: 56

```
This may be a common problem with these BMS, as I have a 10s HCX-D596 and have the same issue with the bms not turning off. @Chase were you able to fix your problem?
```

---
## \#49 Posted by: Chase Posted at: 2018-09-05T02:44:37.552Z Reads: 54

```
I was not ever able to figure it out. I ended up getting a different model.
```

---
## \#50 Posted by: wabbawabbe Posted at: 2018-09-08T22:20:52.014Z Reads: 51

```
Managed to solve my problem - I double checked the wire solder points on the back with a voltmeter and voila - turns out the solder points were bridged. After desoldering the excess solder it works perfectly fine! thanks @Namasaki
```

---
## \#51 Posted by: Namasaki Posted at: 2018-09-09T03:34:53.275Z Reads: 47

```
the solder points for the switch and thermal sensor are too close together. They should have spaced them further apart on the PCB
```

---
