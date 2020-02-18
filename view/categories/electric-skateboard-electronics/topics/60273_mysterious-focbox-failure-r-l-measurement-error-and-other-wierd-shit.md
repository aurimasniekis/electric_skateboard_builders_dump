# Mysterious focbox failure- R&amp;L measurement error and other wierd shit

### Replies: 7 Views: 358

## \#1 Posted by: PatRocks Posted at: 2018-06-28T00:43:24.687Z Reads: 90

```
FIRST: I've spent the past 2 days using every combination of keywords that I could think of searching for an error identical to mine. This thread is unique Imo, and my intention is to thoroughly investigate circumstances, catalysts, and solution to this murder mystery. Soooo many drv-error threads out there, so few resolutions... I'd like to finish this one, damnit!!

As for screen shots and app settings, let's agree that the controller worked error-free on 12s FOC for 8 months, and on 8s FOC four months before that. So...

Short version: Transplanting focboxes to dual heatsink. I didn't do anything wrong to the best of my knowledge. Wires never touched, battery never connected until fully reassembled and ready to detect motors. Ran foc detection carefully. Nothing changed mechanically. Focbox is dead for like, literally no reason (that I've found so far)

NO CAN BUS!! BOTH ESCS ARE INDEPENDENT 
One is good to go, one is dead, no physical signs of damage. Newer unit is running an sk3 sensored 192kv 6374, the dead one-a tb 6374
Both were ackmaniac v3.101, both worked before transplant. 

Long version:
Well, after more than a year in FOC Mode, more than half of which at 12s, my poor VescX ate shit. The interesting thing about this is I HAVE ABSOLUTELY NO IDEA WHAT HAPPENED TO IT!!!

Here's the back story: the recently deceased controller had been in charge of a TB 6374 in sensored FOC mode for a little over a year. Everything was fine, right up until I decided to install the duel focbox case from @3DServisas (thanks @Kug3lis !! Great product!!!). After a careful installation process, with all wire connections double checked, heat pads in place, etc., I went to my computer to run motor detection, and that's where shit hit the fan.

First, I configured my newer focbox, which runs a sensored sk3 6374 on FOC. That process went seamlessly, so I powered off the board and switched USBS to program the other. I closed the vesc tool, reopened it, read all settings, Switched Off the app control, rebooted and attempted to start the FOC detection process.
First thing I noticed, after clicking measure R&L, is that the motor only made it's ticking sound before the large resistance testing sound for about 3 seconds as opposed to the usual 5 to 10. That was very odd I thought, so after hesitating, I clicked on the flux linkage measurement button. There was a pause, as usual but the motor did not spin. Instead it made a pronounced clicking sound, as if the phases were shorted internally, just like when the motor goes to full brake at low speed just before full stop. Terminal reported abs over current. 

I disconnected and reconnected everything, powered off the board, closed and reopened V application, and repeated the above steps. This time I got abs over current, and fault code drv. At this point I noticed that the resistance measurement for the motor was at about 7,800mOhms! Wtf?? 

Last night, a day later,  I resoldered the phase wires, cleaned the flux off, and resoldered the bullets to be sure they were clean joints. I REALLY put my most thorough efforts into making sure I'd done my homework, but when i tried again, the same results showed. "Could not measure flux linkage correctly. Please adjust starting parameters and try again" "Fuck YOU!!", I Shouted, then connected to my other motor which works with the other unit presently, and got the same back-talk from my computer, errors and all.

TL;DR: Nothing changed mechanically, NO PHASE CONNECTORS TOUCHED, all FETS's show the same resistance across, all motor wires, and FET to Phase ends, are the same resistance, every single thing I've thought to check is NORMAL!! 

I'm PISSED!!!, but very interested 🤔

Let's start by discussing why the "MEASURE R&L" detection process would end so early, and why motor resistance measures at 7,884.78 mOhms instead of 13.8?? Which component of the esc performs this measurement?


![20180626_123132|690x388](upload://gdiyP4LVr0ljhDLqZ97ChqH9Eea.jpg)

Some photos of the ESC:
1.
![20180627_010338|690x388](upload://qjqNZMr9QewYFoWoeEZaJRJv3eY.jpg)

2.
![20180627_010344|690x388](upload://nDhUd7hpiqneE1YAeHjZ7oRE6BS.jpg)
3.
![20180627_010352|690x388](upload://jGPvbGj41qy03S9NCcbG2leEwJ5.jpg)
4.
![20180627_010404|690x388](upload://dguCbyCwTuj7ICp4FIb9FkNgkcK.jpg)
5.
![20180627_010417|690x388](upload://oyC0XmynJ6djjB0C5SSsjKZqs1x.jpg)
6.
![20180627_010427|690x388](upload://dMsY4CaISqDoK4ekrD9kyILORwB.jpg)
7.
![20180627_010433|690x388](upload://yyKc2tPjv3Q7PykSEPj9lLp7HcK.jpg)

These photos were taken before resoldering the phase wires to the PCB. When I resoldered, I cleaned off all of the flux to make it look nice. I personally cannot see any obvious signs of damage, but maybe the experts out there can...

Flux error screen shot:
![20180626_123148|690x388](upload://18nCJ6CiXgzqC34TvrYxp9fHmC7.jpg)
And fault codes, both come after flux measurement error. 
![20180626_123213|690x388](upload://oc00cs2QibrrrEL0kBGIp5B8AKP.jpg)
Without sounding arrogant in any way, I'd like to ask that the feedback please be kept free of beginner-level questions and comments. The reason being, I feel that almost every other focbox problems have been addressed elsewhere. As I haven't seen anything quite like this, I intend to document this issue as scientifically as possible to maximize the usefulness of this thread. 

To summarize my theory, I think that if we can determine why the 1st step of foc detection is short cutting (one motor-click, three seconds then BUZZZ) and erroneous resistance readings,  we will be on the right track.
Obviously some parts will need replacement, but I gotta find the problem first.
@JohnnyMeduse @Blasto @Deckoz @Namasaki Anyone that has an idea of what may be going on here, I'd like to see what you think!

I will add all relevant information that I come across as needed!
Respectfully!
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-06-28T01:08:24.248Z Reads: 71

```
R35 is badly solder

