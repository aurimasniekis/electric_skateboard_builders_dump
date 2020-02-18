# Connecting curved parallel batteries in flat series

### Replies: 5 Views: 555

## \#1 Posted by: Brad Posted at: 2017-05-06T19:12:45.299Z Reads: 110

```
I have been thinking about having a Sanyo GA 12s5p battery made for my board soon. 

I wish to keep the compartment slim and the board will be 10 inches wide, allowing me to lay the pack sideways, meaning series goes along the length and parallel goes along the width (L 39.18cm x W 18.5cm) instead of the usual series goes width wise and parallel goes length wise.(L 55.5cm x W 13.6cm)

The wheelbase is 29 inches and 55.5cm wont leave much room at all between the battery and the motors. 

I'm aware that I could lay out the battery in three series width wise making the dimensions (L 37cm x W 19.59cm), however the board will not be slim along the edges because of the concave making the appearance more like a Metro-board from sideways. (No offend intended to Ilan!)

With the series traveling along the length instead of the width, I can get the pack to hug against the board into the concave sides keeping the slim look and also needing much less wire as the positive will be on one side and the series will turn around back at the other end, meaning the negative will end up at the same end as the positive!

The problem I'm having is working out how to use nickel strips to connect each series as there will be a slight curve so just simply folding the series back straight after wielding is not going to work. 

Have any of you tried this or know someone who has done something like this before?
```

---
## \#2 Posted by: sl33py Posted at: 2017-05-06T19:25:30.522Z Reads: 109

```
I'd loop in one of the experts who build 18650 packs - @barajabali.  

As for curving the nickel - if it won't bend to conform to the curve - perhaps breaks periodically w/ braided flat wire, or 12/10awg wire to get the flex/bend?

I'm a visual person - can you lay out the batteries and show us how you want to build to confirm?

GL!
```

---
## \#3 Posted by: Brad Posted at: 2017-05-06T20:14:53.212Z Reads: 92

```
Pardon my third rate photo-shopping.

Series side ways makes the sides thick from the concave. Concave is not to ratio.
<img src="/uploads/db1493/original/3X/1/5/15be071c2e74548280243f22d073c32814c147a8.jpg" width="266" height="284">

Not at thick if series is length ways.
<img src="/uploads/db1493/original/3X/1/3/13092709765d462d8ec6ccd0a543a14b1c309bc5.jpg" width="266" height="284">

Diagram of battery layout.
<img src="/uploads/db1493/original/3X/f/d/fd55b9cd0edff48618a4c5751f86699c383b5af5.jpg" width="513" height="277">

I have been thinking that maybe it could be forced back straight albeit with a wrinkled buckle here and there as the concave is not that severe. Back straight as in fold the nickle strips so the series is in line instead of the series being folded beside each other to have it wielded together.
<img src="/uploads/db1493/original/3X/8/a/8afb98438372f08a5e302efe1d77f9cc39d55898.JPG" width="400" height="98">
```

---
## \#4 Posted by: sl33py Posted at: 2017-05-06T21:12:37.165Z Reads: 75

```
That looks pretty doable.  of the 5p - the outside 2 or 3 might be angled slightly.  Either a small crease/fold in the nickel - or use some braided flat wire or 12/10awg to bridge that gap and let them fold over to conform to the deck bottom?

I might try to build a curved clamp jig for the battery pack as you build?  you could also cut the nickel strips and rotate/angle them in-between each battery or every few batteries to conform to the bend you want.
<img src="/uploads/db1493/original/3X/f/f/ff94030702e421a99355314472b2e63345439cff.JPG" width="321" height="169">
I see your "third rate photo-shopping" and *raise you* my crappy mspaint...  ;)

I would see the first 3 welded to the strip w/ your 4-6 welds, then layer another on top of the last angled to the 4th battery and spot welded another 5-6 times to the below strip already welded.  repeat/layer and angle to reach the 5th battery.  Am i making sense?

I love a low profile build where the batteries are super slim and unobtrusive...  Look forward to seeing your setup!

HTH!
```

---
## \#5 Posted by: Brad Posted at: 2017-05-07T04:16:35.363Z Reads: 56

```
Yes it makes sense, but somewhat concerned about current flow.

I assume you mean the inside 3 parallel side by side to the other series 3 parallel, have both wielded together to make 2s3p, then layer a separate strip not connected to the other 1s5p and wield the second strip of nickel to the other 2 cells to change it to 2s5p. Once that is done, fold the strip that connects the two 1s5p via the inside 3 cells in the to make the two 1s5p head to head instead of side by side.

So the reduced area for current to flow through is not going to be much of an issue? Current from the cells on the edges will have to travel sideways to reach the inside 3 cells area before flowing through to the next series, repeat 7 times to complete the circuit.

If that is an issue, then may have to opt for flat wire to connect the nickel from the outside 3 cells with the next series outside 3 cells.

Another idea which would be so much easier is to cut out a curved nickel strip, wield it on each 1s5p, and just solder each 1s5p together in between the cells to avoid too much heat?
```

---
