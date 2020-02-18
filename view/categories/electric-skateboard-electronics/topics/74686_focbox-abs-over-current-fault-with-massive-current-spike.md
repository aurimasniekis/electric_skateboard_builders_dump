# FOCBOX abs_over_current fault with massive current spike

### Replies: 31 Views: 707

## \#1 Posted by: bobbobman Posted at: 2018-11-14T08:45:54.093Z Reads: 165

```
**New new question:**

Unfortunately, I now have yet another issue. Figured I’d keep using this thread rather than making new ones.

I’ve been riding around on the build for a few days now without issue, until earlier tonight. Going down a hill at low speeds, my brakes cut out for a second. I hopped off, picked the board up, revved it a couple times, and found no issues. Hopped back on, rode a bit further. A couple minutes later, again going very slowly on flat ground, I seemed to lose power completely for a few moments. I glided for a bit, and when I tried to break, there was a short delay as though the VESC has just rebooted.

Coming home, I hooked it up to my computer, booted up the terminal, and was greeted with this:

![11-24-18%20overcurrent%20fault|590x434](https://www.electric-skateboard.builders/uploads/db1493/original/3X/d/f/df32c86a74f345ce46c29e1620645f690b2ed80b.jpeg)

I immediately looked around for other abs_over_current faults on the forums but what struck me was that I haven’t seen any with a current spike as high as mine showed.

Any idea what could be causing this? To my memory, I didn’t do anything that could be considered a high load on my ride tonight. Everything was at very low speeds.






**Second old question:**

Edit: Bonus question: I've got a dual setup over CAN running FOC and when it first boots up, everything works great. The problem is, if I let the system sit for a few minutes idle, the slave VESC's motor doesn't spin anymore while the master's still works fine. Is there a reason for this?





Original old question:

I'm trying to avoid voiding any warranties so I've come up with a sort of makeshift solution that looks like this:
![1542184868646738386622|375x500](upload://xlhrVL242R6B992WMxj7pnaRYit.jpeg)  

Essentially, I jammed the edge of the FOCBOX connector into one of the gaps in the prongs of the 5.5 mm connector. There's good enough contact that allow for motor detection and I've got it spinning without load just fine. My concern is, will the connectors be able to handle the current at full load like this, or does there need to be a more substantial connection?

If it's ok, I would electrical tape it real tight, or maybe hot glue it or something, to make sure the connectors don't get separated. Appreciate any feedback!
```

---
## \#2 Posted by: dareno Posted at: 2018-11-14T08:54:55.915Z Reads: 160

```
As a permanent solution HELL NO.

Solder on some different connectors on the phase wires if you are worried about the warranty.  3.5mm bullets are better than that fiasco.  Seriously?
```

---
## \#3 Posted by: Linny Posted at: 2018-11-14T08:56:39.494Z Reads: 156

```
You can have motor wire extensions as well. So the VESC 3.5mm connects to one end of the motor extension which is 3.5, and the other ends are 5.5mm. No soldering on the VESCs to void warranty, but you need to make the wires yourself with the connectors.
```

---
## \#4 Posted by: dareno Posted at: 2018-11-14T09:02:54.443Z Reads: 157

```
[quote="bobbobman, post:1, topic:74686"]
Edit: Bonus question: I’ve got a dual setup over CAN running FOC and when it first boots up, everything works great. The problem is, if I let the system sit for a few minutes idle, the slave VESC’s motor doesn’t spin anymore while the master’s still works fine. Is there a reason for this?
[/quote]

Connect it all up properly and try it again.  Sorry if I seemed harsh but trying to stop you making expensive mistakes.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-11-14T09:08:30.375Z Reads: 152

```
https://www.electric-skateboard.builders/t/focbox-3-5mm-bullet-connector-to-5-5mm-motor-connector/51033/15?u=andy87
```

---
## \#6 Posted by: bobbobman Posted at: 2018-11-14T09:10:31.238Z Reads: 142

```
No worries. I appreciate the help. I actually never even thought about making my own adapter wires. That's probably what I'll end up doing. Less fire hazard. As fare as the VESC question goes, what throws me off is that everything works properly if I just reboot the system. Then it works until I leave it sitting idle for like fifteen minutes, at which point the slave no longer spins while the master continues to work. Not sure what's going on there, but I'll rewire it all up when I bullets get here and see if it fixes everything.
```

---
## \#7 Posted by: bobbobman Posted at: 2018-11-14T09:11:30.425Z Reads: 138

```
Oh that's an option too...Yeah I'll probably either do that or the adapter wires.
```

---
## \#8 Posted by: dareno Posted at: 2018-11-14T09:23:03.297Z Reads: 128

```
Focboxes are a great vesc probably the best for the money atm but they will go poof if you don't wire them correctly.  Dodgy phase wiring will definitely fry them.  The problem with using adaptor wires is the amount of unnecessary cables so if you don't need extra length then just change the connectors.  5.5mm is better than 3.5mm but that depends on your battery and the amount of current you are drawing. 
Personally I changed the 3.5mm bullets on all mine and have had 2 replaced under warranty so its not a fully enforced rule.  If your wiring is good then run the detection again and then check back in with the results and hopefully the issue will be gone.  If not then we can run through the set up and sort it for you.

