# Reducing inductance

### Replies: 12 Views: 2031

## \#1 Posted by: Hummie Posted at: 2016-03-17T05:56:41.162Z Reads: 79

```
<img src="/uploads/db1493/original/2X/0/05e1a19056831509fb441b5c577e7c87187c10af.jpeg" width="375" height="500">I can't get it confirmed/explained better

If inductors in series add up and inductors in parallel are less than the least inductor.. If I need to span a long distance and have a long battery wire wouldn't it be better to have it be a parallel connection?

I'm hoping to mix connections of 18650s with 2 in parallel, then a series connection to two more in parallel,etc..and make the long connections parallel

Only downside I can consider is the slight variation in resistance will maybe slightly unbalance the batteries a bit more

The point is simply to have less need for capacitors with the long wires creating inductance
```

---
## \#2 Posted by: onloop Posted at: 2016-03-17T07:15:24.930Z Reads: 74

```
pick a category, any category... i would say this has something to do with eboard electronics!
```

---
## \#4 Posted by: Hummie Posted at: 2016-03-18T00:03:30.033Z Reads: 59

```
Sorry this is right.  That pic was missing wires

<img src="/uploads/db1493/original/2X/f/f0abe41764e00015673067d0e3ac5495c0d8a8c9.jpeg" width="666" height="500">

I think this is right.  .?
```

---
## \#5 Posted by: lowGuido Posted at: 2016-03-18T23:08:42.561Z Reads: 46

```
I don't see that it is going to make a whole lot of difference.
```

---
## \#6 Posted by: Hummie Posted at: 2016-03-19T01:41:47.815Z Reads: 41

```
I found out that even though the long connections are "parallel" connections they aren't parallel circuits in the true sense of the word ...they're contained within a series curcuit.  The current is going the same way through both wires.  So no reduced over-all inductance.  Series inductances add up but parallel are the reciprocal of the sum of the reciprocal of all the parallelled conductors in a true curcuit.  Ends up being a lot less.  That's what I was going for 
I am going to do the parallel within the series connections though because it's easier and shorter connections.   Two rows of 12 and if I can figure out how to test,..maybe they can cancel each other's inductance if positioned right
```

---
## \#7 Posted by: trbt555 Posted at: 2016-03-19T08:08:46.329Z Reads: 37

```
I think you might be over engineering things.
You should get out more 😉
```

---
## \#8 Posted by: Hummie Posted at: 2016-03-19T15:01:31.072Z Reads: 36

```
I think with 48 cells my connections will likely be getting too long otherwise and I'll have to add capacitors.  I like the challenge.  I have an LC meter that measures inductance but really doubt it can connect to the battery poles without blowing up
This is nothing...wait till you see this pack done. (Potted in 70 duro clear rubber with compression connections) 

I've got nothing to do until my motors show up
```

---
## \#9 Posted by: chaka Posted at: 2016-03-19T15:13:06.292Z Reads: 39

```
I have built packs twice as big as what you are proposing and I have not had any trouble using 3X 680uf caps. Parallel first then series and you will be fine. I have plans for a kilowatt hour pack and I do not expect any trouble with my caps. You should research what the ebike guys have been doing for some real world results.
```

---
## \#10 Posted by: Hummie Posted at: 2016-03-19T15:23:14.341Z Reads: 41

```
Ok thanks I'll just do it then.  
It's said you should add another 220 cap for every four inches of battery wires added 

For my own understanding though, if you know, when u parallel the series chains the inductance is going to be the inductances of all those series chains added together and not ..the reciprocal of the sum of their reciprocal as with a true parallel connections right?
```

---
## \#11 Posted by: chaka Posted at: 2016-03-19T17:29:52.516Z Reads: 37

```
You want to run your cells in parallel first then wire each paralleled pack in series. I connect each cell using cell level fusing to keep a failing cell from taking the whole pack down. Very similar to how the Tesla packs are made. It is extra work but I think it is worth it for reliability.
```

---
## \#12 Posted by: lowGuido Posted at: 2016-03-19T22:21:31.483Z Reads: 32

```
I think you are looking at it wrong @Hummie. the equation you are trying to apply (1/L=1/L1+1/L2) is for pure inductors in parallel.
while these cells are truly in parallel and probably have high inductance Am I right in thinking that you are more interested in the inductance of the wires? in which case you are looking at it backwards the wires are in series and the cells are in parallel.

either way I think its probably so small its not worth worrying about.
```

---
## \#13 Posted by: Hummie Posted at: 2016-03-19T23:24:00.360Z Reads: 31

```
Frustrated by the complication between simply series and parallel.  I think I'll sober up and see how smart I get. I'm sensing I'm banging my head.  

I've been looking for a way to test inductance of the competed battery.  For fun. I'm not too worried about it.  It's magic.  My LC meter I can't hook up to the poles I imagine.  I have no electronics background but am interested...but finding even series vs parallel is showing a growing, enjoyable, complication.  

Once my board is going again you won't even find me here.
```

---
