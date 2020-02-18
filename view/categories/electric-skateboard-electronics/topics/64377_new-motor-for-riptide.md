# New motor for riptide?

### Replies: 28 Views: 669

## \#1 Posted by: Chelloo Posted at: 2018-08-09T20:34:56.297Z Reads: 160

```
Anyone know what kind of upgrades I can give this board using its VESC? are there better quality motors I can use to increase speed?

![image|600x400](upload://rgSNGyvZ5ihpichgwEK7vv27l9J.jpg)
1800watt motor
```

---
## \#2 Posted by: telnoi Posted at: 2018-08-09T20:45:34.561Z Reads: 150

```
Not really. It does not have a vesc. The esc amp output is hard coded/limited, along with the KV for which the esc is optimized. Then there is the standard battery pack that limits the performance.

You may be able to increase speed by choosing a slightly higher kv motor, but then again the esc might limit the rpm. On top, you will decrease torque.

The downside with any of these boards is that all parts more or less go together with very limited ways of adjusting individual components without having to up the specs of other components in addition to achieve the desired results.
```

---
## \#3 Posted by: Chelloo Posted at: 2018-08-09T20:51:40.365Z Reads: 146

```
So best I can do is add a battery pack in parallel to extend run time? Or use the enclosure and brackets then build my own VESC, Motor and battery combo?
```

---
## \#4 Posted by: telnoi Posted at: 2018-08-09T20:54:12.320Z Reads: 132

```
Depends on why you think the board does not meet your current needs. Does it slow down during hill climbs? If so, it may not even be the motors but severe voltage sag.

What don't you like about it and what are you hoping to achieve.
```

---
## \#5 Posted by: Skunk Posted at: 2018-08-09T21:00:45.698Z Reads: 120

```
The sag on the R1 is real. 
You get that 20mph for a few blocks if you ride hard. Then it slows down. 
I'd be Happy with longer battery life on my R1.

I'll build a new short board after my current build.
```

---
## \#6 Posted by: Chelloo Posted at: 2018-08-09T21:00:48.798Z Reads: 115

```
longer run time and stronger hill climb. I don't think id be able to go any faster with the safety features built in.
```

---
## \#7 Posted by: DAddYE Posted at: 2018-08-10T16:22:22.202Z Reads: 93

```
Check my thread on reddit.  Get a Sanyo 10s2p from meepo or similar. Unsold the jumper on the ESC so it would allow the motors to run fine on 10s. If still not satisfied get 2 5055 mytech and replace the originals. I wouldn’t suggest yet to get VESC. Those motors use way too much amps. You’ll fry it.
```

---
## \#8 Posted by: Skunk Posted at: 2018-08-10T17:13:41.124Z Reads: 88

```
You got links @DAddYE?
```

---
## \#9 Posted by: Jaraya92881 Posted at: 2018-08-10T17:29:50.661Z Reads: 88

```
Add a vesc and immediately see the power and efficiency difference. Then add a better battery with Samsung 30q or 25r cells.Night and day compared to those cheap cells on the lower end model.
```

---
## \#10 Posted by: Jaraya92881 Posted at: 2018-08-10T17:31:28.403Z Reads: 89

```
Negative, you can limit power and the vesc will be fine. Ive used those motors on Iwonder builds before we release the pulseboards echo with hubs and with vesc  it's not going to fry the vesc unless you configure it incorrectly .
```

---
## \#11 Posted by: DAddYE Posted at: 2018-08-11T06:18:57.056Z Reads: 75

```
Here you go: https://www.reddit.com/r/ElectricSkateboarding/comments/8ey4dd/riptide_conversion_to_10s2p_sanyo/
```

---
## \#12 Posted by: Skunk Posted at: 2018-08-11T06:46:49.608Z Reads: 73

```
@DAddYE it Sounds like going from 6s3 to 10s2 made a big difference. I might just do that. Probably not until my other board is done tho.
Unless a battery comes up at a deal.
Altho this 10s2 is cheap....
http://www.diyeboard.com/10s2p-lgsamsung-18650-lithiumion-battery-pack-36v144wh-p-461.html
```

---
## \#13 Posted by: pat.speed Posted at: 2018-08-11T07:54:35.466Z Reads: 63

```
It needs to be one of the new battery packs that use the high current cells from meepo, those packs will be just as bad with voltage sag. 

A 30q 10s2p would be the best option although more costly
```

