# Idea - Joy-Con Controller

### Replies: 3 Views: 138

## \#1 Posted by: Airo Posted at: 2019-11-26T21:53:54.263Z Reads: 31

```
Hey there!

I'm new here and try to figure out how to build my first E-MTB.
Because there is no controller I really like, I started a project for my own controller based on a Nintendo Switch Joy-Con. I have never done anything like this before, but I have a plan of how I want it.
Joy-Cons have built-in bluetooth, so I hope it can be paired with a bluetooth receiver.


![Esk8_Joycon|690x422,75%](upload://A9mWTgLh42BGfhIYAgsyQ2qB6UU.png) 

There is a Joystick for acceleration and brake. R button is used as "dead man button".
With Buttons B and X I want to switch between modes (e.g. increasing/decreasing maximum speed). With Buttons Y and A I want to switch the lights on/off.

SR and SL button are optional. I think there will be additional mechanical brakes if the motor brakes are insufficient (and for a higher chance to use this thing legally on the road).

This will take a lot of time and I'm not sure if I can finish it in a reasonable time.

What do you think, is this possible to do?

Did anybody try something similar and can share experience?
```

---
## \#2 Posted by: Benjo Posted at: 2019-11-26T22:57:48.855Z Reads: 27

```
Hey! It is definitely possible but I would consider it a bit tedious for what you will get. Are you at least decent at programming microcontrollers?
First you need to figure out how to pair the Joy Con with lets say an arduino with integrated bluetooth or a shield. Then you can reverse engineer the protocol that the controller uses. Then you can connect the arduino via uart to a VESC and send it commands (have to figure out the protocol as well, but that should be documented somewhere).

There already exists a solution for an older wii controller, but it completely swaps out the hardware of the thing: https://www.electric-skateboard.builders/t/vesc-nunchuk-rf/588
But the associated software is a good reference.
```

---
## \#3 Posted by: venom121212 Posted at: 2019-11-27T00:04:23.100Z Reads: 24

```
The throw on the joycon thumbstick is sooo tiny. I feel it will give you a bad acceleration curve. Mini remotes are like $20-25 regularly and are rock solid. Black Friday is coming up too.
```

---
