# Wrong firmware flashed on Focbox

### Replies: 12 Views: 202

## \#1 Posted by: Eboosted Posted at: 2019-05-22T23:12:34.673Z Reads: 73

```
I accidentaly flashed a wrong firmware on my FocBox and, without noticing the mistake, I made FOC motor detection, there was magic smoke right after that and my DRV chip is tosted.

I wonder if someone had this happening before?, if an incorrect firmware could cause this to happen or if the error could come from a shorted motor.
```

---
## \#2 Posted by: Jinra Posted at: 2019-05-22T23:17:11.539Z Reads: 69

```
Yep, definitely from the wrong f/w. Installed f/w for hardware version 48 once and same thing happened during detection. Luckily there was a fuse that prevented the VESC from killing itself.
```

---
## \#3 Posted by: Eboosted Posted at: 2019-05-22T23:18:06.873Z Reads: 69

```
Thanks man!

I wonder why they put the 48 FW on top on the list, this happened to a ton of people.
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2019-05-22T23:43:30.877Z Reads: 59

```
This will forever be a mystery
```

---
## \#5 Posted by: xabdullahx Posted at: 2019-08-03T06:53:50.010Z Reads: 30

```
Sorry for reviving an old thread.
I have a raptor 2 and I connected the focbox to focbox unity ui and updated it.
Now I know that focbox and focbox unity are two completely different things (it's really confusing)

Anyway, I don't believe anything burnt, how do I return to the old firmware? Do I really need a programmer? Enertions bldc tool won't connect,(saying version too old) but focbox unity connects fine.
What is the hw version?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-08-03T08:03:35.337Z Reads: 24

```
[quote="xabdullahx, post:5, topic:94677"]
What is the hw version?
[/quote]

Hardware version.
```

---
## \#7 Posted by: xabdullahx Posted at: 2019-08-03T08:33:17.426Z Reads: 20

```
I meant what's the hardware version for the raptor 2 focbox?
```

---
## \#8 Posted by: banjaxxed Posted at: 2019-08-03T08:36:25.351Z Reads: 21

```
You need to get a STLINK usb programmer. If the boot loader no longer works, allowing you to reprogram the f/w, then this is the only way to access the h/w 

hacks asides
```

---
## \#9 Posted by: xabdullahx Posted at: 2019-08-03T08:41:02.085Z Reads: 22

```
[quote="banjaxxed, post:8, topic:94677"]
You need to get a STLINK usb programmer. If the boot loader no longer works, allowing you to reprogram the f/w, then this is the only way to access the h/w
[/quote]

I just realized i can connect with vesc tool by going to the connection tab instead of using the autoconnect.

It lets me connect in limited mode and lets me upload a firmware (supposedly)
![image|690x443](upload://dHlUhjcsz34xIvK8NEObeOtLSOR.png) 

i have firmware 2.18, found here: https://www.electric-skateboard.builders/t/where-can-i-find-the-vesc-2-18-firmware/23852, but theres hw_410_411_412, hw_46_47 and hw_48 folders. i tried flashing hw_410_411_412 VESC_enertion_6355.bin, but fw version is not changing

EDIT: Okay, so i removed the casing and it said v 4.12
```

---
## \#10 Posted by: banjaxxed Posted at: 2019-08-03T08:42:08.263Z Reads: 22

```
[quote="xabdullahx, post:5, topic:94677"]
I connected the focbox to focbox unity ui
[/quote]

If you are using the Unity s/w against an older model Focbox, you are doing it wrong.

I would first try using the vesc tool and see if you can connect & flash it with a stock f/w, then go from there.

Do not willy-nilly use and VESC-type software and randomly select a firmware to upload or you’ll hit this type of problem, it might be clear that lesson has already been learned.
```

---
## \#11 Posted by: xabdullahx Posted at: 2019-08-03T08:43:57.955Z Reads: 22

```
[quote="banjaxxed, post:10, topic:94677"]
clear that lesson has already been learned
[/quote]

How was i supposed to know that Focbox Unity UI is not for updating the box that said Focbox on it:stuck_out_tongue: 
But yes, lesson is learned
```

---
## \#12 Posted by: xabdullahx Posted at: 2019-08-03T09:16:30.339Z Reads: 22

```
Is the st-link for firmware also or only bootloader?

I am still not sure what to do, as you can see in above screenshot, it's detecting fw 23.44 on the focbox which is completely wrong. I upload a screenshot successfully but it's still detecting fw 23.44 when I power cycle
```

---
