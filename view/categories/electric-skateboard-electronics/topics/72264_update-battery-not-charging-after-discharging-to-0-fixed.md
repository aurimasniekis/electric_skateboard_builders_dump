# \[UPDATE\] Battery not charging after discharging to 0% - Fixed!

### Replies: 48 Views: 648

## \#1 Posted by: n8dam8 Posted at: 2018-10-25T03:11:07.444Z Reads: 150

```
Hey, Everyone! So, I went for an afternoon ride today and ended up completely discharging my battery due to heavy winds on a route that would normally leave me with 30% or more battery left.

When I got home to charge the battery, the charger LED remains green and does not initiate charging. I checked the charger and the battery (showed 34.1V) with a multimeter, and power seems to still be flowing.

When I turn on the board while plugged in, the battery indicator rises to 100%, and falls rapidly to 0% when I unplug the charger. Could there be something wrong with the BMS or a battery cell group?

Is there anything further I can do to diagnose or fix this problem? Thank you!

Battery: 10s6p Samsung 30Q pack with a BMS assembled by @psychotiller
```

---
## \#2 Posted by: Rithblu Posted at: 2018-10-25T03:23:03.341Z Reads: 148

```
100% is because its reading the power putting out  from the charger, it won't charge because you drained it to much.
```

---
## \#3 Posted by: Rithblu Posted at: 2018-10-25T03:24:44.411Z Reads: 144

```
The only way to charge it know is to charge it bypassing the BMS
```

---
## \#4 Posted by: n8dam8 Posted at: 2018-10-25T03:35:26.845Z Reads: 139

```
Okay, thanks!
```

---
## \#5 Posted by: DAddYE Posted at: 2018-10-25T04:34:45.569Z Reads: 132

```
Is it safe?
```

---
## \#6 Posted by: Trdolan03 Posted at: 2018-10-25T04:53:37.134Z Reads: 122

```
Yes it’s safe. You are still at 3.4v/cell which is well above the safe discharge voltage.
```

---
## \#7 Posted by: n8dam8 Posted at: 2018-10-25T04:58:42.054Z Reads: 122

```
Okay. So I need some help with bypassing the BMS. Do I just charge with wire coming directly from the charging port to the positive and negative ends of the battery pack?
```

---
## \#8 Posted by: Andy87 Posted at: 2018-10-25T05:00:15.631Z Reads: 120

```
0% would be below 25V on your pack.
I discharge mine till 2,8V per cell without issues.
So it looks like it’s just below your bms setting maybe or your charger makes some crazy stuff.
```

---
## \#9 Posted by: Trdolan03 Posted at: 2018-10-25T05:00:56.280Z Reads: 118

```
Check the voltage out of the charger
```

---
## \#10 Posted by: Andy87 Posted at: 2018-10-25T05:01:28.971Z Reads: 115

```
The plus of the charger to the plus of your pack 
The minus of your charger to the minus of your pack
```

---
## \#11 Posted by: n8dam8 Posted at: 2018-10-25T05:03:11.313Z Reads: 110

```
It's reading 42V
```

---
## \#12 Posted by: n8dam8 Posted at: 2018-10-25T05:03:29.990Z Reads: 107

```
Okay. I did just that and it's still not charging
```

---
## \#13 Posted by: DAddYE Posted at: 2018-10-25T05:05:05.310Z Reads: 106

```
And if it’s below?
```

---
## \#14 Posted by: Trdolan03 Posted at: 2018-10-25T05:05:21.909Z Reads: 104

```
Must be a bad BMS you need to take the negative lead from battery before the BMS and then attach that to the negative of the charger
```

---
## \#15 Posted by: n8dam8 Posted at: 2018-10-25T05:08:06.379Z Reads: 103

```
Hmmm, my negative lead from my battery goes straight to the negative of the charger. I have already cut all wires coming from the negative of the battery pack to the BMS.
```

---
## \#16 Posted by: Trdolan03 Posted at: 2018-10-25T05:09:49.414Z Reads: 100

```
One of your parallel connections in the battery is bad then. Send it back to @psychotiller for repair.
```

