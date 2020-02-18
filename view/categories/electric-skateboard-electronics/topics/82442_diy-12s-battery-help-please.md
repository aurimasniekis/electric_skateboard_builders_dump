# DIY 12S Battery help please

### Replies: 29 Views: 474

## \#1 Posted by: stewie Posted at: 2019-01-29T02:24:15.765Z Reads: 114

```
sorry in advance because I'm gonna sound really stupid.

Since I live in Australia, a big ass country with not many people, building an esk8 is slightly problematic. Even though I live in a relatively urban area of Melbourne, I still have to do, like, 40 kilometres (24.8 miles) just to work and back. I'm currently building an eboard to make my daily commutes. I've got 4 3s 5000 mAh 40C Li-pos (https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-40c.html?___store=en_us) that I originally thought I could wire together in series for a 12s 20,000 mAh battery unit. Apparently If i wired those in series I would only get 12s but still 5000 mAh. My question is that how would I get a battery to meet my specs? if I wanted 20,000 mAh and 44.4V (12s) I would have to have 2x 12s 10,000 mAh to wire in parallel, or 2x 12s 20,000 mAh li-pos in series right? And, as far as I know those don't exist and even if they did they wouldn't fit in an eboard. I'm open to suggestions guys but I generally don't like putting together cells myself because of the extra equipment needed and various other reasons. Also, I would need a bms to charge via a single cable, so which one?

I've got a FOCBOX Unity and dual Torqueboards 6380 170kv Motors if that helps. 
ESC: https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc/
Motors: https:///collections/electric-skateboard-motors/products/electric-skateboard-motor-6380-170kv

Any help would be appreciated, Thanks!
```

---
## \#2 Posted by: SkaterBoy58 Posted at: 2019-01-29T02:31:26.314Z Reads: 107

```
what wheels do you have?
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-01-29T02:32:05.384Z Reads: 104

```
If you want a 12s4p pack of 3.7V 5000mAh lipo cells (which is what I think you are asking for, 44.4V 20,000mAh) then buy 2x of the 6s4p lipo packs from HobbyKing or something and put them in series...should go 60 miles on a single charge


TBH a 12s2p should be enough but won't give much margin of error for range, I'd go 12s3p

A lipo shouldn't have any issues with amperage if your wires don't melt

For that much capacity I would go for a li-ion pack, a 12s4p or 12s5p would be lighter, but you need to weld cells or buy a pack and you'd get less max torque and acceleration

In theory you would need a 12s8p to max out the motors
```

---
## \#4 Posted by: SkaterBoy58 Posted at: 2019-01-29T02:49:31.522Z Reads: 94

```
hobby king do  6S lipos up to 20 Ah 
A pair of these in series would give you 12S 20Ah - approx. 840Wh battery - which on AT wheels  at 14 Wh/km  would give over 60km range 

or a pair of 6S 16 Ah would give 48km range on AT wheels.

Street wheels are generally 8-10 Wh/km - so you can do the range calculation for that as well

