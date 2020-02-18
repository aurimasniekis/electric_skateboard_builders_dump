# FOCBOX robotic platform, encoder issue

### Replies: 13 Views: 733

## \#1 Posted by: Ben_m Posted at: 2018-01-09T07:34:17.607Z Reads: 138

```
OK 2nd time writing this....
We have been testing the use of VESC in an industrial robotics plateform.   Think two independent wheels, skid steer.   We got the basics working, but low speed resolution (control) has been bad, so we upgrading to using 1000P/R abi encoders, instead of the internal hall sensors in the 'hover' board direct drive hub motors. 
We are also switching to FOCBOX at the same time, because we got a pair in the black friday sales. 

We have removed the Hall sensor 'filter' components (R11,12,13, C6,7,8 and shorted out R8,9,10)
When we look at the encoder pulses with an oscilloscope we see nice square wave forms with no slew.  Low 0.3V, high 4.95V,  

But using the VESC tool wizard, it fails encoder detection everytime.  Motor turns with roughtly 20 degree steps one way for about one rev, then repeats in the other direction, it either, just keeps pulsing indefinitely then or stops and drops the comms. either failure mode requires a power cycle of the FocBox to recover. 

So my questions are:
Was removing the filter components necessary? 
Is the 0.3V low, hard enough low, for the logic level low? (assuming so but just asking)
Is there anyway to see the encoder signals on a graph?  I believe BLDC tool, did this but when I run BLDC tool now, it says my firmware version needs updating, what FocBox firmware version does BLDC tool require? 
From a firmware version point of view can I treat the FOCBOX as a 4.12 hardware, I know the Power fet package is much improved but anything that really effects FW?

Any other suggestions? 

Thanks in advance.
```

---
## \#2 Posted by: scepterr Posted at: 2018-01-09T07:52:53.724Z Reads: 127

```
Well the one part of that I can answer is you need to download the BLDC tool from the enertion website for the focbox
```

---
## \#3 Posted by: xilw3r Posted at: 2018-01-09T14:20:03.230Z Reads: 107

```
That is really awesome my dude.

Can we have any more details about your bot? what for. how big, construction? pics are always great :D


About your question... I believe you should probably contact Vedder directly about this. I'm pretty sure he would respond.
```

---
## \#4 Posted by: Ben_m Posted at: 2018-01-09T20:47:04.732Z Reads: 76

```
Did that but it says the firmware needs updating. Any  body know where I can find a focbox firmware?
```

---
## \#5 Posted by: Ben_m Posted at: 2018-01-09T20:48:18.728Z Reads: 69

```
I have a virgin Focbox perhaps the FW can read of it? I'll have a look this morning.
```

---
## \#6 Posted by: scepterr Posted at: 2018-01-09T20:49:02.176Z Reads: 67

```
If it's the firmware the focbox shipped with, the bldc tool from the site is the one you need, if it's different firmware then it needs the corresponding bldc tool
```

---
## \#7 Posted by: Ben_m Posted at: 2018-01-09T20:58:10.787Z Reads: 65

```
Ok, so the Focbox I'm testing with I have been using Vesc tool, I upgraded the FW to the latest 4.12 firmware in Vesc tool.  I'll try the virgin focbox with bldc tool.   Not that I think that will resolve the encoder detection but I do remember bldc tool shows the state of the hall inputs, which will help workout if the encoder signals are making it that far.
```

---
## \#8 Posted by: Ben_m Posted at: 2018-01-09T21:03:08.268Z Reads: 63

```
![20180103_155535|281x500](upload://63M0TtAIZLENpayeeRUE3GVBsAL.jpg)

We make the trolleys on the left, we are now designing the 'caddy' robot to drive under, pick up, and drive autonomously the trolley around. 
So currently it us just a fabricated aluminium chassis, with 2 hubmotor, 2 SLA batteries, 2 Focbox.
We have 3 cameras, 2 depth cameras, pc, li-ion battery, lifting mech, display.  to add.......
```

---
## \#9 Posted by: Ben_m Posted at: 2018-01-09T22:40:45.759Z Reads: 56

```
OK, using virgin FOCBOX, so default firmware, with BLDC Tool from Enertion website, error - this firmware version does not support Encoder. 

So anybody know where FW versions that are FOCBOX suitable available?O
```

---
## \#10 Posted by: scepterr Posted at: 2018-01-09T22:41:41.105Z Reads: 58

```
Oh...you didn't mention encoder error before
The error you're having is not related to vesc/bldc tool firmware mismatch

You can use any 4.12 compatible firmware
I don't know about the encoder support though

http://vedder.se/forums/viewtopic.php?t=728#p4301

> benjamin
Site Admin
Re: "Encoder support is not enabled"
Post17 May 2017, 11:38
Encoder support is enabled in the firmware by default and does not need any special compile any more. To use an encoder you need to choose the correct hall/encoder port mode on the advanced page.
```

---
## \#11 Posted by: notepad Posted at: 2018-01-09T23:08:31.438Z Reads: 56

```
Hey man.   for an updated tool go to http://vesc-project.com/vesc_tool   and get the free vesion,  its exactly the same as the generic bldc tool from enertion but its updated and more userfreindly.  just make sure to upload the correct Firmware to hardware configuration (4.12 hw)

wish you luck, im interested to see how this pans out.

edit: the original (blue version) is out of date, the free one isnt.
```

---
## \#12 Posted by: Ben_m Posted at: 2018-01-09T23:20:53.281Z Reads: 53

```
Thanks, I downloaded vesc tool free, yesterday, updated the firmware on one FOCBOX to FW3.34 latest available for HW4.12, built into the VESC tool. 
Everything is going smoothly except for failed encoder detection.
```

---
## \#13 Posted by: bayetan Posted at: 2019-09-06T23:52:50.850Z Reads: 13

```
Hello Ben_m,
Any luck getting the ABI encoder detection the work?
Thanks,
Ben
```

---
