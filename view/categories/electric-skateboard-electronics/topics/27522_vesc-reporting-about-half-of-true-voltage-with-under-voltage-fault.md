# VESC reporting about half of true voltage with UNDER_VOLTAGE fault

### Replies: 9 Views: 446

## \#1 Posted by: bmcm Posted at: 2017-07-13T14:42:55.182Z Reads: 60

```
I wish I took a screenshot or video, sorry. But in essence, after adjusting my motor mount and plugging everything back together, my motor would just jerk. I thought it was the belt tension being too tight (I did work on that, as it was too loose before), and it was too tight and very difficult to turn. So I fixed that. But the motor would still not spin and just jerk.

TL;DR I plugged in the ESC into BLDC-tool and noticed it faulted UNDER_VOLTAGE, and was reporting 5-20 volts (all over the place). I checked connections, rebooted the ESC, several times. I verified with my multimeter that the voltage coming into the ESC was 39 to 40 volts, which is what my voltage meter attached directly to the BMS was reporting.

I read that it's possible my resistors for the voltage divider became loose and are causing extra resistance, thereby messing up the math. A visual check of the ESC didn't reveal any obvious issues with those resistors, though. Difficult to tell for sure because of Ollin's aluminum plate over that side of the ESC.

What's the fix? Or any other ways I can debug the problem? It's not throwing any DRV faults, and nothing visible looks "blown." Do I need to get Ollin to repair/replace it?

I can upload photos if necessary when I get home tonight.
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-13T14:48:22.366Z Reads: 57

```
Perhaps @chaka can provide input. Just curious, what do you have your battery cutoff values set to, not that it matters much given the reported voltage you mentioned.
```

---
## \#3 Posted by: chaka Posted at: 2017-07-13T15:31:37.087Z Reads: 51

```
Sounds like a minor short somewhere down stream of the DRV chip. If you a sure that your connections are insulated and not a source of the issue please send it in and we will repair or replace the unit.
```

---
## \#4 Posted by: bmcm Posted at: 2017-07-13T15:39:26.299Z Reads: 48

```
Thanks, @chaka, for the quick response. Which connections specifically should I check for a short? And how do you recommend I remove the aluminum heatsink plate (not the finned one on the ports side, but on the underside to access the power input lines and the resistors)? I removed the screws, obviously, but I'm afraid to apply heat to melt the thermal paste that seems to be holding it together.
```

---
## \#5 Posted by: bmcm Posted at: 2017-07-13T15:40:19.482Z Reads: 45

```
@Jinra IIRC, cutoff is at 30 volts.
```

---
## \#6 Posted by: chaka Posted at: 2017-07-13T15:47:40.445Z Reads: 44

```
I generally prefer customers send the unit in for repair if they are at all worried about ruining something. All it takes is for someone to lift a trace and the pcb will be unusable or more difficult to repair. The thermal paste is a silicone product so it will break the bond easily one you unscrew the mounting hardware.

Sometimes a poor connection through the adc port or sensor port can cause problems. In either case you can send it back for repair just don't want you to send it back if it is an easy fix.
```

---
## \#7 Posted by: bmcm Posted at: 2017-07-13T16:41:09.864Z Reads: 41

```
@chaka, okay. The plate heatsink seemed pretty solidly attached when I tried to remove it after unscrewing everything, so I stopped before breaking something.

So I'll contact y'all through your website to get an RMA going?

Oh, and BTW, I asked for rush delivery before the July 4th weekend and y'all really came through. I didn't thank you then, so thank you for that!
```

---
## \#8 Posted by: chaka Posted at: 2017-07-13T16:44:11.307Z Reads: 42

```
This is good enough to get a return for repair/replace going, just be sure to add a few details in a note when you send it in.

Ollin Board Company 
PO Box 1340
Elephant Butte, NM 
87935
```

---
## \#9 Posted by: bmcm Posted at: 2017-07-13T16:45:42.148Z Reads: 41

```
Cool, thanks.
```

---
