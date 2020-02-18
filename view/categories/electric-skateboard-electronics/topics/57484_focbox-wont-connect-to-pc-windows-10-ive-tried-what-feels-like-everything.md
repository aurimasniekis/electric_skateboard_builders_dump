# Focbox Wont connect to pc (windows 10) ive tried what feels like everything

### Replies: 35 Views: 1301

## \#1 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:04:25.933Z Reads: 164

```
I have read every single topic on the forum that has had to do with these issues. Ive had zero luck, im helping a friend setup a brand new focbox and after being powered on (lights up blue and flashes red 3 times) and connected to my laptop, it doesn't do anything for about 10 secs and then connects but says it cant be recognized. ive looked in my device manager and it reads,( unknown usb device (port reset failed)) every time. 
ive unistalled this and restarted.
ive tried 8 different usb cables, taken the case off for each.
tried at different voltages.
tried on other pcs.
even the stmicroelec virtual com port.
tried redownloading both bldc tool and vesc tool.
still nothing.

any insights?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-06-01T15:19:44.091Z Reads: 156

```
It seem to connect to your PC, so it is probably a driver problem or com port problem

http://www.electric-skateboard.builders/t/vesc-x-doesnt-connect-to-pc-need-help/18930/19?u=johnnymeduse
```

---
## \#3 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:23:03.235Z Reads: 145

```
my pc sees it as a device is connected, but it wont show in com ports (either on device manager, bldc, or vesc tool)

any advice for a driver problem? @JohnnyMeduse
```

---
## \#4 Posted by: DeathCookies Posted at: 2018-06-01T15:31:03.892Z Reads: 132

```
I get the same error when using a bad PC cable!
When 9 use my working cable 8 have no problems but somehow i have 10 broken ones and one working one... Lol

The cable Needs to Support data Pass through. Most cables are for Power only...
```

---
## \#5 Posted by: Martinsp Posted at: 2018-06-01T15:34:06.459Z Reads: 117

```
Sometimes when the device is connected to the PC but not recognized it can be that the VESC does not boot correctly. The VESC gets connected after the red LED blinks 3 times and boots. Does it turn on and blink?
```

---
## \#6 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:34:38.266Z Reads: 112

```
yes, every time

maybe ill have to go and get that 9th usb?
```

---
## \#7 Posted by: Martinsp Posted at: 2018-06-01T15:36:32.251Z Reads: 108

```
Does the PC make the sound when you plug the VESC in?
Or give any faults like the unable to recognize device etc?
```

---
## \#8 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:37:31.717Z Reads: 105

```
yes, both makes the connection notification sound, and then gives a warning as it was not recognized.
```

---
## \#9 Posted by: Martinsp Posted at: 2018-06-01T15:38:06.321Z Reads: 107

```
Try different USB ports on the PC and ideally a different VESC if you have one?

Oh and has it ever connected before?
```

---
## \#10 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:38:54.166Z Reads: 109

```
i dont have another vesc to try with and ive tried different usb ports on 2 different laptops. still no luck.

no, its brand new
```

---
## \#11 Posted by: Martinsp Posted at: 2018-06-01T15:39:57.043Z Reads: 103

```
Okay and have you ever connected a VESC to that laptop? If not it is that the drivers are missing probably, I think there is a link in the thread about setting up VESC for the first time, I will try to find it.
```

---
## \#12 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:41:40.134Z Reads: 97

```
yes, i had 2 focboxes which i set up for my board that were fine. but they burned up due to me being uneducated about the plastic film covering the thermal tape/foam inside so im waiting on replacements.
```

---
## \#13 Posted by: Martinsp Posted at: 2018-06-01T15:42:57.882Z Reads: 91

```
Try reinstalling the drivers.
http://www.st.com/en/development-tools/stsw-stm32102.html
```

---
## \#14 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:43:27.064Z Reads: 89

```
i have done this, but i will try again
```

---
## \#15 Posted by: Martinsp Posted at: 2018-06-01T15:45:15.791Z Reads: 88

```
Well if this wont help and the USB cables wont help either, it is down to the FOCBOX :/ which is a bit harder since it does not even have the firmware/stlink connector populated. Plus you would loose warranty flashing firmware
```

---
## \#16 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:51:25.765Z Reads: 91

```
i tried the drivers again and still nothing. 

firmware/stlink?

they test them before shipping? correct me if im wrong.
```

---
## \#17 Posted by: Martinsp Posted at: 2018-06-01T15:52:24.468Z Reads: 89

```
I think they do but accidents happen.
```

---
## \#18 Posted by: Blasto Posted at: 2018-06-01T15:52:25.348Z Reads: 86

```
@CarlCollins can point you in the right direction. I don’t know the exact procedure, but if i remember well it has todo with win10.

