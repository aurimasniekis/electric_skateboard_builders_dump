# Board cutting out under acceleration and (sometimes) braking

### Replies: 28 Views: 1073

## \#1 Posted by: Michaelj1 Posted at: 2018-05-17T02:42:54.028Z Reads: 160

```
So my board is doing this thing where when I accelerate it cuts out for a second. It used to just do it when I was really pushing it but it just did with when I was cruising. I have a GT2B remote, fully charged. I’m running dual VESC 4.12 on FW 3.38 in FOC mode with traction control. It’s really scary and I reallly wanna fix this because it’s annoying. I have dual 170kv sensored 6355 motors and 10s2p battery.
```

---
## \#2 Posted by: Michaelj1 Posted at: 2018-05-17T02:43:38.684Z Reads: 161

```
I also checked the vesc terminals on both VESCs and it’s saying there are no faults. Does this mean they’re rebooting?
```

---
## \#3 Posted by: Michaelj1 Posted at: 2018-05-17T13:17:58.965Z Reads: 134

```
Might have solved the issue, turned traction control off
```

---
## \#4 Posted by: Squidprorow Posted at: 2018-05-17T15:11:17.673Z Reads: 125

```
I am having a similar problem and I think it is related to my BMS cutting out when under too much load.
```

---
## \#5 Posted by: Scoo_B_SK8 Posted at: 2018-05-17T15:22:50.645Z Reads: 121

```
should screen shot your settings and post em, so we can look them over.
```

---
## \#6 Posted by: Michaelj1 Posted at: 2018-05-18T13:25:36.532Z Reads: 107

```
Update: seems to only be happening when the battery is fully charged. Any ideas? I can send a screenshot of that helps the Vesc’s are definitely rebooting because at one point my board stopped responding for like 3 whole seconds.
```

---
## \#7 Posted by: Michaelj1 Posted at: 2018-05-18T16:14:27.711Z Reads: 100

```
It seems to be really bad when the board has a full battery. This morning it cut out and stayed disconnected for over 3 seconds. My indicator stayed on though, which makes me think it’s either receiver or VESC related. I’ll send a screenshot when I have time. Based on what I’ve told you do u have any ideas?
```

---
## \#8 Posted by: Michaelj1 Posted at: 2018-05-18T16:31:16.516Z Reads: 99

```
So what should I do? Do I lower the battery max? The guy who sold me the battery said it can do 40 amps max discharge so I set the battery max to 20 amps per vesc. For the minimum I set it to -10 amps per vesc.
```

---
## \#9 Posted by: briman05 Posted at: 2018-05-18T17:46:34.369Z Reads: 94

```
Does it happen when you are braking as well?
```

---
## \#10 Posted by: Michaelj1 Posted at: 2018-05-18T17:48:23.409Z Reads: 91

```
It happened one time when I was braking kinda hard.
```

---
## \#11 Posted by: Michaelj1 Posted at: 2018-05-18T17:48:39.609Z Reads: 88

```
It’s mostly cutting out under acceleration though
```

---
## \#12 Posted by: briman05 Posted at: 2018-05-18T17:53:52.530Z Reads: 86

```
Well if it is happening when you are braking it could be that the batt regen is to high for a full charge.  If you post your settings that would help everyone try to figure it out
```

---
## \#13 Posted by: Michaelj1 Posted at: 2018-05-18T17:54:19.928Z Reads: 84

```
Sounds good. I’ll post them when I get home
```

---
## \#14 Posted by: professor_shartsis Posted at: 2018-05-18T18:09:53.521Z Reads: 83

```
please verify the absolute current limit setting is set well above the battery and motor current limit settings.
```

---
## \#15 Posted by: Michaelj1 Posted at: 2018-05-18T18:18:39.781Z Reads: 81

```
I’ll check them when I get home. I haven’t touched it but my motor max per motor is 60amps. Also with abs over current doesn’t it throw a fault? Or are there instances where it would cause the vesc to reboot?
```

---
## \#16 Posted by: professor_shartsis Posted at: 2018-05-18T18:20:50.473Z Reads: 80

```
my limited understanding is with 60a motor limit, the vesc will “try its best” to keep it under 60a motor— but if it “accidently” allows 61a motor for a split second, and you have your absolute limit set to 60a, this might possibly lead to a power cut-out.
```

