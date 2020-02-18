# Battery Wiring Diagram Help

### Replies: 5 Views: 1181

## \#1 Posted by: Eric Posted at: 2017-11-22T20:00:58.944Z Reads: 137

```
I haven't been able to find what I'm looking for when wiring up my new 12s8p.  Yes, 8p, it's with those cheap ebay cells, and yes it will be heavy asf.  I drew up a diagram, but realized I only have it for 8s8p, and didn't want to fix it, so just use your imagination. <img src="/uploads/db1493/original/3X/4/e/4e220923c8e9975550d066382f33cf737c2aa1e1.png" width="635" height="500"> So my buddy told me to wire 8 batteries in parallel and then connect 12 of those in series.  Again, this is my first try, so I think I have it right, but I also need help with the balance connectors.  I'm thinking of making it two 6s4p's and being able to plug them into my balance charger, and then they connect in series right before the VESC.  My buddy said this is a bad idea, and I should just buy the bms and charger,  but that's throwing in another $100+.  This layout obviously isn't how it will look, I'm planning on doing two rows going down my longboard, with 2 layers. Let me know with your thoughts and experiences you have on this, thanks.
```

---
## \#2 Posted by: sl33py Posted at: 2017-11-22T20:58:29.317Z Reads: 131

```
You are shorting as you diagrammed it.  You need to disconnect between the Parallel groups as you go in series.  

I'll find a better image or draw one really quick to illustrate.<img src="/uploads/db1493/original/3X/5/2/5203a10c4badbc2e2b2ac4fbdfb87f4cd5326876.jpg" width="690" height="299">

If you measure as you go you will see 4.2 -> 8.4 -> 12.6v... etc as each paralleled group in series increases voltage.  You CANNOT go across like you pictured w/o these important gaps or you are shorting the pack.

Then when you wire your balance plug you attach to each parallel group in series.  I'm not going to draw that out, but a quick search will show you how to do this.

Be careful and triple check!  Even the cheap 18650 cells can provide enough current to weld metal!  (Once. and not work well ever again).  High current is dangerous and I've helped repair a shorted pack...  PITA.  Also make sure you insulate well wherever they could wear through due to vibrations and cause a short.  Fish paper or plastic spacers and heatshrink would be my suggestion.

GL!
```

---
## \#3 Posted by: Eric Posted at: 2017-11-22T21:25:16.623Z Reads: 121

```
Thank you very much.
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-11-22T21:56:49.149Z Reads: 120

```
Here's another good diagram. It's only 10s4p, but you can use your imagination to add the missing cells.<img src="/uploads/db1493/original/3X/7/e/7e43c7258f8629d04064bfdf78f80e5644dbd437.png" width="690" height="446">
```

---
## \#5 Posted by: Namasaki Posted at: 2017-11-22T22:15:38.357Z Reads: 113

```
You would be better off building a 12s 4p out of good name brand batteries like Samsung 30q from a reputable supplier like Lionwholesale.

Because those cheap batteries from eBay could be Chinese counterfeit batteries like the ones that gave hover boards a bad name.

They could even be used batteries that are re-labeled as new. Or low discharge batteries re-labeled as high discharge batteries.

Worst case scenario, you could wind up with a rolling bon fire.

If your going to use a hobby charger and break the battery down to charge it, then you would be better off just using a coupe of 6s Lipos in series.
My first build was 2 6s Lipos connected with 5.5 bullet connectors. That made it easy to hook them up in series and break them apart for charging.

<img src="/uploads/db1493/original/3X/9/3/9367f7e08388a6637b4d6284e81ef498d9d0ad0a.png" width="401" height="499">

<img src="/uploads/db1493/original/3X/6/d/6d2b86fa615bdcc2c6fb8d96db34d8e5863ea4c9.png" width="374" height="499">
```

---
