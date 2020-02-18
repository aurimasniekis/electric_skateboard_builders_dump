# FOCBOX not working

### Replies: 43 Views: 2195

## \#1 Posted by: fuzzyspikez Posted at: 2018-04-18T02:43:11.340Z Reads: 180

```
So last night I updated my FOBOX to the latest firmware and put it in FOC mode, following all the steps listed and adjusting all necessary values. I went on a short 5 minute ride today and it did fine, but when I came to connect it to my computer to tweak some of the settings it didn't recognize it and now the FOCBOX doesn't even work anymore, the light turn on, but even when the controller is connected, the motor does not spin. 

Anyone know how to fix it?
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-04-18T04:17:24.293Z Reads: 173

```
What motor kV at what voltage ?hmm open it up pretty sure you got the good old DVR error. Foc is usually try at your own risk.
```

---
## \#3 Posted by: fuzzyspikez Posted at: 2018-04-18T04:33:30.789Z Reads: 163

```
190kv at the time it was at like 35-36v on a 10s2p battery pack. What is that?
```

---
## \#4 Posted by: E1Allen Posted at: 2018-04-18T04:36:38.330Z Reads: 157

```
Likely not a DRV error.

Does it still connect to the computer?
```

---
## \#5 Posted by: fuzzyspikez Posted at: 2018-04-18T04:38:03.085Z Reads: 150

```
No, it connected for a second this afternoon after my ride, but no luck after that
```

---
## \#6 Posted by: E1Allen Posted at: 2018-04-18T04:39:46.427Z Reads: 150

```
What color are the lights on the focbox when you plug it in?
```

---
## \#7 Posted by: fuzzyspikez Posted at: 2018-04-18T04:40:50.196Z Reads: 151

```
they are Blue
```

---
## \#8 Posted by: E1Allen Posted at: 2018-04-18T04:41:47.382Z Reads: 144

```
That's a good start. Which FW did you upgrade to?
```

---
## \#9 Posted by: fuzzyspikez Posted at: 2018-04-18T04:45:44.667Z Reads: 143

```
I'm not completely sure since I cant hook it back up again, but it was the latest as I did it last night, and it was the FW that works with the new VESC tool software.
```

---
## \#10 Posted by: E1Allen Posted at: 2018-04-18T04:57:52.854Z Reads: 138

```
Well. You might have to wait for the vesc experts to wake up but someone will help you troubleshoot.  Beyond my vesc experience now.
```

---
## \#11 Posted by: Eboosted Posted at: 2018-04-18T05:02:13.074Z Reads: 133

```
Maybe one if the legs of your caps is broken, check on that
```

---
## \#12 Posted by: fuzzyspikez Posted at: 2018-04-18T05:03:44.350Z Reads: 130

```
haha thanks for trying man
```

---
## \#13 Posted by: fuzzyspikez Posted at: 2018-04-18T05:13:36.743Z Reads: 133

```
Where would that be?
```

---
## \#14 Posted by: E1Allen Posted at: 2018-04-18T05:30:44.552Z Reads: 138

```
![IMG_4817|281x500](upload://xQ9PKnlq8gjDXzcBYVVWWzmUzGv.PNG)

Where the colored circles are.  There are two metal posts coming off the caps and connect to the focbox.  Sometimes they come undone.
```

---
## \#15 Posted by: Eboosted Posted at: 2018-04-18T05:33:03.952Z Reads: 136

```
https://www.youtube.com/watch?v=_KvFTwoQVAc
```

---
## \#16 Posted by: CarlCollins Posted at: 2018-04-18T06:33:32.690Z Reads: 133

```
@fuzzyspikez
The firmware must be 3.1
all you need is a VESC tool and Windows or MAC PC (Windows is better)
After upgrading the digital signature for COM drivers got changed so you have uninstall the COM drivers and re-install virtual COM drivers.

After that Restart your system
Disconnect the motor from your system and power on your FOCBOX with USB connected to it.
It will identify it (hopefully)
Check the Values and adjust them accordingly 
Disconnect the FOCBOX and connect your complete setup

Then it will work

(Also FOC is not user friendly so please check any burn marks or weird smell from your FOCBOX's PCB)

I hope this helps
```

---
## \#17 Posted by: fraannk Posted at: 2018-04-18T06:40:19.699Z Reads: 138

```
So you recommend the @Ackmaniac ESC Tool firmware over the stock (new) VESC Tool firmware?
```

---
## \#18 Posted by: CarlCollins Posted at: 2018-04-18T06:41:05.300Z Reads: 134

```
Yeah Ackmaniac one is better
```

---
## \#19 Posted by: SeanHacker Posted at: 2018-04-18T07:48:38.786Z Reads: 130

```
FOC is not user friendly? How so? This is a FOCBox we're talking about right @CarlCollins? That's what this device is made for right?
```

---
## \#20 Posted by: SeanHacker Posted at: 2018-04-18T07:49:06.773Z Reads: 126

```
"Yeah Ackmaniac one is better"

It definitely is. :slight_smile:
```

---
## \#21 Posted by: CarlCollins Posted at: 2018-04-18T07:54:59.724Z Reads: 127

```
@SeanHacker
I am talking about FOC mode, User friendly means it's not plug and play.
You need to be careful while working in FOC specially with 12s setup.

And this device is made for controlling the motor that's why it is called FOCBOX Motor controller :slight_smile:
```

---
## \#22 Posted by: SeanHacker Posted at: 2018-04-18T07:59:39.863Z Reads: 125

```
BLDC is not plug and play either. The vesc needs to be setup while either using FOC or BLDC. it makes no difference. You need to run a motor detection for both as well as settings for the type of battery. Not sure I see what you're saying here?

 It was called the vesc-x before. I don't care what you guys call it. ;)
```

---
## \#23 Posted by: CarlCollins Posted at: 2018-04-18T08:07:58.843Z Reads: 123

```
@SeanHacker
Don't want to argue with you further because there is no use.
BLDC comes pre-programmed with the controller, very slight changes are required to operate any setup.
But for FOC, the case is difference as per my personal experience. :slight_smile:
```

---
## \#24 Posted by: SeanHacker Posted at: 2018-04-18T08:37:47.549Z Reads: 122

```
Huh? BLDC comes preprogrammed to what? Every motor and battery setup is different. That's sounds like a setup for disaster dude. Good luck with that advice.
```

---
## \#25 Posted by: DeathCookies Posted at: 2018-04-18T08:45:50.300Z Reads: 118

```
Initially every FOCBOX is set to BLDC. You have still to make a Motor detection. What actually means is that you do not have to click on BLDC because it is presetted. One click less and if you count the write button then two :D
PS: the focbox detection Needs more steps to make a Motor detection (unless the r2 Firmware)
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2018-04-18T12:46:46.041Z Reads: 109

```
That issue as been resolve 2year ago :wink: since the Alpha phase
```

---
## \#27 Posted by: JohnnyMeduse Posted at: 2018-04-18T12:51:13.338Z Reads: 112

```
OK I'm late to the party.... 

@fuzzyspikez Can you post some picture of your setup, and put more detail, like are you runing sensor or not, type of motor, are you using some inter-connector?
```

---
## \#28 Posted by: L3chef Posted at: 2018-04-18T12:56:13.945Z Reads: 109

```
[quote="CarlCollins, post:18, topic:52611, full:true"]
Yeah Ackmaniac one is better
[/quote]

Won't I lose my warranty on focboxes if I flash ackmaniacs firmware?
```

---
## \#29 Posted by: fuzzyspikez Posted at: 2018-04-18T13:52:17.925Z Reads: 104

```
Sure, I am using a 10s2p battery on a loaded vanguard deck. Single motor sensorless setup. 
![image|374x500](upload://8gCDp7w0Xs6YuxJdYbAZ5KCHjqi.jpeg)
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2018-04-18T15:14:56.209Z Reads: 99

```
I think I might be misunderstood, can you put more info, like screenshots of your parameter (don’t forget to press read before posting them), and picture of your connection. It will be much more efficient of we have access to the most info on your board, because we weren’t there to help you build it and every build have their particularities.
```

---
## \#31 Posted by: fuzzyspikez Posted at: 2018-04-18T15:46:52.384Z Reads: 93

```
that's the problem lol, I cant get it to connect to the VESC tool on my computer.
```

---
## \#32 Posted by: fuzzyspikez Posted at: 2018-04-18T15:47:39.854Z Reads: 91

```
How do I uninstall the COM drives?
```

---
## \#33 Posted by: Bjork3n Posted at: 2018-04-18T16:12:12.692Z Reads: 93

```
Off topic
You need to check your motor mount, it looks crooked?
```

---
## \#34 Posted by: fuzzyspikez Posted at: 2018-04-18T17:34:32.244Z Reads: 92

```
Yeah lol it was, I fixed it already
```

---
## \#35 Posted by: CarlCollins Posted at: 2018-04-19T04:03:16.960Z Reads: 86

```
@L3chef
Flashing firmware other than Enertion one is not recommended
If during flashing process device stopped working then it will not cover under warranty.
```

---
## \#36 Posted by: CarlCollins Posted at: 2018-04-19T04:04:55.967Z Reads: 86

```
@fuzzyspikez

Go to device manager
under COMs & Ports you will see one or two COM port 
right click on it and select Uninstall
Check mark "remove the driver software from the PC"
And Select Ok
```

---
## \#37 Posted by: fuzzyspikez Posted at: 2018-04-19T04:16:41.888Z Reads: 84

```
Is this for BLDC tool, or VESC tool?
```

---
## \#38 Posted by: CarlCollins Posted at: 2018-04-19T04:27:42.712Z Reads: 86

```
This is for both
```

---
## \#39 Posted by: fuzzyspikez Posted at: 2018-04-19T04:29:43.600Z Reads: 86

```
Ok, so you think that should take care of it?
```

---
## \#40 Posted by: CarlCollins Posted at: 2018-04-19T04:31:24.667Z Reads: 85

```
@fuzzyspikez
 I hope so
```

---
## \#41 Posted by: fuzzyspikez Posted at: 2018-04-20T05:08:26.471Z Reads: 80

```
I’m a little confused, what do I click?
![image|374x500](upload://c9jBhu2JSgu1ghkwpvoehet3nus.jpg)
```

---
## \#42 Posted by: fuzzyspikez Posted at: 2018-04-21T05:24:44.289Z Reads: 71

```
I opened it up, doesn't look like any mechanical issues, everything is intact, could reflash the firmware work? If so how can I do that?
```

---
## \#43 Posted by: Scoo_B_SK8 Posted at: 2018-04-21T06:01:04.250Z Reads: 67

```
here's a couple reads that might help???

https://www.electric-skateboard.builders/t/how-to-programm-flash-a-new-born-vesc-4-12-with-st-link-v2-widows-10/52813?source_topic_id=52997

https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103?source_topic_id=52813&source_topic_id=52997
```

---
