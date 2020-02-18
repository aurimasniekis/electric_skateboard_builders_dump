# Wiring schematic

### Replies: 9 Views: 2264

## \#1 Posted by: Koto Posted at: 2016-12-07T00:30:29.471Z Reads: 170

```
Where should i put a buck module / UBEC for LED or USB port? Will it work? The motor is 245kv 
<img src="/uploads/db1493/original/3X/1/9/1984360150725e056f21edb5c4ee5bdf4b61c0aa.png" width="499" height="500">
```

---
## \#2 Posted by: rpn314 Posted at: 2016-12-07T15:41:27.742Z Reads: 116

```
Motor and battery combination looks fine, so does the anti-spark switch (at least that's what I assume the yellow rectangle at the top is)

I'm a little confused by the black wire going between the two yellow rectangles in the middle...
```

---
## \#3 Posted by: DreadBiscuit Posted at: 2016-12-07T15:56:48.938Z Reads: 107

```
@rpn314 I believe Koto is identifying the series connection of the two batteries at that point - as everything else is red-to-red and black-to-black.  This is going to be a 8s setup, correct @Koto?  It all looks good to me as well. 245kV will work.  I will be running 8s on my build and I am using a 240kV motor.  Check this out for more information about motor kV

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125


Just out of curiousity, what are the rectangles labeled 'F' at the corner of each battery?
```

---
## \#4 Posted by: rpn314 Posted at: 2016-12-07T16:13:45.635Z Reads: 76

```
Ah yes. I got lost in all the lines I guess. Sorry, it's the last week of my classes here for me. My brain is a little fried.
```

---
## \#5 Posted by: DreadBiscuit Posted at: 2016-12-07T16:15:11.771Z Reads: 68

```
Ha, I understand that, I'm writing my graduate thesis in the library as we speak!  Here we both are, one week before finals, playing on an electric longboard forum...priorities, right?!  LMAO!  This has been my brain break from the weight of deadlines crushing down on me.
```

---
## \#6 Posted by: Koto Posted at: 2016-12-07T22:21:27.310Z Reads: 58

```
Just to clarify, all yellows are connections (Xt90)
```

---
## \#7 Posted by: Koto Posted at: 2016-12-07T22:22:29.949Z Reads: 56

```
And the F was kind of mistake, it was supposed to be a female xt90
```

---
## \#8 Posted by: jmasta Posted at: 2016-12-07T22:27:41.796Z Reads: 55

```
[quote="DreadBiscuit, post:5, topic:14290, full:true"]
Ha, I understand that, I'm writing my graduate thesis in the library as we speak!  Here we both are, one week before finals, playing on an electric longboard forum...priorities, right?!  LMAO!  This has been my brain break from the weight of deadlines crushing down on me.
[/quote]

Well that makes three of us!  @rpn314 @DreadBiscuit

This is more important than grad school, right?  Right!?!?  

:sweat:
```

---
## \#9 Posted by: Koto Posted at: 2016-12-08T00:24:00.254Z Reads: 51

```
[quote="DreadBiscuit, post:3, topic:14290"]
correct
[/quote]

yep, thats a series connection to make it 8S... hopefully
```

---
