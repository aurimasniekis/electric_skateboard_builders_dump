# Urgent help needed please!

### Replies: 25 Views: 361

## \#1 Posted by: MrDGOrman Posted at: 2018-10-20T10:31:07.823Z Reads: 153

```
Hi everyone,

I'm meant to be going on a group ride today in London but my board has decided to stop working. Not sure why, but it's just unresponsive.

I start up the board and I get a solid blue light on my FOCBOX. I'm fairly sure this is meant to be blinking? I turn my remote on, it seems to connect like normal but the motor doesn't spin when I push the throttle forward. A red light blinks 3 times when I do this. Everything's connected as it should be but for some reason it's just not doing anything.

Thoughts? I'd still like to go on the ride today.

Fast responders with a solution get a free gift. Such gift is yet undecided :laughing: 

Thanks,
Daniel
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-20T10:53:23.435Z Reads: 145

```
have you got a bms in your system? Also what comes up when you type faults into terminal of the bldc tool?
```

---
## \#3 Posted by: MrDGOrman Posted at: 2018-10-20T11:03:46.091Z Reads: 139

```
Yes. I just installed one a few weeks ago. Worked fine before installing the BMS and worked fine after aswell.

I use the vesc project tool. How can I find out faults?
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-10-20T11:05:51.332Z Reads: 131

```
go to the terminal section and type "faults", then hit enter.

this may be an undervoltage issue. what battery do you have?
```

---
## \#5 Posted by: notepad Posted at: 2018-10-20T11:07:52.754Z Reads: 127

```
It might also be a DVR error, as its only happening when you activate the motor.  definitely look at the faults as it would tell you whats going wrong
```

---
## \#6 Posted by: MrDGOrman Posted at: 2018-10-20T11:09:33.522Z Reads: 123

```
Found the faults section. This has come up:

> The following faults were registered since start:
> 
> Fault            : FAULT_CODE_DRV
> Current          : -0.9
> Current filtered : -0.1
> Voltage          : 37.35
> Duty             : -0.003
> RPM              : -0.0
> Tacho            : 1
> Cycles running   : 2
> TIM duty         : -22
> TIM val samp     : 2
> TIM current samp : 4200
> TIM top          : 8400
> Comm step        : 0
> Temperature      : 25.06

Not sure what I'm looking at here!

Thanks,
Daniel
```

---
## \#7 Posted by: mynamesmatt Posted at: 2018-10-20T11:10:28.458Z Reads: 108

```
looks to me like one of your fets have cooked for some reason. right @notepad ?
```

---
## \#8 Posted by: notepad Posted at: 2018-10-20T11:12:12.991Z Reads: 107

```
definitely looks that way,  i would inspect the board just to make sure some debris isn't causing it to short,  if it is, its a quick fix,  if not your looking at a  repair job/ new vesc.
```

---
## \#9 Posted by: MrDGOrman Posted at: 2018-10-20T11:16:30.988Z Reads: 105

```
Okay. Well that sucks big time.

What should I look for? Which bit do you think could be at fault?

I can't seem to take a picture of the FOCBOX just yet. The site won't let me upload it
```

---
## \#10 Posted by: taz Posted at: 2018-10-20T11:18:38.253Z Reads: 102

```
Upload it at a picture sharing site and write the link here.
```

---
## \#11 Posted by: MrDGOrman Posted at: 2018-10-20T11:23:00.578Z Reads: 99

```
https://uploadir.com/u/1jyrw2oq

https://uploadir.com/u/0wx6jjvh

Those images don't seem to do it any justice. It makes it look like it's been sitting in a dirty puddle for weeks!
```

---
## \#12 Posted by: notepad Posted at: 2018-10-20T11:27:11.177Z Reads: 96

```

interesting.   (also the site is borked  for pictures at the moment)

can you get a closer look at the one circled in green.

as for the large object with the copper showing,  I dont remember if its supposed to have any showing - i.e it might be missing a bit of its shell, as if I remember its supposed to have a solid top piece.

as for the fets.  i cant truly make out but is that water damage/corrosion, or just left over flux?
https://prnt.sc/l89w39
https://prnt.sc/l89w9z
```

---
## \#13 Posted by: MrDGOrman Posted at: 2018-10-20T11:43:12.547Z Reads: 95

```
I've had a closer look at the copper ring does look like it's snapped off but i don't know how as it's never been out of the FOCBOX case before. The only time it was taken apart was do remove the bottom part of the case so I could attach it to my heat sink plate.

I've tried taking a close up picture of the one circled in green but I'm struggling to get my phone to focus on it.

The 2 silver bits you've highlighted (I take it these are the fets?) - I'm not sure if it's corrosion or not. I've given it a clean up with a tooth brush and they look the same as the others.
```