![hobbey%20king|690x373](upload://sWS0CT3l3VpyH3e2Y1WjkMptDUA.jpeg)
```

---
## \#5 Posted by: stewie Posted at: 2019-01-29T02:56:40.153Z Reads: 81

```
I've got caguamas
```

---
## \#6 Posted by: stewie Posted at: 2019-01-29T03:02:03.354Z Reads: 82

```
Those look low profile from the search page but once you click into them they become Turnigy instead, and there's no way i'm fitting two of those onto a vanguard, but thanks nonetheless
```

---
## \#7 Posted by: stewie Posted at: 2019-01-29T03:09:05.380Z Reads: 77

```
Thanks dude but hobbyking dosn't sell any 6s2p or 6s4p batteries. Google told me that those lipos are very very very rare and outdated
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-01-29T03:09:27.549Z Reads: 76

```
@stewie 
For such a huge capacity, I'd definitely recommend going with 18650 cells rather than lipos. The resulting pack will be much smaller than a lipo pack of the same specs. 

Regarding your pack calculations, the key rule for figuring it out is, if you put stuff in **series**, you get more **voltage**, but no more capacity.
If you put stuff in **parallel**, you will get more **capacity**, but no more voltage. 

So for 3s 5000mah lipos, you'd need a total of (four in series) times (four in parallel), so sixteen packs. At the list price at that link, that'd be $580.
For a 12s and >20k mAH 18650 pack, you'd need a 12s7p of 30Qs, which is worth about $260.
```

---
## \#9 Posted by: stewie Posted at: 2019-01-29T03:12:31.337Z Reads: 73

```
uh, why 16 packs? dosn't four plus 4 equal 8 or am I missing something? You said times (four time four) but why is that? And with custom batteries, will the discharge be enough? does the speed of the motor depend more on voltage or amperes?
Thanks anyway dude,
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-01-29T03:13:02.020Z Reads: 71

```
It's multiplicative. Four packs in series, times four.
```

---
## \#11 Posted by: ZachTetra Posted at: 2019-01-29T03:16:19.632Z Reads: 70

```
Think of the batteries making a box, height/series gives voltage and width/parallel gives amperage/capacity, but it needs to be a complete rectangle to work
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-01-29T03:16:28.434Z Reads: 65

```
If you have a string of 4 packs of 3 cells in series and 5000mah capacity, that's 12s. To get double the MAH, you need twice as many cells in parallel, so eight packs to get 10,000mah.

To get double the MAH again, you need twice the cells AGAIN, so 12 sets of four cells. If they're in packs of three,  that's 16 packs.
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-01-29T03:18:13.099Z Reads: 57

```
30Q cells are good for 20 amps, times 7 in parallel is 140 amps. 

Speed is dependent on voltage. Acceleration and hill-climbing is dependent on current.
```

---
## \#14 Posted by: stewie Posted at: 2019-01-29T03:20:33.460Z Reads: 56

```
Yeah thanks man your math definitely checks out
```

---
## \#15 Posted by: stewie Posted at: 2019-01-29T03:27:36.755Z Reads: 56

```
If I used a 12s7p of 18650 cells, voltage wouldn't be a problem since 12*3.7= 44.4V (12S) right?

In the specs of my motor it says max amps is 80. The listings in the 30Q cells that I've seen are all rated at max 15 amps continuous discharge, 7*15=105, would both motors draw a combined 160 Amps or just 80?
```

---
## \#16 Posted by: MysticalDork Posted at: 2019-01-29T03:30:13.672Z Reads: 49

```
Battery amps =/= motor amps. Generally you'll pull less from the battery than is going to the motor. 50A in and 80A out is common.

30Q cells are factory rated at 15A, but they perform better at 20A than almost every 20A-rated cell.
```

---
## \#17 Posted by: stewie Posted at: 2019-01-29T03:32:33.101Z Reads: 48

```
Cool. Could you chuck me the link for those 30Q cells? 
Do I have to modify the cells to make them discharge 20A?
Thanks
```

---
## \#18 Posted by: MysticalDork Posted at: 2019-01-29T03:35:16.898Z Reads: 49

```
Nope, they'll do it on their own. https://ru.nkon.nl/samsung-inr-18650-30q-3000mah.html 

Keep in mind, you'll have to either get a spot welder, or get them welded together by someone else.
```

---
## \#19 Posted by: stewie Posted at: 2019-01-29T03:46:47.071Z Reads: 49

```
After a bit of digging I'm about to buy them now. A friend of mine's dad works at a University in mechatronics who's willing to let me use his spot welder. Just checking, how many cells will I need to make a 12s7p or 12s8p?
```

---
## \#20 Posted by: ZachTetra Posted at: 2019-01-29T03:48:06.469Z Reads: 46

```
Multiply the series count by the parallel count so 84 or 96 respectively...and buy some extra if a few cells go bad or get damaged somehow
```

---
## \#21 Posted by: MysticalDork Posted at: 2019-01-29T03:49:35.808Z Reads: 43

```
12x7 or 12x8. Get a few extra cells just in case you fuck up.
```

---
## \#22 Posted by: stewie Posted at: 2019-01-29T03:58:45.452Z Reads: 43

```
bloody hell thats 405 Autralia dollars plus another 80 for shipping but ok
```

---
## \#23 Posted by: MysticalDork Posted at: 2019-01-29T04:01:15.729Z Reads: 44

```
Still cheaper than 16 lipo packs. Big batteries are expensive.
```

---
## \#24 Posted by: mynamesmatt Posted at: 2019-01-30T00:57:32.338Z Reads: 38

```
Ay @stewie , in case you weren't aware, there's a huge esk8 scene in Melbourne. If you need some contacts dm me.
If you're doing a 40km round trip, id probably go 20km up, charge and 20km back. 
Turnigy (HobbyKing) have the Zippy FlightMax's in 2s config and 3s config at 8000mah. Depending what motor you run, you'll get between 25 and 35km out of it (at least i did). 
If you run 4 3s packs it'll get you to 12s 8000mah
if you run 6 2s packs it'll get you 12s 8000mah 

Just remember that the 3s packs are thicker than the 2s. you get me
```

---
## \#25 Posted by: AlexBE Posted at: 2019-01-30T01:39:00.784Z Reads: 35

```
There are a bunch of battery builders in Australia who can build you an 18650 pack to your specs and ship it to you. If you don't know what you are doing, don't try to weld one yourself.
```

---
## \#26 Posted by: totalgeek9224 Posted at: 2019-01-30T05:55:53.173Z Reads: 33

```
@TinnieSinker is based in Australia I believe, and he does custom batteries, maybe try messaging him for some first hand advice.
```

---
## \#27 Posted by: stewie Posted at: 2019-01-30T06:47:31.771Z Reads: 31

```
Thanks, Ill try look him up
```

---
## \#28 Posted by: stewie Posted at: 2019-01-30T06:48:08.779Z Reads: 31

```
Thanks dude ill probably hit you up once my board is done
```

---
## \#29 Posted by: mynamesmatt Posted at: 2019-01-30T08:06:02.488Z Reads: 31

```
No worries, there's a guy in Melbourne who can make you a bloody good motor mount so if you want his details hmu
```

---
