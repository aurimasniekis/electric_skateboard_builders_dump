# Battery enclosures with removable battery/lids

### Replies: 8 Views: 906

## \#1 Posted by: Vampiresquid64 Posted at: 2017-09-16T22:45:53.970Z Reads: 174

```
Ok so trying to design my own enclosure with removeable/swapapable batteries. my version 1 didnt quite work because I chose to  put the door on the small end which made getting batteries out while not having them move around while riding difficult, and put strain on the wires when I pulled the batteries out. I am now trying to build an enclosure with a larger lid on the bottom instead of the side. the actual mechanics of this is not an issue but the most feasible and cheapest way for me to make this is with my 3d printer which has its weaknesses. I am using petg which is quite strong but its not as good as injection molded. I do have room on my board so I can make it a bit beefy. any ideas? or pictures people can post of 3d printed ones they know of that have swapable batteries? (no screwdriver required pls) sry for the long post. btw I am using 2 5000mah 5s lipos. I can post pics if needed
```

---
## \#2 Posted by: wafflejock Posted at: 2017-09-16T22:54:29.276Z Reads: 172

```
I haven't used this one yet but this is my current working design:

https://cad.onshape.com/documents/15cd342c90ae1b0b6fd666bf/w/40780c7d8d67fd69a32fbf6e/e/fe1a99d1423c52e012228250

It's essentially based on how NAS works and uses a spring load on the removable trays to keep them locked into the outside part.  I printed the inside trays and tested the spring load mechanism and printed the outside in two halves out of PLA to test fitting and in an attempt to make a silicone mold... unfortunately that's as far as I've gotten so far.  The silicone is prohibitively expensive for big parts and pouring liquid into a rubber mold when the part has thin walls doesn't always work how you want it to so I've learned a lot in doing molds with smaller 3D printed parts.  If one can make a mold of the 3D printed part then the poured epoxy plastics/urethanes/silicones can be much much stronger than the original 3D printed part, and you can make many of them quickly compared with 3D printing (plastics can cure in 10min-1hr whereas a big print can be an overnight or multiple day endeavour).

Long story short.. I don't have a working solution yet but I think this design would work assuming you can somehow fabricate all the parts needed or if you somehow have access to a maker space with CNC equipment and can make a mold from metal based on the design instead of trying to 3D print then make a **molded part** from that (a metal mold will cost a ton more if you have someone else do it and even by yourself isn't super cheap but it will last a ton longer than a silicone mold and wouldn't have the problems with thin walls collapsing, the rubber is rubbery).


---

**Edit** some pictures:

https://photos.app.goo.gl/9sBK8wOM0XCLOQV83
```

---
## \#3 Posted by: Vampiresquid64 Posted at: 2017-09-16T23:13:15.960Z Reads: 152

```
ok so those 2 plastic compartments in the middle slide out with the spring loaded mechanism. how do u unplug and plug the things in? cuz all the ports ar opposite the side that you slide them out of. did you just glue the battery connectors to the enclosure? and when U slide it in they connect?
```

---
## \#4 Posted by: wafflejock Posted at: 2017-09-16T23:38:32.861Z Reads: 139

```
Yeah I haven't actually glued them in there but the idea was the inside parts will have a male XT90 hooked up to the 5S 5Ah battery leads, and the parts coming out the side are for making the serial connection between the batteries and for feeding the two wires out to the ESC.  You could try having the wires connected inside the enclosure but I didn't want it to be cramped for space inside of there so idea is the female jacks have their wires sticking outside the box and they make the series connection.  The third XT-90 slot is for a loop key, I'll throw it together here with wires and connectors roughly where they'll go and take another picture (worth a thousand words).
```

---
## \#5 Posted by: Vampiresquid64 Posted at: 2017-09-16T23:41:35.911Z Reads: 127

```
yeah I like that idea. only issue is that it take up more space, but other than that seems decent. is there a spot for the balance lead? or just not cadded in yet?
```

---
## \#6 Posted by: wafflejock Posted at: 2017-09-16T23:52:16.720Z Reads: 122

```
Idea with this was I would just pull the battery trays out to charge and the balance leads have a place to be tucked into the inside trays, it would be nice to have a way to get to them for charging in place but not included yet:

https://photos.app.goo.gl/AkJKG3jYtZYVHLmq2

The "3rd eye" is where you'd plug in a loop key to complete the series connection between the two batteries and the red from one and black from the other go off to the VESC box.
```

---
## \#7 Posted by: Vampiresquid64 Posted at: 2017-09-16T23:57:41.685Z Reads: 118

```
yeah, nice clean solution. why didnt you just make a hole for the balance lead like the one for the xt90? the xt90 is longer so I dont think you would need to worry about it hitting the end when you slide the battery in
```

---
## \#8 Posted by: wafflejock Posted at: 2017-09-17T00:00:44.767Z Reads: 125

```
It might be an option but the little white JST connectors are flimsy compared to the xt-90s so not sure if they'd stand up as well to being swapped out (might be less of an issue though since you only need to take them out if you plan to swap on the road then).  Could also just do a little access panel type thing maybe so you can just slide something back to open a window but more moving parts and I already made the thing more complicated than something I can actually make :)  Thanks for the kind thoughts though let me know if you have more questions but hopefully it gives you some ideas too, I'll try to post back once I get around to actually attempting a mold on this thing or decide to just say f it and use the PLA one until it breaks :)

---

Ah also if you're saying just a hole to make them easier to access when you do slide them out that's an easy addition.  I might do it, thanks for the idea.
```

---
