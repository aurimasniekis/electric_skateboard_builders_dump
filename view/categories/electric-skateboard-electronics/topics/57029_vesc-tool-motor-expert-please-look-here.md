# VESC-tool / Motor expert please look here

### Replies: 43 Views: 1505

## \#1 Posted by: DK-Odense Posted at: 2018-05-28T13:47:21.784Z Reads: 191

```
Hi Guys

My APS 8072S setup acts strange - At a certain level of RPM the magnetic rotor starts to vibrate.
This is both happening when going up in speed, and when throttle is totally released and the rpm just decreases naturally.

When the vibration kicks in, the power decrease until you get above the vibration point.
It happens to both motor and they are new, so i doubt the problem is in the motors (unless APS deliver bad motors?).

I made two videos of the problem here.

Overview:
https://youtu.be/he0yy7EHB40

Near:
https://youtu.be/f-diUOkPGPE

Setup is VESC6, APS 8072S, 12S LI-PO turnigy graphene.

Hope you are able to help me out.
```

---
## \#2 Posted by: PXSS Posted at: 2018-05-28T13:49:38.130Z Reads: 174

```
The videos don't work. Please also upload pictures of your settings.

Did you do a motor detection properly and write the values? That would be my first thing to check.
```

---
## \#3 Posted by: DK-Odense Posted at: 2018-05-28T13:52:34.594Z Reads: 168

```
Yep - Motordetection done by wizard.

Did a lot of different setups with wizzard motordetection. Normally i have no problems.
```

---
## \#4 Posted by: Scoo_B_SK8 Posted at: 2018-05-28T13:56:37.388Z Reads: 164

```
I’d dbl check your belt tension, might be pulled to tight and why the housing is out of alignment and is why your able to pull through it at higher revs cause it stretches out
```

---
## \#5 Posted by: PXSS Posted at: 2018-05-28T13:56:44.301Z Reads: 164

```
Videos work now. 
That is indeed very odd!
You're not hitting anything and are your mounts solid? Is it only the can vibrating or the whole thing including mounts?
```

---
## \#6 Posted by: PXSS Posted at: 2018-05-28T13:57:51.874Z Reads: 162

```
It's a gear drive. But that's a good point, vibrations could be coming from the gears.
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2018-05-28T14:00:56.559Z Reads: 154

```
Do the motors act the same under no load?

[quote="PXSS, post:6, topic:57029"]
It’s a gear drive.
[/quote]
😣 just started typing away, usually only seen issue with belt drives.
```

---
## \#8 Posted by: linsus Posted at: 2018-05-28T14:03:09.745Z Reads: 153

```
Could you specify what part of the video you think is strange? 
Is it the exact same behaviour under load? Or didint you ride the board yet? 
What battery are you using?
What limits are set in VESC?
```

---
## \#9 Posted by: DK-Odense Posted at: 2018-05-28T14:37:58.720Z Reads: 149

```
This is with No load. Motors are spinning free in the videos, but on road with gears IT is exactly the same, just Louder.

Brackets are rock solid and had no vibration. IT is only the rotor part that vibrates.

Setup is 12s lipo, vesc6 and 8972s
```

---
## \#10 Posted by: DK-Odense Posted at: 2018-05-28T14:40:06.870Z Reads: 149

```
Turn Up volume, and you Will not have any doubt about which part of the video is wrong :slight_smile:

In the near video you are able to see the rotor "flexing" at a cetain rpm level ☹️
```

---
## \#11 Posted by: linsus Posted at: 2018-05-28T14:43:09.760Z Reads: 138

```
I asked if the behaviour was the same under load. The vid is obv. zeroload. The mechanical resonance RPM maybe sounds and feels scary, but its quite normal. Did u ever look at a washing machine spinning up? At a specific RPM it looks like its gonna take off, then it just settles down.
```

---
## \#12 Posted by: DK-Odense Posted at: 2018-05-28T15:09:32.742Z Reads: 141

```
Exactly the same under load. Powerloss and a terrible Sound ☹️
```

---
## \#13 Posted by: linsus Posted at: 2018-05-28T15:15:14.177Z Reads: 136

```
Alright then, back to the remaining questions, what are your VESC settings and what are you supplying the motors with?
```

---
## \#14 Posted by: DK-Odense Posted at: 2018-05-28T15:23:59.011Z Reads: 132

```
For the third time 12s lipo 6000mah graphene 😁😁😁

Vesc settings is standard. Which do you want, then i can a screendumb 👍🏻
```

---
## \#15 Posted by: evoheyax Posted at: 2018-05-28T15:45:02.196Z Reads: 132

```
It could be the motors cans are imbalanced. If you've taken a motor a part, sometimes you'll see some little blue dots of putty inside the magnets spaces. These are used to balance the motor, along with vibration detection tools to figure out where the imbalance is. The higher the speed, the worse the imbalance gets because the centripetal forces are higher at higher speeds.

