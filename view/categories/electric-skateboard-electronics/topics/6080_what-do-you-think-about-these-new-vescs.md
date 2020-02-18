# What do you think about these new VESC&rsquo;s?

### Replies: 7 Views: 1925

## \#1 Posted by: laikiux Posted at: 2016-07-14T06:02:05.392Z Reads: 264

```
There they are: http://www.ebay.com/itm/VESC-4-12-Motor-controller-open-source-BLDC-Speed-Controller-VESC-vedder-Pcb-/182195728273?hash=item2a6bb62f91:g:oFwAAOSwZ1BXe6Ct 
Are they reliable?
```

---
## \#2 Posted by: Maxid Posted at: 2016-07-14T06:27:33.329Z Reads: 256

```
Don't know them but they say they even redesigned the VESC with all MOSFETs being on the same side now.
Maybe a professional with electronics know-how like @JTAG can tell us if that is a good thing?
```

---
## \#3 Posted by: rpn314 Posted at: 2016-07-14T15:22:32.695Z Reads: 229

```
So take this with a grain of salt, since I'm not JTAG or Vedder, but I do have some electronics experience (currently studying electrical/computer engineering)

I would be a little worried about this. It looks like they've mostly separated the power components and the control components of the board, except for the motor phase wire leads, so it's not truly separated thus losing the benefits of having separated control and power boards. Vedder toyed with this idea of a split board design in VESC 5.0 , but he has since decided to keep it a single board (VESC 6.0)
```

---
## \#4 Posted by: thisrealhuman Posted at: 2016-07-14T16:24:08.257Z Reads: 199

```
The phase wires are in a really odd place, jammed sideways out of the center of the board. The dual board and heat sink looks like a good idea but it needs a mounting plate.
```

---
## \#5 Posted by: JTAG Posted at: 2016-07-14T21:39:18.970Z Reads: 171

```
By the looks now benjamin went for direct fets by international rectifier. These FET's are well suited for cooling trough the metal side of the package (the mail goal of the fets), so it is indeed a good thing he went for these FETs. The downside however is that this package is really challenging to solder (only possible with hot air or infrared).
```

---
## \#6 Posted by: NNGG Posted at: 2016-07-14T22:20:07.385Z Reads: 152

```
I dont think It matters, They cost $160 (USD) for me, and for that I could buy a warrenty enertion vesc
```

---
## \#7 Posted by: laikiux Posted at: 2016-07-31T16:46:33.191Z Reads: 114

```
Maybe there are people, how tried these VESC's. It would be interesting hear something about them.
```

---
