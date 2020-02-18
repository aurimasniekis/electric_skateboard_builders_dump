# Rewinding 90mm hub motor

### Replies: 32 Views: 1175

## \#1 Posted by: MiniChopper4Me Posted at: 2019-01-10T16:28:50.239Z Reads: 217

```
I figured I'd create a new topic to document my project instead of continuing to hijack the 105mm thread.

I decided to rewind the SkullboardVIP motors since they were so problematic.  They are very similar to the Maxfind motors:
24N28P
Maxfind version: 6 turns of 14 strands of .30mm diameter wire (approx. 28.5 gauge), outer wheel diameter 90mm, wye termination, winding scheme AabBCcaABbcCAabBCcaABbcC
Skullboard version: 8 turns of 10 strands of .30mm diameter wire, outer wheel diameter 105mm, wye termination, winding scheme AabBCcaABbcCAabBCcaABbcC
![Original%20winding|690x335](upload://yL4PifqxAoBwoXElwin6JQuN876.jpeg) 

I completed rewiring of 2 motors with:
10 turns of 3 strands of 21AWG, outer wheel diameter 105mm, wye termination, winding scheme A-b-C-a-B-c-;A-b-C-a-B-c-
![New%20winding|690x361](upload://hV7Mb2RGqD5S0knSWA4STfoEz4D.jpeg) 
Tools used:
192ft. of 21AWG magnet wire
Latex gloves, leather gloves
Magnet wire stripping tool
Heat gun
Jeweler's screwdriver (flat)
Toothpicks
Plastic credit card cut in half
Short flat square-nose pliers
30-min epoxy
Soldering iron and soldering tools
Heat shrink, various sizes

I began by disassembling the motors.  Get the stator out of the hub using pressure, not hitting it.  It helps to heat the the hub lightly using the heat gun to make it expand some so that the bearings release easier.  Unsolder the connectors of the wires coming into the motor after documenting where everything is connected.  While wearing leather gloves, heat the sensors until the epoxy softens and either by pulling on the PCB the sensor is attached to or prying it lightly with a sharp flat instrument (I used a jeweler's screwdriver). Beware, the stator will become quite hot.  This is what you're wearing leather gloves for.  Complete releasing all 3 sensors this way so that you can set the PCB aside, along with the plastic guard protecting the wires coming into the motor and the connector itself.  Remove the heatshrink protected connection and cut off the soldered part.  You'll need to do this in order to unwind the motor.  Begin removing the windings carefully, trying not to damage the green protective covering on the stator.  If you examine the windings carefully and remove them in the correct order, this will be quite easy.

Cut all of the segments of wire at one time in order to assure they are all the same length.  I cut them at 64" lengths.  This left 2-3 inches of wire at the beginning and end of each phase.  If you want to simply run the wires (all 6 wire starts) out of the motor and direct to your ESC, account for the additional wire length at this point and make your wire lengths longer.
I began winding the first phase A at the 6th slot CCW from the first sensor position.  This became crucial in having enough room for placing the PCB back in and making all the necessary connections later. I completed all windings wearing a latex glove on the winding hand to get better grip for pulling the wires.  Start winding from the middle to the outside, complete 4 turns.  This will cover the tooth.  At the completion of the 4th turn, insert the credit card pieces into each side of the tooth you are winding, and squeeze the ends using the pliers, but gently.  This is to flatten the windings without damaging them. On turn 5, you will have 1 wire on the inner part, and 2 on the outer part.  If you need to move the windings around, use your nails, or plastic tools.
![Wind%205|470x253](upload://tAhpTxBSM5yCZ9suXd5dY3egHax.jpeg) 
For windings 6-8, I found the best way to be stitching the wire into position one strand at a time. It gets tight at the end of turn 8. After completing turn 8, I repeated the squeezing process, but note that getting the cards in is much more difficult now than after turn 4.  You only need to squeeze the outer edge of the turns to make room for turns 9 and 10. Starting turn 9, you'll create a \ on the tooth, so I did that on the side of the stator with the connections going out, as there is more room on this side of the stator. Once turn 10 is complete, you'll need to jump 2 teeth and start the next winding.  Be careful to run the wire as carefully as possible making it look like in the diagram so that its out of the way when you go to wind the next phase.  When all phases are complete, use the stripping tool to remove expose the ends of each of the wires.  You can now test to ensure none of the wires are shorting out to the stator or to each other.  You can now arrange the phase ends where you want them to end up (see completed winding for specifics) so that you can cut them, re-strip the ends the minimum necessary, and solder them together.  I soldered the phase ends in 2 bundles.  They do not all need to be together in one bundle for the motor to work.  I then did the same thing for the matching phases of each half together (A from the first half to A from the second half, etc.).  I could not get the connections to fit into the PCB cutouts for the phase ends, so I cut off that portion of the PCB.  I then re-glued the sensors into their spots using epoxy and left it overnight to harden.

All that remains is to reconnect the outgoing connector and run it through the provided channel.  End result is 113kv

![image|666x500](upload://9G0VUUmTpJYSXyZ41bYUwJUoXoS.jpeg) ![image|666x500](upload://wzXq2a4BiRzllWEFq6tymyHEZZJ.jpeg) ![image|666x500](upload://1DGT8AYYKrEMcxzoZvloYSGJY2b.jpeg) ![image|375x500](upload://qKG83CECAaHTuAGVOuO2g6YMh8d.jpeg) ![image|375x500](upload://fM95B26hVkw8gaI478x9gvj6wH9.jpeg) ![image|375x500](upload://lkxsRjxun2Pj0Jzl8MdH02FSNLp.jpeg) ![image|375x500](upload://kfLPO8RajusuvqI4lhkrdvlns8t.jpeg) ![image|375x500](upload://pZieZyaZWAqdfmJmsBdGmd8XSm2.jpeg) ![image|375x500](upload://dkVGC5aQSVALppIT5Lu2rO6XW0O.jpeg) ![image|375x500](upload://jYrBcaKDTyWqXdXUc3GBTYtPf6i.jpeg) ![image|375x500](upload://mMMdPSM4g6LRVVE0aiafS9obSE9.jpeg) ![image|375x500](upload://im2okLQPFp8rumexagrBW1w1ms1.jpeg) ![image|375x500](upload://sJiQbJirrv5HV2QP6EHnIIKgis6.jpeg) ![image|375x500](upload://kuxVJROGD8d0HBSusP754PWczkD.jpeg) ![image|375x500](upload://5anYjqvklVaUkB7bmxBiSNsBsKs.jpeg)
```

