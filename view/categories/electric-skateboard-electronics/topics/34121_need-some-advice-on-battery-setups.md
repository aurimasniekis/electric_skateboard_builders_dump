# Need some advice on battery setups

### Replies: 7 Views: 548

## \#1 Posted by: Orin635 Posted at: 2017-09-27T21:50:43.489Z Reads: 67

```
Ok recently finding out that my understanding of lipo batteries was wrong (which now thinking back my understanding made no sense) I thought 2x 3s 5000mah 20c lipos would equal 6s 10000mah battery 20c but I now know its either 3s 10000mah or 6s 5000mah (with double the output) I would prefer more range so id like to go with 3s 10000mah. the esc I am using can take 2-6s lipos so I am wondering will a 3s 10000mah 20c battery supply enough juice to power my parts

parts
Motor- Turnigy Aerodrive SK3 - 5055-280KV Brushless Outrunner Motor            (says it needs 6-10s lipos :/)
ESC: HobbyKing® ™ X-Car Beast Series ESC 1:8 Scale 120A
Batteries: 2x Turnigy 5000mAh 3S 20C Lipo Pack

Forgot to say that i think i worked it out that 20c 5000mah lipo would output at 100amps and my motor only needs 60amps but im not sure if that is important.
```

---
## \#2 Posted by: rich Posted at: 2017-09-27T22:53:10.162Z Reads: 59

```
Definitely go with 6S, 3S is way too low!
You can charge both lipos with a 6S balance charger at once, you can find info in this forum how to do the correct wiring for that.
[quote="Orin635, post:1, topic:34121"]
20c 5000mah lipo would output at 100amps
[/quote]

That's right!
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-09-27T22:59:10.201Z Reads: 50

```
You won't get more range from 3s 10ah than from 6s 5ah, because the energy in the pack is the same either way (3*3.7*10 one way 6*3.7*5 the other, same results).

Dropping from 6s to 3s will cut your speed in half, and if you don't change anything else in your board, it'll also reduce your power. You'll still go just as far, but you'll have no power and no speed.
```

---
## \#4 Posted by: Orin635 Posted at: 2017-09-27T23:09:16.900Z Reads: 48

```
Ok thanks so wire it in series?
```

---
## \#5 Posted by: Orin635 Posted at: 2017-09-27T23:09:44.527Z Reads: 48

```
I'm planning on using a bms instead but thanks anyway
```

---
## \#6 Posted by: rich Posted at: 2017-09-27T23:16:47.429Z Reads: 44

```
That's the best solution :grin: go for BMS for discharge, too. I killed my 10S 10000maH Lipo a couple of days ago because I forgot to switch off my board and 28 hours later the cell voltage dropped from 3.5 to 0.9V, the lipo is puffed and dead. I used my BMS for charging only, bad idea :cry:

Wire the 3s lipos in series.
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-09-28T00:42:35.043Z Reads: 37

```
Yep. 10chars
```

---
