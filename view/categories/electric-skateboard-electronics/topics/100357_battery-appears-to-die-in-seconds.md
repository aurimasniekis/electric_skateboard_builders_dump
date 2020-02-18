# Battery appears to die in seconds

### Replies: 22 Views: 287

## \#1 Posted by: Nahuebusti Posted at: 2019-08-15T22:26:50.400Z Reads: 85

```
Hello people, i'm kinda new on this, I've made my first diy esk8 and i have a problem, i full charge the battery, and after seconds of using, it dies. The battery is 10s2p with BMS. I use an ebay ESC. The output shows 38v, but if i start to use the motors, the V goes down immediately.
```

---
## \#2 Posted by: dareno Posted at: 2019-08-15T22:48:18.239Z Reads: 83

```
Where did the battery come from?
```

---
## \#3 Posted by: Nahuebusti Posted at: 2019-08-15T23:10:39.293Z Reads: 80

```
I made it from LG 18650 cells, first i charged them with a module and then i made the pack
```

---
## \#4 Posted by: dareno Posted at: 2019-08-15T23:17:40.564Z Reads: 80

```
You are definitely using the correct charger?  That pack should output 42v on full charge so if the charger is saying full at 38 then that could be the problem.  Without a detailed look at the pack its hard to speculate really.  Bms is wired for charge only I assume?

Multi meter time my friend.  Check the charger output and carefully check the batteries true voltage and then go through your bms wiring to check the individual p packs.  One could be way out of balance and the charger is trying to balance it which happens after the charge cycle on most chargers.  Check for safetys sake though that all your voltage readings are correct.
```

---
## \#5 Posted by: Nahuebusti Posted at: 2019-08-15T23:43:22.707Z Reads: 74

```
The charger says 42v at the output, so i assume it's ok. BMS just for charge? What do you mean? (Sorry I'm a begginer).
I started testing all the cells, they all are at the same V, and the wiring is ok too. The output of the bms is the same as the pack itself, but when i start to run the motor on the tip speed, it decreases immediately, just in matter of seconds, and then it turns off.![IMG-20190815-WA0027|559x500](upload://r2KtHjuGcRtHKTyXBrIIjPdZIIL.jpeg) 
I'll attach the connection scheme.
```

---
## \#6 Posted by: M.Hboards Posted at: 2019-08-16T00:20:45.733Z Reads: 67

```
The diagram above shows its wired for charge and discharge and since your  probably pulling more then 35 amp the bms is cutting off.
```

---
## \#7 Posted by: Nahuebusti Posted at: 2019-08-16T00:28:07.340Z Reads: 67

```
And what should i do? I just checked with the multimeter and the cells aren't charged fully (all of them in 3.8v) and the charger stopped charging, i seems that the bms is cutting the charging.
```

---
## \#8 Posted by: dareno Posted at: 2019-08-16T01:54:01.737Z Reads: 64

```
![image|690x292](upload://ePeqaXkfMGh1V11b0F16OtDwL87.jpeg) 

This is courtesy of the wonderful gent who is our own @mmaner

Got the lot in there for you.  As @M.Hboards said your bms is cutting off because it should be wired for charge only.  Rewire it and you should be fine.
```

---
## \#9 Posted by: Nahuebusti Posted at: 2019-08-16T11:35:46.607Z Reads: 51

```
Thanks dude, today I'll change the connection. Is the mosfet switch really necessary? Because i don't have it. And there i can't see well, but there is the black wire (near the red ones) connected to the negative of the battery, isn't it?.
Thanks you for your help again
```

---
## \#10 Posted by: Jebe Posted at: 2019-08-16T14:28:09.087Z Reads: 49

```
What LG cells are they? not all 18650's are created equal. try bypassing the BMS for discharge, and only using it for balancing. As you are only getting to 38v it's likely you have a failed cell in there. oh and that layout is for focboxes with a separate eswitch. Those dinky ebay escs have the switch built in.
```

---
## \#11 Posted by: ShutterShock Posted at: 2019-08-16T15:46:38.437Z Reads: 46

