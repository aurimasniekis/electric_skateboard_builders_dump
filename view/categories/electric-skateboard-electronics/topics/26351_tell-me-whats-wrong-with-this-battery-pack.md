# Tell me whats wrong with this battery pack

### Replies: 11 Views: 914

## \#1 Posted by: rok Posted at: 2017-06-28T19:08:16.380Z Reads: 153

```
I wanna build 10s4p battery. My dad just spotwelded this. He is electrician tho. Anyone here who wants to clarify this?
 
<img src="/uploads/db1493/original/3X/f/1/f1527ba3228c841080d0ba7cecee9883c4a66719.jpg" width="690" height="388">

Also, is this diagram ok? 
<img src="/uploads/db1493/original/3X/6/c/6c016d17970e266fc035001d73d413d8189645a5.jpg" width="666" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-28T19:25:53.369Z Reads: 141

```
It looks right, but it's hard to tell with just a single picture. Why not just use a multimeter on the terminals to see if the voltage is correct.
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-06-28T19:33:12.521Z Reads: 138

```
that's an interesting cell layout. why the shift from the 4 inline to trapezoidal layouts at the end? saving some nickel?

Oh and is that the hole-punch-and-solder method? I use that sometimes when i have to patch in a replacement p-group.
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-28T19:34:49.692Z Reads: 132

```
I was wondering that too, I thought he added some solder over the spot welds for some reason. If he didnt switch the stacking pattern though, the pack wouldn't be as even with one layer being a bit longer than the other.
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-06-28T19:58:54.101Z Reads: 111

```
right, and i think going full trapeziodal on the p groups would use more nickel, so yeah it makes sense i suppose. I have a gut feeling that trapezoidal layouts with cross hatched nickel gives more even cell discharge though. That's why i started doing it.
```

---
## \#6 Posted by: rok Posted at: 2017-06-28T20:07:29.996Z Reads: 104

```
What voltage should be there? How much does the vesc handle?
```

---
## \#7 Posted by: wafflejock Posted at: 2017-06-28T20:12:24.930Z Reads: 102

```
You have 10 cells in series it looks like right? 10S 4P so at 3.8V it's 38V when fully charged will really be like 42V, either way is fine VESC can handle 12S.
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-28T20:13:00.855Z Reads: 100

```
for 10s about 36v +/- 6v.

57v max for vesc
```

---
## \#9 Posted by: rok Posted at: 2017-06-28T20:16:17.513Z Reads: 97

```
Thank you very much sirs!
Another question is my wiring diagram. Do you have any proposition to make about that?
```

---
## \#10 Posted by: Hardwiring Posted at: 2017-06-28T20:35:28.694Z Reads: 89

```
I'm about to do this on a 10s5p.... thanks for great posts
```

---
## \#11 Posted by: rok Posted at: 2017-06-30T09:42:48.647Z Reads: 59

```
Doubled nickel band. The current is over 37v. 
<img src="/uploads/db1493/original/3X/0/7/077ccc13153ac0d507c4504b21701dab4a247392.jpg" width="690" height="388">
```

---
