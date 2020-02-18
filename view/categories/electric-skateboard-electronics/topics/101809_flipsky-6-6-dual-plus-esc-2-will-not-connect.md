# Flipsky 6.6 dual plus esc 2 will not connect

### Replies: 9 Views: 265

## \#1 Posted by: JP3D Posted at: 2019-09-15T11:41:54.833Z Reads: 56

```
Hi I'm new here, making my first proper build with the flipsky 6.6 plus but I cant seem to get port 2 to connect so I can update the firmware and run the setup wizard.
I'm using the factory cord and its turned on. I've uploaded the boot loader and firmware on port 1 with no problems but when I try to connect to port 2 I get this error message "could not read firmware version. Make sure that the selected port really belongs to the VESC"

I've got the flipsky VX2 and plugged it in to uart but only the 1 esc is powering the motor, if I swap it to the plug next to it then only the 2 esc works and all 4 lights are on so it seems to be all going and I'm hoping once I can update the firmware then I can switch something on the vesc tool to make both go. 
Any advice would be greatly appreciated 

![20190915_232926|690x335](upload://wHDOqUorcnWVmlPfbkWwvnAtUsQ.jpeg)
```

---
## \#2 Posted by: Fosterqc Posted at: 2019-09-15T12:36:15.047Z Reads: 52

```
When you write the firmware onto the master does it put it on the slave as well? And throw an error when you try to connect to the slave?

Or are you following some instructions and this is what it said to do?

Sorry I'm unfamiliar with Flipsky vesc
```

---
## \#3 Posted by: Braniac Posted at: 2019-09-15T13:58:47.066Z Reads: 49

```
So you have the dual 6.6 plus and you are trying to update firmware? I believe you should be able to configure all settings on the master esc (port 1?) and the slave should follow suit. Do you have both motors connected? Sensors or no? 
(When I did initial setup on my single 6.6 I actually had the sensor wire plugged into the wrong port and it prevented usb connection so be sure to double check all your connections.)

Here's a video they have on their site. . says usb must be connected to master. 
https://www.youtube.com/watch?v=SaLwRQ503jk&feature=youtu.be
```

---
## \#4 Posted by: JP3D Posted at: 2019-09-16T03:25:35.032Z Reads: 38

```
Yes correct dual 6.6 plus fesc. At the start I successfully updated it on the master (port 1) but when I go to the set up wizard it says that not all esc are updated so I figured it must not be communicating. Is there some sort of cam switch like on the standard 6.6 and mini? Or is there a way to turn on cam communication in the vesc tool via the master port?
```

---
## \#5 Posted by: JP3D Posted at: 2019-09-16T03:30:17.143Z Reads: 37

```
Yes I have both motors plugged in but no hall sensors. Which port is for the master board? They have it plugged into port 2 in the video
```

---
## \#6 Posted by: Braniac Posted at: 2019-09-16T12:05:53.724Z Reads: 31

```
It looks like you should be able to select the option for multiple ESC in the vesc tool during setup. . Sounds to me like a hardware issue. .  Sorry I'm pretty new to DIY myself just hoping i could help. Here's a link to a long page discussing dual 6.6. hopefully you can find the info you need somewhere on the forum. Good luck! 

 https://www.electric-skateboard.builders/t/flipsky-dual-fsesc-6-6-discussion-findings/67155/118
```

---
## \#7 Posted by: Braniac Posted at: 2019-09-16T12:21:24.533Z Reads: 30

```
comparing the images of the 6.6 dual to the 6.6 dual plus oh, it looks like there is no switch to activate 2nd ESC on the plus. Looking at the images and applying my powers of deduction I'm noticing that the communication ports are on the side of the ESC that says 2.. and the can bus connection is on side one. . and as you mentioned that they had port 2 connected in the video. Have you tried doing initial setup connected to port 2? Perhaps doing initial setup on port 1 is interfering with setup of port 2 if port one is actually the slave.. I know you said you tried connecting to port 2 and got error message.. 

Hope this isn't confusing.
```

---
## \#8 Posted by: Kodin Posted at: 2019-09-17T07:30:26.783Z Reads: 20

```
I had issues with mine with the latest VESCTool.  Using an older version allowed me to flash both and downgrade them a version, then I was able to connect my flipsky bluetooth adapter and upgrade them one at a time to the latest version.  It was super weird.  I'm assuming it is an issue specifically with the (then) latest version of VESCTool and has since been remedied.   Any time I've tried connecting to either VESC since has gone flawlessly.
```

---
## \#9 Posted by: cherryflavouredpez Posted at: 2019-09-17T09:10:14.701Z Reads: 16

```
did you set a unique VESC ID for each VESC ? If so, you also need to set the send CAN status for the master (VESC 2) and "send 1234" for the secondary  (VESC 1). That way you plug your controller in the primary VESC (2) and it forwards the signal to the secondary (VESC 1)
```

---
