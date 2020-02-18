# VESC: What&rsquo;s the correlation between battery and motor current?

### Replies: 5 Views: 3002

## \#1 Posted by: michaelcpg Posted at: 2016-12-24T04:03:32.969Z Reads: 291

```
This is something I've never fully understood with the VESC. The general rule seems to be that people set their motor current settings a fair bit higher than their battery settings on their VESCs regardless of whether they're using a single or dual setup.

Is there a basic formula that people generally use to determine their motor max/min settings based on the battery max/min settings?
What're the advantages/disadvantages to having a large/small difference in current limit between the battery and motor?

For example, I use a battery min setting of -7A on each of my VESCs but I have the motor min set to -20A (I think?) on each VESC. What would be the likely outcome of increasing/decreasing the motor min value and keep the battery min value the same?
```

---
## \#2 Posted by: NickTheDude Posted at: 2016-12-24T04:53:08.067Z Reads: 276

```
To preface this, I'm not trained in any of this and have absolutely 0 background in EE whatsoever. I've learned all of this from google and this forum so it could be completely wrong.

Basically there are 2 circuits going on with our electronics. The circuit from the battery to the ESC, and the circuit from the ESC to the motor. On the motor/ESC side, the ESC sends pulses of energy in a sinusoidal wave form and voltage at the motor is preportional to how fast it is spinning (rpm/kV). On the battery/ESC side, the voltage is constantly the max voltage the battery supplies. 

Because of this, voltage on the motor/ESC side will always be lower since it will never realistically reach its max no load RPM. 

The circuits have different voltages, but the total power in each one needs to be equal to the other, so the motor side has higher current.

For example if you were using 1000W of power going 20% of your motors max no load RPM with a 37 volt battery, the amps at the battery side would be 1000W/37V = 27A However the amps on the motor side would be 135A = 1000 W/(37*0.2).

So, the ratio between motor amps and battery amps changes based on RPM. 

The motor max limit is important for low RPM otherwise your motor can burn out. You should set this to whatever your motor is rated for.

The battery amp max limit is important to make sure you don't draw too many amps from your battery pack or into the VESC. From what I've seen the VESC's max continuous current is around 25A, so battery amps should be set to that unless your battery is not capable of 25 amps countinous, in which case you should set it to whatever your battery is rated for.

Again, all of this could be totally false but this is how I've understood it so far.
```

---
## \#3 Posted by: LukeL Posted at: 2016-12-25T12:43:42.190Z Reads: 225

```
I don't think you have how esc works correct, there is no AC signal for dc motors, it is like a digital wave that switches from on to off

For 3 phase (3 wires coming out) brushless dc motor the the esc is controlling 6 MOSFETs that switch on and off

these MOSFETs drive the motor phase wires to battery positive voltage, battery negative voltage and one is left floating. The MOSFETs then switch to cycle each wire through a sequence, the point of this is to drive the motor phase voltages (the voltage between each phase line) through the commutative sequence. each run through the sequence is one rotation as the coils are activated to pull the rotor round.

(look at a H bridge circuit on wiki, also note that the commutative sequence is the phase voltages with respect to each other not to ground)

at each step when a MOSFET is turned on PWM is also applied (to change average voltage and current in the coils)

I am studying EE at uni (but i am very much a student not an expert so what i am saying may be wrong)

I can't see what the battery/esc circuit could be, the capacitors smooth the battery output, there will be some dc-dc converter for the 5V receiver power and whatever circuit drives these mosfets none of which would pull as much current as the motor (probably mA) and doesn't need monitoring/limiting as the max current pulled could be calculated and won't depend on the rest of the setup (motor, batter ect).

I also don't think the way you described the power transfer is correct, you've described it like a transformer, which may give near the correct numbers as so little power is dissipated by the rest of the circuit, i imagine the motor will dissipate near 90% of the power.

the only thing i can think of why they have two different limits is something to do with the back emf which i don't know much about, i get the concept as it acts as a generator with the magnets spinning around the coils but i don't know how this effects the circuit
```

---
## \#4 Posted by: NickTheDude Posted at: 2016-12-25T14:13:30.695Z Reads: 191

```
Thanks! Yeah I really wasn't sure how exactly the "wave" of pulses worked but that clears it up. 

From what I've read about back-emf (again, probably nonsense) it's a voltage generated in the opposite direction that's equal to rpm/kV. In order to power the motor you need to apply an average voltage higher than the back-emf in order to "overcome" it. Would this mean that the power output of the motor is current multiplied by voltage supplied minus back-emf?

All I'm really trying to do is calculate the power output of the motors so I can compare setups.
```

---
## \#5 Posted by: patosai Posted at: 2016-12-27T02:41:04.635Z Reads: 178

```
Back EMF is a 'voltage source' generated by the motor when it's moving. It's a function of how fast the rotor is moving; the faster it's moving, the higher the equivalent back EMF.

If you think about it this way, when the motor has no load, it spins as fast as it can so its back EMF is at its maximum, thus less current flows across the motor because the effective voltage is less due to this high back EMF.

Now, let's say you put something really hard to turn on the rotor, so now it stops turning. The back EMF is zero since the motor isn't turning at all, and the voltage drop across the motor is at its highest. Thus there is huge current going across the motor; this is called the stall current of the motor. Since it's the highest current the motor could see, when you build motor controllers you need to make sure it can handle the stall current otherwise if your wheel gets stuck somewhere your controller blows up.
```

---
