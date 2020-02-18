# Space Cell BMS schematics?

### Replies: 21 Views: 3895

## \#1 Posted by: michaelcpg Posted at: 2016-04-04T00:57:12.737Z Reads: 197

```
Hey everyone, 
I've just received my space cell from Jason, only thing is we ended up having to get it sent in parts due to shipping regulations in NZ so I've gotta build the thing myself. Looks fairly straightforward for the most part, mainly just not sure about wiring to the BMS and battery.

Does anyone have schematics for the BMS (or even a link to more information about it?) or photos of their own space cell that they've pulled apart where you can clearly see the wiring configuration for the BMS and cells?
Here's a few photos for reference.

Cheers!

<img src="/uploads/db1493/original/2X/c/c187526754141820d1ac64b2e9384e23a9ba5b8b.jpg" width="690" height="390"><img src="/uploads/db1493/original/2X/4/417e2d4acdcd6d075f22e14d0b77c7ac396e31e9.jpg" width="282" height="500"><img src="/uploads/db1493/original/2X/a/a41fbc0ba9be6d42941206bebdc7a23c795d1726.jpg" width="282" height="500">
```

---
## \#2 Posted by: delta_19 Posted at: 2016-04-04T01:11:10.981Z Reads: 190

```
it should be battery + to xt60, battery- to b- on bms, p- on bms to xt60.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-04-04T01:53:27.477Z Reads: 192

```
Thanks, are you able to confirm if the cells themselves require any more connections between them? I'm struggling to follow how the 10s3p configuration works based on the current connections between the cells...

<img src="/uploads/db1493/original/2X/b/bc47b05d47dd2d654128ead9b463f26c60a6b26c.jpg" width="689" height="390"><img src="/uploads/db1493/original/2X/c/cacb6a91c72530482fdf5cc88fef8143e252c263.jpg" width="689" height="390">
```

---
## \#4 Posted by: cmatson Posted at: 2016-04-04T01:59:46.036Z Reads: 188

```
check out my thread here: it should be helpful, but I'm happy to provide any additional info if you so desire! 
http://www.electric-skateboard.builders/t/space-cell-opened-up/510/3
```

---
## \#5 Posted by: delta_19 Posted at: 2016-04-04T02:09:03.222Z Reads: 183

```
looks like it, just solder her up

forgot to mention that pin 10 of your balance lead should be soldered to the same place as you positive lead on the battery and then 9 to the strip in-between group 1 and 2
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-04-04T02:12:05.449Z Reads: 178

```
Any possibility of you giving a basic description on how they should be connected exactly? First time doing this sort of thing so want to make sure I get it right :p I'm struggling to understand why they're connected in groups of 6, shouldn't it be groups of 3?
```

---
## \#7 Posted by: cmatson Posted at: 2016-04-04T02:14:14.295Z Reads: 170

```

Actually there should be spot welding all the way down both halves of the battery.. 

So I don't think you are ready to go with just wiring up the BMS. Unfortunately I don't have my disassembled Space Cell anymore, but maybe @onloop or someone else who does have a broken down Space Cell can chime in here on which cells need to be connected.
```

---
## \#8 Posted by: delta_19 Posted at: 2016-04-04T02:17:41.915Z Reads: 158

```
they are in groups of 3, how it works are three are connected at there negative to the other threes positive. 

also cm do you see that little tab in the top pic? that looks to be what connects the groups of 2 together.
```

---
## \#9 Posted by: michaelcpg Posted at: 2016-04-04T02:31:24.605Z Reads: 153

```
Any idea why 4 of the groups would currently be connected in groups of 6 cells on one side? Does this mean I need to cut the connections to split them all up into groups of 3 or am I missing something here? Also a bit confused as to why one row has 8 BMS connection tabs (indicated by the bits of tape) whereas the other only has 3
```

---
## \#10 Posted by: Blasto Posted at: 2016-04-04T03:02:51.183Z Reads: 157

```
The bms needs 11 connections, 3+8, for sensing each cell. The six cells connection is 2 packs of 3 cells in series, where i believe there's something missing, is your connections from the top cells to the bottom where all your cells are unconnected. Then again, i can be wrong, i don't or seen a space cell.

Like the 4th pic in my build before the battery is unfolded. Note that my pack is a 10S4P, not a 10S3P. So i have connections of eigth cells instead of six.

http://www.electric-skateboard.builders/t/the-troll-enertion-cf-deck-dual-tbs-6355-sensor-10s-ongoing-build-log/1491
```

---
## \#11 Posted by: michaelcpg Posted at: 2016-04-04T03:34:08.624Z Reads: 161

