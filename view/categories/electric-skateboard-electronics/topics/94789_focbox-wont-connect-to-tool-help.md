# Focbox wont connect to tool. Help!

### Replies: 31 Views: 391

## \#1 Posted by: Migro Posted at: 2019-05-23T21:59:12.994Z Reads: 87

```
Im trying to help my brother after he used countless hours trying to figure this out. Thought i had an idea and used older posts, but unfortunately nothing wanna work as intended. 

The problem is the focbox is not seen by the vesc-tool..

So i read and read and people seemed to use a stlink to upload new bootloader or firmware. It would not allow me to do so. :confused: 
"unable to run verification"

So now i need your knowledge.
```

---
## \#2 Posted by: Saturn_Corp Posted at: 2019-05-24T15:10:54.879Z Reads: 77

```
Does your computer recognize a device has been plugged in when you connect your vesc?

I'm having a problem with one of mine where it's not recognized by Windows or the bldc tool. Hope someone might know what's up here...
```

---
## \#3 Posted by: Migro Posted at: 2019-05-24T15:12:13.022Z Reads: 74

```
I am able to see it in device manager, but nothing in the tool :confused:
```

---
## \#4 Posted by: Saturn_Corp Posted at: 2019-05-24T15:13:16.624Z Reads: 70

```
And is your micro usb cable able to do data transfer? That's a common issue people have.
```

---
## \#5 Posted by: Migro Posted at: 2019-05-24T15:16:46.177Z Reads: 70

```
tried more than 10 usb cables, pretty sure most of them should be able to do data transfer.
```

---
## \#6 Posted by: Saturn_Corp Posted at: 2019-05-24T15:18:09.668Z Reads: 66

```
Hmmm, I don't know then. Maybe @CarlCollins can help whenever the Aussies wake up.
```

---
## \#7 Posted by: Migro Posted at: 2019-05-24T15:29:37.270Z Reads: 59

```
Yeah im just hoping someone have any ideas :slight_smile: thanks tho. 
![image|479x107](upload://upjcG1WIe6ke7Tjh4fNyfOo8dKl.png)
```

---
## \#8 Posted by: Saturn_Corp Posted at: 2019-05-24T15:31:42.266Z Reads: 63

```
You probably already saw the post from 2018, but did you try this?

Step 1: Right click on start menu and select device manager

 Step 2: Go to  **Ports (COM &amp; LPT)** 

 Step 3: Delete all COM Drivers by right clicking on each one and selecting uninstall

 Step 4: Restart Your System and Open Device Manager again to see Which COM ports appears (because some of the systems has multiple attachments attached that’s why multiple COM ports might appear)

 Step 5: Download this driver package: [https://drive.google.com/file/d/1MS1AHeaHXwG0DQmIWHlHhhbm4MExJdw9/view?usp=sharing ](https://drive.google.com/file/d/1MS1AHeaHXwG0DQmIWHlHhhbm4MExJdw9/view?usp=sharing)

Step 6: Extract it and Run “  **VCP_V1.4.0_Setup.exe**  ” (Make sure you run it as Administrator)

 Step 7: After Installation, Connect your FOCBOX to the system

 Step 8: Check Device manager if **STmicroelectronics**  appear with COM PORT Number Under  **Ports (COM &amp; LPT)**  note that number in your mind 

Step 9: Run BLDC/VESC tool and select that COM port from the drop down which you’ve noted in your mind.

Didn't work for me though :/
```

---
## \#9 Posted by: Migro Posted at: 2019-05-24T15:36:57.478Z Reads: 57

```
Strange its involving 2 focboxes right and seems like only one of them is able to be recognised by the computer.
```

---
## \#10 Posted by: Migro Posted at: 2019-05-24T15:44:06.123Z Reads: 52

```
Nope didnt do it for me either :/ i may need to wait for the aussie :stuck_out_tongue:
```

