# No Blue Light &#124; Dual VESC &#124; Nunchuk &#124; Zippy 2x 3S

### Replies: 29 Views: 1396

## \#1 Posted by: Boca Posted at: 2017-07-07T03:07:24.313Z Reads: 120

```
Hi Gurus, I am in debug mode.

1. I received my 90mm hub motors with associated dual Maytech VESC !! Yahoo!! :slight_smile: 

2. I set up the master VESC with the Nyko Kama as per explained in the forum, batteries and motor,

3. Connect to the BLDC tool, set up the nunchuk and leave the default set up. 

4. Test successful --> wheel running fine.


**Dual:**
5. I connect the 2 VESC through the I2C port connecting the Rx master to Rx slave and Tx master to Tx slave. 

6. Connect the power supply in parallel between the 2  VESC, red with red connected to red battery wire, black with black connected to black battery wire.

7. Test unsuccessful : no blue led on the master VESC, blue led on the slave. I was able to connect to the BLDC tool before it shuts down. :frowning:

8. Original set up, master VESC doesn't turn on - 18v instead of 5v on the canbus pins every pins...

9. Single slave VESC: blue led on for 5 sec then nothing - 18v on every 5v pins...

I haven't smell or seen any smoke, no fried component, the only thing visible is 2 bites in the red cable. that is due to the sensor pins forcing into it. Seems to be a known issue...

Any hope? what caused the issue? 
Let me know what additional test can I do?

Thanks in advance,
DaBoca
-
```

---
## \#2 Posted by: rpn314 Posted at: 2017-07-07T15:25:28.569Z Reads: 91

```
Very possible something is fried. Can you upload pictures of those "bites" in the red cable? It's possbile you shorted the UART port pins into the red cable. This was an issue discovered some time ago that Maytech probably didn't care about (no offense to you, they're just a cheap chinese company).

http://www.electric-skateboard.builders/t/vesc-faq-negative-squared-cross-mark-warning-negative-squared-cross-mark-risk-of-short/6805?u=rpn314
```

---
## \#3 Posted by: Boca Posted at: 2017-07-07T16:20:45.606Z Reads: 85

```
I saw this issue they have. can't really takes photos it won't appear on it. 
My question is how can I test if a component fried and which one?

As of now Maytech is not willing to take responsibility and push the fault on me because I removed the plastic (afterwards to test the circuit) and therefore the VESC is not vanilla anymore for them... even before finding the cause, their answer is we don't care, it is your fault, no plastic protection, then no warranty...
Which is not fair and they know it... Let's see, I will keep you posted.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-07T17:01:05.068Z Reads: 73

```
Try to see both sides, if you break a seal on any product and start poking around the manufacturer doesn't really need to take responsibility for anything that happens to the product beyond that.  If this was a microwave or a hard drive and you break the warranty seal it's the same thing (don't make them wrap everything in warranty seals).  I say this because I fried my own VESC once taking off the shrink tube and poking around with a voltmeter.  It might be their fault here, but hard to absolutely pin it on them once you start probing around on the board.

In terms of diagnostics you just need a multi-meter the schematic and time basically.  You can check the components connected to the UART or anything else that is acting goofy and see what blew open/closed but honestly the time to diagnose and fix it likely isn't worth it (need to probably do solder rework on smd components which if it isn't your primary business gets hairy quick).
```

---
## \#5 Posted by: rpn314 Posted at: 2017-07-07T17:09:21.380Z Reads: 60

```
Can you see which pins the bites lined up with? That would give a good idea of where to start. If you're seeing nothing at all, my guess is either the DRV chip or the 3.3v regulator. Either way, @wafflejock is right, you'll have to do some SMD soldering to replace those parts.
```

---
## \#6 Posted by: Boca Posted at: 2017-07-07T17:10:09.905Z Reads: 59

```
yeah I don't have the schematic. I believe the Nunchuk receiver is fried too. The voltmeter is beeping while connected between the ground and 3.3v... 
That sucks and don't know the reason yet... :S
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-07T17:13:56.437Z Reads: 57

```
Hmm yeah regarding the receiver, I've only really used the nrf modules for an extended period of time and they are very sensitive to extra voltage (they would run for a minute then get too hot and fry up completely).  Like @rpn314 said could be a blown voltage regulator but if that blew and was regulating voltage for the mcu as well or other ICs then it could have toasted other components strange that you don't see any physical damage but things can cook internally with no external sign of damage I suppose.  When I blew my VESC it was the DRV chip that cooked but saw some smoke and a little crater in the chip afterwards.
```

