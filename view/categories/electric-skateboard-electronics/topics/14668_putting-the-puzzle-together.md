# Putting the puzzle together

### Replies: 25 Views: 2358

## \#1 Posted by: dedinski Posted at: 2016-12-14T17:05:33.086Z Reads: 142

```
Im really excited about my build, recently a friend made me a custom made deck and all the parts have finally arrived. 

These are the parts and I made a diagram. I have poor knowledge in electronics, can you guys check if what if this wiring will work?<img src="/uploads/db1493/original/3X/7/1/713849e2591c3416386d58fa66e0090fbcbd4a7c.jpg" width="375" height="499"><img src="/uploads/db1493/original/3X/4/7/47688297af7027affe65c67edff7edf54c004be2.jpg" width="666" height="499"><img src="/uploads/db1493/original/3X/6/5/6504eec755789628f38843bd435eede6659146a7.jpg" width="374" height="500">
```

---
## \#2 Posted by: laurnts Posted at: 2016-12-14T17:42:56.315Z Reads: 124

```
Correct!

Just pleaseeee be very careful when working on the lipo battery connections.
Never CUT BOTH WIRES together, work one polarity at one time. Make sure to shrink wrap before cutting loose the other polarity.
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-12-14T17:51:44.399Z Reads: 119

```
Exactly what he said, wrap some tape around the lead you're not working on so they don't accidentally touch. I welded my scissors together by mistake my first time...
```

---
## \#4 Posted by: Tuomalar Posted at: 2016-12-14T18:15:20.932Z Reads: 118

```
Upvote for welded scissors :smiley:
```

---
## \#5 Posted by: dedinski Posted at: 2016-12-14T18:27:05.505Z Reads: 116

```
Awesome, thanks for the help. 

I saw that "slippy" made a 3d printed pull with a rope for the antispark. Is it supposed to be used in this way and should i make it accessible at every moment?
```

---
## \#6 Posted by: sl33py Posted at: 2016-12-14T18:35:06.265Z Reads: 112

```
[quote="dedinski, post:5, topic:14668"]
I saw that "slippy" made a 3d printed pull with a rope for the antispark. Is it supposed to be used in this way and should i make it accessible at every moment?
[/quote]


am i "slippy"?  I did a basic "how-to" for an XT-90 anti-spark loop key:
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

No 3d printed parts, and the small paracord pull tab was simply to make it easier to disconnect, and easier to spot if dropped (yellow w/ reflective in rope).  

as for accessible at any moment - that's not the intent, but w/ some ingenuity you can do this.  This is a simple on/off (really an interrupt) with anti-spark built-in.  cheap/simple.  If you want an emergency stop you'll need to make it reachable on your board - or connect it to yourself when riding.  Problem with that is anytime you jump off you'll disconnect power, or have a tripping hazard (depending how you set it up).  I would rather stick to a simple on/off personally and not have a tripping hazard (falling sucks especially as tall as i am - a long way down!)

HTH - GL!
```

---
## \#7 Posted by: mason Posted at: 2016-12-14T18:53:35.156Z Reads: 95

```
be very, very careful when dealing with the batteries. other than that, looks good :thumbsup:
```

---
## \#8 Posted by: dedinski Posted at: 2016-12-14T19:05:59.522Z Reads: 96

```
Haha, sorry for getting your name wrong, I guess it can be a compliment depending on the context. 

I mixed it up with this 3d printed model. I guess it was made after your design
http://www.thingiverse.com/thing:1558717
```

---
## \#9 Posted by: dedinski Posted at: 2016-12-14T19:08:27.096Z Reads: 96

```
I still have an open doubt on where to open the circuit to recharge the batteries? On the antispark I guess would be the best?
```

---
## \#10 Posted by: jmasta Posted at: 2016-12-14T20:52:33.181Z Reads: 92

```
Those HXT connectors are perfect for wiring lipos in series.  Take a razor blade and carefully cut the connector in half down the middle, to split the positive and negative battery leads.  This basically splits the HXT connector into two 4mm bullet connectors with protective covers.  Then you can directly plug A+ into B- to form the series connection.  The leads of the battery pack are now A- and B+.  You can make a harness with HXT 4mm bullets on one end and XT-90S on the other to plug directly into the VESC

