# Charging Series Batteries in parallel possible?

### Replies: 11 Views: 1286

## \#1 Posted by: Bazingazunga Posted at: 2017-01-14T15:27:18.489Z Reads: 104

```
Quick battery question - i have two 4s batteries wired in series (soldered together). I Also have a 4s Lipo charger. What would happen if i tried to charge just one of the batteries using a 4s JST?

I had a 4S parallel balancing lead from HobbyKing i.e 2 4s JST connectors -> 1 4s connector, didn't think it through and obviously got a big old spark as soon as i connected the batteries. 

Whats the best way to approach charging these batteries? I'd liket to be able to charge them both with the 4s charger if possible.

 Cheers guys
```

---
## \#2 Posted by: abenny Posted at: 2017-01-14T17:03:05.166Z Reads: 94

```
I can't answer the question as to what will happen. But I wouldn't do it, sounds like trouble to me...you should only charge batteries soldered together in series at 8s with either an 8s charger, an 8s BMS, or unsolder them and charge them in parallel as two 4s batteries...
I know none of those answers are what you wanted to hear but I think those are the easiest ways to go about your issue.
```

---
## \#3 Posted by: Bazingazunga Posted at: 2017-01-14T17:05:43.567Z Reads: 85

```
Fair enough mate, thanks very much. Not what i wanted to hear but what i expected to hear!

Think i'll unsolder them, get a bullet connector on each or something then just charge them individually. Should be fine, maybe theyll not be balanced over time but ill worryabout that when i get to it!
```

---
## \#4 Posted by: abenny Posted at: 2017-01-14T17:08:48.143Z Reads: 79

```
Yeah thats almost exactly the solution I had in a very similar battery setup. I had two 4s batteries in series on my board in 8s, and had to remove the batteries to balance charge every time (pain in the ass). Bought an 8s BMS and installed and the board is much cleaner now, and easier to deal with. Only issue was the range was shit, so I upgraded the size of my cells and now get around 20-30km range and can just plug in to an AC adapter that looks like a laptop charger.
```

---
## \#5 Posted by: Bazingazunga Posted at: 2017-01-14T18:04:39.648Z Reads: 68

```
Fully expecting all them issues too, but this is more of a first build so i don't really mind :p in time ill upgrade batteries, and all that other stuff. Your charging solution sounds good to me! 

I just soldered on some bullet connectors now, seems to be working good. Thanks bro!
```

---
## \#6 Posted by: PXSS Posted at: 2017-01-14T18:07:01.848Z Reads: 60

```
What happens if you touch the positive and negative leads of the batteries? Think about how series and parallel connections work and you'll have your answer. Also use the search function of the forum. This question has come up several times in the past 2 weeks
```

---
## \#7 Posted by: Bazingazunga Posted at: 2017-01-14T18:13:02.636Z Reads: 58

```
Mate, dont need to be snide man! I'm fully aware of how batteries work, just had a little brain fart :blush:

Was thinking there might be a way to perhaps snip a positive or negative on the parallel charging harness in order to prevent a short, which seems like semi reasonable logic to me - i'd test it but don't have equipment to spare if it all went tits up. 

I've obviously checked other threads first, most of them concerning how to wire an 8s BMS, but that's not what i'm asking.
```

---
## \#8 Posted by: DilatedPupils Posted at: 2017-01-14T18:29:29.334Z Reads: 48

```
there are actually a few threads here on discharging in series and charging in parallel. use the search function and you will see.
```

---
## \#9 Posted by: PXSS Posted at: 2017-01-14T18:40:36.234Z Reads: 53

```
As @DilatedPupils said. There are several threads pointing out exactly what you are asking. 

In short. You need 2 batteries completely independent with their own deans/xt60. To charge in parallel, you need  a parallel harness on both the balance leads and main leads. To run them in series you need a series harness on the main leads, balance leads disconnected. 

I asked for you to think about how series and parallel connections work so you could come up with the solution yourself as it's really simple.
```

---
## \#10 Posted by: abenny Posted at: 2017-01-14T18:51:08.530Z Reads: 46

```
He already got his answer...I don't see the need to come back with snarky remarks (regardless of their intent)...
```

---
## \#11 Posted by: Bazingazunga Posted at: 2017-01-14T20:56:31.663Z Reads: 40

```
Alright thanks everyone - I mean, all i was asking for was a bit of help, chill out guys we're all in the same boat here.
```

---
