# Changing V-ESC capacitors

### Replies: 7 Views: 1038

## \#1 Posted by: Haplo Posted at: 2016-11-13T16:01:43.692Z Reads: 166

```
Hello,
I'm building my new board with a custom deck and I don't have much room in height for the electronics, only 1cm.
Everything will fit, except the huge capacitors of the VESC.

I wonder if I can change the three 63v 680uf capacitors by seven 63v 330uf.
I think the capacity is still good(2040uf before/2310uf after) but I'm wondering if increasing the number of capacitors does not increase the risk of failures...

I may have another option: My board will run at 6s,  63V caps may be a little oversized... Can I safely change them by some 35V 680uf?

From what I read, the capacitors are here to avoid electric surge from long battery wires and this is common to all ESC but I don't know if the VESC has some specificites about this and I prefer to ask before frying one...

What solution seems to be best for you?
Thanks for your help!
```

---
## \#2 Posted by: ThomasRBK Posted at: 2016-11-13T16:04:45.071Z Reads: 156

```
Maybe you should get some more clearance, because the VESC needs some room to get air to cool down.
```

---
## \#3 Posted by: rpasichnyk Posted at: 2016-11-13T16:12:32.397Z Reads: 144

```
Yes, you can change capacitors to match your maximum voltage or a little bit above to be safe. The most important thing is to use capacitors that can output high current. Make sure you use capacitors designed for high ripple current!
```

---
## \#4 Posted by: Hummie Posted at: 2016-11-13T17:18:52.462Z Reads: 133

```
Multiple in parallel are better anyway. I forget why
```

---
## \#5 Posted by: TarzanHBK Posted at: 2016-11-15T10:44:08.258Z Reads: 91

```
"A couple reasons come to mind:

1.Lower ESR. The effective ESR of the capacitors follows the parallel resistor rule. For example, if one capacitor's ESR is 1 Ohm, putting ten in parallel makes the effective ESR of the capacitor bank ten times smaller. This is especially helpful if you expect a high ripple current on the capacitors.

2.Cost saving. Let's say you need a large amount of capacitance. A single large capacitor might be more expensive than several smalls ones that add up to the same amount.

3.Filtering. Capacitors of different values have different impedance characteristics as a function of frequency. If you're trying to filter out a range of frequencies (noise, EMI, etc), it's helpful to put a range of different capacitors next to each other to present low impedance to as much undesirable frequencies as possible.
Stock availability. Distributors don't carry every possible value of capacitance. You may need to combine multiple caps that add up to a specific capacitance you need.

4.Board Layout. The physical constraints of the PCB or enclosure may allow multiple small parts to fit where a single large part will not."
```

---
## \#6 Posted by: Tomer Posted at: 2018-04-16T12:35:34.479Z Reads: 45

```
I just bought [these 6800uF 63v](https://www.amazon.com/gp/product/B0188FWIFS/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1) capacitors, do you think they are designed for high current?
```

---
## \#7 Posted by: rpasichnyk Posted at: 2018-04-16T19:58:39.653Z Reads: 34

```
Yes, they have 3500mA ripple current which is more than capacitors recommended by Vedder here https://github.com/vedderb/CapPCB so you should be just fine
```

---
