# Sensor wires and Arduino

### Replies: 3 Views: 362

## \#1 Posted by: KTMinni Posted at: 2017-03-04T13:41:29.708Z Reads: 58

```
Hi, I am not sure if this has been done before, but has anyone tried plugging the sensor wires from the motor into an arduino? If so what did you use it for?
```

---
## \#2 Posted by: rpn314 Posted at: 2017-03-04T13:53:39.161Z Reads: 57

```
The sensor wires give the position of the rotor. If you know how to decode that (which I'm sure is written out there somewhere) then you could capture speed, acceleration, and maybe temperature (some sensor wires have a temperature sensor as well).

I suppose you could do some sort of readout, but I've not seen anyone do it as _almost_ everyone that doesn't have a VESC wants to use the sensor wires with their ESC (assuming it can use them, and many can) and everyone who does have a VESC can get a good readout straight from the VESC with or without using them.

TLDR: you can get motor position with which you can calculate speed and acceleration, but most people are either using their sensor wire or get that information from the VESC.
```

---
## \#3 Posted by: KTMinni Posted at: 2017-03-04T19:23:40.250Z Reads: 43

```
Thanks for the quick reply!  But I have a plan that requires that information be read by an arduino.  So hopefully, those wires output an integer and not some random hex code haha. I might have a look at the BLDC code.  Thanks for the ideas.

Sincerely,
Kent
```

---
