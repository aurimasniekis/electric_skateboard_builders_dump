# Board cutting out during acceleration

### Replies: 41 Views: 1871

## \#1 Posted by: ARollNation Posted at: 2017-10-01T22:59:14.228Z Reads: 196

```
Hey all,

So I recently got my E-board up and running but I am experiencing power loss upon acceleration. When throttling up on the nunchuck it will consistently accelerate to a certain speed then start to lag/cut out.

Running 10s with a 190kV motor. 12:40 ratio with 97mm thanes.

Took a couple pics of my BLDC tool. I feel like I have a few settings wrong given my setup. 

<img src="/uploads/db1493/original/3X/c/a/ca9aaee61e62c4c2a4607c5be2afa94b76c3eefd.png" width="690" height="351">

<img src="/uploads/db1493/original/3X/6/c/6c51e9eca65cec3d2573e23cc9fe833e6e9ef61d.png" width="690" height="349">


Any advise would be greatly appreciated, Thanks!
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-10-01T23:02:31.940Z Reads: 166

```
The issue is your remote if you experience a immediate power loss. So if the power drops out and back on like a on off switch then your remotes signal drops out. Nothing you can fix by VESC settings. Just try to place your receiver at a better place (not near phase wires, not inside a carbon enclosure)
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-10-01T23:05:22.340Z Reads: 160

```
See if you can go into the terminal and type faults, see if anything comes up. Also, post up a screenshot or two of the realtime graphs, see if you can catch it acting funny.
```

---
## \#4 Posted by: ARollNation Posted at: 2017-10-01T23:11:15.387Z Reads: 156

```
Yea its immediate. I noticed it act a little better when I hung my hand with the nunchuck lower towards the deck of the board. Besides readjusting the location of my RX, any other known methods of boosting the bluetooth signal coming from the TX/RX?

Also, is the -70A regen too high for my batteries? I got 2 5s 5Ah Lipos in series
```

---
## \#5 Posted by: ARollNation Posted at: 2017-10-01T23:13:20.268Z Reads: 142

```
no fault codes when I ran it earlier today.. I can get it hooked up to the real-time graph in about an hour, I'm away from the board at the moment. Do you have any idea how much Voltage can drop under load?
```

---
## \#6 Posted by: scepterr Posted at: 2017-10-01T23:14:38.460Z Reads: 145

```
Your battery cut off might be too high it'll hit 37V at cont load
Drop both values 2V, test
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-10-01T23:37:45.776Z Reads: 136

```
The nunchuck is known for dropping out under load. I guarantee that a new remote (like the mini from @JLabs) will solve your problem
```

---
## \#8 Posted by: ARollNation Posted at: 2017-10-02T20:55:56.418Z Reads: 111

```
Hey I think you were right, I was having too much voltage sag and when I would accelerate too fast it would dip too low and reset the VESC. I switched my cutoff start to 33V (3.3v per cell) and that did the trick!
```

---
## \#9 Posted by: Battosaii Posted at: 2017-10-02T23:40:47.012Z Reads: 103

```
same issue, my board was working fine for months but now im having drop outs at random, accelerating and braking....
```

---
## \#10 Posted by: Namasaki Posted at: 2017-10-02T23:56:21.489Z Reads: 99

```
If your running Li-ions, you should be able to go lower than 33v.
```

---
## \#11 Posted by: ARollNation Posted at: 2017-10-03T00:12:48.283Z Reads: 99

```
Nah I'm runnin LiPos. 3.3 is ok for them right?
```

---
## \#12 Posted by: GrecoMan Posted at: 2017-10-03T00:13:57.865Z Reads: 98

```
I’d raise it to atleast 3.5.  3.3 is a bit low for lipos
```

---
## \#13 Posted by: Namasaki Posted at: 2017-10-03T00:19:58.594Z Reads: 101

```
I agree with @GrecoMan 3.3 is low for Lipos because you can not go below 3.0 on any cell.
If you let the vesc take your battery down to 33 total, it could have a cell go below 3.0.
I run my cutoff start at 34v with Lipos buy I also monitor my voltage with a meter mounted through the deck and I never ride it below 36v (although I did once to do a range test) and most of the time I don't ride it below 38v at rest. But then again, I'm a recreational rider not a commuter.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-10-03T00:23:21.443Z Reads: 93

