# My new VESC just went bang

### Replies: 16 Views: 896

## \#1 Posted by: Gabegds2001 Posted at: 2017-12-27T01:18:29.376Z Reads: 190

```
I just bought a 12s VESC from  I have a 6s 5000mah 60c Zippy Compact battery and a now fried 149kv Turnigy Aerodrive SK3.... I connected the VESC to my computer with the BLDC Tool that i downloaded from  . I configured everything as the Tutorial on their site told me to.. Everthing was fine but the throttle response made the board un-rideable. I tried changing all the values that were supposed to make it slow down a little but they didnt work. I went through some forums and found a guy that made his own firmware for VESCs like mine. His name is @Ackmaniac. I downloaded his software that was a modified BLDC tool like the one i was using. The modification was watt control but i couldn't use the full extent of the software because my firmware was "Outdated" I had v2.18 firmware previously but i went ahead and uploaded what i thought was v2.18 software from the modified tool. I thought that i might have recieved the VESC with old firmware. After that, it reset all of my values so i changed them to their old values and after that i started doing all of these tests like i had before. After i clicked the R and L test i heard a strange beep from my motor and then a pop from my VESC. I saw smoke so i unplugged my battery as soon as i could. Here are some pictures of the aftermath.<img src="/uploads/db1493/original/3X/0/a/0ae85abb8adf9b4f788b6d1b06fd822fd5e31332.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/c/a/caeb7beec802ad86a1000bbcbe6d9efdfd85ae58.jpg" width="375" height="500"> Obviously i cant troubleshoot because the soldered connections melted. I wonder if the Soldering was faulty on arrival. The vesc doesn't have a warranty either. 
If anyone is experienced with fixing these kinds of issues please message me.
Any help or info is helpful. Please and Thank you.        Update: I took off the three wires that connect to the motor and it turns out that the Vesc was just making the motor stay still while it wasnt plugged into a battery. That makes me feel better!             Update 2: i sent my vesc to kevin in Florida. I also bought another identical battery for parallel and I understand that I should buy them at the same time but I noticed that next to each other the batteries vary in size... <img src="/uploads/db1493/original/3X/d/a/daf95ad2039a89ebe92513f547b6b30ef1878b5e.jpg" width="375" height="500"> The top battery is the old one. It's been used probably about 20 cycles. (Zippy compact 6s 5000mah 60c) Is it safe to use these batteries in parallel? 😥
```

---
## \#2 Posted by: emepror Posted at: 2017-12-27T01:26:04.433Z Reads: 170

```
Can you try and get as clear as possible a photo of both sides? Looks like one of the shunt resistors nearly blew off, there's a possibility something was shorted beforehand which would cause that.
```

---
## \#3 Posted by: Gabegds2001 Posted at: 2017-12-27T01:50:13.886Z Reads: 158

```
This is as clear a picture i can get on my phone. If necessary i will get out my dlr.
<img src="/uploads/db1493/original/3X/b/9/b935a754010e29408a1b3f533a53897ceef0dcc0.jpg" width="666" height="499"><img src="/uploads/db1493/original/3X/c/a/caeb7beec802ad86a1000bbcbe6d9efdfd85ae58.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/7/771959690dbdcb23ac2d2aeabd562d6d531fa5c7.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/a/2a6cc236750b3011a500015758781f1c2253f6c4.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/a/0ae85abb8adf9b4f788b6d1b06fd822fd5e31332.jpg" width="374" height="500">
```

---
## \#4 Posted by: banjaxxed Posted at: 2017-12-27T04:03:40.122Z Reads: 123

```
Probably the problem
[quote="Gabegds2001, post:1, topic:41962"]
so i changed them to their old values
[/quote]

Also you can download the firmware bin file separately if confused, first you flash then when reconnected don't change back to old values, do read sequence of tasks @Ackmaniac has in post #1
```

---
## \#5 Posted by: DEEIF Posted at: 2017-12-27T04:21:25.503Z Reads: 120

```
@GrecoMan
10 char
```

---
## \#6 Posted by: Eboosted Posted at: 2017-12-27T05:24:25.723Z Reads: 106

```
The solder was not melted.

You need to run BLDC not FOC,its much safer for the VESC. 

I've been runing 1.5 years on BLDC on that same vesc.
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2017-12-27T05:48:48.079Z Reads: 101

```
Are you sure your motor is fried? Motors are pretty hard to fry.
You should contact Dexter and see if he can do anything for you
```

---
## \#8 Posted by: Gabegds2001 Posted at: 2017-12-27T08:47:13.902Z Reads: 88

```
The reason I think it's fried/ruined is because when I turn it it is very hard to turn. And I think the short ruined the magnets.
```

---
## \#9 Posted by: ARetardedPillow Posted at: 2017-12-27T08:49:34.833Z Reads: 88

```
Sounds like youve shorted the phase wires, make sure theyre not touching, you cant ruin the magnets unless you heat them up to like 150c or break them lol
```

---
## \#10 Posted by: Fabar Posted at: 2017-12-27T08:51:41.707Z Reads: 87

```
are you using Ackmaniac in that board?
```

---
## \#11 Posted by: Gabegds2001 Posted at: 2017-12-27T08:51:44.487Z Reads: 87

```
Ok I'll check that. Thanks.
```

---
## \#12 Posted by: Gabegds2001 Posted at: 2017-12-27T08:54:48.009Z Reads: 87

```
Before the vesc fried I was using a regular bldc tool I downloaded from  and after I kept falling off the board because of throttle being too sensitive I looked up how to make the motor accelerate slower and ended up using his software.
```

---
## \#13 Posted by: banjaxxed Posted at: 2017-12-27T12:58:19.960Z Reads: 77

```


One of the fets looks damaged and you need to clean your nails other than that I would imagine the vesc is fried not the motor, if the motor does not turn in a consistent way you're going to have to open to see why not, if you changed the m4 bolts make sure they aren't too long
```

---
## \#14 Posted by: Gabegds2001 Posted at: 2017-12-27T16:43:13.661Z Reads: 60

```
Ok thanks ill get my nails fixed. lol
```

---
## \#15 Posted by: evoheyax Posted at: 2017-12-27T16:52:02.121Z Reads: 59

```
If you disconnect the motor from the vesc, and it's hard to spin, your motor has a short in the phase wires. If you leave the motor connected to the vesc and have resistance, it could just be the vesc causing the motor to feel stiff.

As for the vesc, if you heard a pop, it's usually fried. Send it to the drv wizard @JohnnyMeduse! He'll fix it up!
```

---
## \#16 Posted by: Gabegds2001 Posted at: 2017-12-27T16:54:20.183Z Reads: 57

```
Thanks for the help. Im currently trying to get in contact with this repair guy in Florida.
```

---
