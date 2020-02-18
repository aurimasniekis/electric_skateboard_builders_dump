# Charger not charging

### Replies: 16 Views: 303

## \#1 Posted by: amms50 Posted at: 2019-05-11T10:37:50.316Z Reads: 88

```
Hello everyone :grin:

I recently finished my diy board and was really satisfied with it, unfortunately i ordered a 42v charger off of AliExpress and it didn’t reach me but that’s a story for another time so I am using my friend’s charger. Anyways I ordered a Bosch 42v 3.5a for electric bikes and soldered a new plug that I found laying around and was really happy about it.
![image|281x500](upload://wqBa1GCJXXsBKjnT3KRgltoFpfd.jpeg) 
 ![image|375x500](upload://AeDNv2mYigFSFJYiwXi51iCoWre.jpeg) 
![image|375x500](upload://xwEfm7y4iOGc1r5kxdMzpUM8Dao.jpeg) 
So I plugged it in and left it for a whole day only to come back, turn the board on and find out that it didn’t charge a single bit. The problem too is that there isn’t any light on the charger to indicate that it is charging or no so at the beginning it was a guessing game but now I’m sure it doesn’t charge.

So what do you guys think I could do to make it work?
```

---
## \#2 Posted by: bartroosen12 Posted at: 2019-05-11T10:39:35.624Z Reads: 78

```
Can you measure the voltage of the charger to be sure it's working?
```

---
## \#3 Posted by: amms50 Posted at: 2019-05-11T21:37:16.839Z Reads: 67

```
Yea I just measured it its 42.06v
```

---
## \#4 Posted by: Jinra Posted at: 2019-05-11T21:42:28.767Z Reads: 66

```
You sure you got the polarity right?
```

---
## \#5 Posted by: pat.speed Posted at: 2019-05-11T22:16:29.412Z Reads: 59

```
First few things to check at if the bms is receiving the 42v from charger, if yes then could be a bms issue or wiring issue between the bms and battery. If it’s not getting charge I would first check continuity between the plug and charger pcb, if that’s all good check to make sure the wiring between charge port and bms is all g. Also check to make sure that the plug you have is actually the same as your charge port. There are different sized inside prongs and you may be larger than the other and not making contact. 

One of these is likely to be your issue so I’d go through these and thorough check your wiring and polarity, posting your wiring schematic here would also be beneficial.

Ps. do not stick the multimeter in the charger port no matter what lol
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-05-12T01:38:19.565Z Reads: 50

```
plug it into a spare charge port not hooked up to a battery. try and measure voltage off the back of the port and make sure its correct. some have 3 pins and 1 isnt even hooked up
```

---
## \#7 Posted by: amms50 Posted at: 2019-05-12T08:13:21.510Z Reads: 44

```
I did that and also got a measurement of 42.06v
```

---
## \#8 Posted by: amms50 Posted at: 2019-05-12T08:14:18.159Z Reads: 43

```
Yes I am sure I even tested it out before soldering the plug
```

---
## \#9 Posted by: amms50 Posted at: 2019-05-12T08:22:54.654Z Reads: 38

```
I checked every single one of those point and got the results I was waiting for which is 42.06v, to the point that I disassembled my whole board and measured every single contact to make sure that the power was getting through and it got through in every single contact, it is the correct plug cuz I tested the plug with another charger and it charged my board fully.

What I wasn’t comfortable about was that the charger was making weird noise every 3-4 second while it is plugged in the board, it sounded like spark inside the power brick and that was annoying me a bit, tried opening the brick but unfortunately it’s sealed with three layers of silicon and two other (german quality :sweat_smile: )
```

---
## \#10 Posted by: pat.speed Posted at: 2019-05-12T11:43:31.321Z Reads: 35

```
Hmm this is weird then. May I ask what bms you are using? And if it would be possible to try and charge the battery a little directly from the charger. This will tell you if it’s a battery wiring issue or bms problem

If it charges fine directly to the battery I would assume a dodgy bms, if it doesn’t charge the battery then there could be a problem in the battery wiring.

Also something I just thought of is the bms must not be connecting the battery to the charger, because if it was you wouldn’t have measured 42v at the contacts but somthing lower similar to the batteries current voltage. 

Also are you bypassing the bms for charge only or discharging through it
```

---
## \#11 Posted by: amms50 Posted at: 2019-05-12T14:28:08.445Z Reads: 29

```
This is the bms I am using:
![image|281x500](upload://eDgP8Qohm9xpC4sjCCwZa3YDLt4.jpeg) 

I just tried it and it kept on making the weird spark noise from inside the charger which I think indicates that it is not charging but let’s not also forget that with my friend’s 42v 2a ownboard charger it charges without a problem

Yea yea right I just remember when I measured the battery contacts I got 36v not 42 sorry :sweat_smile:

I am discharging through the bms
```

---
## \#12 Posted by: J_Dizzle Posted at: 2019-05-12T14:33:02.911Z Reads: 28

```
I had the same problem a while ago and it was that my wiring from my bms to my batteries was wrong. have you double checked your wiring?
```

---
## \#13 Posted by: amms50 Posted at: 2019-05-12T14:37:27.241Z Reads: 28

```
I am pretty sure it is not from the bms cuz when I charge with other chargers it charges without a problem but with the one I have it doesn’t
```

---
## \#14 Posted by: Namasaki Posted at: 2019-05-12T14:46:43.721Z Reads: 27

```
[quote="amms50, post:13, topic:93467"]
when I charge with other chargers it charges without a problem but with the one I have it doesn’t
[/quote]

You have solved the problem. 
Your charger is defective. 
Your gonna need a new charger.
```

---
## \#15 Posted by: amms50 Posted at: 2019-05-12T14:58:57.908Z Reads: 25

```
Yea I guess so, I thought maybe there was a fault with the board or something but I guess I just have to get a new charger
```

---
## \#16 Posted by: pat.speed Posted at: 2019-05-12T22:11:32.544Z Reads: 16

```
Yeah it must be the charger then. I thought you said that the charger worked on your friends board Burbank I must have read it round the wrong way. 

You should be able to get a replacement or refund, and get a new one
```

---
