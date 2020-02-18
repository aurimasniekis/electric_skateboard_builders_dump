# Payment for help Battery won’t switch off (start at post 42)

### Replies: 44 Views: 2090

## \#1 Posted by: Chase Posted at: 2018-05-06T00:22:29.823Z Reads: 207

```
So I built a 12s4p with the bestech 12s hcx-d596. Everything worked fine at first when I tuned it on. I noticed that the indicator was already reading 100. I plugged in the charger and the red lighting came on so I figured it was working. I turned it back on about 30 min later and now the indicator just flashes on and the right back off. If I plug the charger in it will show 100 percent on the indicator and not disappear instantly. It’s only when I I turn the power switch on and without it charging and then it just comes on then right back off. I tried changing infdicators and power switches Any advice would be greatly appreciated
```

---
## \#2 Posted by: anorak234 Posted at: 2018-05-06T02:27:00.579Z Reads: 188

```
Open it up - check everything. Balance wires, connections, look for marks on the BMS. If there’s nothing there - @barajabali can probably help with a diagnosis
```

---
## \#3 Posted by: Chase Posted at: 2018-05-06T03:21:18.508Z Reads: 182

```
I did. Everything is secure. It’s weird because as I connect the black wire from the indicator, the voltage between the xt90 leads drops from like 25 to two. If I plug in the charger during this time, the voltage shoots up and the indicator stays on. When it’s not plugged in the indicator shuts off. 

When indicator is not plugged in the Multimeter read from positive to negative terminals on batter is 42. The voltage between B- and the red lead in xt-90 is 42. The voltage between P- and the red xt90 lead is only 25. If the charger is plugged in it will go back up to 42. If the charger isn’t plugged it, it reads 25 unless I connect the black wire of thenindicator and then it drops to like two.
```

---
## \#4 Posted by: Bloop Posted at: 2018-05-06T03:39:51.270Z Reads: 169

```
Hmm when you connect the charger and measure is normal to show 42v because thats what the charger gives you. 

What is your diagram ? where you connected the indicator ? 

Maybe something is wrong with your indicatore or smth dont really know now. Try to remove it measure the battery voltage. Than connect the charger. If the charger turns tu red it means that is charging let it for 10-15 mins than remove it and measure the batteries.

Also are you sure you connected all the ballance wires is the proper order ? Please share some pics maybe ?
```

---
## \#5 Posted by: barajabali Posted at: 2018-05-06T03:42:18.295Z Reads: 159

```
Show pics of your pack wiring
```

---
## \#6 Posted by: barajabali Posted at: 2018-05-06T03:43:05.177Z Reads: 154

```
Also use a multimeter to see what voltage is going to the display and test if it drops to zero when off
```

---
## \#7 Posted by: Chase Posted at: 2018-05-06T04:21:06.856Z Reads: 148

```
Ok guys I really appreciate the help @Bloop @anorak234 and @barajabali   . Here are pictures diagrams and a movie

![image|375x500](upload://lpI7TxgJa7X6rFs9lsVT3BBdqEp.jpeg)![image|666x500](upload://uSBc5bwGPgKVSljkBIN0eCMID2K.jpeg)![image|666x500](upload://yqcPP5PmeMulf2sofNy1DD7zBd3.jpeg)![image|375x500](upload://scMxE28DF3i9aAdQB3rpYzjn1y7.jpeg)![image|375x500]



YouTube video
That does a better job at showing the issue 
https://youtu.be/39_Qt4unyos
```

---
## \#8 Posted by: Chase Posted at: 2018-05-06T04:24:09.053Z Reads: 140

```
![image|375x500](upload://syBKtR3dVvZPDcNMhhTDTU3NBej.jpeg)![image|375x500]
```

---
## \#9 Posted by: Bloop Posted at: 2018-05-06T05:48:26.192Z Reads: 129

```
Also can you measure your battery directly from battery wires not from bms ?
Is your bms wires as here ??

http://www.electric-skateboard.builders/t/bestech-hcx-d596-the-new-80a-bms-wiring/41047/14?u=bloop
```

