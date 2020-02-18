# How do you wire all these balance wires?

### Replies: 44 Views: 865

## \#1 Posted by: Gabegds2001 Posted at: 2018-11-08T00:36:13.139Z Reads: 173

```
So I've been looking all over the place on here and cannot find a single person with the same battery setup.  (4x3s batteries in series(12s)) I'm confused on how to wire it because there's 4 balance wires on each battery (4x4=16 balance wires) that have to be plugged into 12 wires from the bms. I know that b1 starts at the primary negative battery and b12 ends at the primary positive but that's it.. please help me. ![1541637310529233468156|374x500](upload://cB6yyRcQ7sZ5JduBOey86MSalzU.jpeg)
```

---
## \#2 Posted by: Devilmycry Posted at: 2018-11-08T06:16:59.417Z Reads: 143

```
For what i see 
You have to use balance changer with this battery 
No bms
```

---
## \#3 Posted by: J0ker3366 Posted at: 2018-11-08T06:35:55.052Z Reads: 140

```
[quote="Devilmycry, post:2, topic:73879"]
You have to use balance changer
[/quote]

Not true. I run 6x 2s1 lipos and charge them in a 6s config. That's 3 2s1 lipos in series in one charge. Ive also got a 10s that's 2 5s1 and it was ran through bms. 

Search the "beautiful wiring diagrams" thread. You'll find what youre looking for. You could also ask @Namasaki. He's the one that helped me with mine.

Also, the way you have your lipos wired looks like they are all in parellel and not series.
```

---
## \#4 Posted by: bigben Posted at: 2018-11-08T06:56:02.627Z Reads: 137

```
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
The bulk of the information you are looking for is contained here.
```

---
## \#5 Posted by: Devilmycry Posted at: 2018-11-08T07:02:58.718Z Reads: 123

```
Humm very interesting 
I have to look more at this lipo battery
```

---
## \#6 Posted by: longboardshort Posted at: 2018-11-08T07:22:07.721Z Reads: 116

```
It's not pretty but I drew a diagram for you. Hopefully you can make sense of it.![IMG_1389|640x480](upload://1PSNVaUOcpaYew2QmhqvCRdrgTs.jpeg)
```

---
## \#7 Posted by: Gabegds2001 Posted at: 2018-11-08T13:40:21.510Z Reads: 96

```
Nah they're series connectors and the primary connector is 44.4v
```

---
## \#8 Posted by: Gabegds2001 Posted at: 2018-11-08T13:42:42.038Z Reads: 96

```
Wow thanks! I've seen so many 12s bms diagrams but not with 4 3s batteries. This is exactly what I needed.
```

---
## \#9 Posted by: Gabegds2001 Posted at: 2018-11-09T22:09:01.800Z Reads: 82

```
![1541801237443837341574|375x500](upload://9u5fgO4ohm5LLelSQdDEEWEQflB.jpeg) Is this the correct wiring? I don't want to plug it in and blow it up. I haven't put the charge port in yet. The primary positive will have to be branched off to the positive of the charge port right? And the negative of the charge port to the c-?
```

---
## \#10 Posted by: Badgermilk Posted at: 2018-11-09T22:19:00.395Z Reads: 78

```
Looks wrong. All the BMS I've used don't have any contact for the positive leads. Just negative. What solder pad is that on the right side of the BMS that the wire is soldered to?
```

---
## \#11 Posted by: Badgermilk Posted at: 2018-11-09T22:20:47.799Z Reads: 76

```
It looks like the one on the right is the negative load output
```

---
## \#12 Posted by: Badgermilk Posted at: 2018-11-09T22:22:41.457Z Reads: 75

```
The wire soldered to the load output is your positive load wire and should go to the ESC.
```

---
## \#13 Posted by: Badgermilk Posted at: 2018-11-09T22:30:07.402Z Reads: 69

```
The primary positive will need to be branched to the positive charge port, and the c- will go to your negative charge port. Remove the primary positive from the board or you will destroy it.
```

---
## \#14 Posted by: Gabegds2001 Posted at: 2018-11-09T22:33:13.762Z Reads: 68

```
It's the p-. As far as I know ther are no positive wires connected to the bms
```

---
## \#15 Posted by: Badgermilk Posted at: 2018-11-09T22:38:29.126Z Reads: 67

```
Also make sure that all your white wires are connected like the picture above. If you are unsure use a volt meter. Each successive wire will be 3.6-4.2 ish volts higher than the previous one
```

---
## \#16 Posted by: Badgermilk Posted at: 2018-11-09T22:39:48.996Z Reads: 66

```
That big black wire is your positive for the battery pack. Remove it from the bms
```

---
## \#17 Posted by: Gabegds2001 Posted at: 2018-11-09T22:46:14.274Z Reads: 64

