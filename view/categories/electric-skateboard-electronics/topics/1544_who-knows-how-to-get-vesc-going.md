# Who knows how to get vesc going?

### Replies: 9 Views: 1188

## \#1 Posted by: Hummie Posted at: 2016-02-26T01:06:00.317Z Reads: 80

```
I had it going but sent it to chaka to make sure it wasnt damaged when i shorted the motor.  I cant get it to connect to the bldc tool now.  These are his instructions but im still not sure what to do:     

You have version 2.15 fimware on those now. You can you use the bootloader to revert back to whatever version bldc-tool you are using, just be sure to install the correct version for 4.10 hardware.
```

---
## \#2 Posted by: evoheyax Posted at: 2016-02-26T01:30:22.501Z Reads: 78

```
What are you seeing right now when you plug it into your computer and supply power to the VESC?

Do you not see the option in the bldc tool to connect to it?

Are you getting any lights?

Are you using the battery (if so, what battery) to configure or are you using a regulated power supply?

Do you know what version of the bldc tool you are using?
```

---
## \#3 Posted by: Hummie Posted at: 2016-02-26T03:31:33.588Z Reads: 71

```
I'm using 50 volts😬  with my battery.  I do have a power source that maybe could go down to 44 but didn't bother trying. Come to think of it I have a laptop charger that would probably work if I added a plug.  But I'm not worried about that now

 It comes on as usual with the blinking lights.  I can't get it to connect to the bldc tool.  The option is there though and when I try it will make the vesc blink again which is encouraging.  I don't know names of things but I'm thinking the bldc program isn't a match to the vescs and needs to be. I can download it or revert back to the old program.  I think. But I'd like to hear from someone the details 
  I have a feeling this is simple but want to hear I'm not going to screw it up. 
I don't know what bootloading is either and what to do in practical terms.  Chaka's message is straight forward and someone who knows these terms hopefully can tell me what to do.
```

---
## \#4 Posted by: onloop Posted at: 2016-02-26T03:54:04.430Z Reads: 66

```
what OS are you using?
Are the drivers installed?
What port is the VESC connected to?
have you tried another USB cable?
have you tried another computer?
Have you tried another BLDC version?
```

---
## \#5 Posted by: Hummie Posted at: 2016-02-26T04:05:35.987Z Reads: 62

```
Windows
It was going earlier do I have to instal again
Using the mini usb as before.  
...I think the answer is in what Chaka wrote me.  I think I just need to download a new bldc program or else update the vescs.  I think
```

---
## \#6 Posted by: evoheyax Posted at: 2016-02-26T05:29:42.122Z Reads: 57

```
When I first booted up my vescs from @onloop, they has 1.14 firmware. I was using bldc tool which only supported 2.15, so when I plugged it in and used the tool, I got a warning that I can't change any settings till updating the firmware. I did that for both of my vescs, then I was able to edit the settings. It should still be able to connect, regardless of firmware/bldc version by my understanding.
```

---
## \#7 Posted by: elkick Posted at: 2016-02-26T09:24:43.402Z Reads: 48

```
Just use an other com port in the field above the "connect" button and it will connect. From there you could do the updates in the firmware tab on top, but make sure to use the "default.bin" firmware in the "410_411"-folder, and nothing else, else you will kill your VESC.
```

---
## \#8 Posted by: Hummie Posted at: 2016-02-26T17:29:53.561Z Reads: 42

```
Id had to change to com4 instead of the com3 to get it going before but that won't do it now
Maybe just write com5?  I'll be trying again today.
```

---
## \#9 Posted by: elkick Posted at: 2016-02-26T17:32:45.608Z Reads: 41

```
Installing BLDC again? Those windows drivers are crazy, I even now people using com7 or com8. Mac or Ubuntu is much easier though...
Just step through up to 10.
```

---
