# JST lipo balancing with packs connected in parallel

### Replies: 6 Views: 177

## \#1 Posted by: Nedtrampz Posted at: 2019-05-28T16:00:02.017Z Reads: 56

```
OK, so i have 8x 6s lipo 3300mah. I want to make 4x 6s 6600mah. Then this will make 2x 12s 6600mah after connecting 2 in series. My charger has 2x 6s balance for charging 12s. So each 12s pack must be able to balance thru 2x 6s jst plugs.

My question is after connecting 2 packs in parallel, how do i then balance both packs through 1 6s jst plug? Is it possible? 

Its needs to be this way to actually work with the box i have.
```

---
## \#2 Posted by: 3LD Posted at: 2019-05-28T16:09:37.526Z Reads: 52

```
wire the balance leads of the 2 parallel 6s packs into a single jst connector(or make an adapter harness). 
Look at the "2x 3s parallel balance adapter" wiring diagram for reference.

http://www.tjinguytech.com/charging-how-tos/parallel-charging
```

---
## \#3 Posted by: Nedtrampz Posted at: 2019-05-28T17:02:32.052Z Reads: 32

```
Thats what i had in mind but i do worry over time that balancing in parellel wont enable proper balancing.
```

---
## \#4 Posted by: captclearleft Posted at: 2019-05-28T17:40:01.114Z Reads: 29

```
That's actually kind of a good idea.

I personally would not wire them up permanently.  I would make it so that they can be unplugged and re balanced.  Parallel charging (I am sure you know) has the effect of allowing one cell to be high, while another is low.  If you don't check them individually on occasion you could end up catching the thing on fire while charging or riding...  

To answer your question.  You would need to charge the 6s4p packs individually with a charger that can charge 6s packs, or...  [A Charger like this - That can charge 14s...](https://www.maxamps.com/graupner-polaron-pro-touch-screen-charger-14s-500w-20a)  

There might be a way to Just use a BMS like the Lion guys use in their setups.  Lipo packs are a little more sensitive than Lion, so be careful with that.
```

---
## \#5 Posted by: 3LD Posted at: 2019-05-28T18:32:39.384Z Reads: 28

```
If you're worried, go the adapter harness route, and then every month or so you can unplug the harness and balance each battery individually. 

Cells in parallel seem to self balance IME tho

edit: according to the page I linked, cells in parallel do balance themselves.

> How does it work you ask?
It's actually pretty simple. When you place all the packs in parallel, they all become the same voltage. I am not speaking in metaphors here, they really all do become the same voltage. Not the average of the packs either. Current actually flows between the packs and they actually all adjust voltage until they all perfectly match each other. The charger only "sees" one larger pack and charges it as if it were a single pack.
```

---
## \#6 Posted by: mynamesmatt Posted at: 2019-05-28T20:02:52.314Z Reads: 23

```
yes as mentioned above, cells in parallel will balance themselves. as you arent just putting the main leads in parallel but you're putting the balance leads in parallel too, all cells that are in parallel will Equalize.
```

---
