# What does this mean? It&rsquo;s not saving the firmware update help please

### Replies: 30 Views: 374

## \#1 Posted by: Jcammarata4 Posted at: 2019-05-13T15:36:21.169Z Reads: 94

```
![20190513_113411|690x388](upload://xHffXj3HOs3mkYMM4UuFauXIh4q.jpeg)
```

---
## \#2 Posted by: pookybear Posted at: 2019-05-13T15:41:16.962Z Reads: 89

```
After a complete firmware upload, it does this. I believe this is normal. You have to wait at least 10 secs before you power off the board. Then you can turn it back on. It should be good to go after that.
```

---
## \#3 Posted by: Jcammarata4 Posted at: 2019-05-13T15:44:43.655Z Reads: 82

```
It says it's in limited mode also is this also an issue..also I have a maytec super vesc 50a.....and it's firmware is very 3.103......is that the version I need every time I plug this in it says my vesc needs update...and yes I am saving it correctly ive read over and o
Over the process...
```

---
## \#4 Posted by: pookybear Posted at: 2019-05-13T15:46:59.754Z Reads: 79

```
Oh. If it still tells you limited, then it didn't take the firmware. 

Redo it. Upload firmware. Once upload is complete. Wait 15 secs just to be safe. Power off. Meaning disconnect battery. Then turn it on. 

What hw do you have? 4.x? What tool version are you using?
```

---
## \#5 Posted by: Sn4pz Posted at: 2019-05-13T15:49:23.957Z Reads: 73

```
You know, I've been having issues saving my app config on my Maytech vescs as well. Same ones as yours.

Very odd 🤔🤔🤔🤔
```

---
## \#6 Posted by: Jcammarata4 Posted at: 2019-05-13T16:07:49.105Z Reads: 71

```
It's hardware very 4.10...one last quest. How do I get rid of the push to start option. It's a giant pain in the ass on a mountainboard and prior to replacing my motors ..it wasn't like this.....thx
```

---
## \#7 Posted by: Jcammarata4 Posted at: 2019-05-13T16:14:44.024Z Reads: 66

```
App ver. Is ackamaniac-esc tool 0.2
```

---
## \#8 Posted by: Jcammarata4 Posted at: 2019-05-13T16:19:14.686Z Reads: 63

```
Anyone know how to remove push to start or make its threshold way easier to get moving...the board never did this with original motor...it's a scramboard with new turning 6374 149kv 10s4p Samsung 25r 20a discharge 2500mah.....pleeeaaassseee
```

---
## \#9 Posted by: trampa Posted at: 2019-05-13T17:13:43.103Z Reads: 56

```
Use VESC-Tool and re-flash it. Upload the bootloader if it doesn't accept the Firmware update. 
Or use the SWD Prog feature if you have a second VESC based ESC to hand.
Interconnect SWD to SWD with 8cm short cables  (only io, clk and gnd) power up both ESCs and start VESC-Tool.
Connect to working VESC, open SWD PROG window, click connect, choose correct Hardware version and press upload to flash the other ESC with corresponding FW.
```

---
## \#10 Posted by: JensSjogren Posted at: 2019-05-13T17:15:51.960Z Reads: 52

```
You probably dont have the bootloader installed on the ESC, i had this problem with my flipsky 6.6's. Go to firmware page and you have a tab called bootloader. Install that and then you should be able to update firmware
```

---
## \#11 Posted by: Jcammarata4 Posted at: 2019-05-13T17:21:25.782Z Reads: 51

```
Ok so it won't destroy anything reinstalling bootloader ...may be silly question but the actual bootloader files to be loaded are already in the vesc tool....meaning I don't have to go find a bootloader...it's already there right .just gotta load it
```

---
## \#12 Posted by: Jcammarata4 Posted at: 2019-05-13T17:22:05.853Z Reads: 47

```
I'm sorry may be a dumb question but what's swd...a setting ?
```

---
## \#13 Posted by: trampa Posted at: 2019-05-13T17:24:46.911Z Reads: 46

```
Serial wire debug, the backdoor to the processor, straight access.
```

---
## \#14 Posted by: Jcammarata4 Posted at: 2019-05-13T17:25:04.488Z Reads: 45

```
And one last q....these vescs aren't new they previously had other motors connected but we're already running super well....so knowing that....should I still try and upload bootloader.......I think that was all ready done by the makers at scramboard
```

---
## \#15 Posted by: Jcammarata4 Posted at: 2019-05-13T17:25:57.478Z Reads: 46

```
Sorry kinda new at configuring vescs....
```

---
## \#16 Posted by: Jcammarata4 Posted at: 2019-05-13T17:27:37.992Z Reads: 44

```
Thank you trampa and Jen's for quick respnses. So helpful since im in the workshop doing this step by step asking questions 
...super helpful
```

---
## \#17 Posted by: trampa Posted at: 2019-05-13T17:29:10.035Z Reads: 41

