# How do I setup TorqueBoard&rsquo;s 12S ESC? (Partially Solved) Post #6 Lists new problem

### Replies: 32 Views: 2494

## \#1 Posted by: Brando Posted at: 2016-08-16T18:20:26.688Z Reads: 150

```
I recently received The TB 12S ESC, but I dont know how to make it run...
I programmed it with the programming card, the only setting I was unsure about was BEC voltage. I just left it at 5V.
The motor does that little jerk that it is supposed to do every time I change a setting on the card, so i know my motor is connected properly.
My receiver is binded properly to my remote as indicated by the solid red light on the receiver.
Everything seems okay but when I wire it all up the remote throttle does not control the motor... Help
```

---
## \#2 Posted by: treenutter Posted at: 2016-08-16T19:08:30.507Z Reads: 145

```
@torqueboards is on the forum he can probably help with this @Brando. I'm wondering if it's a trim control issue; have you tried modifying the trim settings on the remote? 

Can we see a pic of your wiring? Are you sure your motor leads are properly connected?
```

---
## \#3 Posted by: torqueboards Posted at: 2016-08-16T20:10:04.370Z Reads: 143

```
Which remote are you using? If it's the TB Mini, your trim knobs on top (white) should be 12 oclock and 2 oclock.
```

---
## \#4 Posted by: sl33py Posted at: 2016-08-16T21:19:31.000Z Reads: 140

```
Also, if you are using GT2b - make sure you are on CH2 which is throttle.  I'd swap the to all the channels and re-try throttle in case that fixes.
```

---
## \#5 Posted by: Brando Posted at: 2016-08-16T22:06:44.990Z Reads: 129

```
Thanks all! It was a trim issue on the remote. Btw, I have the nano remote. I just turned the trim until it responded.
```

---
## \#6 Posted by: Brando Posted at: 2016-08-17T00:26:10.500Z Reads: 117

```
@torqueboards So I came across another problem after testing the board on the road. It is very slow. I had to turn the throttle trim on your nano remote all the way down because that is the only way that the motor would actual stop spinning on neutral throttle. If I turn the trim up then the motor reaches max speed, but when I take my hand of the trigger the motor is still spinning. how can I get full speed and still have the motor coast when I take my hand off the throttle?
```

---
## \#7 Posted by: torqueboards Posted at: 2016-08-17T00:45:10.725Z Reads: 112

```
@Brando - Not too sure on that one. I don't use the Nano personally as much. But technically that is what the trim does.

What is your setup? Voltage? Motors? Single/Dual?

Not sure if anyone has any other advice or suggestions for this?
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-17T00:47:13.314Z Reads: 108

```
If you adjust trim on the nano, you have to rebind to recenter the throttle.
```

---
## \#9 Posted by: Brando Posted at: 2016-08-17T00:58:04.611Z Reads: 104

```
@Jinra I'll try that when my batteries finish charging in a bit
@torqueboards I have two 5Ah 3S Lipo's in series, and one of your 230KV 2650W motors.
```

---
## \#10 Posted by: Brando Posted at: 2016-08-17T03:04:07.367Z Reads: 105

```
@jinra I re-binded my nano remote with the trim on max and it didnt fix it. How do you tell the esc what your neutral point is? on my old 6S esc from tb, there was a set button on it that you used to calibrate it.
```

---
## \#11 Posted by: barajabali Posted at: 2016-08-17T16:56:51.486Z Reads: 98

```
How slow is it going exactly because you're only running 6s?
```

---
## \#12 Posted by: Brando Posted at: 2016-08-17T17:35:34.197Z Reads: 102

```
It goes 13mph which is obviously low for 6S. I can get it up to 18mph if I stick a screwdriver in the remote trim while im riding it lol. But then when I take my hand off the controller it goes at about half speed instead of coasting.
```

---
## \#13 Posted by: barajabali Posted at: 2016-08-17T17:46:43.016Z Reads: 97

```
Oh man so it does sound like a remote issue then... I've never used that remote so I'm not sure how it operates
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-17T18:23:01.953Z Reads: 96

```
My remote has a 1.11 min with a 2.1x max on default, which can go up and down depending on trim. My min stays the same regardless of trim though. Neutral moves with trim as well. This is probably why he's having problems.
```

---
## \#15 Posted by: Brando Posted at: 2016-08-17T19:52:31.107Z Reads: 94

```
@Jinra Are you suggesting that your nano remote works differently than mine? I got mine from . how about you?
```

