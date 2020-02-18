# Can someone look at this diagram for a charging setup and give me a hand

### Replies: 9 Views: 371

## \#1 Posted by: CrimzonGryphon Posted at: 2018-11-07T21:02:28.714Z Reads: 81

```
https://i.imgur.com/QlGMfe0.png

Ok so I understand what's happening, don't need an explanation.

My questions:

1. Dumb question: Is it safe to use the XT60 connection as a power switch of sorts? For some reason I feel like the answer the answer is HELL NO.

2. Do I need some special charger to do this? Or is it safe to just use a regular charger.

3. I set the voltage to that of a single battery correct?

Shoutout to whoever invented this solution btw, I love it. And shout out to Dunkirk for the diagram.
```

---
## \#2 Posted by: bigben Posted at: 2018-11-07T21:20:08.856Z Reads: 61

```
You want an xt90-s for a final battery connection so the connection doesn't spark every time it is connected and disconnected. 
In you diagram for charging there seems to be no allowance for balancing the cells?
```

---
## \#3 Posted by: CrimzonGryphon Posted at: 2018-11-07T21:34:02.886Z Reads: 60

```
[quote="bigben, post:2, topic:73851"]
t90-s for a final battery connection so the connection doesn’t spark every time it is connected and disconnected.
[/quote]

That was my concern when I looked at it. People keep saying "use a BMS" and I understand how I'd do that if I were building my own battery with 18650s but I don't get it here. How am I supposed to hook up each cell in the lipo pack to a 10s BMS? Or maybe I only need a 2s BMS? And then I have to worry about currents all over again. Argh!

And is there an elegant solution for balanced charging series packs without having to open up their enclosure and taking the series connector off?

And would I only need an anti spark for the xt90? Is it basically only needed for whichever one I plug in last?

Thanks for your help though you seem to know what you're talking about.
```

---
## \#4 Posted by: CrimzonGryphon Posted at: 2018-11-07T21:38:24.120Z Reads: 51

```
I just realised what the other cables are for on the Lipo packs. Duh.
```

---
## \#5 Posted by: CrimzonGryphon Posted at: 2018-11-07T21:50:54.042Z Reads: 48

```
Also I sketched this quickly. https://i.imgur.com/19QRIJO.png

I'm thinking of making a shroud for the connectors and loop so that they can't be plugged in simultaneously.

Edit: just realised I'd need a weird connector for this.
```

---
## \#6 Posted by: bigben Posted at: 2018-11-07T21:51:20.881Z Reads: 51

```
There's more info than you will ever need on this thread.
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
I built quite a few builds like this and used a bestech bms with switch. They're a good mid range solution with great burst power.
```

---
## \#7 Posted by: b264 Posted at: 2018-11-08T08:34:38.251Z Reads: 34

```
Look at this, except with 2 batteries instead of 5

https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/119?u=b264
```

---
## \#8 Posted by: CrimzonGryphon Posted at: 2018-11-08T13:44:37.750Z Reads: 25

```
That is fairly nice, think I'm gonna go with that now actually.  Some questions:

Are there any major advantages/disadvantages to using the P terminal on the BMS? Can you ignore the discharge current rating of the BMS if you don't use it? The P terminal is for discharge right?

I'm fairly new to BMS, are each of those batteries 2s?

Can you use any regular 36v power source for this?

What happens if you charge with the loop key plugged in?

Is it fairly easy to determine which cell is which from 1-10 if I'm using lipo packs?

Btw I'm posting a parts list in a few hours once I've decided on my charging solution. Stay tuned.
```

---
## \#9 Posted by: b264 Posted at: 2018-11-08T18:25:36.026Z Reads: 21

```
[quote="CrimzonGryphon, post:8, topic:73851"]
Can you use any regular 36v power source for this?
[/quote]

No; not using the correct charger can start a fire.  You should read a lot more on this forum before you start buying or building.
```

---
