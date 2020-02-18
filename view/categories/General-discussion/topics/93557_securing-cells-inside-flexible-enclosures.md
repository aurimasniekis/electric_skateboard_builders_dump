# Securing cells inside Flexible Enclosures

### Replies: 16 Views: 376

## \#1 Posted by: ducktaperules Posted at: 2019-05-12T10:30:46.008Z Reads: 171

```
I am building a flexible battery to fit inside a @Kaly segmented enclosure and im trying to work out the best way to securely mount the cells.

My plan was to make neoprene / EPDM sheet that would fold up around each parallel group.

![cellpack|690x435](upload://ozNaQwQETfY3pIdhVuEeLc9Q9dI.png) 

When folded this would protect against vibration. 

![FullBuild%20v6-Cells1|690x322](upload://kXRxVPjXzcrff7svR266ky1K1bT.jpeg) 

Additionally I expect that once they are all packed in together it would add extra isolation to prevent shorts between cell groups. Looks like these should fit sungley inside the Kaly enclosure but will still allow small amounts of movement if needed.

![FullBuild%20v6-cellspackedin|690x322](upload://bYLvdCn6D4s9FBLxfKNubeg58R.jpeg) 

BUT THEN I DECIDED TO SEE HOW @Kaly  DOES IT . . .
After some detective work i found a few images of inside his boards.

![30086913_1667892859932466_5353265598719590400_n|400x500](upload://wHZwUsTtG6jTj34Gj66LiL0QhY3.jpg) 

Looks like hes spadged the cells into place with some type of glue or silicone

![kaly_26071448_143051296405025_252030592189726720_n|400x500](upload://qUxc35gqGATHuCV9OREBQOCbnL6.jpeg) 

Now im not sure what to do . . . .

It seems that gluing them in place does reduce the risk of them ever moving and would reduce strain on connecting cables however i cant imagine that it offers much in the way of protecting against vibration. One thing i don't want is anything that can rattle whilst riding.

**How do you guys mount your cells in flexible enclosures?**

Do you have any positive or negative experiences using either if the methods i mentioned above?
```

---
## \#2 Posted by: Grozniy Posted at: 2019-05-12T11:04:12.984Z Reads: 150

```
I think your method will work perfectly. Just  use silicone wires instead of braid to allow for small movement. And maybe add a cell holder for each pack under the PCB ?
```

---
## \#3 Posted by: pjotr47 Posted at: 2019-05-12T11:13:18.278Z Reads: 150

```
![image|375x500](upload://5SAZrphHUc4DR9cFlYY08lhmcYZ.jpeg) 

I use good quality hotglue. Never had any problem
```

---
## \#4 Posted by: ducktaperules Posted at: 2019-05-12T11:19:43.065Z Reads: 141

```
@pjotr47 That looks great, few questions . . .

* Did you glue under the cells?
* Did you glue round the edges or just in the middle?
* What size braided cable did you use?
```

---
## \#5 Posted by: pjotr47 Posted at: 2019-05-12T11:40:28.355Z Reads: 131

```
Under the cells and in the middle. 

For the size I must check. But take the biggest you can :wink:
```

---
## \#6 Posted by: rojitor Posted at: 2019-05-12T11:41:06.782Z Reads: 127

```
Neoprene keeps the body WARM....keep that in mind if you wrap cells with it.
```

---
## \#7 Posted by: banjaxxed Posted at: 2019-05-12T11:46:47.841Z Reads: 124

```
Having the enclosure carry the weight of the cells puts a lot of strain on the enclosure holes which can deform or split

A lot of folks use 3m strong Velcro to attach the packs to the deck instead.

Enclosure hole splitting is a problem with flexible decks, if the holes are elongated slots instead of holes this may give the enclosure a chance to move longitudinally relative to the bolt a little instead of wrecking the hole
```

---
## \#8 Posted by: ducktaperules Posted at: 2019-05-12T11:54:32.043Z Reads: 120

```
@rojitor this is something that i had not considered. I guess its not a good idea to wrap your cells in heat insulating material.
```

---
## \#9 Posted by: Acido Posted at: 2019-05-12T12:08:27.292Z Reads: 115

```
But that is probably still better than to wrap them in heatshrink, at least the top is open
```

---
## \#10 Posted by: ducktaperules Posted at: 2019-05-12T12:09:35.188Z Reads: 116

```
[quote="banjaxxed, post:7, topic:93557"]
Having the enclosure carry the weight of the cells puts a lot of strain on the enclosure holes which can deform or split
[/quote]

I agree, I actually suffered with this on my previous board. 

![IMG_20180224_183821|690x235](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/b/b/bb7a2f06790afd05bc557ab82ff5de75652f36bb_2_690x235.jpg)

However the Kaly enclosure is quite thick and feels very robust. Additionally there are metal bars that distribute the force at the mounting points. 

It seems like he secures all his cells in his enclosures rather than to the board. Im pretty sure this the the way @Eboosted do their enclosures too. 

I feel like if kaly enclosures were cracking and splitting then this would be bigger news that we would of heard about before.
```

---
## \#11 Posted by: ducktaperules Posted at: 2019-05-12T12:41:52.034Z Reads: 111

```
[quote="pjotr47, post:5, topic:93557"]
But take the biggest you can
[/quote]

I have 2x20mm braiding ![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/1/f1269d61d08c6cd64a9367ece7f9f2053936ea56.jpeg)

But i think its way to much, dont know if it will stay together if i cut it into strips that short and i dont think it will be that flexible over such short lengths
```

---
## \#12 Posted by: banjaxxed Posted at: 2019-05-12T12:47:29.927Z Reads: 105

```
Ah right metal bars did not know, sounds like a good solution
```

---
## \#13 Posted by: banjaxxed Posted at: 2019-05-12T12:49:37.256Z Reads: 104

```
[quote="ducktaperules, post:11, topic:93557"]
dont know if it will stay together if i cut it into strips that short
[/quote]

possible to pre-solder where the cut is to keep from fraying?
```

---
## \#14 Posted by: IndyPilot Posted at: 2019-05-12T13:02:29.447Z Reads: 103

```
Something to think about with vibration - are you trying to shock absorb individual cells or groups of cells?  I would worry more about wiring and electronic components and circuit boards.  

In aviation we snug all the wiring tight with wire ties, zero movement.  I would try to absorb for the electronics though.  For the cells, I’d just try to keep them from being severely jarred, rather than dampening small vibrations.

But I’m a pre-noob at eskate, so take my advice with input from others first.
```

---
## \#15 Posted by: Minim Posted at: 2019-05-12T20:48:07.446Z Reads: 79

```
Check about 15minutes out in this video how the new evolve flexible pack is made. Damn sexy batterypack design! https://www.youtube.com/watch?v=vQQ-FxI5DRo&amp;fbclid=IwAR3EXBlaZwMlDW9LxZl14pQRp8BYWF3v7POAVRkbqSmlo9zoaDh8b0MVtlM
```

---
## \#17 Posted by: Eboosted Posted at: 2019-05-13T03:52:41.744Z Reads: 56

```
[quote="ducktaperules, post:10, topic:93557"]
It seems like he secures all his cells in his enclosures rather than to the board. Im pretty sure this the the way @Eboosted do their enclosures too.
[/quote]

I wonder if that's one of my enclosures.
```

---
