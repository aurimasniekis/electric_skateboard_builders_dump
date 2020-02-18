# Receiver connecting to remote but no power for VESC?

### Replies: 10 Views: 432

## \#1 Posted by: brently Posted at: 2018-05-10T05:15:42.499Z Reads: 62

```
Ok so to level set this is my first build I’m no electrical engineer, more mechanical than anything else. 

Set up is a 12s4p and 60/150 BMS system from TorqueBoards into a xt90 to dual xt60 split using 12 awg copper wire into two Focboxs. 

So my issue is I’ve connected my brand new system together and it’s doing some wierd stuff:

- when I turn on the board it usually (14 times out of 15) won’t stay on, it will flash on for a second then shut off. The battery will flash random Volt readings, ~20 V usually but It reads 45.3 V when not connected to the splitter. However, and this was probably dumb on my part, when I flick the battery on and off quickly it will eventually start to read that it’s got its full voltage. Then it will stay on. 

- Also when I do get it to stay on the Focbox’s won’t read that they have power but the reciver for my remote will look for a signal and lock on to my remote when I turn it on. Focboxs are obviously unresponsive when throttle is applied. 

In the pic below you can see what time talking about the remote is paired but the focboxs look off. Also posted pics of some of my solder work to see if you guys think my first pass at soldering might actually be the culprit here. 

![image|375x500](upload://vbhbOyOmOhHFFe1Tmi5nCNAAYNq.jpeg)![image|375x500](upload://w8FvQQhZMo6uC3BGLIFHAteXzce.jpeg)![image|375x500](upload://tlUBZ1TXC2k6PjZPHmf6Urq7oeI.jpeg)![image|375x500](upload://vLmy1Xn57jvUpb0ugx0EOpTuYE8.jpeg)

I’m assuming the worst and that I’ve fried something. Someone please tell me I’m wrong. 

Thanks!
```

---
## \#2 Posted by: E1Allen Posted at: 2018-05-10T06:50:51.276Z Reads: 47

```
@brently The battery seems to have an issue.  You shouldn't get crazy readings and it should just turn on.  Could be something with the switch.  I'd contact torque boards after trying the stuff below if it doesn't work.

Disconnect the xt90 from the battery to the splitter.  Turn it on and check voltage coming from the xt90, then check all your splitter welds.  Then check voltage to each xt60

Disconnect the can cable. Disconnect one FocBox not providing power to the RX. 

Try powering on one FocBox at a time.

If it still doesn't power on the focbox I would try a different battery.  If you have a 3s lipo or anything to give you a power source that you can check the TB battery against.

I don't think you've fried anything.. so hopefully we can find a solution.
```

---
## \#3 Posted by: Deckoz Posted at: 2018-05-10T10:10:58.412Z Reads: 42

```
I'm just gonna add this here. Once you get them powered on, do not immediately try to use the throttle like you are doing, you will kill something.

You need to do a motor detection first, and setup your PPM.

Just plugging in and trying to get a throttle response, is the wrong way to setup a board... :) Make sure you do motor detections before you touch that throttle...

But everything @E1Allen said is what you should verify. Also at any point have you powered on the focboxes separately with the canbus wire attached? Because that's a no no too and kinda makes me think if it's not the battery, probably your can chips..
```

---
## \#4 Posted by: brently Posted at: 2018-05-10T12:56:10.376Z Reads: 36

```
Thanks! I’ll will give this all a try when I’m back from work tonight. I don’t have an extra battery laying are unfortunately though. 

I’ll report back with my findings.
```

---
## \#5 Posted by: brently Posted at: 2018-05-10T13:51:20.056Z Reads: 34

```
Ok very small update. I didn’t have my multimeter with me so I couldn’t check voltages but the battery acts normal when I plug it into one focbox at a time (with the canbus connector and RX unplugged). However neither of the focboxs woild turn on or blink blue to show they have power. Fearing the worst I popped the focboxs open and it all does look ok in there (to my untrained eye). I’ll get my multimeter tonight and check the voltage coming off the connectors as a next step. 

![image|375x500](upload://1N1KDjFbv8mqEWimixjswXzCN9k.jpeg)![image|375x500](upload://gmFth1xx9fLpMRhU1Tfb2pSWjzT.jpeg)
```

---
## \#6 Posted by: brently Posted at: 2018-05-11T04:46:30.605Z Reads: 27

```
I got home put my multimeter on the xt90 and it reads 45.6v I check both xt60s, they read the same thing. plugin one focbox in at a time, still doesn't turn on either. 

Should I buy this cheap battery on amazon as a tester? https://www.amazon.com/Gens-ace-2200mAh-Battery-Quadcopter/dp/B0711XG9MZ/ref=sr_1_6?ie=UTF8&qid=1526012020&sr=8-6&keywords=3s+xt60

The battery would do the same weird stuff it was doing before and wouldn't stay on with both focbox's connected without the canbus hooked up. However, with one connected the battery would stay on.
```

---
## \#7 Posted by: brently Posted at: 2018-05-11T04:49:13.847Z Reads: 29

```
I was worried I jumped the gun and set this up wrong before doing my research. Might have learned my lesson the hard way. I don't remember putting power to one focbox with the canbus connector on it but could see my dumb ass doing it. 

Is there a way to check if the can chips are toast? I opened both of them up and I don't think I see any issues but again I'm a total newb at when it comes to electronics.
```

---
## \#8 Posted by: CarlCollins Posted at: 2018-05-12T06:45:16.517Z Reads: 26

```
@brently

Try plugging in only single FOCBOX, Turn your setup on, connect the FOCBOX to the PC to check if it shows detection.
Sometimes only LEDs stop working and rest of the PCB works. 
If it shows an error firmware read or response error then your CAN transceiver is fried.
(Always check the USB cable first using any Android based phone, if you have one)
```

---
## \#9 Posted by: brently Posted at: 2018-05-15T15:45:09.745Z Reads: 23

```
Ok so update: 

yeah pretty sure I fried my can chips. I pre-ordered two more focbox's from @longhairedboy. Expensive hobby. 

Anybody know which chips are the can chips and have any reco's on trying to replace them or know someone who can? I might as well try and fix the currently faulty focbox's. 

Still worried about my battery too. it acts weird just being plugged into a single focbox. Upon the first time start up, connected to a focbox it will shut off after reading no voltage on the display. It also does this if I let it sit for more than an few hours without turning it on. However, when I checked the voltage while it's reading this blank screen on the volts are what I usually see when the display is functioning correctly. Seem's strange. 

If I turn off the battery right after it blanks and shuts off, then turn it back on while connected to a single focbox it stays on.. I think I know why it won't stay on with two connected. Likely because I didn't properly set up the focbox's initially and with both of them connected it likely tries to draw too many amps, at which point the BMS shuts down the battery? (still new to all this) 

reached out to @torqueboards about it, they asked for my order number. Still waiting on a follow up after that.


If anybody is in the NYC/Jersey City area and wants some free pizza and beer while trying to help me with this stuff once I get the new focboxs you are more than welcome.
```

---
## \#10 Posted by: brently Posted at: 2018-05-15T17:55:21.472Z Reads: 21

```
Also do you guys have a recommended data cable for tuning VESC's? I've tried my TB micro remote cable and ps4 cable and am unsure on how to confirm if they are suited for setting up a focbox.
```

---
