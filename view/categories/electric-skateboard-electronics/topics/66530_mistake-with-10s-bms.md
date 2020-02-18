# Mistake with 10s BMS?

### Replies: 7 Views: 318

## \#1 Posted by: never4getf150forums Posted at: 2018-08-30T06:28:05.688Z Reads: 106

```
I recently bought a bestech d140 to replace what my old d140 that blew, but they seem to differ a bit.

my older bms had a 8 prong connector, and this one had a 9 prong connector, but that didn't stop me from connecting it and running it with a loose prong stickin out.

Anyway, this is how I plugged it in, and my fear is now I have an unbalanced P pack because I did something wrong.

Tell me, is this correct, thanks!

![image|666x500](upload://p8u4I7eodeSDbHZdWRE2sT3mWmh.jpeg)![image|666x500](upload://efxWPi8fZNXcmk3qBHzhDrhJUuC.jpeg)![image|666x500](upload://m1kXJUv3wa6aGiWlfRbCvJbYQoa.jpeg)![image|374x500](upload://7wl0zXbXTG03aHiyvzucCzWvbUO.jpeg)


@JLabs any help would be appreciated
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-30T10:14:09.179Z Reads: 89

```
your balance b- not connected now
like this your bms can´t measure the voltage for each serial pack.

how the bms before was working? got the balance b- from the main - on the board?
probably, if not I guess you now would already have a short and broken bms.
```

---
## \#3 Posted by: Brdchris Posted at: 2018-08-30T10:32:33.941Z Reads: 84

```
This new batch of d140 bms has two b-. One on the board like our old ones, and one on the connector. I don’t have the answer but I’m following as I’m having the same problem. 

I was planning on using my multimeter to see if the two b- places are electrically common to each other, I.e. 0 ohms when checked across the two. If so, I assume it will be safe to only connect one
```

---
## \#4 Posted by: SilentException Posted at: 2018-08-30T10:45:34.748Z Reads: 82

```
On few of BMS here I see that there is a through-hole for balance B- connector and they sometimes come with full balance count connector (series count + 1) or sometimes they skip that pad because main B- is already connected. Balance and main B- are connected of course (you can see traces on PCB or check with multimeter if you'd like). You'll be fine.
```

---
## \#5 Posted by: JLabs Posted at: 2018-08-30T12:21:15.719Z Reads: 71

```
It’s not the same as other connectors. You will need to attach the B- wire. I would just install the new wires on the battery
```

---
## \#6 Posted by: Brdchris Posted at: 2018-08-31T00:11:52.032Z Reads: 41

```
![image|374x500](upload://evUBTAIUtaX72uq6I7jjrR4MqIU.jpeg)
```

---
## \#7 Posted by: Winfly Posted at: 2018-08-31T00:15:34.402Z Reads: 39

```
your old D140 probably has the b- internally wired up from the big B- for the battery lead. it's safest to wire a new b- lead from the battery to the b- balance lead.
```

---
