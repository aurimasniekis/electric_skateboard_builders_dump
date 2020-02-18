# B6AC V2 charging limit

### Replies: 19 Views: 279

## \#1 Posted by: malJohann Posted at: 2018-10-20T00:11:43.835Z Reads: 73

```
To limit my B6AC to charge only 75% capacity of my 6,000mAh LiPo battery, can I simply set it to charge up to 4,500mAh?
```

---
## \#2 Posted by: pat.speed Posted at: 2018-10-20T03:50:52.825Z Reads: 66

```
Erm I don’t think you can set a capacity limit, although I’m not entirely sure. I think you might just have to stop it when it gets to about 4v per cell
```

---
## \#3 Posted by: malJohann Posted at: 2018-10-20T04:04:34.290Z Reads: 58

```
On the B6AC you choose the cell count and capacity, it then delivers the correct voltage and current over a predetermined time. I was just wondering if this was appropriate use of technology.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-10-20T04:40:37.668Z Reads: 53

```
Well I assume so, I can’t be sure as my b6 didn’t have the choice of capacity
```

---
## \#5 Posted by: Andy87 Posted at: 2018-10-20T05:51:56.825Z Reads: 44

```
I have only the b6. I can’t choose the capacity only balance charge or normal/fast charge.
The problem is that I run into time limit.
After 2h the charger stop charging, which is usually about 4.4ah, which means I need to start a new charge cycles to get the full 5ah of my packs.
How it works on your, I mean if you discharge your packs you never know how much you really discharge. What if you set 6ah but there was still 500mah left in the pack. It will overcharge the pack?
```

---
## \#6 Posted by: malJohann Posted at: 2018-10-20T05:54:56.552Z Reads: 39

```
Still monitors it somehow, the capacity setting is only the upper limit. If I set it to 4,500mAh and there were still 500mAh in the pack, it’ll take it to 4,500mAh or there about. I’ve charged partially drained packs and they stop early.

My guess is it monitors the voltage, which would be ideal, because then I could set a voltage cutoff to get to n% of the pack capacity.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-20T05:59:11.267Z Reads: 31

```
You don’t have the option to just balance charge on the b6ac?
```

---
## \#8 Posted by: malJohann Posted at: 2018-10-20T06:01:04.254Z Reads: 35

```
I do, and alternate between two charge cycles to one balance cycle. Why?
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-20T06:04:30.228Z Reads: 36

```
Just was interested in case i will buy the ac version too one day. 
So in fact you can charge your packs to 100% just not with the capacity mode right?
```

---
## \#10 Posted by: malJohann Posted at: 2018-10-20T06:07:10.058Z Reads: 36

```
You still set the capacity and cell count, and yes I can charge to 100%, but read that doing that will shorten their lifespan, and I should really only be charging to 75%. Hence the reason for this thread.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-10-20T06:22:02.837Z Reads: 31

```
Ah damn it 🙈to early in the morning.
I read you can’t charge over 75%....
The thing is that mine only start balancing when one cell reached 4.2v.
Would be interesting if your charger balance to the capacity you set it to charge.
I stick to this thread. Hope somebody can answer your question.
```

---
## \#12 Posted by: murloc992 Posted at: 2018-10-20T08:43:22.289Z Reads: 27

```
You could always flash [Chea-Li Charger](https://github.com/stawel/cheali-charger) Firmware to the iMax B6AC and get a lot of settings into it. You might need to calibrate and configure it a lot though.. **Make sure to backup the flash and the EEPROM before flashing the new firmware.**
```

---
## \#13 Posted by: Okami Posted at: 2018-10-20T10:39:00.053Z Reads: 26

```
@murloc992 thats some good stuff. Have u tried the custom firmware and how did u find about it anyways? 

I think u just showed a 2nd chance for my 8s charger which is busted and shows Input Voltage  too low, even if i attach 19v power supply
```

---
## \#14 Posted by: murloc992 Posted at: 2018-10-20T12:12:29.632Z Reads: 25

```
I have it on my charger and it's very nice. Just the calibration is kind of fiddly and requires some time and very accurate multimeter. :slight_smile:
```

---
## \#15 Posted by: malJohann Posted at: 2018-10-20T20:56:57.693Z Reads: 22

```
Thanks, but if I can wing it, or the standard capabilities of the charger can work, I’m not modifying anything.
```

---
## \#16 Posted by: malJohann Posted at: 2018-10-23T12:34:17.834Z Reads: 21

```
Should I be concerned? This was after charging partially drained batteries. How would I tell whether I was losing capacity?

![image|666x500](upload://96GIAAA56INiX8bUGIVV6nJIr1a.jpeg)
```

---
## \#17 Posted by: malJohann Posted at: 2019-01-09T21:34:11.995Z Reads: 20

```
So I forgot to put my LiPos on a storage charge before going on holiday, and now they only charge 1500mAh or thereabouts. Is there a way to repair/restore LiPos? Any help appreciated.
```

---
## \#18 Posted by: Andy87 Posted at: 2019-01-10T07:21:40.768Z Reads: 18

```
up to which voltage you can charge them?
```

---
## \#19 Posted by: malJohann Posted at: 2019-01-28T09:17:20.702Z Reads: 12

```
Did a bit of research on restoring LiPos, and found this advice.

[quote="KyleB198"]With due respect, you are wrong and this is a dangerous thing you're recommending.

The problem with an over-discharged LiPo cell is not because the internal resistance rises... it's because once the battery is completely depleted, the lithium metal starts to plate out on the anode. This causes dendrite structures to form, which can puncture the separator, causing an internal short-circuit. 

Even if you successfully give a 'dead' LiPo a charge, that dendrite remains. You don't remove the hazard.

A battery with a proper embedded protection circuit will have lock-out for voltages under 2.5V, in other words, it won't take a charge no matter WHAT you do to the battery (except maybe dismantle it). In the hobby world, these circuits generally aren't provided because they add weight & cost. 

There's a reason a properly designed battery charger will refuse to charge an over-discharged cell. It's not just because they wanna sell you more batteries.[/quote]

Based on that I bought 4x new Graphene 4S 5,000mAh batteries at 35% discount (combination sale and voucher) today.

So wired up it’s 8S 10,000mAh instead of the 6,000mAh I had before at only $40 more than the original cost.
```

---
