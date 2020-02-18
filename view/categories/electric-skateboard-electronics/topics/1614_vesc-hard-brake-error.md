# VESC - Hard Brake error

### Replies: 28 Views: 3007

## \#1 Posted by: CyrusArdain Posted at: 2016-03-01T12:50:09.450Z Reads: 217

```
Hello everyone.  I have been lurking here for a while but cant seems to find anything fully related to my problem.

Setup:
 - Space Cell
 - 2 R-spec Motors
 - 2 VESC (Updated to 2.15)

I have tweaked all the settings to the VESC per data from this forum.  Currently running in CANBUS.  PPM mode, current no reverse with brake

Problem:
When I go from full throttle to full hard brake, the motors will cut out and only the (slave) VESC will have a blinking red light.  If I wait a few seconds for everything to settle, I can throttle again with no issue.  Slow braking does not cause an issue.

What can I do to stop this?
```

---
## \#2 Posted by: onloop Posted at: 2016-03-01T13:11:55.295Z Reads: 216

```
what regen settings do you have>?

for battery & also motors?
```

---
## \#3 Posted by: CyrusArdain Posted at: 2016-03-01T13:15:55.663Z Reads: 212

```
I am following this link

http://www.electric-skateboard.builders/t/vesc-faq-optimized-s-p-a-c-e-cell-settings/414

For each VESC:
Motor Max: 80A
Motor min (regen): -60A
Batt Max: 15A
Batt Min (regen): -12A
```

---
## \#4 Posted by: onloop Posted at: 2016-03-01T13:54:20.543Z Reads: 193

```
try lowering the settings

Motor Max: 60A (or 40A)
Motor Min (regen): -20
```

---
## \#5 Posted by: CyrusArdain Posted at: 2016-03-01T23:14:30.572Z Reads: 174

```
eh. not working.  now it seems to cause so intermittant issues with throttling back up.  starts cogging (i think is the term) when throttling back up.
```

---
## \#6 Posted by: CyrusArdain Posted at: 2016-03-01T23:24:29.048Z Reads: 172

```
disabled CANBUS and I dont have the problem with single motor/vesc settings.  guessing i am tripping some current limit...
```

---
## \#7 Posted by: onloop Posted at: 2016-03-02T03:47:56.686Z Reads: 171

```
Did you run the motor detection after updating firmware?
```

---
## \#8 Posted by: zpoole27 Posted at: 2016-11-03T20:17:00.196Z Reads: 118

```
old thread i know...

im having the same issue, did you ever find a solution?
```

---
## \#9 Posted by: Ackmaniac Posted at: 2016-11-04T09:31:14.159Z Reads: 104

```
Post Screenshots of your general motor and advance motor settings.
```

---
## \#10 Posted by: ekitesurfer Posted at: 2016-11-15T05:39:54.573Z Reads: 104

```
I am having this issue with dual carvon's/ space cell 4... Settings are as follows:

motor max: 30a
Motor min: -30
bat max: 20a
batt min: -8a
abs max: 65a

I have one board with these settings and 97mm wheels that works fine, this board has 90mm wheels. Anyone think the wheel size could make a difference? Anyone have any suggestions?
```

---
## \#11 Posted by: Blasto Posted at: 2016-11-15T06:25:46.526Z Reads: 94

```
Raise your absolute max current to 120-130A
```

---
## \#12 Posted by: ekitesurfer Posted at: 2016-11-15T06:27:10.765Z Reads: 95

```
These are settings for a dual vesc...
```

---
## \#13 Posted by: Blasto Posted at: 2016-11-15T06:31:44.441Z Reads: 94

```
Ok, raise your absolute current max on each vesc to 120-130A.

If you have this value to low the vesc will shutdown on a current spike and risk street your face
```

---
## \#14 Posted by: ekitesurfer Posted at: 2016-11-15T06:36:38.272Z Reads: 94

```
Oh, ok, I thought all the numbers where supposed to be divided in half?
```

