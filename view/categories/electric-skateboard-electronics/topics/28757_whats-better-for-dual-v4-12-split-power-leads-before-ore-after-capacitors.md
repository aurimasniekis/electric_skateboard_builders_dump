# What&rsquo;s better for dual V4.12, split power leads before ore after capacitors?

### Replies: 4 Views: 364

## \#1 Posted by: rich Posted at: 2017-07-27T13:12:54.413Z Reads: 59

```
I am setting up a dual V4.12 (in an aluminium enclosure)  with the smallest possible dimensions and hidden cables. In winter i will add antispark switch, receiver and bluetooth module to the enclosure (now the other electronics are outside because i need to ride!)

<img src="/uploads/db1493/original/3X/f/1/f1a8e142ecb956367e4a831ba93991ab2022c2ac.jpg" width="690" height="388">

So i just want to finish the dual V4.12 and have this question:

Is it better to split the power leads before capacitors that each V4.12 has his own capacitors or put all capacitors in parallel and split the lead after them?

I prefer option 2 but if it's more safe for the controllers with their own capacitors i would do that.
If one fails, would it affect the other V4.12 more with option 1 or 2?

Any Ideas?
```

---
## \#2 Posted by: Maxid Posted at: 2017-07-27T13:20:10.698Z Reads: 54

```
I think more capacitance is always better, so I'd say putting all of them in parallel and then splitting the cable might be better. But that is really only a benefit when one of the VESCs would die so the other could use double the capacitance.
Since I don't hope that happens to you and since it would be a weird "optimization", I'd say that it does not really matter how you connect them. Choose whatever fits your enclosure better.

I am not a specialist on electronics though. Maybe someone who actually knows this stuff can chime in? @SimosMCmuffin
```

---
## \#3 Posted by: rpn314 Posted at: 2017-07-27T13:23:34.326Z Reads: 53

```
I have seen it both ways. It frankly doesn't really matter. The only thing that may make a slight difference is if the distance between the VESC and the caps ends up being longer. You want the wire length between the caps and the VESCs to be as short as possible. Just keep them close by and you should be okay.

The capacitors are in parallel to each other and they'll all still be in parallel no matter where you split them. As for the failure potential (I've never seen those large caps fail, but I suppose it's possible), having them split after would probably be better for balacing what capacitors are left between the two VESCs. If one of the VESCs fails, then the other would still be able to use both and in that case having the caps as close to each other would balance how they're used best.

TLDR: Doesn't really matter for usability. In terms of failure possibilties (caps or VESCs), splitting after the caps is probably slightly better.
```

---
## \#4 Posted by: rich Posted at: 2017-07-27T14:14:10.222Z Reads: 41

```
Thanks @Maxid and @rpn314!  

[quote="rpn314, post:3, topic:28757"]
You want the wire length between the caps and the VESCs to be as short as possible
[/quote]

that's why i want less distance to the caps as original.
it would look like this (cables just for demonstration that you know what i mean):

<img src="/uploads/db1493/original/3X/1/a/1abd521ed48f5b781b8199eada25b837427f09ca.jpg" width="690" height="388">


[quote="rpn314, post:3, topic:28757"]
The capacitors are in parallel to each other and they'll all still be in parallel no matter where you split them
[/quote]

:joy::joy::joy: Jesus!!! You are totally right, i think my whole question makes no sense because it makes no difference at all!
[quote="Maxid, post:2, topic:28757"]
Choose whatever fits your enclosure better
[/quote]

True! That's what i'm gonna do....
```

---
