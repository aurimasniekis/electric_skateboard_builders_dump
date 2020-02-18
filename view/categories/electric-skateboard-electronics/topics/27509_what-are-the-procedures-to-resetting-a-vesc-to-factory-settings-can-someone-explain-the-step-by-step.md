# What are the procedures to resetting a VESC to factory settings? Can someone explain the step by step?

### Replies: 22 Views: 1278

## \#1 Posted by: Tampaesk8er Posted at: 2017-07-13T11:27:27.755Z Reads: 104

```
Having major issues with VESC and 2.4ghz mini controller.
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-07-13T11:36:01.712Z Reads: 104

```
I don't know the procedure exactly so I won't comment on it. However if you post some screenshots of your settings someone might be able to help you salvage it without a re-install.
```

---
## \#3 Posted by: Tampaesk8er Posted at: 2017-07-13T11:39:51.221Z Reads: 100

```
I been having this issue about a week, i had given up on it, now i'm back trying to fix the issue.

1- After setting (binding) up my 2.4 mini controller over and over again, when I squeeze trigger to max and I put my board on the floor, it barely moves. when i lift board off the floor (cause no weight on it) and squeeze triggger the motor spins but has no coasting. 

2- When I release trigger, it slams the brakes.

3- I cant even set my controller in the display setting to 50% without squeezed trigger.<img src="/uploads/db1493/original/3X/8/a/8a206b75fc904671af7593f257a8be2fb6a7cead.JPG" width="669" height="499">
```

---
## \#4 Posted by: Tampaesk8er Posted at: 2017-07-13T11:44:39.290Z Reads: 92

```
Can someone please check all the boxes that are checked and the numbers see if i have them correct?
```

---
## \#5 Posted by: DeathCookies Posted at: 2017-07-13T11:48:59.206Z Reads: 92

```
To Setup your remote do the following:
1. disable the control mode
2. press the Trigger to full throttle
3. read the pulsewidth (down right) and insert this value in the number box of max pulsewidth
4. press the Trigger to full brake
5. repeat 3 with the min pulsewidth

When you release the remote (neutral Position) it should be about 50%.
```

---
## \#6 Posted by: Tampaesk8er Posted at: 2017-07-13T11:52:59.660Z Reads: 91

```
ive done the setup about 6 times already, i believe the issue is somewhere in the vesc settings, please look carefully at pic and look at all checked boxes (erpm, etc.) and numbers to make sure they are correct.
```

---
## \#7 Posted by: DeathCookies Posted at: 2017-07-13T12:04:52.566Z Reads: 87

```
Do you have a dual build? if not remove the check from "multiple escs over can""
The only number which seems uncorrect is the min pulse width but maybe it is the correct value.
```

---
## \#8 Posted by: Tampaesk8er Posted at: 2017-07-13T12:11:33.343Z Reads: 82

```
single build, for some reason, it doesnt let the controller go to 50% in pulsewidth (when not squeezed trigger, even when i turn the trimming button) setting and it also slams the brake when trigger is released, no coasting.

SO F****** frustrating, feel like just slamming board on floor, maybe it gets fixed, LoL.
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-07-13T12:44:18.775Z Reads: 77

```
That would cost you. But I feel the frustration. You may have done this already but it's worth mentioning. Have you rebound the remote to the receiver? Set all pots to center before binding? Then set it up again in bldc tool. Do you have a second remote you can try?

Off to work, hope this gets sorted.
```

---
## \#10 Posted by: Tampaesk8er Posted at: 2017-07-13T13:03:00.638Z Reads: 75

```
thanks, im scared to use the controller from my other board, dont want that controller to start acting weird, thinking of ordering another controller.
```

---
## \#11 Posted by: psychotiller Posted at: 2017-07-13T13:51:41.800Z Reads: 70

```
You should try binding your remote/receiver again like @i2oadsweepei2 said. make sure to center up your trim knobs first.
```

---
## \#12 Posted by: Tampaesk8er Posted at: 2017-07-13T13:58:31.678Z Reads: 64

```
ok, i'll try again. have to step out the house, i'll do it again when i get back.
```

---
## \#13 Posted by: Tampaesk8er Posted at: 2017-07-13T19:28:59.803Z Reads: 63

```
OK, finally got the controller going.

Now the problem is, when I squeeze the trigger to the max, i'm not getting full max. power at 100%. What can I do to have the full potential of power, my batteries are fully charged 6s 22.2v. CAN YOU CHECK MY SETTINGS PICS. AND SEE WHAT IS WRONG PLEASE? Thank you.<img src="/uploads/db1493/original/3X/d/2/d2a1aafa08823803ba9b5908da47b408bdd53409.JPG" width="669" height="499"><img src="/uploads/db1493/original/3X/3/2/326c435b6492bead679bbe8c710d5d8aa6953145.JPG" width="669" height="499">
```

---
## \#14 Posted by: psychotiller Posted at: 2017-07-13T20:57:51.238Z Reads: 55

```
Go up to the top of ppm and click disable, click write. Then adjust your min and max pulsewidths until you see the green readout at 50%. You have to click write everytime to see the result. once you're at 50%, click current no reverse with brake, click write and ride it.

You are at 56% so if you raise your max pulse width by like 5 points it will get closer.
```

---
## \#15 Posted by: evoheyax Posted at: 2017-07-13T21:48:52.916Z Reads: 50

```
I can see this has been solved to some degree already, but as for the original question for those looking for the answer, the easiest way I see is to re-flash your firmware with the BLDC tool... Simply select the defualt.bin file from the folder for your pcb version number (not the software version number), which for most is the hw_410_411_412 folder, and click upload. Give it 15 seconds or so to install and restart and you'll be good to go.
```

---
## \#16 Posted by: Tampaesk8er Posted at: 2017-07-14T20:59:22.051Z Reads: 42

```
Thank you, I did reflashed the firmware and it worked. Thankfully I had saved the files to flash and update firmware (4.10, 4.11, 4.12) on my pc. Everything is working again.
```

---
## \#17 Posted by: Tampaesk8er Posted at: 2017-07-14T21:02:16.468Z Reads: 46

```
Thank you to all who took time to share their knowledge, I hope this thread helps someone else with similar issues someday, I def. learned something new in this forum everyday, so greatful to be a part of this community, without it, we be lost. Thanks again. 👍👍👍👍
```

---
## \#18 Posted by: flaviuschris4 Posted at: 2018-04-19T18:08:56.638Z Reads: 29

```
how did you reflash the vesc??
```

---
## \#19 Posted by: flaviuschris4 Posted at: 2018-04-19T18:11:21.938Z Reads: 29

```
where do I select the default.bin?
```

---
## \#20 Posted by: Exiledd_Top Posted at: 2018-04-19T18:15:06.460Z Reads: 29

```
I'll pm u and help u
```

---
## \#21 Posted by: flaviuschris4 Posted at: 2018-04-19T18:15:22.983Z Reads: 29

```
ok thanks dude!
```

---
## \#22 Posted by: Exiledd_Top Posted at: 2018-04-19T20:13:35.362Z Reads: 22

```
[quote="flaviuschris4, post:21, topic:27509, full:true"]
ok thanks dude!
[/quote]

okay after 2 hours ish we seemed to have fixed the problem phase wires were touching
```

---
