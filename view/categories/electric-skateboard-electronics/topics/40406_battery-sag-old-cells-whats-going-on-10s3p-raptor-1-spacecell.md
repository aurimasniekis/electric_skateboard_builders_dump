# Battery Sag? Old Cells? What&rsquo;s going on? (10s3p Raptor 1 SpaceCell)

### Replies: 16 Views: 621

## \#1 Posted by: Mikenopolis Posted at: 2017-12-07T18:59:29.669Z Reads: 136

```
Here's a video of what's going on with my rebuilt dual 6355 Raptor 1 (original spacecell 25R?, new vescs and motors). I've never really noticed this until a few weeks ago. When I started with 100% and after a block or two it was in the 70's with no throttle, then in the 50's when I throttled. After 2 miles I stopped and it was reading 85%. This extreme behavior doesn't happen to the CarvOn V3 Raptor build (newer cells).

Question is what is going on here? Anyone see this issue?

@onloop This is obviously out of warranty, just waiting on your Raptor 1 news before deciding on what to do next

@joeadams101 did yours start doing this as well? 

@barajabali This is what I was talking about, so the thing you fixed wasn't the issue. 1:22 into the video the meter read 43%
https://www.youtube.com/watch?v=UVJcdGATCgM
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-12-07T19:14:27.522Z Reads: 127

```
when's the last time you measured each P group voltage?

I've had an entire P group drop down to zero volt, and it kind of exhibited this behavior. 

to measure, take the balance leads out of bms, ground negative probe to pack negative, then measure each balance lead on bms connector
```

---
## \#3 Posted by: PXSS Posted at: 2017-12-07T19:15:59.093Z Reads: 122

```
This ^
A whole group is most likely dead.
```

---
## \#4 Posted by: barajabali Posted at: 2017-12-07T19:26:57.744Z Reads: 120

```
I did that, everything checks out fine on this battery.  

My diagnoses is that its just a 10s3p (not huge) and the cells are a bit aged. So it shows heavy sag.
```

---
## \#5 Posted by: PXSS Posted at: 2017-12-07T19:36:04.709Z Reads: 108

```
Did you measure capacity???
```

---
## \#6 Posted by: barajabali Posted at: 2017-12-07T19:45:18.432Z Reads: 103

```
@Mikenopolis You're not experiencing extremely reduced range right?  Those displays arent really the most accurate for reading while you ride because all batteries will sag under load and this display does nothing to counter at that. It'll just show you what the output voltage is. The best way to use them is when there is no load on the board. 

As for @PXSS  No I did not measure the capacity of the entire pack or each individual cell as all voltages were normal and he was not experiencing extreme range loss. Also replacing a parallel group this late in the batteries life is not recommended and can be dangerous.
```

---
## \#7 Posted by: PXSS Posted at: 2017-12-07T19:55:48.225Z Reads: 95

```
[quote="barajabali, post:6, topic:40406"]
Also replacing a parallel group this late in the batteries life is not recommended and can be dangerous.
[/quote]

I wouldn't replace it. I would take it out entirely and keep using the pack as a 9S. The dead one will kill the other groups eventually as they get overloaded or the dead group could blow up during charging.
```

---
## \#8 Posted by: barajabali Posted at: 2017-12-07T20:23:35.054Z Reads: 89

```
[quote="PXSS, post:7, topic:40406"]
The dead one will kill the other groups eventually as they get overloaded or the dead group could blow up during charging.
[/quote]

Have you inspected this pack? I have... Its not dead.
```

---
## \#9 Posted by: Battosaii Posted at: 2017-12-07T20:33:15.358Z Reads: 86

```
I'm not looking forward to this in the future but I've gotten pretty confident with batteries after i fixed my spare space cell and put that one in my diy.

My current space cell on the Raptor is still working fine but lately it will only charge to 100% sometimes usually the charger stops at 94-97% and I have tried other chargers maybe my battery is showing it's age finally
```

---
## \#10 Posted by: michaelcpg Posted at: 2017-12-07T21:10:15.545Z Reads: 80

```
That sounds more like you've got a cell in one of your P groups that's had the spot weld become disconnected
```

---
## \#11 Posted by: Mikenopolis Posted at: 2017-12-07T21:32:10.413Z Reads: 79

```
Thanks all for your insights. I haven't used this dual 6355 for distance for a while because of the Carvon V3 build. I'll probably attempt a 10-15 mile ride this weekend to see how range has been affected.

@barajabali thanks for checking it out for me. Would this sag cause a cutoff to the motors? that 90 to 40% drop is what I'm worried about most. Once Enertion lets us know what they are planning for the Raptor 1s I can decide what to do. I'm hoping for a 10s4p 30q with smaller BMS, otherwise I'm gonna need to commission you for another build for this deck again. Have you looked into puzzling together 40 cells with two FocBoxes and BMS? I know someone did it with regular vescs


Also, I can't wait to get the deck hook so I can bring a backup board for these kind of tests. so embarrassing getting an Uber holding a dead board. Did that with the Landwheel twice now
```

---
## \#12 Posted by: Sender Posted at: 2017-12-07T21:37:47.703Z Reads: 76

```
Unrelated note, how do you like the CARVON build over the dual 6355?  Which setup do you feel yourself gravitating to more?
```

---
## \#13 Posted by: Mikenopolis Posted at: 2017-12-07T21:54:19.849Z Reads: 74

```
@sender Belt drive slaps a smile on my face! This dual 6355 is BLDC and the torque and sound goes well together. The CarvOn is FOC and to me is more of a "sophisticated" ride if you will. It'll get up to speed but just lacks that punch dual belts give you.

I've been gravitating more towards the Carvon mostly because it's the newest toy and I was testing the replaced FocBox in FOC. If I had to choose between the two Raptor builds walking out the door (having good battery, same wheels and modes on both ) I would probably go dual 6355 belt.
```

---
## \#14 Posted by: PXSS Posted at: 2017-12-07T22:56:28.541Z Reads: 66

```
I was replying to the hypothetical. No need to be a douche about it.
```

---
## \#15 Posted by: willpark16 Posted at: 2017-12-07T23:11:34.064Z Reads: 64

```
Your problem is in fact commmon and is a problem that I've seen on many raptor 1 battery repairs. The 25r is not a terrible cell, if it was you guys wouldn't have been using it before this 30q hype began. The issue is these batteries were horribly designed, the bypassed bms, while allowing access to all of the battery amps often leads people to over stressing their batteries, if you want more amps you need more cells in parallel simple as that
```

---
## \#16 Posted by: barajabali Posted at: 2017-12-08T01:26:40.876Z Reads: 53

```
My bad didn’t mean to come off as douchey
```

---
