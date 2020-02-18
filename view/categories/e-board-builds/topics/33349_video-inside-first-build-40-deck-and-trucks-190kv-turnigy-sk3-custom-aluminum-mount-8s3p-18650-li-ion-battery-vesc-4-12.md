# (Video Inside!) First Build &#124; $40 Deck and Trucks &#124; 190kv Turnigy SK3 &#124; Custom Aluminum Mount &#124; 8s3p 18650 Li-Ion Battery &#124; VESC 4.12

### Replies: 7 Views: 657

## \#1 Posted by: Auhv Posted at: 2017-09-17T18:44:33.095Z Reads: 157

```
Hey everyone, I've finally finished my first build after browsing these forums regularly for the past 4 months. I don't have any pictures, but I made a video instead.  Let me know what you think:

[https://www.youtube.com/watch?v=czH7M9UbVVA](https://www.youtube.com/watch?v=czH7M9UbVVA)
```

---
## \#2 Posted by: Jammeslu Posted at: 2017-09-17T19:20:05.195Z Reads: 141

```
Do you get any voltage sag?
```

---
## \#3 Posted by: pjotr47 Posted at: 2017-09-17T19:25:30.530Z Reads: 137

```
What pulley set do you use?
```

---
## \#4 Posted by: Auhv Posted at: 2017-09-17T20:16:14.053Z Reads: 125

```
15T/36T, 255mm 5M HTD belt,  it can be found here:

http://www.ebay.com/itm/DIY-Electric-Skateboard-ABEC-Flywheel-Pulley-Kit-15mm-Wide-Belts-/182618936000?hash=item2a84efd2c0%3Ag%3AjxsAAOSwjvJZP6e6
```

---
## \#5 Posted by: mptrs Posted at: 2017-09-17T20:37:00.399Z Reads: 115

```
Nice video, good to see it's possible to solder those batteries. Do watch you joints, some looked to me a bit brittle and 'cold'. 
Bit scary with the metal box tho.

But it's nice to see you made almost everything yourself.

Very nice first build!
```

---
## \#6 Posted by: Auhv Posted at: 2017-09-17T20:47:18.280Z Reads: 104

```
I actually insulated the bottom of where the vesc was sitting to make sure nothing would short, I was worried about this too.
```

---
## \#7 Posted by: Auhv Posted at: 2017-10-15T06:20:40.157Z Reads: 69

```
Voltage sag is relatively small, but still significant with my specific pack because of the internal resistance of the cells.

Every cell has ~20milliohms IR which will be the cause of the power dissipation and voltage sag.  Total power at the terminals of the pack is 

       P = IV - I^2*R

where I^2*R is the loss dissipated as heat due to internal resistance. Since we're only drawing 60A maximum,

     I^2*R = (60)^2*(.020*8 cells in series) = 576 watts

and then at the terminals, ideal power is:

    3.7V*8 cells in series * 60A = 1.776 kW

so we can set up a ratio to find voltage sag and actual power:

    1776W/29.6V = (1776W-576W)/x volts -> x = 20V

so we're getting a voltage sag of approx 

    29.6V - 20V = 9.6V 

at maximum current draw, and voltage sag will decrease exponentially from P = I^2*R as the ESC draws less current 

All calculations aside, it accelerates quick enough, and although voltage sag is an unfortunate characteristic of non-ideal voltage sources, we can still draw more current to account for power loss as long as it's not above 60A
```

---
