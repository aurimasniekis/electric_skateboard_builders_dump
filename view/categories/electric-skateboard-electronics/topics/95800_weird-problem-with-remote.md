# Weird problem with remote

### Replies: 9 Views: 175

## \#1 Posted by: sash Posted at: 2019-06-04T01:53:08.433Z Reads: 69

```
Hey all,

I've being riding my esk8 for several years without major problems, but last couple of times a weird problem started to happen with remote.   Occasionally, the esk8 stops to react to input from remote.  (I mean that it does not accelerate when I pull the trigger.)  When I take my finger off the trigger for a second and then put it back on the trigger, the esk8 behaves as if nothing happened (accelerates and brakes as usual).

My setup:

Mini remote
2 VESC-X  (setup in FOC mode)
Dual Torqueboards 6355/190kV motors
10S4P battery with 30Q cells

Just to eliminate a few obvious reasons:

1.  It is not batteries in the remote.  Just changed them, and the problem is still happening.
2.  I don't think it has to do with loosely connected wires between remote receiver and VESCs.   All connections are soldered.  (I used to have a problem with wires getting loose.  So I soldered everything, and never had this problem again.)

I was able to reproduce the problem at home.  I put the esk8 on the back and run motors at various speeds.  Occasionally, motors just stop when my finger is still on the trigger, and they don't react to any movements of the trigger.  If I take my finger off the trigger, and put it back, it works normal again.

I think it might have to do with the way how I pull the trigger.  (Maybe it happens if I pull it too fast, but I am not sure.)

Does anybody have an idea what might be the cause?   Did anybody have a similar problem?

I include screenshots with my VESC settings.  (These are screenshots from 2017, but I don't think I changed them since then.)

Thanks a lot!


![21%20AM|690x431](upload://dxzcoEBPtISzPbPT1q2tEakf5vm.png) 

![05%20PM|690x431](upload://dZaAB6s8OjHNoUGWvWjJpwNgMoW.png) 

![11%20PM|690x431](upload://ipV63p8pIyxy8pkOHkaRdG2fjnE.png)
```

---
## \#2 Posted by: wafflejock Posted at: 2019-06-04T04:08:33.600Z Reads: 48

```
In real-time data activate ppm display to see if receiver is sending bad signal which means either transmitter or receiver issue.  I've had homemade remotes go bad in a similar way when the potentiometer I was using would eventually wear out so have since switched to using hall sensors.  If ppm data looks good though and motor stops responding check terminal tab and type faults to see any faults since startup.
```

---
## \#3 Posted by: sash Posted at: 2019-06-04T05:33:26.837Z Reads: 41

```
Thanks for the tips.  I am going to run tests tomorrow.   

One thing I was thinking about:   Can this kind of problem happen because of FOC mode?   I've read that FOC can do weird things and cause problems like sudden braking when riding at high speed, etc.   I've being planning to switch back to BLDC mode for a while.   But my esk8 was working fine, so I have not done it yet.

Can my problem be one of FOC quirks?   Why does it happen now, when it was working fine before?
```

---
## \#4 Posted by: wafflejock Posted at: 2019-06-04T05:38:35.018Z Reads: 36

```
Well if it is something with the remote it could be a lot of things really.  If a connection comes loose either on the transmitter or receiver or has a bad solder joint that intermittently breaks then that can cause the VESC to go into whatever timeout is configured (usually brake or go to neutral) if it hasn't had a consistent signal from the receiver coming in.  Basically need to debug further though to really pin it down, it could be something related to FOC mode but I can't really say either way, would guess in general repetitive stresses and vibration can be the cause of a lot of problems.  In my case with a custom made remote built by myself with no experience designing such things I'm sure I was just putting strange lateral stresses on the potentiometers over time that they just didn't deal with well, also temp changes outside can effect resistivity of things along with any moisture etc. the hall sensors seem less prone to changes from the outside but my experience with them is more limited.
```

---
## \#5 Posted by: dareno Posted at: 2019-06-04T05:40:01.115Z Reads: 35

```
As @wafflejock has stated its probably a worn out trigger on the transmitter.  When trouble shooting start with where the problem is.  Intermittent response from the transmitter then try a different transmitter because other wise you tie yourself up in knots trying to find it.  If you put some sideways pressure on the trigger does it come back in?  I have had this happen a few times
on trigger remotes after extensive use.
```

---
## \#6 Posted by: sash Posted at: 2019-06-04T05:49:27.201Z Reads: 34

```
@wafflejock @dareno Thanks again for suggestions.    I was also thinking that trigger might be a possible reason.  Going to try to pin it down.
```

---
## \#7 Posted by: Jinra Posted at: 2019-06-04T06:42:09.860Z Reads: 31

```
as @wafflejock said, check for faults, should be your go to for any vesc related issues, barring anything obvious externally. 

VESC has a behavior where it wont accept input until it reads neutral PPM for a certain amount of time (very quick). So if the VESC is rebooting, for instance, it will not accelerate or brake if your throttle was in a non-neutral position when it boots up.
```

---
## \#8 Posted by: dareno Posted at: 2019-06-04T08:06:12.019Z Reads: 26

```
Good point and would also be the case for a physical problem.  A worn potentiometer would display the same characteristics.  Non neutral.  Actually check the trim buttons on the throttle channel.  Might be something simple.
```

---
## \#9 Posted by: sash Posted at: 2019-06-04T14:55:20.366Z Reads: 14

```
[quote="Jinra, post:7, topic:95800"]
VESC has a behavior where it wont accept input until it reads neutral PPM for a certain amount of time (very quick).
[/quote]

This sounds exactly what might be happening in my problem.   Going to check for VESC faults.
```

---
