# VESC update issue

### Replies: 4 Views: 382

## \#1 Posted by: chrismccabe Posted at: 2018-07-21T09:03:23.920Z Reads: 73

```
Hey guys,

Probably I am forgetting something stupid here but don't seem to be able to update the firmware on my Maytech VESC.
It was shipped with 3.30 and I can't change the settings it in BLDC or VESC tool, it only allows for firmware update it says because of "too old version".
I tried to update it automatically with VESC tool. That seems to be doing something but eventually isn't successful after rebooting. Still the 3.30 version shows.

I also tried pulling the latest version from GitHub here:
https://github.com/vedderb/bldc/

Using the default for 410_o_411_o_412

And even though it says it uploaded the firmware it doesn't. Not sure what is happening here.

Update:
Using BLDC tool I get a timeout error on buffer erase. Is there a way to check if it is going into bootloader mode?
```

---
## \#2 Posted by: goldrabe Posted at: 2018-07-21T09:17:42.341Z Reads: 58

```
It´s likely there is no bootloader installed. My older Maytech Vesc´s came without bootloader, after installing it i was able to update the firmware.

Edit* With the new VescTool you are able to install the bootloader without the st-link connector.
```

---
## \#3 Posted by: trampa Posted at: 2018-07-21T09:35:47.741Z Reads: 54

```
On top of the FW update window you will find the bootloader tab. Simply upload the Bootloader for HW 410 411 412.

Frank
```

---
## \#4 Posted by: chrismccabe Posted at: 2018-07-21T09:43:34.172Z Reads: 48

```
You guys are AWESOME! That indeed was the problem. Strange, I was in doubt about it actually going into bootloader mode but it did say writing was successful even though it wasn't.
After updating it was giving me the next issues telling me I didn't have the latest version of VESC tool, but that was because I took the GitHub FW version which is 3.39 and doesn't seem compatible still with VESC tool 0.94. Managed to get the 3.38 going now.

Thanks again guys! :D
```

---