---
## \#14 Posted by: Skunk Posted at: 2018-08-11T07:58:53.945Z Reads: 60

```
I figured as much. I'd honestly rather start Gathering parts for a second build after my hummie deck then put money into the riptide
```

---
## \#15 Posted by: pat.speed Posted at: 2018-08-11T07:59:14.884Z Reads: 58

```
Yeah thats a good idea
```

---
## \#16 Posted by: Skunk Posted at: 2018-08-11T08:07:24.173Z Reads: 58

```
$255 would be enough to get me into my first spot welder and supplies to start practicing making my own damn batteries
```

---
## \#17 Posted by: Skunk Posted at: 2018-08-11T08:33:59.850Z Reads: 52

```
If a Used one pops up for cheap though I'm  jumping on that ish.
```

---
## \#18 Posted by: Chelloo Posted at: 2018-08-13T16:10:41.414Z Reads: 49

```
This is a pretty cool read! So what do you think so far? You changed to a 10s battery and unsoldered the 2 joints to make it 10s capable, or have you changed the vesc all together? the breaking sucks on this board as well, have you done anything to resolve this?
```

---
## \#19 Posted by: telnoi Posted at: 2018-08-13T17:01:55.720Z Reads: 47

```
The used esc is a a cheap solution that is offered by multiple resellers, including diyeboard.

It offers no customization other than soldering or desoldering bridges for different voltage ranges. The braking strength is hard coded as are all other firmware related features, thus other than changing modes there is little you can do.

Again, there is a dependency if you exchange components. If you indeed start using vesc related hardware, you can adjust the braking strength, but you will limited by how much amps you can push towards your Li-Ion pack during regen braking, which will be better and you can tune it to your liking, but the max brake strength will be limited by max amp.

Besides upgrading to a vesc and using a higher amp discharge/charge li-ion pack to allow for improved regen braking, bigger motors will also impact braking strength. It's all related.
```

---
## \#20 Posted by: Chelloo Posted at: 2018-08-13T17:31:08.930Z Reads: 42

```
Compared to riptide motors would you say these are an upgrade?

http://www.michobby.com/product/maytech-5055-220kv-brushless-sensor-motor-for-electric-skateboardse-bike/

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html

Anyone use these before?
```

---
## \#21 Posted by: Skunk Posted at: 2018-08-13T17:53:17.192Z Reads: 39

```
[quote="Chelloo, post:18, topic:64377"]
what do you think
[/quote]

[quote="Chelloo, post:18, topic:64377"]
the breaking sucks
[/quote]

He says on his Reddit post that going to the Sanyo 10s2p fixed alot of the downsides of the board.
```

---
## \#22 Posted by: Skunk Posted at: 2018-08-13T17:57:46.546Z Reads: 38

```
Also unless you plan on changing vesc it's my understanding that you gotta keep a lower kv.
The eBay vesc they use has a limit of about 6400rpm (25ish mph) 
At 10s you'll wanna be around  170kv

(Still learning so someone correct me if I'm wrong)
```

---
## \#23 Posted by: Skunk Posted at: 2018-08-13T18:01:03.615Z Reads: 37

```
Also https://www.electric-skateboard.builders/t/maytech-mto-5055-ha-motor-2/64602
```

---
## \#24 Posted by: hyperIon1 Posted at: 2018-08-13T19:54:27.626Z Reads: 33

```
Remember that the riders weight and your gearing ratio effects this as well. A good comparison would be the motors used on the boosted board and riptide.
```

---
## \#25 Posted by: Chelloo Posted at: 2018-08-13T21:40:31.972Z Reads: 29

```
Do you still have those motors?
```

---
## \#26 Posted by: hyperIon1 Posted at: 2018-08-13T21:41:37.719Z Reads: 28

```
The orange 5055?
```

---
## \#27 Posted by: hyperIon1 Posted at: 2018-08-13T21:42:04.587Z Reads: 28

```
![IMG_7725|374x500](upload://no8TGeUPVmYJkMbkxMm0BXX1vZF.JPG)
```

---
## \#28 Posted by: Chelloo Posted at: 2018-08-13T21:51:07.364Z Reads: 26

```
Yes how would you compare them to riptide motors or boosted? Good replacement for the current motors?
```

---
