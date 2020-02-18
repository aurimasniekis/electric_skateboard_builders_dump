# VESC troubleshooting. H.king 4.10 VESC

### Replies: 24 Views: 1345

## \#1 Posted by: Jakebarnhill1 Posted at: 2018-01-30T10:19:24.581Z Reads: 162

```
Hi everyone. 

The reason I made this thread was to work out what has been damaged on my VESC, I fried a DRV on a hobbyking 4.10 VESC because a phase wire shorted out onto the micro-usb plug while I was riding.

I know that the DRV is fried as there is a black spot on it. I am not sure wether anything else is damaged as well as the DRV chip, since when I power the VESC up, there are no lights that turn on, and when I plug it into the computer the BLDC tool does not recognise it has been plugged in. Does this mean that there is more damage than just the DRV chip?

I bought 3 spare DRV8302DCA chips from Mouser electric, https://au.mouser.com/search/refine.aspx?Ntk=P_MarCom&Ntt=113734323, and am hoping to repair the DRV myself, but I am now thinking that there may be more damage than just the DRV chip.

I am sure one of you VESC guru's can point me in the right direction. (below are some pics of the VESC)

![IMG_1423|500x375](upload://jIDdy5gCkCAdh1D8Jj8fPMbs1Qn.JPG)

![IMG_1422|500x375](upload://428XvMKeaW4b2JPZQg3n8ry9X9G.JPG)

Cheers
Jake
```

---
## \#2 Posted by: Martinsp Posted at: 2018-01-30T11:14:07.858Z Reads: 137

```
You will have to replace the drv to see because the drv is responsible for creating the 5v which is turned into 3v3 that the logic(mcu) needs to turn on
After replacing the drv check for short on all lines as well as phase outputs and battery input. If there is no short plug it in and see if the mcu boots
```

---
## \#3 Posted by: Jakebarnhill1 Posted at: 2018-01-31T10:15:09.396Z Reads: 121

```
That answers my question, thanks a lot!

Do you have any tips for replacing the DRV? This will be my first time doing such a precise soldering job.
```

---
## \#4 Posted by: Martinsp Posted at: 2018-01-31T10:17:24.395Z Reads: 115

```
Well, dont forget the pad underneath and avoid solder balls getting where they should not be so inspect the PCB throughly before powering it on, also make sure the chip is flat when you solder the pad. With some magnifying glass or a microscope check if all legs of the chip are connected
```

---
## \#5 Posted by: Jakebarnhill1 Posted at: 2018-01-31T10:20:21.001Z Reads: 111

```
Ok thanks, with the bottom pad, is the hot air enough to melt the solder that is under the chip? Thanks for the help!
```

---
## \#6 Posted by: Martinsp Posted at: 2018-01-31T10:22:38.262Z Reads: 106

```
Yeah it is definitely, even more than enough. There is no real rule to how much temperature and time is the max before some damage is done so you will just have to be careful. You can slide the plastic part of the JST connectors off without desoldering the pins that way you wont melt the plastic
```

---
## \#7 Posted by: Jakebarnhill1 Posted at: 2018-01-31T10:26:46.762Z Reads: 99

```
Thats a good tip about taking off the plastic parts. Thanks for the help, ill be sure to post how it goes :+1:
```

---
## \#8 Posted by: Jakebarnhill1 Posted at: 2018-01-31T10:30:29.364Z Reads: 96

```
ok, one more question. What temperature would you use on the hot air gun? I'm thinking 250-300C, and would 30 seconds be the limit of hot air exposure for the components?
```

---
## \#9 Posted by: Martinsp Posted at: 2018-01-31T10:44:24.635Z Reads: 92

```
I use 320C and I think it might take less before the solder melts I am not sure never measured it :/
It is hard to say because there is a lot of factors to it, like air flow, distance of the nozzle from the component, and the diameter of the nozzle to or the area that the air is focused on.

Before going full temp I suggest you set it to for example to 200C and blow on it for a minute to let the pcb heat up to prevent heat shock (big temperature differences between places on the pcb)
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2018-01-31T19:47:02.377Z Reads: 83

```
Hi Jake, 

solder melt at around 200c, so you should set your heat gun at around 240-250c and make sure your flow of air is as low as you can, you don’t want to see part flying around.

Also check if the resistor R48 to R51 are at 100ohms (give or take 10%). 

Regards
JF
```

---
## \#11 Posted by: Jakebarnhill1 Posted at: 2018-02-01T07:54:49.655Z Reads: 79

```
Thanks for the info @JohnnyMeduse , I measured those resistors and had an interesting result...

R48: 100.7 ohms
R49: 49.8 ohms
R50: 32 ohms
R51: 4.3 ohms

Im measuring by touching the ends of the multimeter wires at the ends of each resistor as you would. Do you think the resistors are damaged?

Thanks!
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2018-02-02T15:12:11.651Z Reads: 72

```
HI Jake, 

Hmmm, they are all supposed to be 100Ohms but if the DRV is damage it could lead to false measurement, maybe try to measure them once the DRV is remove or replace. 

Regards
JF
```

---
## \#13 Posted by: Jakebarnhill1 Posted at: 2018-02-18T06:01:06.538Z Reads: 68

