# VESC 6 not connecting to computer for setup

### Replies: 30 Views: 635

## \#1 Posted by: Dook Posted at: 2018-07-02T13:48:59.179Z Reads: 119

```
Hi Guys

Help needed.

Powered up my 2 Vedder VESC6's. I have a can bus cable linking them. I plugged in my USB cable from the VESC6 with a blue solid light, into my computer. The other VESC6 is flashing red (I'm guessing because this needs to be linked via the set up wizard)

When I start up the Vesctool wizard it cannot connect at all to the Vesc.

I have an old laptop running windows 7. I've tried several USB cables and it is not connecting at all.

I do have a MacBook but there is no Mac version on the VESC-project website so see if it is a computer issue.

The only thing I can think of is I have an old laptop but cannot see how that can be the issue.

I am totally stumped. Can anyone in Esk8 land help a brother out?

Cheers
```

---
## \#2 Posted by: rich Posted at: 2018-07-02T15:09:39.984Z Reads: 107

```
Did you try all your USB ports? On my laptop with windows7 only one port works with vesc. Also wait at least 1 Minute after connecting it for the first time BEFORE you start vesc-tool, otherwise the drivers are missing and vesc-tool can't connect. Did you read the vesc-tool tutorials on vesc-project.com?

Never connect CAN bus before everything is setup, that's the last step. If you power only one of 2 vescs when Can bus is connected then you probably blow the can bus chip.
```

---
## \#3 Posted by: Dook Posted at: 2018-07-02T15:32:02.815Z Reads: 98

```
Hi Rich, I downloaded the Mac version and all ok. But thanks for advice especially on connecting the CAN after set up and waiting 1 minute after connecting before starting the VESC tool. And yep, I've been reading up on tutorials. I think my windows computer is an old piece of c@ap hence a complete blank from VESC to laptop.
```

---
## \#4 Posted by: rich Posted at: 2018-07-02T16:00:35.484Z Reads: 100

```
Glad it's working now. 
I was talking about the USB cable connection. Windows take some time to install the driver for the very first time.

It's best to connect the CAN bus cable after programming both vescs.
```

---
## \#5 Posted by: Dook Posted at: 2018-07-02T20:52:00.512Z Reads: 84

```
I set up the first vesc with motor wizard no problem, FOC sensored. I went to do the same with the second vesc and got as far as the Motor flux linkage before I got this message

‘Could not measure the flux linkage properly. Adjust the start parameters according to the help text and try again.’

Any ideas? The wiring to the second VESC is the same as the first, with wiring from the motor and the usb cable plugged in. Although the second VESC is flashing red which the first one was not?

I sent this message to Frank at Trampa as well to see if he had any input.
```

---
## \#6 Posted by: Dook Posted at: 2018-07-02T21:06:39.312Z Reads: 75

```
![image|666x500](upload://hSF5XzswcxK4X09dhD6ZTTPJAwB.jpeg)

This is where I’m stuck at on setting up the second VESC and motor
```

---
## \#7 Posted by: wafflejock Posted at: 2018-07-02T21:09:52.932Z Reads: 69

```
Don't have any experience with FOC myself but did you try following the help steps under the first button?
```

---
## \#8 Posted by: Dook Posted at: 2018-07-02T21:14:04.700Z Reads: 69

```
yeah, it does say play around with settings but I have no idea about this stuff so I don't know what to charge it too.
```

---
## \#9 Posted by: wafflejock Posted at: 2018-07-02T21:16:30.848Z Reads: 69

```
Think it gives more specific steps if detection fails but understand the trepidation personally would wait to hear back from Frank/trampa since I've seen/heard of lots of issues with people blowing a second VESC over canbus from bad configuration.
```

---
## \#10 Posted by: Dook Posted at: 2018-07-02T21:19:21.007Z Reads: 65

```
yeah, I'm hoping I haven't blown it. Still have the flashing red light on it if that is of any positive note. but yeah, will se what Frank comes back with. cheers
```

---
## \#11 Posted by: banjaxxed Posted at: 2018-07-02T21:22:12.017Z Reads: 60

```
What version of windows? You may need drivers for sub-10
```

---
## \#12 Posted by: Dook Posted at: 2018-07-02T21:36:27.151Z Reads: 57

```
I'm running through my Mac now. Something is wrong with the VES as Ive looked on the manual. When it flashes red it says "fault code, something is wrong. Read out the fault code in VESC tool" but have no clue how to do this and can't find anything in the manuals
```

---
## \#13 Posted by: rich Posted at: 2018-07-02T21:37:53.890Z Reads: 57

```
AFAIK the worst thing which can happen is a blown CAN bus chip (if two vescs are connected via CAN bus but only 1 vesc is powered on) but not the whole vesc. Also this would not effect the motor detection. You could try another motor detection with the first motor to be sure it's not the second motor. Didn't read too much about the start parameters but people had success after changing the values.

But if the red flashing light is permanent then it's a fault code.
```

---
## \#14 Posted by: rich Posted at: 2018-07-02T21:40:57.187Z Reads: 55

```
[quote="Dook, post:12, topic:60702"]
Read out the fault code in VESC tool”
[/quote]

Easy, in the menu bar Terminal --> Print Faults
```

