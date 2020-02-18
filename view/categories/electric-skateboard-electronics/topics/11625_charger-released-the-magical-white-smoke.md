# Charger released the magical white smoke

### Replies: 15 Views: 1419

## \#1 Posted by: minimorris77 Posted at: 2016-10-21T15:46:26.143Z Reads: 131

```
<img src="/uploads/db1493/original/3X/2/c/2ce49d74aaf7ab7ce302afee80ce6dc929a15cf4.JPG" width="375" height="500">

Does this pic mean anything to anyone? It looks like I burned up my 4th cell balancing resistors. Does this mean I should only charge up to 3s with this charger?
```

---
## \#2 Posted by: IDVert3X Posted at: 2016-10-21T16:08:29.036Z Reads: 118

```
Just replace the resistor if the traces are okay...
```

---
## \#3 Posted by: Blasto Posted at: 2016-10-21T16:14:49.514Z Reads: 118

```
the resistors are 121Ohm what seems to be 1206 package (1/4W)

but if you burnt these resistors, you may have a damaged mosfet/transistor.

<img src="/uploads/db1493/original/3X/6/3/63bdd6e7c3a5bccbc06498e3d17f4a7873554c27.jpg" width="690" height="481">
```

---
## \#4 Posted by: minimorris77 Posted at: 2016-10-21T16:30:18.663Z Reads: 112

```
<img src="/uploads/db1493/original/3X/c/e/ce61f288d6cd1e74884bb7ea07362d2fbb13c233.jpg" width="375" height="500">

Transistor looks okay but who knows. Can I still use this charger for 3s until I get the resistors swapped?
```

---
## \#5 Posted by: Monte Posted at: 2016-10-21T16:41:33.288Z Reads: 106

```
I think no ones can answer this question correctly. If you still want to use this charger, its on your own risk.(I would not use it ;))
```

---
## \#6 Posted by: chinzw Posted at: 2016-10-21T18:21:52.848Z Reads: 96

```
I believe you burnt your 3rd cell resistors so you'd be able to charge 2s if the board still works.
Btw, how did this happen?
```

---
## \#7 Posted by: Jakebarnhill1 Posted at: 2016-10-22T02:54:15.092Z Reads: 81

```
I agree with @chinzw you burnt your 3rd cell resistors, you should be able to balance charge 2s, but you can still use it to  do a regular charge on any li-po. you can still balance by charging each cell individually :slight_smile:
```

---
## \#8 Posted by: minimorris77 Posted at: 2016-10-22T15:36:16.442Z Reads: 62

```
It is the 4th cell balance resistor. It is set 4 of 6 in the pic. It successfully balanced charged a 3s yesterday.
```

---
## \#9 Posted by: minimorris77 Posted at: 2016-10-22T15:39:02.947Z Reads: 62

```
<img src="/uploads/db1493/original/3X/e/f/efa2c908f4a47f5446c4b15ca95e3e491d1e8e39.jpg" width="375" height="500">

 I made a series adapter, and it didnt like it. Do you see any problems with it? I think it shorted cause my joints are not taped up real good..
```

---
## \#10 Posted by: chinzw Posted at: 2016-10-23T04:33:54.555Z Reads: 53

```
That's not how it should be wired. This is how you do it:
<img src="/uploads/db1493/original/2X/9/93d42fbdc21084daec19f199e9d9bf075d60db12.gif" width="365" height="500">

And if you mix your positive and negative leads you'll fry something too
```

---
## \#11 Posted by: 2-alex-2 Posted at: 2016-10-23T06:02:01.560Z Reads: 50

```
That leads looks fine just maybe more heat shrink. It also depends how your main +\- are wired so take a pic of this and the batteries wired up together.
```

---
## \#12 Posted by: lowGuido Posted at: 2016-10-23T10:12:19.904Z Reads: 43

```
You had the battery balance leads the wrong way around and burt up your resistors as a result. You can remove that bank of resistors and replace them and probably the little transistor on that bank too.
It should still be ok after you replace those components
```

---
## \#13 Posted by: minimorris77 Posted at: 2016-10-26T21:06:01.685Z Reads: 30

```
The idea in my case is to make sure both red wires come from the same battery correct?

How does this look?
<img src="/uploads/db1493/original/3X/2/e/2eabc0696566d63273bcb80cd92b6c44dc2bbf2f.jpg" width="375" height="500">
```

---
## \#14 Posted by: chinzw Posted at: 2016-10-26T21:10:00.064Z Reads: 27

```
I think it looks ok, to make sure, before you plug it to the balance charger just measure the pins to make sure they're working and wired correctly and not inverted

you should get 4.2,8.4, etc if at any point you get a jump bigger than 4.2v then they're wrong.
```

---
## \#15 Posted by: 2-alex-2 Posted at: 2016-10-26T21:56:18.053Z Reads: 26

```
No don't think that looks right connect your batteries as well so we can see them connected to make sure.
```

---