---
## \#17 Posted by: Michaelj1 Posted at: 2018-05-18T18:26:00.557Z Reads: 74

```
I never messed with the absolute max amps setting so I’m assuming it’s whatever the default is, (I think it’s 130 amps?)
```

---
## \#18 Posted by: Ebisane9 Posted at: 2018-05-18T18:26:19.739Z Reads: 75

```
settings...post...please
```

---
## \#19 Posted by: professor_shartsis Posted at: 2018-05-18T21:19:28.719Z Reads: 72

```
you could also try bypassing the bms to determine whether the bms is responsible for causing the cutouts...
```

---
## \#20 Posted by: Michaelj1 Posted at: 2018-05-18T23:44:11.090Z Reads: 74

```
![image|690x388](upload://tdacB821vD8EGOWeC02iscFkoEK.png)
![image|690x388](upload://icvBRa5JPBgtD0PtTR3H9kytVcv.png)
![image|690x388](upload://gSoqH6exThbPpSUmqPGdoNvLS3z.png)
![image|690x388](upload://gN4fHwQ5GEsoL9padH4RRDxyre0.png)
![image|690x388](upload://j0Ufdi3lAI8I0MRiGOOu8kUAz1z.png)

let me know if you need a screenshot of anything else. i think ive narrowed it down to the connection between the board and remote as it showed up the further i walked away from the board. not 100% sure though.
```

---
## \#21 Posted by: Michaelj1 Posted at: 2018-05-19T00:33:16.948Z Reads: 69

```
My gt2b has a mod I got off ebay, can't remember the name of the mod lol, but I bought the case with screws here:

https://www.ebay.com/itm/GT2B-Electric-Skateboard-Controller-Housing-Case-Enclosure-BLACK/253470237462

I re-positioned the antenna so it sticks out of the remote's enclosure to see if that helps. I'll keep you guys posted
```

---
## \#22 Posted by: Michaelj1 Posted at: 2018-05-19T04:40:53.020Z Reads: 64

```
Hey guys I stuck the antenna outside of the gt2b enclosure and so far the cutouts are 100% gone. I’ll test on a fully charged battery but it surprised me that the gt2b was having connectivity issues🤔
```

---
## \#23 Posted by: Mikenopolis Posted at: 2018-05-19T05:31:56.489Z Reads: 65

```
That's weird. I have three boards using that remote and never had connectivity issues. You are not using anything carbon fiber right?

Also did you wrap that metal gold piece of the antenna in electrical tape? Maybe that was touching something inside and causing your cutouts?

I had an issue recently possibly due to using split ppm and dual receivers. Once I went canbus the problem went away

![image|690x387](upload://6RpvGjC73tKVjOk2bg3XAq2FcTS.jpeg)
```

---
## \#24 Posted by: Michaelj1 Posted at: 2018-05-19T05:48:55.844Z Reads: 65

```
Yeah it was in electrical tape lol I had the whole thing wrapped up. Might’ve been part of the issue
```

---
## \#25 Posted by: Michaelj1 Posted at: 2018-05-19T05:55:30.715Z Reads: 63

```
I basically just wrapped the wire up in electrical tape and it was pressing up agains the transmitter board with nothing to insulate it. I noticed there are some little contacts down there, and I’ll bet it was touching those. You might have just found the problem!
```

---
## \#26 Posted by: Michaelj1 Posted at: 2018-05-20T17:15:06.498Z Reads: 57

```
Thanks for the help guys, just did a full charge yesterday and no problems so far! I’ll keep you guys posted and I’m posting a build log later of all the different iterations I’ve gone through
```

---
## \#27 Posted by: Michaelj1 Posted at: 2018-10-16T14:03:59.395Z Reads: 34

```
Small update: the issue persists. Since then I have upgraded to the baby buffalo mod, which uses the gt2b’s steering pot instead of the throttle, and the failsafe is a little weird. I’m still having issues with this enclosure, I even bought a new remote and put in new internals and it’s still an issue. I made sure none of the antennas are shorting out against anything. Anyone ave any ideas?
```

---
## \#28 Posted by: Michaelj1 Posted at: 2018-10-16T14:15:47.715Z Reads: 34

```
Any help would be greatly appreciated, I’ve been dealing with this ever since I switched to the GT2B and I really wanna get to the bottom of it
```

---
