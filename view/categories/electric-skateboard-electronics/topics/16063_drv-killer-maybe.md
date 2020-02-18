# DRV Killer (maybe?)

### Replies: 6 Views: 862

## \#1 Posted by: zmoney Posted at: 2017-01-13T23:33:56.010Z Reads: 134

```
The guys at Infineon were talking to me about a new driver. Check it out. Might be a good substitute for the DRV (if someone could compile firmware for it).

http://www.mouser.com/ProductDetail/Infineon-Technologies/IRS26302DJPBF/?qs=sGAEpiMZZMvQcoNRkxSQkuxFHgU%2fOEtLrPtSTXV9fjg%3d
```

---
## \#2 Posted by: chaka Posted at: 2017-01-13T23:49:10.575Z Reads: 128

```
You would be better off using seperate drivers for each phase and some current shunt amplifiers if you want to drive larger FETS. You would also need to provide a regulator for 12v power in this scenario.  

Are you looking for more current handling or higher voltage capability?
```

---
## \#3 Posted by: zmoney Posted at: 2017-01-13T23:58:47.234Z Reads: 119

```
Just something that caught my eye :slight_smile:. Thought it might be interesting
```

---
## \#4 Posted by: chaka Posted at: 2017-01-14T00:06:30.842Z Reads: 116

```
Check out vedder's forum. Someone is working on a high voltage version, I think they have a working model.
```

---
## \#5 Posted by: zmoney Posted at: 2017-01-14T00:21:32.540Z Reads: 110

```
Yeah I saw that, although I haven't really put much thought into it.
```

---
## \#6 Posted by: Dimitri Posted at: 2017-05-31T03:27:29.998Z Reads: 40

```

The IRS26302 would probably handle stress a lot better and not blow,

BUT it's output current ability is TOO LOW (0.2A) for driving large FET gate capacitances (for example the IRFS7530 in VESC 4)

The result would be **Overheating of the FETs** due to SLOW TURN ON.... 
i would NEVER use that. instead, most likely you will find high current FET drivers as single drivers... as chaka suggested (so you would need 3 of them... 1 for each Half Bridge)

But even a high current ability is **not enough**.. you still need to have low propagation delay and large enough (but not too large) dead times...

There is a big variety of high current drivers out there, you would need to have similar specifications with the DRV8302/DRV8301
```

---