---
## \#15 Posted by: wafflejock Posted at: 2018-07-02T21:41:04.207Z Reads: 57

```
In the terminal tab/section in the vesc/bldc tool you can type 'faults' to see any issues the VESC has seen since boot up.
```

---
## \#16 Posted by: Dook Posted at: 2018-07-02T21:43:51.966Z Reads: 60

```
![image|666x500](upload://4XBzUsrI5e7CiwHMzwO4Our1HQC.jpeg)

Ok these are the results. What does this error mean?
```

---
## \#17 Posted by: wafflejock Posted at: 2018-07-02T21:49:44.929Z Reads: 60

```
MC is for 'motor configuration' just means any of the values you give it have been saved when it says write OK the bad detection result error is just the same thing you're seeing in the tab when trying to configure it so nothing major wrong there (aside from the lack of good detection).  If you see DRV_FAULT it's a bad sign that the DRV chip that opens/closes the gates for the MOSFETs to let power in/out of the motor has failed but so far just appears bad configuration values.
```

---
## \#18 Posted by: Dook Posted at: 2018-07-02T21:53:39.039Z Reads: 60

```
ok, so I read somewhere to use a shorter USB cable to solve the problem? and if not what else can I try?

and I'm still confused as to why the second VESC flashes red when plugged in to the power on start up, whilst the first VESC was fine with solid blue light.
```

---
## \#19 Posted by: wafflejock Posted at: 2018-07-02T21:59:41.053Z Reads: 61

```
Usually the USB cable thing is all or nothing, that is it will work and you can connect and read/write or you can't.  Regarding the FOC detection it could be related to cables hooked up between the ESC and motor to some degree since it's using those to drive and measure what's going on with the motor.   Actually since you have two of everything I'd try using the other motor with the VESC that isn't detecting properly and see if you can get it working (would also just keep them disconnected from each other until you know each VESC is working as expected).
```

---
## \#20 Posted by: Dook Posted at: 2018-07-02T22:02:23.606Z Reads: 61

```
Good idea. I'll switch over the VESC to the motor thats running fine. Will let you know what I come back with.
```

---
## \#21 Posted by: Battosaii Posted at: 2018-07-02T22:03:08.774Z Reads: 57

```
Yea my buddies old windows 7 laptop would not recognize the vesc he had to get a windows 10 laptop.

I have a mac book pro with dual boot OSX and Windows 10. I use windows for tuning my car with AEM EMS and for my Raptor tool since there is no Rator 2 tool for Mac
```

---
## \#22 Posted by: Dook Posted at: 2018-07-03T08:27:10.946Z Reads: 46

```
ok so its definitely the sensor wiring on the second motor.

Just spun the first motor with the second Vesc on motor wizard and it ran perfectly.

I am going to strip down the sensor reconnections I made on the second motor, check and redo them.

Thanks for the advice dude, Frank at Trampa was a lot of help too. Big shout out to him as well!
```

---
## \#23 Posted by: TarzanHBK Posted at: 2018-07-03T10:10:32.820Z Reads: 44

```
Just tagging @trampa here to take a look ;)
```

---
## \#24 Posted by: trampa Posted at: 2018-07-03T10:29:38.951Z Reads: 44

```
The VESCs have their pin assignment printed onto them, so it should be easy to re-map any motor sensor wires. Our motors are plug and play, other motors might need you to swap over cables. Using a needle you should be able to get the cables out of the plastic housing of your motor sensor connector.

Frank
```

---
## \#25 Posted by: Dook Posted at: 2018-07-03T11:32:49.826Z Reads: 39

```
Cheers dude
```

---
## \#26 Posted by: Dook Posted at: 2018-07-03T11:35:47.248Z Reads: 41

```
Ok so this is what I PM’d Frank with

Still getting FOC error message after remapping sensor wiring (bottom right hand of screen). 

Again as soon as I powered up VESC it was flashing red, butbwas fine when paired up against the first motor.

The only thing I cannot think of is the motor itself?

![image|375x500](upload://qT8CShhJl56oN6oPZuwKe88l9ei.jpeg)
```

---
## \#27 Posted by: Dook Posted at: 2018-07-03T11:57:46.352Z Reads: 41

```
looks like it is a problem with the motor itself. I tested both Vesc's against the motor ,and as soon as both powered up, they were flashing red and both recorded FOC errors during the Motor Wizard setup.

And both VESCS were tested with the other motor and they set up perfectly with this motor.

Contacting Alien APS as I type.\

So annoyed!
```

---
## \#28 Posted by: wafflejock Posted at: 2018-07-03T13:41:40.481Z Reads: 37

```
Glad you got it sorted out thanks for reporting back on how that went, let us know how aps handles it always good to know which vendors take care of it when things go wrong.
```

---
## \#29 Posted by: Dook Posted at: 2018-07-03T13:47:40.757Z Reads: 35

```
yep will do. cheers
```

---
## \#30 Posted by: Devilmycry Posted at: 2018-10-29T17:58:42.709Z Reads: 21

```
Hi
I’m starting testing different motor
And my last test for some motor .
I have some difficulty to do motor detection like the vesc tool told my : we can’t detect motor flux linkage
And tried 2 or 3 time for each motor for make it work
Any idea what happened ?
My wire for the sensor are ok I look everything match 
Thank you
```

---
