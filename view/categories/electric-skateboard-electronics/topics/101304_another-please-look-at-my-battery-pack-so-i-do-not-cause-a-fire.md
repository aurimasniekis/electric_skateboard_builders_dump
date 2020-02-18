# Another Please Look at my Battery Pack So I Do Not Cause a Fire

### Replies: 8 Views: 155

## \#1 Posted by: itsrow Posted at: 2019-09-03T16:28:17.381Z Reads: 58

```
I don't have too much to say, just want a look over so I understand how to bypass a BMS correctly.![WIP%20Board%20layout%20SHORT|690x237](upload://8movmdVE0BlpxD5zGGWfonBQWS2.png)
```

---
## \#2 Posted by: Tinp123 Posted at: 2019-09-03T17:24:55.249Z Reads: 52

```
Why did you wire your balance wire Nr. 0 between 10th and 11th group? That doesn't make any sense. It should go on main battery negative, before 1st group. Also, you could wire additional wire, lets say 14 or 16awg between battery main negative and B- on your bms. Main charging current will go through it, I dont think that only one thin balance wire will be enough. Well if you want to charge this battery with 1 amp charger, I guess it will work. But I don't see reason for not installing additional thicker wire
```

---
## \#3 Posted by: itsrow Posted at: 2019-09-03T17:35:24.178Z Reads: 45

```
Balance wire Nr. 0 I wired to ground of last cell in series and B- as virtually 0 energy will be flowing through there.  Also the thin wire is still 20ga and I will only be charging at 4a, so the thin wire is okay for charging current.
```

---
## \#4 Posted by: Tinp123 Posted at: 2019-09-03T18:06:54.877Z Reads: 40

```
Balamce wire Nr. 0 should go on main battery negative, before first group. It is not just ground wire, it is balance wire too. Maybe I didn't read your scheme right, but did you connect that thin black balance wire with thick black wire from bat - to vesc -, or are they just crossing each other?

During charging, current will go through B- on bms to bat -. Balance wires will only carry small current during balancig phase.
```

---
## \#5 Posted by: itsrow Posted at: 2019-09-03T18:27:56.725Z Reads: 36

```
I changed the diagram to have BMS B- and balance wire Nr. 0 to connect to main batt-, guess I dont have to connect the ground in the last cell to anything![WIP%20Board%20layout%20Edited|690x234](upload://yUgCflcTlTVXjZ6enmQbGPiUvaM.png) ?
```

---
## \#6 Posted by: Tinp123 Posted at: 2019-09-03T19:54:20.006Z Reads: 28

```
Looks good to me now! :+1:


And no, you don't have to connect black wire in last group to anything.
```

---
## \#7 Posted by: itsrow Posted at: 2019-09-03T19:55:08.864Z Reads: 27

```
Damn that makes me feel stupid, thank you so much.
```

---
## \#8 Posted by: Tinp123 Posted at: 2019-09-03T19:56:09.944Z Reads: 27

```
No problem! Like you said, better to ask than get fire 😁


Good luck with your build!
```

---
