# Using drill batteries as an alternative to lipos?

### Replies: 6 Views: 1388

## \#1 Posted by: mach5 Posted at: 2016-11-18T17:40:11.969Z Reads: 152

```
After many attempts to power my board, i always seem to destroy my lipo balance wires within the first day of my purchase. I have no ideas how this happens. I am using a 5000mah 3s battery in series with the same battery. The volt meter says that the batteries are fully charged but the balance mode recognises the battery as something different. After spending loads of money on lipos that break, i am looking into using drill batteries to power my board. Specifically, makita 18v 3ah batteries. I am planning to connect 2 in parallel and then those pairs in series which will give me 36 volts (4 batteries total). My motor is a 280kv sk3 motor from hobbyking. Gear ratio is up for change. I plan to buy a vesc x esc so i can regulate the voltage that goes to the motor. I want to regulate it at 30 volts because the motor says 37 max voltage. Will these makita batteries work? I dont care about the weight, i only weigh 115. I am most concerned with the discharge rate of the makita batteries which i could not find specs on.
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-18T18:08:27.880Z Reads: 143

```
Makita makes 36v batteries too, so i would use that instead of the 18v ones. I would do some reasearch before commiting to something like this, a quick search on google seems to show that this batteries, once a cell fails the circuit board inside them prevents them from charging, FOREVER.

As for the cells inside, they are Sony Konion 18650 1.5ah, max discharge 10C, max charge rate 1C.
If you consider the 18V pack, its 5S2P so you would have a discharge rate of 10Cx1.5Ah * 2 = 30A
```

---
## \#3 Posted by: mach5 Posted at: 2016-11-18T18:26:05.572Z Reads: 131

```
Thanks, so that means with my setup with the 18v batteries it will be at 60 amps? Does that means the vesc x can handle it? It says it can handle 60 amps continuous.
```

---
## \#4 Posted by: chinzw Posted at: 2016-11-18T18:29:44.661Z Reads: 125

```
That would be 60A max discharge rate yeah. The vesc can handle 60A.
```

---
## \#5 Posted by: Mrossi1115 Posted at: 2016-12-29T09:01:56.067Z Reads: 86

```
do you have any pictures of your board using the makita batteries?
```

---
## \#6 Posted by: PXSS Posted at: 2016-12-29T13:16:50.617Z Reads: 68

```
 You do realize they are 18650cells inside those burly boxes right? Why not just buy the cells and make your own or buy a premade one from someone here?

Cells are $4 a pop for samsung 25r. So a 5s4p like 2 18v makitas, would run you at $80. 80A max discharge and 66% more range
```

---
