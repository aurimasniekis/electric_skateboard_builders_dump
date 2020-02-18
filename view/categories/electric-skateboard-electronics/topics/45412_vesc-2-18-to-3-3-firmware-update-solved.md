# VESC 2.18 to 3.3 firmware update *SOLVED*

### Replies: 5 Views: 1340

## \#1 Posted by: goldrabe Posted at: 2018-02-03T03:28:27.041Z Reads: 167

```
Hi builders,

i am trying to update my Maytech 4.12´s Vesc with the VESCTool. The current firmware is 2.18 if i connect the VESC the software says firmware is too old but boot-loader is detected please update the firmware.
If i do this, it does it´s thing and i wait the appropriate time, but after reconnecting the VESC it still says old firmware and after checking with the old BLDC tool it says still 2.18 firmware.
Does anyone know´s what i am doing wrong?
Help please.
And sorry yes, i used the search bar but could not find anything.

Thanks!!

*SOLUTION*

The solution was, that the Maytech VESC´S came without the bootloader installed. The Vesc Tool gives you false positives regarding a installed bootloader. Installing the bootloader is so easy now, you can just do it via USB cable.

Anyways thanks to everyone trying to help me!!
```

---
## \#2 Posted by: kyletrainy Posted at: 2018-02-03T04:11:16.401Z Reads: 153

```
How did you go about updating the firmware? Did it give you the screen where it allows you to choose hw version 4.10/4.12 and then you could click on the firmware version?
```

---
## \#3 Posted by: goldrabe Posted at: 2018-02-03T04:29:59.624Z Reads: 143

```
Thanks for your help!

Yes i choose 4.10 4.11 4.12 and then the bin file, after that the green bar advances to 100% and the VESC disconnects, then i wait and nothing happens. To reconnect the VESC i have to power off and on again.
```

---
## \#4 Posted by: kyletrainy Posted at: 2018-02-03T04:52:59.116Z Reads: 130

```
That’s weird because I’m pretty sure the vesc should disconnect and automatically reconnect after a couple seconds. Try a different usb cable and see it that changes anything otherwise I think you should switch to ackmaniacs extended bldc tool and use his firmware or go back to the original bldc tool with 2.18 fw
```

---
## \#5 Posted by: goldrabe Posted at: 2018-02-03T05:00:41.020Z Reads: 124

```
Thank´s man!!
I tried already two cables... will try further!
The strange thing is that the tool doesn´t show VESC COM 05, it only shows COM 05.
I opened the tool as administrator, shut off the virus protection all to no avail.
Thanks anyways the motors are spinning with the old firmware too, so not a big deal!
```

---
