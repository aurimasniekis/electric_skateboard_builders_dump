# LED strip connection, wire size, receiver connection

### Replies: 11 Views: 1399

## \#1 Posted by: ninja Posted at: 2016-09-15T21:26:40.355Z Reads: 204

```
Hi, Builders! 
My setup will be: 2x 4s 8000mah, sk3 245kv, enertion vesc 4.12.  So i'm about to solder  wires, i'll be using 10 AWG wires for motor and also for battery harness. I don't know where to connect my 12v led strip. I'll be using voltage converter, so i'm going to use main battery to light up my led strip.

1) What size wires i need for that led strip before voltage converter, also 10 AWG? 
2) What kind of switch i can use for that led strip? 
3) Where That switch should be- before voltage converter or just before led strip (on that side where will be 12v)?
4) To which gt2b receiver channel i should connect vesc to?
<img src="/uploads/db1493/original/3X/e/b/eb1087cf2b2ac68ca40eca4a57c67f275e51cbcd.jpg" width="666" height="500">
```

---
## \#2 Posted by: ninja Posted at: 2016-09-16T12:33:26.273Z Reads: 162

```
Anybody? :)
```

---
## \#3 Posted by: michaeld33 Posted at: 2016-09-16T12:48:27.118Z Reads: 158

```
Connect it to the + and - wires of the battery, or connect it after the switch so you can turn it on and off.
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-09-16T12:48:48.356Z Reads: 159

```
Not sure about GT2B...
```

---
## \#5 Posted by: mccloed Posted at: 2016-09-16T15:10:07.304Z Reads: 152

```
Hey there, GT2B should be channel 2 for throttle. Channel one would be the steering.
```

---
## \#6 Posted by: ninja Posted at: 2016-09-16T17:18:40.137Z Reads: 144

```
Yeah, i will connect to +/-  of battery! But i want to know what size wires? Also 10AWG? So 10 AWG goes from battery to volt converter. After converter they are normal small wires for 12v led strip, am i right? Any way i want to put a switch for that led light, so where to i should  put it? I know that i can put it after converter where is 12v, it's simple any switch to 5A will do! But i don't want to that converter suck out power from my battery while i'm not using led lights. If i'll put it before converter i should use some monster switch with anti spark or what? Please, guys help me out.
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-09-16T17:37:23.609Z Reads: 137

```
It's not crazy amperage, so you should be able to get away with 12-16? Doesn't really matter.
```

---
## \#8 Posted by: ninja Posted at: 2016-09-16T18:58:28.544Z Reads: 135

```
So i can use 12-16 AWG for led lights? 
What about  switch right before voltage converter, what Amps for that? No need for anti spark there? 
Can i use just bullet connector as a switch for led or it will spark and damage electronics?
```

---
## \#9 Posted by: Ultimat3ging3r Posted at: 2016-10-20T23:49:09.708Z Reads: 117

```
12-16 awg should be fine going in and 18-20 coming out to led strips. Your better off using a switch or xt90 antispark better safe than sorry in my opinion. Your switch can be any where on that circuit, since it would be an open(or off) circuit while the switch is off your converter shouldn't be pulling any power. you have the exact same setup I have. But I'm wanting to know if you can hook them up to the vesc and turn them on and off with the remote?
```

---
## \#10 Posted by: Ultimat3ging3r Posted at: 2016-10-21T00:05:38.049Z Reads: 116

```
What are you using as your power converter?
```

---
## \#11 Posted by: ninja Posted at: 2016-10-22T21:31:31.503Z Reads: 107

```
I use this one:
 http://www.ebay.co.uk/itm/291692573003?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
