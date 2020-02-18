# VESC blew up&hellip; Any ideas?!? (edit: solved)

### Replies: 21 Views: 4051

## \#1 Posted by: cmatson Posted at: 2015-09-12T22:53:39.994Z Reads: 172

```
So this is what happened as soon as I plugged my battery into the VESC... I'm guessing I'm screwed at this point, right?
I even made sure all the wires were in their specific places before plugging it in., None of them had strands hanging off that could short it out; but yet, the mystical smoke still made it's appearance. Anyone know what could've gone wrong?
<img src="/uploads/db1493/original/1X/5b14ca34c0b38269c471e853ad73551803609076.jpg" width="500" height="500"> <img src="/uploads/db1493/original/1X/20a15c4d0fbe4ca9382673bab6f89b32d99d4591.jpg" width="500" height="500">
```

---
## \#2 Posted by: onloop Posted at: 2015-09-12T23:08:31.097Z Reads: 170

```
That sucks!.

Did you try power from a low power power supply first?

Laptops power supplies are recommended, the one I use is 18v 10A.

But even lower is recommended.

I don't know what could cause this. Each unit was powered up to have firmware loaded.

Did you use the capacitor? Can really see how it's connected.
```

---
## \#3 Posted by: cmatson Posted at: 2015-09-12T23:25:27.910Z Reads: 168

```
I had no idea you had to start off with a smaller power supply... I just hooked it up to the SPACE cell because that is what I was planning to run... 

I did use the capacitor, as show by the picture. It has each of it's prongs in the wire (in the correct orientation for positive/negative), and dowsed in solder.
<img src="/uploads/db1493/original/1X/3e7cd1635c739970395c73f01a98aed193727be1.jpg" width="500" height="500">
```

---
## \#4 Posted by: cmatson Posted at: 2015-09-12T23:34:14.764Z Reads: 153

```
On another note, even after it blew up, the leds continued to work before I turned off the battery. So maybe it could just be that one mosfet that blew, and my replacing it, I could get it to work again.

Do you have any more vesc's in stock Jason? I might be ordering one before you go on your vacation... the question will be how to explain to my parents that I need to buy another one- I guess I'll have to use the "it's my money, so I can spend it however I want" tactic

**EDIT:** I realized by saying "as soon as I plugged in my battery" it was kinda misleading. I plugged it into the space cell, *and then* turned on the space cell. It blew within a second or two of being turned on: not at the exact moment it received power.
```

---
## \#5 Posted by: onloop Posted at: 2015-09-12T23:51:51.795Z Reads: 151

```
Dont worry ill credit you, It's covered under warranty.  Just go to our website, login to your account, submit RA for credit. Send it back.

You can order another one from the next batch.

Alternatively you could try to fix it. The mosfets are a few $. But maybe that's not the problem..

Looks like it shorted out somehow... maybe a solder bridge.
```

---
## \#6 Posted by: cmatson Posted at: 2015-09-13T00:05:01.848Z Reads: 145

```
ok sounds good- I also posted it up on ES, just to get some more opinions. Tomorrow I'll figure out what I'm gonna do.
```

---
## \#7 Posted by: lowGuido Posted at: 2015-09-14T00:59:58.397Z Reads: 135

```
without trying to be a jerk...  the soldering on those wires is horrible. I'd probably guess that it may have caused a short on the red wire at a glance.
it could still be salvageable..
```

---
## \#8 Posted by: cmatson Posted at: 2015-09-14T01:33:41.634Z Reads: 143

```
ya I know. 

haha it's not being a jerk, it's just a fact. I have a low end soldering iron (only 30w, so it doesn't get very hot), and I think that's part of the problem. I am going to get the one torqueboards recommended, so I don't have to worry about it anymore.

On another note just overall, I tested it today with a cheap nickel metal battery (equivalent to like a 2.5s lipo), and vesc still lights up and works. I even connected it to the desktop BLDC tool no problem. I hooked it up to my dying old 245kv motor, and the motor detection actually got the motor to sorta spin, but cogged alot in the process so it still said failed. Maybe @onloop can give some input based on this point, because it makes me feel like I just shorted out the one mosfet... but that's not something I'd really like to replace.
```

---
## \#9 Posted by: sl33py Posted at: 2015-09-14T05:31:56.868Z Reads: 137

```
@cmatson - Try checking in the BLDC tool under realtime data for errors while running it.  Also i think under the terminal tab you can type in "fault" and it will return fault codes.  Might help you figure out what specifically failed.

Here's a DRV8302 chip failure (Jamesonotc who is local to me is going to help me replace - i cannot smb solder (yet!)).
[img]/uploads/db1493/original/1X/3e03e0a085fc403658b14d4c6a0603641420586c.jpg[/img]

One other thing to note - your cap/capacitor is WAY too far away from the VESC.  You want it as close as you can physically move it to the PCB board.  All the way out by the power plug doesn't help and might have contributed.

Here's one i'll likely replace and move slightly closer:
[img]/uploads/db1493/original/1X/7f109e90d2fed51e067364f2465094a1e6b3c8cf.jpg[/img]
It's one that came on a board i bought.  Nice quality, but the solder on the caps to wires could use a little more heat (so says Vedder, so i take that as solid advice).

GL!
```