EDIT.  Just to be clear.
good connectors are the ones with the least resistance.  By just touching each bullet together on the side you are creating resistance and this will give you a false detection result on your motors and therefore create issues down the line.
```

---
## \#9 Posted by: bobbobman Posted at: 2018-11-14T09:39:59.206Z Reads: 118

```
Ah that makes sense. I'll rewire everything later this week and update. Thanks for the help!
```

---
## \#10 Posted by: billappleton Posted at: 2018-11-15T18:46:08.501Z Reads: 103

```
You can cram one into the other and solder works great


![image|375x500](upload://cGr9GwannncZTVF7fxLBa7ha1oL.jpeg)
```

---
## \#11 Posted by: Battosaii Posted at: 2018-11-15T19:04:29.176Z Reads: 98

```
Just solder on new connections warranty doesn't matter cause of you blow a drv chip or a fett they will say it's user error and not cover it anyway.
```

---
## \#12 Posted by: bobbobman Posted at: 2018-11-17T08:22:07.960Z Reads: 82

```
Update: It's all wired up properly now but I still run into the same issue of the slave motor stopping after a few minutes. Upon startup, they both spin fine but after a couple minutes idle, its like the slave FOCBOX goes to sleep and no longer takes input. Any idea what could be going on?
```

---
## \#13 Posted by: J0ker3366 Posted at: 2018-11-17T08:29:45.443Z Reads: 83

```
Screen shots of vesc settings please
```

---
## \#14 Posted by: bobbobman Posted at: 2018-11-17T08:44:31.846Z Reads: 78

```
Here:

Master:

![M-Gen|690x347](upload://wTfNbGeAgM4Pvm2Jsanf01r0g0H.jpeg) ![M-FOC|690x344](upload://hIpIeW0sFlgFLe4DhgrkGwlfYiD.jpeg) ![M-Motor|690x327](upload://hSM7yRz2S4Yc223pu2Jj3Kh5fP0.jpeg) ![M-PPM|690x332](upload://oqB7Bh4yMWDKfeMxErVRXtgtKeM.jpeg) 

Slave:

![S-Gen|690x338](upload://onPncejhzKp2vzWmI3pNYkCjJyf.jpeg) ![S-FOC|690x340](upload://tp1MQ97SCgYgy4ndsmgxuporj2I.jpeg) ![S-PPM|690x321](upload://wrQEJEKFvLMUf9wbeojBP5kPVYu.jpeg) ![S-Motor|690x342](upload://hSH1uLkXVzIOXtBGU1wbIDrQjr5.jpeg)
```

---
## \#15 Posted by: Blasto Posted at: 2018-11-17T08:53:22.246Z Reads: 67

```
Set the MAX input voltage back to 57V
```

---
## \#16 Posted by: bobbobman Posted at: 2018-11-17T08:55:36.184Z Reads: 69

```
Oh yeah I guess I shouldn't have messed with that. Is that what's causing the cutout?
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2018-11-17T13:37:24.659Z Reads: 67

```
This should be uncheck in the master.

![image|666x500](upload://l8SMV5UQAyIhvFs35h9X0Y6uNBD.jpeg)
```

---
## \#18 Posted by: dareno Posted at: 2018-11-17T21:08:13.611Z Reads: 63

```
:arrow_up:  this.
```

---
## \#19 Posted by: bobbobman Posted at: 2018-11-25T09:27:11.179Z Reads: 62

```
Alright update: I finally got some time to tinker a couple days ago. Changed all the settings and it solved the slave cutout issue. Thanks! 

Unfortunately, I now have yet another issue. Figured I'd keep using this thread rather than making new ones. 

I've been riding around on the build for a few days now without issue, until earlier tonight. Going down a hill at low speeds, my brakes cut out for a second. I hopped off, picked the board up, revved it a couple times, and found no issues. Hopped back on, rode a bit further. A couple minutes later, again going very slowly on flat ground, I seemed to lose power completely for a few moments. I glided for a bit, and when I tried to break, there was a short delay as though the VESC has just rebooted. 

Coming home, I hooked it up to my computer, booted up the terminal, and was greeted with this:
![11-24-18%20overcurrent%20fault|590x434](upload://vQvhdxG7tupniWtqt6G9PyH3woz.jpeg) 

I immediately looked around for other abs_over_current faults on the forums but what struck me was that I haven't seen any with a current spike as high as mine showed. 

Any idea what could be causing this? To my memory, I didn't do anything that could be considered a high load on my ride tonight. Everything was at very low speeds.
```

---
## \#20 Posted by: bobbobman Posted at: 2018-11-25T17:49:46.386Z Reads: 59

```
Bump, any ideas?
```

---
## \#21 Posted by: strattos Posted at: 2018-11-25T18:03:04.970Z Reads: 57

```
It's a broken connection 99% of the time it took me months to find mine as a cap leg was broken but still perfectly aligned because of the housing. Double and triple check your connections one of them is bad.
```

---
## \#22 Posted by: dareno Posted at: 2018-11-25T23:52:41.595Z Reads: 52

```
Was the board fully charged when you went down the hill?
```

---
## \#23 Posted by: bobbobman Posted at: 2018-11-26T02:44:17.716Z Reads: 49

```
Hmm I'll have to check again. I looked at all the obvious connections already but maybe I missed something.
```

---
## \#24 Posted by: bobbobman Posted at: 2018-11-26T02:45:21.426Z Reads: 50

```
No, it shouldn't have been. I'd already ridden it up a couple hills before I tried going down. Wouldn't it cause a negative current spike if it were an issue with too much current being sent through braking?
```

---
## \#25 Posted by: dareno Posted at: 2018-11-26T02:47:10.356Z Reads: 49

```
Thinking more of the bms cutting out from over voltage.
```

---
## \#26 Posted by: bobbobman Posted at: 2018-11-26T02:52:29.497Z Reads: 46

```
Oh interesting. I'll have to keep a look out. I took it for very ginger test ride around today, up and down the same hills and didn't run into the same issue so I'm going to have to just keep monitoring it. I just wanted to make sure I wasn't making some super glaring mistake. Do you think there could be some issue with inductance from too much wire between the vesc and the battery? I've got probably about a 20 inches with the antispark switch, the battery's own output wire, and the flat braid spanning the split enclosures.
```

---
## \#27 Posted by: dareno Posted at: 2018-11-26T02:56:24.862Z Reads: 46

```
No.  thats fine.
```

---
## \#28 Posted by: lrdesigns Posted at: 2018-11-26T04:39:56.980Z Reads: 42

```
I would also say a broken capacitor leg. If not that some other loose connection in the power system. 

Did you open the vesc and check the capacitor legs?

What about the phase wire connections? Some other uses had them break under the shrink wrap, so maybe worth removing the shrink if you cant find anything else loose.
```

---
## \#29 Posted by: skatardude10 Posted at: 2018-11-26T04:44:08.018Z Reads: 41

```
I've had this problem lately... More and more... 

I'm thinking about looking for loose connections and resoldering if I find any, and glopping a ton of e6000 for vibration damping for good measure.

I did that to my boost converter, but not the mosfets. Guess what failed due to vibration? The one mosfet I didn't glop e6000 on. Resoldered and glopped it up, and all is well. Maybe my vescs need the same sort of love.
```

---
## \#30 Posted by: bobbobman Posted at: 2018-11-27T22:22:45.616Z Reads: 37

```
Even running it in FOC?
```

---
## \#31 Posted by: bobbobman Posted at: 2018-11-27T22:23:21.735Z Reads: 38

```
Yeah, I've checked all those connections, though probably not as closely as I should. So frustrating. I'll double check it.
```

---
