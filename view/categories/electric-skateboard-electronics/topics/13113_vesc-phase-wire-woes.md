# VESC Phase wire woes

### Replies: 3 Views: 794

## \#1 Posted by: mikey Posted at: 2016-11-15T19:49:13.383Z Reads: 157

```
I'm using dual Vescs with Carvon 2.5 hubs in FOC.
I didn't like how long my phase wires were so I cut them shorter. 

My problem was soldering the 4mm bullet connectors onto the 10 gauge wire.

1st attempt: Soldered everything. Had a lot of issues with one wire. Nothing shorted, but I got a DRV8302 fault.
found out it was because of my soldering job. (It worked again when I fiddled with the wires)

2nd attempt: I cut them even shorter and cleaned up the wire even more before I soldered the bullet connectors on. Still couldn't get all the strands in on connector but I put a lot of solder on it. Now I'm getting either UNDER_VOLTAGE or ABS_OVER_CURRENT when I test the board without any load. I assume its this soldering job again because there are burnt chips on my vescs as fas as I can see.

My question is should I try to desolder the phase wires from the vesc altogether and replace them with AWG12gauge silicone wire? I'm thinking 12 gauge because it is easier to work with and the motor wires on the carvon 2.5's are 12gauge anyways. 

Or should I just send it back to @chaka  and have a professional do it? 

BTW Im using a weller 40watt soldering iron. :frowning:
```

---
## \#2 Posted by: chaka Posted at: 2016-11-15T20:14:20.958Z Reads: 144

```
40 watts is a little low for 10 awg cable. Normally use something around 100 watts to solder connectors. We also use a wire stripper and reduce the wire strands to 12awg before tinning in order to fit the cable into 4mm connectors or xt-60. You can switch to a smaller gauge wire if needed but you may still have trouble with cold joints using a 40 watt iron. A good liquid flux helps the whole process.
```

---
## \#3 Posted by: chinzw Posted at: 2016-11-17T00:40:58.655Z Reads: 86

```
Also, make sure you redo all the motor detection/calibration as the resistance will change ever so slightly, and that can throw off the vesc.
Ill second chaka on the flux! Use it, you will get beautiful solder joints, every time.
```

---
