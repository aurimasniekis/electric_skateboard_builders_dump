# Battery overvoltage protection - dump load

### Replies: 8 Views: 355

## \#1 Posted by: Nordle Posted at: 2018-07-11T06:48:57.090Z Reads: 60

```
Hello,
because i run several times into overvoltage cutoff and have no other brakes than my motors on electric boards, i tried to make a circuit to solve this problem.
It should switch a dump load in parallel to my battery and ''v''esc whenever the voltage in said lines goes above a set value (0,5 volts less than cutoff is set in vesc), and switch it back off when voltage is aprox. (depends a bit on set voltage) 0.5v lower than the set point.
here is my circuit:
![circuit%20(1)|690x411](upload://owVuJ05aRPQI7gDXjOhp0mqbyKW.png)
**any toughts?**
**how big should the dump load be? the same size as i set my battery regen current? and any ideas what i could use, these resistors are big...**
```

---
## \#2 Posted by: Ishayc Posted at: 2018-07-11T11:00:58.719Z Reads: 44

```
Try figuring out why you are getting this errors first.
What is your setup?
Is there a specific time/ something you're doing that makes this overvoltage happen?
```

---
## \#3 Posted by: Nordle Posted at: 2018-07-11T11:16:10.065Z Reads: 40

```
it's normal you brake and generate voltage, when the battery is full it's full...
read again maybe
```

---
## \#4 Posted by: Narnash Posted at: 2018-07-11T11:29:43.902Z Reads: 40

```
There is also another easy solution, charge your batteries only to 4.1-4.15V. You may loose 5% usable capacity but you shouldn't have overvoltage problems anymore. 
You will also charge up faster since the last couple % charge usually very slowly. Depending on the batteries you also might get a modest amount of extra life cyles from them (for certain if you really over charged them sometimes)
```

---
## \#5 Posted by: Ishayc Posted at: 2018-07-11T11:37:46.757Z Reads: 37

```
If it's from full battery and regenerative braking then just try not to charge your battery to full unless it bothers you that much to lose a small amount of range. 
The only issue might be the balancing if you use BMS, since the balance mode kicks in when battery is full.
```

---
## \#6 Posted by: Nordle Posted at: 2018-07-11T11:44:48.315Z Reads: 30

```
no, i rather design a circuit to solve this problem by it's roots...
even if i only charge my 10s (21Ah) pack to 41V i run into this problem sometimes...
i'm not stupid how can you even give such advise, do you understand at least the circuit?
```

---
## \#7 Posted by: Ishayc Posted at: 2018-07-11T11:53:36.254Z Reads: 28

```
Yup, I'm happen to be an electrical engineer. 
No one implied you're dumb, just suggested it's not worth the trouble and time from my aspect but whatever dude. Good luck with that.
```

---
## \#8 Posted by: Nordle Posted at: 2018-07-11T11:57:39.424Z Reads: 25

```
well i doubt that too, but it’s fucking scary to go over 30km/h down a mountain and suddenly brakes skip out
```

---
