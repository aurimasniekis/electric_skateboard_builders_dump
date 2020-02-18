# Motor rolling resistance when powered off

### Replies: 55 Views: 1695

## \#1 Posted by: flywithgriff Posted at: 2017-08-29T15:24:59.240Z Reads: 180

```
I have just rode my current build and I am having what feels like increased motor drag than I'm used to. When the board is powered on or off and I turn the rear wheels manually it feels like the motors are slightly braking. I am running FOC on @Ackmaniac FW and used auto wizard on controller setup so I'm not sure it would be the beak engaging.
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-29T15:28:41.544Z Reads: 172

```
could be a shorted motor. Try unplugging all the phase leads (and make sure they're not touching) and see if it's still providing resistance.
```

---
## \#3 Posted by: darkkevind Posted at: 2017-08-29T15:28:55.442Z Reads: 166

```
Have you calibrated your controller in BLDC Tool? Could be applying a small amount of brake.
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-08-29T15:39:07.839Z Reads: 159

```
I did, I used the auto wizard.
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-08-29T15:40:10.985Z Reads: 157

```
That was my first thought but both motors are doing itvtge same amount.
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-29T15:50:39.218Z Reads: 152

```
So, both motors are slightly braking even when unplugged?
```

---
## \#7 Posted by: flywithgriff Posted at: 2017-08-29T15:53:19.388Z Reads: 145

```
Unplugged no, connected to FOCBOX and powered on or off, yes.
```

---
## \#8 Posted by: Jinra Posted at: 2017-08-29T15:54:46.643Z Reads: 138

```
huh, that's weird. I wonder if there's an internal short on the vescs..
```

---
## \#9 Posted by: flywithgriff Posted at: 2017-08-29T15:57:09.885Z Reads: 134

```
i certainly hope not!! They are brand new. @Ackmaniac could I need to manual set the controller values instead of the wizard?
```

---
## \#10 Posted by: Jinra Posted at: 2017-08-29T15:58:41.801Z Reads: 130

```
I can't imagine software has anything to do with it as it happens when your board is off as well.
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-08-29T15:59:37.084Z Reads: 128

```
You should check in bldc-tool what the ppm display shows. It should be in the area of 50%. With the deadband parameter you can adjust the sensitivity.
```

---
## \#12 Posted by: darkkevind Posted at: 2017-08-29T15:59:47.103Z Reads: 123

```
Depends what 'off' actually is :smirk:
```

---
## \#13 Posted by: flywithgriff Posted at: 2017-08-29T16:01:12.903Z Reads: 119

```
The ppm display is at 50% so I thought it would be correct. Thanks for the reply.
```

---
## \#14 Posted by: banjaxxed Posted at: 2017-08-30T21:38:56.320Z Reads: 99

```
Both rolling the same way? 😂
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-08-30T23:12:12.209Z Reads: 99

```
Are your belts insanely tight?
```

---
## \#16 Posted by: flywithgriff Posted at: 2017-08-31T00:08:08.271Z Reads: 101

```
They are insanely loose! I run idler bearings.
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-08-31T00:11:39.304Z Reads: 98

```
Ahhhhh that's not the problem then...  Maybe post a pic of the VESC so we can take a look at the solders and stuff like that?
Edit: maybe some vesc settings too
```

---
## \#18 Posted by: psychotiller Posted at: 2017-08-31T00:31:08.045Z Reads: 97

```
Could be the beginnings of a mosfet issue. It has happened to me. Where the mosfets phased out.
```

---
## \#19 Posted by: Jinra Posted at: 2017-08-31T00:32:07.402Z Reads: 94

```
both vescs though? seems unlikely itd happen to two vescs at the same time
```

---
## \#20 Posted by: psychotiller Posted at: 2017-08-31T00:36:25.791Z Reads: 94

```
True that is odd. Try switching out for one fresh vesc, use the same settings and see if its the same.

If it is, it's a setting, if it's not it's a hardware issue
```

---
## \#21 Posted by: Jinra Posted at: 2017-08-31T00:37:53.432Z Reads: 86

```
But it happens while it's off too :thinking:
```

---
## \#22 Posted by: psychotiller Posted at: 2017-08-31T00:38:53.938Z Reads: 86

```
Which leads back to the mosfets.

Motors unplugged, no phase wires touching. No resistence
Motors plugged in, resistance  

Mosfets
```

---
## \#23 Posted by: scepterr Posted at: 2017-08-31T00:39:44.133Z Reads: 86

```
Both with fet issue?
```

---
## \#24 Posted by: Eboosted Posted at: 2017-08-31T00:40:00.653Z Reads: 85

```
I had that issue 2 weeks ago, it's posted somewhere in one of my threads. 

The issue was a shorted Focbox, you can easily tell if the Focbox is bad by unplugging a single phase wire at a time, when you unplug the shorted wire from the braked motor with the battery off and the motor disengages and spin freely then your Focbox needs to be replaced.
```

---
## \#25 Posted by: scepterr Posted at: 2017-08-31T00:41:16.730Z Reads: 82

```
@Eboosted when did you get your focbox?
```

---
## \#26 Posted by: flywithgriff Posted at: 2017-08-31T00:49:29.299Z Reads: 78

```
Well that would suck! They are brand new!
```

---
## \#27 Posted by: scepterr Posted at: 2017-08-31T01:02:02.929Z Reads: 81

```
@flywithgriff when did you get yours btw?
```

---
## \#28 Posted by: Eboosted Posted at: 2017-08-31T01:05:36.409Z Reads: 83

```
Mine was also brand new, I got it 2 months ago from Kaly batch 

I wonder if the newer ones had these issues resolved. 

Not sure if I should ship it to @johnnymeduse or try to fix it myself
```

---
## \#29 Posted by: scepterr Posted at: 2017-08-31T01:17:21.283Z Reads: 84

```
I got mine direct from Enertion mid July, dead in just under 30 days
```

---
## \#30 Posted by: flywithgriff Posted at: 2017-08-31T01:19:29.061Z Reads: 86

```
I got mine in the last group buy from @yummyblobs.
```

---
## \#31 Posted by: flywithgriff Posted at: 2017-09-02T12:45:18.506Z Reads: 74

```
I have removed my tension pulleys and the resistance is considerably less. Pretty sure that was the issue.
```

---
## \#32 Posted by: psychotiller Posted at: 2017-09-02T14:44:13.933Z Reads: 74

```
Seems odd to me being that the whole point of the idler/tensioner pulley is so that you can maintain tooth contact and run your belt tension looser. When I've used them I always got that result.
```

---
## \#33 Posted by: flywithgriff Posted at: 2017-09-02T18:17:59.213Z Reads: 68

```
My belt tension is pretty loose. Not sure why it's happening. All I know is when I removed the tensioner the resistance decreases.
```

---
## \#34 Posted by: Jinra Posted at: 2017-09-02T19:28:43.776Z Reads: 63

```
did you check the rolling resistance of the idler itself? Perhaps the bearing needs a cleaning
```

---
## \#35 Posted by: psychotiller Posted at: 2017-09-02T20:29:11.007Z Reads: 59

```
does the tensioner bend or pinch the belt? maybe too close to one of the pulleys?
```

---
## \#36 Posted by: Martinsp Posted at: 2017-09-02T20:30:32.318Z Reads: 62

```
Why not try to eliminate the whole wheel belt situation by removing the motor or popping off the belt and trying to test the motor without any load on it? That is what I would do anyway.. :D
```

---
## \#37 Posted by: flywithgriff Posted at: 2017-09-02T20:33:03.762Z Reads: 63

```
@Jinra they are new bearings and nice and clean.

@psychotiller the idler may be to close to the motor pulley. That's the only place they would fit but do disrupt the path of the belt about 15mm.

@Martinsp I have already ruled out motor and FOCBOX issues.
```

---
## \#38 Posted by: Martinsp Posted at: 2017-09-02T20:36:04.700Z Reads: 65

```
Oh sorry, overlooked that probably.

It looks like the bearings then.. check wheels without load on them like the belt etc.
```

---
## \#39 Posted by: Jinra Posted at: 2017-09-02T21:09:23.672Z Reads: 63

```
you put the idler on the slack side right? not tension side
```

---
## \#40 Posted by: psychotiller Posted at: 2017-09-02T21:16:52.992Z Reads: 67

```
[quote="flywithgriff, post:37, topic:31747"]
the idler may be to close to the motor pulley. That's the only place they would fit but do disrupt the path of the belt about 15mm.
[/quote]

Have a picture with the idler on?
```

---
## \#41 Posted by: flywithgriff Posted at: 2017-09-02T21:36:04.010Z Reads: 67

```
 These aren't the best pics put it's all I have right now. The idler is on the side in which the belt is pushed by the Idler pulley, not pulled.
<img src="/uploads/db1493/original/3X/a/6/a6ca57c75cfd39a90d33bdd285217086f7f44bf9.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/3/93d2a847982010da1655a3790e6d65d3f3d8427b.JPG" width="500" height="500">
```

---
## \#42 Posted by: scepterr Posted at: 2017-09-03T00:03:25.097Z Reads: 61

```
Anybody trying these as idler bearings?
<img src="/uploads/db1493/original/3X/b/b/bb309eb321761b8bc996e8204075888f4b81e61b.jpg" width="480" height="500">
```

---
## \#43 Posted by: Cobber Posted at: 2017-09-03T01:04:28.036Z Reads: 60

```
It is hard to tell from the angle of your pictures Griff, Looks like we are talking about your mountain board w/ the motors mounted behind the rear axel?

If that is the case the jockey wheel or idler bearing should be on the upper/sky side of the mount. Is that how you have it? :neutral_face:
Is the first pic upside down?
```

---
## \#44 Posted by: scepterr Posted at: 2017-09-03T01:06:57.891Z Reads: 59

```
Going by the coke bottle in the background it's right side up so idler is ground facing :hushed:
Also upward trajectory of splashes on mount in second pic indicate orientation :spy:
```

---
## \#45 Posted by: flywithgriff Posted at: 2017-09-03T01:58:41.118Z Reads: 59

```
haha I agree the pictures are tough to make out. They are indeed on the upward side.

@scepterr These look like a nice solution.
```

---
## \#46 Posted by: scepterr Posted at: 2017-09-03T02:18:52.632Z Reads: 55

```
@flywithgriff Are you laying under the board while taking the pics? Lol
```

---
## \#47 Posted by: flywithgriff Posted at: 2017-09-03T02:28:22.658Z Reads: 54

```
Lol it's an elegant dance between machine and human! The board is actually standing on its end and leaning against my desk.
```

---
## \#48 Posted by: JLabs Posted at: 2017-09-03T02:31:54.700Z Reads: 55

```
They are linear bearings for 3d printers meant to move back and forth on a shaft, not spin around, so in this case it would not work for an islet Pulley.
```

---
## \#49 Posted by: Cobber Posted at: 2017-09-03T02:38:01.035Z Reads: 53

```
They also look a bit small even if they would work don't you think @JLabs?
```

---
## \#50 Posted by: scepterr Posted at: 2017-09-03T02:45:28.777Z Reads: 55

```
@JLabs  Oh that sucks, totally overlooked them being linear lol, the dimensions caught my eye
@Cobber it's 8mm bore, 15mm OD, 24mm width
```

---
## \#51 Posted by: Cobber Posted at: 2017-09-03T02:53:52.960Z Reads: 53

```
15mm is pretty small, it will increase belt wear/ resistance... :frowning:
It is just due to the angle the belt is bent around the roller.

_bigger roller = less angle_
```

---
## \#52 Posted by: flywithgriff Posted at: 2017-09-03T02:56:07.480Z Reads: 52

```
I don't believe any one is wrapping the belt at an extreme distance with an idler. I don't see the few mm out of line these bearings are to cause a drastic reaction.
```

---
## \#53 Posted by: Cobber Posted at: 2017-09-03T03:27:23.016Z Reads: 54

```
Read up on some engineering sites Griff, I'm also not the first to mention it. It has also been mentioned in the _I love idlers_ thread...
It is not a will it work, or won't it work thing. But it will play in to long term reliability and the efficiency of the system. That said in a industrial setting _0%_ failure is often the object. With DIY most are not so demanding the odd failure is accepted and reduced life span is often the norm.
```

---
## \#54 Posted by: JLabs Posted at: 2017-09-03T15:13:19.072Z Reads: 46

```
What would you say is the ideal distance from both pulleys to the idler? 20-25mm on each side??
```

---
## \#55 Posted by: flywithgriff Posted at: 2017-09-03T18:13:05.383Z Reads: 42

```
I am very familiar with the principals of engineering and the effects of a fixed location of stress applied to the belts by the idler. My reply was referring to the fact that we only use about 15% of the bearings circumference. If the belts were wrapping around the idlers and contacting 50% or more of the circumstance then I agree the stress applied to the belts in a small area would cause much more concern.
```

---