---
## \#10 Posted by: lowGuido Posted at: 2015-09-14T05:48:34.763Z Reads: 127

```
while I agree that the Cap will be more efficient if its closer to the board. having it further away won't cause your VESC to fail.
```

---
## \#11 Posted by: cmatson Posted at: 2015-09-14T10:06:53.912Z Reads: 126

```
thanks for the info Sl33py-
I'll test the VESC real time data with the BLDC tool this afternoon.
```

---
## \#12 Posted by: cmatson Posted at: 2015-09-14T20:35:46.507Z Reads: 125

```
so this is what I'm getting: it is fluctuating between the two. The motor current will also change when I hit full brake, or release. In addition, all the mosfet's are around the same temp. 
<img src="/uploads/db1493/original/1X/0329e67698a9bdf46a234046bfc2b920904fa3e2.png" width="690" height="367">  

<img src="/uploads/db1493/original/1X/d16154818e9d3166345dbb7caf7be624ed4dd11a.png" width="690" height="384"> 

<img src="/uploads/db1493/original/1X/861cb8e582640f0c6f6618e50735991694a5eb89.png" width="690" height="356">
```

---
## \#13 Posted by: sl33py Posted at: 2015-09-14T21:22:52.958Z Reads: 109

```
I don't see any errors in the "Fault code" area of the bottom left grey box...  Is the motor spinning or no?

If you go to the Terminal tab and type in "fault" what does it give you?
```

---
## \#14 Posted by: cmatson Posted at: 2015-09-14T22:18:10.835Z Reads: 110

```
I did not have my motor hooked up for the test, because yesterday with the motor it wouldn't detect it. With the enertion 190kv motor what settings do you have for motor parameters did you put in to get it to detect on your vesc? @sl33py
```

---
## \#15 Posted by: cmatson Posted at: 2015-09-14T22:40:06.414Z Reads: 110

```
I am currently uploading a video to youtube showing what is happening

edit: maybe @onloop can take a look at the video once it is up too

Video: https://youtu.be/hOnaayCZVr0
```

---
## \#16 Posted by: sl33py Posted at: 2015-09-14T23:59:13.615Z Reads: 117

```
at work so couldn't turn it up too loud.  However, watching the video it looks like the red LED blinks 3 times and it was hard to read, but possibly you are getting a temporary DRV8302 error pop up in the grey box "fault code"?

This looks very similar to my DRV failure (chip needs to be replaced), but mine wouldn't spin up at all.  

If you get it to error a couple times (blinking red light) - in the terminal do you get a fault response after typing "fault" (i think) and hitting enter?
```

---
## \#17 Posted by: cmatson Posted at: 2015-09-15T01:08:51.831Z Reads: 117

```
it just tells me "bad connection results received" when I try to do the motor detection. 

also, I typed fault into the terminal, but each time it said no fault found...
```

---
## \#18 Posted by: cmatson Posted at: 2015-09-15T01:26:12.999Z Reads: 118

```
I've got it!

I wasn't typing in the fault code fast enough, and now that I typed it while the light was blinking, it said "fault code DRV8302!

the motor (with PPM input setup) would work perfectly at braking, but just give a tiny cog/mini spin with throttle input, and then freak out with blinking red lights for a couple seconds. I'm uploading that video now-

edit: here's the vid: https://youtu.be/BrOuvl3R9Yw
```

---
## \#19 Posted by: sl33py Posted at: 2015-09-15T01:51:39.331Z Reads: 112

```
It sounds like @onloop is taking care of you (nicely done).  If it's simply a dead DRV8302 chip - they are about $6 ea from mouser and you just need someone with the skill to swap it.

I'd call it D.E.D. for now.
```

---
## \#20 Posted by: cmatson Posted at: 2015-09-15T02:06:04.849Z Reads: 112

```
to be honest, considering my solder joints with the 10 gauge wire (granted it was with a $10 cheapo 30w soldering iron) I don't think I would be able to pull that off...

I'd probably just screw it up even more.

I'll return it back to @onloop for store credit, and order one from his new batch coming in October. The bright side to all this, is I learned alot more about the VESC than I would have otherwise, like fiddling with everything in the BLDC tool. Getting to the bottom of the issue is also pretty nice- makes less work for for @onloop, and the least I can do considering he's going to replace it for me. 

Thanks so much for the help @sl33py, I REALLY appreciate it man!
```

---
## \#21 Posted by: cmatson Posted at: 2015-11-13T04:14:40.315Z Reads: 101

```
Looks like the poor soldering was the culprit:

The positive lead coming from the battery must have touched or gotten close enough to the "copper bridge thingy" (that's the technical term incase anyone is wondering...) and caused it to short out.

Moral of the story: don't use a cheap soldering iron!!! It'll screw you over in the long run.
```

---
