# What happens if a motor wants more constant current then the VESC can handle?

### Replies: 10 Views: 261

## \#1 Posted by: Achmed20 Posted at: 2019-07-30T09:47:19.634Z Reads: 90

```
Lets take an old vesc 4.12 as example.
peak current is something about 240A as far as i remember and constant current is 50A.

what would happen if (for whatever reason) the motor wants more then 50A over a longer time. will the VESC limit it by itself or will is just burn out sooner or later?
```

---
## \#2 Posted by: Andy87 Posted at: 2019-07-30T09:52:22.903Z Reads: 89

```
the motor does not want. the vesc always give.
it´s all up to the settings you put in the vesc while setup.
```

---
## \#4 Posted by: Achmed20 Posted at: 2019-07-30T14:43:06.267Z Reads: 73

```
i am fairly certain that a motor "draws" current! you are talking about voltage.
Otherwhise the current protection boards on stepper drivers wont make much sense. its just there to protect the driver from more current then it can handle. and a stepper motor is pretty much the same thing like a phases motor, just has more phases. and loading a motor results in more current use.
thats even true for dc motors hooked up directly to a powersource.

edit: Electroboom video proof: https://youtu.be/yO9xIVv8ryc?t=400
```

---
## \#5 Posted by: rich Posted at: 2019-07-30T18:28:43.744Z Reads: 55

```
You can draw more than 50A but not for a long time. Like @Andy87 said it's all about the settings like motor max and batt max. 

BTW 50A cont. from battery is not realistic, above 27A the vesc 4.12 gets hot, but don't mix this with motor amps.

And no the vesc won't burn because of the temp cutoffs.
```

---
## \#6 Posted by: wafflejock Posted at: 2019-07-30T18:30:54.223Z Reads: 53

```
Eh sort of, a motor has windings in it that are just wires with a set resistance if you apply a voltage (charge potential difference) to each end of the wire then current flows through it.  How much voltage is applied is controlled by the VESC in this case by opening/closing the gates of the MOSFETs.  Vid there is referencing brushed DC motors which work differently from Brushless DC (BLDC) motors.

A DC motor with a set resistance will have a set current flow through it given the same voltage, and so will "draw" or use a certain amount of power (Watts, amps times volts) at a given voltage.  The VESC or any sort of speed controller adjusts the voltage applied to the motor and in the case of Brushless DC which coils are energized to get/keep the motor spinning.
```

---
## \#7 Posted by: Achmed20 Posted at: 2019-07-30T18:49:44.256Z Reads: 46

```
[quote="rich, post:5, topic:99389"]
And no the vesc won’t burn because of the temp cutoffs.
[/quote]
perfect, that was pretty much what i was looking for.

PS: i know that it is unrealistic, but i am a sucker for details, whats why im asking.
```

---
## \#8 Posted by: Achmed20 Posted at: 2019-07-30T18:56:45.005Z Reads: 43

```
[quote="wafflejock, post:6, topic:99389"]
Vid there is referencing brushed DC motors which work differently from Brushless DC (BLDC) motors.
[/quote]
i see coils and magnets and some mechanic (the brushes) that powering individual coils to make the motor spin by creating magnetic fields. so the only thing different is the ESC which handles the "brush" part. care to elaborate where that is different? from a physics stanndpoint i mean.
```

---
## \#9 Posted by: wafflejock Posted at: 2019-07-30T21:21:54.519Z Reads: 34

```
Yah didn't mean to say they are electrically much different, just that the video is explaining a different kind of motor from the ones we're typically using.  Any coil with current going through it is going to act as a solenoid, guess the major differences with BLDC vs brushed DC are the greater efficiency of BLDC and faster switching rate for given RPM needed for smooth operation of BLDC motors.
```

---
## \#10 Posted by: Andy87 Posted at: 2019-07-31T05:28:06.324Z Reads: 23

```
[quote="Achmed20, post:4, topic:99389"]
motor “draws” current
[/quote]

yes a motor draw current.... 
but if your current draw is limited by the vesc software...
how ever, i think you got your answer anyway.
```

---
## \#11 Posted by: deucesdown Posted at: 2019-07-31T14:50:28.652Z Reads: 14

```
The principal of operation of brushed motors and bldc motors is very different.

Brushed DC motors, you just apply voltage (with 2 wires) and they go. The rotation of the motor physically determines which brushes are in contact with which coils. No control electronics are required. As you said, the motors *draw* power.

BLDC motors on the other hand have 3 phases, and applying DC voltage to them will do nothing. They need a smart controller to feed power to the 3 phases in a very specific way. This speed controller will have pretty much total control over the power the motor can use. The default mode in vesc is called "current control", and that's exacly what it does.
```

---
