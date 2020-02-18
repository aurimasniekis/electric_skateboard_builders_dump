# Separate battery power supplies for two VESCs

### Replies: 16 Views: 487

## \#1 Posted by: janpom Posted at: 2018-07-16T08:03:13.176Z Reads: 170

```
I was just wondering if there's a major problem with running two VESCs each with its own battery pack. The only issue I can think of is that the battery on one can run out earlier than on the other one.

Why I'm asking. I'm currently running single drive with 4x 3S LIPOs. I'm considering my upgrade options for dual drive and extended range. One idea is getting two more 3S LIPOs and change the current 12s1p to 9s2p. Using one 9s1p for each motor would then make wiring easier than doing 9s2p that's wired to both motors. Any thoughts on that?

BTW, I have XT150 and AS150 connectors on my batteries and I take the battery pack apart for charging anyway, so that's not an issue.

Here's a pic of how things are currently wired up:
![DSC01443|690x460](upload://iSJBZGAu0apKfpXJHFCqqUcIq2P.jpg)

Yeah, I use cardboard for my battery "enclosure". :slight_smile: Has been working fine so far.
```

---
## \#2 Posted by: BensonYong Posted at: 2018-07-16T09:23:00.639Z Reads: 148

```
If the main V6 (esc connected to the receiver) is not powered, the remote will not be able to control the ESK8.Even batteries of the same specification may have different discharges during use, It may cause the motor to be out of sync and affect the riding experience.
```

---
## \#3 Posted by: janpom Posted at: 2018-07-17T20:49:22.708Z Reads: 126

```
@BensonYong Thanks for chiming in. I'm not too worried about the master VESC getting powered off. The point about different discharge rate is an interesting one, though. I thought the VESCs would keep the motors in sync. That's the reason they communicate to each other, no?
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-07-17T23:03:17.442Z Reads: 118

```
Why would you not just connect them in parallel? Use a splitter cable. If you're using two vesc's you should put them in a master / slave config using a can bus cable. If that cable is connected and one vesc is on and the other is off it tends to fry things.

Tldr; use a splitter cable and keep your batteries in parallel.
```

---
## \#5 Posted by: JdogAwesome Posted at: 2018-07-17T23:43:04.505Z Reads: 109

```
Yeah I see no benefit in doing this, only potential problems lol. Also why are you using XT150 connectors, those things are huge! Use XT60's and if you really wanna be overkill use XT90's even tho XT60's are plenty for almost any board.
```

---
## \#6 Posted by: b264 Posted at: 2018-07-18T01:32:35.853Z Reads: 92

```
You could make two completely independent drivetrains (with zero wires between them) if you use a remote capable of using two receivers, like the Mini Remote.  Plus, added confidence that a failure will not leave you with no brakes or unable to get home easily.
```

---
## \#7 Posted by: Cobber Posted at: 2018-07-18T01:41:42.655Z Reads: 87

```
I've got a build now that will have 2 x separate battery/esc systems. MoeStooge does his raceboard that way as well.
```

---
## \#8 Posted by: janpom Posted at: 2018-07-18T08:20:43.400Z Reads: 76

```
Thanks everyone for your input.

[quote="TowerCrisis, post:4, topic:61986"]
Why would you not just connect them in parallel?
[/quote]

Just to have less wiring. No other reason. This may very well not justify the potential problems.

[quote="JdogAwesome, post:5, topic:61986"]
Yeah I see no benefit in doing this, only potential problems lol. Also why are you using XT150 connectors, those things are huge! Use XT60’s
[/quote]

I use XT150 because they make it easy to wire up the batteries in series. XT60 is a dual cable connector. It's a different thing. It's not about how much amps I can get through. XT150 works for me.

[quote="b264, post:6, topic:61986"]
You could make two completely independent drivetrains (with zero wires between them) if you use a remote capable of using two receivers, like the Mini Remote.
[/quote]

Interesting. Don't the motors get out of sync then though?

I assumed that with two interconnected VESCs the motors would be kept in sync. Am I wrong thinking that and the VESCs don't really worry about synchronization? Does the master VESC merely forward the remote controller input to the slave VESC?

[quote="Cobber, post:7, topic:61986"]
I’ve got a build now that will have 2 x separate battery/esc systems.
[/quote]

Cool! Good to know. May I ask why? Are there advantages apart from simpler wiring? The redundance (increased reliability) @b264 mentioned?
```

---
## \#9 Posted by: b264 Posted at: 2018-07-18T08:42:09.942Z Reads: 68

```
[quote="janpom, post:8, topic:61986"]
Interesting. Don’t the motors get out of sync then though?

I assumed that with two interconnected VESCs the motors would be kept in sync. Am I wrong thinking that and the VESCs don’t really worry about synchronization? Does the master VESC merely forward the remote controller input to the slave VESC?
[/quote]

Yes, the motors will always be out-of-sync, or you could just use one controller.  The thing being controlled is the amount of power applied to the motor -- the actual voltages applied depend on rotor position fed through some complex formulas and will be different for each motor.  So with two remote receivers, the amount of power being requested is still the same.  It will be implmented with different signals to the same end result.  But if you have a failure, one whole drivetrain would still work, brakes and all.
```

---
## \#10 Posted by: Cobber Posted at: 2018-07-18T11:47:36.383Z Reads: 60

```
like b246 said:

[quote="b264, post:9, topic:61986"]
...if you have a failure, one whole drivetrain would still work...
[/quote]

Brakes are important, but you also blow both speed controllers and the brakes can lock  :open_mouth:

@MoeStooge have you got that video, I think it was spd1 when you were doing a speed test and blew your esc and streeted face?
```

---
## \#11 Posted by: MoeStooge Posted at: 2018-07-18T12:20:34.293Z Reads: 57

```
[quote="Cobber, post:10, topic:61986"]
streeted face?
[/quote]

I burned down a motor(47mph run) in the V1 raceboard that backfed the other esc through the 5v reference tied  through the receiver wires that we're paralleled blowing both circuit boards (no crash). On the street face (Artie's board 50m drag race run) It was volt sag ( 10c 10ah on 200a demand) low voltage esc reset. Nothing burned down on That run cept some pride. The only thing connecting my esc's now is the power source, paralleling esc 
radio side is a big mistake.  https://youtu.be/jQcbA5fYCws
```

---
## \#12 Posted by: Pablo_702 Posted at: 2019-05-03T16:15:19.257Z Reads: 33

```
Hey man i saw your video and i dont want to be that guy, currently in the sketch process of a TBDD 2wd possibly 4wd, and your post caught my eyes, could you elaborate on this, i been off the forum for more than 2 years now and when i left things were different, a diagonal build was the sickest thing out there, no hubs nor dd and ppl were happy with 30mph 🤣🤣🤣🤣
```

---
## \#13 Posted by: janpom Posted at: 2019-05-03T20:43:00.945Z Reads: 25

```
Wrong thread?
```

---
## \#14 Posted by: Pablo_702 Posted at: 2019-05-04T01:35:52.142Z Reads: 20

```
Forgot to tag him sorry and thank you @MoeStooge
```

---
## \#15 Posted by: Andy87 Posted at: 2019-05-04T02:03:14.036Z Reads: 18

```
Moe has some threads about his racing stuff as well as the racer room thread. I think that would be a better place to ask your question @Pablo_702
```

---
## \#16 Posted by: Pablo_702 Posted at: 2019-05-04T02:16:13.299Z Reads: 19

```
Thanks for the advice, will check it out
```

---
