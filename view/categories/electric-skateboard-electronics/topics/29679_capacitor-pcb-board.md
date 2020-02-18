# Capacitor PCB / Board

### Replies: 18 Views: 1211

## \#1 Posted by: banjaxxed Posted at: 2017-08-04T12:54:59.090Z Reads: 161

```
Hey I've got some spare 63v low ESR quality caps and I know I should wire them in parallel but I'd like to use a PCB to do this. I've seen @onloop post about the Enertion one that VESC-X / FOCBOX use and have a couple of VESC-x (pre-FOCBOX).

Is there any source of Vedder's design for this aside from Enertion?
I think that they will not be available to buy except as part of a FOCBOX 

http://www.electric-skateboard.builders/t/new-dual-vesc-capacitor-board/6549
```

---
## \#2 Posted by: banjaxxed Posted at: 2017-08-04T12:56:10.649Z Reads: 157

```
Vedder did make a design for this
https://github.com/vedderb/CapPCB

@chaka @goldenHusky @DeathCookies @esk8 @fottaz @Kaly @barajabali      do you have anything?
```

---
## \#3 Posted by: DougM Posted at: 2017-08-04T15:11:38.956Z Reads: 133

```
I have one shared out on OshPark

[ESK8 capacitor board](https://oshpark.com/projects/HPMHDtD6)
```

---
## \#4 Posted by: banjaxxed Posted at: 2017-08-04T15:15:56.517Z Reads: 124

```
Thanks, I'm in Ireland but hopefully shipping would not be a prob. Looking now at ordering a few
```

---
## \#5 Posted by: banjaxxed Posted at: 2017-08-04T15:19:14.510Z Reads: 121

```
Cool, resources coming out of the woodwork, axle also sell from their webstore, ding ding ding

https://goaxle.com/shop/cappcb
```

---
## \#6 Posted by: banjaxxed Posted at: 2017-08-04T15:25:11.347Z Reads: 109

```
Thanks @DougM I've placed an order  :)
```

---
## \#7 Posted by: banjaxxed Posted at: 2017-08-04T15:44:58.314Z Reads: 112

```
Wondering if possible to remove(snip?) or carefully break the PCB on either end to take off one of the three cap positions from the PCB without destroying it?

I bought these deluxe VESC cases and it would be a shame to not use them, to me only two caps will fit side-by-side in it

Dimensions 110x47x26

http://www.ebay.com/itm/142365493004
```

---
## \#8 Posted by: DougM Posted at: 2017-08-04T15:57:50.616Z Reads: 103

```
one end of the board has the extra length that comprises a mount-hole, so you can remove that end easily.  Would it fit then?

just make sure you don't breathe in the dust while you're cutting the board.  It's really bad.
```

---
## \#9 Posted by: banjaxxed Posted at: 2017-08-04T16:12:07.389Z Reads: 98

```
I'll watch out for the ould Silicosis for sure :slight_smile:

No idea but  I can only chop on one side, then insulate the chopped end to avoid a short, the case is aluminium so that would be a distinct possibility

Oh and I think @sl33py may also have some for anyone looking, found a post on ES
```

---
## \#10 Posted by: monkey32 Posted at: 2017-08-04T18:36:26.076Z Reads: 84

```
I was just thinking about this, legit gentlemen, thanks.
```

---
## \#11 Posted by: banjaxxed Posted at: 2017-09-16T10:28:22.234Z Reads: 70

```
So OshPark delivered me 3 superbly made PCBs,  room for 3 caps on the board, but like I said it would have to be cut down to 2 caps for teh VESC enclosure I have.

Here's the thing though on inspection of the Vanda VESCs, they seem to have one brutish cap hard wired in, 63v and 200Uf capacity, wondering if that is enough? Seems to be  X 100Uf caps in a FOCBOX, so maybe this is a pointless step I'm doing and should just through them into the enclosures and be done.

Voltage spike with a single 2200Uf 63V cap, that's not going to happen right?
```

---
## \#12 Posted by: Nordle Posted at: 2017-09-16T10:49:44.964Z Reads: 68

```
Traces in this pcb are so simple you can make your own with 2 copper pieces and some random piece of wood, plastic or whatever non conductive thing you can find
```

---
## \#13 Posted by: banjaxxed Posted at: 2017-09-16T10:54:27.967Z Reads: 67

```
thanks I hear you, I'm thinking though that 2200Uf is enough already is the real question
```

---
## \#14 Posted by: scepterr Posted at: 2017-09-25T00:18:46.263Z Reads: 59

```
It fits the standard 3x 680uf caps in the bom perfectly
```

---
## \#15 Posted by: Cobber Posted at: 2017-09-25T01:49:56.024Z Reads: 55

```
If you search the rc forums, the rule of thumb most are using one small cap (230/280? or something) per 10cm of battery-esc wire. Apparently smaller caps have some marginal gain over larger ones.
Some of the manufacturers are recommending this in their literature as well.

edit: I had a look at my YGE cap banks and they are 63v 330uf (x5) and 390uf (x9).
```

---
## \#16 Posted by: Nordle Posted at: 2017-09-25T06:16:50.202Z Reads: 50

```
Smaller ones most of the time have lower ESR, thats why they are preffered.
```

---
## \#17 Posted by: banjaxxed Posted at: 2017-09-25T23:25:16.474Z Reads: 40

```
Thanks I'm good so
```

---
## \#18 Posted by: scepterr Posted at: 2017-09-25T23:43:44.062Z Reads: 40

```
If you need more of those enclosures let me know, I got the remaining stock 😉
```

---
