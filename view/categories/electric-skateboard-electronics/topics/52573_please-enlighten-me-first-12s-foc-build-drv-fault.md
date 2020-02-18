# Please enlighten me. First 12s FOC build. DRV Fault?

### Replies: 44 Views: 1209

## \#1 Posted by: Mikenopolis Posted at: 2018-04-17T17:29:30.560Z Reads: 169

```
Hey Guys,

Spent a few days aligning parts, soldering and setting up the two FocBoxes on this dual 6374 build. Everything seems to run fine, both motors turned on the bench sensors detected fine blah blah blah

I screwed on the enclosure/cover, turn it on and pressed the throttle a little, one motor turned and the other didn’t 😔. Opened everything up and saw the dread red led. Plugged it into the PC and this is the fault I see...

Can you tell what I did wrong by these images?![image|375x500](upload://aXLegmzqkQ569mibrmTFySHBR6c.jpeg)![image|374x500](upload://wd7BgTXEhZPmnby9NGeZIhoHIgq.jpeg)![image|375x500](upload://gzxjrxc5w3cWmTWtAFrDo7XIR3p.jpeg)
```

---
## \#2 Posted by: Deckoz Posted at: 2018-04-17T17:31:09.948Z Reads: 151

```
You detected in FOC independently for both? 

At any time did any of the phase wires touch while powered on...
```

---
## \#3 Posted by: RedEagle Posted at: 2018-04-17T17:32:49.938Z Reads: 150

```
Never spin it up on the bench. Number one reason why people fry drv's. Ooh and bad solder jobs. 
Did you manage to ride it?
```

---
## \#4 Posted by: Acido Posted at: 2018-04-17T17:34:08.956Z Reads: 147

```
why? assuming you do not fry your motherboard like i did :D
```

---
## \#5 Posted by: Exiledd_Top Posted at: 2018-04-17T17:36:07.078Z Reads: 148

```
[quote="Mikenopolis, post:1, topic:52573"]
saw the dread red led.
[/quote]

I can lend u my spare vesc if u want till you get that one repair/replace .
```

---
## \#6 Posted by: RedEagle Posted at: 2018-04-17T17:37:57.140Z Reads: 146

```
There is no load while bench testing. This means you can go over the erpm limit very quickly if there is one. That and all sorts of other things. 

It won't hurt just spinning the motor a little bit but most of us go full throttle right then and there. That's where the error lies.
```

---
## \#8 Posted by: Mikenopolis Posted at: 2018-04-17T17:39:17.130Z Reads: 142

```
How about my numbers, would any of that be my issue?

@Deckoz each was detected independently. I have a receiver for each focbox.

@RedEagle basic solder jobs on my end would not be bad. I've been soldering stuff since I was like 4 since my dad was a electrical engineer. Can't do most of what he can, but this I can do. as for spin up on bench. I only did slow spins to check direction, not really full throttle or anything. I never stepped on it since I'm still waiting for belts and one of the motor pulleys.

@scepterr Can you send me back the two FocBoxes when you get a chance. Might need it now
```

---
## \#9 Posted by: mmaner Posted at: 2018-04-17T17:39:27.334Z Reads: 140

```
Awwww dude, Im so sorry.  that sucks.  If you need a loaner I have a couple of spares on the way.
```

---
## \#10 Posted by: ThermalM16 Posted at: 2018-04-17T17:41:59.119Z Reads: 133

```
Are you 100% sure you loaded the correct FW on there? Everything you have posted on there looks fine to me. I know on the newer VESC Tools, it can be easy to pick the wrong one from the list they give you
```

---
## \#11 Posted by: Mikenopolis Posted at: 2018-04-17T17:43:37.780Z Reads: 133

```
I'll double check tonight, but I'l 99% sure I picked the correct 4.12 FW when I updated it to Ackmaniac
```

---
## \#12 Posted by: mmaner Posted at: 2018-04-17T17:44:31.466Z Reads: 129

```
Im staying at 2.54.  I had a ton of issue when trying to get 3.1 on latest FoxBox's.
```

---
## \#13 Posted by: RedEagle Posted at: 2018-04-17T17:44:54.007Z Reads: 129

