# Vesc battery limits

### Replies: 7 Views: 761

## \#1 Posted by: kmanbxv Posted at: 2018-07-30T02:08:26.755Z Reads: 162

```
I saw on the forum that the vesc 4.12 can only handle 27 amps? I want to set motor max and battery max higher (right now they are at 60 and 25) because I think they can handle it, but I guess the vesc can't. Could someone confirm this is the case? I want these settings as high as i can put them safely. I'll post the relevant information below. Thanks!

vesc 4.12
2 3s 5000mah 20c lipo in series
6374 192kv motor

From what I've read, the motor max could theoretically be 4032(motor rating)/12.6(pack voltage)= 320A but obviously the battery cannot output this (I plan to add one or two more 3s packs in the future btw). 

By a similar argument, the battery should be able to handle 20C * 5Ah = 100A.

Is the only answer that I need a higher battery voltage so that fewer amps are drawn by the motor? Or are 60 and 25 really a starting point that you then dial for the best performance?
Also, I have some heat sinks I could attach to the vesc, but is that overkill? It should just limit current if it starts getting hot and I don't think I'm pushing its limits with 6s.

Wow. that was a lot of questions for one post. Sorry, I've gotta learn this stuff somehow. 
**TLDR:**
**Is it ok to run vesc 4.12 at higher settings than motor max = 60 and battery max = 25?**
```

---
## \#2 Posted by: RedEagle Posted at: 2018-07-30T02:23:12.011Z Reads: 148

```
What brand is your vesc?
```

---
## \#3 Posted by: kmanbxv Posted at: 2018-07-30T02:39:33.238Z Reads: 137

```
I got it from diy electric skateboard
```

---
## \#4 Posted by: AutoItKing Posted at: 2018-07-30T02:45:57.354Z Reads: 135

```
Motor current refers to phase current which will always be higher than battery current. I run mine at 60/60 and it barely hits 20 amps battery. Battery current is approximately equal to motor current times duty cycle. So for example, at 10% duty cycle and 10A battery current, phase current is 100A! You have to remember that the motor is being switched on and off at a few kHz with a good chunk of it being off. Battery current is basically the time averaged motor current.
Of course at 100% duty cycle motor current = battery current which is where that limit finally kicks in.

The 27 amp VESC rating is battery current.
```

---
## \#5 Posted by: RedEagle Posted at: 2018-07-30T13:20:45.592Z Reads: 106

```
It's okay to run it with 60a motor max and 25a batt max. Mine is a maytech and I'm running 30a batt max without problems.
```

---
## \#6 Posted by: kmanbxv Posted at: 2018-07-30T13:42:05.880Z Reads: 94

```
But are those the upper limits? It seems like you are saying they are but then you run yours at 30 so is it a soft limit or will I definitely fry my vesc if i go above 25?
```

---
## \#7 Posted by: RedEagle Posted at: 2018-07-30T13:50:39.417Z Reads: 89

```
No, you won't fry your vesc if you go over 25a. The vesc is rated 27a continious before it goes nuclear. 
This means on a setup with a 10s battery you can have 972 watts of power. 
Most vescs nowadays can output far more power. I've seen people running 40/50a batt max. 
How much your battery can output also is a factor in power. If your battery sags alot under load you won't get good performance.
I hope this answers your question.
```

---