---
## \#11 Posted by: CarlCollins Posted at: 2019-05-25T17:00:57.560Z Reads: 47

```
Your issue is fixed or not?
```

---
## \#12 Posted by: Migro Posted at: 2019-05-25T19:36:27.296Z Reads: 43

```
Nope i have not
```

---
## \#13 Posted by: CarlCollins Posted at: 2019-05-26T09:37:26.241Z Reads: 37

```
I would like to inspect both of them using a remote access to your Windows PC
```

---
## \#14 Posted by: Migro Posted at: 2019-05-26T12:18:13.009Z Reads: 36

```
Sure. The only problem is time difference. 
And i cant Seem to see one of Them on The computer.
But definetly give it a try
```

---
## \#15 Posted by: CarlCollins Posted at: 2019-05-27T04:38:39.860Z Reads: 34

```
Let me know when you are ready
```

---
## \#16 Posted by: Migro Posted at: 2019-05-27T05:54:09.891Z Reads: 34

```
You Got time now?
```

---
## \#17 Posted by: CarlCollins Posted at: 2019-05-27T18:19:56.228Z Reads: 31

```
Available now
```

---
## \#19 Posted by: CarlCollins Posted at: 2019-05-29T11:39:25.106Z Reads: 18

```
I am available for next 4 hours now
```

---
## \#20 Posted by: Migro Posted at: 2019-05-29T13:24:51.226Z Reads: 16

```
Ill be home in less tHan an hour
```

---
## \#21 Posted by: CarlCollins Posted at: 2019-05-29T13:30:19.797Z Reads: 14

```
Alright, waiting for you
```

---
## \#22 Posted by: Migro Posted at: 2019-05-29T14:10:12.779Z Reads: 13

```
Im ready 
How Should we do this?
```

---
## \#23 Posted by: CarlCollins Posted at: 2019-05-29T14:29:28.371Z Reads: 13

```
Download and install teamviewer on your Windows PC
```

---
## \#24 Posted by: Migro Posted at: 2019-05-29T14:30:49.373Z Reads: 13

```
Allready did :wink:

 1 286 334 369

m8du59
```

---
## \#25 Posted by: AlanZhou Posted at: 2019-05-29T14:32:24.614Z Reads: 13

```
Should put those numbers in pm... Anyone can connect to your computer via those numbers on TeamViewer
```

---
## \#26 Posted by: Migro Posted at: 2019-05-29T14:33:44.976Z Reads: 13

```
Yeah i know but hope it doesn't happen for now
```

---
## \#27 Posted by: Migro Posted at: 2019-05-29T14:34:08.823Z Reads: 12

```
ill get some new and pm him :+1:
```

---
## \#28 Posted by: CarlCollins Posted at: 2019-05-29T14:34:51.435Z Reads: 12

```
That's what I was going to say, 
Thanks for the reminder mate
```

---
## \#29 Posted by: Migro Posted at: 2019-05-29T15:36:55.858Z Reads: 12

```
Okay thanks to @CarlCollins helped me fix one of them. I just assumed the worst when it was pretty straight forward :stuck_out_tongue: 

But the other one seems faulty. Could this mean a burned drv chip? This is from the focbox thats not working

![rip%20focbox|375x500](upload://dxVQXB8v6u5J91m9DKQSxIllXeJ.jpeg)   
The other focbox looks like this on the drv chip

![Fino%20focbox|375x500](upload://fD79KAMiUrh79mEYzdreF6iiRUq.jpeg)
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-05-29T15:41:32.042Z Reads: 12

```
That drv looks cooked from the picture... But can't see that well
```

---
## \#31 Posted by: Migro Posted at: 2019-05-29T15:49:59.932Z Reads: 12

```
yeah thanks just what i thought
```

---
## \#32 Posted by: CarlCollins Posted at: 2019-05-29T20:11:38.926Z Reads: 10

```
Happy to Help
```

---
