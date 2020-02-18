# Cell level fusing for esk8

### Replies: 10 Views: 393

## \#1 Posted by: Moja Posted at: 2019-10-12T20:21:28.328Z Reads: 89

```
Regarding battery safety, I have witnessed a pack blow up and it was a big explosion. I want to use cell level fusing on my boards from now on. 

Tesla use cell level fusing that uses copper wire between each cell that act as fuses. I just came across this awesome design that would take less space in the design of the pack, although they have only developed strips that handle up to 3 amps. 

Has anyone implemented cell level fusing on their boards so far? 

https://batteryhookup.com/collections/cell-level-nickel-fuse/products/nickel-fuse-2p-wide-continuous-roll-by-the-foot-18650-cell-level-fusing
```

---
## \#2 Posted by: Shred_Sheran Posted at: 2019-10-12T20:35:34.217Z Reads: 88

```
This actually looks rather cool, If only i knew about this.

That said if the boad is going to be of any real speed you are likely going to be pulling 10amps from a battery that is a 6p, more if its smaller
ideally if there was one that could handle 20 amps that would be the winning ticket on this idea.
```

---
## \#3 Posted by: bigben Posted at: 2019-10-12T20:44:39.733Z Reads: 80

```
Hi Moja, @Kaly does it on all his boards and is now incorporating really neat PCBs.
Check out his instagram.
https://www.instagram.com/nyc.kaly/
```

---
## \#4 Posted by: DJase Posted at: 2019-10-12T22:19:08.921Z Reads: 76

```
I need that setup for my haya 🥺
```

---
## \#5 Posted by: jasonbhuynh Posted at: 2019-10-12T22:53:21.888Z Reads: 74

```
Those are far too low amperage for our purposes. We use up to around 20a per cell on 30qs, but the nickle strip fuses you linked say they blow fast at 8a and support 3a continuous. Once they have higher amperage versions available then this product will be more viable.

That being said: this has been discussed before here: https://www.electric-skateboard.builders/t/fishpaper-and-cell-level-fusing-use-it/35026

Some builders use it, some don't. I've done it on some batteries and skipped it on others personally. It increases the amount of labor to build a battery by quite a bit. I only build batteries for myself though.
```

---
## \#6 Posted by: skatardude10 Posted at: 2019-10-13T01:17:21.773Z Reads: 66

```
I'd love to know or see some data on voltage drop from the resistance of fuses in a pack. 

Just doing some rough calculations, depending on what material and thickness and length of fuse wire you use, say 22AWG copper or Aluminum in a 4P group there could be anywhere from 0.05 to 0.2v drop more or less per P group, meaning anywhere from 0.5v to 2v of voltage drop in a 10S pack from adding fuses alone. 

Under full load, 2V extra drop ontop of the cells internal resistance/voltage drop under load is kind of substantial, especially if you are already using saggy cells and pulling high amps (my 25r pack would drop 9v under load, this is already pretty shitty but add fuses and 11v drop would be absolutely unacceptable) But I guess it's not that bad if safety is a huge priority.

one interesting thing about cell level fusing, correct me if I am wrong someone @professor_shartsis, but cell level fusing is basically pointless in 2P and probably pointless in 3P. If a cell internally shorts, the adjacent cells have to be able to deliver enough current without blowing through their fuses but still enough to blow the shorted cells fuse. If it's 2P, that means both fuses would blow [good, but completely dead pack now], or both would just dump as much current as they can and not blow the fuse if the current they can provide is less than the fuse you chose will blow at or if your fuse doesn't blow in time before the cells sag and IR rises to drop the shorted current below the load that would blow your fuse and you still have a short- I think this is why careful selection of fuse material and thickness is critical...
 not sure just spitballing. I've never intentionally shorted an 18650 and measured the current... can a cell like the 25R deliver 40+ amps or something crazy higher if shorted? 

Nevermind, just reading up on a cells internal resistance, if a 25R is about 10mOhm, at 3.6v that means it can short at 360A, and assuming IR will rise and voltage will drop super quick under this load but I guess this is why shorted cells spark so violently.

Tesla cell level fusing is ideal because they have like 100+ cells in parallel, and if one goes out it's easy peasy for the 99 other cells to blow that one cells fuse and still have the headroom to keep operating normally as a P group.
```

---
## \#7 Posted by: mishrasubhransu Posted at: 2019-10-13T04:52:06.100Z Reads: 52

```
They say that you can stack them for higher amps.
```

---
## \#8 Posted by: jasonbhuynh Posted at: 2019-10-13T05:06:07.982Z Reads: 55

```
that is one option with the kit. However, you need to make extra sure that your welds are strong enough, as nickel to nickel welds are often harder to do properly compared to nickel-steel welds. That being said, it's certainly safer to lose 1p to a loose weld than it is for your entire board due to thermal runaway.
```

---
## \#9 Posted by: Kaly Posted at: 2019-10-13T22:47:07.817Z Reads: 42

```
Hi 
Just shipping in. :slight_smile:

For small packs your logic is true.
What i like on the fuses is that is better to be safe and if there is an issue the user will notice since the rest of the cells in the parallel pack will likely blow the fuse too.

it is way better to open up and check what is going on than to deal with a big problem.
```

---
## \#10 Posted by: elhnad Posted at: 2019-12-06T04:59:54.446Z Reads: 10

```
The only thing i can think is this would seem  more annoying if you had to find and replace a bad cell
```

---
