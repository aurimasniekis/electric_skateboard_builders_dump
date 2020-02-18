# Best Battery for 18560 1P pack for hubs

### Replies: 14 Views: 683

## \#1 Posted by: mrquin Posted at: 2018-03-25T05:52:46.881Z Reads: 166

```
I have a Lou board that can only fit a 10s1p pack so I want to know the group consensus for good battery cells. Should I use vtc6 or 30q or 25r or ...?? What the best balance of current vs capacity for a 18560 1p pack?
```

---
## \#2 Posted by: chuttney1 Posted at: 2018-03-25T06:47:28.206Z Reads: 163

```
It's the 30Q that's the best for the price for 18650. The VTC6 has better stats over the 30Q, but I don't remember if this cell is cooler than the 30Q.
```

---
## \#3 Posted by: E1Allen Posted at: 2018-03-25T06:49:09.895Z Reads: 161

```
So it has a Max output of 1500w according to the specs... But you have to draw over 40a to get that? Seems overrated.  Those 2.2a cells it currently has might be rated for 35a?  If you pick 25r or 30q they are both basically 20a batteries.  Even the vtc4 which was rated at 30a but performed as a 23a continuous cell isn't much of a improvement.  So I'm not sure what to tell you.  I'd just go with 30q or a custom 10s lipo.  Either way this board was meant for light riders and you're going to beat the snot out of those batteries regardless.
```

---
## \#4 Posted by: rey8801 Posted at: 2018-03-25T07:52:02.302Z Reads: 148

```
If you want to use the the all motor potential you probably need lipo otherwise the discharge current is gonna be lower than requested by the motor. Although this board is meant as last mile vehicle so if you want stay safer go for a lion and to me take the one with better e quality price. 30Q is the best but for this board I see the 25R better. Less capacity but you wouldn't probably ride to long with it anyway and cheaper than 30Q. Just my two cents.
```

---
## \#5 Posted by: E1Allen Posted at: 2018-03-25T08:03:51.995Z Reads: 137

```
I didn't think to consider the ESC maybe can't even handle 1500w that the motors put out
```

---
## \#6 Posted by: Namasaki Posted at: 2018-03-26T02:48:43.487Z Reads: 104

```
I'm gonna say Lipos as well.
You can have the discharge current you need in a more compact battery.
```

---
## \#7 Posted by: michaelcpg Posted at: 2018-03-26T02:58:26.248Z Reads: 99

```
20700A's? If you can find them
```

---
## \#8 Posted by: pat.speed Posted at: 2018-03-26T05:01:39.813Z Reads: 93

```
A123 lifepo is the way to go. 30-70 amp discharge
```

---
## \#9 Posted by: TarzanHBK Posted at: 2018-03-26T08:30:37.637Z Reads: 83

```
Don´t go with a 18650 with only 1p. You´ll destroy them pretty fast if you take more than 15A - 20A regularly out of this pack. Not to mention the enormous voltage sag.

Lipo or A123 lifepo in my opinion!
```

---
## \#10 Posted by: E1Allen Posted at: 2018-03-26T09:12:29.330Z Reads: 79

```
So for the price of the board compared to what he would spend on batteries it seems like lipo would be a cheaper option.  Looks like a fairly protected battery box as well.
```

---
## \#11 Posted by: TranxFu Posted at: 2018-03-26T11:27:07.119Z Reads: 75

```
The one in the Lou board has a 10a continuous discharge. Problem is that Lipo, A123 and 21700/20700 won't fit in there. I went with 10s1p 30Q just to reuse the BMS thats inside. But you could also fit 12/11s1p or 6s2p in there with a replacement drive train.
```

---
## \#12 Posted by: TarzanHBK Posted at: 2018-03-26T12:02:53.677Z Reads: 70

```
lol ok :smiley:
than you´re more than ok with a 10s1p 30q
```

---
## \#13 Posted by: E1Allen Posted at: 2018-03-26T17:03:23.041Z Reads: 57

```
With lipo you could still use the bms.
```

---
## \#14 Posted by: teapot Posted at: 2018-03-31T02:33:38.307Z Reads: 43

```
I dont know if anyone touched on this, but lipos are soft.. and you're basically stepping on your batteries with out the lou board is constructed.. I dont know if its a great idea. I have a Maxfind C that also only has space for a 10s1p configuration and the amount of amps the motor drew, destroyed my battery so we're both in the same boat here
```

---
