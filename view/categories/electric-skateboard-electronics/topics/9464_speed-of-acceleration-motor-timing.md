# Speed of Acceleration&hellip;Motor Timing?

### Replies: 19 Views: 2062

## \#1 Posted by: mmaner Posted at: 2016-09-12T16:44:10.544Z Reads: 160

```
I have a question regarding the speed of acceleration.  Using the TorqueBoards 120A 6S ESC, TorqueBoards 2.4ghz Nano Remote Controller & Electric Skateboard Motor 5055 280KV the speed of acceleration is very high.  I have set the ESC Acceleration to LOW but if you hit the remote trigger to full throttle the board will rocket away, leaving me on my butt :).  I also tried moving from 6s (series) to 3s (parallel) thinking half the voltage = half the speed but the speed of acceleration is not signifigantly different.  

I am wondering if I set the Motor Timing to Low if that would further lower the speed of acceleration.  My ESC settings are listed below in case there is another option.  thanks

Motor Timing:	High
Acceleration:	Low
Running Mode:	For/Brake
Brake Force:	20%, 40%
Drag Brake:	0%
Cut-Off Vol:	3.2v/Cell
Max For Force:	80%%
Max Rev Force:	40%
Motor Rotation:	Normal
Netral Range:	7%
Battery Type:	Lipo
```

---
## \#2 Posted by: peter Posted at: 2016-09-12T17:02:10.997Z Reads: 144

```
You can try reducing the Max For Force setting
```

---
## \#3 Posted by: mmaner Posted at: 2016-09-12T17:47:31.892Z Reads: 141

```
Does that reduce the max speed or something else?  I haven't been able to find a definition for each of the programming items or a manual, have googled like a madman too :).
```

---
## \#4 Posted by: Namasaki Posted at: 2016-09-12T18:23:07.193Z Reads: 131

```
Reducing max force will reduce top speed. 
Setting acceleration to "Low" gives you more torque  at Low Rpm. 
I believe you're rig is accelerating to quickly because your using the nano remote which has too short a throttle range. 
The mini remote works much better.
```

---
## \#5 Posted by: mmaner Posted at: 2016-09-12T18:56:49.961Z Reads: 112

```
That makes sense.  I was assuming that an acceleration 'curve' would resolve the issue...it still might but its nice to know about the remote.  thanks.

Is there anyway to hack in a longer throttle range?
```

---
## \#6 Posted by: sl33py Posted at: 2016-09-12T19:03:30.484Z Reads: 105

```
[quote="mmaner, post:5, topic:9464"]
Is there anyway to hack in a longer throttle range?
[/quote]

Absolutely.

GT2b

:stuck_out_tongue_winking_eye:
```

---
## \#7 Posted by: Namasaki Posted at: 2016-09-12T20:10:42.737Z Reads: 91

```
Unfortunately, it's a physical design limitation of the remote. 
Trigger remotes are just the best. 
Wether the Gt2b or the RC mini 
They are the best and most dependable available. 
I started with the Yuneec Ego which has by far the best thumb control of any eboard. 
When I built my diy, I had to switch to a trigger. 
Now that I'm used to the trigger I can look back and say that it's better than even the ego thumb control.
```

---
## \#8 Posted by: Mobutusan Posted at: 2016-09-12T21:41:39.693Z Reads: 82

```
@mmaner Try dropping your neutral range to 3% and try dropping your timing to low. What firmware are you using?
```

---
## \#9 Posted by: mmaner Posted at: 2016-09-12T21:44:28.684Z Reads: 79

```
Ill try that and let you know the results.  I am using the firmware that came on it, v1.00_160427.  Where do get new firmware revisions?  I haven't been able to find a manual or anything.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-09-12T21:59:21.447Z Reads: 75

```
3% neutral will also give you more top speed. 
At least it did with my TB 12s Esc. 
Check with Dexter at Torquesboard to see if you have the latest firmware. 
The easiest and fastest way to reach him is through the chat window on his website. 
Also, don't depend on the low voltage cut off to protect your batteries. It's not accurate or dependable. 
Example: if you turn the Esc on with a battery that's not fully charged, it will miss calculate the number of cells.
```

---
## \#11 Posted by: mmaner Posted at: 2016-09-12T22:12:20.524Z Reads: 72

```
Well, not the ESC is going crazy, even after I set the programming options back to default...Motor Timing: Very High, Max For Force: 100%, etc.  Its blinking Green to Yellow, Red when I hit the trigger.
```

---
## \#12 Posted by: Mobutusan Posted at: 2016-09-12T22:18:10.505Z Reads: 66

```
I think you need to update your firmware. I think that is an older version. Like @Namasaki said, contact Torqueboards through his live chat on his website and update your firmware. He's probably available now, I would guess.
```

---
## \#13 Posted by: mmaner Posted at: 2016-09-12T22:19:52.270Z Reads: 68

```
I did, said he didnt have a new version.  Im googling for tips now :)
```

---
## \#14 Posted by: Namasaki Posted at: 2016-09-12T22:46:43.564Z Reads: 65

```
Don't try to get a different firmware somewhere else. 
It will likely be wrong and ruin your Esc.
```

---
## \#15 Posted by: Namasaki Posted at: 2016-09-12T22:49:33.027Z Reads: 67

```
You might ask if he will let you trade the nano remote in on the mini. I've tried both and the mini better by far. 
Dexter is really a cool guy. Good chance that he will work with you on this.
```

---
## \#16 Posted by: Cisphyx Posted at: 2016-09-12T23:00:39.257Z Reads: 67

```
Do your brakes work okay? I seem to be having the opposite issue with my TB 12S ESC, I can adjust the acceleration fine, but nothing I do seems to make the brakes do anything other than slam on full blast, even with everything on the lowest possible settings.
```

---
## \#17 Posted by: mmaner Posted at: 2016-09-13T01:05:42.382Z Reads: 64

```
My brakes are are working normally, I think.  They are set at 40%, which is great for flat and uphill, not so much for downhill.  

I'm thinking the optimal brake solution would be an application of force on a curve based on current torque but I have no idea if that can be done or not.  

I think I'm just going to focus on the remote for now.  Ill get with Dexter tomorrow on that.  

As far as the blinking lights, I think that was  a battery issue.  Ive got one battery that is showing low voltage on a cell and I haven't figured out how to charge it yet so I pulled out another one and rebuilt my parallel adapter with 5.5mm bullets and now all is good.  You can see the build [here](http://www.electric-skateboard.builders/t/bad-hand-santa-cruz-screaming-hand-180mm-rev-kingpin-trucks-diy-5055-280kv-chinese-mount-torqueboards-120a-6s-esc/8819/23) (as soon as I get it updated :slight_smile:) .
```

---
## \#18 Posted by: popopopop Posted at: 2016-09-13T14:44:42.717Z Reads: 53

```
This is so strange. So "low" on acceleration means higher torque at lower RPM? Can someone confirm this and save me 10 minutes of messing around? It really sounds like it should be the opposite.
```

---
## \#19 Posted by: Namasaki Posted at: 2016-09-13T15:23:58.609Z Reads: 49

```
I know it sounds strange. I played around a lot with the settings on my TB Esc's  trying different combinations. 
Higher timing seemed to smooth out the torque but also made the Esc run hotter. 
Acceleration setting seems to move the power band up or down.
```

---
