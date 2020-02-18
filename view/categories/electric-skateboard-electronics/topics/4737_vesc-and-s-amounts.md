# VESC and S amounts

### Replies: 19 Views: 2718

## \#1 Posted by: ecuadorche Posted at: 2016-06-15T15:11:20.503Z Reads: 181

```
Im currently building my first board and I have a few questions about the S numbers, Im building a board that will be mostly powered at 5s by a single battery  but i was able to get some batteries for really cheap the other day and they are 3s i know i will have to run them in parallel for 6s, Is it possible to swap in between batteries without changing anything or damaging anything on the vesc????  Like if i run out of power on the 5s could i switch to the 6s by simply plugging in the batteries
```

---
## \#2 Posted by: rpn314 Posted at: 2016-06-15T15:40:22.925Z Reads: 172

```
The s number refers to how many cells are in "series," which is connecting positive terminal to negative terminal. Parallel is the inverse of series. It's when you connect the positive terminal(s) to the positive terminals of each cell and the negative to the negative.

Found this example after a quick google search, just in case your a visual person like me :slight_smile: 

http://www.radiocontrolinfo.com/wp-content/uploads/2014/10/Parallel-verse-Series-300x238.jpg
```

---
## \#3 Posted by: ecuadorche Posted at: 2016-06-15T15:44:56.673Z Reads: 155

```
i just want to know if i can switch between different s number batteries without any issues 


like board has 1 5s battery which gets drained  can i switch to an extra set of batteries of  6s without any setting changes or issues?????
```

---
## \#4 Posted by: rpn314 Posted at: 2016-06-15T15:48:31.206Z Reads: 151

```
With the VESC, I think you'd be just fine. I'm not aware of any settings you'd have to change (full disclosure: I don't have a VESC, I've just researched it a bunch...mine is on order)
I would be worried about running 5s though, as a lot of motors seem to like 6s-10s. So just pay attention to the motor your looking at to make sure it can handle the number of series cells you'd like to run.
```

---
## \#5 Posted by: Karmannghiagirl Posted at: 2016-06-15T16:30:10.352Z Reads: 133

```
switching between voltages shouldn't be an issue. I would say that if you have a vesc to try and go for a higher cell count though, maybe get another 5s and run it in series so its basically a 10s, your motor and vesc will run cooler that way.
```

---
## \#6 Posted by: ecuadorche Posted at: 2016-06-15T17:02:22.635Z Reads: 137

```
HMmm

Here is my idea and situation, i bought some cheap batteries that are 5s 4000mah 15c I have four of these batteries 2 for my board to do a dual drive 10s board and the other two i was going to use for a board for my wife she doesent want it to be powerful as she isnt experienced so i was thinking about using a single 5s battery for her board and then i got a good deal on some 3s batteries that im going to run at 6s on her board when the 5s runs out.  I should be able to switch between 5s and 6s no problem but its healthier for vesc and motor to run at higher s count?
```

---
## \#7 Posted by: DilatedPupils Posted at: 2016-06-15T17:49:33.030Z Reads: 120

```
seems like there's only gonna be an issue with the low voltage cutoff.
```

---
## \#8 Posted by: sl33py Posted at: 2016-06-15T18:43:12.514Z Reads: 119

```
No issues and this is exactly what i do.

My GF's board with VESC - i run 8s (2x4s), and give her 6s (2x3s) when she rides it.  It's a single 6354 200kv and she (no joking) goes about 8mph top speed.  Very tentative rider, but great she rides w/ me.  I give my Marbel to friends (especially new riders as i can set it in learning mode and then progressively set faster as they get comfortable), and rider "her" board.  I always joke she steals my stuff - if i let her ride it it's "hers" then...

Vanguard 41" Flex 1, dual 8Ah in series (3 or 4s), no-name 6354 200kv (10mm motor shaft a PITA - i'll never re-gear), enertion motor mount, Wiiceiver (DIYes), and VESC 4.7 running old BLDC.  (edit - also has 3d printed Nylon wheel gear for the 83mm flywheel clones) Nice weight at about 13.5-14.5lbs depending on 6s vs 8s batteries.
[img]https://lh3.googleusercontent.com/-kPs33sPKzlw/Vb_dcirbVwI/AAAAAAAAlIA/NzRnTo6FBtoPlqxjEW9CZpgyPJLeqvd_gCCo/s912/20150802_210037.jpg[/img]
```

