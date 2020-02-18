# Battery Pack Help? Cells keep dying

### Replies: 9 Views: 201

## \#1 Posted by: yulaw2k Posted at: 2019-09-13T18:35:42.775Z Reads: 68

```
![battery|375x499](upload://pgB4iFMtfGPe2GUnCGDD6WFXehy.jpeg) ![battery1|250x500](upload://4EivYI1BhUP1sMRyNV15YoxwP8g.png) 

I used this BMS for the past year or so. Its worked fine. I was using crappy low powered 18650's in my last pack, but it worked, just slow.... I decided to upgrade my battery pack and soldered together this battery pack with samsung 25R's.

My problem: Its been sitting for a week waiting for me to print a new case. In the picture you can see two  cells died, or 4 since its 10s2p. This is the second time i let the pack sit for a week waiting for parts and i come back and part of the pack is dead. Last time I pulled the cells out and all 4 were 0voltage. So I am assuming this is also what has happened. Both times I put together the skaeboard with some tape and rode around just fine.

The blue line shows the voltage over the past few days on one of the cells, the other cell is similar. Can anyone make sense of why it would just go crazy like this?![Screenshot_20190913-170321|250x500](upload://qyGGMcoUvLFwN4IFcX3IAYQJ8yY.png)
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-09-14T00:31:24.432Z Reads: 55

```
A couple ideas come to mind: First, unless you're very good and have a good soldering iron, it's really easy to damage cells by soldering them.

Second, your wiring is a mess, which makes me suspect that the issue is related to bad connections somewhere. Break out the multimeter and start digging.
```

---
## \#3 Posted by: torqueboards Posted at: 2019-09-14T00:58:52.622Z Reads: 52

```
You could also have a bad BMS. I'd swap the BMS and test again but I wouldn't use that same BMS again.
```

---
## \#4 Posted by: yulaw2k Posted at: 2019-09-14T01:03:58.799Z Reads: 50

```
I use acid when soldering metal, it literally takes half a second to solder the battery when using an acid vs a couple seconds you see people online soldering batteries with normal flux, so I cant imagine I damaged the batteries soldering. Would the batteries become damaged immediately if it was due to heat? 

Another person also said it's probably my BMS..... I should have just bought a one wheel... I'll buy a new BMS board and replace the four batteries if the 4 cells are indeed dead. I think I spent 100$ on the BMS which makes me cringe having to replace it.
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-09-14T01:36:17.269Z Reads: 44

```
Before you start buying new parts, check all your connections with a multimeter. Wiggle the plugs and see if anythings changes. Check the cell voltages with a multimeter if you haven't already.

The use of an aggressive flux is a great improvement - I've built three packs by soldering and they're all doing OK, so it's definitely doable. The trick as you know is going very fast, to minimize heat input.
```

---
## \#6 Posted by: torqueboards Posted at: 2019-09-14T01:36:42.431Z Reads: 44

```
If you use good cells and your cells drift. Typically, it's BMS. I've had it happen quite a bit in the past until I changed out the BMS. Must of been a bad batch or something.
```

---
## \#7 Posted by: yulaw2k Posted at: 2019-09-14T02:54:04.043Z Reads: 39

```
I just checked the voltage on the four cells with a multimeter, sadly all four are 0volts... so I guess I'm buying four new cells and a BMS.
```

---
## \#8 Posted by: Santino Posted at: 2019-09-20T06:52:59.151Z Reads: 29

```
RIP sorry for your lost....New cells with same IR, BMS, some order, spot welder, clear build...would be nice....Hope you are able to keep rolling soon...
```

---
## \#9 Posted by: MysticalDork Posted at: 2019-09-21T03:44:23.717Z Reads: 15

```
A real lifesaving tool for things like this is a multimeter with a DC clamp function - you can check the current being drawn from your cells by the BMS balance wires, without disconnecting anything. I have an uni-t UT210E and it's fantastic for stuff like this, finding an elusive parasitic drain or a BMS that's "balancing" when it shouldn't.
```

---