If your lucky he’s maybe on the live chat
```

---
## \#19 Posted by: Martinsp Posted at: 2018-06-01T15:54:18.857Z Reads: 82

```
Yeah, try contacting enertion support on their website or here on the forum as Blasto suggested
```

---
## \#20 Posted by: ProgressionOfFun Posted at: 2018-06-01T15:56:40.533Z Reads: 83

```
will do, thanks guys
```

---
## \#21 Posted by: b264 Posted at: 2018-06-01T16:09:13.282Z Reads: 74

```
Use a different USB cable that is not from a cell-phone box
```

---
## \#22 Posted by: briman05 Posted at: 2018-06-01T16:13:10.144Z Reads: 71

```
I it has to be a usb cable capable of transmitting data and not a charge. That is why the charger cable for a nano-x won’t work but a ps4 controller cable will work.
```

---
## \#23 Posted by: esk8taylor Posted at: 2018-06-01T17:01:25.455Z Reads: 73

```
I also had this issue and tried 5 cables.  I went to Target and picked up a cell phone data cable and that was the fix for me.
```

---
## \#24 Posted by: ProgressionOfFun Posted at: 2018-06-01T17:21:31.709Z Reads: 69

```
I've tried 2 PS4 cables but I'll try to get a new one
```

---
## \#25 Posted by: banjaxxed Posted at: 2018-06-01T20:18:42.381Z Reads: 66

```
Check the USB port of the focbox to make sure it's clean - no fluff
If you get the connect sound and not recognised msg it's unlikely to be the cable/drivers
```

---
## \#26 Posted by: ProgressionOfFun Posted at: 2018-06-01T21:05:54.501Z Reads: 62

```
I got a new cable and it still didn't work, I'll look at the Port next.
```

---
## \#27 Posted by: Benjamin899 Posted at: 2018-06-01T22:27:09.945Z Reads: 64

```
your focbox does have a energy source right?
```

---
## \#28 Posted by: NYCeboardDude Posted at: 2018-06-02T00:15:47.173Z Reads: 62

```
I had problems connecting to my focbox too, seems my usb wire cant connect properly due to focbox case. I had to hold the wire and push it in for it to work.
```

---
## \#29 Posted by: CarlCollins Posted at: 2018-06-02T07:50:08.200Z Reads: 54

```
It happens due to incorrect COM drives or non signature drivers 
Windows 10 requires signature drivers to operate.

Also it happens when wrong USB port is used 
Required one for Windows 10 is 2.0 or higher

If the issue is not resolved yet, I will happily assist customer over team viewer. :slight_smile:
```

---
## \#30 Posted by: ProgressionOfFun Posted at: 2018-06-02T14:33:56.594Z Reads: 51

```
It is still an issue @CarlCollins I'm leaning towards drivers. Could you let me know which ones work for Windows 10 specifically?
```

---
## \#31 Posted by: CarlCollins Posted at: 2018-06-02T17:52:08.033Z Reads: 49

```
@ProgressionOfFun 
Try following this 

Step 1: Right click on start menu and select device manager 
Step 2: Go to **Ports (COM & LPT)**
Step 3: Delete all COM Drivers by right clicking on each one and selecting uninstall
Step 4: Restart Your System and Open Device Manager again to see Which COM ports appears (because some of the systems has multiple attachments attached that's why multiple COM ports might appear)
Step 5: Download this driver package: https://drive.google.com/file/d/1MS1AHeaHXwG0DQmIWHlHhhbm4MExJdw9/view?usp=sharing
Step 6: Extract it and Run "**VCP_V1.4.0_Setup.exe**" (Make sure you run it as Administrator)
Step 7: After Installation, Connect your FOCBOX to the system
Step 8: Check Device manager if **STmicroelectronics** appear with COM PORT Number Under **Ports (COM & LPT)** note that number in your mind
Step 9: Run BLDC/VESC tool and select that COM port from the drop down which you've noted in your mind.

That's it! I hope this helps

If you still face any difficulties, please let me know, Love to assist you over Team viewer
```

---
## \#32 Posted by: ProgressionOfFun Posted at: 2018-06-02T18:07:34.460Z Reads: 48

```
My laptops device manager won't show any "ports". I'll take pictures and post when I get home.
```

---
## \#33 Posted by: CarlCollins Posted at: 2018-06-02T18:13:49.405Z Reads: 47

```
@ProgressionOfFun
Then Skip to the Step 5 and do the rest
```

---
## \#34 Posted by: CarlCollins Posted at: 2018-06-02T21:28:40.633Z Reads: 41

```
Update:

Issue is not due to drivers, checked over team viewer.
Tried multiple systems with multiple cables.
It must be issue with the Port on FOCBOX or with the hardware of FOCBOX.
```

---
## \#35 Posted by: ProgressionOfFun Posted at: 2018-06-02T21:52:43.066Z Reads: 43

```
Pictures of PCB. 

Battery specs tested at:
12s 8AH 30-40c LiPo
20000uf Capacitor Pack

![20180602_164555|666x500](upload://yxtbcrfHT8l23Q6tzPDL5zBqWuD.jpg)![20180602_164505|374x500](upload://eee3kMfRxcITYoNhBUIU3vx1jPr.jpg)
```

---
