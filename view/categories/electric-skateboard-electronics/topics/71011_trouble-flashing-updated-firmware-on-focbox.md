# Trouble flashing updated firmware on FOCBOX

### Replies: 27 Views: 663

## \#1 Posted by: RHill051 Posted at: 2018-10-12T18:56:05.979Z Reads: 117

```
Hey guys, I know this is a pretty common topic but after reading dozens of threads I'm looking for some advice on what is going on. A little backstory, I fried the MCU in my FOCBOX and after replacing it the FOCBOX now powers on and I can connect to it. @CarlCollins was incredibly helpful getting the FOCBOX to connect to my computer and set up for my motor and hardware using the BLDC tool (turns out I didn't have the right drivers on my computer). However I was wanting to try using the Ackmaniac tool or the new VESC Tool but when I connect to the FOCBOX it says that the firmware is out of date (which makes sense since I have 2.18 on the FOCBOX) so I go to the firmware tab, select "**410 & 411 & 412**" then the VESC_default.bin and click upload. It appears to upload but as soon as it completes it shows an error message (which I though was supposed to be normal) but never becomes available to connect to again. I have to pull the loop key and restart the ESC in order to get it to connect again and the firmware has not been updated. I'm not really sure what to do. I mean the board works and I can go ride no problem but I was wanting to try using Ackmaniac so I could play around with the Bluetooth connection to read info from the ESC. My only guesses now are that something is going on with the bootloader or maybe there is an issue with something else hardware wise on the board. I'm open to all suggestions to better understand what is going on here.
```

---
## \#2 Posted by: MatrixWriter Posted at: 2018-12-07T04:12:07.437Z Reads: 102

```
I'm having the same issue as well - did you manage to resolve this? I have an ST-Link arriving to me in a few days from now.  

Maybe the issue is that the FOCBOX doesn't have a bootloader so one needs to be flashed to it?
After flashing then it can be updated to a newer firmware to use VESC Tool as BLDC Tool is pretty much outdated.

Hopefully someone can help, otherwise I'll sell these like-new FOCBOXs 2.18 FW on eBay and get a VESC as this is getting annoying.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-12-07T04:45:04.644Z Reads: 94

```
What exactly is your problem and how it came to it? You also replaced the MCU or you just wanted to flash a new fw and now nothing is working anymore?
```

---
## \#4 Posted by: MatrixWriter Posted at: 2018-12-07T05:36:00.917Z Reads: 91

```
I acquired 2 like-new condition and fully functioning FOCBOXs, however I would like to use it on VESC Tool as BLDC Tool with FW 2.18 is lacking in some features that typically like with VESC Tool and newer FW.

The 2 units still work, but they refuse to update to later firmware. When I try to update, it just says 2.18 FW. 

I've tried different methods of updating and using Ackmaniac FW and Extended BLDC Tool and VESC Tool Bootloader section with no luck at all. Last thing I'll try is flashing the bootloader when I get the STW-Link in the next few days.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-07T05:41:38.699Z Reads: 89

```
that´s strange, as Focboxes usually come with a bootloader on, so it shouldn´t be and issue to upgrade to fw 3.xx via VESC tool only.
Hope it will work with the ST-Link than!
I think you know that you first need to solder some jst- plug on the fockbox before you can use the ST-link (maybe not soldering, but as min fix it somehow in the PCB).
```

---
## \#6 Posted by: MatrixWriter Posted at: 2018-12-07T06:04:52.673Z Reads: 83

```
Yeah, that's what I thought too! I'll keep everyone posted on what happens when I receive the ST-Link.

Thanks for the info about the soldering heads up for the FOCBOX!
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-07T06:26:06.807Z Reads: 82

```
you can find a good description here
https://www.electric-skateboard.builders/t/help-with-focbox-firmware-bootloader-upgrade-vesc-tool/34810/38?u=andy87

just in case.
```

---
## \#8 Posted by: MatrixWriter Posted at: 2018-12-07T06:59:39.747Z Reads: 78

```
Looks good! Will have to wait until I get the ST-Link.

Here's what VESC Tool shows about the FOCBOX as there is no HW ID info. Only 2.18 FW, so pretty much no bootloader from what I saw in other posts.

