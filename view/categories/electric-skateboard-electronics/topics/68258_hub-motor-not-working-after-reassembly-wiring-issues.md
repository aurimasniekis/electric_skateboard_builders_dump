# Hub Motor Not Working After Reassembly&hellip;.Wiring Issues

### Replies: 23 Views: 926

## \#1 Posted by: jackgr83 Posted at: 2018-09-16T21:24:34.765Z Reads: 95

```
Hello All,

I recently decided to disassemble my hub motor budget board(Skatebolt). I did this because the board was beeping at me mid-ride and motors stopped working at 75% battery. I decided to unplug everything under the enclosure and then plug it back up for a reboot and educational purposes. However, as I was re-connecting the phase wires, one of the metal wire connectors on one of the phase wires snapped, so I had to strip back the wire enclosure, twist both wires together, and connect them with a wire cap connector(wire nut). Now, when I turned everything back on and applied acceleration, the hub motor with the phase wires leading into it that I "wire-nutted" back together works fine, but the other hub motor whose phase wires I did not snap and were reconnected in the same way I found them is not working. I am wondering if I confused the ESC or something by using the wire nut, and all the power is just going to that motor. 
I have attached a couple pictures to show what I did. The first picture shows the wires of the motor that works, and the second picture shows the wires of the motor which does not work. Any help or suggestions is greatly appreciated!

![HUB1|690x335](upload://t6ytRlmdYkBpm3k6NSHndN7cavO.jpg)
![HUB2|243x500](upload://26MtaFb6Azh01knZxRnYO4gyNAF.jpg)
```

---
## \#2 Posted by: dareno Posted at: 2018-09-16T22:00:35.849Z Reads: 84

```
You haven't confused it with that wire nut but you may have shorted the phase wiring to the other motor(the blue green yellow ones) They look very close together there in the top pic.  First thing to do is unplug the battery connection which will probably be a yellow connector (xt60) with red and black wiring.  (Hope I'm not being patronising here my friend but you seem new to this)   Make sure the insulating covers are back on the motor wires.  Try Removing the sensor wires to both motors. They are the thin red yellow blue green black wires coming from the motors with the white connectors
![cbfcc4de3369c987a616f86972339420d990a28c_1_690x335_LI|690x334](upload://VVeAa0H7pOSeY7urirujUu0PVe.jpg)
 Plug the battery back in and give it a go.  If the motor still doesn't turn then you have most probably fried the esc but most of the time when those esc's fail they fail on both motors so its a bit strange.  
Can you take a pic of the whole esc for me?
```

---
## \#3 Posted by: jackgr83 Posted at: 2018-09-16T22:58:03.498Z Reads: 69

```
Hi Dareno,

No luck. I did as you said and tried without the sensor wires and still had the same problem. I will add that when I turn the board and try to free-spin both wheels with my hand, the motor that does not work has a lot more resistance to it. It feels similar to screwing on a gas cap or medicine bottle top where there is resistance in clicks, if that makes sense. It only has this resistance to it though when the board is on. The other wheel free spins fine. Therefore, I do not believe I fried the esc....at least hopefully not, but it does feel like the motor is stuck somehow. Here are pictures of the esc. Top one is a close up with the board off, and the bottom picture shows the board on, with the one motor spinning. Also, working on uploading a video.
Thank you for helping, I greatly appreciate it.

Jack

![HUB4|243x500](upload://sKhOmJpkachLSaeic5XeVZaSCJr.jpg)
![HUB3|243x500](upload://8E59hlcyeT5QD3AvLiqUJ1yJeJ0.jpg)
```

---
## \#4 Posted by: J0ker3366 Posted at: 2018-09-16T23:23:38.861Z Reads: 53

```
Can you get a closer shot of the esc? Need to see more details on it.
```

---
## \#5 Posted by: J0ker3366 Posted at: 2018-09-16T23:31:29.137Z Reads: 50

```
I had some Genesis hubs that did the same thing but both motors. I ended up taking the hubs apart, cleaned the inside, did a very light sanding to remove imperfections, put back together and they were good to go. Not saying it will fix it but its worth a try. 

If you have a voltmeter, check voltage and continuity on every wire. Wait! Have you tried flipping the motors? Meaning wire the problem hub to the working phase wires. If it spins, its most likely the esc. If it doesn't then you're looking at new hubs.
```

---
## \#6 Posted by: goldrabe Posted at: 2018-09-16T23:59:51.535Z Reads: 44

```
What is the not working hub doing, does it stutters or makes strange noises when accelerating?
```

---
## \#7 Posted by: J0ker3366 Posted at: 2018-09-17T00:02:59.081Z Reads: 45

```
Not trying be an ass or anything but he describes everything in his previous posts...
```

---
## \#8 Posted by: goldrabe Posted at: 2018-09-17T00:09:36.335Z Reads: 40

```
He just says they are not working, but not in which way, that's why I was asking.
```

---
## \#9 Posted by: J0ker3366 Posted at: 2018-09-17T00:11:06.537Z Reads: 44

