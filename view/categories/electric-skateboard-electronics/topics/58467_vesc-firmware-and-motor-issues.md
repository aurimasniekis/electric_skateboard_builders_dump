# VESC firmware and motor issues

### Replies: 22 Views: 1156

## \#1 Posted by: mgertner Posted at: 2018-06-10T23:32:32.758Z Reads: 211

```
Alright so I have a big issue:

I bought a replacement VESC from tourque boards after my other one broke. And I received it a couple days ago. However, when i plugged it in to my BLDC Tool it says "The firmware on the connected VESC is too old. Please update it using a programmer." So i asked the support guys for help and they told me to download the VESC Tool software. So I did so and updated the firmware following the instructions:

blogs/diy-electric-skateboard-tutorials/how-to-update-vesc-firmware 

So I opened up the BLDC Tool and tried connecting it again and it still said the firmware was too old. So i tried it again to see if I did something wrong  the first time, but it failed again . Then I realized I could configure it using the VESC Tool. So I ran some detections and tried configuring the VESC and nothing happened. The resistance is like 25,000 ohms which is way too high. And the fault reads FAULT_CODE_DRV. Also, when I try pulling the trigger on the controlling, nothing happens either.

Now im starting to think that it is a faulty VESC and I should replace it, or if it really is a firmware issue.

I will leave screenshots of the VESC terminal and Debug console to show the Faults and the failed detections if that'll help at all. 


 ![12%20PM|690x453](upload://cEOal5EQBGeMj0oTfxqWlU3CPDX.png)![50%20PM|690x453](upload://eKkhIUejSAzTEp5ek3miG0FyZR2.png)![58%20PM|690x453](upload://sGxlH3H9p0Zc52XvplYVx0m6eAf.png)
![51%20PM|690x453](upload://qLdQFw1y0L66iK0sBPHX1k0KoDx.png)

Thanks!
```

---
## \#3 Posted by: CarlCollins Posted at: 2018-06-11T11:00:40.980Z Reads: 150

```
@mgertner

I think I got this, 
Just need to confirm which Windows version you were using?
```

---
## \#4 Posted by: mgertner Posted at: 2018-06-13T03:12:30.168Z Reads: 120

```
I’m using Mac OSX. I found download for the software for Mac.
```

---
## \#5 Posted by: CarlCollins Posted at: 2018-06-13T19:11:32.164Z Reads: 112

```
Have you tried again using Windows PC?
```

---
## \#6 Posted by: mgertner Posted at: 2018-06-13T22:10:29.165Z Reads: 102

```
Yeah so I originally used Bootcamp to run Windows on my Mac before I found the Mac version. The version on that was Windows 10.
```

---
## \#7 Posted by: CarlCollins Posted at: 2018-06-14T03:23:54.211Z Reads: 98

```
@mgertner

Now try using VESC tool to flash the FW of FOCBOX
```

---
## \#8 Posted by: mgertner Posted at: 2018-06-14T17:50:08.398Z Reads: 91

```
What do you mean by “flash the firmware”
```

---
## \#9 Posted by: Ebisane9 Posted at: 2018-06-14T18:14:57.719Z Reads: 87

```
upload new firmware = flash the firmware. 

Get that reading time up :) this might have been avoidable
```

---
## \#10 Posted by: mgertner Posted at: 2018-06-14T18:52:27.077Z Reads: 84

```
I can try uploading a new firmware but i already tried like 4 times. All with firmware 3.38, 412
```

---
## \#11 Posted by: Ebisane9 Posted at: 2018-06-14T19:44:18.593Z Reads: 82

```
might need to replace the drv then. also correct me if i'm wrong @Deckoz but if you run the foc detection all the boxes for foc should be highlighted green. I don't use foc on my tb vesc so I can't give advice on that. I run hybrid bldc and my whine is actually not too loud. *sensored*
```

---
## \#12 Posted by: Deckoz Posted at: 2018-06-14T20:42:20.380Z Reads: 79

```
Yes all should be green
```

---
## \#13 Posted by: mgertner Posted at: 2018-06-14T23:23:56.702Z Reads: 73

```
Yeah i was suspecting there was a faulty drv chip
```

---
## \#14 Posted by: CarlCollins Posted at: 2018-06-15T01:32:17.882Z Reads: 69

```
@mgertner
Then you have to get it to a DRV wizard for repair
```

---
## \#15 Posted by: mgertner Posted at: 2018-06-16T14:05:26.485Z Reads: 57

```
Do you know any?
```

---
## \#16 Posted by: Sebike Posted at: 2018-06-16T14:11:57.056Z Reads: 56

```
Depends on your location
```

---
## \#17 Posted by: mgertner Posted at: 2018-06-16T15:51:55.063Z Reads: 56

```
Oh so it's an actual person that you have to go to?
```

---
## \#18 Posted by: ryan.kareme Posted at: 2018-09-06T17:08:48.509Z Reads: 44

```
Hi All - 

I am having a somewhat similar issue and havent been able to find an answer in any of the forums I have checked already - hoping someone here has some troubleshooting options - Ill try to be brief:

- I initially built a single-motor board using mostly TB parts (motor, mount, VESC, etc.)
- Used that board for 6+ months with no issues and then decided to upgrade to dual motor setup (w @psychotiller Six Shooters :slight_smile:)
- Purchased an additional Vesc, motor, and mount from diyelectricstakeboard.com

Now here are my issues:
- My VESCs are physically the same but have different firmware - i have tried several different ways to update the firmware on each one and continue to get errors. Most commonly I am getting this error: 

**"The I/O operation has been aborted because of either a thread exit or an application request"**

I have tried updating the firmware via the VESC Tool, tried the normal update and tried the bootloader avenue - nothing works. I have tried a shorter USB cable, tried changing the settings on the port, etc., but I cannot get the firmware to update and therefore I cant change any of the settings to make my dual motor setup work. Getting very frustrated.

Anyone have any ideas? Ill try almost anything at this point.

Thank you!!!!!
Ryan
```

---
## \#19 Posted by: ryan.kareme Posted at: 2018-09-06T17:10:47.743Z Reads: 47

```
By the way. I have spent HOURS AND HOURS reading in this forum so please do not use my reading time as a measure of my commitment lol. I spent most of the time reading before I actually created an account.
```

---
## \#20 Posted by: Andy87 Posted at: 2018-09-06T17:59:23.181Z Reads: 48

```
Didn’t get it right, you checked if there is a bootloader installed on the vesc?

You should always be able to flash the fw with a stl link v2. It’s about 5-10€ on amazon
```

---
## \#21 Posted by: ryan.kareme Posted at: 2018-09-06T18:02:02.768Z Reads: 52

```
When i start up the VESC tool is says there is a bootloader installed and to update the FW using the Firmware tab. But when I do that I get the Serial Port error I mentioned.
```

---
## \#22 Posted by: Marvelous Posted at: 2019-08-15T02:35:57.316Z Reads: 22

```
I do have the same problem with the same vesc. Diyelectricskateboard team aren't answering my mail...
```

---
## \#23 Posted by: CarlCollins Posted at: 2019-08-21T23:20:18.719Z Reads: 18

```
Try running the App as administrator
And also remove the COM drivers and re-install it.
```

---
