# FPGA based BLDC motor controller

### Replies: 15 Views: 1164

## \#1 Posted by: norbertbonnici Posted at: 2017-06-16T17:56:09.201Z Reads: 151

```
I am in the process of developing a BLDC motor controller based on an FPGA design. Would anyone be interested in a modular HV motor controller. It will incorporate up to four swappable motor connections and some wireless chip to interface with a remote directly. Would anyone be interested in such an implementation?
```

---
## \#2 Posted by: Maxid Posted at: 2017-06-16T22:00:34.541Z Reads: 144

```
Sounds interesting. Can you educate us about what this will do better than say a VESC? Personally I don't have any experience with fpgas but heard that they can do amazing things.
```

---
## \#3 Posted by: norbertbonnici Posted at: 2017-06-16T22:28:49.752Z Reads: 135

```
It’s more of a personal interest... as far as I know it’s will be much easier to scale say from 1 to 2 to 4 motors running off the same chip, and having the ability to integrate other functionality in the same chip. Performance wise, I haven’t seen a VESC yet so I don’t know if it can outperform it, might be slightly faster and consumes less power (but in the grand scheme of this this might not be as big of an advantage). I guess I will find out once I get to build it...
```

---
## \#4 Posted by: mmaner Posted at: 2017-06-17T00:23:06.851Z Reads: 121

```
If you can control 4 motors from a single ESC and keep the cost comparable to the VESC you'll make a million bucks 😀
```

---
## \#5 Posted by: wmj259 Posted at: 2017-06-17T01:06:05.253Z Reads: 110

```
This will be something to definitely keep my eye on.
```

---
## \#6 Posted by: Blasto Posted at: 2017-06-17T01:17:51.847Z Reads: 109

```
What type of fpga are you thinking of?
```

---
## \#7 Posted by: norbertbonnici Posted at: 2017-06-17T07:03:26.976Z Reads: 106

```
I’m not doing this for the money but if people are interested I can try to find a way how to share it with the community. The cost might be the same or a bit more for the test board but if you buy components by the bulk it gets cheaper. I’ll try to get an estimate of costs today.
```

---
## \#8 Posted by: norbertbonnici Posted at: 2017-06-17T07:05:12.356Z Reads: 105

```
At the moment I have a few Spartan 6 LX9 lying around so I’ll use them for the initial prototype. If board size will Ben an issue (or 144 pins are too much) I’ll consider migrating to a Max 10 or an igloo
```

---
## \#9 Posted by: Blasto Posted at: 2017-06-17T14:40:45.881Z Reads: 97

```
[quote="norbertbonnici, post:8, topic:25516"]
Spartan 6
[/quote]

way overkill, nice!
```

---
## \#10 Posted by: Namasaki Posted at: 2017-06-18T04:59:28.712Z Reads: 83

```
Can hardly wait to see it!!!!
```

---
## \#11 Posted by: yosoufe Posted at: 2017-06-22T19:16:36.585Z Reads: 66

```
Is it possible to use that IP in Zynq series?? then you can have both complicated calculation and software on the ARM side along a parallel motor controller.

I do not know anything about FPGAs but i am really eager to learn.
```

---
## \#12 Posted by: norbertbonnici Posted at: 2017-06-23T07:37:59.553Z Reads: 56

```
Yes it should be compatible with a Zynq, but as a heads up there is no quad flatpack package for a Zynq and their prices are quite high if you buy just a single chip. You don't need a hard processor in your design as you can synthesis a soft processor such as the microblaze.
```

---
## \#13 Posted by: Martinsp Posted at: 2017-06-23T07:42:33.903Z Reads: 55

```
This sounds super interesting... I am definitely interested in this! Keep us updated please :)
```

---
## \#14 Posted by: boonem1992 Posted at: 2017-12-26T18:38:08.444Z Reads: 34

```
I’m interested in this.
```

---
## \#15 Posted by: boonem1992 Posted at: 2017-12-26T18:41:46.067Z Reads: 33

```
Do you have any recommended reading material on this topic (books, etc...)?
```

---