```
[quote="jackgr83, post:3, topic:68258"]
Hi Dareno,

No luck. I did as you said and tried without the sensor wires and still had the same problem. I will add that when I turn the board and try to free-spin both wheels with my hand, the motor that does not work has a lot more resistance to it. It feels similar to screwing on a gas cap or medicine bottle top where there is resistance in clicks, if that makes sense. It only has this resistance to it though when the board is on. The other wheel free spins fine. Therefore, I do not believe I fried the esc…at least hopefully not, but it does feel like the motor is stuck somehow. Here are pictures of the esc. Top one is a close up with the
[/quote]

You sure about that?
```

---
## \#10 Posted by: J0ker3366 Posted at: 2018-09-17T00:12:23.018Z Reads: 40

```
And now that I read that again, @dareno, could it be stuck in brake mode? Like its shortex out to have constant brake on?
```

---
## \#11 Posted by: jackgr83 Posted at: 2018-09-17T00:13:09.362Z Reads: 38

```
Thanks for the advice. I'm going to try that tomorrow when I have some free time.
```

---
## \#13 Posted by: jackgr83 Posted at: 2018-09-17T00:16:44.977Z Reads: 39

```
It does nothing, makes no noises. The only thing noticeable is the resistance when trying to free spin it.
```

---
## \#15 Posted by: dareno Posted at: 2018-09-17T00:45:52.688Z Reads: 36

```
You definitely disconnected the sensors?  It sounds like a sensor issue to me.  Especially with the motor resisting when on.  Spins freely when off?  
You could try to swap the motors over but don't connect the bad one to the esc just the good one to the bad side.  That way you isolate the motor issue from the esc. You are much less likely to hurt a motor with an esc than you are to hurt an esc with a motor.  At least then you know the speed controller is cool.  If you get the same issue then your esc is toast. If you don't then there is an issue with the motor.  Again though its a strange issue with that set up.  Those duals fail completely usually not side by side in my experience. Aint diy fun??:roll_eyes:
```

---
## \#16 Posted by: goldrabe Posted at: 2018-09-17T00:48:55.205Z Reads: 36

```
Maybe he confused the sensor plugs, to try swopping them might solve it.
```

---
## \#17 Posted by: dareno Posted at: 2018-09-17T00:59:24.474Z Reads: 39

```
I asked him to disconnect completely so that shouldn't be an issue.  Those controllers work fine without sensors.
@jackgr83 whats this?
![c97858a889ec1da39cc69912fbfb56cc2e283b29_LI|242x500](upload://6SLFgCKwdnxewUp0mBf19jQE05a.jpg)
```

---
## \#18 Posted by: goldrabe Posted at: 2018-09-17T01:04:49.988Z Reads: 37

```
Yeah that put me off too.
And usually when having them swopped it stutters. The colors from the phase wires are matching too, but for me it looks like they are shorted in some way.
```

---
## \#19 Posted by: jackgr83 Posted at: 2018-09-17T01:13:29.786Z Reads: 37

```
Those two white wires connect from the esc to two separate LED lights on the outside of the enclosure which you can see on either side of the motor cables in the picture. One of them actually broke, but I would not think that would affect the motor, just the lights.
```

---
## \#20 Posted by: jackgr83 Posted at: 2018-09-17T01:14:29.894Z Reads: 35

```
I am going to try this tomorrow, and I did definitely disconnect the sensors.
```

---
## \#21 Posted by: jackgr83 Posted at: 2018-09-17T01:19:20.293Z Reads: 34

```
@goldrabe Actually I did switch the sensors, and then the working motor did that stuttering, but the other motor still did nothing.
```

---
## \#22 Posted by: goldrabe Posted at: 2018-09-17T01:32:14.223Z Reads: 33

```
Yeah I think the best advice is what @dareno said, trying to swop the motors.
I had three ESC'S of this kind some with matching phase wire colors some with non matching. I wired them in maybe all possible ways but when wrongly wired they always made some kind of noise or where stuttering.
I hope you can solve it without having to buy new parts!
```

---
## \#23 Posted by: dareno Posted at: 2018-09-17T01:37:07.990Z Reads: 33

```
Timezone issues lol  good night man.  let us know.
```

---
## \#24 Posted by: jackgr83 Posted at: 2018-10-13T21:54:18.818Z Reads: 23

```
Update: It's the ESC/Power board that is the problem. Both motors work fine. Now, with battery and motors working, I just need a new esc, power board, remote control, etc.

Or could just get this: http://www.diyeboard.com/dual-hub-motor-esc-speed-control-kit-p-560.html
```

---
## \#25 Posted by: Enabledmoon Posted at: 2019-09-25T05:33:48.235Z Reads: 7

```
When I replaced my motors they had one different color so I assumed that was the one for the other differing color, but when I plugged the battery in sparks came from the yellow 12V battery connectors I put together. This fried the positive side of the connector. I switched the one weird wire with the next best and got even more sparks and the connectors are completely done. There’s nothing out of the ordinary about any other wire or connection. There would had to of been a draw of power right?
```

---