---
## \#15 Posted by: Blasto Posted at: 2016-11-15T06:57:29.318Z Reads: 95

```
Not the absolute max, it's a safety mechanism for the vesc and it's sensitive to current spikes (will shutdown the vesc once it hits that value)

But if you are having a shutdown issue apon braking, is your max input voltage set at 57V?
```

---
## \#16 Posted by: ekitesurfer Posted at: 2016-11-15T06:59:52.157Z Reads: 88

```
57v yep..

I wonder if the smaller wheels generate more amps? The 97mm board has the same settings and does not have the hard brake error...
```

---
## \#17 Posted by: chinzw Posted at: 2016-11-15T07:13:58.146Z Reads: 85

```
Are you using FOC or BLDC?
```

---
## \#18 Posted by: Jinra Posted at: 2016-11-15T07:18:36.392Z Reads: 87

```
I thought I already mentioned that they should be higher :stuck_out_tongue: Did you check for faults like I mentioned?
```

---
## \#19 Posted by: ekitesurfer Posted at: 2016-11-15T07:28:30.985Z Reads: 85

```
I am using FOC... Does anyone really use BLDC???  Can't really check for faults because the vesc's only cut out for a second, they are fine by the time I get home..
```

---
## \#20 Posted by: Jinra Posted at: 2016-11-15T07:30:19.363Z Reads: 85

```
I'd say most people use BLDC, myself included. I'll never use FOC until the VESC 6 as I'm not comfortable risking a $170 speed controller and potentially my life since I live in a place with a lot of hills.

Why can't you check for faults? When they cut out they might be generating a fault. Just go home, plug it in, check for faults in BLDC tool. Just make sure you don't turn it off in the time between.
```

---
## \#21 Posted by: chinzw Posted at: 2016-11-15T07:33:19.853Z Reads: 82

```
Hmm, im pretty sure most of us use BLDC. Braking and FOC is very VERY hit and miss. If you have long lead wires from your battery to the VESC you will have problems. As for faults, they don't go away until you shut down the VESC, so as long as you keep it on, all the faults are still there for you to check.
```

---
## \#22 Posted by: ekitesurfer Posted at: 2016-11-15T07:41:19.557Z Reads: 80

```
Interesting... With how nice FOC is, I just figured everybody was using it... I have a lot of hills around my place also, the warranties should cover any monetary risk and as a rule of thumb I try to not go faster than I am willing to jump off the board and hit the ground running. I can't check for faults because as soon as it cuts out, it comes back...
```

---
## \#23 Posted by: Jinra Posted at: 2016-11-15T07:44:39.540Z Reads: 76

```
The VESC will still record the fault. If you go to the terminal tab and type "faults" it'll list every fault it's run into since startup.
```

---
## \#24 Posted by: ekitesurfer Posted at: 2016-11-15T07:46:08.335Z Reads: 73

```
ah, cool. Good to know! I have got to be getting the over current error...
```

---
## \#25 Posted by: chinzw Posted at: 2016-11-15T07:47:24.369Z Reads: 71

```
When it cuts out and comes back, if there's a fault, it will get stored in memory, and it wont go away until you power of the vesc. When i was trying FOC, anything lower than -20 motor min would make it cut off, and i would get a DRV8302 fault registered, which i could see when i plugged to the computer.

Is the length of your wires more than 20cm (8") if so, that would be a posible cause for your problems.
```

---
## \#26 Posted by: ekitesurfer Posted at: 2016-11-15T07:51:48.912Z Reads: 71

```
The wires are the standard length that came with carvons and diy vescs...
```

---
## \#27 Posted by: chinzw Posted at: 2016-11-15T07:53:21.624Z Reads: 69

```
Im talking about the wires from your battery all the way to the vesc, counting any switches, etc you might have in between.
```

---
## \#28 Posted by: ekitesurfer Posted at: 2016-11-15T07:55:30.620Z Reads: 70

```
Changing the abs max to 120a on each vesc seemed to fix it. Thanks guys!
```

---
