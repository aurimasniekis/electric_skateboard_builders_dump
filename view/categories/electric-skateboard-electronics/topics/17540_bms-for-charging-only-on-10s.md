# BMS for charging only on 10S

### Replies: 15 Views: 1166

## \#1 Posted by: Eboosted Posted at: 2017-02-11T06:06:31.575Z Reads: 162

```
If I use the BMS for charging only for a 10S4P can I use the 10S 30A BMS?
```

---
## \#2 Posted by: Surfer Posted at: 2017-02-11T06:39:41.834Z Reads: 163

```
Yes, you can.
```

---
## \#3 Posted by: benwong Posted at: 2017-02-11T10:26:27.074Z Reads: 158

```

Same here, i confuse the connection if Bms, here is my diagram. i need connect step 1 > 2 > 3? or 2 > 3 > 1?? <img src="/uploads/db1493/original/3X/0/7/07e03f1abd10bde965ecc6bc20587a6cbcb732e8.JPG" width="534" height="499">
```

---
## \#4 Posted by: Martinsp Posted at: 2017-02-11T10:30:46.021Z Reads: 145

```
If you only wanto to charge it through the BMS then you can of course, even lower amperage because i doubt that you are going to charge the pack with 30A... But if you want to discharge the pack through the BMS then you should get a BMS capable of discharging the pack at the maximum amperage you are planning on pulling out of the pack or higher for some headroom and safety.
```

---
## \#5 Posted by: Martinsp Posted at: 2017-02-11T10:32:45.427Z Reads: 137

```
and the diagram.. I dont think that it matters, you can connect it in whatever order you wand as long as you dont short anything it should be OK. 
hope I understood the question right :)
```

---
## \#6 Posted by: lowGuido Posted at: 2017-02-11T10:55:31.892Z Reads: 133

```
don't join the B positive and A negative in the balance leads. it's a recipe for confusion. 
...if I has a dollar for every thread on this forum from people who messed that up...

also you don't need to connect the B balance negative to the BMS. thats already done in the negative wire.
```

---
## \#7 Posted by: RiGo Posted at: 2017-02-11T11:03:53.605Z Reads: 128

```
n00b question, but if you're regulating current draw through the VESC, then would there be any advantages to also using the BMS for discharge?
```

---
## \#8 Posted by: lowGuido Posted at: 2017-02-11T11:07:04.393Z Reads: 124

```
no. not really.

BMS just has a MOSFET switch built in that will turn off if the voltage gets too low.

you can program all this with VESC.. hence why some people opt for using a lower Amperage BMS for charging only.
```

---
## \#9 Posted by: RiGo Posted at: 2017-02-11T11:17:34.739Z Reads: 123

```
Thanks, so how do you bypass the BMS for discharge when soldering the connections? Do you only connect the balancing wires to the BMS and connect the main +ve -ve leads to the charging port?
```

---
## \#10 Posted by: benwong Posted at: 2017-02-11T11:19:26.038Z Reads: 119

```
Balance lead A  negative should not connect to balance lead b positive?  So means that lead A black wire should cut it. only 8 positive pin connect to BMS?
```

---
## \#11 Posted by: Surfer Posted at: 2017-02-11T11:22:24.610Z Reads: 114

```
Not sure about it, but I think the advantage of discharging trough BMS is the undervoltage protection for individual cell, and with the vesc the protection is with the total voltage.
```

---
## \#12 Posted by: lowGuido Posted at: 2017-02-11T11:39:23.488Z Reads: 111

```
The bms ties all the cells to the same voltage by bleeding the higher cells through a series of resistors and fets which it is doing regardless of what you have it connected to.

You people are fooling yourselves if you think there is some super smart individual cell monitoring goin on in your BMS
```

---
## \#13 Posted by: lowGuido Posted at: 2017-02-11T11:42:44.709Z Reads: 114

```
@benwong yes cut it. Its already connected via the main wires. its no longer necessary.
```

---
## \#14 Posted by: benwong Posted at: 2017-02-11T12:00:46.091Z Reads: 111

```
@lowGuido Okay. So i follow the step 1>2>3 to connect should be okay right? Hope that don smoke and burn my house.
```

---
## \#15 Posted by: lowGuido Posted at: 2017-02-11T20:03:42.341Z Reads: 99

```
Yeah just makebsure the B battery is connected to the B balance plug and vise versa. So many people get that wrong.
```

---
