# FOC&rsquo;ing around (weak brakes and cutout)

### Replies: 117 Views: 4253

## \#1 Posted by: Jinra Posted at: 2017-09-15T15:11:25.324Z Reads: 365

```
Hey all,

With the release of vesc tool and 3.28 I decided to try FOC. setup was a bit buggy as i got failed detections and the "r is 0" bug, but i was eventually able to get everything setup. I copied my current limits from bldc on 2.18, but had a couple issues in my first ride. Here's my setup...

10s4p Samsung 25R
Each VESC (dual Ollin 4.12 setup):
motor max: 70
motor min: -70
battery max: 40
battery min: -8
FOC sensored

The problem:

1. The brakes are noticeably weaker than bldc while startup is about the same strength. There is a slight delay when accelerating and braking as well but i chalked this up to FOC limitations. I've already decreased ramp up time to .1s

2. When i blast the throttle from standstill (unloaded) or quickly speed up going uphill (or I assume anytime I'm drawing a lot of current), The Vescs cutout and the wheels stop spinning until i let go and throttle again. The behavior is as if I'm getting over current, which i may very well be, but not sure why this happens in FOC and not BLDC. Haven't checked error codes yet, but I'm assuming over current, will update later.

The board otherwise works fine with smooth startup and no issues running at 50k erpm. Any input is appreciated!
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-09-15T15:41:29.649Z Reads: 321

```
FOC is sensitive to sudden acceleration, mine cuts out at 0-100% throttle momentarily, It some times lose pole detection, also momentary, but sensored shouldn't do that
but if its over current u can increase absolute max up to 150a safely, though I only goes 140a.
accelerating ramping u can just kill it with 0s, but I saw people complaining even after that. I haven't try so..
```

---
## \#3 Posted by: Jinra Posted at: 2017-09-15T15:44:13.872Z Reads: 317

```
Sensored shouldn't have much to do with it given that it moves over to sensorless at about 3mph (7000eRPM). If I am getting over current faults I'll check tonight to see how much current I'm drawing.

If the full throttle cutouts are something i "just have to live with" then I'll probably switch back to BLDC.

I will miss the quietness and battery efficency though, I ended up with like 4-5% more battery at the end of my 3.7 mile ride.
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-09-15T15:52:46.350Z Reads: 302

```
Strangely my case was opposite to you XD
I had over current in BLDC in braking and Switched to FOC,
Efficiency only noticeable over 10miles I think, I get 3 miles more over BLDC
```

---
## \#5 Posted by: chinzw Posted at: 2017-09-15T17:05:54.939Z Reads: 290

```
I have similar issue, but only cuts out when braking. Even if i brake and try to push the board with my feet, the vesc resets.
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-15T17:25:48.057Z Reads: 272

```
Getting abs over current fault?
```

---
## \#7 Posted by: Jinra Posted at: 2017-09-15T17:26:48.962Z Reads: 263

```
Will check when I get home :) If I am, any ideas what might be causing it?
```

---
## \#8 Posted by: scepterr Posted at: 2017-09-15T17:39:15.510Z Reads: 263

```
Honestly I've encountered that on every vesc, about 6 diff ones now. I can't pin down the problem. I replaced everything from the fets, the shunts and caps, resistors and the issue always shows up again
```

---
## \#9 Posted by: Jinra Posted at: 2017-09-15T17:40:59.443Z Reads: 258

```
Have you tried the FOCBOX? When we were blasting the throttle at the Raptor 2 event, it didn't seem to fault.
```

---
## \#10 Posted by: scepterr Posted at: 2017-09-15T17:41:45.102Z Reads: 255

```
Focbox on raptor is supposedly running some tweaked firmware. And yah happened on focbox too
```

---
## \#11 Posted by: Jinra Posted at: 2017-09-15T17:42:30.665Z Reads: 250

```
When you get OC faults, what's the current reported for you?
```

---
## \#12 Posted by: scepterr Posted at: 2017-09-15T17:43:07.872Z Reads: 251

```
Over 130 filtered, actual is normal
I have 4inches between batt and vesc, I've tried everything imaginable lol
```

---
## \#13 Posted by: Jinra Posted at: 2017-09-15T17:43:37.618Z Reads: 242

```
if it's about 130A then we should be able to just set the abs max higher and it should be fine right?
```

---
## \#14 Posted by: Sebike Posted at: 2017-09-15T17:44:30.104Z Reads: 238

```
If battery is full, focbox with bms does give brake cut outs at the beginning of the ride - fault code over voltage
```

---
## \#15 Posted by: scepterr Posted at: 2017-09-15T17:44:52.403Z Reads: 237

```
Probably, I actually looked for that yesterday but I don't think the extended bldc tool has that option...
Also it might fix the error but not the cause
```

---
## \#16 Posted by: Jinra Posted at: 2017-09-15T17:46:08.890Z Reads: 243

```
Sure it does, it's Absolute Max in the currents tab

