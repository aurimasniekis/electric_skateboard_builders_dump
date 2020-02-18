# Vesc Bad Motor Detection/0 Faults/Motor&amp;Solder Joints Ok/FW 2.18 Vesc 4.12 PLEASE HELP!

### Replies: 52 Views: 1721

## \#1 Posted by: GhettoFab.rictation Posted at: 2017-12-23T02:40:25.169Z Reads: 114

```
Alright ladies and gentlemen! My vesc blinks green during motor detection once in the beginning and once in the end. The green lights stay solid when sending signal during bench test as it should. The motor was tested on another esc opto using the vesc signal power as a bec and receiver signal came from the opto esc. Motor responded as should and runs great. I have turnigy sk3 192kv with two 6s 5000mah samsung 25r (green not cyan) cells running in series to 12s (I've run the vesc with half power and then full power with no results) with @eLDoska 40amp 2mosfet switch also with drok step down converter to 3amp 36watt 12v for my leds also my vesc has 2.18 Firmware and is a 4.12 )I purchased vesc a year ago). I am able to write configurations, but at first it took 2 configuration writes for the vesc to hold the configurations. After reboot now it rewrites fine. The cord I'm using is dinky and I'm thinking that may be the issue, but if that was the case would the vesc even connect to bldc tool and then be able to write configurations?? Another issue I can think of is downloading the incorrect bldc tool as mine now looks different from my older 2.16 firmware version (as I expected, but now learning all over again). This is making it more difficult for me to understand as I'm least experienced in the area of programming these computers. The settings are basically set as the stock configuration the vesc was able to read aside from a few changes I made. The failed motor detection with no fault was before and after the configuration writes. Also the controller worked with the esc and there is no signal received on vesc, signal is received on bench test, but motor won't turn. Can someone please help with installing the correct 2.18 bldc tool to rule it out and I will try to get my hands on my nice old gold tip usb cable I have buried somewhere around the house to rule that out as well. Any ides guys and gals?!?! Any help is much appreciated, but PLEASE stay on topic :wink:
<img src="/uploads/db1493/original/3X/0/5/05548766df03b0f1c114a27386fa1c427f4f809a.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/c/7/c7420ec7760458dc9513e18930abe010ebb5622e.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/d/b/dbc3e7584db562574ac28a3119097a3c14d8b263.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/f/a/fa9f6e8dbb441ed398c9363362c11001cd2f7a82.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/4/f/4f2adf5b388ad7b2c9204f68fcf6e72427645fcf.jpg" width="281" height="500">
```

---
## \#2 Posted by: scepterr Posted at: 2017-12-23T03:00:07.590Z Reads: 97

```
Pics of bldc tool settings please
```

---
## \#3 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:26:12.164Z Reads: 96

```
These are the green lights of bench test. Now no signal received to vesc from receiver. <img src="/uploads/db1493/original/3X/b/c/bc60982a71c196aba85c3d38bcafc9e9027f8013.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/6/a/6aa159471d4cbd2377b1882859729f3ed50b8032.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/a/4/a4f57fe3a743c3353b4c06ab4c0b786ade2b00c9.jpg" width="690" height="388">  <img src="/uploads/db1493/original/3X/3/c/3c31f6e0d063a82950aa0e1ad8df14663b4e7df0.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/c/1/c1b625157ee3df10e2f46ae5e929835e38c5f77d.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/3/9/390ff0a696749fda9f501298ca0778ffff96ecaf.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/4/1/415e248f97937b0430afe665753e53c4ee22c53b.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/d/2/d2366edf615a4d772a95ce489583f5b10f2c8183.jpg" width="690" height="388">  <img src="/uploads/db1493/original/3X/5/8/586dfa77614bd73788ce27dbeaa8559f23dc2e7f.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/2/3/23bd0eb862550e239630e52cf818fca77f661599.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/2/d/2d16a129705d8418af04121eb798f9256958f8c9.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/b/2/b29e993aa38d1c029b8708156295dd1f0463dd49.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/6/d/6d10ba99b253f37580bffe943cad754be63b257b.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/2/6/2606ceed85dd55760f59164726de87efecdde2a8.jpg" width="690" height="388">
```

---
## \#4 Posted by: scepterr Posted at: 2017-12-23T03:32:15.608Z Reads: 81

```
So then the problem is you cant do motor detection?
```

---
## \#5 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:35:36.759Z Reads: 80

```
Yes and bench test doesn't turn my motor and my receiver doesn't send any signals to vesc. Tested motor and receiver/controller on another esc and they work. I feel like I may need to download a different bldc tool. If I'm connected and writing configurations that means it's not the tool right?
```

---
## \#6 Posted by: scepterr Posted at: 2017-12-23T03:36:27.205Z Reads: 81

```
Ok forget about everything but the motor detection right now. What happens when you do motor detection?

Unless you want to fry your vesc don't try to "use" it before it's setup properly
```

---
## \#7 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:39:53.987Z Reads: 78

```
It shows those last two pictures, bad motor detection, then when I type in faults it states no faults registered since startup
```