![2018-12-06%2022_55_35-ESC%20Tool|690x379](upload://8kYkwDXmfWnTmHycrBYLS4LfUdA.png)
```

---
## \#9 Posted by: Andy87 Posted at: 2018-12-07T07:05:21.789Z Reads: 73

```
If you one day will find out what "limited mode" means in the right down corner, let me please know. always interested to learn new things.
maybe @CarlCollins our Focbox guru has a minute to have a look at your problem to update to a new FW.
```

---
## \#10 Posted by: MatrixWriter Posted at: 2018-12-07T07:28:43.237Z Reads: 72

```
Limited mode means that only firmware section feature only works. 

I had this issue with a Flipsky VESC that was on an older FW and updated it. Then all the other features worked.
```

---
## \#11 Posted by: CarlCollins Posted at: 2018-12-08T15:45:55.641Z Reads: 69

```
@MatrixWriter
Looks like you just need to flash the firmware using normal flashing process 
Use default BLDC tool, then it will work
Limited mode only shows when loaded firmware is older or newer than the supported one for VESC tool

For FOCBOX, I strongly recommend using BLDC tool from our website
You can get them here:
**Windows Version:** https://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/
**MAC Version:** https://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-mac/
```

---
## \#12 Posted by: CarlCollins Posted at: 2018-12-08T15:53:46.239Z Reads: 67

```
If you still want to use VESC tool
You have to flash the supported firmware on it but this will void the warranty on your FOCBOX (platinum warranty excluded)

See the attached image!
![2018-12-08_2050|690x379](upload://ijTzuElQszK6d8z60bhsyuMi1o2.png)
```

---
## \#13 Posted by: CarlCollins Posted at: 2018-12-08T15:57:15.378Z Reads: 65

```
If you are having issue that you are not able to flash the 3.1xx firmware on the FOCBOX 
Try using following method 
1: Get the Vesc_default.bin from the VESC tool firmware directory and put it on your desktop
2: Run BLDC tool and select that file, perform a flash and then turn the setup off 
3: Connect it again to PC and run VESC tool, then it will work :slight_smile:
```

---
## \#14 Posted by: Bjork3n Posted at: 2018-12-08T16:22:06.521Z Reads: 60

```
May i ask why you recommend bldc tool over vesc tool for the focbox?
Vesc tool seems far more user friendly compared to the old bldc tool.
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-12-08T19:26:23.906Z Reads: 59

```
@Bjork3n
We got reports from customers that Ackmaniac firmware cause issues with the FOCBOX but still not sure why
That's why we recommend default BLDC tool (Enertion Version)
```

---
## \#16 Posted by: Bjork3n Posted at: 2018-12-08T19:31:42.913Z Reads: 60

```
Really? Thats weird since it seems to be  to most common used Fw for the focboxes.
So youre saying that enertion only recommends the 2.18fw and that people should avoid upgrading over 2.18fw on the focbox hardware?
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-12-08T19:33:31.301Z Reads: 61

```
@Bjork3n
Upgrading to foreign firmware will void the warranty (default 60 days one only) so we always recommend 2.18
Noobs can stick to 2.18 and BLDC tool, professionals can use any firmware they want with the consequences :slight_smile:
```

---
## \#18 Posted by: MatrixWriter Posted at: 2018-12-09T12:26:58.262Z Reads: 59

```
I tried both methods of updating the FW and no luck from Carl's instructions. 

Decided to go with my original method - used ST-Link I got in the mail and flashed the bootloader hex file (Vedder forums for BLDC Bootloader download is broken so I had to compile my own -- sucks) and got it updated to VESC FW 3.40. It's much better than 2.18 and I have not had issues with it with my other VESCs that is on the latest FW.

Super annoyed that I had to go through this and that the FOCBOXs that I got did not have bootloader. I will make a YouTube tutorial video on flashing, troubleshooting and updating the FW for FOCBOXs since I have one more to flash.

-----------
TLDR: If you can't update the FW and it only shows the version number without a UUID, you don't have a bootloader, so it needs to be flashed.

PS: It isn't recommended to connect the 3.3V line for the Link, power the VESC from your battery.

![2018-12-09%2003_07_33-VESC%20Tool|690x379](upload://2MHmdkcAT8ffBAFLaPhbhY04Jvo.png) 
![2018-12-09%2004_09_14-VESC%20Tool|690x388](upload://qkGg5hIR12BjKQWjdM7Kmnfh0B7.png)
```

---
## \#19 Posted by: MatrixWriter Posted at: 2018-12-09T12:28:21.507Z Reads: 58

```
![2018-12-09%2004_14_05-VESC%20Tool|690x388](upload://2NBL8fMIHLdmBxPuiVR34KbCGQy.png) 
![2018-12-09%2004_14_24-VESC%20Tool|690x388](upload://7cvcvT1v4ciur8GsLPZlySQjLL2.png)
```

---
## \#20 Posted by: CarlCollins Posted at: 2018-12-09T20:08:38.840Z Reads: 54

```
That's odd, FOCBOX came with a bootloader
I think there might be some other issue
```

---
## \#21 Posted by: trampa Posted at: 2018-12-29T20:30:42.521Z Reads: 45

```
If VESC-Tool can't update the FW: 98% chance the boot loader is missing.
You can flash the boot loader without using a ST-link. There is a boot loader tab in Vesc-Tool!

BLDC-tool is outdated and lacks certain safety features. It is not recommended to use BLDC-Tool any longer! Vedder strongly advises to switch to Vesc-Tool and always keep the device updated. VESC-Tool and Vesc-Tool mobile will inform you about available updates when connecting to the device. This way you don't miss out the updates. 

Recommending to use the old BLDC-Tool is no good idea. 
It lacks features like temperature headroom for brakes, which prevents a complete loss of brakes due to over temp shutoff. There are more safety critical updates in VESC-Tool that you should not miss out. 
It is very advisable to use the latest Vedder software only.
There is a reason why VESC-Tool is compatible with old HW-designs like the 4.xx 
BLDC-Tool hasn't seen any updates since VESC-Tool replaced it.
```

---
## \#22 Posted by: MatrixWriter Posted at: 2019-01-03T09:04:28.354Z Reads: 39

```
Yup, absolutely agree with you on these points! Everything is updated. I just need to finish making a clear tutorial video and such.

Thanks everyone!
```

---
## \#23 Posted by: sayekim Posted at: 2019-01-03T09:16:13.798Z Reads: 40

```
Have you always tried the same usb cable?
Try a different one that can handle data. 

I don’t recommend fw3.40. This one gives me over current faults when the combined motor amps reach 160amps. 

No problem with 3.38 so far. 

@trampa
```

---
## \#24 Posted by: MatrixWriter Posted at: 2019-01-09T08:31:53.582Z Reads: 41

```
I tried with different USB cables and still had issues.

Anyway, good to know about FW 3.40. I haven't done enough testing but will keep it in consideration.
On my non Focbox VESC, I am running FW 3.38 and it's rock solid. I might downgrade the FW on the Focboxes.

What were your motor and battery current values when you had the fault issue?

On my board, the motor is set to 50A and battery is 30A.
My friend's board settings are 60A and battery is 60A as he has stronger motors and a bigger battery than me.
Both have gone hundreds of miles without any issues.
```

---
## \#25 Posted by: sayekim Posted at: 2019-01-09T09:47:46.096Z Reads: 43

```
As long as the absolute max current on each esc is set to 160 amps it won’t be a problem when the combined motor amps don’t reach 160 amps. 

In your case with 50 motor amps you would be safe since the combined current would only be 100 amps. 

I have tried with 80 amps which is at the limit and it will cut off the power when I hit it in fw3.40. No such problem in 3.38. 

My settings were in 3.40:

Motor amps
80 and 100 and 120
-60

Battery amps
60
-30

Since neither one of you have a combined motor current value of over 120amps there is no problem since the default absolute max current in fw3.40 is 130 amps.
```

---
## \#26 Posted by: MatrixWriter Posted at: 2019-01-09T19:35:53.262Z Reads: 31

```
Excellent info, thanks for sharing!
You might just have saved me and many others from a nasty high speed fall!
```

---
## \#27 Posted by: sayekim Posted at: 2019-01-09T21:42:22.480Z Reads: 27

```
I’d like to think so yet I have yet to hear from anyone else with the same problem. 

I’d also like to think so that I can’t be the only one here who’s run fw3.40 and gone over combined 130 or 160 motor amps for a dual setup. 

Mind you I did have to test this while sitting on the board for 1 I’m leaning madly forward to counter act the torque and 2 for the fear that when it does cut off I can’t be thrown off since that was the case with 3.40.

It’s times like these I wish you know who was around to confirm shit like this.
```

---