---
## \#17 Posted by: n8dam8 Posted at: 2018-10-25T05:13:57.137Z Reads: 97

```
Alright. Thanks for all of your help!
```

---
## \#18 Posted by: Andy87 Posted at: 2018-10-25T05:25:20.008Z Reads: 94

```
If it’s below 2.5V per cell it’s a problem.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-10-25T05:30:00.562Z Reads: 96

```
Shouldn’t the charger non the less charge? 🤔
I mean it’s a simple charger not a balance charger. This charger see only measure the input voltage not the cell count or anything else.
Even if a cell in the p group is bad (or one connection is bad) the over all voltage of the pack is still 34 something volt, which should be enough to make the charger charge. No?
```

---
## \#20 Posted by: Trdolan03 Posted at: 2018-10-25T05:31:53.695Z Reads: 96

```
I guess. The only other recommendation I would have would would be to check the individual P group voltages and make sure they are all the same.
```

---
## \#21 Posted by: Andy87 Posted at: 2018-10-25T05:36:40.886Z Reads: 93

```
This plus change the charger if possible.
Just because 42v on the output does not mean that the charger is also outputting a current.
If the charger sees always 4.2v from the battery side (out of which reason ever) he will not rise the charge current
```

---
## \#22 Posted by: Marsen Posted at: 2018-10-25T05:42:21.170Z Reads: 85

```
Measure the cell group voltages at the bms plug if all good then bypass charge as suggested. The bms may not be allowing charge to happen if one group is too low. The bms should shut the battery off if any of the cell volts drops below bottom cut of voltage, it should come back on when a charge voltage is applied though. You definitely need to know total voltage and cell group voltages before going any further .
```

---
## \#23 Posted by: dareno Posted at: 2018-10-25T06:06:09.273Z Reads: 83

```
Are these the facts?
Have you completely disconnected the bms?
The charger is outputting 42v on a multi meter?
The battery is reading 34.1 volts?
Its still not charging?
```

---
## \#24 Posted by: n8dam8 Posted at: 2018-10-25T11:39:19.732Z Reads: 73

```
Yes to all questions.
```

---
## \#25 Posted by: PXSS Posted at: 2018-10-25T12:19:03.136Z Reads: 73

```
Can you measure all the voltages coming out of the battery?

Main leads should be in the 30s
Between any two balance wires, it should be 3.0-4.2

In the end, you should have 10 cell measurements and one main leads measurement. 

The reason I am asking is that if you fully discharged, your pack could have gone out of balance. There could be 9 groups sitting at 4.2v and 1 group at 2.0v which could look like all 10 are at 4.0. The BMS is preventing you from charging because you would overcharge the battery and possibly cause a fire. In this scenario if you bypass the BMS, you will 100% damage your battery and maybe blow up your home.

The other scenario is that all your cells are reading 3.x and your charger/BMS is faulty. If you bypass the BMS and it still doesn't work, then the charger is probably at fault. 

Be careful. This stuff is dangerous. 

---

Shame on all of you for advicing someone to bypass the BMS without having knowledge of all the facts. I recommend you stay away from batteries or giving out advice on troubleshooting. 

@Trdolan03 no, bypassing the BMS is not safe.
```

---
## \#26 Posted by: dareno Posted at: 2018-10-25T12:39:53.471Z Reads: 66

```
[quote="PXSS, post:25, topic:72264"]
If you bypass the BMS and it still doesn’t work, then the charger is probably at fault.
[/quote]

Point 1  Is this not you advocating the bypass

Shame on all of you for advicing someone to bypass the BMS without having knowledge of all the facts.
[/quote]
Point 2 is this not you saying not to bypass the bms?