```
I am absolutely sure that this was not the issue. The battery cutoff start and end works very smooth. So you would nit experience a immediate cutout. And the VESC doesn't restart, it simply reduces the power until the voltage is ok again.

Think what you experienced was simply a run without remote cutouts.
```

---
## \#15 Posted by: scepterr Posted at: 2017-10-03T00:31:59.061Z Reads: 92

```
[quote="ARollNation, post:1, topic:34523"]
So I recently got my E-board up and running but I am experiencing power loss upon acceleration. When throttling up on the nunchuck it will consistently accelerate to a certain speed then start to lag/cut out.
[/quote]

@Ackmaniac I don't think his vesc was resetting, just hit hitting the low voltage slowdown thus not  accelerating
```

---
## \#16 Posted by: Namasaki Posted at: 2017-10-03T00:32:27.497Z Reads: 92

```
Unless his voltage dropped so fast that it hit 37and within 1 second hit 35  so that the vesc started to cut power and then shut down.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2017-10-03T00:38:21.129Z Reads: 91

```
It only shuts down below 8V (Minimum input voltage)
```

---
## \#18 Posted by: Namasaki Posted at: 2017-10-03T00:40:30.588Z Reads: 94

```
[quote="Ackmaniac, post:17, topic:34523, full:true"]
It only shuts down below 8V (Minimum input voltage)
[/quote]


I see, but loss controller connection would make it shut down either though right ?

You know at first he said it was just lagging and cutting out.
Later he said the vesc was reseting. So I'm wondering if it was reseting or just cutting back.
```

---
## \#19 Posted by: ARollNation Posted at: 2017-10-03T00:42:28.365Z Reads: 92

```
Thanks @GrecoMan @Namasaki for the input on the cutoff I'll raise it 1 or 2 volts to play on the safe side.

I've only went on one ride around the block today with the new settings saved, I'll check back in when I have spent some more time on the board.
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-10-03T00:42:45.370Z Reads: 88

```
loss of connection would result in a immediate power loss (like on-off). No shut down. Only the command for power is missing
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-10-03T00:44:11.012Z Reads: 85

```
If you are aiming for the most charge cycles (while still maintaining a decent range), the best way is to only charge your lipos up to to 4.1v instead of 4.2 and discharge to 3.5v. Charging to 4.1v should double the amount of charge cycles for you batteries
```

---
## \#22 Posted by: ARollNation Posted at: 2017-10-03T00:45:20.148Z Reads: 85

```
What remote are y'all runnin/recommend? @Ackmaniac @Namasaki @scepterr
```

---
## \#23 Posted by: GrecoMan Posted at: 2017-10-03T00:47:21.628Z Reads: 86

```
Lol, the one person you didn’t tag...

