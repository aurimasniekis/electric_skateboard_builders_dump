# Voltage Meter Wiring different voltage supply

### Replies: 7 Views: 719

## \#1 Posted by: WrinklyWink Posted at: 2016-11-19T11:25:08.851Z Reads: 135

```
I have a Voltage Meter I would like to incorporate in my build however I would like it to be turned on by a separate switch. Also since its cheap it requires a 30V max power supply. I'll be powering it with an ubec.
Its just confusing because it has 3 wires which means it has to use a common ground and I don't know which ground to give it.
The specific voltage meter I'm talking about is here: http://www.ebay.com/itm/36-Red-LED-Panel-Meter-Digital-Voltmeter-DC-0-100V-Motor-Motorcycle-EA77-/331868974262
The spst switch is on the red wire.
I made a diagram:
<img src="/uploads/db1493/original/3X/6/4/64f52b1457003e97ee9c5cef6d23ff79b6c71849.png" width="629" height="326">
Which choice should I do?
```

---
## \#2 Posted by: Randyc1 Posted at: 2016-11-19T16:07:23.436Z Reads: 116

```
I think you put Red +Black on your (up to 30v power supply),... then put blue wire on the Pos side of skateboard's  battery pack
```

---
## \#3 Posted by: SORRENTINO Posted at: 2016-11-19T17:52:25.592Z Reads: 100

```
Both the battery ground and the bec ground go to black. bec positive goes to red which is 30v or less and then battery positive goes to blue. IMO
```

---
## \#4 Posted by: SORRENTINO Posted at: 2016-11-19T17:53:56.024Z Reads: 95

```
Also I have this one and its awesome. You can take the shroud off for a slimmer voltmeter. http://www.ebay.com/itm/282156101427?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#5 Posted by: SORRENTINO Posted at: 2016-11-19T17:56:34.552Z Reads: 82

```
The way I describe how to wire it is the way it is listed in the info section of that Ebay listing.


Wiring:
Red: power supply +
Black: power supply -, measure -
Blue: measure +
```

---
## \#6 Posted by: WrinklyWink Posted at: 2016-11-19T18:07:31.727Z Reads: 74

```
I read that too, but I also read somewhere that you shouldn't mix different grounds.
```

---
## \#7 Posted by: SORRENTINO Posted at: 2016-11-19T18:11:07.221Z Reads: 69

```
who said that and what was there reasoning? This is a common ground, shouldnt hurt anything. I think not mixing grounds only applies if its a signal wire and ground Because you want a closed loop.
```

---
