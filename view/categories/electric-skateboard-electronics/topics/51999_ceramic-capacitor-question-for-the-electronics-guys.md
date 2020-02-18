# Ceramic capacitor question for the electronics guys

### Replies: 11 Views: 385

## \#1 Posted by: danielz Posted at: 2018-04-12T02:28:15.156Z Reads: 69

```
I dont know if this is the right place to ask this question but here goes.

I was reading the drv8302 spec sheet, and if i understood it correctly(Thats a big if) it recommends a 4.7uf cap of its various supply inputs.

I looked at the bom for the 4.12 vesc and the caps used are package 1206 50v 10uf UMK316BBJ106ML-T. However on its spec sheet it states at 40-50v the capacitance is -90%! so only 1uf.

I see people upgrading the caps to 1206 100v 4.7uf, for example the 12061Z475KAT2A but after looking at its spec sheet. Even they dont fair much better at -70% 40-50v so only 1.4uf...

Am i missing something? or does the capacitance not matter so much for the transients? maybe the drv spec sheet takes into account all this when recommending the 4.7uf.

Im considering either stacking 2x 1206 100v 4.7uf or 1 x 10uf 100v package 1210 package assuming the extra width will fit.
```

---
## \#2 Posted by: JLabs Posted at: 2018-04-12T02:49:18.883Z Reads: 57

```
Calling @JohnnyMeduse
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2018-04-12T02:51:59.268Z Reads: 55

```
Deflecting it on @Blasto
```

---
## \#4 Posted by: JLabs Posted at: 2018-04-12T02:58:11.238Z Reads: 51

```
![image|690x158](upload://ys7FJOkUgvtB1ervWkyhMCBYw00.jpeg)

@JohnnyMeduse that’s not allowed! Your tag says DRV Wizard, I’m putting @psychotiller’s mom on you!
```

---
## \#5 Posted by: danielz Posted at: 2018-04-12T02:58:53.341Z Reads: 49

```
I just noticed there are few in parallel on the vesc schematic :laughing: That explains it and makes sense doh. 2 x 50v and 1 x 100v, not sure why not 3 x100vs. No doubt something else i dont understand yet lol. Its all very interesting though.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2018-04-12T03:10:17.355Z Reads: 46

```
[quote="JLabs, post:4, topic:51999"]
Your tag says DRV Wizard
[/quote]

Yeah.... NOT CAPACITOR WIZARD..... :joy::joy::joy: 

@danielz but the higher rated voltage the better, but I think 1206 10uF 100V doesn't exist :thinking:
```

---
## \#7 Posted by: Deckoz Posted at: 2018-04-12T03:37:26.173Z Reads: 42

```
[quote="JLabs, post:4, topic:51999"]
DRV Wizard
[/quote]

![i-takes-it-off-and-i-puts-it-on|582x326](upload://dOmfo3Yzzw6WzggbU7oBZ0jhyOU.jpg)
```

---
## \#8 Posted by: pat.speed Posted at: 2018-04-12T04:02:38.254Z Reads: 36

```
Maybe this is one of @chaka’s mods that help improve reliability, adding higher uf caps
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-04-12T04:05:01.756Z Reads: 33

```
Chaka mod was 4,7uF 100V and 2 X 15uF 100V, but as I experiment in a few time it is not a bullet proof upgrade.
```

---
## \#10 Posted by: danielz Posted at: 2018-04-12T04:06:13.160Z Reads: 32

```
1210 :smiley:
```

---
## \#11 Posted by: danielz Posted at: 2018-04-12T04:07:05.798Z Reads: 32

```
I need me an oscilloscope!
```

---
