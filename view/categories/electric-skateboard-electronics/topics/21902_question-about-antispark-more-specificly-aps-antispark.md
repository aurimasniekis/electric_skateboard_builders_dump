# Question about antispark - More specificly APS antispark!

### Replies: 4 Views: 497

## \#1 Posted by: Guacamoleface Posted at: 2017-04-27T14:00:40.302Z Reads: 151

```
Hey ! 

Im just curious how the APS antispark works - does it not break the positive connection?
It seems to me that current flows through the positive wire, I notice this on my Battery capacity meter.

Its wired to negative battery wire, and positive output on the antispark - and its not that its leaking voltage then the % would not show correct - the voltage is correct the so the voltage from negative battery wire along with after output wire on antispark is still the full!
```

---
## \#2 Posted by: emepror Posted at: 2017-04-27T14:09:44.378Z Reads: 147

```
Current flows in a loop, there has to be a return path for current to flow. You can also measure current draw on either the high side or the negative, and its easier to design a low (gnd) side switch for the antispark.
```

---
## \#3 Posted by: Guacamoleface Posted at: 2017-04-27T14:12:20.653Z Reads: 145

```
Ok, thanks for the reply. 
so if I understood this correct - an antispark cant cut off the current from both poles as the flowing current has to flow back into the battery?
```

---
## \#4 Posted by: emepror Posted at: 2017-04-27T14:33:13.551Z Reads: 130

```
Well because you cut off part of the connection with the antispark, the current wont flow to begin with, so no issue with it acting as a switch.
```

---
