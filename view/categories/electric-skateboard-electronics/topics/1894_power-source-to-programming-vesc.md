# Power source to programming vesc

### Replies: 23 Views: 2621

## \#1 Posted by: Vito Posted at: 2016-03-21T04:34:03.318Z Reads: 196

```
Hi. I'm using 10s lipo (2 5s in series) in my build but to programming the vesc's I'll be using 3s lipo to be safe. I have been reading all the vesc info that i found in this forum but still have some questions. So if im programming and doing the motor detection with 3s lipo, lets say 11.1v, i will be get my vesc right to run 10s? Can i program with the 3s lipo and set the cut off for my 10s battery? How do you guys do? What im saing is when you are doing motor detection with 3s you get different specs like if you was doing with 10s. If somebody can help me with this i will be glad. Regards from Toronto
```

---
## \#2 Posted by: gamma2 Posted at: 2016-03-21T18:56:29.657Z Reads: 186

```
I am also interested in this. I don't have access to a lab power supply for a couple weeks and would like to setup my VESC with a 3s 1.5Ah LiPo. Many of the guides make no mention of power supply during setup.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-03-21T20:40:42.840Z Reads: 181

```
My understanding is you should use a regulated power supply, as it has protections from short circuits and spikes, while lipos without fuses do not have any protection from shorts or spikes.

Even a 3s lipo puts your vesc at risk. I bought a regulated power supply on amazon for $45 USD, which works great, and is half the cost of a vesc. Better to be safe than sorry.

It shouldn't be a big deal if you don't use a regulated power supply. But its like anything else that's dangerous. You don't expect to get hit while driving, but it happens. That's why you have insurance, seat belts, and airbags. Similarly, you shouldn't have issues configuring your vesc with a battery instead of a regulated power supply. But spikes can occur that will fry your vesc, so its best to use a regulated power supply, which acts as your seat belt and airbag when spikes do occur.

And like I said, they are available for less than half the cost of a vesc.

In terms of motor detection, I had no issue with my settings doing the motor detection at 11.1 volts with my regulated power supply, and then using a space cell (which is a 10s) as the power source to be used while riding.

Maybe someone with more experience can elaborate as to why it works, but I can tell you from experience, that it does work.
```

---
## \#4 Posted by: gamma2 Posted at: 2016-03-21T20:50:32.581Z Reads: 160

```
Is it that likely to occur though? It seems that if its able to run at 12s that 11.1V shouldn't be that likely to kill. I also saw a couple of mentions of being able to use a laptop power supply. Do you know anything about how to accomplish that?
```

---
## \#5 Posted by: evoheyax Posted at: 2016-03-21T21:00:46.531Z Reads: 157

```
I can't speak of how likely it is to happen. I did configure some using the space cell as I was curious myself. I had no issues. However, onloop for example has nothing to gain (and possibly business to lose from those turned off by this) by recommending the use of a regulated lab power supply. The fact he is saying this speaks to say it has happened to his customers (and possibly himself), and could happen to you.

As for the laptop power supply, many run at 1.5 or 2 amps. If you cut a laptop power supply cable off at the end you would plug into your laptop, you should find a positive and a negative wire that can be hooked up the the positive and negative of your vesc. I personally, feel sketched by this idea. I feel like if you don't know what your doing, you could short you could cut into the wires when stripping the shielding off without noticing this, and cause a short when you plug it to your vesc. I feel better using the battery itself personally.

But again, the best option to avoid any issues whats soever is to use a regulated power supply.
```

---
## \#6 Posted by: gamma2 Posted at: 2016-03-21T21:03:33.217Z Reads: 152

```
So a laptop supply would probably be safer than using a 3s LiPo.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-03-21T21:07:59.965Z Reads: 150

```
If you do it correctly, yes. That box inline of your power supply would break before your vesc would if a spike occurred.

But you need to be careful stripping the wires. You will need to solder also. You could also find a female adapter for your laptop power supply so you don't have to cut an cables, which I think would be safer. But you would have to find the right female plug for it to plug into.
```

---
## \#8 Posted by: gamma2 Posted at: 2016-03-21T21:11:32.804Z Reads: 144

