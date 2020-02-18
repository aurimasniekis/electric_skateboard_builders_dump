# The Difference Between Motors Commutation BLDC vs (FOC Trapeziodal / Sinosuidal)

### Replies: 17 Views: 20748

## \#1 Posted by: laurnts Posted at: 2016-05-08T16:17:49.298Z Reads: 1339

```
I know alot of members are still confused the real difference between FOC and BLDC mode within their VESC or any other ESC that performs such commutation. What are known to most are FOC mode is much more quite than BLDC mode which is true. I am personally not an electrician, just normal person like all of you and I am going to tell you by diagram below the differences.
<br/>
<br/>
<br/>
**BLDC Commutation**<br/>
<img src="/uploads/db1493/original/2X/0/0754714e43c2699ec482da6740c2a82e42141f62.gif" width="441" height="366">
<br/>
<br/>
<br/>
**BLDC Trapezoidal Commutation**
<img src="/uploads/db1493/original/2X/2/2d20428795586315c7f2b434013f60388270e3b7.png" width="410" height="271">
<br/>
<br/>
<br/>
**Sinusuidal Commutation (FOC)**
<img src="/uploads/db1493/original/2X/c/cb73679ef87f3d677b1524a4b61a164f96e08448.jpg" width="422" height="344">
<br/>
<br/>
<br/>
---

**So what these people are calling their commutations are based on the diagram of the motor current output.** BLDC is simply fast switching phases On and OFF, while trapezoidal and sinusoidal has no switching but modulating the phases.

**Since there is no high current fast switching within FOC mode, there is simply no high pitch sound you usually hear from BLDC commutation.**

**Logically since FOC is modulating the phases, it maximizes the torque output at any point** due to that the ABC phase are always charged and each of them are using only as much as what do they require for each rotor position within the motor.

Logically since sinusoidal control are creating smooth wave form instead of spikes like BLDC and Trapezoidal, the peak point of each amplitude is less than BLDC mode and or trapezoidal mode. **Therefore it has slightly less top speed.**

Within FOC Sinusoidal commutation when each ABC phases are electrically being given what exactly they need on what ever rotor position / stator position they have, **it does make sense that they run more efficient.**

---

In general this is what I understand as a beginner. I might be wrong on certain things, but the general explanation in performance factors and diagrams are surely why they are named after each other. I hope others / members could grasp the idea.
```

---
## \#2 Posted by: Bender Posted at: 2016-05-08T19:45:43.954Z Reads: 1151

```
Thanks for that info
I'm trying to wrap my head around it and this certainly helps
Pictures (graphs in this case) make it easier to understand
```

---
## \#3 Posted by: onloop Posted at: 2016-05-09T02:57:04.300Z Reads: 1101

```
GREAT INFo!.... well done, nice & simple
```

---
## \#4 Posted by: evoheyax Posted at: 2016-05-09T04:44:41.393Z Reads: 1051

```
A some, will link this in the VESC guide I wrote :)
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-07-14T14:25:03.535Z Reads: 708

```
Ok this makes more sense now. 

Except one thing is bugging me. How does the mosfet do anything other than ON and OFF? I think what's happening here is the mosfet is simply adjusting its switch timing according the curve instead of a more linear fashion. Does that seem right?

I have a tendancy to think literally so i get hung up on stuff like this.
```

---
## \#6 Posted by: goldenHusky Posted at: 2017-07-14T14:57:47.487Z Reads: 658

```
Yea, pretty much.
BLDC is simply switching on and off (classic 6-step commutation), in FOC the Mosfets are also switching on and off but the algorithm behind is different. So in FOC the voltage vector must reach all positions (changing angle and length of the vector) to enable the FOC benefits, while BLDC has only 8 positions on a fixed length (each Mosfet can be on/off, so there are two states and we have 3 halfbridges so total possibilities are 2^3=8  --> 6 useable and 2 where all 3 motor windings are shorted to + or -).

In the gif below you see how two vectors U1 and U2 create a new, desired vector Ua, by powering 2 windings half of a period each, because of that 50/50 ratio, the new vector has its angle exactly in the middle of the two "parent" vectors. The principle is similar to PWM but with angles instead of voltages.

https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/Raumzeigermodulation_zeigerdiagramm_animation-1.gif/330px-Raumzeigermodulation_zeigerdiagramm_animation-1.gif

So now the angle can be adjusted but the length of the vector still  needs to be modified aswell.
I wrote that there are 8 switching possibilities of the Mosfets, on two of them the motor windings are shorted, so there is no voltage drop on the windings. The other 6 switching possibilities can now be held in a ratio with the ones that provide 0 voltage (PWM principle again) and by varying this ratio of voltage/ non voltage the length of the vector can be adjusted.

So in BLDC the vector rather jumps in 45° degree steps (360 divided through 8 switch states) and FOC allows the vector to move around the origin-point in a nearly stepless circle. Of course the math behind is much more complex than in BLDC.

My diploma thesis was about that stuff. You can read all this on wikipedia, I just tried to shorten it and to explain it in a more practical way.
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2017-07-14T15:06:53.138Z Reads: 568