@Trdolan03, @Andy87 @Marsen 
actually know their stuff and are just trying to ascertain whether the bms is at fault or the charger.
I just wanted to appraise myself of the facts before advising.
Batteries are dangerous and should never be taken lightly but plugging a charger in to see if it registers is very different to leaving it charging with a suspect group or any other fault.  
The next step if you had let it happen would have been a check of the charger (which is probably the culprit to be honest) by plugging it in for a second and seeing if it had a red light. 
Think it might be you who needs to be in full receipt of the facts before you start to throw shame around.
```

---
## \#27 Posted by: n8dam8 Posted at: 2018-10-25T12:49:31.854Z Reads: 62

```
Thanks guys. I'm just going to bring it in to @psychotiller to see if he can diagnose the problem. A bad group of cells would explain why I ran out of battery before hitting 10 miles with a 10s6p and AT wheels, even though there was some wind. I usually get much more range than that.
```

---
## \#28 Posted by: Rithblu Posted at: 2018-10-25T12:51:53.955Z Reads: 60

```
Sorry for doing so, I personal did it, but shouldn’t have advice you are any one to bypass the BMS, It is very dangerous to do so.
```

---
## \#29 Posted by: Andy87 Posted at: 2018-10-25T12:52:12.728Z Reads: 57

```
one infromation i would like to get from you, just to make my soul relax.
I need to admit I forgot to ask you to which voltage your battery cut off is set in the vesc?
```

---
## \#30 Posted by: Andy87 Posted at: 2018-10-25T13:15:14.186Z Reads: 56

```
[quote="PXSS, post:25, topic:72264"]
Can you measure all the voltages coming out of the battery?
[/quote]

34,1V with 0% on the voltmeter with 10s (so still 1V per cell over dead cell level)

[quote="PXSS, post:25, topic:72264"]
If you bypass the BMS and it still doesn’t work, then the charger is probably at fault.
[/quote]

That´s exactly what i meant with it. 
Not "bypas the bms and fuck about it and continue charge without BMS". 
Just connect to the battery direct to check if the charger get red and start charging. 
After that further inspection would be neccesary for sure.
```

---
## \#31 Posted by: Marsen Posted at: 2018-10-25T13:26:12.961Z Reads: 54

```
 It was stated numerous times by several people to check cell group voltages. The charger was also checked for correct voltage. I still see no reason after checking all the voltages for not proceeding in a BMS bypass charge. You will still need to monitor the cell voltages to see if a charge is going in or if you have one a dc clamp meter to measure the current. You obviously do not continue charging if either it did accept a charge or not as this would have indicated 1. charging - fault is bms. 2. Not charging - fault in charger or battery.
```

---
## \#32 Posted by: n8dam8 Posted at: 2018-10-25T14:27:20.736Z Reads: 50

```
I'm actually not sure. @psychotiller did the initial setup. I tried to connect my board to my PC at home, but I wasn't able to update the firmware on the VESCs, so the software couldn't connect to them. I'll update them when I bring in the board.

I believe my battery was above 10% left when the board shut off. I was at 17% when I checked before it shut off after traveling a few hundred feet at jogging speed.
```

---
## \#33 Posted by: Sebike Posted at: 2018-10-25T14:38:04.411Z Reads: 48

```
Does the board turn on?

Did you carefully inspect battery for bad connections or any visible damage?
```

---
## \#34 Posted by: n8dam8 Posted at: 2018-10-25T14:40:12.447Z Reads: 45

```
Yeah, it turns on just fine. I exposed the BMS, but I didn't unwrap the whole battery. I don't want to mess anything up, so I'll just bring it in when I can.
```

---
## \#35 Posted by: Sebike Posted at: 2018-10-25T14:49:34.371Z Reads: 46

```
And did you get correct reads on all the balance leads? 3,4; 6,8; 10,2; all the way up to 34,0 aso or whatever voltage your individual cells are at..
```

---
## \#36 Posted by: n8dam8 Posted at: 2018-10-25T15:23:47.372Z Reads: 49

```
No. Like I said, I didn't unwrap the whole battery. I do not want to cause any further damage, so I'm bringing my board back to get it looked at.
```

---
## \#37 Posted by: Trdolan03 Posted at: 2018-10-25T15:27:26.806Z Reads: 48

```
Please report your findings once you get them.
```

---
## \#38 Posted by: Sebike Posted at: 2018-10-25T15:49:02.562Z Reads: 51

```
I understand. But you said the BMS was exposed, so you should be able to get the reads off of the connector/pcb.
```

---
## \#39 Posted by: n8dam8 Posted at: 2018-10-25T18:12:29.800Z Reads: 48

```
Ah okay. I think I'll leave it alone for now until I bring it in next weekend. I'll update as soon as we find the issue.
```

---
## \#40 Posted by: dareno Posted at: 2018-10-25T18:48:25.238Z Reads: 49

```
Thats the best bet my friend.  Good luck
```

---
## \#41 Posted by: PXSS Posted at: 2018-10-25T20:56:21.055Z Reads: 48

```
Please read my post as a whole and dont take things out of context. 

