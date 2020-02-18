# Burnt VESC? How do i troubleshoot

### Replies: 10 Views: 263

## \#1 Posted by: razad7 Posted at: 2018-05-27T17:48:11.171Z Reads: 59

```
Hi!
My VESC stopped working completely mid ride.
It won't power on through battery or USB so i can't check the BLDC for issues.
I don't see anything visually burnt.
Any suggestions?
Thanks!

![IMG_7816|375x500](upload://4xF5zl8iAQeblXJjBZotbPB60B3.JPG)![IMG_7873|375x500](upload://biLuRizbPZa2sfSVsrUyQoieTeb.JPG)
```

---
## \#2 Posted by: L3chef Posted at: 2018-05-27T17:53:59.585Z Reads: 52

```
Mosfet has blown
```

---
## \#3 Posted by: razad7 Posted at: 2018-05-27T18:07:17.537Z Reads: 50

```
The one over the red wire in picture two?
(don't mind the residue on the top of them they had heatsinks)
```

---
## \#4 Posted by: L3chef Posted at: 2018-05-27T18:21:09.210Z Reads: 48

```
First pic. Mosfet to the left. But it can be residue. Hard to tell from the pic.
@JohnnyMeduse is the guy you want an opinion from
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2018-05-27T18:27:23.798Z Reads: 50

```
Is it a dual or single setup?
```

---
## \#6 Posted by: Martinsp Posted at: 2018-05-27T18:42:21.871Z Reads: 46

```
![image|312x333](upload://jNRD85qbU83QWLgGgnJLBUgReJ8.jpg)
Is this some kind of damage you know about or is it something new? That exposed trace is connected to battery positive and it may be either mechanical damage or soldermask (the purple stuff on the PCB in your case) peeling due to heat which means a short.
```

---
## \#7 Posted by: razad7 Posted at: 2018-05-27T18:50:48.443Z Reads: 42

```
Single Setup
```

---
## \#8 Posted by: razad7 Posted at: 2018-05-27T18:52:47.057Z Reads: 39

```
Hey,
Yeah i noticed that too.
Didn't notice before, but not sure if it's new... or i just didn't notice :frowning:
It's very well protected under my board so i doubt it's any physical damage. 
Do you have any recommendation to how to solve this?
Thanks!
```

---
## \#9 Posted by: Martinsp Posted at: 2018-05-27T18:57:12.783Z Reads: 38

```
Do you own a multimeter?

If so you should start by measuring resistance ("beep mode" continuity if your multimeter has such a feature) between battery + and - it may beep/show low resistance for a moment as the capacitors are charging up but it should stop. After that, measure resistance between battery + and each phase wire, the same goes for battery - and each phase wire. None of them should be shorted.
Next you can measure resistance between gnd and 5V and also between gnd and 3.3V again, these should not be shorted.

Your issue will most probably be the DRV since the VESC does not turn on at all, but that is just a guess at this point.
```

---
## \#10 Posted by: razad7 Posted at: 2018-05-27T19:10:57.378Z Reads: 32

```
I'll check this, Thanks!
```

---
