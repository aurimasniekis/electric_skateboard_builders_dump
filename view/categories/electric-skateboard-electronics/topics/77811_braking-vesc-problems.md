# Braking /// vesc problems

### Replies: 32 Views: 748

## \#1 Posted by: xeroxgame Posted at: 2018-12-12T16:59:01.603Z Reads: 147

```
Hey guys! I've almost finished building my longboard, but the brakes doesn't work well for me. I have Flipsky 50a vesc and i don't know how to make it, to make braking (by pulling the throttle down) less sensentive , because i fell of  the board every time when I'm trying to brake. Thanks for taking your time!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-12T17:19:22.153Z Reads: 145

```
Probably wrong settings in the vesc tool.
Post your motor and battery max/min settings please.
```

---
## \#3 Posted by: xeroxgame Posted at: 2018-12-12T18:07:20.195Z Reads: 135

```
![1111|690x404](upload://g0mIM5GR0Mq4WOevbVW37VdkeRK.png)  If it's important, i am using 2x 5s 5Ah batteries connected in series and my motor is 190kV 6374 3250W
```

---
## \#4 Posted by: mmaner Posted at: 2018-12-12T18:09:56.634Z Reads: 125

```
Move motor current max brake to around -20 and try it again.  Most of the time you just have to get it dialed in.
```

---
## \#5 Posted by: xeroxgame Posted at: 2018-12-12T18:12:45.954Z Reads: 126

```
A big thank you! And btw, is using FOC correct for my setup?
```

---
## \#7 Posted by: mmaner Posted at: 2018-12-12T18:43:45.024Z Reads: 116

```
You have confused me, but I think this statement...

[quote="Andy87, post:6, topic:77811"]
In general, so deeper the value the stronger the breaks. Means with bat min to -20 the breaks will become stronger.
[/quote]

Is incorrect.

Here's my reasoning.

Motor Min Regen or Motor Current Max Brake controls brake force at mid to low speeds.  This max value is the max amps the motor can handle.  Lets assume that in this case the max amps are 60a.  So max regen amperage would be -60a.  If you lower that value to -30, then you are in effect applying half of the total braking force, or max regen amps.  

Does that sound correct to you?
```

---
## \#8 Posted by: mmaner Posted at: 2018-12-12T18:44:22.212Z Reads: 106

```
I would not start with FOC, its dangerous to the VESC.  I would start with BLDC and get some experience there first.
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-12-12T19:00:19.481Z Reads: 108

```
[quote="mmaner, post:7, topic:77811"]
Motor Min Regen or Motor Current Max Brake controls brake force at mid to low speeds. This max value is the max amps the motor can handle. Lets assume that in this case the max amps are 60a. So max regen amperage would be -60a. If you lower that value to -30, then you are in effect applying half of the total braking force, or max regen amps.
[/quote]

Your motor amps depend on duty (voltage, speed) if you at full duty (full speed) the maximum current is basically your max battery negative and it scales based on duty so if you have -10A on battery at slow speeds your brakes with -60A will be strong the time you reach higher speeds your brakes will suck.

Here is a small graphs to imagine how motor/bat currents work regarding duty :)

This how looks motor 130A and 60A battery at 12S :slight_smile: Y axis maximum current at X axis is duty cycle :slight_smile:

![image](https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/0/306dcf298d8b06bbb88cb59928ff7690dc679224.jpeg)

Just to see that motor current depends on battery current its 130A motor 20A bat (This is more the case with his issues)

![image](https://www.electric-skateboard.builders/uploads/db1493/original/3X/b/5/b586847577865f3de39c55d205b7dc216291d643.jpeg)
```

---
## \#10 Posted by: xeroxgame Posted at: 2018-12-12T19:27:53.367Z Reads: 95

```
Ok, I don't understand much of this (I'm 14 yo) but so far I understood to change from FOC to BLDC and to change my motor max brake to -10 A. Did i get everything right? But now motor doesn't react to remote ( vesc is plugged off from the pc, red light stays solid both on reciever and remote, averything is plugged in, i can control motor by vesc tool) how do i fix it?)
```

---
## \#11 Posted by: briman05 Posted at: 2018-12-12T19:32:58.962Z Reads: 90

```
No @mmaner said -20.  You have to write everything and you also have to select the ppm current with brake no reverse and calibrate your remote so if you give it the beans it is it is going to start to hall ass and full brake will act like full break.  What motor are you using because if your are using a 50a vesc and single drive your 85A will be to much and could damage your vesc if I'm understanding it right.
```

---
## \#12 Posted by: xeroxgame Posted at: 2018-12-12T19:35:20.004Z Reads: 88

```
Yes my vesc is 50a. My motor is 6374 3250w 190kV https://flipsky.net/products/flipsky-electric-skateboard-motor-r-6374-190kv-3250w
```

---
## \#13 Posted by: mmaner Posted at: 2018-12-12T19:36:40.438Z Reads: 86

```
just set it at -20 and see if its better, then adjust from there.
```

---
## \#14 Posted by: xeroxgame Posted at: 2018-12-12T19:40:05.413Z Reads: 81

```
ok, but as i mentioned earlier, motor is not reacting to remote and @briman05 on my vesc there's an information "50A - 240A" Then i guess i am ok?
```

---
## \#15 Posted by: briman05 Posted at: 2018-12-12T19:42:57.901Z Reads: 82

```
240a is peak the 50a is continuous
```

---
## \#16 Posted by: xeroxgame Posted at: 2018-12-12T19:48:14.567Z Reads: 81

```
ok, then i'll change it to 50A
```

---
## \#17 Posted by: xeroxgame Posted at: 2018-12-12T19:56:21.818Z Reads: 78

```
any ideas what can i do to make my remote working agian?
```

---
## \#18 Posted by: briman05 Posted at: 2018-12-12T19:58:52.248Z Reads: 79

```
go into the ppm tab  after you have done a motor detection and select current with brake no reverse.  set your pulse width and then write to the vesc
```

---
## \#19 Posted by: xeroxgame Posted at: 2018-12-12T20:08:36.396Z Reads: 78

```
now even vesc tool can't detect throttle changes , and by write to the vesc, you mean "apply"?
```

---
## \#20 Posted by: xeroxgame Posted at: 2018-12-12T20:14:57.331Z Reads: 79

```
god, unexpectedly motor started spinning, i turned eveything off and now as i turned on the remote it's as it was earlier ( nothing reacts to remote)
```

---
## \#21 Posted by: briman05 Posted at: 2018-12-12T20:47:26.479Z Reads: 79

```
https://www.youtube.com/watch?v=5HLZaMcYRuY

watch this video it explains everything very well.
```

---
## \#22 Posted by: xeroxgame Posted at: 2018-12-13T17:49:22.394Z Reads: 67

```
God, I think I broke my motor. On this video i am trying to move it using arrows on my keyboard but it does that sound. How bad does it sound?

https://youtu.be/xRM8nOzCQak
```

---
## \#23 Posted by: StefanMe Posted at: 2018-12-14T04:54:33.659Z Reads: 60

```
That’s normal for me... 😂 don’t use the keyboard... try with remote after switch off and on everything. Mine makes the same sound with the keyboard.
```

---
## \#24 Posted by: briman05 Posted at: 2018-12-14T05:40:05.319Z Reads: 55

```
Did you do a motor detection?
```

---
## \#25 Posted by: xeroxgame Posted at: 2018-12-18T13:37:30.105Z Reads: 50

```
I did motor detection and all sort of stuff, vesc doesn't react to remote even after turning off and on. Beforehand it worked, with remote and arrow keys. Light on vesc is solid, now i think that vesc is broken, because i think motor is quite hard to break
```

---
## \#26 Posted by: briman05 Posted at: 2018-12-18T13:45:42.802Z Reads: 51

```
Did you have then belt on when you did the detection. Take the belt off and try spinning it with the arrow keys.
```

---
## \#27 Posted by: xeroxgame Posted at: 2018-12-18T16:43:07.827Z Reads: 45

```
I'll try that tomowrrow (today i don't have acces to screwdriver
```

---
## \#28 Posted by: briman05 Posted at: 2018-12-18T16:54:50.429Z Reads: 42

```
You are making a diy board without basic tools
```

---
## \#29 Posted by: xeroxgame Posted at: 2018-12-18T17:40:00.736Z Reads: 41

```
I left it at my gradndma's house, because i thought i won't need it
```

---
## \#30 Posted by: xeroxgame Posted at: 2018-12-23T15:11:58.577Z Reads: 38

```
I haven't got a computer for a while, but now i have took off the bel, did motor detection and tried to move an it still does this weird sound. What now? I also would like to notice, that it doesn't spin neither with remote nor arrowy keys, but it spins while doing motor detection
```

---
## \#31 Posted by: briman05 Posted at: 2018-12-23T16:20:43.556Z Reads: 36

```
It is supposed to spin and make noise during motor detection set up the ppm settings with the max and minimum pulse width on your remote. Did you watch the video I posted?
```

---
## \#32 Posted by: xeroxgame Posted at: 2018-12-23T17:05:16.146Z Reads: 34

```
Yes i did, but i haven't got a pc at the time. I watched it again and it's working! :slight_smile: Thanks for your help very much!
```

---
## \#33 Posted by: briman05 Posted at: 2018-12-24T03:13:55.907Z Reads: 29

```
No problem glad you got it working
```

---
