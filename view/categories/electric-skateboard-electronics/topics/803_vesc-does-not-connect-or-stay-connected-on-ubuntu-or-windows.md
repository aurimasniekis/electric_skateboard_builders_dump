# VESC &#124; does not connect or stay connected on ubuntu or windows

### Replies: 20 Views: 4045

## \#1 Posted by: longhairedboy Posted at: 2015-12-24T18:47:06.887Z Reads: 249

```
I'm not a noob to computers, coms, serial, or usb. I'm a total noob to VESC, however, and this is the first time i've tried connecting one to BLDC tool.This is an Enertion VESC that went out with the most recent batch. I keep seeing how "easy" this is and figured most of the uissues would be ironed out by now, so maybe i'm doing something stupid. 

I have the VESC powered by a DC power supply set to a max of 22 volts. It can only draw 5 amps from this unit. Should be plenty for bench testing and motor detection. 

I installed the windows bldc tool and usb/serial drivers it came with. I made sure nothing was plugged into my serial port (i have a smart power strip that i use on my desk). I Connected the USB cable to the VESC and my PC. plugged in the motor phase wires. The default connection is set to COM3. 

I click connect and it says DEVICE NOT FOUND. 

I switched to COM2 and got the same thing. 

I switched to COM1 and it says CONNECTED, then after a second or two it says NO FIRMWARE READ RESPONSE. and then says Not Connected again. 

As soon as its powered on, the blue LED begins blinking rapidly and just keeps doing so sort of like a hard drive light does when its reading. 

Before i tried it on windows, i got the same issue on Ubuntu. DEVICE NOT FOUND every time i hit connect no matter what COM i was using.  

What am i doing wrong here? I tried both VESCs thinking maybe one was just bad. They both do this.
```

---
## \#2 Posted by: sk8ace Posted at: 2015-12-24T19:14:02.044Z Reads: 235

```
Open up Device Manager in windows and check to see what Com port it is actually using instead of trying to guess. Mine was on Com7. Plug in the vesc after you have device manager open and you should see it pop up on the list.
```

---
## \#3 Posted by: longhairedboy Posted at: 2015-12-24T19:51:43.501Z Reads: 227

```
i rebooted, then reconnected the VESC thinking i had a com conflict and then went into the device manager and powered on the VESC. I'm still only seeing COM1 in the device manager. ITs as if the drivers for the virtual COM ports isn't working right. i reinstalled the drivers, still no dice. 

I tried three different cables, one of which isd a known good USB data cable and not just a charge cable from an old device. 

This hurty my head.
```

---
## \#4 Posted by: longhairedboy Posted at: 2015-12-24T21:18:48.188Z Reads: 204

```
just uninstalled the virtual com port drivers that came with the windows bldc tool from onloop's google drive link  and tried some different ones from someone else. Still nothing. 

Is there possibly some kind of version conflict between the tool and the VESC? It looks like the tool is version 2.5. I have no idea what version of anything is on the VESC since its not written enaywhere on the board and I can't get it to connect and tell me.  .
```

---
## \#5 Posted by: cmatson Posted at: 2015-12-24T21:30:01.426Z Reads: 192

```
I'm going to try setting up my VESC from enertion's batch either tonight or sometime tomorrow. (I'm on windows aswell)

I recently set up the one I got from @chaka, so I at least know my software is working- from there I can see what's possibly different about this newer batch... 

I think the BLDC tool I currently have is 1.14 if I'm not mistaken; or whatever the latest one was before FOC. 

So do enertion's new VESC's come with the firmware for FOC, or are they still rocking the older stuff? could using a new BLDC tool with an older VESC make any problems?

just spitballin here because I know basically as much as you do about VESC stuff...

Hope you get it sorted out
```

---
## \#6 Posted by: psychotiller Posted at: 2015-12-24T21:37:46.585Z Reads: 174

```
My Vesc's from Ollin came with 2.4 and then I was prompted to update the firmware as soon as I connected them to 2.5. It took a few trys and some fumbling to get them to connect though. I would click connect, nothing, connect, nothing , connect, nothing...and then it was like "hey man, what's up?"
```

---
## \#7 Posted by: kai Posted at: 2015-12-24T21:54:21.340Z Reads: 171

```
ok i had the same problem. i cant figure out how to install firmware for 2.5 with windows so if you want to get up and running without foc.... just download bldc tool 1.14 since that is what is installed on your vesc right now. no foc but you can at least ride and test it.
```

---
## \#8 Posted by: onloop Posted at: 2015-12-24T22:10:14.629Z Reads: 171

