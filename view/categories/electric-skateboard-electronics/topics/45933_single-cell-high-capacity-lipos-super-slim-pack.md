# Single cell high capacity lipos? Super slim pack?

### Replies: 9 Views: 1007

## \#1 Posted by: BenTheBarre Posted at: 2018-02-09T04:30:41.258Z Reads: 154

```
Hey guys. Browsing eBay I stumbled upon this- 

https://m.ebay.com/itm/3-7V-10000mAH-8870129-8873130-LiPo-Li-ion-Polymer-Rechargeable-Battery-/232410445121?_trksid=p2385738.m4383.l4275.c10&_mwBanner=1

How would you feel about building a super slim 10s or whatever pack with these?? Has anyone done this? Is there a lot of risk involved directly soldering individual lipo packs??

Pretty inexpensive as well. Id be skeptical of the quality of the cells though, at that price point.
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-02-09T04:45:59.308Z Reads: 151

```
Most lipo cells have aluminum tabs, which means regular solder won't stick to them, no matter how much flux you use. You can either spot-weld the tabs or get special aluminum solder and flux.

I've seen several builders that have taken apart multicell lipo packs to rearrange the cells into a thinner pack. It's a delicate and involved process.

Lipos are fussy, delicate and always want to be on fire at the best times. I personally wouldn't touch this project with a 10ft fireproof pole, but that's just me.
```

---
## \#3 Posted by: DanSkates Posted at: 2018-02-09T04:49:20.279Z Reads: 145

```
I can't comment on the quality or process as such but I've also been wondering whether this would be a good way to go if you were to build with lipos just because of how you could design the packs - and how slim you could get it to the deck.

I came across this video and quizzed the guy in the comments on the pack he was using and he evetually shared with me his build thread:

[Youtube Video](https://www.youtube.com/watch?v=kxKRKMB9dnU&lc=z22nvz0h3sbdgx5fkacdp435xw5flubf2sbhme2lmgpw03c010c.1517889281652966)
[Build Thread](http://cafe.naver.com/electriclongboard/39129)

So totally doable.  

I'd also be really intersted to hear others experience building with single cell lipos and any options for quality cells.
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2018-02-09T05:00:39.058Z Reads: 138

```
I highly doubt that thing is 10000mah, also look at this review
![image|690x226](upload://96XTCIP4xEEEa0Fg1NYbaiVfdiO.png)
```

---
## \#5 Posted by: scepterr Posted at: 2018-02-09T05:17:54.475Z Reads: 125

```
I'm certain that's not a high discharge cell and its not that small to begin with, they're what's in the cheapo power banks
Dimensions: 8.8 x 70 x 129 mm

http://m.globalsources.com/gsol/I/Lithium-polymer/p/sm/1148315774.htm
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-02-09T06:23:29.840Z Reads: 114

```
37wh for $7 hum.. :thinking: 370wh for $70? Even if it's low current rating, it still doesn't sound very legit considering it's lipo. Better spend your money on authentic cells like samsung 30q, it's not worth the risk. :mask:
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-02-09T06:33:37.958Z Reads: 112

```
The wires coming off of that lipo are already really thin and there isn't even something like a C-Rate or current capability given in the specs, so i wouldn't do an esk8 with that particular cell.

However on better Lipo cells it's definitely possible to do so. 
I used that technique in my first build. But it's really a pain in the ass, the lipos i had didn't have a pcb to which the cells were soldered but instead they were spot welded together. Once i seperated them (shorting them a billion times in the process) i used aluminium based solder to tin the tabs with an even coat, then regular solder with flux to attach the wires. Worked out kind of well in the end although i would do a MUCH better job insulating and protecting everything the next time around.

 Well tbh next time i will just go with 18650 cells since i don't have old big lipos laying around anymore and spot welding seems kind of fun compared to this.


![image|281x500](upload://2i8TEpIPcAYtuhnlui71dzi6smE.jpg)
![image|374x500](upload://qh5EXdSnCuHd85WB0xgASzB4biZ.jpg)
```

---
## \#8 Posted by: Namasaki Posted at: 2018-02-10T04:27:54.559Z Reads: 68

```
I agree with @scepterr on this one. Those look like power bank cells capable of only 1-2 amp discharge.
The output wires are a dead give away.
```

---
## \#9 Posted by: bartroosen12 Posted at: 2018-02-10T11:38:25.353Z Reads: 51

```
If you wanna build a slim battery pack, use cells with higher discharge rate these won't give you 'power'.
I really like building a slim pack and used hobbyking 5Ah 20C cells: https://hobbyking.com/en_us/turnigy-5000mah-1s-20c-lipoly-single-cell.html?___store=en_us
I have a 10S1P and a 6S2P with these cells and works great.
```

---
