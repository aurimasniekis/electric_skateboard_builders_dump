# E-wolf &#124; Loaded Vanguard (flex 1) &#124; Space Cell 10s3p &#124; Abec Flywheels 97mm &#124; Nano-X &#124; Dual 6355 190kV &#124; VESC

### Replies: 11 Views: 2255

## \#1 Posted by: Schulerbible Posted at: 2017-01-21T11:27:45.073Z Reads: 237

```
Hi there,

Just wanted to present my (almost) finished first build. It's a half DIY based on the Raptor V1 technology. Parts used for this build:

Deck: Loaded Vanguard (flex 1)
Trucks: Caliber II 50 degree
Motor setup: dual Enertion 6355 190kV 
Remote: Nano-X
Battery: Enertion Space Cell 10s3p 
Wheels: 97mm ABEC 11 (78a)

Total weight: about 8.6 kg

**Things to do**:
Need to modify the cable length of the space cell, print a new riser with cable holder (only backside), exchange the green straps against black ones and heat shrink the bullet connectors.

The metal enclosure houses the two VESCs which are thermally connected via heat pads.  

Enjoy, more pictures will follow ...<img src="/uploads/db1493/original/3X/6/4/64b9869d258cdc4fb174f572a87a01414b72de00.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/3/4329f18407dd4004e2818dad19fee22bc1d722ac.jpg" width="690" height="388">
```

---
## \#2 Posted by: IDVert3X Posted at: 2017-01-21T13:46:18.368Z Reads: 207

```
You are going to break the battery :slight_smile:
The middle part of the board flexes a lot and battery cant handle the flex.
It's made out of 18650 cells and connected using thin nickel strips.
That's why everybody with Vanguard is doing split encloser design.
Take a look at @whitepony's builds.
```

---
## \#3 Posted by: AndyPG Posted at: 2017-01-21T18:54:44.195Z Reads: 188

```
Wow, some nice hardware there.
Be great to see a video of it in action when finished.

Andy.
```

---
## \#4 Posted by: TranxFu Posted at: 2017-01-21T19:59:21.406Z Reads: 176

```
If he is at this point of the build I think he knows whats up with the flex and battery enclosure situation... Keep in mind that this is the Flex 1 which is quite a lot stiffer than whiteponys flex3. Lets see what he has to say :D
```

---
## \#5 Posted by: IDVert3X Posted at: 2017-01-21T20:13:05.505Z Reads: 166

```
Whiteponny used 42" version, so either Flex 1 or 2. Don't remember which one.
And still, mounting solid part in the middle of a flexy deck is really not that great idea.

@onloop should be able to tell. Space cell is his product :)
```

---
## \#6 Posted by: Schulerbible Posted at: 2017-01-22T00:53:00.842Z Reads: 156

```
@IDVert3X thanks for clarification! I wasn't aware of that :wink:
```

---
## \#7 Posted by: whitepony Posted at: 2017-01-22T01:06:43.345Z Reads: 157

```
i was using a 42" flex2, the flex1 is still a flexy board, so it would kill a battery like a space cell over time, unless it was only loosely mounted (there are ways to mount a stiff battery loosely to a flexy board, for example with extending rubber tubes). your velcro straps might be loose enough that its not bending with the board? bit unfortunate that you velcro'ed it to the most flexing part (middle).

either way, I think it looks a) more elegant, b) prevents flexing of battery and most importantly c) does not interfere with the beautiful vanguard flex if you split enclosures close to the trucks. :slight_smile:
```

---
## \#8 Posted by: Schulerbible Posted at: 2017-01-22T01:07:40.158Z Reads: 152

```
Thanks! Had to change a few components (controller and wheelz) but I am happy with the build. 
Will post a video soon.
```

---
## \#9 Posted by: Schulerbible Posted at: 2017-01-22T01:14:55.719Z Reads: 150

```
[quote="whitepony, post:7, topic:16432"]
your velcro straps might be loose enough that its not bending with the 
board? bit unfortunate that you velcro'ed it to the most flexing part 
(middle).[/quote]

Hmm, that's right. The board flexes about 6-7cm or 2.35-2.75 inches (downwards) at my weight (70kg) when I jump on it. The amount of flex is the same with or w/o the battery.

The velcro straps are tightened in this build!
```

---
## \#10 Posted by: whitepony Posted at: 2017-01-22T08:13:47.150Z Reads: 132

```
well yea, they migt be tight, but its still a comparably loose way of mounting. youre prooving that by saying that your boards flex is not affected ;)

maybe let someone else jump the board and you shoot fotos or look at the battery. not 100% sure how a space cell looks on the inside, but the regular spot weld nickel connections will wear and tear under constant stress.
```

---
## \#11 Posted by: Schulerbible Posted at: 2017-01-22T09:31:00.073Z Reads: 130

```
> well yea, they migt be tight, but its still a comparably loose way of 
> mounting. youre prooving that by saying that your boards flex is not 
> affected

I agree, it's definitely looser than when bolted down. To be precise the spacecell is only fixed at two positions (straps) which prevents flexure of the battery pack. The cell has four contact points (two on each side) which enable contact with the board. Two of these are velcro pads (ie. fixed points) and the other two are felt pads (for improved sliding along the board). When the board changes its shape from convex to concave under the influence of a load (human weight) the effective length of the board changes. That means the battery should only be constrained at one point/line along the deck. All of these pads lower the spacecell by about 1cm (referred to the middle point) from the deck which enables the board to flex. The battery is additionally soft constraint by two velcro pads on each side to prevent lateral movement.

It does not matter which curvature the board has (a) convex, (b) flat or (c) concave there is always a gap between the spacecell and the deck. However, this only works for a light person (60-80Kg) and a flex 1 board (not sure about the flex 2). I do have a spotwelder and I am fully aware about the interior of a raptor spacecell but I did want to keep the pack as is.<img src="/uploads/db1493/original/3X/4/3/43ffc9bc4c4e5b64f484b6a984e34992813f6c93.jpg" width="690" height="266">
```

---
