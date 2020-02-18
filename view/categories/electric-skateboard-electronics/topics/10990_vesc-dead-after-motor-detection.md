# Vesc dead after motor detection

### Replies: 26 Views: 2115

## \#1 Posted by: Ultimat3ging3r Posted at: 2016-10-11T23:35:02.583Z Reads: 135

```
@onloop doing as described. 
Hooked up my vesc that I finally received today and plugged up the USB connected the motor turned it on. Read configuration worked. Went to do motor detection the motor jerked then said detection failed and began to flash pink and blue. Checked for fault and received a DRV8302 fault. From what I see that means a chip is bad and has to be replaced? 
Powered down checked all connections and all where connected. 
Tried my desktop-no joy
Uninstalled and reinstalled- blinked a little different but then went back to the same thing. 
Different cable, power supply, checked settings - no joy
Don't have another motor or controller. 

Not sure where to go from here.
```

---
## \#2 Posted by: Blasto Posted at: 2016-10-11T23:49:19.366Z Reads: 131

```
Post some pics of your setup and your settings in the bldc tool
```

---
## \#3 Posted by: Ultimat3ging3r Posted at: 2016-10-11T23:54:23.669Z Reads: 130

```
<img src="/uploads/db1493/original/3X/f/a/fa8e3e23be9fd307c4cb2635f3fc700f370fd255.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/c/2c678b2f605cc51c7c451e74e8aa9db59570159a.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/8/283fe583d677f4719963f4fb466b816b862b93e1.JPG" width="666" height="499">
```

---
## \#4 Posted by: Goombaacez84 Posted at: 2016-10-11T23:55:13.324Z Reads: 122

```
What kind of power source are you using?
```

---
## \#5 Posted by: Ultimat3ging3r Posted at: 2016-10-11T23:57:16.189Z Reads: 123

```
two 4s batteries in series so 8s zippy 30c.
```

---
## \#6 Posted by: Goombaacez84 Posted at: 2016-10-12T00:21:54.994Z Reads: 122

```
The only thing I can think of is that whole topic of using low voltage for the first boot-up as suggested by Chaka here:

http://www.electric-skateboard.builders/t/vesc-faq-when-to-use-low-voltage-vesc-configuration/1965

I don't think I've read of anyone that's actually fried a non-Ollin VESC from not using low voltage though. Perhaps someone who has a better eye for those short-prone spots on the PCB might be able to point out an area that shorted when you tried to spin up the motor. This thread sounds similar:

http://www.electric-skateboard.builders/t/vesc-shorting-on-first-try/10411/8
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-10-12T00:25:37.946Z Reads: 120

```
Put the max voltage to 57v and try again
```

---
## \#8 Posted by: Ultimat3ging3r Posted at: 2016-10-12T00:27:35.987Z Reads: 117

```
<img src="/uploads/db1493/original/3X/c/4/c4e3f6db26f9944c5cca3c7d58e460853ee31302.jpg" width="375" height="500">

I actually thought about and read that before and used my low volt to power up then connected my battery after. And as for popping on the xt60 connectors I have a 170 amp fuse I use to turn off all power so no worries there.
```

---
## \#9 Posted by: Blasto Posted at: 2016-10-12T00:33:29.300Z Reads: 117

```
[quote="JohnnyMeduse, post:7, topic:10990, full:true"]
Put the max voltage to 57v and try again
[/quote]

Do this, your max input is to low
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-10-12T00:36:19.038Z Reads: 113

```
Did you also change the original motor lead... Make sure you didn't brake any of the resistor or short the mosfet.
```

---
## \#11 Posted by: Ultimat3ging3r Posted at: 2016-10-12T00:37:08.445Z Reads: 109

```
no go ghost rider.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-10-12T00:37:56.828Z Reads: 110

```
Check your settings on these pages:
<img src="/uploads/db1493/original/3X/9/0/90cc6428eed97515ea743d7e942abf1fc85472ba.png" width="690" height="364">
<img src="/uploads/db1493/original/3X/1/7/1702b32f5a0189f886dbe1832570703c95d517c8.png" width="690" height="364">
```

---
## \#13 Posted by: Ultimat3ging3r Posted at: 2016-10-12T00:38:08.343Z Reads: 105

```
yes a soldered it straight to the board due to not having connectors.
```

---
## \#14 Posted by: Ultimat3ging3r Posted at: 2016-10-12T00:41:24.014Z Reads: 106

```
<img src="/uploads/db1493/original/3X/a/c/ac7d5a94753fd78d2536e2ddf600e58d12a1352e.JPG" width="666" height="499">[Uploading...]()
```

---
## \#15 Posted by: Ultimat3ging3r Posted at: 2016-10-12T00:42:14.156Z Reads: 101

```
but i couldn't even get an original motor detection so this is just what was on here.
```

---
## \#16 Posted by: Namasaki Posted at: 2016-10-12T00:46:27.563Z Reads: 99

```
Use cmd shift 4 for selective screen shot on mac
cmd shift 3 for full screen shot
```

---
## \#17 Posted by: Goombaacez84 Posted at: 2016-10-12T00:47:22.719Z Reads: 97

```
Perhaps a fresh 2.18 firmware update and then try again? I'm no VESC expert and am just throwing obvious ideas out :slight_smile:
```

---
## \#18 Posted by: Namasaki Posted at: 2016-10-12T00:49:08.900Z Reads: 98

```
Fresh firmware is a good idea.
Check your max current ramp step on the advance tab. it should be .04
```

---
## \#19 Posted by: Ultimat3ging3r Posted at: 2016-10-12T01:03:56.500Z Reads: 94

```
did it like 4 times.
```

---
## \#20 Posted by: Ultimat3ging3r Posted at: 2016-10-12T01:05:23.513Z Reads: 92

```
i did and it is.
```

---
## \#21 Posted by: Ultimat3ging3r Posted at: 2016-10-12T01:08:03.778Z Reads: 91

```
<img src="/uploads/db1493/original/3X/5/2/5251f100bf0eeee02b16594d581fa1f00daae428.png" width="690" height="431">
```

---
## \#22 Posted by: Namasaki Posted at: 2016-10-12T01:33:20.726Z Reads: 85

```
You might have a cold solder joint on one of the motor wires to the pcb.
Or, a bad connection where the motor wires are spliced,
If one of the motor wires is not connecting, the more will just jerk and not spin
```

---
## \#23 Posted by: Ultimat3ging3r Posted at: 2016-10-12T23:15:10.560Z Reads: 67

```
it doesn't even jerk after the first time.
```

---
## \#24 Posted by: psychotiller Posted at: 2016-10-12T23:30:30.955Z Reads: 61

```
If you saw the DRV fault code you may as well stop troubleshooting. Get a new chip and replace it or send the VESC back for replacement.
```

---
## \#25 Posted by: Ultimat3ging3r Posted at: 2016-10-15T00:00:36.332Z Reads: 48

```
i would love to but the three email I've sent to enertion have not been replied too.
```

---
## \#27 Posted by: JuniorPotato93 Posted at: 2016-10-15T00:26:20.454Z Reads: 48

```
@Ultimat3ging3r I did my set up with the only battery I had available to me which was a n 8S li-ion pack I had made and I had no issues.  I did use one of Chaka's VESCs so dont know if that makes a big difference in terms of getting it set up from an electrical standpoint. I know hes upgraded components.
```

---
