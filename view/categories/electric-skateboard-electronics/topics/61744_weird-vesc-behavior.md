# Weird VESC Behavior

### Replies: 2 Views: 133

## \#1 Posted by: Gamer43 Posted at: 2018-07-13T08:34:08.459Z Reads: 52

```
Alright so this might be a bit difficult to describe, but here it goes.

My setup is dual hub motor (8 inch hoverboard motors) controlled by two VESC 4.12's and split ppm with ideal diode.

One of the VESCs is store bought, my friend gave it to me after it blew up on him and I repaired it by swapping out the DRV8302 using a heat gun. (Don't worry I intend to pay him once I get my first paycheck).

The other is partially assembled, and I finished the assembly myself. (link to partially assembled PCB I purchased https://www.diygadget.com/electric-skateboard-parts/176-vesc-bldc-open-source-electric-skateboard-esc-partially-assembled.html).

This is the one with the weird behavior. 
So what happens is, I run these hub motors using field oriented control (the application where it actually matters) and after a couple of minutes, the motor controlled by the hand assembled VESC starts to cog and vibrate mildly, sometimes violently, but still spins at the desired speed and maintains functionality. Real-time data indicates sporadic motor currents (jumps back and forth between negative and positive). 
And this is where the interesting part comes in, if I press my finger on specific areas of the PCB, the vibration and cogging goes away COMPLETELY. These areas are the part of the DRV8302 next the inductor, the CAN transceiver, and the side on the STM32f405 next to the CAN transceiver, best performance is the area right smack dap in the middle of this. 

I can't explain this; what my finger provides to the board is a couple hundred picofarads of capacitance to ground, but the components in that area are bypass caps and passives for the buck converter, and the signals in that area are mostly digital (usb, can). I can't test the opposite side of the board because the power wires are in the way, but what's there is the TVS diode and phase sense resistors (which are unused for FOC, but used in trapezoidal control).

There is no vibration if I use trapezoidal control (slow decay); the motors scream at me regardless.

If anyone can explain this, or offer suggestions as to what can replace my finger so I can hot-snot it onto the board that would be much appreciated.
```

---
## \#2 Posted by: Gamer43 Posted at: 2018-07-13T08:54:02.742Z Reads: 41

```
Looks like conductive anti-static PU foam does the trick, now the question is how do I mount the foam flush with the PCB.
```

---
