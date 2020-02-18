# Correlation between capacity (%) and voltage (V) of Samsung 30Q 18650

### Replies: 8 Views: 1166

## \#1 Posted by: Eboosted Posted at: 2017-06-18T22:28:57.540Z Reads: 153

```
I'm trying to set this parameter as precise as possible on VESC monitor, have you guys found the correct correlation between this specific battery and the percentage of capacity?

[img]http://i.imgur.com/6kjjbCu.png[/img]

This was my first attempt, I used the capacity meassure in Ah at 5A from constant current discharge chart by Mooch

[img]http://i.imgur.com/rjjSaUG.png[/img]

<img src="/uploads/db1493/original/3X/6/1/61c2c3b02b68f16cde8da04b658d2bc4cb6cd04a.png" width="289" height="349">
```

---
## \#2 Posted by: Maxid Posted at: 2017-06-18T22:31:40.442Z Reads: 145

```
5A discharge is quite high already. You basically want the no load voltage for your measurements so look for 1 or 2A discharges. In principal this is the way to go though.
```

---
## \#3 Posted by: Eboosted Posted at: 2017-06-18T22:45:42.921Z Reads: 143

```
[quote="Maxid, post:2, topic:25638"]
5A discharge is quite high already. You basically want the no load voltage for your measurements so look for 1 or 2A discharges
[/quote]

Yeah but the idea is that at 5% you can barely keep it rolling and at 0% you reach cutoff end voltage and board can no longer move
```

---
## \#4 Posted by: Maxid Posted at: 2017-06-18T22:57:17.448Z Reads: 137

```
What does that have to do with anything? Your cut off can be set however you want.
For a 3P battery you are currently using voltages for a 15A discharge - that is a lot.
```

---
## \#5 Posted by: Eboosted Posted at: 2017-06-18T23:07:24.229Z Reads: 134

```
[quote="Maxid, post:4, topic:25638, full:true"]
What does that have to do with anything? Your cut off can be set however you want
[/quote]

Setting 5% with no load (as ssuggested) could lead you to think that you still have a couple of kilometers more of range before board dies, but as soon as you give it some throttle, sag would kick cutoff end turn off the board.

So that why I was suggesting to meassure capacity using the discharge map at 5A.
```

---
## \#6 Posted by: Maxid Posted at: 2017-06-18T23:13:04.743Z Reads: 125

```
But 5% is a completely arbitrary number that you chose just like you can choose the cut off. 
The voltage that is supposed to be measured is the no load voltage - not load at 5A voltage.
How many percents give you what distance is then up to you to find out.

This is like setting the time on your clock 5min early so you are not late to the bus. If you want that you could also just set it right and do the math in your head.

For a 30Q you low voltage end could also be well below 3.07V.
I use 2.8V for my 25Rs (never actually getting there but still)
```

---
## \#7 Posted by: Eboosted Posted at: 2017-06-18T23:17:42.660Z Reads: 116

```
That's correct, I need to find out how many miles I have left when cutoff start kicks in and how many miles I can ride before the the board turns off, that should be 5% and 0% respectively.
```

---
## \#8 Posted by: Winfly Posted at: 2018-11-03T05:17:25.202Z Reads: 54

```
just wondering. Have anyone found the golden voltage vs capacity numbers for 30Qs yet?
```

---