```
''Its carvon speed drive I full throttle it all the time when I was fixing it without load they don’t pass the erpm limit . never had issues''

Well, if your erpm is under 60k, solder job's good. you're using reliable psu/battery then it all comes down to the esc. If you're lucky you'll get one of the good batch.

For example I've had only one maytech vesc fail on me and it was my fault. Never used any other brand.
```

---
## \#14 Posted by: Exiledd_Top Posted at: 2018-04-17T17:45:35.742Z Reads: 124

```
I read it wrong its 6374 motor @RedEagle
```

---
## \#15 Posted by: RedEagle Posted at: 2018-04-17T17:47:00.255Z Reads: 119

```
How long are your main battery wires? I would also check which rail is shorted.
```

---
## \#16 Posted by: Exiledd_Top Posted at: 2018-04-17T17:47:07.157Z Reads: 123

```
[quote="mmaner, post:12, topic:52573"]
Im staying at 2.54
[/quote]

I generally stay at stock firmware I think its 2.14 or 2.17 never had issues if it ain't broke don't fix It lol.
```

---
## \#17 Posted by: mmaner Posted at: 2018-04-17T17:47:55.514Z Reads: 125

```
I like @Ackmaniac at 2.54, I get the app, modes, acceleration/brake curve...all good.
```

---
## \#18 Posted by: RedEagle Posted at: 2018-04-17T17:49:01.748Z Reads: 121

```
No issues here. Running maytech 4.12 on 3.1
Really curious about which issues.
```

---
## \#19 Posted by: ThermalM16 Posted at: 2018-04-17T17:54:20.243Z Reads: 118

```
The biggest thing with the new FW is that the VESC Tool UI is very different from the old BLDC Tool. Both of them work fine and some functions are more optimized on the new FWs, but if you don't take the time to familiarize yourself with the software... you're gonna have a bad time
```

---
## \#20 Posted by: Acido Posted at: 2018-04-17T17:55:05.642Z Reads: 121

```
why go full throttle(with arrow keys), just put it on like 5k rpm and see if it spins nicely
```

---
## \#21 Posted by: Mikenopolis Posted at: 2018-04-17T18:25:29.659Z Reads: 116

```
hmmm so are you saying no to ackmaniac? not that I care what I use. I just want this thing to work
```

---
## \#22 Posted by: Battosaii Posted at: 2018-04-17T18:39:51.003Z Reads: 108

```
That sucks man I've been wanting to go FOC but have not because I'm scared this will happen and my board has been rock solid since I built it.
```

---
## \#23 Posted by: mmaner Posted at: 2018-04-17T18:44:39.550Z Reads: 109

```
No, I'm saying go ackimaniacs 2.54. It's fool proof. I've yet to get the ride quality on any other firmware/version.
```

---
## \#24 Posted by: Mikenopolis Posted at: 2018-04-17T18:53:03.794Z Reads: 108

```
I've probably ridden the 10s FocBox in FOC for maybe 150 miles with no issues except the the initial two DRV errors, same one failed twice, I think it was a bad batch. but no issue with that one some far. I was thinking this was a 12s problem.

@mmaner ahhh. I used ackmaniac 3.10, just downloaded 2.54. I'll try that
```

---
## \#25 Posted by: Battosaii Posted at: 2018-04-17T18:58:14.560Z Reads: 107

```
I'm also running 12s
```

---
## \#26 Posted by: E1Allen Posted at: 2018-04-17T19:08:32.591Z Reads: 106

```
If he spun up in FOC after setting up, how would he have erpm limits?
```

---
## \#27 Posted by: Mikenopolis Posted at: 2018-04-17T19:11:48.820Z Reads: 104

```
@barajabali ran 12s Focboxes with no issues so I assume these wouldn't have a problem with it
```

---
## \#28 Posted by: Deckoz Posted at: 2018-04-17T19:13:14.994Z Reads: 105

```
You made sure to flash the 410_411_412 bin correct?
```

---
## \#29 Posted by: Mikenopolis Posted at: 2018-04-17T19:19:50.342Z Reads: 101

```
yeah, under the "Hardware Version" I selected "410 & 411 & 412"
```

---
## \#30 Posted by: Deckoz Posted at: 2018-04-17T19:20:33.769Z Reads: 99