```
![15418032244241788593767|375x500](upload://ycrFPIIJdOvAGfEM84y8xNY5yU2.jpeg) ![15418032645281978431134|374x500](upload://xd9BNbfmFOTGkFAhq9j4pHkrJFM.jpeg) ![15418036638171804427241|375x500](upload://eAyiuQRu3rlxzcqSEoYppLB7MpA.jpeg) I think you are not seeing it correctly. The first two pictures show the female connectors that connect to another series connector to make 12s (4x3s.) The third picture is the last connector that will go to the esc and I have not yet wired the charge port into the red wire because I don't have it yet. As far as I know a positive wires never touches the bms.
```

---
## \#18 Posted by: Badgermilk Posted at: 2018-11-09T22:53:36.398Z Reads: 59

```
I see that now. You're all good
```

---
## \#19 Posted by: Gabegds2001 Posted at: 2018-11-10T20:22:09.415Z Reads: 56

```
![1541881165778257294527|375x500](upload://8LEB3fahk7pxezvtuElPjpIwNZt.jpeg) So I wired everything the way I think it's suppose to be wired and the esc doesn't get any power. When I plug the charger into the c- and the primary positive, (the red wire with the cut in it) the esc turns on. I'm so confused as to why the charger is powering the esc because b-,p-, and c- are all wired correctly (as far as I know) anyone know why it's not working? @Namasaki  @Badgermilk
```

---
## \#20 Posted by: pat.speed Posted at: 2018-11-10T21:32:32.606Z Reads: 54

```
I’m assuming the balance wires are ordered correctly? I would connect the multi meter to the b- and check the balance wire to make sure all voltages go up by 3.6 - 4.2v
```

---
## \#21 Posted by: Gabegds2001 Posted at: 2018-11-10T21:44:56.144Z Reads: 49

```
All of the voltages on the cells are correct, but the voltage drops about 3 volts from the total voltage when it goes through the bms. Primary positive and b- is 45.2 and primary positive and p- is 42.1... how does the bms draw that much?? Also, when I plug it in to the vesc nothing happens and the vesc voltage is 2.7-3 volts... I have no clue what's wrong. I've read that my vesc might not be capable of using a bms.
```

---
## \#22 Posted by: pat.speed Posted at: 2018-11-10T21:47:24.373Z Reads: 47

```
Your vesc can definitely use a bms what you’ve heard is nonsense. I would check the main connections, I had something like this the other day and it ended up being a cold solder joint in my b-
```

---
## \#23 Posted by: Gabegds2001 Posted at: 2018-11-10T21:48:42.443Z Reads: 48

```
Alright I will try re soldering the negative battery connections (b- and p-)
```

---
## \#24 Posted by: Badgermilk Posted at: 2018-11-10T21:59:58.154Z Reads: 45

```
How close we're all the cells voltages before you connected them to the BMS?  What was the difference between the highest cell voltage and the lowest in your 12 cells?
```

---
## \#25 Posted by: Badgermilk Posted at: 2018-11-10T22:00:44.347Z Reads: 42

```
Were not we're. Fing auto correct! L
```

---
## \#26 Posted by: Gabegds2001 Posted at: 2018-11-10T22:10:15.402Z Reads: 39

```
They were balance charged by my other lipo charger individually. They should all be about 3.85 volts.
```

---
## \#27 Posted by: Badgermilk Posted at: 2018-11-10T22:17:06.565Z Reads: 39

```
Good. It's weird that the P minus output is reading 42.1. It almost seems like a 10s BMS has gone into over-voltage protection and is bleeding off 3 volts.
```

---
## \#28 Posted by: Badgermilk Posted at: 2018-11-10T22:19:05.165Z Reads: 39

```
IDK. Even at 42v it should turn on your ESC.  You do have an anti spark switch right?
```

---
## \#29 Posted by: Gabegds2001 Posted at: 2018-11-10T22:21:28.552Z Reads: 40

```
The bms has an e-switch but it has no effect on whether the esc works or not. I have no clue what's wrong.
```

---
## \#30 Posted by: pat.speed Posted at: 2018-11-10T22:23:33.672Z Reads: 44

```
Have you tried charging, you need the eswitch on to charge
```

---
## \#31 Posted by: Gabegds2001 Posted at: 2018-11-10T22:55:32.859Z Reads: 45

```
Ok so I plugged in the charger and the vesc turns on and flipping the switch has no effect. The vesc stays on at all times and I'm pretty sure the vesc is being powered by the charger because when I unplug the charger it turns off. ![15418904015001858382445|375x500](upload://7dOpfo8DHChuENheB8J4xv3a9cu.jpeg)
```

---
## \#32 Posted by: pat.speed Posted at: 2018-11-10T23:04:47.906Z Reads: 41

