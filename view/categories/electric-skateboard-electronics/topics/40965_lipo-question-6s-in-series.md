# LIPO Question (6s in Series)

### Replies: 6 Views: 509

## \#1 Posted by: coderman Posted at: 2017-12-13T23:42:37.686Z Reads: 60

```
So I bought this battery from ebay:https://www.ebay.com/itm/352226705515
If I wire them in series, what should be the cutoff start and end voltages? Im not sure how to calculate it for 12s in this specific setup, and I really dont want to brick the battery. I'm fairly sure that it should be 3.3V per cell minumum. however I'm not completely sure how to get the cutoff start and end voltages from this. if 3.3 is the right number should I do 3.3*12 to get the cutoff end? and maybe something like 3.4*12 to get the cutoff start? thanks in advance for clarifying for me!
```

---
## \#2 Posted by: Martinsp Posted at: 2017-12-13T23:55:24.318Z Reads: 57

```
You pretty much have it.
the cut off end is the voltage when your VESC turns off to prevent the battery from being damaged due to over discharging.
the cut off start is the voltage when your VESC limits the power output so that your voltage does not sag too much and also it will give you a little bit more range with slower speed.
So 3.3*12 is 39.6V Set this to cutoff end
and if you want to you can set 3.4*12 or whatever higher than 3.3*12 as your cutoff start, this is just your choice so you can for example want the limit power when at 30% if the battery which in this case would be 3.57*12=42.84V as your cutoff start
```

---
## \#3 Posted by: coderman Posted at: 2017-12-14T00:08:45.390Z Reads: 45

```
so does 12s=44.4V? if so would 2V from nominal to cutoff be too little of a gap or am I getting something wrong? thanks for the reply also!
```

---
## \#4 Posted by: Namasaki Posted at: 2017-12-14T02:08:42.427Z Reads: 33

```
A 12s Lipo setup will have 50.4v at full charge. 44.4v is nominal charge.
If you are going to trust only the Vesc low voltage cutoff then you need to use a conservative number because you can not depend on your battery cells to drain evenly.
3.6v per cell would be considered a conservative number. for low voltage start. and 3.4v per cell for low voltage end.
So for a 12s battery that would be 43.2v start and 40.8 end. I would round it off to 44v start and 40v end.
The point is that you stop riding if and when you hit the 44v low voltage start. You do not want to continue to the low voltage end where all power is shut down. If this happens while your going fast, the sudden loss of power could throw you off the board.
```

---
## \#5 Posted by: coderman Posted at: 2017-12-14T02:21:57.334Z Reads: 33

```
literally all the information i needed. thank you!!!!!!!!!!!!!!!!!!!
```

---
## \#6 Posted by: Namasaki Posted at: 2017-12-14T02:22:48.178Z Reads: 33

```
Glad I could help.
Btw, I've been using Lipos for over a year on my boards and I love them.
```

---
