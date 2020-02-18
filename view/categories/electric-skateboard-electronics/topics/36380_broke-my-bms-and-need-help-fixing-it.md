# Broke my BMS&hellip; (and need help fixing it)

### Replies: 14 Views: 674

## \#1 Posted by: UltimaA380 Posted at: 2017-10-24T18:58:22.558Z Reads: 118

```
I bought a Supowerbattery BMS and it worked great, however after not using my board for a while because of a dead cell, I decided to build an 18650 pack. When taking my BMS out of the board to make some room and move it somewhere else, I noticed a chip on the side with half a resistor hanging off, I would like to fix it as there is no need to buy a whole new bms because of a component or two, I also noticed another component with a chip on the side, can anyone link me to the resistor and that component so I can solder it back on? Thanks. (all the bottom resistors are the same)

<img src="/uploads/db1493/original/3X/0/d/0d7053675fa338e74dfa33ac860b6737034ac926.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/4/0/4037fb3c3170cf3fb118eecd464c73872294701a.jpg" width="281" height="500">
```

---
## \#2 Posted by: Deckoz Posted at: 2017-10-24T19:41:08.289Z Reads: 101

```
Start by washing what looks to be flux off that board.

Iso wash = your friend
```

---
## \#3 Posted by: Fatos Posted at: 2017-10-24T19:48:09.857Z Reads: 99

```
Water??
It looks that that's the reason og a bad cell. If you didn't pay to much for it it's really noe worth the bother. 
But if you want to try, and if you manage to fix it use so. Water resistant spray on top of it when done :)
```

---
## \#4 Posted by: UltimaA380 Posted at: 2017-10-24T20:31:24.096Z Reads: 96

```
For the resistor I found this, could it be the right one? http://www.ebay.ca/itm/100PCS-0805-2012-SMD-Chip-Resistor-200K-ohm-200K-204-5-1-8W/391419762705?hash=item5b226f9811%3Ag%3AZrcAAOSw~bFWGnpv&_trkparms=pageci%253A30b40b8c-b8fa-11e7-a273-74dbd18057e3%257Cparentrq%253A501467c215f0aa12b3c44f7effff043c%257Ciid%253A7
```

---
## \#5 Posted by: MontPierre Posted at: 2017-10-24T21:37:59.335Z Reads: 83

```
Just serach for YouTube tutorials on smd soldering. It’s not too hard. I have broken 4.12 maytech vesc and I’m gearing up to change DRV myself ;)
```

---
## \#6 Posted by: UltimaA380 Posted at: 2017-10-24T21:49:02.097Z Reads: 74

```
I have absolutely no problem soldering it, I have quite a few years of experience. Just need component names and links :P
```

---
## \#7 Posted by: MontPierre Posted at: 2017-10-24T22:03:29.180Z Reads: 68

```
I think you can get so called Boom on GitHub - showing all components.
```

---
## \#8 Posted by: UltimaA380 Posted at: 2017-10-24T22:58:28.671Z Reads: 58

```
[quote="MontPierre, post:7, topic:36380"]
Boom on GitHub
[/quote]

Could you link me?
```

---
## \#9 Posted by: wafflejock Posted at: 2017-10-24T23:04:47.359Z Reads: 55

```
do people call the BOM (build of materials) the Boom? I haven't heard that but I work in a bubble.

https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC4.12_BOM.ods

^^ that's the BOM for the VESC dunno anything about this BMS though.

Working from the board itself that resistor you linked looks correct but can also measure the dimensions of the existing ones to make sure it's right (usually they are 02x04 or 03x06 I believe).
```

---
## \#10 Posted by: MontPierre Posted at: 2017-10-24T23:23:34.353Z Reads: 52

```
Sorry autocorrect .... and the 5 beers I had - didn’t help ;) 

@UltimaA380 see if you can find some documentation for bms online. If not, perhaps Unsolder good resistor of same shape and check it’s resistance ? As a last resort!
```

---
## \#11 Posted by: UltimaA380 Posted at: 2017-10-24T23:36:16.678Z Reads: 52

```
I believe the resistor I linked is the correct one as I tried checking with a multimeter as well. One question though, above the resistor there is a 3 pin component (SOT maybe? Im not sure) How would I know what to get for that? Or is it even broken? just looks like a chip on the plastic
```

---
## \#12 Posted by: wafflejock Posted at: 2017-10-24T23:42:38.867Z Reads: 53

```
Not sure off hand, I'd guess maybe voltage regulator but yeah if you can just find a schematic for a BMS (or maybe even just lipo charger) can probably get an idea of what goes where in terms of components.  I know you can typically test different legs of a component off the board to see if it's open or closed or shows resistance between the "correct" legs but how you test exactly depends on if it's a BJT or MOSFET or whatever, my guess is some sort of linear voltage regulator but really not sure how to test.

---

Can probably find vids on identifying smd/smt components but know there are vids on how to test if they have failed on the youtubes, only downside is you need to take them out of circuit typically to test.

---

Edit 2 could also just do a comparative test with one that looks good just see that it has the same "characteristics" (continuity and resistance between the legs is the same between "known good" and "suspected bad")
```

---
## \#13 Posted by: UltimaA380 Posted at: 2017-10-25T14:54:11.937Z Reads: 30

```
Still looking to find out what that 3 pin component is, guessing not a voltage regulator because looks nothing like it, maybe sot but have no idea how to find out or get values. :(
```

---
## \#14 Posted by: UltimaA380 Posted at: 2017-10-25T22:32:45.247Z Reads: 23

```
So, I managed to find out what all the parts were, thank you guys for your help :)
```

---
