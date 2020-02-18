# Balance lead ground on supower bms?

### Replies: 3 Views: 265

## \#1 Posted by: BenTheBarre Posted at: 2018-02-14T00:24:43.972Z Reads: 45

```
I have 2x 5s lipos wired in series connected to a 60a 10s supower bms. However, the balance lead port on the supper BMS's only have 10 slots for each cell, and no extra slot for a ground. Do I need to have one ground wire from the balance leads (from the battery) attached to either b- or p-? Or can I just disregard the ground leads? Thanks!
```

---
## \#2 Posted by: butt_stallion Posted at: 2018-02-14T01:33:28.555Z Reads: 41

```
The wiring should look like the picture below.  All the balance leads attach to the positive's of the cells and the main negative will go to B- on the board and then the P- is used to charge the board and for the ESC.  

![0126180910|690x388](upload://A3FqtvGxnHHoxvlQefDmYxJ083I.jpg)
```

---
## \#3 Posted by: rich Posted at: 2018-02-14T01:34:29.482Z Reads: 38

```
There are 10s BMS with 11 pins and with 10 pins like yours. You don't have to connect the negative balance wire of the first lipo because with B-  it's already connected. Lipo 1 is the negative lead (and balance 1+ - 5+ on BMS) and Lipo 2 the positive (balance 6+ - 10+)
```

---
