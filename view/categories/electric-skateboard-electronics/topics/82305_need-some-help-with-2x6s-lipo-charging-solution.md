# Need some help with 2x6s lipo charging solution

### Replies: 11 Views: 281

## \#1 Posted by: Suppaswag Posted at: 2019-01-27T22:27:00.946Z Reads: 63

```
I just started using 2 turnigy 4000mAh 6s lipos for a single motor shortboard and they work fantastic but I wanted some help figuring out a cheap balance charging plug-and-forget system without a hobby balance charger. I was thinking of using 2 cheap amazon 6s BMS's and bypassing the over current but didn't know how if I needed to use a 50.4v charger and put the BMS's in series or a 25.2v charger with them in parallel. Thanks in advance

**[Bms's](https://www.amazon.com/Diymore-Protection-Li-ion-Lithium-Battery/dp/B0748DVZ4P/ref=pd_sbs_328_14?_encoding=UTF8&pd_rd_i=B0748DVZ4P&pd_rd_r=770be2ce-1d1f-11e9-9903-adb2453778b8&pd_rd_w=MHfo1&pd_rd_wg=UuFy7&pf_rd_p=7d5d9c3c-5e01-44ac-97fd-261afd40b865&pf_rd_r=7MNVBT5QT0NSK4H753G8&refRID=7MNVBT5QT0NSK4H753G8&th=1)**
**[50.4v charger](https://www.amazon.com/Battery-Charger-Skateboard-Electric-110-220V/dp/B076KJD4J5/ref=sr_1_1_sspa?ie=UTF8&qid=1546833515&sr=8-1-spons&keywords=50.4v+charger&psc=1)**
**[Possible 25.2v charger](https://www.amazon.com/Charger-Lithium-Li-ion-Battery-Tangspower/dp/B074SG8PX3/ref=sr_1_3?ie=UTF8&qid=1548449805&sr=8-3&keywords=25.2v+charger)**
```

---
## \#2 Posted by: Bor.inc Posted at: 2019-01-27T22:36:28.842Z Reads: 62

```
You can just hook up one bms to both the batteries and then use a 25.2v charger, otherwise you can also use one bms per battery and hook them up in parralel (so both the C+ and C-)  and you can then still use a 25.2v charger, I would not recommend hooking the 2 bms's in series up :slight_smile:

Hey and maybe you can ask this sort of questions in this thread first before making a whole thread by yourself :grin:
https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-01-27T22:48:31.986Z Reads: 50

```
Are you running the 6s packs in series or in parallel?

If series, then you need a 12s BMS and 50.4v charger, or a 12s balance charger.
If parallel, you can just use a single 6s BMS and a 25.2v charger, or a 6s balance charger.

If you're running parallel, just make up a wiring harness that combines both balance leads together so the BMS can balance both sets of cells.
```

---
## \#4 Posted by: Livid Posted at: 2019-01-27T22:56:47.235Z Reads: 45

```
I put 2 5s packs in my short board, use a 10s bms only connected to the balance lead (you will need to run a few wires to make this work), discharge through the main leads totally separate from the bms
```

---
## \#5 Posted by: Suppaswag Posted at: 2019-01-27T22:58:08.906Z Reads: 42

```
I'm running them in series to make 50.4v but I would like to avoid an expensive 12s BMS because I'm just using the balance charging and very simple protection. I would like to use 2 inexpensive 6s BMS's and was wondering how to connect the charing leads of them.
```

---
## \#6 Posted by: Suppaswag Posted at: 2019-01-27T23:00:15.015Z Reads: 39

```
Ive used a 10s 18650 pack on the same board but it didn't really have the performance i was looking for so i switched to 12s.
```

---
## \#7 Posted by: Livid Posted at: 2019-01-27T23:16:16.574Z Reads: 37

```
chinese bms's are super cheap, bms's usually dont like being run in series
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-01-27T23:21:52.325Z Reads: 32

```
I don't recommend trying to run multiple BMS' in series. They're not designed for that, and may fail or freak out. A 12s BMS doesn't cost much more than a pair of decent 6s ones will, and I don't think it's something worth pursuing to save $10 or so. It's a bad idea to pinch pennies on something that's designed to keep your board from catching on fire.
```

---
## \#9 Posted by: Suppaswag Posted at: 2019-01-27T23:23:28.895Z Reads: 32

```
Any recommendations for a good bms?
```

---
## \#10 Posted by: Livid Posted at: 2019-01-27T23:28:22.108Z Reads: 29

```
tbh i just grabbed the cheapest one  on banggood.com, if you are just charging through it it'l probably be fine, but i wouldn't trust discharging through it
```

---
## \#11 Posted by: MysticalDork Posted at: 2019-01-28T02:17:09.054Z Reads: 22

```
For charge-only, I'd recommend a Bestech D140. They're about $30. I've had a couple of the really cheap banggood ones fail and drain one of the cells down to ~1.5 volts before.
```

---
