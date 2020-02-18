# Does the number of cells in series matter to the ESC?

### Replies: 5 Views: 203

## \#1 Posted by: hamac2003 Posted at: 2019-05-21T20:54:28.672Z Reads: 77

```
I'm 98% certain that I already know the answer to this, but I just wanted to clarify that the number of battery cells wired in series does not matter to the ESC whatsoever, so long as the resultant voltage is within the required limits for that particular ESC. So a 3s battery with 4v cells would be identical in terms of compatibility with any given ESC as a 6s battery with 2v cells (I understand that the two setups would not be _exactly_ the same, I'm simplifying for clarity.
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-05-21T20:58:12.286Z Reads: 73

```
Yeah, that's all there is to it.  If the voltage is in bounds then there is no issue, just make sure you measure from the max voltage to see if the system can handle it correctly.  You may see issues with the cutoff voltage being wrong depending on the chemistry.  I think all the VESCs have options for liion/lipo/lifepo4 but that's just a preset for the expected and safe voltages

Whatcha trynna do with unusual voltages?
```

---
## \#3 Posted by: Sebike Posted at: 2019-05-21T21:13:21.340Z Reads: 52

```
When number of cells in series are specified for an esc, bms or whatnot, it is usually for li-ions/ lipos, ie 4,2 volts/series at full charge ... If say a BMS is intended for li-fe po cells, it's clearly stated. 

When setting up an ESC types of cells matter when setting cut-off voltages etc, so pay extra attention that everything is set up correctly!
```

---
## \#4 Posted by: hamac2003 Posted at: 2019-05-21T21:24:52.709Z Reads: 42

```
> Whatcha trynna do with unusual voltages?

Nothing much, I'm thinking about buying a budget board completely assembled. And if I don't like the range on it, I want to throw together a custom dewalt battery system I've been wanting to build to give it some more juice. But I wanted to make sure I could safely power the control system of said board with a different number of cells than are in the stock battery. Sounds like it should work fine, as long as I can get the upper and lower voltage range to match.
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-05-21T21:30:00.809Z Reads: 37

```
Just make sure you don't run batteries in parallel with different voltage, disconnected the board battery then plug in the external battery

If you are using external cells then disconnect the board at the ESC/BMS junction and to use an antispark in there, you can replace the BMS/drill out leads with an XT90s and the ESC with and XT90 male so it's a little smaller
```

---