I asked for him to perform one action only,

[quote="PXSS, post:25, topic:72264"]
Can you measure all the voltages coming out of the battery?

Main leads should be in the 30s
Between any two balance wires, it should be 3.0-4.2
[/quote]

I gave an insight of what the results could mean by outlining two possible outcomes.
The first being, what would happen if the battery is out of balance, and the second being what would happen if the battery was in balance. Given the information above, there is no mention of the cells being in balance. I do not see anywhere him stating that the individual cell groups have been tested. Just a bunch of assumptions that they are balanced. 

Without that critical piece of info, he should not proceed. 

[quote="Andy87, post:30, topic:72264"]
34,1V with 0% on the voltmeter with 10s (so still 1V per cell over dead cell level)
[/quote]
34.1V total. There is no information there about how much voltage per cell there is. 
34.1v could mean 8 cells at 4.2v and 2 cells at 0.25v or 9 cells at 3.8v and 1 cell at 0v or 10 cells at 3.4v. All three of these scenarios would be treated differently. 

[quote="Andy87, post:30, topic:72264"]
That´s exactly what i meant with it.
Not “bypas the bms and fuck about it and continue charge without BMS”.
Just connect to the battery direct to check if the charger get red and start charging.
After that further inspection would be neccesary for sure.
[/quote]

Sure, but that should not have been the advice without the knowledge of the battery balance. 
That is the point I am trying to make. 

---

Regardless, @n8dam8 should probably just let @psychotiller handle it.
```

---
## \#42 Posted by: dareno Posted at: 2018-10-25T21:00:20.825Z Reads: 43

```
Absolutely fine my friend and I get it you know your stuff but please don't assume that everyone else is a complete moron.  Need to work on your bedside manner.
```

---
## \#43 Posted by: PXSS Posted at: 2018-10-25T21:05:39.018Z Reads: 46

```
When your advice can result in someone accidentally starting a fire in their home and getting hurt, I am going to be nothing but honest and blunt about it. 
But thats enough for derailing this thread. Take my words however you see fit.
```

---
## \#44 Posted by: n8dam8 Posted at: 2018-10-25T22:38:49.380Z Reads: 47

```
I greatly appreciate all of your help and concerns. I didn't mean for my problem to spark an argument among fellow eskating enthusiasts. I'm still pretty new to this and I don't want to harm myself or others with a fire as I live in an apartment complex, so I'm stopping my testing for now.

It seems that my chargers are still working just fine, so I'll leave it to my builder to find out what's wrong with the BMS or the battery pack.
```

---
## \#45 Posted by: PXSS Posted at: 2018-10-25T22:46:30.369Z Reads: 46

```
Hopefully the battery can be fixed easily. :)
```

---
## \#46 Posted by: n8dam8 Posted at: 2018-11-07T02:07:13.160Z Reads: 41

```
So, it turns out 1 group of 6 cells were dead at 0 Volts left. Also, my BMS got fried.
@psychotiller has replaced the 6 cells and the BMS and he says the pack charges just fine now!

Thanks, everyone, for all of your help!
```

---
## \#47 Posted by: PXSS Posted at: 2018-11-07T02:11:59.713Z Reads: 41

```
Great to hear!

This scenario is the one where you definitely didn't want to bypass the bms as it could cause a fire by overcharging the other cells.
The others can learn from this too :slight_smile:
@dareno
```

---
## \#48 Posted by: dareno Posted at: 2018-11-07T04:34:20.200Z Reads: 37

```
Why did you tag me?  If you remember Or bothered to read the original post I did not tell the guy to do anything at all I just told you to behave yourself.
```

---
