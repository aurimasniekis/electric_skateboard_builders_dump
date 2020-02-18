# Motor turns and coils

### Replies: 8 Views: 762

## \#1 Posted by: NewbieBoardBuilder Posted at: 2017-02-06T18:40:46.657Z Reads: 82

```
A higher turn number means more wire which means more resistance which means a slower motor. So, turns is just the opposite of Kv in the sense that with turns a lower number means faster. For example, 4.5-turn motor would be considerably faster than a 15.5-turn motor.

BUT how does motor turns effect speed acceleration and torque?
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-02-07T02:31:02.329Z Reads: 62

```
Torque is a function of the magnetic flux generated from a coil wire when electrons flow through it. From general RC knowledge. Having 4.5 turns per each section on a stator would allow you to use the larger diameter copper wire as oppose to 15.5 turns. Theoretically, both motor can have the same magnetic flux levels however the 4.5 turn motor can handle more current than the 15.5 turn motor because of the wire's diameter. There is a limit on the number of fewest turns you can have before a motor no longer spins. More turns in a motor have a stronger magnetic flux giving a lower motor constant (kV) and more torque and vice versa. I just confirmed your first part, but its to get to the understanding of speed and acceleration in relation to torque.

Thinking of this is car terms to answer speed and acceleration. The rotation of the crankshaft is the torque generated to drive the wheels forward. The transmission changes that giving you speed and acceleration. Shorter gears such as a 9:1 ratio taken from the Model S, Allow the car to go 0 to 60 mph in 2.6 seconds while having a larger torque multiplication and no wheel slip. Only the motor's kV value would matter if you were running 1:1, but that's not efficient for a car.

There are many tiny things that affect your speed and acceleration.
```

---
## \#3 Posted by: wmj259 Posted at: 2017-02-07T04:08:06.528Z Reads: 50

```
Just learned about this today, Black and Decker motor specialist came into Machine Design course.

Adding bigger wire diameter would cause more current to flow through the wire.
He also spoke of how the diameter of the motor, length of the motor, type of wire, diameter of wire, # of turns, materials...... affect the performance. 
Will get back to this tomorrow.
```

---
## \#4 Posted by: NewbieBoardBuilder Posted at: 2017-02-07T23:40:14.288Z Reads: 38

```
Got anything more? You said you would come back...
```

---
## \#5 Posted by: wmj259 Posted at: 2017-02-08T00:07:58.070Z Reads: 29

```
Trying to see if the presenter can share the powerpoint with me, I now wish I asked if I could record him.
```

---
## \#6 Posted by: NewbieBoardBuilder Posted at: 2017-02-09T20:31:55.676Z Reads: 19

```
Dang it... I hope you find it. If you do PLEASE send it to me.
Can you just tell me the basics of what you remember.
```

---
## \#7 Posted by: Hummie Posted at: 2017-02-09T20:42:21.941Z Reads: 20

```
torque and speed specifically?
torque in the motor is limited more so by the iron core than the coils.  at some point the strength of the magnetic field which is being made by the coils, and then empowered by the iron, becomes too much for the iron core and it reaches magnetic saturation and further current ends up not increasing the magnetic field but turning to heat.

speed is just a function of the voltage and kv or kt which is determined by how many turns of wire there are, the kv and kt are inversely related.  

the current to your motor is more so decided by the esc.  

what are you trying to find out?

something often overlooked is you can get just as much torque or speed out of a motor and it just depends how it's wound.  it could have 33 turns of wire, and will need less amps to get that torque (but increased heat as those many turns of wire will have more resistance) or you can have few turns of wire and need more amps.  You can run a motor with these different turns of wire, with the same motor case and magnets and everything else, and get the same performance if you adjust the voltage and amps you feed it. same performance meaning same amount of heat to torque or power.  although actually if you wind it with too many coils you're going to be reducing the speed and that will decrease power as speed x torque equals power.  
  One doesnt have more torque or speed than the other, just different windings which would need different mixes of amps and voltage to get what you want generally
```

---
## \#8 Posted by: NewbieBoardBuilder Posted at: 2017-02-09T22:28:24.458Z Reads: 13

```
Thanks a lot.
```

---
