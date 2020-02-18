# BMS Wiring Check for Parallel Lipos

### Replies: 4 Views: 186

## \#1 Posted by: Vykku Posted at: 2019-04-03T09:37:45.448Z Reads: 43

```
I am planning to use 4x 5S 8Ah Lipos for a total of 10S 16Ah and I think using common port BMS would be most suitable. However I wanted to double check the wiring with others who have more experience and knowledge. TI am planning to use them in the following way:

![screenshot%201|585x500](upload://kGuzYDK7NiRK0qUC7jqb9y65Iqx.png) 

Here there would be pretty much two separate 10S batteries connected together, and balanced separately. I was thinking that if a cell from a lipo gets damaged, it would not affect the rest so I could just replace that Lipo.

I was also thinking that it might be overkill, and I could just use a single BMS, and every single cell wired in parallel as follows: 

![screenshot%201|597x500](upload://11O5N2kYZfipNXxwuuI6zBuz61f.png) 

I haven't drawn the balance cables too detailed since I am confident with their wiring, and hopefully these images can get the point across.

What do you think would be the best way to wire them?
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-04-03T10:16:33.500Z Reads: 38

```
I've got mine wired as option b. the easiest way to wire them is to make parallel balance lead adapters for each group of 2, then wack em together as shown in the diagram.

i run a 10s2p nano tech config and it was a pain but turned out v nice

![20181209_225026|666x500](upload://l7Ud9OnZ1Uu8gKn7enc2B62FiH7.jpeg) ![20181209_215236|375x500](upload://fJMxbEg2lgCvlzYMADOFBGDpqUE.jpeg)
```

---
## \#3 Posted by: Vykku Posted at: 2019-04-03T13:56:22.123Z Reads: 32

```
Cheers, I guess I will go with a single BMS then.

By the way, what kind of plastic did you use for your enclosure? And did you cover it in fiberglass or just in epoxy?

I looked at your build log and couldn't find that out. I was thinking to maybe 3D print a very thin enclosure, even out of PLA and then skin it with a few layers of fibreglass  on the outside for rigidity.
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-04-03T14:45:56.308Z Reads: 24

```
yeah so basically i 3d printed the enclosure in parts, epoxied the pieces together, then bolted the enclosure on, then fibreglassed the rest to make it flush on the deck. then sanded and applied dyed epoxy, then sanded, then spray painted with multiple coats etc
```

---
