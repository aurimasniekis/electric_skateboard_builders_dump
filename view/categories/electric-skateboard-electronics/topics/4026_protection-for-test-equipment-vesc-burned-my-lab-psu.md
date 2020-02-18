# Protection for test equipment? VESC burned my lab PSU

### Replies: 4 Views: 1097

## \#1 Posted by: RideTheIon Posted at: 2016-05-30T19:12:28.973Z Reads: 115

```
Today I was making the final config changes to my dual VESC setup and I burned my power supply :disappointed:

Every time the motors brakes, the PSU would go into error mode and I had the power it off/on to reset. This was an annoyance but it was manageable.
I was so stoked to see both motors spinning that I took it to full throttle. When I inched the control back slightly, the PSU started beeping and this time it gave out a little bit of smoke. Now it is in over-current mode without anything connected.
It was only a cheap Chinese power supply (Atten 3005T) and it's maybe fixable, if some charred component is yelling replace me when I open it up.

Anyway, this is a bummer and should be avoidable with a few diodes and a resistor.
The first diode would obviously prevent the current for going back into the power supply.
The second diode would direct the current into a resistor that can take a few watts of power.
The other end of the resistor is tied to the ground, so that it would simulate regenerative braking. 

There's the double voltage drop of 1.4-2 volts that makes a dead zone, but I don't think this will cause problems. In practice, the setup would go from being powered by the PSU to an open circuit for a short while, then the simulated regenerative braking would kick in.

Has anyone made something like this or does everyone own a proper lab supply?
If you have, please share if it worked and tell us what component values you chose.

Its probably a smart idea to over-rate the diodes by at least 5x the PSU rating?

The resistor should probably be a 10 ohm power resistor to simulate the battery? 

This circuit would also be handy for the people with one-touch startup units that ramp up the current without a spark-eliminator switch. Like my last power supply, these also aren’t compatible with regenerative braking.
```

---
## \#2 Posted by: JTAG Posted at: 2016-05-30T22:11:30.614Z Reads: 94

```
The 2 diode thing you are thinking about is not going to work (if you don't want that the power supply to feed directly into the resistor). Just sketch it and you will see.

There are a few ways to tackle this problem (when not considering testing on a battery):
1) disable breaking by setting the negative battery current or motor current to 0.
2) add a big fat resistor that dissipates all energy that breaking could generate (with the caveat that it will ALWAYS dissipate this much energy, also when not breaking).
3) buy a DC load with constant voltage setting that is able to dissipate enough energy (expensive).
```

---
## \#3 Posted by: RideTheIon Posted at: 2016-05-31T08:36:18.883Z Reads: 63

```
> Just sketch it and you will see.

Already sketched it last night when the idea still seemed brilliant. 
Jep, looking at it now, if I remove the VESC from the sketch and I'm left with 2 diodes in series feeding directly into the resistor. 
If the resistor is small, almost none of the current will go into the VESC.
Damn you Kirchhoff and your silly laws :grin:

It's doable with a few current-sensing resistors, some comparators and a relay/fet-pair.
But this would require a proto PCB, some testing ect. So its not a simple hack.
Your third suggestion would probably be easier to construct than a circuit that connects/disconnects the PSU and resistor.

> 1) disable breaking by setting the negative battery current or motor current to 0.

That’s probably the best solution.

What will happen to the VESC if I only add one diode between the PSU and VESC (without any load resistors)?
Probably no braking will happen, but would it be harmful to the VESC?
```

---
## \#4 Posted by: JTAG Posted at: 2016-05-31T19:26:04.315Z Reads: 42

```
On your last question: 
The inductance in combination with the mosfet switching action (with the input caps as output) will acht as boost converter. The goal of breaking is to draw energy from the motor and feed it back into the power source (battery in the ideal case). In the situation you sketch the capacitors will accept the energy and will accumulate it. The result will be a rapidly climbing voltage across their terminals that might possibly exceed the max 60V (depending on how fast the over voltage safety mechanism catches the error situation ).
```

---
