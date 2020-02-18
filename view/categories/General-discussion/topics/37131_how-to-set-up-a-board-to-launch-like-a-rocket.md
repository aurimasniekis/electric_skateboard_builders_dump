# How to set up a board to launch like a rocket

### Replies: 43 Views: 1877

## \#1 Posted by: pshaw Posted at: 2017-11-02T02:31:19.063Z Reads: 256

```
So I have been up until now keeping it at a cool 65a motor max until I started doing some research. I realized that as long as your motors don't get too hot to the touch you really can crank it up over 100a and still be pretty safe it seems. So right now I'm sitting at 120a motor max on this setup...

12S4P dual 6374 190kv 16t/40t on 107mm flywheels

My vescs are shutting down and rebooting at around the 2-3mph mark after launching. At 100a it was fine but 120a I'm assuming at that low of a duty cycle it is pulling crazy amps and triggering this fault code...

<img src="/uploads/db1493/original/3X/9/6/96bc543b5392299bb15bc838096c5cd8d0aeeead.jpeg" width="281" height="500">

Anyone have any suggestions on this one? I know I can mess with throttle curve or duty cycle ramping to get around this... but I really want the full 120a in my face without smoothing the acceleration out to get around it :stuck_out_tongue:
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-11-02T02:33:50.506Z Reads: 232

```
there is absolutely no way your pulling 120a
ever.
```

---
## \#3 Posted by: pshaw Posted at: 2017-11-02T02:38:02.114Z Reads: 229

```
[quote="GrecoMan, post:2, topic:37131, full:true"]
there is absolutely no way your pulling 120a
ever.
[/quote]

well I logged 75a just doing a light acceleration unless the data is wrong in the metr app ... whatever the true amps are I'm not concerned with. I'm just tying to solve my issue here because the vescs are restricting me.

@BigBoyToys get in here and spead them knowledges :stuck_out_tongue:
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-11-02T02:39:02.647Z Reads: 221

```
i would lower you motor a until you stop getting faults
```

---
## \#5 Posted by: jbruce Posted at: 2017-11-02T02:39:30.041Z Reads: 223

```
This is motor amps, not battery amps, so since he is at a relitivly low speed the duty cycle is low meaning he's pulling a a lot of amps at a low voltage, a low wattage. His battery amps at 1mph could never get to 120 as his duty cycle would be too low.
```

---
## \#6 Posted by: pshaw Posted at: 2017-11-02T02:39:40.446Z Reads: 222

```
[quote="GrecoMan, post:4, topic:37131, full:true"]
i would lower you motor a until you stop getting faults
[/quote]

where's the fun in that?
```

---
## \#7 Posted by: NickTheDude Posted at: 2017-11-02T02:40:03.503Z Reads: 208

```
At low duty cycle it's definitely possible to be pulling 120 motor amps. Sadly I can't help much with you problem though. In the readout is the "Current" it's refering to battery amps? If so then at 0.18 duty you'd be at 76.2/0.18 = 423A in the motor... That can't be right, can it?
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-11-02T02:40:08.928Z Reads: 200

```
you get to actually ride! 😜
```

---
## \#9 Posted by: pshaw Posted at: 2017-11-02T02:40:17.598Z Reads: 206

```
[quote="jbruce, post:5, topic:37131, full:true"]
This is motor amps, not battery amps, so since he is at a relitivly low speed the duty cycle is low meaning he's pulling a a lot of amps at a low voltage, a low wattage. His battery amps at 1mph could never get to 120 as his duty cycle would be too low.
[/quote]

This^ 


 10 char
