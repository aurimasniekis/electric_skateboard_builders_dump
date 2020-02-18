# Changing 12s power to 10s?

### Replies: 11 Views: 453

## \#1 Posted by: sunnyD Posted at: 2018-07-12T08:01:47.545Z Reads: 102

```
Hello folks! I have a boosted v2 battery (12s1p A123 battery) and I was wondering if there is some converter of sorts that can dumb down the power a bit so that I can use my 10s ESC and Hub motors on it? Any advise welcome.
Thanks!
```

---
## \#2 Posted by: TarzanHBK Posted at: 2018-07-12T08:31:20.893Z Reads: 94

```
there are step down converter, but they are usually huge if you want to use our standard currents.
Better to use a suiting battery for your ESC, or a suiting ESC for your battery.
```

---
## \#3 Posted by: sunnyD Posted at: 2018-07-12T08:37:51.215Z Reads: 92

```
That would make sense. You think I could strip two batteries off the boosted battery and replace the bms to make it work?
```

---
## \#4 Posted by: rojitor Posted at: 2018-07-12T09:03:34.522Z Reads: 83

```
Li ion      10s X 4.2v= 42v
Lifepo4   12s X 3.6v= 43.2v
Where is the problem?
```

---
## \#5 Posted by: linsus Posted at: 2018-07-12T09:05:20.083Z Reads: 79

```
[quote="rojitor, post:4, topic:61628"]
ion 10s X 4.2v= 42v
Lifepo4 12s X 3.6v= 43.2v
Where is the problem?
[/quote]

This 10char
```

---
## \#6 Posted by: sunnyD Posted at: 2018-07-12T09:28:51.318Z Reads: 69

```
I guess the only problem is my math skills. So this will not make much of a difference? I’d be using a 12s bms, a 10s esc and 10s hub motors. XD
```

---
## \#7 Posted by: rojitor Posted at: 2018-07-12T09:58:23.787Z Reads: 65

```
Bms counts cells (and volts according to the chemistry). Esc counts volts. Since the difference is meaningless you will have no problem.
```

---
## \#8 Posted by: TarzanHBK Posted at: 2018-07-12T11:27:27.290Z Reads: 54

```
Your Esc has a voltage range for operation. If your battery is in it fully charged, you're good to go
```

---
## \#9 Posted by: sunnyD Posted at: 2018-07-12T17:24:25.242Z Reads: 37

```
Would there be some sort of limiter I could put in place in order to be sure it doesn't go over the right amount of charge?
```

---
## \#10 Posted by: boardman Posted at: 2018-07-12T23:19:22.099Z Reads: 28

```
If you switch to VESCS, I believe there is a way to run your motors at 10s.

Take a look:

https://www.electric-skateboard.builders/t/vesc-faq-limit-output-voltage-according-to-motor-maximum-specs/683

Edit: Accidentally shared wrong link at first
```

---
## \#11 Posted by: sunnyD Posted at: 2018-07-12T23:21:10.297Z Reads: 22

```
Okay cool. Ill look into that!
```

---
