# How to calculate center to center distance with an Idler Pulley?

### Replies: 6 Views: 2006

## \#1 Posted by: JLabs Posted at: 2017-08-19T19:09:30.403Z Reads: 141

```
So after all the buzz about idler pulleys, I figured I would implement them into the next versions of my motor mounts.. I am running into trouble calculating what center to center distance to use and what belts would properly fit common gear ratios (32, 34, 36, 40, 44t wheel pulleys and 14, 15, 16t motor pulleys).

Any help is greatly appreciated!!

Jared
```

---
## \#2 Posted by: PoorlyExecuted Posted at: 2017-08-19T20:01:59.906Z Reads: 135

```
You can mock up pulleys and idlers by using a cad program of some sort. In Fusion 360 you can make a shape and then measure it's perimeter http://i.imgur.com/MWtO8aL.png. Perimeter is listed as loop length in Fusion. You'll need to make sure that there aren't any lines on the inside of the shape in order to make it easy to measure. It can give you a rough idea of what belt length you are looking for. I imagine that you aren't looking for something too precise though since generally one of the pulleys is adjustable Arranging pulleys to a specific belt length though is mostly trial and error though.
```

---
## \#3 Posted by: pakue Posted at: 2017-08-19T20:03:32.500Z Reads: 134

```
Not sure if there is a formula to calculate the center distance with an idler, but maybe [calculate](http://pic-designcatalog.com/CGI-BIN/lansaweb?webapp=WCALC+webrtn=bpCalc+ml=LANSA:XHTML+partition=DEV+language=ENG) how much "extra" belt slack you have from a gear ratio with the biggest pulleys (e.g. 44t - 16t) and smallest (32t - 14t) and see if you can compensate that with your idler range.
```

---
## \#4 Posted by: Cobber Posted at: 2017-08-19T20:19:34.361Z Reads: 122

```
Eww... with out the idler from a geometry perspective (I'm not a ME):
Belt length is half the circumference (not radius) of both sheaves plus 2x the shaft center distance without accounting for belt thickness or stretch.
With the idler the math becomes real messy, i'd do the above calc or use [one of the many online](https://www.google.com.au/search?q=calculate+belt+length+for+pulleys&oq=calculate+belt+length+for+pulleys&gs_l=psy-ab.3..35i39k1l2j0i22i30k1l2.252603.255546.0.256757.18.12.0.0.0.0.473.2258.2-1j3j2.6.0....0...1.1.64.psy-ab..17.1.473.BmASW8f_ABk) to calc. length sans idler as a guide then i'd get out my compass & ruler and draw it. Then measure with string. Or measure on your board with a dummy idler and string.
All of that said there is a pretty standard deviation of pulley diameters, distance between pulleys and idler size and belt deflection and collective experience should be able to yield a rule of thumb answer such as: +10-15mm to your usual length.
I'll be interested to see what the answer is.
```

---
## \#5 Posted by: SilentException Posted at: 2017-08-19T20:59:38.457Z Reads: 115

```
Basically you calculate belt length as you would normally and then count in the difference made with the pulley. Sounds more simple than it actually is but here are few calculations I just did that could be helpful.

<img src="/uploads/db1493/original/3X/1/7/178e7ed29a64ea877afebbc65dab34dbd53e5d5b.jpg" width="322" height="500">

You know both radiuses and the center distance so you calculate the theta θ angle. After that you can calculate the X part of the belt.

Edit: While doing this, calculating the angle seemed like the most important part but now I remembered that it is not necessary. You can get X by doing X = sqrt(C^2 - (R-r)^2)
:)

Now you count in for idler deviation over the X part of the belt. At the end you get "Bi" which was meant as belt difference to be added to normal belt length (without idler).
```

---
## \#6 Posted by: JLabs Posted at: 2017-08-19T21:29:16.010Z Reads: 105

```
Wow, thanks for all the great info guys!! @SilentException @PoorlyExecuted @pakue @Cobber
```

---