```
Can you still run Detection in either FOC or bldc? Or is Detection also giving faults...
```

---
## \#31 Posted by: Mikenopolis Posted at: 2018-04-17T19:21:40.059Z Reads: 98

```
I'll reflash again tonight when I get home and see what I can do
```

---
## \#32 Posted by: Battosaii Posted at: 2018-04-17T19:21:47.713Z Reads: 99

```
Still scared of doing it haha. Not saying it won't work but I've seen this happen often enough to keep me spooked I know @Deckoz runs them at 13s and it's fine for him. 

Maybe once my Raptor comes in this week I'll mess with my board I don't want to be rideless if my focbox blow up.
```

---
## \#33 Posted by: Deckoz Posted at: 2018-04-17T19:29:39.407Z Reads: 97

```
[quote="Battosaii, post:32, topic:52573"]
@Deckoz runs them at 13s and it’s fine for him
[/quote]

While this is true... I typically do my detections at 4s or a lower voltage, as detections can be...well.. interesting.  Not necessary by any means.. but just something I do...
```

---
## \#34 Posted by: Mikenopolis Posted at: 2018-04-18T00:31:05.070Z Reads: 95

```
![image|374x500](upload://iId7JeVAmxKbCjqrUWmMWm2KWNw.jpeg)Visually, does anything stand out? I’m not seeing anything. 

I reflashed the FW, rebooted and when I tried to detect motor, the motor made a slight click noise and I see the red led
```

---
## \#35 Posted by: Deckoz Posted at: 2018-04-18T00:39:41.263Z Reads: 96

```
![image|346x500](upload://v233MfhCXFVeSsnPNZHGgTBsyPN.jpg)

@JohnnyMeduse is that flux or a burn?
```

---
## \#36 Posted by: Mikenopolis Posted at: 2018-04-18T01:07:43.439Z Reads: 95

```
I was looking at that too.
```

---
## \#37 Posted by: JohnnyMeduse Posted at: 2018-04-18T02:04:57.149Z Reads: 93

```
Could be but they aren't using water base flux, so it should not affect any of the electronic.
```

---
## \#38 Posted by: CarlCollins Posted at: 2018-04-19T05:26:33.795Z Reads: 80

```
@Mikenopolis
Can you tell me if your FOCBOX constantly flashing fault lights or only flashes at initial startup and then stay at blue or blue & green?
Also, on which firmware you are currently at?
Have you tried using BLDC tool to check? Instead of VESC tool?
```

---
## \#39 Posted by: Mikenopolis Posted at: 2018-04-19T06:32:36.984Z Reads: 76

```
No it flashed when I throttled just a tiny bit. First fault with ackmaniac. I reflashed the firmware back to original. Attempted to start over and detect motor and it flashed red
```

---
## \#40 Posted by: CarlCollins Posted at: 2018-04-19T06:35:12.551Z Reads: 77

```
Have you tried it using Enertion's BLDC tool with Enertion's FW?
```

---
## \#41 Posted by: Mikenopolis Posted at: 2018-04-19T06:39:54.587Z Reads: 76

```
hmmm I don’t think so. I used the old bldc tool, the one vesc tool from vedder, and ackmaniac which everyone said was superior. I’m think it was either the 12s or FOC that caused the fault.
```

---
## \#42 Posted by: CarlCollins Posted at: 2018-04-19T06:41:15.200Z Reads: 77

```
Why don't you give a try to Enertion Version?
If you need any assistance I can guide you using team viewer
```

---
## \#43 Posted by: Mikenopolis Posted at: 2018-04-19T06:47:15.122Z Reads: 73

```
Thanks Carl. I’ll give that a try

@ThermalM16 since it’s already in the mail can you please give Carl’s advise above a try to see if there’s still a fault?
```

---
## \#44 Posted by: ThermalM16 Posted at: 2018-04-19T19:11:00.726Z Reads: 64

```
For sure. Before I start replacing anything, I’ll give that a shot and diagnose as much as I possibly can with software before I start replacing parts.
```

---
## \#45 Posted by: CarlCollins Posted at: 2018-04-20T10:00:25.363Z Reads: 48

```
@ThermalM16

Let me know the results please
```

---
