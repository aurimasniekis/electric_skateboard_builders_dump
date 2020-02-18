# Different 18650 cells in series

### Replies: 4 Views: 265

## \#1 Posted by: paoloalb Posted at: 2018-06-20T10:59:22.363Z Reads: 75

```
Hi, I am new to making battery packs and I have some 18650 laying around. The problem is that these cells are not from the same batch, but from different manufacturers ( i extracted them from old laptop batteries). I want to make a 10s pack. I heard that connecting different cells could lead to problems, but if I use a BMS could this be a problem? Shouldn't the bms cut the current flow if a battery discharges? Should I try it or is it better to buy new cells?
```

---
## \#2 Posted by: AreaKruzer Posted at: 2018-06-20T11:15:43.009Z Reads: 68

```
It is better to buy new cells for this purpose. 

If done wrongly, you will put yourself in danger.
```

---
## \#3 Posted by: willumpie82 Posted at: 2018-06-20T14:31:42.415Z Reads: 49

```
I started this way 
- tested/Measured all cells (~200) (full charge, voltage hold test ~14days, discharge)
- combined a 10s3P pack of all > 2000mah cells (using https://secondlifestorage.com/repacker.php)
- use a smart BMS with logging capability

Result:
- The pack ran quite hot and a lot of sag
- there where two cell groups that where bad, more voltage drop than others
most laptop cells only have a max discharge of about 2A, check the datasheet and/or check https://secondlifestorage.com/celldatabase.php

I ended up buying 30 brand new 30Q cells (which have 15A discharge :smiley: ), no more sag, cool batteries
```

---
## \#4 Posted by: wafflejock Posted at: 2018-06-20T14:42:50.255Z Reads: 34

```
Save yourself the headache and potential board on fire situation get it done by someone who knows what they are doing with spot welding 18650 cells or someone who is willing to hold your hand through the process and get it right.  Not worth saving a hundred bucks or whatever if your whole board goes up like any of the board on fire posts, if something goes wrong you are likely to lose the board and anything attached to it (wheels included).
```

---
