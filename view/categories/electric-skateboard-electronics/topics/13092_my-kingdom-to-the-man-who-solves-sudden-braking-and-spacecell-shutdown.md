# My kingdom to the man who solves - sudden braking and Spacecell shutdown

### Replies: 21 Views: 1513

## \#1 Posted by: CRABOLSKY Posted at: 2016-11-15T10:04:55.636Z Reads: 214

```
Okay here goes! 

I've have had my [Snappy Chariot](http://www.electric-skateboard.builders/t/snappy-chariot-jet-hot-potato-deck-caliber-ii-50-190kv-r-spec-6372-spacecell/4267/29?u=crabolsky) on and off the road for two months. In that time I've had a series of issues surrounding remotes, charging, motor shorting out, and blown dvr chip.

I think that all these items are incidental issues and are secondary to another larger problem at play. Without going into too much detail (see links if interested), my braking issue under acceleration with the [Steeze](http://www.electric-skateboard.builders/t/charging-produces-tiny-motor-pulses-video-space-cell-solved/11174/16?u=crabolsky) and the [Winning Remote](http://www.electric-skateboard.builders/t/winning-remote-issue-changing-response-and-braking/12446/5?u=crabolsky) has not been solved with rectifying the [shorting phase wires](http://www.electric-skateboard.builders/t/r-spec-shorted-phase-wire-problem-solution/6474/56?u=crabolsky) on the R Spec windings. 

With the recent motor repair I though I was going to be all set, however to night the problem has progressed. After 5 km of riding I noticed the the now familiar suggest brake pulse under acceleration came back. I then backed off and checked for heat on the vesc or motor and it was fine. No evidence of any burning smell or overheating.  I then started off again slowly only to have the same problem happen again. Only now, when the braking pulse happens (it feels like the break has been tapped briefly), the board will coast for a second or as it doesn't most often, the Spacecell shuts down. 

So now if I accelerate, I get the brake sensation then the LCD screen and power with switch off. A toggle back and forth on the Spacecell brings it back to life. So I think the phase wires (while starting to brake down) were probably not the source of the braking problem.  

I am pretty confident that this isn't related to the remote. I'd like to think I've solved the phase wire issue with the additional heat shrink. I don't think this is a VESC setting issue since my settings are based on @whitepony settings and he hasn't had any of these issues. Is this a VESC or BMS issue??? @onloop, @lox897, @Jinra @evoheyax  you've all helped nail these past issues.  I am at a loss!
```

---
## \#2 Posted by: lox897 Posted at: 2016-11-15T10:12:26.432Z Reads: 203

```
I'd try looking at the BMS and posting your vesc settings
```

---
## \#3 Posted by: TarzanHBK Posted at: 2016-11-15T10:19:30.849Z Reads: 190

```
sounds like an BMS issue, maybe a loose solderconnection. I´d check all wires first and then work my way up, starting from the battery to BMS and so on
```

---
## \#4 Posted by: CRABOLSKY Posted at: 2016-11-15T10:26:04.581Z Reads: 182

```
Hey Lox these are my settings except the bat min regen is now set to -12 not -20. 
<img src="/uploads/db1493/original/3X/e/5/e5222a201986e23591bb43f2d36c3de2967c282e.PNG" width="690" height="388">
I guess I am going to have to break open the cell to investigate.
```

---
## \#5 Posted by: CRABOLSKY Posted at: 2016-11-15T10:31:27.421Z Reads: 166

```
@TarzanHBK I think that could be the deal. I think the vibration that our batteries are subjected to on the streets is pretty substantial and can loosen solder points.
```

---
## \#6 Posted by: 2-alex-2 Posted at: 2016-11-15T10:54:01.060Z Reads: 164

```
Not only vibrations but if you setup hasn't been working right solder joins may have become warm as well which combined with vibrations will start to loosen them.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-11-15T16:06:13.166Z Reads: 141

```
It does sound weird to me that a loose wire in the bms could cause such behavior.

When it brakes on its only, does the space cell shut off every time?

Maybe its a vesc issue. Have you looked at the vesc carefully to see if anything stands out?

I wish you had more ride data. Seeing a graph of everything that's happening in your vesc might give us a better idea of exactly what's happening. This is why I've spent so much time developing a bluetooth system for recording and graphing as much data as possible about the vesc in operation.
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-15T16:47:21.897Z Reads: 120

```
Try checking for faults first. Ride your board until it errors out and then plug it in to BLDC tool and check for faults. Just make sure not to turn it off in the time between.
```

---
## \#9 Posted by: CRABOLSKY Posted at: 2016-11-15T23:22:48.817Z Reads: 103