```
So you have the vesc connected to P- and batt +. The charger connected to C- and batt +. And the battery connected to B-. 

If all that’s right well then I’m assuming that the bms might not be registering that the battery is connected. The reason the vesc gets powered by the charger is because the p- and c- are usually connected together. I would check the switch and make sure it is turning on the bms when charging/ discharging
```

---
## \#33 Posted by: pat.speed Posted at: 2018-11-10T23:08:24.416Z Reads: 40

```
Also if you have a multimeter check the continuity of the wires, they should read very low. That will let you know if there’s a bad connection
```

---
## \#34 Posted by: Gabegds2001 Posted at: 2018-11-10T23:23:45.073Z Reads: 36

```
So you're saying my wiring is wrong? If my vesc Powers up when the charger is plugged in, the way it is now, can I just switch the p- and the c-? Because right now that seems like it would make it work. The batteries are charging the way it is right now, but when you unplug the charger nothing can discharge the batteries
```

---
## \#35 Posted by: Namasaki Posted at: 2018-11-10T23:30:47.706Z Reads: 34

```
The charger will turn the Vesc on even if the bms is turned off. (that is normal)
If everything is wired correctly and there are no low cell voltages but bms is not outputting full voltage to the P-,
then the most likely problem is that the e-switch wires are either broken somewhere between the toggle switch and the circuit board or the solder connection of the e-switch wires to the circuit board is faulty so that the bms is not turning on when you flip the switch.

I have seen this problem with the e-switch wires before. I believe it is because of the stiff wire they use.
Also try connecting the e-switch wires together without the toggle switch to rule out the possibility of a faulty toggle switch.
```

---
## \#36 Posted by: Gabegds2001 Posted at: 2018-11-10T23:39:39.105Z Reads: 38

```
I understand what you're saying, but by the looks of the bottom of the switch wires on the circuit board there is nothing disrupting the connection to the switch. ![1541893044781104415844|375x500](upload://ta1buTG2YayEKIRSyTpGpFOF2iu.jpeg) [Uploading...]() The wires are covered in sugru type stuff so I can't really tell. I think after the batteries fully charge I'll check the connection by putting a wire between them. I checked the continuitity of the toggle switch and it isn't faulty.
```

---
## \#37 Posted by: Namasaki Posted at: 2018-11-11T00:01:29.842Z Reads: 35

```
There can be a break somewhere in one of the wires. This has happened before.
try disconnecting the wires from the toggle switch and check them with your continuity meter between the solder joint and the end of the wire and check each wire separately.
```

---
## \#38 Posted by: Gabegds2001 Posted at: 2018-11-11T02:09:43.156Z Reads: 31

```
The e-switch isn't messed up and my vesc seems to work now without the charger plugged in. I don't know what changed other than the charger changing the voltage of the batteries. Also, is the e-switch supposed to completely cut off power to the vesc or what Because for me it just lowers the voltage 6 volts. I think I'll just use a loop key in the battery wire to turn the board on and off completely Because from what I see the switch just lowers the voltage.
```

---
## \#39 Posted by: Sn4pz Posted at: 2018-11-11T02:12:13.387Z Reads: 32

```
yeah looks like your switch is a bit messed up

if you plan on doing the loop key yourself, do alot of research because ive seen some gems scattered about materials that you can use to strengthen the key, and other improvements to enable the switch to last longer and more predictably :)
```

---
## \#40 Posted by: Gabegds2001 Posted at: 2018-11-11T03:02:43.010Z Reads: 31

```
So I unplugged the 4 batteries from the bms to measure their cell voltages and the 1st battery (the primary positive battery) had 12.7 volts and the other three had 12.1/.3 volts. It might be unbalanced because I was charging it and i didn't give it time to balance them but I'm not sure. Is it because the first battery is getting the charge first?
```

---
## \#41 Posted by: Sn4pz Posted at: 2018-11-11T12:00:16.593Z Reads: 29

```
I'm not exactly sure, so I csnt answer for sure. Sorry.

The way I thought it worked was that the voltage would disperse evenly across the p groups

Were the batteries balanced before you connected them to the battery?
```

---
## \#42 Posted by: Gabegds2001 Posted at: 2018-11-11T12:40:31.050Z Reads: 27

```
I have a balance charger I used before I got a bms and I charged them all to about 70%
```

---
## \#43 Posted by: Sn4pz Posted at: 2018-11-11T12:46:11.361Z Reads: 29

```
Unfortunately that means they're likely unbalanced. Balancing during charging happens during the later part of the charging period, once batteries are mostly full. 


Sounds like the bms isn't the issue, and speaking from experience, it's only bad to keep poking around with the shit that works 😂😂

Focus on the loop key for now, maybe that will fix your problem
```

---
## \#44 Posted by: Gabegds2001 Posted at: 2018-11-11T13:20:15.792Z Reads: 25

```
Yea I was just gonna do that because the switch isn't fully turning the vesc off. I don't want the batteries to drain all the time.
```

---