```
Here is the older version of BLDC tool. This is compatible with the firmware that is installed on the last batch of vesc. 

Also. I don't know if this matters.. but I have never had to manually install the STM driver... windows always detected and installed the driver automatically. I have lots of usb ports so normally I'm on COM12.

I have never had a problem with connecting this way

https://drive.google.com/file/d/0B4M52aF7FaMWM2lsalBNbjlWNWM/view?usp=sharing
```

---
## \#9 Posted by: longhairedboy Posted at: 2015-12-24T23:11:36.284Z Reads: 164

```
I just downloaded the 1.14 version and i'm still getting the same issue. Windows just isn't seeing the device and isn't having any reaction to it when i plug it in or unplug it. Nothing pops up in device manager and a manual sweep across COM1-20 doesn't allow me to connect. BLDC tool only reacts to COM! and then after a few seconds of saying its connected, it tells me it can't read the firmware. 

I wonder if the fact that i have an actual, physical serial port on com1 is causing a problem. I'm going to disable it in the uefi for now and see what happens.
```

---
## \#10 Posted by: sk8ace Posted at: 2015-12-24T23:37:54.993Z Reads: 158

```
Did you try to install the driver? I had to install one to make it work. The driver install is in the "bldc-tool-windows-drivers" folder
```

---
## \#11 Posted by: kai Posted at: 2015-12-24T23:42:28.942Z Reads: 155

```
the first usb port i tried has been acting up and wouldnt detect it so i had to use the one on the motherboard. when i did that windows update downloaded chibios and i was golden at that point. worth a try
```

---
## \#12 Posted by: longhairedboy Posted at: 2015-12-24T23:53:13.876Z Reads: 150

```
yes. I installed, reinstalled, unistalled then reinstalled, rebooted after reinstalling, disabled my actual serial port in the thinking there may be a conflict, i got nothing. 

I even tried a different USB COMs driver, the one from FTDI. Still nothing but "Device Not Found."

So far i have 2.5 and 1.14 on windows and neither will connect to the vesc. I also have a laptop running ubuntu where i previously did a make/make install compile of BLDC tool for 1.14 and its no worky there either. On that one it just says "unknown error" when i hit connect. 

I have tio be doing something wrong and i'm sure its something stupid. 

On the VESC the blue LED is blinking very rapidly and there's a tiny orange LED right next to it that's just barely glowing tinyest bit.

I havn't tried a different power supply. I'm about to try that now.
```

---
## \#13 Posted by: kai Posted at: 2015-12-25T00:02:26.964Z Reads: 139

```
I did it with my space cell. I had a blue and green light not blinking
```

---
## \#14 Posted by: longhairedboy Posted at: 2015-12-25T00:24:48.246Z Reads: 139

```
@kai that clue regarding the not blinking just confirmed a suspicion i had... and that suspicion confirmation may have just been backed up by what i'm seeing now. 

I've already torn apart my space cell, but luckily i have a whole mess of alligator clip jumpers to tie everything back togethr temporarily. 

I've got the space cell powering the VESC and i no longer have blinky lights, and Windows just piopped up a message about a device being on COM3. 

Hold your breath.. i'm about to hit the connect button.
```

---
## \#15 Posted by: longhairedboy Posted at: 2015-12-25T00:25:58.936Z Reads: 136

```
well hot damn i'm connected.
```

---
## \#16 Posted by: longhairedboy Posted at: 2015-12-25T00:48:39.305Z Reads: 135

```
Motor detection just happened!

Thanks guys for the assist. 

WHAT WENT WRONG MOMENT

I was using one of those PS-305D DC power supplies. I don't know if maybe i wa using it incorrectly of if the PS literally stands for Peice of Shit, but i will be doing more resaerch into why it didn't do its job today. I bought an extra one for my 14 yo son to play around with since he's getting into electronics and stuff. I hope i didn't make a mistake in doing that.
```

---
## \#17 Posted by: lowGuido Posted at: 2015-12-25T02:19:14.174Z Reads: 127

```
did you crank the current to the Max setting?
```

---
## \#18 Posted by: longhairedboy Posted at: 2015-12-25T04:00:22.284Z Reads: 122

```
I thought I did but I may not have, or I may have reset it at some point. I'll have to play with it some more.
```

---
## \#19 Posted by: boardthebuilder Posted at: 2016-08-26T09:16:26.566Z Reads: 86

```
Just got my 2 new VESC's and i am having the same problem. i know this is an old post but i thought you'd probably know more than me. i am using two LiPo batteries in series, i know its not ideal for configuring the VESCs but its all I've got. i don't have any kind of power supply. it only connects on COM1. was wondering what i could do to fix it
```

---
## \#20 Posted by: thylen11 Posted at: 2017-03-11T16:11:15.557Z Reads: 51

```
I got the same problem (no firmware read response when connecting vesc). When I try to install the drivers that come with the BLDC file they fail to download/install.
Anyone got some advice?
```

---
