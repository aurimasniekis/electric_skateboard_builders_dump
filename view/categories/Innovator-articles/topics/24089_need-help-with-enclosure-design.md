# Need help with enclosure design

### Replies: 8 Views: 856

## \#1 Posted by: mm6ix Posted at: 2017-05-28T21:44:31.530Z Reads: 154

```
I just started designing an enclosure for my board using fusion360, i'm new to the program and don't really know how to move forward with my design. 

Currently I have a basic design for the enclosure (to fit a 10s3p, BMS and a VESC) and a 3d scan of my deck with the battery sitting on top of it, like so: (scan only consists of about 4/5 of the board)
<img src="/uploads/db1493/original/3X/0/0/0059f4c10c97eab67fab446f399977eba49813c6.png" width="690" height="385"> 

As you can see above there are side channels on the deck so I cannot just design a flat lip around the entire enclosure because it wont sit on a flat surface. 

Another pic of the board: (click to enlarge)
<img src="/uploads/db1493/original/3X/6/c/6c6bd38408b9e79daae7cdca79a391a8bebe2e83.png" width="213" height="500">

I was wondering if it was possible to somehow extend the enclosure into the curves of the deck and get a enclosure that is perfectly contoured to the deck. Or similar to cutting a model with a plane instead cutting the model using the scan of the deck. 

I've searched online but have not found any answers. Does anyone know what search terms would help me find a tutorial or solution for this? Also any other suggestions for a solution are welcome.
```

---
## \#2 Posted by: mm6ix Posted at: 2017-06-03T15:57:21.906Z Reads: 110

```
So I've decided not to drop the enlosure into those side channels but instead, just fill them with some putty or something and just make an enclosure that contours to the shape of the deck. 

I've got a decent enclosure design but have a really stupid problem, I'm sure it a super simple solution but fusion360 is not letting me make the changes I want to. 

<img src="/uploads/db1493/original/3X/1/7/1799dc0dbe0122eb4193e26fa6edc06d9e5ef16e.png" width="673" height="189">
<img src="/uploads/db1493/original/3X/c/7/c70ddee8613f4bd42bd5a9714ce390a64a1289b6.png" width="505" height="171">

Basically I'd like to put a few cutouts on the highlighted face for a battery meter, on off switch, charge port and the 3 motor wires. But for some reason it's just not working. Anyone know what the problem might be?
```

---
## \#3 Posted by: L3chef Posted at: 2017-06-03T20:15:46.978Z Reads: 101

```
I'm not on a computer right now, so this is just off the top of my head.
Model- Sketch-rectangel(or what shape you want to cut out) choose correct plane and draw cut out.
Then right click on the cutout and "push" and push through the model. Select " cut" under operation tab.
Should do it.
```

---
## \#4 Posted by: mm6ix Posted at: 2017-06-03T21:52:01.355Z Reads: 96

```
Tried doing that doesn't seem to work. I think it has to do something with the way I modeled it, I think I unnecessarily  over complicated the model and sketches and now that face is locked or something. Been trying to figure this out for days, its the last step before I send the file to get printed.
```

---
## \#5 Posted by: L3chef Posted at: 2017-06-04T07:55:08.464Z Reads: 87

```
Yeah it can be due to the sketch it wont allow you. 
You could try to cut it from either under or over the model. sometimes it helps to change directions.
```

---
## \#6 Posted by: mm6ix Posted at: 2017-06-04T18:04:17.150Z Reads: 76

```
Finally figured it out, the part was an assembly of two different models. So I just had to make the cuts in the original model and it just updated in the assembly.
```

---
## \#7 Posted by: SirDiff Posted at: 2017-06-04T21:33:37.465Z Reads: 68

```
How did you get the 3d scan of the board?
```

---
## \#8 Posted by: mm6ix Posted at: 2017-06-04T22:41:37.758Z Reads: 63

```
I borrowed a 3d scanner from my local library
```

---
