# VESC help required! 3.3v shorted to ground

### Replies: 3 Views: 1059

## \#1 Posted by: makepeace Posted at: 2016-04-27T06:45:13.192Z Reads: 107

```
So I'm testing a VESC for my university, who want to start building them for projects and to sell in South Africa. The guy in the electronics workshop soldered it up. It looks pretty good mostly to the eye. The only visible issues are the usual bridges on the DRV chip.

I went over the board briefly to check for continuities/discontinuities, and there seems to be a short between the 3.3v rail and the ground plane. 

This is obviously hampering my first step to testing the board ie programming it. I'm going to take it back to the electronics guy to go over it, but before I do that I just wanted to check in with the community in case there is a quick and easy fix.

Has anyone had an issue like this before, after assembling the board? Any things to check? Could be a dud regulator, but that's unlikely, as the guy is pretty good at soldering and you shouldn't get a dud regulator off the supply line...

Any help or ideas would be greatly appreciated.

Peace eout.
```

---
## \#2 Posted by: JTAG Posted at: 2016-04-27T13:09:56.087Z Reads: 90

```
Assuming you used genuine components and you didn't power the board yet. It can only be a soldering error or a defect in the PCB, the latter being the worst. And assuming the short you measured is a dead short ( 0Ohms in resistance or 0Volts in diode) the following is likely the case:

*I checked the schematic, 3V3 (or VCC in the schematic) is only connected to pins 9 & 24 please check these pins for shorts to GND.
*One or multiple pins on the STM32 package have shorts (very likely please check!), most of the 3V3 supply rail connections are to the STM32.

Since the DRV is much easier to solder than the stm32 and you found shorts in de DRV package I really suspect the STM32 to have the solder joints. 

Good luck! And if no succes, please share pictures.
```

---
## \#3 Posted by: Fungineers Posted at: 2019-10-03T06:15:10.179Z Reads: 19

```
Did u figure this out?
```

---