---
## \#16 Posted by: barajabali Posted at: 2016-08-17T19:59:00.386Z Reads: 91

```
This may seem off topic, but how is the braking?
```

---
## \#17 Posted by: Jinra Posted at: 2016-08-17T19:59:10.225Z Reads: 89

```
I'm not suggesting it's different, just giving you an idea of how it's setup, at least on mine. I got mine from @kaly
```

---
## \#18 Posted by: Brando Posted at: 2016-08-17T22:24:26.667Z Reads: 90

```
@barajabali breaking is fine. Seems pretty strong even at 30%. When it was at 80% it would use ABS breaking I think. The breaks would pulse.
```

---
## \#19 Posted by: Brando Posted at: 2016-08-17T22:27:51.609Z Reads: 91

```
Okay, I dont think kaly's would work differently. So all you did was rebind and it set the neutral point? Im still not home, but when I do get back ill send a video documenting my whole problem.
```

---
## \#20 Posted by: Jinra Posted at: 2016-08-17T22:30:02.695Z Reads: 90

```
Well my setup is different since I'm running VESCs. I can set min and max pulsewidth on it.
```

---
## \#21 Posted by: Namasaki Posted at: 2016-08-18T06:49:26.813Z Reads: 79

```
The TB 12s comes default with the neutral width set at 7
With your program box, turn it down to 3 
When I did this It increased my top end speed.
```

---
## \#22 Posted by: Namasaki Posted at: 2016-08-18T06:51:22.681Z Reads: 82

```
There's no pulse width setting on the TB12s, just neutral width.
The mini RC remote is very compatible with the TB12s
I tried the nano remote and it worked, but not as well as the mini.
IMO, the long pull trigger controls smoke the short push thumb controls.
```

---
## \#23 Posted by: Brando Posted at: 2016-08-18T13:39:50.362Z Reads: 77

```
Yeah sounds like the nano remote wasn't meant for this esc which kinda sucks. My nuetral range was already 3 so that wont help :sweat:
```

---
## \#24 Posted by: Brando Posted at: 2016-08-18T15:18:04.177Z Reads: 75

```
**Something to point out:**
When the ESC makes a successful connection with the remote, it will make my motor beep three times. After this point, I can use the remote to control the motor. 
But...
The motor will only beep and become controllable if I turn the trim all the way down. At this point I can change the trim, but like I said, raising the top speed will also raise neutral speed. I feel like if there is a way for my motor to beep at a non-minimum trim I would be okay, but the esc refuses to connect unless my trim is all the way down.
Basically what I'm asking is, what makes the esc decide to beep the motor and ready up? I got the motor to beep once by randomly pushing and pulling the throttle.
```

---
## \#25 Posted by: michaeld33 Posted at: 2016-08-18T15:26:36.029Z Reads: 70

```
Beep 3 times? I may be wrong (@torqueboards) but doesn't the beeping mean it's counting the number of cells in the lipo? So that means it may be reading 3s? That could explain the slow speed... Also, why are you using the TB 12s ESC if you could use a car ESC @ 6s?
```

---
## \#26 Posted by: barajabali Posted at: 2016-08-18T15:34:34.844Z Reads: 69

```
The newest firmware does.
```

---
## \#27 Posted by: Brando Posted at: 2016-08-26T04:01:33.908Z Reads: 65

```
I am upgrading to 12S later. Also the whole reason I bought it is because my 6S car esc broke and I wanted a more stable one. 
Plus, this esc has better acceleration tunning and better breaking, and it is slimer and silent because there is no fan.
```

---
## \#28 Posted by: Pantologist Posted at: 2016-09-05T03:14:24.477Z Reads: 55

```
Weird, my 12S TB ESC doesn't beep for anything....
```

---
## \#29 Posted by: i2oadsweepei2 Posted at: 2016-09-05T03:19:39.508Z Reads: 56

```
Same here no beeps on either one in my dual setup.
```

---
## \#30 Posted by: barajabali Posted at: 2016-09-05T03:26:14.702Z Reads: 53

```
Your firmware doesn't beep.
```

---
## \#31 Posted by: Pantologist Posted at: 2016-09-05T04:06:20.862Z Reads: 54

```
An older firmware?
```

---
## \#32 Posted by: torqueboards Posted at: 2016-09-05T04:26:24.349Z Reads: 54

```
The TB ESC's that don't beep are from an older firmware. The firmware itself is pretty much the same. The only difference is I took the beeps off initially.
```

---
