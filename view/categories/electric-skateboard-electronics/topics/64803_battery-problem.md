# Battery problem **

### Replies: 27 Views: 517

## \#1 Posted by: Travo Posted at: 2018-08-14T00:59:16.632Z Reads: 111

```
Hello everyone, I opened my board hoping to install a Bluetooth module to he vesc. Instead I opened it only to find that my battery was emitting smoke. I quickly ripped the connections off as to prevent a fire or explosion. The orange wire from the BMS was completed burnt as well. I'm not sure why this happened but when I desoldered the pack and re Soldered it I kept getting sparks from one battery port ( The one with the purple wire). (I know the negative nickel strip is off I've reattached it since)Can anyone answer why this is? I would really appreciate it![15342080887467376134023808635031|666x499](upload://vrCafPNxG7iG4I80SuWeY0QCsPa.jpg)![15342081581818406449221388895023|666x499](upload://iQJb3OO0BrABrjJj3qstTOToBBB.jpg)![1534208230355704953248080066741|666x499](upload://k2lHYFt6I9h72gP2xZCZagoCpHj.jpg)
```

---
## \#2 Posted by: b264 Posted at: 2018-08-14T01:03:17.382Z Reads: 101

```
Take it outdoors IMMEDIATELY until you know why it's venting.  Like RIGHT NOW.
```

---
## \#3 Posted by: SeanHacker Posted at: 2018-08-14T01:04:58.200Z Reads: 100

```
Take @b264's advice immediately.
```

---
## \#4 Posted by: b264 Posted at: 2018-08-14T01:05:04.014Z Reads: 101

```
[quote="Travo, post:1, topic:64803"]
I opened my board hoping to install a Bluetooth module
[/quote]

It's very likely that the problem was caused when it was opened up because if it was smoking, by no means would it be smoking for days and still be operational and not a fireball
```

---
## \#5 Posted by: Travo Posted at: 2018-08-14T01:06:30.315Z Reads: 98

```
Already put it out, sitting on a large cement area so won't catch anything on fire if something happens
```

---
## \#6 Posted by: b264 Posted at: 2018-08-14T01:07:05.366Z Reads: 95

```
Do you have a multimeter?  Are you able to check the voltage of each P-pack
```

---
## \#7 Posted by: Travo Posted at: 2018-08-14T01:07:40.537Z Reads: 97

```
Yea, I'll do that right now
```

---
## \#8 Posted by: b264 Posted at: 2018-08-14T01:07:45.834Z Reads: 94

```
Also I'd unplug the BMS too until you know what's wrong
```

---
## \#9 Posted by: mikenyc Posted at: 2018-08-14T01:13:20.443Z Reads: 92

```
Who made this pack?!
```

---
## \#11 Posted by: Travo Posted at: 2018-08-14T01:14:41.668Z Reads: 89

```
I did about 1 month ago
```

---
## \#12 Posted by: mikenyc Posted at: 2018-08-14T01:16:29.037Z Reads: 90

```
Disconnect the bms and check the voltage of each p group as mentioned above. 

Did you spot weld or solder the nickel strips onto the pack?
```

---
## \#13 Posted by: strattos Posted at: 2018-08-14T01:17:45.817Z Reads: 87

```
The series connections look under built. Esp considering I'm guessing that's nickel plated steel as I've never seen true 100% nickel sold in that format. And I looked for a long fricken time.
```

---
## \#14 Posted by: Travo Posted at: 2018-08-14T01:17:57.628Z Reads: 87

```
I inserted each cell into a 18650 holder and soldered onto it to avoid heating batteries.
```

---
## \#15 Posted by: Travo Posted at: 2018-08-14T01:19:16.497Z Reads: 87

```
Should I double it up?
```

---
## \#16 Posted by: strattos Posted at: 2018-08-14T01:22:34.990Z Reads: 85

```
Get rid of the battery holder's they aren't designed to handle the currents or vibrations. All that being said taking a closer look at your pictures it looks like on your bms the bottom most mosfet is fried the pins look a little scorched and I'm guessing something shorted when you where taking off the enclosure.
```

---
## \#17 Posted by: mikenyc Posted at: 2018-08-14T01:30:10.484Z Reads: 85

```
The heat will travel from the nickel onto the cell unless you’re soldering before attaching to the cell.

Regardless, get yourself a spot welder, they’re not terribly expensive and you’ll save yourself a lot of headache. Don’t solder directly onto the cell. And yes, get rid of those cell holders.
```

---
## \#18 Posted by: Travo Posted at: 2018-08-14T01:32:24.805Z Reads: 84

```
Okay, I have a new BMS already on its was to replace that one. Going to get rid of those holders and get myself a spot welder. Any you prefer?
```

---
## \#19 Posted by: Travo Posted at: 2018-08-14T01:33:32.233Z Reads: 79

```
Is there a spot welder that you prefer or found works well
```

---
## \#20 Posted by: accrobrandon Posted at: 2018-08-14T02:41:55.931Z Reads: 60

```
The "boss" ... Easy to use amd smaller than a sunko which has its own issues and requirements
```

---
## \#21 Posted by: Travo Posted at: 2018-08-14T02:44:12.497Z Reads: 55

```
Do you have a link?
```

---
## \#22 Posted by: Travo Posted at: 2018-08-14T02:47:55.069Z Reads: 50

```
[quote="b264, post:2, topic:64803"]
until you know why it’s venting
[/quote]

Did you mean the battery it self venting? The 18650 wasn't releasing anything but it was the connection between the battery casing and the nickel strip that was the reason small sparks where occuring
```

---
## \#23 Posted by: b264 Posted at: 2018-08-14T03:30:33.781Z Reads: 43

```
[quote="Travo, post:1, topic:64803"]
I opened it ... to find that my battery was emitting smoke
[/quote]

Until you knew what, that's what I meant.
```

---
## \#24 Posted by: accrobrandon Posted at: 2018-08-14T03:31:57.344Z Reads: 45

```
https://www.electric-skateboard.builders/t/boss-level-custom-spot-welder/25980
```

---
## \#25 Posted by: Travo Posted at: 2018-08-14T03:33:23.673Z Reads: 44

```
Oh gotcha. I've just now completely dismantled the whole pack and put each battery in one of those plastic 18650 cases. Going to see if someone locally can spot weld it together for me or look into doing it myself. Thanks for the quick response though really, really appreciate it :slight_smile:
```

---
## \#26 Posted by: Travo Posted at: 2018-08-14T03:51:10.201Z Reads: 38

```
UPDATE!

Turns out the BMS was completely f*cked. Not sure what these little guys are but they're burnt. I have a new BMS in transit but I'm super glad the batteries where not the responsible party here (or so it seems). I've completed dismantled the whole pack and am waiting to see if I can get someone to spot weld a new pack together for me, or alternatively buying one myself. THANK YOU for all you quick responses and safety measures. Really appreciate all of it. Hopefully the battery will be back sooner than later.![15342186028498772804473835539753|375x500](upload://ueCXKM7Ecqh47rIaBIqaEI6GNGm.jpg)
![15342187773703818267894054229370|375x500](upload://jMwomKGaA1Uf1IdALmNeyezcyZf.jpg)
```

---
## \#27 Posted by: accrobrandon Posted at: 2018-08-14T03:56:42.773Z Reads: 36

```
Where u located? I'm on the verge of starting to offer my services and feeling confident in my spot welding and battery assembly skills if interested.
```

---
## \#28 Posted by: Travo Posted at: 2018-08-14T03:57:20.651Z Reads: 37

```
I'll send you a pm
```

---
