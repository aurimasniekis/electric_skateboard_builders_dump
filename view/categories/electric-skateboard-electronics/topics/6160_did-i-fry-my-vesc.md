# Did i fry my vesc?

### Replies: 18 Views: 1598

## \#1 Posted by: clpjan Posted at: 2016-07-15T19:12:36.605Z Reads: 137

```
so i got my vesc 4.12 today. i have a 12 battery with a xt90 plug already so soldered that to the vesc. then i connected the 192 kv sk3 motor an. when i plugged the vesc in there was a huge spark between the xt90s and also smoke. 
does anyone know what happened ?
```

---
## \#2 Posted by: barajabali Posted at: 2016-07-15T19:13:44.422Z Reads: 140

```
Sounds to me like you don't have an anti spark xt90. 

Seems normal
```

---
## \#3 Posted by: clpjan Posted at: 2016-07-15T19:15:39.659Z Reads: 140

```
i used another esc in the exact same setup and the spark was only minimal and didn´t melt the connectors
```

---
## \#4 Posted by: sl33py Posted at: 2016-07-15T19:19:05.210Z Reads: 139

```
a pretty big spark without anti-spark of some sort is pretty normal.  What concerns me is the "also smoke"...  

Did it work once connected?  Double check your batteries connectors.  And let us know battery configuration (what batteries, in series assuming, and how many) - make sure you didn't inadvertently connect something backwards and short something.  That would be both big spark and possibly smoke (i don't like letting the magic smoke out).

Give us some more detail or pics of your setup so we can help troubleshoot.  I would not reconnect the VESC if the last time you did this it didn't work.  Check the board thoroughly for scorch marks - check under the power cable to make sure one of the components or pins didn't pierce the wire sheathing and short, etc.

I might also recommend starting off at lower series like 6/8/9s (depending if you are using 3s in series or 4s in series for 12s).

HTH!
```

---
## \#5 Posted by: clpjan Posted at: 2016-07-15T19:23:35.816Z Reads: 132

```
i use 2 6s lipos in series. this was the first time i tried to connect it and i immediatly unpluged it 
give me a sec i will take some pictures
```

---
## \#6 Posted by: sl33py Posted at: 2016-07-15T19:30:23.805Z Reads: 124

```
Double check your connectors - and only connect one of the two batteries for 6s instead of 12s.  Once we know it's working for you, then try 12s.

looking forward to pics to see if anything else looks out of place.  Did you check the VESC for scorch marks?  i'd look around all power wires and on the PCB for any black/carbon/soot marks.
```

---
## \#7 Posted by: clpjan Posted at: 2016-07-15T19:40:29.228Z Reads: 117

```
https://scontent-lhr.xx.fbcdn.net/v/t1.0-9/13690716_1142063875816946_2126115583764967357_n.jpg?oh=7462f196bb67df3b71b788b5e5efbb2a&oe=582C234C 
https://scontent-lhr.xx.fbcdn.net/v/t1.0-9/13718600_1142063979150269_4654450710064621226_n.jpg?oh=11f05cd538a8662a006141064b9e75f0&oe=57F318BD
https://scontent-lhr.xx.fbcdn.net/v/t1.0-9/13718763_1142064005816933_2121752870884363829_n.jpg?oh=5c302b9df33f84a053d8ee816bedfa9b&oe=58223BA6
https://scontent-lhr.xx.fbcdn.net/v/t1.0-9/13716163_1142063672483633_104835296416573460_n.jpg?oh=47e64ac2e0013ef4bbbf7230c2e42338&oe=57F2CFA4
https://scontent-lhr.xx.fbcdn.net/v/t1.0-9/13621006_1142063695816964_4047688215060774404_n.jpg?oh=8e85e59b55bc53adb9dd0dad90b74523&oe=57EF4907
```

---
## \#8 Posted by: clpjan Posted at: 2016-07-15T19:43:19.490Z Reads: 111

```
there also are some indentations/holes in the red cable from where it was pressed against the pins of that white connector. i read in another post that this my cause a short
```

---
## \#9 Posted by: mason Posted at: 2016-07-15T20:14:31.894Z Reads: 107

```
if you soldered the polarity wrong on the xt90 that can create big problems.
```

---
## \#10 Posted by: clpjan Posted at: 2016-07-15T20:16:57.724Z Reads: 106

```
did it the same way as with my other esc
```

---
## \#11 Posted by: Blasto Posted at: 2016-07-15T20:46:18.447Z Reads: 102

```
<img src="/uploads/db1493/original/2X/0/0c869f109da3089a1cba2a7d6f275ec05f48cc32.png" width="513" height="472">

middle seems to be shorted
```

---
## \#12 Posted by: clpjan Posted at: 2016-07-15T20:47:54.442Z Reads: 99

```
that would be a maufactoring error right?
```

---
## \#13 Posted by: Blasto Posted at: 2016-07-15T20:50:21.995Z Reads: 99

```
well does it short? do you have a multimeter handy?

put in continuity mode (the little diode), put one probe on the wire side and the other on the tab of the fet, if it beeeeeeeeeeeeeeeeeeeps, you have a short
```

---
## \#14 Posted by: clpjan Posted at: 2016-07-15T20:52:30.841Z Reads: 98

```
dont have one right now . what do you mean by wire side?
```

---
## \#15 Posted by: Blasto Posted at: 2016-07-15T20:56:20.655Z Reads: 98

```
<img src="/uploads/db1493/original/2X/4/4e47af1f77a2aee81eb5d59f1db97ea3d0abcf04.png" width="512" height="474">


a multimeter should be in every esk8 tool box
```

---
## \#16 Posted by: clpjan Posted at: 2016-07-15T21:02:47.455Z Reads: 96

```
thanks electronics isnt really my strong arm
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-07-16T22:30:23.235Z Reads: 71

```
[quote="clpjan, post:3, topic:6160, full:true"]
i used another esc in the exact same setup and the spark was only minimal and didn´t melt the connectors
[/quote]

Well, did the other ESC have some "Antispark feature". My last heli esc had such a feature and the spark was minimal!

 [quote="clpjan, post:1, topic:6160"]
when i plugged the vesc in there was a huge spark between the xt90s and also smoke.
[/quote]
Did you just get a spark and therefore did not test the VESC or did you try the VESC after the spark?

Using 12S there will be always a big spark because the capacitors pull much energy from the battery. Maybe you look into "anti spark"
```

---
## \#18 Posted by: clpjan Posted at: 2016-07-17T20:23:09.095Z Reads: 56

```
alright so i finaly got around to testing the connection and it does goe beeep meaning i have a short.
i will write to enertion support tomorrow
```

---
