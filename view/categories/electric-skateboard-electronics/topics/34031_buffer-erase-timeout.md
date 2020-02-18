# Buffer Erase Timeout

### Replies: 9 Views: 1578

## \#1 Posted by: spannepacker Posted at: 2017-09-26T21:37:10.533Z Reads: 126

```
I'm finally building up my first board! I got it set up and it was working great on my workbench. I then flashed my FOCBOX to the correct firmware for @rpasichnyk's apps (VESC_default_410_o_411_o_412.bin). The write went fine but now I can't get my motor to spin and I am unable to flash any other firmware.

The message I get is "Buffer Erase Timeout." Anyone have some tips how to get back to 2.18? The FOCBOX seems to still be running and I am able to view the stats via the metr app.

Thanks!
```

---
## \#2 Posted by: Martinsp Posted at: 2017-09-26T21:48:47.042Z Reads: 122

```
If you are using the right version of BLDC-tool or its mods then you will probably have to upload the firmware using the stlink
```

---
## \#3 Posted by: spannepacker Posted at: 2017-09-26T21:53:57.991Z Reads: 122

```
Thanks, I was just reading out the STlink. Would this be the correct piece of hardware?

https://www.amazon.com/Logisaf-ST-Link-Emulator-Downloader-Programming/dp/B01N79YDJE/ref=sr_1_2
```

---
## \#4 Posted by: rpasichnyk Posted at: 2017-09-26T21:58:05.462Z Reads: 110

```
No panic :) You do not need ST-Link. Your issue is that you are trying to use BLDC Tool with 3.x firmware, this will not work. If you want to go back to old firmware, get VESC Tool, not BLDC Tool and flash 2.x firmware with it. After you flash 2.18 with VESC Tool, continue with BLDC Tool.
```

---
## \#5 Posted by: Martinsp Posted at: 2017-09-26T22:04:28.065Z Reads: 108

```
Either way it would sort the issue :D JK, I thought you were using correct tool.
@rpasichnyk knows his stuff more than I do of course so do as he says :D
```

---
## \#6 Posted by: spannepacker Posted at: 2017-09-26T23:33:16.070Z Reads: 90

```
@rpasichnyk, you hit it on the mark. I’m back up and running. Thanks for your help!
```

---
## \#7 Posted by: Electroshmog Posted at: 2018-02-19T19:20:32.677Z Reads: 66

```
@rpasichnyk DAMN!!! You saved my life!!
```

---
## \#8 Posted by: moronicity Posted at: 2018-04-22T20:01:53.251Z Reads: 54

```
@rpasichnyk Im stuck with the same issue. All i see is the Hardware 48 and Im not able to flsh it with the vesc tool to 2.18, it says its uploading and then disconnects and then after power cycle, it still shows 48. Am I missing somethings? ![37 PM|561x500](upload://iLhP9LNkdJfdBISXd4RTYoqOJQV.png)
```

---
## \#9 Posted by: ualsteve94 Posted at: 2019-06-08T08:48:18.049Z Reads: 20

```
How do I get firmware 2.18 using the VESC tool?  I too am receiving the “buffer erase timeout” on bldc tool when trying to install 2.18 onto my Focbox.   My current firmware is 3.57.  I just cant figure out how to install the 2.18 using vesc tool.  

Thank you 🙏🏽
```

---
