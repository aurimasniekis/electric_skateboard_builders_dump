# Need someone to double check this battery schematic, to do 4way split 10s4p

### Replies: 6 Views: 257

## \#1 Posted by: itsmikeholland Posted at: 2018-10-22T19:47:59.347Z Reads: 65

```
Hey guys!
So im trying to learn to make batteries, I have a hollowcore project board im working on that im trying to fit a 10s4p battery into, but im not sure how to handle wiring a BMS to 2 parallel packs that are split in in half with wire, seems like 12s4p would be easier to split 4ways, but Im curious if I got this diagram right anyways. I read a few discussions on here and this is what I came up with for 10s4p split into 4 equal sections.

Thanks guys! Any input is appreciated, this is my first time at the battery rodeo so any advice would be appreciated! Any alternative schemes are appreciated to! Have a good one!

![20181022_124147|690x335](upload://sMmsK9VNyV48gVbLd4wox0k190A.jpeg)
```

---
## \#2 Posted by: accrobrandon Posted at: 2018-10-25T15:49:52.837Z Reads: 40

```
your arrows are backward... you work from the 1st negative end of the battery... from the vesc in this pic...

the positive wire of number 3 (top left pack) left side... goes to negative terminal of 4....(bottom left, left side)
just like the jumper on yur bottom 2 packs... same deal on the left side... one jumper wire only

and the power wire would go TO the vesc.... but really the bms would be between the battery and vesc...

![IMG_20181025_115507_651~2|690x366](upload://vU7pJaud3TFVoOSH73fL4KXh5Sx.jpeg)
```

---
## \#3 Posted by: DilatedPupils Posted at: 2018-10-25T16:16:40.227Z Reads: 34

```
He's trying to build a 10s4p, @accrobrandon your diagram is making 12s with uneven p groups. It's a little confusing with the way he's doing it but it looks like his diagram is correct.
@itsmikeholland  just curious why the vesc is in the middle, doing a diagonal drive?
```

---
## \#4 Posted by: itsmikeholland Posted at: 2018-10-25T16:33:22.156Z Reads: 30

```
Hey! The vesc and BMS are near the middle since they are mostly thinner than the batteries. theyre not directly in the middle, theyre offset by a few mm so that the center of the hollowcore is an inch thick chunk of wood. im making a bamboo hollowcore and need the center of the board to be as thick with bamboo as possible. the battery is split 4 ways because this will allow for an inch thick "spine" and two outer ribs to reinforce the board from flexing too much despite how thin the wood will be underneath the batteries. The entire board will be just an inch thick so the area under the batteries is just only 5 or so mm!

Do you think the 2 split parellel packs will be problematic? If I go with 12s, we wont need to split any parallels with wire vs strips
```

---
## \#5 Posted by: accrobrandon Posted at: 2018-10-25T17:21:23.203Z Reads: 23

```
Oh yeah maybe... He mentiones a 12s in the original post so thats where I was going...
```

---
## \#6 Posted by: DilatedPupils Posted at: 2018-10-25T17:34:01.867Z Reads: 22

```
Your diagram for 10S should work just fine but If you have resources and everything else, I don't see why you shouldn't just go with 12S, specially if it makes it less complicated.
```

---
