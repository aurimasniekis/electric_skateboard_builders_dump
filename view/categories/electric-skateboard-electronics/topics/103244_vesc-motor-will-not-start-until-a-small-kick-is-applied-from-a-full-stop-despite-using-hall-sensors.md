# VESC - Motor will not start until a small kick is applied from a full stop despite using hall sensors

### Replies: 3 Views: 118

## \#1 Posted by: 010203040506070809 Posted at: 2019-10-23T21:13:59.882Z Reads: 41

```
Hi everyone,

I’m using a 4.12 VESC and having some issues. The motor will not start until a small kick is applied from a full stop. For example, in the initial motor calibration wizard using VESC Tools, after you press fwd to test direction (to determine whether to invert phase wires) and you press rev afterward, the motor just stalls. Even after the motor is full configured, the throttle does nothing (using ADC input) unless I “kick” off the scooter.

I have the hall sensors all wired up properly (at least I think so, matched all the colors) so I don’t know why this is an issue. i want it so that it can start from a full stop using the throttle and without me having to kick off.

Anyone know why the VESC is doing this and how to fix it?

My configuration: max motor current 35a, max regen current -12a, max current 80a, rpm 150k, max watt 750w
```

---
## \#2 Posted by: Andy87 Posted at: 2019-10-24T12:48:16.943Z Reads: 27

```
its not about matching the colors on the sensor wires, they need to have the right order as well. there is no norm for colors on sensor wires unfortunately. 
what das the motor detection say? hall sensor detection successfull or not?

Also, it doesn´t make sense to have higher bat max settings than motor max settings (doesn´t have anything to do with your problem thou)
```

---
## \#3 Posted by: 010203040506070809 Posted at: 2019-10-24T16:10:52.002Z Reads: 20

```
Motor detection says hall sensor detection successful. Does that mean the order is right or no?
```

---