---
## \#10 Posted by: Chase Posted at: 2018-05-06T06:02:29.030Z Reads: 121

```
That post was how I knew to wire how I did. If o touch just the negarive and positive battery terminals with no bms it reads 37 V. They’re obviously not fully charged so I don’t know why then indicator and charger were showing full when they were plugged in.
```

---
## \#11 Posted by: Bloop Posted at: 2018-05-06T06:08:39.868Z Reads: 120

```
Alright so from what i understand the battery is fine with 37v ( not fully charged but not dmged as you said it showed 25v) 

So the only thing that i can imagine is something wrong with the bms wireing. I cannot understand from the pics what each wire do. Also check the ballance wires again. measure one end of the battery with each ballance wire and see if they are all giving the right voltage
```

---
## \#12 Posted by: Chase Posted at: 2018-05-06T06:27:38.887Z Reads: 109

```
If I check the  terminals of the batteries it’s 37. If I test the positive leed inside the xt90 and then hold the negative leed to the B- port on the BMS I still get 37 V. It’s only after switching to measuring the positive Xt90 leed vs the P-  (instead of B-) port that s suddenly drops to 25. Since P- is also where the black indicator wire connects, it seems like there
Must be some issue when passing between those two parts of the bms.
```

---
## \#13 Posted by: Bloop Posted at: 2018-05-06T06:34:58.491Z Reads: 108

```
Yeah something is not ok with the bms. I had some problems when the ballance wires were not connected properly. 

For start you should make it just get you 37v on P-. for this id remove the chargin id remove all other wires from the indicator and only keep B- and C- and the ballancing wires chech every and each of them. If you cannot get 37v from P- and ballancing wires are ok then maybe something is wrong with the bms and might be worth checking with lucy
```

---
## \#14 Posted by: Chase Posted at: 2018-05-06T06:36:14.290Z Reads: 106

```
Since the balance Leeds are 13 pin for a 12s I followed the balance diagram here just for a 12s instead of 10

![image|500x500](upload://62qauV5637X3KFAMcx6im73O4x7.jpeg)
```

---
## \#15 Posted by: Chase Posted at: 2018-05-06T06:37:41.235Z Reads: 96

```
I already tried this. The p- with nothing on it is the point where it drops to 25
```

---
## \#16 Posted by: Bloop Posted at: 2018-05-06T06:43:05.088Z Reads: 100

```
What do you mean '12s instead of 10' ? is normal to have 13 pins for a 12s battery.

b0 is with the neggative battery wire and with B-
b1 is for the first cell
.
.
.
b12 is the last cell

This diagram you added is exactly what you need to do
```

---
## \#17 Posted by: Chase Posted at: 2018-05-06T06:55:50.619Z Reads: 98

```
Your right for some reason at the last moment I thought I had put in a 10s diagram. That is exactly what I did
```

---
## \#18 Posted by: Chase Posted at: 2018-05-07T02:19:22.495Z Reads: 84

```
So the only things that’s abnormal about the pack is that it’s jist shutting back off immediately. When you test the leeds on a normal pack there is very little voltage until you turn it on then it shoots up to where it is supposed to be. So in my pack when I have it off it measures a low voltage and then when I turn it on the voltage shoots up for just a brief second then goes back down. Same with the indicator, it comes on for a brief second right when the voltage shoots up then right back off. I wired it exactly how in the diagram above. Can anyone help please?
```

---
## \#19 Posted by: strattos Posted at: 2018-05-07T03:01:35.767Z Reads: 79

```
You've verified all your balance wires being connected correctly and being connected to the Bms properly if so then i'd say something is fucked with your  BMS. Also nice bag in your video there :stuck_out_tongue:

I've been thinking about this last night but the only thing i could imagine it being is a improperly wired balance wire or a fucked up BMS of course its hard to say without having the pack inhand but did/have you verified the voltage between all the balance wires before plugging in?
```

---
## \#20 Posted by: Chase Posted at: 2018-05-07T04:52:26.982Z Reads: 72

