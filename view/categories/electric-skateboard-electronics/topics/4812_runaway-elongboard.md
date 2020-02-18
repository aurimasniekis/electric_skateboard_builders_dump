# Runaway elongboard!

### Replies: 22 Views: 2947

## \#1 Posted by: DougM Posted at: 2016-06-17T15:09:06.721Z Reads: 345

```
Well, I had a full-fledged runaway last night.  I was riding my board on a stretch of bike trail and had been riding for about 30 minutes when suddenly the board stopped responding to the controller and started slowly accelerating.  

At the time I was going about 20mph (guess) I knew that if the board continued to accelerate there was no way I was going to be able to get off it and stay on my feet.  To my right was a chain link fence and to my left a ditch full of brambles - no good places to bail.  I had not been on this trail before so I had no idea what was ahead.

Miraculously I was able to jump off the board and stay on my feet.  The board took off, hit the fence once, bounced back onto the trail, went another 50 feet and hit the fence again, this time coming to a stop, motor still spinning.

Total damage was a severely bruised heel, a broken headlight, a big noogie taken out of one of the front rails and the display got ripped off the control board.  When I re-powered the system the control board was completely dead but the VESC came up blue and green lights.  Of course nothing worked and I had to push back to the car.

I will dig into forensics this weekend and will post what I find here, but 3 things:

1: if anyone knows Vedder's email addy let him know that in firmware 2.18 there might be a code path that allows the motor to continue to run (and in fact accelerate) even though a signal is no longer there (in my case a serial signal)  It is of course also possible that the fault lay in the code in my control board, but I believe the board was offline when the event occurred.

2: never build a board that goes faster than you can run.  I'm going to gear this board down.

3: I'm going to start working on a power switch that can be accessed from the top of the board by stepping on it - similar to emergency cutoff mushroom buttons on manufacturing equipment.

4. this sport isn't so innocent as I thought it was.  I was wearing a bike helmet but...

DougM
```

---
## \#2 Posted by: Blasto Posted at: 2016-06-17T15:14:32.391Z Reads: 322

```
I had this happen to me a few times with the nunchuck... dam remote would turn off while accelerating and continued accelerating. needless to say I'm running with the gt2b now, flawless, appart from not having any cruise.

what remote you were using?
```

---
## \#3 Posted by: DougM Posted at: 2016-06-17T15:17:51.529Z Reads: 319

```
It's a custom home-built remote so it's entirely possible that the control board was continuing to send serial messages even though it was not reading the remote.  There is quite a bit of code in there to check the connection state but I will be scouring it again.

This is where a log would be nice.

DougM
```

---
## \#4 Posted by: Hummie Posted at: 2016-06-17T15:26:12.739Z Reads: 297

```
Many times I have my board decide to accelerate or stop because of a bad connection between the receiver and esc.  A loose connection between the two with many different receivers has done this to me
```

---
## \#5 Posted by: DougM Posted at: 2016-06-17T15:30:54.015Z Reads: 292

```
Was this using VESC or something else?  Sounds like this happens a lot more than I thought!!!

DougM
```

---
## \#6 Posted by: Jeff Posted at: 2016-06-17T15:35:17.928Z Reads: 280

```
I run a gt2b and have never had any issues. I can even turn the remote off while riding and the VESC will just coast the board to a stop.
```

---
## \#7 Posted by: barajabali Posted at: 2016-06-17T15:48:26.045Z Reads: 268

```
Oh man the detail was excruciating.... 
I'm sorry for your loss buddy.
```

---
## \#8 Posted by: treenutter Posted at: 2016-06-17T17:04:31.445Z Reads: 250

```
I've had the same experience as @Jeff with GT2B... not a single problem with it ever. For all I've read and experimented with, I won't use anything but GT2B until another proven and reliable controller is available. Losing control is too dangerous. Sorry you had to experience it @DougM! Glad you're OK!
```

---
## \#9 Posted by: flatsp0t Posted at: 2016-06-17T18:22:49.384Z Reads: 243

```
I thought of a system with a loop key and some rope attatched to me, so if me and the board separate it will cut power.
```

---
## \#10 Posted by: Kaly Posted at: 2016-06-17T18:28:01.098Z Reads: 242

```
I stop using the wiiceiver for that same reason. ( NYC intersection + runaway board ) was lucky enough that the light changed to green on my direction. 
 I most to have been going almost 30mph. :poop: :poop:   After that just 2.4ghz remote for me.
```

---
## \#11 Posted by: Hillso Posted at: 2016-06-17T18:39:55.817Z Reads: 240

```
bluetooth is also 2.4 :slight_smile:
```

---
## \#12 Posted by: Kaly Posted at: 2016-06-17T18:46:53.265Z Reads: 240

```
Yes, it is 2.4 ghz 

but the way of implementing the comunication is different. A Rc remote is more secure for this type of connection and is less suceptible to interference from cell towers and other sources.
```

---
## \#13 Posted by: DougM Posted at: 2016-06-17T23:32:08.149Z Reads: 233

