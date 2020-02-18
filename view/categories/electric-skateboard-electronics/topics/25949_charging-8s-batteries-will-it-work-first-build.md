# Charging 8s batteries?// Will it work? // First Build

### Replies: 6 Views: 479

## \#1 Posted by: Peetaa Posted at: 2017-06-22T21:05:55.525Z Reads: 70

```
Hello

I'm in the process of building my first board. I've been reading a lot on this forum and I think I've decided on a soloution but I'm not sure it will work. Can some of you check it out?

I first thought I was going to use a BMS but because it's my first build I want to keep it simple and keep the cost down
I plan on using a VESC aswell. Hopefully the FOCBOX from enertion.

<img src="/uploads/db1493/original/3X/8/a/8aa2c8e1ba03a74289ff63bebbff7f123087ddcf.jpg" width="375" height="500">

Greetings from Sweden

Thank you
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-06-23T00:27:13.860Z Reads: 54

```
I believe you will also need to also break the series connection between the two batteries.
```

---
## \#3 Posted by: gee Posted at: 2017-06-23T01:46:07.990Z Reads: 44

```
like i2oadsweepei2 said. You can't charge them in SERIES unless you have the BMS. You CAN charge them in parallel but you need the parallel board to charge it. There's a tutorial on youtube somewhere.
```

---
## \#4 Posted by: Peetaa Posted at: 2017-06-23T11:01:03.838Z Reads: 43

```
I see!

Would this be a better soloution? Will this work?
I plan on removing the part between the batteries when charging. 

<img src="/uploads/db1493/original/3X/b/6/b66bf4b14d3cc3f990513b983a70dbe33fcbe844.jpg" width="666" height="500">
```

---
## \#5 Posted by: Challlsss Posted at: 2017-06-23T15:06:49.565Z Reads: 32

```
- You do need to break the series connection...  however this can easily be done by turning off your board. You decide to do the power switch and you won't need to break the circuit twice.

- You can do series charging with a Lipo Balance charger. As long as you know what you are doing it's very simple *but*....

- Most series lipo chargers only go up to 6S (or they're stupid expensive) So you'll have to charge each cell individually unless you parallel charge (I don't recommend this) When you connect 2 batteries in parallel they become 1 big battery and the difference in voltage will balance out. This happens through rush of current through the batteries. You would have to have a way to disconnect the parallel connection after charging each time and whenever you reconnect it you would be putting strain on the batteries.

- **best option:** Get a BMS and bypass it for discharging (or spend the extra money for higher current). If you "bypass" the BMS you are just putting in parallel to the VESC, rather than series. (once again you'll need a power switch if you decide to bypass BMS) Once you've done that you can get a basic wall charger to plug directly into the board. You wont need a balance charger. This will make your build look nicer and charging will be more simple.
```

---
## \#6 Posted by: Peetaa Posted at: 2017-06-23T15:10:12.007Z Reads: 28

```
That's properly how I'll do it then!
Thanks for the advice!
```

---