```
An update, I managed to replace the DRV which seemed to work, however only the blue light was on after i installed it, no green light. I believe this was due to a faulty processor, so I got my other (very) cooked Vesc and unsoldered the processor off it and soldered it onto the VESC. It worked for a while until I did a motor detection and a mosfet lit on fire :slight_smile: . I knew I was so close to fixing it! so I thought f**k it ill just run the vesc on my single motor on FOC mode so I fry the DRV (I know the DRV always fries with FOC on the SK3 192KV 6364 motor, as this is what fried the other VESC) so as I hoped, the DRV fried within a minute, flashing red light on the VESC and DRV8302 error on the app. So I unsoldered the DRV to replace but in the process I permanently shorted 2 of the pads! so the board was toast :( anyway at least I got good at hot air surface mount soldering!

Thanks again for the guidance @Martinsp @JohnnyMeduse
```

---
## \#14 Posted by: ZackoryCramer Posted at: 2018-02-18T06:06:45.966Z Reads: 67

```
No need to cook the vesc just because you blew a fet. :no_mouth: Congrats on your drv replacement though.:grinning:
```

---
## \#15 Posted by: Martinsp Posted at: 2018-02-18T17:02:10.923Z Reads: 54

```
@Jakebarnhill1  What do you mean permanently shorted?
```

---
## \#16 Posted by: Jakebarnhill1 Posted at: 2018-02-18T20:12:35.796Z Reads: 50

```
2 of the pads for the DRV chip were shorted with solder and I know that you can normally use solder wick and an iron but that didn't work it seemed to be like the 2 pads joined somehow?
```

---
## \#17 Posted by: Martinsp Posted at: 2018-02-18T20:21:48.480Z Reads: 47

```
There are two times two pads shorted, it is on pins 53+54 and 51+50. These **are supposed** to be shorted as you can see on the picture below.
![vesc top|375x500](upload://yB3OQ4z0BFkhCPAZvRPGBaUZ7PX.jpg)
```

---
## \#18 Posted by: Jakebarnhill1 Posted at: 2018-02-18T20:23:26.119Z Reads: 46

```
ohhhh right...I think i only noticed one shorted, does it work if the second one isn't shorted?
```

---
## \#19 Posted by: Martinsp Posted at: 2018-02-18T20:27:27.105Z Reads: 46

```
It is shorted on the PCB anyway so even if it looked like there are no shorts visible, the traces underneath are shorted.
```

---
## \#20 Posted by: ThermalM16 Posted at: 2018-02-19T01:05:45.903Z Reads: 45

```
Martinsp is correct. Here's a picture of what the wires look like. You're looking at 50-51 and 53-54. You're still in the clear. That VESC may just come back to life yet.

 ![Capture|343x500](upload://9TlnDJhWQYcUnEZRBzmnmufjHVv.PNG)
```

---
## \#21 Posted by: Jakebarnhill1 Posted at: 2018-02-19T21:14:06.241Z Reads: 38

```
@Martinsp thats definitely a possibility, ill check the solder joints later and see if I missed any shorts.

@ThermalM16. Thats good to know! ill have another crack at it later, hopefully it will be revived!
```

---
## \#22 Posted by: Jakebarnhill1 Posted at: 2018-02-25T05:39:46.161Z Reads: 34

```
Progress has been made. I Re-soldered DRV and put it back on, and I have a red flashing light (DRV error), but at least i know the VESC still works. My soldering is very bad, I know that :sweat_smile:. when plugged in to the esc configurator, in RT data, it shows that the current isn't on 0 and is a little bit higher or lower, and the Mosfet temperatures are in the negatives. So I'm sure that I put the DRV on badly. here are some pictures:

![IMG_1479|666x500](upload://gkKj4pbGuEDPQIL1GnUG5gLJXb7.JPG)![IMG_1477|375x500](upload://AbWKRIEu0DQpRQYDbH0wyWLOp9p.JPG)![IMG_1475|375x500](upload://veYFXHBWdeIYOU2YalvT6enYNbb.JPG)![IMG_1480|666x500](upload://a9EYa2nXcYgPBvDsEDRnSPnVmKZ.JPG)![IMG_1478|666x500](upload://ioJNYEIvmAQivL9v9vk5ChoTMmR.JPG)![IMG_1476|375x500](upload://2pcKHfO9bwZvOf9sgCDQ4JAoMMl.JPG)

Do you think that the reason the solder joints are coming out so badly is because i'm using lead free solder paste? I've installed the chip by tinning the ground pad with a soldering iron, cleaning up the solder pads with solder wick, apply a small amount of flux, then solder paste on top, then put the chip on and hot air solder it on. then there are a fair few bridges between the pins of the DRV so I clean them up with solder wick, but it seems that the solder wick is taking off to much solder. anyway i think ill order a few more DRV8302DCA chips and start again with a fresh DRV, as this chip is probably dead now after all my soldering abuse.

Cheers 
Jake

Edit: I also replaced the ARM chip from another VESC, since the firmware was wiped from the original chip.
```

---
## \#23 Posted by: pat.speed Posted at: 2018-02-25T05:54:48.440Z Reads: 31

```
Hmm some pins don't look like they are even connected, just do a check and make sure as one pin near the top of the last pic on the right side looks to be disconnected


Edit: How was the Vesc going before this happened? And did you contact HobbyKing about a refund?
```

---
## \#24 Posted by: Martinsp Posted at: 2018-02-25T09:13:14.715Z Reads: 31

```
You are definitely on the right track, but it is a little too misaligned, the solder joints would be definitely more easily done with leaded solder.
Wick cant remove too much, there will always be a little bit underneath the leg of the chip.
Check R48-R51, all 4 should be 100 ohms (with some tolerance 1% most probably). I had similar problem before with a 4.10 where these were faulty and displaying wrong current. The resistors are on lines between shunts and DRV.
```

---
