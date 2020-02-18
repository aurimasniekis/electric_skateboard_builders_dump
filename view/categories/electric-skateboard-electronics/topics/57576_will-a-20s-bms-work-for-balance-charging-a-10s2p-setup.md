# Will a 20S BMS work for balance charging a 10s2p setup?

### Replies: 20 Views: 636

## \#1 Posted by: BrokenGloves Posted at: 2018-06-02T18:28:14.168Z Reads: 125

```
I can't find anything more than a 10S thread on here, just wanna know if anyone has done this or if it will work? will i need 2 10S BMS's or a balance charger? thanks in advance
```

---
## \#2 Posted by: b264 Posted at: 2018-06-02T19:14:18.920Z Reads: 122

```
If you're asking about a 20S charger with a 10S battery: no, it won't work because it's not 42 Volts.  Don't do it.

If you're asking about a 20S BMS with a 10S battery, maybe but it depends.

What exactly is the question?
```

---
## \#3 Posted by: pixelsilva Posted at: 2018-06-02T19:21:48.639Z Reads: 113

```
https://media.giphy.com/media/glmRyiSI3v5E4/giphy.gif
```

---
## \#4 Posted by: BrokenGloves Posted at: 2018-06-02T19:28:45.866Z Reads: 103

```
sorry i muddled my words it's just for balance charging a 10s2p. would a 20s bms work?
```

---
## \#5 Posted by: rojitor Posted at: 2018-06-02T19:34:03.690Z Reads: 99

```
Smart bms allow to do It. Can also be done if you know how to modify It. Do not mess with that unless you know exactly what you are doing.
Selling It and buying a 10s is the best option. You can even earn some cash.
```

---
## \#6 Posted by: BoostedBuilder Posted at: 2018-06-02T19:34:20.459Z Reads: 93

```
Yes, but it's most likely 2x the size of a 10s BMS. What's the point?

Rojitor beat me to it : )
```

---
## \#7 Posted by: b264 Posted at: 2018-06-02T19:47:14.224Z Reads: 90

```
[quote="BrokenGloves, post:4, topic:57576"]
it’s ... for balance charging a 10s2p. would a 20s bms work?
[/quote]

Most of the time, yes.  **IF** you wire it correctly.  I'm sure there are some BMS that won't, it would depend a lot on the specific BMS

Start from the negative side and leave the extra on the positive end
```

---
## \#8 Posted by: BrokenGloves Posted at: 2018-06-02T20:11:41.592Z Reads: 74

```
Any 20s Bms you'd recommend? i want to be able to charge all at once and its less wiring
```

---
## \#9 Posted by: BoostedBuilder Posted at: 2018-06-02T20:13:44.001Z Reads: 71

```
I have a Bestech 10s 35a BMS, you want it?
```

---
## \#10 Posted by: b264 Posted at: 2018-06-02T20:14:54.856Z Reads: 71

```
[quote="BrokenGloves, post:8, topic:57576, full:true"]
Any 20s Bms you’d recommend? i want to be able to charge all at once and its less wiring
[/quote]

You need a 10S BMS

I was under the impression you already had a 20S that you wanted to try to use.  If you don't have one yet, you need a 10S BMS

What battery are you using?  Do you have a photo?  What charger are you using?  Do you have a photo?  Do you have a BMS now?  Do you have a photo?  What cells are you using? Do you have a photo?

Using a 20S BMS on a 10S battery will just mean half of the BMS isn't being used and is wasted space/weight/money.  It won't charge faster or better.
```

---
## \#11 Posted by: BrokenGloves Posted at: 2018-06-02T23:04:27.578Z Reads: 54

```
yeah but if I'm wanting to charge 2 10S's at the same time in parallel could i do that with a 20S bms?
```

---
## \#12 Posted by: BoostedBuilder Posted at: 2018-06-02T23:17:58.432Z Reads: 53

```
No    ‍      ‍      ‍      ‍
```

---
## \#13 Posted by: b264 Posted at: 2018-06-03T00:38:53.759Z Reads: 49

```
[quote="BrokenGloves, post:11, topic:57576"]
if I’m wanting to charge 2 10S’s at the same time in parallel could i do that with a 20S bms?
[/quote]

No. That's precisely what a 10S BMS does.
```

---
## \#14 Posted by: BrokenGloves Posted at: 2018-06-03T21:52:07.118Z Reads: 35

```
so do i just double up the charging cables going into the bms? i don't understand how i can charge 20 cells all at once with a 10S BMS?
```

---
## \#15 Posted by: BoostedBuilder Posted at: 2018-06-03T21:58:57.912Z Reads: 33

```
You will be charging them in parallel. You have a 10s BMS for a 10s2p battery, so the 42V are equally divided through the series connection, and the current is divided by 2 for the 2x 10s packs.

Do you need a 10s BMS?
```

---
## \#16 Posted by: b264 Posted at: 2018-06-03T22:20:53.540Z Reads: 33

```
https://physics.bu.edu/py106/notes/Circuits.html
```

---
## \#17 Posted by: Trdolan03 Posted at: 2018-06-04T06:52:35.726Z Reads: 26

```
I have a similar question so I am high jacking the thread. I have 6 4s 5.2ah turnigy graphine batteries wired 3s 2p. Could someone help me figure out the wiring to that 1 BMS could balance all 6 batteries?
```

---
## \#18 Posted by: E1Allen Posted at: 2018-06-04T07:29:14.494Z Reads: 21

```
Sounds like your doing 12s2p.  You need a12s bms. Then search on the forum about how to wire it.  One BMS will charge all 6, but you have some reading to do.
```

---
## \#19 Posted by: rojitor Posted at: 2018-06-04T07:54:08.153Z Reads: 18

```
You only need one wire per parallel. 10s2p and 10s20p will work with the same bms. Watch some vídeos at YouTube about battery welding.
```

---
## \#20 Posted by: faithfulpuppy Posted at: 2018-06-04T12:48:32.459Z Reads: 13

```
the way this works is that you take your twenty cells and group them into the parallel groups they will be in (in you case, ten pairs of two cells). Because they have the same internal resistance, they should discharge at the same rate, and because they're in parallel they will maintain each other at the same voltage. You then connect the parallel groups in series to form 10s with 2p groups as each "cell" in the series. you can then treat each parallel group as one cell when connecting to the BMS because they are, electrically, one cell. 

having two batteries in parallel is electrically indistinguishable from having one large battery. After all, a larger battery is just the same as the small battery but with more chemicals inside it covering a larger surface area with their contact, if that makes sense (i know it doesn't really but trust me on this - they're the same)

i suggest you do more reading too, any battery build guide covers this info pretty well
```

---
