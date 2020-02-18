# Quick question about kV

### Replies: 4 Views: 404

## \#1 Posted by: NickTheDude Posted at: 2016-11-16T02:27:49.834Z Reads: 60

```
Is the average voltage being supplied to a motor by the VESC determined by rpm divided by the kV of the motor?

And then are the amps pushed out by the VESC determined by throttle in order to supply the wattage required?
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-16T02:36:35.680Z Reads: 54

```
it's more so the RPM is determined by the supplied voltage times the kv.

Second part is correct and is how current control works. Though it doesn't try to achieve a wattage, it just supplies a current until back emf matches supplied voltage.
```

---
## \#3 Posted by: jmasta Posted at: 2016-11-16T02:43:58.393Z Reads: 53

```
In general, voltage is proportional to speed, and current is proportional to torque
```

---
## \#4 Posted by: KMeyerson Posted at: 2016-11-16T03:45:45.810Z Reads: 41

```
[quote="NickTheDude, post:1, topic:13137"]
And then are the amps pushed out by the VESC determined by throttle in order to supply the wattage required?
[/quote]
@NickTheDude 

In the simplest sense, yes.

Your remote reads a value from the physical throttle (lets say in a range from 0-1024) and then transmits this to a receiver which is communicating with the speed controller.

This input value interrupts an active process on the STM32 on the VESC by stating a motor state change is needed. The processes determines that you're ramping up the speed (or braking/reversing).  It communicates with the DRV8302 through seven PWM signal (made of 0s and 1s that are sent out very quickly). It tells the DRV8302 En_Gate to prepare for a new instruction, then six signals to six gate drivers. These drivers (acting as amplifiers) then turn off/on (01s) the MOSFETs very quickly. The motor doesn't see these 0/1s however.  It sees them the way a slow exposure camera sees moving light - it blurs them together.  The square waves of 0s and 1s blurs to produce a shape - a sinusoidal wave in this case - which travels across two gates at a time.

The above is a slightly more complex way to look at how the throttle works.

The more you know!
```

---