```
Most VESC based ESCs feature a SWD port. If you mess things up, you can re-flash via SWD port using a second ESC as a programmer. Or you can buy a ST-Link V2 to do the job.
USB usually doesn't work if the software gets messed up.
```

---
## \#18 Posted by: Jcammarata4 Posted at: 2019-05-13T17:33:08.054Z Reads: 36

```
Is there a way to see if bootloader is installed ..will it show up in some window with version ...so can I see if it's there first b4....Shaking right now.....I'll litterally lose my mind bricking these.....haven't had a single issue in over a year...I replaced motors and thought I'd be easier but am happy to learn more....
```

---
## \#19 Posted by: Jcammarata4 Posted at: 2019-05-13T17:44:37.888Z Reads: 36

```
I may be wrong but these must have bootloader installed if they've been used already correct...when it was sent it was already dialed in...although to different motors..but the vescs must have had bootloader installed already from scramboards.....right ....I just saw the "you'll destroy your vesc if you try to install bootloader over another bootloader
```

---
## \#20 Posted by: trampa Posted at: 2019-05-13T17:52:45.377Z Reads: 36

```
It probably has no bootloader installed. If it doesn't update the FW, there is no bootloader installed. You can't destroy it, just mess up the software. This can be resolved by re- flashing via SWD.
```

---
## \#21 Posted by: Jcammarata4 Posted at: 2019-05-13T17:57:36.044Z Reads: 34

```
Confirmed firmware is 3.103 now ...and stable. It stuck. So now is it possible to eliminate push to start without having sensors.....that's how it was originally with scram motors ..which had no sensors....what's the setting called that'll reduce or eliminate the need to push off
```

---
## \#22 Posted by: trampa Posted at: 2019-05-13T18:03:31.536Z Reads: 32

```
3.103 is no official FW, but a forked FW. I would switch to original VESC Firmware if possible. Lots of things have changed in the recent time. Benjamin Vedder has coded like a Ninja.
```

---
## \#23 Posted by: Jcammarata4 Posted at: 2019-05-13T18:05:21.057Z Reads: 31

```
Ackamaniack version of software.....![15577706743062295773505243371546|690x388](upload://1Ury2Y2JUSdg3fBahEGB0aiOPkO.jpeg)
```

---
## \#24 Posted by: Jcammarata4 Posted at: 2019-05-13T18:32:37.837Z Reads: 31

```
Ok got fw ver3.56 loaded. To both vesc. Now that it's dialed in the fw. My ? Is still can I lose the kick to start b.s. I'm almost sure since previously without sensored motors it was that way ..never needed to push off it just went from standstill......does anyone know how this is achieveable...it's my last issue on list..
```

---
## \#25 Posted by: Jcammarata4 Posted at: 2019-05-13T18:48:40.871Z Reads: 32

```
![15577732986086114165909819209127|281x500](upload://xDbpgBcIffz5M27QFTvmrdC9Vh0.jpeg)
```

---
## \#26 Posted by: trampa Posted at: 2019-05-13T21:30:25.702Z Reads: 26

```
Without sensors, you have to accept that the motors cogg a bit on startup. There is a reason why everyone wants sensors.
```

---
## \#27 Posted by: mmaner Posted at: 2019-05-13T21:39:38.613Z Reads: 26

```
Increase the startup boost. It is entirely possible  to minimize cogging on a tuned setup without sensors. Litterally hundreds of people have done it.
```

---
## \#28 Posted by: pookybear Posted at: 2019-05-14T00:57:12.337Z Reads: 24

```
[quote="mmaner, post:27, topic:93704, full:true"]
Increase the startup boost. It is entirely possible to minimize cogging on a tuned setup without sensors. Litterally hundreds of people have done it.
[/quote]

Can this be used on FOC sensorless? I only read up about it on BLDC. Thanks!
```

---
## \#29 Posted by: mmaner Posted at: 2019-05-14T01:05:02.925Z Reads: 23

```
[quote="Jcammarata4, post:24, topic:93704"]
without sensored motors
[/quote]

I thought you were running bldc?
```

---
## \#30 Posted by: Jcammarata4 Posted at: 2019-05-14T08:39:52.501Z Reads: 15

```
No sir the original config was a scramboard build sensorless motors...don't know what the vesc was set to as it came ride ready ...no push to go....and had no issues for over a year til I banged up a motor. So I know that sensorless will run from dead stop no prob if setup right. I don't know much ...but that I do know. So I was really looking for someone to just translate electrical jargon to plain English so I could set up and tweak til it's right.........
someone ought to come up with a document that litterally translates the electric terms used into understandable and frankly more user friendly terms......as in.....motor min current= brake...or whatever.....seems someone with some experience could do this quick and easy...fir the major things...and would prob cut the time consuming question and answer waiting game to a min.....am I correct
```

---
