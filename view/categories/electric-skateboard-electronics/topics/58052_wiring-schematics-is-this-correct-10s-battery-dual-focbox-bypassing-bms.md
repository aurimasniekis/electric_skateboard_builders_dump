# Wiring Schematics- Is this correct? 10s battery &#124; Dual focbox &#124; Bypassing BMS

### Replies: 18 Views: 1076

## \#1 Posted by: J.Biggs Posted at: 2018-06-06T19:42:09.411Z Reads: 175

```
As the title states I would like to have someone check to see if my wiring is correct. 
Question 1: Is the loop key in the right place?
Question 2: Where does the voltage meter go?
Question 3: Will this bypass the BMS for discharge?

![Wiring%20V1|690x388](upload://erzOcLV737ANdGrg5XorRSJUJbl.jpg)

Here is the BMS

https://www.ebay.com/itm/282923151393?ul_noapp=true
```

---
## \#2 Posted by: b264 Posted at: 2018-06-06T20:12:56.198Z Reads: 149

```
No; you want the loop key on the negative line, between battery negative and ESC negative.  Also it helps to make thick lines 10AWG and thin lines 22AWG
```

---
## \#4 Posted by: b264 Posted at: 2018-06-06T20:15:42.172Z Reads: 148

```
Yes, this is in "bypass" configuration.  The voltmeter goes in parallel to the ESCs, just like if you had a third ESC, but it can use 22 - 26 AWG wire
```

---
## \#5 Posted by: J.Biggs Posted at: 2018-06-06T20:16:47.687Z Reads: 145

```
Thanks, I'll redraw it real quick. :grin:
```

---
## \#6 Posted by: J.Biggs Posted at: 2018-06-06T20:43:49.128Z Reads: 139

```
Does this look better?

![Wiring%20V2|690x388](upload://qDn2g6CBU0esuJGZHf7qUBPl1pB.jpg)
```

---
## \#7 Posted by: b264 Posted at: 2018-06-06T21:57:02.368Z Reads: 129

```
Yes; except the wire from the battery to the BMS "B-" doesn't have to be 10AWG because P- is not connected.  22AWG is okay
```

---
## \#8 Posted by: J.Biggs Posted at: 2018-06-06T21:58:13.828Z Reads: 124

```
Alright, thanks for the help.
```

---
## \#9 Posted by: b264 Posted at: 2018-06-06T21:58:37.727Z Reads: 117

```
Pay attention to the BMS if it starts "B0, B1, B2" or "B1, B2, B3"

Some need the B- to be the same as B0 and some start with the next cell for B1
```

---
## \#10 Posted by: Deckoz Posted at: 2018-06-06T22:00:30.547Z Reads: 115

```
I think it doesn't matter the side of the Antispark loop, plus I would rather leave my electronics grounded with the positive disconnected. Just my 2¢

The schematic looks good, but for future reference when drawing crossing wires, to designate they aren't connected, draw the wire like the Omega symbol as if the wire is "going over"
```

---
## \#11 Posted by: J.Biggs Posted at: 2018-06-06T22:05:40.891Z Reads: 109

```
Is there any way to tell which one it starts with or is it just trial and error?
```

---
## \#12 Posted by: b264 Posted at: 2018-06-06T22:09:46.529Z Reads: 112

```
Do you know which BMS it is or have a photo or both?
```

---
## \#13 Posted by: J.Biggs Posted at: 2018-06-06T22:12:07.676Z Reads: 111

```
I haven't bought it yet I was thinking about using this one.

https://www.ebay.com/itm/282923151393?ul_noapp=true
```

---
## \#14 Posted by: b264 Posted at: 2018-06-06T22:13:15.618Z Reads: 110

```
Yeah that one has 11 connections instead of 10, so B0 through B10 or 0V through 42V, as opposed to 4.2V through 42V

Your diagram only has ten balance wires and not eleven
```

---
## \#15 Posted by: J.Biggs Posted at: 2018-06-06T22:15:34.792Z Reads: 103

```
I'll draw it again, brb.
```

---
## \#16 Posted by: b264 Posted at: 2018-06-06T22:24:14.299Z Reads: 104

```
Also the series connections between the batteries need to be large wire
```

---
## \#17 Posted by: J.Biggs Posted at: 2018-06-06T23:00:40.922Z Reads: 99

```
So, when I was sketching I couldn't figure out which ground wire I needed to connect to B0. Could I get some help? 1 is for the main wire and 2 is the smaller one in the middle

![20180606_175250%5B1%5D|690x388](upload://oh4E6tsuxoA7ccddYbRcKOULsan.jpg)
```

---
## \#18 Posted by: J.Biggs Posted at: 2018-06-07T19:44:47.192Z Reads: 76

```
V3:  Alright, I think it's complete. Hopefully third times a charm. :sweat_smile:

![Wiring%20V4|690x388](upload://pwzMhtyXOPVyu5FSAnbdtyPUh21.jpg)
```

---
## \#19 Posted by: GUAN1111 Posted at: 2019-04-12T19:53:05.291Z Reads: 27

```
Hi, can anyone just take a quick look at this whirring and tell me if it is right(I will bypass the BMS). Do I nead the black whier form battery 2 to B- on the BMS?
this is the BMS i use.
https://www.ebay.com/itm/10S-36V-Lipo-Li-Ion-Batterie-Charger-Ladeger%C3%A4t-Schutz-BMS-PCB-Board-mit-Balance/263914313397?ssPageName=STRK%3AMEBIDX%3AIT&amp;_trksid=p2060353.m2749.l2649

Thanks ;-)

![Untitled|690x360](upload://t1tQssshfPQ0hdWRDT8g8PXx1yF.jpeg)
```

---
