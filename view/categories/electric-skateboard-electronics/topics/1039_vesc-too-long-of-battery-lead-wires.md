# VESC - Too long of battery lead wires

### Replies: 9 Views: 2241

## \#1 Posted by: Sharkface Posted at: 2016-01-18T18:56:47.818Z Reads: 217

```
Hello All!

This is something that I had stumbled upon and wanted to get a discussion going for my own purposes. 

With the VESC I have heard a rumor that if your battery lead wires are more than 20cm you can run into some errors on the VESC. I am guessing that this is because the draw from the batteries takes too long to get to the VESC and the capacitors cant cope with that level of draw. Can Anybody confirm that I am looking into this correctly?

Also with that kind of limitation, how do you accomodate for a diagnol build? Wouldnt it be really tight to run the battery lead wires at the desired length? Or could you lengthin the motor phase wires? Putting length to those seems like another recipe for disaster though....

Thanks all!!!
```

---
## \#2 Posted by: Iceni Posted at: 2016-01-18T20:33:27.811Z Reads: 215

```
From what i've read the 20cm restriction only applies when running FOC, since that seems to be more sensitive.
```

---
## \#3 Posted by: treenutter Posted at: 2016-01-18T21:30:42.029Z Reads: 211

```
@Sharkface I think that using VESC in BLDC mode vs FOC mode makes a difference here. My understanding is that FOC mode carries this limitation, but BLDC mode does not.
```

---
## \#4 Posted by: Sharkface Posted at: 2016-01-18T23:30:45.202Z Reads: 206

```
So if I were to run FOC mode, how would I compensate for that limitation on a diagnol drive? short board? lolol
```

---
## \#5 Posted by: paragon Posted at: 2016-01-18T23:59:45.534Z Reads: 202

```
Instead of having a long battery cable, have long motor wires.
```

---
## \#6 Posted by: Sharkface Posted at: 2016-01-19T01:17:23.064Z Reads: 196

```
Sweet thanks,

Anybody have the science behind why this is the case?
```

---
## \#7 Posted by: paragon Posted at: 2016-01-19T03:53:43.000Z Reads: 190

```
http://www.rcgroups.com/forums/showthread.php?t=952523
```

---
## \#8 Posted by: trbt555 Posted at: 2016-01-19T05:59:53.954Z Reads: 185

```
Continuing the discussion from [VESC noob: what&#x27;s the (edit) capacitor for?](http://www.electric-skateboard.builders/t/vesc-noob-whats-the-edit-capacitor-for/372/6):

[quote="trbt555, post:6, topic:372, full:true"]
Some very relevant pages:

 - [Explanation of the Brushless Motor / ESC System and Capacitor Function][1]
 - [Too long battery wires will kill ESC over time: precautions, solutions & workarounds][2]
 - [ESC capacitors.  What do they do?][3]

  [1]: https://traxxas.com/forums/showthread.php?8958604-Explanation-of-the-Brushless-Motor-ESC-System-and-Capacitor-Function
  [2]: http://www.rcgroups.com/forums/showthread.php?t=952523
  [3]: http://www.rcgroups.com/forums/showthread.php?t=975333
[/quote]
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-01-19T15:15:09.308Z Reads: 170

```
All of this length of cable stuff confirms in my head that monolithic box designs are the way to go for a fully versatile "1 size fits most" box and deck combination.
```

---
