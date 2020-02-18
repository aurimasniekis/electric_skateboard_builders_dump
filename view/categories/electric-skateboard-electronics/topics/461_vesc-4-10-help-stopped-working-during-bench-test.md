# VESC 4.10 Help stopped working during bench test

### Replies: 24 Views: 2985

## \#1 Posted by: korryh Posted at: 2015-11-13T00:28:00.685Z Reads: 92

```
Decided to change out my 6s, hobbywing esc, Life system with the VESC and SpaceCell.  Just received the new VESC 10.4 and Plugged in the battery, nunchuck and computer, started detection (per instructions) and it spun up. I filled in the info per the instructions then changed some of the motor settings optomized for the spacecell.  I made the nunchuck settings and the little motor wasn't spinning.  I know the nunchuk worked as I saw the display bar go up and down when I throttled.  I made sure the current was checked, rebooted and connected again.  The display bar does a little dance between 50 and 51 but still goes up and down with the joystick.  I went back to the motor settings again and tried detection - the motor just makes a high pitched sound and jitters a bit.  I am now at this and I am sure it is something simple.  I looked and several forums, google searches and messed around with the settings but nothing helped.  I even went back to the original settings but nothing worked.  I have an NTM 5060 motor, plan is to upgrade this as well but need to get the new system working first. Here are some pics of the VESC in case it helps. Would appreciate anyone's help to get this badboy working - Thanks <img src="/uploads/db1493/original/1X/e77e321e3912233b0e62c90e75a2c2cbef9acea7.JPG" width="375" height="500">. 
 
<img src="/uploads/db1493/original/1X/04df727dafd27979eba474b32c7ea0e96096a6dd.JPG" width="666" height="500">
```

---
## \#2 Posted by: onloop Posted at: 2015-11-13T00:42:40.073Z Reads: 82

```
Do you have any other motors to test? Last time something like this happen to me was due to a bad solder joint on the motors wires.... took me ages to work it out.
```

---
## \#3 Posted by: korryh Posted at: 2015-11-13T00:58:23.798Z Reads: 83

```
Unfortunately, I dont have any other motors.  The motor was working with my old system, I just plugged in the VESC today.  I will check the solder connections though - thanks.
```

---
## \#4 Posted by: korryh Posted at: 2015-11-14T00:23:20.469Z Reads: 78

```
Tried soldering the motor connections again and still the same thing.  I just get the high frequency noise with the jitters.  I checked the temp and it peaks out about 27. not sure what else to check since I know next to nothing other than what is in the instructions. I turned off the app config to rule out the nunchuck and still the same thing. Please helpl
```

---
## \#5 Posted by: korryh Posted at: 2015-11-14T22:16:47.985Z Reads: 74

```
Chaka on ES pointed out that there looks like there is a solder bridge on theDRV. It looks like there are 2 solder bridges after looking at it again. If I try to fix it with solder wick is it going to void any warranty or would you rather me send it back to you.  Thought I would ask before I tried anything.
```

---
## \#6 Posted by: lowGuido Posted at: 2015-11-14T22:19:33.438Z Reads: 71

```
I have been told in the other thread that those 2 solder bridges are supposed to be there.
mine has the same.
```

---
## \#7 Posted by: chaka Posted at: 2015-11-14T22:38:35.135Z Reads: 68

```
Those two bridges on the side next to the fets should be there. Nothing wrong with those. The bridge I mentioned looks hair thin. On the opposite row.

<img src="/uploads/db1493/original/1X/1fce3880049c06df4c3edf7939ad2154df89f6d7.png" width="666" height="500">
```

---
## \#8 Posted by: korryh Posted at: 2015-11-14T23:44:06.865Z Reads: 63

```
Thanks guys, glad the kids had gymnastics or I would have made more work for myself. I'll check the other side. Thanks again.
```

---
## \#9 Posted by: tomtnt Posted at: 2015-11-15T06:28:28.326Z Reads: 65

```
Weird, your nunchuck red/black looks reverse?  1st pin = 5v (unused), 2nd pin = 3.3v, 3rd pin = ground
```

---
## \#10 Posted by: korryh Posted at: 2015-11-15T08:45:17.988Z Reads: 62

```
Yes, the wires are reversed but the pin connections are correct. I bought the jst off the internet and didn't feel like switching the colors. Good eye.
```

---
## \#11 Posted by: jacobbloy Posted at: 2015-11-15T09:01:57.479Z Reads: 63

```
Jump into real time data  and check for an error, do motor detection again and see if it spins again. Reflashing firmware to default the make sure you click read data on both motor and app tab then again do motor detection. If you do r read data correctly you will miss data fields and it won't work.
```

---
## \#12 Posted by: onloop Posted at: 2015-11-16T02:36:46.998Z Reads: 61

```
how are you going with this?

If the motor still doesn’t spin up properly, Adjust “Current” and “Min ERPM” until it does. In general, small motors should have lower current and higher ERPM and larger motors the other way around. Current usually is in the range 1A to 6A and min ERPM usually is in the range 300 to 1200.
If spinning up works but running slowly afterwards doesn’t (the motor just stutters), try increasing “Low duty” to 0.1 or so. Increasing low duty will make it easier for the motor to run slowly during the test, but the result will become less accurate.
```

