# ESC why sensors?

### Replies: 5 Views: 183

## \#1 Posted by: DanishDynamite Posted at: 2019-02-07T20:20:54.513Z Reads: 88

```
I am running sensorles on my trampa build and woundering if anybody knows why you need the sensors for soft start???
The reason i ask is that at work we use a lot of 400v 3~ motors (from 0,5kw - 500kw) and a ABB driver to control them there are no sensors at all and they always start the right way no matter what because of the way the mains are connected to the motor some are controled by tourqe some by voltage and som by frekvenz (Hz) so why cannot the esc make sure that the the pahse are the same on each main to the motor??
Just woundering
Great forum guys👍🏻👍🏻
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-02-07T21:10:56.710Z Reads: 67

```
Because 3-phase industrial motors aren't the same as BLDC motors. BLDC motors are synchronous, and industrial motors generally aren't. That means that a brushless speed controller has to know what the motor position is much more than an industrial motor controller/VFD does.
```

---
## \#3 Posted by: dareno Posted at: 2019-02-07T21:12:51.035Z Reads: 59

```
sensors are for pussies
@Andy87  :stuck_out_tongue_winking_eye:
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-02-07T21:20:12.556Z Reads: 55

```
Induction motors (that covers most industrial motors) generate a rotating magnetic field that "drags" the rotor along with it, with some degree of slip. That slip allows you to feed the motor 3-phase at 60hz and the rotor will get dragged up to speed.

BLDC (also known as Permanent Magnet Synchronous Motors, PMSM) have magnets in them and that keeps the rotor locked to the magnetic fields, in sync. Because of this, you can't just feed a PMSM 3-phase 60hz power and have it start to spin. It'll just vibrate. You have to start at 0 hz, matched to the rotor position, and increase from there. To do that, the controller has to either fake it and guess the position (which causes the roughness and jitter in sensorless startup), or have some kind of sensor to know where the rotor is.
```

---
## \#5 Posted by: DanishDynamite Posted at: 2019-02-07T22:39:55.775Z Reads: 33

```
Thanks:-) worked so longe with induction motors that i did not think of a permanent magnet motor
```

---