![image|690x388](upload://4SVQtDpT67oBPZsU9iNkS0iI1Dn.jpg)

Edit: Maybe you could check if you didn't knock up any other resistor
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-06-28T01:16:56.392Z Reads: 66

```
Yeah, that's gate resistor I guess (If so it doesn't switch one mosfet which fails everything... Good thing no shortages for you...). Plus all solder joints are so skinny like there are just a little of solder

EDIT: R20 is also looks like one side is in air
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2018-06-28T01:20:20.454Z Reads: 67

```
No solder join is out of solder... Do you even know your IPC standard?

Edit: He probably knock the resistor while replacing is lead cable.
```

---
## \#5 Posted by: PatRocks Posted at: 2018-06-28T01:22:49.968Z Reads: 61

```
Thanks guys, definitely going to loo at all joints tonight
Edit: @JohnnyMeduse great point! That's the only thing I touched between it working and not working
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-06-28T01:23:23.402Z Reads: 62

```
Yeah, I know but don't forget this is high vibration environment, you don't want to have a cracked solder joint to start sparking with Li* batteries :D
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2018-06-28T01:44:28.950Z Reads: 60

```
If you have a good solder join, you would never get any issue with vibration. If a solder crack at one point, it because the solder wasn't made properly (or cold) or there a constant stress on the PCB (which can be cause using an improper gap pad in the case of a focbox). 

Here is what a good (perfect situation) should look like 

![images-1|223x177](upload://cMYtXLbD7mi6vrwkvNoCrj76O43.jpg)

Here is what a cold solder (or improper) solder joint will look like

![Unit8_R33|690x473](upload://kpW2jgnpgVythQu6lfS2sTDwXvY.jpg)

But with the current that we are using those should fail fast. 

Here is what happen if you don't use the right Gap pad, all the stress is trasfer to the pcb. (BTW that only 1mm of difference). As you can see the pcb is clearly bending, transfering stressall the component on the top. 

![image|666x500](upload://AiZyyOlDm1dMAbMZF1frnCxSC7.jpeg)
```

---
