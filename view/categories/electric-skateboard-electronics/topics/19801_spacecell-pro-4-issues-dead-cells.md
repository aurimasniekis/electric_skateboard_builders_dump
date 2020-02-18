# Spacecell Pro 4 Issues - Dead Cells?

### Replies: 12 Views: 755

## \#1 Posted by: Zach Posted at: 2017-03-28T03:18:20.515Z Reads: 101

```
Hi Guys, I am after some help. 
I only have approx 5x charge cycles on my Enertion Spacecell Pro 4 due to it being Winter and not riding at the moment. It has now stopped charging fully. It stops at 37V instead of 42V, which shows 51% on the meter as expected. I do not believe the BMS to be the issue.

I tested the voltage at each of the balance points on the pack. I have attached a photo showing the voltage at each point. The voltage remains the same after the 5th and 6th parallel batches.

Measuring across the the 5th batch yields 0V. 

I'm guessing this means one or more cells in the 5th parallel batch are bad? Or am I not understanding how it's set up?

I'm hoping to get some guidance as I contacted Enertion months ago and their suggestion was 'read the forums'...

Thanks heaps, Zach.

<img src="/uploads/db1493/original/3X/a/9/a9badb9c7bc614534a207307e76f3eb2b16bf4da.jpg" width="666" height="500">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-28T03:55:35.823Z Reads: 90

```
If you are out of warranty then you will Likely need to get the battery pack out of the enclosure and disconnected from the bms and test the battery groups individually. And look for broken connections between the battery groups.
```

---
## \#3 Posted by: Pantologist Posted at: 2017-03-28T04:10:35.160Z Reads: 91

```
Either 4, 5 or 6 has a dead cell or damaged nickel strip connection. This is why I hate big hot glued together battery packs... You can't tell what is going wrong and there usually is something going wrong because they have no other structure except hot glue. This battery design scores like an F on a safety test...
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-28T04:20:24.759Z Reads: 86

```
Is that what the white goop on the edges of the pack is, hot glue?
If so, it looks like the whole pack is glued to the enclosure.
```

---
## \#5 Posted by: Pantologist Posted at: 2017-03-28T04:25:42.035Z Reads: 86

```
The white goop looks more like a silicon type, but still. The enclosure is flexible and any bump or flex that alerts the shape of the enclosure, affects the batteries which are only supported by that very glue.
```

---
## \#6 Posted by: Zach Posted at: 2017-03-28T04:32:37.930Z Reads: 82

```
Thanks for the replies, they confirm my suspicion. It's still in warrantee, I have emailed them multiple times asking for advice in case it was something simple, but like usual don't get a reply.  
The white glue is some some of silicone/urethane. Since I'm in Canada and will have to pay for shipping to return it to America I'm tossing up whether it will be cheaper to fix myself. Pretty disappointing for it to go bad so quickly.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-03-28T05:22:47.927Z Reads: 75

```
Truly sorry for your misfortune. 
It may be your best option to fix it yourself.
If the silicone is soft, you should be able to cut it with a razor to get the pack out and then peel it off
```

---
## \#8 Posted by: onloop Posted at: 2017-03-28T06:17:39.144Z Reads: 73

```
What deck you have? is it super stiff or has some flex? Normally this problem is related to some flexing breaking the welds.

@JohnnyMeduse might be able to help, he's getting well know for his vesc repairs & is your country. Maybe he is looking to expand to pack welding?

If the fault is a manufacturing problem ill cover the cost of the repair fee.
```

---
## \#9 Posted by: PXSS Posted at: 2017-03-28T19:11:47.775Z Reads: 52

```
You have a short across group 5. If it's still in warranty replace it. If the issue was a broken connection then you would get an open loop between terminals, not a missing block. You have a dead cell within 5 which killed the entire group
```

---
## \#10 Posted by: Zach Posted at: 2017-03-29T00:29:02.339Z Reads: 43

```
Bingo, that's spot on PXSS. Measuring across each cell in group 5 and the are all 0V. Is there any reason this would have happened or just bad luck?
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2017-03-29T02:22:32.556Z Reads: 40

```
don't know if you seen it in your pm, but as @onloop propose it I'm will be more than happy to help you with your space cell .
```

---
## \#12 Posted by: PXSS Posted at: 2017-03-29T04:11:56.753Z Reads: 32

```
Get it replaced. You need to have the whole group 5 swapped for new cells which by itself is not an easy task since I hear that the cells are hot glued together. Plus now you're mixing new and used cells. Your BMS will have a hard time balancing the pack from now on and will fail prematurely again if not monitored extremely closely.
```

---
