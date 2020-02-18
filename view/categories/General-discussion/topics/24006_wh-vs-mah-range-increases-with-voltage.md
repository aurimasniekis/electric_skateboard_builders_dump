# Wh vs Mah /Range increases with voltage?

### Replies: 10 Views: 1134

## \#1 Posted by: IsTalo Posted at: 2017-05-27T16:27:49.489Z Reads: 101

```
Hello, I've calculated that I have a 140Wh battery, 6300mah=1000*Wh/22.2, but if I had a 10s battery the Watt hour would be higher, with the SAME mah, and here is my question, does a 10s 5000mah have a higher range than a 6s 5000mah battery?
```

---
## \#2 Posted by: Trans-amers Posted at: 2017-05-27T16:47:03.390Z Reads: 98

```
Short Answer: Yes
Long Answer:
Range(km) ≈ Battery Capacity (Wh)/10
10s 5000mah = 10*3.7V*5Ah=185Wh
Range ≈ 185Wh/10=18.5km
6s 5000mah = 6*3.7V*5Ah=111Wh
Range ≈ 111Wh/10=11.1km
```

---
## \#3 Posted by: IsTalo Posted at: 2017-05-27T16:53:11.426Z Reads: 99

```
But why it happens? Isn't Voltage=Power and Mah=Range?
```

---
## \#4 Posted by: anorak234 Posted at: 2017-05-27T17:31:14.158Z Reads: 94

```
Higher voltage is more watt/hours and a more efficient system. The higher you go, the more cells you have, the less strain is on each cell (less drawing of amperage). That's why a 12s1p pack could give you up to 2 or 3 times the range as a 6s1p.
```

---
## \#5 Posted by: IsTalo Posted at: 2017-05-27T17:39:32.431Z Reads: 83

```
Man, so 10 or 12s is always better in a Esk8, right?
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-05-27T18:07:33.420Z Reads: 79

```
If the ESC and motor can take it, pretty much.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-05-28T01:10:31.816Z Reads: 65

```
mAh is a good indication of range, but its not the whole story.

people prefer to use Wh for range because it levels the playing field a bit. a 6S battery would need to pull about twice as many Amps to match the performance of a 12S
so all things being equal (which they arent but whatever) a 12S 5000mAh is near enough to a 6S 10,000mAh range.

if that makes sense?
```

---
## \#8 Posted by: IsTalo Posted at: 2017-05-28T01:41:41.469Z Reads: 59

```
Yeah, it makes, and it's something thay everybody should know, because I saw people preferring 6s4p than a 12s2p
```

---
## \#9 Posted by: lowGuido Posted at: 2017-05-28T01:51:44.956Z Reads: 55

```
well an easy way of looking at it is how many cells?
12S2P is 24 cells and a 6S4P is 24 cells.. so its gonna be roughly same range.

however maybe they prefer a 6S4P so they can have a cheap ESC, or maybe the prefer a 12S2P so they can draw less current.

both work more or less the same. you could argue that 12S is more efficient because it draws less current and therfore there is less energy lost as heat... but it literally is 6 of one and half a dozen of the other.
```

---
## \#10 Posted by: IsTalo Posted at: 2017-05-28T02:09:51.274Z Reads: 51

```
That is something that was on my mind for months, and I think a lot of people have this doubt
```

---