---
## \#2 Posted by: MiniChopper4Me Posted at: 2019-01-10T16:47:52.193Z Reads: 169

```
![image|375x500](upload://2fwvvofGS3eNf5jNXgf5gpOqryB.jpeg)
Completed rewinding, outer connections to be done
```

---
## \#3 Posted by: MiniChopper4Me Posted at: 2019-01-10T22:12:06.698Z Reads: 149

```
@myreala @donta42 this thread's for you!
```

---
## \#4 Posted by: MiniChopper4Me Posted at: 2019-01-10T22:20:51.074Z Reads: 152

```
So some of the calculations I made in order to arrive at my choice.

Below find the cross-sectional area of copper filled area in the airspace in each tooth using different turns/wire gauge combinations:

When I calculated the CSA of the Skullboard motor, the result was
(8 x 10 x (.15 x .15 x pi) x 2) = 11.3093355mm^2
When I calculated the CSA of the Maxfind motor, the result was
(6 x 14 x (.15 x .15 x pi) x 2) = 11.8752202mm^2

I knew that I wanted to ideally have more copper than the Maxfind motor, but definitely more than the Skullboard motor.  I worked backwards and created the below table to find the closest values to what I wanted.

5 turns
1 wire - lower 17AWG - 10.4 higher 16AWG - 13.1
2 wire - lower 20AWG - 10.36 higher 19AWG - 13.06
**3 wire - lower 22AWG - 9.78 higher 21AWG - 12.3 THIS FITS!**  
4 wire - lower 23AWG - 10.32 higher 22AWG - 13.04
5 wire - lower 24AWG - 10.25 higher 23AWG - 12.9
6 wire - lower 25AWG - 9.72 higher 24AWG - 12.3
7 wire - lower 25AWG - 11.34 higher 24AWG - 14.35
8 wire - lower 26AWG - 10.32 higher 25AWG - 12.96
9 wire - lower 26AWG - 11.61 higher 25AWG - 14.58
10 wire - lower 27AWG - 10.2 higher 26AWG - 12.9

6 turns 
1 wire - lower 18AWG - 9.876 higher 17AWG - 12.48
2 wire - lower 21AWG - 9.84 higher 20AWG - 12.432
3 wire - lower 22AWG - 11.736 higher 21AWG - 14.76
4 wire - lower 24AWG - 9.84 higher 23AWG - 12.384
5 wire - lower 25AWG - 9.72 higher 24AWG - 12.3
6 wire - lower 25AWG - 11.664 higher 24AWG - 14.76
7 wire - lower 26AWG - 10.836 higher 25AWG - 13.608
8 wire - lower 27AWG - 9.792 higher 26AWG - 12.384
9 wire - lower 27AWG - 11.016 higher 26AWG - 13.932
10 wire - lower 28AWG - 9.72 higher 27AWG - 12.24

7 turns
1 wire - lower 18AWG - 11.522 higher 17AWG - 14.56
2 wire - lower 21AWG - 11.48 higher 20AWG - 14.504
3 wire - lower 23AWG - 10.836 higher 22AWG - 13.692
4 wire - lower 24AWG - 11.48 higher 23AWG - 14.448
5 wire - lower 25AWG - 11.34 higher 24AWG - 14.35
6 wire - lower 26AWG - 10.836 higher 25AWG - 13.608
7 wire - lower 27AWG - 9.996 higher 26AWG - 12.642
8 wire - lower 27AWG - 11.424 higher 26AWG - 14.448

8 turns
1 wire - lower 19AWG - 10.448 higher 18AWG - 13.168
2 wire - lower 22AWG - 10.432 higher 21AWG - 13.12
3 wire - lower 24AWG - 9.84 higher 23AWG - 12.384
4 wire - lower 25AWG - 10.368 higher 24AWG - 13.12
5 wire - lower 26AWG - 10.32 higher 25AWG - 12.96
6 wire - lower 27AWG - 9.792 higher 26AWG - 12.384
7 wire - lower 27AWG - 11.424 higher 26AWG - 14.448
8 wire - lower 28AWG - 10.368 higher 27AWG - 13.056

9 turns
1 wire - lower 19AWG - 11.754 higher 18AWG - 14.814
2 wire - lower 22AWG - 11.736 higher 21AWG - 14.76
3 wire - lower 24AWG - 11.07 higher 23AWG - 13.932
4 wire - lower 25AWG - 11.664 higher 24AWG - 14.76
5 wire - lower 26AWG - 11.61 higher 25AWG - 14.58
6 wire - lower 27AWG - 11.016 higher 26AWG - 13.932
7 wire - lower 28AWG - 10.206 higher 27AWG - 12.852
```

