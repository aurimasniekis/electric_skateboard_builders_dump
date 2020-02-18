# Is this a bad idea?

### Replies: 12 Views: 1177

## \#1 Posted by: Pantologist Posted at: 2017-02-26T00:38:22.044Z Reads: 165

```
I've got these Ryobi batteries super cheap. They are Samsung 20Q 2000 mAh 15A cells which is kind of a bummer. 

[Datasheet](http://gamma.spb.ru/media/pdf/liion-lipolymer-lifepo4-akkumulyatory/INR18650_20Q.pdf) 

So here are some pictures of the cells in their current layout. 
<img src="/uploads/db1493/original/3X/5/4/5499bc250290ab20f92fa8f9459af5bc031b6c36.jpg" width="690" height="425"><img src="/uploads/db1493/original/3X/a/1/a1f7042b754b56dee4277194c22ef8fe6b9310c1.jpg" width="690" height="384"><img src="/uploads/db1493/original/3X/b/d/bd1e6ea695e82640b79c24f4f1c4890010fac161.jpg" width="663" height="499"><img src="/uploads/db1493/original/3X/9/e/9e6e88a2538c89086e510c778f28be7cbb13ee88.jpg" width="690" height="422"><img src="/uploads/db1493/original/3X/8/d/8d2dea75a398561d97eeeb22f0c4de7728a598e2.jpg" width="548" height="500">



This is my plan for the final layout for putting two in parallel to have a 8Ah pack. 

<img src="/uploads/db1493/original/3X/5/b/5b40e4f6531eb145ef6f0409177186f3e142cacf.png" width="607" height="500">
```

---
## \#2 Posted by: barajabali Posted at: 2017-02-26T00:40:37.376Z Reads: 158

```
why is it a bummer?
```

---
## \#3 Posted by: TranxFu Posted at: 2017-02-26T00:45:42.248Z Reads: 153

```
I don't think you can reach 36v/8ah with just 20 of these(as far as I can tell). You'd need a 10s4p. This puts 4 of these in parallel to get 4x 2000mah = 8ah.

Or do you happen to have 2 of these packs which adds up to 40 cells ?

::// and 15A is not bad at all. It'll add up to 60A continuous.
```

---
## \#4 Posted by: Pantologist Posted at: 2017-02-26T00:49:58.913Z Reads: 148

```
Sorry I forgot to mention that I got two packs. 

@barajabali I thought these batteries would have a higher discharge rate than that. Still great cells.
```

---
## \#5 Posted by: TranxFu Posted at: 2017-02-26T00:53:29.914Z Reads: 138

```
I guess, why not :) Go for it. Check voltage and balance beforehand. 

Just noticed these can be grabbed for 25$ 18v pack... Not that bad of an deal. And 20Q should definitely be usable in eSkate.
```

---
## \#6 Posted by: Pantologist Posted at: 2017-02-26T00:54:25.908Z Reads: 134

```
This is the 40V version. Ryobi Model number OP4040 in case you wanted to check em out.

Basically just two 18V 4Ah packs in series.
```

---
## \#7 Posted by: boards Posted at: 2017-02-26T02:13:35.601Z Reads: 116

```
15 amps per cell is actually pretty good!
```

---
## \#8 Posted by: rpn314 Posted at: 2017-02-26T05:19:57.987Z Reads: 106

```
Indeed. Only a little behind the Samsung 25R's that we frequently use, so a few in parallel should be fantastic!
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-11-25T20:54:35.300Z Reads: 61

```
Sorry to dig this up. Winter is here and I have an itch :slight_smile: I have a bunch of Ryobi batteries that seem to have defective bms’s. The pack and parallel group voltages look promising. I have one more of these p108’s and two smaller packs to take apart still. Did you go through with it? Did they perform ok?
<img src="/uploads/db1493/original/3X/9/9/99ebe45242bdcc190906a672fca0322eb07fef6e.jpg" width="375" height="500">

Not sure of the smaller packs use 20q’s too but if they do I have about 60 cells and would hope really for an 10s4p or maybe 5p if the cells check out.

Thanks for any feedback.
```

---
## \#10 Posted by: Pantologist Posted at: 2017-11-26T00:38:32.398Z Reads: 46

```
I would try to get a data sheet on those exact cells. Are you planning on leaving the cells in there current welded configs? If so it might be hard to integrate a BMS. Taking the welds apart is so time consuming as well so be sure a 10s4/5p pack would be sufficient for the high max current you need..
```

---
## \#11 Posted by: scepterr Posted at: 2017-11-26T00:41:10.244Z Reads: 44

```
The 13P and 20P get horribly hot at 2-3A loads
At least the 200 or so I've harvested
```

---
## \#12 Posted by: i2oadsweepei2 Posted at: 2017-11-26T10:41:47.552Z Reads: 24

```
 I'll take a look for a data sheet. I'm going to start charging the parallel pairs and see how that goes with my Hyperion duo. Hoping to leave them in their bulky bricks and just run them as 2 x 5s 4p packs for charging. I think I can actually stuff four of them into my psychotiller flagship enclosure with one vesc-x. 

*edit* I found the spec sheet for them here http://lygte-info.dk/review/batteries2012/Samsung%20INR18650-20Q%202000mAh%20%28green%29%20UK.html
```

---
