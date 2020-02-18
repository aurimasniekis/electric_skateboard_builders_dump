# 6S battery woes (6S thinks its a 5S)

### Replies: 7 Views: 806

## \#1 Posted by: Tonto2k Posted at: 2017-01-12T09:57:40.210Z Reads: 89

```
Hi all,

I have been using 2 x  Foxtech 5000mah 6S battery packs in series for my board. I have been charging each pack individually with a 6s B4AC pro charger.

Both packs have been fine for a couple of weeks now with regular usage.

Up until the other day, First 6S battery pack charges up fine but the second one no longer charges fully. It took ages to charge and I kept on getting "Vol Sel Err" as I tried to charge it.

I tried balance charging the lipo but it kept on giving the same "Vol Sel Err" error. This is a 6s Pack and I had it selected as 6S on my charger.

When I connect the balance lead to the charger it says something along the lines of "R.5 S.6" if I remember correctly?

This leads me to believe my 6S is being read as a 5S battery ?? The maximum voltage I can get in the pack is 20.8V.

So.... I connected a low votage alarm to check the cells, cells 1 - 5 were all ok but cell six gave "A.SS" reading, I can't find out what this means ?

Can anyone give me any advice please?
```

---
## \#2 Posted by: rwxr Posted at: 2017-01-12T10:43:58.040Z Reads: 81

```
Sounds like one of the cells is broken. Are all of the balance cables ok?
```

---
## \#3 Posted by: Tonto2k Posted at: 2017-01-12T11:29:17.794Z Reads: 71

```
Yeah I think so mate, I checked down to the heat shrink on the lipo itself. Can I use it as a 5s ?
```

---
## \#4 Posted by: rwxr Posted at: 2017-01-12T12:36:57.018Z Reads: 66

```
I wouldn't recommend it.
There could be a short or a wire glitch that could be triggered while charging or discharging the battery.

If you really want to use it as 5s you should remove the broken cell completely and rewire the balance leads to 5s.
```

---
## \#5 Posted by: Tonto2k Posted at: 2017-01-15T10:02:25.741Z Reads: 42

```
I ended up taking the pack apart today, one of the cells had worn on the ground back when I was using velcro to hold 2 x 6s batteries to the board !

It had worn on the corner of the lipo and one of the cells had leaked out. Thats why it would charge, it had lost all its mega-trons :frowning:

So today I removed the faulty cell and rewired as a 5s. I now have a perfectly servicable 5s pack.

Going to see what its like running on 11S !!
```

---
## \#6 Posted by: wmj259 Posted at: 2017-01-15T18:36:39.808Z Reads: 31

```
Did you make sure to wash /clean the other cells? I would have sprinkled on some baking soda and wiped off. 
So the velcro was able to cut through the lipos wrapping?

But that's good work,  you have pics of the work as you remove the dead cell? :clap:
```

---
## \#7 Posted by: Tonto2k Posted at: 2017-01-16T00:29:27.619Z Reads: 28

```
I never cleaned the other cells (probably should have), It was only the one cell on the outside corner.

Regarding the velcro, I had it holding on the battery pack to 2 x 6s battery packs. It had previously held 1 pack fine. The velcro couldn't hold the extra pack eventually though :frowning:

After driving along a fairly old pavement I heard a dragging noise. I stopped and saw the pack rubbing on the ground ! Luckily it had a hard metal casing on it. It seems one of the cells in the pack was still damaged though.

I never took any pics but I will next time I have the battery compartment open.
```

---