---
## \#5 Posted by: donta42 Posted at: 2019-01-10T22:30:05.460Z Reads: 128

```
Dude - NICE WORK!!!!!!

Are you running them with VESC ? Or have you tested them with the stock esc?? 

Bravo!
```

---
## \#6 Posted by: MiniChopper4Me Posted at: 2019-01-10T22:43:13.444Z Reads: 130

```
I ran the first motor using Flipsky VESC 4.2 dual on 10S, with 60A.  No cogging, no issues ON THE BENCH.  Now that motor #2 is done, I can go for a test ride.  I'm hoping the sensors on motor #2 work as well, and I'll do motor #2 sensored (motor #1 I broke the sensors while completing the rewind, so I learned how to remove them for motor #2).  I don't know how sensitive the sealed ESCs are to changes, but since I changed the number of windings, I doubt it would work "right".  You could always rewind it with the same # of turns just different gauge wire and get rid of the efficiency (motor heating and poor battery consumption) problems.  I think if you did that, you'd be able to drive it with the stock ESC.
```

---
## \#7 Posted by: donta42 Posted at: 2019-01-10T22:47:01.336Z Reads: 128

```
Looking forward to seeing it in action!
```

---
## \#8 Posted by: Minim Posted at: 2019-01-10T23:03:57.709Z Reads: 124

```
Ooooh bookmarked! I have a raptor 2 motor with bad windings due to a screw hitting the end. I think I need to rewind it and it looks very similar to yours. Is it a difficult job for someone who never did it before?  

 ![DSC04535|690x460](upload://sok4nb6S7WPcTRt5pldNhwQR610.jpeg)
```

---
## \#9 Posted by: MiniChopper4Me Posted at: 2019-01-10T23:10:37.165Z Reads: 122

```
I did it, and I had never done it before, so I think its definitely doable even for a first-timer. Be warned though, its not easy or quick.  Each phase took me roughly 90 mins to complete.

However, you need a fair value's worth of tools in order to accomplish it, including one I bought just for this job (magnet wire stripper, $50).

Make sure you can easily source the same wire your motor is wound with.  My motor was originally wound with a non-AWG wire (.30mm diameter wire maybe commonly used in China, but not something I looked into).  However, I wanted to use thicker wire anyways, so that requires calculations in order to determine.
```

---
## \#10 Posted by: myreala Posted at: 2019-01-11T01:02:18.525Z Reads: 119

```
Great work man, can't wait to see your results. Definitely following this thread. If the results make it look like it was worth it, this would make a great and fun project.
```

---
## \#11 Posted by: MiniChopper4Me Posted at: 2019-01-11T03:16:11.377Z Reads: 108

