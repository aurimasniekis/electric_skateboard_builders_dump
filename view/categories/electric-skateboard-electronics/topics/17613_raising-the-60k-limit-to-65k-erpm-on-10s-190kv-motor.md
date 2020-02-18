# Raising the 60k limit to 65k ERPM on 10S 190KV motor

### Replies: 11 Views: 999

## \#1 Posted by: Eboosted Posted at: 2017-02-12T22:29:26.868Z Reads: 199

```
I've decreased the motor pulley from 16T to 13T, my wheel pulley is 36T.

My top speed is 35Km/Hr, I really miss my old 42km/Hr, how safe would be to increase the max ERPM from 60k to 70k?, if I do it should the battery be discharged exponencially?
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-02-12T22:31:30.010Z Reads: 198

```
The max ERPM of 190kV and 10S is well below 60k so changing your max ERPM on the VESC will have no effect.
```

---
## \#3 Posted by: Eboosted Posted at: 2017-02-12T22:54:23.515Z Reads: 192

```
Thanks man!
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-12T22:56:33.318Z Reads: 185

```
Whats your Motor and Motor max and Batter max settings?
```

---
## \#5 Posted by: Eboosted Posted at: 2017-02-12T23:03:54.348Z Reads: 180

```
Hey Nico, these are the settings

[img]http://i.imgur.com/f8YgBaN.jpg[/img]

I have even increased the Start Up Boost from 0.03 to 0.05
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-12T23:07:22.088Z Reads: 170

```
Do you have a dual setup and a 10S4P. Sorry i guess you told me already multiple times but there are so many here that i give advice.
And what did you want to achieve by going down to 13 teeth.
```

---
## \#7 Posted by: Eboosted Posted at: 2017-02-12T23:19:21.568Z Reads: 169

```
No problem, it's all good you help a ton of people! 

Yes I have 10S4P with Samsung 25R, I also have an Evolve Bamboo and the acceleration on the Evolve is way faster it has noticeably more torque, I'm guessing it's because of the smaller motors as well but if I could add more torque on low speed it'll be awesome.

With a 13T pulley I'd like to get more torque but I'm pretty sure I'll loose even more topend, I might have to go with a 12S setup to get more final speed.h
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-02-12T23:34:53.876Z Reads: 165

```
16/36 gearing is a little high. 15 teeth would be better.
But first you should try to set your Motor max to 80 Amps. That will already give 33% more power at low speeds.
You could also go with 100 amps but that would be on your own risk. But i think that would work as well.
If you like more braking power then raise the motor min to -80 and set the battery min to -10 (could only be reached at high speeds for a short moment so it doesn't really harm your cells).
```

---
## \#9 Posted by: Eboosted Posted at: 2017-02-13T03:47:18.989Z Reads: 146

```
Thanks Nico, don't get me wrong, my board is runing pretty amazing at the moment. I can't believe I have applied so many any tune ups and tricks to customize it as I wanted, every mod you suggested has been spot on.

I'll raise motor max right now from 60A to 80A and see how it performs, I'll keep you updated, not sure how would the motor get so many amps as the 10S4P only has a 80A discharge capacity, 40A for each motor/VESC, but I trust on your recomendations always so I'll do that.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-02-13T07:27:19.419Z Reads: 131

```
That's PWM (pulse width modulation) 
When you are for example at 10% duty cycle then the motor is at only 10% of the batterys voltage. But at the same time the battery is at only 10% of the motors amps. 
So at 10% duty cycle and 40 battery volts and 8 battery amps the motor is at 4V and 80 Amps. 
The faster you go the higher the duty cycle gets and the closer the volts and amps come together.
```

---
## \#11 Posted by: Eboosted Posted at: 2017-02-14T05:23:31.347Z Reads: 109

```
So, right now the setting for each VESC, master ad slave, is Motor Max = 60A and 40V of battery, at 10% DC I'll have 6 * 4 = 24 Watts of power, at 100% DC 2400 Watts. Max Watt has been restricted to 1300 Watts on master VESC.

If I raise motor Max to 80A (on each VESC), at 10% DC I should be getting 8 x 4 = 32 Watts (33% more torque), at 100% DC 80A * 40V = 3200 Watts!!!, Is this the total power for each motor, or should I split this between the two motors and just raise the Max Watt to 1600 watts?
```

---
