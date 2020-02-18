# Adding a 10s1p to an existing 10s1p&hellip; possible? how to charge?

### Replies: 18 Views: 475

## \#1 Posted by: SecrIT Posted at: 2018-10-12T03:04:25.766Z Reads: 127

```
I have a board that has a 10s1p LG setup.  I am wanting to add a 10s1p battery pack in Parallel to basically create a (10s2p 4.4Ah setup).

(Note both batteries have separate BMS connection.)

My question is:

If I put these batteries in parallel will I be able to charge them as a single unit?  Or do i have to disconnect the series connection and charge them individually?

....Think of a meepo board that has a 10s1p.... then purchasing another 10s1p battery setup from them in enclosure.  How do i connect them together, and how do i make it so i can charge them together?

Thanks all
```

---
## \#2 Posted by: thisguyhere Posted at: 2018-10-12T03:15:46.164Z Reads: 117

```
series would make it a 20s1p

itd be parallel to make two 10s1p into 10s2p

It can be done, make sure voltages are close, like within .2v and connect them in parallel.

but charging them together, you could just charge it connected like that but only the one pack connected to bms will be balanced.
```

---
## \#3 Posted by: SecrIT Posted at: 2018-10-12T04:13:11.873Z Reads: 107

```
Youre right, i updated post to say parallel.

They are lithium-ion could i somehow charge them all together ?

Sorry i dont understand the battery stuff
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-12T06:32:59.520Z Reads: 92

```
you can charge them without bms (without to say i recommend it)
but this way it would work if the packs have close the same voltage like @thisguyhere already said.
```

---
## \#5 Posted by: thisguyhere Posted at: 2018-10-12T06:35:15.784Z Reads: 93

```
yea the battery part is the most confusing when starting, no worries.

so...you've got two 10s1p pack, each has its own bms, right?

if that's the case, you could wire it in a way that a single charge port could charge both packs at the same time.

going to sleep now but i could diagram it for you.  remind me tomorrow.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-10-12T11:37:04.829Z Reads: 63

```
I think he could just get a parallel connector and plug the batteries together. That is assuming each pack has a bms of it’s own.
```

---
## \#7 Posted by: SecrIT Posted at: 2018-10-12T14:40:34.114Z Reads: 52

```
If each pack has it's own BMS and I charge with a Laptop (42v - 2Amp) charger, if they are connected in parallel If i just plug into the charge port of one setup, i assume the other will not charge properly as the BMS is connected to it's own charge port?  Or once in parallel it will charge properly?  thx
```

---
## \#8 Posted by: pat.speed Posted at: 2018-10-12T19:33:54.339Z Reads: 45

```
If they are both connected in parallel exactly how the board originally was it will charge fine
```

---
## \#9 Posted by: SecrIT Posted at: 2018-10-12T19:54:17.033Z Reads: 42

```
Sorry if I wasnt clear, still trying to wrap my brain around things.  The board originally only has a single (10s1p) with charge port.  I would add a secondary 10s in parallel giving me 10s2p.  Once the second battery pack is in parallel, could i charge both through the original charge port, or would i need to charge them separately?  thx
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-10-12T20:07:48.604Z Reads: 39

```
does your second pack already have the charge port installed?

why don't u take a photo of the second pack
```

---
## \#11 Posted by: b264 Posted at: 2018-10-12T20:13:33.586Z Reads: 39

```
I second the request for photos, but you should be able to connect the charge port wires and battery output wires in parallel.  HOWEVER, you MUST make sure both packs are at the exact same (within 0.1V, or within 0.05V if in the 35-39 range) voltage when you connect them together.  This is important.  Easiest way is to charge both of them until green light with the same charger, one after the other.  Another way is to connect the positives together first, then put an old-style incandescent automotive light bulb between the negative (B-) connections until the voltages are the same.
```

---
## \#12 Posted by: thisguyhere Posted at: 2018-10-12T20:15:14.145Z Reads: 39

```
kind sucks in one color, kind of hard to follow connections, just look at it closely

![1012181312_HDR|684x500](upload://a8tc7V9etseQkAKaBIO8Utbk4k3.jpeg)
```

---
## \#13 Posted by: b264 Posted at: 2018-10-12T20:16:09.408Z Reads: 34

```
[quote="b264, post:11, topic:70944"]
HOWEVER, you MUST make sure both packs are at the exact same ... voltage when you connect them together.
[/quote]

failure to heed could result in fire
```

---
## \#14 Posted by: thisguyhere Posted at: 2018-10-12T20:17:29.853Z Reads: 31

```
one hundred percent.

i once connected a lipo and liion pack i use in parallel for spot welding with a .5v difference and the lipo got really hot, really fast.

don't do it.
```

---
## \#15 Posted by: pat.speed Posted at: 2018-10-12T20:19:49.607Z Reads: 29

```
You can keep everything how it is. All you need to do is attach the batteries together in parallel
```

---
## \#16 Posted by: SecrIT Posted at: 2018-10-12T20:26:09.968Z Reads: 32

```
Sorry, I have no picks for everyone.... .but interesting.  I could tie the charge port wires together, and then just charge with my 42v/2amp charger.  That seems like it could work.

I also totally understand making sure both are same voltage before putting in parallel.
```

---
## \#17 Posted by: pat.speed Posted at: 2018-10-12T20:38:55.790Z Reads: 30

```
It will, it will just take longer. Many people do this. Even if you search for ebike batteries and power walls they do it. I was watching a video just yesterday of a guy that connected the same batteries as meepo use together in parallel to make a mini power wall to power an inverter. It’s the same concept
```

---
## \#18 Posted by: SecrIT Posted at: 2018-10-12T21:31:54.925Z Reads: 24

```
Thanks All !
```

---