```
Ok, a little more information.

My control system is driven by a Teensy 3.2.  When I powered up the board today that control system was dark - no LEDs.  I tested the 5V rail at 5V, but the 3.3v rail was about 1.1v.  I removed the Teensy and the power LED and XBee connect LED immediately came up.  This means the Teensy died.

I replaced the Teensy with a new one and the board came back to life immediately.  All control was perfect except, obviously the smashed headlight.

I think the Teensy failure was caused by static.  It is very close to the front tires (which are rubber) and not enclosed in any way.

So the Teensy died catastrophically, pulling the control system down.  This means that no amount of software controls were going to make any difference at all - that the runaway was likely at the VESC level - there is likely a code path in the VESC that does not correctly identify when messages stop arriving.  If anyone is talking to Vedder let him know that it would be very cool if in his new design he had a dedicated deadman pin - if it gets pulled low the system shuts down.

So my focus is going to be on 2 things.  The first is more static protection - so I'm going to cover the control board with a metal plate attached to the frame; and 2) a manual hard cutoff system available by stomping on the rear riser of the board.  I will post some piccies of the latter when I get it done, hopefully tomorrow.

In the longer term I might look at Vedder's anti-spark power system and see if i can integrate a hard deadman into that and offer as open source.

Also, as I said before, I'm going to gear the thing down to reduce the top speed (more torque!)

Thank you all for your support and stories.  I had no idea this happened so often.  It's a big dangerous issue.

DougM
```

---
## \#14 Posted by: Hummie Posted at: 2016-06-17T23:38:19.326Z Reads: 215

```
I doubt it's the vesc because so many people don't have trouble with it.  The fact receiver is also dead makes me think even more so it's ur receiver that's the problem. I've had it happen a couple times and the connection between the nunchuck is notorious for doing things.  I had the nunchuck going 5 minutes before decided no way.  I have the same problems I bet and I was just asking about soldering the connection...seems a solution.  A deadman switch won't solve the problems As the board could accelerate or brake really hard and you'll be so unbalanced.  Best just make it work right from the get-go I think
```

---
## \#15 Posted by: DougM Posted at: 2016-06-17T23:48:15.465Z Reads: 212

```
Well, except if the controller is dead then the VESC is no longer receiving messages and should shut down after the timeout.  I do have to check the timeout in the firmware and make sure I didn't disable it or set it to some weird number.

I'd actually prefer that this were my issue then fixing it would be in my control - which of course it is to some extent (static hardening, etc.) But we shouldn't ignore the fact that VESC might be misbehaving in a bad way in certain circumstances.

My deadman switch would be a hard power cutoff - so the board will coast to a stop.  Vedders would likely have the same behavior. 

I sent him a mail - will let you know if I get a response.

Thanks,

DougM
```

---
## \#16 Posted by: Hummie Posted at: 2016-06-17T23:53:51.502Z Reads: 199

```
What I mean is for me repeatedly the connection between a working receiver and the vesc is not good and that has sent my board off on its own or slamming on the brakes even when batteries aren't connected
```

---
## \#17 Posted by: Dedbny Posted at: 2016-06-18T00:13:09.984Z Reads: 195

```
Go the GT2B its ugly but tested by many here and reliable and predicable. Once you calibrate it its a perfect controller.
```

---
## \#18 Posted by: Hummie Posted at: 2016-06-18T00:15:47.360Z Reads: 191

```
I have a smashed gt2b transmitter from the same issue.  Poor connection from esc to receiver
```

---
## \#19 Posted by: DougM Posted at: 2016-06-18T18:02:44.781Z Reads: 185

```
update, I re-configured the gearing from 10:21 to 10:26 which isn't huge but was the biggest cog I had handy.  The rest I can control by putting in an RPM limit.  Later on when I have more time I'll cut a bigger cog so I can climb trees.

I added a metal static shield over the controller board.

I also picked up a couple of these:

https://www.amazon.com/gp/product/B0094GM004/ref=od_aui_detailpages00?ie=UTF8&psc=1

that I am going to attach to Vedder's anti-spark switch and mount on top of the rear riser so I can smash it with my foot should something go awry.

DougM
```

---
## \#20 Posted by: loose_nickers Posted at: 2016-07-19T04:33:45.286Z Reads: 150

```
https://m.reddit.com/r/ElectricSkateboarding/comments/4titl6/issues_with_enertion_vesc_diy_controller/
```

---
## \#21 Posted by: sl33py Posted at: 2016-08-22T21:10:26.094Z Reads: 121

```
[quote="DougM, post:19, topic:4812"]
I also picked up a couple of these:
[/quote]


I'd be careful with these.  It's doubtful they can handle a full single motor, let alone a dual motor, Amp load.  Rated for 10A only - so you might have a meltdown trying to run 40-60A through it.

I'd clip the loop key to your shoe or something as a kill switch - it's at least built to handle the amps needed.  Just might be difficult to do and push or even reposition your foot.

I like the idea of setting a max RPM in the VESC if gearing down doesn't reduce your top speed enough.  I might do this for my GF's board.
```

---
## \#22 Posted by: DougM Posted at: 2016-08-22T21:30:47.880Z Reads: 113

```
@sl33py I came to the same conclusion.  The buttons were actually on the low-power side of the anti-spark switch so the current wasn't an issue, but there is no way that I can pick up my back foot and push that button at 20+mph without killing myself.

So I'm focusing on hardening the controller - I put a big aluminum plate over the whole assembly, and in the new version will have TVS's on the power and control lines.

Funny story with those mushroom buttons, the switch on my drill press went bad one day so I thought I'd just swap one of those in - it melted.  so 10A is optimistic.
```

---
