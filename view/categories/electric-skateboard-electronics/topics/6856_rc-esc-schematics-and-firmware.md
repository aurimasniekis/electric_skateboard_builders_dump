# RC ESC Schematics and Firmware

### Replies: 11 Views: 1890

## \#1 Posted by: brams Posted at: 2016-07-30T14:16:55.452Z Reads: 97

```
Seems that every Chinese is capable of manufacturing a RC Car ESC like these FVT 120A http://www.szfvt.com/eproducts/98.html sold everywhere or the Flier ones.

Has someone ever seen plans, schematics, BOM and firmwares for these ESCs? I plan to do some rearrangements to make them more slim like the VESC.
```

---
## \#2 Posted by: barajabali Posted at: 2016-07-30T14:19:28.049Z Reads: 97

```
You want to make the FVT 6s thinner? It's easy just take it apart and put the fan somewhere else. Or just remove the fan in general not really needed as long as the heat sink is near air flow
```

---
## \#3 Posted by: brams Posted at: 2016-07-30T14:22:14.075Z Reads: 92

```
Yes, but I need only one PCB, and the FVT is made of two stacked like a sandwich. Also I want to get rid of the beeps and integrate an RF receiver
```

---
## \#4 Posted by: JTAG Posted at: 2016-07-30T15:25:35.516Z Reads: 88

```
Why not take the vesc design and do exactly this?
```

---
## \#5 Posted by: brams Posted at: 2016-07-30T15:38:48.668Z Reads: 84

```
Because VESC BOM is 10X the price
```

---
## \#6 Posted by: JTAG Posted at: 2016-07-30T15:54:37.976Z Reads: 83

```
So you want to develop a ESC because you want to make it cheaper? Interesting.

Good luck.
```

---
## \#7 Posted by: brams Posted at: 2016-07-30T16:13:01.799Z Reads: 77

```
[quote="JTAG, post:6, topic:6856"]
Good luck.
[/quote]

I don't want to "develop" an ESC, I want to change the template of an existing one.
ESCs are not that much complicated electronics, it's basically MOSFETs and a MCU, there is just 100 ways to build one. The VESC is a complicated one because 32Bits, Ti DRV, CAN, 120 Amps, FOC Etc... Others are just 8Bits.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-07-30T16:13:31.271Z Reads: 77

```
The VESC is open source, and the Esc your looking for is already a rip off. You can always reverse engineering it, but I think,  you may need to start from scratch on this one. And at the end VESC will become a cheaper option. Except if you really want to challenge yourself, I wish you the best of luck.
```

---
## \#9 Posted by: brams Posted at: 2016-07-30T16:17:26.661Z Reads: 73

```
I just want to make it fit into a single PCB, with MOSFETs on one side and integrate a RF receiver. Just need the BOM and the schematics...
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-07-30T16:22:34.942Z Reads: 73

```
This is what I'm trying to say : You probably be unable to find them, because the product isn't open source, and generally BOM and schematics are not share by the companies who market the product.
```

---
## \#11 Posted by: JTAG Posted at: 2016-07-30T16:37:06.117Z Reads: 68

```
The hardware of the VESC and regular hobby ESC is not that different. The main and only significant difference is Current sending + CAN. Other differences you mentioned are not that relevant to express difficulty. 

The difficult bits of ESCs are FET driving + routing, voltage sensing and if desired current sensing.

There are 2 mayor opensource firmwares that are implemented by "chinese" manufacturers. There are even a few opensource HW BLDC ESCs. 

I don't want to sound to pessimistic but if you say ESCs are not that difficult you are very skilled ( by the many ESCs you already designed + made + used ) or there is a big smoking surprise waiting xD.
```

---