```
Yeah. I certainly appreciate you taking the time to give your input
```

---
## \#21 Posted by: Chase Posted at: 2018-05-08T00:27:49.272Z Reads: 66

```
I think I may have wired the balance wires backwards. I’m going to check with bestech on the wiring diagram to see which is the B1 and which is B12 pin. If I did do it backwards, did I screw up my BMS?
```

---
## \#22 Posted by: Chase Posted at: 2018-05-08T02:01:05.028Z Reads: 73

```
Can anyone verify the balance order in this picture? I wired the one with the arrow as B- but it may be B12. Can anyone look at this picture and lemme know which pin is B12? Its the Bestech D223V1 with 13 pins. 
![bms|429x499](upload://r30EH2DQIAJ2drLtZdu0uV9OAfp.jpg)

![IMG_0457|375x500](upload://s00u6iOtOs9xqijskSaLRVgsnIi.jpg)
```

---
## \#23 Posted by: Chase Posted at: 2018-05-08T05:43:30.366Z Reads: 65

```
I guess I was too out of it to remember if I checked the voltage between balance wires before plugging in. For some reason between B7 and B8 it goes from positive to negative voltage. Do you know what this means? If I measure between the first and last cell with the BMS plugged in I get a positive 37.7 V but it’s still negative only between  B7 and B8
```

---
## \#24 Posted by: Chase Posted at: 2018-05-08T06:33:27.229Z Reads: 67

```
Ok this has been solved. A nickel strip had come loose and broken the circuit. I feel dumb that it took so long to find out.
```

---
## \#25 Posted by: Chase Posted at: 2018-05-08T22:15:52.812Z Reads: 58

```
So my battery turned on and now I can’t get it to turn off. This video shows it best. I tried different indicators and used a multimeter to verify that the voltage is what the indicator is reading on the video.
```

---
## \#26 Posted by: Bloop Posted at: 2018-05-09T06:09:38.255Z Reads: 58

```
Hey Chase i remember i had a similar problem and not sure but i think you need to have the vesc connected.

In my vase i tested the battery with the bms and the eswitch wont turn it off.. had no idea why and after i connected my vescs and everything it worked as intended. 

I can only imagine that the bms has some state capacitors that wont go to 0 if there is no load connected.

Another thing.. test with multimeter the voltage will be more reliable than the indicator.
```

---
## \#27 Posted by: Chase Posted at: 2018-05-09T06:42:19.010Z Reads: 55

```
Thanks for the reply. I confirmed the voltage on the indicator with a multimeter. I just filmed the indicator because it was reading the same, and easier to film.  It’s stange how when I plug in the charger it reads like 18 but when it’s notnplugged in it’s zero. I gotta say I’m a little nervous about plugging in any of my foc boxes to a battery that isn’t necessarily working yet.
```

---
## \#28 Posted by: Bloop Posted at: 2018-05-09T06:54:44.911Z Reads: 57

```
if you try to charge your battery will it go further than 0 ? or it wont vharge at all? 

If you connect the charger is normal to show some voltage because is getting the voltage from the charger.. but if you measure your battery and it says it has some voltage and from bms output is different then there is still something wrong with the bms.

I assumed this is not the case since you tested the on off.
```

---
## \#29 Posted by: Chase Posted at: 2018-05-09T07:08:39.478Z Reads: 53

```
It shows that it charging (gaining percentage) until I unplug it then it goes back to zero. I show it somewhere in the middle of that last video I posted.
```

---
## \#30 Posted by: Bloop Posted at: 2018-05-09T07:13:32.574Z Reads: 51

```
yeah but you need more than a few sec to charge the battery that.s why i asked.

Hmm im still thinking
```

---
## \#31 Posted by: Bloop Posted at: 2018-05-09T12:36:33.404Z Reads: 45

```
so then again what is the problem right now ?

The battery is discharged or charged ? 
Will it charge ?
Do you get same voltage from bms outpus as from battery ends ?
Or the bms just keeps it on and never cuts the power ?
```

---
## \#32 Posted by: Chase Posted at: 2018-05-09T20:20:29.065Z Reads: 40