```
So it started to happen where I would accelerate and then it would brake pulse and coast for a second and then I could accelerate for a bit and if would do it again. Every time this happened the battery still appeared to be on and functioning.   Sometimes I would have to reconnect the remote. 

After doing this for about 5 minutes I noticed that it would sometime switch the battery off. I tried to take it out last night to get it to trip again but every time the battery would just switch off. This makes it difficult to capture the faults. I need to get the bluetooth going asap. @Jinra Even when I leave the battery on, whenever I try and connect the usb to BLDC, it doesnt actually show up under the connect tab until I switch it of and on again (I am running a MAC). 

I don't think this would be causing the problem, but I'll throw it out there... See below photo showing the wiring path - at the junction, there are bullet connectors, heat shrink and electrical tape separating them. 

<img src="/uploads/db1493/original/3X/c/9/c9ffada541b7249f361d85dc399de13eb03f4c3e.jpg" width="690" height="458">
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-15T23:24:24.066Z Reads: 97

```
The little 'refresh' button should work to redetect the VESC as well. You shouldn't have to cycle off and on to connect.
```

---
## \#11 Posted by: CRABOLSKY Posted at: 2016-11-15T23:28:46.605Z Reads: 95

```
Unfortunately the refresh button didn't do it. Maybe I'll get a better result next time.
```

---
## \#12 Posted by: CRABOLSKY Posted at: 2016-11-16T10:19:37.108Z Reads: 79

```
I've got the battery to stay alive after one of the brake glitches and have connected it to BLDC... 
At first hook up it came back as fault code none, so I ran it while on the bench and the pack stitched off and came back as FAULT UNDER_VOLTAGE. Sounds like the space cell is at fault here? I wasn't sure how to export the data so I've taken 3 screen captures of the live BLDC report right after the fault. 

<img src="/uploads/db1493/original/3X/4/5/45e516cbbb3e6cf1bcc0a950995da95f095d499e.png" width="689" height="434"><img src="/uploads/db1493/original/3X/8/c/8c435a0ca497f933920ff5a072d35a4d304a3ad9.png" width="690" height="429"><img src="/uploads/db1493/original/3X/2/d/2dbcf5e379ccac38875de676d5873fbfaacf8a57.png" width="690" height="425">
```

---
## \#13 Posted by: lox897 Posted at: 2016-11-16T10:28:29.009Z Reads: 69

```
It would be good to measure the output voltage of the space cell pack because maybe it isn't putting out the required voltage.
```

---
## \#14 Posted by: CRABOLSKY Posted at: 2016-11-16T10:37:28.469Z Reads: 72

```
For comparison, the attached screenshot shows its output while running normally on the bench 37.6v . It looks okay but must glitch when under load maybe?

<img src="/uploads/db1493/original/3X/d/3/d3d274b31494978405affbdecd68ad6917fba3e2.png" width="690" height="433">
```

---
## \#15 Posted by: TarzanHBK Posted at: 2016-11-16T12:16:53.324Z Reads: 70

```
sounds more and more like a battery/BMS issue.
Have you checked the connections there?
```

---
## \#16 Posted by: Jinra Posted at: 2016-11-16T14:49:44.111Z Reads: 65

```
it could be sagging so much it triggers the under volt error. try running the system on the bench while measuring voltage.
```

---
## \#17 Posted by: evoheyax Posted at: 2016-11-16T15:48:32.296Z Reads: 63

```
Am I the only one whose reading the voltage along with the fault code from these screen shots? It says the current voltage is 0.5 volts in all but the last one.

The thing is, it's hard to say what's at fault still. My second enertion vesc broke the second day with an error saying under voltage, but it stays there permanently, it'll never go away. This comes and goes, so I would be more willing to say it's the battery.

Do you have any other batteries laying around?

And are you sure the wiring is solid between the vesc and battery?

At this point, you might be best trying another vesc or another battery if possible. That would 100% narrow it down.
```

---
## \#18 Posted by: CRABOLSKY Posted at: 2016-11-16T21:34:35.887Z Reads: 56

```
Thanks guys, to clarify the last screenshot represents it running as it should (before the error). The first three show the results once the fault has happened. The .05 volts must have been the final reading before the vesc/battery shut off. 

I'll be able to test another vesc before I'll be able to test another battery so I'll start there. 

If it is a bms issue, I wonder if it is just purely faulty rather that a loose wire?

Push skating to the tram this morning... man this sucks!
```

---
## \#19 Posted by: CRABOLSKY Posted at: 2016-11-16T21:52:37.066Z Reads: 55

```
Btw that last slide is it running normal on the bench.but I guess you mean with a volt meter?
```

---
## \#20 Posted by: Jebe Posted at: 2017-02-26T00:08:04.154Z Reads: 42

```
Did you get this sorted?
```

---
## \#21 Posted by: CRABOLSKY Posted at: 2017-02-28T23:45:49.144Z Reads: 32

```
Hey Jebe, this problem was related to a faltering BMS.  I did happen to change the VESC at the same time as replacing the spacecell, however I believe it was a BMS failure that was causing the problems.
```

---
