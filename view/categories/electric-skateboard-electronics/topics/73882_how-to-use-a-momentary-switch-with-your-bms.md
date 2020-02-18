# How to use a momentary switch with your BMS

### Replies: 5 Views: 301

## \#1 Posted by: chaka Posted at: 2018-11-08T01:30:09.549Z Reads: 86

```
Some of you might be familiar with the online distributor Pololu. So many cool components on this site but one very useful device they carry is a simple push button power circuit. It is possible to incorporate this circuit into your build to turn your BMS on and off with a momentary push button switch instead of a toggle!
 [https://www.pololu.com/product/2809](https://www.pololu.com/product/2809)
https://a.pololu-files.com/picture/0J6790.600x480.jpg?7e4b267e642a5afbf9f2803d2b9c360b
```

---
## \#2 Posted by: deltazeta Posted at: 2018-11-08T01:49:34.340Z Reads: 74

```
what would the wiring diagram look for this? I'm confused how the circuit gets power, since usually the switch circuit on a bms/antispark is just short detection, not power delivery
```

---
## \#3 Posted by: chaka Posted at: 2018-11-08T01:55:06.003Z Reads: 69

```
If you check the wires on the bms that are intended to be connected to a toggle switch one will have a voltage reading. Connect that wire to the Vin and the other wire to Vout. You also need to connect the GND on the latching circuit to your battery negative. The last connection is to your momentary switch using the appropriate pins on the latching circuit.


https://a.pololu-files.com/picture/0J6762.350.jpg?f2d48058bfbb41772fe2f325ae7d60f8
```

---
## \#4 Posted by: deltazeta Posted at: 2018-11-08T02:03:05.697Z Reads: 63

```
Would you be able to wire this for a 3 pin switch, like is required for antisparks?
```

---
## \#5 Posted by: chaka Posted at: 2018-11-08T02:05:07.429Z Reads: 63

```
Unfortunately, no that would not work as far as I am aware. Not with this circuit.
```

---