```
I would also be curious what cells, 10s2p isn't much either.  The switch is not necessary for you either but on the other hand, you won't have a huge amount of performance out of an Ebay ESC anyway.

I would question the battery build - what exactly is it and where are the pictures haha sounds like you're missing a group
```

---
## \#12 Posted by: dareno Posted at: 2019-08-16T17:29:00.933Z Reads: 41

```
You don't have to take the whole diagram as a template bro.  Just take what you need from it.  Its just a nice clear wiring diagram for the charge only mod you need to do.
```

---
## \#13 Posted by: Nahuebusti Posted at: 2019-08-16T19:40:43.397Z Reads: 38

```
![IMG_20190816_163449886|666x500](upload://zoAEQY4RHS6UvBCjayteVTDZvBi.jpeg) 

Here you all have my set (it's a prototype, i haven't finished it, and please don't hate me for the wiring haha). I didn't use a spot welder because i don't have one, and i know i didn't use the best products, but please understand me, i live in Argentina and everything is very expensive haha. However, the wiring is OK, and now i changed the connection like you said and for discharge is still happening the same, the V go down in seconds.
```

---
## \#14 Posted by: Nahuebusti Posted at: 2019-08-16T23:59:52.137Z Reads: 33

```
Is it maybe too weak for 2 motors? May i build more parallel groups??
```

---
## \#15 Posted by: Jebe Posted at: 2019-08-17T00:42:28.705Z Reads: 31

```
Soldering can damage cells if you get too much heat into them. Measure the voltage between each group. Should be close to equal. Then measure under load. And what exact cells are you using?
```

---
## \#16 Posted by: Nahuebusti Posted at: 2019-08-17T01:01:34.399Z Reads: 29

```
I charged them and they where all between 4.1 and 4.2v, so i assume they charge equal. The cell has LGDAS31865 K206G254A6 written on it. I just ride the skate in the minimum velocity and it worked fine, then passed to medium and it turned off :frowning:
```

---
## \#17 Posted by: Jebe Posted at: 2019-08-17T07:23:50.410Z Reads: 25

```
Search the net for the max discharge rating on those cells. Not all 18650s are the same. Tje discharge rating on these is less than half an amp. Peak is 3.2 amps. Throw these into a portable usb charger and look for some decent cells. You want something thats minimum 15amp discharge for a 2p battery for eskate. That pack is a flare waiting to happen
```

---
## \#18 Posted by: Sedmii Posted at: 2019-08-17T10:30:23.588Z Reads: 24

```
[quote="Nahuebusti, post:1, topic:100357"]
and i have a problem, i full charge the battery, and after seconds of using, it dies. The battery is 10s2p with BMS. I use an ebay ESC. The output shows 38v, but if i start to use the motors, the V goes down
[/quote]

Dont bypass the BMS for discharge. You have 2p groups, so even if the cells can do 15A (which they cant since the datasheet says 3A max) thats withing limits of BMS. If the BMS is cutting then thats to protect the cells. If you pull more than 35A from these cells you are gona have a ''fun'' time
```

---
## \#19 Posted by: Nahuebusti Posted at: 2019-08-17T21:18:14.902Z Reads: 20

```
Ok people, i understood, i don't want to transform my skate into a wood fire. I'll change them, what brand or type do u recommend?
```

---
## \#20 Posted by: bsancken Posted at: 2019-08-17T23:23:08.108Z Reads: 19

```
[quote="Nahuebusti, post:16, topic:100357"]
LGDAS31865
[/quote]
I know that this has already been found but - 
https://secondlifestorage.com/t-LG-LGDAS31865-Cell-Specifications

This is a great resource for looking up cells you have or are looking at BTW
https://secondlifestorage.com/celldatabase.php
```

---
## \#21 Posted by: Nahuebusti Posted at: 2019-08-17T23:34:16.667Z Reads: 17

```
Thank you for that information man! I'm new on this and i have no idea of a lot of things, for example, the cells 😂
```

---
## \#22 Posted by: bsancken Posted at: 2019-08-17T23:35:44.559Z Reads: 17

```
I actually haven't seen this site referenced here and I'm watch that forum's youtuber's live stream and though of throwing that here. 

Good luck!
```

---