```
I figured I would just strip the ends and solder on bullets or even an XT90-S just to be extra safe.
```

---
## \#9 Posted by: Vito Posted at: 2016-03-21T22:02:09.003Z Reads: 141

```
thank you for your reply!! Voltage regulator sems to be the way to go but i dont have access to it right now i will buy one probably. But i gonna try with lipo with xt90 anti spark. So you do the motor detection at 11.1v then you program the esc for running the space cell and no problem at all?
```

---
## \#10 Posted by: evoheyax Posted at: 2016-03-22T01:11:38.103Z Reads: 138

```
Yes. You will have issues running the motors at low voltage. But the detection will work, and once you plug it into your battery, the motors should work.
```

---
## \#11 Posted by: gamma2 Posted at: 2016-03-22T19:49:51.778Z Reads: 132

```
So I have two different laptop power supplies. One is 12V @ 2.5 amp. The other is 8.4V at 1.5 amp. Any idea which would be preferable?
```

---
## \#12 Posted by: evoheyax Posted at: 2016-03-22T21:03:33.452Z Reads: 126

```
Lower amps is better. However, the biggest reason to use them is to protect from spikes, which both should do. And since both are pretty close in voltage and both are low in amps, either is fine. Anything low amps between 8V – 60V is fine.
```

---
## \#13 Posted by: DougM Posted at: 2016-03-23T00:18:24.998Z Reads: 121

```
I would be careful with switching power supplies like laptop supplies.  I had all sorts of problems with VESC and motor configuration using an old PC power supply - they aren't designed for the heavy loads a quick motor spin up can put on them.  I finally just dug up 2 small 12V lead acid batteries and wired them in series.  No safeties but I've never smoked a VESC during configuration.

Advantage that it exactly matches the voltage of my 6S configuration

DougM
```

---
## \#14 Posted by: Vito Posted at: 2016-05-03T02:20:58.846Z Reads: 109

```
i have been using es lipo 1000mah to run motor detection and no problems so far.
```

---
## \#15 Posted by: ambrojohn Posted at: 2016-06-29T03:19:18.194Z Reads: 101

```
How do you set your regulated power supply? In particular which current level?
```

---
## \#16 Posted by: mason Posted at: 2016-06-29T04:12:25.532Z Reads: 101

```
If you are buying from ollin, no need to because he already did initial setup on it. After initial setup you're fine with your normal batteries.
```

---
## \#17 Posted by: ambrojohn Posted at: 2016-06-29T04:23:07.572Z Reads: 102

```
I did buy it from Ollin (still have to arrive though).
But I have to re-program it for a personal project.
```

---
## \#18 Posted by: mason Posted at: 2016-06-29T04:31:32.659Z Reads: 102

```
then you should be fine with your normal batteries
```

---
## \#19 Posted by: Nordle Posted at: 2016-06-29T04:47:20.290Z Reads: 102

```
I use my normal battery and a 5A fuse while doing detection or other settings.
Fuse keeps it simple and does the thing;)
```

---
## \#20 Posted by: ambrojohn Posted at: 2016-07-06T07:35:24.226Z Reads: 88

```
Yet I have a regulated power supply and I would like to use it.
So I can set it , say, 12V and 5A? or is 2A safer?
```

---
## \#21 Posted by: ambrojohn Posted at: 2016-08-11T01:34:11.984Z Reads: 67

```
At the end I use a regulated power supply either at 21.2V (you can choose any value I guess) and 4A limited current.
```

---
## \#22 Posted by: ambrojohn Posted at: 2016-08-11T01:36:40.460Z Reads: 67

```
Question:
When I power the VESC from external source and operate it, can I leave the st-link debugger USB dongle connected to the VESC (but disconnected from the PC)?

I noticed that the VESC makes the little led on the usb blinking and I was wondering if that may be a problem.
```

---
## \#23 Posted by: ambrojohn Posted at: 2016-08-11T02:04:16.196Z Reads: 64

```
I have just realized myself that the VESC does not start with the debugger plugged in. Even with the 3.3V and GND pin disconnected
```

---
