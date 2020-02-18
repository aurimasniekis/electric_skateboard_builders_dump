# Best way to connect 4 Lipo Batteries together?

### Replies: 11 Views: 228

## \#1 Posted by: Rudybpyt Posted at: 2019-08-28T10:41:41.238Z Reads: 49

```
Hi all, 

I am making a budget build so I am using Lipo batteries, I have my eyes on these 4500mAh 3s 40c Lipo Packs that give a voltage of 11.1V, I plan to buy 4 of them to get 44.4 volts and to use my VESC to set a voltage limit of 36V, Would using 3x Y connectors to connect the packs be suitable or just dangerous?
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-08-28T14:13:58.075Z Reads: 44

```
you need 4 series connectors. also, your vesc will not limit voltage. it can only take what it's given by the battery. in your case, 50.2v full, 44.4v nominal and 38.4v empty. you can set voltage limits on the esc, but if it's below the battery voltage it simply won't work
```

---
## \#3 Posted by: Rudybpyt Posted at: 2019-08-28T14:17:42.471Z Reads: 42

```
is there a 4 series connector out there?

What do you mean if its below the battery voltage?
The motors i have are 600w and the site says they take between 24 to 36 volts, I was planning to set the max voltage to 36 on the VESC, and look at tutorials for setting up the rest.
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-08-28T14:20:44.268Z Reads: 43

```
buddy please. you have 2 hrs read time. this isn't enough for what you're doing. 44v dc is very dangerous. you will hurt yourself if you don't know what you're doing

to answer your question, no. you need 4 separate series adapters for your 4 batteries. 

If you set the esc voltage limit to lower than what the battery is, it won't work. the voltage isn't what's going out of the vesc, it's what's going in.
```

---
## \#5 Posted by: Rudybpyt Posted at: 2019-08-28T14:42:51.498Z Reads: 39

```
Ok I understand your point, I will read up more 

![diagram|353x500,50%](upload://pXSvD0aiV2u41Bbdw27cs4Uuu7I.png)

 where would the 4th adaptor go?

Ok, so I need to get a battery or a set up that is under or exactly 36V?
```

---
## \#6 Posted by: footloops Posted at: 2019-08-28T20:09:09.796Z Reads: 33

```
![Untitled|450x500](upload://to5DodljcLvutNrpgmqXoSMydJ4.png) 

Here is an example of a series harness for 4 lipos in series. The diagram you drew made no sense as the battery pack as two negative terminals instead of a positive and a negative
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-08-28T21:15:12.886Z Reads: 29

```
you cannot get a battery that is "exactly under 36v". that's not how batterys work. if you don't know this please don't build a battery
```

---
## \#8 Posted by: thisguyhere Posted at: 2019-08-28T21:54:02.787Z Reads: 28

```
that's a bit rough, everyone has to start somewhere.

this is a good place to start.

https://www.electric-skateboard.builders/t/wiki-a-beginner-guide-to-diy-an-esk8/46844

then watch videos, read some more.

then go build!
```

---
## \#9 Posted by: mynamesmatt Posted at: 2019-08-28T23:32:52.404Z Reads: 23

```
i dont think im being rough. he needs to know the very basics of electronics before he hurts himself
```

---
## \#11 Posted by: Rudybpyt Posted at: 2019-08-29T06:35:42.833Z Reads: 18

```
Who says Im building a battery? I was gonna simply connect packs together but now im using different ones that sit in the middle of the voltage range
```

---
## \#12 Posted by: Rudybpyt Posted at: 2019-08-29T06:36:21.009Z Reads: 18

```
Thanks Ill check them out
```

---
