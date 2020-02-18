# Building Your Own VESC

### Replies: 9 Views: 5453

## \#1 Posted by: claudiofiore88 Posted at: 2015-10-08T19:23:43.182Z Reads: 286

```
Has anyone here built their vesc from scratch? How much did it cost you? What were the savings versus buying one from someone like @onloop? Would you say it's worth the savings? I know you can get 3 pcb's made from OSH Park for like $20. I can adequately solder through hole components, but it's pretty daunting even thinking about smd soldering and flashing the firmware and bootloader.
```

---
## \#2 Posted by: sl33py Posted at: 2015-10-08T20:29:31.553Z Reads: 285

```
On my list to try.

I took Ben's BOM and priced it out.  Buying just single components from Mouser is where it gets expensive.  I think you are better off buys in 10's for hte inexpensive parts, then singles of the more expensive components (like the DRV).

Single price for the components was around $65 iirc.  I kept the modified sheet - i'll pull it up and confirm.
EDIT - i was WAY off - single VESC pricing for mouser parts to build was 86.63 before shipping.  building 10 to compare the price breaks was 58.73 ea (almost 600 invested).  Now imagine doing a run of 100!  

So besides the ability to repair and build an extra when needed, it's definitely not cheaper than a single VESC for 100-120'ish (getting the solder paste, no-clean flux, shipping, etc.)

Still think i'm going ot give it a shot sometime soon!

As for SMD soldering - Jamesonotc helped me swap the DRV chip on one of mine that i killed (on the bench on 12s - does not like hard stop/start repeatedly - just FYI don't do it).  After watching him i think i can totally do it.  Do you have a hot air rework on your solder iron / station?

I'll dig up my modified BOM and get some more detail.
```

---
## \#3 Posted by: sl33py Posted at: 2015-10-08T20:40:09.194Z Reads: 275

```
here's a snipped of how i priced this out:
[img]/uploads/db1493/original/1X/ba9e1af253408e89dea0e42d394a219612cb5c2e.JPG[/img]
```

---
## \#4 Posted by: Blasto Posted at: 2015-10-08T21:45:01.493Z Reads: 270

```
I've built 2 VESC for about 110$ each. 3hrs of soldering each. I bought 2 others from from enertion boards because i couldn't be bothered with another 6hours of soldering.

<img src="/uploads/db1493/original/1X/bc6cf76a00c941269f6eb2ef929edc32f1ce7cfd.jpeg" width="375" height="500">

The price break sweet spot is about 10 units, where you can get you BOM down to about 75$ per unit.

The pcbs OSH park is about 40$ for 3 since this is a 4 layer board.
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2015-10-08T21:45:04.901Z Reads: 253

```
Wow, not cheap. I supposed it wouldn't be worth it then unless it's done for fun. I actually do have a hot air rework on my soldering station, but I've never used it for anything more than shrinking heat shrink.
```

---
## \#6 Posted by: claudiofiore88 Posted at: 2015-10-08T21:47:49.573Z Reads: 250

```
This is the one I found already uploaded to OSH Park. It's $19.50 for 3 pcb's.

[https://oshpark.com/shared_projects/cIUJ8Qor][1]


  [1]: https://oshpark.com/shared_projects/cIUJ8Qor
```

---
## \#7 Posted by: Blasto Posted at: 2015-10-08T21:51:20.313Z Reads: 247

```
Oh and when ordering from osh park, make sure you're ordering 4 layers... The side by side pic, thats me transfering all the components from a useless 2 layer pcb to a good 4 layer pcb.

I felt pretty dumb when i realised that mistake
```

---
## \#8 Posted by: Blasto Posted at: 2015-10-08T21:53:48.786Z Reads: 243

```
<img src="/uploads/db1493/original/1X/fbba881d2854ab18a8fdf9b7ca6b8038b458b852.png" width="281" height="499">

Mr wisconsinrobotics is sharing garbage, it's a 2 layer board...

Well i least i'm not the only one who did that mistake haha
```

---
## \#9 Posted by: sl33py Posted at: 2015-10-08T22:07:48.088Z Reads: 230

```
we call that "*practice*"!  hehehe

that sucks!

I'm ordering up some of the CapPCB's from hackvana to see how that process works.  Definitely a lot less expensive than OSH Park - but also about 3 weeks before they arrive.  I could spend another $30 for faster shipping and have it in 2 weeks, but i'm in no rush actually.

Mitch at hackvana was really easy and communicative, so i'd recommend them if you are looking for less expense and willing to take a little while longer.
```

---