---
## \#8 Posted by: wafflejock Posted at: 2017-07-07T17:19:13.372Z Reads: 52

```
Also regarding schematic if it's a standard VESC it's open source hardware the schematics are on Benjamin Vedder's github I'm pretty sure (or on his site).
```

---
## \#9 Posted by: Boca Posted at: 2017-07-07T17:22:07.824Z Reads: 50

```
yeah right, I haven't seen any smoke or smell. I have an engineer background in electronics and electicity so I have some basics but haven't detected any signs of shortage except the visible bite on the red cable...
```

---
## \#10 Posted by: Boca Posted at: 2017-07-07T17:24:25.090Z Reads: 48

```
loosing 300$ without knowing the reason is annoying. The second VESC slave works ok, I am able to connect to the BLDC tool, read and detect it. However after a few minutes, the VESC warms up, the USB port gets supa hot and the error message shows error firmware reading... Can't go any further. I believe it might be this VESC which was faulty and damaged the master one...
```

---
## \#11 Posted by: wafflejock Posted at: 2017-07-07T17:42:43.802Z Reads: 44

```
Yeah don't get me wrong, I feel for ya I've cooked plenty of hardware, luckily most of it cheaper stuff.  Probably something like 75/25 my fault to manufacturers fault (or crap instructions).  I can't really add much about the two VESC setup since I've never run or setup dual drive myself but it does seem to be a gauntlet of potential issues.
```

---
## \#12 Posted by: rpn314 Posted at: 2017-07-07T22:18:44.894Z Reads: 43

```
If you fried the nunchuck receiver as well, my guess is that red cable coming in from the big capacitors/the battery shorted the 3.3v, 5v, and/or ground pins of the UART port. So my guess is still a fried 3.3v regulator and/or DRV.

@wafflejock I use the NRF modules with my nunchuck and I don't think I've ever fried an NRF module....

@Boca I don't know if you just had some bad luck or if the manufacturer was legimately careless. Unfortunately I'm leaning towards the latter. I soldered my own VESCs (dual setup) and the only issues I've had was the DRV chip, which was an issue with a bad firmware (bug in v2.18 about a year ago). But since I soldered it myself, I knew how to replace it myself so I just ordered the part and did it. While I don't suggest everyone solder their own, I do steer people as far away as possible from Maytech and other Chinese venders.

[quote="Boca, post:10, topic:26959"]
Can't go any further. I believe it might be this VESC which was faulty and damaged the master one...
[/quote]

How do you have the can-bus (what connects the VESCs to each other) wired? With the exception of a catarosphic explosion, the only way I see one directly affecting the other is if you have all 4 wires hooked up (VCC, RX, TX, and GND).

The only way I think it's possible
```

---
## \#13 Posted by: wafflejock Posted at: 2017-07-07T22:21:41.446Z Reads: 42

```
I had them burning up because the FTDI connector I got was supposed to be 3.3V but had 5V coming through the VCC, the arduino I was programming with it seemed to survive but if there was an NRF chip attached to it the chip cooked.  In normal operation with the correct voltage they're fine but take the 3.3 up to 5 and they cook after a minute or so of seemingly working fine.  Had me scratching my head till I checked the voltage on the FTDI board I have... now I just use a separate 3.3V supply or voltage regulator when I'm programming with that.

---

https://www.amazon.com/FT232RL-Serial-Adapter-switch-selectable/dp/B01KOMED8S/ref=sr_1_1?ie=UTF8&qid=1499466452&sr=8-1&keywords=deek+ftdi

Can see in the comments someone mentions the issue but I apparently hadn't read that comment.
```

---
## \#14 Posted by: Boca Posted at: 2017-07-09T04:18:12.334Z Reads: 38

```
yeah it is a good point about the canbus. I kinda messed up and didn't use the Canbus port but instead solder the 2 Rx master and RX slave and the Tx master with the Tx slave. but no ground or vcc. 
So I agree it is not the most standard way and it might actually not even work, but don't how could that damage the VESC... Please let me know if you think it might be the case...
```

---
## \#15 Posted by: rpn314 Posted at: 2017-07-09T04:54:41.348Z Reads: 38

```
@wafflejock Oh, got it. Yeah, I've always connected it to 3.3 or used a 3.3v regulator (when using them with Arduino or something), and I haven't used an FTDI board....what are you using that for exactly?

@Boca I think you did it right. To connect the canbus, you really only need to connect the Can-H and Can-L lines on the master and slave together (I wrote RX and TX above; it's actually H and L, sorry for the mistake), but you really dont need the ground or 5v connected between the VESCs. I asked because having the ground and 5v lines connected could have been how one fried the other.
```

