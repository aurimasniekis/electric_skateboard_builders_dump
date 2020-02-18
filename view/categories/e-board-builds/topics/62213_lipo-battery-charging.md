# LiPo battery charging

### Replies: 6 Views: 391

## \#1 Posted by: MrDGOrman Posted at: 2018-07-18T17:29:25.158Z Reads: 96

```
Hi everyone,

First time doing this so I want to make sure I get it right. I've got a Keenstone C1-XR charger and want to charge my 3 batteries using a parallel charging board. Each battery is 5000mah 3 cell 11.1v (zippy flightmax 20c). What settings do I use on the charger to charge the batteries? Do I pick 5000mah or 15000mah (5000x3)?

Any help is really appreciated!
```

---
## \#2 Posted by: deucesdown Posted at: 2018-07-18T17:55:18.381Z Reads: 91

```
Very important, make sure batteries are not connected in series. The packs also need to be at a very similar state-of-charge (they'll balance charge each other through the balance leads at full power as soon as you connect them through the parallel board).

Parallel will be a sum of amp hours, so 5000mah x 3 in parallel is 15000mah.

If charging at 1C, on some chargers, you'll specify 15000ma.

Some chargers will allow you to choose something like 5000ma, 3 in parallel.
```

---
## \#3 Posted by: MrDGOrman Posted at: 2018-07-18T20:55:08.441Z Reads: 81

```
@deucesdown thank you. The batteries are individual packs. 3 cells in each pack. And then I've got 3 of them.

My main concern was the mah setting. I'll put in 15000mah. They're also brand new batteries all with the same level of charge in them.

Thanks for the help. I really appreciate it.
Daniel
```

---
## \#4 Posted by: wafflejock Posted at: 2018-07-18T21:00:08.059Z Reads: 68

```
Advice given is good one other thing to note since the charger is limited to 10A and 100W you'll be limited to about 7.5A (whatever 100W/(4.2x3) equals will need to be a little under that typically) on the charger side before it will likely do thermal shutdown also likely they limited it to 10A max charge rate in the software.  Less than 1C is generally safer for the batteries anyhow.

At 1C they would be charged in about an hour plus maybe 10-15 minutes balancing lower rate means longer time.

---

Fixed estimated max amps for charging based on charger wattage.
```

---
## \#5 Posted by: deucesdown Posted at: 2018-07-18T21:09:51.765Z Reads: 60

```
Nice guy, you actually ran down the charger specs? :slight_smile:

10A max, 100w max, the lowest will be the limiting factor. at 3s assuming 3.6v min, 100w / (3.6v * 3) = 9.2A. This is the fastest your charger will charge 3s packs, and this will only happen when the pack is mostly empty. It'll slow to 7.5A as the pack gets closer to full.

Your 1C rate for 3 packs in parallel is 15A (aka 15000ma). You cannot achieve this.

Aaaand one last safety tip. If using parallel charging, stay in the room and watch the pack. There are many failure modes with parallel charging, even with per-balance wire fuses on the parallel board and top shelf high quality packs. And most of them are scary.
```

---
## \#6 Posted by: MrDGOrman Posted at: 2018-07-20T10:12:52.670Z Reads: 42

```
@wafflejock @deucesdown

Thank you both for the help. I'll be charging the batteries during the day  in my office so I'll be with it all the time. I'll also have the batteries in a lipo charging bag just incase. I have an old ammunition case from my shooting days that I can use as a secondary deterrent if I need to.

Much love to you both <3
```

---
