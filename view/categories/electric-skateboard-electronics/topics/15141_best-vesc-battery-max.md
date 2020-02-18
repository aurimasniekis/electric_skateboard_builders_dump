# Best VESC battery max?

### Replies: 17 Views: 4684

## \#1 Posted by: NickTheDude Posted at: 2016-12-24T02:41:34.061Z Reads: 539

```
So it seems (for most setups) in terms of amperage the VESC is our bottleneck. So what is the best battery max amps for longevity and reliability while maintaining maximum power? Does it depend on the quality of the VESC you have and therefor vendor? 

Just curious what you guys though about this. Currently I'm running dual motors with both set to 20A.
```

---
## \#2 Posted by: michaelcpg Posted at: 2016-12-24T03:13:52.701Z Reads: 534

```
Largely depends on your battery configuration
```

---
## \#3 Posted by: LukeL Posted at: 2016-12-24T03:37:13.294Z Reads: 520

```
I am using 5Ah lipos with 25C constant (35C peak) discharge rating, currently have vesc battery max set to 60A and it works fine.

would there be any disadvantages to increasing this if the battery can handle output of 125A?

Is there a point where it could damage the vesc? would the vesc ever draw more than it can handle?

Do you know how this value works? does the vesc start reducing the on time of the mosfets to reduce average current drawn from the battery when it reaches this value, or is it something else?
```

---
## \#4 Posted by: NickTheDude Posted at: 2016-12-24T03:41:49.863Z Reads: 512

```
From what I've heard, the VESC's continuous limit has been measured at 23A so even with dual motors a regular 20C 5Ah lipo would easily surpass that or even a 3p of samsung 25r's.

I figured since the VESC's continuous is much lower than most batteries or motors that you would be able to use the motor max setting in order to protect the VESC.

However, I have no idea how the VESC really works so this could be a bad way of going about it  :disappointed_relieved: 

I would have imagined with a battery max of 125A you would have fried your VESC. What is your motor max set to?
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-12-24T03:45:28.248Z Reads: 483

```
motor max should be around 60amp and battery at 25amp
```

---
## \#6 Posted by: Randyc1 Posted at: 2016-12-24T04:42:01.662Z Reads: 477

```
Hi Bud,..Is 25 Battery Amps enough ??

Was watching Vedders Data Lgging Video on Youtube,.. he frequently goes over (30 Battery Amp)  when Accelerating on Flat Roads. So if he was going uphill he would probably be pulling much Higher Battery Amps ? correct?
```

---
## \#7 Posted by: Pathaim Posted at: 2016-12-24T07:34:10.887Z Reads: 463

```
i have a 10s3p samsung 25r andi set max to 40, i heard the vesc can do 50 but starts heating up around 30, 40 is enough or most stuff and is what the raptor max is set to (i believe)
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-12-24T12:14:36.758Z Reads: 446

```
You can set this relatively high. The only problem is that the Temperatur rises with more amps. But when the VESC get's too hot it regulates it self to reduce the amps that it can't overheat. When Vedder mentioned that the VESC is OK with 23A continuous then he meant that the VESC will have no overheat issues with that amps. But when we ride with the boards then the continuous Amps don't matter because we never have the same amp draw continuously.
Officially Vedder tells that the VESC can handle 240A at peaks. I wouldn't go that high but for example 60A or 80A on each VESC should be no issue. When it gets too hot it reduces the power automatically. On a single drive you can face those issues. On a dual drive with a street setup you mostly don't overheat. But most of us won't use that high values because it is too powerful and the belt starts slipping.

So in reality the temperature of the VESC is the better indicator. And of course the battery and the fuse (if existing) also limit the max battery amps.
```

---
## \#9 Posted by: LukeL Posted at: 2016-12-24T12:29:00.860Z Reads: 423

