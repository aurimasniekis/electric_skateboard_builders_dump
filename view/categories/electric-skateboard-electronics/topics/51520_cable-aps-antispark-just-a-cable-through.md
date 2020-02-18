# +cable APS antispark just a cable through?

### Replies: 4 Views: 311

## \#1 Posted by: Guacamoleface Posted at: 2018-04-07T22:06:15.190Z Reads: 57

```
So Im currently building another board, and curious about the APS Anti-spark.

Wanted to redo the cables as they were changed so many times before and started getting messy. Noticed however that the positive cable seems to be attached to another cable that just goes thru the antispark and then attached on the other side aswell.

Is the Positive cable just a cable that goes thru the APS with no components inbetween?

I noticed a quite interesting way of how its connected when I removed the shrinktube and it looks as its just a cable and the only thing thats actually affected by this component is the negative cable. You will see in picture below.

![30264600_10211820833417861_134574867415564288_o|375x500](upload://oUAxbs21q0NEZbCaRqsbGchYynx.jpg)
```

---
## \#2 Posted by: FabianOdermatt Posted at: 2018-04-07T22:14:37.677Z Reads: 56

```
Yeah, the positive cable is just going through. I don't know the schematics of this one, but it should be kind of the same as vedders' anti spark switch. With the mosfets you're just switching the negative side.

(just without the fuse)
![Schematic|690x216](upload://iLJQuk0FhqjdrAGUhxpgmHDNpEO.png)
```

---
## \#3 Posted by: Guacamoleface Posted at: 2018-04-07T22:19:24.727Z Reads: 53

```
Ah cool, thanks!

So the positive going to the switch(P3) is only to power the switch(led) I guess?
```

---
## \#4 Posted by: FabianOdermatt Posted at: 2018-04-07T22:27:13.540Z Reads: 51

```
When you press the switch, power goes from P3 to P7 and to the gate(G) from the mosfets. When the gate gets powered, the source(S) and the drain(D) get connected and this turns the VESC on.
```

---