---
## \#16 Posted by: Boca Posted at: 2017-07-09T20:22:06.520Z Reads: 32

```
yeah so in my case just to clarify, I connected the Rx Tx I2C port to I2C port.
```

---
## \#17 Posted by: rpn314 Posted at: 2017-07-09T20:53:37.356Z Reads: 31

```
....I2C? For what purpose were you connecting VESCs together on the I2C port? (Which is the same port as used for UART and SPI, reference picture below, from Vedder's site)

<img src="/uploads/db1493/original/3X/f/1/f1ea40a9ec2e11acedb4d90424c66d7a2ae43d5e.jpg" width="690" height="460">
```

---
## \#18 Posted by: Boca Posted at: 2017-07-09T21:06:56.957Z Reads: 31

```
ok so I plugged the nunchuck to the I2C port, as explained in the forum. The only difference is for the dual VESC where I connected directly the I2C to the other I2C port, of course no VCC or GND.

So it is kind of the same as having the nyko kama in parallel...
```

---
## \#19 Posted by: rpn314 Posted at: 2017-07-09T21:09:41.941Z Reads: 28

```
Oh, got it. Yeah, I think that's at least part of your problem (it would not have worked, probably unrelated to the frying issues). To my knowledge, the only port that can be connected in parallel like that is the ppm signal. The UART/I2C/SPI are 2 way communication ports and are thus a 1-to-1 connection.
Minimally, that explains how they were connected (I obviously didn't understand before). If there was a short from the battery coming in to either the TX or RX pins of that port, it could have easily transferred to the second vesc and fried both. I don't think the parallel RX/TX connection would have fried it, but it's possible.
```

---
## \#20 Posted by: Boca Posted at: 2017-07-09T21:19:17.485Z Reads: 26

```
there was no shorting between the Rx and Tx... the only issue is that I haven't tested the slave VESC in standalone. I connected it directly but I believe there was a default on the slave which burnt the master one... :frowning:
```

---
## \#21 Posted by: rpn314 Posted at: 2017-07-09T21:20:42.292Z Reads: 23

```
Sorry, I just edited my post for clarity. I didn't mean a short between them but to either (or both) from the big red wire going to the battery (as you'd indicated before)
```

---
## \#22 Posted by: Boca Posted at: 2017-07-09T21:27:20.464Z Reads: 24

```
yeah gotcha, thx for clarifying
```

---
## \#23 Posted by: rpn314 Posted at: 2017-07-09T21:54:20.214Z Reads: 22

```
Okay, now that I (think I) fully understand how you had it set up, let's see if we can get them resurrected!

So VESC 1 (what was originally your master) doesn't turn on at all. No lights, no heat, but you do see 18V on the 5V can-bus pin, correct? I think this one at least has a dead DRV chip (it has the buck converter to supply 5V everywhere else). No way to fix this but replace it. @JohnnyMeduse is the DRV wizard in both name and practice.

VESC 2 (what was the slave) powers on, connects to BLDC-Tool, etc, but the USB jack itself heats up quickly and at that point it disconnects from BLDC-Tool, correct? If it doesn't get too hot to touch, can you check if any other chip gets hot?
```

---
## \#24 Posted by: Boca Posted at: 2017-07-09T22:25:28.567Z Reads: 20

```
Right you got it! :) for the slave vesc there are also someother components getting pretty warm like I can't leave my hands on.
```

---
## \#25 Posted by: rpn314 Posted at: 2017-07-09T22:28:12.155Z Reads: 19

```
Which components exactly? (Don't burn yourself!) Don't worry about the names of the components; you can take a picture and circle them or whatever works. I'm asking cause I'd be surprised if it was the USB connector itself
```

---
## \#26 Posted by: Boca Posted at: 2017-07-10T01:20:14.334Z Reads: 20

```
So I feel a little concern about plugging the faulty VESC again. I would rather send it back to maytech in this state to let them confirm that it has a shorting...
```

---
## \#27 Posted by: rpn314 Posted at: 2017-07-10T01:50:44.304Z Reads: 21

```
That's a good call if you can. I thought you'd taken the wrap off both. Go for it!
```

---
## \#28 Posted by: Boca Posted at: 2017-07-10T02:07:20.713Z Reads: 22

```
Right, I took the wrap off afterwards to take some metrix of the regulators... They are already saying they won't accept the return....
```

---
## \#29 Posted by: rpn314 Posted at: 2017-07-10T02:25:31.220Z Reads: 22

```
Well just tag or PM me if they don't accept it/you want to diagnose some more.
```

---