---
## \#14 Posted by: notepad Posted at: 2018-10-20T11:51:09.737Z Reads: 93

```
im putting my money on that copper coil.  I just took apart one of my spare focboxes(its a dead one (i uploaded the wrong firmware)) and it does indeed have a full top with no copper showing.  

pretty sure that component has caused these problems.
```

---
## \#15 Posted by: MrDGOrman Posted at: 2018-10-20T11:53:24.768Z Reads: 88

```
Is the entire thing meant t be covered or just the top? How could missing that part cause this problem? I'm not 100% on the workings of circuit boards etc
```

---
## \#16 Posted by: linsus Posted at: 2018-10-20T12:07:23.866Z Reads: 86

```
The copper thing :rofl: thats the inductor..Its a very vital part. The stuff thats broken off is ferrite. An inductive material that helps to create the magnetic field which stores energy. Well, thats the short verision of explaning it anyway. Its damaged, but my gut says that it should work anyway. Probably the DRV that is fried. 
If you had the plastic enclosure on all the time, I cant imagine how its been beaten up. Wonder if that was mounted damaged.. Its easy to replace however. Just two pads that needs to be desoldered. think its 38uH if im not misstaken.
```

---
## \#17 Posted by: MrDGOrman Posted at: 2018-10-20T12:13:27.767Z Reads: 81

```
My apologies linsus. I'm really not very good at the PCB side of things! I'll come up with nick names and you can decipher it :laughing:

It was first kept in the original box and then I purchased a heat sink so I undone the 3 screws and attached it to the heat sink straight away. The device worked so I had no need to investigate it further.

I'm fairly decent with a soldering iron. Where can I get the new fet(s) from? If I had instructions I'd be more than capable of following them I'm sure.

Thanks,
Daniel
```

---
## \#18 Posted by: linsus Posted at: 2018-10-20T12:20:58.603Z Reads: 82

```
Im not so sure the FETs are the issue, if you are familiar with how the FETs are connected you can find out if theyre fried or not with a multimeter. Look up the schematic for the vesc 4.12 on github. You should have a certain amount of resistance between the terminals. See if any of the fets gives you a value that differs from the others. 

If the drv is fried you need a hot air soldering gun. And a new DRV ofc. I usually shop from Mouser. 
either you shop some pare components there untill you reach free shipping, like a few MCUs, som extra FETs, few DRVs and you learn to repair the VESCs yourself. Or you send it to someone who can repair it for you. Think we have a few on the forum that still does that
```

---
## \#19 Posted by: MrDGOrman Posted at: 2018-10-20T12:27:29.316Z Reads: 83

```
Enertion have said I can purchase the extended warranty and they'll have a new one set out straight away. I might just do that and be done with it!

Unless of course someone is able to fix it for a couple bottles of beer :laughing:
```

---
## \#20 Posted by: TowerCrisis Posted at: 2018-10-20T13:48:24.138Z Reads: 72

```
I'd get the extended warranty and just have it done with
```

---
## \#21 Posted by: MrDGOrman Posted at: 2018-10-20T16:20:04.421Z Reads: 59

```
Yeah that's what I've done. So much easier. It was £50 GBP in the end so in the grand scheme of things it's a cheap price to pay to have it replaced
```

---
## \#22 Posted by: dareno Posted at: 2018-10-20T22:25:05.700Z Reads: 44

```
They did the same for me when I fried 2.  Good customer service.  FYI I had one also show exactly what yours is doing with the 3 red blinks and it was indeed the drv that was fried.
```

---
## \#23 Posted by: MrDGOrman Posted at: 2018-10-20T22:56:35.319Z Reads: 39

```
Fingers crossed nothing else is fried then. Can't imagine anything will be. I'm going to do some better water tightening to prevent water based damage aswell. Just incase and all!

How would a DRV chip fry?
```

---
## \#24 Posted by: dareno Posted at: 2018-10-20T23:13:02.508Z Reads: 38

```
Mine was a catastrophic battery short that the bms took the brunt of but fried the drv on the vesc.  
@b264 is the resident expert on all things water resisting / proofing. I'm sure if you ask him nicely he will point you in the right direction of some great products.
```

---
## \#25 Posted by: MrDGOrman Posted at: 2018-10-22T21:07:15.923Z Reads: 20

```
I'm getting the Hummie deck and enclosure so I'll be doing a complete redesign with better waterproofing in mind.

Any suggestions on waterproofing would be greatly appreciated though!
```

---
