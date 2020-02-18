# Motor cutting out when accelerating (solved I think)

### Replies: 15 Views: 2887

## \#1 Posted by: Cube Posted at: 2016-05-09T23:39:16.870Z Reads: 216

```
As title says.. I'm running a vesc with 8s lipo and tacon 245kv and a gt2b bad wolf mod. I have read everywhere trying to figure this out to no avail. I'm fairly sure it's not the gt2b. I have lowered the vesc battery cutoff start and stop to 27.5v start 24v stop which should be plenty. Not sure what else to try and this cutout has made me faceplate twice now. That cutout only lasts for half a second and it seems to happen at random. Any guesses or suggestions?
```

---
## \#2 Posted by: makevoid Posted at: 2016-05-09T23:51:24.709Z Reads: 215

```
i guess you have to increase motor max and/or battery max because there's not enough power for your motor, or it could be a battery issue not outputting enough amps, What battery do you have? What's your C rating?

i'm no expert I have the vesc from 3 days and I'm still trying the configs, I had your same problem and it seems solved by increasing those two values,

It could also be the remote connection flaky but that will happen not only when accelerating but also when cruising or worse when braking. But if it was like me, that happened only when accelerating hard, and especially uphill, then it should be a power/amps problem caused by settings or battery discharge rate. Hope this helps.
```

---
## \#3 Posted by: treenutter Posted at: 2016-05-09T23:55:25.847Z Reads: 205

```
@cube I ride a similar setup with VESC, gt2b and 8s. If your cutoff voltages are set properly, and there is no issue with the gt2b, I'd look at the max Amps you've configured VESC to pull. Is that setting aligned w your battery system? Is it possible that the battery is damaged and sagging during discharge?

It might help to try limiting your top speed temporarily using the rpm limits in VESC. A lower rpm range might also limit the voltage drawn so you can ride safely while you figure this out.
```

---
## \#4 Posted by: Cube Posted at: 2016-05-10T00:08:45.493Z Reads: 185

```
@makevoid they are zippy compact 25c 5800 and are almost brand new all cells are good so I don't think it's a bad battery. 
@treenutter  I think the cutoff start at 27.5v and end at 24v are good. The max amps are at default of 60amps. Do I need to change the amps or cutoffs based on these batteries?
```

---
## \#5 Posted by: treenutter Posted at: 2016-05-10T00:36:05.673Z Reads: 179

```
@cube For 8S I set the cutoff start value at 28.0 and the cutoff end at 26.4. I use similar batteries, the 5000mAh version of the Zippy 4S compact, also at 25C. I'll take a screenshot of my VESC parameters so you can compare. Have you adjusted the pulsewidth for PPM control?
```

---
## \#6 Posted by: Cube Posted at: 2016-05-10T02:29:25.146Z Reads: 166

```
A screen shot would be awesome. I ran identical cutoffs and lowered them even more to make sure that wasn't the issue. I change the battery max amps  from 60 to 80amps. Just went out and it's still cutting out. I also did do the pulsewidth.
```

---
## \#7 Posted by: hexakopter Posted at: 2016-05-10T12:28:10.442Z Reads: 157

```
What is when you connect your VESC to the PC after you have this failure and type "faults" in the terminal? (without a reboot/ so not disconnect from power source)
```

---
## \#8 Posted by: chaka Posted at: 2016-05-10T12:38:17.657Z Reads: 152

```
I believe you need to be connected to the bldc-tool to log faults.
```

---
## \#9 Posted by: chaka Posted at: 2016-05-10T12:40:59.392Z Reads: 151

```
@cube If the cutout only lasts half a second then it is most likely your remote or a bad connection somewhere. If it were a VESC fault it would last a few seconds before regaining power.
```

---
## \#10 Posted by: hexakopter Posted at: 2016-05-10T13:02:36.415Z Reads: 146

```
I mean the bldc-tool terminal. :) So connecting to PC = connecting to bldc-tool
I know that at least a over current fault last longer, but would be good to exclude a VESC detected fault.
```

---
## \#11 Posted by: chaka Posted at: 2016-05-10T13:06:44.600Z Reads: 143

```
I think you need to be connected to a pc during the fault for it to log.
```

---
## \#12 Posted by: hexakopter Posted at: 2016-05-10T19:39:34.770Z Reads: 135

```
You produce these things in lots so you must know it. :grin:
But I can tell you that my VESC is saving its faults and they can be read (in the bldc-tool terminal) after the ride. So no connection is needed while driving. Just don't power the vesc of between the ride and the fault reading.
```

---
## \#13 Posted by: Cube Posted at: 2016-05-10T20:04:37.666Z Reads: 131

```
@hexakopter OK thanks... I'm not seeing any faults from the vesc.
@chaka every connection on the board seems to be really solid. I now have a new weird symptom. When I'm cruising on flat ground at about 10mph and let off the trigger the motor makes a little stuttering like I'm tapping the trigger. I'm starting to think this is a transmitter/receiver issue but I haven't heard of one person having issues with the gt2b. Another odd thing I can do is put the board about 15 feet away from me and when I tap the trigger for what should be a small Rev from the motor it ends up acting like I held it at half throttle for two seconds. Doesn't do this when I'm within a foot or two of the board. Any ideas? I only have the one bad wolf gt2b so I can't trouble shoot with another controller. Thanks for the help.
```

---
## \#14 Posted by: Cube Posted at: 2016-05-12T02:51:41.478Z Reads: 122

```
Just realized how close my battery leads were to my vesc receiver connection and the actual receiver. Remembering back to my rc days all cables can cause interference. Moved the vesc and receiver to another location. Went for a test ride and not a single cut out. Then my motor mount snapped about 5 miles into the ride. So for now this is case closed.
```

---
## \#15 Posted by: SteveS Posted at: 2016-07-19T19:29:23.972Z Reads: 107

```
Any update, Cube? I'm having the same problem with power cutting out on acceleration. I've had the problem very intermittently for some time, but it has become much more common since I made two changes: updated the firmware to 2.18 and starting using a Steez remote.
```

---
