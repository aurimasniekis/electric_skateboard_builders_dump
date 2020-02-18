# VESC no auto detection no motor spin up

### Replies: 12 Views: 2872

## \#1 Posted by: PeterAufAbwegen Posted at: 2015-10-07T13:24:44.067Z Reads: 174

```
Hey guys, I just finished soldering my VESC, sadly the auto detection doesn't work. The motor (SK3 213kv) doesn't spin up... I'm trying to fix the error, but there is no fault code in the terminal. Is there another way of debugging the VESC? Maybe someone had similar problems. I took two videos of the error.

https://www.youtube.com/watch?v=-8lobvuVLAI
https://www.youtube.com/watch?v=1cMLq5WUhPo



Thanks,
Peter
```

---
## \#2 Posted by: treenutter Posted at: 2015-10-07T14:30:09.104Z Reads: 165

```
@PeterAufAbwegen are you getting VESC to communicate w BDLC Tool in any other way? i.e. can you read your version of the firmware, or read\write configurations? If so, that eliminates a bunch of variables. I'd look at the connection to your motor if you can communicate with the VESC via BLDC Tool.
```

---
## \#3 Posted by: PeterAufAbwegen Posted at: 2015-10-07T17:08:05.075Z Reads: 163

```
Hi, jep I can connect the VESC, can upload the firmware and read and write configurations and also get realtime data. I just measured the 3 Motor Phases and they get voltage... I think the timing of the commutation is wrong..
```

---
## \#4 Posted by: sl33py Posted at: 2015-10-07T20:52:31.492Z Reads: 169

```
I would find another shorter USB cable (possibly with the built in filter/ferrites if possible) to test with.  I think Vedder cautioned long USB cable can cause issues.  Worth a shot to eliminate.
```

---
## \#5 Posted by: baxter Posted at: 2015-11-25T12:41:07.489Z Reads: 154

```


Hi, I'm having the same sort of problem.

I’m trying to use the Windows BLDC tool FW 1.14 for a vesc V4.10 that I recently bought from enertion.

I have downloaded and installed the VCP driver, before running the BLDC tool. 

I have plugged in the USB cable from the vesc to my PC, and ensured the vesc is powered up. I get the standard windows audible response that it is plugged in.

I dont think the BLDC tool is recognising the vesc when I click on the upper “Connect” button in the top right hand corner of the screen. In the bottom right hand corner of the BLDC tool it says "Connected” for three seconds before it gets replaced with “No firmware read response” highlighted in red.

According to my windows device manager I only have a single USB port number “COM1” (the vesc is not appearing in the device manager).

I have opened the firmware tab, and then clicked on the “Read firmware version” button and I get no response. I have also tried multiple USB cables to connect it to my PC.

I am fairly inexperienced with this sort of open source technology, and if anyone knows where I am going wrong, I’d appreciate your help.
```

---
## \#6 Posted by: locktight Posted at: 2015-11-25T12:50:02.758Z Reads: 145

```
Try other COMs. I know it only says you have one but my computer worked at COM7 and it only has 2 USB ports.
```

---
## \#7 Posted by: baxter Posted at: 2015-11-25T13:24:41.850Z Reads: 142

```
Thanks,  I have just tried everything from COM1 all the way to COM120. No luck.
```

---
## \#8 Posted by: cmatson Posted at: 2015-11-25T16:12:36.165Z Reads: 136

```
did you download the drivers for the BLDC tool?

there is a folder labeled "drivers" (or maybe it is "windows drivers"... I can't really remember) and there is a driver in that folder that you need to download.

Hope you get it all sorted out!
```

---
## \#9 Posted by: baxter Posted at: 2015-11-26T07:30:18.680Z Reads: 129

```
Yes, I've done that.  

[quote="baxter, post:5, topic:277"]
I have downloaded and installed the VCP driver, before running the BLDC tool.
[/quote]
```

---
## \#10 Posted by: cmatson Posted at: 2015-11-26T15:41:18.495Z Reads: 129

```
Sorry... guess I didn't see that. 

Have you read this thread and made sure your VESC was all set up correctly? (i.e. Using a power supply) I'm pretty much a noob to VESC stuff, so if this doesn't help at all, I'm sure someone else with more experience could chime in and help you solve this :smile: 

http://www.electric-skateboard.builders/t/vesc-faq-warning-handle-with-care-read-before-buying/491
```

---
## \#11 Posted by: Flo Posted at: 2016-02-07T18:44:15.939Z Reads: 109

```
I know that thread is pretty old already but was there a solution to that problem? I have a quite similar problem now... : 
http://www.electric-skateboard.builders/t/vesc-red-blinking-no-firmware-update-possible-no-motor-turn/1177/12
```

---
## \#12 Posted by: Pafrican Posted at: 2017-04-29T23:16:25.512Z Reads: 34

```
You are awesome! Fixed my issue
```

---