```

---
## \#10 Posted by: pshaw Posted at: 2017-11-02T02:40:50.987Z Reads: 199

```
Motor amps not batt amps @NickTheDude
```

---
## \#11 Posted by: jbruce Posted at: 2017-11-02T02:44:36.128Z Reads: 192

```
If you're running FOC you could try increasing your switching frequency from 20k to 30k as it may be the vesc is not taking measurements at precise enough intervals and accidently over shooting it causing a over current error. (idk if there is something like this for BLDC) Also you could try increasing your absolute motor max setting as that is what will cause the vesc to reboot if it measures a current above that.
```

---
## \#12 Posted by: jbruce Posted at: 2017-11-02T02:46:56.007Z Reads: 184

```
Before you try changing the frequency, try changing the absolute max value to something like 160-170. I'm assuming when you changed your motor max you left your absolute max at 130.
```

---
## \#13 Posted by: pshaw Posted at: 2017-11-02T02:47:02.125Z Reads: 189

```
[quote="jbruce, post:11, topic:37131, full:true"]
If you're running FOC you could try increasing your switching frequency from 20k to 30k as it may be the vesc is not taking measurements at precise enough intervals and accidently over shooting it causing a over current error. (idk if there is something like this for BLDC) Also you could try increasing your absolute motor max setting as that is what will cause the vesc to reboot if it measures a current above that.
[/quote]

Now we are getting somewhere! :slight_smile:

I'm actually running in Hybrid mode because I like having still having my DRVs intact lmao. I wonder where it switches over from sensored to unsensored.... Edit**** right there is literally a value for that in the config *facepalm*

Yep left abs max at 130a and motor max cranked up to 120a
```

---
## \#14 Posted by: jbruce Posted at: 2017-11-02T02:48:57.733Z Reads: 172

```
Sensored/hybrid vs unsensored are different things from BLDC vs FOC btw.
```

---
## \#15 Posted by: pshaw Posted at: 2017-11-02T02:52:05.140Z Reads: 176

```
[quote="jbruce, post:14, topic:37131, full:true"]
Sensored/hybrid vs unsensored are different things from BLDC vs FOC btw.
[/quote]

Yeah but using the hall sensors would give more precise measurements than non sensored right?

Also some other tidbits... along with abs max being set to 130 I'm have max watts unchecked and batt max at 40 (this prob can at least go to 50 right?)
```

---
## \#16 Posted by: b264 Posted at: 2017-11-02T02:54:52.321Z Reads: 179

```
[quote="GrecoMan, post:2, topic:37131, full:true"]
there is absolutely no way your pulling 120a
ever.
[/quote]

Agree -- at 120A you are melting the 10 or 12 gauge wire coming into the ESC or vaporising the leads on the esc capacitors.  It's just not happening.  You might have like milliseconds where you're pulling that, but there is no way you are pulling that for more than that.  So basically, it's not going to really hurt you to turn it down, I would think.

In fact I vaporised the leads on an Evolve ESC's capacitors before, and that's only an 80A system... supposedly
```

---
## \#17 Posted by: jbruce Posted at: 2017-11-02T02:55:41.732Z Reads: 174

```
I don't think hall sensors will effect preciseness of current measurements but I could be wrong, I believed they were just for a smooth startup as the vesc knows which phase to energize. Changing motor min will effect braking ability but isn't part of your over current problem.
```

---
## \#18 Posted by: pshaw Posted at: 2017-11-02T02:56:07.456Z Reads: 175

```
[quote="b264, post:16, topic:37131, full:true"]
[quote="GrecoMan, post:2, topic:37131, full:true"]
there is absolutely no way your pulling 120a
ever.
[/quote]

Agree -- at 120A you are melting the 10 or 12 gauge wire coming into the ESC or vaporising the leads on the esc capacitors.  It's just not happening.  You might have like milliseconds where you're pulling that, but there is no way you are pulling that for more than that.  So basically, it's not going to really hurt you to turn it down, I would think.

In fact I vaporised the leads on an Evolve ESC's capacitors before, and that's only an 80A system... supposedly
[/quote]

