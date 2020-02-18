# Motor spins during charging

### Replies: 8 Views: 185

## \#1 Posted by: johan1007 Posted at: 2019-04-02T20:41:58.307Z Reads: 87

```
Hello

I have a problem. When i charge my board the motor starts to spin with a jerky motion and some times it spinns to full throtle. Happens even when the remote is off. Also when i ride the board it can some times do the same thing when i come to a stop. 

When charging i have to unplug the charging cable and wait for a few seconds before pluging it back in. 

Any ideas? 
My setup:
Focbox 4.12
Bestech BMS 80A, charge/discharge
Firefly remote

This is a simple wiring diagram of my setup.
![image|690x300](upload://8w5qaxpfWunUS6frQiwBxWZROUF.jpeg)
```

---
## \#2 Posted by: olestra Posted at: 2019-04-02T20:49:50.820Z Reads: 78

```
bet the signal wires from your receiver to the VESC are near the BMS or the charge wires, and are picking up an inducted signal.
Ideally your ESCs should not be powered when charging
```

---
## \#3 Posted by: olestra Posted at: 2019-04-02T20:54:36.781Z Reads: 76

```
For a test, unplug your receiver when charging and see. 

If things still spin your ESC has a floating ground, and you should tie a wire from the negative side of the receiver to something like a truck -- that might help
```

---
## \#4 Posted by: banjaxxed Posted at: 2019-04-02T21:07:42.612Z Reads: 66

```
Try a ferrite ring around the cable
```

---
## \#5 Posted by: pat.speed Posted at: 2019-04-02T21:12:15.007Z Reads: 60

```
You probably don’t have the failsafe set up. 

[quote="olestra, post:2, topic:89141"]
picking up an inducted signal
[/quote]

This is possible but the fact that it happens during riding sometimes when stopped is probably because failsafe isn’t set properly or the throttle dead range is slightly too small.

I would plug it in to charge and wait for it to happen, while it’s doing it turn on your remote to see if the stuttering stops
```

---
## \#6 Posted by: b264 Posted at: 2019-04-02T21:14:26.727Z Reads: 55

```
Yes, this :arrow_up:

If you have Mini Remote, [set the failsafe](https://forum./t/how-to-bind-the-mini-remote/95) then set up the PPM tab in your VESC to have the correct center point.

If you don't have mini, check how to set your failsafe point and then set up the PPM tab in your VESC to have the correct center point.
```

---
## \#7 Posted by: olestra Posted at: 2019-04-02T21:15:56.700Z Reads: 55

```
I didn't think of the deadzone or fail safe... I've got a really long receiver wire and when I was first setting up it was draped across the motor leads -- gave me some really fun behaviors!
```

---
## \#8 Posted by: johan1007 Posted at: 2019-04-13T09:16:23.018Z Reads: 18

```
Thx for all info :) il uppdate when i get the time to open my board.
```

---
