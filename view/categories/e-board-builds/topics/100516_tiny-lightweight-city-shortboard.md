# Tiny lightweight city shortboard

### Replies: 6 Views: 424

## \#1 Posted by: kntzn Posted at: 2019-08-18T20:51:48.043Z Reads: 112

```
Hello everyone. 
After creating my first build and making it work i’ve successfully picked up so much knowlege that i’ve decided to create quite ambitious build that could be carried arround the city, it’s cafes and underground without any trouble, because you know that feeling when you are carrying 16-pound 1-meter long piece of wood with wheels in underground during the peak-hour: ![image|375x500](upload://3aiDtRtsdq1JtUzWK48NgamM74Z.jpeg) 

*my board is standing on the floor* 

So i decided not to only make a shortboard but to make it as lightweight as possible. I’m planning to use carbon fiber as the deck’s material, house the electronics inside the board and use a dual hub motors (because, let’s face it, direct drive for shortboard is kind of weird and pricy while belts and gears are noticeably heavier)

I want to use swapable 5s2p li-ion packs not only because they are smaller and lighter but also because you can easily take this pack with you in any plane (because it does not exceed the 100 Wh limit). At the same time, 110kv hubs  with 83mm diameter are capable to push you up to 18 mph which is enough when you are riding the overcrowded pavements of the Moscow city’s center.
Receiver and bms as well as remote are going to be custom-made like in my previous build. And two/dual VESC, obviously, as the ESCs

So there is my sketch with the hardware I want to use:![image|666x500](upload://nfEoum3WV3xeJ8OGVUAnCDipmqD.jpeg) 

Let me know what do you think about my concept.
```

---
## \#2 Posted by: pjotr47 Posted at: 2019-08-18T21:12:57.780Z Reads: 98

```
Skip that 5s2p pack. Go then for 10s1p. It has a higher efficiency & it is more universal. 

10s1p or 5s2p is the same amount off wattage
```

---
## \#3 Posted by: kntzn Posted at: 2019-08-18T21:23:11.018Z Reads: 92

```
Higly doubt the fact about the efficiency.

How high voltage can increase it? 

But I agree with you about it’s universality
```

---
## \#4 Posted by: Anubis Posted at: 2019-08-18T21:43:18.715Z Reads: 90

```
High current, high inefficiency. High current causes connections to heat up, high voltage does not. You need to change the motor kv though, 110 is far too high for 10S.
Edit: also the weight savings for carbon fibre decks aren't worth it. The price is very high and you save practically no weight. If you want true weight savings without shitty performance, go for a ~12S1P Samsung 40T (Or 13S LiFePo4, etc). 

Also a dual vesc would be massive overkill for a hub motor shortboard. You don't need that high a current, high quality ESCs exist which would be more suitable. 

Look into the Arc Aleiron, they do it really well. Lou board and Miles board don't ride well and have issues due to their internal enclosures and shortboard + carbon fibre + hubs.
```

---
## \#5 Posted by: kntzn Posted at: 2019-08-18T22:03:06.313Z Reads: 90

```
Ok, got you. 10s, 60kv.

I do not understand how 12x70g cells can be lighter than 10x48g. Also 40t are bigger. 

Default ESCs is defenetely not the way to go for me. For my first board i had to go over 3 ESCs. Only 4th controller for me works perfectly. And it’s name is VESC. I really can’t imagine the ESC that can not be configured the way iI want it to be.

And, finaly, about aileron. I love this board. But single drive is also not pleasant to ride at all. But may be, may be. 

Anyway, thank you for your reply and don’t forget it’s currently just a concept in my mind.
```

---
## \#6 Posted by: b264 Posted at: 2019-08-18T23:38:37.449Z Reads: 79

```
Did you see [the Blue One](https://forum./t/the-blue-one-12s-lifepo4-170kv-6374-caliber-2-30-43-powell-peralta-focbox/75)?  It's built to be a lightweight city shortboard and version 2 I am building now will be even better (including dual drive), so stay tuned :slight_smile:
```

---