---
## \#9 Posted by: Nordle Posted at: 2016-06-15T18:44:42.131Z Reads: 107

```
[quote="DilatedPupils, post:7, topic:4737, full:true"]
seems like there's only gonna be an issue with the low voltage cutoff.
[/quote]

:point_up_2:
-edit- but I see on the pic the voltge bzzer does the thing :D ..however I would connect both batterys
```

---
## \#10 Posted by: ecuadorche Posted at: 2016-06-15T20:06:11.004Z Reads: 98

```
so i need one of those little buzzers???? for all my batteries when they are being used???
```

---
## \#11 Posted by: treenutter Posted at: 2016-06-15T20:33:38.764Z Reads: 95

```
@ecuadorche I wouldn't swap batteries of different voltage unless you go into BLDC Tool and edit the battery parameters for the alternate battery. The voltage settings are there for a reason.

 You could carefully monitor the voltages with a meter, but you'd have to be diligent about it. The others are right that you might consider just standardizing on one battery platform that is 6S or higher.

Another reason to use consistent voltage is that your motor (or, more specifically, the KV of your motor) should be selected based on the voltage of your battery. @chaka gave some guidelines for that in this thread:

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#12 Posted by: ecuadorche Posted at: 2016-06-15T21:42:45.615Z Reads: 81

```
im not too worried about the motor kv and vesci already looked into it and that post but i didnt know about choosing battery parameters on the vesc only one of my boards will do this and its a switch from 5s to 6s will it matter much??  I just want to make sure I dont fry a vesc  any input you can shed @chaka i ordered your motors for this setup
```

---
## \#13 Posted by: chaka Posted at: 2016-06-15T21:55:17.644Z Reads: 80

```
Going with 5s is a bad idea. 6s is the absolute min voltage you should use to power an adult. I personally do not use the voltage parameters within the VESC. I leave it at default and rely on my bms to protect my cells. There have been a few cases were the VESC's firmware has been wiped clean when the voltage drops below the min threshold so be sure to adjust it if you use a lower voltage pack.
```

---
## \#14 Posted by: treenutter Posted at: 2016-06-15T22:00:21.007Z Reads: 80

```
[quote="chaka, post:13, topic:4737"]
I leave it at default and rely on my bms to protect my cells.
[/quote]

@chaka does your BMS have a soft cutoff feature? It seems that if you hit a low voltage threshold and rely on your BMS to protect the cells, it's just going to cut power completely at the threshold. What I like about VESCs LVC is that you get a warning because it slows down to let you know you're close to the limit. You may have a way better BMS than I do :) 

@ecuadorche is probably not using a BMS, so VESC or a battery meter are his options.
```

---
## \#15 Posted by: chaka Posted at: 2016-06-15T22:09:43.179Z Reads: 78

```
I use huge packs so I rarely ever deplete my pack. Over 750 watthours on my current ride.  I also use a voltage readout to monitor my total voltage.

You shouldn't have any issues using the VESC voltage limits but you need to be sure you never try to run it off a power source below the threshold. Switching back and forth between different packs is bound to cause problems since we are human and we do make mistakes.
```

---
## \#16 Posted by: treenutter Posted at: 2016-06-15T22:14:05.939Z Reads: 80

```
@ecuadorche in summary, increase your voltage to 6S and configure VESC to those voltage specifications.
```

---
## \#17 Posted by: ecuadorche Posted at: 2016-06-15T22:58:57.846Z Reads: 74

```
what about this?  ill bump hers up to 10s like mine since i have four 5s packs and could i use the 6s pack as a just in case pack????   i got these batteries really cheap and i figured might as well get them, i paid about 10 dollars for each one they are 3s 3000mah 30c batteries i was thinking of keeping them as backup pair anyways  @treenutter @chaka @sl33py
```

---
## \#18 Posted by: DilatedPupils Posted at: 2016-06-15T23:55:33.841Z Reads: 67

```
or you could just modify your packs, make them into 5S packs.
```

---
## \#19 Posted by: sl33py Posted at: 2016-06-16T15:39:16.384Z Reads: 56

```
i charge them together, and monitor the lowest battery's (individual cell) voltage.  I rarely draw below 3.6v per cell, so plenty of room and not worried too much this way.
```

---
