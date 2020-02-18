# What BMS to choose for a 2700W motor running on 6S5P 18650

### Replies: 7 Views: 496

## \#1 Posted by: pcapelo Posted at: 2017-06-02T19:06:22.667Z Reads: 64

```
I am thinking about building a battery pack 6S5P and since I don't have a lot of experience I would like to ask the group how big of a BMS should I consider buying. I am using the Sk3 6364 245kv.

What would be the correct discharge rate, in A?

Thanks in advance
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-02T19:07:57.561Z Reads: 64

```
60A+ should be good, 80 if you want to be safe. Though I personally bypass BMS so I can save space in my enclosure with a smaller BMS.
```

---
## \#3 Posted by: pcapelo Posted at: 2017-06-02T19:19:09.936Z Reads: 61

```
what do you mean about bypassing the BMS, do you mean to use a BMS for charging only and connect the ESC directly to the battery?
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-02T19:23:40.131Z Reads: 58

```
yep you got it. That's what I do for both my boards.
```

---
## \#5 Posted by: Achmed20 Posted at: 2017-06-02T21:05:56.474Z Reads: 45

```
same here, saves alot of money and time.

unless you start mixing old with new batteries, it schouldnt be a problem anyway.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-02T22:11:01.121Z Reads: 41

```
You should know however that when you bypass the bms during discharge cycle that your batteries will not have the same protection that they will if you do not bypass.
While the Vesc can monitor total pack voltage and shut down if it gets too low, It does not monitor cells or cell groups individually.
When you discharge through the bms, it monitors each cell or cell group's voltage and if any cell or group drops to the detection voltage the bms shuts down. It will also protect your battery against shorts and over current.
So the optimum setup is to charge and discharge through the bms.
```

---
## \#7 Posted by: pcapelo Posted at: 2017-06-02T23:50:25.924Z Reads: 37

```
It makes sense, thanks :)
```

---