I highly recommend the mini remote, rock solid reliable and cheap.  I bet the other guys will agree with me
```

---
## \#24 Posted by: ARollNation Posted at: 2017-10-03T00:47:48.195Z Reads: 85

```
Oh that's interesting I didn't know that last 5-10% charge makes that much of a difference over the batteries life. Thanks for the tip!
```

---
## \#25 Posted by: ARollNation Posted at: 2017-10-03T00:48:36.152Z Reads: 82

```
Haha cuz you recommended it to me yesterday 😎 I appreciate your help and advise my man!!
```

---
## \#26 Posted by: scepterr Posted at: 2017-10-03T00:48:38.331Z Reads: 81

```
I'm using the nano-x, no complaints.
```

---
## \#27 Posted by: GrecoMan Posted at: 2017-10-03T00:50:35.811Z Reads: 80

```
Oh shoot! Did I really? Lol well my opinion hasn’t changed 😂
```

---
## \#28 Posted by: Namasaki Posted at: 2017-10-03T00:54:56.910Z Reads: 78

```
I still charge my batteries to 4.2 I don't care what the battery university says.
Been charging them full for over a year now and their still going strong.
Besides Lipos are easy to replace.
```

---
## \#29 Posted by: scepterr Posted at: 2017-10-03T16:32:24.459Z Reads: 74

```
I don't think you would notice any affect till atleast 200 cycles. There really is no gain to charging to 4.2 Vs 4.1 in terms of usable capacity. This is a little test I ran with a hundred identical cells and this was the result. 
<img src="/uploads/db1493/original/3X/0/a/0a79d57c199850663a227859a170823814863b6a.png" width="690" height="171">
```

---
## \#30 Posted by: Namasaki Posted at: 2017-10-03T18:16:02.967Z Reads: 72

```
I can't say for sure that my bms will balance my cells if I stop charging below 4.2
```

---
## \#31 Posted by: scepterr Posted at: 2017-10-03T18:16:43.084Z Reads: 71

```
Yeah with BMS that's tricky they tend to only balance at their detected full charge
I get mine with 4.1 cutoff
```

---
## \#32 Posted by: Namasaki Posted at: 2017-10-03T18:19:07.091Z Reads: 72

```
I just checked, the balance voltage on mine is 4.2v
So you got your balance voltage set at 4.1v ?
```

---
## \#33 Posted by: scepterr Posted at: 2017-10-03T18:25:40.576Z Reads: 73

```
Yeah, I'm also using custom charger that'll charge whatever S configuration to 4.1*S  with this it does normal CC charge curve just at 4.1 instead of 4.2
<img src="/uploads/db1493/original/3X/f/6/f696da1e71281550acf6e34dfe38e03813bbd9ec.jpg" width="666" height="499">
```

---
## \#34 Posted by: ARollNation Posted at: 2017-10-04T23:39:23.580Z Reads: 69

```
Update: After taking it for a couple more rides the dropouts and throttle sticking is still occurring. I ordered a clip on ferrite ring to see if that will help. If not, it looks like I'll be buying a new remote haha
```

---
## \#35 Posted by: sunerphey Posted at: 2017-10-11T15:52:08.966Z Reads: 65

```
Is your motor mount plastic ?
```

---
## \#36 Posted by: ARollNation Posted at: 2017-10-11T18:01:08.328Z Reads: 68

```
no its welded .25" Aluminum flat-bar
```

---
## \#37 Posted by: sunerphey Posted at: 2017-10-11T20:01:16.582Z Reads: 65

```
I have similar problems and the cause is voltage spikes from the motor which are with very high voltages (in some cases over 5mm through the air to the scooter aluminium body). I think giving an easy path outside for a small spike can save the vesc, but not 100% sure.
```

---
## \#38 Posted by: ARollNation Posted at: 2017-10-30T01:04:24.808Z Reads: 61

```
Just wanted to give everyone an update:

After purchasing a new remote from @JLabs the cutting out problem was completely diminished. Been riding around for almost a month with no issues whatsoever.

Thanks for all the help and support guys!

-AAron
```

---
## \#39 Posted by: GrecoMan Posted at: 2017-10-30T01:05:36.226Z Reads: 62

```
Glad you got it figured out!
```

---
## \#40 Posted by: fakesantos Posted at: 2018-05-17T14:12:08.715Z Reads: 41

```
Why was the remote the problem?  How would that force the vesc to reset?
```

---
## \#41 Posted by: ARollNation Posted at: 2018-05-17T22:23:48.998Z Reads: 39

```
I’m not sure if it forced the Vesc to reset I think that it had to do with the fact that the Bluetooth signal was not strong enough to maintain connectivity the whole time given the fact those brushless motors can cause some interference from their magnetic field when under throttle. So once I was giving some throttle the power would cut out and the controller would blink telling me the signal was lost.

As much as I wanted to use the nunchuck it just wasn’t worth the bother of all the cutouts. Any 2.4ghz controller and receiver will perform far better than the nunchuck
```

---