```
The battery is partially charged and will charge but it always goes back to zero % when I unplug it from the charger.
Yes I get the same from bms output as battery ends until I flip the switch off then it bounces back and forth on the bms voltage output.

Also the indicator I’m using won’t light up the green led background like it usually does when it’s plugged into a working battery switched on. The green light only comes on when I switch it off and it blinks as the voltage is bouncing back and forth.
```

---
## \#33 Posted by: Acido Posted at: 2018-05-09T20:28:19.673Z Reads: 37

```
its labeled behind the pins
```

---
## \#34 Posted by: Acido Posted at: 2018-05-09T20:29:21.387Z Reads: 38

```
where are you measuring to get a discharged voltage?
bestech bms needs to be on to charge
```

---
## \#35 Posted by: Chase Posted at: 2018-05-09T20:40:40.804Z Reads: 38

```
From the xt-90 output. I turn it on when I try to charge it.
```

---
## \#36 Posted by: Bloop Posted at: 2018-05-10T07:09:39.901Z Reads: 40

```
For feature refference plase dont test with charger pluged. Because mainly is irelevant since you are not measuring the battery but also the charger so im not sure what you expect to see.

Can you make some pictures with the battery and label the cells in series and then with the bms something clear so we can understand where each wire is going ? 

Also tell us again (with the charger Disconnected) what is the battery voltage and the bms output.( with switch on and off)

Sorry im asking you to do this again but im sure is something small that we are missing. 

Cheers.
```

---
## \#37 Posted by: Chase Posted at: 2018-05-11T01:05:31.030Z Reads: 40

```
I’m just thankful that you are still trying to solve my issue. I’ll be posting those diagrams as soon as I get a chance this week. Thanks again.

-Chase
```

---
## \#38 Posted by: Bloop Posted at: 2018-05-11T05:33:03.284Z Reads: 38

```
Haha no problem man i know how annoying is to have a problem like this.
```

---
## \#39 Posted by: Chase Posted at: 2018-05-13T06:09:26.096Z Reads: 38

```
Here are the diagrams on how I developed the battery. I also currently looking into shorts as pointed out. Thanks again everyone.

![batt issue|549x500](upload://4fYrdF7NZE8DsTvQ6KG6r1Uie5u.GIF)
```

---
## \#40 Posted by: Chase Posted at: 2018-05-13T06:47:50.068Z Reads: 39

```
Finally solved. I got a PM from @spei suggestting I check some of the solder joints ton the underside oft the bms that appeared to be close and possibly causing a short. Thank you everyone for your help.

Chase
```

---
## \#41 Posted by: Chase Posted at: 2018-05-13T09:50:14.825Z Reads: 37

```
Ant then it broke agin. SO it worked for like an hour. I was able to power on and off and it worked perfectly. Now the led screen shows that it charges. When i unplug it will still stay green and hold charge. The voltage output from the xt-90 is what it should be. Hours later, In fact the only thing that is happening now is the power switch will not turn off the indicator screen or the voltage output from the XT-90. It seems like the switch suddenly stopped working in the past few hours. It has absolutely no effect when I try to switch off or on. My indicator and votage from the xt-90 stays up.
```

---
## \#42 Posted by: Chase Posted at: 2018-05-13T20:56:36.364Z Reads: 32

```
Anyone who lives nearby in San Francisco who can come check it out and FIX this I’ll pay 30 bux. The battery works fine, it just won’t turn off when I flip th eswitch.

Here is the most recent video of the current problem.

https://youtu.be/5OPFBBHrQYk
```

---
## \#43 Posted by: Bloop Posted at: 2018-05-13T21:00:34.429Z Reads: 32

```
You tried connecting the vescs ? 
From what i understand everything else is working just fine so if you have the right voltage on BMS output why dont you just try this ?
```

---
## \#44 Posted by: Chase Posted at: 2018-05-13T21:01:22.579Z Reads: 32

```
I did hook up a load to it. I plugged in a light bulb and it lit up but I still couldn’t get it to switch off.
```

---
