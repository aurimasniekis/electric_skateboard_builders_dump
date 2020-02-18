# Using copper strips between series groups when (re)building a battery

### Replies: 10 Views: 460

## \#1 Posted by: t0m_r1dd1e Posted at: 2018-05-02T16:22:06.607Z Reads: 120

```
Alright, don't call me crazy but...

I've been thinking about reconfiguring my battery from it's current state as a flat pack, to being stacked. The idea is to put the battery and VESCs between my feet on top of the board so I can get the deck as low to the ground as possible. I don't have access to a spot welder and would rather not buy one just for this. But I'm very confident with a soldering iron. I'm thinking about taking apart the battery, cutting the nickle strips between some of the cell groups, reconfiguring the groups, and soldering them back together them with copper strips. Obviously I'll need to shield the copper with polyimide tape to prevent shorts.

My questions:
1. Is this generally a stupid idea?
2. Is something like this going to flow enough current?https://www.amazon.com/gp/product/B01F1FN488/ref=ox_sc_act_title_1?smid=AT22DXNO0OK49&psc=1
```

---
## \#2 Posted by: banjaxxed Posted at: 2018-05-02T17:14:17.094Z Reads: 112

```
You'll want to be using fishpaper instead of kapton tape
```

---
## \#3 Posted by: deucesdown Posted at: 2018-05-02T17:32:03.865Z Reads: 105

```
If soldering why not use wire? Flat braid if space is an issue.
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2018-05-02T17:45:02.556Z Reads: 99

```
Hmm, I'm not opposed to that. That probably would be easier to work with.
```

---
## \#5 Posted by: t0m_r1dd1e Posted at: 2018-05-02T17:45:09.412Z Reads: 96

```
Ah, good to know, thanks.
```

---
## \#6 Posted by: PXSS Posted at: 2018-05-02T18:14:48.563Z Reads: 87

```
Copper strips don't solder well. The solder joints will break with vibrations. Grounding straps / tinned copper braid solders a lot better. 

The issue still lies in that the cells themselves don't take solder well either. It will look like a solid joint but if you put it through enough vibrations, the solder usually pulls off cleanly from the cells. This is the main reason I would never trust soldered battery packs. 

Welds are a million times better in regards to vibrations. Not only that, but heating up batteries to solder them will reduce cycle life. Performance wise, they will be identical at first but over time, cells exposed to soldering will deteriorate faster, won't hold as much capacity and will sag more. You won't notice this more than likely unless you have a welded pack to compare directly against. 

As far conductivity goes, there is flat copper braid that is 0.25in wide and 0.04in thick on mcmaster that is the equivalent to a 12AWG copper wire. That is what I personally use.
```

---
## \#7 Posted by: t0m_r1dd1e Posted at: 2018-05-02T18:27:39.781Z Reads: 78

```
Thanks for the response.

The cell groups are already welded with nickle strips, so I'd just be soldering to the nickle. Think that would work alright?
```

---
## \#8 Posted by: PXSS Posted at: 2018-05-02T18:41:27.557Z Reads: 75

```
Nickel strip does take solder better than the cells themselves. Solder between cells and not on top of cells and you'll have a much easier time. Take care on the positive side to not melt the heatshrink around the edges as the edge of the cell and the rest of the can is the negative terminal. 

On the negative side, the cells absorb a ton of heat. Work between cells with enough flux with the temp on your soldering iron as high as possible, largest tip you have and limit yourself to 5-8 seconds on the cell. Too much time on it cools down the tip and transfers most of the heat straight into the cell, limiting yourself helps keep the local area hot without sinking that much heat to the cell. 

I have a digital soldering iron which I set to 450C and when I see the temp drop below 410C I stop and move on to a different area. Come back to it after a few minutes.
```

---
## \#9 Posted by: E1Allen Posted at: 2018-05-03T00:08:08.926Z Reads: 57

```
[quote="PXSS, post:6, topic:54152"]
Copper strips don’t solder well.
[/quote]

So I had real good experience with .02 copper strips that I added solder to the nickel then to copper separate then quickly welded them together.  I tried to pull apart it, it wasn't going to happen.  The intent would be to add solder to the series nickel strips then solder copper on top.
```

---
## \#10 Posted by: PXSS Posted at: 2018-05-03T08:58:51.220Z Reads: 50

```
The issue is not can I pull them apart, but will it stand to vibrations. Constant vibration is harsh on solder joints and in my experience I've had to redo more than twice as many joints to copper pads in half the time than I ever did to nickel pads. But again, soldering copper to nickel is way easier than copper to cells but even easier is soldering tinned copper braid. 

Adding strain relief to copper braid is easy so vibrations won't damage joints. The upside to copper plate is that it has a higher current capacity. 

That is just my opinion based on my experience welding and soldering 50+ packs over the past 3 years...
```

---
