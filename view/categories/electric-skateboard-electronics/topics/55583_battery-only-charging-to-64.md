# Battery only charging to 64%

### Replies: 27 Views: 828

## \#1 Posted by: Freddiecook Posted at: 2018-05-15T19:48:45.829Z Reads: 129

```
Like the title says it charges to 64% but then stops and the green light on the charger turns on, I’ve tried to leave it to see if it’s having an issue balancing but to no avail, I’ve also replaced the bms which didn’t help, anyone got any ideas? I’m skipping the discharge on the bms btw
Charger 
![image|281x500](upload://zznv0F1RiHObvva7PZYXD06Jgmc.png)
Bms
![image|281x500](upload://ywEvc6lbSxroWvaOQpNXlOZx6LG.png)
```

---
## \#2 Posted by: b264 Posted at: 2018-05-15T19:51:52.511Z Reads: 122

```
Is your battery gauge set to 12S instead of 10S?

What battery is it?
```

---
## \#3 Posted by: clistpdx Posted at: 2018-05-15T19:55:08.011Z Reads: 116

```
Try using a multimeter to measure the actual voltage from the pack to see if's really giving you 42V
```

---
## \#4 Posted by: Freddiecook Posted at: 2018-05-15T20:45:47.383Z Reads: 103

```
Made sure it’s set to 10s, it a 10s4p Samsung 25r pack I got made from one of the members on the forum, did 2 full cycles on the battery then this happened
```

---
## \#5 Posted by: L3chef Posted at: 2018-05-15T20:47:46.873Z Reads: 94

```
What are you measuring the voltage with?
```

---
## \#6 Posted by: Sender Posted at: 2018-05-15T20:56:29.623Z Reads: 88

```
What is the voltage actually coming out of the charger?  I had a "6s" charger that should have been pushing 25 volts but it was rebranded and mislabeled and was only actually pushing 16.4 volts or so.
```

---
## \#7 Posted by: Freddiecook Posted at: 2018-05-15T20:57:18.207Z Reads: 85

```
Using one of those 10s voltmeters 
But also using a voltmeter to measure the actual output and it’s only 38V
```

---
## \#8 Posted by: Freddiecook Posted at: 2018-05-15T20:57:34.753Z Reads: 86

```
I’ll have a look now
```

---
## \#9 Posted by: Freddiecook Posted at: 2018-05-15T21:00:14.370Z Reads: 86

```
It’s outputting 42V still
```

---
## \#10 Posted by: Silverline Posted at: 2018-05-15T21:00:28.159Z Reads: 85

```
I think you have a bad connection in the battery. If the charger worked before...
```

---
## \#11 Posted by: Freddiecook Posted at: 2018-05-15T21:15:55.459Z Reads: 79

```
I’ll have a little look in there tomorrow, gunna need to get some replacement heat shrink
```

---
## \#12 Posted by: Silverline Posted at: 2018-05-15T21:21:07.056Z Reads: 75

```
If one of the parallel connections is bad, the other batteries in the same parallel group wil reach 4,20v Long before the others, and proceed, because the total end voltage still is to low, and then the bms shuts down the charger because it's protects the battery cells. This could maybe be your problem.
```

---
## \#13 Posted by: Freddiecook Posted at: 2018-05-15T21:43:38.799Z Reads: 70

```
Thanks, I’ll have a look at each parallel group tomorrow and report back
```

---
## \#15 Posted by: Freddiecook Posted at: 2018-05-16T19:53:17.965Z Reads: 49

```
So I’ve tested all of the parallel packs and one of the packs is giving literally 0 volts, I am so puzzled, there is a connection there as I checked with the ‘beep’ mode but there is nothing there :thinking:
:confused:
```

---
## \#16 Posted by: darkkevind Posted at: 2018-05-18T15:00:00.362Z Reads: 46

```
How did you check and get zero volts? If it's through the BMS balance wires then the balance wire may have come loose. This would explain why the main discharge wires are still giving you 42v.

It may be a simple case of re-soldering back the balance wire...
```

---
## \#17 Posted by: Freddiecook Posted at: 2018-05-18T15:19:44.007Z Reads: 43

```
Each cell apart from those 4 are outputting 4.2V but those 4 are giving 0, checked with a voltmeter
The charger is giving out 42V but the pack is not
```

---
## \#18 Posted by: darkkevind Posted at: 2018-05-18T15:45:41.997Z Reads: 42

```
So what voltage are you getting from the discharge wires of the pack?
```

---
## \#19 Posted by: Freddiecook Posted at: 2018-05-18T16:09:53.106Z Reads: 43

```
38V
10 char
```

---
## \#20 Posted by: Deckoz Posted at: 2018-05-18T16:15:33.851Z Reads: 42

```
Did you measure that from the balance leads or directly on the cells.

If you measured at the balance leads a lead could be broken. If you measured the nickel at the cell the spot welds could be broken. If you measured at the cell and the cells are 0v you need to replace those cells.

My bet is on nickel or balance leads broken
```

---
## \#21 Posted by: Freddiecook Posted at: 2018-05-18T18:52:09.506Z Reads: 36

```
I’m measuring it on the tracks, the connections are made though, just no voltage through them
```

---
## \#22 Posted by: Deckoz Posted at: 2018-05-18T18:53:22.676Z Reads: 34

```
[quote="Freddiecook, post:21, topic:55583"]
on the tracks
[/quote]

Tracks?? 10char
```

---
## \#23 Posted by: Freddiecook Posted at: 2018-05-18T18:54:42.415Z Reads: 30

```
The lines of nickel
```

---
## \#24 Posted by: b264 Posted at: 2018-05-18T18:54:57.237Z Reads: 30

```
[quote="Freddiecook, post:17, topic:55583"]
checked with a voltmeter
[/quote]

where?  Did you put the voltmeter leads on the ends of the cells or on a wire that comes out of the pack, or on the BMS?

Do you have a photo
```

---
## \#25 Posted by: Freddiecook Posted at: 2018-05-18T18:55:16.702Z Reads: 30

```
The ends of the cells, I’ll post a photo when I get home
```

---
## \#26 Posted by: Deckoz Posted at: 2018-05-18T19:41:46.674Z Reads: 27

```
Can you check each cell of that group individually touching behind the nickel,to verify it's not broken spot welds and that the cells themselves are 0v. Likely I'm guessing your pack didn't use insulators or kapton on the positive side and the PVC wrap has melted under the nickel and shorted the whole group against the cell body...
```

---
## \#27 Posted by: Freddiecook Posted at: 2018-05-18T21:00:29.799Z Reads: 25

```
I’ll try tomorrow morning when I’m home as I’m currently away :slight_smile:
```

---
## \#28 Posted by: Freddiecook Posted at: 2018-05-19T11:00:47.559Z Reads: 17

```
I can't manage to get my probes under the welds, they all seem securely on and I don't really want to rip them off as then I'll have to send the pack off to get welded again. But the pack is using insulation on the positive ends
```

---
