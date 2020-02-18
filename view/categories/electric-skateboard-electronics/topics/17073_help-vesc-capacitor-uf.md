# Help - Vesc capacitor uF?

### Replies: 4 Views: 959

## \#1 Posted by: tilmnater Posted at: 2017-02-02T03:55:44.790Z Reads: 120

```
I'm trying to determine if three 560uF 63V capacitors on my vesc is sufficient for a 245kv 10s setup? Most of the ones I see these days have 680uF or higher. 

I know this motor/battery setup isn't ideal for the vesc, but it's what I've decided to do for my first build. This was the only part that arrived "not as described" and I do have the option to return it if necessary. It also came with 14 awg wire, but I can always replace it with 10 awg. Thanks in advance for your help.
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-02-02T05:45:55.527Z Reads: 113

```
The capacitance value is chosen base on factors relating to inrush current between the battery and VESC and resistance value within the circuit. Easier said than done. The original creator of the VESC used a single 2000 μF capacitor that he had lying around. Using more than one is fine. I would choose the capacitor with the lowest resistance (ESR) value since three of either the 560 or 680 in parallel is sufficient.
```

---
## \#3 Posted by: tilmnater Posted at: 2017-02-02T06:13:11.087Z Reads: 109

```
Thanks @chuttney1. So there would be no noticeable performance difference if I had say three 680 or two 1000 vs my current setup?
```

---
## \#4 Posted by: chuttney1 Posted at: 2017-02-02T06:46:25.842Z Reads: 98

```
It's not really about performance you can feel. Capacitors are used to smooth out changing voltages within a circuit. Just go for the low ESR capacitors. You will need to look at data sheets to compare. To answer your question directly, you would not see anything different between using 680 μF and 1000 μF capacitors. The physical difference is the size between both. What is related to choosing the number of capacitors is how long your wires are from the battery to the ESC.

This topic has been discussed in an RC forum linked below.
https://www.rcgroups.com/forums/showthread.php?952523-too-long-battery-wires-will-kill-ESC-over-time-precautions-solutions-workarounds
```

---