---
## \#8 Posted by: scepterr Posted at: 2017-12-23T03:40:29.803Z Reads: 74

```
Ok, what happens when you run the test, does the motor move at all, make a sound?
```

---
## \#9 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:41:42.274Z Reads: 71

```
No nothing at all :frowning:
```

---
## \#10 Posted by: scepterr Posted at: 2017-12-23T03:42:17.497Z Reads: 71

```
Ok, increase Current A to 8 in the little window and try again
```

---
## \#11 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:43:21.775Z Reads: 69

```
Bad results received again, detection failed
```

---
## \#12 Posted by: scepterr Posted at: 2017-12-23T03:44:03.055Z Reads: 70

```
No sound or shake,movement from motor?
```

---
## \#13 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:46:17.353Z Reads: 76

```
No, no nothing :cry:. The motor was tested good and solder connections and wires from vesc tested good. Nothing though not a peep
```

---
## \#14 Posted by: scepterr Posted at: 2017-12-23T03:46:47.318Z Reads: 76

```
Bump min rpm try again

Oh and go to the FOC tab, and run hall detection there, see if that works
```

---
## \#15 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:47:38.366Z Reads: 75

```
To what 300?
```

---
## \#16 Posted by: scepterr Posted at: 2017-12-23T03:48:06.023Z Reads: 71

```
Yeah 300 is fine
```

---
## \#17 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:50:51.539Z Reads: 74

```
All didn't work <img src="/uploads/db1493/original/3X/f/2/f2d9f6fc6a3a2d736fedeb51f708fb583e237f7a.jpg" width="690" height="388">
```

---
## \#18 Posted by: scepterr Posted at: 2017-12-23T03:52:57.366Z Reads: 73

```
Hmm I dunno , I would upgrade it to 2.54, ackmaniacs fw, might just be something buggy with it if there's no hardware issues
```

---
## \#19 Posted by: GhettoFab.rictation Posted at: 2017-12-23T03:54:05.853Z Reads: 72

```
ok I'll give that a shot, how do I do that? I kind of think I remember how
```

---
## \#20 Posted by: scepterr Posted at: 2017-12-23T03:56:44.709Z Reads: 74

```
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#21 Posted by: GhettoFab.rictation Posted at: 2017-12-23T04:11:41.236Z Reads: 64

```
he statees you need ubuntu, can I use this with windows??
```

---
## \#22 Posted by: scepterr Posted at: 2017-12-23T04:12:26.717Z Reads: 66

```
Yes there's a windows version right there
```

---
## \#23 Posted by: GhettoFab.rictation Posted at: 2017-12-23T04:14:44.335Z Reads: 66

```
thank you forthe help! I will post on what happens!
```

---
## \#24 Posted by: GhettoFab.rictation Posted at: 2017-12-23T04:39:41.277Z Reads: 67

```
unknown error in bottom left hand corner where it always says connected. In the beginning it stated it was connected,limited for fw update. After upload I try to connect and refresh the tool and it can't find the device.
The device "disconnects" from the computer. I hear the computer make the sound of a device leaving my computer after upload. After restarting the vesc and rebooting my tool it reads 2.18 fw again. :unamused:
```

---
## \#25 Posted by: GhettoFab.rictation Posted at: 2017-12-23T04:41:26.076Z Reads: 65

```
also after upload the green light goes away and it's just the blue light until I restart the vesc
```

---
## \#26 Posted by: scepterr Posted at: 2017-12-23T04:50:18.454Z Reads: 64

```
Hmm your vesc might be one of the old ones that didn't have a bootloader preinstalled

You could use Vesc-tool to install the 2.54 firmware and a bootloader
```

---
## \#27 Posted by: GhettoFab.rictation Posted at: 2017-12-23T04:56:06.534Z Reads: 60

```
That tool in the files? I'm sorry I don't quite know what tool you mean the ackamniac tool or another bldc tool? I deleted my other tools, but no biggie because had nothing saved haha. Can you help me with how to get the bootloader on my vesc?
```

---
## \#28 Posted by: scepterr Posted at: 2017-12-23T04:59:47.331Z Reads: 60

```
http://vesc-project.com/vesc_tool
```

---
## \#29 Posted by: GhettoFab.rictation Posted at: 2017-12-23T05:43:41.325Z Reads: 59

```
now I'm super confused because on ackmaniac's tool it stated I already had a bootloader on my vesc and now on this tool it's telling me if I have a bootloader and try to download another bootloader it will ruin the vesc and I can't upload fw anymore?
```

---
## \#30 Posted by: scepterr Posted at: 2017-12-23T05:45:49.989Z Reads: 59

```
Try flashing 2.54 firmware first then with vesc-tool
Bin file from ackmaniacs on vesc-tool
```

---
## \#31 Posted by: GhettoFab.rictation Posted at: 2017-12-23T06:20:04.581Z Reads: 58

```
ok so I flashed the bootloader on it at first because remember the 2.54 firmware wouldn't load before. It was successsful to update to the 2.54!!! But now I'm still having issues with motor detection :neutral_face: so I'm getting closer, but not quite there yet haha
```

---
## \#32 Posted by: GhettoFab.rictation Posted at: 2017-12-23T06:27:14.980Z Reads: 57

```
what do you mean bin?
```

---
## \#33 Posted by: scepterr Posted at: 2017-12-23T06:28:37.921Z Reads: 56

```
That was the firmware file but since you already flashed it doesn't matter lol

