# BMS potential problem down the road?

### Replies: 8 Views: 247

## \#1 Posted by: SkyTheEpic Posted at: 2018-12-21T21:15:42.680Z Reads: 66

```
Is it normal for the BMS to produce a lot of heat when the battery is almost fully charged even when the board is powered down? My board works fine it charges and i can ride it without an issue. I'm just concerned the heat might affect lifespan and if it will cause future problems. I can feel the heat through the enclosure i'm not sure if that's ok. It just seems to happen close to full charge. 
I've been following this diagram:
![oeNLTjn|690x398](upload://5a8zS1YPNuL44BtnnYvY15f52tY.jpeg) 
Here are some pics, in case i messed up :slight_smile: 
![P_20181221_203743|690x388](upload://wnf2cJi6Dbln6FvMVgyB2jVT6G9.jpeg) ![P_20181221_203925|690x388](upload://j29XAInzKpIlJs06BuRTBighRoc.jpeg) ![P_20181221_204054|690x388](upload://4pWWajlSghMaP8KYZc8Uv9UxIv5.jpeg)
```

---
## \#2 Posted by: rojitor Posted at: 2018-12-21T22:48:19.639Z Reads: 54

```
If the cells are really out of balance it's normal to notice a rise of temperature on the bms. How hot is It? You should notice It warm the first few uses but not everytime. If the battery is well built/legit cells... The heat should not be noticeable after a couple cycles. If the battery is new leave the charger plugged for a few hours when is fully charged.
If the heat persists then you have a problem if not it's ok.
```

---
## \#3 Posted by: thisguyhere Posted at: 2018-12-21T22:55:08.923Z Reads: 50

```
this is why i don't like attaching the bms to the battery itself.

bms basically overcharges to like 4.25v, then drains each p group down to 4.2v through resistors, and they get hot.

this process repeats until all cells in the pack reach balance (4.2v)
```

---
## \#4 Posted by: rojitor Posted at: 2018-12-21T23:00:58.633Z Reads: 46

```
![IMG_20181221_2357012393449786062906310|375x500](upload://meSweZWSRrlH4BnN2VVhilRFGy8.jpeg) 


This is my laser thermometer. I use It for my first cycle. I check temperatures on cells and bms so i know everything is according to the plan. Btw never leave charging unattended. Mostly first few charges.
```

---
## \#5 Posted by: SkyTheEpic Posted at: 2018-12-21T23:01:34.672Z Reads: 47

```
Its a pretty new battery i completed the build only yesterday, i will hook everything up again and give it a shot. 
Thanks
```

---
## \#6 Posted by: Fiori Posted at: 2018-12-21T23:12:52.435Z Reads: 44

```
Overcharges what to 4.25? The first group you mean?

I know my bluetooth BMS starts balancing when the pack reaches 4.00V.  I'm sure every non adjustable BMS acts slightly different.
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-12-21T23:34:30.836Z Reads: 41

```
i really need to try one of these smart bms...bestech is apparently working on one.

but...yea, the normal run of the mill bms overcharges then balances through slow bleed via resistors.  at least that's how it's been described to me by bestech themselves.
```

---
## \#8 Posted by: pat.speed Posted at: 2018-12-21T23:37:43.655Z Reads: 37

```
That’s not quite right. Close tho. The bms charges the cells until 4.2v when they hit the balance voltage (usually 4.2v) the bleed resistors kick in. The problem is these only draw less than 100ma in most cases so they can’t always compete with the input current of the charger. Thus sometimes a cell group is overcharged but not every time just occasionally if the pack can’t be balanced fast enough
```

---