```
Thanks for all the input guys, I'm starting to understand how this all works. 
The main thing I'm confused about at the moment is the placing of the stickers/connections for the balancing leads, eg. The group of 2s3p cells on the left has a connection for a balance lead on one parallel set but none for the other, as opposed to the other group which has two balance lead connections on one parallel set and one connection on the other parallel set. The same can be said about the two groups of 1s3p cells I have, one has 2 balance lead connections while the other only has one. Is someone able to explain the reasoning behind this? I would have thought that there would be one balance lead per set of 3 parallel cells? 

Also, if my assumption about one balance lead per 3p parallel set is correct, does it then matter in which order each parallel set is connected to the BMS or do I specifically need to connect the numbers on the cells to the corresponding number on the BMS?

<img src="/uploads/db1493/original/2X/a/a9dc916013136afb975656881f1b420626592ded.jpg" width="689" height="390">
```

---
## \#12 Posted by: Blasto Posted at: 2016-04-04T03:54:46.142Z Reads: 155

```
best i can do at the moment... hope it helps, the numbers are the balance leads

<img src="/uploads/db1493/original/2X/1/145013fe1b0ef647a505a9a98b1ccb422d95d039.png" width="690" height="350">
```

---
## \#13 Posted by: michaelcpg Posted at: 2016-04-04T04:11:23.278Z Reads: 151

```
Wow thanks man, makes much more sense now. Really appreciate this!
```

---
## \#14 Posted by: delta_19 Posted at: 2016-04-04T04:32:33.280Z Reads: 150

```
Looking at the bms I don't think you hook a positive lead to it. I think it's just like the ones sold by battery support where only the negative is connected.
```

---
## \#15 Posted by: Blasto Posted at: 2016-04-04T04:44:41.167Z Reads: 148

```
Right that's possible, my fancy paint drawing should read "POS to load" and "NEG to load". Because the connections to the bms can vary from bms to another bms
```

---
## \#16 Posted by: michaelcpg Posted at: 2016-04-04T04:51:16.363Z Reads: 145

```
Sorry would you guys mind confirming that last part? My BMS has 11 wires for connecting to the battery (10 white, 1 black) and as you can see in the initial photo, the battery has 11 connection points for lead wires. So do the numbers from @Blasto's diagram correspond to the numbered wires on the BMS directly with the exception of wire 11 in the diagram which would connect to connection B0 on the BMS? ie. 1 - B1, 2 - B2 ...... 10 - B10 11 - B0?
```

---
## \#17 Posted by: Blasto Posted at: 2016-04-04T05:04:18.762Z Reads: 143

```
@delta_19 was refering to high current leads, on some bms's only one side of the battery pack is connected.

The diagram is just for educational purposes, i have no idea how the space cell's balace leads are connected, but the idea stays the same.
```

---
## \#18 Posted by: michaelcpg Posted at: 2016-04-07T02:43:50.598Z Reads: 126

```
Ah I see, thanks Blasto. 

Still hoping for someone to confirm the correct configuration for connecting the balance leads to the battery. Main thing is I'm not sure if the B0 lead on the BMS corresponds to the number 11 connection on the battery or the number 1 connection on the battery? If the second option is the case then I'd assume that every other balance lead from the BMS 'N' would connect to number 'N + 1' on the battery? Is anyone please able to confirm which case is true?

I've messaged @onloop but haven't heard back from him yet so thought I'd check to see if anyone else knew :)
```

---
## \#19 Posted by: michaelcpg Posted at: 2016-04-07T12:12:39.046Z Reads: 120

```
Hey @delta_19 would you mind elaborating on this a little? The BMS seems to have 2 P- terminals (Well a 'P-' and a 'P-1'), which of these do I connect the xt60 to? I've been looking at @cmatson's thread of his opened space cell for a while which has been helpful to some extent but his version of the space cell uses a different BMS with different connections. At this stage I'm also not exactly sure where the LCD, power switch and charging port are connected in the circuit. Any information on this would be greatly appreciated too :) 

On the upside, I've made some progress with the rest of the battery. The cells are all soldered together and the balance leads connected :) 
<img src="/uploads/db1493/original/2X/5/57c73abc783b10afa0d4d090dd577cc66f8ed0bf.jpg" width="689" height="390">
```

---
## \#20 Posted by: delta_19 Posted at: 2016-04-07T12:22:24.509Z Reads: 116

```
Not to sure  i have just been going by what i know about bms's, you could ask @onloop it is his bms
```

---
## \#21 Posted by: michaelcpg Posted at: 2016-04-07T12:38:55.438Z Reads: 116

```
No worries, thanks anyway. I'm waiting to hear back from onloop atm
```

---