---
## \#13 Posted by: korryh Posted at: 2015-11-16T09:03:31.951Z Reads: 58

```
Thank you jacobbloy. Can you let me know where I can get the firmware to flash.
```

---
## \#14 Posted by: korryh Posted at: 2015-11-16T09:05:00.024Z Reads: 56

```
Hi onloop

Still doing the same thing- justjittering.
```

---
## \#15 Posted by: jacobbloy Posted at: 2015-11-16T10:48:28.511Z Reads: 55

```
have you tried to refresh the firmware?

https://drive.google.com/folderview?id=0Bym9XrdeViekfkRETmRndENkcVpySW5sWjIzOWdrLThCY01HY3BPOXpqYVRHUlQxS0R5ZlU&usp=sharing

FW and mc config folder

if you have a drv that should show in real time data, also if the motor was working before and not know have you modified any thing at all? in-between did you plug in the nunchuck incorrectly?
```

---
## \#16 Posted by: korryh Posted at: 2015-11-16T17:42:52.308Z Reads: 56

```
Just reflashed the default and IT WORKED!!!  wooohooo.

THANK YOU!!! 

Ill let you know how the rest of the set up goes. unfortunately I have to get back to work.
```

---
## \#17 Posted by: korryh Posted at: 2015-11-16T17:45:02.698Z Reads: 54

```
I also wanted to thank everyone else who chimed in to help - this community ROCKS.
```

---
## \#18 Posted by: emotiva Posted at: 2015-11-17T04:28:22.750Z Reads: 61

```
Similar issues here, but with the r-spec motor (Spacecell, VESC 4.10, FW 1.14). I've attempted troubleshooting from this thread and [here][1], but no luck so far. I'm able to connect to VESC, and turning the motor by hand is seen in the realtime data. "Start Detection" yields "Bad Detection Result" and no movement of the motor occurs. No faults are reported during this time and no red LED activity on VESC.

The other 3 issues that might help in diagnosing: 1) the Rotor Position reading in bldc tool is just noise, 2) the motor current is reported as non-zero most of the time even when I'm not trying to "detect motor". I'm talking on the order of an amp, which I'm thinking might indicate a short in the motor windings or a problem on the board. Also, 3) I see no mapping of my GTB2 to the ppm input (I have attempted motor detection with the ppm disabled as well), but that's probably unrelated. 

I have reloaded the firmware, making sure to "Read configuration" before loading the XML that - a) shipped with the VESC, b) the default file that Jason posted around here somewhere, and c) the one that Jacob provides for the r-spec in the mc_config folder for FW1.14. - and writing configuration. 

I don't have my DMM with me at home, but can troubleshoot with that tomorrow, perhaps. 
Any ideas?

  [1]: http://www.electric-skateboard.builders/t/vesc-blew-up-any-ideas-edit-solved/201
```

---
## \#19 Posted by: chaka Posted at: 2015-11-17T15:39:20.050Z Reads: 58

```
Might be a bad drv chip. I never let a VESC ship if it wont run detection on a motor and sometimes everything will load and connect but will fail detection without any fault codes. Replacing the drv solved the problem when I have encountered this. Adjusting the temperature profile of my re-flow oven has kept it happening again.
```

---
## \#20 Posted by: korryh Posted at: 2015-11-17T17:17:04.168Z Reads: 57

```
Not sure if this is going to help but here is the story - I tested my VESC for the first time at home and all I was getting was the jittering and high frequency noise.  I took it to work the next day and downloaded the bldc tool.  I dont remember downloading the .exe in the bldc-tool-windows-drivers folder at home but I did run at work.  I found the right port, re flashed the firmware with the "default" .bin in the mc_config_&FW / firmware 1.14, hit the "read configuration" in motor and sensor tabs then start detection and it spun up.

I ended up turning off the app configuration to rule out the nunchuck settings. and reconfigured when it spun up and changed numbers from detection results. Good Luck
```

---
## \#21 Posted by: korryh Posted at: 2015-11-17T17:18:24.713Z Reads: 54

```
Forgot to add that I received a bunch of help from many fine folks on this forum and ES while trouble shooting.
```

---
## \#22 Posted by: emotiva Posted at: 2015-11-18T02:10:48.248Z Reads: 51

```
Thanks. Yeah, I have tried reinstalling that firmware, but it doesn't seem to fix the problem in my case. Will update with any resolution.
```

---
## \#23 Posted by: emotiva Posted at: 2015-11-18T07:39:59.250Z Reads: 51

```
Missed your reply, previously. Hmm. Good to know. Nothing I can do to test if this is my issue?
```

---
## \#24 Posted by: emotiva Posted at: 2015-11-18T10:13:20.757Z Reads: 51

```
Never mind. Dropped a wire while troubleshooting and shorted the caps to the board. Definitely dead now. At least I have one coming tomorrow from chaka, himself, so not dead in the water for weeks. I had just previously gotten comms established with the Nyko and was able to see throttle input from that in bldc tool. Still not sure why I couldn't see the GT2B input before.
```

---
