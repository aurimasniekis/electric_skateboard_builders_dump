# Conformal coating direct FETS

### Replies: 15 Views: 594

## \#1 Posted by: telnoi Posted at: 2017-12-21T09:19:03.517Z Reads: 160

```
Planning on conformal coating my focboxes for added security against any moisture.
Is there a negative impact on heat dissipation when coating the direct FETs?

Bought the silicone type.
```

---
## \#2 Posted by: Kug3lis Posted at: 2017-12-21T10:11:19.956Z Reads: 152

```
yes, ofcourse... You need direct contact otherwise you will have no heat transfer...
```

---
## \#3 Posted by: telnoi Posted at: 2017-12-21T11:13:03.438Z Reads: 144

```
In a way, there is no direct contact to begin with. There is a thick layer of silicone based thermal tape in between the fets and the alu case, thus really wondering if a thin layer of silicone coating will mess things up.

There would still be contact between the tape and coating.
```

---
## \#4 Posted by: rene Posted at: 2017-12-21T11:35:21.317Z Reads: 141

```
maybe you wanna watch this

[https://www.youtube.com/watch?v=s4z8QMgTEA4](https://www.youtube.com/watch?v=s4z8QMgTEA4)
```

---
## \#5 Posted by: Kug3lis Posted at: 2017-12-21T11:58:04.286Z Reads: 132

```
Those pads are thermal transfer not simple silicone...
```

---
## \#6 Posted by: telnoi Posted at: 2017-12-21T13:28:28.168Z Reads: 119

```
k, I'll tape them off during the process. Thx for the help.
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-12-21T13:33:00.064Z Reads: 115

```
[quote="telnoi, post:3, topic:41614"]
In a way, there is no direct contact to begin with. There is a thick layer of silicone based thermal tape in between the fets and the alu case, thus really wondering if a thin layer of silicone coating will mess things up.
[/quote]

Siicone is terrible at transferring heat. That's why they use it on everyone's favorite wire: high strand count silicone insulated wire. It is so terrible at transfering heat that a soldering iron won't even melt it in most cases, wires have been known to wick up _inside the tube_ with no visible outward indication, and you can actually hold the wire near the stripped end while soldering without burning yourself in most cases.

 Yes, it will absolutely negatively affect the heat transfer between your fets and heat sink. There will be very little to no heat transfer between the fet and heat sink if you put silicone in there.
```

---
## \#8 Posted by: telnoi Posted at: 2017-12-21T13:35:17.347Z Reads: 108

```
Crap. You'd think that there is a gap in the market for single & dual VESC CNC machined cases with rubber sealing. :expressionless: :wink:..only crappy part is taking care of the connectors.
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-12-21T14:02:27.889Z Reads: 104

```
you could just take an assembled unit, wire it in like you normally would, and simply fill in any and all air gaps with Corning 737. that would eliminate fluid ingress and wouldn't affect thremal transfer to your heat sink. and 737 is neutral cure so you wont have deposits or even corrosion on your cheaper wires and heat shrink that often come built in with things.
```

---
## \#10 Posted by: banjaxxed Posted at: 2017-12-21T16:40:06.897Z Reads: 85

```
I have @Kug3lis cases, I plan on coating the pcbs but not the fets with acf50, heat shrinking the pcbs with sections cut out for the fets to press against the thermal tape supplied, the case itself will have a silastic type gasket sealant. Sugru the ports as needed
```

---
## \#11 Posted by: Kug3lis Posted at: 2017-12-21T16:41:37.045Z Reads: 80

```
I just used the kapron tape on everything what does not have touch inside but it's personal choice what to use ;)
```

---
## \#12 Posted by: Hummie Posted at: 2017-12-21T17:50:29.246Z Reads: 73

```
some of the best thermally transfering resin is silicone though and there's different types out there. as an example of the differences I was surprised the standard silicone at the hardware store sticks to practically anything (cells for one) while all the silicone I have for molds will stick to nothing,
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-12-21T19:29:54.789Z Reads: 62

```
after its been doped with something thermally conductive, sure.
```

---
## \#14 Posted by: Kug3lis Posted at: 2017-12-21T19:36:26.860Z Reads: 58

```
Guys, I suggest to not experiment with stuff you have zero understanding. Go read documentation of DirectFET package. It states it needs a really high Wattage capable heatsink as the package has not much metal on it as a buffer it will fry before it will be able to transfer heat to the heatsink.
```

---
## \#15 Posted by: banjaxxed Posted at: 2017-12-21T19:53:47.866Z Reads: 59

```
So lose the heat shrink otherwise as I posted above?
```

---
