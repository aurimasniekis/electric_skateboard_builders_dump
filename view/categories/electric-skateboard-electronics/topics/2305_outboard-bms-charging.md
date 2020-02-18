# Outboard BMS charging

### Replies: 14 Views: 1771

## \#1 Posted by: makepeace Posted at: 2016-04-12T07:06:03.691Z Reads: 197

```
Hi all,

I want to know if it's possible to charge my 8s LiPo battery by including a + and - terminal as well as a balance charge receptacle on the battery enclosure of my board. The + and - terminal will be connected across the battery leads, ie in parallel with the power switch and ESC part of the circuit. I would then have an out board 8s BMS to which I will connect the + and - terminal on the board as well as the balance charge terminals. I would then plug a normal charger into the BMS.

The BMS I plan to use is this one:
http://www.batterysupports.com/28v-29v-30v-30a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-262.html

And the charger is something like this one:
http://www.fypoweradapter.com/eproduct.asp?BigClassID=2&cid=16&nid=65

What do people think about this?

The idea here is that all I'll have on my board is the batteries, ESCs, receiver and a + and - receptacle and balance receptacle and I could just plug the BMS + charger directly into my board when I want to charge.

As a side note, the idea here is to optimise charging to be the cheapest, easiest and fastest, in that order.

Any advice would be greatly appreciated.
```

---
## \#2 Posted by: massy Posted at: 2016-04-12T08:54:56.324Z Reads: 177

```
I guess it should work, but be careful connecting the BMS, doing it in the wrong order may cause it to burn the BMS. I'm going for a mounted BMS myself and will balance charge in a lipo balance charger every now and then just to be safe.
```

---
## \#3 Posted by: lowGuido Posted at: 2016-04-12T10:35:11.450Z Reads: 166

```
isn't that just called using a balance charger?

rhetorical question. It is.

that's what myself and hundreds of others do every day. although keep in mind one of the benefits of a BMS is that it will stop you from over discharging accidentally.
dont waste money on a BMS unless you are putting it on the board... that's what they are for.
```

---
## \#4 Posted by: makepeace Posted at: 2016-04-12T10:50:21.322Z Reads: 155

```
Agreed, but show me a wall powered 8s 10 A balance charger for less than $60? Please. It would make life lots easier. ;)

Oh yes and I have another far lighter, smaller and cheaper plan for over-discharge protection.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-04-12T10:59:37.891Z Reads: 148

```
touché

-----------------------
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-04-12T14:40:12.637Z Reads: 131

```
Does it make noise and look like a volt meter?
```

---
## \#7 Posted by: makepeace Posted at: 2016-04-12T15:00:50.981Z Reads: 131

```
No! It uses a programmable brain board thingy to make magical rainbow light emenate from a plastic eye poking from the deck and trips my power switch circuit when it's tired. And probably sends some stuff via the invisible spectrum to my hand held telephonic robot to tell me how long it can go on for.
```

---
## \#8 Posted by: makepeace Posted at: 2016-04-12T15:02:05.873Z Reads: 131

```
But for reals, is there such a thing or am I wasting my life on this. I'm totally open to ideas.
```

---
## \#9 Posted by: Kaly Posted at: 2016-04-12T17:28:57.116Z Reads: 129

```
 This should work fine. 
make sure to make a enclosure for the BMS.
```

---
## \#10 Posted by: lowGuido Posted at: 2016-04-12T23:02:14.331Z Reads: 124

```
you are right. you can use a BMS externally to charge, and it will probably save you a bunch of cash on a charger.
my previous comments were under the assumption that every one has 1 or 5 battery chargers lying around.
```

---
## \#11 Posted by: Bender Posted at: 2016-07-17T14:05:37.998Z Reads: 104

```
I'd really like to do outboard BMS charging does anyone have a wiring diagram?
```

---
## \#13 Posted by: makepeace Posted at: 2016-07-17T14:47:03.574Z Reads: 98

```
The way I thought of it:

Board with balance lead jack and HV+- jack connected to your batteries, with the low side MOSFET switch on the VESC side of the HV jack. This will put the charger and batteries in "parallel", so to speak, from the view of the MOSFET switch/VESCs etc.

Charger connected up to BMS charging terminals, balance plug out to board, HV plug out to board.

With he switch on your board off, plug in the HV and balance leads, plug charger into wall and away you go.

Could probably even do it relatively safely while the board is on, but be careful to not draw too much current or you'll pop stuff.
```

---
## \#14 Posted by: Bender Posted at: 2016-07-18T13:33:15.025Z Reads: 88

```
Thanks @makepeace
What does HV stand for?
Sorry to be so ignorant
```

---
## \#15 Posted by: makepeace Posted at: 2016-07-18T13:56:52.285Z Reads: 84

```
High Voltage ie the positive and negative terminals of your total battery (with all of the cells in series or whatever).
```

---