```
ahhh it looks like linear transformations im scared =(
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-14T15:12:49.765Z Reads: 558

```
Could that contribute to why FOC blows up standard VESCs like nobodies business? Since it now switches at a much higher frequency (by my undersatnding) than bldc?
```

---
## \#9 Posted by: goldenHusky Posted at: 2017-07-14T15:26:14.010Z Reads: 554

```
[quote="trancejunkiexxl, post:7, topic:3002, full:true"]
ahhh it looks like linear transformations im scared =(
[/quote]

The FOC algorithm uses Park and Clarke transformations.. some years ago I thought Laplace and Z- transformations were difficult but suddenly this hits you lol :joy:
```

---
## \#10 Posted by: goldenHusky Posted at: 2017-07-14T15:32:37.802Z Reads: 535

```
@Jinra Yes, the high switching frequency is needed to get greater efficiency and a more quiet motor. The switching frequencies in FOC are usually around 20-40 kHz, interestingly, above around 60 kHz the switching losses caused  are bigger than the gained advantages because increased switching frequency decreases drive efficiency. But this usually very dependent on the system (motor inductance etc.)
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-14T15:34:28.497Z Reads: 516

```
Thanks! By comparison, what's the average switching frequency of BLDC 1KHz~?
```

---
## \#12 Posted by: goldenHusky Posted at: 2017-07-14T15:41:15.624Z Reads: 497

```
The ideal switching frequency for each motor can be calculated with a formula dependent on L/R. Usually (at least what I always did) was selecting it as high as possible to reduce noise in the audible frequency range, so usually between 14 and 20 kHz but he BLDC drivers limit you anyway..:sweat_smile:
```

---
## \#13 Posted by: trancejunkiexxl Posted at: 2017-07-14T15:53:43.498Z Reads: 477

```
more about noise reduction i get alottt of chatter, feel like im riding on a westell 56k modem.. i assume just experiment with 14 to 20, is it bad to operate 20khz constantly
```

---
## \#14 Posted by: goldenHusky Posted at: 2017-07-14T16:02:10.349Z Reads: 470

```
[quote="trancejunkiexxl, post:13, topic:3002"]
is it bad to operate 20khz constantly
[/quote]

If the bldc pre driver is designed and rated for 20 kHz and if there is a proper external wiring (short traces and stuff), I don't see why it should be bad.
```

---
## \#15 Posted by: trancejunkiexxl Posted at: 2017-07-19T00:38:13.071Z Reads: 455

```
 bldc mode fails for me when you gun it, but in FOC if try to force torque  at any particular moment the motor will just screetch if the load is too great. having just switched back to BLDC and ate it really bad (motor full hault), I dont feel as safe as in FOC, where I can build up speed safely with a feeling that there is better motor control to avoid stressing(there is an audible noise under load) and can better avoid this and abrupt vesc shutdown.
```

---
## \#16 Posted by: gchenfc Posted at: 2019-04-24T03:39:52.721Z Reads: 126

```
This page is one of the first results that pops up on Google when searching the difference between FOC and sinusoidal but I think, while well intentioned, there's some issues that warrant clarification.

1) There is no such thing as "trapezoidal FOC" or "Sinusoidal FOC" (as far as I'm aware).  Trapezoidal control is what you seem to refer to as "BLDC commutation".  Although VESC tool refers to trapezoidal control this way, I think most EE's would be confused by this term as it's almost universally referred to as trapezoidal control.

2) The difference between trapezoidal and sinusoidal/FOC is that, in sinusoidal/FOC, you generate a "smooth" current waveform which creates less torque ripple and noise.  In contrast, trapezoidal generates some strange shaped current waveforms.  In theory, a lot of people draw them like modified square waves but in practice I usually find that they look more like curly "w"s.

3) The difference between sinusoidal control and FOC is that sinusoidal control controls phase current whereas FOC applies coordinate transformations to control "direct" and "quadrature" current.

Allow me to make a more organized comparison:
There are 3 primary methods of BLDC motor control:

1. Trapezoidal - this is the easiest.  It's just a lookup table: for some hall sensor reading, apply a high voltage to one phase, low voltage to another phase, and float the third phase.  Which phase gets what depends on the hall sensor readings.  laurnts got this mostly correct.  It only changes every 60° (I think he mistakenly said 45° but more or less the right idea.  The reason there's only 6 states and not 8 even though there's 8 possibilities for 3 binary values is because two possibilities: 000/111 should never occur).
2. Sinusoidal - this requires a continuous rotor angle estimate so rather than just knowing within 60° what the rotor angle is, you need to actually know exactly how many degrees the rotor angle is.  Then, it's basically a "look up table" again where, whatever the rotor angle is, there's a specific current that each phase should be at and you try to make the currents match what they should be.  The "look up table" in this case is actually just a sine function shifted in time.
3. FOC (also called flux vectoring and variants of that) - laurnts actually got this pretty close to correct.  You also need a continuous rotor angle estimation here.  You use that in the Park transformation.  In FOC, first you transform the 3 measured phase currents into a 2D representation using the Clarke transform (yes, linear algebra but it's super simple I promise).  Then, you transform these into a rotating coordinate frame with the Park transform using the rotor angle.  This gives you a d and q component of the current (direct and quadrature).  The q component represents the current which produces motor torque and the d component is the "flux" component.  For now, we can just pretend the d current is "wasted" power.  In actuality it becomes important for something called field weakening, but many motor controllers don't implement this because it can cause states that are impossible to recover from without breaking your electronics if you aren't careful.  Anyway, in FOC we try to make the d current = 0 and make the q current = some user controlled value.  To do this, we apply voltages in the d and q directions, use the inverse Park to get back to a non-rotating reference frame, then use the inverse Clarke to get to the three phase wires and finally we have the voltage we need at the three phase wires.  Also I'll quickly mention that the Clarke, Park, and their inverse transformations are actually really simple - just a couple multiplications and divisions and a sine/cosine here and there.  Compared to Laplace and Z-transforms, they're easier than cake.

Now as for "commutation" vs "PWM", there's some misunderstandings here.  Almost every motor controller will use PWM.  PWM just means, if you have a 10V battery but you need 5V, the way you do it is by turning the MOSFET on half the time and off half the time and switch on/off really really fast..  On average, you get 5V.  Trapezoidal control uses PWM so that you don't have to go full throttle all the time.  Sinusoidal and FOC use PWM to generate their roughly sinusoidal voltage waveforms which in turn generate roughly sinusoidal current waveforms.  The difference between trapezoidal commutation and the other two is that trapezoidal commutation only changes voltages every 60° whereas sinusoidal and FOC is changing voltages continuously, but they all use PWM to generate voltages smaller than the battery voltage.

Finally, the last thing which wasn't discussed in laurnts post but which I think is maybe what he was getting at calling trapezoidal FOC is the types of sensors you can use to apply these control schemes.  There's 4 main ways to sense rotor position:
1) sensorless - you can read the back-emf of the phase wires to figure out the position of the rotor.  Generally you get 60° resolution and it's offset from the proper trapezoidal commutation by 30°.
2) hall sensors - you get 60° resolution and it matches up correctly with the proper trapezoidal commutation.
3) encoder - usually black/white lines and a light sensor that allow you to measure the rotor position to within, say, 1/4096 of a revolution.  Some are better some are worse.  With a bit of coding, these can give you the rotor position to within the resolution of the encoder.  There also exist magnetic encoders, potentiometers, and probably some other encoders I'm forgetting about.
4) resolver - I don't totally understand how these work but it's some magic with injecting a current and measuring the magnetic response or something weird like that.  These are incredibly robust and accurate but they're ridiculously expensive and difficult to install.  Almost certainly out of the range of hobbyists.

**Any 4 of these sensor methods can be used with trapezoidal, sinusoidal, or FOC!!!**  Though if using 1 or 2 for sinusoidal/FOC, you need to do some coding/math to extrapolate the rotor position in between the 60° resolutions.

In addition to rotor angle sensing, sinusoidal and FOC also require phase current sensors.  These are usually pretty straightforward and inexpensive to include on a motor controller.

Regarding practical implementation considerations, FOC will always be superior if it has perfect PWM and perfect angle estimation, but PWM in the real world causes losses/noise and angle estimation is heavily dependent on the sensor you're using.  If you don't have any sensors (sensorless) or use hall sensors, FOC will probably be pretty bad at low speeds because extrapolating position at low speeds from the 60° resolution of these methods is pretty hard.  Stick with trapezoidal at low speeds if you have hall sensors.  If you're running sensorless, you need to run in "open loop" at low speeds but I'm pretty sure benjamin has already handled the hard work for you if you just use "sensorless" in the BLDC tab (I'm skeptical of sensorless and hall FOC at low speeds, I don't use FOC unless I have an encoder).  If you're using an encoder, FOC should be superior at any speed unless the motor control hasn't been coded optimally (but the VESC firmware is coded very well).


So, to sum up, there are 3 primary BLDC motor control schemes: trapezoidal, sinusoidal, and FOC.
All of these control schemes use PWM (though technically trapezoidal doesn't require it, it's almost always used to give throttle control as opposed to just on/off).
Each of these control schemes can use sensorless, hall sensor, encoder, or resolvers methods to detect rotor position, but in practice sinusoidal and FOC are pretty crap without an encoder or resolver.

*edit: by the way, in terms of my qualifications, I'm about to finish my undergrad as an ECE major and I handle the electronics for the [Duke Electric Vehicles](http://duke-ev.org) team so I work with BLDC motors extensively.  Feel free to reach out to us on our website, [Facebook](facebook.com/DukeElectricVehicles), or email (dukeecomarathon@gmail).*

I hope I was able to set the record straight on some of these terminologies and help people figure out the differences between the different control schemes.
```

---
## \#17 Posted by: laurnts Posted at: 2019-04-25T11:57:31.464Z Reads: 92

```
Such a great explanation! At the time I was writing this, it was nothing much in the science behind it. It was simply me trying to explain why BLDC is louder than FOC mode. There were tons of member asking the difference between BLDC and FOC mode (that also because at that time VESC aren't that reliable on FOC mode).
```

---
