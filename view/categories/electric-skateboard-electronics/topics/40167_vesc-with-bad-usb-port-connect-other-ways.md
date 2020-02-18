# VESC with bad USB port, connect other ways?

### Replies: 7 Views: 775

## \#1 Posted by: zhud Posted at: 2017-12-05T06:09:38.131Z Reads: 111

```
I have a VESC with a bad USB connection, I am having it replaced, but I am trying to see if I can use this until the replacement comes.

I have an ST-LINK USB connection, and I also have a HM-10 BLE. The settings on the VESC are set with UART off, using ADC for a hall sensor throttle. 

Wanting to know if it might be possible to manually send commands via the ST-Link, or the possibility to use the ST-Link USB or the HM-10 as a com port for the BLDC/Vesc tool?
```

---
## \#2 Posted by: scepterr Posted at: 2017-12-05T06:17:41.041Z Reads: 108

```
If you have a soldering iron and know how to use it, it's pretty simply to touch up the legs on the USB port if that's the issue, just 4 pins
```

---
## \#3 Posted by: zhud Posted at: 2017-12-05T06:39:11.688Z Reads: 100

```
I'm pretty decent with a soldering iron, it's just that the PCB copper wiring lifted from the board. I'd need to make jumpers to the resistors in order to get it working. It is something I may have to do, but it'd like to avoid having to do any microsoldering
```

---
## \#4 Posted by: Nordle Posted at: 2017-12-05T09:42:41.824Z Reads: 82

```
I had the same problem, solder pads were gone.. i soldered the 2 data wires directly to the usb resistors, and gnd somwhere to a gnd pin, you don't need any other connection for normal use.
```

---
## \#5 Posted by: lilracerboi Posted at: 2018-06-07T00:34:51.916Z Reads: 52

```
I burnt off the negative data pad...
What resistor is connected to the data pins?
```

---
## \#6 Posted by: Nordle Posted at: 2018-06-07T06:09:07.834Z Reads: 47

```
Is the resistor still there? Then you could solder directly on it.
```

---
## \#7 Posted by: banjaxxed Posted at: 2018-06-14T14:42:34.019Z Reads: 39

```
Hm-10 might suit tcp bridge

https://www.electric-skateboard.builders/t/change-vesc-4-12-settings-without-usb-port-broke-off-solved/46418

https://www.electric-skateboard.builders/t/best-way-to-program-vesc-via-bluetooth/57437/4?u=banjaxxed
```

---
