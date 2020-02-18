# What&rsquo;s the most reliable/cheap esc for belt drive systems?

### Replies: 17 Views: 442

## \#1 Posted by: samr Posted at: 2019-07-13T23:04:24.199Z Reads: 106

```
I just bought a used chinese board (paean H2B) for a really good price. I don't like the esc that it has in it (feels too binary and unresponsive). Honestly, I just don't feel safe on it. I also have a wowgo 2s which has a much better esc (hobbywing right?). From what I've read, this esc is pretty hard to get and is only for hub motors. Any suggestions on a cheap-ish esc that will work with a belt drive?

Motors: 2x 900w motors
Battery: Samsung 10c.2p 42v
```

---
## \#2 Posted by: xjujo Posted at: 2019-07-13T23:18:21.311Z Reads: 106

```
There was a recent sale for Flipsky Dual 4.20plus
```

---
## \#3 Posted by: samr Posted at: 2019-07-13T23:28:24.948Z Reads: 99

```
Do you have a link to it?
```

---
## \#4 Posted by: xjujo Posted at: 2019-07-13T23:43:19.093Z Reads: 95

```
https://flipsky.net/products/dual-fsesc4-12-100a
Or you can grab the plus version
```

---
## \#5 Posted by: samr Posted at: 2019-07-14T00:18:18.977Z Reads: 90

```
That's a tad out of my budget unfortunately. Would an esc designed for hub motors (like the wowgo one) work with this belt drive system?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-07-14T04:46:49.966Z Reads: 83

```
There is a belt version one it's actually called a, esc substitute, but remember buy cheap buy twice, the esc substitute's have a tendency for half of the esc to die
```

---
## \#7 Posted by: M.Hboards Posted at: 2019-07-14T04:50:59.090Z Reads: 82

```
Get 2 of these you won't be disappointed

https://m.aliexpress.com/item/32951134782.html?pid=808_0000_0101&spm=a2g0n.search-amp.list.32951134782&aff_trace_key=ba35e58400064c7f8261f7d67f9f05b7-1561386329563-00292-VnYZvQVf&aff_platform=msite&m_page_id=7693amp-anR8OfHEZuV5kpPCTMB48A1563079804651
```

---
## \#8 Posted by: samr Posted at: 2019-07-14T04:57:15.184Z Reads: 79

```
That looks like more of my price range. How would I hook up the remote with this setup? Is there a wiring diagram somewhere for doing two of these?

(nevermind, found it here: https://www.electric-skateboard.builders/t/what-is-the-correct-esc-amp-calculation/38078)Also how do I pick the right amp rating for the esc? I would assume that it depends on my battery and the motors but I'm not sure how to do the calculation :sweat_smile:
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-07-14T04:59:08.204Z Reads: 76

```
You'll have to get two of them.

And you can run them in CAN BUS, or SPLIT PPM

And you could get a mini remote for 15$ off of AliExpress

[quote="samr, post:8, topic:98407"]
Also how do I pick the right amp rating for the esc?
[/quote]

You don't, it's a VESC it's fully configurable
```

---
## \#10 Posted by: samr Posted at: 2019-07-14T05:18:31.162Z Reads: 68

```
[quote="AlanZhou, post:9, topic:98407, full:true"]
You'll have to get two of them.

And you can run them in CAN BUS, or SPLIT PPM

And you could get a mini remote for 15$ off of AliExpress

[quote="samr, post:8, topic:98407"]
Also how do I pick the right amp rating for the esc?
[/quote]

You don't, it's a VESC it's fully configurable
[/quote]


Right but it seems like they're rated for how many amps it can put out (in the hardware). ex: that aliexpress one is 50A. I looked around on the forum and read this: https://www.electric-skateboard.builders/t/what-is-the-correct-esc-amp-calculation/38078/3 but I'm still a bit confused. I understand that I can limit the power draw with a vesc but I want to make sure that I get the full performance from my board and not bottleneck it in the esc.

For the remote, can I use any 2.4 ghz remote? Would the one from the hobbywing esc (wowgo 2s) work?
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-07-14T13:08:48.965Z Reads: 45

```
[quote="samr, post:10, topic:98407"]
Would the one from the hobbywing esc (wowgo 2s) work?
[/quote]

No you need a remote that includes a receiver.
```

---
## \#12 Posted by: samr Posted at: 2019-07-15T00:19:48.622Z Reads: 29

```
Do I connect the two in series or parallel to the battery?
```

---
## \#13 Posted by: M.Hboards Posted at: 2019-07-15T00:31:05.615Z Reads: 29

```
Parallel

10char
```

---
## \#14 Posted by: samr Posted at: 2019-07-15T00:38:42.230Z Reads: 29

```
What about the fuse/switch? The board that I have just has a push button switch with 4 wires coming out (2 for led, 2 for button?). 

I also have a battery indicator light thing. Would that be able to plug into the the vesc to show remaining battery?
```

---
## \#15 Posted by: MysticalDork Posted at: 2019-07-15T00:46:00.291Z Reads: 27

```
Your best, cheapest and most reliable option is a loopkey. Basically an XT90-S connector on the positive wire between the battery and ESC, with the mating plug bridged with a wire. To turn stuff on, plug in the key (connector). To turn stuff off, unplug it. Rock simple.
```

---
## \#16 Posted by: M.Hboards Posted at: 2019-07-15T00:47:04.263Z Reads: 26

```
For that you would need to use a anti spark switch or Loop key and install the battery indicator after whichever one you choose.
```

---
## \#17 Posted by: MysticalDork Posted at: 2019-07-15T00:49:40.133Z Reads: 26

```
You obviously are trying to build this on a shoestring budget, so don't even bother with an electronic antispark. They're expensive and they break.

For an indicator, you can get either a digital voltmeter module that just tells you the voltage, or you can get an actual battery meter module that does the math and tells you a %. Either is available from Amazon, ebay, or many of the esk8 hardware sellers.
```

---