```
Thanks for all the support! I’d wanted to try rewinding a motor since my RC days, but never got around to it, mostly because the motors were so small.  I finally had the chance to do it with a beefy motor.  It was not easy by a longshot, but I am glad I finally tried it. Learned quite alot!
```

---
## \#12 Posted by: MiniChopper4Me Posted at: 2019-01-12T18:24:17.719Z Reads: 96

```
I took it for a test ride this morning.  Its working fine, but there is a big lack of torque.  It did get up to speed, eventually, and its running quiet, plus after a 5 mile ride, the motors are not too hot to touch.  The 2nd motor definitely came out better than the first, sensors notwithstanding.  Going to take it for another ride with 60 -60 60 -40 instead of 40 -40 40 -30 like the first test.

I may need to do this again, with 15 turns instead of 10.  With what I've learned so far, it shouldn't be too difficult, plus I'll have better torque instead of ludicrous top speed.  This time I'll run the leads all the way out of the motor to avoid having to make a junction inside.
```

---
## \#13 Posted by: myreala Posted at: 2019-01-14T00:45:47.836Z Reads: 91

```
Ah that sucks man, lets hope your second attempt goes better, btw did you consider cutting out the leftover parts of the stator so you can get more copper on the ones you are using?
```

---
## \#14 Posted by: murdomeek Posted at: 2019-01-14T00:54:26.975Z Reads: 91

```
whats the specs of the motor after the rewinding?
(kv, power, etc)
```

---
## \#15 Posted by: MiniChopper4Me Posted at: 2019-01-14T01:06:45.374Z Reads: 87

```
I don't think it works that way.  I didn't just skip those teeth, its just another method of winding, LRK versus dLRK.
```

---
## \#16 Posted by: MiniChopper4Me Posted at: 2019-01-14T01:08:06.825Z Reads: 88

```
kv is 113, but it lacks torque at low speed.  I was able to pump 50 amps through it though.  The other winding did not take more than 30.  I'm considering either rewinding with 14 or 15 turns.
```

---
## \#17 Posted by: myreala Posted at: 2019-01-14T02:14:05.687Z Reads: 86

```
Huh, did not know that. Yeah torque issue is probably because of high kv never seen above 90 for a direct drive or hub motors, Ideal would probably be around 70.
```

---
## \#18 Posted by: MiniChopper4Me Posted at: 2019-03-13T16:07:32.082Z Reads: 81

```
So I completed the second rewind of the motors!

I went with the same wind pattern, but 15 turns with 2 * 21AWG instead of 10 turns of 3 * 21AWG.  This time I went all out and replaced all the sensors as well, and ran the leads a little long so that I could run them all the way out to the VESCs instead of having to wire in a joint in the motors.  They run surprisingly quiet and do not heat up, although if I were to do it again, I would go even more turns to give them a little more power.

My tests today were using:
30 motor power
-30 motor brake
20 battery draw
-10 battery regen

I rode 4 miles and at the end of the ride, the motors were warm to the touch.  I could hold my fingers on them and not have to pull them away.  My top speed was 22mph, and I weigh 190lbs.

I found possible reasons for vibration issues reported by different people.  The hubs and motors are not manufactured with any semblance of QC.  I found 2 of each of the 4 motors and wheels I have to be off-center, and totally unbalanced.  I had to add lead tape in large amounts in order to make up for the terrible offset and get the wheels stop making the whole board shake.

I need to make a portable battery checker like @MManer so that I can check how much battery I've used before and after a ride to confirm what I imagine to be the case, that there is no longer any issue with these motors running down the battery.  I think that this was due to the terrible copper-fill in the motors, something I managed to improve drastically with the rewind.

Again, if I were to do it again, something that's not very likely to happen, I would probably go with 18-20 turns and see what I got as a result, but as it stands I'm quite satisfied with the results.  This will make a great second board for sharing with my nieces/nephews to ride on the beach boardwalk etc.  I'll focus my attention on other projects now.
```

---
## \#19 Posted by: rey8801 Posted at: 2019-03-13T16:27:55.916Z Reads: 76

```
[quote="MiniChopper4Me, post:1, topic:80491"]
make
[/quote]

Hi. Did you never measure the stator size. Meaning the steel part in diameter and lenght? 
Like this
![IMG_20190309_003120|690x388](upload://kqzZfZUB5TFXkXnvWmQ4B4dcwTS.jpeg) ![IMG_20190309_003157|281x500](upload://toXKfy1H2Sgbjlb6xmQfWIWAZw9.jpeg)
```

---
## \#20 Posted by: MiniChopper4Me Posted at: 2019-03-13T17:33:49.954Z Reads: 69

