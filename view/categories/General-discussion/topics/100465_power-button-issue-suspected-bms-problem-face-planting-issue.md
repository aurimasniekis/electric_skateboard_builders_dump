# Power button issue suspected BMS problem? FACE-PLANTING ISSUE

### Replies: 9 Views: 238

## \#1 Posted by: ju5t Posted at: 2019-08-17T21:37:40.293Z Reads: 78

```
I was riding home on [the BrumBeast](https://www.electric-skateboard.builders/t/the-brumbeast-37mph-dual-6374-maytech-12s4p-unity-bergmeister-wheels-fatboy-nano-gear-drive-bigben-enclosure-landyatchz-evo-tb218-first-build) when suddenly the board cut out throwing me on my face in the middle of the road.



The issue breaks down like this;

I rebuilt everything again to check for problems and after recalibrating the motors unloaded i tested it again. 
As soon as i accelerated on the board with me on, it cut out and then wont power back on.


To get the power button to work again have to plug in the charge cable and then the power button works again without issues till i try and ride the board.


This has got to be a bms issue shorting and staying off till charging the board resets it?

the BMS is a Bestech HCX-D596 12S 80A BMS, 12s4p samsung 30q battery

the Focbox Unity showing no faults in console.

**the motors appear to work fine unloaded no cutting out!!!!!!!!!!!!!!!!!**


Man what a run of luck on this thing now

![image|375x500,50%](upload://bTnt0nLdOWZs5PbSqabjEFIGJUO.jpeg) 

If anyone can assist in what i can do to troubleshoot more or tests to narrow down the issue i would appreciate the help.
```

---
## \#2 Posted by: bigben Posted at: 2019-08-18T06:23:16.925Z Reads: 63

```
You could bypass the bms and use a loop key as your switch to see if the bms is the issue?
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-08-18T06:36:00.646Z Reads: 61

```
Dumb question: What's your battery max current set at?
```

---
## \#4 Posted by: ju5t Posted at: 2019-08-18T12:09:15.287Z Reads: 50

```
[quote="MysticalDork, post:3, topic:100465, full:true"]
Dumb question: What’s your battery max current set at?
[/quote]

if you mean on the focbox app 60amp 

[quote="bigben, post:2, topic:100465, full:true"]
You could bypass the bms and use a loop key as your switch to see if the bms is the issue?
[/quote]

Does that look like it has shorted on the BMS?
How would i wire this to be discharge direct? Im looking at the wiring diagram but not clear

![20190818_125921|281x500](upload://siThyxFbtkOtJGgMLj1z8mlcuE7.jpeg) ![20190818_125913|281x500](upload://5DPqN6jYkANLSfsF13BiLGKodjJ.jpeg) ![20190818_130452|690x388](upload://lK5vTKuwwrhsS45XGAgmIcbhaC6.jpeg)
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-08-18T19:37:17.895Z Reads: 35

```
@ju5t Is that 60 battery amps **per side**, or 60 amps **total**?
```

---
## \#6 Posted by: ju5t Posted at: 2019-08-18T20:56:37.315Z Reads: 33

```
[quote="MysticalDork, post:5, topic:100465"]
Is that 60 battery amps **per side** , or 60 amps **total** ?
[/quote]
![Screenshot_20190818-141913|236x500](upload://cf8FWY9qhIGmsf2vYQn6kNzYa6q.jpeg)
```

---
## \#7 Posted by: ju5t Posted at: 2019-08-18T21:04:15.833Z Reads: 32

```

As an update I have rewired the BMS to charge only and direct discharge that got everything working.

However the Battery doesnt charge through the BMS and clearly a faulty BMS is the problem here.
Just need to test the cells ensure theres no possibility its a dead cell or problem pack and then replace the BMS.

Not looking forward to the fiddly soldering work connecting a BMS to the cell packs

Welcome to DIY folks
```

---
## \#8 Posted by: itsrow Posted at: 2019-09-01T19:03:08.464Z Reads: 22

```
These bestech BMS' have had crazy high failure rates as of late, anyone know whats up?
```

---
## \#9 Posted by: Tinp123 Posted at: 2019-09-01T19:55:07.151Z Reads: 21

```
At the end, it wasn't bms fault. Last two balance wires on separate connector were swithed and bms killed last group
```

---