<img src="/uploads/db1493/original/3X/f/f/ff73ece4064eae5eea55dee9b159bd94a4b1ab46.jpg" width="666" height="500">
```

---
## \#11 Posted by: sl33py Posted at: 2016-12-14T21:32:33.903Z Reads: 85

```
[quote="dedinski, post:8, topic:14668"]
Haha, sorry for getting your name wrong,
[/quote]

I've been called worse...:wink: no worries!

@FLATLINEcustoms - that's his bracket and super awesome IF YOU HAVE A DROP THROUGH DECK!  Then there are quite a few other challenges around motor mounts and motor clearance, etc.  This still wouldn't really be an emergency interrupt without some sort of connection to your shoe/leg/etc.  Still something i'd avoid as a tripping hazard and it's not unusual for me to jump off - i wouldn't want to lose power every time personally.

a loop key won't let you charge - unless you do two.  You are only inline w/ the + or -, so it won't be a charging connector.  Or you'll need another port that connects to both + and - "behind" the loop key if you want to do this. 

Looking at your batteries pictured - two 3s in series for 6s - you'll want 3s to 6s balance plug adapters too if you want to have one connector for the balance plug, and the one for charging.

Here's my rough quick sketch - hope it makes sense and you can read my quick scrawl:
[img]https://goo.gl/wOPDi8[/img]

