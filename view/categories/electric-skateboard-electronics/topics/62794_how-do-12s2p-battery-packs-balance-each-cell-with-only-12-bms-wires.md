# How Do 12S2P Battery Packs Balance Each Cell with Only 12 BMS Wires?

### Replies: 6 Views: 285

## \#1 Posted by: walleywalker Posted at: 2018-07-25T03:38:54.618Z Reads: 106

```
I'm sure this is awfully simple, but it is eluding me. 

How do the 24 cells in a 12S2P get individually balanced by the BMS if there are only 12 leads to the pack?
```

---
## \#2 Posted by: PatRocks Posted at: 2018-07-25T03:50:42.954Z Reads: 105

```
Parallel cells balance themselves
```

---
## \#3 Posted by: walleywalker Posted at: 2018-07-25T03:59:20.646Z Reads: 99

```
Ahh!! Like magic, thank you!!
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-07-25T06:53:08.744Z Reads: 90

```
elaborating on what @PatRocks said, yes they do balance themselves. When cells are in parallel their voltage together between + & - are the value of one cell. the only difference being the current output and capacity. So when the cells are parallel, the bms essentially only reads the voltage which will be 3.7v. If the cells are slightly different in voltage, then they leak a little bit of power into the other cell until they're level. 
Eg. an 18650 cell is nominal at 3.7V. Lets say its a 30q so its about 2500mah (capacity) and can spit out 30A. So, between negative and positive, the two batteries in parallel will still be 3.7V. However, as there are 2 in parallel, it essentially becomes a single battery that is 5000mah (2x2500mah) and can produce 60A (2x30A).
Hope this helps
```

---
## \#5 Posted by: walleywalker Posted at: 2018-07-25T14:49:09.129Z Reads: 68

```
yeah that totally helps. Now if you have a damaged cell, that for what ever reason doesn't allow the pair's voltage to reach 3.7v (for example) then will the BMS if it's doing its job properly, stop charging all together? Or if it's a fancy BMS throw some kind of error code?
```

---
## \#6 Posted by: marsrover001 Posted at: 2018-07-25T16:46:52.768Z Reads: 49

```
That pair will balance each other out (so one will be limited by the capacity of the other).

It might look like it charges up to 4.2v/cell, but if you ride it a bit and notice some serious sag, check each cell group and you might find one much lower than the others. That's how you'd know there's a bad cell in that group. Most people replace the whole group, but you could take it apart and put each one on a single cell charger and figure out which one is bad.
```

---