Can't say if this is your case, I would double and triple check all software/hardward first before jumping to this possibility. But I have strong feeling this might be your problem.
```

---
## \#16 Posted by: Deckoz Posted at: 2018-05-28T15:53:21.275Z Reads: 130

```
@DK-Odense rerun motor detection with a higher duty cycle. :slight_smile:

That sound is from a bad detection. And the controller having bad math trying to properly read  motor position. The noise is two magnetic flux linkages crossing causing the can to harmonize. 

A redectection with higher duty cycle will help, or running sensored should eliminate this(hybrid doesn't count)
```

---
## \#17 Posted by: DK-Odense Posted at: 2018-05-28T20:12:19.327Z Reads: 123

```
Hi Deckoz

I have now tried with different duty cycle settings in the detection part, going from 0,3 to 0,9 without any results.
I tried with both motors, and the problem is the same :frowning:

 https://youtu.be/LFQSmIPuAU8 

Is it possible that motor wizzard just dont work on these motors?
```

---
## \#18 Posted by: Deckoz Posted at: 2018-05-28T20:21:21.754Z Reads: 114

```
It could be possible @DK-Odense 

Try resting to a defaults config. Avoid the motor wizard. And go to the bldc tab and run a detection manually with .05  .10 or 0.15
```

---
## \#19 Posted by: Sebike Posted at: 2018-05-28T20:44:38.351Z Reads: 113

```
This exact thing happened to me with my 6374 motor last year. (There should be an old thread on this as well.) 

I opened up the motor and it looked as if some of the magnets were slightly touching the stator, as there were very light marks on the magnets.

I couldn't see why this was happening at the time, so I kept riding the board. After a while though the noise kept getting worse and changed, and eventually the motor broke down totally and it turned out that some magnets had come loose, ie I could move the with a screw driver as the glue had let go.

I got the can replaced with a new one, which solved the issue.
```

---
## \#20 Posted by: Sebike Posted at: 2018-05-28T20:55:02.139Z Reads: 122

```
Here's my old thread

http://www.electric-skateboard.builders/t/motor-making-knocking-ticking-sounds-at-low-speed/33700

If you search for "screeching motor" you'll find a couple of others that had the same issue with this  noise at a certain rpm that was due to magnets coming loose.
```

---
## \#21 Posted by: Deodand Posted at: 2018-05-28T22:28:39.169Z Reads: 113

```
I'm assuming you are using FOC since you have vesc 6? screen dump after you run R/L/ flux linkage calibration. What is motor kV supposed to be? We could take a look at flux linkage measurement and compare it to your motor kV. If this value is wrong it could cause estimator to track poorly. 

A screen recording of the realtime data screens while this phenomenon happens could also help.  FOC tab might be most useful to see how FOC currents are tracking. 

I might also suggest tuning the current controller time constant of your motor controller. I think by default it is 1000 us, try something like 2000-3000 us for less aggressive current controller gains.

Try BLDC also... if same phenomenon happens in FOC and BLDC, it is probably a mechanical issue with the motor.
```

---
## \#22 Posted by: aethyr Posted at: 2018-05-28T22:39:17.582Z Reads: 113

```
Does this happen in a single motor configuration with each motor? How about without the gears attached, just bare motor?

Also what others said, about trying it in BLDC mode, but try without sensors (is it sensored?). The idea is to see if the vibration happens with these different methods to rule out ESC issue.

Although it seems highly improbable that both motors have the same mechanical issue.
```

---
## \#23 Posted by: Sebike Posted at: 2018-05-28T22:53:31.078Z Reads: 110

```
Oops,, I actually didn't read the part where you say you had this issue with both motors.

So you did actually spin up the motors -one at a time- and both motors make this noise?

Did you hear this from the very beginning or is this something that has appeared after a while with this setup?
```

---
## \#24 Posted by: DK-Odense Posted at: 2018-05-31T12:13:25.970Z Reads: 97

```
Hi Guys

I tried in BLDC mode - No difference.

That let me to the conclusion that it must be an mechanical balancing fault. 
I tried balancing with different object just to try if it made any difference at all - No diffenrence :frowning:

https://image.ibb.co/nEuLHd/IMG_20180531_125547.jpg

Back to VESC6 Settings - Autodetect settings ends up like this:

https://image.ibb.co/cAjLHd/Udklip.png

The motor is this one: http://alienpowersystem.com/shop/brushless-motors/aps8072s-sensored-bldc-motor-165kv-6000w/

RPM Video of the problem (Motor goes up to certain RPM level and then vibrates even harder if i turn up the trottle, until it "breaks through" and gets above the vibration RPM zone: https://youtu.be/6_BeUVZet9A

FOC video of the problem: https://youtu.be/DCSm_yTTXGU

Current video: https://www.youtube.com/watch?v=TmRTynFcgBQ&feature=youtu.be

I´m lost guys - Help med out here :slight_smile:
 
And again, motor is running free with no gears attached.
VESC6, LIPO 12S
```

---
## \#25 Posted by: aethyr Posted at: 2018-05-31T17:00:15.754Z Reads: 84

```
Did you try running in unsensored mode as I suggested earlier?
```

---
## \#26 Posted by: DK-Odense Posted at: 2018-05-31T17:54:15.700Z Reads: 84

```
Yep - foc, bldc, sensored, unsensored e.g.... ☹️
```

---
## \#27 Posted by: Sebike Posted at: 2018-05-31T18:01:01.907Z Reads: 82

```
Open up the motors and check for loose magnets or sign of magnets touching the stator.
```

---
## \#28 Posted by: Deckoz Posted at: 2018-05-31T18:06:51.927Z Reads: 84

```
I think I see metal shrapnel and likely an incompletely glued magnet

![Screenshot_20180531-140523|281x500](upload://cNN5arWIaj6swRLwQO8sTg3kY58.jpg)
```

---
## \#29 Posted by: DK-Odense Posted at: 2018-05-31T18:25:26.678Z Reads: 78

```
I know 🙂  I also thought that was the problem, so i took all magnets out today and 3d printet a guide for the other end (they are only guide at one side originally) and re-fixed all magnets totally aligned... And tada!!! No changes at all ☹️
```

---
## \#30 Posted by: Deckoz Posted at: 2018-05-31T18:30:45.661Z Reads: 76

```
What did you use to repot the magnets?
```

---
## \#31 Posted by: Sebike Posted at: 2018-05-31T20:28:04.860Z Reads: 71

```
:rofl::rofl::rofl::joy::joy::joy::sweat_smile::sweat_smile::sweat_smile:
time for another oops. oh, so you did open up the motors already lol.

you have to excuse me.. been sitting for 7 hours straight doing our final big exam. brain is messed up.
```

---
## \#32 Posted by: aethyr Posted at: 2018-05-31T21:20:58.612Z Reads: 70

```
Both motors are doing this at the exact same rpm range, with different vesc? 

It seems highly unlikely that 2 motors would have the same exact mechanical defect and that both vesc would have same issue. So at this point perhaps they are incompatible :frowning:
```

---
## \#33 Posted by: Deodand Posted at: 2018-06-01T00:05:12.983Z Reads: 69

```
I would say if bldc and foc both produce this resonance, it is probably a poorly designed motor? At some speeds motors can have mechanical resonance but ultimatley should be designed with resonance peaks far from the operating range.
```

---
## \#34 Posted by: aethyr Posted at: 2018-06-01T00:08:00.985Z Reads: 68

```
Yeah I would send Bruno the vids of both motors exhibiting the problem and send them back.
```

---
## \#35 Posted by: Ackmaniac Posted at: 2018-06-01T00:34:09.631Z Reads: 67

```
Just try each motor without the other. Maybe you have traction control enabled.
```

---
## \#36 Posted by: b264 Posted at: 2018-06-01T00:38:39.816Z Reads: 65

```
Also try the motors on a different ESC or the ESC on a different motor
```

---
## \#37 Posted by: Silverline Posted at: 2018-06-13T19:28:46.843Z Reads: 64

```
Have the same problem with the same motor, together with Escape vesc.....

To me it's sounds like a motor timing issue, could it help to change the Hz.... That is possible in @Ackmaniac firmware ?
```

---
## \#38 Posted by: banjaxxed Posted at: 2018-06-15T00:25:35.692Z Reads: 59

```
This is a badass setup, what are we talking about? 16hp? 

Feeling inadequate with 6374 here 🐌
```

---
## \#39 Posted by: Silverline Posted at: 2018-06-15T04:46:53.109Z Reads: 53

```
Yes it is...

But not cool, when it sounds like this :-/
https://youtu.be/yxok02O2vSM
```

---
## \#40 Posted by: chocol4te Posted at: 2018-07-17T14:49:19.650Z Reads: 39

```
I am having the exact same issue with my 8072S (~65% RPM on a 12s). Did you ever find a solution?
```

---
## \#41 Posted by: Silverline Posted at: 2018-07-17T14:55:31.828Z Reads: 34

```
Yes... The solution for me and @DK-Odense was to send the motors back for a refound... The motors have design flaws, wich can't be fixed. Why Bruno sells these motors still, i dont understand.
```

---
## \#42 Posted by: chocol4te Posted at: 2018-07-17T15:02:24.531Z Reads: 34

```
Damn, I tested it on a 4s I had lying around and it worked so I went ahead and soldered a new sensor lead as well replacing the motor leads with stranded silicone ones. I doubt he'll give me a refund :/
```

---
## \#43 Posted by: Silverline Posted at: 2018-07-17T15:09:25.202Z Reads: 32

```
He is Selling "defective" motors.... So he should. 

I had crimpt 6p connectors on for vesc 6, and cut the motor wires to the length, and soldered on bullets, i told him these thing in the mail, and he offered a refound. I think he is on holyday right now, but i sure hope he is holding his word.
```

---
