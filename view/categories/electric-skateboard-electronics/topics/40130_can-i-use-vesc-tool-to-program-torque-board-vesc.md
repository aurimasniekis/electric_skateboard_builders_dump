# Can I use VESC tool to program torque board VESC?

### Replies: 9 Views: 1531

## \#1 Posted by: herojeanpierre Posted at: 2017-12-04T20:27:14.533Z Reads: 160

```
Hello! 

I was wondering if any of you have bought the [torque boards vesc](products/torque-esc-vesc-bldc-electronic-speed-controller) and used the [vesc tool](http://vesc-project.com/vesc_tool) to program it. 

Because on torque board site, it says it has the latest firmware  (v2.18 Firmware (Latest)), but the vesc tool offers another firmware update to 3.x

<img src="/uploads/db1493/original/3X/7/b/7b4353826689269670240f1ef92bed0c4d82be40.png" width="482" height="186">

Is it safe to update the firmware of this vesc using this vesc tool? 

This is a screenshot of the vesc tool for reference 
<img src="/uploads/db1493/original/3X/d/5/d51b7e44107a292d73e71f0e602169d941b9d853.png" width="690" height="390">
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-12-04T20:44:17.744Z Reads: 150

```
yes...

if you had used the search function you would know
```

---
## \#3 Posted by: Colson003 Posted at: 2017-12-04T20:46:40.220Z Reads: 151

```
Currently running mine on 3.34fw Sensoered FOC
```

---
## \#4 Posted by: lasplaner Posted at: 2017-12-04T20:46:58.917Z Reads: 149

```
There are multiple different firmware versions that you can use with the VESC.

You can totally use VESC Tool with **ANY** standard VESC, as the VESC 4.12 Hardware is compatible with Firmware 3.x. That means you can get any VESC from any vendor, as long as it is a standard version, you should be able to upload any version of the firmware available.

There are 3 main firmware versions you can upload to your VESC as of today.

1. **FW 2.18** - "Stock Standard" Firmware used with the **BLDC TOOL**. You should reinstall firmware if you get your VESC new. You should know how to do this.
2. **FW 2.54** - Ackmaniac Firmware, used with his **modified BLDC TOOL**. You can get it/install firmware here: (I would recommend this, many benefits)
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
3. **FW 3.x** - VESC TOOL firmware. You already know how to get this. Also has its benefits.

Quick note, you may want to be careful install firmwares, and make sure to upload the correct firmware with the Torque Boards VESC, or bad things will happen!

Good Luck!

-lasplaner
```

---
## \#5 Posted by: herojeanpierre Posted at: 2017-12-04T20:53:14.378Z Reads: 121

```
Awesome, I think I'll try 2.54. Thanks for the information!
```

---
## \#6 Posted by: herojeanpierre Posted at: 2017-12-05T03:01:00.506Z Reads: 110

```
For the torque board vesc would I select the 412 firmware in the vesc tool?
```

---
## \#7 Posted by: lasplaner Posted at: 2017-12-05T03:15:30.818Z Reads: 101

```
Look at your VESC board, and see if it says 4.12.
<img src="/uploads/db1493/original/3X/6/4/6487d27c2ae58d753563ed9e7a7688cf728880cb.png" width="521" height="499">

If it does, then yes. The firmware version should also 4.12 or 412 or whatever in the name.
```

---
## \#8 Posted by: herojeanpierre Posted at: 2017-12-05T03:42:37.881Z Reads: 94

```
Thanks, I know my questions are very simple. I'm just being cautious!
```

---
## \#10 Posted by: gee Posted at: 2019-02-12T15:12:23.099Z Reads: 16

```
So recently I use the VESC TOOL on my TorqueBoard vesc and I burned it so I wouldn't suggest anyone try this. ![IMG_2224|375x500](upload://wqKdbNjUtGLx856sHHE65iG5IF8.jpeg) ![IMG_2225|375x500](upload://jPBLbua0Exjgzmnl9qr0cSygI1k.jpeg)
```

---