@Sebike easily fixable by increasing max input voltage, not sure why Enertion would mess with this setting though.

@scepterr Here it is on both windows

<img src="/uploads/db1493/original/3X/d/3/d3ee93032f6e672594d9ec2498d1817afb9d5c5d.png" width="628" height="500">
```

---
## \#17 Posted by: scepterr Posted at: 2017-09-15T17:50:24.157Z Reads: 226

```
Wierd guess 4am tweaking isn't smart lol
```

---
## \#18 Posted by: scepterr Posted at: 2017-09-15T22:00:46.742Z Reads: 227

```
Let me know if upping the max, gets rid of the error. I'm going through and doubling all the caps in the vesc  lol
```

---
## \#19 Posted by: Jinra Posted at: 2017-09-16T01:05:12.414Z Reads: 231

```
VESC 1
> Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 280.5
Current filtered : 125.2
Voltage          : 28.19
Duty             : 0.705
RPM              : 13659.7
Tacho            : 365
Cycles running   : 1176
TIM duty         : 5918
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 38.06

VESC 2
>Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 329.6
Current filtered : 128.3
Voltage          : 28.04
Duty             : 0.932
RPM              : 13752.8
Tacho            : 368
Cycles running   : 1186
TIM duty         : 7830
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 33.40

:0

This is full throttle on the bench from dead stop with the wheels/belt attached
```

---
## \#20 Posted by: Jinra Posted at: 2017-09-16T01:08:25.464Z Reads: 217

```
<img src="/uploads/db1493/original/3X/9/5/95255eeef70de83a944d017341e83e9b24206730.png" width="690" height="116">

LIES! @trampa
```

---
## \#21 Posted by: scepterr Posted at: 2017-09-16T01:16:16.942Z Reads: 207

```
I'm also curious why the voltage reading drops, I'm guessing the one shown in the fault wasn't your actual voltage?
```

---
## \#22 Posted by: Jinra Posted at: 2017-09-16T01:17:29.718Z Reads: 201

```
It cut out nearly instantaneously, so my guess is it that its because it never ramped up to full duty cycle (see .7 duty cycle in VESC 1).
```

---
## \#23 Posted by: scepterr Posted at: 2017-09-16T01:18:43.340Z Reads: 202

```
I've seen that on mine with duty cycles all over the place
```

---
## \#24 Posted by: Jinra Posted at: 2017-09-16T01:22:50.795Z Reads: 199

```
I upped my ABS max to 140 and it seems to have stopped the OC faults on the bench, I'll try it in real world riding and see how it goes.
```

---
## \#25 Posted by: scepterr Posted at: 2017-09-16T01:23:33.781Z Reads: 190

```
I just did the same 🤞
```

---
## \#26 Posted by: Jinra Posted at: 2017-09-16T01:30:55.284Z Reads: 189

```
Hoping the 40% polynomial braking curve helps with the braking reponse as well
```

---
## \#27 Posted by: Jinra Posted at: 2017-09-16T01:47:44.100Z Reads: 190

```
Welp, just ran a block and hit 148 amp OC fault one VESC and none on the other. Only once in the 2 minute ride, however.  Perhaps 150-160 would be a better setting.

As for the braking, 40% polynomial did not help, simpy made the braking more unpredictable.
```

---
## \#28 Posted by: scepterr Posted at: 2017-09-16T01:49:13.443Z Reads: 193

```
Do you know what the fault stop time setting under the advanced tab in motor config does? Would that increase how long it has to read the over current to fault?
```

---
## \#29 Posted by: Jinra Posted at: 2017-09-16T01:50:09.177Z Reads: 197

```
Pretty sure it just disables your control for the set time, mine is .5 seconds by default. Also you can't set ABS max over 150 as the program limits you to that...
```

---
## \#30 Posted by: scepterr Posted at: 2017-09-16T01:52:28.233Z Reads: 198

```
This setting
<img src="/uploads/db1493/original/3X/8/6/86c6f4cd1042a2acaec09f13b91c0cb708857525.jpg" width="666" height="500">
```

---
## \#31 Posted by: Jinra Posted at: 2017-09-16T01:53:16.176Z Reads: 187

```
<img src="/uploads/db1493/original/3X/c/0/c03cf2c92c60b06fd1ff9f48d342cb35f782cc39.png" width="690" height="128">