Still no motor movement or sound and no faults?
```

---
## \#34 Posted by: GhettoFab.rictation Posted at: 2017-12-23T06:34:56.197Z Reads: 56

```
oh haha :smile: well now to get my motor detection done! What tool is better the ackmaniac or vesc website one?
```

---
## \#35 Posted by: scepterr Posted at: 2017-12-23T06:35:42.738Z Reads: 56

```
You said it doesn't work still, which were you using, you can only use one with each specific version
```

---
## \#36 Posted by: GhettoFab.rictation Posted at: 2017-12-23T06:37:32.486Z Reads: 54

```
Ackmaniac's but still bad motor detection
```

---
## \#37 Posted by: scepterr Posted at: 2017-12-23T06:38:17.809Z Reads: 54

```
Still no sound,movement or faults during/after detection?

Can you post a pic of the real-time tab and make sure to activate sampling
```

---
## \#38 Posted by: GhettoFab.rictation Posted at: 2017-12-23T06:42:04.474Z Reads: 54

```
sure do you want me to press any of the arrow keys or just let the realtime data show by itself for certain amount of time?
```

---
## \#39 Posted by: GhettoFab.rictation Posted at: 2017-12-23T07:06:31.927Z Reads: 56

```
<img src="/uploads/db1493/original/3X/9/0/90471db4932204957797851f50e26a1695be9cb5.jpg" width="690" height="388">
```

---
## \#40 Posted by: GhettoFab.rictation Posted at: 2017-12-23T07:09:16.241Z Reads: 57

```
<img src="/uploads/db1493/original/3X/7/7/77e7151d9924e58c6000893e66f45c5eb06c86b0.jpg" width="690" height="388">
```

---
## \#41 Posted by: scepterr Posted at: 2017-12-23T07:10:19.689Z Reads: 54

```
Your battery voltage is below your cutoff start I believe
And yeah you're cutoff start is 36

Uhm are you running 6s or 12s? Cause that's VERY low for 12s
```

---
## \#42 Posted by: GhettoFab.rictation Posted at: 2017-12-23T07:13:12.932Z Reads: 53

```
Haha right now 6s (one battery) but my settings for v are in half. <img src="/uploads/db1493/original/3X/a/7/a79d2f6ca8363e1c5aac6ab9dddf6c1ff023a02e.jpg" width="690" height="388">
```

---
## \#43 Posted by: scepterr Posted at: 2017-12-23T07:14:05.824Z Reads: 50

```
Dude how about you give me accurate information for what you're doing so I don't waste my time, please
```

---
## \#44 Posted by: scepterr Posted at: 2017-12-23T07:15:23.748Z Reads: 47

```
Try increasing detection current to 10 A
As soon as you hit ok on start detection switch to real-time tab and watch what happens
```

---
## \#45 Posted by: GhettoFab.rictation Posted at: 2017-12-23T07:17:16.137Z Reads: 49

```
It is accurate I've been doing 12s all night tonight and I'm in my bed and took one to try and get this working does that make a big enough difference for that? Your help is appreciated mate not trying to be a piss ant, but I'd been working on this for hours and it's 1am so yeah if it's a big deal for the setup to run on 12s again I'll grab the other battery
```

---
## \#46 Posted by: scepterr Posted at: 2017-12-23T07:17:40.106Z Reads: 53

```
Lol well at lower voltage you need higher current 
And it's 2am here 😉

Changing a variable during troubleshooting without notification is a no-no, that's all 😋
```

---
## \#47 Posted by: scepterr Posted at: 2017-12-23T07:20:18.923Z Reads: 51

```
We can continue this tomorrow, better to start on a fresh head
```

---
## \#48 Posted by: ARetardedPillow Posted at: 2017-12-23T08:31:25.837Z Reads: 50

```
Try scraping off the maytech logo and see if it works
```

---
## \#49 Posted by: GhettoFab.rictation Posted at: 2017-12-23T16:50:55.953Z Reads: 44

```
I would have spent fifty dollars on repairing my ollin vesc had I known I'd run into this. But it's sad the ollin vesc broke in the first place. I guess last case scenario I'll have them both repaired for 100 bucks
```

---
## \#50 Posted by: GhettoFab.rictation Posted at: 2017-12-23T16:51:28.825Z Reads: 44

```
Thanks for the help @ARetardedPillow
```

---
## \#51 Posted by: GhettoFab.rictation Posted at: 2017-12-23T17:55:47.012Z Reads: 45

```
yeah I'm going to find different usb. Even going back to running 12s, same issues...
```

---
## \#52 Posted by: GhettoFab.rictation Posted at: 2017-12-24T01:01:40.315Z Reads: 40

```
I guess I'm sending them in for repairs
```

---
