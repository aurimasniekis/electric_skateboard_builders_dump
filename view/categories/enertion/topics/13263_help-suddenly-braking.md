# HELP! Suddenly braking!

### Replies: 22 Views: 2263

## \#1 Posted by: SeanHacker Posted at: 2016-11-18T05:29:35.690Z Reads: 144

```
Alright guys. This is my first topic ever so go easy on my. I've been working with my Enertion Raptor for 3 weeks now and never had an issue until now. 

For some reason it wants to brake on its own. It's actually kinda scary because I will be going forward and it will want to brake all of the sudden in short bursts. Does anyone have any clue as to what's going on here. Let me know what kinda info you guys need and I will provide it. Thanks ahead of time!

https://youtu.be/APESk-VAIhA
```

---
## \#2 Posted by: SeanHacker Posted at: 2016-11-18T05:30:46.092Z Reads: 141

```
@onloop any idea? @chaka @barajabali @longhairedboy ??? Sorry for bothering you guys, but I know you all know e-boards.
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-18T05:31:45.325Z Reads: 137

```
plug it into BLDC tool and check your throttle and deadband. My guess is that your neutral position is closer to the braking threshold so it's kind of in a "almost braking" position. If that is the problem, you can increase deadband or adjust your min/max pulsewidth to fix it.
```

---
## \#4 Posted by: SeanHacker Posted at: 2016-11-18T05:32:45.292Z Reads: 135

```
Thanks for the super fast response. i did that already, but I'm going to do it again just to be sure.
```

---
## \#5 Posted by: onloop Posted at: 2016-11-18T05:32:51.103Z Reads: 134

```
Check all the connections, make sure no loose wires or anything obvious like a shorted phase wire.
```

---
## \#6 Posted by: SeanHacker Posted at: 2016-11-18T05:35:51.230Z Reads: 131

```
@onloop Thanks. I'll check. One thing I noticed earlier today is that my right hand motor was making a chirp almost like a bird on a 6 mile ride I did earlier. Do you think I might be having a motor issue?
```

---
## \#7 Posted by: SeanHacker Posted at: 2016-11-18T06:07:03.479Z Reads: 127

```
All the connections to everything looks good. BLDC looks good as far as I know. Not only is it braking, it's jolting forward also at times. Fuck. i love this board. It feels like my kid a deathly ill or something. :frowning:
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-11-18T06:22:27.034Z Reads: 120

```
Is it braking when you release the trigger ?
```

---
## \#9 Posted by: SeanHacker Posted at: 2016-11-18T06:26:15.854Z Reads: 118

```
it's neither. It will start braking and speeding up without any type of remote control. Both in short burst.
```

---
## \#10 Posted by: SeanHacker Posted at: 2016-11-18T06:43:59.647Z Reads: 116

```
Found it!!! One of the remote wires to the vesc came loose. Barely though. I mean it was maybe a mm out of place. Just did another test run and after hitting it with hot glue it works just fine again. Or at least I hope. Going to take it on a long night ride right now to make sure. :)

P.S- I'm about to go on a long ride tonight. I'll post here when I'm done.
```

---
## \#11 Posted by: Rob.Endless Posted at: 2016-11-18T07:19:42.602Z Reads: 115

```
I took the lid off my GT and hot glued every connection I can find lol. Even plugs such as the motor plugs (they are not three separate plugs, instead they are fitted into one plug) which takes a hell of a lot of force to pull apart, I hot glued.

I'm glad you found the problem, sucks falling off at 20+mph.
```

---
## \#12 Posted by: Pimousse Posted at: 2016-11-18T07:28:37.799Z Reads: 115

```
Give a try to @Ackmaniac firmware to precisely set the neutral of the remote.
I always have lot of pain setting propreperly the remote with the official VESC firmware.
With Acmaniac one, now, it's very easy and reliable.
```

---
## \#13 Posted by: SeanHacker Posted at: 2016-11-18T07:53:12.772Z Reads: 113

```
I already use that firmware and version of BLCD. Its the shit! Everything is working as usual now after gluing the remote wires.
```

---
## \#14 Posted by: Pimousse Posted at: 2016-11-18T07:56:06.892Z Reads: 112

```
Oh sorry, I missed your post.

Why do you say Acmaniac firmware is a shit ?
Do you have trouble with it ?
```

---
## \#15 Posted by: SeanHacker Posted at: 2016-11-18T07:58:11.587Z Reads: 108

```
Lol. I didn't say its shit. I said it's the shit. Like it the best thing ever when it comes to programming my vesc's.
```

---
## \#16 Posted by: Ackmaniac Posted at: 2016-11-18T11:48:39.995Z Reads: 96

```
Happy to hear that it helped solving your issues. Did you only use it to adjust the center position or did you also test the watt control mode.
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2016-11-18T14:53:32.552Z Reads: 88

```
[quote="SeanHacker, post:10, topic:13263"]
Found it!!!
[/quote]


Nice work... now go out and have some fun :stuck_out_tongue_winking_eye:
```

---
## \#19 Posted by: mikey Posted at: 2016-11-18T15:20:33.020Z Reads: 84

```
[quote="Pimousse, post:12, topic:13263, full:true"]
Give a try to @Ackmaniac firmware to precisely set the neutral of the remote.I always have lot of pain setting propreperly the remote with the official VESC firmware.With Acmaniac one, now, it's very easy and reliable.
[/quote]

What's this Acmaniac firmware? Is it only for Enertion raptors? Or does it relate to VESCs in general? Link please.
```

---
## \#20 Posted by: Pimousse Posted at: 2016-11-18T15:28:25.865Z Reads: 82

```
It works with every HW 4.10+ VESC

See his thread :
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-11-18T15:34:33.982Z Reads: 78

```
this is why some of us have started soldering the remote leads instead of using the usual servo connectors.
```

---
## \#22 Posted by: SeanHacker Posted at: 2016-11-18T23:27:39.565Z Reads: 62

```
I just need to learn how to solder. Then I'm going to do that. :slight_smile:
```

---
## \#23 Posted by: SeanHacker Posted at: 2016-11-18T23:28:34.522Z Reads: 61

```
I used it to adjust center position and for wattage control. I love it!!!
```

---