I would have both the 6s balance and charging plug on the same side.  It should be "behind" or on the battery side of the loop-key/disconnect (so your VESC isn't powered when charging).

HTH - GL!
```

---
## \#12 Posted by: dedinski Posted at: 2016-12-16T21:58:54.172Z Reads: 73

```
Well, that moment when you feel like you just conquered the world was right before I sat down and connected everything. So now I need your help again. Heres what happened and I dont know why....PICS


<img src="/uploads/db1493/original/3X/6/a/6a7a1feaa9929bfa66ef20fd3979eb1fe030d70c.jpg" width="375" height="499"><img src="/uploads/db1493/original/3X/4/4/44a1d976658f05c7a09c887a9ff7a4e0832eb704.jpg" width="375" height="499">

I got a spark on the xt60(pic2) when I was connecting the battery packs (connected together 6s/24v as on the pic1) to the VESC. Can you guys assume where the problem is?
```

---
## \#13 Posted by: laurnts Posted at: 2016-12-16T23:09:06.806Z Reads: 69

```
Spark is normal as long as the vesc is powered up and the wiring is correct. Thats why some of use anti spark xt90 for loop key.

The spark caused by high amp draw from the vesc capacitors.
```

---
## \#14 Posted by: laurnts Posted at: 2016-12-16T23:12:12.830Z Reads: 68

```
cant see from phto clearly, make sure black wire goes to negative side of xt60 and red wire positive side of xt60.
```

---
## \#15 Posted by: dedinski Posted at: 2016-12-17T13:56:07.123Z Reads: 60

```
Thanks a lot for the help, I just finished setting it up! Pics soon :smiley:
```

---
## \#16 Posted by: dedinski Posted at: 2017-01-12T18:07:10.679Z Reads: 62

```
So I manged to figure out how to put it together, but still have a bit of a problem. I did not finish the circuit completely, but have put the main parts to see how it acts. 

In the end I will add pics that might explain my problem better.

Problems
1. "bad detection result received"  when running a 2.18 fw
2. the motor doesent seem to give as much power as expected. 

1. What does this step give me and do I need extra hardware to flash/upgrade like on youtube?
2. I did make the setup as instructed on youtube, and it has decent power, but I dont believe it will manage an uphill ride. Also it needs a push to get going and its relatively easily stopped by hand when upside down especially if the motor is cold (video). I did however try it only around the house since its freezing outside...
3. Could making it 9s help?

Heres some pics and snips

<img src="/uploads/db1493/original/3X/0/1/010c210cfd20ecfbfd7159e4d11df81fb2b88baa.JPG" width="690" height="410"><img src="/uploads/db1493/original/3X/9/3/93d1618a5d23a94836b886891109f901b08b7a78.JPG" width="690" height="424"><img src="/uploads/db1493/original/3X/0/a/0a3a689602c08a53f3a02fdd2e0c6430e305f841.JPG" width="690" height="356"><img src="/uploads/db1493/original/3X/1/0/105420986f41a01549f51608113755d3593fdc71.JPG" width="690" height="405"><img src="/uploads/db1493/original/3X/f/4/f467d652f4e092eec3dd71dd21ad9b40434052f5.JPG" width="690" height="382"><img src="/uploads/db1493/original/3X/e/d/ed32d5b5b5f7a501a325c15e408529d2fe7f6f41.jpg" width="375" height="499">
```

---
## \#17 Posted by: Ackmaniac Posted at: 2017-01-12T19:20:32.658Z Reads: 53

```
If i saw it right you have a 6S battery. 

6S * 3,7V * 25A max battery = 555 Watts.
Just set the max battery amps to 60 or even 80 and the motor max to 80A.
That will make it much more powerful.
6S * 3,7V * 60A max battery = 1332Watts.

Also disapble the "Send status over CAN" for your single drive
```

---
## \#18 Posted by: dedinski Posted at: 2017-01-13T12:58:37.124Z Reads: 48

```
I put it both to 80 and tweaked the mount a bit so i got 15k rpm.

The board will not move by itself, especially with my weight on top (80kg). It seems to go ok with a slight push, but it has to do better than that from what i saw on the videos. 

How relevant is this motor detection failure? Im on firmware 2.18, i dont know upgrading would resolve the problem and evenutally lead to better performance? 

Any other ideas?
```

---
## \#19 Posted by: Ackmaniac Posted at: 2017-01-13T13:09:47.817Z Reads: 46

```
The board won't move by itself because you have no sensors. So the VESC doesn't know where the exact motor position is at a stand still. So you have to give it a little push.
And please post a Screenshot from your ppm tab.
```

---
## \#20 Posted by: dedinski Posted at: 2017-01-13T13:17:29.500Z Reads: 45

```
<img src="/uploads/db1493/original/3X/4/c/4cbe8eae77f74404d33b0d98e514b5d1211c3864.JPG" width="690" height="407">
```

---
## \#21 Posted by: Ackmaniac Posted at: 2017-01-13T14:08:23.339Z Reads: 40

```
Looks like your minimum and maximum pulse width is not adjusted yet. Please check in the forum how to set them properly. But that is also no explanation for the drop outs during breaking.
```

---
## \#22 Posted by: dedinski Posted at: 2017-01-13T14:17:12.450Z Reads: 42

```
I did adjust them, at some point I put it on 0,9 and 1,9. The strange thing after leaving it at that setting was when the remote was set to "off" the motor would go full power forward :confused:

Im not sure what you mean by drop outs during breaking, I wasnt breaking during the test? I also noticed that its much harder to spin the motor when the remote is on and Im not adding speed...
```

---
## \#23 Posted by: Ackmaniac Posted at: 2017-01-13T14:33:39.276Z Reads: 42

```
You have to enable the display check box. Then move the throttle completely forward and backward and check the valuesin the box with the label Pulsewidth (ms). Set the lowest as minimum and the highest as maximum. Then write the settings and check afterwards what % the display shows. When the throttle is in idle it should be at 50%. If it is not you have to adjust the minimum and maximum. So that it is at 50% when in idle. Always when you make changes write the settings first and then check the percentage of the display box.
Sounds complicated but give yourself some time and try to understand how it works.
```

---
## \#24 Posted by: dedinski Posted at: 2017-01-17T20:18:05.926Z Reads: 35

```
Does this chart work in my case? I calculated cutoff start 21 and cutoff end 19,8. With these settings the skateboard is now really overpowered (id actually like to downpower it), but also it manages to get motor detection unlike with 33/30 setting.

 Is this safe for the circuit to leave it at this? 

<img src="/uploads/db1493/original/3X/6/b/6ba8b9c4bed13ed7b2b81e8be1f08bc94adae5a3.JPG" width="690" height="339">
```

---
## \#25 Posted by: dedinski Posted at: 2017-01-19T01:04:32.260Z Reads: 31

```
I really need some info on battery cut-off start/end.

 Are they 33/30 respectively for any motor/battery combination or can this number vary?
```

---
