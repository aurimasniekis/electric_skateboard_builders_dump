# Looking for way to switch between batteries in backpack and on board batteries

### Replies: 10 Views: 1422

## \#1 Posted by: BurritoBun Posted at: 2016-04-26T14:35:03.871Z Reads: 153

```
Hey everyone,

I'll start off with my plan. I'm going to be making an electric mountain board, and I will have two 6S 5200mAh in series for a total voltage of 44.4v. My goal is to be able to fill a backpack with more batteries, and to have a system to switch between on board batteries and the external ones in my backpack. How would I go about this? Is there a premade circuit board out there? Or do I have to make my own? If so, where would I find some good diagrams?

Any help is appreciated,

Thanks!
```

---
## \#2 Posted by: Karmannghiagirl Posted at: 2016-04-26T14:44:30.998Z Reads: 152

```
you could do something like this and modify it so you could operate it with your foot, you would have a short period of no power while it switches over, but it would be faster than stopping and unplugging one battery, and plugging in the other.

http://www.westmarine.com/buy/blue-sea-systems--m-series-mini-battery-switches--P009_272_004_505
```

---
## \#3 Posted by: treenutter Posted at: 2016-04-26T14:52:29.129Z Reads: 143

```
That's a good find @Karmannghiagirl I hadn't seen these before.

@BurritoBun if you're plan is to need to swap packs, why not just install packs with more capacity? Assuming you're going to top-mount your enclosure. Mountainboard enclosures usually have plenty of space! You don't need any
```

---
## \#4 Posted by: mattdig Posted at: 2016-04-26T15:07:50.881Z Reads: 129

```
The other option is to not switch at all, put a parallel connection port on the board. But this requires that the batteries in your bag are the exact same as those on the board, and at the same charge level when connected. If you're going on a long ride, just connect the bag to the board before you head out.
```

---
## \#5 Posted by: BurritoBun Posted at: 2016-04-26T15:31:39.869Z Reads: 123

```
I really like that idea. Do you think there's a smaller version of that somewhere?
```

---
## \#6 Posted by: Karmannghiagirl Posted at: 2016-04-26T15:32:38.251Z Reads: 117

```
probably, just search around for marine battery switch.
```

---
## \#7 Posted by: BurritoBun Posted at: 2016-04-26T15:32:46.163Z Reads: 113

```
I actually plan on putting as many batteries as possible on the board, but I'm going to an insane range goal for this board.
```

---
## \#8 Posted by: BurritoBun Posted at: 2016-04-26T15:33:29.252Z Reads: 110

```
That's also a good idea. I'll have to look into that since I don't have a problem using the same batteries.
```

---
## \#9 Posted by: BurritoBun Posted at: 2016-04-26T15:35:42.832Z Reads: 103

```
I actually found a few diagrams as to how these work, so I might try to source some components and see if I can throw them onto a board.
```

---
## \#10 Posted by: Karmannghiagirl Posted at: 2016-04-26T15:39:27.049Z Reads: 100

```
Another thought I just had is that you can get a single pole double throw relay, and wire it up so when one battery dies it automagically switches to the other (using some sort of low battery warning device that is seperately powered). http://www.learningaboutelectronics.com/Articles/How-to-connect-a-single-pole-double-throw-relay-in-a-circuit
```

---
