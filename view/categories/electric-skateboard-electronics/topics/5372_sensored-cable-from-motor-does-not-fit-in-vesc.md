# Sensored cable from motor does not fit in VESC

### Replies: 13 Views: 2249

## \#1 Posted by: WrinklyWink Posted at: 2016-06-30T09:03:13.952Z Reads: 326

```
the sensored cable from my 6355 motor is small (10.43mm wide male) while the female connector on my vesc is about 12.85mm wide. How may I connect the sensored cable without having to cut and solder? I tried looking online for an adapter piece but I don't even know where to begin my search terms. I've search the forums here and there but I haven't read anything about the sensored cable-connector discrepancy. Does anyone know how I might fix this problem?

Please help me
```

---
## \#2 Posted by: karma Posted at: 2016-06-30T14:43:46.089Z Reads: 289

```
You will need to get new connectors and solder them on.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-06-30T14:58:23.909Z Reads: 285

```
If you really don't want to solder anything, you can use these 06KR-D6S-P (6pin 2mm Jst connector KRD series. http://www.digikey.ca/product-detail/en/jst-sales-america-inc/06KR-D6S-P/455-2674-ND/2797509). But you will need to cut the wire.
```

---
## \#4 Posted by: Kaly Posted at: 2016-06-30T16:52:32.982Z Reads: 272

```
That's what I did to my motors and is 100% worth it. Make sure you plug it in the right direction otherwise the VESC will not recognize the Hal sensors.
```

---
## \#5 Posted by: WrinklyWink Posted at: 2016-06-30T18:11:06.757Z Reads: 255

```
do I do the exact same order? is it aligned the same way as the other connector or do I need to flip it? I'm ordering it right now.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-06-30T18:17:59.276Z Reads: 250

```
Exact same order
```

---
## \#7 Posted by: Freddiecook Posted at: 2017-04-01T13:45:06.978Z Reads: 173

```
So does that mean I should wire it up like so? Even if the colours don't match?
<img src="/uploads/db1493/original/3X/e/f/ef014fa8fd36558bf12bf96e973d2f8c2da6c8a5.JPG" width="666" height="500">
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-05-13T20:51:30.853Z Reads: 150

```
What did you do? I'm having the same problem.
```

---
## \#9 Posted by: Freddiecook Posted at: 2017-05-14T21:19:44.851Z Reads: 143

```
I haven't done it yet but I'm just going to solder them together like I showed in the picture
```

---
## \#10 Posted by: flywithgriff Posted at: 2017-05-14T21:20:30.722Z Reads: 144

```
Don't! That's the wrong order.
```

---
## \#11 Posted by: WrinklyWink Posted at: 2017-05-15T08:08:32.279Z Reads: 136

```
check out the image here: diy-electric-skateboard-kits-parts/vesc-sensor-wires/
it shows the right order. Green and yellow are swapped.
```

---
## \#12 Posted by: Bataleon Posted at: 2017-05-15T11:57:33.132Z Reads: 135

```
Only the GND (black) and VCC (red) need to match. It doesn't look like there's a temprature sensor, so the remaining wires can be connected in any order.

Once connected, launch the BLDC Tool, click _"Motor configuration"_ tab, then select _"BLDC"_ and click _"Start detection"_ (labelled 1). The results of the hall sensor order will then need to be entered into the Table (labelled 2).<img src="/uploads/db1493/original/3X/5/c/5cc3aeaa9e51c320dc547ffcfbabf791451aedc5.jpg" width="690" height="368">
```

---
## \#13 Posted by: venom121212 Posted at: 2019-02-03T13:48:28.171Z Reads: 36

```
Update for anyone having this issue

https://www.electric-skateboard.builders/t/gauging-interest-sensor-wire-extension-cables/82598?u=venom121212
```

---