let's not get hung up on the does it really draw that much part... all I know is it felt faster at 120 than 100 on the ol butt dyno.
```

---
## \#19 Posted by: pshaw Posted at: 2017-11-02T02:58:24.758Z Reads: 159

```
[quote="jbruce, post:17, topic:37131, full:true"]
I don't think hall sensors will effect preciseness of current measurements but I could be wrong, I believed they were just for a smooth startup as the vesc knows which phase to energize. Changing motor min will effect braking ability but isn't part of your over current problem.
[/quote]

sorry that was a typo... fixed it 

BATT MAX not motor min
```

---
## \#20 Posted by: jbruce Posted at: 2017-11-02T03:21:46.706Z Reads: 151

```
Still affecting braking ability. Just change your absolute motor max to 160 and try that. It should solve all your problems.
```

---
## \#21 Posted by: pshaw Posted at: 2017-11-02T03:27:47.260Z Reads: 144

```
[quote="jbruce, post:20, topic:37131, full:true"]
Still affecting braking ability. Just change your absolute motor max to 160 and try that. It should solve all your problems.
[/quote]

jesus I can't get it right tonight. I'm meaning to say batt max (which affects high speed side) for 12s4p you think it's plenty safe to up from 40 to 50?

I'll try upping abs max and see if that does the trick...
```

---
## \#22 Posted by: pshaw Posted at: 2017-11-02T03:47:44.559Z Reads: 140

```
<img src="/uploads/db1493/original/3X/6/0/60c98194d490aebb49f3db4929c108fdc9af0566.jpeg" width="281" height="500">

Up we go. I feel like I’m playing with fire here ....
```

---
## \#23 Posted by: pshaw Posted at: 2017-11-02T03:59:41.734Z Reads: 130

```
And esc is dead after bumping to 140 abs max. Hopped on for a 150 test and realized I only had one motor running.... 

Can’t say I didn’t see that coming....
```

---
## \#24 Posted by: BigBoyToys Posted at: 2017-11-02T04:11:40.863Z Reads: 137

```
Sorry im still in Hawaii on vacay.

I run 150A abs max on one of my builds and havent lost an esc in a while. Full throttle take offs from a dead stop have usually been where the problems happen the most.

If the code only happens at low dutycycle, Id suggest softening the bottom end of the throttle curve. Youll lose a little of the line but youll still have more than you did at 65A motor.

Replace that drv and try again 😉.
```

---
## \#25 Posted by: pshaw Posted at: 2017-11-02T04:36:00.329Z Reads: 136

```
[quote="BigBoyToys, post:24, topic:37131, full:true"]
Sorry im still in Hawaii on vacay.

I run 150A abs max on one of my builds and havent lost an esc in a while. Full throttle take offs from a dead stop have usually been where the problems happen the most.

If the code only happens at low dutycycle, Id suggest softening the bottom end of the throttle curve. Youll lose a little of the line but youll still have more than you did at 65A motor.

Replace that drv and try again 😉.
[/quote]

Yeah it would only happen at low duty cycle (like 2-3mph). 

I'm assuming the vesc6 would solve this almost certainly correct?
```

---
## \#26 Posted by: saul Posted at: 2017-11-02T04:47:24.811Z Reads: 125

```
just strap a rocket on... one time use.. the end...
```

---
## \#27 Posted by: BigBoyToys Posted at: 2017-11-02T04:49:20.445Z Reads: 127

```
Hard to say, I run 37.5 batttery Amps per motor and 100-120A  motor amps per motor on my 4wd's and have never seen that code on FOC box's.
```

---
## \#28 Posted by: saul Posted at: 2017-11-02T04:52:51.283Z Reads: 125

```
with 4wd you won't hit as many amps per esc as a dual would...
```

---
## \#29 Posted by: pshaw Posted at: 2017-11-02T04:53:13.193Z Reads: 125

```
[quote="BigBoyToys, post:27, topic:37131, full:true"]
Hard to say, I run 37.5 batttery Amps per motor and 100-120A  motor amps per motor on my 4wd's and have never seen that code on FOC box's.
[/quote]

