# \[SOLVED\] Problem, VESC motor rotation direction switching during ride and lock-up

### Replies: 6 Views: 333

## \#1 Posted by: SimosMCmuffin Posted at: 2019-07-12T11:13:53.538Z Reads: 71

```
Got finally my new rear end assembled (new motor mounts and drivetrain) and went out for a test ride, got about 200 meters from my door when testing out my brakes it seemed to lock-up my other side motor. Rolled to a stop and noticed that the direction of my other motor was changing it's forward rotating direction (using only forward and brake, no reverse), so clearly there is something weird going on, but I haven't seen or heard of this before.

I then re-detected the motor through the VESC tool, but results we're identical to earlier detected motor values.

I then went out again and I was able to get the problem to appear again before setting off, so I shot this little video reproducing the problem.

https://youtu.be/RqwwTB-q8GI

**NOTE**. when the motor starts running in the wrong direction it has a lot harsher whine to it, then compared to the correct direction.

The lock-up might be explained with that if you coast for a moment and then try to accelerate or decelerate and the VESC for some reason thinks the motor is running in the wrong direction and therefore locks it. Only happened when acceleration or deceleration commanded. Coasting didn't have any problems.

**Background and possible leads:**

Broke one of my motor mounts couple of weeks ago. Motor did take some hard knocks as seen by the scuffs on the bell, but I straightened the bell on the axle so it wouldn't grind on the stator teeth, so there can be possibly damage in the motor leads, except that if there was a short between 2 phases the motor would bind constantly and I don't expect it to turn as well as seen on the video.

Other possibility is that the drive stage of the VESC took a possible spike when the motor ripped off, but I then proceeded to ride to work and back on a single setup using the VESC from the broken mount side, as shown below. I didn't change anything else for the single running except increase motor and battery currents to get going with a single motor.

**One thing I did notice** though after the motor had snapped off and I had stopped, looked at the situation, cleaned up and attempted to limp ride myself back home with the now single left side Slave VESC's motor is that it kept juttering/stuttering under acceleration and braking and was not able to keep going. Now whether this was caused by the right side Master VESC losing it's motor which then caused it to "freak out" and command all the Slave VESCs weirdly because it didn't have a motor connected to it.

![IMAG0313|690x389](upload://vXXf6srwdbBaLr8iha9hXkun6TI.jpeg) 

**Summary:**

Personally it would seem to be something with the VESC settings, because if the motor leads were short circuiting it probably shouldn't even commutate properly, or there should be clear indications of the leads shorting from vibration if the phase insulation was nicked slightly with sharp stutters. The VESC HW itself also seems to be good, as if it was a HW problem I doubt it would commutate reliably at all or detect the motor with identical settings.

I'm gonna try switching the motors around and seeing if the problem does or doesn't move with the motor.

Otherwise all questions, suggestions and theorycrafting are welcome at this point.
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2019-07-13T17:43:58.567Z Reads: 57

```
After some research and testing I conclude that the behavior is caused by one of the motor phases disconnecting or being intermittent. Tested with the normal side, by unplugging one of the phases and it started to also exhibit that reversing direction behavior on start-up.

I have actually had this happen to me twice before. Once when one of the phase wires had un-plugged itself during a ride from vibration. After that I added an extra heatshrink on top of the banana plugs to bind the plug & socket together. Then couple weeks later, one of the phase wires cracked at the solder joint causing intermittent phase connection. I re-did the solder jobs on both sides after that.

Now I did check and re-do both sides' soldered connections, but on the surface they both looked okay, so one of the phase wires might be cracked inside the motor itself from the jerk/hit when the motor fell off with the broken motor mount. I'll leave the "uncertain" motor's side's belt a little looser for a test ride, so if it starts getting intermittent then it'll just allow the belt to skip over the teeth and lessen the jerk from it.

Gotta order new motor if the phase lead is indeed cracked inside the stator itself.
```

---
## \#3 Posted by: b264 Posted at: 2019-07-16T23:01:37.800Z Reads: 45

```
Are you sure?  I read this on the new builder forum and thought of you.

[quote="wafflejock"]
don’t set your Regen amperage to a positive number or very strange things start happening. Board accelerates when hitting brakes, and goes backwards seemingly randomly when pulling throttle… Do not recommend
[/quote]

https://forum./t/pollution-and-the-myth/4395/77?u=b264
```

---
## \#4 Posted by: trampa Posted at: 2019-07-17T01:40:14.201Z Reads: 32

```
That's a metr.at app issue. Vesc-Tool will set a negative value.
```

---
## \#5 Posted by: wafflejock Posted at: 2019-07-17T19:10:22.024Z Reads: 19

```
Good to know would be nice if the VESC firmware handled setting this negative or responding with an error if possible and leaving the value unchanged.  Guess question is, is there any use case for positive Regen values ever?
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2019-07-18T06:56:22.154Z Reads: 13

```
I think I found where the intermittent connection was. It wasn't in the motor's phase wires, but on the ESC side of the banana/bullet connectors. 

I was doing some maintenance and pulled on the phase wire and it split in two about halfway between the banana/bullet connector and the VESC. The wire was high strand # silicone wire, so it is very flexible by nature, but all the strands had broken quite neatly at one point. I suppose it could be that the solder had wicked itself up the strands from the bullet connector and then caused a stress spot that had then over time started to fatigue due to vibration and ride impacts.
```

---