```
![image|375x500](upload://l3fyuNW9Bh7eeOCrjCO1HingmQR.jpeg) ![image|666x500](upload://4chMQXXLGO9uaB6Bbm3DiHTq96g.jpeg)
@rey8801
```

---
## \#21 Posted by: rey8801 Posted at: 2019-03-13T17:39:54.920Z Reads: 66

```
Thanks man! Are those Raptor or what?
```

---
## \#22 Posted by: MiniChopper4Me Posted at: 2019-03-13T17:40:57.100Z Reads: 67

```
They are SkullboardVIPs, but exactly the same stator as Maxfind motors.  The aluminum "shaft" is different length.
```

---
## \#23 Posted by: rey8801 Posted at: 2019-03-13T17:41:31.162Z Reads: 68

```
Ah ok. They look a bit too small to be a raptor. I got confused from you precious statement above

Ah no I was refering to @Minim 's pic.
```

---
## \#24 Posted by: MiniChopper4Me Posted at: 2019-03-13T17:42:41.641Z Reads: 66

```
Someone in this thread asked about rewinding Raptor motors.  I've been working with Maxfind/Skullboard motors from the start :slight_smile:
```

---
## \#25 Posted by: rey8801 Posted at: 2019-03-13T17:43:10.660Z Reads: 66

```
Yes my bad. Thanks for the insight.
```

---
## \#26 Posted by: MiniChopper4Me Posted at: 2019-03-13T17:54:08.672Z Reads: 67

```
As I mentioned to @Minim as well, I wouldn't be scared of rewinding the Raptor motor (now, with what I've learned ;) ) but I wouldn't call it easy to do either.  Especially trying to get better copper fill and/or changing the wire gauge.  I'd suspect the Raptor motors are pretty well engineered as is.  With these crappy ex-fan motors, just taking them apart illustrated just how poorly engineered they were, and quite easy for even a first-timer like me to improve.

I tried a couple of times to rewind using the same pattern as in the Raptor motor, with each strand going around the entire motor, half the number of turns on one tooth, half on the neighboring tooth, but it was alot more difficult to figure out how to do it, especially by hand.  I gave up and went with what I used.  Easier for sure.
```

---
## \#27 Posted by: rey8801 Posted at: 2019-03-13T18:02:49.494Z Reads: 61

```
I think rewind a Raptor hubs would be as difficult as yours. You would manage for sure. I was interested in knowing the stator size.
```

---
## \#28 Posted by: MiniChopper4Me Posted at: 2019-03-13T22:52:45.819Z Reads: 57

```
Ok, so starting with a 42.0V battery (Samsung 30Q 10S4P), riding 4.6 miles at an average speed of 14.7mph, top speed 22.2mph, left me at 39.4V and a temp reading on the motors of 60C.  I'd say this was a successful test of range and that the motor/wheel problems are solved with the rewinding.![image|281x500](upload://4g6hc8CB8JaTtMd6grZ2FFrzPOF.jpeg)
```

---
## \#29 Posted by: MiniChopper4Me Posted at: 2019-03-13T22:55:11.873Z Reads: 55

```
I love to be able to tell people now, "I made my own motors".  Not entirely true, but moreso than not :smiley:
```

---
## \#30 Posted by: MiniChopper4Me Posted at: 2019-03-13T23:01:44.235Z Reads: 56

```
@murdomeek I get at WOT on the bench 4133 rpm on a 10S battery.  This is supposed to be 112kv, but this didn't appear to change when I rewound from the first time.  I don't know what I might be doing wrong with my testing, but I'm happier with the results this second time around with performance, power, heat, and battery life.

I can't think of a way to do the drill press method with these motors, not to mention I don't own a drill press :stuck_out_tongue:
```

---
## \#31 Posted by: rollinsoul Posted at: 2019-04-16T16:56:14.634Z Reads: 48

```
Wow. Great work. I have said skullboard dud hubs. Been waiting for version 2 to arrive. Love how the handle in the wet, hate how sluggish and inefficient they are. If they don't come out with version 2 I'll definitely will try your mod. Thanks again for the great work.
```

---
## \#32 Posted by: MiniChopper4Me Posted at: 2019-08-01T21:08:42.803Z Reads: 31

```
Update:

These are still going strong.  I since discovered some issues I was having was due to the battery I bought having the discharge hooked up despite specifically having asked for it to be bypassed.  Also had the Flipsky 4.2 dual repaired by @JohnnyMeduse.

I got ~11 miles with ~25% battery left yesterday, one long non-stop ride.
[https://metr.at/r/UlLLo](https://metr.at/r/UlLLo)
```

---
