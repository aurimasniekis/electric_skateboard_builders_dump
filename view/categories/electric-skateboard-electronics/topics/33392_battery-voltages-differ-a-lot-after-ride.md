# Battery voltages differ a lot after ride

### Replies: 18 Views: 431

## \#1 Posted by: Panthera Posted at: 2017-09-18T09:36:39.623Z Reads: 122

```
I have 3x 3s 5000 mah lipo batteries. I got my board done and went for ride. After ride I checked my battery packs voltages. They were 2.8 V 2.8 V 2.9 V in first one then second had 3.3 V in all 3 cells and third one had 3.7 V 3.6 V 3.4 V in its cells. What could be the cause?
```

---
## \#2 Posted by: Vieo Posted at: 2017-09-18T09:39:25.519Z Reads: 123

```
From my experience LiPo's cell voltage tend to drift apart. You running 9S? Did you balance charge them all to the exact same before the ride? Which LiPo brand are you using?
```

---
## \#3 Posted by: Cobber Posted at: 2017-09-18T09:41:54.664Z Reads: 116

```
What does your wiring loom/harness look like bro?
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-18T09:42:38.835Z Reads: 115

```
That's too much drift from regular use, test resistance of all the cells and check all connections/solder joints. 
Are they all the same packs? Were they all the same voltage before ride?
```

---
## \#5 Posted by: Panthera Posted at: 2017-09-18T10:06:01.197Z Reads: 103

```
They were all at same voltage and fully charged before ride. There might have been 0.01 V gap between them but I think thats acceptable. Resistance seems normal varying from 4 to 8 mΩ.
All of them are Zippy 5000mah 3s 20C.
All of the connections seems to be on point and were covered.
@scepterr
```

---
## \#6 Posted by: Panthera Posted at: 2017-09-18T10:36:35.615Z Reads: 98

```
<img src="/uploads/db1493/original/3X/5/2/52922d727a9d38d516aa52fb13790f074fbe2644.jpg" width="375" height="500">
```

---
## \#7 Posted by: Cobber Posted at: 2017-09-18T11:41:52.077Z Reads: 83

```
um...
what sort of connectors are they?
you wired in?
your battery leads are?
what sort of esc are you running?
```

---
## \#8 Posted by: Panthera Posted at: 2017-09-18T11:48:40.166Z Reads: 81

```
There are bullet connectors which came with the battery and XT-60 connectors.
?
?
Benjamin Vedder vesc 4.12
```

---
## \#9 Posted by: Vieo Posted at: 2017-09-18T11:50:28.916Z Reads: 77

```
Are the batterys new? How many cycled have they been through?

(sorry for the interrogation)
```

---
## \#10 Posted by: Panthera Posted at: 2017-09-18T11:52:33.813Z Reads: 77

```
Update
I charged them all up and tried if it just was somekind of error that happens once in million, but wasnt lucky. I rode like 5 kilometer and checked their voltages and it looked good all of the cells were 3.86 V. Then i rode the other half and went home and checked them and it looked like before all messed up.
```

---
## \#11 Posted by: Cobber Posted at: 2017-09-18T11:55:49.685Z Reads: 73

```
what are your vesc settings bro?
```

---
## \#12 Posted by: Panthera Posted at: 2017-09-18T11:55:50.516Z Reads: 70

```
No problem. 
They are new. Now they have been through 2 cycles.
```

---
## \#13 Posted by: Panthera Posted at: 2017-09-18T12:07:38.668Z Reads: 71

```
<img src="/uploads/db1493/original/3X/f/b/fbbbbeaa09540eb8111d9f9be1879d4d8527f3fd.png" width="690" height="410">
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-09-18T13:58:31.815Z Reads: 62

```
You did damage your cells already!
Lipos shouldn´t be taken down under 3,5V!
You need to monitor them with a cell meter during your ride.
If you run them in series, you have a 9s 5000mah battery:
9 x 3,7V x 5ah = 166,5 Wh with a consumption of about 10 Wh/km brings you to about 16 km range.
These cells with 20C sag a lot and that´s what you are experiencing with these cell drifts.
```

---
## \#15 Posted by: Panthera Posted at: 2017-09-18T14:26:24.057Z Reads: 57

```
I'll change my settings about that voltage cutoff. Many guides had cutoff at 3,4 V per cell so I followed that.
About sag, that was a big mistake from me not knowing about that before now. I read about sag and I was thinking if i lower my amp draw would it sag less, but take bit away from acceleration?
And my range is only 10 km. Sag has probably something to do with that.
By the way can you explain why my voltage stays stable until i hit something like 3.7 V per cell?
```

---
## \#16 Posted by: SORRENTINO Posted at: 2017-09-18T16:44:33.102Z Reads: 50

```
They are new batteries I would charge them and ride a few times and they should settle out. This is common sometimes with new batteries to have cells discharge irregularly.
```

---
## \#17 Posted by: Panthera Posted at: 2017-09-18T17:26:06.768Z Reads: 42

```
Okay. Lets see Ill ride them few times more and see what happens.
```

---
## \#18 Posted by: jmasta Posted at: 2017-09-18T21:23:12.768Z Reads: 34

```
[quote="Panthera, post:15, topic:33392, full:true"]

By the way can you explain why my voltage stays stable until i hit something like 3.7 V per cell?
[/quote]

That's what lipos do.  They have a very flat discharge curve, until you reach about 3.6V. Then they drop exponentially.  Some cells will hit the "lipo cliff" before the others, which is why the voltages can differ so much.  They should stay in balance very well from 4.2 to 3.7V

As others have mentioned, you already took them way too low. If they were at 2.8V resting, they would be even lower under load. You likely have already caused permanent damage to your lipo batteries
```

---
