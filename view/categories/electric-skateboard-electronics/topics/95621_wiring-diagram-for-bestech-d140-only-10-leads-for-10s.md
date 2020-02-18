# Wiring diagram for bestech d140 - only 10 leads for 10s?

### Replies: 12 Views: 432

## \#1 Posted by: craj1031tx Posted at: 2019-06-01T21:22:23.433Z Reads: 89

```
![Screenshot_20190527-183833_Chrome|243x500](upload://gbZX9osohpsPTvYbCcRXR9ODz8m.jpeg)

There are only ten leads on the schematic where as every other bms I have seen, even charge only, have your s number + 1 (so my 10s would have 11 leads.) 

Why is this controller different? Want to make sure the diagram isn't mistaken before I take apart my current config. Additionally I saw a pic in a sale thread for a d140 in 12s and it appeared to have 13 pins from the pic so I am a bit confused.

Thanks!
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-06-01T21:30:36.578Z Reads: 80

```
[quote="craj1031tx, post:1, topic:95621"]
12s and it appeared to have 13 pins from the pic so I am a bit confused.
[/quote]

if you get 12s you will get 13 pins, it just shows as 17 pins cause its the stock photo.

also the wiring diagram shows 11 pins... it just does not count the first one lol, also there are many bms's with 10 pins for 10s
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-06-01T21:34:50.290Z Reads: 81

```
i will upload pics, the actual first pin goes to B -, i beleive

![7e7fd5e8d61521e78f043d09aa6f8957|548x499](upload://dOKU9COZOliR7tctcKfptOTIFaL.png)
```

---
## \#4 Posted by: craj1031tx Posted at: 2019-06-01T21:47:49.350Z Reads: 81

```
I feel lik I'm going crazy here. The bms I have o ly has ten pins total, one 8 pin jst and one 2 pin jst. The large male jst on the board only has eight pins while the one in the picture has nine. As you can see the package says it is a 10s system. @thisguyhere can you assist? I bought this bms from your store 😃
```

---
## \#5 Posted by: craj1031tx Posted at: 2019-06-01T21:49:25.621Z Reads: 81

```
![20190601_164615|374x500](upload://raHfxV9FidYT5v8scyYvPO7jRxf.jpeg)
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-06-01T21:51:00.034Z Reads: 78

```
dont worry about it some D140's have the extra pin and some dont, they are 50+ versions of the d140
```

---
## \#7 Posted by: craj1031tx Posted at: 2019-06-01T21:54:50.659Z Reads: 78

```
Ok great, thank you, so essentially the negative end of the battery doesn't connect to the jst plug at all, it just goes directly to the bms b- solder pad?
```

---
## \#8 Posted by: thisguyhere Posted at: 2019-06-02T16:06:34.753Z Reads: 58

```
Correct, no pack negative balance lead, on the pcb u can see it's not connected to anything. 

Lemme know if u need more help
```

---
## \#9 Posted by: longboardshort Posted at: 2020-01-01T17:24:46.031Z Reads: 15

```
Dumb question - for having a power switch with the d140, just run either the b+ or b- through an xt90s antispark or if I want an actual led power switch then buy an anti spark pcb, correct?

It’s going to be for a build w a unity but I don’t trust the antispark built in that.
```

---
## \#10 Posted by: longboardshort Posted at: 2020-01-02T15:07:25.291Z Reads: 12

```
Bump

10char
```

---
## \#11 Posted by: thisguyhere Posted at: 2020-01-02T16:49:02.145Z Reads: 12

```
i think i understand what you're saying.

yea, put your loopkey (xt90s) along the battery + or -.

if using an antispark swtich, just connect it to battery + and -.

if your d140 has a switch (two wires), just have them connected so it's powered on all the time.  bms switch is irrelevant here since it's discharge byassed.

i have a loop key in all my boards even though the unity has a switch built in.
```

---
## \#12 Posted by: longboardshort Posted at: 2020-01-02T17:16:24.082Z Reads: 9

```
Thanks much !
```

---