But DD and on top of that 4wd isn't a fair comparison is it? Also do you leave max amps unchecked or is it limited?
```

---
## \#30 Posted by: Acido Posted at: 2017-11-02T06:09:21.381Z Reads: 123

```
You will possibly end up frying something, just go dual I guess
```

---
## \#31 Posted by: pat.speed Posted at: 2017-11-02T11:10:56.419Z Reads: 116

```
May I ask but why do you really need to set it that high, why not have just left it at 100a max
```

---
## \#32 Posted by: longhairedboy Posted at: 2017-11-02T11:20:07.270Z Reads: 115

```
I've never been able to get it to launch like a rocket (the way i would like) and not reset at least one of the vesc based ESCs during or immediately after the hard acceleration part.
```

---
## \#33 Posted by: pshaw Posted at: 2017-11-02T16:50:02.807Z Reads: 109

```


@longhairedboy 

 Bummer. Maybe it’s just a limitation that’s unavoidable from a 2wd belt setup. 

I know they are doing it on 4x hubs
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-11-02T17:09:42.244Z Reads: 109

```
i see what you did there.
```

---
## \#35 Posted by: pshaw Posted at: 2017-11-02T20:51:23.218Z Reads: 103

```
[quote="pat.speed, post:31, topic:37131, full:true"]
May I ask but why do you really need to set it that high, why not have just left it at 100a max
[/quote]

Ever launched a Tesla in ludacrous mode? For them feels dude. Them feels. With a guy with speed in the name I feel like you would get it :stuck_out_tongue:
```

---
## \#36 Posted by: Idle Posted at: 2017-11-02T22:10:47.738Z Reads: 102

```
https://streamable.com/ferwe
```

---
## \#37 Posted by: pat.speed Posted at: 2017-11-03T04:48:53.661Z Reads: 92

```
Hahah yes I love speed but I also like smooth acceleration
```

---
## \#38 Posted by: MysticalDork Posted at: 2017-11-03T05:25:57.130Z Reads: 89

```
I'm running 80a per motor in FOC with dual 6355s with a vesc6, and it doesn't stutter, doesn't jerk, doesn't anything. SUUUPER smooth. I can't stay on it with a full throttle pull unless I'm sitting on the board.
```

---
## \#39 Posted by: pshaw Posted at: 2017-11-03T16:45:45.034Z Reads: 83

```
Turns out the vesc somehow reset settings and I didn’t kill the drv. 

Went back in and we are back at it. Here’s a log of messing around without launching. 

Hit 97.5a motor at 18mph..... so it’s definitly getting up there. 


https://metr.at/r/vHcpM
```

---
## \#40 Posted by: longhairedboy Posted at: 2017-11-03T18:39:43.486Z Reads: 78

```
[quote="pshaw, post:39, topic:37131"]
Turns out the vesc somehow reset settings and I didn’t kill the drv.
[/quote]

its does that doesn't it? Mother fucker i thought i was seeing shit. This happened to my customer not too long ago. 

@zpoole27 you see this?
```

---
## \#41 Posted by: Deckoz Posted at: 2017-11-03T19:00:41.093Z Reads: 74

```
Hahaha dude its weird...its happened a few times when we've been messing with pshaws board. Shit just resets to defaults...and then disassembling the trampa to get to the slave to reconfigure is a pain. But no your not seeing shit lol
```

---
## \#42 Posted by: longhairedboy Posted at: 2017-11-03T19:03:59.257Z Reads: 73

```
i basically had him dump and copy the settings from his secondary vesc and everything was fine. but he was like "dude... did you program the second vesc?" i was like.. "what?"
```

---
## \#43 Posted by: Deckoz Posted at: 2017-11-03T19:54:33.433Z Reads: 66

```
Hahaha yea. First time it happened it was like...OK I know I had a couple beers but...I swear we did this...

Then I think its happened like 5 or 6 times total since the July. So it was like wait wut? Werent you just riding it?
```

---
