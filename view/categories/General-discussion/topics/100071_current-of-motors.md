# Current of motors?

### Replies: 6 Views: 157

## \#1 Posted by: Jonisonvespa Posted at: 2019-08-10T23:50:45.412Z Reads: 67

```
hi 
i saw a list somewhere here of different motors and how much current they draw, can someone pleased show me where it is thanks
```

---
## \#2 Posted by: Saturn_Corp Posted at: 2019-08-11T00:06:57.595Z Reads: 66

```
Motors will have listed max watt ratings like 2500 or 4000 or 1500 or what have you. Multiply your battery voltage by however many amps you want to put through it and resulting number is the wattage.
```

---
## \#3 Posted by: Jonisonvespa Posted at: 2019-08-11T00:09:10.120Z Reads: 66

```
a bit confused, im trying to work out what bms to get for my 12s 5p battery im trying to buy the biggest motors i can get either 230 or 270 kv i intent to have two motors, and a bit unsure on what VESC to get as well though id get 2 of these which should be enough.

https://flipsky.net/collections/electronic-products/products/flipsky-fsesc-6-6-based-upon-vesc%C2%AE-6-heat-sink
```

---
## \#4 Posted by: Saturn_Corp Posted at: 2019-08-11T00:21:42.833Z Reads: 54

```
You might have issues with motors over 190kv on 12s. I'm assuming samsung 30q battery so that's 100 amps total output. Split that between motors for 50 each. That leaves you with around 2500 watts you can give to each motor so anything with that or higher will do you well. Those vescs are rated for 60amps so hopefully they won't blow up if you're giving them max power. Flipsky's rep is pretty good.

BMS I think you can bypass for discharge but I'm far from an expert on putting together batteries so ignore my advice there.
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-08-11T01:42:03.077Z Reads: 46

```
@Jonisonvespa  Any motor you buy will have numbers on the page of the seller telling you the maximum wattage/voltage/current. These numbers can be fudged to a significant degree either direction, but they're a good starting place.

Motors are passive devices - there's nothing inside other than wire and magnets. The more current (and power) you run through them, the hotter they will get. With this in mind, if you're not running them continuously up a miles-long hill, you can drive them significantly harder than their continuous rating for short periods of time without any ill effects. The main thing to keep an eye on is the temperature - don't exceed 80*c or so, or you'll start to cook the magnets.

I really wouldn't recommend 270 (or even 230)KV motors for 12s - they just spin too fast, which can cause issues for the motor controller, and you'll also need more gear reduction to keep from having a top speed measured in mach numbers. I'd say 170 or 190 KV is ideal, maybe up to 200 in a pinch.

Keep in mind also that battery amps (The amount the battery/BMS can put out) does not necessarily equal motor amps (the amount going through the phase wires of the motor). The ESC can act like a step-down converter, converting for example 50A at 50V from the battery to say 100A at 25V to the motor when the motor isn't spinning super fast. (The motor current is highest at low speed, the battery current is highest at high speed.)

In general a 5065 motor is good for ~40-50A. A 6355 motor is fine for ~60-80A, and A 6374 is good for ~80-100. (This all also depends on the KV, and the quality/manufacturer of the motor, and the amount of cooling it has, and and and.) In general the bigger and heavier a motor is, the more current it can handle. 

So between a cheap 800g 6374 and a more expensive 1200g 6374 (I'm pulling numbers out of my ass), the heavier one will win.
```

---
## \#6 Posted by: Jonisonvespa Posted at: 2019-08-11T09:58:51.744Z Reads: 30

```
Ok will go for a 6355 190 kv motor
Will that vesc be ok?

Think will definatly need a bms as letting voltaged go too low on a 18650 could damage it, also if you  reduce the min voltage and max voltage of the cell greatly increases the lift of it 

Thanks for the help
```

---
