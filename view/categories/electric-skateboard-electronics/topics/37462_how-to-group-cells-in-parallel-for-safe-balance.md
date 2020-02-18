# How to group cells in parallel for safe balance

### Replies: 13 Views: 756

## \#1 Posted by: D_Sk8 Posted at: 2017-11-06T02:23:07.055Z Reads: 115

```
I'm having a hard time tracking down any info on grouping cells together in parallel with a single BMS. I've seem a couple videos and not certain of a couple things. 

After testing the capacity of each cell and determing the capacity of each:

1. How much variance is acceptable? What's the biggest variance we've worked with without seeing an issue. 
2. It seems to make more sense to make certain each set of parallel cells are as close to the same capacity so when charging them to 4.2 volt, none of them get overcharged but I think I saw a video where someone specifically selected cells with a low and high range but the total capacity of each set of (what I think was) parallel set of cells ended up being the same across the series of parallel cells.

Long story short, I have 60 cells ready to build a 12s5p and they are all between 2000-2150. If I group the closest 5 cells based off capacity, for example, one parallel set will have a total mah of 10,000 and most will be closer to 10,750, which is a 7% difference. The parallel set will hit 2.8 volts 7% faster than the highest set. Is that the best way to move forward or is there a better way to group the cells together. I think the video that I think I understand was someone grouping small and large together is confusing me.

Any help is greatly appreciated.
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-06T03:40:19.207Z Reads: 98

```
Cells in parallel behave as if they were all just one big cell, No need for anything special. Cell-level fusing is a good idea so that if any one cell fails and goes short circuit it won't damage the others in the parallel group, but not everyone uses this.

If you have mismatched cells in **series** however, that's where the problems happen.

Basically you want each of the 12 5p packs to have the same capacity. It doesn't matter if you have the highest and lowest capacity individual cells in the same pack or different, just that the whole pack has the same total capacity as all the others.

Cells in parallel share voltage between themselves since they're essentially shorted positive to positive, negative to negative. Any voltage variation initially will be rapidly equalized.
```

---
## \#3 Posted by: D_Sk8 Posted at: 2017-11-06T03:48:53.460Z Reads: 82

```
Aww, I got confused. So I need 12 cells with nearly the same capacity so the BMS charges the 12 to 50.4v and the assumption is each will be 4.2v each. I guess that should also make the difference between each series a little closer together although the difference in mah per cell in series could be a decent rage, I figure 3-4% between high/low.
```

---
## \#4 Posted by: baxter Posted at: 2017-11-06T03:54:45.454Z Reads: 76

```
Try a google search for “bottom balancing”
```

---
## \#5 Posted by: D_Sk8 Posted at: 2017-11-06T04:43:22.214Z Reads: 71

```
I guess that's my problem. My question involves bottom balancing, I thought. 

All cells I have are now 2.80v. 

My current understanding (or misunderstanding) is that my balance lead will be connected to 1 of the 12 groups of cells. I assumed that meant the lead would charge the 5 batteries in that group (12s5p) until the BMS reads 4.20v. I assumed that meant the BMS reads the voltage of the 5 batteries and one of the 5 would reach 4.20 where, maybe, a larger capacity cell could be at 3.70v, which is an average of 3.95v. The 4.20v would continue to charge until the total average is 4.20v.

Of that's wrong, anyone have anything in layman's terms to help correct it.
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-11-06T04:44:12.712Z Reads: 62

```
Parallel cells are basically shorted together. Any one cell in a parallel pack cannot get a different charge voltage then eny of the others, because they're connected together. If the parallel pack is 4.2v, ti's guaranteed that every one of the cells in it will be as well.

If your whole series pack reads 12*4.2, and some of the sells in series have different capacities, that's where you have balance issues. 

A BMS will help keep everything happy even if there is a slight mismatch.
```

---
## \#7 Posted by: D_Sk8 Posted at: 2017-11-06T05:37:28.746Z Reads: 61

```
Aww ok. So even when the BMS cuts off at 4.20v, any of the smaller batteries will steal energy from the other ones and it will start charging again until they are all 4.20v, that makes sense, thank you.

Would it then make sense to try to build each series with the same mah capacity, or try to keep the mah the same  with the 12 batteries in the series and not worry too much about the overall capacity of each series?
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-11-06T05:43:30.821Z Reads: 62

```
Take a look at this diagram:<img src="/uploads/db1493/original/3X/3/9/3999003e056932ffc1c887a8b9bc2c7c49742d44.png" width="690" height="478">

The blue wires are for the BMS to balance.

The BMS doesn't know (or care) if you have 1 or 100 cells in parallel, since electrically each parallel pack behaves like one big battery.

You should try to make each 5p have the same capacity as all the other 5ps.
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-11-06T05:54:48.126Z Reads: 51

```
Let's say you check each cell, and you have 12 that are either way higher or way lower than the rest. Let's say they came from a different source or are a different brand, whatever.  It's best to have them distributed like this:<img src="/uploads/db1493/original/3X/1/3/13111bd9cf65f79b8f5d88c845c24c03c6473009.png" width="690" height="478">
than like this: <img src="/uploads/db1493/original/3X/c/4/c42cc45ca11eeffdf141bbdd428328fc0e23b753.png" width="690" height="478"> because in example two, you'd have just a few 5p packs with different capacity than the rest, which will lead to unbalanced charging.

In example 1, each 5p pack has just one different cell, so they all have the same capacity. They all match.
```

---
## \#10 Posted by: Colson003 Posted at: 2017-11-06T05:54:57.932Z Reads: 50

```
@MysticalDork might wanna filp the middle column  + and - labels :wink:
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-11-06T05:55:53.968Z Reads: 52

```
lol I just saw that. It's a pic I grabbed offline, don't blame me :P **edit** fixed.
```

---
## \#12 Posted by: D_Sk8 Posted at: 2017-11-06T15:19:02.756Z Reads: 46

```
Awesome ya'll, thank you. I am gonna start today so I appreciate the feedback.
```

---
## \#13 Posted by: MysticalDork Posted at: 2017-11-06T18:11:03.560Z Reads: 35

```
Take a look at the "fish paper and cell level fusing" thread, they've got some good info on there.
```

---
