# Flipsky Vx2 remote with dual 4.12 Vesc’s

### Replies: 3 Views: 211

## \#1 Posted by: Birdman_177 Posted at: 2019-10-27T13:16:10.084Z Reads: 66

```
Wondering if anyone can help me out. I have a dual motor set up with 2 single 4.12 Vesc’s from  and I want to use the Flipsky Vx2 remote with them without a CAN BUS cable connecting the 2 Vesc’s. Right now I have a ppm split cable going from my receiver to each vesc and the only reason I’m not using CAN BUS is because I can’t seem to get get it working. So is this possible without CAN BUS? Do you just split the rx and tx wires to go to each vesc and have all the other wires going to only 1 vesc?
```

---
## \#2 Posted by: Movation Posted at: 2019-10-28T15:12:01.077Z Reads: 46

```
Firmware has to the the same accross both vesc. And recent firmware version, if you cant update fw a vx1 is a better option. Try flipping rx and tx wires. Also set up as nfr option. If your fw is older try nunchuck.
```

---
## \#3 Posted by: lelingzhou0924 Posted at: 2019-11-12T06:46:52.339Z Reads: 20

```
I think build the dual for two single vescs needs the can-bus connector, like sth. bridge. If no CAN-bus connector, they are not combined and cannot be controlled by the same firmware. Also, need the same battery, I think.
```

---