thats mine
```

---
## \#32 Posted by: scepterr Posted at: 2017-09-16T01:55:44.217Z Reads: 182

```
Interesting, never changed it. Is that on the new fw?
```

---
## \#33 Posted by: Jinra Posted at: 2017-09-16T01:58:34.638Z Reads: 183

```
yea it's probably a new default value
```

---
## \#34 Posted by: scepterr Posted at: 2017-09-16T04:05:22.340Z Reads: 181

```
Do you hear a tick before getting the fault?
```

---
## \#35 Posted by: Jinra Posted at: 2017-09-16T04:06:34.779Z Reads: 183

```
haven't noticed, it's pretty loud at full speed, also more worried about not eating it when i get a fault while riding
```

---
## \#36 Posted by: scepterr Posted at: 2017-09-16T04:08:53.022Z Reads: 187

```
Lol yeah I know that feeling. I'm doing runs holding my phone in front of me watching the fault live 😁
I hear a tick and I know a fault is coming within seconds unless I let go of the throttle. The tick prior to fault has been pretty consistent
```

---
## \#37 Posted by: scepterr Posted at: 2017-09-16T04:10:31.639Z Reads: 188

```
From motor/s to vesc what connectors are you using?
I never had this error on prior build that was using mt60 from motor to vesc. On this one I continued with the connectors that came on the motor which were the 5mm bullet with the springy part on the male side. I *think* those springy bullets might be at fault
```

---
## \#38 Posted by: Jinra Posted at: 2017-09-16T04:13:36.071Z Reads: 185

```
5.5mm bullets 12 awg
```

---
## \#39 Posted by: JohnnyMeduse Posted at: 2017-09-16T05:57:43.365Z Reads: 186

```
@Jinra ... Tips... The new firmware is still a experimental thing... I've try it and from personal experience I really don't like it, because the brake are not really nice, it like they are fully on then disappear.... still the best firmware is @Ackmaniac (still using it in current... but ... I'm not dead yet)
```

---
## \#40 Posted by: Jinra Posted at: 2017-09-16T05:59:48.719Z Reads: 190

```
I have the opposite experience, where they're fairly weak, then as I approach PPM min, it brakes harder.

The problem with ackmaniac's f/w was that FOC wouldn't run at all. Detection would work, but throttling to around 80% duty cycle caused the motor to cog and spaz out.
```

---
## \#41 Posted by: JohnnyMeduse Posted at: 2017-09-16T06:03:57.107Z Reads: 175

```
hummmm... it's kinda of weird... FOC motor detection is suppose to allow you more flexibility...
```

---
## \#42 Posted by: scepterr Posted at: 2017-09-16T06:06:55.351Z Reads: 176

```
I'm 99% sure I narrowed it down to a springy bullet connector, 1 of the 3 phase leads if I rattle it aggressively I can hear the ticks and then over current fault
@Jinra try it on the bench, full throttle, secure 2 leads and abuse one like you're going over tough terrain, go through each
I'm switching everything to mt60 tomorrow
```

---
## \#43 Posted by: Crossfire Posted at: 2017-09-16T06:14:16.309Z Reads: 171

```
I'm using 2.18 stock firmware on my FOOCbox, 2x4S 5Ah Lipo 245kV and full throttle acceleration and punchouts work flawlessly. No BMS, old fashion charging and discharging.
4mm bullets on my SK3 and Focbox, everthing else is XT90.
```

---
## \#44 Posted by: scepterr Posted at: 2017-09-16T06:16:17.079Z Reads: 170

```
I've seen some in use for almost a year in FOC without a single fault, and others dead in less than 10 miles. It's really the luck of the draw with the focbox.
```

---
## \#45 Posted by: Jinra Posted at: 2017-09-16T06:16:42.236Z Reads: 176

```
I don't think it's a physical connection issue for me. all my connections are rock solid and like i said, it can go over current on the bench as well.
```

---
## \#46 Posted by: scepterr Posted at: 2017-09-16T06:18:53.652Z Reads: 169

```
Mine can go overcurrent on the bench too without movement, but not consistently, I can force a fault if I shake 1 phase wire. Jiggle and twist it at every connection including on the vesc. 
I can replicate on 2 vescs
```

---
## \#47 Posted by: Jinra Posted at: 2017-09-16T06:20:48.411Z Reads: 165

```
mine is consistent with both vescs. I'm using split ppm so can bus wouldn't be influencing each other. Every time i blast full throttle with the default 130a abs max, it throws the fault on the bench
```

---
## \#48 Posted by: scepterr Posted at: 2017-09-16T06:22:22.700Z Reads: 161

```
If you run at full throttle for a few min on the bench do any of the connections heat up?
```

---
## \#49 Posted by: Jinra Posted at: 2017-09-16T06:24:15.478Z Reads: 164

```
never tested but i can check it out after riding tomorrow. i imagine that would be a better test than running it on bench.  

The raptor 2 uses tiny 3.5mm bullets and 14 awg cable and it seems to run fine
```

---
## \#50 Posted by: scepterr Posted at: 2017-09-16T06:26:07.535Z Reads: 163

```
On mine the bad one heats up on the bench, the others dont.  Just seems like a bad plug
```

---
## \#51 Posted by: trampa Posted at: 2017-09-16T10:01:00.101Z Reads: 166

```
Do your setup without belts to get best accuracy. Do it at system voltage! Use 50A max to get started. Increase step by step.
Weak brakes are a matter of your battery min.
I suggest to use the same values for motor max, battery max, and motor min, battery min. Then you can start to spread the values further apart.

Frank
```

---
## \#52 Posted by: Jinra Posted at: 2017-09-16T14:49:07.397Z Reads: 159

```
already did all that, and like i said, this setup and settings was working great on bldc 2.18. it only started having problems after transitioning to FOC 3.28

Also, why is the default value for battery regen -40? Seems excessively high.
```

---
## \#53 Posted by: trampa Posted at: 2017-09-16T15:51:11.616Z Reads: 159

```
30-40A is about the current that will flow when you brake hard. You need to shoot it somewhere and that's your battery. Whenever you brake you generate. Usually you don't do that continuously, so its not to much of an issue to use higher values. 
It's happens only for a few seconds.

Frank
```

---
## \#54 Posted by: Jinra Posted at: 2017-09-16T15:59:45.463Z Reads: 155

```
unless you're going down a long and steep hill. Going down a mountain braking with -40a current sounds like an easy way to make them explode given a standard 18650 only takes up to 4a current
```

---
## \#55 Posted by: Silverline Posted at: 2017-09-16T16:09:45.944Z Reads: 156

```
Going down a steep hill, the higheste current i have regen. is around 6,5amp pr. vesc...
```

---
## \#56 Posted by: Jinra Posted at: 2017-09-16T16:13:22.911Z Reads: 155

```
what's your regen set to?
```

---
## \#57 Posted by: Silverline Posted at: 2017-09-16T16:23:46.415Z Reads: 158

```
First i had bat min : -20a then bat min. -8a . Dosn`t change a thing.... same thing on the mobile log...
```

---
## \#58 Posted by: Jinra Posted at: 2017-09-16T16:29:06.571Z Reads: 155

```
honestly anecdotal evidence doesn't really matter. The point is that -40a current on a setup like 3p 18650 sounds dangerous. That setup can only accept 12a continuous.

I do get that that's the maximum current it can have and should only apply when you hit regen speeds, but it still sounds sketchy.

I don't understand why the brakes are so different from 2.18 to 3.28 on the same settings
```

---
## \#59 Posted by: trampa Posted at: 2017-09-16T18:00:14.759Z Reads: 153

```
When your motor acts as a generator, braking your board, it generates electricity and that needs to go somewhere. Either you evaporate it into heat (heat plate) or feed your battery. Going down a long steep hill, constantly braking, you feed the battery and the hill should not be steeper than your battery can cope with. You will roughly pump the same amount of energy into the battery than what you would use to go up the hill minus the losses you have when you shift kinetic energy into electric energy. Battery min. defines your maximum braking force, same like battery max. defines you maximum system power.

Frank
```

---
## \#60 Posted by: Jinra Posted at: 2017-09-16T18:35:10.076Z Reads: 152

```
Shouldn't Motor min determine your max braking force given that battery min always has to be lower?

I just don't see why the change was made between the old and new f/w? It worked great on 2.18
```

---
## \#61 Posted by: trampa Posted at: 2017-09-16T18:50:54.272Z Reads: 149

```
Conservation of energy..... The energy needs to go somewhere. Either into heat, using a strong electric heater attached under your board, or you shift the energy towards your battery. It needs to go somewhere. If one value is lower than the other, the software uses the lower of both values to protect your system. You can't evaporate energy into the universe. Conservation of energy...

It's the same for acceleration. If you only allow 8amps from the battery, increasing your motor max to 100A will not increase the boards absolute performance. The lower value defines your max output power, since we can't suck energy from the universe.

Frank
```

---
## \#62 Posted by: Bataleon Posted at: 2017-09-16T21:45:48.093Z Reads: 152

```
If `batt min` is set to -5A, for example, and `motor min` is set to -20A won't the 15A difference be dissipated by the motor as heat?
```

---
## \#63 Posted by: Jinra Posted at: 2017-09-16T21:47:30.726Z Reads: 152

```
that's how i assume it works in 2.18
```

---
## \#64 Posted by: Bataleon Posted at: 2017-09-16T22:13:15.467Z Reads: 153

```
Would be really interesting to hear Benjamin's response. I've always wondered about this.
```

---
## \#65 Posted by: SilentException Posted at: 2017-09-16T22:36:00.431Z Reads: 172

```
[quote="Bataleon, post:64, topic:33203"]
Would be really interesting to hear Benjamin's response.
[/quote]

Sure would. This whole regenerative braking is always creating more questions than answers.
I actually thought the difference would be dissipated 'somewhere' in the VESC and not the motor. But who can tell for sure? Maybe it's time to ask the questions about it on vesc-project.com forum? :)
```

---
## \#66 Posted by: Ackmaniac Posted at: 2017-09-16T22:59:01.764Z Reads: 168

```
The VESC converts the voltage of the battery to the right amount of voltage for the motor. This is the duty cycle.
So when the vesc works at 10% duty cycle then the motor runs at 10% of the batterys voltage. At the same time the battery only has to provide 10% of the motors current.

    10% duty cycle
    Battery 40V   4A
    Motor    4V  40A

At 90% duty cycle the motor runs at 90% of the batterys voltage and the battery only has to provide 90% of the motor current.

    90% duty cycle
    Battery 40V  36A
    Motor   36V  40A

Now braking works exactly the same. Only the power is going in the other direction but the duty cycle and ratios behave the same.

So when you do a full brake and the duty cycle is at 50% and the motor min is set to -70A and battery min to -10A then battery min sets the limit.

    50% duty cycle
    Battery 40V  35A
    Motor   20V  70A

So in this case you would exceed the limit of -10A amps by far. So the VESC reduces the brake power to -10A at the battery which results at 50% duty cylce to -20A at the motor.

And when the speed goes down the duty cycle becomes lower and so the ratio changes and the VESC is allowed to use more and more amps at the motor side for braking.
So the maximum brake power is allowed at duty cycles below  14A (10A / 70A).

So the higher you set your battery min the stronger the brakes will be at high speeds.
```

---
## \#67 Posted by: SilentException Posted at: 2017-09-16T23:42:55.470Z Reads: 159

```
Thanks for the explanation! So basically, if I got it correctly, Motor Min is like brake force parameter that will be adjusted according to the Battery Min and the duty cycle. There is no difference that should be dissipated.

Do you happen to be able to know or explain the voltage VESC puts back at the battery while braking (or how does that work)? It is not a set parameter as far as I can tell..
```

---
## \#68 Posted by: Deckoz Posted at: 2017-09-17T05:58:22.004Z Reads: 157

```
First off

If your in FOC and hear ticking and are expecting a fault. Your running the motor at the wring Hz. Change to something else. (I think 20000hz is default) go higher. 

Second calculating voltage for what comes in is easy. RPM/kv = V

However...amps will turn into volts if there's no path for the current and can cause over voltage.
```

---
## \#69 Posted by: crustyxpunk Posted at: 2017-09-17T14:33:13.020Z Reads: 149

```
Just wanted to report in, my 6374, TB vesc, on 12sp4 battery is running good on FOC, however like others have said brakes are a bit weak, but not terrible. I also found that after climbing a pretty steep hill 25% grade thats decently long the brakes and throttle are fairly anemic for a short time, but return after about 30 seconds.
```

---
## \#70 Posted by: Ackmaniac Posted at: 2017-09-17T15:29:25.200Z Reads: 143

```
Guess that's because your Vesc overheats.
```

---
## \#71 Posted by: trampa Posted at: 2017-09-18T08:04:22.090Z Reads: 145

```
That is very likely. Your temp soft cuttoff is preventing that you overheat your system any further. Basically you surpassed the limits of your hardware and its time for an upgrade of components, or ride less steep hills. After 30 seconds the temp reaches acceptable values again and your brakes/power come back back to life. At this point you are close to reaching critical values again, so don't attack a hill (riding downhill) because your brakes could fail again and you have no redundant brake system to compensate the loss of your motor brake. This is why I suggest to use disc brakes in addition (on MTBs it's possible) when riding in hilly areas. 

Frank
```

---
## \#72 Posted by: crustyxpunk Posted at: 2017-09-18T08:45:09.046Z Reads: 143

```
Okay good to know! I thought I had pretty good components already. TB 6374 Motor, TB VESC and TB 12s4p battery. Which components would you consider an upgrade? The board is street only, not a MTB, so disc brakes dont really seem to be an option or something I really want. My area definitely isn't as hilly as say San Fransisco or anything like that. Thanks in advance!
```

---
## \#73 Posted by: Ackmaniac Posted at: 2017-09-18T11:22:38.254Z Reads: 138

```
Add heatsinks or buy a esc that has already heatsinks.
```

---
## \#74 Posted by: trampa Posted at: 2017-09-18T14:41:16.178Z Reads: 140

```
Or lower motor KV, or both, or twin drive etc. Anything relieving strain from the ESC.

Frank
```

---
## \#75 Posted by: crustyxpunk Posted at: 2017-09-18T23:16:22.388Z Reads: 141

```
I think for my next build I'll go dual 6355 190kv. This motor is 190kv but I do beat on it pretty hard. In the interim I'll try and add a heat sink or maybe even a small fan to the enclosure and see if that helps.  Thanks for the replies!
```

---
## \#76 Posted by: Jinra Posted at: 2017-09-21T15:12:58.300Z Reads: 139

```
So i guess the weather brakes issue has been addressed, but does anyone know why i get over current faults on high load? Mainly happens when i accelerate too quickly. Today one of my motors also cutout and was in perma brake mode, but resolved itself after a restart. Is this a sign of a burnt drv?

@Eboosted @scepterr @Ackmaniac
```

---
## \#77 Posted by: crustyxpunk Posted at: 2017-09-21T15:55:25.432Z Reads: 134

```
Okay so I switched back to FOC and also made some current changes to my setup and it seems to have helped somewhat with my vesc overheating issue when going up hills. I also played with the throttle/brake curve a bit and that also seems to have given me a little more brake at speed. Having adjusted the expo brake curve has made the brakes a bit more responsive when I'm at speed while decreasing the amount of brake I have while going slower. It's still not great but it does feel better. Here are some screen shots for reference. 

<img src="/uploads/db1493/original/3X/3/1/31727da3c95b1d84322da1d94859682d44f459ce.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/3/03248a8cc2a03646acf8533cccdc2a29003df485.JPG" width="666" height="500">
```

---
## \#78 Posted by: scepterr Posted at: 2017-09-21T17:56:20.844Z Reads: 125

```
Maybe bad fet
```

---
## \#79 Posted by: Jinra Posted at: 2017-09-21T19:17:10.830Z Reads: 125

```
hm, weird that it worked after turning it back on again though. Still, that overcurrent problem is a killer.. I'll probably step back down to f/w 2.54
```

---
## \#80 Posted by: scepterr Posted at: 2017-09-21T19:23:41.934Z Reads: 130

```
I'm not messing with vesc6 fw till an update or 2
```

---
## \#81 Posted by: Jinra Posted at: 2017-09-22T04:14:20.750Z Reads: 132

```
@scepterr @JohnnyMeduse @Blasto

Figured out why I was getting OC faults while blasting the throttle. This is precisely what the positive/negative ramping time in PPM is. with a sudden increase in current, the VESC pulls too much too fast due to the abrupt PPM signal change. Using a positive ramping time will give it some breathing room to gradually bring up the current to the requested levels without causing a huge spike.

I'm finding .2s to be satisfactory in relieving OC faults on the bench. Will test in the field tomorrow.
```

---
## \#82 Posted by: scepterr Posted at: 2017-09-22T04:16:16.255Z Reads: 133

```
Interesting, do you have stock BOM caps or upgraded?
```

---
## \#83 Posted by: Jinra Posted at: 2017-09-22T04:38:58.300Z Reads: 132

```
Upgraded, dual ollinboards VESC

Oh @scepterr, I went back to FOC on 2.54 and I noticed something strange. After setting it up and detection, I found that I can ramp to full duty cycle at about 30% throttle, but anything after that makes the motor spin at a lower pitch sound, like there's resistance or something. This doesn't happen on 3.29 so I think i'll stick on the newer f/w; I feel like I'm going to blow a DRV with that sound.
```

---
## \#84 Posted by: scepterr Posted at: 2017-09-22T04:42:49.755Z Reads: 130

```
Peculiar, identical behavior on both vescs?
```

---
## \#85 Posted by: Jinra Posted at: 2017-09-22T04:44:12.253Z Reads: 126

```
For the OC issue on 3.28/3.29 yes, for the weird change in pitch, no... 

I tried FOC once before on 2.54, but I forgot which of the Ollin VESCs I used, at high eRPM the motor would cog and spaz the fuck out so I was really afraid to try again. This time it didn't cog, but made a disconcerting lower pitch whine.

Sorry should've taken a vid.
```

---
## \#86 Posted by: Eboosted Posted at: 2017-09-22T06:12:12.625Z Reads: 129

```
Are you guys getting much less power delivery with the new firmware under the same current settings?

Tomorrow I'll go back to the old firmware and will install ackmaniac firmware
```

---
## \#87 Posted by: Jinra Posted at: 2017-09-22T06:15:06.737Z Reads: 134

```
I'm not noticing less power delivery. Are you using the same current settings as before? Here's what i'm using..

10s4p dual 6355 230kv
Motor Max: 70
Motor Min: -60
Battery Max: 40
Battery min: -25
ABS max: 150

These are per VESC
```

---
## \#88 Posted by: Eboosted Posted at: 2017-09-22T06:42:22.243Z Reads: 136

```
12S4P
Motor Max: 65
Motor Min: -45
Battery Max: 40
Battery min: -25
ABS max: 130

So you did change the battery min from -8A to -25A per VESC, how are you feeling your brakes now?
```

---
## \#89 Posted by: Jinra Posted at: 2017-09-22T06:49:53.455Z Reads: 132

```
I haven't tested -25 yet but -30 each VESC felt pretty good, though still not as linear as I'd like. At slow speeds it tends to brake hard.
```

---
## \#90 Posted by: Jinra Posted at: 2017-09-22T13:46:40.878Z Reads: 132

```
Guess that explains my locked up motor

http://vesc-project.com/node/123
```

---
## \#91 Posted by: Mikenopolis Posted at: 2017-09-22T17:07:42.669Z Reads: 131

```
I'm working on my Carvon V3 with a Raptor 1 deck. These are my last two changes, (80 Motor max was recommended by Carvon). In the first setting I was getting cogging when I pushed the throttle too hard so I messed with it and got the the second settings which got rid of the cogging but now I have weak brakes that won't even stop me. Any idea of what I need to change to get brakes back but not have cogging?

I'm using a 10s3p battery with vesc-x 

<img src="/uploads/db1493/original/3X/7/8/7834c16dc190822f599bf3827836b9bc30b86ff1.jpg" width="690" height="296">
```

---
## \#92 Posted by: Mikkiller Posted at: 2017-09-24T14:16:59.785Z Reads: 124

```
Where did you find that setting? Is it on the new VESC tool only?
```

---
## \#93 Posted by: Jinra Posted at: 2017-09-24T16:26:12.104Z Reads: 127

```
correct only on the new tool
```

---
## \#94 Posted by: Jinra Posted at: 2017-09-24T20:26:49.201Z Reads: 131

```
@scepterr @Eboosted  Ugh one issue solved, another arises. Now when I'm going a certain duty cycle and apply more throttle on a slight/moderate incline, the board stutters for a second like it's out of sync. I'm assuming this only happens uphill since downhill doesn't apply much current.

Any ideas guys? I'll try to get a fault reading later
```

---
## \#95 Posted by: scepterr Posted at: 2017-09-24T20:30:55.785Z Reads: 131

```
Hmm that's a new one, no idea
Increase ramp step?
```

---
## \#96 Posted by: Jinra Posted at: 2017-09-24T20:46:36.233Z Reads: 128

```
I think ramp step is only for bldc
```

---
## \#97 Posted by: scepterr Posted at: 2017-09-24T20:49:33.778Z Reads: 123

```
Oh right, then back to no idea 🤔

Any chance battery sagging below limits?
```

---
## \#98 Posted by: Jinra Posted at: 2017-09-24T21:04:27.968Z Reads: 122

```
nah these are new and full charge. I did notice that when it happens the motors are making a louder than average whine. At high and low duty it doesn't make that loud whine.
```

---
## \#99 Posted by: scepterr Posted at: 2017-09-24T21:10:29.500Z Reads: 126

```
Something I was thinking about today....
Motor detection is best with battery that will be used....but typically that would be done with a full battery, while actual use will be at nominal voltage at least 70% of the time. Detection results do vary with voltage....so would it be best to do detection with battery at nominal voltage?
```

---
## \#100 Posted by: Jinra Posted at: 2017-09-24T21:16:11.472Z Reads: 124

```
Hmm not sure. I really like FOC, so i sure hope i can iron this out
```

---
## \#101 Posted by: Eboosted Posted at: 2017-09-24T23:33:47.756Z Reads: 124

```
I'm having studdering at light accelerations from stand still, like if the sensors were not synced correctly, this might be the same thing you are feeling at light inclines.
```

---
## \#102 Posted by: Jinra Posted at: 2017-09-24T23:36:24.066Z Reads: 124

```
I don't think it's the sensors because at that point it's running pure sensorless because it's way past the sensorless erpm
```

---
## \#103 Posted by: Jinra Posted at: 2017-09-25T00:23:14.845Z Reads: 126

```
Got the fault, the dreaded overcurrent fault again :frowning:

> Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 318.3
Current filtered : 153.8
Voltage          : 24.93
Duty             : 0.950
RPM              : 27241.8
Tacho            : 16706
Cycles running   : 70844
TIM duty         : 7980
TIM val samp     : 2
TIM current samp : 4200
TIM top          : 8400
Comm step        : 0
Temperature      : 29.52

Going to try using "Stator Saturation Compensation" as that sounds like it might help
```

---
## \#104 Posted by: scepterr Posted at: 2017-09-25T00:32:39.957Z Reads: 125

```
That's a crazy amount of current it read....
```

---
## \#105 Posted by: Jinra Posted at: 2017-09-25T00:33:10.341Z Reads: 125

```
Yea thats pretty much been all my OC faults... still unsure as to why, but always related to a sudden increase in acceleration.
```

---
## \#106 Posted by: Jinra Posted at: 2017-09-25T00:48:53.535Z Reads: 132

```
welp that didn't work, fuck it i'm going back to BLDC

(╯°□°）╯︵ ┻━┻
```

---
## \#107 Posted by: Jinra Posted at: 2017-09-26T02:25:01.068Z Reads: 131

```
After seeing this message in the vesc-tool I decided to try doubling my Observer Gain and... my problems might be fixed!! I haven't gotten OC faults either on the bench or while riding, but only time will tell!

<img src="/uploads/db1493/original/3X/c/d/cd9441bab3c2f5406873e2495eea20cfdf1980a8.png" width="690" height="335">

EDIT: Confirmed, this fixed my overcurrent problems! Doubling it worked great, halving it also worked, however caused some weird acceleration behavior intermittently when doing full throttle from standstill.
```

---
## \#108 Posted by: scepterr Posted at: 2017-09-26T02:32:25.960Z Reads: 126

```
What the hell does that setting do...why are 2x or .5 suggested alternate values..lol Itll be crazy if thats what's causing the myriad of oc faults
```

---
## \#109 Posted by: Jinra Posted at: 2017-09-26T02:33:56.828Z Reads: 121

```
Yea I tried googling it, but it just made me feel dumb. So far doubling has produced no OC faults, but.. it might've gotten louder? Hard to tell.
```

---
## \#110 Posted by: scepterr Posted at: 2017-09-26T02:37:14.384Z Reads: 121

```
I hate this blindly changing settings to fix one issue not knowing what other issues it could cause. Like I expect "detected values" to be correct...if not, why not
```

---
## \#111 Posted by: Jinra Posted at: 2017-09-26T02:40:21.438Z Reads: 125

```
I think FOC is too complex to have a "catch all solution" especially with the wide variety of motors, but perhaps there could be something set in place that tests the motors are varying currents and duty to see if there are any faults and/or cogging.
```

---
## \#112 Posted by: scepterr Posted at: 2017-09-26T02:45:22.857Z Reads: 125

```
I think some kind of understanding of what values a specific motor should have to be able to know if detected values are correct would help. Also I think anybody selling esk8 motors should provide a datasheet with "expected, valid results with certain battery configurations"  that would help immensely
```

---
## \#113 Posted by: Jinra Posted at: 2017-09-26T02:46:44.980Z Reads: 127

```
I agree, but the esk8 scene (especially DIY esk8 scene) isn't mature enough yet. I mean, we only have 1 semi-dedicated ESC right now. Hopefully the scene will evolve over the next couple years and give us more options, standardization, competition, and stability.
```

---
## \#114 Posted by: Martinsp Posted at: 2017-11-02T11:47:23.557Z Reads: 100

```
Hi, @Jinra 
How is the solution holding up over time?
```

---
## \#115 Posted by: Jinra Posted at: 2017-11-02T15:16:04.731Z Reads: 98

```
It's been good! I had a wipe out that gave me a concussion, but that turned out to be a mixture of a shorted motor and a bad VESC. After replacing both motor and VESC, I've been cautious while riding, but haven't encountered anything weird yet and no faults have been thrown. 

The official Vedder f/w 3.3 has this stated in the change log.

>=== FW 3.30 ===
* Activated iterative observer for better operation at high ERPM.
* Check for NAN and truncate some FOC variables.
* Speed controller windup protection improvement

Not sure if this means that I no longer have to double the observer gain, but I'll hold off on updating for now.
```

---
## \#116 Posted by: Martinsp Posted at: 2017-11-02T16:26:33.176Z Reads: 94

```
I heared about your accident :/ Hope it is all coming together well. :)

I am using 2.54 FW in watt mode and BLDC now because I had problems with sensored FOC a while back. I found your thread recently and decided to revisit the FOC for the quiteness mainly :D I am having the same issue that in BLDC the motor starts fine but stutters in FOC at low speeds. I am going to try sensorless but I think I did that already with no change so I dont blame the sensors for now. I will try messing with the observer gain and see what happens now that I know it has worked for you!
```

---
## \#117 Posted by: Jinra Posted at: 2017-11-02T16:38:31.433Z Reads: 92

```
Just FYI I had issues with FOC in 2.xx as well where it would stutter (at high RPM though), but FOC runs a LOT better in 3.xx f/w
```

---
