# Lipo Voltage Difference when connecting in Series

### Replies: 11 Views: 481

## \#1 Posted by: florensvb Posted at: 2017-07-25T19:59:24.122Z Reads: 55

```
Hey guys, 

I just got two new Lipos from Ebay. I dont have a voltage meter at home, but I do have an LED battery indicator which showed me 57% and 64%. 

Problem is that my batteries came with a bullet connector and my charger has an xt60. I was hoping I could put them in series first and then charge them up, since I am going to put them in series and build my own charging adapter anyways. 

Question is: Is it ok to put them in series when they have ~7% difference? Also I am not sure how accurate my 5 bucks led indicator is haha

Whats the drill here?

Cheers !
```

---
## \#2 Posted by: SilentException Posted at: 2017-07-25T20:28:51.206Z Reads: 48

```
_dV_ doesn't matter when connecting in series. It will be one big unbalanced pack. Just don't "normal" charge them like this. Balance charge instead, until cells are balanced, which will take a while for such unbalanced pack :)
```

---
## \#3 Posted by: darkkevind Posted at: 2017-07-25T20:31:07.379Z Reads: 45

```
Do you have a balance charger? How many cells are there in each lipo pack?
```

---
## \#4 Posted by: florensvb Posted at: 2017-07-25T20:33:16.570Z Reads: 42

```
yes I have the SKYRC e8 100W balance charger and 2 x 4S 8000mAh Zippys :)
```

---
## \#5 Posted by: darkkevind Posted at: 2017-07-25T20:35:57.630Z Reads: 42

```
I would put them in series and then connect both 4s balance wires, although, do you have a 2 x 4s > 8s balance lead?

If not, charge them individually for now, it's the best way, then place them in series when you use them.

If you plan to just plug in your (one) XT60 from the series connection to charge in future, you'll need one of those adaptor leads.
```

---
## \#6 Posted by: florensvb Posted at: 2017-07-25T20:38:37.971Z Reads: 35

```
I was going to charge them up individually first but the thing is that i can not connect the bullet to the xt60 without soldering, and if i am gonna solder them anyways, might as well already do it the way the should be hooked up. for the balance leads i was planing on combining the 2 x 4s balance leads into one 8s balance lead, using a 15 pin VGA adapter
```

---
## \#7 Posted by: darkkevind Posted at: 2017-07-25T20:41:32.842Z Reads: 32

```
As long as you have the relevant JST connectors you can do that, but you need the right one to connect to your charger regardless of the 15pin VGA adaptor.

Do you have crocodile clips with the leads that came with your charger? Use those to connect to the main battery connections to charge.
```

---
## \#8 Posted by: darkkevind Posted at: 2017-07-25T20:42:49.488Z Reads: 27

```
You need an 8s one of these to connect to your charger...

<img src="/uploads/db1493/original/3X/e/6/e660b151a549de24cf52a3c8f0c582c180c51ce6.png" width="500" height="500">
```

---
## \#9 Posted by: florensvb Posted at: 2017-07-25T20:45:17.922Z Reads: 28

```
i dont think there were any crocodile clips. 

the charger did come with an 8s JST connector and a balance board, but the board only allows for 1 x 4S at a time. 

The leads from the charger have an xt60 at the end.
```

---
## \#10 Posted by: florensvb Posted at: 2017-07-25T20:47:04.943Z Reads: 27

```
[This is the link to the charger ](https://www.tomtop.com/charger-adaptor-1226/p-rm3758eu.html)
```

---
## \#11 Posted by: darkkevind Posted at: 2017-07-25T20:52:01.008Z Reads: 25

```
The best thing to do is solder an XT60 connector to that lead and be done with that.

But you still need a 2 x 4s to single 8s balance lead adapter.
```

---