```
I have battery max set to 60A I had slowly increased it from around 40A and can definitely feel a big difference in performance. 

I think most people on here using lipos will similarly be able to pump out around 100A,  but I think the VESC should just  draw what it needs as they are a voltage source. 

My motor max is set to 60A, I don't understand why this should be different? I assume most current from battery is going through the Mosfets to the motor, I guess you could set it lower as a limit but why would you set it higher?
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-12-24T13:15:18.282Z Reads: 392

```
Because at 50 % duty cycle the motor uses only 50% of the batterys voltage. But it could create twice the amps. So even when you have set the batterys max to 25A the motor could draw 50A. So expecially at lower speeds the motor could draw more amps than the battery can provide.
```

---
## \#11 Posted by: NickTheDude Posted at: 2016-12-24T14:27:05.308Z Reads: 374

```
Thanks for clearing that up, time to tune my board up a notch :grin:
```

---
## \#12 Posted by: LukeL Posted at: 2016-12-24T14:28:48.473Z Reads: 369

```
So what is that battery max limiting? I thought it was the most the VESC would ever draw from the battery, and wouldn't the duty cycle still use the same voltage but because you switch it on/off its the average voltage (rms)  that's 50%,  same for current.

I think the high current at start up is because a lot of torque is needed so motor needs more power?
```

---
## \#13 Posted by: Ackmaniac Posted at: 2016-12-24T17:19:08.217Z Reads: 354

```
Battery Max is limiting the maximum amps the vesc is allowed to draw. And duty cycle only means how much percent of the battery volts are going to the motor. So at 10% duty cycle with a 42V battery there are only 4.2V at the motor. And the duty cycle changes with the speed. The faster the higher is the duty cycle. Because the motors spin faster the motor volts are going into the motor. And the power that goes into the motor is calculated by motor volts * motor amps. So at 10% duty cycle and 10 amps it is 42 watt. At 50% duty cycle and the same amps it is already 210 watts. And the vesc can only go up to 95 % duty cycle. So max power at 10 amps would be 399 watts.

And to have more power at low speeds (low duty cycle) you need more amps. So it is possible for the vesc to provide more amps to the motor. That is then the max motor amps value.
```

---
## \#14 Posted by: NickTheDude Posted at: 2016-12-24T17:19:46.747Z Reads: 339

```
The battery is always going at full voltage. But the motor is not, however each side has equal power. So at 50% the battery is drawing full voltage and a certain amount of amps.

Battery side 
W = V * A

Motor side 
W = (V/2) * 2x

There are 2 separate circuits at play.
```

---
## \#16 Posted by: Hummie Posted at: 2016-12-24T17:42:12.423Z Reads: 327

```
70/70 without ever a temp shutdown
```

---
## \#17 Posted by: LukeL Posted at: 2016-12-24T18:04:19.622Z Reads: 326

```
I thought the battery drives some control circuit for the mosfets, which should use very little current as mosfet gates need very little to switch on and off. then when the mosfets are on the full battery voltage is applied across the phase lines of the motor, and current would depend on coil resistance (and maybe impedance as they act as inductors)

what are the separate circuits?

why would power be equal? if two sides you mean are before and after mosfet the power would be less as you are turning the circuit on and off
```

---
## \#18 Posted by: NickTheDude Posted at: 2016-12-24T19:37:14.133Z Reads: 318

```
Honestly, I have no idea how the VESC works or what a MOSFET even does... I'm just repeating what I've read around the forums and deduced from that. Everything I've said is likely extremely simplified.

How I understand it is that there are two circuits (not sure if that is the correct terminology) one for the battery/ESC and one for the ESC/motor. The battery one has a constant voltage, and the VESC pulls amps to get a desired power figure. On the motor circuit the voltage is determined by % of no load RPM (duty cycle) and the amps are equal to the power supplies by the battery divided by the voltage determined from the speed of the motor (RPM/kV).

This is assuming that power is equal on both sides. I have no idea whether that is true not not.

Again, all of this could be complete bullshit and I'd love for someone that actually knows what their talking about to explain in more detail but this is what I've gathered so far.
```

---
